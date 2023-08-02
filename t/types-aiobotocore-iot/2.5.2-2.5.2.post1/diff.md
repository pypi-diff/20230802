# Comparing `tmp/types-aiobotocore-iot-2.5.2.tar.gz` & `tmp/types-aiobotocore-iot-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iot-2.5.2.tar", last modified: Sat Jul  8 01:43:45 2023, max compression
+gzip compressed data, was "types-aiobotocore-iot-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:26 2023, max compression
```

## Comparing `types-aiobotocore-iot-2.5.2.tar` & `types-aiobotocore-iot-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:45.966289 types-aiobotocore-iot-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:32:23.000000 types-aiobotocore-iot-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    55298 2023-07-08 01:43:45.958289 types-aiobotocore-iot-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    53749 2023-07-08 01:32:23.000000 types-aiobotocore-iot-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:45.966289 types-aiobotocore-iot-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-08 01:32:23.000000 types-aiobotocore-iot-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:45.958289 types-aiobotocore-iot-2.5.2/types_aiobotocore_iot/
--rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-07-08 01:32:23.000000 types-aiobotocore-iot-2.5.2/types_aiobotocore_iot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14184 2023-07-08 01:32:23.000000 types-aiobotocore-iot-2.5.2/types_aiobotocore_iot/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-08 01:32:23.000000 types-aiobotocore-iot-2.5.2/types_aiobotocore_iot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   190083 2023-07-08 01:32:24.000000 types-aiobotocore-iot-2.5.2/types_aiobotocore_iot/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   189765 2023-07-08 01:32:24.000000 types-aiobotocore-iot-2.5.2/types_aiobotocore_iot/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    24962 2023-07-08 01:32:26.000000 types-aiobotocore-iot-2.5.2/types_aiobotocore_iot/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    24960 2023-07-08 01:32:26.000000 types-aiobotocore-iot-2.5.2/types_aiobotocore_iot/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    71939 2023-07-08 01:32:26.000000 types-aiobotocore-iot-2.5.2/types_aiobotocore_iot/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    71878 2023-07-08 01:32:26.000000 types-aiobotocore-iot-2.5.2/types_aiobotocore_iot/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:32:23.000000 types-aiobotocore-iot-2.5.2/types_aiobotocore_iot/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   257109 2023-07-08 01:32:32.000000 types-aiobotocore-iot-2.5.2/types_aiobotocore_iot/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   256782 2023-07-08 01:32:29.000000 types-aiobotocore-iot-2.5.2/types_aiobotocore_iot/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:32:23.000000 types-aiobotocore-iot-2.5.2/types_aiobotocore_iot/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:45.958289 types-aiobotocore-iot-2.5.2/types_aiobotocore_iot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    55298 2023-07-08 01:43:45.000000 types-aiobotocore-iot-2.5.2/types_aiobotocore_iot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-08 01:43:45.000000 types-aiobotocore-iot-2.5.2/types_aiobotocore_iot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:45.000000 types-aiobotocore-iot-2.5.2/types_aiobotocore_iot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:45.000000 types-aiobotocore-iot-2.5.2/types_aiobotocore_iot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:45.000000 types-aiobotocore-iot-2.5.2/types_aiobotocore_iot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:43:45.000000 types-aiobotocore-iot-2.5.2/types_aiobotocore_iot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.305564 types-aiobotocore-iot-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:24.000000 types-aiobotocore-iot-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    57024 2023-08-02 14:52:26.297564 types-aiobotocore-iot-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    55522 2023-08-02 14:40:24.000000 types-aiobotocore-iot-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:26.305564 types-aiobotocore-iot-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:40:24.000000 types-aiobotocore-iot-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.297564 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/
+-rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-08-02 14:40:24.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14184 2023-08-02 14:40:24.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:40:24.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   190224 2023-08-02 14:40:26.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   189906 2023-08-02 14:40:25.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    24962 2023-08-02 14:40:28.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24960 2023-08-02 14:40:28.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    71670 2023-08-02 14:40:28.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71609 2023-08-02 14:40:27.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:24.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   272446 2023-08-02 14:40:35.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   272098 2023-08-02 14:40:31.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:24.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.297564 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    57024 2023-08-02 14:52:26.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:52:26.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:26.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:26.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:26.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:26.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iot-2.5.2/LICENSE` & `types-aiobotocore-iot-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-2.5.2/PKG-INFO` & `types-aiobotocore-iot-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,62 +1,29 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-iot
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IoT 2.5.2 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iot type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iot"></a>
 
 # types-aiobotocore-iot
 
 [![PyPI - types-aiobotocore-iot](https://img.shields.io/pypi/v/types-aiobotocore-iot.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iot?color=blue)](https://pypistats.org/packages/types-aiobotocore-iot)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot)](https://pepy.tech/project/types-aiobotocore-iot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoT 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
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
 [types-aiobotocore-iot docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +41,15 @@
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
@@ -643,137 +610,120 @@
 )
 
 
 def check_value(value: AbortActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iot.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iot.type_defs import (
     AbortCriteriaTypeDef,
     AcceptCertificateTransferRequestRequestTypeDef,
     CloudwatchAlarmActionTypeDef,
     CloudwatchLogsActionTypeDef,
     CloudwatchMetricActionTypeDef,
     DynamoDBActionTypeDef,
     ElasticsearchActionTypeDef,
     FirehoseActionTypeDef,
     IotAnalyticsActionTypeDef,
     IotEventsActionTypeDef,
-    KafkaActionTypeDef,
+    KafkaActionOutputTypeDef,
     KinesisActionTypeDef,
     LambdaActionTypeDef,
     OpenSearchActionTypeDef,
     S3ActionTypeDef,
     SalesforceActionTypeDef,
     SnsActionTypeDef,
     SqsActionTypeDef,
     StepFunctionsActionTypeDef,
-    MetricValueTypeDef,
+    KafkaActionTypeDef,
+    MetricValueOutputTypeDef,
     ViolationEventAdditionalInfoTypeDef,
     AddThingToBillingGroupRequestRequestTypeDef,
     AddThingToThingGroupRequestRequestTypeDef,
+    AddThingsToThingGroupParamsOutputTypeDef,
     AddThingsToThingGroupParamsTypeDef,
+    AggregationTypeOutputTypeDef,
     AggregationTypeTypeDef,
     AlertTargetTypeDef,
     PolicyTypeDef,
     AssetPropertyTimestampTypeDef,
     AssetPropertyVariantTypeDef,
     AssociateTargetsWithJobRequestRequestTypeDef,
-    AssociateTargetsWithJobResponseTypeDef,
+    ResponseMetadataTypeDef,
     AttachPolicyRequestRequestTypeDef,
     AttachPrincipalPolicyRequestRequestTypeDef,
     AttachSecurityProfileRequestRequestTypeDef,
     AttachThingPrincipalRequestRequestTypeDef,
+    AttributePayloadOutputTypeDef,
     AttributePayloadTypeDef,
     AuditCheckConfigurationTypeDef,
     AuditCheckDetailsTypeDef,
     AuditMitigationActionExecutionMetadataTypeDef,
     AuditMitigationActionsTaskMetadataTypeDef,
+    AuditMitigationActionsTaskTargetOutputTypeDef,
     AuditMitigationActionsTaskTargetTypeDef,
     AuditNotificationTargetTypeDef,
     AuditTaskMetadataTypeDef,
+    AuthInfoOutputTypeDef,
     AuthInfoTypeDef,
     AuthorizerConfigTypeDef,
     AuthorizerDescriptionTypeDef,
     AuthorizerSummaryTypeDef,
     AwsJobAbortCriteriaTypeDef,
     AwsJobRateIncreaseCriteriaTypeDef,
     AwsJobPresignedUrlConfigTypeDef,
     AwsJobTimeoutConfigTypeDef,
     MachineLearningDetectionConfigTypeDef,
     StatisticalThresholdTypeDef,
+    MetricValueTypeDef,
     BehaviorModelTrainingSummaryTypeDef,
     MetricDimensionTypeDef,
     BillingGroupMetadataTypeDef,
     BillingGroupPropertiesTypeDef,
+    BlobTypeDef,
     BucketTypeDef,
     TermsAggregationTypeDef,
     CertificateValidityTypeDef,
     CACertificateTypeDef,
     CancelAuditMitigationActionsTaskRequestRequestTypeDef,
     CancelAuditTaskRequestRequestTypeDef,
     CancelCertificateTransferRequestRequestTypeDef,
     CancelDetectMitigationActionsTaskRequestRequestTypeDef,
     CancelJobExecutionRequestRequestTypeDef,
     CancelJobRequestRequestTypeDef,
-    CancelJobResponseTypeDef,
     TransferDataTypeDef,
     CertificateTypeDef,
     CodeSigningCertificateChainTypeDef,
-    CodeSigningSignatureTypeDef,
+    CodeSigningSignatureOutputTypeDef,
     ConfigurationTypeDef,
     ConfirmTopicRuleDestinationRequestRequestTypeDef,
+    TimestampTypeDef,
     TagTypeDef,
-    CreateAuthorizerResponseTypeDef,
-    CreateBillingGroupResponseTypeDef,
     CreateCertificateFromCsrRequestRequestTypeDef,
-    CreateCertificateFromCsrResponseTypeDef,
-    CreateCustomMetricResponseTypeDef,
-    CreateDimensionResponseTypeDef,
     TlsConfigTypeDef,
-    CreateDomainConfigurationResponseTypeDef,
-    CreateDynamicThingGroupResponseTypeDef,
-    CreateFleetMetricResponseTypeDef,
     PresignedUrlConfigTypeDef,
     TimeoutConfigTypeDef,
-    CreateJobResponseTypeDef,
     MaintenanceWindowTypeDef,
-    CreateJobTemplateResponseTypeDef,
     CreateKeysAndCertificateRequestRequestTypeDef,
     KeyPairTypeDef,
-    CreateMitigationActionResponseTypeDef,
-    CreateOTAUpdateResponseTypeDef,
     CreatePackageRequestRequestTypeDef,
-    CreatePackageResponseTypeDef,
     CreatePackageVersionRequestRequestTypeDef,
-    CreatePackageVersionResponseTypeDef,
-    CreatePolicyResponseTypeDef,
     CreatePolicyVersionRequestRequestTypeDef,
-    CreatePolicyVersionResponseTypeDef,
     CreateProvisioningClaimRequestRequestTypeDef,
     ProvisioningHookTypeDef,
-    CreateProvisioningTemplateResponseTypeDef,
     CreateProvisioningTemplateVersionRequestRequestTypeDef,
-    CreateProvisioningTemplateVersionResponseTypeDef,
-    CreateRoleAliasResponseTypeDef,
-    CreateScheduledAuditResponseTypeDef,
-    CreateSecurityProfileResponseTypeDef,
-    CreateStreamResponseTypeDef,
-    CreateThingGroupResponseTypeDef,
-    CreateThingResponseTypeDef,
     ThingTypePropertiesTypeDef,
-    CreateThingTypeResponseTypeDef,
     DeleteAccountAuditConfigurationRequestRequestTypeDef,
     DeleteAuthorizerRequestRequestTypeDef,
     DeleteBillingGroupRequestRequestTypeDef,
     DeleteCACertificateRequestRequestTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     DeleteCustomMetricRequestRequestTypeDef,
     DeleteDimensionRequestRequestTypeDef,
@@ -809,374 +759,355 @@
     TaskStatisticsTypeDef,
     DescribeAuthorizerRequestRequestTypeDef,
     DescribeBillingGroupRequestRequestTypeDef,
     DescribeCACertificateRequestRequestTypeDef,
     RegistrationConfigTypeDef,
     DescribeCertificateRequestRequestTypeDef,
     DescribeCustomMetricRequestRequestTypeDef,
-    DescribeCustomMetricResponseTypeDef,
     DescribeDetectMitigationActionsTaskRequestRequestTypeDef,
     DescribeDimensionRequestRequestTypeDef,
-    DescribeDimensionResponseTypeDef,
     DescribeDomainConfigurationRequestRequestTypeDef,
     ServerCertificateSummaryTypeDef,
     DescribeEndpointRequestRequestTypeDef,
-    DescribeEndpointResponseTypeDef,
     DescribeFleetMetricRequestRequestTypeDef,
     DescribeIndexRequestRequestTypeDef,
-    DescribeIndexResponseTypeDef,
     DescribeJobExecutionRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeJobTemplateRequestRequestTypeDef,
     DescribeManagedJobTemplateRequestRequestTypeDef,
     DocumentParameterTypeDef,
     DescribeMitigationActionRequestRequestTypeDef,
     DescribeProvisioningTemplateRequestRequestTypeDef,
     DescribeProvisioningTemplateVersionRequestRequestTypeDef,
-    DescribeProvisioningTemplateVersionResponseTypeDef,
     DescribeRoleAliasRequestRequestTypeDef,
     RoleAliasDescriptionTypeDef,
     DescribeScheduledAuditRequestRequestTypeDef,
-    DescribeScheduledAuditResponseTypeDef,
     DescribeSecurityProfileRequestRequestTypeDef,
     DescribeStreamRequestRequestTypeDef,
     DescribeThingGroupRequestRequestTypeDef,
     DescribeThingRegistrationTaskRequestRequestTypeDef,
-    DescribeThingRegistrationTaskResponseTypeDef,
     DescribeThingRequestRequestTypeDef,
-    DescribeThingResponseTypeDef,
     DescribeThingTypeRequestRequestTypeDef,
     ThingTypeMetadataTypeDef,
+    ThingTypePropertiesOutputTypeDef,
     S3DestinationTypeDef,
     DetachPolicyRequestRequestTypeDef,
     DetachPrincipalPolicyRequestRequestTypeDef,
     DetachSecurityProfileRequestRequestTypeDef,
     DetachThingPrincipalRequestRequestTypeDef,
     DetectMitigationActionExecutionTypeDef,
     DetectMitigationActionsTaskStatisticsTypeDef,
+    DetectMitigationActionsTaskTargetOutputTypeDef,
+    ViolationEventOccurrenceRangeOutputTypeDef,
     DetectMitigationActionsTaskTargetTypeDef,
-    ViolationEventOccurrenceRangeTypeDef,
     DisableTopicRuleRequestRequestTypeDef,
     DomainConfigurationSummaryTypeDef,
     PutItemInputTypeDef,
     EffectivePolicyTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableIoTLoggingParamsTypeDef,
     EnableTopicRuleRequestRequestTypeDef,
     ErrorInfoTypeDef,
     RateIncreaseCriteriaTypeDef,
     FieldTypeDef,
     S3LocationTypeDef,
     StreamTypeDef,
     FleetMetricNameAndArnTypeDef,
-    GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetBehaviorModelTrainingSummariesRequestRequestTypeDef,
     GetCardinalityRequestRequestTypeDef,
-    GetCardinalityResponseTypeDef,
     GetEffectivePoliciesRequestRequestTypeDef,
     GetJobDocumentRequestRequestTypeDef,
-    GetJobDocumentResponseTypeDef,
-    GetLoggingOptionsResponseTypeDef,
     GetOTAUpdateRequestRequestTypeDef,
     VersionUpdateByJobsConfigTypeDef,
     GetPackageRequestRequestTypeDef,
-    GetPackageResponseTypeDef,
     GetPackageVersionRequestRequestTypeDef,
-    GetPackageVersionResponseTypeDef,
     GetPercentilesRequestRequestTypeDef,
     PercentPairTypeDef,
     GetPolicyRequestRequestTypeDef,
-    GetPolicyResponseTypeDef,
     GetPolicyVersionRequestRequestTypeDef,
-    GetPolicyVersionResponseTypeDef,
-    GetRegistrationCodeResponseTypeDef,
     GetStatisticsRequestRequestTypeDef,
     StatisticsTypeDef,
     GetTopicRuleDestinationRequestRequestTypeDef,
     GetTopicRuleRequestRequestTypeDef,
-    GetV2LoggingOptionsResponseTypeDef,
     GroupNameAndArnTypeDef,
     HttpActionHeaderTypeDef,
     SigV4AuthorizationTypeDef,
     HttpContextTypeDef,
     HttpUrlDestinationConfigurationTypeDef,
     HttpUrlDestinationPropertiesTypeDef,
     HttpUrlDestinationSummaryTypeDef,
+    IndexingFilterOutputTypeDef,
     IndexingFilterTypeDef,
     IssuerCertificateIdentifierTypeDef,
     JobExecutionStatusDetailsTypeDef,
     JobExecutionSummaryTypeDef,
     RetryCriteriaTypeDef,
     JobProcessDetailsTypeDef,
     JobSummaryTypeDef,
     JobTemplateSummaryTypeDef,
     ScheduledJobRolloutTypeDef,
-    ListActiveViolationsRequestListActiveViolationsPaginateTypeDef,
     ListActiveViolationsRequestRequestTypeDef,
-    ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef,
     ListAttachedPoliciesRequestRequestTypeDef,
-    ListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef,
     ListAuditMitigationActionsExecutionsRequestRequestTypeDef,
-    ListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef,
-    ListAuditMitigationActionsTasksRequestRequestTypeDef,
-    ListAuditTasksRequestListAuditTasksPaginateTypeDef,
-    ListAuditTasksRequestRequestTypeDef,
-    ListAuthorizersRequestListAuthorizersPaginateTypeDef,
     ListAuthorizersRequestRequestTypeDef,
-    ListBillingGroupsRequestListBillingGroupsPaginateTypeDef,
     ListBillingGroupsRequestRequestTypeDef,
-    ListCACertificatesRequestListCACertificatesPaginateTypeDef,
     ListCACertificatesRequestRequestTypeDef,
-    ListCertificatesByCARequestListCertificatesByCAPaginateTypeDef,
     ListCertificatesByCARequestRequestTypeDef,
-    ListCertificatesRequestListCertificatesPaginateTypeDef,
     ListCertificatesRequestRequestTypeDef,
-    ListCustomMetricsRequestListCustomMetricsPaginateTypeDef,
     ListCustomMetricsRequestRequestTypeDef,
-    ListCustomMetricsResponseTypeDef,
-    ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef,
-    ListDetectMitigationActionsExecutionsRequestRequestTypeDef,
-    ListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef,
-    ListDetectMitigationActionsTasksRequestRequestTypeDef,
-    ListDimensionsRequestListDimensionsPaginateTypeDef,
     ListDimensionsRequestRequestTypeDef,
-    ListDimensionsResponseTypeDef,
-    ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef,
     ListDomainConfigurationsRequestRequestTypeDef,
-    ListFleetMetricsRequestListFleetMetricsPaginateTypeDef,
     ListFleetMetricsRequestRequestTypeDef,
-    ListIndicesRequestListIndicesPaginateTypeDef,
     ListIndicesRequestRequestTypeDef,
-    ListIndicesResponseTypeDef,
-    ListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef,
     ListJobExecutionsForJobRequestRequestTypeDef,
-    ListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef,
     ListJobExecutionsForThingRequestRequestTypeDef,
-    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
-    ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef,
     ListManagedJobTemplatesRequestRequestTypeDef,
     ManagedJobTemplateSummaryTypeDef,
-    ListMetricValuesRequestListMetricValuesPaginateTypeDef,
-    ListMetricValuesRequestRequestTypeDef,
-    ListMitigationActionsRequestListMitigationActionsPaginateTypeDef,
     ListMitigationActionsRequestRequestTypeDef,
     MitigationActionIdentifierTypeDef,
-    ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef,
     ListOTAUpdatesRequestRequestTypeDef,
     OTAUpdateSummaryTypeDef,
-    ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef,
     ListOutgoingCertificatesRequestRequestTypeDef,
     OutgoingCertificateTypeDef,
-    ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
     ListPackageVersionsRequestRequestTypeDef,
     PackageVersionSummaryTypeDef,
-    ListPackagesRequestListPackagesPaginateTypeDef,
     ListPackagesRequestRequestTypeDef,
     PackageSummaryTypeDef,
-    ListPoliciesRequestListPoliciesPaginateTypeDef,
     ListPoliciesRequestRequestTypeDef,
-    ListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef,
     ListPolicyPrincipalsRequestRequestTypeDef,
-    ListPolicyPrincipalsResponseTypeDef,
     ListPolicyVersionsRequestRequestTypeDef,
     PolicyVersionTypeDef,
-    ListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef,
     ListPrincipalPoliciesRequestRequestTypeDef,
-    ListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef,
     ListPrincipalThingsRequestRequestTypeDef,
-    ListPrincipalThingsResponseTypeDef,
-    ListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef,
     ListProvisioningTemplateVersionsRequestRequestTypeDef,
     ProvisioningTemplateVersionSummaryTypeDef,
-    ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef,
     ListProvisioningTemplatesRequestRequestTypeDef,
     ProvisioningTemplateSummaryTypeDef,
-    ListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef,
     ListRelatedResourcesForAuditFindingRequestRequestTypeDef,
-    ListRoleAliasesRequestListRoleAliasesPaginateTypeDef,
     ListRoleAliasesRequestRequestTypeDef,
-    ListRoleAliasesResponseTypeDef,
-    ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef,
     ListScheduledAuditsRequestRequestTypeDef,
     ScheduledAuditMetadataTypeDef,
-    ListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef,
     ListSecurityProfilesForTargetRequestRequestTypeDef,
-    ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef,
     ListSecurityProfilesRequestRequestTypeDef,
     SecurityProfileIdentifierTypeDef,
-    ListStreamsRequestListStreamsPaginateTypeDef,
     ListStreamsRequestRequestTypeDef,
     StreamSummaryTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
     ListTargetsForPolicyRequestRequestTypeDef,
-    ListTargetsForPolicyResponseTypeDef,
-    ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef,
     ListTargetsForSecurityProfileRequestRequestTypeDef,
     SecurityProfileTargetTypeDef,
-    ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef,
     ListThingGroupsForThingRequestRequestTypeDef,
-    ListThingGroupsRequestListThingGroupsPaginateTypeDef,
     ListThingGroupsRequestRequestTypeDef,
-    ListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef,
     ListThingPrincipalsRequestRequestTypeDef,
-    ListThingPrincipalsResponseTypeDef,
-    ListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef,
     ListThingRegistrationTaskReportsRequestRequestTypeDef,
-    ListThingRegistrationTaskReportsResponseTypeDef,
-    ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef,
     ListThingRegistrationTasksRequestRequestTypeDef,
-    ListThingRegistrationTasksResponseTypeDef,
-    ListThingTypesRequestListThingTypesPaginateTypeDef,
     ListThingTypesRequestRequestTypeDef,
-    ListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef,
     ListThingsInBillingGroupRequestRequestTypeDef,
-    ListThingsInBillingGroupResponseTypeDef,
-    ListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef,
     ListThingsInThingGroupRequestRequestTypeDef,
-    ListThingsInThingGroupResponseTypeDef,
-    ListThingsRequestListThingsPaginateTypeDef,
     ListThingsRequestRequestTypeDef,
     ThingAttributeTypeDef,
-    ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef,
     ListTopicRuleDestinationsRequestRequestTypeDef,
-    ListTopicRulesRequestListTopicRulesPaginateTypeDef,
     ListTopicRulesRequestRequestTypeDef,
     TopicRuleListItemTypeDef,
-    ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef,
     ListV2LoggingLevelsRequestRequestTypeDef,
-    ListViolationEventsRequestListViolationEventsPaginateTypeDef,
-    ListViolationEventsRequestRequestTypeDef,
     LocationTimestampTypeDef,
     LogTargetTypeDef,
     LoggingOptionsPayloadTypeDef,
     PublishFindingToSnsParamsTypeDef,
     ReplaceDefaultPolicyVersionParamsTypeDef,
     UpdateCACertificateParamsTypeDef,
     UpdateDeviceCertificateParamsTypeDef,
-    MqttContextTypeDef,
     UserPropertyTypeDef,
-    PaginatorConfigTypeDef,
     PolicyVersionIdentifierTypeDef,
     PutVerificationStateOnViolationRequestRequestTypeDef,
-    RegisterCACertificateResponseTypeDef,
     RegisterCertificateRequestRequestTypeDef,
-    RegisterCertificateResponseTypeDef,
     RegisterCertificateWithoutCARequestRequestTypeDef,
-    RegisterCertificateWithoutCAResponseTypeDef,
     RegisterThingRequestRequestTypeDef,
-    RegisterThingResponseTypeDef,
     RejectCertificateTransferRequestRequestTypeDef,
     RemoveThingFromBillingGroupRequestRequestTypeDef,
     RemoveThingFromThingGroupRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     SearchIndexRequestRequestTypeDef,
     ThingGroupDocumentTypeDef,
     SetDefaultAuthorizerRequestRequestTypeDef,
-    SetDefaultAuthorizerResponseTypeDef,
     SetDefaultPolicyVersionRequestRequestTypeDef,
     SetV2LoggingOptionsRequestRequestTypeDef,
     SigningProfileParameterTypeDef,
-    StartAuditMitigationActionsTaskResponseTypeDef,
-    StartDetectMitigationActionsTaskResponseTypeDef,
     StartOnDemandAuditTaskRequestRequestTypeDef,
-    StartOnDemandAuditTaskResponseTypeDef,
     StartThingRegistrationTaskRequestRequestTypeDef,
-    StartThingRegistrationTaskResponseTypeDef,
     StopThingRegistrationTaskRequestRequestTypeDef,
     TlsContextTypeDef,
-    TestInvokeAuthorizerResponseTypeDef,
     ThingConnectivityTypeDef,
     TimestreamDimensionTypeDef,
     TimestreamTimestampTypeDef,
     VpcDestinationConfigurationTypeDef,
     VpcDestinationSummaryTypeDef,
     VpcDestinationPropertiesTypeDef,
     TransferCertificateRequestRequestTypeDef,
-    TransferCertificateResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAuthorizerRequestRequestTypeDef,
-    UpdateAuthorizerResponseTypeDef,
-    UpdateBillingGroupResponseTypeDef,
     UpdateCertificateRequestRequestTypeDef,
     UpdateCustomMetricRequestRequestTypeDef,
-    UpdateCustomMetricResponseTypeDef,
     UpdateDimensionRequestRequestTypeDef,
-    UpdateDimensionResponseTypeDef,
-    UpdateDomainConfigurationResponseTypeDef,
-    UpdateDynamicThingGroupResponseTypeDef,
-    UpdateMitigationActionResponseTypeDef,
     UpdatePackageRequestRequestTypeDef,
     UpdatePackageVersionRequestRequestTypeDef,
     UpdateRoleAliasRequestRequestTypeDef,
-    UpdateRoleAliasResponseTypeDef,
     UpdateScheduledAuditRequestRequestTypeDef,
-    UpdateScheduledAuditResponseTypeDef,
-    UpdateStreamResponseTypeDef,
-    UpdateThingGroupResponseTypeDef,
     UpdateThingGroupsForThingRequestRequestTypeDef,
     UpdateTopicRuleDestinationRequestRequestTypeDef,
     ValidationErrorTypeDef,
+    AbortConfigOutputTypeDef,
     AbortConfigTypeDef,
     MetricDatumTypeDef,
-    DescribeFleetMetricResponseTypeDef,
+    AggregationTypeUnionTypeDef,
     UpdateFleetMetricRequestRequestTypeDef,
     AllowedTypeDef,
     ExplicitDenyTypeDef,
     ImplicitDenyTypeDef,
+    AssetPropertyValueTypeDef,
+    AssociateTargetsWithJobResponseTypeDef,
+    CancelJobResponseTypeDef,
+    CreateAuthorizerResponseTypeDef,
+    CreateBillingGroupResponseTypeDef,
+    CreateCertificateFromCsrResponseTypeDef,
+    CreateCustomMetricResponseTypeDef,
+    CreateDimensionResponseTypeDef,
+    CreateDomainConfigurationResponseTypeDef,
+    CreateDynamicThingGroupResponseTypeDef,
+    CreateFleetMetricResponseTypeDef,
+    CreateJobResponseTypeDef,
+    CreateJobTemplateResponseTypeDef,
+    CreateMitigationActionResponseTypeDef,
+    CreateOTAUpdateResponseTypeDef,
+    CreatePackageResponseTypeDef,
+    CreatePackageVersionResponseTypeDef,
+    CreatePolicyResponseTypeDef,
+    CreatePolicyVersionResponseTypeDef,
+    CreateProvisioningTemplateResponseTypeDef,
+    CreateProvisioningTemplateVersionResponseTypeDef,
+    CreateRoleAliasResponseTypeDef,
+    CreateScheduledAuditResponseTypeDef,
+    CreateSecurityProfileResponseTypeDef,
+    CreateStreamResponseTypeDef,
+    CreateThingGroupResponseTypeDef,
+    CreateThingResponseTypeDef,
+    CreateThingTypeResponseTypeDef,
+    DescribeCustomMetricResponseTypeDef,
+    DescribeDimensionResponseTypeDef,
+    DescribeEndpointResponseTypeDef,
+    DescribeFleetMetricResponseTypeDef,
+    DescribeIndexResponseTypeDef,
+    DescribeProvisioningTemplateVersionResponseTypeDef,
+    DescribeScheduledAuditResponseTypeDef,
+    DescribeThingRegistrationTaskResponseTypeDef,
+    DescribeThingResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCardinalityResponseTypeDef,
+    GetJobDocumentResponseTypeDef,
+    GetLoggingOptionsResponseTypeDef,
+    GetPackageResponseTypeDef,
+    GetPackageVersionResponseTypeDef,
+    GetPolicyResponseTypeDef,
+    GetPolicyVersionResponseTypeDef,
+    GetRegistrationCodeResponseTypeDef,
+    GetV2LoggingOptionsResponseTypeDef,
     ListAttachedPoliciesResponseTypeDef,
+    ListCustomMetricsResponseTypeDef,
+    ListDimensionsResponseTypeDef,
+    ListIndicesResponseTypeDef,
     ListPoliciesResponseTypeDef,
+    ListPolicyPrincipalsResponseTypeDef,
     ListPrincipalPoliciesResponseTypeDef,
-    AssetPropertyValueTypeDef,
+    ListPrincipalThingsResponseTypeDef,
+    ListRoleAliasesResponseTypeDef,
+    ListTargetsForPolicyResponseTypeDef,
+    ListThingPrincipalsResponseTypeDef,
+    ListThingRegistrationTaskReportsResponseTypeDef,
+    ListThingRegistrationTasksResponseTypeDef,
+    ListThingsInBillingGroupResponseTypeDef,
+    ListThingsInThingGroupResponseTypeDef,
+    RegisterCACertificateResponseTypeDef,
+    RegisterCertificateResponseTypeDef,
+    RegisterCertificateWithoutCAResponseTypeDef,
+    RegisterThingResponseTypeDef,
+    SetDefaultAuthorizerResponseTypeDef,
+    StartAuditMitigationActionsTaskResponseTypeDef,
+    StartDetectMitigationActionsTaskResponseTypeDef,
+    StartOnDemandAuditTaskResponseTypeDef,
+    StartThingRegistrationTaskResponseTypeDef,
+    TestInvokeAuthorizerResponseTypeDef,
+    TransferCertificateResponseTypeDef,
+    UpdateAuthorizerResponseTypeDef,
+    UpdateBillingGroupResponseTypeDef,
+    UpdateCustomMetricResponseTypeDef,
+    UpdateDimensionResponseTypeDef,
+    UpdateDomainConfigurationResponseTypeDef,
+    UpdateDynamicThingGroupResponseTypeDef,
+    UpdateMitigationActionResponseTypeDef,
+    UpdateRoleAliasResponseTypeDef,
+    UpdateScheduledAuditResponseTypeDef,
+    UpdateStreamResponseTypeDef,
+    UpdateThingGroupResponseTypeDef,
+    ThingGroupPropertiesOutputTypeDef,
+    AttributePayloadUnionTypeDef,
     CreateThingRequestRequestTypeDef,
     ThingGroupPropertiesTypeDef,
     UpdateThingRequestRequestTypeDef,
     ListAuditMitigationActionsExecutionsResponseTypeDef,
     ListAuditMitigationActionsTasksResponseTypeDef,
+    AuditMitigationActionsTaskTargetUnionTypeDef,
     StartAuditMitigationActionsTaskRequestRequestTypeDef,
     DescribeAccountAuditConfigurationResponseTypeDef,
     UpdateAccountAuditConfigurationRequestRequestTypeDef,
     ListAuditTasksResponseTypeDef,
-    TestAuthorizationRequestRequestTypeDef,
+    AuthInfoUnionTypeDef,
     DescribeAuthorizerResponseTypeDef,
     DescribeDefaultAuthorizerResponseTypeDef,
     ListAuthorizersResponseTypeDef,
     AwsJobAbortConfigTypeDef,
     AwsJobExponentialRolloutRateTypeDef,
+    BehaviorCriteriaOutputTypeDef,
     BehaviorCriteriaTypeDef,
     GetBehaviorModelTrainingSummariesResponseTypeDef,
     MetricToRetainTypeDef,
     DescribeBillingGroupResponseTypeDef,
     UpdateBillingGroupRequestRequestTypeDef,
+    CodeSigningSignatureTypeDef,
+    MqttContextTypeDef,
     GetBucketsAggregationResponseTypeDef,
     BucketsAggregationTypeTypeDef,
     CACertificateDescriptionTypeDef,
     ListCACertificatesResponseTypeDef,
     CertificateDescriptionTypeDef,
     ListCertificatesByCAResponseTypeDef,
     ListCertificatesResponseTypeDef,
-    CustomCodeSigningTypeDef,
+    CustomCodeSigningOutputTypeDef,
     DescribeEventConfigurationsResponseTypeDef,
     UpdateEventConfigurationsRequestRequestTypeDef,
+    ListAuditMitigationActionsTasksRequestRequestTypeDef,
+    ListAuditTasksRequestRequestTypeDef,
+    ListDetectMitigationActionsExecutionsRequestRequestTypeDef,
+    ListDetectMitigationActionsTasksRequestRequestTypeDef,
+    ListMetricValuesRequestRequestTypeDef,
+    ListViolationEventsRequestRequestTypeDef,
+    ViolationEventOccurrenceRangeTypeDef,
     CreateAuthorizerRequestRequestTypeDef,
     CreateBillingGroupRequestRequestTypeDef,
     CreateCustomMetricRequestRequestTypeDef,
     CreateDimensionRequestRequestTypeDef,
     CreateFleetMetricRequestRequestTypeDef,
     CreatePolicyRequestRequestTypeDef,
     CreateRoleAliasRequestRequestTypeDef,
     CreateScheduledAuditRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDomainConfigurationRequestRequestTypeDef,
     UpdateDomainConfigurationRequestRequestTypeDef,
+    SchedulingConfigOutputTypeDef,
     SchedulingConfigTypeDef,
     CreateKeysAndCertificateResponseTypeDef,
     CreateProvisioningClaimResponseTypeDef,
     CreateProvisioningTemplateRequestRequestTypeDef,
     DescribeProvisioningTemplateResponseTypeDef,
     UpdateProvisioningTemplateRequestRequestTypeDef,
     CreateThingTypeRequestRequestTypeDef,
@@ -1184,38 +1115,99 @@
     RegisterCACertificateRequestRequestTypeDef,
     UpdateCACertificateRequestRequestTypeDef,
     DescribeDomainConfigurationResponseTypeDef,
     DescribeManagedJobTemplateResponseTypeDef,
     DescribeRoleAliasResponseTypeDef,
     DescribeThingTypeResponseTypeDef,
     ThingTypeDefinitionTypeDef,
+    ThingTypePropertiesUnionTypeDef,
     DestinationTypeDef,
     ListDetectMitigationActionsExecutionsResponseTypeDef,
-    StartDetectMitigationActionsTaskRequestRequestTypeDef,
+    DetectMitigationActionsTaskTargetUnionTypeDef,
     ListDomainConfigurationsResponseTypeDef,
     DynamoDBv2ActionTypeDef,
     GetEffectivePoliciesResponseTypeDef,
     ExponentialRolloutRateTypeDef,
+    ThingGroupIndexingConfigurationOutputTypeDef,
     ThingGroupIndexingConfigurationTypeDef,
     StreamFileTypeDef,
     FileLocationTypeDef,
     ListFleetMetricsResponseTypeDef,
+    GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef,
+    ListActiveViolationsRequestListActiveViolationsPaginateTypeDef,
+    ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef,
+    ListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef,
+    ListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef,
+    ListAuditTasksRequestListAuditTasksPaginateTypeDef,
+    ListAuthorizersRequestListAuthorizersPaginateTypeDef,
+    ListBillingGroupsRequestListBillingGroupsPaginateTypeDef,
+    ListCACertificatesRequestListCACertificatesPaginateTypeDef,
+    ListCertificatesByCARequestListCertificatesByCAPaginateTypeDef,
+    ListCertificatesRequestListCertificatesPaginateTypeDef,
+    ListCustomMetricsRequestListCustomMetricsPaginateTypeDef,
+    ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef,
+    ListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef,
+    ListDimensionsRequestListDimensionsPaginateTypeDef,
+    ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef,
+    ListFleetMetricsRequestListFleetMetricsPaginateTypeDef,
+    ListIndicesRequestListIndicesPaginateTypeDef,
+    ListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef,
+    ListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef,
+    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
+    ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef,
+    ListMetricValuesRequestListMetricValuesPaginateTypeDef,
+    ListMitigationActionsRequestListMitigationActionsPaginateTypeDef,
+    ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef,
+    ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef,
+    ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+    ListPackagesRequestListPackagesPaginateTypeDef,
+    ListPoliciesRequestListPoliciesPaginateTypeDef,
+    ListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef,
+    ListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef,
+    ListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef,
+    ListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef,
+    ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef,
+    ListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef,
+    ListRoleAliasesRequestListRoleAliasesPaginateTypeDef,
+    ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef,
+    ListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef,
+    ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef,
+    ListStreamsRequestListStreamsPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
+    ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef,
+    ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef,
+    ListThingGroupsRequestListThingGroupsPaginateTypeDef,
+    ListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef,
+    ListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef,
+    ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef,
+    ListThingTypesRequestListThingTypesPaginateTypeDef,
+    ListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef,
+    ListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef,
+    ListThingsRequestListThingsPaginateTypeDef,
+    ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef,
+    ListTopicRulesRequestListTopicRulesPaginateTypeDef,
+    ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef,
+    ListViolationEventsRequestListViolationEventsPaginateTypeDef,
     GetPackageConfigurationResponseTypeDef,
     UpdatePackageConfigurationRequestRequestTypeDef,
     GetPercentilesResponseTypeDef,
     GetStatisticsResponseTypeDef,
     ListBillingGroupsResponseTypeDef,
     ListThingGroupsForThingResponseTypeDef,
     ListThingGroupsResponseTypeDef,
     ThingGroupMetadataTypeDef,
     HttpAuthorizationTypeDef,
+    ThingIndexingConfigurationOutputTypeDef,
     ThingIndexingConfigurationTypeDef,
     JobExecutionTypeDef,
     JobExecutionSummaryForJobTypeDef,
     JobExecutionSummaryForThingTypeDef,
+    JobExecutionsRetryConfigOutputTypeDef,
     JobExecutionsRetryConfigTypeDef,
     ListJobsResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     ListManagedJobTemplatesResponseTypeDef,
     ListMitigationActionsResponseTypeDef,
     ListOTAUpdatesResponseTypeDef,
     ListOutgoingCertificatesResponseTypeDef,
@@ -1231,55 +1223,73 @@
     SecurityProfileTargetMappingTypeDef,
     ListThingsResponseTypeDef,
     ListTopicRulesResponseTypeDef,
     LocationActionTypeDef,
     LogTargetConfigurationTypeDef,
     SetV2LoggingLevelRequestRequestTypeDef,
     SetLoggingOptionsRequestRequestTypeDef,
+    MitigationActionParamsOutputTypeDef,
     MitigationActionParamsTypeDef,
+    MqttHeadersOutputTypeDef,
     MqttHeadersTypeDef,
     ResourceIdentifierTypeDef,
-    TestInvokeAuthorizerRequestRequestTypeDef,
     ThingDocumentTypeDef,
+    TimestreamActionOutputTypeDef,
     TimestreamActionTypeDef,
     TopicRuleDestinationConfigurationTypeDef,
     TopicRuleDestinationSummaryTypeDef,
     TopicRuleDestinationTypeDef,
     ValidateSecurityProfileBehaviorsResponseTypeDef,
+    AbortConfigUnionTypeDef,
     ListMetricValuesResponseTypeDef,
     DeniedTypeDef,
+    PutAssetPropertyValueEntryOutputTypeDef,
     PutAssetPropertyValueEntryTypeDef,
     CreateDynamicThingGroupRequestRequestTypeDef,
     CreateThingGroupRequestRequestTypeDef,
+    ThingGroupPropertiesUnionTypeDef,
     UpdateDynamicThingGroupRequestRequestTypeDef,
     UpdateThingGroupRequestRequestTypeDef,
+    TestAuthorizationRequestRequestTypeDef,
     AwsJobExecutionsRolloutConfigTypeDef,
+    BehaviorOutputTypeDef,
     BehaviorTypeDef,
+    CustomCodeSigningTypeDef,
+    TestInvokeAuthorizerRequestRequestTypeDef,
     GetBucketsAggregationRequestRequestTypeDef,
     DescribeCACertificateResponseTypeDef,
     DescribeCertificateResponseTypeDef,
+    StartDetectMitigationActionsTaskRequestRequestTypeDef,
+    ViolationEventOccurrenceRangeUnionTypeDef,
+    SchedulingConfigUnionTypeDef,
     ListThingTypesResponseTypeDef,
     StartSigningJobParameterTypeDef,
     JobExecutionsRolloutConfigTypeDef,
+    ThingGroupIndexingConfigurationUnionTypeDef,
     CreateStreamRequestRequestTypeDef,
     StreamInfoTypeDef,
     UpdateStreamRequestRequestTypeDef,
     DescribeThingGroupResponseTypeDef,
+    HttpActionOutputTypeDef,
     HttpActionTypeDef,
     GetIndexingConfigurationResponseTypeDef,
+    ThingIndexingConfigurationUnionTypeDef,
     UpdateIndexingConfigurationRequestRequestTypeDef,
     DescribeJobExecutionResponseTypeDef,
     ListJobExecutionsForJobResponseTypeDef,
     ListJobExecutionsForThingResponseTypeDef,
+    JobExecutionsRetryConfigUnionTypeDef,
     ListSecurityProfilesForTargetResponseTypeDef,
     ListV2LoggingLevelsResponseTypeDef,
-    CreateMitigationActionRequestRequestTypeDef,
     DescribeMitigationActionResponseTypeDef,
     MitigationActionTypeDef,
+    CreateMitigationActionRequestRequestTypeDef,
+    MitigationActionParamsUnionTypeDef,
     UpdateMitigationActionRequestRequestTypeDef,
+    RepublishActionOutputTypeDef,
     RepublishActionTypeDef,
     AuditSuppressionTypeDef,
     CreateAuditSuppressionRequestRequestTypeDef,
     DeleteAuditSuppressionRequestRequestTypeDef,
     DescribeAuditSuppressionRequestRequestTypeDef,
     DescribeAuditSuppressionResponseTypeDef,
     ListAuditFindingsRequestListAuditFindingsPaginateTypeDef,
@@ -1291,56 +1301,62 @@
     UpdateAuditSuppressionRequestRequestTypeDef,
     SearchIndexResponseTypeDef,
     CreateTopicRuleDestinationRequestRequestTypeDef,
     ListTopicRuleDestinationsResponseTypeDef,
     CreateTopicRuleDestinationResponseTypeDef,
     GetTopicRuleDestinationResponseTypeDef,
     AuthResultTypeDef,
+    IotSiteWiseActionOutputTypeDef,
     IotSiteWiseActionTypeDef,
     ActiveViolationTypeDef,
-    CreateSecurityProfileRequestRequestTypeDef,
     DescribeSecurityProfileResponseTypeDef,
-    UpdateSecurityProfileRequestRequestTypeDef,
     UpdateSecurityProfileResponseTypeDef,
-    ValidateSecurityProfileBehaviorsRequestRequestTypeDef,
     ViolationEventTypeDef,
+    BehaviorUnionTypeDef,
+    CodeSigningOutputTypeDef,
     CodeSigningTypeDef,
     CreateJobRequestRequestTypeDef,
     CreateJobTemplateRequestRequestTypeDef,
     DescribeJobTemplateResponseTypeDef,
     JobTypeDef,
     UpdateJobRequestRequestTypeDef,
     DescribeStreamResponseTypeDef,
     DescribeAuditMitigationActionsTaskResponseTypeDef,
     DetectMitigationActionsTaskSummaryTypeDef,
     ListAuditSuppressionsResponseTypeDef,
     AuditFindingTypeDef,
     ListRelatedResourcesForAuditFindingResponseTypeDef,
     TestAuthorizationResponseTypeDef,
+    ActionOutputTypeDef,
     ActionTypeDef,
     ListActiveViolationsResponseTypeDef,
     ListViolationEventsResponseTypeDef,
+    CreateSecurityProfileRequestRequestTypeDef,
+    UpdateSecurityProfileRequestRequestTypeDef,
+    ValidateSecurityProfileBehaviorsRequestRequestTypeDef,
+    OTAUpdateFileOutputTypeDef,
     OTAUpdateFileTypeDef,
     DescribeJobResponseTypeDef,
     DescribeDetectMitigationActionsTaskResponseTypeDef,
     ListDetectMitigationActionsTasksResponseTypeDef,
     DescribeAuditFindingResponseTypeDef,
     ListAuditFindingsResponseTypeDef,
-    TopicRulePayloadTypeDef,
     TopicRuleTypeDef,
-    CreateOTAUpdateRequestRequestTypeDef,
+    TopicRulePayloadTypeDef,
     OTAUpdateInfoTypeDef,
+    OTAUpdateFileUnionTypeDef,
+    GetTopicRuleResponseTypeDef,
     CreateTopicRuleRequestRequestTypeDef,
     ReplaceTopicRuleRequestRequestTypeDef,
-    GetTopicRuleResponseTypeDef,
     GetOTAUpdateResponseTypeDef,
+    CreateOTAUpdateRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AbortCriteriaTypeDef:
+def get_value() -> AbortCriteriaTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iot-2.5.2/README.md` & `types-aiobotocore-iot-2.5.2.post1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-iot
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IoT 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore iot type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iot"></a>
 
 # types-aiobotocore-iot
 
 [![PyPI - types-aiobotocore-iot](https://img.shields.io/pypi/v/types-aiobotocore-iot.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iot?color=blue)](https://pypistats.org/packages/types-aiobotocore-iot)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot)](https://pepy.tech/project/types-aiobotocore-iot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoT 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
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
 [types-aiobotocore-iot docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/).
 
 See how it helps to find and fix potential bugs:
 
@@ -41,15 +73,15 @@
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
@@ -610,137 +642,120 @@
 )
 
 
 def check_value(value: AbortActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iot.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iot.type_defs import (
     AbortCriteriaTypeDef,
     AcceptCertificateTransferRequestRequestTypeDef,
     CloudwatchAlarmActionTypeDef,
     CloudwatchLogsActionTypeDef,
     CloudwatchMetricActionTypeDef,
     DynamoDBActionTypeDef,
     ElasticsearchActionTypeDef,
     FirehoseActionTypeDef,
     IotAnalyticsActionTypeDef,
     IotEventsActionTypeDef,
-    KafkaActionTypeDef,
+    KafkaActionOutputTypeDef,
     KinesisActionTypeDef,
     LambdaActionTypeDef,
     OpenSearchActionTypeDef,
     S3ActionTypeDef,
     SalesforceActionTypeDef,
     SnsActionTypeDef,
     SqsActionTypeDef,
     StepFunctionsActionTypeDef,
-    MetricValueTypeDef,
+    KafkaActionTypeDef,
+    MetricValueOutputTypeDef,
     ViolationEventAdditionalInfoTypeDef,
     AddThingToBillingGroupRequestRequestTypeDef,
     AddThingToThingGroupRequestRequestTypeDef,
+    AddThingsToThingGroupParamsOutputTypeDef,
     AddThingsToThingGroupParamsTypeDef,
+    AggregationTypeOutputTypeDef,
     AggregationTypeTypeDef,
     AlertTargetTypeDef,
     PolicyTypeDef,
     AssetPropertyTimestampTypeDef,
     AssetPropertyVariantTypeDef,
     AssociateTargetsWithJobRequestRequestTypeDef,
-    AssociateTargetsWithJobResponseTypeDef,
+    ResponseMetadataTypeDef,
     AttachPolicyRequestRequestTypeDef,
     AttachPrincipalPolicyRequestRequestTypeDef,
     AttachSecurityProfileRequestRequestTypeDef,
     AttachThingPrincipalRequestRequestTypeDef,
+    AttributePayloadOutputTypeDef,
     AttributePayloadTypeDef,
     AuditCheckConfigurationTypeDef,
     AuditCheckDetailsTypeDef,
     AuditMitigationActionExecutionMetadataTypeDef,
     AuditMitigationActionsTaskMetadataTypeDef,
+    AuditMitigationActionsTaskTargetOutputTypeDef,
     AuditMitigationActionsTaskTargetTypeDef,
     AuditNotificationTargetTypeDef,
     AuditTaskMetadataTypeDef,
+    AuthInfoOutputTypeDef,
     AuthInfoTypeDef,
     AuthorizerConfigTypeDef,
     AuthorizerDescriptionTypeDef,
     AuthorizerSummaryTypeDef,
     AwsJobAbortCriteriaTypeDef,
     AwsJobRateIncreaseCriteriaTypeDef,
     AwsJobPresignedUrlConfigTypeDef,
     AwsJobTimeoutConfigTypeDef,
     MachineLearningDetectionConfigTypeDef,
     StatisticalThresholdTypeDef,
+    MetricValueTypeDef,
     BehaviorModelTrainingSummaryTypeDef,
     MetricDimensionTypeDef,
     BillingGroupMetadataTypeDef,
     BillingGroupPropertiesTypeDef,
+    BlobTypeDef,
     BucketTypeDef,
     TermsAggregationTypeDef,
     CertificateValidityTypeDef,
     CACertificateTypeDef,
     CancelAuditMitigationActionsTaskRequestRequestTypeDef,
     CancelAuditTaskRequestRequestTypeDef,
     CancelCertificateTransferRequestRequestTypeDef,
     CancelDetectMitigationActionsTaskRequestRequestTypeDef,
     CancelJobExecutionRequestRequestTypeDef,
     CancelJobRequestRequestTypeDef,
-    CancelJobResponseTypeDef,
     TransferDataTypeDef,
     CertificateTypeDef,
     CodeSigningCertificateChainTypeDef,
-    CodeSigningSignatureTypeDef,
+    CodeSigningSignatureOutputTypeDef,
     ConfigurationTypeDef,
     ConfirmTopicRuleDestinationRequestRequestTypeDef,
+    TimestampTypeDef,
     TagTypeDef,
-    CreateAuthorizerResponseTypeDef,
-    CreateBillingGroupResponseTypeDef,
     CreateCertificateFromCsrRequestRequestTypeDef,
-    CreateCertificateFromCsrResponseTypeDef,
-    CreateCustomMetricResponseTypeDef,
-    CreateDimensionResponseTypeDef,
     TlsConfigTypeDef,
-    CreateDomainConfigurationResponseTypeDef,
-    CreateDynamicThingGroupResponseTypeDef,
-    CreateFleetMetricResponseTypeDef,
     PresignedUrlConfigTypeDef,
     TimeoutConfigTypeDef,
-    CreateJobResponseTypeDef,
     MaintenanceWindowTypeDef,
-    CreateJobTemplateResponseTypeDef,
     CreateKeysAndCertificateRequestRequestTypeDef,
     KeyPairTypeDef,
-    CreateMitigationActionResponseTypeDef,
-    CreateOTAUpdateResponseTypeDef,
     CreatePackageRequestRequestTypeDef,
-    CreatePackageResponseTypeDef,
     CreatePackageVersionRequestRequestTypeDef,
-    CreatePackageVersionResponseTypeDef,
-    CreatePolicyResponseTypeDef,
     CreatePolicyVersionRequestRequestTypeDef,
-    CreatePolicyVersionResponseTypeDef,
     CreateProvisioningClaimRequestRequestTypeDef,
     ProvisioningHookTypeDef,
-    CreateProvisioningTemplateResponseTypeDef,
     CreateProvisioningTemplateVersionRequestRequestTypeDef,
-    CreateProvisioningTemplateVersionResponseTypeDef,
-    CreateRoleAliasResponseTypeDef,
-    CreateScheduledAuditResponseTypeDef,
-    CreateSecurityProfileResponseTypeDef,
-    CreateStreamResponseTypeDef,
-    CreateThingGroupResponseTypeDef,
-    CreateThingResponseTypeDef,
     ThingTypePropertiesTypeDef,
-    CreateThingTypeResponseTypeDef,
     DeleteAccountAuditConfigurationRequestRequestTypeDef,
     DeleteAuthorizerRequestRequestTypeDef,
     DeleteBillingGroupRequestRequestTypeDef,
     DeleteCACertificateRequestRequestTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     DeleteCustomMetricRequestRequestTypeDef,
     DeleteDimensionRequestRequestTypeDef,
@@ -776,374 +791,355 @@
     TaskStatisticsTypeDef,
     DescribeAuthorizerRequestRequestTypeDef,
     DescribeBillingGroupRequestRequestTypeDef,
     DescribeCACertificateRequestRequestTypeDef,
     RegistrationConfigTypeDef,
     DescribeCertificateRequestRequestTypeDef,
     DescribeCustomMetricRequestRequestTypeDef,
-    DescribeCustomMetricResponseTypeDef,
     DescribeDetectMitigationActionsTaskRequestRequestTypeDef,
     DescribeDimensionRequestRequestTypeDef,
-    DescribeDimensionResponseTypeDef,
     DescribeDomainConfigurationRequestRequestTypeDef,
     ServerCertificateSummaryTypeDef,
     DescribeEndpointRequestRequestTypeDef,
-    DescribeEndpointResponseTypeDef,
     DescribeFleetMetricRequestRequestTypeDef,
     DescribeIndexRequestRequestTypeDef,
-    DescribeIndexResponseTypeDef,
     DescribeJobExecutionRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeJobTemplateRequestRequestTypeDef,
     DescribeManagedJobTemplateRequestRequestTypeDef,
     DocumentParameterTypeDef,
     DescribeMitigationActionRequestRequestTypeDef,
     DescribeProvisioningTemplateRequestRequestTypeDef,
     DescribeProvisioningTemplateVersionRequestRequestTypeDef,
-    DescribeProvisioningTemplateVersionResponseTypeDef,
     DescribeRoleAliasRequestRequestTypeDef,
     RoleAliasDescriptionTypeDef,
     DescribeScheduledAuditRequestRequestTypeDef,
-    DescribeScheduledAuditResponseTypeDef,
     DescribeSecurityProfileRequestRequestTypeDef,
     DescribeStreamRequestRequestTypeDef,
     DescribeThingGroupRequestRequestTypeDef,
     DescribeThingRegistrationTaskRequestRequestTypeDef,
-    DescribeThingRegistrationTaskResponseTypeDef,
     DescribeThingRequestRequestTypeDef,
-    DescribeThingResponseTypeDef,
     DescribeThingTypeRequestRequestTypeDef,
     ThingTypeMetadataTypeDef,
+    ThingTypePropertiesOutputTypeDef,
     S3DestinationTypeDef,
     DetachPolicyRequestRequestTypeDef,
     DetachPrincipalPolicyRequestRequestTypeDef,
     DetachSecurityProfileRequestRequestTypeDef,
     DetachThingPrincipalRequestRequestTypeDef,
     DetectMitigationActionExecutionTypeDef,
     DetectMitigationActionsTaskStatisticsTypeDef,
+    DetectMitigationActionsTaskTargetOutputTypeDef,
+    ViolationEventOccurrenceRangeOutputTypeDef,
     DetectMitigationActionsTaskTargetTypeDef,
-    ViolationEventOccurrenceRangeTypeDef,
     DisableTopicRuleRequestRequestTypeDef,
     DomainConfigurationSummaryTypeDef,
     PutItemInputTypeDef,
     EffectivePolicyTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableIoTLoggingParamsTypeDef,
     EnableTopicRuleRequestRequestTypeDef,
     ErrorInfoTypeDef,
     RateIncreaseCriteriaTypeDef,
     FieldTypeDef,
     S3LocationTypeDef,
     StreamTypeDef,
     FleetMetricNameAndArnTypeDef,
-    GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetBehaviorModelTrainingSummariesRequestRequestTypeDef,
     GetCardinalityRequestRequestTypeDef,
-    GetCardinalityResponseTypeDef,
     GetEffectivePoliciesRequestRequestTypeDef,
     GetJobDocumentRequestRequestTypeDef,
-    GetJobDocumentResponseTypeDef,
-    GetLoggingOptionsResponseTypeDef,
     GetOTAUpdateRequestRequestTypeDef,
     VersionUpdateByJobsConfigTypeDef,
     GetPackageRequestRequestTypeDef,
-    GetPackageResponseTypeDef,
     GetPackageVersionRequestRequestTypeDef,
-    GetPackageVersionResponseTypeDef,
     GetPercentilesRequestRequestTypeDef,
     PercentPairTypeDef,
     GetPolicyRequestRequestTypeDef,
-    GetPolicyResponseTypeDef,
     GetPolicyVersionRequestRequestTypeDef,
-    GetPolicyVersionResponseTypeDef,
-    GetRegistrationCodeResponseTypeDef,
     GetStatisticsRequestRequestTypeDef,
     StatisticsTypeDef,
     GetTopicRuleDestinationRequestRequestTypeDef,
     GetTopicRuleRequestRequestTypeDef,
-    GetV2LoggingOptionsResponseTypeDef,
     GroupNameAndArnTypeDef,
     HttpActionHeaderTypeDef,
     SigV4AuthorizationTypeDef,
     HttpContextTypeDef,
     HttpUrlDestinationConfigurationTypeDef,
     HttpUrlDestinationPropertiesTypeDef,
     HttpUrlDestinationSummaryTypeDef,
+    IndexingFilterOutputTypeDef,
     IndexingFilterTypeDef,
     IssuerCertificateIdentifierTypeDef,
     JobExecutionStatusDetailsTypeDef,
     JobExecutionSummaryTypeDef,
     RetryCriteriaTypeDef,
     JobProcessDetailsTypeDef,
     JobSummaryTypeDef,
     JobTemplateSummaryTypeDef,
     ScheduledJobRolloutTypeDef,
-    ListActiveViolationsRequestListActiveViolationsPaginateTypeDef,
     ListActiveViolationsRequestRequestTypeDef,
-    ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef,
     ListAttachedPoliciesRequestRequestTypeDef,
-    ListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef,
     ListAuditMitigationActionsExecutionsRequestRequestTypeDef,
-    ListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef,
-    ListAuditMitigationActionsTasksRequestRequestTypeDef,
-    ListAuditTasksRequestListAuditTasksPaginateTypeDef,
-    ListAuditTasksRequestRequestTypeDef,
-    ListAuthorizersRequestListAuthorizersPaginateTypeDef,
     ListAuthorizersRequestRequestTypeDef,
-    ListBillingGroupsRequestListBillingGroupsPaginateTypeDef,
     ListBillingGroupsRequestRequestTypeDef,
-    ListCACertificatesRequestListCACertificatesPaginateTypeDef,
     ListCACertificatesRequestRequestTypeDef,
-    ListCertificatesByCARequestListCertificatesByCAPaginateTypeDef,
     ListCertificatesByCARequestRequestTypeDef,
-    ListCertificatesRequestListCertificatesPaginateTypeDef,
     ListCertificatesRequestRequestTypeDef,
-    ListCustomMetricsRequestListCustomMetricsPaginateTypeDef,
     ListCustomMetricsRequestRequestTypeDef,
-    ListCustomMetricsResponseTypeDef,
-    ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef,
-    ListDetectMitigationActionsExecutionsRequestRequestTypeDef,
-    ListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef,
-    ListDetectMitigationActionsTasksRequestRequestTypeDef,
-    ListDimensionsRequestListDimensionsPaginateTypeDef,
     ListDimensionsRequestRequestTypeDef,
-    ListDimensionsResponseTypeDef,
-    ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef,
     ListDomainConfigurationsRequestRequestTypeDef,
-    ListFleetMetricsRequestListFleetMetricsPaginateTypeDef,
     ListFleetMetricsRequestRequestTypeDef,
-    ListIndicesRequestListIndicesPaginateTypeDef,
     ListIndicesRequestRequestTypeDef,
-    ListIndicesResponseTypeDef,
-    ListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef,
     ListJobExecutionsForJobRequestRequestTypeDef,
-    ListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef,
     ListJobExecutionsForThingRequestRequestTypeDef,
-    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
-    ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef,
     ListManagedJobTemplatesRequestRequestTypeDef,
     ManagedJobTemplateSummaryTypeDef,
-    ListMetricValuesRequestListMetricValuesPaginateTypeDef,
-    ListMetricValuesRequestRequestTypeDef,
-    ListMitigationActionsRequestListMitigationActionsPaginateTypeDef,
     ListMitigationActionsRequestRequestTypeDef,
     MitigationActionIdentifierTypeDef,
-    ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef,
     ListOTAUpdatesRequestRequestTypeDef,
     OTAUpdateSummaryTypeDef,
-    ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef,
     ListOutgoingCertificatesRequestRequestTypeDef,
     OutgoingCertificateTypeDef,
-    ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
     ListPackageVersionsRequestRequestTypeDef,
     PackageVersionSummaryTypeDef,
-    ListPackagesRequestListPackagesPaginateTypeDef,
     ListPackagesRequestRequestTypeDef,
     PackageSummaryTypeDef,
-    ListPoliciesRequestListPoliciesPaginateTypeDef,
     ListPoliciesRequestRequestTypeDef,
-    ListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef,
     ListPolicyPrincipalsRequestRequestTypeDef,
-    ListPolicyPrincipalsResponseTypeDef,
     ListPolicyVersionsRequestRequestTypeDef,
     PolicyVersionTypeDef,
-    ListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef,
     ListPrincipalPoliciesRequestRequestTypeDef,
-    ListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef,
     ListPrincipalThingsRequestRequestTypeDef,
-    ListPrincipalThingsResponseTypeDef,
-    ListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef,
     ListProvisioningTemplateVersionsRequestRequestTypeDef,
     ProvisioningTemplateVersionSummaryTypeDef,
-    ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef,
     ListProvisioningTemplatesRequestRequestTypeDef,
     ProvisioningTemplateSummaryTypeDef,
-    ListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef,
     ListRelatedResourcesForAuditFindingRequestRequestTypeDef,
-    ListRoleAliasesRequestListRoleAliasesPaginateTypeDef,
     ListRoleAliasesRequestRequestTypeDef,
-    ListRoleAliasesResponseTypeDef,
-    ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef,
     ListScheduledAuditsRequestRequestTypeDef,
     ScheduledAuditMetadataTypeDef,
-    ListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef,
     ListSecurityProfilesForTargetRequestRequestTypeDef,
-    ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef,
     ListSecurityProfilesRequestRequestTypeDef,
     SecurityProfileIdentifierTypeDef,
-    ListStreamsRequestListStreamsPaginateTypeDef,
     ListStreamsRequestRequestTypeDef,
     StreamSummaryTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
     ListTargetsForPolicyRequestRequestTypeDef,
-    ListTargetsForPolicyResponseTypeDef,
-    ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef,
     ListTargetsForSecurityProfileRequestRequestTypeDef,
     SecurityProfileTargetTypeDef,
-    ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef,
     ListThingGroupsForThingRequestRequestTypeDef,
-    ListThingGroupsRequestListThingGroupsPaginateTypeDef,
     ListThingGroupsRequestRequestTypeDef,
-    ListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef,
     ListThingPrincipalsRequestRequestTypeDef,
-    ListThingPrincipalsResponseTypeDef,
-    ListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef,
     ListThingRegistrationTaskReportsRequestRequestTypeDef,
-    ListThingRegistrationTaskReportsResponseTypeDef,
-    ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef,
     ListThingRegistrationTasksRequestRequestTypeDef,
-    ListThingRegistrationTasksResponseTypeDef,
-    ListThingTypesRequestListThingTypesPaginateTypeDef,
     ListThingTypesRequestRequestTypeDef,
-    ListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef,
     ListThingsInBillingGroupRequestRequestTypeDef,
-    ListThingsInBillingGroupResponseTypeDef,
-    ListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef,
     ListThingsInThingGroupRequestRequestTypeDef,
-    ListThingsInThingGroupResponseTypeDef,
-    ListThingsRequestListThingsPaginateTypeDef,
     ListThingsRequestRequestTypeDef,
     ThingAttributeTypeDef,
-    ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef,
     ListTopicRuleDestinationsRequestRequestTypeDef,
-    ListTopicRulesRequestListTopicRulesPaginateTypeDef,
     ListTopicRulesRequestRequestTypeDef,
     TopicRuleListItemTypeDef,
-    ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef,
     ListV2LoggingLevelsRequestRequestTypeDef,
-    ListViolationEventsRequestListViolationEventsPaginateTypeDef,
-    ListViolationEventsRequestRequestTypeDef,
     LocationTimestampTypeDef,
     LogTargetTypeDef,
     LoggingOptionsPayloadTypeDef,
     PublishFindingToSnsParamsTypeDef,
     ReplaceDefaultPolicyVersionParamsTypeDef,
     UpdateCACertificateParamsTypeDef,
     UpdateDeviceCertificateParamsTypeDef,
-    MqttContextTypeDef,
     UserPropertyTypeDef,
-    PaginatorConfigTypeDef,
     PolicyVersionIdentifierTypeDef,
     PutVerificationStateOnViolationRequestRequestTypeDef,
-    RegisterCACertificateResponseTypeDef,
     RegisterCertificateRequestRequestTypeDef,
-    RegisterCertificateResponseTypeDef,
     RegisterCertificateWithoutCARequestRequestTypeDef,
-    RegisterCertificateWithoutCAResponseTypeDef,
     RegisterThingRequestRequestTypeDef,
-    RegisterThingResponseTypeDef,
     RejectCertificateTransferRequestRequestTypeDef,
     RemoveThingFromBillingGroupRequestRequestTypeDef,
     RemoveThingFromThingGroupRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     SearchIndexRequestRequestTypeDef,
     ThingGroupDocumentTypeDef,
     SetDefaultAuthorizerRequestRequestTypeDef,
-    SetDefaultAuthorizerResponseTypeDef,
     SetDefaultPolicyVersionRequestRequestTypeDef,
     SetV2LoggingOptionsRequestRequestTypeDef,
     SigningProfileParameterTypeDef,
-    StartAuditMitigationActionsTaskResponseTypeDef,
-    StartDetectMitigationActionsTaskResponseTypeDef,
     StartOnDemandAuditTaskRequestRequestTypeDef,
-    StartOnDemandAuditTaskResponseTypeDef,
     StartThingRegistrationTaskRequestRequestTypeDef,
-    StartThingRegistrationTaskResponseTypeDef,
     StopThingRegistrationTaskRequestRequestTypeDef,
     TlsContextTypeDef,
-    TestInvokeAuthorizerResponseTypeDef,
     ThingConnectivityTypeDef,
     TimestreamDimensionTypeDef,
     TimestreamTimestampTypeDef,
     VpcDestinationConfigurationTypeDef,
     VpcDestinationSummaryTypeDef,
     VpcDestinationPropertiesTypeDef,
     TransferCertificateRequestRequestTypeDef,
-    TransferCertificateResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAuthorizerRequestRequestTypeDef,
-    UpdateAuthorizerResponseTypeDef,
-    UpdateBillingGroupResponseTypeDef,
     UpdateCertificateRequestRequestTypeDef,
     UpdateCustomMetricRequestRequestTypeDef,
-    UpdateCustomMetricResponseTypeDef,
     UpdateDimensionRequestRequestTypeDef,
-    UpdateDimensionResponseTypeDef,
-    UpdateDomainConfigurationResponseTypeDef,
-    UpdateDynamicThingGroupResponseTypeDef,
-    UpdateMitigationActionResponseTypeDef,
     UpdatePackageRequestRequestTypeDef,
     UpdatePackageVersionRequestRequestTypeDef,
     UpdateRoleAliasRequestRequestTypeDef,
-    UpdateRoleAliasResponseTypeDef,
     UpdateScheduledAuditRequestRequestTypeDef,
-    UpdateScheduledAuditResponseTypeDef,
-    UpdateStreamResponseTypeDef,
-    UpdateThingGroupResponseTypeDef,
     UpdateThingGroupsForThingRequestRequestTypeDef,
     UpdateTopicRuleDestinationRequestRequestTypeDef,
     ValidationErrorTypeDef,
+    AbortConfigOutputTypeDef,
     AbortConfigTypeDef,
     MetricDatumTypeDef,
-    DescribeFleetMetricResponseTypeDef,
+    AggregationTypeUnionTypeDef,
     UpdateFleetMetricRequestRequestTypeDef,
     AllowedTypeDef,
     ExplicitDenyTypeDef,
     ImplicitDenyTypeDef,
+    AssetPropertyValueTypeDef,
+    AssociateTargetsWithJobResponseTypeDef,
+    CancelJobResponseTypeDef,
+    CreateAuthorizerResponseTypeDef,
+    CreateBillingGroupResponseTypeDef,
+    CreateCertificateFromCsrResponseTypeDef,
+    CreateCustomMetricResponseTypeDef,
+    CreateDimensionResponseTypeDef,
+    CreateDomainConfigurationResponseTypeDef,
+    CreateDynamicThingGroupResponseTypeDef,
+    CreateFleetMetricResponseTypeDef,
+    CreateJobResponseTypeDef,
+    CreateJobTemplateResponseTypeDef,
+    CreateMitigationActionResponseTypeDef,
+    CreateOTAUpdateResponseTypeDef,
+    CreatePackageResponseTypeDef,
+    CreatePackageVersionResponseTypeDef,
+    CreatePolicyResponseTypeDef,
+    CreatePolicyVersionResponseTypeDef,
+    CreateProvisioningTemplateResponseTypeDef,
+    CreateProvisioningTemplateVersionResponseTypeDef,
+    CreateRoleAliasResponseTypeDef,
+    CreateScheduledAuditResponseTypeDef,
+    CreateSecurityProfileResponseTypeDef,
+    CreateStreamResponseTypeDef,
+    CreateThingGroupResponseTypeDef,
+    CreateThingResponseTypeDef,
+    CreateThingTypeResponseTypeDef,
+    DescribeCustomMetricResponseTypeDef,
+    DescribeDimensionResponseTypeDef,
+    DescribeEndpointResponseTypeDef,
+    DescribeFleetMetricResponseTypeDef,
+    DescribeIndexResponseTypeDef,
+    DescribeProvisioningTemplateVersionResponseTypeDef,
+    DescribeScheduledAuditResponseTypeDef,
+    DescribeThingRegistrationTaskResponseTypeDef,
+    DescribeThingResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCardinalityResponseTypeDef,
+    GetJobDocumentResponseTypeDef,
+    GetLoggingOptionsResponseTypeDef,
+    GetPackageResponseTypeDef,
+    GetPackageVersionResponseTypeDef,
+    GetPolicyResponseTypeDef,
+    GetPolicyVersionResponseTypeDef,
+    GetRegistrationCodeResponseTypeDef,
+    GetV2LoggingOptionsResponseTypeDef,
     ListAttachedPoliciesResponseTypeDef,
+    ListCustomMetricsResponseTypeDef,
+    ListDimensionsResponseTypeDef,
+    ListIndicesResponseTypeDef,
     ListPoliciesResponseTypeDef,
+    ListPolicyPrincipalsResponseTypeDef,
     ListPrincipalPoliciesResponseTypeDef,
-    AssetPropertyValueTypeDef,
+    ListPrincipalThingsResponseTypeDef,
+    ListRoleAliasesResponseTypeDef,
+    ListTargetsForPolicyResponseTypeDef,
+    ListThingPrincipalsResponseTypeDef,
+    ListThingRegistrationTaskReportsResponseTypeDef,
+    ListThingRegistrationTasksResponseTypeDef,
+    ListThingsInBillingGroupResponseTypeDef,
+    ListThingsInThingGroupResponseTypeDef,
+    RegisterCACertificateResponseTypeDef,
+    RegisterCertificateResponseTypeDef,
+    RegisterCertificateWithoutCAResponseTypeDef,
+    RegisterThingResponseTypeDef,
+    SetDefaultAuthorizerResponseTypeDef,
+    StartAuditMitigationActionsTaskResponseTypeDef,
+    StartDetectMitigationActionsTaskResponseTypeDef,
+    StartOnDemandAuditTaskResponseTypeDef,
+    StartThingRegistrationTaskResponseTypeDef,
+    TestInvokeAuthorizerResponseTypeDef,
+    TransferCertificateResponseTypeDef,
+    UpdateAuthorizerResponseTypeDef,
+    UpdateBillingGroupResponseTypeDef,
+    UpdateCustomMetricResponseTypeDef,
+    UpdateDimensionResponseTypeDef,
+    UpdateDomainConfigurationResponseTypeDef,
+    UpdateDynamicThingGroupResponseTypeDef,
+    UpdateMitigationActionResponseTypeDef,
+    UpdateRoleAliasResponseTypeDef,
+    UpdateScheduledAuditResponseTypeDef,
+    UpdateStreamResponseTypeDef,
+    UpdateThingGroupResponseTypeDef,
+    ThingGroupPropertiesOutputTypeDef,
+    AttributePayloadUnionTypeDef,
     CreateThingRequestRequestTypeDef,
     ThingGroupPropertiesTypeDef,
     UpdateThingRequestRequestTypeDef,
     ListAuditMitigationActionsExecutionsResponseTypeDef,
     ListAuditMitigationActionsTasksResponseTypeDef,
+    AuditMitigationActionsTaskTargetUnionTypeDef,
     StartAuditMitigationActionsTaskRequestRequestTypeDef,
     DescribeAccountAuditConfigurationResponseTypeDef,
     UpdateAccountAuditConfigurationRequestRequestTypeDef,
     ListAuditTasksResponseTypeDef,
-    TestAuthorizationRequestRequestTypeDef,
+    AuthInfoUnionTypeDef,
     DescribeAuthorizerResponseTypeDef,
     DescribeDefaultAuthorizerResponseTypeDef,
     ListAuthorizersResponseTypeDef,
     AwsJobAbortConfigTypeDef,
     AwsJobExponentialRolloutRateTypeDef,
+    BehaviorCriteriaOutputTypeDef,
     BehaviorCriteriaTypeDef,
     GetBehaviorModelTrainingSummariesResponseTypeDef,
     MetricToRetainTypeDef,
     DescribeBillingGroupResponseTypeDef,
     UpdateBillingGroupRequestRequestTypeDef,
+    CodeSigningSignatureTypeDef,
+    MqttContextTypeDef,
     GetBucketsAggregationResponseTypeDef,
     BucketsAggregationTypeTypeDef,
     CACertificateDescriptionTypeDef,
     ListCACertificatesResponseTypeDef,
     CertificateDescriptionTypeDef,
     ListCertificatesByCAResponseTypeDef,
     ListCertificatesResponseTypeDef,
-    CustomCodeSigningTypeDef,
+    CustomCodeSigningOutputTypeDef,
     DescribeEventConfigurationsResponseTypeDef,
     UpdateEventConfigurationsRequestRequestTypeDef,
+    ListAuditMitigationActionsTasksRequestRequestTypeDef,
+    ListAuditTasksRequestRequestTypeDef,
+    ListDetectMitigationActionsExecutionsRequestRequestTypeDef,
+    ListDetectMitigationActionsTasksRequestRequestTypeDef,
+    ListMetricValuesRequestRequestTypeDef,
+    ListViolationEventsRequestRequestTypeDef,
+    ViolationEventOccurrenceRangeTypeDef,
     CreateAuthorizerRequestRequestTypeDef,
     CreateBillingGroupRequestRequestTypeDef,
     CreateCustomMetricRequestRequestTypeDef,
     CreateDimensionRequestRequestTypeDef,
     CreateFleetMetricRequestRequestTypeDef,
     CreatePolicyRequestRequestTypeDef,
     CreateRoleAliasRequestRequestTypeDef,
     CreateScheduledAuditRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDomainConfigurationRequestRequestTypeDef,
     UpdateDomainConfigurationRequestRequestTypeDef,
+    SchedulingConfigOutputTypeDef,
     SchedulingConfigTypeDef,
     CreateKeysAndCertificateResponseTypeDef,
     CreateProvisioningClaimResponseTypeDef,
     CreateProvisioningTemplateRequestRequestTypeDef,
     DescribeProvisioningTemplateResponseTypeDef,
     UpdateProvisioningTemplateRequestRequestTypeDef,
     CreateThingTypeRequestRequestTypeDef,
@@ -1151,38 +1147,99 @@
     RegisterCACertificateRequestRequestTypeDef,
     UpdateCACertificateRequestRequestTypeDef,
     DescribeDomainConfigurationResponseTypeDef,
     DescribeManagedJobTemplateResponseTypeDef,
     DescribeRoleAliasResponseTypeDef,
     DescribeThingTypeResponseTypeDef,
     ThingTypeDefinitionTypeDef,
+    ThingTypePropertiesUnionTypeDef,
     DestinationTypeDef,
     ListDetectMitigationActionsExecutionsResponseTypeDef,
-    StartDetectMitigationActionsTaskRequestRequestTypeDef,
+    DetectMitigationActionsTaskTargetUnionTypeDef,
     ListDomainConfigurationsResponseTypeDef,
     DynamoDBv2ActionTypeDef,
     GetEffectivePoliciesResponseTypeDef,
     ExponentialRolloutRateTypeDef,
+    ThingGroupIndexingConfigurationOutputTypeDef,
     ThingGroupIndexingConfigurationTypeDef,
     StreamFileTypeDef,
     FileLocationTypeDef,
     ListFleetMetricsResponseTypeDef,
+    GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef,
+    ListActiveViolationsRequestListActiveViolationsPaginateTypeDef,
+    ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef,
+    ListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef,
+    ListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef,
+    ListAuditTasksRequestListAuditTasksPaginateTypeDef,
+    ListAuthorizersRequestListAuthorizersPaginateTypeDef,
+    ListBillingGroupsRequestListBillingGroupsPaginateTypeDef,
+    ListCACertificatesRequestListCACertificatesPaginateTypeDef,
+    ListCertificatesByCARequestListCertificatesByCAPaginateTypeDef,
+    ListCertificatesRequestListCertificatesPaginateTypeDef,
+    ListCustomMetricsRequestListCustomMetricsPaginateTypeDef,
+    ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef,
+    ListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef,
+    ListDimensionsRequestListDimensionsPaginateTypeDef,
+    ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef,
+    ListFleetMetricsRequestListFleetMetricsPaginateTypeDef,
+    ListIndicesRequestListIndicesPaginateTypeDef,
+    ListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef,
+    ListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef,
+    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
+    ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef,
+    ListMetricValuesRequestListMetricValuesPaginateTypeDef,
+    ListMitigationActionsRequestListMitigationActionsPaginateTypeDef,
+    ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef,
+    ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef,
+    ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+    ListPackagesRequestListPackagesPaginateTypeDef,
+    ListPoliciesRequestListPoliciesPaginateTypeDef,
+    ListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef,
+    ListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef,
+    ListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef,
+    ListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef,
+    ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef,
+    ListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef,
+    ListRoleAliasesRequestListRoleAliasesPaginateTypeDef,
+    ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef,
+    ListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef,
+    ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef,
+    ListStreamsRequestListStreamsPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
+    ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef,
+    ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef,
+    ListThingGroupsRequestListThingGroupsPaginateTypeDef,
+    ListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef,
+    ListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef,
+    ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef,
+    ListThingTypesRequestListThingTypesPaginateTypeDef,
+    ListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef,
+    ListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef,
+    ListThingsRequestListThingsPaginateTypeDef,
+    ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef,
+    ListTopicRulesRequestListTopicRulesPaginateTypeDef,
+    ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef,
+    ListViolationEventsRequestListViolationEventsPaginateTypeDef,
     GetPackageConfigurationResponseTypeDef,
     UpdatePackageConfigurationRequestRequestTypeDef,
     GetPercentilesResponseTypeDef,
     GetStatisticsResponseTypeDef,
     ListBillingGroupsResponseTypeDef,
     ListThingGroupsForThingResponseTypeDef,
     ListThingGroupsResponseTypeDef,
     ThingGroupMetadataTypeDef,
     HttpAuthorizationTypeDef,
+    ThingIndexingConfigurationOutputTypeDef,
     ThingIndexingConfigurationTypeDef,
     JobExecutionTypeDef,
     JobExecutionSummaryForJobTypeDef,
     JobExecutionSummaryForThingTypeDef,
+    JobExecutionsRetryConfigOutputTypeDef,
     JobExecutionsRetryConfigTypeDef,
     ListJobsResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     ListManagedJobTemplatesResponseTypeDef,
     ListMitigationActionsResponseTypeDef,
     ListOTAUpdatesResponseTypeDef,
     ListOutgoingCertificatesResponseTypeDef,
@@ -1198,55 +1255,73 @@
     SecurityProfileTargetMappingTypeDef,
     ListThingsResponseTypeDef,
     ListTopicRulesResponseTypeDef,
     LocationActionTypeDef,
     LogTargetConfigurationTypeDef,
     SetV2LoggingLevelRequestRequestTypeDef,
     SetLoggingOptionsRequestRequestTypeDef,
+    MitigationActionParamsOutputTypeDef,
     MitigationActionParamsTypeDef,
+    MqttHeadersOutputTypeDef,
     MqttHeadersTypeDef,
     ResourceIdentifierTypeDef,
-    TestInvokeAuthorizerRequestRequestTypeDef,
     ThingDocumentTypeDef,
+    TimestreamActionOutputTypeDef,
     TimestreamActionTypeDef,
     TopicRuleDestinationConfigurationTypeDef,
     TopicRuleDestinationSummaryTypeDef,
     TopicRuleDestinationTypeDef,
     ValidateSecurityProfileBehaviorsResponseTypeDef,
+    AbortConfigUnionTypeDef,
     ListMetricValuesResponseTypeDef,
     DeniedTypeDef,
+    PutAssetPropertyValueEntryOutputTypeDef,
     PutAssetPropertyValueEntryTypeDef,
     CreateDynamicThingGroupRequestRequestTypeDef,
     CreateThingGroupRequestRequestTypeDef,
+    ThingGroupPropertiesUnionTypeDef,
     UpdateDynamicThingGroupRequestRequestTypeDef,
     UpdateThingGroupRequestRequestTypeDef,
+    TestAuthorizationRequestRequestTypeDef,
     AwsJobExecutionsRolloutConfigTypeDef,
+    BehaviorOutputTypeDef,
     BehaviorTypeDef,
+    CustomCodeSigningTypeDef,
+    TestInvokeAuthorizerRequestRequestTypeDef,
     GetBucketsAggregationRequestRequestTypeDef,
     DescribeCACertificateResponseTypeDef,
     DescribeCertificateResponseTypeDef,
+    StartDetectMitigationActionsTaskRequestRequestTypeDef,
+    ViolationEventOccurrenceRangeUnionTypeDef,
+    SchedulingConfigUnionTypeDef,
     ListThingTypesResponseTypeDef,
     StartSigningJobParameterTypeDef,
     JobExecutionsRolloutConfigTypeDef,
+    ThingGroupIndexingConfigurationUnionTypeDef,
     CreateStreamRequestRequestTypeDef,
     StreamInfoTypeDef,
     UpdateStreamRequestRequestTypeDef,
     DescribeThingGroupResponseTypeDef,
+    HttpActionOutputTypeDef,
     HttpActionTypeDef,
     GetIndexingConfigurationResponseTypeDef,
+    ThingIndexingConfigurationUnionTypeDef,
     UpdateIndexingConfigurationRequestRequestTypeDef,
     DescribeJobExecutionResponseTypeDef,
     ListJobExecutionsForJobResponseTypeDef,
     ListJobExecutionsForThingResponseTypeDef,
+    JobExecutionsRetryConfigUnionTypeDef,
     ListSecurityProfilesForTargetResponseTypeDef,
     ListV2LoggingLevelsResponseTypeDef,
-    CreateMitigationActionRequestRequestTypeDef,
     DescribeMitigationActionResponseTypeDef,
     MitigationActionTypeDef,
+    CreateMitigationActionRequestRequestTypeDef,
+    MitigationActionParamsUnionTypeDef,
     UpdateMitigationActionRequestRequestTypeDef,
+    RepublishActionOutputTypeDef,
     RepublishActionTypeDef,
     AuditSuppressionTypeDef,
     CreateAuditSuppressionRequestRequestTypeDef,
     DeleteAuditSuppressionRequestRequestTypeDef,
     DescribeAuditSuppressionRequestRequestTypeDef,
     DescribeAuditSuppressionResponseTypeDef,
     ListAuditFindingsRequestListAuditFindingsPaginateTypeDef,
@@ -1258,56 +1333,62 @@
     UpdateAuditSuppressionRequestRequestTypeDef,
     SearchIndexResponseTypeDef,
     CreateTopicRuleDestinationRequestRequestTypeDef,
     ListTopicRuleDestinationsResponseTypeDef,
     CreateTopicRuleDestinationResponseTypeDef,
     GetTopicRuleDestinationResponseTypeDef,
     AuthResultTypeDef,
+    IotSiteWiseActionOutputTypeDef,
     IotSiteWiseActionTypeDef,
     ActiveViolationTypeDef,
-    CreateSecurityProfileRequestRequestTypeDef,
     DescribeSecurityProfileResponseTypeDef,
-    UpdateSecurityProfileRequestRequestTypeDef,
     UpdateSecurityProfileResponseTypeDef,
-    ValidateSecurityProfileBehaviorsRequestRequestTypeDef,
     ViolationEventTypeDef,
+    BehaviorUnionTypeDef,
+    CodeSigningOutputTypeDef,
     CodeSigningTypeDef,
     CreateJobRequestRequestTypeDef,
     CreateJobTemplateRequestRequestTypeDef,
     DescribeJobTemplateResponseTypeDef,
     JobTypeDef,
     UpdateJobRequestRequestTypeDef,
     DescribeStreamResponseTypeDef,
     DescribeAuditMitigationActionsTaskResponseTypeDef,
     DetectMitigationActionsTaskSummaryTypeDef,
     ListAuditSuppressionsResponseTypeDef,
     AuditFindingTypeDef,
     ListRelatedResourcesForAuditFindingResponseTypeDef,
     TestAuthorizationResponseTypeDef,
+    ActionOutputTypeDef,
     ActionTypeDef,
     ListActiveViolationsResponseTypeDef,
     ListViolationEventsResponseTypeDef,
+    CreateSecurityProfileRequestRequestTypeDef,
+    UpdateSecurityProfileRequestRequestTypeDef,
+    ValidateSecurityProfileBehaviorsRequestRequestTypeDef,
+    OTAUpdateFileOutputTypeDef,
     OTAUpdateFileTypeDef,
     DescribeJobResponseTypeDef,
     DescribeDetectMitigationActionsTaskResponseTypeDef,
     ListDetectMitigationActionsTasksResponseTypeDef,
     DescribeAuditFindingResponseTypeDef,
     ListAuditFindingsResponseTypeDef,
-    TopicRulePayloadTypeDef,
     TopicRuleTypeDef,
-    CreateOTAUpdateRequestRequestTypeDef,
+    TopicRulePayloadTypeDef,
     OTAUpdateInfoTypeDef,
+    OTAUpdateFileUnionTypeDef,
+    GetTopicRuleResponseTypeDef,
     CreateTopicRuleRequestRequestTypeDef,
     ReplaceTopicRuleRequestRequestTypeDef,
-    GetTopicRuleResponseTypeDef,
     GetOTAUpdateResponseTypeDef,
+    CreateOTAUpdateRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AbortCriteriaTypeDef:
+def get_value() -> AbortCriteriaTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iot-2.5.2/setup.py` & `types-aiobotocore-iot-2.5.2.post1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iot",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_iot"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IoT 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore iot type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore iot type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_iot": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-iot-2.5.2/types_aiobotocore_iot/__init__.py` & `types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-2.5.2/types_aiobotocore_iot/__init__.pyi` & `types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-2.5.2/types_aiobotocore_iot/__main__.py` & `types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoT 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.IoT 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT\nOther"
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

### Comparing `types-aiobotocore-iot-2.5.2/types_aiobotocore_iot/client.py` & `types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("iot") as client:
         client: IoTClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     AuditFrequencyType,
     AuditMitigationActionsExecutionStatusType,
@@ -114,29 +113,29 @@
     ListThingTypesPaginator,
     ListTopicRuleDestinationsPaginator,
     ListTopicRulesPaginator,
     ListV2LoggingLevelsPaginator,
     ListViolationEventsPaginator,
 )
 from .type_defs import (
-    AbortConfigTypeDef,
-    AggregationTypeTypeDef,
+    AbortConfigUnionTypeDef,
+    AggregationTypeUnionTypeDef,
     AlertTargetTypeDef,
     AssociateTargetsWithJobResponseTypeDef,
-    AttributePayloadTypeDef,
+    AttributePayloadUnionTypeDef,
     AuditCheckConfigurationTypeDef,
-    AuditMitigationActionsTaskTargetTypeDef,
+    AuditMitigationActionsTaskTargetUnionTypeDef,
     AuditNotificationTargetTypeDef,
-    AuthInfoTypeDef,
+    AuthInfoUnionTypeDef,
     AuthorizerConfigTypeDef,
     AwsJobAbortConfigTypeDef,
     AwsJobExecutionsRolloutConfigTypeDef,
     AwsJobPresignedUrlConfigTypeDef,
     AwsJobTimeoutConfigTypeDef,
-    BehaviorTypeDef,
+    BehaviorUnionTypeDef,
     BillingGroupPropertiesTypeDef,
     BucketsAggregationTypeTypeDef,
     CancelJobResponseTypeDef,
     ConfigurationTypeDef,
     CreateAuthorizerResponseTypeDef,
     CreateBillingGroupResponseTypeDef,
     CreateCertificateFromCsrResponseTypeDef,
@@ -194,15 +193,15 @@
     DescribeScheduledAuditResponseTypeDef,
     DescribeSecurityProfileResponseTypeDef,
     DescribeStreamResponseTypeDef,
     DescribeThingGroupResponseTypeDef,
     DescribeThingRegistrationTaskResponseTypeDef,
     DescribeThingResponseTypeDef,
     DescribeThingTypeResponseTypeDef,
-    DetectMitigationActionsTaskTargetTypeDef,
+    DetectMitigationActionsTaskTargetUnionTypeDef,
     EmptyResponseMetadataTypeDef,
     GetBehaviorModelTrainingSummariesResponseTypeDef,
     GetBucketsAggregationResponseTypeDef,
     GetCardinalityResponseTypeDef,
     GetEffectivePoliciesResponseTypeDef,
     GetIndexingConfigurationResponseTypeDef,
     GetJobDocumentResponseTypeDef,
@@ -216,15 +215,15 @@
     GetPolicyVersionResponseTypeDef,
     GetRegistrationCodeResponseTypeDef,
     GetStatisticsResponseTypeDef,
     GetTopicRuleDestinationResponseTypeDef,
     GetTopicRuleResponseTypeDef,
     GetV2LoggingOptionsResponseTypeDef,
     HttpContextTypeDef,
-    JobExecutionsRetryConfigTypeDef,
+    JobExecutionsRetryConfigUnionTypeDef,
     JobExecutionsRolloutConfigTypeDef,
     ListActiveViolationsResponseTypeDef,
     ListAttachedPoliciesResponseTypeDef,
     ListAuditFindingsResponseTypeDef,
     ListAuditMitigationActionsExecutionsResponseTypeDef,
     ListAuditMitigationActionsTasksResponseTypeDef,
     ListAuditSuppressionsResponseTypeDef,
@@ -281,41 +280,42 @@
     ListTopicRulesResponseTypeDef,
     ListV2LoggingLevelsResponseTypeDef,
     ListViolationEventsResponseTypeDef,
     LoggingOptionsPayloadTypeDef,
     LogTargetTypeDef,
     MaintenanceWindowTypeDef,
     MetricToRetainTypeDef,
-    MitigationActionParamsTypeDef,
+    MitigationActionParamsUnionTypeDef,
     MqttContextTypeDef,
-    OTAUpdateFileTypeDef,
+    OTAUpdateFileUnionTypeDef,
     PresignedUrlConfigTypeDef,
     ProvisioningHookTypeDef,
     RegisterCACertificateResponseTypeDef,
     RegisterCertificateResponseTypeDef,
     RegisterCertificateWithoutCAResponseTypeDef,
     RegisterThingResponseTypeDef,
     RegistrationConfigTypeDef,
     ResourceIdentifierTypeDef,
-    SchedulingConfigTypeDef,
+    SchedulingConfigUnionTypeDef,
     SearchIndexResponseTypeDef,
     SetDefaultAuthorizerResponseTypeDef,
     StartAuditMitigationActionsTaskResponseTypeDef,
     StartDetectMitigationActionsTaskResponseTypeDef,
     StartOnDemandAuditTaskResponseTypeDef,
     StartThingRegistrationTaskResponseTypeDef,
     StreamFileTypeDef,
     TagTypeDef,
     TestAuthorizationResponseTypeDef,
     TestInvokeAuthorizerResponseTypeDef,
-    ThingGroupIndexingConfigurationTypeDef,
-    ThingGroupPropertiesTypeDef,
-    ThingIndexingConfigurationTypeDef,
-    ThingTypePropertiesTypeDef,
+    ThingGroupIndexingConfigurationUnionTypeDef,
+    ThingGroupPropertiesUnionTypeDef,
+    ThingIndexingConfigurationUnionTypeDef,
+    ThingTypePropertiesUnionTypeDef,
     TimeoutConfigTypeDef,
+    TimestampTypeDef,
     TlsConfigTypeDef,
     TlsContextTypeDef,
     TopicRuleDestinationConfigurationTypeDef,
     TopicRulePayloadTypeDef,
     TransferCertificateResponseTypeDef,
     UpdateAuthorizerResponseTypeDef,
     UpdateBillingGroupResponseTypeDef,
@@ -327,15 +327,15 @@
     UpdateRoleAliasResponseTypeDef,
     UpdateScheduledAuditResponseTypeDef,
     UpdateSecurityProfileResponseTypeDef,
     UpdateStreamResponseTypeDef,
     UpdateThingGroupResponseTypeDef,
     ValidateSecurityProfileBehaviorsResponseTypeDef,
     VersionUpdateByJobsConfigTypeDef,
-    ViolationEventOccurrenceRangeTypeDef,
+    ViolationEventOccurrenceRangeUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -589,15 +589,15 @@
 
     async def create_audit_suppression(
         self,
         *,
         checkName: str,
         resourceIdentifier: ResourceIdentifierTypeDef,
         clientRequestToken: str,
-        expirationDate: Union[datetime, str] = ...,
+        expirationDate: TimestampTypeDef = ...,
         suppressIndefinitely: bool = ...,
         description: str = ...
     ) -> Dict[str, Any]:
         """
         Creates a Device Defender audit suppression.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_audit_suppression)
@@ -701,15 +701,15 @@
         """
 
     async def create_dynamic_thing_group(
         self,
         *,
         thingGroupName: str,
         queryString: str,
-        thingGroupProperties: ThingGroupPropertiesTypeDef = ...,
+        thingGroupProperties: ThingGroupPropertiesUnionTypeDef = ...,
         indexName: str = ...,
         queryVersion: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateDynamicThingGroupResponseTypeDef:
         """
         Creates a dynamic thing group.
 
@@ -718,15 +718,15 @@
         """
 
     async def create_fleet_metric(
         self,
         *,
         metricName: str,
         queryString: str,
-        aggregationType: AggregationTypeTypeDef,
+        aggregationType: AggregationTypeUnionTypeDef,
         period: int,
         aggregationField: str,
         description: str = ...,
         queryVersion: str = ...,
         indexName: str = ...,
         unit: FleetMetricUnitType = ...,
         tags: Sequence[TagTypeDef] = ...
@@ -745,22 +745,22 @@
         targets: Sequence[str],
         documentSource: str = ...,
         document: str = ...,
         description: str = ...,
         presignedUrlConfig: PresignedUrlConfigTypeDef = ...,
         targetSelection: TargetSelectionType = ...,
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
-        abortConfig: AbortConfigTypeDef = ...,
+        abortConfig: AbortConfigUnionTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         namespaceId: str = ...,
         jobTemplateArn: str = ...,
-        jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...,
+        jobExecutionsRetryConfig: JobExecutionsRetryConfigUnionTypeDef = ...,
         documentParameters: Mapping[str, str] = ...,
-        schedulingConfig: SchedulingConfigTypeDef = ...,
+        schedulingConfig: SchedulingConfigUnionTypeDef = ...,
         destinationPackageVersions: Sequence[str] = ...
     ) -> CreateJobResponseTypeDef:
         """
         Creates a job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_job)
@@ -772,18 +772,18 @@
         jobTemplateId: str,
         description: str,
         jobArn: str = ...,
         documentSource: str = ...,
         document: str = ...,
         presignedUrlConfig: PresignedUrlConfigTypeDef = ...,
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
-        abortConfig: AbortConfigTypeDef = ...,
+        abortConfig: AbortConfigUnionTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...,
+        jobExecutionsRetryConfig: JobExecutionsRetryConfigUnionTypeDef = ...,
         maintenanceWindows: Sequence[MaintenanceWindowTypeDef] = ...,
         destinationPackageVersions: Sequence[str] = ...
     ) -> CreateJobTemplateResponseTypeDef:
         """
         Creates a job template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_job_template)
@@ -802,15 +802,15 @@
         """
 
     async def create_mitigation_action(
         self,
         *,
         actionName: str,
         roleArn: str,
-        actionParams: MitigationActionParamsTypeDef,
+        actionParams: MitigationActionParamsUnionTypeDef,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateMitigationActionResponseTypeDef:
         """
         Defines an action that can be applied to audit findings by using
         StartAuditMitigationActionsTask.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_mitigation_action)
@@ -818,15 +818,15 @@
         """
 
     async def create_ota_update(
         self,
         *,
         otaUpdateId: str,
         targets: Sequence[str],
-        files: Sequence[OTAUpdateFileTypeDef],
+        files: Sequence[OTAUpdateFileUnionTypeDef],
         roleArn: str,
         description: str = ...,
         protocols: Sequence[ProtocolType] = ...,
         targetSelection: TargetSelectionType = ...,
         awsJobExecutionsRolloutConfig: AwsJobExecutionsRolloutConfigTypeDef = ...,
         awsJobPresignedUrlConfig: AwsJobPresignedUrlConfigTypeDef = ...,
         awsJobAbortConfig: AwsJobAbortConfigTypeDef = ...,
@@ -965,15 +965,15 @@
         """
 
     async def create_security_profile(
         self,
         *,
         securityProfileName: str,
         securityProfileDescription: str = ...,
-        behaviors: Sequence[BehaviorTypeDef] = ...,
+        behaviors: Sequence[BehaviorUnionTypeDef] = ...,
         alertTargets: Mapping[Literal["SNS"], AlertTargetTypeDef] = ...,
         additionalMetricsToRetain: Sequence[str] = ...,
         additionalMetricsToRetainV2: Sequence[MetricToRetainTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateSecurityProfileResponseTypeDef:
         """
         Creates a Device Defender security profile.
@@ -999,44 +999,44 @@
         """
 
     async def create_thing(
         self,
         *,
         thingName: str,
         thingTypeName: str = ...,
-        attributePayload: AttributePayloadTypeDef = ...,
+        attributePayload: AttributePayloadUnionTypeDef = ...,
         billingGroupName: str = ...
     ) -> CreateThingResponseTypeDef:
         """
         Creates a thing record in the registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_thing)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_thing)
         """
 
     async def create_thing_group(
         self,
         *,
         thingGroupName: str,
         parentGroupName: str = ...,
-        thingGroupProperties: ThingGroupPropertiesTypeDef = ...,
+        thingGroupProperties: ThingGroupPropertiesUnionTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateThingGroupResponseTypeDef:
         """
         Create a thing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_thing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_thing_group)
         """
 
     async def create_thing_type(
         self,
         *,
         thingTypeName: str,
-        thingTypeProperties: ThingTypePropertiesTypeDef = ...,
+        thingTypeProperties: ThingTypePropertiesUnionTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateThingTypeResponseTypeDef:
         """
         Creates a new thing type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_thing_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_thing_type)
@@ -1980,16 +1980,16 @@
         self,
         *,
         taskId: str = ...,
         checkName: str = ...,
         resourceIdentifier: ResourceIdentifierTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         listSuppressedFindings: bool = ...
     ) -> ListAuditFindingsResponseTypeDef:
         """
         Lists the findings (results) of a Device Defender audit or of the audits
         performed during a specified time period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_audit_findings)
@@ -2011,16 +2011,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_audit_mitigation_actions_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_audit_mitigation_actions_executions)
         """
 
     async def list_audit_mitigation_actions_tasks(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         auditTaskId: str = ...,
         findingId: str = ...,
         taskStatus: AuditMitigationActionsTaskStatusType = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListAuditMitigationActionsTasksResponseTypeDef:
         """
@@ -2045,16 +2045,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_audit_suppressions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_audit_suppressions)
         """
 
     async def list_audit_tasks(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         taskType: AuditTaskTypeType = ...,
         taskStatus: AuditTaskStatusType = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> ListAuditTasksResponseTypeDef:
         """
         Lists the Device Defender audits that have been performed during a given time
@@ -2141,32 +2141,32 @@
 
     async def list_detect_mitigation_actions_executions(
         self,
         *,
         taskId: str = ...,
         violationId: str = ...,
         thingName: str = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListDetectMitigationActionsExecutionsResponseTypeDef:
         """
         Lists mitigation actions executions for a Device Defender ML Detect Security
         Profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_detect_mitigation_actions_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_detect_mitigation_actions_executions)
         """
 
     async def list_detect_mitigation_actions_tasks(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListDetectMitigationActionsTasksResponseTypeDef:
         """
         List of Device Defender ML Detect mitigation actions tasks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_detect_mitigation_actions_tasks)
@@ -2285,16 +2285,16 @@
         """
 
     async def list_metric_values(
         self,
         *,
         thingName: str,
         metricName: str,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         dimensionName: str = ...,
         dimensionValueOperator: DimensionValueOperatorType = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListMetricValuesResponseTypeDef:
         """
         Lists the values reported for an IoT Device Defender metric (device-side metric,
@@ -2684,16 +2684,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_v2_logging_levels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_v2_logging_levels)
         """
 
     async def list_violation_events(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         thingName: str = ...,
         securityProfileName: str = ...,
         behaviorCriteriaType: BehaviorCriteriaTypeType = ...,
         listSuppressedAlerts: bool = ...,
         verificationState: VerificationStateType = ...,
         nextToken: str = ...,
         maxResults: int = ...
@@ -2893,33 +2893,33 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#set_v2_logging_options)
         """
 
     async def start_audit_mitigation_actions_task(
         self,
         *,
         taskId: str,
-        target: AuditMitigationActionsTaskTargetTypeDef,
+        target: AuditMitigationActionsTaskTargetUnionTypeDef,
         auditCheckToActionsMapping: Mapping[str, Sequence[str]],
         clientRequestToken: str
     ) -> StartAuditMitigationActionsTaskResponseTypeDef:
         """
         Starts a task that applies a set of mitigation actions to the specified target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.start_audit_mitigation_actions_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#start_audit_mitigation_actions_task)
         """
 
     async def start_detect_mitigation_actions_task(
         self,
         *,
         taskId: str,
-        target: DetectMitigationActionsTaskTargetTypeDef,
+        target: DetectMitigationActionsTaskTargetUnionTypeDef,
         actions: Sequence[str],
         clientRequestToken: str,
-        violationEventOccurrenceRange: ViolationEventOccurrenceRangeTypeDef = ...,
+        violationEventOccurrenceRange: ViolationEventOccurrenceRangeUnionTypeDef = ...,
         includeOnlyActiveViolations: bool = ...,
         includeSuppressedAlerts: bool = ...
     ) -> StartDetectMitigationActionsTaskResponseTypeDef:
         """
         Starts a Device Defender ML Detect mitigation actions task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.start_detect_mitigation_actions_task)
@@ -2961,15 +2961,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#tag_resource)
         """
 
     async def test_authorization(
         self,
         *,
-        authInfos: Sequence[AuthInfoTypeDef],
+        authInfos: Sequence[AuthInfoUnionTypeDef],
         principal: str = ...,
         cognitoIdentityPoolId: str = ...,
         clientId: str = ...,
         policyNamesToAdd: Sequence[str] = ...,
         policyNamesToSkip: Sequence[str] = ...
     ) -> TestAuthorizationResponseTypeDef:
         """
@@ -3033,15 +3033,15 @@
         """
 
     async def update_audit_suppression(
         self,
         *,
         checkName: str,
         resourceIdentifier: ResourceIdentifierTypeDef,
-        expirationDate: Union[datetime, str] = ...,
+        expirationDate: TimestampTypeDef = ...,
         suppressIndefinitely: bool = ...,
         description: str = ...
     ) -> Dict[str, Any]:
         """
         Updates a Device Defender audit suppression.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_audit_suppression)
@@ -3141,15 +3141,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_domain_configuration)
         """
 
     async def update_dynamic_thing_group(
         self,
         *,
         thingGroupName: str,
-        thingGroupProperties: ThingGroupPropertiesTypeDef,
+        thingGroupProperties: ThingGroupPropertiesUnionTypeDef,
         expectedVersion: int = ...,
         indexName: str = ...,
         queryString: str = ...,
         queryVersion: str = ...
     ) -> UpdateDynamicThingGroupResponseTypeDef:
         """
         Updates a dynamic thing group.
@@ -3170,15 +3170,15 @@
 
     async def update_fleet_metric(
         self,
         *,
         metricName: str,
         indexName: str,
         queryString: str = ...,
-        aggregationType: AggregationTypeTypeDef = ...,
+        aggregationType: AggregationTypeUnionTypeDef = ...,
         period: int = ...,
         aggregationField: str = ...,
         description: str = ...,
         queryVersion: str = ...,
         unit: FleetMetricUnitType = ...,
         expectedVersion: int = ...
     ) -> EmptyResponseMetadataTypeDef:
@@ -3188,16 +3188,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_fleet_metric)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_fleet_metric)
         """
 
     async def update_indexing_configuration(
         self,
         *,
-        thingIndexingConfiguration: ThingIndexingConfigurationTypeDef = ...,
-        thingGroupIndexingConfiguration: ThingGroupIndexingConfigurationTypeDef = ...
+        thingIndexingConfiguration: ThingIndexingConfigurationUnionTypeDef = ...,
+        thingGroupIndexingConfiguration: ThingGroupIndexingConfigurationUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the search configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_indexing_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_indexing_configuration)
         """
@@ -3205,32 +3205,32 @@
     async def update_job(
         self,
         *,
         jobId: str,
         description: str = ...,
         presignedUrlConfig: PresignedUrlConfigTypeDef = ...,
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
-        abortConfig: AbortConfigTypeDef = ...,
+        abortConfig: AbortConfigUnionTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         namespaceId: str = ...,
-        jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...
+        jobExecutionsRetryConfig: JobExecutionsRetryConfigUnionTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates supported fields of the specified job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_job)
         """
 
     async def update_mitigation_action(
         self,
         *,
         actionName: str,
         roleArn: str = ...,
-        actionParams: MitigationActionParamsTypeDef = ...
+        actionParams: MitigationActionParamsUnionTypeDef = ...
     ) -> UpdateMitigationActionResponseTypeDef:
         """
         Updates the definition for the specified mitigation action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_mitigation_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_mitigation_action)
         """
@@ -3327,15 +3327,15 @@
         """
 
     async def update_security_profile(
         self,
         *,
         securityProfileName: str,
         securityProfileDescription: str = ...,
-        behaviors: Sequence[BehaviorTypeDef] = ...,
+        behaviors: Sequence[BehaviorUnionTypeDef] = ...,
         alertTargets: Mapping[Literal["SNS"], AlertTargetTypeDef] = ...,
         additionalMetricsToRetain: Sequence[str] = ...,
         additionalMetricsToRetainV2: Sequence[MetricToRetainTypeDef] = ...,
         deleteBehaviors: bool = ...,
         deleteAlertTargets: bool = ...,
         deleteAdditionalMetricsToRetain: bool = ...,
         expectedVersion: int = ...
@@ -3363,30 +3363,30 @@
         """
 
     async def update_thing(
         self,
         *,
         thingName: str,
         thingTypeName: str = ...,
-        attributePayload: AttributePayloadTypeDef = ...,
+        attributePayload: AttributePayloadUnionTypeDef = ...,
         expectedVersion: int = ...,
         removeThingType: bool = ...
     ) -> Dict[str, Any]:
         """
         Updates the data for a thing.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_thing)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_thing)
         """
 
     async def update_thing_group(
         self,
         *,
         thingGroupName: str,
-        thingGroupProperties: ThingGroupPropertiesTypeDef,
+        thingGroupProperties: ThingGroupPropertiesUnionTypeDef,
         expectedVersion: int = ...
     ) -> UpdateThingGroupResponseTypeDef:
         """
         Update a thing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_thing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_thing_group)
@@ -3414,15 +3414,15 @@
         Updates a topic rule destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_topic_rule_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_topic_rule_destination)
         """
 
     async def validate_security_profile_behaviors(
-        self, *, behaviors: Sequence[BehaviorTypeDef]
+        self, *, behaviors: Sequence[BehaviorUnionTypeDef]
     ) -> ValidateSecurityProfileBehaviorsResponseTypeDef:
         """
         Validates a Device Defender security profile behaviors specification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.validate_security_profile_behaviors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#validate_security_profile_behaviors)
         """
```

### Comparing `types-aiobotocore-iot-2.5.2/types_aiobotocore_iot/client.pyi` & `types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("iot") as client:
         client: IoTClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     AuditFrequencyType,
     AuditMitigationActionsExecutionStatusType,
@@ -114,29 +113,29 @@
     ListThingTypesPaginator,
     ListTopicRuleDestinationsPaginator,
     ListTopicRulesPaginator,
     ListV2LoggingLevelsPaginator,
     ListViolationEventsPaginator,
 )
 from .type_defs import (
-    AbortConfigTypeDef,
-    AggregationTypeTypeDef,
+    AbortConfigUnionTypeDef,
+    AggregationTypeUnionTypeDef,
     AlertTargetTypeDef,
     AssociateTargetsWithJobResponseTypeDef,
-    AttributePayloadTypeDef,
+    AttributePayloadUnionTypeDef,
     AuditCheckConfigurationTypeDef,
-    AuditMitigationActionsTaskTargetTypeDef,
+    AuditMitigationActionsTaskTargetUnionTypeDef,
     AuditNotificationTargetTypeDef,
-    AuthInfoTypeDef,
+    AuthInfoUnionTypeDef,
     AuthorizerConfigTypeDef,
     AwsJobAbortConfigTypeDef,
     AwsJobExecutionsRolloutConfigTypeDef,
     AwsJobPresignedUrlConfigTypeDef,
     AwsJobTimeoutConfigTypeDef,
-    BehaviorTypeDef,
+    BehaviorUnionTypeDef,
     BillingGroupPropertiesTypeDef,
     BucketsAggregationTypeTypeDef,
     CancelJobResponseTypeDef,
     ConfigurationTypeDef,
     CreateAuthorizerResponseTypeDef,
     CreateBillingGroupResponseTypeDef,
     CreateCertificateFromCsrResponseTypeDef,
@@ -194,15 +193,15 @@
     DescribeScheduledAuditResponseTypeDef,
     DescribeSecurityProfileResponseTypeDef,
     DescribeStreamResponseTypeDef,
     DescribeThingGroupResponseTypeDef,
     DescribeThingRegistrationTaskResponseTypeDef,
     DescribeThingResponseTypeDef,
     DescribeThingTypeResponseTypeDef,
-    DetectMitigationActionsTaskTargetTypeDef,
+    DetectMitigationActionsTaskTargetUnionTypeDef,
     EmptyResponseMetadataTypeDef,
     GetBehaviorModelTrainingSummariesResponseTypeDef,
     GetBucketsAggregationResponseTypeDef,
     GetCardinalityResponseTypeDef,
     GetEffectivePoliciesResponseTypeDef,
     GetIndexingConfigurationResponseTypeDef,
     GetJobDocumentResponseTypeDef,
@@ -216,15 +215,15 @@
     GetPolicyVersionResponseTypeDef,
     GetRegistrationCodeResponseTypeDef,
     GetStatisticsResponseTypeDef,
     GetTopicRuleDestinationResponseTypeDef,
     GetTopicRuleResponseTypeDef,
     GetV2LoggingOptionsResponseTypeDef,
     HttpContextTypeDef,
-    JobExecutionsRetryConfigTypeDef,
+    JobExecutionsRetryConfigUnionTypeDef,
     JobExecutionsRolloutConfigTypeDef,
     ListActiveViolationsResponseTypeDef,
     ListAttachedPoliciesResponseTypeDef,
     ListAuditFindingsResponseTypeDef,
     ListAuditMitigationActionsExecutionsResponseTypeDef,
     ListAuditMitigationActionsTasksResponseTypeDef,
     ListAuditSuppressionsResponseTypeDef,
@@ -281,41 +280,42 @@
     ListTopicRulesResponseTypeDef,
     ListV2LoggingLevelsResponseTypeDef,
     ListViolationEventsResponseTypeDef,
     LoggingOptionsPayloadTypeDef,
     LogTargetTypeDef,
     MaintenanceWindowTypeDef,
     MetricToRetainTypeDef,
-    MitigationActionParamsTypeDef,
+    MitigationActionParamsUnionTypeDef,
     MqttContextTypeDef,
-    OTAUpdateFileTypeDef,
+    OTAUpdateFileUnionTypeDef,
     PresignedUrlConfigTypeDef,
     ProvisioningHookTypeDef,
     RegisterCACertificateResponseTypeDef,
     RegisterCertificateResponseTypeDef,
     RegisterCertificateWithoutCAResponseTypeDef,
     RegisterThingResponseTypeDef,
     RegistrationConfigTypeDef,
     ResourceIdentifierTypeDef,
-    SchedulingConfigTypeDef,
+    SchedulingConfigUnionTypeDef,
     SearchIndexResponseTypeDef,
     SetDefaultAuthorizerResponseTypeDef,
     StartAuditMitigationActionsTaskResponseTypeDef,
     StartDetectMitigationActionsTaskResponseTypeDef,
     StartOnDemandAuditTaskResponseTypeDef,
     StartThingRegistrationTaskResponseTypeDef,
     StreamFileTypeDef,
     TagTypeDef,
     TestAuthorizationResponseTypeDef,
     TestInvokeAuthorizerResponseTypeDef,
-    ThingGroupIndexingConfigurationTypeDef,
-    ThingGroupPropertiesTypeDef,
-    ThingIndexingConfigurationTypeDef,
-    ThingTypePropertiesTypeDef,
+    ThingGroupIndexingConfigurationUnionTypeDef,
+    ThingGroupPropertiesUnionTypeDef,
+    ThingIndexingConfigurationUnionTypeDef,
+    ThingTypePropertiesUnionTypeDef,
     TimeoutConfigTypeDef,
+    TimestampTypeDef,
     TlsConfigTypeDef,
     TlsContextTypeDef,
     TopicRuleDestinationConfigurationTypeDef,
     TopicRulePayloadTypeDef,
     TransferCertificateResponseTypeDef,
     UpdateAuthorizerResponseTypeDef,
     UpdateBillingGroupResponseTypeDef,
@@ -327,15 +327,15 @@
     UpdateRoleAliasResponseTypeDef,
     UpdateScheduledAuditResponseTypeDef,
     UpdateSecurityProfileResponseTypeDef,
     UpdateStreamResponseTypeDef,
     UpdateThingGroupResponseTypeDef,
     ValidateSecurityProfileBehaviorsResponseTypeDef,
     VersionUpdateByJobsConfigTypeDef,
-    ViolationEventOccurrenceRangeTypeDef,
+    ViolationEventOccurrenceRangeUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -566,15 +566,15 @@
         """
     async def create_audit_suppression(
         self,
         *,
         checkName: str,
         resourceIdentifier: ResourceIdentifierTypeDef,
         clientRequestToken: str,
-        expirationDate: Union[datetime, str] = ...,
+        expirationDate: TimestampTypeDef = ...,
         suppressIndefinitely: bool = ...,
         description: str = ...
     ) -> Dict[str, Any]:
         """
         Creates a Device Defender audit suppression.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_audit_suppression)
@@ -671,15 +671,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_domain_configuration)
         """
     async def create_dynamic_thing_group(
         self,
         *,
         thingGroupName: str,
         queryString: str,
-        thingGroupProperties: ThingGroupPropertiesTypeDef = ...,
+        thingGroupProperties: ThingGroupPropertiesUnionTypeDef = ...,
         indexName: str = ...,
         queryVersion: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateDynamicThingGroupResponseTypeDef:
         """
         Creates a dynamic thing group.
 
@@ -687,15 +687,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_dynamic_thing_group)
         """
     async def create_fleet_metric(
         self,
         *,
         metricName: str,
         queryString: str,
-        aggregationType: AggregationTypeTypeDef,
+        aggregationType: AggregationTypeUnionTypeDef,
         period: int,
         aggregationField: str,
         description: str = ...,
         queryVersion: str = ...,
         indexName: str = ...,
         unit: FleetMetricUnitType = ...,
         tags: Sequence[TagTypeDef] = ...
@@ -713,22 +713,22 @@
         targets: Sequence[str],
         documentSource: str = ...,
         document: str = ...,
         description: str = ...,
         presignedUrlConfig: PresignedUrlConfigTypeDef = ...,
         targetSelection: TargetSelectionType = ...,
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
-        abortConfig: AbortConfigTypeDef = ...,
+        abortConfig: AbortConfigUnionTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         namespaceId: str = ...,
         jobTemplateArn: str = ...,
-        jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...,
+        jobExecutionsRetryConfig: JobExecutionsRetryConfigUnionTypeDef = ...,
         documentParameters: Mapping[str, str] = ...,
-        schedulingConfig: SchedulingConfigTypeDef = ...,
+        schedulingConfig: SchedulingConfigUnionTypeDef = ...,
         destinationPackageVersions: Sequence[str] = ...
     ) -> CreateJobResponseTypeDef:
         """
         Creates a job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_job)
@@ -739,18 +739,18 @@
         jobTemplateId: str,
         description: str,
         jobArn: str = ...,
         documentSource: str = ...,
         document: str = ...,
         presignedUrlConfig: PresignedUrlConfigTypeDef = ...,
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
-        abortConfig: AbortConfigTypeDef = ...,
+        abortConfig: AbortConfigUnionTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...,
+        jobExecutionsRetryConfig: JobExecutionsRetryConfigUnionTypeDef = ...,
         maintenanceWindows: Sequence[MaintenanceWindowTypeDef] = ...,
         destinationPackageVersions: Sequence[str] = ...
     ) -> CreateJobTemplateResponseTypeDef:
         """
         Creates a job template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_job_template)
@@ -767,30 +767,30 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_keys_and_certificate)
         """
     async def create_mitigation_action(
         self,
         *,
         actionName: str,
         roleArn: str,
-        actionParams: MitigationActionParamsTypeDef,
+        actionParams: MitigationActionParamsUnionTypeDef,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateMitigationActionResponseTypeDef:
         """
         Defines an action that can be applied to audit findings by using
         StartAuditMitigationActionsTask.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_mitigation_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_mitigation_action)
         """
     async def create_ota_update(
         self,
         *,
         otaUpdateId: str,
         targets: Sequence[str],
-        files: Sequence[OTAUpdateFileTypeDef],
+        files: Sequence[OTAUpdateFileUnionTypeDef],
         roleArn: str,
         description: str = ...,
         protocols: Sequence[ProtocolType] = ...,
         targetSelection: TargetSelectionType = ...,
         awsJobExecutionsRolloutConfig: AwsJobExecutionsRolloutConfigTypeDef = ...,
         awsJobPresignedUrlConfig: AwsJobPresignedUrlConfigTypeDef = ...,
         awsJobAbortConfig: AwsJobAbortConfigTypeDef = ...,
@@ -919,15 +919,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_scheduled_audit)
         """
     async def create_security_profile(
         self,
         *,
         securityProfileName: str,
         securityProfileDescription: str = ...,
-        behaviors: Sequence[BehaviorTypeDef] = ...,
+        behaviors: Sequence[BehaviorUnionTypeDef] = ...,
         alertTargets: Mapping[Literal["SNS"], AlertTargetTypeDef] = ...,
         additionalMetricsToRetain: Sequence[str] = ...,
         additionalMetricsToRetainV2: Sequence[MetricToRetainTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateSecurityProfileResponseTypeDef:
         """
         Creates a Device Defender security profile.
@@ -951,42 +951,42 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_stream)
         """
     async def create_thing(
         self,
         *,
         thingName: str,
         thingTypeName: str = ...,
-        attributePayload: AttributePayloadTypeDef = ...,
+        attributePayload: AttributePayloadUnionTypeDef = ...,
         billingGroupName: str = ...
     ) -> CreateThingResponseTypeDef:
         """
         Creates a thing record in the registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_thing)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_thing)
         """
     async def create_thing_group(
         self,
         *,
         thingGroupName: str,
         parentGroupName: str = ...,
-        thingGroupProperties: ThingGroupPropertiesTypeDef = ...,
+        thingGroupProperties: ThingGroupPropertiesUnionTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateThingGroupResponseTypeDef:
         """
         Create a thing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_thing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_thing_group)
         """
     async def create_thing_type(
         self,
         *,
         thingTypeName: str,
-        thingTypeProperties: ThingTypePropertiesTypeDef = ...,
+        thingTypeProperties: ThingTypePropertiesUnionTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateThingTypeResponseTypeDef:
         """
         Creates a new thing type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_thing_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_thing_type)
@@ -1832,16 +1832,16 @@
         self,
         *,
         taskId: str = ...,
         checkName: str = ...,
         resourceIdentifier: ResourceIdentifierTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         listSuppressedFindings: bool = ...
     ) -> ListAuditFindingsResponseTypeDef:
         """
         Lists the findings (results) of a Device Defender audit or of the audits
         performed during a specified time period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_audit_findings)
@@ -1861,16 +1861,16 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_audit_mitigation_actions_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_audit_mitigation_actions_executions)
         """
     async def list_audit_mitigation_actions_tasks(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         auditTaskId: str = ...,
         findingId: str = ...,
         taskStatus: AuditMitigationActionsTaskStatusType = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListAuditMitigationActionsTasksResponseTypeDef:
         """
@@ -1893,16 +1893,16 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_audit_suppressions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_audit_suppressions)
         """
     async def list_audit_tasks(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         taskType: AuditTaskTypeType = ...,
         taskStatus: AuditTaskStatusType = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> ListAuditTasksResponseTypeDef:
         """
         Lists the Device Defender audits that have been performed during a given time
@@ -1982,31 +1982,31 @@
         """
     async def list_detect_mitigation_actions_executions(
         self,
         *,
         taskId: str = ...,
         violationId: str = ...,
         thingName: str = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListDetectMitigationActionsExecutionsResponseTypeDef:
         """
         Lists mitigation actions executions for a Device Defender ML Detect Security
         Profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_detect_mitigation_actions_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_detect_mitigation_actions_executions)
         """
     async def list_detect_mitigation_actions_tasks(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListDetectMitigationActionsTasksResponseTypeDef:
         """
         List of Device Defender ML Detect mitigation actions tasks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_detect_mitigation_actions_tasks)
@@ -2115,16 +2115,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_managed_job_templates)
         """
     async def list_metric_values(
         self,
         *,
         thingName: str,
         metricName: str,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         dimensionName: str = ...,
         dimensionValueOperator: DimensionValueOperatorType = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListMetricValuesResponseTypeDef:
         """
         Lists the values reported for an IoT Device Defender metric (device-side metric,
@@ -2480,16 +2480,16 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.list_v2_logging_levels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#list_v2_logging_levels)
         """
     async def list_violation_events(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         thingName: str = ...,
         securityProfileName: str = ...,
         behaviorCriteriaType: BehaviorCriteriaTypeType = ...,
         listSuppressedAlerts: bool = ...,
         verificationState: VerificationStateType = ...,
         nextToken: str = ...,
         maxResults: int = ...
@@ -2673,32 +2673,32 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.set_v2_logging_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#set_v2_logging_options)
         """
     async def start_audit_mitigation_actions_task(
         self,
         *,
         taskId: str,
-        target: AuditMitigationActionsTaskTargetTypeDef,
+        target: AuditMitigationActionsTaskTargetUnionTypeDef,
         auditCheckToActionsMapping: Mapping[str, Sequence[str]],
         clientRequestToken: str
     ) -> StartAuditMitigationActionsTaskResponseTypeDef:
         """
         Starts a task that applies a set of mitigation actions to the specified target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.start_audit_mitigation_actions_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#start_audit_mitigation_actions_task)
         """
     async def start_detect_mitigation_actions_task(
         self,
         *,
         taskId: str,
-        target: DetectMitigationActionsTaskTargetTypeDef,
+        target: DetectMitigationActionsTaskTargetUnionTypeDef,
         actions: Sequence[str],
         clientRequestToken: str,
-        violationEventOccurrenceRange: ViolationEventOccurrenceRangeTypeDef = ...,
+        violationEventOccurrenceRange: ViolationEventOccurrenceRangeUnionTypeDef = ...,
         includeOnlyActiveViolations: bool = ...,
         includeSuppressedAlerts: bool = ...
     ) -> StartDetectMitigationActionsTaskResponseTypeDef:
         """
         Starts a Device Defender ML Detect mitigation actions task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.start_detect_mitigation_actions_task)
@@ -2735,15 +2735,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#tag_resource)
         """
     async def test_authorization(
         self,
         *,
-        authInfos: Sequence[AuthInfoTypeDef],
+        authInfos: Sequence[AuthInfoUnionTypeDef],
         principal: str = ...,
         cognitoIdentityPoolId: str = ...,
         clientId: str = ...,
         policyNamesToAdd: Sequence[str] = ...,
         policyNamesToSkip: Sequence[str] = ...
     ) -> TestAuthorizationResponseTypeDef:
         """
@@ -2802,15 +2802,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_account_audit_configuration)
         """
     async def update_audit_suppression(
         self,
         *,
         checkName: str,
         resourceIdentifier: ResourceIdentifierTypeDef,
-        expirationDate: Union[datetime, str] = ...,
+        expirationDate: TimestampTypeDef = ...,
         suppressIndefinitely: bool = ...,
         description: str = ...
     ) -> Dict[str, Any]:
         """
         Updates a Device Defender audit suppression.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_audit_suppression)
@@ -2902,15 +2902,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_domain_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_domain_configuration)
         """
     async def update_dynamic_thing_group(
         self,
         *,
         thingGroupName: str,
-        thingGroupProperties: ThingGroupPropertiesTypeDef,
+        thingGroupProperties: ThingGroupPropertiesUnionTypeDef,
         expectedVersion: int = ...,
         indexName: str = ...,
         queryString: str = ...,
         queryVersion: str = ...
     ) -> UpdateDynamicThingGroupResponseTypeDef:
         """
         Updates a dynamic thing group.
@@ -2929,15 +2929,15 @@
         """
     async def update_fleet_metric(
         self,
         *,
         metricName: str,
         indexName: str,
         queryString: str = ...,
-        aggregationType: AggregationTypeTypeDef = ...,
+        aggregationType: AggregationTypeUnionTypeDef = ...,
         period: int = ...,
         aggregationField: str = ...,
         description: str = ...,
         queryVersion: str = ...,
         unit: FleetMetricUnitType = ...,
         expectedVersion: int = ...
     ) -> EmptyResponseMetadataTypeDef:
@@ -2946,47 +2946,47 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_fleet_metric)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_fleet_metric)
         """
     async def update_indexing_configuration(
         self,
         *,
-        thingIndexingConfiguration: ThingIndexingConfigurationTypeDef = ...,
-        thingGroupIndexingConfiguration: ThingGroupIndexingConfigurationTypeDef = ...
+        thingIndexingConfiguration: ThingIndexingConfigurationUnionTypeDef = ...,
+        thingGroupIndexingConfiguration: ThingGroupIndexingConfigurationUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the search configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_indexing_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_indexing_configuration)
         """
     async def update_job(
         self,
         *,
         jobId: str,
         description: str = ...,
         presignedUrlConfig: PresignedUrlConfigTypeDef = ...,
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
-        abortConfig: AbortConfigTypeDef = ...,
+        abortConfig: AbortConfigUnionTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         namespaceId: str = ...,
-        jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...
+        jobExecutionsRetryConfig: JobExecutionsRetryConfigUnionTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates supported fields of the specified job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_job)
         """
     async def update_mitigation_action(
         self,
         *,
         actionName: str,
         roleArn: str = ...,
-        actionParams: MitigationActionParamsTypeDef = ...
+        actionParams: MitigationActionParamsUnionTypeDef = ...
     ) -> UpdateMitigationActionResponseTypeDef:
         """
         Updates the definition for the specified mitigation action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_mitigation_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_mitigation_action)
         """
@@ -3076,15 +3076,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_scheduled_audit)
         """
     async def update_security_profile(
         self,
         *,
         securityProfileName: str,
         securityProfileDescription: str = ...,
-        behaviors: Sequence[BehaviorTypeDef] = ...,
+        behaviors: Sequence[BehaviorUnionTypeDef] = ...,
         alertTargets: Mapping[Literal["SNS"], AlertTargetTypeDef] = ...,
         additionalMetricsToRetain: Sequence[str] = ...,
         additionalMetricsToRetainV2: Sequence[MetricToRetainTypeDef] = ...,
         deleteBehaviors: bool = ...,
         deleteAlertTargets: bool = ...,
         deleteAdditionalMetricsToRetain: bool = ...,
         expectedVersion: int = ...
@@ -3110,29 +3110,29 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_stream)
         """
     async def update_thing(
         self,
         *,
         thingName: str,
         thingTypeName: str = ...,
-        attributePayload: AttributePayloadTypeDef = ...,
+        attributePayload: AttributePayloadUnionTypeDef = ...,
         expectedVersion: int = ...,
         removeThingType: bool = ...
     ) -> Dict[str, Any]:
         """
         Updates the data for a thing.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_thing)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_thing)
         """
     async def update_thing_group(
         self,
         *,
         thingGroupName: str,
-        thingGroupProperties: ThingGroupPropertiesTypeDef,
+        thingGroupProperties: ThingGroupPropertiesUnionTypeDef,
         expectedVersion: int = ...
     ) -> UpdateThingGroupResponseTypeDef:
         """
         Update a thing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_thing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_thing_group)
@@ -3157,15 +3157,15 @@
         """
         Updates a topic rule destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_topic_rule_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_topic_rule_destination)
         """
     async def validate_security_profile_behaviors(
-        self, *, behaviors: Sequence[BehaviorTypeDef]
+        self, *, behaviors: Sequence[BehaviorUnionTypeDef]
     ) -> ValidateSecurityProfileBehaviorsResponseTypeDef:
         """
         Validates a Device Defender security profile behaviors specification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.validate_security_profile_behaviors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#validate_security_profile_behaviors)
         """
```

### Comparing `types-aiobotocore-iot-2.5.2/types_aiobotocore_iot/literals.py` & `types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-2.5.2/types_aiobotocore_iot/literals.pyi` & `types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-2.5.2/types_aiobotocore_iot/paginator.py` & `types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,16 +132,15 @@
         list_things_in_thing_group_paginator: ListThingsInThingGroupPaginator = client.get_paginator("list_things_in_thing_group")
         list_topic_rule_destinations_paginator: ListTopicRuleDestinationsPaginator = client.get_paginator("list_topic_rule_destinations")
         list_topic_rules_paginator: ListTopicRulesPaginator = client.get_paginator("list_topic_rules")
         list_v2_logging_levels_paginator: ListV2LoggingLevelsPaginator = client.get_paginator("list_v2_logging_levels")
         list_violation_events_paginator: ListViolationEventsPaginator = client.get_paginator("list_violation_events")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import (
     AuditMitigationActionsExecutionStatusType,
     AuditMitigationActionsTaskStatusType,
@@ -220,14 +219,15 @@
     ListThingTypesResponseTypeDef,
     ListTopicRuleDestinationsResponseTypeDef,
     ListTopicRulesResponseTypeDef,
     ListV2LoggingLevelsResponseTypeDef,
     ListViolationEventsResponseTypeDef,
     PaginatorConfigTypeDef,
     ResourceIdentifierTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "GetBehaviorModelTrainingSummariesPaginator",
     "ListActiveViolationsPaginator",
     "ListAttachedPoliciesPaginator",
     "ListAuditFindingsPaginator",
@@ -302,15 +302,15 @@
 class GetBehaviorModelTrainingSummariesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.GetBehaviorModelTrainingSummaries)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#getbehaviormodeltrainingsummariespaginator)
     """
 
     def paginate(
-        self, *, securityProfileName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, securityProfileName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetBehaviorModelTrainingSummariesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.GetBehaviorModelTrainingSummaries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#getbehaviormodeltrainingsummariespaginator)
         """
 
 
@@ -324,34 +324,30 @@
         self,
         *,
         thingName: str = ...,
         securityProfileName: str = ...,
         behaviorCriteriaType: BehaviorCriteriaTypeType = ...,
         listSuppressedAlerts: bool = ...,
         verificationState: VerificationStateType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListActiveViolationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListActiveViolations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listactiveviolationspaginator)
         """
 
 
 class ListAttachedPoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAttachedPolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listattachedpoliciespaginator)
     """
 
     def paginate(
-        self,
-        *,
-        target: str,
-        recursive: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, target: str, recursive: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAttachedPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAttachedPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listattachedpoliciespaginator)
         """
 
 
@@ -363,18 +359,18 @@
 
     def paginate(
         self,
         *,
         taskId: str = ...,
         checkName: str = ...,
         resourceIdentifier: ResourceIdentifierTypeDef = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         listSuppressedFindings: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAuditFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listauditfindingspaginator)
         """
 
 
@@ -386,15 +382,15 @@
 
     def paginate(
         self,
         *,
         taskId: str,
         findingId: str,
         actionStatus: AuditMitigationActionsExecutionStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAuditMitigationActionsExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditMitigationActionsExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listauditmitigationactionsexecutionspaginator)
         """
 
 
@@ -403,20 +399,20 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditMitigationActionsTasks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listauditmitigationactionstaskspaginator)
     """
 
     def paginate(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         auditTaskId: str = ...,
         findingId: str = ...,
         taskStatus: AuditMitigationActionsTaskStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAuditMitigationActionsTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditMitigationActionsTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listauditmitigationactionstaskspaginator)
         """
 
 
@@ -428,15 +424,15 @@
 
     def paginate(
         self,
         *,
         checkName: str = ...,
         resourceIdentifier: ResourceIdentifierTypeDef = ...,
         ascendingOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAuditSuppressionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditSuppressions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listauditsuppressionspaginator)
         """
 
 
@@ -445,19 +441,19 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditTasks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listaudittaskspaginator)
     """
 
     def paginate(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         taskType: AuditTaskTypeType = ...,
         taskStatus: AuditTaskStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAuditTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listaudittaskspaginator)
         """
 
 
@@ -468,30 +464,30 @@
     """
 
     def paginate(
         self,
         *,
         ascendingOrder: bool = ...,
         status: AuthorizerStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAuthorizersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuthorizers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listauthorizerspaginator)
         """
 
 
 class ListBillingGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListBillingGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listbillinggroupspaginator)
     """
 
     def paginate(
-        self, *, namePrefixFilter: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, namePrefixFilter: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBillingGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListBillingGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listbillinggroupspaginator)
         """
 
 
@@ -502,30 +498,30 @@
     """
 
     def paginate(
         self,
         *,
         ascendingOrder: bool = ...,
         templateName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCACertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCACertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listcacertificatespaginator)
         """
 
 
 class ListCertificatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCertificates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listcertificatespaginator)
     """
 
     def paginate(
-        self, *, ascendingOrder: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ascendingOrder: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listcertificatespaginator)
         """
 
 
@@ -536,30 +532,30 @@
     """
 
     def paginate(
         self,
         *,
         caCertificateId: str,
         ascendingOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCertificatesByCAResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCertificatesByCA.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listcertificatesbycapaginator)
         """
 
 
 class ListCustomMetricsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCustomMetrics)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listcustommetricspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCustomMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCustomMetrics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listcustommetricspaginator)
         """
 
 
@@ -571,17 +567,17 @@
 
     def paginate(
         self,
         *,
         taskId: str = ...,
         violationId: str = ...,
         thingName: str = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDetectMitigationActionsExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDetectMitigationActionsExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listdetectmitigationactionsexecutionspaginator)
         """
 
 
@@ -590,80 +586,77 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDetectMitigationActionsTasks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listdetectmitigationactionstaskspaginator)
     """
 
     def paginate(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDetectMitigationActionsTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDetectMitigationActionsTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listdetectmitigationactionstaskspaginator)
         """
 
 
 class ListDimensionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDimensions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listdimensionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDimensionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDimensions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listdimensionspaginator)
         """
 
 
 class ListDomainConfigurationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDomainConfigurations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listdomainconfigurationspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        serviceType: ServiceTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, serviceType: ServiceTypeType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDomainConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDomainConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listdomainconfigurationspaginator)
         """
 
 
 class ListFleetMetricsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListFleetMetrics)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listfleetmetricspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFleetMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListFleetMetrics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listfleetmetricspaginator)
         """
 
 
 class ListIndicesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListIndices)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listindicespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListIndicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListIndices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listindicespaginator)
         """
 
 
@@ -674,15 +667,15 @@
     """
 
     def paginate(
         self,
         *,
         jobId: str,
         status: JobExecutionStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListJobExecutionsForJobResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobExecutionsForJob.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listjobexecutionsforjobpaginator)
         """
 
 
@@ -695,30 +688,30 @@
     def paginate(
         self,
         *,
         thingName: str,
         status: JobExecutionStatusType = ...,
         namespaceId: str = ...,
         jobId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListJobExecutionsForThingResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobExecutionsForThing.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listjobexecutionsforthingpaginator)
         """
 
 
 class ListJobTemplatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobTemplates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listjobtemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListJobTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listjobtemplatespaginator)
         """
 
 
@@ -732,30 +725,30 @@
         self,
         *,
         status: JobStatusType = ...,
         targetSelection: TargetSelectionType = ...,
         thingGroupName: str = ...,
         thingGroupId: str = ...,
         namespaceId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listjobspaginator)
         """
 
 
 class ListManagedJobTemplatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListManagedJobTemplates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listmanagedjobtemplatespaginator)
     """
 
     def paginate(
-        self, *, templateName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, templateName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListManagedJobTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListManagedJobTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listmanagedjobtemplatespaginator)
         """
 
 
@@ -766,19 +759,19 @@
     """
 
     def paginate(
         self,
         *,
         thingName: str,
         metricName: str,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         dimensionName: str = ...,
         dimensionValueOperator: DimensionValueOperatorType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMetricValuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListMetricValues.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listmetricvaluespaginator)
         """
 
 
@@ -788,15 +781,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listmitigationactionspaginator)
     """
 
     def paginate(
         self,
         *,
         actionType: MitigationActionTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMitigationActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListMitigationActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listmitigationactionspaginator)
         """
 
 
@@ -806,30 +799,30 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listotaupdatespaginator)
     """
 
     def paginate(
         self,
         *,
         otaUpdateStatus: OTAUpdateStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListOTAUpdatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListOTAUpdates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listotaupdatespaginator)
         """
 
 
 class ListOutgoingCertificatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListOutgoingCertificates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listoutgoingcertificatespaginator)
     """
 
     def paginate(
-        self, *, ascendingOrder: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ascendingOrder: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListOutgoingCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListOutgoingCertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listoutgoingcertificatespaginator)
         """
 
 
@@ -840,45 +833,45 @@
     """
 
     def paginate(
         self,
         *,
         packageName: str,
         status: PackageVersionStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPackageVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPackageVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listpackageversionspaginator)
         """
 
 
 class ListPackagesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPackages)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listpackagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPackagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPackages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listpackagespaginator)
         """
 
 
 class ListPoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listpoliciespaginator)
     """
 
     def paginate(
-        self, *, ascendingOrder: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ascendingOrder: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listpoliciespaginator)
         """
 
 
@@ -889,15 +882,15 @@
     """
 
     def paginate(
         self,
         *,
         policyName: str,
         ascendingOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPolicyPrincipalsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPolicyPrincipals.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listpolicyprincipalspaginator)
         """
 
 
@@ -908,105 +901,105 @@
     """
 
     def paginate(
         self,
         *,
         principal: str,
         ascendingOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPrincipalPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPrincipalPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listprincipalpoliciespaginator)
         """
 
 
 class ListPrincipalThingsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPrincipalThings)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listprincipalthingspaginator)
     """
 
     def paginate(
-        self, *, principal: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, principal: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPrincipalThingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPrincipalThings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listprincipalthingspaginator)
         """
 
 
 class ListProvisioningTemplateVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListProvisioningTemplateVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listprovisioningtemplateversionspaginator)
     """
 
     def paginate(
-        self, *, templateName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, templateName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProvisioningTemplateVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListProvisioningTemplateVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listprovisioningtemplateversionspaginator)
         """
 
 
 class ListProvisioningTemplatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListProvisioningTemplates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listprovisioningtemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProvisioningTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListProvisioningTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listprovisioningtemplatespaginator)
         """
 
 
 class ListRelatedResourcesForAuditFindingPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListRelatedResourcesForAuditFinding)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listrelatedresourcesforauditfindingpaginator)
     """
 
     def paginate(
-        self, *, findingId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, findingId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRelatedResourcesForAuditFindingResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListRelatedResourcesForAuditFinding.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listrelatedresourcesforauditfindingpaginator)
         """
 
 
 class ListRoleAliasesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListRoleAliases)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listrolealiasespaginator)
     """
 
     def paginate(
-        self, *, ascendingOrder: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ascendingOrder: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRoleAliasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListRoleAliases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listrolealiasespaginator)
         """
 
 
 class ListScheduledAuditsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListScheduledAudits)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listscheduledauditspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListScheduledAuditsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListScheduledAudits.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listscheduledauditspaginator)
         """
 
 
@@ -1017,15 +1010,15 @@
     """
 
     def paginate(
         self,
         *,
         dimensionName: str = ...,
         metricName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSecurityProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListSecurityProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listsecurityprofilespaginator)
         """
 
 
@@ -1036,75 +1029,75 @@
     """
 
     def paginate(
         self,
         *,
         securityProfileTargetArn: str,
         recursive: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSecurityProfilesForTargetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListSecurityProfilesForTarget.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listsecurityprofilesfortargetpaginator)
         """
 
 
 class ListStreamsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListStreams)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#liststreamspaginator)
     """
 
     def paginate(
-        self, *, ascendingOrder: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ascendingOrder: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStreamsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListStreams.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#liststreamspaginator)
         """
 
 
 class ListTagsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTagsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTagsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listtagsforresourcepaginator)
         """
 
 
 class ListTargetsForPolicyPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTargetsForPolicy)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listtargetsforpolicypaginator)
     """
 
     def paginate(
-        self, *, policyName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, policyName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTargetsForPolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTargetsForPolicy.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listtargetsforpolicypaginator)
         """
 
 
 class ListTargetsForSecurityProfilePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTargetsForSecurityProfile)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listtargetsforsecurityprofilepaginator)
     """
 
     def paginate(
-        self, *, securityProfileName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, securityProfileName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTargetsForSecurityProfileResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTargetsForSecurityProfile.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listtargetsforsecurityprofilepaginator)
         """
 
 
@@ -1116,45 +1109,45 @@
 
     def paginate(
         self,
         *,
         parentGroup: str = ...,
         namePrefixFilter: str = ...,
         recursive: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListThingGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthinggroupspaginator)
         """
 
 
 class ListThingGroupsForThingPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingGroupsForThing)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthinggroupsforthingpaginator)
     """
 
     def paginate(
-        self, *, thingName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, thingName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListThingGroupsForThingResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingGroupsForThing.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthinggroupsforthingpaginator)
         """
 
 
 class ListThingPrincipalsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingPrincipals)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthingprincipalspaginator)
     """
 
     def paginate(
-        self, *, thingName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, thingName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListThingPrincipalsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingPrincipals.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthingprincipalspaginator)
         """
 
 
@@ -1165,45 +1158,45 @@
     """
 
     def paginate(
         self,
         *,
         taskId: str,
         reportType: ReportTypeType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListThingRegistrationTaskReportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingRegistrationTaskReports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthingregistrationtaskreportspaginator)
         """
 
 
 class ListThingRegistrationTasksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingRegistrationTasks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthingregistrationtaskspaginator)
     """
 
     def paginate(
-        self, *, status: StatusType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, status: StatusType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListThingRegistrationTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingRegistrationTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthingregistrationtaskspaginator)
         """
 
 
 class ListThingTypesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingTypes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthingtypespaginator)
     """
 
     def paginate(
-        self, *, thingTypeName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, thingTypeName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListThingTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthingtypespaginator)
         """
 
 
@@ -1216,30 +1209,30 @@
     def paginate(
         self,
         *,
         attributeName: str = ...,
         attributeValue: str = ...,
         thingTypeName: str = ...,
         usePrefixAttributeValue: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListThingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthingspaginator)
         """
 
 
 class ListThingsInBillingGroupPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingsInBillingGroup)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthingsinbillinggrouppaginator)
     """
 
     def paginate(
-        self, *, billingGroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, billingGroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListThingsInBillingGroupResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingsInBillingGroup.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthingsinbillinggrouppaginator)
         """
 
 
@@ -1250,30 +1243,30 @@
     """
 
     def paginate(
         self,
         *,
         thingGroupName: str,
         recursive: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListThingsInThingGroupResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingsInThingGroup.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthingsinthinggrouppaginator)
         """
 
 
 class ListTopicRuleDestinationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTopicRuleDestinations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listtopicruledestinationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTopicRuleDestinationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTopicRuleDestinations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listtopicruledestinationspaginator)
         """
 
 
@@ -1284,33 +1277,30 @@
     """
 
     def paginate(
         self,
         *,
         topic: str = ...,
         ruleDisabled: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTopicRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTopicRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listtopicrulespaginator)
         """
 
 
 class ListV2LoggingLevelsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListV2LoggingLevels)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listv2logginglevelspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        targetType: LogTargetTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, targetType: LogTargetTypeType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListV2LoggingLevelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListV2LoggingLevels.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listv2logginglevelspaginator)
         """
 
 
@@ -1319,20 +1309,20 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListViolationEvents)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listviolationeventspaginator)
     """
 
     def paginate(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         thingName: str = ...,
         securityProfileName: str = ...,
         behaviorCriteriaType: BehaviorCriteriaTypeType = ...,
         listSuppressedAlerts: bool = ...,
         verificationState: VerificationStateType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListViolationEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListViolationEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listviolationeventspaginator)
         """
```

### Comparing `types-aiobotocore-iot-2.5.2/types_aiobotocore_iot/paginator.pyi` & `types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -132,16 +132,15 @@
         list_things_in_thing_group_paginator: ListThingsInThingGroupPaginator = client.get_paginator("list_things_in_thing_group")
         list_topic_rule_destinations_paginator: ListTopicRuleDestinationsPaginator = client.get_paginator("list_topic_rule_destinations")
         list_topic_rules_paginator: ListTopicRulesPaginator = client.get_paginator("list_topic_rules")
         list_v2_logging_levels_paginator: ListV2LoggingLevelsPaginator = client.get_paginator("list_v2_logging_levels")
         list_violation_events_paginator: ListViolationEventsPaginator = client.get_paginator("list_violation_events")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import (
     AuditMitigationActionsExecutionStatusType,
     AuditMitigationActionsTaskStatusType,
@@ -220,14 +219,15 @@
     ListThingTypesResponseTypeDef,
     ListTopicRuleDestinationsResponseTypeDef,
     ListTopicRulesResponseTypeDef,
     ListV2LoggingLevelsResponseTypeDef,
     ListViolationEventsResponseTypeDef,
     PaginatorConfigTypeDef,
     ResourceIdentifierTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "GetBehaviorModelTrainingSummariesPaginator",
     "ListActiveViolationsPaginator",
     "ListAttachedPoliciesPaginator",
     "ListAuditFindingsPaginator",
@@ -299,15 +299,15 @@
 class GetBehaviorModelTrainingSummariesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.GetBehaviorModelTrainingSummaries)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#getbehaviormodeltrainingsummariespaginator)
     """
 
     def paginate(
-        self, *, securityProfileName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, securityProfileName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetBehaviorModelTrainingSummariesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.GetBehaviorModelTrainingSummaries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#getbehaviormodeltrainingsummariespaginator)
         """
 
 class ListActiveViolationsPaginator(AioPaginator):
@@ -320,33 +320,29 @@
         self,
         *,
         thingName: str = ...,
         securityProfileName: str = ...,
         behaviorCriteriaType: BehaviorCriteriaTypeType = ...,
         listSuppressedAlerts: bool = ...,
         verificationState: VerificationStateType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListActiveViolationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListActiveViolations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listactiveviolationspaginator)
         """
 
 class ListAttachedPoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAttachedPolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listattachedpoliciespaginator)
     """
 
     def paginate(
-        self,
-        *,
-        target: str,
-        recursive: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, target: str, recursive: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAttachedPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAttachedPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listattachedpoliciespaginator)
         """
 
 class ListAuditFindingsPaginator(AioPaginator):
@@ -357,18 +353,18 @@
 
     def paginate(
         self,
         *,
         taskId: str = ...,
         checkName: str = ...,
         resourceIdentifier: ResourceIdentifierTypeDef = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         listSuppressedFindings: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAuditFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listauditfindingspaginator)
         """
 
 class ListAuditMitigationActionsExecutionsPaginator(AioPaginator):
@@ -379,15 +375,15 @@
 
     def paginate(
         self,
         *,
         taskId: str,
         findingId: str,
         actionStatus: AuditMitigationActionsExecutionStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAuditMitigationActionsExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditMitigationActionsExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listauditmitigationactionsexecutionspaginator)
         """
 
 class ListAuditMitigationActionsTasksPaginator(AioPaginator):
@@ -395,20 +391,20 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditMitigationActionsTasks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listauditmitigationactionstaskspaginator)
     """
 
     def paginate(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         auditTaskId: str = ...,
         findingId: str = ...,
         taskStatus: AuditMitigationActionsTaskStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAuditMitigationActionsTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditMitigationActionsTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listauditmitigationactionstaskspaginator)
         """
 
 class ListAuditSuppressionsPaginator(AioPaginator):
@@ -419,15 +415,15 @@
 
     def paginate(
         self,
         *,
         checkName: str = ...,
         resourceIdentifier: ResourceIdentifierTypeDef = ...,
         ascendingOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAuditSuppressionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditSuppressions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listauditsuppressionspaginator)
         """
 
 class ListAuditTasksPaginator(AioPaginator):
@@ -435,19 +431,19 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditTasks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listaudittaskspaginator)
     """
 
     def paginate(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         taskType: AuditTaskTypeType = ...,
         taskStatus: AuditTaskStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAuditTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listaudittaskspaginator)
         """
 
 class ListAuthorizersPaginator(AioPaginator):
@@ -457,29 +453,29 @@
     """
 
     def paginate(
         self,
         *,
         ascendingOrder: bool = ...,
         status: AuthorizerStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAuthorizersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuthorizers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listauthorizerspaginator)
         """
 
 class ListBillingGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListBillingGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listbillinggroupspaginator)
     """
 
     def paginate(
-        self, *, namePrefixFilter: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, namePrefixFilter: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBillingGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListBillingGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listbillinggroupspaginator)
         """
 
 class ListCACertificatesPaginator(AioPaginator):
@@ -489,29 +485,29 @@
     """
 
     def paginate(
         self,
         *,
         ascendingOrder: bool = ...,
         templateName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCACertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCACertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listcacertificatespaginator)
         """
 
 class ListCertificatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCertificates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listcertificatespaginator)
     """
 
     def paginate(
-        self, *, ascendingOrder: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ascendingOrder: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listcertificatespaginator)
         """
 
 class ListCertificatesByCAPaginator(AioPaginator):
@@ -521,29 +517,29 @@
     """
 
     def paginate(
         self,
         *,
         caCertificateId: str,
         ascendingOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCertificatesByCAResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCertificatesByCA.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listcertificatesbycapaginator)
         """
 
 class ListCustomMetricsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCustomMetrics)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listcustommetricspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCustomMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCustomMetrics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listcustommetricspaginator)
         """
 
 class ListDetectMitigationActionsExecutionsPaginator(AioPaginator):
@@ -554,17 +550,17 @@
 
     def paginate(
         self,
         *,
         taskId: str = ...,
         violationId: str = ...,
         thingName: str = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDetectMitigationActionsExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDetectMitigationActionsExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listdetectmitigationactionsexecutionspaginator)
         """
 
 class ListDetectMitigationActionsTasksPaginator(AioPaginator):
@@ -572,76 +568,73 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDetectMitigationActionsTasks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listdetectmitigationactionstaskspaginator)
     """
 
     def paginate(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDetectMitigationActionsTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDetectMitigationActionsTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listdetectmitigationactionstaskspaginator)
         """
 
 class ListDimensionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDimensions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listdimensionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDimensionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDimensions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listdimensionspaginator)
         """
 
 class ListDomainConfigurationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDomainConfigurations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listdomainconfigurationspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        serviceType: ServiceTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, serviceType: ServiceTypeType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDomainConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDomainConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listdomainconfigurationspaginator)
         """
 
 class ListFleetMetricsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListFleetMetrics)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listfleetmetricspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFleetMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListFleetMetrics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listfleetmetricspaginator)
         """
 
 class ListIndicesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListIndices)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listindicespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListIndicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListIndices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listindicespaginator)
         """
 
 class ListJobExecutionsForJobPaginator(AioPaginator):
@@ -651,15 +644,15 @@
     """
 
     def paginate(
         self,
         *,
         jobId: str,
         status: JobExecutionStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListJobExecutionsForJobResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobExecutionsForJob.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listjobexecutionsforjobpaginator)
         """
 
 class ListJobExecutionsForThingPaginator(AioPaginator):
@@ -671,29 +664,29 @@
     def paginate(
         self,
         *,
         thingName: str,
         status: JobExecutionStatusType = ...,
         namespaceId: str = ...,
         jobId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListJobExecutionsForThingResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobExecutionsForThing.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listjobexecutionsforthingpaginator)
         """
 
 class ListJobTemplatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobTemplates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listjobtemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListJobTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listjobtemplatespaginator)
         """
 
 class ListJobsPaginator(AioPaginator):
@@ -706,29 +699,29 @@
         self,
         *,
         status: JobStatusType = ...,
         targetSelection: TargetSelectionType = ...,
         thingGroupName: str = ...,
         thingGroupId: str = ...,
         namespaceId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listjobspaginator)
         """
 
 class ListManagedJobTemplatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListManagedJobTemplates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listmanagedjobtemplatespaginator)
     """
 
     def paginate(
-        self, *, templateName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, templateName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListManagedJobTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListManagedJobTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listmanagedjobtemplatespaginator)
         """
 
 class ListMetricValuesPaginator(AioPaginator):
@@ -738,19 +731,19 @@
     """
 
     def paginate(
         self,
         *,
         thingName: str,
         metricName: str,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         dimensionName: str = ...,
         dimensionValueOperator: DimensionValueOperatorType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMetricValuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListMetricValues.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listmetricvaluespaginator)
         """
 
 class ListMitigationActionsPaginator(AioPaginator):
@@ -759,15 +752,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listmitigationactionspaginator)
     """
 
     def paginate(
         self,
         *,
         actionType: MitigationActionTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMitigationActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListMitigationActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listmitigationactionspaginator)
         """
 
 class ListOTAUpdatesPaginator(AioPaginator):
@@ -776,29 +769,29 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listotaupdatespaginator)
     """
 
     def paginate(
         self,
         *,
         otaUpdateStatus: OTAUpdateStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListOTAUpdatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListOTAUpdates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listotaupdatespaginator)
         """
 
 class ListOutgoingCertificatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListOutgoingCertificates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listoutgoingcertificatespaginator)
     """
 
     def paginate(
-        self, *, ascendingOrder: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ascendingOrder: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListOutgoingCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListOutgoingCertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listoutgoingcertificatespaginator)
         """
 
 class ListPackageVersionsPaginator(AioPaginator):
@@ -808,43 +801,43 @@
     """
 
     def paginate(
         self,
         *,
         packageName: str,
         status: PackageVersionStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPackageVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPackageVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listpackageversionspaginator)
         """
 
 class ListPackagesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPackages)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listpackagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPackagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPackages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listpackagespaginator)
         """
 
 class ListPoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listpoliciespaginator)
     """
 
     def paginate(
-        self, *, ascendingOrder: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ascendingOrder: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listpoliciespaginator)
         """
 
 class ListPolicyPrincipalsPaginator(AioPaginator):
@@ -854,15 +847,15 @@
     """
 
     def paginate(
         self,
         *,
         policyName: str,
         ascendingOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPolicyPrincipalsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPolicyPrincipals.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listpolicyprincipalspaginator)
         """
 
 class ListPrincipalPoliciesPaginator(AioPaginator):
@@ -872,99 +865,99 @@
     """
 
     def paginate(
         self,
         *,
         principal: str,
         ascendingOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPrincipalPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPrincipalPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listprincipalpoliciespaginator)
         """
 
 class ListPrincipalThingsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPrincipalThings)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listprincipalthingspaginator)
     """
 
     def paginate(
-        self, *, principal: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, principal: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPrincipalThingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPrincipalThings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listprincipalthingspaginator)
         """
 
 class ListProvisioningTemplateVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListProvisioningTemplateVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listprovisioningtemplateversionspaginator)
     """
 
     def paginate(
-        self, *, templateName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, templateName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProvisioningTemplateVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListProvisioningTemplateVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listprovisioningtemplateversionspaginator)
         """
 
 class ListProvisioningTemplatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListProvisioningTemplates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listprovisioningtemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProvisioningTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListProvisioningTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listprovisioningtemplatespaginator)
         """
 
 class ListRelatedResourcesForAuditFindingPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListRelatedResourcesForAuditFinding)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listrelatedresourcesforauditfindingpaginator)
     """
 
     def paginate(
-        self, *, findingId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, findingId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRelatedResourcesForAuditFindingResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListRelatedResourcesForAuditFinding.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listrelatedresourcesforauditfindingpaginator)
         """
 
 class ListRoleAliasesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListRoleAliases)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listrolealiasespaginator)
     """
 
     def paginate(
-        self, *, ascendingOrder: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ascendingOrder: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRoleAliasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListRoleAliases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listrolealiasespaginator)
         """
 
 class ListScheduledAuditsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListScheduledAudits)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listscheduledauditspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListScheduledAuditsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListScheduledAudits.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listscheduledauditspaginator)
         """
 
 class ListSecurityProfilesPaginator(AioPaginator):
@@ -974,15 +967,15 @@
     """
 
     def paginate(
         self,
         *,
         dimensionName: str = ...,
         metricName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSecurityProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListSecurityProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listsecurityprofilespaginator)
         """
 
 class ListSecurityProfilesForTargetPaginator(AioPaginator):
@@ -992,71 +985,71 @@
     """
 
     def paginate(
         self,
         *,
         securityProfileTargetArn: str,
         recursive: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSecurityProfilesForTargetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListSecurityProfilesForTarget.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listsecurityprofilesfortargetpaginator)
         """
 
 class ListStreamsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListStreams)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#liststreamspaginator)
     """
 
     def paginate(
-        self, *, ascendingOrder: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ascendingOrder: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStreamsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListStreams.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#liststreamspaginator)
         """
 
 class ListTagsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTagsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTagsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listtagsforresourcepaginator)
         """
 
 class ListTargetsForPolicyPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTargetsForPolicy)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listtargetsforpolicypaginator)
     """
 
     def paginate(
-        self, *, policyName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, policyName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTargetsForPolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTargetsForPolicy.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listtargetsforpolicypaginator)
         """
 
 class ListTargetsForSecurityProfilePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTargetsForSecurityProfile)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listtargetsforsecurityprofilepaginator)
     """
 
     def paginate(
-        self, *, securityProfileName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, securityProfileName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTargetsForSecurityProfileResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTargetsForSecurityProfile.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listtargetsforsecurityprofilepaginator)
         """
 
 class ListThingGroupsPaginator(AioPaginator):
@@ -1067,43 +1060,43 @@
 
     def paginate(
         self,
         *,
         parentGroup: str = ...,
         namePrefixFilter: str = ...,
         recursive: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListThingGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthinggroupspaginator)
         """
 
 class ListThingGroupsForThingPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingGroupsForThing)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthinggroupsforthingpaginator)
     """
 
     def paginate(
-        self, *, thingName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, thingName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListThingGroupsForThingResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingGroupsForThing.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthinggroupsforthingpaginator)
         """
 
 class ListThingPrincipalsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingPrincipals)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthingprincipalspaginator)
     """
 
     def paginate(
-        self, *, thingName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, thingName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListThingPrincipalsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingPrincipals.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthingprincipalspaginator)
         """
 
 class ListThingRegistrationTaskReportsPaginator(AioPaginator):
@@ -1113,43 +1106,43 @@
     """
 
     def paginate(
         self,
         *,
         taskId: str,
         reportType: ReportTypeType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListThingRegistrationTaskReportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingRegistrationTaskReports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthingregistrationtaskreportspaginator)
         """
 
 class ListThingRegistrationTasksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingRegistrationTasks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthingregistrationtaskspaginator)
     """
 
     def paginate(
-        self, *, status: StatusType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, status: StatusType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListThingRegistrationTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingRegistrationTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthingregistrationtaskspaginator)
         """
 
 class ListThingTypesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingTypes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthingtypespaginator)
     """
 
     def paginate(
-        self, *, thingTypeName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, thingTypeName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListThingTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthingtypespaginator)
         """
 
 class ListThingsPaginator(AioPaginator):
@@ -1161,29 +1154,29 @@
     def paginate(
         self,
         *,
         attributeName: str = ...,
         attributeValue: str = ...,
         thingTypeName: str = ...,
         usePrefixAttributeValue: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListThingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthingspaginator)
         """
 
 class ListThingsInBillingGroupPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingsInBillingGroup)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthingsinbillinggrouppaginator)
     """
 
     def paginate(
-        self, *, billingGroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, billingGroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListThingsInBillingGroupResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingsInBillingGroup.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthingsinbillinggrouppaginator)
         """
 
 class ListThingsInThingGroupPaginator(AioPaginator):
@@ -1193,29 +1186,29 @@
     """
 
     def paginate(
         self,
         *,
         thingGroupName: str,
         recursive: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListThingsInThingGroupResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingsInThingGroup.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listthingsinthinggrouppaginator)
         """
 
 class ListTopicRuleDestinationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTopicRuleDestinations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listtopicruledestinationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTopicRuleDestinationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTopicRuleDestinations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listtopicruledestinationspaginator)
         """
 
 class ListTopicRulesPaginator(AioPaginator):
@@ -1225,32 +1218,29 @@
     """
 
     def paginate(
         self,
         *,
         topic: str = ...,
         ruleDisabled: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTopicRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTopicRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listtopicrulespaginator)
         """
 
 class ListV2LoggingLevelsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListV2LoggingLevels)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listv2logginglevelspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        targetType: LogTargetTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, targetType: LogTargetTypeType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListV2LoggingLevelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListV2LoggingLevels.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listv2logginglevelspaginator)
         """
 
 class ListViolationEventsPaginator(AioPaginator):
@@ -1258,20 +1248,20 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListViolationEvents)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listviolationeventspaginator)
     """
 
     def paginate(
         self,
         *,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         thingName: str = ...,
         securityProfileName: str = ...,
         behaviorCriteriaType: BehaviorCriteriaTypeType = ...,
         listSuppressedAlerts: bool = ...,
         verificationState: VerificationStateType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListViolationEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListViolationEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/paginators/#listviolationeventspaginator)
         """
```

### Comparing `types-aiobotocore-iot-2.5.2/types_aiobotocore_iot/type_defs.py` & `types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_iot.type_defs import AbortCriteriaTypeDef
 
-    data: AbortCriteriaTypeDef = {...}
+    data: AbortCriteriaTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -99,118 +99,101 @@
     "CloudwatchLogsActionTypeDef",
     "CloudwatchMetricActionTypeDef",
     "DynamoDBActionTypeDef",
     "ElasticsearchActionTypeDef",
     "FirehoseActionTypeDef",
     "IotAnalyticsActionTypeDef",
     "IotEventsActionTypeDef",
-    "KafkaActionTypeDef",
+    "KafkaActionOutputTypeDef",
     "KinesisActionTypeDef",
     "LambdaActionTypeDef",
     "OpenSearchActionTypeDef",
     "S3ActionTypeDef",
     "SalesforceActionTypeDef",
     "SnsActionTypeDef",
     "SqsActionTypeDef",
     "StepFunctionsActionTypeDef",
-    "MetricValueTypeDef",
+    "KafkaActionTypeDef",
+    "MetricValueOutputTypeDef",
     "ViolationEventAdditionalInfoTypeDef",
     "AddThingToBillingGroupRequestRequestTypeDef",
     "AddThingToThingGroupRequestRequestTypeDef",
+    "AddThingsToThingGroupParamsOutputTypeDef",
     "AddThingsToThingGroupParamsTypeDef",
+    "AggregationTypeOutputTypeDef",
     "AggregationTypeTypeDef",
     "AlertTargetTypeDef",
     "PolicyTypeDef",
     "AssetPropertyTimestampTypeDef",
     "AssetPropertyVariantTypeDef",
     "AssociateTargetsWithJobRequestRequestTypeDef",
-    "AssociateTargetsWithJobResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AttachPolicyRequestRequestTypeDef",
     "AttachPrincipalPolicyRequestRequestTypeDef",
     "AttachSecurityProfileRequestRequestTypeDef",
     "AttachThingPrincipalRequestRequestTypeDef",
+    "AttributePayloadOutputTypeDef",
     "AttributePayloadTypeDef",
     "AuditCheckConfigurationTypeDef",
     "AuditCheckDetailsTypeDef",
     "AuditMitigationActionExecutionMetadataTypeDef",
     "AuditMitigationActionsTaskMetadataTypeDef",
+    "AuditMitigationActionsTaskTargetOutputTypeDef",
     "AuditMitigationActionsTaskTargetTypeDef",
     "AuditNotificationTargetTypeDef",
     "AuditTaskMetadataTypeDef",
+    "AuthInfoOutputTypeDef",
     "AuthInfoTypeDef",
     "AuthorizerConfigTypeDef",
     "AuthorizerDescriptionTypeDef",
     "AuthorizerSummaryTypeDef",
     "AwsJobAbortCriteriaTypeDef",
     "AwsJobRateIncreaseCriteriaTypeDef",
     "AwsJobPresignedUrlConfigTypeDef",
     "AwsJobTimeoutConfigTypeDef",
     "MachineLearningDetectionConfigTypeDef",
     "StatisticalThresholdTypeDef",
+    "MetricValueTypeDef",
     "BehaviorModelTrainingSummaryTypeDef",
     "MetricDimensionTypeDef",
     "BillingGroupMetadataTypeDef",
     "BillingGroupPropertiesTypeDef",
+    "BlobTypeDef",
     "BucketTypeDef",
     "TermsAggregationTypeDef",
     "CertificateValidityTypeDef",
     "CACertificateTypeDef",
     "CancelAuditMitigationActionsTaskRequestRequestTypeDef",
     "CancelAuditTaskRequestRequestTypeDef",
     "CancelCertificateTransferRequestRequestTypeDef",
     "CancelDetectMitigationActionsTaskRequestRequestTypeDef",
     "CancelJobExecutionRequestRequestTypeDef",
     "CancelJobRequestRequestTypeDef",
-    "CancelJobResponseTypeDef",
     "TransferDataTypeDef",
     "CertificateTypeDef",
     "CodeSigningCertificateChainTypeDef",
-    "CodeSigningSignatureTypeDef",
+    "CodeSigningSignatureOutputTypeDef",
     "ConfigurationTypeDef",
     "ConfirmTopicRuleDestinationRequestRequestTypeDef",
+    "TimestampTypeDef",
     "TagTypeDef",
-    "CreateAuthorizerResponseTypeDef",
-    "CreateBillingGroupResponseTypeDef",
     "CreateCertificateFromCsrRequestRequestTypeDef",
-    "CreateCertificateFromCsrResponseTypeDef",
-    "CreateCustomMetricResponseTypeDef",
-    "CreateDimensionResponseTypeDef",
     "TlsConfigTypeDef",
-    "CreateDomainConfigurationResponseTypeDef",
-    "CreateDynamicThingGroupResponseTypeDef",
-    "CreateFleetMetricResponseTypeDef",
     "PresignedUrlConfigTypeDef",
     "TimeoutConfigTypeDef",
-    "CreateJobResponseTypeDef",
     "MaintenanceWindowTypeDef",
-    "CreateJobTemplateResponseTypeDef",
     "CreateKeysAndCertificateRequestRequestTypeDef",
     "KeyPairTypeDef",
-    "CreateMitigationActionResponseTypeDef",
-    "CreateOTAUpdateResponseTypeDef",
     "CreatePackageRequestRequestTypeDef",
-    "CreatePackageResponseTypeDef",
     "CreatePackageVersionRequestRequestTypeDef",
-    "CreatePackageVersionResponseTypeDef",
-    "CreatePolicyResponseTypeDef",
     "CreatePolicyVersionRequestRequestTypeDef",
-    "CreatePolicyVersionResponseTypeDef",
     "CreateProvisioningClaimRequestRequestTypeDef",
     "ProvisioningHookTypeDef",
-    "CreateProvisioningTemplateResponseTypeDef",
     "CreateProvisioningTemplateVersionRequestRequestTypeDef",
-    "CreateProvisioningTemplateVersionResponseTypeDef",
-    "CreateRoleAliasResponseTypeDef",
-    "CreateScheduledAuditResponseTypeDef",
-    "CreateSecurityProfileResponseTypeDef",
-    "CreateStreamResponseTypeDef",
-    "CreateThingGroupResponseTypeDef",
-    "CreateThingResponseTypeDef",
     "ThingTypePropertiesTypeDef",
-    "CreateThingTypeResponseTypeDef",
     "DeleteAccountAuditConfigurationRequestRequestTypeDef",
     "DeleteAuthorizerRequestRequestTypeDef",
     "DeleteBillingGroupRequestRequestTypeDef",
     "DeleteCACertificateRequestRequestTypeDef",
     "DeleteCertificateRequestRequestTypeDef",
     "DeleteCustomMetricRequestRequestTypeDef",
     "DeleteDimensionRequestRequestTypeDef",
@@ -246,374 +229,355 @@
     "TaskStatisticsTypeDef",
     "DescribeAuthorizerRequestRequestTypeDef",
     "DescribeBillingGroupRequestRequestTypeDef",
     "DescribeCACertificateRequestRequestTypeDef",
     "RegistrationConfigTypeDef",
     "DescribeCertificateRequestRequestTypeDef",
     "DescribeCustomMetricRequestRequestTypeDef",
-    "DescribeCustomMetricResponseTypeDef",
     "DescribeDetectMitigationActionsTaskRequestRequestTypeDef",
     "DescribeDimensionRequestRequestTypeDef",
-    "DescribeDimensionResponseTypeDef",
     "DescribeDomainConfigurationRequestRequestTypeDef",
     "ServerCertificateSummaryTypeDef",
     "DescribeEndpointRequestRequestTypeDef",
-    "DescribeEndpointResponseTypeDef",
     "DescribeFleetMetricRequestRequestTypeDef",
     "DescribeIndexRequestRequestTypeDef",
-    "DescribeIndexResponseTypeDef",
     "DescribeJobExecutionRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
     "DescribeJobTemplateRequestRequestTypeDef",
     "DescribeManagedJobTemplateRequestRequestTypeDef",
     "DocumentParameterTypeDef",
     "DescribeMitigationActionRequestRequestTypeDef",
     "DescribeProvisioningTemplateRequestRequestTypeDef",
     "DescribeProvisioningTemplateVersionRequestRequestTypeDef",
-    "DescribeProvisioningTemplateVersionResponseTypeDef",
     "DescribeRoleAliasRequestRequestTypeDef",
     "RoleAliasDescriptionTypeDef",
     "DescribeScheduledAuditRequestRequestTypeDef",
-    "DescribeScheduledAuditResponseTypeDef",
     "DescribeSecurityProfileRequestRequestTypeDef",
     "DescribeStreamRequestRequestTypeDef",
     "DescribeThingGroupRequestRequestTypeDef",
     "DescribeThingRegistrationTaskRequestRequestTypeDef",
-    "DescribeThingRegistrationTaskResponseTypeDef",
     "DescribeThingRequestRequestTypeDef",
-    "DescribeThingResponseTypeDef",
     "DescribeThingTypeRequestRequestTypeDef",
     "ThingTypeMetadataTypeDef",
+    "ThingTypePropertiesOutputTypeDef",
     "S3DestinationTypeDef",
     "DetachPolicyRequestRequestTypeDef",
     "DetachPrincipalPolicyRequestRequestTypeDef",
     "DetachSecurityProfileRequestRequestTypeDef",
     "DetachThingPrincipalRequestRequestTypeDef",
     "DetectMitigationActionExecutionTypeDef",
     "DetectMitigationActionsTaskStatisticsTypeDef",
+    "DetectMitigationActionsTaskTargetOutputTypeDef",
+    "ViolationEventOccurrenceRangeOutputTypeDef",
     "DetectMitigationActionsTaskTargetTypeDef",
-    "ViolationEventOccurrenceRangeTypeDef",
     "DisableTopicRuleRequestRequestTypeDef",
     "DomainConfigurationSummaryTypeDef",
     "PutItemInputTypeDef",
     "EffectivePolicyTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableIoTLoggingParamsTypeDef",
     "EnableTopicRuleRequestRequestTypeDef",
     "ErrorInfoTypeDef",
     "RateIncreaseCriteriaTypeDef",
     "FieldTypeDef",
     "S3LocationTypeDef",
     "StreamTypeDef",
     "FleetMetricNameAndArnTypeDef",
-    "GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetBehaviorModelTrainingSummariesRequestRequestTypeDef",
     "GetCardinalityRequestRequestTypeDef",
-    "GetCardinalityResponseTypeDef",
     "GetEffectivePoliciesRequestRequestTypeDef",
     "GetJobDocumentRequestRequestTypeDef",
-    "GetJobDocumentResponseTypeDef",
-    "GetLoggingOptionsResponseTypeDef",
     "GetOTAUpdateRequestRequestTypeDef",
     "VersionUpdateByJobsConfigTypeDef",
     "GetPackageRequestRequestTypeDef",
-    "GetPackageResponseTypeDef",
     "GetPackageVersionRequestRequestTypeDef",
-    "GetPackageVersionResponseTypeDef",
     "GetPercentilesRequestRequestTypeDef",
     "PercentPairTypeDef",
     "GetPolicyRequestRequestTypeDef",
-    "GetPolicyResponseTypeDef",
     "GetPolicyVersionRequestRequestTypeDef",
-    "GetPolicyVersionResponseTypeDef",
-    "GetRegistrationCodeResponseTypeDef",
     "GetStatisticsRequestRequestTypeDef",
     "StatisticsTypeDef",
     "GetTopicRuleDestinationRequestRequestTypeDef",
     "GetTopicRuleRequestRequestTypeDef",
-    "GetV2LoggingOptionsResponseTypeDef",
     "GroupNameAndArnTypeDef",
     "HttpActionHeaderTypeDef",
     "SigV4AuthorizationTypeDef",
     "HttpContextTypeDef",
     "HttpUrlDestinationConfigurationTypeDef",
     "HttpUrlDestinationPropertiesTypeDef",
     "HttpUrlDestinationSummaryTypeDef",
+    "IndexingFilterOutputTypeDef",
     "IndexingFilterTypeDef",
     "IssuerCertificateIdentifierTypeDef",
     "JobExecutionStatusDetailsTypeDef",
     "JobExecutionSummaryTypeDef",
     "RetryCriteriaTypeDef",
     "JobProcessDetailsTypeDef",
     "JobSummaryTypeDef",
     "JobTemplateSummaryTypeDef",
     "ScheduledJobRolloutTypeDef",
-    "ListActiveViolationsRequestListActiveViolationsPaginateTypeDef",
     "ListActiveViolationsRequestRequestTypeDef",
-    "ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef",
     "ListAttachedPoliciesRequestRequestTypeDef",
-    "ListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef",
     "ListAuditMitigationActionsExecutionsRequestRequestTypeDef",
-    "ListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef",
-    "ListAuditMitigationActionsTasksRequestRequestTypeDef",
-    "ListAuditTasksRequestListAuditTasksPaginateTypeDef",
-    "ListAuditTasksRequestRequestTypeDef",
-    "ListAuthorizersRequestListAuthorizersPaginateTypeDef",
     "ListAuthorizersRequestRequestTypeDef",
-    "ListBillingGroupsRequestListBillingGroupsPaginateTypeDef",
     "ListBillingGroupsRequestRequestTypeDef",
-    "ListCACertificatesRequestListCACertificatesPaginateTypeDef",
     "ListCACertificatesRequestRequestTypeDef",
-    "ListCertificatesByCARequestListCertificatesByCAPaginateTypeDef",
     "ListCertificatesByCARequestRequestTypeDef",
-    "ListCertificatesRequestListCertificatesPaginateTypeDef",
     "ListCertificatesRequestRequestTypeDef",
-    "ListCustomMetricsRequestListCustomMetricsPaginateTypeDef",
     "ListCustomMetricsRequestRequestTypeDef",
-    "ListCustomMetricsResponseTypeDef",
-    "ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef",
-    "ListDetectMitigationActionsExecutionsRequestRequestTypeDef",
-    "ListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef",
-    "ListDetectMitigationActionsTasksRequestRequestTypeDef",
-    "ListDimensionsRequestListDimensionsPaginateTypeDef",
     "ListDimensionsRequestRequestTypeDef",
-    "ListDimensionsResponseTypeDef",
-    "ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef",
     "ListDomainConfigurationsRequestRequestTypeDef",
-    "ListFleetMetricsRequestListFleetMetricsPaginateTypeDef",
     "ListFleetMetricsRequestRequestTypeDef",
-    "ListIndicesRequestListIndicesPaginateTypeDef",
     "ListIndicesRequestRequestTypeDef",
-    "ListIndicesResponseTypeDef",
-    "ListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef",
     "ListJobExecutionsForJobRequestRequestTypeDef",
-    "ListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef",
     "ListJobExecutionsForThingRequestRequestTypeDef",
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     "ListJobTemplatesRequestRequestTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
-    "ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef",
     "ListManagedJobTemplatesRequestRequestTypeDef",
     "ManagedJobTemplateSummaryTypeDef",
-    "ListMetricValuesRequestListMetricValuesPaginateTypeDef",
-    "ListMetricValuesRequestRequestTypeDef",
-    "ListMitigationActionsRequestListMitigationActionsPaginateTypeDef",
     "ListMitigationActionsRequestRequestTypeDef",
     "MitigationActionIdentifierTypeDef",
-    "ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef",
     "ListOTAUpdatesRequestRequestTypeDef",
     "OTAUpdateSummaryTypeDef",
-    "ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef",
     "ListOutgoingCertificatesRequestRequestTypeDef",
     "OutgoingCertificateTypeDef",
-    "ListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
     "ListPackageVersionsRequestRequestTypeDef",
     "PackageVersionSummaryTypeDef",
-    "ListPackagesRequestListPackagesPaginateTypeDef",
     "ListPackagesRequestRequestTypeDef",
     "PackageSummaryTypeDef",
-    "ListPoliciesRequestListPoliciesPaginateTypeDef",
     "ListPoliciesRequestRequestTypeDef",
-    "ListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef",
     "ListPolicyPrincipalsRequestRequestTypeDef",
-    "ListPolicyPrincipalsResponseTypeDef",
     "ListPolicyVersionsRequestRequestTypeDef",
     "PolicyVersionTypeDef",
-    "ListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef",
     "ListPrincipalPoliciesRequestRequestTypeDef",
-    "ListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef",
     "ListPrincipalThingsRequestRequestTypeDef",
-    "ListPrincipalThingsResponseTypeDef",
-    "ListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef",
     "ListProvisioningTemplateVersionsRequestRequestTypeDef",
     "ProvisioningTemplateVersionSummaryTypeDef",
-    "ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef",
     "ListProvisioningTemplatesRequestRequestTypeDef",
     "ProvisioningTemplateSummaryTypeDef",
-    "ListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef",
     "ListRelatedResourcesForAuditFindingRequestRequestTypeDef",
-    "ListRoleAliasesRequestListRoleAliasesPaginateTypeDef",
     "ListRoleAliasesRequestRequestTypeDef",
-    "ListRoleAliasesResponseTypeDef",
-    "ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef",
     "ListScheduledAuditsRequestRequestTypeDef",
     "ScheduledAuditMetadataTypeDef",
-    "ListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef",
     "ListSecurityProfilesForTargetRequestRequestTypeDef",
-    "ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef",
     "ListSecurityProfilesRequestRequestTypeDef",
     "SecurityProfileIdentifierTypeDef",
-    "ListStreamsRequestListStreamsPaginateTypeDef",
     "ListStreamsRequestRequestTypeDef",
     "StreamSummaryTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef",
     "ListTargetsForPolicyRequestRequestTypeDef",
-    "ListTargetsForPolicyResponseTypeDef",
-    "ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef",
     "ListTargetsForSecurityProfileRequestRequestTypeDef",
     "SecurityProfileTargetTypeDef",
-    "ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef",
     "ListThingGroupsForThingRequestRequestTypeDef",
-    "ListThingGroupsRequestListThingGroupsPaginateTypeDef",
     "ListThingGroupsRequestRequestTypeDef",
-    "ListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef",
     "ListThingPrincipalsRequestRequestTypeDef",
-    "ListThingPrincipalsResponseTypeDef",
-    "ListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef",
     "ListThingRegistrationTaskReportsRequestRequestTypeDef",
-    "ListThingRegistrationTaskReportsResponseTypeDef",
-    "ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef",
     "ListThingRegistrationTasksRequestRequestTypeDef",
-    "ListThingRegistrationTasksResponseTypeDef",
-    "ListThingTypesRequestListThingTypesPaginateTypeDef",
     "ListThingTypesRequestRequestTypeDef",
-    "ListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef",
     "ListThingsInBillingGroupRequestRequestTypeDef",
-    "ListThingsInBillingGroupResponseTypeDef",
-    "ListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef",
     "ListThingsInThingGroupRequestRequestTypeDef",
-    "ListThingsInThingGroupResponseTypeDef",
-    "ListThingsRequestListThingsPaginateTypeDef",
     "ListThingsRequestRequestTypeDef",
     "ThingAttributeTypeDef",
-    "ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef",
     "ListTopicRuleDestinationsRequestRequestTypeDef",
-    "ListTopicRulesRequestListTopicRulesPaginateTypeDef",
     "ListTopicRulesRequestRequestTypeDef",
     "TopicRuleListItemTypeDef",
-    "ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef",
     "ListV2LoggingLevelsRequestRequestTypeDef",
-    "ListViolationEventsRequestListViolationEventsPaginateTypeDef",
-    "ListViolationEventsRequestRequestTypeDef",
     "LocationTimestampTypeDef",
     "LogTargetTypeDef",
     "LoggingOptionsPayloadTypeDef",
     "PublishFindingToSnsParamsTypeDef",
     "ReplaceDefaultPolicyVersionParamsTypeDef",
     "UpdateCACertificateParamsTypeDef",
     "UpdateDeviceCertificateParamsTypeDef",
-    "MqttContextTypeDef",
     "UserPropertyTypeDef",
-    "PaginatorConfigTypeDef",
     "PolicyVersionIdentifierTypeDef",
     "PutVerificationStateOnViolationRequestRequestTypeDef",
-    "RegisterCACertificateResponseTypeDef",
     "RegisterCertificateRequestRequestTypeDef",
-    "RegisterCertificateResponseTypeDef",
     "RegisterCertificateWithoutCARequestRequestTypeDef",
-    "RegisterCertificateWithoutCAResponseTypeDef",
     "RegisterThingRequestRequestTypeDef",
-    "RegisterThingResponseTypeDef",
     "RejectCertificateTransferRequestRequestTypeDef",
     "RemoveThingFromBillingGroupRequestRequestTypeDef",
     "RemoveThingFromThingGroupRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "SearchIndexRequestRequestTypeDef",
     "ThingGroupDocumentTypeDef",
     "SetDefaultAuthorizerRequestRequestTypeDef",
-    "SetDefaultAuthorizerResponseTypeDef",
     "SetDefaultPolicyVersionRequestRequestTypeDef",
     "SetV2LoggingOptionsRequestRequestTypeDef",
     "SigningProfileParameterTypeDef",
-    "StartAuditMitigationActionsTaskResponseTypeDef",
-    "StartDetectMitigationActionsTaskResponseTypeDef",
     "StartOnDemandAuditTaskRequestRequestTypeDef",
-    "StartOnDemandAuditTaskResponseTypeDef",
     "StartThingRegistrationTaskRequestRequestTypeDef",
-    "StartThingRegistrationTaskResponseTypeDef",
     "StopThingRegistrationTaskRequestRequestTypeDef",
     "TlsContextTypeDef",
-    "TestInvokeAuthorizerResponseTypeDef",
     "ThingConnectivityTypeDef",
     "TimestreamDimensionTypeDef",
     "TimestreamTimestampTypeDef",
     "VpcDestinationConfigurationTypeDef",
     "VpcDestinationSummaryTypeDef",
     "VpcDestinationPropertiesTypeDef",
     "TransferCertificateRequestRequestTypeDef",
-    "TransferCertificateResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAuthorizerRequestRequestTypeDef",
-    "UpdateAuthorizerResponseTypeDef",
-    "UpdateBillingGroupResponseTypeDef",
     "UpdateCertificateRequestRequestTypeDef",
     "UpdateCustomMetricRequestRequestTypeDef",
-    "UpdateCustomMetricResponseTypeDef",
     "UpdateDimensionRequestRequestTypeDef",
-    "UpdateDimensionResponseTypeDef",
-    "UpdateDomainConfigurationResponseTypeDef",
-    "UpdateDynamicThingGroupResponseTypeDef",
-    "UpdateMitigationActionResponseTypeDef",
     "UpdatePackageRequestRequestTypeDef",
     "UpdatePackageVersionRequestRequestTypeDef",
     "UpdateRoleAliasRequestRequestTypeDef",
-    "UpdateRoleAliasResponseTypeDef",
     "UpdateScheduledAuditRequestRequestTypeDef",
-    "UpdateScheduledAuditResponseTypeDef",
-    "UpdateStreamResponseTypeDef",
-    "UpdateThingGroupResponseTypeDef",
     "UpdateThingGroupsForThingRequestRequestTypeDef",
     "UpdateTopicRuleDestinationRequestRequestTypeDef",
     "ValidationErrorTypeDef",
+    "AbortConfigOutputTypeDef",
     "AbortConfigTypeDef",
     "MetricDatumTypeDef",
-    "DescribeFleetMetricResponseTypeDef",
+    "AggregationTypeUnionTypeDef",
     "UpdateFleetMetricRequestRequestTypeDef",
     "AllowedTypeDef",
     "ExplicitDenyTypeDef",
     "ImplicitDenyTypeDef",
+    "AssetPropertyValueTypeDef",
+    "AssociateTargetsWithJobResponseTypeDef",
+    "CancelJobResponseTypeDef",
+    "CreateAuthorizerResponseTypeDef",
+    "CreateBillingGroupResponseTypeDef",
+    "CreateCertificateFromCsrResponseTypeDef",
+    "CreateCustomMetricResponseTypeDef",
+    "CreateDimensionResponseTypeDef",
+    "CreateDomainConfigurationResponseTypeDef",
+    "CreateDynamicThingGroupResponseTypeDef",
+    "CreateFleetMetricResponseTypeDef",
+    "CreateJobResponseTypeDef",
+    "CreateJobTemplateResponseTypeDef",
+    "CreateMitigationActionResponseTypeDef",
+    "CreateOTAUpdateResponseTypeDef",
+    "CreatePackageResponseTypeDef",
+    "CreatePackageVersionResponseTypeDef",
+    "CreatePolicyResponseTypeDef",
+    "CreatePolicyVersionResponseTypeDef",
+    "CreateProvisioningTemplateResponseTypeDef",
+    "CreateProvisioningTemplateVersionResponseTypeDef",
+    "CreateRoleAliasResponseTypeDef",
+    "CreateScheduledAuditResponseTypeDef",
+    "CreateSecurityProfileResponseTypeDef",
+    "CreateStreamResponseTypeDef",
+    "CreateThingGroupResponseTypeDef",
+    "CreateThingResponseTypeDef",
+    "CreateThingTypeResponseTypeDef",
+    "DescribeCustomMetricResponseTypeDef",
+    "DescribeDimensionResponseTypeDef",
+    "DescribeEndpointResponseTypeDef",
+    "DescribeFleetMetricResponseTypeDef",
+    "DescribeIndexResponseTypeDef",
+    "DescribeProvisioningTemplateVersionResponseTypeDef",
+    "DescribeScheduledAuditResponseTypeDef",
+    "DescribeThingRegistrationTaskResponseTypeDef",
+    "DescribeThingResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetCardinalityResponseTypeDef",
+    "GetJobDocumentResponseTypeDef",
+    "GetLoggingOptionsResponseTypeDef",
+    "GetPackageResponseTypeDef",
+    "GetPackageVersionResponseTypeDef",
+    "GetPolicyResponseTypeDef",
+    "GetPolicyVersionResponseTypeDef",
+    "GetRegistrationCodeResponseTypeDef",
+    "GetV2LoggingOptionsResponseTypeDef",
     "ListAttachedPoliciesResponseTypeDef",
+    "ListCustomMetricsResponseTypeDef",
+    "ListDimensionsResponseTypeDef",
+    "ListIndicesResponseTypeDef",
     "ListPoliciesResponseTypeDef",
+    "ListPolicyPrincipalsResponseTypeDef",
     "ListPrincipalPoliciesResponseTypeDef",
-    "AssetPropertyValueTypeDef",
+    "ListPrincipalThingsResponseTypeDef",
+    "ListRoleAliasesResponseTypeDef",
+    "ListTargetsForPolicyResponseTypeDef",
+    "ListThingPrincipalsResponseTypeDef",
+    "ListThingRegistrationTaskReportsResponseTypeDef",
+    "ListThingRegistrationTasksResponseTypeDef",
+    "ListThingsInBillingGroupResponseTypeDef",
+    "ListThingsInThingGroupResponseTypeDef",
+    "RegisterCACertificateResponseTypeDef",
+    "RegisterCertificateResponseTypeDef",
+    "RegisterCertificateWithoutCAResponseTypeDef",
+    "RegisterThingResponseTypeDef",
+    "SetDefaultAuthorizerResponseTypeDef",
+    "StartAuditMitigationActionsTaskResponseTypeDef",
+    "StartDetectMitigationActionsTaskResponseTypeDef",
+    "StartOnDemandAuditTaskResponseTypeDef",
+    "StartThingRegistrationTaskResponseTypeDef",
+    "TestInvokeAuthorizerResponseTypeDef",
+    "TransferCertificateResponseTypeDef",
+    "UpdateAuthorizerResponseTypeDef",
+    "UpdateBillingGroupResponseTypeDef",
+    "UpdateCustomMetricResponseTypeDef",
+    "UpdateDimensionResponseTypeDef",
+    "UpdateDomainConfigurationResponseTypeDef",
+    "UpdateDynamicThingGroupResponseTypeDef",
+    "UpdateMitigationActionResponseTypeDef",
+    "UpdateRoleAliasResponseTypeDef",
+    "UpdateScheduledAuditResponseTypeDef",
+    "UpdateStreamResponseTypeDef",
+    "UpdateThingGroupResponseTypeDef",
+    "ThingGroupPropertiesOutputTypeDef",
+    "AttributePayloadUnionTypeDef",
     "CreateThingRequestRequestTypeDef",
     "ThingGroupPropertiesTypeDef",
     "UpdateThingRequestRequestTypeDef",
     "ListAuditMitigationActionsExecutionsResponseTypeDef",
     "ListAuditMitigationActionsTasksResponseTypeDef",
+    "AuditMitigationActionsTaskTargetUnionTypeDef",
     "StartAuditMitigationActionsTaskRequestRequestTypeDef",
     "DescribeAccountAuditConfigurationResponseTypeDef",
     "UpdateAccountAuditConfigurationRequestRequestTypeDef",
     "ListAuditTasksResponseTypeDef",
-    "TestAuthorizationRequestRequestTypeDef",
+    "AuthInfoUnionTypeDef",
     "DescribeAuthorizerResponseTypeDef",
     "DescribeDefaultAuthorizerResponseTypeDef",
     "ListAuthorizersResponseTypeDef",
     "AwsJobAbortConfigTypeDef",
     "AwsJobExponentialRolloutRateTypeDef",
+    "BehaviorCriteriaOutputTypeDef",
     "BehaviorCriteriaTypeDef",
     "GetBehaviorModelTrainingSummariesResponseTypeDef",
     "MetricToRetainTypeDef",
     "DescribeBillingGroupResponseTypeDef",
     "UpdateBillingGroupRequestRequestTypeDef",
+    "CodeSigningSignatureTypeDef",
+    "MqttContextTypeDef",
     "GetBucketsAggregationResponseTypeDef",
     "BucketsAggregationTypeTypeDef",
     "CACertificateDescriptionTypeDef",
     "ListCACertificatesResponseTypeDef",
     "CertificateDescriptionTypeDef",
     "ListCertificatesByCAResponseTypeDef",
     "ListCertificatesResponseTypeDef",
-    "CustomCodeSigningTypeDef",
+    "CustomCodeSigningOutputTypeDef",
     "DescribeEventConfigurationsResponseTypeDef",
     "UpdateEventConfigurationsRequestRequestTypeDef",
+    "ListAuditMitigationActionsTasksRequestRequestTypeDef",
+    "ListAuditTasksRequestRequestTypeDef",
+    "ListDetectMitigationActionsExecutionsRequestRequestTypeDef",
+    "ListDetectMitigationActionsTasksRequestRequestTypeDef",
+    "ListMetricValuesRequestRequestTypeDef",
+    "ListViolationEventsRequestRequestTypeDef",
+    "ViolationEventOccurrenceRangeTypeDef",
     "CreateAuthorizerRequestRequestTypeDef",
     "CreateBillingGroupRequestRequestTypeDef",
     "CreateCustomMetricRequestRequestTypeDef",
     "CreateDimensionRequestRequestTypeDef",
     "CreateFleetMetricRequestRequestTypeDef",
     "CreatePolicyRequestRequestTypeDef",
     "CreateRoleAliasRequestRequestTypeDef",
     "CreateScheduledAuditRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDomainConfigurationRequestRequestTypeDef",
     "UpdateDomainConfigurationRequestRequestTypeDef",
+    "SchedulingConfigOutputTypeDef",
     "SchedulingConfigTypeDef",
     "CreateKeysAndCertificateResponseTypeDef",
     "CreateProvisioningClaimResponseTypeDef",
     "CreateProvisioningTemplateRequestRequestTypeDef",
     "DescribeProvisioningTemplateResponseTypeDef",
     "UpdateProvisioningTemplateRequestRequestTypeDef",
     "CreateThingTypeRequestRequestTypeDef",
@@ -621,38 +585,99 @@
     "RegisterCACertificateRequestRequestTypeDef",
     "UpdateCACertificateRequestRequestTypeDef",
     "DescribeDomainConfigurationResponseTypeDef",
     "DescribeManagedJobTemplateResponseTypeDef",
     "DescribeRoleAliasResponseTypeDef",
     "DescribeThingTypeResponseTypeDef",
     "ThingTypeDefinitionTypeDef",
+    "ThingTypePropertiesUnionTypeDef",
     "DestinationTypeDef",
     "ListDetectMitigationActionsExecutionsResponseTypeDef",
-    "StartDetectMitigationActionsTaskRequestRequestTypeDef",
+    "DetectMitigationActionsTaskTargetUnionTypeDef",
     "ListDomainConfigurationsResponseTypeDef",
     "DynamoDBv2ActionTypeDef",
     "GetEffectivePoliciesResponseTypeDef",
     "ExponentialRolloutRateTypeDef",
+    "ThingGroupIndexingConfigurationOutputTypeDef",
     "ThingGroupIndexingConfigurationTypeDef",
     "StreamFileTypeDef",
     "FileLocationTypeDef",
     "ListFleetMetricsResponseTypeDef",
+    "GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef",
+    "ListActiveViolationsRequestListActiveViolationsPaginateTypeDef",
+    "ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef",
+    "ListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef",
+    "ListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef",
+    "ListAuditTasksRequestListAuditTasksPaginateTypeDef",
+    "ListAuthorizersRequestListAuthorizersPaginateTypeDef",
+    "ListBillingGroupsRequestListBillingGroupsPaginateTypeDef",
+    "ListCACertificatesRequestListCACertificatesPaginateTypeDef",
+    "ListCertificatesByCARequestListCertificatesByCAPaginateTypeDef",
+    "ListCertificatesRequestListCertificatesPaginateTypeDef",
+    "ListCustomMetricsRequestListCustomMetricsPaginateTypeDef",
+    "ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef",
+    "ListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef",
+    "ListDimensionsRequestListDimensionsPaginateTypeDef",
+    "ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef",
+    "ListFleetMetricsRequestListFleetMetricsPaginateTypeDef",
+    "ListIndicesRequestListIndicesPaginateTypeDef",
+    "ListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef",
+    "ListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef",
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
+    "ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef",
+    "ListMetricValuesRequestListMetricValuesPaginateTypeDef",
+    "ListMitigationActionsRequestListMitigationActionsPaginateTypeDef",
+    "ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef",
+    "ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef",
+    "ListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
+    "ListPackagesRequestListPackagesPaginateTypeDef",
+    "ListPoliciesRequestListPoliciesPaginateTypeDef",
+    "ListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef",
+    "ListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef",
+    "ListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef",
+    "ListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef",
+    "ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef",
+    "ListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef",
+    "ListRoleAliasesRequestListRoleAliasesPaginateTypeDef",
+    "ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef",
+    "ListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef",
+    "ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef",
+    "ListStreamsRequestListStreamsPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef",
+    "ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef",
+    "ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef",
+    "ListThingGroupsRequestListThingGroupsPaginateTypeDef",
+    "ListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef",
+    "ListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef",
+    "ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef",
+    "ListThingTypesRequestListThingTypesPaginateTypeDef",
+    "ListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef",
+    "ListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef",
+    "ListThingsRequestListThingsPaginateTypeDef",
+    "ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef",
+    "ListTopicRulesRequestListTopicRulesPaginateTypeDef",
+    "ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef",
+    "ListViolationEventsRequestListViolationEventsPaginateTypeDef",
     "GetPackageConfigurationResponseTypeDef",
     "UpdatePackageConfigurationRequestRequestTypeDef",
     "GetPercentilesResponseTypeDef",
     "GetStatisticsResponseTypeDef",
     "ListBillingGroupsResponseTypeDef",
     "ListThingGroupsForThingResponseTypeDef",
     "ListThingGroupsResponseTypeDef",
     "ThingGroupMetadataTypeDef",
     "HttpAuthorizationTypeDef",
+    "ThingIndexingConfigurationOutputTypeDef",
     "ThingIndexingConfigurationTypeDef",
     "JobExecutionTypeDef",
     "JobExecutionSummaryForJobTypeDef",
     "JobExecutionSummaryForThingTypeDef",
+    "JobExecutionsRetryConfigOutputTypeDef",
     "JobExecutionsRetryConfigTypeDef",
     "ListJobsResponseTypeDef",
     "ListJobTemplatesResponseTypeDef",
     "ListManagedJobTemplatesResponseTypeDef",
     "ListMitigationActionsResponseTypeDef",
     "ListOTAUpdatesResponseTypeDef",
     "ListOutgoingCertificatesResponseTypeDef",
@@ -668,55 +693,73 @@
     "SecurityProfileTargetMappingTypeDef",
     "ListThingsResponseTypeDef",
     "ListTopicRulesResponseTypeDef",
     "LocationActionTypeDef",
     "LogTargetConfigurationTypeDef",
     "SetV2LoggingLevelRequestRequestTypeDef",
     "SetLoggingOptionsRequestRequestTypeDef",
+    "MitigationActionParamsOutputTypeDef",
     "MitigationActionParamsTypeDef",
+    "MqttHeadersOutputTypeDef",
     "MqttHeadersTypeDef",
     "ResourceIdentifierTypeDef",
-    "TestInvokeAuthorizerRequestRequestTypeDef",
     "ThingDocumentTypeDef",
+    "TimestreamActionOutputTypeDef",
     "TimestreamActionTypeDef",
     "TopicRuleDestinationConfigurationTypeDef",
     "TopicRuleDestinationSummaryTypeDef",
     "TopicRuleDestinationTypeDef",
     "ValidateSecurityProfileBehaviorsResponseTypeDef",
+    "AbortConfigUnionTypeDef",
     "ListMetricValuesResponseTypeDef",
     "DeniedTypeDef",
+    "PutAssetPropertyValueEntryOutputTypeDef",
     "PutAssetPropertyValueEntryTypeDef",
     "CreateDynamicThingGroupRequestRequestTypeDef",
     "CreateThingGroupRequestRequestTypeDef",
+    "ThingGroupPropertiesUnionTypeDef",
     "UpdateDynamicThingGroupRequestRequestTypeDef",
     "UpdateThingGroupRequestRequestTypeDef",
+    "TestAuthorizationRequestRequestTypeDef",
     "AwsJobExecutionsRolloutConfigTypeDef",
+    "BehaviorOutputTypeDef",
     "BehaviorTypeDef",
+    "CustomCodeSigningTypeDef",
+    "TestInvokeAuthorizerRequestRequestTypeDef",
     "GetBucketsAggregationRequestRequestTypeDef",
     "DescribeCACertificateResponseTypeDef",
     "DescribeCertificateResponseTypeDef",
+    "StartDetectMitigationActionsTaskRequestRequestTypeDef",
+    "ViolationEventOccurrenceRangeUnionTypeDef",
+    "SchedulingConfigUnionTypeDef",
     "ListThingTypesResponseTypeDef",
     "StartSigningJobParameterTypeDef",
     "JobExecutionsRolloutConfigTypeDef",
+    "ThingGroupIndexingConfigurationUnionTypeDef",
     "CreateStreamRequestRequestTypeDef",
     "StreamInfoTypeDef",
     "UpdateStreamRequestRequestTypeDef",
     "DescribeThingGroupResponseTypeDef",
+    "HttpActionOutputTypeDef",
     "HttpActionTypeDef",
     "GetIndexingConfigurationResponseTypeDef",
+    "ThingIndexingConfigurationUnionTypeDef",
     "UpdateIndexingConfigurationRequestRequestTypeDef",
     "DescribeJobExecutionResponseTypeDef",
     "ListJobExecutionsForJobResponseTypeDef",
     "ListJobExecutionsForThingResponseTypeDef",
+    "JobExecutionsRetryConfigUnionTypeDef",
     "ListSecurityProfilesForTargetResponseTypeDef",
     "ListV2LoggingLevelsResponseTypeDef",
-    "CreateMitigationActionRequestRequestTypeDef",
     "DescribeMitigationActionResponseTypeDef",
     "MitigationActionTypeDef",
+    "CreateMitigationActionRequestRequestTypeDef",
+    "MitigationActionParamsUnionTypeDef",
     "UpdateMitigationActionRequestRequestTypeDef",
+    "RepublishActionOutputTypeDef",
     "RepublishActionTypeDef",
     "AuditSuppressionTypeDef",
     "CreateAuditSuppressionRequestRequestTypeDef",
     "DeleteAuditSuppressionRequestRequestTypeDef",
     "DescribeAuditSuppressionRequestRequestTypeDef",
     "DescribeAuditSuppressionResponseTypeDef",
     "ListAuditFindingsRequestListAuditFindingsPaginateTypeDef",
@@ -728,52 +771,58 @@
     "UpdateAuditSuppressionRequestRequestTypeDef",
     "SearchIndexResponseTypeDef",
     "CreateTopicRuleDestinationRequestRequestTypeDef",
     "ListTopicRuleDestinationsResponseTypeDef",
     "CreateTopicRuleDestinationResponseTypeDef",
     "GetTopicRuleDestinationResponseTypeDef",
     "AuthResultTypeDef",
+    "IotSiteWiseActionOutputTypeDef",
     "IotSiteWiseActionTypeDef",
     "ActiveViolationTypeDef",
-    "CreateSecurityProfileRequestRequestTypeDef",
     "DescribeSecurityProfileResponseTypeDef",
-    "UpdateSecurityProfileRequestRequestTypeDef",
     "UpdateSecurityProfileResponseTypeDef",
-    "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
     "ViolationEventTypeDef",
+    "BehaviorUnionTypeDef",
+    "CodeSigningOutputTypeDef",
     "CodeSigningTypeDef",
     "CreateJobRequestRequestTypeDef",
     "CreateJobTemplateRequestRequestTypeDef",
     "DescribeJobTemplateResponseTypeDef",
     "JobTypeDef",
     "UpdateJobRequestRequestTypeDef",
     "DescribeStreamResponseTypeDef",
     "DescribeAuditMitigationActionsTaskResponseTypeDef",
     "DetectMitigationActionsTaskSummaryTypeDef",
     "ListAuditSuppressionsResponseTypeDef",
     "AuditFindingTypeDef",
     "ListRelatedResourcesForAuditFindingResponseTypeDef",
     "TestAuthorizationResponseTypeDef",
+    "ActionOutputTypeDef",
     "ActionTypeDef",
     "ListActiveViolationsResponseTypeDef",
     "ListViolationEventsResponseTypeDef",
+    "CreateSecurityProfileRequestRequestTypeDef",
+    "UpdateSecurityProfileRequestRequestTypeDef",
+    "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
+    "OTAUpdateFileOutputTypeDef",
     "OTAUpdateFileTypeDef",
     "DescribeJobResponseTypeDef",
     "DescribeDetectMitigationActionsTaskResponseTypeDef",
     "ListDetectMitigationActionsTasksResponseTypeDef",
     "DescribeAuditFindingResponseTypeDef",
     "ListAuditFindingsResponseTypeDef",
-    "TopicRulePayloadTypeDef",
     "TopicRuleTypeDef",
-    "CreateOTAUpdateRequestRequestTypeDef",
+    "TopicRulePayloadTypeDef",
     "OTAUpdateInfoTypeDef",
+    "OTAUpdateFileUnionTypeDef",
+    "GetTopicRuleResponseTypeDef",
     "CreateTopicRuleRequestRequestTypeDef",
     "ReplaceTopicRuleRequestRequestTypeDef",
-    "GetTopicRuleResponseTypeDef",
     "GetOTAUpdateResponseTypeDef",
+    "CreateOTAUpdateRequestRequestTypeDef",
 )
 
 AbortCriteriaTypeDef = TypedDict(
     "AbortCriteriaTypeDef",
     {
         "failureType": JobExecutionFailureTypeType,
         "action": Literal["CANCEL"],
@@ -948,33 +997,35 @@
 )
 
 
 class IotEventsActionTypeDef(_RequiredIotEventsActionTypeDef, _OptionalIotEventsActionTypeDef):
     pass
 
 
-_RequiredKafkaActionTypeDef = TypedDict(
-    "_RequiredKafkaActionTypeDef",
+_RequiredKafkaActionOutputTypeDef = TypedDict(
+    "_RequiredKafkaActionOutputTypeDef",
     {
         "destinationArn": str,
         "topic": str,
-        "clientProperties": Mapping[str, str],
+        "clientProperties": Dict[str, str],
     },
 )
-_OptionalKafkaActionTypeDef = TypedDict(
-    "_OptionalKafkaActionTypeDef",
+_OptionalKafkaActionOutputTypeDef = TypedDict(
+    "_OptionalKafkaActionOutputTypeDef",
     {
         "key": str,
         "partition": str,
     },
     total=False,
 )
 
 
-class KafkaActionTypeDef(_RequiredKafkaActionTypeDef, _OptionalKafkaActionTypeDef):
+class KafkaActionOutputTypeDef(
+    _RequiredKafkaActionOutputTypeDef, _OptionalKafkaActionOutputTypeDef
+):
     pass
 
 
 _RequiredKinesisActionTypeDef = TypedDict(
     "_RequiredKinesisActionTypeDef",
     {
         "roleArn": str,
@@ -1099,23 +1150,45 @@
 
 class StepFunctionsActionTypeDef(
     _RequiredStepFunctionsActionTypeDef, _OptionalStepFunctionsActionTypeDef
 ):
     pass
 
 
-MetricValueTypeDef = TypedDict(
-    "MetricValueTypeDef",
+_RequiredKafkaActionTypeDef = TypedDict(
+    "_RequiredKafkaActionTypeDef",
+    {
+        "destinationArn": str,
+        "topic": str,
+        "clientProperties": Mapping[str, str],
+    },
+)
+_OptionalKafkaActionTypeDef = TypedDict(
+    "_OptionalKafkaActionTypeDef",
+    {
+        "key": str,
+        "partition": str,
+    },
+    total=False,
+)
+
+
+class KafkaActionTypeDef(_RequiredKafkaActionTypeDef, _OptionalKafkaActionTypeDef):
+    pass
+
+
+MetricValueOutputTypeDef = TypedDict(
+    "MetricValueOutputTypeDef",
     {
         "count": int,
-        "cidrs": Sequence[str],
-        "ports": Sequence[int],
+        "cidrs": List[str],
+        "ports": List[int],
         "number": float,
-        "numbers": Sequence[float],
-        "strings": Sequence[str],
+        "numbers": List[float],
+        "strings": List[str],
     },
     total=False,
 )
 
 ViolationEventAdditionalInfoTypeDef = TypedDict(
     "ViolationEventAdditionalInfoTypeDef",
     {
@@ -1143,14 +1216,36 @@
         "thingName": str,
         "thingArn": str,
         "overrideDynamicGroups": bool,
     },
     total=False,
 )
 
+_RequiredAddThingsToThingGroupParamsOutputTypeDef = TypedDict(
+    "_RequiredAddThingsToThingGroupParamsOutputTypeDef",
+    {
+        "thingGroupNames": List[str],
+    },
+)
+_OptionalAddThingsToThingGroupParamsOutputTypeDef = TypedDict(
+    "_OptionalAddThingsToThingGroupParamsOutputTypeDef",
+    {
+        "overrideDynamicGroups": bool,
+    },
+    total=False,
+)
+
+
+class AddThingsToThingGroupParamsOutputTypeDef(
+    _RequiredAddThingsToThingGroupParamsOutputTypeDef,
+    _OptionalAddThingsToThingGroupParamsOutputTypeDef,
+):
+    pass
+
+
 _RequiredAddThingsToThingGroupParamsTypeDef = TypedDict(
     "_RequiredAddThingsToThingGroupParamsTypeDef",
     {
         "thingGroupNames": Sequence[str],
     },
 )
 _OptionalAddThingsToThingGroupParamsTypeDef = TypedDict(
@@ -1164,14 +1259,35 @@
 
 class AddThingsToThingGroupParamsTypeDef(
     _RequiredAddThingsToThingGroupParamsTypeDef, _OptionalAddThingsToThingGroupParamsTypeDef
 ):
     pass
 
 
+_RequiredAggregationTypeOutputTypeDef = TypedDict(
+    "_RequiredAggregationTypeOutputTypeDef",
+    {
+        "name": AggregationTypeNameType,
+    },
+)
+_OptionalAggregationTypeOutputTypeDef = TypedDict(
+    "_OptionalAggregationTypeOutputTypeDef",
+    {
+        "values": List[str],
+    },
+    total=False,
+)
+
+
+class AggregationTypeOutputTypeDef(
+    _RequiredAggregationTypeOutputTypeDef, _OptionalAggregationTypeOutputTypeDef
+):
+    pass
+
+
 _RequiredAggregationTypeTypeDef = TypedDict(
     "_RequiredAggregationTypeTypeDef",
     {
         "name": AggregationTypeNameType,
     },
 )
 _OptionalAggregationTypeTypeDef = TypedDict(
@@ -1256,21 +1372,22 @@
 class AssociateTargetsWithJobRequestRequestTypeDef(
     _RequiredAssociateTargetsWithJobRequestRequestTypeDef,
     _OptionalAssociateTargetsWithJobRequestRequestTypeDef,
 ):
     pass
 
 
-AssociateTargetsWithJobResponseTypeDef = TypedDict(
-    "AssociateTargetsWithJobResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "jobArn": str,
-        "jobId": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AttachPolicyRequestRequestTypeDef = TypedDict(
     "AttachPolicyRequestRequestTypeDef",
     {
         "policyName": str,
@@ -1298,14 +1415,23 @@
     "AttachThingPrincipalRequestRequestTypeDef",
     {
         "thingName": str,
         "principal": str,
     },
 )
 
+AttributePayloadOutputTypeDef = TypedDict(
+    "AttributePayloadOutputTypeDef",
+    {
+        "attributes": Dict[str, str],
+        "merge": bool,
+    },
+    total=False,
+)
+
 AttributePayloadTypeDef = TypedDict(
     "AttributePayloadTypeDef",
     {
         "attributes": Mapping[str, str],
         "merge": bool,
     },
     total=False,
@@ -1355,24 +1481,34 @@
         "taskId": str,
         "startTime": datetime,
         "taskStatus": AuditMitigationActionsTaskStatusType,
     },
     total=False,
 )
 
-AuditMitigationActionsTaskTargetTypeDef = TypedDict(
-    "AuditMitigationActionsTaskTargetTypeDef",
+AuditMitigationActionsTaskTargetOutputTypeDef = TypedDict(
+    "AuditMitigationActionsTaskTargetOutputTypeDef",
     {
         "auditTaskId": str,
         "findingIds": List[str],
         "auditCheckToReasonCodeFilter": Dict[str, List[str]],
     },
     total=False,
 )
 
+AuditMitigationActionsTaskTargetTypeDef = TypedDict(
+    "AuditMitigationActionsTaskTargetTypeDef",
+    {
+        "auditTaskId": str,
+        "findingIds": Sequence[str],
+        "auditCheckToReasonCodeFilter": Mapping[str, Sequence[str]],
+    },
+    total=False,
+)
+
 AuditNotificationTargetTypeDef = TypedDict(
     "AuditNotificationTargetTypeDef",
     {
         "targetArn": str,
         "roleArn": str,
         "enabled": bool,
     },
@@ -1385,14 +1521,33 @@
         "taskId": str,
         "taskStatus": AuditTaskStatusType,
         "taskType": AuditTaskTypeType,
     },
     total=False,
 )
 
+_RequiredAuthInfoOutputTypeDef = TypedDict(
+    "_RequiredAuthInfoOutputTypeDef",
+    {
+        "resources": List[str],
+    },
+)
+_OptionalAuthInfoOutputTypeDef = TypedDict(
+    "_OptionalAuthInfoOutputTypeDef",
+    {
+        "actionType": ActionTypeType,
+    },
+    total=False,
+)
+
+
+class AuthInfoOutputTypeDef(_RequiredAuthInfoOutputTypeDef, _OptionalAuthInfoOutputTypeDef):
+    pass
+
+
 _RequiredAuthInfoTypeDef = TypedDict(
     "_RequiredAuthInfoTypeDef",
     {
         "resources": Sequence[str],
     },
 )
 _OptionalAuthInfoTypeDef = TypedDict(
@@ -1489,14 +1644,27 @@
     "StatisticalThresholdTypeDef",
     {
         "statistic": str,
     },
     total=False,
 )
 
+MetricValueTypeDef = TypedDict(
+    "MetricValueTypeDef",
+    {
+        "count": int,
+        "cidrs": Sequence[str],
+        "ports": Sequence[int],
+        "number": float,
+        "numbers": Sequence[float],
+        "strings": Sequence[str],
+    },
+    total=False,
+)
+
 BehaviorModelTrainingSummaryTypeDef = TypedDict(
     "BehaviorModelTrainingSummaryTypeDef",
     {
         "securityProfileName": str,
         "behaviorName": str,
         "trainingDataCollectionStartDate": datetime,
         "modelStatus": ModelStatusType,
@@ -1537,14 +1705,15 @@
     "BillingGroupPropertiesTypeDef",
     {
         "billingGroupDescription": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BucketTypeDef = TypedDict(
     "BucketTypeDef",
     {
         "keyValue": str,
         "count": int,
     },
     total=False,
@@ -1650,24 +1819,14 @@
 
 class CancelJobRequestRequestTypeDef(
     _RequiredCancelJobRequestRequestTypeDef, _OptionalCancelJobRequestRequestTypeDef
 ):
     pass
 
 
-CancelJobResponseTypeDef = TypedDict(
-    "CancelJobResponseTypeDef",
-    {
-        "jobArn": str,
-        "jobId": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TransferDataTypeDef = TypedDict(
     "TransferDataTypeDef",
     {
         "transferMessage": str,
         "rejectReason": str,
         "transferDate": datetime,
         "acceptDate": datetime,
@@ -1693,18 +1852,18 @@
     {
         "certificateName": str,
         "inlineDocument": str,
     },
     total=False,
 )
 
-CodeSigningSignatureTypeDef = TypedDict(
-    "CodeSigningSignatureTypeDef",
+CodeSigningSignatureOutputTypeDef = TypedDict(
+    "CodeSigningSignatureOutputTypeDef",
     {
-        "inlineDocument": Union[str, bytes, IO[Any], StreamingBody],
+        "inlineDocument": bytes,
     },
     total=False,
 )
 
 ConfigurationTypeDef = TypedDict(
     "ConfigurationTypeDef",
     {
@@ -1716,14 +1875,15 @@
 ConfirmTopicRuleDestinationRequestRequestTypeDef = TypedDict(
     "ConfirmTopicRuleDestinationRequestRequestTypeDef",
     {
         "confirmationToken": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalTagTypeDef = TypedDict(
@@ -1735,33 +1895,14 @@
 )
 
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
 
-CreateAuthorizerResponseTypeDef = TypedDict(
-    "CreateAuthorizerResponseTypeDef",
-    {
-        "authorizerName": str,
-        "authorizerArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateBillingGroupResponseTypeDef = TypedDict(
-    "CreateBillingGroupResponseTypeDef",
-    {
-        "billingGroupName": str,
-        "billingGroupArn": str,
-        "billingGroupId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateCertificateFromCsrRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCertificateFromCsrRequestRequestTypeDef",
     {
         "certificateSigningRequest": str,
     },
 )
 _OptionalCreateCertificateFromCsrRequestRequestTypeDef = TypedDict(
@@ -1776,81 +1917,22 @@
 class CreateCertificateFromCsrRequestRequestTypeDef(
     _RequiredCreateCertificateFromCsrRequestRequestTypeDef,
     _OptionalCreateCertificateFromCsrRequestRequestTypeDef,
 ):
     pass
 
 
-CreateCertificateFromCsrResponseTypeDef = TypedDict(
-    "CreateCertificateFromCsrResponseTypeDef",
-    {
-        "certificateArn": str,
-        "certificateId": str,
-        "certificatePem": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateCustomMetricResponseTypeDef = TypedDict(
-    "CreateCustomMetricResponseTypeDef",
-    {
-        "metricName": str,
-        "metricArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDimensionResponseTypeDef = TypedDict(
-    "CreateDimensionResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TlsConfigTypeDef = TypedDict(
     "TlsConfigTypeDef",
     {
         "securityPolicy": str,
     },
     total=False,
 )
 
-CreateDomainConfigurationResponseTypeDef = TypedDict(
-    "CreateDomainConfigurationResponseTypeDef",
-    {
-        "domainConfigurationName": str,
-        "domainConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDynamicThingGroupResponseTypeDef = TypedDict(
-    "CreateDynamicThingGroupResponseTypeDef",
-    {
-        "thingGroupName": str,
-        "thingGroupArn": str,
-        "thingGroupId": str,
-        "indexName": str,
-        "queryString": str,
-        "queryVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFleetMetricResponseTypeDef = TypedDict(
-    "CreateFleetMetricResponseTypeDef",
-    {
-        "metricName": str,
-        "metricArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PresignedUrlConfigTypeDef = TypedDict(
     "PresignedUrlConfigTypeDef",
     {
         "roleArn": str,
         "expiresInSec": int,
     },
     total=False,
@@ -1860,41 +1942,22 @@
     "TimeoutConfigTypeDef",
     {
         "inProgressTimeoutInMinutes": int,
     },
     total=False,
 )
 
-CreateJobResponseTypeDef = TypedDict(
-    "CreateJobResponseTypeDef",
-    {
-        "jobArn": str,
-        "jobId": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MaintenanceWindowTypeDef = TypedDict(
     "MaintenanceWindowTypeDef",
     {
         "startTime": str,
         "durationInMinutes": int,
     },
 )
 
-CreateJobTemplateResponseTypeDef = TypedDict(
-    "CreateJobTemplateResponseTypeDef",
-    {
-        "jobTemplateArn": str,
-        "jobTemplateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateKeysAndCertificateRequestRequestTypeDef = TypedDict(
     "CreateKeysAndCertificateRequestRequestTypeDef",
     {
         "setAsActive": bool,
     },
     total=False,
 )
@@ -1904,35 +1967,14 @@
     {
         "PublicKey": str,
         "PrivateKey": str,
     },
     total=False,
 )
 
-CreateMitigationActionResponseTypeDef = TypedDict(
-    "CreateMitigationActionResponseTypeDef",
-    {
-        "actionArn": str,
-        "actionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateOTAUpdateResponseTypeDef = TypedDict(
-    "CreateOTAUpdateResponseTypeDef",
-    {
-        "otaUpdateId": str,
-        "awsIotJobId": str,
-        "otaUpdateArn": str,
-        "awsIotJobArn": str,
-        "otaUpdateStatus": OTAUpdateStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePackageRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackageRequestRequestTypeDef",
     {
         "packageName": str,
     },
 )
 _OptionalCreatePackageRequestRequestTypeDef = TypedDict(
@@ -1948,24 +1990,14 @@
 
 class CreatePackageRequestRequestTypeDef(
     _RequiredCreatePackageRequestRequestTypeDef, _OptionalCreatePackageRequestRequestTypeDef
 ):
     pass
 
 
-CreatePackageResponseTypeDef = TypedDict(
-    "CreatePackageResponseTypeDef",
-    {
-        "packageName": str,
-        "packageArn": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePackageVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackageVersionRequestRequestTypeDef",
     {
         "packageName": str,
         "versionName": str,
     },
 )
@@ -1984,39 +2016,14 @@
 class CreatePackageVersionRequestRequestTypeDef(
     _RequiredCreatePackageVersionRequestRequestTypeDef,
     _OptionalCreatePackageVersionRequestRequestTypeDef,
 ):
     pass
 
 
-CreatePackageVersionResponseTypeDef = TypedDict(
-    "CreatePackageVersionResponseTypeDef",
-    {
-        "packageVersionArn": str,
-        "packageName": str,
-        "versionName": str,
-        "description": str,
-        "attributes": Dict[str, str],
-        "status": PackageVersionStatusType,
-        "errorReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePolicyResponseTypeDef = TypedDict(
-    "CreatePolicyResponseTypeDef",
-    {
-        "policyName": str,
-        "policyArn": str,
-        "policyDocument": str,
-        "policyVersionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePolicyVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePolicyVersionRequestRequestTypeDef",
     {
         "policyName": str,
         "policyDocument": str,
     },
 )
@@ -2032,25 +2039,14 @@
 class CreatePolicyVersionRequestRequestTypeDef(
     _RequiredCreatePolicyVersionRequestRequestTypeDef,
     _OptionalCreatePolicyVersionRequestRequestTypeDef,
 ):
     pass
 
 
-CreatePolicyVersionResponseTypeDef = TypedDict(
-    "CreatePolicyVersionResponseTypeDef",
-    {
-        "policyArn": str,
-        "policyDocument": str,
-        "policyVersionId": str,
-        "isDefaultVersion": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateProvisioningClaimRequestRequestTypeDef = TypedDict(
     "CreateProvisioningClaimRequestRequestTypeDef",
     {
         "templateName": str,
     },
 )
 
@@ -2069,24 +2065,14 @@
 )
 
 
 class ProvisioningHookTypeDef(_RequiredProvisioningHookTypeDef, _OptionalProvisioningHookTypeDef):
     pass
 
 
-CreateProvisioningTemplateResponseTypeDef = TypedDict(
-    "CreateProvisioningTemplateResponseTypeDef",
-    {
-        "templateArn": str,
-        "templateName": str,
-        "defaultVersionId": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateProvisioningTemplateVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProvisioningTemplateVersionRequestRequestTypeDef",
     {
         "templateName": str,
         "templateBody": str,
     },
 )
@@ -2102,101 +2088,23 @@
 class CreateProvisioningTemplateVersionRequestRequestTypeDef(
     _RequiredCreateProvisioningTemplateVersionRequestRequestTypeDef,
     _OptionalCreateProvisioningTemplateVersionRequestRequestTypeDef,
 ):
     pass
 
 
-CreateProvisioningTemplateVersionResponseTypeDef = TypedDict(
-    "CreateProvisioningTemplateVersionResponseTypeDef",
-    {
-        "templateArn": str,
-        "templateName": str,
-        "versionId": int,
-        "isDefaultVersion": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateRoleAliasResponseTypeDef = TypedDict(
-    "CreateRoleAliasResponseTypeDef",
-    {
-        "roleAlias": str,
-        "roleAliasArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateScheduledAuditResponseTypeDef = TypedDict(
-    "CreateScheduledAuditResponseTypeDef",
-    {
-        "scheduledAuditArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSecurityProfileResponseTypeDef = TypedDict(
-    "CreateSecurityProfileResponseTypeDef",
-    {
-        "securityProfileName": str,
-        "securityProfileArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateStreamResponseTypeDef = TypedDict(
-    "CreateStreamResponseTypeDef",
-    {
-        "streamId": str,
-        "streamArn": str,
-        "description": str,
-        "streamVersion": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateThingGroupResponseTypeDef = TypedDict(
-    "CreateThingGroupResponseTypeDef",
-    {
-        "thingGroupName": str,
-        "thingGroupArn": str,
-        "thingGroupId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateThingResponseTypeDef = TypedDict(
-    "CreateThingResponseTypeDef",
-    {
-        "thingName": str,
-        "thingArn": str,
-        "thingId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ThingTypePropertiesTypeDef = TypedDict(
     "ThingTypePropertiesTypeDef",
     {
         "thingTypeDescription": str,
         "searchableAttributes": Sequence[str],
     },
     total=False,
 )
 
-CreateThingTypeResponseTypeDef = TypedDict(
-    "CreateThingTypeResponseTypeDef",
-    {
-        "thingTypeName": str,
-        "thingTypeArn": str,
-        "thingTypeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteAccountAuditConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteAccountAuditConfigurationRequestRequestTypeDef",
     {
         "deleteScheduledAudits": bool,
     },
     total=False,
 )
@@ -2703,54 +2611,28 @@
 DescribeCustomMetricRequestRequestTypeDef = TypedDict(
     "DescribeCustomMetricRequestRequestTypeDef",
     {
         "metricName": str,
     },
 )
 
-DescribeCustomMetricResponseTypeDef = TypedDict(
-    "DescribeCustomMetricResponseTypeDef",
-    {
-        "metricName": str,
-        "metricArn": str,
-        "metricType": CustomMetricTypeType,
-        "displayName": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
     "DescribeDetectMitigationActionsTaskRequestRequestTypeDef",
     {
         "taskId": str,
     },
 )
 
 DescribeDimensionRequestRequestTypeDef = TypedDict(
     "DescribeDimensionRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-DescribeDimensionResponseTypeDef = TypedDict(
-    "DescribeDimensionResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "type": Literal["TOPIC_FILTER"],
-        "stringValues": List[str],
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDomainConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeDomainConfigurationRequestRequestTypeDef",
     {
         "domainConfigurationName": str,
     },
 )
 
@@ -2768,46 +2650,28 @@
     "DescribeEndpointRequestRequestTypeDef",
     {
         "endpointType": str,
     },
     total=False,
 )
 
-DescribeEndpointResponseTypeDef = TypedDict(
-    "DescribeEndpointResponseTypeDef",
-    {
-        "endpointAddress": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeFleetMetricRequestRequestTypeDef = TypedDict(
     "DescribeFleetMetricRequestRequestTypeDef",
     {
         "metricName": str,
     },
 )
 
 DescribeIndexRequestRequestTypeDef = TypedDict(
     "DescribeIndexRequestRequestTypeDef",
     {
         "indexName": str,
     },
 )
 
-DescribeIndexResponseTypeDef = TypedDict(
-    "DescribeIndexResponseTypeDef",
-    {
-        "indexName": str,
-        "indexStatus": IndexStatusType,
-        "schema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeJobExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeJobExecutionRequestRequestTypeDef",
     {
         "jobId": str,
         "thingName": str,
     },
 )
@@ -2893,25 +2757,14 @@
     "DescribeProvisioningTemplateVersionRequestRequestTypeDef",
     {
         "templateName": str,
         "versionId": int,
     },
 )
 
-DescribeProvisioningTemplateVersionResponseTypeDef = TypedDict(
-    "DescribeProvisioningTemplateVersionResponseTypeDef",
-    {
-        "versionId": int,
-        "creationDate": datetime,
-        "templateBody": str,
-        "isDefaultVersion": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeRoleAliasRequestRequestTypeDef = TypedDict(
     "DescribeRoleAliasRequestRequestTypeDef",
     {
         "roleAlias": str,
     },
 )
 
@@ -2932,27 +2785,14 @@
 DescribeScheduledAuditRequestRequestTypeDef = TypedDict(
     "DescribeScheduledAuditRequestRequestTypeDef",
     {
         "scheduledAuditName": str,
     },
 )
 
-DescribeScheduledAuditResponseTypeDef = TypedDict(
-    "DescribeScheduledAuditResponseTypeDef",
-    {
-        "frequency": AuditFrequencyType,
-        "dayOfMonth": str,
-        "dayOfWeek": DayOfWeekType,
-        "targetCheckNames": List[str],
-        "scheduledAuditName": str,
-        "scheduledAuditArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeSecurityProfileRequestRequestTypeDef = TypedDict(
     "DescribeSecurityProfileRequestRequestTypeDef",
     {
         "securityProfileName": str,
     },
 )
 
@@ -2973,55 +2813,21 @@
 DescribeThingRegistrationTaskRequestRequestTypeDef = TypedDict(
     "DescribeThingRegistrationTaskRequestRequestTypeDef",
     {
         "taskId": str,
     },
 )
 
-DescribeThingRegistrationTaskResponseTypeDef = TypedDict(
-    "DescribeThingRegistrationTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "templateBody": str,
-        "inputFileBucket": str,
-        "inputFileKey": str,
-        "roleArn": str,
-        "status": StatusType,
-        "message": str,
-        "successCount": int,
-        "failureCount": int,
-        "percentageProgress": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeThingRequestRequestTypeDef = TypedDict(
     "DescribeThingRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 
-DescribeThingResponseTypeDef = TypedDict(
-    "DescribeThingResponseTypeDef",
-    {
-        "defaultClientId": str,
-        "thingName": str,
-        "thingId": str,
-        "thingArn": str,
-        "thingTypeName": str,
-        "attributes": Dict[str, str],
-        "version": int,
-        "billingGroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeThingTypeRequestRequestTypeDef = TypedDict(
     "DescribeThingTypeRequestRequestTypeDef",
     {
         "thingTypeName": str,
     },
 )
 
@@ -3031,14 +2837,23 @@
         "deprecated": bool,
         "deprecationDate": datetime,
         "creationDate": datetime,
     },
     total=False,
 )
 
+ThingTypePropertiesOutputTypeDef = TypedDict(
+    "ThingTypePropertiesOutputTypeDef",
+    {
+        "thingTypeDescription": str,
+        "searchableAttributes": List[str],
+    },
+    total=False,
+)
+
 S3DestinationTypeDef = TypedDict(
     "S3DestinationTypeDef",
     {
         "bucket": str,
         "prefix": str,
     },
     total=False,
@@ -3098,32 +2913,42 @@
         "actionsExecuted": int,
         "actionsSkipped": int,
         "actionsFailed": int,
     },
     total=False,
 )
 
-DetectMitigationActionsTaskTargetTypeDef = TypedDict(
-    "DetectMitigationActionsTaskTargetTypeDef",
+DetectMitigationActionsTaskTargetOutputTypeDef = TypedDict(
+    "DetectMitigationActionsTaskTargetOutputTypeDef",
     {
         "violationIds": List[str],
         "securityProfileName": str,
         "behaviorName": str,
     },
     total=False,
 )
 
-ViolationEventOccurrenceRangeTypeDef = TypedDict(
-    "ViolationEventOccurrenceRangeTypeDef",
+ViolationEventOccurrenceRangeOutputTypeDef = TypedDict(
+    "ViolationEventOccurrenceRangeOutputTypeDef",
     {
         "startTime": datetime,
         "endTime": datetime,
     },
 )
 
+DetectMitigationActionsTaskTargetTypeDef = TypedDict(
+    "DetectMitigationActionsTaskTargetTypeDef",
+    {
+        "violationIds": Sequence[str],
+        "securityProfileName": str,
+        "behaviorName": str,
+    },
+    total=False,
+)
+
 DisableTopicRuleRequestRequestTypeDef = TypedDict(
     "DisableTopicRuleRequestRequestTypeDef",
     {
         "ruleName": str,
     },
 )
 
@@ -3150,21 +2975,14 @@
         "policyName": str,
         "policyArn": str,
         "policyDocument": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnableIoTLoggingParamsTypeDef = TypedDict(
     "EnableIoTLoggingParamsTypeDef",
     {
         "roleArnForLogging": str,
         "logLevel": LogLevelType,
     },
 )
@@ -3227,23 +3045,22 @@
     {
         "metricName": str,
         "metricArn": str,
     },
     total=False,
 )
 
-GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef = (
-    TypedDict(
-        "GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef",
-        {
-            "securityProfileName": str,
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
 )
 
 GetBehaviorModelTrainingSummariesRequestRequestTypeDef = TypedDict(
     "GetBehaviorModelTrainingSummariesRequestRequestTypeDef",
     {
         "securityProfileName": str,
         "maxResults": int,
@@ -3271,22 +3088,14 @@
 
 class GetCardinalityRequestRequestTypeDef(
     _RequiredGetCardinalityRequestRequestTypeDef, _OptionalGetCardinalityRequestRequestTypeDef
 ):
     pass
 
 
-GetCardinalityResponseTypeDef = TypedDict(
-    "GetCardinalityResponseTypeDef",
-    {
-        "cardinality": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetEffectivePoliciesRequestRequestTypeDef = TypedDict(
     "GetEffectivePoliciesRequestRequestTypeDef",
     {
         "principal": str,
         "cognitoIdentityPoolId": str,
         "thingName": str,
     },
@@ -3296,31 +3105,14 @@
 GetJobDocumentRequestRequestTypeDef = TypedDict(
     "GetJobDocumentRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 
-GetJobDocumentResponseTypeDef = TypedDict(
-    "GetJobDocumentResponseTypeDef",
-    {
-        "document": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetLoggingOptionsResponseTypeDef = TypedDict(
-    "GetLoggingOptionsResponseTypeDef",
-    {
-        "roleArn": str,
-        "logLevel": LogLevelType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetOTAUpdateRequestRequestTypeDef = TypedDict(
     "GetOTAUpdateRequestRequestTypeDef",
     {
         "otaUpdateId": str,
     },
 )
 
@@ -3336,51 +3128,22 @@
 GetPackageRequestRequestTypeDef = TypedDict(
     "GetPackageRequestRequestTypeDef",
     {
         "packageName": str,
     },
 )
 
-GetPackageResponseTypeDef = TypedDict(
-    "GetPackageResponseTypeDef",
-    {
-        "packageName": str,
-        "packageArn": str,
-        "description": str,
-        "defaultVersionName": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPackageVersionRequestRequestTypeDef = TypedDict(
     "GetPackageVersionRequestRequestTypeDef",
     {
         "packageName": str,
         "versionName": str,
     },
 )
 
-GetPackageVersionResponseTypeDef = TypedDict(
-    "GetPackageVersionResponseTypeDef",
-    {
-        "packageVersionArn": str,
-        "packageName": str,
-        "versionName": str,
-        "description": str,
-        "attributes": Dict[str, str],
-        "status": PackageVersionStatusType,
-        "errorReason": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetPercentilesRequestRequestTypeDef = TypedDict(
     "_RequiredGetPercentilesRequestRequestTypeDef",
     {
         "queryString": str,
     },
 )
 _OptionalGetPercentilesRequestRequestTypeDef = TypedDict(
@@ -3413,59 +3176,22 @@
 GetPolicyRequestRequestTypeDef = TypedDict(
     "GetPolicyRequestRequestTypeDef",
     {
         "policyName": str,
     },
 )
 
-GetPolicyResponseTypeDef = TypedDict(
-    "GetPolicyResponseTypeDef",
-    {
-        "policyName": str,
-        "policyArn": str,
-        "policyDocument": str,
-        "defaultVersionId": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "generationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPolicyVersionRequestRequestTypeDef = TypedDict(
     "GetPolicyVersionRequestRequestTypeDef",
     {
         "policyName": str,
         "policyVersionId": str,
     },
 )
 
-GetPolicyVersionResponseTypeDef = TypedDict(
-    "GetPolicyVersionResponseTypeDef",
-    {
-        "policyArn": str,
-        "policyName": str,
-        "policyDocument": str,
-        "policyVersionId": str,
-        "isDefaultVersion": bool,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "generationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetRegistrationCodeResponseTypeDef = TypedDict(
-    "GetRegistrationCodeResponseTypeDef",
-    {
-        "registrationCode": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetStatisticsRequestRequestTypeDef",
     {
         "queryString": str,
     },
 )
 _OptionalGetStatisticsRequestRequestTypeDef = TypedDict(
@@ -3510,24 +3236,14 @@
 GetTopicRuleRequestRequestTypeDef = TypedDict(
     "GetTopicRuleRequestRequestTypeDef",
     {
         "ruleName": str,
     },
 )
 
-GetV2LoggingOptionsResponseTypeDef = TypedDict(
-    "GetV2LoggingOptionsResponseTypeDef",
-    {
-        "roleArn": str,
-        "defaultLogLevel": LogLevelType,
-        "disableAllLogs": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GroupNameAndArnTypeDef = TypedDict(
     "GroupNameAndArnTypeDef",
     {
         "groupName": str,
         "groupArn": str,
     },
     total=False,
@@ -3578,18 +3294,26 @@
     "HttpUrlDestinationSummaryTypeDef",
     {
         "confirmationUrl": str,
     },
     total=False,
 )
 
+IndexingFilterOutputTypeDef = TypedDict(
+    "IndexingFilterOutputTypeDef",
+    {
+        "namedShadowNames": List[str],
+    },
+    total=False,
+)
+
 IndexingFilterTypeDef = TypedDict(
     "IndexingFilterTypeDef",
     {
-        "namedShadowNames": List[str],
+        "namedShadowNames": Sequence[str],
     },
     total=False,
 )
 
 IssuerCertificateIdentifierTypeDef = TypedDict(
     "IssuerCertificateIdentifierTypeDef",
     {
@@ -3676,64 +3400,28 @@
     "ScheduledJobRolloutTypeDef",
     {
         "startTime": str,
     },
     total=False,
 )
 
-ListActiveViolationsRequestListActiveViolationsPaginateTypeDef = TypedDict(
-    "ListActiveViolationsRequestListActiveViolationsPaginateTypeDef",
-    {
-        "thingName": str,
-        "securityProfileName": str,
-        "behaviorCriteriaType": BehaviorCriteriaTypeType,
-        "listSuppressedAlerts": bool,
-        "verificationState": VerificationStateType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListActiveViolationsRequestRequestTypeDef = TypedDict(
     "ListActiveViolationsRequestRequestTypeDef",
     {
         "thingName": str,
         "securityProfileName": str,
         "behaviorCriteriaType": BehaviorCriteriaTypeType,
         "listSuppressedAlerts": bool,
         "verificationState": VerificationStateType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef",
-    {
-        "target": str,
-    },
-)
-_OptionalListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef",
-    {
-        "recursive": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef(
-    _RequiredListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef,
-    _OptionalListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAttachedPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListAttachedPoliciesRequestRequestTypeDef",
     {
         "target": str,
     },
 )
 _OptionalListAttachedPoliciesRequestRequestTypeDef = TypedDict(
@@ -3750,38 +3438,14 @@
 class ListAttachedPoliciesRequestRequestTypeDef(
     _RequiredListAttachedPoliciesRequestRequestTypeDef,
     _OptionalListAttachedPoliciesRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef",
-    {
-        "taskId": str,
-        "findingId": str,
-    },
-)
-_OptionalListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef",
-    {
-        "actionStatus": AuditMitigationActionsExecutionStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef(
-    _RequiredListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef,
-    _OptionalListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAuditMitigationActionsExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredListAuditMitigationActionsExecutionsRequestRequestTypeDef",
     {
         "taskId": str,
         "findingId": str,
     },
 )
@@ -3799,201 +3463,46 @@
 class ListAuditMitigationActionsExecutionsRequestRequestTypeDef(
     _RequiredListAuditMitigationActionsExecutionsRequestRequestTypeDef,
     _OptionalListAuditMitigationActionsExecutionsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef = TypedDict(
-    "_RequiredListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef = TypedDict(
-    "_OptionalListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef",
-    {
-        "auditTaskId": str,
-        "findingId": str,
-        "taskStatus": AuditMitigationActionsTaskStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef(
-    _RequiredListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef,
-    _OptionalListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListAuditMitigationActionsTasksRequestRequestTypeDef = TypedDict(
-    "_RequiredListAuditMitigationActionsTasksRequestRequestTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListAuditMitigationActionsTasksRequestRequestTypeDef = TypedDict(
-    "_OptionalListAuditMitigationActionsTasksRequestRequestTypeDef",
-    {
-        "auditTaskId": str,
-        "findingId": str,
-        "taskStatus": AuditMitigationActionsTaskStatusType,
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-
-class ListAuditMitigationActionsTasksRequestRequestTypeDef(
-    _RequiredListAuditMitigationActionsTasksRequestRequestTypeDef,
-    _OptionalListAuditMitigationActionsTasksRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredListAuditTasksRequestListAuditTasksPaginateTypeDef = TypedDict(
-    "_RequiredListAuditTasksRequestListAuditTasksPaginateTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListAuditTasksRequestListAuditTasksPaginateTypeDef = TypedDict(
-    "_OptionalListAuditTasksRequestListAuditTasksPaginateTypeDef",
-    {
-        "taskType": AuditTaskTypeType,
-        "taskStatus": AuditTaskStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAuditTasksRequestListAuditTasksPaginateTypeDef(
-    _RequiredListAuditTasksRequestListAuditTasksPaginateTypeDef,
-    _OptionalListAuditTasksRequestListAuditTasksPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListAuditTasksRequestRequestTypeDef = TypedDict(
-    "_RequiredListAuditTasksRequestRequestTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListAuditTasksRequestRequestTypeDef = TypedDict(
-    "_OptionalListAuditTasksRequestRequestTypeDef",
-    {
-        "taskType": AuditTaskTypeType,
-        "taskStatus": AuditTaskStatusType,
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-
-class ListAuditTasksRequestRequestTypeDef(
-    _RequiredListAuditTasksRequestRequestTypeDef, _OptionalListAuditTasksRequestRequestTypeDef
-):
-    pass
-
-
-ListAuthorizersRequestListAuthorizersPaginateTypeDef = TypedDict(
-    "ListAuthorizersRequestListAuthorizersPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "status": AuthorizerStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAuthorizersRequestRequestTypeDef = TypedDict(
     "ListAuthorizersRequestRequestTypeDef",
     {
         "pageSize": int,
         "marker": str,
         "ascendingOrder": bool,
         "status": AuthorizerStatusType,
     },
     total=False,
 )
 
-ListBillingGroupsRequestListBillingGroupsPaginateTypeDef = TypedDict(
-    "ListBillingGroupsRequestListBillingGroupsPaginateTypeDef",
-    {
-        "namePrefixFilter": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListBillingGroupsRequestRequestTypeDef = TypedDict(
     "ListBillingGroupsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "namePrefixFilter": str,
     },
     total=False,
 )
 
-ListCACertificatesRequestListCACertificatesPaginateTypeDef = TypedDict(
-    "ListCACertificatesRequestListCACertificatesPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "templateName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCACertificatesRequestRequestTypeDef = TypedDict(
     "ListCACertificatesRequestRequestTypeDef",
     {
         "pageSize": int,
         "marker": str,
         "ascendingOrder": bool,
         "templateName": str,
     },
     total=False,
 )
 
-_RequiredListCertificatesByCARequestListCertificatesByCAPaginateTypeDef = TypedDict(
-    "_RequiredListCertificatesByCARequestListCertificatesByCAPaginateTypeDef",
-    {
-        "caCertificateId": str,
-    },
-)
-_OptionalListCertificatesByCARequestListCertificatesByCAPaginateTypeDef = TypedDict(
-    "_OptionalListCertificatesByCARequestListCertificatesByCAPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListCertificatesByCARequestListCertificatesByCAPaginateTypeDef(
-    _RequiredListCertificatesByCARequestListCertificatesByCAPaginateTypeDef,
-    _OptionalListCertificatesByCARequestListCertificatesByCAPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListCertificatesByCARequestRequestTypeDef = TypedDict(
     "_RequiredListCertificatesByCARequestRequestTypeDef",
     {
         "caCertificateId": str,
     },
 )
 _OptionalListCertificatesByCARequestRequestTypeDef = TypedDict(
@@ -4010,244 +3519,70 @@
 class ListCertificatesByCARequestRequestTypeDef(
     _RequiredListCertificatesByCARequestRequestTypeDef,
     _OptionalListCertificatesByCARequestRequestTypeDef,
 ):
     pass
 
 
-ListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
-    "ListCertificatesRequestListCertificatesPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCertificatesRequestRequestTypeDef = TypedDict(
     "ListCertificatesRequestRequestTypeDef",
     {
         "pageSize": int,
         "marker": str,
         "ascendingOrder": bool,
     },
     total=False,
 )
 
-ListCustomMetricsRequestListCustomMetricsPaginateTypeDef = TypedDict(
-    "ListCustomMetricsRequestListCustomMetricsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCustomMetricsRequestRequestTypeDef = TypedDict(
     "ListCustomMetricsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListCustomMetricsResponseTypeDef = TypedDict(
-    "ListCustomMetricsResponseTypeDef",
-    {
-        "metricNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef = TypedDict(
-    "ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef",
-    {
-        "taskId": str,
-        "violationId": str,
-        "thingName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListDetectMitigationActionsExecutionsRequestRequestTypeDef = TypedDict(
-    "ListDetectMitigationActionsExecutionsRequestRequestTypeDef",
-    {
-        "taskId": str,
-        "violationId": str,
-        "thingName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-_RequiredListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef = TypedDict(
-    "_RequiredListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef = TypedDict(
-    "_OptionalListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef(
-    _RequiredListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef,
-    _OptionalListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListDetectMitigationActionsTasksRequestRequestTypeDef = TypedDict(
-    "_RequiredListDetectMitigationActionsTasksRequestRequestTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListDetectMitigationActionsTasksRequestRequestTypeDef = TypedDict(
-    "_OptionalListDetectMitigationActionsTasksRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-
-class ListDetectMitigationActionsTasksRequestRequestTypeDef(
-    _RequiredListDetectMitigationActionsTasksRequestRequestTypeDef,
-    _OptionalListDetectMitigationActionsTasksRequestRequestTypeDef,
-):
-    pass
-
-
-ListDimensionsRequestListDimensionsPaginateTypeDef = TypedDict(
-    "ListDimensionsRequestListDimensionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDimensionsRequestRequestTypeDef = TypedDict(
     "ListDimensionsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListDimensionsResponseTypeDef = TypedDict(
-    "ListDimensionsResponseTypeDef",
-    {
-        "dimensionNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef = TypedDict(
-    "ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef",
-    {
-        "serviceType": ServiceTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDomainConfigurationsRequestRequestTypeDef = TypedDict(
     "ListDomainConfigurationsRequestRequestTypeDef",
     {
         "marker": str,
         "pageSize": int,
         "serviceType": ServiceTypeType,
     },
     total=False,
 )
 
-ListFleetMetricsRequestListFleetMetricsPaginateTypeDef = TypedDict(
-    "ListFleetMetricsRequestListFleetMetricsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFleetMetricsRequestRequestTypeDef = TypedDict(
     "ListFleetMetricsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListIndicesRequestListIndicesPaginateTypeDef = TypedDict(
-    "ListIndicesRequestListIndicesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListIndicesRequestRequestTypeDef = TypedDict(
     "ListIndicesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListIndicesResponseTypeDef = TypedDict(
-    "ListIndicesResponseTypeDef",
-    {
-        "indexNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef = TypedDict(
-    "_RequiredListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef",
-    {
-        "jobId": str,
-    },
-)
-_OptionalListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef = TypedDict(
-    "_OptionalListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef",
-    {
-        "status": JobExecutionStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef(
-    _RequiredListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef,
-    _OptionalListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListJobExecutionsForJobRequestRequestTypeDef = TypedDict(
     "_RequiredListJobExecutionsForJobRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 _OptionalListJobExecutionsForJobRequestRequestTypeDef = TypedDict(
@@ -4264,39 +3599,14 @@
 class ListJobExecutionsForJobRequestRequestTypeDef(
     _RequiredListJobExecutionsForJobRequestRequestTypeDef,
     _OptionalListJobExecutionsForJobRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef = TypedDict(
-    "_RequiredListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef",
-    {
-        "thingName": str,
-    },
-)
-_OptionalListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef = TypedDict(
-    "_OptionalListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef",
-    {
-        "status": JobExecutionStatusType,
-        "namespaceId": str,
-        "jobId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef(
-    _RequiredListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef,
-    _OptionalListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListJobExecutionsForThingRequestRequestTypeDef = TypedDict(
     "_RequiredListJobExecutionsForThingRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 _OptionalListJobExecutionsForThingRequestRequestTypeDef = TypedDict(
@@ -4315,67 +3625,37 @@
 class ListJobExecutionsForThingRequestRequestTypeDef(
     _RequiredListJobExecutionsForThingRequestRequestTypeDef,
     _OptionalListJobExecutionsForThingRequestRequestTypeDef,
 ):
     pass
 
 
-ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListJobTemplatesRequestRequestTypeDef = TypedDict(
     "ListJobTemplatesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "ListJobsRequestListJobsPaginateTypeDef",
-    {
-        "status": JobStatusType,
-        "targetSelection": TargetSelectionType,
-        "thingGroupName": str,
-        "thingGroupId": str,
-        "namespaceId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "status": JobStatusType,
         "targetSelection": TargetSelectionType,
         "maxResults": int,
         "nextToken": str,
         "thingGroupName": str,
         "thingGroupId": str,
         "namespaceId": str,
     },
     total=False,
 )
 
-ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef = TypedDict(
-    "ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef",
-    {
-        "templateName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListManagedJobTemplatesRequestRequestTypeDef = TypedDict(
     "ListManagedJobTemplatesRequestRequestTypeDef",
     {
         "templateName": str,
         "maxResults": int,
         "nextToken": str,
     },
@@ -4390,77 +3670,14 @@
         "description": str,
         "environments": List[str],
         "templateVersion": str,
     },
     total=False,
 )
 
-_RequiredListMetricValuesRequestListMetricValuesPaginateTypeDef = TypedDict(
-    "_RequiredListMetricValuesRequestListMetricValuesPaginateTypeDef",
-    {
-        "thingName": str,
-        "metricName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListMetricValuesRequestListMetricValuesPaginateTypeDef = TypedDict(
-    "_OptionalListMetricValuesRequestListMetricValuesPaginateTypeDef",
-    {
-        "dimensionName": str,
-        "dimensionValueOperator": DimensionValueOperatorType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListMetricValuesRequestListMetricValuesPaginateTypeDef(
-    _RequiredListMetricValuesRequestListMetricValuesPaginateTypeDef,
-    _OptionalListMetricValuesRequestListMetricValuesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListMetricValuesRequestRequestTypeDef = TypedDict(
-    "_RequiredListMetricValuesRequestRequestTypeDef",
-    {
-        "thingName": str,
-        "metricName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListMetricValuesRequestRequestTypeDef = TypedDict(
-    "_OptionalListMetricValuesRequestRequestTypeDef",
-    {
-        "dimensionName": str,
-        "dimensionValueOperator": DimensionValueOperatorType,
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-
-class ListMetricValuesRequestRequestTypeDef(
-    _RequiredListMetricValuesRequestRequestTypeDef, _OptionalListMetricValuesRequestRequestTypeDef
-):
-    pass
-
-
-ListMitigationActionsRequestListMitigationActionsPaginateTypeDef = TypedDict(
-    "ListMitigationActionsRequestListMitigationActionsPaginateTypeDef",
-    {
-        "actionType": MitigationActionTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMitigationActionsRequestRequestTypeDef = TypedDict(
     "ListMitigationActionsRequestRequestTypeDef",
     {
         "actionType": MitigationActionTypeType,
         "maxResults": int,
         "nextToken": str,
     },
@@ -4473,23 +3690,14 @@
         "actionName": str,
         "actionArn": str,
         "creationDate": datetime,
     },
     total=False,
 )
 
-ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef = TypedDict(
-    "ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef",
-    {
-        "otaUpdateStatus": OTAUpdateStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOTAUpdatesRequestRequestTypeDef = TypedDict(
     "ListOTAUpdatesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "otaUpdateStatus": OTAUpdateStatusType,
     },
@@ -4502,23 +3710,14 @@
         "otaUpdateId": str,
         "otaUpdateArn": str,
         "creationDate": datetime,
     },
     total=False,
 )
 
-ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef = TypedDict(
-    "ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOutgoingCertificatesRequestRequestTypeDef = TypedDict(
     "ListOutgoingCertificatesRequestRequestTypeDef",
     {
         "pageSize": int,
         "marker": str,
         "ascendingOrder": bool,
     },
@@ -4534,37 +3733,14 @@
         "transferDate": datetime,
         "transferMessage": str,
         "creationDate": datetime,
     },
     total=False,
 )
 
-_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
-    {
-        "packageName": str,
-    },
-)
-_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
-    {
-        "status": PackageVersionStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPackageVersionsRequestListPackageVersionsPaginateTypeDef(
-    _RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
-    _OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPackageVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListPackageVersionsRequestRequestTypeDef",
     {
         "packageName": str,
     },
 )
 _OptionalListPackageVersionsRequestRequestTypeDef = TypedDict(
@@ -4593,22 +3769,14 @@
         "status": PackageVersionStatusType,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
     },
     total=False,
 )
 
-ListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
-    "ListPackagesRequestListPackagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPackagesRequestRequestTypeDef = TypedDict(
     "ListPackagesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -4621,56 +3789,24 @@
         "defaultVersionName": str,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
     },
     total=False,
 )
 
-ListPoliciesRequestListPoliciesPaginateTypeDef = TypedDict(
-    "ListPoliciesRequestListPoliciesPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPoliciesRequestRequestTypeDef = TypedDict(
     "ListPoliciesRequestRequestTypeDef",
     {
         "marker": str,
         "pageSize": int,
         "ascendingOrder": bool,
     },
     total=False,
 )
 
-_RequiredListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef = TypedDict(
-    "_RequiredListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef",
-    {
-        "policyName": str,
-    },
-)
-_OptionalListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef = TypedDict(
-    "_OptionalListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef(
-    _RequiredListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef,
-    _OptionalListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPolicyPrincipalsRequestRequestTypeDef = TypedDict(
     "_RequiredListPolicyPrincipalsRequestRequestTypeDef",
     {
         "policyName": str,
     },
 )
 _OptionalListPolicyPrincipalsRequestRequestTypeDef = TypedDict(
@@ -4687,23 +3823,14 @@
 class ListPolicyPrincipalsRequestRequestTypeDef(
     _RequiredListPolicyPrincipalsRequestRequestTypeDef,
     _OptionalListPolicyPrincipalsRequestRequestTypeDef,
 ):
     pass
 
 
-ListPolicyPrincipalsResponseTypeDef = TypedDict(
-    "ListPolicyPrincipalsResponseTypeDef",
-    {
-        "principals": List[str],
-        "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListPolicyVersionsRequestRequestTypeDef = TypedDict(
     "ListPolicyVersionsRequestRequestTypeDef",
     {
         "policyName": str,
     },
 )
 
@@ -4713,37 +3840,14 @@
         "versionId": str,
         "isDefaultVersion": bool,
         "createDate": datetime,
     },
     total=False,
 )
 
-_RequiredListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef",
-    {
-        "principal": str,
-    },
-)
-_OptionalListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef(
-    _RequiredListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef,
-    _OptionalListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPrincipalPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListPrincipalPoliciesRequestRequestTypeDef",
     {
         "principal": str,
     },
 )
 _OptionalListPrincipalPoliciesRequestRequestTypeDef = TypedDict(
@@ -4760,36 +3864,14 @@
 class ListPrincipalPoliciesRequestRequestTypeDef(
     _RequiredListPrincipalPoliciesRequestRequestTypeDef,
     _OptionalListPrincipalPoliciesRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef = TypedDict(
-    "_RequiredListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef",
-    {
-        "principal": str,
-    },
-)
-_OptionalListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef = TypedDict(
-    "_OptionalListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef(
-    _RequiredListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef,
-    _OptionalListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPrincipalThingsRequestRequestTypeDef = TypedDict(
     "_RequiredListPrincipalThingsRequestRequestTypeDef",
     {
         "principal": str,
     },
 )
 _OptionalListPrincipalThingsRequestRequestTypeDef = TypedDict(
@@ -4805,45 +3887,14 @@
 class ListPrincipalThingsRequestRequestTypeDef(
     _RequiredListPrincipalThingsRequestRequestTypeDef,
     _OptionalListPrincipalThingsRequestRequestTypeDef,
 ):
     pass
 
 
-ListPrincipalThingsResponseTypeDef = TypedDict(
-    "ListPrincipalThingsResponseTypeDef",
-    {
-        "things": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef",
-    {
-        "templateName": str,
-    },
-)
-_OptionalListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef(
-    _RequiredListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef,
-    _OptionalListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListProvisioningTemplateVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListProvisioningTemplateVersionsRequestRequestTypeDef",
     {
         "templateName": str,
     },
 )
 _OptionalListProvisioningTemplateVersionsRequestRequestTypeDef = TypedDict(
@@ -4869,22 +3920,14 @@
         "versionId": int,
         "creationDate": datetime,
         "isDefaultVersion": bool,
     },
     total=False,
 )
 
-ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef = TypedDict(
-    "ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProvisioningTemplatesRequestRequestTypeDef = TypedDict(
     "ListProvisioningTemplatesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -4900,36 +3943,14 @@
         "lastModifiedDate": datetime,
         "enabled": bool,
         "type": TemplateTypeType,
     },
     total=False,
 )
 
-_RequiredListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef = TypedDict(
-    "_RequiredListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef",
-    {
-        "findingId": str,
-    },
-)
-_OptionalListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef = TypedDict(
-    "_OptionalListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef(
-    _RequiredListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef,
-    _OptionalListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRelatedResourcesForAuditFindingRequestRequestTypeDef = TypedDict(
     "_RequiredListRelatedResourcesForAuditFindingRequestRequestTypeDef",
     {
         "findingId": str,
     },
 )
 _OptionalListRelatedResourcesForAuditFindingRequestRequestTypeDef = TypedDict(
@@ -4945,50 +3966,24 @@
 class ListRelatedResourcesForAuditFindingRequestRequestTypeDef(
     _RequiredListRelatedResourcesForAuditFindingRequestRequestTypeDef,
     _OptionalListRelatedResourcesForAuditFindingRequestRequestTypeDef,
 ):
     pass
 
 
-ListRoleAliasesRequestListRoleAliasesPaginateTypeDef = TypedDict(
-    "ListRoleAliasesRequestListRoleAliasesPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRoleAliasesRequestRequestTypeDef = TypedDict(
     "ListRoleAliasesRequestRequestTypeDef",
     {
         "pageSize": int,
         "marker": str,
         "ascendingOrder": bool,
     },
     total=False,
 )
 
-ListRoleAliasesResponseTypeDef = TypedDict(
-    "ListRoleAliasesResponseTypeDef",
-    {
-        "roleAliases": List[str],
-        "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef = TypedDict(
-    "ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListScheduledAuditsRequestRequestTypeDef = TypedDict(
     "ListScheduledAuditsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -5002,41 +3997,14 @@
         "frequency": AuditFrequencyType,
         "dayOfMonth": str,
         "dayOfWeek": DayOfWeekType,
     },
     total=False,
 )
 
-_RequiredListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef",
-        {
-            "securityProfileTargetArn": str,
-        },
-    )
-)
-_OptionalListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef",
-        {
-            "recursive": bool,
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-
-class ListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef(
-    _RequiredListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef,
-    _OptionalListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSecurityProfilesForTargetRequestRequestTypeDef = TypedDict(
     "_RequiredListSecurityProfilesForTargetRequestRequestTypeDef",
     {
         "securityProfileTargetArn": str,
     },
 )
 _OptionalListSecurityProfilesForTargetRequestRequestTypeDef = TypedDict(
@@ -5053,24 +4021,14 @@
 class ListSecurityProfilesForTargetRequestRequestTypeDef(
     _RequiredListSecurityProfilesForTargetRequestRequestTypeDef,
     _OptionalListSecurityProfilesForTargetRequestRequestTypeDef,
 ):
     pass
 
 
-ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef = TypedDict(
-    "ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef",
-    {
-        "dimensionName": str,
-        "metricName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSecurityProfilesRequestRequestTypeDef = TypedDict(
     "ListSecurityProfilesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "dimensionName": str,
         "metricName": str,
@@ -5082,23 +4040,14 @@
     "SecurityProfileIdentifierTypeDef",
     {
         "name": str,
         "arn": str,
     },
 )
 
-ListStreamsRequestListStreamsPaginateTypeDef = TypedDict(
-    "ListStreamsRequestListStreamsPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStreamsRequestRequestTypeDef = TypedDict(
     "ListStreamsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "ascendingOrder": bool,
     },
@@ -5112,36 +4061,14 @@
         "streamArn": str,
         "streamVersion": int,
         "description": str,
     },
     total=False,
 )
 
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -5156,36 +4083,14 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef = TypedDict(
-    "_RequiredListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef",
-    {
-        "policyName": str,
-    },
-)
-_OptionalListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef = TypedDict(
-    "_OptionalListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef(
-    _RequiredListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
-    _OptionalListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTargetsForPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredListTargetsForPolicyRequestRequestTypeDef",
     {
         "policyName": str,
     },
 )
 _OptionalListTargetsForPolicyRequestRequestTypeDef = TypedDict(
@@ -5201,49 +4106,14 @@
 class ListTargetsForPolicyRequestRequestTypeDef(
     _RequiredListTargetsForPolicyRequestRequestTypeDef,
     _OptionalListTargetsForPolicyRequestRequestTypeDef,
 ):
     pass
 
 
-ListTargetsForPolicyResponseTypeDef = TypedDict(
-    "ListTargetsForPolicyResponseTypeDef",
-    {
-        "targets": List[str],
-        "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef = (
-    TypedDict(
-        "_RequiredListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef",
-        {
-            "securityProfileName": str,
-        },
-    )
-)
-_OptionalListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef = (
-    TypedDict(
-        "_OptionalListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef",
-        {
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-
-class ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef(
-    _RequiredListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef,
-    _OptionalListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTargetsForSecurityProfileRequestRequestTypeDef = TypedDict(
     "_RequiredListTargetsForSecurityProfileRequestRequestTypeDef",
     {
         "securityProfileName": str,
     },
 )
 _OptionalListTargetsForSecurityProfileRequestRequestTypeDef = TypedDict(
@@ -5266,36 +4136,14 @@
 SecurityProfileTargetTypeDef = TypedDict(
     "SecurityProfileTargetTypeDef",
     {
         "arn": str,
     },
 )
 
-_RequiredListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef = TypedDict(
-    "_RequiredListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef",
-    {
-        "thingName": str,
-    },
-)
-_OptionalListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef = TypedDict(
-    "_OptionalListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef(
-    _RequiredListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef,
-    _OptionalListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListThingGroupsForThingRequestRequestTypeDef = TypedDict(
     "_RequiredListThingGroupsForThingRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 _OptionalListThingGroupsForThingRequestRequestTypeDef = TypedDict(
@@ -5311,59 +4159,26 @@
 class ListThingGroupsForThingRequestRequestTypeDef(
     _RequiredListThingGroupsForThingRequestRequestTypeDef,
     _OptionalListThingGroupsForThingRequestRequestTypeDef,
 ):
     pass
 
 
-ListThingGroupsRequestListThingGroupsPaginateTypeDef = TypedDict(
-    "ListThingGroupsRequestListThingGroupsPaginateTypeDef",
-    {
-        "parentGroup": str,
-        "namePrefixFilter": str,
-        "recursive": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListThingGroupsRequestRequestTypeDef = TypedDict(
     "ListThingGroupsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "parentGroup": str,
         "namePrefixFilter": str,
         "recursive": bool,
     },
     total=False,
 )
 
-_RequiredListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef = TypedDict(
-    "_RequiredListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef",
-    {
-        "thingName": str,
-    },
-)
-_OptionalListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef = TypedDict(
-    "_OptionalListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef(
-    _RequiredListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef,
-    _OptionalListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListThingPrincipalsRequestRequestTypeDef = TypedDict(
     "_RequiredListThingPrincipalsRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 _OptionalListThingPrincipalsRequestRequestTypeDef = TypedDict(
@@ -5379,46 +4194,14 @@
 class ListThingPrincipalsRequestRequestTypeDef(
     _RequiredListThingPrincipalsRequestRequestTypeDef,
     _OptionalListThingPrincipalsRequestRequestTypeDef,
 ):
     pass
 
 
-ListThingPrincipalsResponseTypeDef = TypedDict(
-    "ListThingPrincipalsResponseTypeDef",
-    {
-        "principals": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef = TypedDict(
-    "_RequiredListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef",
-    {
-        "taskId": str,
-        "reportType": ReportTypeType,
-    },
-)
-_OptionalListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef = TypedDict(
-    "_OptionalListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef(
-    _RequiredListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef,
-    _OptionalListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListThingRegistrationTaskReportsRequestRequestTypeDef = TypedDict(
     "_RequiredListThingRegistrationTaskReportsRequestRequestTypeDef",
     {
         "taskId": str,
         "reportType": ReportTypeType,
     },
 )
@@ -5435,93 +4218,34 @@
 class ListThingRegistrationTaskReportsRequestRequestTypeDef(
     _RequiredListThingRegistrationTaskReportsRequestRequestTypeDef,
     _OptionalListThingRegistrationTaskReportsRequestRequestTypeDef,
 ):
     pass
 
 
-ListThingRegistrationTaskReportsResponseTypeDef = TypedDict(
-    "ListThingRegistrationTaskReportsResponseTypeDef",
-    {
-        "resourceLinks": List[str],
-        "reportType": ReportTypeType,
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef = TypedDict(
-    "ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef",
-    {
-        "status": StatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListThingRegistrationTasksRequestRequestTypeDef = TypedDict(
     "ListThingRegistrationTasksRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "status": StatusType,
     },
     total=False,
 )
 
-ListThingRegistrationTasksResponseTypeDef = TypedDict(
-    "ListThingRegistrationTasksResponseTypeDef",
-    {
-        "taskIds": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListThingTypesRequestListThingTypesPaginateTypeDef = TypedDict(
-    "ListThingTypesRequestListThingTypesPaginateTypeDef",
-    {
-        "thingTypeName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListThingTypesRequestRequestTypeDef = TypedDict(
     "ListThingTypesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "thingTypeName": str,
     },
     total=False,
 )
 
-_RequiredListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef = TypedDict(
-    "_RequiredListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef",
-    {
-        "billingGroupName": str,
-    },
-)
-_OptionalListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef = TypedDict(
-    "_OptionalListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef(
-    _RequiredListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef,
-    _OptionalListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListThingsInBillingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredListThingsInBillingGroupRequestRequestTypeDef",
     {
         "billingGroupName": str,
     },
 )
 _OptionalListThingsInBillingGroupRequestRequestTypeDef = TypedDict(
@@ -5537,46 +4261,14 @@
 class ListThingsInBillingGroupRequestRequestTypeDef(
     _RequiredListThingsInBillingGroupRequestRequestTypeDef,
     _OptionalListThingsInBillingGroupRequestRequestTypeDef,
 ):
     pass
 
 
-ListThingsInBillingGroupResponseTypeDef = TypedDict(
-    "ListThingsInBillingGroupResponseTypeDef",
-    {
-        "things": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef = TypedDict(
-    "_RequiredListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef",
-    {
-        "thingGroupName": str,
-    },
-)
-_OptionalListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef = TypedDict(
-    "_OptionalListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef",
-    {
-        "recursive": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef(
-    _RequiredListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef,
-    _OptionalListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListThingsInThingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredListThingsInThingGroupRequestRequestTypeDef",
     {
         "thingGroupName": str,
     },
 )
 _OptionalListThingsInThingGroupRequestRequestTypeDef = TypedDict(
@@ -5593,35 +4285,14 @@
 class ListThingsInThingGroupRequestRequestTypeDef(
     _RequiredListThingsInThingGroupRequestRequestTypeDef,
     _OptionalListThingsInThingGroupRequestRequestTypeDef,
 ):
     pass
 
 
-ListThingsInThingGroupResponseTypeDef = TypedDict(
-    "ListThingsInThingGroupResponseTypeDef",
-    {
-        "things": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListThingsRequestListThingsPaginateTypeDef = TypedDict(
-    "ListThingsRequestListThingsPaginateTypeDef",
-    {
-        "attributeName": str,
-        "attributeValue": str,
-        "thingTypeName": str,
-        "usePrefixAttributeValue": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListThingsRequestRequestTypeDef = TypedDict(
     "ListThingsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "attributeName": str,
         "attributeValue": str,
@@ -5639,41 +4310,23 @@
         "thingArn": str,
         "attributes": Dict[str, str],
         "version": int,
     },
     total=False,
 )
 
-ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef = TypedDict(
-    "ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTopicRuleDestinationsRequestRequestTypeDef = TypedDict(
     "ListTopicRuleDestinationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListTopicRulesRequestListTopicRulesPaginateTypeDef = TypedDict(
-    "ListTopicRulesRequestListTopicRulesPaginateTypeDef",
-    {
-        "topic": str,
-        "ruleDisabled": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTopicRulesRequestRequestTypeDef = TypedDict(
     "ListTopicRulesRequestRequestTypeDef",
     {
         "topic": str,
         "maxResults": int,
         "nextToken": str,
         "ruleDisabled": bool,
@@ -5689,90 +4342,24 @@
         "topicPattern": str,
         "createdAt": datetime,
         "ruleDisabled": bool,
     },
     total=False,
 )
 
-ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef = TypedDict(
-    "ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef",
-    {
-        "targetType": LogTargetTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListV2LoggingLevelsRequestRequestTypeDef = TypedDict(
     "ListV2LoggingLevelsRequestRequestTypeDef",
     {
         "targetType": LogTargetTypeType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListViolationEventsRequestListViolationEventsPaginateTypeDef = TypedDict(
-    "_RequiredListViolationEventsRequestListViolationEventsPaginateTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListViolationEventsRequestListViolationEventsPaginateTypeDef = TypedDict(
-    "_OptionalListViolationEventsRequestListViolationEventsPaginateTypeDef",
-    {
-        "thingName": str,
-        "securityProfileName": str,
-        "behaviorCriteriaType": BehaviorCriteriaTypeType,
-        "listSuppressedAlerts": bool,
-        "verificationState": VerificationStateType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListViolationEventsRequestListViolationEventsPaginateTypeDef(
-    _RequiredListViolationEventsRequestListViolationEventsPaginateTypeDef,
-    _OptionalListViolationEventsRequestListViolationEventsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListViolationEventsRequestRequestTypeDef = TypedDict(
-    "_RequiredListViolationEventsRequestRequestTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListViolationEventsRequestRequestTypeDef = TypedDict(
-    "_OptionalListViolationEventsRequestRequestTypeDef",
-    {
-        "thingName": str,
-        "securityProfileName": str,
-        "behaviorCriteriaType": BehaviorCriteriaTypeType,
-        "listSuppressedAlerts": bool,
-        "verificationState": VerificationStateType,
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-
-class ListViolationEventsRequestRequestTypeDef(
-    _RequiredListViolationEventsRequestRequestTypeDef,
-    _OptionalListViolationEventsRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredLocationTimestampTypeDef = TypedDict(
     "_RequiredLocationTimestampTypeDef",
     {
         "value": str,
     },
 )
 _OptionalLocationTimestampTypeDef = TypedDict(
@@ -5854,42 +4441,22 @@
 UpdateDeviceCertificateParamsTypeDef = TypedDict(
     "UpdateDeviceCertificateParamsTypeDef",
     {
         "action": Literal["DEACTIVATE"],
     },
 )
 
-MqttContextTypeDef = TypedDict(
-    "MqttContextTypeDef",
-    {
-        "username": str,
-        "password": Union[str, bytes, IO[Any], StreamingBody],
-        "clientId": str,
-    },
-    total=False,
-)
-
 UserPropertyTypeDef = TypedDict(
     "UserPropertyTypeDef",
     {
         "key": str,
         "value": str,
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
 PolicyVersionIdentifierTypeDef = TypedDict(
     "PolicyVersionIdentifierTypeDef",
     {
         "policyName": str,
         "policyVersionId": str,
     },
     total=False,
@@ -5914,23 +4481,14 @@
 class PutVerificationStateOnViolationRequestRequestTypeDef(
     _RequiredPutVerificationStateOnViolationRequestRequestTypeDef,
     _OptionalPutVerificationStateOnViolationRequestRequestTypeDef,
 ):
     pass
 
 
-RegisterCACertificateResponseTypeDef = TypedDict(
-    "RegisterCACertificateResponseTypeDef",
-    {
-        "certificateArn": str,
-        "certificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRegisterCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterCertificateRequestRequestTypeDef",
     {
         "certificatePem": str,
     },
 )
 _OptionalRegisterCertificateRequestRequestTypeDef = TypedDict(
@@ -5947,23 +4505,14 @@
 class RegisterCertificateRequestRequestTypeDef(
     _RequiredRegisterCertificateRequestRequestTypeDef,
     _OptionalRegisterCertificateRequestRequestTypeDef,
 ):
     pass
 
 
-RegisterCertificateResponseTypeDef = TypedDict(
-    "RegisterCertificateResponseTypeDef",
-    {
-        "certificateArn": str,
-        "certificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRegisterCertificateWithoutCARequestRequestTypeDef = TypedDict(
     "_RequiredRegisterCertificateWithoutCARequestRequestTypeDef",
     {
         "certificatePem": str,
     },
 )
 _OptionalRegisterCertificateWithoutCARequestRequestTypeDef = TypedDict(
@@ -5978,23 +4527,14 @@
 class RegisterCertificateWithoutCARequestRequestTypeDef(
     _RequiredRegisterCertificateWithoutCARequestRequestTypeDef,
     _OptionalRegisterCertificateWithoutCARequestRequestTypeDef,
 ):
     pass
 
 
-RegisterCertificateWithoutCAResponseTypeDef = TypedDict(
-    "RegisterCertificateWithoutCAResponseTypeDef",
-    {
-        "certificateArn": str,
-        "certificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRegisterThingRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterThingRequestRequestTypeDef",
     {
         "templateBody": str,
     },
 )
 _OptionalRegisterThingRequestRequestTypeDef = TypedDict(
@@ -6008,23 +4548,14 @@
 
 class RegisterThingRequestRequestTypeDef(
     _RequiredRegisterThingRequestRequestTypeDef, _OptionalRegisterThingRequestRequestTypeDef
 ):
     pass
 
 
-RegisterThingResponseTypeDef = TypedDict(
-    "RegisterThingResponseTypeDef",
-    {
-        "certificatePem": str,
-        "resourceArns": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRejectCertificateTransferRequestRequestTypeDef = TypedDict(
     "_RequiredRejectCertificateTransferRequestRequestTypeDef",
     {
         "certificateId": str,
     },
 )
 _OptionalRejectCertificateTransferRequestRequestTypeDef = TypedDict(
@@ -6061,25 +4592,14 @@
         "thingGroupArn": str,
         "thingName": str,
         "thingArn": str,
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
 _RequiredSearchIndexRequestRequestTypeDef = TypedDict(
     "_RequiredSearchIndexRequestRequestTypeDef",
     {
         "queryString": str,
     },
 )
 _OptionalSearchIndexRequestRequestTypeDef = TypedDict(
@@ -6115,23 +4635,14 @@
 SetDefaultAuthorizerRequestRequestTypeDef = TypedDict(
     "SetDefaultAuthorizerRequestRequestTypeDef",
     {
         "authorizerName": str,
     },
 )
 
-SetDefaultAuthorizerResponseTypeDef = TypedDict(
-    "SetDefaultAuthorizerResponseTypeDef",
-    {
-        "authorizerName": str,
-        "authorizerArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetDefaultPolicyVersionRequestRequestTypeDef = TypedDict(
     "SetDefaultPolicyVersionRequestRequestTypeDef",
     {
         "policyName": str,
         "policyVersionId": str,
     },
 )
@@ -6152,63 +4663,31 @@
         "certificateArn": str,
         "platform": str,
         "certificatePathOnDevice": str,
     },
     total=False,
 )
 
-StartAuditMitigationActionsTaskResponseTypeDef = TypedDict(
-    "StartAuditMitigationActionsTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartDetectMitigationActionsTaskResponseTypeDef = TypedDict(
-    "StartDetectMitigationActionsTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartOnDemandAuditTaskRequestRequestTypeDef = TypedDict(
     "StartOnDemandAuditTaskRequestRequestTypeDef",
     {
         "targetCheckNames": Sequence[str],
     },
 )
 
-StartOnDemandAuditTaskResponseTypeDef = TypedDict(
-    "StartOnDemandAuditTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartThingRegistrationTaskRequestRequestTypeDef = TypedDict(
     "StartThingRegistrationTaskRequestRequestTypeDef",
     {
         "templateBody": str,
         "inputFileBucket": str,
         "inputFileKey": str,
         "roleArn": str,
     },
 )
 
-StartThingRegistrationTaskResponseTypeDef = TypedDict(
-    "StartThingRegistrationTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopThingRegistrationTaskRequestRequestTypeDef = TypedDict(
     "StopThingRegistrationTaskRequestRequestTypeDef",
     {
         "taskId": str,
     },
 )
 
@@ -6216,26 +4695,14 @@
     "TlsContextTypeDef",
     {
         "serverName": str,
     },
     total=False,
 )
 
-TestInvokeAuthorizerResponseTypeDef = TypedDict(
-    "TestInvokeAuthorizerResponseTypeDef",
-    {
-        "isAuthenticated": bool,
-        "principalId": str,
-        "policyDocuments": List[str],
-        "refreshAfterInSeconds": int,
-        "disconnectAfterInSeconds": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ThingConnectivityTypeDef = TypedDict(
     "ThingConnectivityTypeDef",
     {
         "connected": bool,
         "timestamp": int,
         "disconnectReason": str,
     },
@@ -6322,22 +4789,14 @@
 class TransferCertificateRequestRequestTypeDef(
     _RequiredTransferCertificateRequestRequestTypeDef,
     _OptionalTransferCertificateRequestRequestTypeDef,
 ):
     pass
 
 
-TransferCertificateResponseTypeDef = TypedDict(
-    "TransferCertificateResponseTypeDef",
-    {
-        "transferredCertificateArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -6363,31 +4822,14 @@
 
 class UpdateAuthorizerRequestRequestTypeDef(
     _RequiredUpdateAuthorizerRequestRequestTypeDef, _OptionalUpdateAuthorizerRequestRequestTypeDef
 ):
     pass
 
 
-UpdateAuthorizerResponseTypeDef = TypedDict(
-    "UpdateAuthorizerResponseTypeDef",
-    {
-        "authorizerName": str,
-        "authorizerArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateBillingGroupResponseTypeDef = TypedDict(
-    "UpdateBillingGroupResponseTypeDef",
-    {
-        "version": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateCertificateRequestRequestTypeDef = TypedDict(
     "UpdateCertificateRequestRequestTypeDef",
     {
         "certificateId": str,
         "newStatus": CertificateStatusType,
     },
 )
@@ -6396,74 +4838,22 @@
     "UpdateCustomMetricRequestRequestTypeDef",
     {
         "metricName": str,
         "displayName": str,
     },
 )
 
-UpdateCustomMetricResponseTypeDef = TypedDict(
-    "UpdateCustomMetricResponseTypeDef",
-    {
-        "metricName": str,
-        "metricArn": str,
-        "metricType": CustomMetricTypeType,
-        "displayName": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateDimensionRequestRequestTypeDef = TypedDict(
     "UpdateDimensionRequestRequestTypeDef",
     {
         "name": str,
         "stringValues": Sequence[str],
     },
 )
 
-UpdateDimensionResponseTypeDef = TypedDict(
-    "UpdateDimensionResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "type": Literal["TOPIC_FILTER"],
-        "stringValues": List[str],
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateDomainConfigurationResponseTypeDef = TypedDict(
-    "UpdateDomainConfigurationResponseTypeDef",
-    {
-        "domainConfigurationName": str,
-        "domainConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateDynamicThingGroupResponseTypeDef = TypedDict(
-    "UpdateDynamicThingGroupResponseTypeDef",
-    {
-        "version": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateMitigationActionResponseTypeDef = TypedDict(
-    "UpdateMitigationActionResponseTypeDef",
-    {
-        "actionArn": str,
-        "actionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdatePackageRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePackageRequestRequestTypeDef",
     {
         "packageName": str,
     },
 )
 _OptionalUpdatePackageRequestRequestTypeDef = TypedDict(
@@ -6528,23 +4918,14 @@
 
 class UpdateRoleAliasRequestRequestTypeDef(
     _RequiredUpdateRoleAliasRequestRequestTypeDef, _OptionalUpdateRoleAliasRequestRequestTypeDef
 ):
     pass
 
 
-UpdateRoleAliasResponseTypeDef = TypedDict(
-    "UpdateRoleAliasResponseTypeDef",
-    {
-        "roleAlias": str,
-        "roleAliasArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateScheduledAuditRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateScheduledAuditRequestRequestTypeDef",
     {
         "scheduledAuditName": str,
     },
 )
 _OptionalUpdateScheduledAuditRequestRequestTypeDef = TypedDict(
@@ -6562,41 +4943,14 @@
 class UpdateScheduledAuditRequestRequestTypeDef(
     _RequiredUpdateScheduledAuditRequestRequestTypeDef,
     _OptionalUpdateScheduledAuditRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateScheduledAuditResponseTypeDef = TypedDict(
-    "UpdateScheduledAuditResponseTypeDef",
-    {
-        "scheduledAuditArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateStreamResponseTypeDef = TypedDict(
-    "UpdateStreamResponseTypeDef",
-    {
-        "streamId": str,
-        "streamArn": str,
-        "description": str,
-        "streamVersion": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateThingGroupResponseTypeDef = TypedDict(
-    "UpdateThingGroupResponseTypeDef",
-    {
-        "version": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateThingGroupsForThingRequestRequestTypeDef = TypedDict(
     "UpdateThingGroupsForThingRequestRequestTypeDef",
     {
         "thingName": str,
         "thingGroupsToAdd": Sequence[str],
         "thingGroupsToRemove": Sequence[str],
         "overrideDynamicGroups": bool,
@@ -6616,50 +4970,38 @@
     "ValidationErrorTypeDef",
     {
         "errorMessage": str,
     },
     total=False,
 )
 
+AbortConfigOutputTypeDef = TypedDict(
+    "AbortConfigOutputTypeDef",
+    {
+        "criteriaList": List[AbortCriteriaTypeDef],
+    },
+)
+
 AbortConfigTypeDef = TypedDict(
     "AbortConfigTypeDef",
     {
         "criteriaList": Sequence[AbortCriteriaTypeDef],
     },
 )
 
 MetricDatumTypeDef = TypedDict(
     "MetricDatumTypeDef",
     {
         "timestamp": datetime,
-        "value": MetricValueTypeDef,
+        "value": MetricValueOutputTypeDef,
     },
     total=False,
 )
 
-DescribeFleetMetricResponseTypeDef = TypedDict(
-    "DescribeFleetMetricResponseTypeDef",
-    {
-        "metricName": str,
-        "queryString": str,
-        "aggregationType": AggregationTypeTypeDef,
-        "period": int,
-        "aggregationField": str,
-        "description": str,
-        "queryVersion": str,
-        "indexName": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "unit": FleetMetricUnitType,
-        "version": int,
-        "metricArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+AggregationTypeUnionTypeDef = Union[AggregationTypeTypeDef, AggregationTypeOutputTypeDef]
 _RequiredUpdateFleetMetricRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFleetMetricRequestRequestTypeDef",
     {
         "metricName": str,
         "indexName": str,
     },
 )
@@ -6705,63 +5047,886 @@
     "ImplicitDenyTypeDef",
     {
         "policies": List[PolicyTypeDef],
     },
     total=False,
 )
 
+_RequiredAssetPropertyValueTypeDef = TypedDict(
+    "_RequiredAssetPropertyValueTypeDef",
+    {
+        "value": AssetPropertyVariantTypeDef,
+        "timestamp": AssetPropertyTimestampTypeDef,
+    },
+)
+_OptionalAssetPropertyValueTypeDef = TypedDict(
+    "_OptionalAssetPropertyValueTypeDef",
+    {
+        "quality": str,
+    },
+    total=False,
+)
+
+
+class AssetPropertyValueTypeDef(
+    _RequiredAssetPropertyValueTypeDef, _OptionalAssetPropertyValueTypeDef
+):
+    pass
+
+
+AssociateTargetsWithJobResponseTypeDef = TypedDict(
+    "AssociateTargetsWithJobResponseTypeDef",
+    {
+        "jobArn": str,
+        "jobId": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelJobResponseTypeDef = TypedDict(
+    "CancelJobResponseTypeDef",
+    {
+        "jobArn": str,
+        "jobId": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAuthorizerResponseTypeDef = TypedDict(
+    "CreateAuthorizerResponseTypeDef",
+    {
+        "authorizerName": str,
+        "authorizerArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateBillingGroupResponseTypeDef = TypedDict(
+    "CreateBillingGroupResponseTypeDef",
+    {
+        "billingGroupName": str,
+        "billingGroupArn": str,
+        "billingGroupId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCertificateFromCsrResponseTypeDef = TypedDict(
+    "CreateCertificateFromCsrResponseTypeDef",
+    {
+        "certificateArn": str,
+        "certificateId": str,
+        "certificatePem": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCustomMetricResponseTypeDef = TypedDict(
+    "CreateCustomMetricResponseTypeDef",
+    {
+        "metricName": str,
+        "metricArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDimensionResponseTypeDef = TypedDict(
+    "CreateDimensionResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDomainConfigurationResponseTypeDef = TypedDict(
+    "CreateDomainConfigurationResponseTypeDef",
+    {
+        "domainConfigurationName": str,
+        "domainConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDynamicThingGroupResponseTypeDef = TypedDict(
+    "CreateDynamicThingGroupResponseTypeDef",
+    {
+        "thingGroupName": str,
+        "thingGroupArn": str,
+        "thingGroupId": str,
+        "indexName": str,
+        "queryString": str,
+        "queryVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFleetMetricResponseTypeDef = TypedDict(
+    "CreateFleetMetricResponseTypeDef",
+    {
+        "metricName": str,
+        "metricArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateJobResponseTypeDef = TypedDict(
+    "CreateJobResponseTypeDef",
+    {
+        "jobArn": str,
+        "jobId": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateJobTemplateResponseTypeDef = TypedDict(
+    "CreateJobTemplateResponseTypeDef",
+    {
+        "jobTemplateArn": str,
+        "jobTemplateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMitigationActionResponseTypeDef = TypedDict(
+    "CreateMitigationActionResponseTypeDef",
+    {
+        "actionArn": str,
+        "actionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateOTAUpdateResponseTypeDef = TypedDict(
+    "CreateOTAUpdateResponseTypeDef",
+    {
+        "otaUpdateId": str,
+        "awsIotJobId": str,
+        "otaUpdateArn": str,
+        "awsIotJobArn": str,
+        "otaUpdateStatus": OTAUpdateStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePackageResponseTypeDef = TypedDict(
+    "CreatePackageResponseTypeDef",
+    {
+        "packageName": str,
+        "packageArn": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePackageVersionResponseTypeDef = TypedDict(
+    "CreatePackageVersionResponseTypeDef",
+    {
+        "packageVersionArn": str,
+        "packageName": str,
+        "versionName": str,
+        "description": str,
+        "attributes": Dict[str, str],
+        "status": PackageVersionStatusType,
+        "errorReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePolicyResponseTypeDef = TypedDict(
+    "CreatePolicyResponseTypeDef",
+    {
+        "policyName": str,
+        "policyArn": str,
+        "policyDocument": str,
+        "policyVersionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePolicyVersionResponseTypeDef = TypedDict(
+    "CreatePolicyVersionResponseTypeDef",
+    {
+        "policyArn": str,
+        "policyDocument": str,
+        "policyVersionId": str,
+        "isDefaultVersion": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProvisioningTemplateResponseTypeDef = TypedDict(
+    "CreateProvisioningTemplateResponseTypeDef",
+    {
+        "templateArn": str,
+        "templateName": str,
+        "defaultVersionId": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProvisioningTemplateVersionResponseTypeDef = TypedDict(
+    "CreateProvisioningTemplateVersionResponseTypeDef",
+    {
+        "templateArn": str,
+        "templateName": str,
+        "versionId": int,
+        "isDefaultVersion": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRoleAliasResponseTypeDef = TypedDict(
+    "CreateRoleAliasResponseTypeDef",
+    {
+        "roleAlias": str,
+        "roleAliasArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateScheduledAuditResponseTypeDef = TypedDict(
+    "CreateScheduledAuditResponseTypeDef",
+    {
+        "scheduledAuditArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSecurityProfileResponseTypeDef = TypedDict(
+    "CreateSecurityProfileResponseTypeDef",
+    {
+        "securityProfileName": str,
+        "securityProfileArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStreamResponseTypeDef = TypedDict(
+    "CreateStreamResponseTypeDef",
+    {
+        "streamId": str,
+        "streamArn": str,
+        "description": str,
+        "streamVersion": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateThingGroupResponseTypeDef = TypedDict(
+    "CreateThingGroupResponseTypeDef",
+    {
+        "thingGroupName": str,
+        "thingGroupArn": str,
+        "thingGroupId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateThingResponseTypeDef = TypedDict(
+    "CreateThingResponseTypeDef",
+    {
+        "thingName": str,
+        "thingArn": str,
+        "thingId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateThingTypeResponseTypeDef = TypedDict(
+    "CreateThingTypeResponseTypeDef",
+    {
+        "thingTypeName": str,
+        "thingTypeArn": str,
+        "thingTypeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeCustomMetricResponseTypeDef = TypedDict(
+    "DescribeCustomMetricResponseTypeDef",
+    {
+        "metricName": str,
+        "metricArn": str,
+        "metricType": CustomMetricTypeType,
+        "displayName": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDimensionResponseTypeDef = TypedDict(
+    "DescribeDimensionResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "type": Literal["TOPIC_FILTER"],
+        "stringValues": List[str],
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEndpointResponseTypeDef = TypedDict(
+    "DescribeEndpointResponseTypeDef",
+    {
+        "endpointAddress": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeFleetMetricResponseTypeDef = TypedDict(
+    "DescribeFleetMetricResponseTypeDef",
+    {
+        "metricName": str,
+        "queryString": str,
+        "aggregationType": AggregationTypeOutputTypeDef,
+        "period": int,
+        "aggregationField": str,
+        "description": str,
+        "queryVersion": str,
+        "indexName": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "unit": FleetMetricUnitType,
+        "version": int,
+        "metricArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeIndexResponseTypeDef = TypedDict(
+    "DescribeIndexResponseTypeDef",
+    {
+        "indexName": str,
+        "indexStatus": IndexStatusType,
+        "schema": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeProvisioningTemplateVersionResponseTypeDef = TypedDict(
+    "DescribeProvisioningTemplateVersionResponseTypeDef",
+    {
+        "versionId": int,
+        "creationDate": datetime,
+        "templateBody": str,
+        "isDefaultVersion": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeScheduledAuditResponseTypeDef = TypedDict(
+    "DescribeScheduledAuditResponseTypeDef",
+    {
+        "frequency": AuditFrequencyType,
+        "dayOfMonth": str,
+        "dayOfWeek": DayOfWeekType,
+        "targetCheckNames": List[str],
+        "scheduledAuditName": str,
+        "scheduledAuditArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeThingRegistrationTaskResponseTypeDef = TypedDict(
+    "DescribeThingRegistrationTaskResponseTypeDef",
+    {
+        "taskId": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "templateBody": str,
+        "inputFileBucket": str,
+        "inputFileKey": str,
+        "roleArn": str,
+        "status": StatusType,
+        "message": str,
+        "successCount": int,
+        "failureCount": int,
+        "percentageProgress": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeThingResponseTypeDef = TypedDict(
+    "DescribeThingResponseTypeDef",
+    {
+        "defaultClientId": str,
+        "thingName": str,
+        "thingId": str,
+        "thingArn": str,
+        "thingTypeName": str,
+        "attributes": Dict[str, str],
+        "version": int,
+        "billingGroupName": str,
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
+GetCardinalityResponseTypeDef = TypedDict(
+    "GetCardinalityResponseTypeDef",
+    {
+        "cardinality": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetJobDocumentResponseTypeDef = TypedDict(
+    "GetJobDocumentResponseTypeDef",
+    {
+        "document": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetLoggingOptionsResponseTypeDef = TypedDict(
+    "GetLoggingOptionsResponseTypeDef",
+    {
+        "roleArn": str,
+        "logLevel": LogLevelType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPackageResponseTypeDef = TypedDict(
+    "GetPackageResponseTypeDef",
+    {
+        "packageName": str,
+        "packageArn": str,
+        "description": str,
+        "defaultVersionName": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPackageVersionResponseTypeDef = TypedDict(
+    "GetPackageVersionResponseTypeDef",
+    {
+        "packageVersionArn": str,
+        "packageName": str,
+        "versionName": str,
+        "description": str,
+        "attributes": Dict[str, str],
+        "status": PackageVersionStatusType,
+        "errorReason": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPolicyResponseTypeDef = TypedDict(
+    "GetPolicyResponseTypeDef",
+    {
+        "policyName": str,
+        "policyArn": str,
+        "policyDocument": str,
+        "defaultVersionId": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "generationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPolicyVersionResponseTypeDef = TypedDict(
+    "GetPolicyVersionResponseTypeDef",
+    {
+        "policyArn": str,
+        "policyName": str,
+        "policyDocument": str,
+        "policyVersionId": str,
+        "isDefaultVersion": bool,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "generationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRegistrationCodeResponseTypeDef = TypedDict(
+    "GetRegistrationCodeResponseTypeDef",
+    {
+        "registrationCode": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetV2LoggingOptionsResponseTypeDef = TypedDict(
+    "GetV2LoggingOptionsResponseTypeDef",
+    {
+        "roleArn": str,
+        "defaultLogLevel": LogLevelType,
+        "disableAllLogs": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListAttachedPoliciesResponseTypeDef = TypedDict(
     "ListAttachedPoliciesResponseTypeDef",
     {
         "policies": List[PolicyTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCustomMetricsResponseTypeDef = TypedDict(
+    "ListCustomMetricsResponseTypeDef",
+    {
+        "metricNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDimensionsResponseTypeDef = TypedDict(
+    "ListDimensionsResponseTypeDef",
+    {
+        "dimensionNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListIndicesResponseTypeDef = TypedDict(
+    "ListIndicesResponseTypeDef",
+    {
+        "indexNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPoliciesResponseTypeDef = TypedDict(
     "ListPoliciesResponseTypeDef",
     {
         "policies": List[PolicyTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPolicyPrincipalsResponseTypeDef = TypedDict(
+    "ListPolicyPrincipalsResponseTypeDef",
+    {
+        "principals": List[str],
+        "nextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPrincipalPoliciesResponseTypeDef = TypedDict(
     "ListPrincipalPoliciesResponseTypeDef",
     {
         "policies": List[PolicyTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredAssetPropertyValueTypeDef = TypedDict(
-    "_RequiredAssetPropertyValueTypeDef",
+ListPrincipalThingsResponseTypeDef = TypedDict(
+    "ListPrincipalThingsResponseTypeDef",
     {
-        "value": AssetPropertyVariantTypeDef,
-        "timestamp": AssetPropertyTimestampTypeDef,
+        "things": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalAssetPropertyValueTypeDef = TypedDict(
-    "_OptionalAssetPropertyValueTypeDef",
+
+ListRoleAliasesResponseTypeDef = TypedDict(
+    "ListRoleAliasesResponseTypeDef",
     {
-        "quality": str,
+        "roleAliases": List[str],
+        "nextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+ListTargetsForPolicyResponseTypeDef = TypedDict(
+    "ListTargetsForPolicyResponseTypeDef",
+    {
+        "targets": List[str],
+        "nextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class AssetPropertyValueTypeDef(
-    _RequiredAssetPropertyValueTypeDef, _OptionalAssetPropertyValueTypeDef
-):
-    pass
+ListThingPrincipalsResponseTypeDef = TypedDict(
+    "ListThingPrincipalsResponseTypeDef",
+    {
+        "principals": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListThingRegistrationTaskReportsResponseTypeDef = TypedDict(
+    "ListThingRegistrationTaskReportsResponseTypeDef",
+    {
+        "resourceLinks": List[str],
+        "reportType": ReportTypeType,
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListThingRegistrationTasksResponseTypeDef = TypedDict(
+    "ListThingRegistrationTasksResponseTypeDef",
+    {
+        "taskIds": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListThingsInBillingGroupResponseTypeDef = TypedDict(
+    "ListThingsInBillingGroupResponseTypeDef",
+    {
+        "things": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListThingsInThingGroupResponseTypeDef = TypedDict(
+    "ListThingsInThingGroupResponseTypeDef",
+    {
+        "things": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterCACertificateResponseTypeDef = TypedDict(
+    "RegisterCACertificateResponseTypeDef",
+    {
+        "certificateArn": str,
+        "certificateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterCertificateResponseTypeDef = TypedDict(
+    "RegisterCertificateResponseTypeDef",
+    {
+        "certificateArn": str,
+        "certificateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterCertificateWithoutCAResponseTypeDef = TypedDict(
+    "RegisterCertificateWithoutCAResponseTypeDef",
+    {
+        "certificateArn": str,
+        "certificateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterThingResponseTypeDef = TypedDict(
+    "RegisterThingResponseTypeDef",
+    {
+        "certificatePem": str,
+        "resourceArns": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetDefaultAuthorizerResponseTypeDef = TypedDict(
+    "SetDefaultAuthorizerResponseTypeDef",
+    {
+        "authorizerName": str,
+        "authorizerArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartAuditMitigationActionsTaskResponseTypeDef = TypedDict(
+    "StartAuditMitigationActionsTaskResponseTypeDef",
+    {
+        "taskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartDetectMitigationActionsTaskResponseTypeDef = TypedDict(
+    "StartDetectMitigationActionsTaskResponseTypeDef",
+    {
+        "taskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartOnDemandAuditTaskResponseTypeDef = TypedDict(
+    "StartOnDemandAuditTaskResponseTypeDef",
+    {
+        "taskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartThingRegistrationTaskResponseTypeDef = TypedDict(
+    "StartThingRegistrationTaskResponseTypeDef",
+    {
+        "taskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestInvokeAuthorizerResponseTypeDef = TypedDict(
+    "TestInvokeAuthorizerResponseTypeDef",
+    {
+        "isAuthenticated": bool,
+        "principalId": str,
+        "policyDocuments": List[str],
+        "refreshAfterInSeconds": int,
+        "disconnectAfterInSeconds": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TransferCertificateResponseTypeDef = TypedDict(
+    "TransferCertificateResponseTypeDef",
+    {
+        "transferredCertificateArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAuthorizerResponseTypeDef = TypedDict(
+    "UpdateAuthorizerResponseTypeDef",
+    {
+        "authorizerName": str,
+        "authorizerArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBillingGroupResponseTypeDef = TypedDict(
+    "UpdateBillingGroupResponseTypeDef",
+    {
+        "version": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateCustomMetricResponseTypeDef = TypedDict(
+    "UpdateCustomMetricResponseTypeDef",
+    {
+        "metricName": str,
+        "metricArn": str,
+        "metricType": CustomMetricTypeType,
+        "displayName": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDimensionResponseTypeDef = TypedDict(
+    "UpdateDimensionResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "type": Literal["TOPIC_FILTER"],
+        "stringValues": List[str],
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDomainConfigurationResponseTypeDef = TypedDict(
+    "UpdateDomainConfigurationResponseTypeDef",
+    {
+        "domainConfigurationName": str,
+        "domainConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDynamicThingGroupResponseTypeDef = TypedDict(
+    "UpdateDynamicThingGroupResponseTypeDef",
+    {
+        "version": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateMitigationActionResponseTypeDef = TypedDict(
+    "UpdateMitigationActionResponseTypeDef",
+    {
+        "actionArn": str,
+        "actionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRoleAliasResponseTypeDef = TypedDict(
+    "UpdateRoleAliasResponseTypeDef",
+    {
+        "roleAlias": str,
+        "roleAliasArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateScheduledAuditResponseTypeDef = TypedDict(
+    "UpdateScheduledAuditResponseTypeDef",
+    {
+        "scheduledAuditArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateStreamResponseTypeDef = TypedDict(
+    "UpdateStreamResponseTypeDef",
+    {
+        "streamId": str,
+        "streamArn": str,
+        "description": str,
+        "streamVersion": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateThingGroupResponseTypeDef = TypedDict(
+    "UpdateThingGroupResponseTypeDef",
+    {
+        "version": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+ThingGroupPropertiesOutputTypeDef = TypedDict(
+    "ThingGroupPropertiesOutputTypeDef",
+    {
+        "thingGroupDescription": str,
+        "attributePayload": AttributePayloadOutputTypeDef,
+    },
+    total=False,
+)
 
+AttributePayloadUnionTypeDef = Union[AttributePayloadTypeDef, AttributePayloadOutputTypeDef]
 _RequiredCreateThingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateThingRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 _OptionalCreateThingRequestRequestTypeDef = TypedDict(
@@ -6815,27 +5980,30 @@
 
 
 ListAuditMitigationActionsExecutionsResponseTypeDef = TypedDict(
     "ListAuditMitigationActionsExecutionsResponseTypeDef",
     {
         "actionsExecutions": List[AuditMitigationActionExecutionMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAuditMitigationActionsTasksResponseTypeDef = TypedDict(
     "ListAuditMitigationActionsTasksResponseTypeDef",
     {
         "tasks": List[AuditMitigationActionsTaskMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AuditMitigationActionsTaskTargetUnionTypeDef = Union[
+    AuditMitigationActionsTaskTargetTypeDef, AuditMitigationActionsTaskTargetOutputTypeDef
+]
 StartAuditMitigationActionsTaskRequestRequestTypeDef = TypedDict(
     "StartAuditMitigationActionsTaskRequestRequestTypeDef",
     {
         "taskId": str,
         "target": AuditMitigationActionsTaskTargetTypeDef,
         "auditCheckToActionsMapping": Mapping[str, Sequence[str]],
         "clientRequestToken": str,
@@ -6846,15 +6014,15 @@
     "DescribeAccountAuditConfigurationResponseTypeDef",
     {
         "roleArn": str,
         "auditNotificationTargetConfigurations": Dict[
             Literal["SNS"], AuditNotificationTargetTypeDef
         ],
         "auditCheckConfigurations": Dict[str, AuditCheckConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAccountAuditConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateAccountAuditConfigurationRequestRequestTypeDef",
     {
         "roleArn": str,
@@ -6867,65 +6035,41 @@
 )
 
 ListAuditTasksResponseTypeDef = TypedDict(
     "ListAuditTasksResponseTypeDef",
     {
         "tasks": List[AuditTaskMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredTestAuthorizationRequestRequestTypeDef = TypedDict(
-    "_RequiredTestAuthorizationRequestRequestTypeDef",
-    {
-        "authInfos": Sequence[AuthInfoTypeDef],
-    },
-)
-_OptionalTestAuthorizationRequestRequestTypeDef = TypedDict(
-    "_OptionalTestAuthorizationRequestRequestTypeDef",
-    {
-        "principal": str,
-        "cognitoIdentityPoolId": str,
-        "clientId": str,
-        "policyNamesToAdd": Sequence[str],
-        "policyNamesToSkip": Sequence[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class TestAuthorizationRequestRequestTypeDef(
-    _RequiredTestAuthorizationRequestRequestTypeDef, _OptionalTestAuthorizationRequestRequestTypeDef
-):
-    pass
-
-
+AuthInfoUnionTypeDef = Union[AuthInfoTypeDef, AuthInfoOutputTypeDef]
 DescribeAuthorizerResponseTypeDef = TypedDict(
     "DescribeAuthorizerResponseTypeDef",
     {
         "authorizerDescription": AuthorizerDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDefaultAuthorizerResponseTypeDef = TypedDict(
     "DescribeDefaultAuthorizerResponseTypeDef",
     {
         "authorizerDescription": AuthorizerDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAuthorizersResponseTypeDef = TypedDict(
     "ListAuthorizersResponseTypeDef",
     {
         "authorizers": List[AuthorizerSummaryTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AwsJobAbortConfigTypeDef = TypedDict(
     "AwsJobAbortConfigTypeDef",
     {
         "abortCriteriaList": Sequence[AwsJobAbortCriteriaTypeDef],
@@ -6937,14 +6081,28 @@
     {
         "baseRatePerMinute": int,
         "incrementFactor": float,
         "rateIncreaseCriteria": AwsJobRateIncreaseCriteriaTypeDef,
     },
 )
 
+BehaviorCriteriaOutputTypeDef = TypedDict(
+    "BehaviorCriteriaOutputTypeDef",
+    {
+        "comparisonOperator": ComparisonOperatorType,
+        "value": MetricValueOutputTypeDef,
+        "durationSeconds": int,
+        "consecutiveDatapointsToAlarm": int,
+        "consecutiveDatapointsToClear": int,
+        "statisticalThreshold": StatisticalThresholdTypeDef,
+        "mlDetectionConfig": MachineLearningDetectionConfigTypeDef,
+    },
+    total=False,
+)
+
 BehaviorCriteriaTypeDef = TypedDict(
     "BehaviorCriteriaTypeDef",
     {
         "comparisonOperator": ComparisonOperatorType,
         "value": MetricValueTypeDef,
         "durationSeconds": int,
         "consecutiveDatapointsToAlarm": int,
@@ -6956,15 +6114,15 @@
 )
 
 GetBehaviorModelTrainingSummariesResponseTypeDef = TypedDict(
     "GetBehaviorModelTrainingSummariesResponseTypeDef",
     {
         "summaries": List[BehaviorModelTrainingSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredMetricToRetainTypeDef = TypedDict(
     "_RequiredMetricToRetainTypeDef",
     {
         "metric": str,
@@ -6988,15 +6146,15 @@
     {
         "billingGroupName": str,
         "billingGroupId": str,
         "billingGroupArn": str,
         "version": int,
         "billingGroupProperties": BillingGroupPropertiesTypeDef,
         "billingGroupMetadata": BillingGroupMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateBillingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBillingGroupRequestRequestTypeDef",
     {
         "billingGroupName": str,
@@ -7015,20 +6173,38 @@
 class UpdateBillingGroupRequestRequestTypeDef(
     _RequiredUpdateBillingGroupRequestRequestTypeDef,
     _OptionalUpdateBillingGroupRequestRequestTypeDef,
 ):
     pass
 
 
+CodeSigningSignatureTypeDef = TypedDict(
+    "CodeSigningSignatureTypeDef",
+    {
+        "inlineDocument": BlobTypeDef,
+    },
+    total=False,
+)
+
+MqttContextTypeDef = TypedDict(
+    "MqttContextTypeDef",
+    {
+        "username": str,
+        "password": BlobTypeDef,
+        "clientId": str,
+    },
+    total=False,
+)
+
 GetBucketsAggregationResponseTypeDef = TypedDict(
     "GetBucketsAggregationResponseTypeDef",
     {
         "totalCount": int,
         "buckets": List[BucketTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BucketsAggregationTypeTypeDef = TypedDict(
     "BucketsAggregationTypeTypeDef",
     {
         "termsAggregation": TermsAggregationTypeDef,
@@ -7056,15 +6232,15 @@
 )
 
 ListCACertificatesResponseTypeDef = TypedDict(
     "ListCACertificatesResponseTypeDef",
     {
         "certificates": List[CACertificateTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CertificateDescriptionTypeDef = TypedDict(
     "CertificateDescriptionTypeDef",
     {
         "certificateArn": str,
@@ -7086,56 +6262,210 @@
 )
 
 ListCertificatesByCAResponseTypeDef = TypedDict(
     "ListCertificatesByCAResponseTypeDef",
     {
         "certificates": List[CertificateTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCertificatesResponseTypeDef = TypedDict(
     "ListCertificatesResponseTypeDef",
     {
         "certificates": List[CertificateTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CustomCodeSigningTypeDef = TypedDict(
-    "CustomCodeSigningTypeDef",
+CustomCodeSigningOutputTypeDef = TypedDict(
+    "CustomCodeSigningOutputTypeDef",
     {
-        "signature": CodeSigningSignatureTypeDef,
+        "signature": CodeSigningSignatureOutputTypeDef,
         "certificateChain": CodeSigningCertificateChainTypeDef,
         "hashAlgorithm": str,
         "signatureAlgorithm": str,
     },
     total=False,
 )
 
 DescribeEventConfigurationsResponseTypeDef = TypedDict(
     "DescribeEventConfigurationsResponseTypeDef",
     {
         "eventConfigurations": Dict[EventTypeType, ConfigurationTypeDef],
         "creationDate": datetime,
         "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEventConfigurationsRequestRequestTypeDef = TypedDict(
     "UpdateEventConfigurationsRequestRequestTypeDef",
     {
         "eventConfigurations": Mapping[EventTypeType, ConfigurationTypeDef],
     },
     total=False,
 )
 
+_RequiredListAuditMitigationActionsTasksRequestRequestTypeDef = TypedDict(
+    "_RequiredListAuditMitigationActionsTasksRequestRequestTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListAuditMitigationActionsTasksRequestRequestTypeDef = TypedDict(
+    "_OptionalListAuditMitigationActionsTasksRequestRequestTypeDef",
+    {
+        "auditTaskId": str,
+        "findingId": str,
+        "taskStatus": AuditMitigationActionsTaskStatusType,
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+
+class ListAuditMitigationActionsTasksRequestRequestTypeDef(
+    _RequiredListAuditMitigationActionsTasksRequestRequestTypeDef,
+    _OptionalListAuditMitigationActionsTasksRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredListAuditTasksRequestRequestTypeDef = TypedDict(
+    "_RequiredListAuditTasksRequestRequestTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListAuditTasksRequestRequestTypeDef = TypedDict(
+    "_OptionalListAuditTasksRequestRequestTypeDef",
+    {
+        "taskType": AuditTaskTypeType,
+        "taskStatus": AuditTaskStatusType,
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+
+class ListAuditTasksRequestRequestTypeDef(
+    _RequiredListAuditTasksRequestRequestTypeDef, _OptionalListAuditTasksRequestRequestTypeDef
+):
+    pass
+
+
+ListDetectMitigationActionsExecutionsRequestRequestTypeDef = TypedDict(
+    "ListDetectMitigationActionsExecutionsRequestRequestTypeDef",
+    {
+        "taskId": str,
+        "violationId": str,
+        "thingName": str,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+_RequiredListDetectMitigationActionsTasksRequestRequestTypeDef = TypedDict(
+    "_RequiredListDetectMitigationActionsTasksRequestRequestTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListDetectMitigationActionsTasksRequestRequestTypeDef = TypedDict(
+    "_OptionalListDetectMitigationActionsTasksRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+
+class ListDetectMitigationActionsTasksRequestRequestTypeDef(
+    _RequiredListDetectMitigationActionsTasksRequestRequestTypeDef,
+    _OptionalListDetectMitigationActionsTasksRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredListMetricValuesRequestRequestTypeDef = TypedDict(
+    "_RequiredListMetricValuesRequestRequestTypeDef",
+    {
+        "thingName": str,
+        "metricName": str,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListMetricValuesRequestRequestTypeDef = TypedDict(
+    "_OptionalListMetricValuesRequestRequestTypeDef",
+    {
+        "dimensionName": str,
+        "dimensionValueOperator": DimensionValueOperatorType,
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+
+class ListMetricValuesRequestRequestTypeDef(
+    _RequiredListMetricValuesRequestRequestTypeDef, _OptionalListMetricValuesRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredListViolationEventsRequestRequestTypeDef = TypedDict(
+    "_RequiredListViolationEventsRequestRequestTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListViolationEventsRequestRequestTypeDef = TypedDict(
+    "_OptionalListViolationEventsRequestRequestTypeDef",
+    {
+        "thingName": str,
+        "securityProfileName": str,
+        "behaviorCriteriaType": BehaviorCriteriaTypeType,
+        "listSuppressedAlerts": bool,
+        "verificationState": VerificationStateType,
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+
+class ListViolationEventsRequestRequestTypeDef(
+    _RequiredListViolationEventsRequestRequestTypeDef,
+    _OptionalListViolationEventsRequestRequestTypeDef,
+):
+    pass
+
+
+ViolationEventOccurrenceRangeTypeDef = TypedDict(
+    "ViolationEventOccurrenceRangeTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+
 _RequiredCreateAuthorizerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAuthorizerRequestRequestTypeDef",
     {
         "authorizerName": str,
         "authorizerFunctionArn": str,
     },
 )
@@ -7332,15 +6662,15 @@
 
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -7397,14 +6727,25 @@
 class UpdateDomainConfigurationRequestRequestTypeDef(
     _RequiredUpdateDomainConfigurationRequestRequestTypeDef,
     _OptionalUpdateDomainConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
+SchedulingConfigOutputTypeDef = TypedDict(
+    "SchedulingConfigOutputTypeDef",
+    {
+        "startTime": str,
+        "endTime": str,
+        "endBehavior": JobEndBehaviorType,
+        "maintenanceWindows": List[MaintenanceWindowTypeDef],
+    },
+    total=False,
+)
+
 SchedulingConfigTypeDef = TypedDict(
     "SchedulingConfigTypeDef",
     {
         "startTime": str,
         "endTime": str,
         "endBehavior": JobEndBehaviorType,
         "maintenanceWindows": Sequence[MaintenanceWindowTypeDef],
@@ -7415,26 +6756,26 @@
 CreateKeysAndCertificateResponseTypeDef = TypedDict(
     "CreateKeysAndCertificateResponseTypeDef",
     {
         "certificateArn": str,
         "certificateId": str,
         "certificatePem": str,
         "keyPair": KeyPairTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateProvisioningClaimResponseTypeDef = TypedDict(
     "CreateProvisioningClaimResponseTypeDef",
     {
         "certificateId": str,
         "certificatePem": str,
         "keyPair": KeyPairTypeDef,
         "expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateProvisioningTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProvisioningTemplateRequestRequestTypeDef",
     {
         "templateName": str,
@@ -7472,15 +6813,15 @@
         "lastModifiedDate": datetime,
         "defaultVersionId": int,
         "templateBody": str,
         "enabled": bool,
         "provisioningRoleArn": str,
         "preProvisioningHook": ProvisioningHookTypeDef,
         "type": TemplateTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateProvisioningTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProvisioningTemplateRequestRequestTypeDef",
     {
         "templateName": str,
@@ -7534,15 +6875,15 @@
     {
         "taskStatus": AuditTaskStatusType,
         "taskType": AuditTaskTypeType,
         "taskStartTime": datetime,
         "taskStatistics": TaskStatisticsTypeDef,
         "scheduledAuditName": str,
         "auditDetails": Dict[str, AuditCheckDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRegisterCACertificateRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterCACertificateRequestRequestTypeDef",
     {
         "caCertificate": str,
@@ -7603,113 +6944,92 @@
         "serverCertificates": List[ServerCertificateSummaryTypeDef],
         "authorizerConfig": AuthorizerConfigTypeDef,
         "domainConfigurationStatus": DomainConfigurationStatusType,
         "serviceType": ServiceTypeType,
         "domainType": DomainTypeType,
         "lastStatusChangeDate": datetime,
         "tlsConfig": TlsConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeManagedJobTemplateResponseTypeDef = TypedDict(
     "DescribeManagedJobTemplateResponseTypeDef",
     {
         "templateName": str,
         "templateArn": str,
         "description": str,
         "templateVersion": str,
         "environments": List[str],
         "documentParameters": List[DocumentParameterTypeDef],
         "document": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRoleAliasResponseTypeDef = TypedDict(
     "DescribeRoleAliasResponseTypeDef",
     {
         "roleAliasDescription": RoleAliasDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeThingTypeResponseTypeDef = TypedDict(
     "DescribeThingTypeResponseTypeDef",
     {
         "thingTypeName": str,
         "thingTypeId": str,
         "thingTypeArn": str,
-        "thingTypeProperties": ThingTypePropertiesTypeDef,
+        "thingTypeProperties": ThingTypePropertiesOutputTypeDef,
         "thingTypeMetadata": ThingTypeMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ThingTypeDefinitionTypeDef = TypedDict(
     "ThingTypeDefinitionTypeDef",
     {
         "thingTypeName": str,
         "thingTypeArn": str,
-        "thingTypeProperties": ThingTypePropertiesTypeDef,
+        "thingTypeProperties": ThingTypePropertiesOutputTypeDef,
         "thingTypeMetadata": ThingTypeMetadataTypeDef,
     },
     total=False,
 )
 
+ThingTypePropertiesUnionTypeDef = Union[
+    ThingTypePropertiesTypeDef, ThingTypePropertiesOutputTypeDef
+]
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "s3Destination": S3DestinationTypeDef,
     },
     total=False,
 )
 
 ListDetectMitigationActionsExecutionsResponseTypeDef = TypedDict(
     "ListDetectMitigationActionsExecutionsResponseTypeDef",
     {
         "actionsExecutions": List[DetectMitigationActionExecutionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
-    "_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef",
-    {
-        "taskId": str,
-        "target": DetectMitigationActionsTaskTargetTypeDef,
-        "actions": Sequence[str],
-        "clientRequestToken": str,
-    },
-)
-_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
-    "_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef",
-    {
-        "violationEventOccurrenceRange": ViolationEventOccurrenceRangeTypeDef,
-        "includeOnlyActiveViolations": bool,
-        "includeSuppressedAlerts": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class StartDetectMitigationActionsTaskRequestRequestTypeDef(
-    _RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef,
-    _OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef,
-):
-    pass
-
-
+DetectMitigationActionsTaskTargetUnionTypeDef = Union[
+    DetectMitigationActionsTaskTargetTypeDef, DetectMitigationActionsTaskTargetOutputTypeDef
+]
 ListDomainConfigurationsResponseTypeDef = TypedDict(
     "ListDomainConfigurationsResponseTypeDef",
     {
         "domainConfigurations": List[DomainConfigurationSummaryTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DynamoDBv2ActionTypeDef = TypedDict(
     "DynamoDBv2ActionTypeDef",
     {
         "roleArn": str,
@@ -7717,38 +7037,61 @@
     },
 )
 
 GetEffectivePoliciesResponseTypeDef = TypedDict(
     "GetEffectivePoliciesResponseTypeDef",
     {
         "effectivePolicies": List[EffectivePolicyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExponentialRolloutRateTypeDef = TypedDict(
     "ExponentialRolloutRateTypeDef",
     {
         "baseRatePerMinute": int,
         "incrementFactor": float,
         "rateIncreaseCriteria": RateIncreaseCriteriaTypeDef,
     },
 )
 
+_RequiredThingGroupIndexingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredThingGroupIndexingConfigurationOutputTypeDef",
+    {
+        "thingGroupIndexingMode": ThingGroupIndexingModeType,
+    },
+)
+_OptionalThingGroupIndexingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalThingGroupIndexingConfigurationOutputTypeDef",
+    {
+        "managedFields": List[FieldTypeDef],
+        "customFields": List[FieldTypeDef],
+    },
+    total=False,
+)
+
+
+class ThingGroupIndexingConfigurationOutputTypeDef(
+    _RequiredThingGroupIndexingConfigurationOutputTypeDef,
+    _OptionalThingGroupIndexingConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredThingGroupIndexingConfigurationTypeDef = TypedDict(
     "_RequiredThingGroupIndexingConfigurationTypeDef",
     {
         "thingGroupIndexingMode": ThingGroupIndexingModeType,
     },
 )
 _OptionalThingGroupIndexingConfigurationTypeDef = TypedDict(
     "_OptionalThingGroupIndexingConfigurationTypeDef",
     {
-        "managedFields": List[FieldTypeDef],
-        "customFields": List[FieldTypeDef],
+        "managedFields": Sequence[FieldTypeDef],
+        "customFields": Sequence[FieldTypeDef],
     },
     total=False,
 )
 
 
 class ThingGroupIndexingConfigurationTypeDef(
     _RequiredThingGroupIndexingConfigurationTypeDef, _OptionalThingGroupIndexingConfigurationTypeDef
@@ -7775,23 +7118,916 @@
 )
 
 ListFleetMetricsResponseTypeDef = TypedDict(
     "ListFleetMetricsResponseTypeDef",
     {
         "fleetMetrics": List[FleetMetricNameAndArnTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef = (
+    TypedDict(
+        "GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef",
+        {
+            "securityProfileName": str,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+ListActiveViolationsRequestListActiveViolationsPaginateTypeDef = TypedDict(
+    "ListActiveViolationsRequestListActiveViolationsPaginateTypeDef",
+    {
+        "thingName": str,
+        "securityProfileName": str,
+        "behaviorCriteriaType": BehaviorCriteriaTypeType,
+        "listSuppressedAlerts": bool,
+        "verificationState": VerificationStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef",
+    {
+        "target": str,
+    },
+)
+_OptionalListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef",
+    {
+        "recursive": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef(
+    _RequiredListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef,
+    _OptionalListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef",
+    {
+        "taskId": str,
+        "findingId": str,
+    },
+)
+_OptionalListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef",
+    {
+        "actionStatus": AuditMitigationActionsExecutionStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+
+class ListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef(
+    _RequiredListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef,
+    _OptionalListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef = TypedDict(
+    "_RequiredListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef = TypedDict(
+    "_OptionalListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef",
+    {
+        "auditTaskId": str,
+        "findingId": str,
+        "taskStatus": AuditMitigationActionsTaskStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
+
+class ListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef(
+    _RequiredListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef,
+    _OptionalListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListAuditTasksRequestListAuditTasksPaginateTypeDef = TypedDict(
+    "_RequiredListAuditTasksRequestListAuditTasksPaginateTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListAuditTasksRequestListAuditTasksPaginateTypeDef = TypedDict(
+    "_OptionalListAuditTasksRequestListAuditTasksPaginateTypeDef",
+    {
+        "taskType": AuditTaskTypeType,
+        "taskStatus": AuditTaskStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAuditTasksRequestListAuditTasksPaginateTypeDef(
+    _RequiredListAuditTasksRequestListAuditTasksPaginateTypeDef,
+    _OptionalListAuditTasksRequestListAuditTasksPaginateTypeDef,
+):
+    pass
+
+
+ListAuthorizersRequestListAuthorizersPaginateTypeDef = TypedDict(
+    "ListAuthorizersRequestListAuthorizersPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "status": AuthorizerStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListBillingGroupsRequestListBillingGroupsPaginateTypeDef = TypedDict(
+    "ListBillingGroupsRequestListBillingGroupsPaginateTypeDef",
+    {
+        "namePrefixFilter": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCACertificatesRequestListCACertificatesPaginateTypeDef = TypedDict(
+    "ListCACertificatesRequestListCACertificatesPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "templateName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListCertificatesByCARequestListCertificatesByCAPaginateTypeDef = TypedDict(
+    "_RequiredListCertificatesByCARequestListCertificatesByCAPaginateTypeDef",
+    {
+        "caCertificateId": str,
+    },
+)
+_OptionalListCertificatesByCARequestListCertificatesByCAPaginateTypeDef = TypedDict(
+    "_OptionalListCertificatesByCARequestListCertificatesByCAPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListCertificatesByCARequestListCertificatesByCAPaginateTypeDef(
+    _RequiredListCertificatesByCARequestListCertificatesByCAPaginateTypeDef,
+    _OptionalListCertificatesByCARequestListCertificatesByCAPaginateTypeDef,
+):
+    pass
+
+
+ListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
+    "ListCertificatesRequestListCertificatesPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCustomMetricsRequestListCustomMetricsPaginateTypeDef = TypedDict(
+    "ListCustomMetricsRequestListCustomMetricsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef = TypedDict(
+    "ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef",
+    {
+        "taskId": str,
+        "violationId": str,
+        "thingName": str,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef = TypedDict(
+    "_RequiredListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef = TypedDict(
+    "_OptionalListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef(
+    _RequiredListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef,
+    _OptionalListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef,
+):
+    pass
+
+
+ListDimensionsRequestListDimensionsPaginateTypeDef = TypedDict(
+    "ListDimensionsRequestListDimensionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef = TypedDict(
+    "ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef",
+    {
+        "serviceType": ServiceTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListFleetMetricsRequestListFleetMetricsPaginateTypeDef = TypedDict(
+    "ListFleetMetricsRequestListFleetMetricsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListIndicesRequestListIndicesPaginateTypeDef = TypedDict(
+    "ListIndicesRequestListIndicesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef = TypedDict(
+    "_RequiredListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef",
+    {
+        "jobId": str,
+    },
+)
+_OptionalListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef = TypedDict(
+    "_OptionalListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef",
+    {
+        "status": JobExecutionStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef(
+    _RequiredListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef,
+    _OptionalListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef = TypedDict(
+    "_RequiredListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef",
+    {
+        "thingName": str,
+    },
+)
+_OptionalListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef = TypedDict(
+    "_OptionalListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef",
+    {
+        "status": JobExecutionStatusType,
+        "namespaceId": str,
+        "jobId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef(
+    _RequiredListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef,
+    _OptionalListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef,
+):
+    pass
+
+
+ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "ListJobsRequestListJobsPaginateTypeDef",
+    {
+        "status": JobStatusType,
+        "targetSelection": TargetSelectionType,
+        "thingGroupName": str,
+        "thingGroupId": str,
+        "namespaceId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef = TypedDict(
+    "ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef",
+    {
+        "templateName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListMetricValuesRequestListMetricValuesPaginateTypeDef = TypedDict(
+    "_RequiredListMetricValuesRequestListMetricValuesPaginateTypeDef",
+    {
+        "thingName": str,
+        "metricName": str,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListMetricValuesRequestListMetricValuesPaginateTypeDef = TypedDict(
+    "_OptionalListMetricValuesRequestListMetricValuesPaginateTypeDef",
+    {
+        "dimensionName": str,
+        "dimensionValueOperator": DimensionValueOperatorType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListMetricValuesRequestListMetricValuesPaginateTypeDef(
+    _RequiredListMetricValuesRequestListMetricValuesPaginateTypeDef,
+    _OptionalListMetricValuesRequestListMetricValuesPaginateTypeDef,
+):
+    pass
+
+
+ListMitigationActionsRequestListMitigationActionsPaginateTypeDef = TypedDict(
+    "ListMitigationActionsRequestListMitigationActionsPaginateTypeDef",
+    {
+        "actionType": MitigationActionTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef = TypedDict(
+    "ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef",
+    {
+        "otaUpdateStatus": OTAUpdateStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef = TypedDict(
+    "ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
+    {
+        "packageName": str,
+    },
+)
+_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
+    {
+        "status": PackageVersionStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPackageVersionsRequestListPackageVersionsPaginateTypeDef(
+    _RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+    _OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+):
+    pass
+
+
+ListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
+    "ListPackagesRequestListPackagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPoliciesRequestListPoliciesPaginateTypeDef = TypedDict(
+    "ListPoliciesRequestListPoliciesPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef = TypedDict(
+    "_RequiredListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef",
+    {
+        "policyName": str,
+    },
+)
+_OptionalListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef = TypedDict(
+    "_OptionalListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef(
+    _RequiredListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef,
+    _OptionalListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef",
+    {
+        "principal": str,
+    },
+)
+_OptionalListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef(
+    _RequiredListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef,
+    _OptionalListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef = TypedDict(
+    "_RequiredListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef",
+    {
+        "principal": str,
+    },
+)
+_OptionalListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef = TypedDict(
+    "_OptionalListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef(
+    _RequiredListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef,
+    _OptionalListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef",
+    {
+        "templateName": str,
+    },
+)
+_OptionalListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef(
+    _RequiredListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef,
+    _OptionalListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef,
+):
+    pass
+
+
+ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef = TypedDict(
+    "ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef = TypedDict(
+    "_RequiredListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef",
+    {
+        "findingId": str,
+    },
+)
+_OptionalListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef = TypedDict(
+    "_OptionalListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef(
+    _RequiredListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef,
+    _OptionalListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef,
+):
+    pass
+
+
+ListRoleAliasesRequestListRoleAliasesPaginateTypeDef = TypedDict(
+    "ListRoleAliasesRequestListRoleAliasesPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef = TypedDict(
+    "ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef",
+        {
+            "securityProfileTargetArn": str,
+        },
+    )
+)
+_OptionalListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef",
+        {
+            "recursive": bool,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+
+class ListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef(
+    _RequiredListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef,
+    _OptionalListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef,
+):
+    pass
+
+
+ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef = TypedDict(
+    "ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef",
+    {
+        "dimensionName": str,
+        "metricName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListStreamsRequestListStreamsPaginateTypeDef = TypedDict(
+    "ListStreamsRequestListStreamsPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
+_RequiredListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef = TypedDict(
+    "_RequiredListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef",
+    {
+        "policyName": str,
+    },
+)
+_OptionalListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef = TypedDict(
+    "_OptionalListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef(
+    _RequiredListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
+    _OptionalListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef = (
+    TypedDict(
+        "_RequiredListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef",
+        {
+            "securityProfileName": str,
+        },
+    )
+)
+_OptionalListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef = (
+    TypedDict(
+        "_OptionalListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef",
+        {
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+
+class ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef(
+    _RequiredListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef,
+    _OptionalListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef,
+):
+    pass
+
+
+_RequiredListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef = TypedDict(
+    "_RequiredListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef",
+    {
+        "thingName": str,
+    },
+)
+_OptionalListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef = TypedDict(
+    "_OptionalListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef(
+    _RequiredListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef,
+    _OptionalListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef,
+):
+    pass
+
+
+ListThingGroupsRequestListThingGroupsPaginateTypeDef = TypedDict(
+    "ListThingGroupsRequestListThingGroupsPaginateTypeDef",
+    {
+        "parentGroup": str,
+        "namePrefixFilter": str,
+        "recursive": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef = TypedDict(
+    "_RequiredListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef",
+    {
+        "thingName": str,
+    },
+)
+_OptionalListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef = TypedDict(
+    "_OptionalListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef(
+    _RequiredListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef,
+    _OptionalListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef = TypedDict(
+    "_RequiredListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef",
+    {
+        "taskId": str,
+        "reportType": ReportTypeType,
+    },
+)
+_OptionalListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef = TypedDict(
+    "_OptionalListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef(
+    _RequiredListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef,
+    _OptionalListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef,
+):
+    pass
+
+
+ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef = TypedDict(
+    "ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef",
+    {
+        "status": StatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListThingTypesRequestListThingTypesPaginateTypeDef = TypedDict(
+    "ListThingTypesRequestListThingTypesPaginateTypeDef",
+    {
+        "thingTypeName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef = TypedDict(
+    "_RequiredListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef",
+    {
+        "billingGroupName": str,
+    },
+)
+_OptionalListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef = TypedDict(
+    "_OptionalListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef(
+    _RequiredListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef,
+    _OptionalListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef = TypedDict(
+    "_RequiredListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef",
+    {
+        "thingGroupName": str,
+    },
+)
+_OptionalListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef = TypedDict(
+    "_OptionalListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef",
+    {
+        "recursive": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef(
+    _RequiredListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef,
+    _OptionalListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef,
+):
+    pass
+
+
+ListThingsRequestListThingsPaginateTypeDef = TypedDict(
+    "ListThingsRequestListThingsPaginateTypeDef",
+    {
+        "attributeName": str,
+        "attributeValue": str,
+        "thingTypeName": str,
+        "usePrefixAttributeValue": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef = TypedDict(
+    "ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTopicRulesRequestListTopicRulesPaginateTypeDef = TypedDict(
+    "ListTopicRulesRequestListTopicRulesPaginateTypeDef",
+    {
+        "topic": str,
+        "ruleDisabled": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef = TypedDict(
+    "ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef",
+    {
+        "targetType": LogTargetTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListViolationEventsRequestListViolationEventsPaginateTypeDef = TypedDict(
+    "_RequiredListViolationEventsRequestListViolationEventsPaginateTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListViolationEventsRequestListViolationEventsPaginateTypeDef = TypedDict(
+    "_OptionalListViolationEventsRequestListViolationEventsPaginateTypeDef",
+    {
+        "thingName": str,
+        "securityProfileName": str,
+        "behaviorCriteriaType": BehaviorCriteriaTypeType,
+        "listSuppressedAlerts": bool,
+        "verificationState": VerificationStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListViolationEventsRequestListViolationEventsPaginateTypeDef(
+    _RequiredListViolationEventsRequestListViolationEventsPaginateTypeDef,
+    _OptionalListViolationEventsRequestListViolationEventsPaginateTypeDef,
+):
+    pass
+
+
 GetPackageConfigurationResponseTypeDef = TypedDict(
     "GetPackageConfigurationResponseTypeDef",
     {
         "versionUpdateByJobsConfig": VersionUpdateByJobsConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePackageConfigurationRequestRequestTypeDef = TypedDict(
     "UpdatePackageConfigurationRequestRequestTypeDef",
     {
         "versionUpdateByJobsConfig": VersionUpdateByJobsConfigTypeDef,
@@ -7800,50 +8036,50 @@
     total=False,
 )
 
 GetPercentilesResponseTypeDef = TypedDict(
     "GetPercentilesResponseTypeDef",
     {
         "percentiles": List[PercentPairTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStatisticsResponseTypeDef = TypedDict(
     "GetStatisticsResponseTypeDef",
     {
         "statistics": StatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBillingGroupsResponseTypeDef = TypedDict(
     "ListBillingGroupsResponseTypeDef",
     {
         "billingGroups": List[GroupNameAndArnTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListThingGroupsForThingResponseTypeDef = TypedDict(
     "ListThingGroupsForThingResponseTypeDef",
     {
         "thingGroups": List[GroupNameAndArnTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListThingGroupsResponseTypeDef = TypedDict(
     "ListThingGroupsResponseTypeDef",
     {
         "thingGroups": List[GroupNameAndArnTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ThingGroupMetadataTypeDef = TypedDict(
     "ThingGroupMetadataTypeDef",
     {
         "parentGroupName": str,
@@ -7857,28 +8093,55 @@
     "HttpAuthorizationTypeDef",
     {
         "sigv4": SigV4AuthorizationTypeDef,
     },
     total=False,
 )
 
+_RequiredThingIndexingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredThingIndexingConfigurationOutputTypeDef",
+    {
+        "thingIndexingMode": ThingIndexingModeType,
+    },
+)
+_OptionalThingIndexingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalThingIndexingConfigurationOutputTypeDef",
+    {
+        "thingConnectivityIndexingMode": ThingConnectivityIndexingModeType,
+        "deviceDefenderIndexingMode": DeviceDefenderIndexingModeType,
+        "namedShadowIndexingMode": NamedShadowIndexingModeType,
+        "managedFields": List[FieldTypeDef],
+        "customFields": List[FieldTypeDef],
+        "filter": IndexingFilterOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class ThingIndexingConfigurationOutputTypeDef(
+    _RequiredThingIndexingConfigurationOutputTypeDef,
+    _OptionalThingIndexingConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredThingIndexingConfigurationTypeDef = TypedDict(
     "_RequiredThingIndexingConfigurationTypeDef",
     {
         "thingIndexingMode": ThingIndexingModeType,
     },
 )
 _OptionalThingIndexingConfigurationTypeDef = TypedDict(
     "_OptionalThingIndexingConfigurationTypeDef",
     {
         "thingConnectivityIndexingMode": ThingConnectivityIndexingModeType,
         "deviceDefenderIndexingMode": DeviceDefenderIndexingModeType,
         "namedShadowIndexingMode": NamedShadowIndexingModeType,
-        "managedFields": List[FieldTypeDef],
-        "customFields": List[FieldTypeDef],
+        "managedFields": Sequence[FieldTypeDef],
+        "customFields": Sequence[FieldTypeDef],
         "filter": IndexingFilterTypeDef,
     },
     total=False,
 )
 
 
 class ThingIndexingConfigurationTypeDef(
@@ -7919,152 +8182,159 @@
     {
         "jobId": str,
         "jobExecutionSummary": JobExecutionSummaryTypeDef,
     },
     total=False,
 )
 
+JobExecutionsRetryConfigOutputTypeDef = TypedDict(
+    "JobExecutionsRetryConfigOutputTypeDef",
+    {
+        "criteriaList": List[RetryCriteriaTypeDef],
+    },
+)
+
 JobExecutionsRetryConfigTypeDef = TypedDict(
     "JobExecutionsRetryConfigTypeDef",
     {
         "criteriaList": Sequence[RetryCriteriaTypeDef],
     },
 )
 
 ListJobsResponseTypeDef = TypedDict(
     "ListJobsResponseTypeDef",
     {
         "jobs": List[JobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobTemplatesResponseTypeDef = TypedDict(
     "ListJobTemplatesResponseTypeDef",
     {
         "jobTemplates": List[JobTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListManagedJobTemplatesResponseTypeDef = TypedDict(
     "ListManagedJobTemplatesResponseTypeDef",
     {
         "managedJobTemplates": List[ManagedJobTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMitigationActionsResponseTypeDef = TypedDict(
     "ListMitigationActionsResponseTypeDef",
     {
         "actionIdentifiers": List[MitigationActionIdentifierTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOTAUpdatesResponseTypeDef = TypedDict(
     "ListOTAUpdatesResponseTypeDef",
     {
         "otaUpdates": List[OTAUpdateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOutgoingCertificatesResponseTypeDef = TypedDict(
     "ListOutgoingCertificatesResponseTypeDef",
     {
         "outgoingCertificates": List[OutgoingCertificateTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPackageVersionsResponseTypeDef = TypedDict(
     "ListPackageVersionsResponseTypeDef",
     {
         "packageVersionSummaries": List[PackageVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPackagesResponseTypeDef = TypedDict(
     "ListPackagesResponseTypeDef",
     {
         "packageSummaries": List[PackageSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPolicyVersionsResponseTypeDef = TypedDict(
     "ListPolicyVersionsResponseTypeDef",
     {
         "policyVersions": List[PolicyVersionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProvisioningTemplateVersionsResponseTypeDef = TypedDict(
     "ListProvisioningTemplateVersionsResponseTypeDef",
     {
         "versions": List[ProvisioningTemplateVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProvisioningTemplatesResponseTypeDef = TypedDict(
     "ListProvisioningTemplatesResponseTypeDef",
     {
         "templates": List[ProvisioningTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListScheduledAuditsResponseTypeDef = TypedDict(
     "ListScheduledAuditsResponseTypeDef",
     {
         "scheduledAudits": List[ScheduledAuditMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSecurityProfilesResponseTypeDef = TypedDict(
     "ListSecurityProfilesResponseTypeDef",
     {
         "securityProfileIdentifiers": List[SecurityProfileIdentifierTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamsResponseTypeDef = TypedDict(
     "ListStreamsResponseTypeDef",
     {
         "streams": List[StreamSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTargetsForSecurityProfileResponseTypeDef = TypedDict(
     "ListTargetsForSecurityProfileResponseTypeDef",
     {
         "securityProfileTargets": List[SecurityProfileTargetTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SecurityProfileTargetMappingTypeDef = TypedDict(
     "SecurityProfileTargetMappingTypeDef",
     {
         "securityProfileIdentifier": SecurityProfileIdentifierTypeDef,
@@ -8074,24 +8344,24 @@
 )
 
 ListThingsResponseTypeDef = TypedDict(
     "ListThingsResponseTypeDef",
     {
         "things": List[ThingAttributeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTopicRulesResponseTypeDef = TypedDict(
     "ListTopicRulesResponseTypeDef",
     {
         "rules": List[TopicRuleListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredLocationActionTypeDef = TypedDict(
     "_RequiredLocationActionTypeDef",
     {
         "roleArn": str,
@@ -8134,27 +8404,53 @@
 SetLoggingOptionsRequestRequestTypeDef = TypedDict(
     "SetLoggingOptionsRequestRequestTypeDef",
     {
         "loggingOptionsPayload": LoggingOptionsPayloadTypeDef,
     },
 )
 
+MitigationActionParamsOutputTypeDef = TypedDict(
+    "MitigationActionParamsOutputTypeDef",
+    {
+        "updateDeviceCertificateParams": UpdateDeviceCertificateParamsTypeDef,
+        "updateCACertificateParams": UpdateCACertificateParamsTypeDef,
+        "addThingsToThingGroupParams": AddThingsToThingGroupParamsOutputTypeDef,
+        "replaceDefaultPolicyVersionParams": ReplaceDefaultPolicyVersionParamsTypeDef,
+        "enableIoTLoggingParams": EnableIoTLoggingParamsTypeDef,
+        "publishFindingToSnsParams": PublishFindingToSnsParamsTypeDef,
+    },
+    total=False,
+)
+
 MitigationActionParamsTypeDef = TypedDict(
     "MitigationActionParamsTypeDef",
     {
         "updateDeviceCertificateParams": UpdateDeviceCertificateParamsTypeDef,
         "updateCACertificateParams": UpdateCACertificateParamsTypeDef,
         "addThingsToThingGroupParams": AddThingsToThingGroupParamsTypeDef,
         "replaceDefaultPolicyVersionParams": ReplaceDefaultPolicyVersionParamsTypeDef,
         "enableIoTLoggingParams": EnableIoTLoggingParamsTypeDef,
         "publishFindingToSnsParams": PublishFindingToSnsParamsTypeDef,
     },
     total=False,
 )
 
+MqttHeadersOutputTypeDef = TypedDict(
+    "MqttHeadersOutputTypeDef",
+    {
+        "payloadFormatIndicator": str,
+        "contentType": str,
+        "responseTopic": str,
+        "correlationData": str,
+        "messageExpiry": str,
+        "userProperties": List[UserPropertyTypeDef],
+    },
+    total=False,
+)
+
 MqttHeadersTypeDef = TypedDict(
     "MqttHeadersTypeDef",
     {
         "payloadFormatIndicator": str,
         "contentType": str,
         "responseTopic": str,
         "correlationData": str,
@@ -8177,40 +8473,14 @@
         "roleAliasArn": str,
         "issuerCertificateIdentifier": IssuerCertificateIdentifierTypeDef,
         "deviceCertificateArn": str,
     },
     total=False,
 )
 
-_RequiredTestInvokeAuthorizerRequestRequestTypeDef = TypedDict(
-    "_RequiredTestInvokeAuthorizerRequestRequestTypeDef",
-    {
-        "authorizerName": str,
-    },
-)
-_OptionalTestInvokeAuthorizerRequestRequestTypeDef = TypedDict(
-    "_OptionalTestInvokeAuthorizerRequestRequestTypeDef",
-    {
-        "token": str,
-        "tokenSignature": str,
-        "httpContext": HttpContextTypeDef,
-        "mqttContext": MqttContextTypeDef,
-        "tlsContext": TlsContextTypeDef,
-    },
-    total=False,
-)
-
-
-class TestInvokeAuthorizerRequestRequestTypeDef(
-    _RequiredTestInvokeAuthorizerRequestRequestTypeDef,
-    _OptionalTestInvokeAuthorizerRequestRequestTypeDef,
-):
-    pass
-
-
 ThingDocumentTypeDef = TypedDict(
     "ThingDocumentTypeDef",
     {
         "thingName": str,
         "thingId": str,
         "thingTypeName": str,
         "thingGroupNames": List[str],
@@ -8218,14 +8488,38 @@
         "shadow": str,
         "deviceDefender": str,
         "connectivity": ThingConnectivityTypeDef,
     },
     total=False,
 )
 
+_RequiredTimestreamActionOutputTypeDef = TypedDict(
+    "_RequiredTimestreamActionOutputTypeDef",
+    {
+        "roleArn": str,
+        "databaseName": str,
+        "tableName": str,
+        "dimensions": List[TimestreamDimensionTypeDef],
+    },
+)
+_OptionalTimestreamActionOutputTypeDef = TypedDict(
+    "_OptionalTimestreamActionOutputTypeDef",
+    {
+        "timestamp": TimestreamTimestampTypeDef,
+    },
+    total=False,
+)
+
+
+class TimestreamActionOutputTypeDef(
+    _RequiredTimestreamActionOutputTypeDef, _OptionalTimestreamActionOutputTypeDef
+):
+    pass
+
+
 _RequiredTimestreamActionTypeDef = TypedDict(
     "_RequiredTimestreamActionTypeDef",
     {
         "roleArn": str,
         "databaseName": str,
         "tableName": str,
         "dimensions": Sequence[TimestreamDimensionTypeDef],
@@ -8282,36 +8576,62 @@
 )
 
 ValidateSecurityProfileBehaviorsResponseTypeDef = TypedDict(
     "ValidateSecurityProfileBehaviorsResponseTypeDef",
     {
         "valid": bool,
         "validationErrors": List[ValidationErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AbortConfigUnionTypeDef = Union[AbortConfigTypeDef, AbortConfigOutputTypeDef]
 ListMetricValuesResponseTypeDef = TypedDict(
     "ListMetricValuesResponseTypeDef",
     {
         "metricDatumList": List[MetricDatumTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeniedTypeDef = TypedDict(
     "DeniedTypeDef",
     {
         "implicitDeny": ImplicitDenyTypeDef,
         "explicitDeny": ExplicitDenyTypeDef,
     },
     total=False,
 )
 
+_RequiredPutAssetPropertyValueEntryOutputTypeDef = TypedDict(
+    "_RequiredPutAssetPropertyValueEntryOutputTypeDef",
+    {
+        "propertyValues": List[AssetPropertyValueTypeDef],
+    },
+)
+_OptionalPutAssetPropertyValueEntryOutputTypeDef = TypedDict(
+    "_OptionalPutAssetPropertyValueEntryOutputTypeDef",
+    {
+        "entryId": str,
+        "assetId": str,
+        "propertyId": str,
+        "propertyAlias": str,
+    },
+    total=False,
+)
+
+
+class PutAssetPropertyValueEntryOutputTypeDef(
+    _RequiredPutAssetPropertyValueEntryOutputTypeDef,
+    _OptionalPutAssetPropertyValueEntryOutputTypeDef,
+):
+    pass
+
+
 _RequiredPutAssetPropertyValueEntryTypeDef = TypedDict(
     "_RequiredPutAssetPropertyValueEntryTypeDef",
     {
         "propertyValues": Sequence[AssetPropertyValueTypeDef],
     },
 )
 _OptionalPutAssetPropertyValueEntryTypeDef = TypedDict(
@@ -8377,14 +8697,17 @@
 
 class CreateThingGroupRequestRequestTypeDef(
     _RequiredCreateThingGroupRequestRequestTypeDef, _OptionalCreateThingGroupRequestRequestTypeDef
 ):
     pass
 
 
+ThingGroupPropertiesUnionTypeDef = Union[
+    ThingGroupPropertiesTypeDef, ThingGroupPropertiesOutputTypeDef
+]
 _RequiredUpdateDynamicThingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDynamicThingGroupRequestRequestTypeDef",
     {
         "thingGroupName": str,
         "thingGroupProperties": ThingGroupPropertiesTypeDef,
     },
 )
@@ -8425,23 +8748,70 @@
 
 class UpdateThingGroupRequestRequestTypeDef(
     _RequiredUpdateThingGroupRequestRequestTypeDef, _OptionalUpdateThingGroupRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredTestAuthorizationRequestRequestTypeDef = TypedDict(
+    "_RequiredTestAuthorizationRequestRequestTypeDef",
+    {
+        "authInfos": Sequence[AuthInfoUnionTypeDef],
+    },
+)
+_OptionalTestAuthorizationRequestRequestTypeDef = TypedDict(
+    "_OptionalTestAuthorizationRequestRequestTypeDef",
+    {
+        "principal": str,
+        "cognitoIdentityPoolId": str,
+        "clientId": str,
+        "policyNamesToAdd": Sequence[str],
+        "policyNamesToSkip": Sequence[str],
+    },
+    total=False,
+)
+
+
+class TestAuthorizationRequestRequestTypeDef(
+    _RequiredTestAuthorizationRequestRequestTypeDef, _OptionalTestAuthorizationRequestRequestTypeDef
+):
+    pass
+
+
 AwsJobExecutionsRolloutConfigTypeDef = TypedDict(
     "AwsJobExecutionsRolloutConfigTypeDef",
     {
         "maximumPerMinute": int,
         "exponentialRate": AwsJobExponentialRolloutRateTypeDef,
     },
     total=False,
 )
 
+_RequiredBehaviorOutputTypeDef = TypedDict(
+    "_RequiredBehaviorOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalBehaviorOutputTypeDef = TypedDict(
+    "_OptionalBehaviorOutputTypeDef",
+    {
+        "metric": str,
+        "metricDimension": MetricDimensionTypeDef,
+        "criteria": BehaviorCriteriaOutputTypeDef,
+        "suppressAlerts": bool,
+    },
+    total=False,
+)
+
+
+class BehaviorOutputTypeDef(_RequiredBehaviorOutputTypeDef, _OptionalBehaviorOutputTypeDef):
+    pass
+
+
 _RequiredBehaviorTypeDef = TypedDict(
     "_RequiredBehaviorTypeDef",
     {
         "name": str,
     },
 )
 _OptionalBehaviorTypeDef = TypedDict(
@@ -8456,14 +8826,51 @@
 )
 
 
 class BehaviorTypeDef(_RequiredBehaviorTypeDef, _OptionalBehaviorTypeDef):
     pass
 
 
+CustomCodeSigningTypeDef = TypedDict(
+    "CustomCodeSigningTypeDef",
+    {
+        "signature": CodeSigningSignatureTypeDef,
+        "certificateChain": CodeSigningCertificateChainTypeDef,
+        "hashAlgorithm": str,
+        "signatureAlgorithm": str,
+    },
+    total=False,
+)
+
+_RequiredTestInvokeAuthorizerRequestRequestTypeDef = TypedDict(
+    "_RequiredTestInvokeAuthorizerRequestRequestTypeDef",
+    {
+        "authorizerName": str,
+    },
+)
+_OptionalTestInvokeAuthorizerRequestRequestTypeDef = TypedDict(
+    "_OptionalTestInvokeAuthorizerRequestRequestTypeDef",
+    {
+        "token": str,
+        "tokenSignature": str,
+        "httpContext": HttpContextTypeDef,
+        "mqttContext": MqttContextTypeDef,
+        "tlsContext": TlsContextTypeDef,
+    },
+    total=False,
+)
+
+
+class TestInvokeAuthorizerRequestRequestTypeDef(
+    _RequiredTestInvokeAuthorizerRequestRequestTypeDef,
+    _OptionalTestInvokeAuthorizerRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredGetBucketsAggregationRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketsAggregationRequestRequestTypeDef",
     {
         "queryString": str,
         "aggregationField": str,
         "bucketsAggregationType": BucketsAggregationTypeTypeDef,
     },
@@ -8486,32 +8893,63 @@
 
 
 DescribeCACertificateResponseTypeDef = TypedDict(
     "DescribeCACertificateResponseTypeDef",
     {
         "certificateDescription": CACertificateDescriptionTypeDef,
         "registrationConfig": RegistrationConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCertificateResponseTypeDef = TypedDict(
     "DescribeCertificateResponseTypeDef",
     {
         "certificateDescription": CertificateDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
+    "_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef",
+    {
+        "taskId": str,
+        "target": DetectMitigationActionsTaskTargetTypeDef,
+        "actions": Sequence[str],
+        "clientRequestToken": str,
+    },
+)
+_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
+    "_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef",
+    {
+        "violationEventOccurrenceRange": ViolationEventOccurrenceRangeTypeDef,
+        "includeOnlyActiveViolations": bool,
+        "includeSuppressedAlerts": bool,
     },
+    total=False,
 )
 
+
+class StartDetectMitigationActionsTaskRequestRequestTypeDef(
+    _RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef,
+    _OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef,
+):
+    pass
+
+
+ViolationEventOccurrenceRangeUnionTypeDef = Union[
+    ViolationEventOccurrenceRangeTypeDef, ViolationEventOccurrenceRangeOutputTypeDef
+]
+SchedulingConfigUnionTypeDef = Union[SchedulingConfigTypeDef, SchedulingConfigOutputTypeDef]
 ListThingTypesResponseTypeDef = TypedDict(
     "ListThingTypesResponseTypeDef",
     {
         "thingTypes": List[ThingTypeDefinitionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartSigningJobParameterTypeDef = TypedDict(
     "StartSigningJobParameterTypeDef",
     {
         "signingProfileParameter": SigningProfileParameterTypeDef,
@@ -8526,14 +8964,17 @@
     {
         "maximumPerMinute": int,
         "exponentialRate": ExponentialRolloutRateTypeDef,
     },
     total=False,
 )
 
+ThingGroupIndexingConfigurationUnionTypeDef = Union[
+    ThingGroupIndexingConfigurationTypeDef, ThingGroupIndexingConfigurationOutputTypeDef
+]
 _RequiredCreateStreamRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStreamRequestRequestTypeDef",
     {
         "streamId": str,
         "files": Sequence[StreamFileTypeDef],
         "roleArn": str,
     },
@@ -8595,23 +9036,44 @@
 DescribeThingGroupResponseTypeDef = TypedDict(
     "DescribeThingGroupResponseTypeDef",
     {
         "thingGroupName": str,
         "thingGroupId": str,
         "thingGroupArn": str,
         "version": int,
-        "thingGroupProperties": ThingGroupPropertiesTypeDef,
+        "thingGroupProperties": ThingGroupPropertiesOutputTypeDef,
         "thingGroupMetadata": ThingGroupMetadataTypeDef,
         "indexName": str,
         "queryString": str,
         "queryVersion": str,
         "status": DynamicGroupStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredHttpActionOutputTypeDef = TypedDict(
+    "_RequiredHttpActionOutputTypeDef",
+    {
+        "url": str,
     },
 )
+_OptionalHttpActionOutputTypeDef = TypedDict(
+    "_OptionalHttpActionOutputTypeDef",
+    {
+        "confirmationUrl": str,
+        "headers": List[HttpActionHeaderTypeDef],
+        "auth": HttpAuthorizationTypeDef,
+    },
+    total=False,
+)
+
+
+class HttpActionOutputTypeDef(_RequiredHttpActionOutputTypeDef, _OptionalHttpActionOutputTypeDef):
+    pass
+
 
 _RequiredHttpActionTypeDef = TypedDict(
     "_RequiredHttpActionTypeDef",
     {
         "url": str,
     },
 )
@@ -8629,73 +9091,105 @@
 class HttpActionTypeDef(_RequiredHttpActionTypeDef, _OptionalHttpActionTypeDef):
     pass
 
 
 GetIndexingConfigurationResponseTypeDef = TypedDict(
     "GetIndexingConfigurationResponseTypeDef",
     {
-        "thingIndexingConfiguration": ThingIndexingConfigurationTypeDef,
-        "thingGroupIndexingConfiguration": ThingGroupIndexingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "thingIndexingConfiguration": ThingIndexingConfigurationOutputTypeDef,
+        "thingGroupIndexingConfiguration": ThingGroupIndexingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ThingIndexingConfigurationUnionTypeDef = Union[
+    ThingIndexingConfigurationTypeDef, ThingIndexingConfigurationOutputTypeDef
+]
 UpdateIndexingConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateIndexingConfigurationRequestRequestTypeDef",
     {
         "thingIndexingConfiguration": ThingIndexingConfigurationTypeDef,
         "thingGroupIndexingConfiguration": ThingGroupIndexingConfigurationTypeDef,
     },
     total=False,
 )
 
 DescribeJobExecutionResponseTypeDef = TypedDict(
     "DescribeJobExecutionResponseTypeDef",
     {
         "execution": JobExecutionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobExecutionsForJobResponseTypeDef = TypedDict(
     "ListJobExecutionsForJobResponseTypeDef",
     {
         "executionSummaries": List[JobExecutionSummaryForJobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobExecutionsForThingResponseTypeDef = TypedDict(
     "ListJobExecutionsForThingResponseTypeDef",
     {
         "executionSummaries": List[JobExecutionSummaryForThingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+JobExecutionsRetryConfigUnionTypeDef = Union[
+    JobExecutionsRetryConfigTypeDef, JobExecutionsRetryConfigOutputTypeDef
+]
 ListSecurityProfilesForTargetResponseTypeDef = TypedDict(
     "ListSecurityProfilesForTargetResponseTypeDef",
     {
         "securityProfileTargetMappings": List[SecurityProfileTargetMappingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListV2LoggingLevelsResponseTypeDef = TypedDict(
     "ListV2LoggingLevelsResponseTypeDef",
     {
         "logTargetConfigurations": List[LogTargetConfigurationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeMitigationActionResponseTypeDef = TypedDict(
+    "DescribeMitigationActionResponseTypeDef",
+    {
+        "actionName": str,
+        "actionType": MitigationActionTypeType,
+        "actionArn": str,
+        "actionId": str,
+        "roleArn": str,
+        "actionParams": MitigationActionParamsOutputTypeDef,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MitigationActionTypeDef = TypedDict(
+    "MitigationActionTypeDef",
+    {
+        "name": str,
+        "id": str,
+        "roleArn": str,
+        "actionParams": MitigationActionParamsOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateMitigationActionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMitigationActionRequestRequestTypeDef",
     {
         "actionName": str,
         "roleArn": str,
         "actionParams": MitigationActionParamsTypeDef,
     },
@@ -8712,59 +9206,59 @@
 class CreateMitigationActionRequestRequestTypeDef(
     _RequiredCreateMitigationActionRequestRequestTypeDef,
     _OptionalCreateMitigationActionRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeMitigationActionResponseTypeDef = TypedDict(
-    "DescribeMitigationActionResponseTypeDef",
+MitigationActionParamsUnionTypeDef = Union[
+    MitigationActionParamsTypeDef, MitigationActionParamsOutputTypeDef
+]
+_RequiredUpdateMitigationActionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateMitigationActionRequestRequestTypeDef",
     {
         "actionName": str,
-        "actionType": MitigationActionTypeType,
-        "actionArn": str,
-        "actionId": str,
-        "roleArn": str,
-        "actionParams": MitigationActionParamsTypeDef,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-
-MitigationActionTypeDef = TypedDict(
-    "MitigationActionTypeDef",
+_OptionalUpdateMitigationActionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateMitigationActionRequestRequestTypeDef",
     {
-        "name": str,
-        "id": str,
         "roleArn": str,
         "actionParams": MitigationActionParamsTypeDef,
     },
     total=False,
 )
 
-_RequiredUpdateMitigationActionRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateMitigationActionRequestRequestTypeDef",
+
+class UpdateMitigationActionRequestRequestTypeDef(
+    _RequiredUpdateMitigationActionRequestRequestTypeDef,
+    _OptionalUpdateMitigationActionRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredRepublishActionOutputTypeDef = TypedDict(
+    "_RequiredRepublishActionOutputTypeDef",
     {
-        "actionName": str,
+        "roleArn": str,
+        "topic": str,
     },
 )
-_OptionalUpdateMitigationActionRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateMitigationActionRequestRequestTypeDef",
+_OptionalRepublishActionOutputTypeDef = TypedDict(
+    "_OptionalRepublishActionOutputTypeDef",
     {
-        "roleArn": str,
-        "actionParams": MitigationActionParamsTypeDef,
+        "qos": int,
+        "headers": MqttHeadersOutputTypeDef,
     },
     total=False,
 )
 
 
-class UpdateMitigationActionRequestRequestTypeDef(
-    _RequiredUpdateMitigationActionRequestRequestTypeDef,
-    _OptionalUpdateMitigationActionRequestRequestTypeDef,
+class RepublishActionOutputTypeDef(
+    _RequiredRepublishActionOutputTypeDef, _OptionalRepublishActionOutputTypeDef
 ):
     pass
 
 
 _RequiredRepublishActionTypeDef = TypedDict(
     "_RequiredRepublishActionTypeDef",
     {
@@ -8815,15 +9309,15 @@
         "resourceIdentifier": ResourceIdentifierTypeDef,
         "clientRequestToken": str,
     },
 )
 _OptionalCreateAuditSuppressionRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAuditSuppressionRequestRequestTypeDef",
     {
-        "expirationDate": Union[datetime, str],
+        "expirationDate": TimestampTypeDef,
         "suppressIndefinitely": bool,
         "description": str,
     },
     total=False,
 )
 
 
@@ -8854,54 +9348,54 @@
     "DescribeAuditSuppressionResponseTypeDef",
     {
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
         "expirationDate": datetime,
         "suppressIndefinitely": bool,
         "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAuditFindingsRequestListAuditFindingsPaginateTypeDef = TypedDict(
     "ListAuditFindingsRequestListAuditFindingsPaginateTypeDef",
     {
         "taskId": str,
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
         "listSuppressedFindings": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListAuditFindingsRequestRequestTypeDef = TypedDict(
     "ListAuditFindingsRequestRequestTypeDef",
     {
         "taskId": str,
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
         "maxResults": int,
         "nextToken": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
         "listSuppressedFindings": bool,
     },
     total=False,
 )
 
 ListAuditSuppressionsRequestListAuditSuppressionsPaginateTypeDef = TypedDict(
     "ListAuditSuppressionsRequestListAuditSuppressionsPaginateTypeDef",
     {
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
         "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListAuditSuppressionsRequestRequestTypeDef = TypedDict(
     "ListAuditSuppressionsRequestRequestTypeDef",
     {
@@ -8940,15 +9434,15 @@
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
     },
 )
 _OptionalUpdateAuditSuppressionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateAuditSuppressionRequestRequestTypeDef",
     {
-        "expirationDate": Union[datetime, str],
+        "expirationDate": TimestampTypeDef,
         "suppressIndefinitely": bool,
         "description": str,
     },
     total=False,
 )
 
 
@@ -8961,15 +9455,15 @@
 
 SearchIndexResponseTypeDef = TypedDict(
     "SearchIndexResponseTypeDef",
     {
         "nextToken": str,
         "things": List[ThingDocumentTypeDef],
         "thingGroups": List[ThingGroupDocumentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTopicRuleDestinationRequestRequestTypeDef = TypedDict(
     "CreateTopicRuleDestinationRequestRequestTypeDef",
     {
         "destinationConfiguration": TopicRuleDestinationConfigurationTypeDef,
@@ -8977,186 +9471,141 @@
 )
 
 ListTopicRuleDestinationsResponseTypeDef = TypedDict(
     "ListTopicRuleDestinationsResponseTypeDef",
     {
         "destinationSummaries": List[TopicRuleDestinationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTopicRuleDestinationResponseTypeDef = TypedDict(
     "CreateTopicRuleDestinationResponseTypeDef",
     {
         "topicRuleDestination": TopicRuleDestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTopicRuleDestinationResponseTypeDef = TypedDict(
     "GetTopicRuleDestinationResponseTypeDef",
     {
         "topicRuleDestination": TopicRuleDestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AuthResultTypeDef = TypedDict(
     "AuthResultTypeDef",
     {
-        "authInfo": AuthInfoTypeDef,
+        "authInfo": AuthInfoOutputTypeDef,
         "allowed": AllowedTypeDef,
         "denied": DeniedTypeDef,
         "authDecision": AuthDecisionType,
         "missingContextValues": List[str],
     },
     total=False,
 )
 
+IotSiteWiseActionOutputTypeDef = TypedDict(
+    "IotSiteWiseActionOutputTypeDef",
+    {
+        "putAssetPropertyValueEntries": List[PutAssetPropertyValueEntryOutputTypeDef],
+        "roleArn": str,
+    },
+)
+
 IotSiteWiseActionTypeDef = TypedDict(
     "IotSiteWiseActionTypeDef",
     {
         "putAssetPropertyValueEntries": Sequence[PutAssetPropertyValueEntryTypeDef],
         "roleArn": str,
     },
 )
 
 ActiveViolationTypeDef = TypedDict(
     "ActiveViolationTypeDef",
     {
         "violationId": str,
         "thingName": str,
         "securityProfileName": str,
-        "behavior": BehaviorTypeDef,
-        "lastViolationValue": MetricValueTypeDef,
+        "behavior": BehaviorOutputTypeDef,
+        "lastViolationValue": MetricValueOutputTypeDef,
         "violationEventAdditionalInfo": ViolationEventAdditionalInfoTypeDef,
         "verificationState": VerificationStateType,
         "verificationStateDescription": str,
         "lastViolationTime": datetime,
         "violationStartTime": datetime,
     },
     total=False,
 )
 
-_RequiredCreateSecurityProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSecurityProfileRequestRequestTypeDef",
-    {
-        "securityProfileName": str,
-    },
-)
-_OptionalCreateSecurityProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSecurityProfileRequestRequestTypeDef",
-    {
-        "securityProfileDescription": str,
-        "behaviors": Sequence[BehaviorTypeDef],
-        "alertTargets": Mapping[Literal["SNS"], AlertTargetTypeDef],
-        "additionalMetricsToRetain": Sequence[str],
-        "additionalMetricsToRetainV2": Sequence[MetricToRetainTypeDef],
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateSecurityProfileRequestRequestTypeDef(
-    _RequiredCreateSecurityProfileRequestRequestTypeDef,
-    _OptionalCreateSecurityProfileRequestRequestTypeDef,
-):
-    pass
-
-
 DescribeSecurityProfileResponseTypeDef = TypedDict(
     "DescribeSecurityProfileResponseTypeDef",
     {
         "securityProfileName": str,
         "securityProfileArn": str,
         "securityProfileDescription": str,
-        "behaviors": List[BehaviorTypeDef],
+        "behaviors": List[BehaviorOutputTypeDef],
         "alertTargets": Dict[Literal["SNS"], AlertTargetTypeDef],
         "additionalMetricsToRetain": List[str],
         "additionalMetricsToRetainV2": List[MetricToRetainTypeDef],
         "version": int,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSecurityProfileRequestRequestTypeDef",
-    {
-        "securityProfileName": str,
-    },
-)
-_OptionalUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSecurityProfileRequestRequestTypeDef",
-    {
-        "securityProfileDescription": str,
-        "behaviors": Sequence[BehaviorTypeDef],
-        "alertTargets": Mapping[Literal["SNS"], AlertTargetTypeDef],
-        "additionalMetricsToRetain": Sequence[str],
-        "additionalMetricsToRetainV2": Sequence[MetricToRetainTypeDef],
-        "deleteBehaviors": bool,
-        "deleteAlertTargets": bool,
-        "deleteAdditionalMetricsToRetain": bool,
-        "expectedVersion": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class UpdateSecurityProfileRequestRequestTypeDef(
-    _RequiredUpdateSecurityProfileRequestRequestTypeDef,
-    _OptionalUpdateSecurityProfileRequestRequestTypeDef,
-):
-    pass
-
-
 UpdateSecurityProfileResponseTypeDef = TypedDict(
     "UpdateSecurityProfileResponseTypeDef",
     {
         "securityProfileName": str,
         "securityProfileArn": str,
         "securityProfileDescription": str,
-        "behaviors": List[BehaviorTypeDef],
+        "behaviors": List[BehaviorOutputTypeDef],
         "alertTargets": Dict[Literal["SNS"], AlertTargetTypeDef],
         "additionalMetricsToRetain": List[str],
         "additionalMetricsToRetainV2": List[MetricToRetainTypeDef],
         "version": int,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ValidateSecurityProfileBehaviorsRequestRequestTypeDef = TypedDict(
-    "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
-    {
-        "behaviors": Sequence[BehaviorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ViolationEventTypeDef = TypedDict(
     "ViolationEventTypeDef",
     {
         "violationId": str,
         "thingName": str,
         "securityProfileName": str,
-        "behavior": BehaviorTypeDef,
-        "metricValue": MetricValueTypeDef,
+        "behavior": BehaviorOutputTypeDef,
+        "metricValue": MetricValueOutputTypeDef,
         "violationEventAdditionalInfo": ViolationEventAdditionalInfoTypeDef,
         "violationEventType": ViolationEventTypeType,
         "verificationState": VerificationStateType,
         "verificationStateDescription": str,
         "violationEventTime": datetime,
     },
     total=False,
 )
 
+BehaviorUnionTypeDef = Union[BehaviorTypeDef, BehaviorOutputTypeDef]
+CodeSigningOutputTypeDef = TypedDict(
+    "CodeSigningOutputTypeDef",
+    {
+        "awsSignerJobId": str,
+        "startSigningJobParameter": StartSigningJobParameterTypeDef,
+        "customCodeSigning": CustomCodeSigningOutputTypeDef,
+    },
+    total=False,
+)
+
 CodeSigningTypeDef = TypedDict(
     "CodeSigningTypeDef",
     {
         "awsSignerJobId": str,
         "startSigningJobParameter": StartSigningJobParameterTypeDef,
         "customCodeSigning": CustomCodeSigningTypeDef,
     },
@@ -9238,20 +9687,20 @@
         "jobTemplateId": str,
         "description": str,
         "documentSource": str,
         "document": str,
         "createdAt": datetime,
         "presignedUrlConfig": PresignedUrlConfigTypeDef,
         "jobExecutionsRolloutConfig": JobExecutionsRolloutConfigTypeDef,
-        "abortConfig": AbortConfigTypeDef,
+        "abortConfig": AbortConfigOutputTypeDef,
         "timeoutConfig": TimeoutConfigTypeDef,
-        "jobExecutionsRetryConfig": JobExecutionsRetryConfigTypeDef,
+        "jobExecutionsRetryConfig": JobExecutionsRetryConfigOutputTypeDef,
         "maintenanceWindows": List[MaintenanceWindowTypeDef],
         "destinationPackageVersions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
         "jobArn": str,
@@ -9261,26 +9710,26 @@
         "forceCanceled": bool,
         "reasonCode": str,
         "comment": str,
         "targets": List[str],
         "description": str,
         "presignedUrlConfig": PresignedUrlConfigTypeDef,
         "jobExecutionsRolloutConfig": JobExecutionsRolloutConfigTypeDef,
-        "abortConfig": AbortConfigTypeDef,
+        "abortConfig": AbortConfigOutputTypeDef,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "completedAt": datetime,
         "jobProcessDetails": JobProcessDetailsTypeDef,
         "timeoutConfig": TimeoutConfigTypeDef,
         "namespaceId": str,
         "jobTemplateArn": str,
-        "jobExecutionsRetryConfig": JobExecutionsRetryConfigTypeDef,
+        "jobExecutionsRetryConfig": JobExecutionsRetryConfigOutputTypeDef,
         "documentParameters": Dict[str, str],
         "isConcurrent": bool,
-        "schedulingConfig": SchedulingConfigTypeDef,
+        "schedulingConfig": SchedulingConfigOutputTypeDef,
         "scheduledJobRollouts": List[ScheduledJobRolloutTypeDef],
         "destinationPackageVersions": List[str],
     },
     total=False,
 )
 
 _RequiredUpdateJobRequestRequestTypeDef = TypedDict(
@@ -9310,55 +9759,55 @@
     pass
 
 
 DescribeStreamResponseTypeDef = TypedDict(
     "DescribeStreamResponseTypeDef",
     {
         "streamInfo": StreamInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAuditMitigationActionsTaskResponseTypeDef = TypedDict(
     "DescribeAuditMitigationActionsTaskResponseTypeDef",
     {
         "taskStatus": AuditMitigationActionsTaskStatusType,
         "startTime": datetime,
         "endTime": datetime,
         "taskStatistics": Dict[str, TaskStatisticsForAuditCheckTypeDef],
-        "target": AuditMitigationActionsTaskTargetTypeDef,
+        "target": AuditMitigationActionsTaskTargetOutputTypeDef,
         "auditCheckToActionsMapping": Dict[str, List[str]],
         "actionsDefinition": List[MitigationActionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectMitigationActionsTaskSummaryTypeDef = TypedDict(
     "DetectMitigationActionsTaskSummaryTypeDef",
     {
         "taskId": str,
         "taskStatus": DetectMitigationActionsTaskStatusType,
         "taskStartTime": datetime,
         "taskEndTime": datetime,
-        "target": DetectMitigationActionsTaskTargetTypeDef,
-        "violationEventOccurrenceRange": ViolationEventOccurrenceRangeTypeDef,
+        "target": DetectMitigationActionsTaskTargetOutputTypeDef,
+        "violationEventOccurrenceRange": ViolationEventOccurrenceRangeOutputTypeDef,
         "onlyActiveViolationsIncluded": bool,
         "suppressedAlertsIncluded": bool,
         "actionsDefinition": List[MitigationActionTypeDef],
         "taskStatistics": DetectMitigationActionsTaskStatisticsTypeDef,
     },
     total=False,
 )
 
 ListAuditSuppressionsResponseTypeDef = TypedDict(
     "ListAuditSuppressionsResponseTypeDef",
     {
         "suppressions": List[AuditSuppressionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AuditFindingTypeDef = TypedDict(
     "AuditFindingTypeDef",
     {
         "findingId": str,
@@ -9377,26 +9826,56 @@
 )
 
 ListRelatedResourcesForAuditFindingResponseTypeDef = TypedDict(
     "ListRelatedResourcesForAuditFindingResponseTypeDef",
     {
         "relatedResources": List[RelatedResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestAuthorizationResponseTypeDef = TypedDict(
     "TestAuthorizationResponseTypeDef",
     {
         "authResults": List[AuthResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ActionOutputTypeDef = TypedDict(
+    "ActionOutputTypeDef",
+    {
+        "dynamoDB": DynamoDBActionTypeDef,
+        "dynamoDBv2": DynamoDBv2ActionTypeDef,
+        "lambda": LambdaActionTypeDef,
+        "sns": SnsActionTypeDef,
+        "sqs": SqsActionTypeDef,
+        "kinesis": KinesisActionTypeDef,
+        "republish": RepublishActionOutputTypeDef,
+        "s3": S3ActionTypeDef,
+        "firehose": FirehoseActionTypeDef,
+        "cloudwatchMetric": CloudwatchMetricActionTypeDef,
+        "cloudwatchAlarm": CloudwatchAlarmActionTypeDef,
+        "cloudwatchLogs": CloudwatchLogsActionTypeDef,
+        "elasticsearch": ElasticsearchActionTypeDef,
+        "salesforce": SalesforceActionTypeDef,
+        "iotAnalytics": IotAnalyticsActionTypeDef,
+        "iotEvents": IotEventsActionTypeDef,
+        "iotSiteWise": IotSiteWiseActionOutputTypeDef,
+        "stepFunctions": StepFunctionsActionTypeDef,
+        "timestream": TimestreamActionOutputTypeDef,
+        "http": HttpActionOutputTypeDef,
+        "kafka": KafkaActionOutputTypeDef,
+        "openSearch": OpenSearchActionTypeDef,
+        "location": LocationActionTypeDef,
+    },
+    total=False,
+)
+
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "dynamoDB": DynamoDBActionTypeDef,
         "dynamoDBv2": DynamoDBv2ActionTypeDef,
         "lambda": LambdaActionTypeDef,
         "sns": SnsActionTypeDef,
@@ -9424,25 +9903,102 @@
 )
 
 ListActiveViolationsResponseTypeDef = TypedDict(
     "ListActiveViolationsResponseTypeDef",
     {
         "activeViolations": List[ActiveViolationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListViolationEventsResponseTypeDef = TypedDict(
     "ListViolationEventsResponseTypeDef",
     {
         "violationEvents": List[ViolationEventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateSecurityProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSecurityProfileRequestRequestTypeDef",
+    {
+        "securityProfileName": str,
+    },
+)
+_OptionalCreateSecurityProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSecurityProfileRequestRequestTypeDef",
+    {
+        "securityProfileDescription": str,
+        "behaviors": Sequence[BehaviorUnionTypeDef],
+        "alertTargets": Mapping[Literal["SNS"], AlertTargetTypeDef],
+        "additionalMetricsToRetain": Sequence[str],
+        "additionalMetricsToRetainV2": Sequence[MetricToRetainTypeDef],
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateSecurityProfileRequestRequestTypeDef(
+    _RequiredCreateSecurityProfileRequestRequestTypeDef,
+    _OptionalCreateSecurityProfileRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSecurityProfileRequestRequestTypeDef",
+    {
+        "securityProfileName": str,
+    },
+)
+_OptionalUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSecurityProfileRequestRequestTypeDef",
+    {
+        "securityProfileDescription": str,
+        "behaviors": Sequence[BehaviorUnionTypeDef],
+        "alertTargets": Mapping[Literal["SNS"], AlertTargetTypeDef],
+        "additionalMetricsToRetain": Sequence[str],
+        "additionalMetricsToRetainV2": Sequence[MetricToRetainTypeDef],
+        "deleteBehaviors": bool,
+        "deleteAlertTargets": bool,
+        "deleteAdditionalMetricsToRetain": bool,
+        "expectedVersion": int,
+    },
+    total=False,
+)
+
+
+class UpdateSecurityProfileRequestRequestTypeDef(
+    _RequiredUpdateSecurityProfileRequestRequestTypeDef,
+    _OptionalUpdateSecurityProfileRequestRequestTypeDef,
+):
+    pass
+
+
+ValidateSecurityProfileBehaviorsRequestRequestTypeDef = TypedDict(
+    "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
+    {
+        "behaviors": Sequence[BehaviorUnionTypeDef],
+    },
+)
+
+OTAUpdateFileOutputTypeDef = TypedDict(
+    "OTAUpdateFileOutputTypeDef",
+    {
+        "fileName": str,
+        "fileType": int,
+        "fileVersion": str,
+        "fileLocation": FileLocationTypeDef,
+        "codeSigning": CodeSigningOutputTypeDef,
+        "attributes": Dict[str, str],
     },
+    total=False,
 )
 
 OTAUpdateFileTypeDef = TypedDict(
     "OTAUpdateFileTypeDef",
     {
         "fileName": str,
         "fileType": int,
@@ -9455,119 +10011,87 @@
 )
 
 DescribeJobResponseTypeDef = TypedDict(
     "DescribeJobResponseTypeDef",
     {
         "documentSource": str,
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDetectMitigationActionsTaskResponseTypeDef = TypedDict(
     "DescribeDetectMitigationActionsTaskResponseTypeDef",
     {
         "taskSummary": DetectMitigationActionsTaskSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDetectMitigationActionsTasksResponseTypeDef = TypedDict(
     "ListDetectMitigationActionsTasksResponseTypeDef",
     {
         "tasks": List[DetectMitigationActionsTaskSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAuditFindingResponseTypeDef = TypedDict(
     "DescribeAuditFindingResponseTypeDef",
     {
         "finding": AuditFindingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAuditFindingsResponseTypeDef = TypedDict(
     "ListAuditFindingsResponseTypeDef",
     {
         "findings": List[AuditFindingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredTopicRulePayloadTypeDef = TypedDict(
-    "_RequiredTopicRulePayloadTypeDef",
-    {
-        "sql": str,
-        "actions": Sequence[ActionTypeDef],
-    },
-)
-_OptionalTopicRulePayloadTypeDef = TypedDict(
-    "_OptionalTopicRulePayloadTypeDef",
-    {
-        "description": str,
-        "ruleDisabled": bool,
-        "awsIotSqlVersion": str,
-        "errorAction": ActionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class TopicRulePayloadTypeDef(_RequiredTopicRulePayloadTypeDef, _OptionalTopicRulePayloadTypeDef):
-    pass
-
-
 TopicRuleTypeDef = TypedDict(
     "TopicRuleTypeDef",
     {
         "ruleName": str,
         "sql": str,
         "description": str,
         "createdAt": datetime,
-        "actions": List[ActionTypeDef],
+        "actions": List[ActionOutputTypeDef],
         "ruleDisabled": bool,
         "awsIotSqlVersion": str,
-        "errorAction": ActionTypeDef,
+        "errorAction": ActionOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateOTAUpdateRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateOTAUpdateRequestRequestTypeDef",
+_RequiredTopicRulePayloadTypeDef = TypedDict(
+    "_RequiredTopicRulePayloadTypeDef",
     {
-        "otaUpdateId": str,
-        "targets": Sequence[str],
-        "files": Sequence[OTAUpdateFileTypeDef],
-        "roleArn": str,
+        "sql": str,
+        "actions": Sequence[ActionTypeDef],
     },
 )
-_OptionalCreateOTAUpdateRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateOTAUpdateRequestRequestTypeDef",
+_OptionalTopicRulePayloadTypeDef = TypedDict(
+    "_OptionalTopicRulePayloadTypeDef",
     {
         "description": str,
-        "protocols": Sequence[ProtocolType],
-        "targetSelection": TargetSelectionType,
-        "awsJobExecutionsRolloutConfig": AwsJobExecutionsRolloutConfigTypeDef,
-        "awsJobPresignedUrlConfig": AwsJobPresignedUrlConfigTypeDef,
-        "awsJobAbortConfig": AwsJobAbortConfigTypeDef,
-        "awsJobTimeoutConfig": AwsJobTimeoutConfigTypeDef,
-        "additionalParameters": Mapping[str, str],
-        "tags": Sequence[TagTypeDef],
+        "ruleDisabled": bool,
+        "awsIotSqlVersion": str,
+        "errorAction": ActionTypeDef,
     },
     total=False,
 )
 
 
-class CreateOTAUpdateRequestRequestTypeDef(
-    _RequiredCreateOTAUpdateRequestRequestTypeDef, _OptionalCreateOTAUpdateRequestRequestTypeDef
-):
+class TopicRulePayloadTypeDef(_RequiredTopicRulePayloadTypeDef, _OptionalTopicRulePayloadTypeDef):
     pass
 
 
 OTAUpdateInfoTypeDef = TypedDict(
     "OTAUpdateInfoTypeDef",
     {
         "otaUpdateId": str,
@@ -9576,24 +10100,34 @@
         "lastModifiedDate": datetime,
         "description": str,
         "targets": List[str],
         "protocols": List[ProtocolType],
         "awsJobExecutionsRolloutConfig": AwsJobExecutionsRolloutConfigTypeDef,
         "awsJobPresignedUrlConfig": AwsJobPresignedUrlConfigTypeDef,
         "targetSelection": TargetSelectionType,
-        "otaUpdateFiles": List[OTAUpdateFileTypeDef],
+        "otaUpdateFiles": List[OTAUpdateFileOutputTypeDef],
         "otaUpdateStatus": OTAUpdateStatusType,
         "awsIotJobId": str,
         "awsIotJobArn": str,
         "errorInfo": ErrorInfoTypeDef,
         "additionalParameters": Dict[str, str],
     },
     total=False,
 )
 
+OTAUpdateFileUnionTypeDef = Union[OTAUpdateFileTypeDef, OTAUpdateFileOutputTypeDef]
+GetTopicRuleResponseTypeDef = TypedDict(
+    "GetTopicRuleResponseTypeDef",
+    {
+        "ruleArn": str,
+        "rule": TopicRuleTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateTopicRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTopicRuleRequestRequestTypeDef",
     {
         "ruleName": str,
         "topicRulePayload": TopicRulePayloadTypeDef,
     },
 )
@@ -9616,23 +10150,45 @@
     "ReplaceTopicRuleRequestRequestTypeDef",
     {
         "ruleName": str,
         "topicRulePayload": TopicRulePayloadTypeDef,
     },
 )
 
-GetTopicRuleResponseTypeDef = TypedDict(
-    "GetTopicRuleResponseTypeDef",
+GetOTAUpdateResponseTypeDef = TypedDict(
+    "GetOTAUpdateResponseTypeDef",
     {
-        "ruleArn": str,
-        "rule": TopicRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "otaUpdateInfo": OTAUpdateInfoTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetOTAUpdateResponseTypeDef = TypedDict(
-    "GetOTAUpdateResponseTypeDef",
+_RequiredCreateOTAUpdateRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateOTAUpdateRequestRequestTypeDef",
     {
-        "otaUpdateInfo": OTAUpdateInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "otaUpdateId": str,
+        "targets": Sequence[str],
+        "files": Sequence[OTAUpdateFileUnionTypeDef],
+        "roleArn": str,
     },
 )
+_OptionalCreateOTAUpdateRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateOTAUpdateRequestRequestTypeDef",
+    {
+        "description": str,
+        "protocols": Sequence[ProtocolType],
+        "targetSelection": TargetSelectionType,
+        "awsJobExecutionsRolloutConfig": AwsJobExecutionsRolloutConfigTypeDef,
+        "awsJobPresignedUrlConfig": AwsJobPresignedUrlConfigTypeDef,
+        "awsJobAbortConfig": AwsJobAbortConfigTypeDef,
+        "awsJobTimeoutConfig": AwsJobTimeoutConfigTypeDef,
+        "additionalParameters": Mapping[str, str],
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateOTAUpdateRequestRequestTypeDef(
+    _RequiredCreateOTAUpdateRequestRequestTypeDef, _OptionalCreateOTAUpdateRequestRequestTypeDef
+):
+    pass
```

### Comparing `types-aiobotocore-iot-2.5.2/types_aiobotocore_iot/type_defs.pyi` & `types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_iot.type_defs import AbortCriteriaTypeDef
 
-    data: AbortCriteriaTypeDef = {...}
+    data: AbortCriteriaTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -98,118 +98,101 @@
     "CloudwatchLogsActionTypeDef",
     "CloudwatchMetricActionTypeDef",
     "DynamoDBActionTypeDef",
     "ElasticsearchActionTypeDef",
     "FirehoseActionTypeDef",
     "IotAnalyticsActionTypeDef",
     "IotEventsActionTypeDef",
-    "KafkaActionTypeDef",
+    "KafkaActionOutputTypeDef",
     "KinesisActionTypeDef",
     "LambdaActionTypeDef",
     "OpenSearchActionTypeDef",
     "S3ActionTypeDef",
     "SalesforceActionTypeDef",
     "SnsActionTypeDef",
     "SqsActionTypeDef",
     "StepFunctionsActionTypeDef",
-    "MetricValueTypeDef",
+    "KafkaActionTypeDef",
+    "MetricValueOutputTypeDef",
     "ViolationEventAdditionalInfoTypeDef",
     "AddThingToBillingGroupRequestRequestTypeDef",
     "AddThingToThingGroupRequestRequestTypeDef",
+    "AddThingsToThingGroupParamsOutputTypeDef",
     "AddThingsToThingGroupParamsTypeDef",
+    "AggregationTypeOutputTypeDef",
     "AggregationTypeTypeDef",
     "AlertTargetTypeDef",
     "PolicyTypeDef",
     "AssetPropertyTimestampTypeDef",
     "AssetPropertyVariantTypeDef",
     "AssociateTargetsWithJobRequestRequestTypeDef",
-    "AssociateTargetsWithJobResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AttachPolicyRequestRequestTypeDef",
     "AttachPrincipalPolicyRequestRequestTypeDef",
     "AttachSecurityProfileRequestRequestTypeDef",
     "AttachThingPrincipalRequestRequestTypeDef",
+    "AttributePayloadOutputTypeDef",
     "AttributePayloadTypeDef",
     "AuditCheckConfigurationTypeDef",
     "AuditCheckDetailsTypeDef",
     "AuditMitigationActionExecutionMetadataTypeDef",
     "AuditMitigationActionsTaskMetadataTypeDef",
+    "AuditMitigationActionsTaskTargetOutputTypeDef",
     "AuditMitigationActionsTaskTargetTypeDef",
     "AuditNotificationTargetTypeDef",
     "AuditTaskMetadataTypeDef",
+    "AuthInfoOutputTypeDef",
     "AuthInfoTypeDef",
     "AuthorizerConfigTypeDef",
     "AuthorizerDescriptionTypeDef",
     "AuthorizerSummaryTypeDef",
     "AwsJobAbortCriteriaTypeDef",
     "AwsJobRateIncreaseCriteriaTypeDef",
     "AwsJobPresignedUrlConfigTypeDef",
     "AwsJobTimeoutConfigTypeDef",
     "MachineLearningDetectionConfigTypeDef",
     "StatisticalThresholdTypeDef",
+    "MetricValueTypeDef",
     "BehaviorModelTrainingSummaryTypeDef",
     "MetricDimensionTypeDef",
     "BillingGroupMetadataTypeDef",
     "BillingGroupPropertiesTypeDef",
+    "BlobTypeDef",
     "BucketTypeDef",
     "TermsAggregationTypeDef",
     "CertificateValidityTypeDef",
     "CACertificateTypeDef",
     "CancelAuditMitigationActionsTaskRequestRequestTypeDef",
     "CancelAuditTaskRequestRequestTypeDef",
     "CancelCertificateTransferRequestRequestTypeDef",
     "CancelDetectMitigationActionsTaskRequestRequestTypeDef",
     "CancelJobExecutionRequestRequestTypeDef",
     "CancelJobRequestRequestTypeDef",
-    "CancelJobResponseTypeDef",
     "TransferDataTypeDef",
     "CertificateTypeDef",
     "CodeSigningCertificateChainTypeDef",
-    "CodeSigningSignatureTypeDef",
+    "CodeSigningSignatureOutputTypeDef",
     "ConfigurationTypeDef",
     "ConfirmTopicRuleDestinationRequestRequestTypeDef",
+    "TimestampTypeDef",
     "TagTypeDef",
-    "CreateAuthorizerResponseTypeDef",
-    "CreateBillingGroupResponseTypeDef",
     "CreateCertificateFromCsrRequestRequestTypeDef",
-    "CreateCertificateFromCsrResponseTypeDef",
-    "CreateCustomMetricResponseTypeDef",
-    "CreateDimensionResponseTypeDef",
     "TlsConfigTypeDef",
-    "CreateDomainConfigurationResponseTypeDef",
-    "CreateDynamicThingGroupResponseTypeDef",
-    "CreateFleetMetricResponseTypeDef",
     "PresignedUrlConfigTypeDef",
     "TimeoutConfigTypeDef",
-    "CreateJobResponseTypeDef",
     "MaintenanceWindowTypeDef",
-    "CreateJobTemplateResponseTypeDef",
     "CreateKeysAndCertificateRequestRequestTypeDef",
     "KeyPairTypeDef",
-    "CreateMitigationActionResponseTypeDef",
-    "CreateOTAUpdateResponseTypeDef",
     "CreatePackageRequestRequestTypeDef",
-    "CreatePackageResponseTypeDef",
     "CreatePackageVersionRequestRequestTypeDef",
-    "CreatePackageVersionResponseTypeDef",
-    "CreatePolicyResponseTypeDef",
     "CreatePolicyVersionRequestRequestTypeDef",
-    "CreatePolicyVersionResponseTypeDef",
     "CreateProvisioningClaimRequestRequestTypeDef",
     "ProvisioningHookTypeDef",
-    "CreateProvisioningTemplateResponseTypeDef",
     "CreateProvisioningTemplateVersionRequestRequestTypeDef",
-    "CreateProvisioningTemplateVersionResponseTypeDef",
-    "CreateRoleAliasResponseTypeDef",
-    "CreateScheduledAuditResponseTypeDef",
-    "CreateSecurityProfileResponseTypeDef",
-    "CreateStreamResponseTypeDef",
-    "CreateThingGroupResponseTypeDef",
-    "CreateThingResponseTypeDef",
     "ThingTypePropertiesTypeDef",
-    "CreateThingTypeResponseTypeDef",
     "DeleteAccountAuditConfigurationRequestRequestTypeDef",
     "DeleteAuthorizerRequestRequestTypeDef",
     "DeleteBillingGroupRequestRequestTypeDef",
     "DeleteCACertificateRequestRequestTypeDef",
     "DeleteCertificateRequestRequestTypeDef",
     "DeleteCustomMetricRequestRequestTypeDef",
     "DeleteDimensionRequestRequestTypeDef",
@@ -245,374 +228,355 @@
     "TaskStatisticsTypeDef",
     "DescribeAuthorizerRequestRequestTypeDef",
     "DescribeBillingGroupRequestRequestTypeDef",
     "DescribeCACertificateRequestRequestTypeDef",
     "RegistrationConfigTypeDef",
     "DescribeCertificateRequestRequestTypeDef",
     "DescribeCustomMetricRequestRequestTypeDef",
-    "DescribeCustomMetricResponseTypeDef",
     "DescribeDetectMitigationActionsTaskRequestRequestTypeDef",
     "DescribeDimensionRequestRequestTypeDef",
-    "DescribeDimensionResponseTypeDef",
     "DescribeDomainConfigurationRequestRequestTypeDef",
     "ServerCertificateSummaryTypeDef",
     "DescribeEndpointRequestRequestTypeDef",
-    "DescribeEndpointResponseTypeDef",
     "DescribeFleetMetricRequestRequestTypeDef",
     "DescribeIndexRequestRequestTypeDef",
-    "DescribeIndexResponseTypeDef",
     "DescribeJobExecutionRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
     "DescribeJobTemplateRequestRequestTypeDef",
     "DescribeManagedJobTemplateRequestRequestTypeDef",
     "DocumentParameterTypeDef",
     "DescribeMitigationActionRequestRequestTypeDef",
     "DescribeProvisioningTemplateRequestRequestTypeDef",
     "DescribeProvisioningTemplateVersionRequestRequestTypeDef",
-    "DescribeProvisioningTemplateVersionResponseTypeDef",
     "DescribeRoleAliasRequestRequestTypeDef",
     "RoleAliasDescriptionTypeDef",
     "DescribeScheduledAuditRequestRequestTypeDef",
-    "DescribeScheduledAuditResponseTypeDef",
     "DescribeSecurityProfileRequestRequestTypeDef",
     "DescribeStreamRequestRequestTypeDef",
     "DescribeThingGroupRequestRequestTypeDef",
     "DescribeThingRegistrationTaskRequestRequestTypeDef",
-    "DescribeThingRegistrationTaskResponseTypeDef",
     "DescribeThingRequestRequestTypeDef",
-    "DescribeThingResponseTypeDef",
     "DescribeThingTypeRequestRequestTypeDef",
     "ThingTypeMetadataTypeDef",
+    "ThingTypePropertiesOutputTypeDef",
     "S3DestinationTypeDef",
     "DetachPolicyRequestRequestTypeDef",
     "DetachPrincipalPolicyRequestRequestTypeDef",
     "DetachSecurityProfileRequestRequestTypeDef",
     "DetachThingPrincipalRequestRequestTypeDef",
     "DetectMitigationActionExecutionTypeDef",
     "DetectMitigationActionsTaskStatisticsTypeDef",
+    "DetectMitigationActionsTaskTargetOutputTypeDef",
+    "ViolationEventOccurrenceRangeOutputTypeDef",
     "DetectMitigationActionsTaskTargetTypeDef",
-    "ViolationEventOccurrenceRangeTypeDef",
     "DisableTopicRuleRequestRequestTypeDef",
     "DomainConfigurationSummaryTypeDef",
     "PutItemInputTypeDef",
     "EffectivePolicyTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableIoTLoggingParamsTypeDef",
     "EnableTopicRuleRequestRequestTypeDef",
     "ErrorInfoTypeDef",
     "RateIncreaseCriteriaTypeDef",
     "FieldTypeDef",
     "S3LocationTypeDef",
     "StreamTypeDef",
     "FleetMetricNameAndArnTypeDef",
-    "GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetBehaviorModelTrainingSummariesRequestRequestTypeDef",
     "GetCardinalityRequestRequestTypeDef",
-    "GetCardinalityResponseTypeDef",
     "GetEffectivePoliciesRequestRequestTypeDef",
     "GetJobDocumentRequestRequestTypeDef",
-    "GetJobDocumentResponseTypeDef",
-    "GetLoggingOptionsResponseTypeDef",
     "GetOTAUpdateRequestRequestTypeDef",
     "VersionUpdateByJobsConfigTypeDef",
     "GetPackageRequestRequestTypeDef",
-    "GetPackageResponseTypeDef",
     "GetPackageVersionRequestRequestTypeDef",
-    "GetPackageVersionResponseTypeDef",
     "GetPercentilesRequestRequestTypeDef",
     "PercentPairTypeDef",
     "GetPolicyRequestRequestTypeDef",
-    "GetPolicyResponseTypeDef",
     "GetPolicyVersionRequestRequestTypeDef",
-    "GetPolicyVersionResponseTypeDef",
-    "GetRegistrationCodeResponseTypeDef",
     "GetStatisticsRequestRequestTypeDef",
     "StatisticsTypeDef",
     "GetTopicRuleDestinationRequestRequestTypeDef",
     "GetTopicRuleRequestRequestTypeDef",
-    "GetV2LoggingOptionsResponseTypeDef",
     "GroupNameAndArnTypeDef",
     "HttpActionHeaderTypeDef",
     "SigV4AuthorizationTypeDef",
     "HttpContextTypeDef",
     "HttpUrlDestinationConfigurationTypeDef",
     "HttpUrlDestinationPropertiesTypeDef",
     "HttpUrlDestinationSummaryTypeDef",
+    "IndexingFilterOutputTypeDef",
     "IndexingFilterTypeDef",
     "IssuerCertificateIdentifierTypeDef",
     "JobExecutionStatusDetailsTypeDef",
     "JobExecutionSummaryTypeDef",
     "RetryCriteriaTypeDef",
     "JobProcessDetailsTypeDef",
     "JobSummaryTypeDef",
     "JobTemplateSummaryTypeDef",
     "ScheduledJobRolloutTypeDef",
-    "ListActiveViolationsRequestListActiveViolationsPaginateTypeDef",
     "ListActiveViolationsRequestRequestTypeDef",
-    "ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef",
     "ListAttachedPoliciesRequestRequestTypeDef",
-    "ListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef",
     "ListAuditMitigationActionsExecutionsRequestRequestTypeDef",
-    "ListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef",
-    "ListAuditMitigationActionsTasksRequestRequestTypeDef",
-    "ListAuditTasksRequestListAuditTasksPaginateTypeDef",
-    "ListAuditTasksRequestRequestTypeDef",
-    "ListAuthorizersRequestListAuthorizersPaginateTypeDef",
     "ListAuthorizersRequestRequestTypeDef",
-    "ListBillingGroupsRequestListBillingGroupsPaginateTypeDef",
     "ListBillingGroupsRequestRequestTypeDef",
-    "ListCACertificatesRequestListCACertificatesPaginateTypeDef",
     "ListCACertificatesRequestRequestTypeDef",
-    "ListCertificatesByCARequestListCertificatesByCAPaginateTypeDef",
     "ListCertificatesByCARequestRequestTypeDef",
-    "ListCertificatesRequestListCertificatesPaginateTypeDef",
     "ListCertificatesRequestRequestTypeDef",
-    "ListCustomMetricsRequestListCustomMetricsPaginateTypeDef",
     "ListCustomMetricsRequestRequestTypeDef",
-    "ListCustomMetricsResponseTypeDef",
-    "ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef",
-    "ListDetectMitigationActionsExecutionsRequestRequestTypeDef",
-    "ListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef",
-    "ListDetectMitigationActionsTasksRequestRequestTypeDef",
-    "ListDimensionsRequestListDimensionsPaginateTypeDef",
     "ListDimensionsRequestRequestTypeDef",
-    "ListDimensionsResponseTypeDef",
-    "ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef",
     "ListDomainConfigurationsRequestRequestTypeDef",
-    "ListFleetMetricsRequestListFleetMetricsPaginateTypeDef",
     "ListFleetMetricsRequestRequestTypeDef",
-    "ListIndicesRequestListIndicesPaginateTypeDef",
     "ListIndicesRequestRequestTypeDef",
-    "ListIndicesResponseTypeDef",
-    "ListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef",
     "ListJobExecutionsForJobRequestRequestTypeDef",
-    "ListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef",
     "ListJobExecutionsForThingRequestRequestTypeDef",
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     "ListJobTemplatesRequestRequestTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
-    "ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef",
     "ListManagedJobTemplatesRequestRequestTypeDef",
     "ManagedJobTemplateSummaryTypeDef",
-    "ListMetricValuesRequestListMetricValuesPaginateTypeDef",
-    "ListMetricValuesRequestRequestTypeDef",
-    "ListMitigationActionsRequestListMitigationActionsPaginateTypeDef",
     "ListMitigationActionsRequestRequestTypeDef",
     "MitigationActionIdentifierTypeDef",
-    "ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef",
     "ListOTAUpdatesRequestRequestTypeDef",
     "OTAUpdateSummaryTypeDef",
-    "ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef",
     "ListOutgoingCertificatesRequestRequestTypeDef",
     "OutgoingCertificateTypeDef",
-    "ListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
     "ListPackageVersionsRequestRequestTypeDef",
     "PackageVersionSummaryTypeDef",
-    "ListPackagesRequestListPackagesPaginateTypeDef",
     "ListPackagesRequestRequestTypeDef",
     "PackageSummaryTypeDef",
-    "ListPoliciesRequestListPoliciesPaginateTypeDef",
     "ListPoliciesRequestRequestTypeDef",
-    "ListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef",
     "ListPolicyPrincipalsRequestRequestTypeDef",
-    "ListPolicyPrincipalsResponseTypeDef",
     "ListPolicyVersionsRequestRequestTypeDef",
     "PolicyVersionTypeDef",
-    "ListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef",
     "ListPrincipalPoliciesRequestRequestTypeDef",
-    "ListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef",
     "ListPrincipalThingsRequestRequestTypeDef",
-    "ListPrincipalThingsResponseTypeDef",
-    "ListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef",
     "ListProvisioningTemplateVersionsRequestRequestTypeDef",
     "ProvisioningTemplateVersionSummaryTypeDef",
-    "ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef",
     "ListProvisioningTemplatesRequestRequestTypeDef",
     "ProvisioningTemplateSummaryTypeDef",
-    "ListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef",
     "ListRelatedResourcesForAuditFindingRequestRequestTypeDef",
-    "ListRoleAliasesRequestListRoleAliasesPaginateTypeDef",
     "ListRoleAliasesRequestRequestTypeDef",
-    "ListRoleAliasesResponseTypeDef",
-    "ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef",
     "ListScheduledAuditsRequestRequestTypeDef",
     "ScheduledAuditMetadataTypeDef",
-    "ListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef",
     "ListSecurityProfilesForTargetRequestRequestTypeDef",
-    "ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef",
     "ListSecurityProfilesRequestRequestTypeDef",
     "SecurityProfileIdentifierTypeDef",
-    "ListStreamsRequestListStreamsPaginateTypeDef",
     "ListStreamsRequestRequestTypeDef",
     "StreamSummaryTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef",
     "ListTargetsForPolicyRequestRequestTypeDef",
-    "ListTargetsForPolicyResponseTypeDef",
-    "ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef",
     "ListTargetsForSecurityProfileRequestRequestTypeDef",
     "SecurityProfileTargetTypeDef",
-    "ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef",
     "ListThingGroupsForThingRequestRequestTypeDef",
-    "ListThingGroupsRequestListThingGroupsPaginateTypeDef",
     "ListThingGroupsRequestRequestTypeDef",
-    "ListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef",
     "ListThingPrincipalsRequestRequestTypeDef",
-    "ListThingPrincipalsResponseTypeDef",
-    "ListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef",
     "ListThingRegistrationTaskReportsRequestRequestTypeDef",
-    "ListThingRegistrationTaskReportsResponseTypeDef",
-    "ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef",
     "ListThingRegistrationTasksRequestRequestTypeDef",
-    "ListThingRegistrationTasksResponseTypeDef",
-    "ListThingTypesRequestListThingTypesPaginateTypeDef",
     "ListThingTypesRequestRequestTypeDef",
-    "ListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef",
     "ListThingsInBillingGroupRequestRequestTypeDef",
-    "ListThingsInBillingGroupResponseTypeDef",
-    "ListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef",
     "ListThingsInThingGroupRequestRequestTypeDef",
-    "ListThingsInThingGroupResponseTypeDef",
-    "ListThingsRequestListThingsPaginateTypeDef",
     "ListThingsRequestRequestTypeDef",
     "ThingAttributeTypeDef",
-    "ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef",
     "ListTopicRuleDestinationsRequestRequestTypeDef",
-    "ListTopicRulesRequestListTopicRulesPaginateTypeDef",
     "ListTopicRulesRequestRequestTypeDef",
     "TopicRuleListItemTypeDef",
-    "ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef",
     "ListV2LoggingLevelsRequestRequestTypeDef",
-    "ListViolationEventsRequestListViolationEventsPaginateTypeDef",
-    "ListViolationEventsRequestRequestTypeDef",
     "LocationTimestampTypeDef",
     "LogTargetTypeDef",
     "LoggingOptionsPayloadTypeDef",
     "PublishFindingToSnsParamsTypeDef",
     "ReplaceDefaultPolicyVersionParamsTypeDef",
     "UpdateCACertificateParamsTypeDef",
     "UpdateDeviceCertificateParamsTypeDef",
-    "MqttContextTypeDef",
     "UserPropertyTypeDef",
-    "PaginatorConfigTypeDef",
     "PolicyVersionIdentifierTypeDef",
     "PutVerificationStateOnViolationRequestRequestTypeDef",
-    "RegisterCACertificateResponseTypeDef",
     "RegisterCertificateRequestRequestTypeDef",
-    "RegisterCertificateResponseTypeDef",
     "RegisterCertificateWithoutCARequestRequestTypeDef",
-    "RegisterCertificateWithoutCAResponseTypeDef",
     "RegisterThingRequestRequestTypeDef",
-    "RegisterThingResponseTypeDef",
     "RejectCertificateTransferRequestRequestTypeDef",
     "RemoveThingFromBillingGroupRequestRequestTypeDef",
     "RemoveThingFromThingGroupRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "SearchIndexRequestRequestTypeDef",
     "ThingGroupDocumentTypeDef",
     "SetDefaultAuthorizerRequestRequestTypeDef",
-    "SetDefaultAuthorizerResponseTypeDef",
     "SetDefaultPolicyVersionRequestRequestTypeDef",
     "SetV2LoggingOptionsRequestRequestTypeDef",
     "SigningProfileParameterTypeDef",
-    "StartAuditMitigationActionsTaskResponseTypeDef",
-    "StartDetectMitigationActionsTaskResponseTypeDef",
     "StartOnDemandAuditTaskRequestRequestTypeDef",
-    "StartOnDemandAuditTaskResponseTypeDef",
     "StartThingRegistrationTaskRequestRequestTypeDef",
-    "StartThingRegistrationTaskResponseTypeDef",
     "StopThingRegistrationTaskRequestRequestTypeDef",
     "TlsContextTypeDef",
-    "TestInvokeAuthorizerResponseTypeDef",
     "ThingConnectivityTypeDef",
     "TimestreamDimensionTypeDef",
     "TimestreamTimestampTypeDef",
     "VpcDestinationConfigurationTypeDef",
     "VpcDestinationSummaryTypeDef",
     "VpcDestinationPropertiesTypeDef",
     "TransferCertificateRequestRequestTypeDef",
-    "TransferCertificateResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAuthorizerRequestRequestTypeDef",
-    "UpdateAuthorizerResponseTypeDef",
-    "UpdateBillingGroupResponseTypeDef",
     "UpdateCertificateRequestRequestTypeDef",
     "UpdateCustomMetricRequestRequestTypeDef",
-    "UpdateCustomMetricResponseTypeDef",
     "UpdateDimensionRequestRequestTypeDef",
-    "UpdateDimensionResponseTypeDef",
-    "UpdateDomainConfigurationResponseTypeDef",
-    "UpdateDynamicThingGroupResponseTypeDef",
-    "UpdateMitigationActionResponseTypeDef",
     "UpdatePackageRequestRequestTypeDef",
     "UpdatePackageVersionRequestRequestTypeDef",
     "UpdateRoleAliasRequestRequestTypeDef",
-    "UpdateRoleAliasResponseTypeDef",
     "UpdateScheduledAuditRequestRequestTypeDef",
-    "UpdateScheduledAuditResponseTypeDef",
-    "UpdateStreamResponseTypeDef",
-    "UpdateThingGroupResponseTypeDef",
     "UpdateThingGroupsForThingRequestRequestTypeDef",
     "UpdateTopicRuleDestinationRequestRequestTypeDef",
     "ValidationErrorTypeDef",
+    "AbortConfigOutputTypeDef",
     "AbortConfigTypeDef",
     "MetricDatumTypeDef",
-    "DescribeFleetMetricResponseTypeDef",
+    "AggregationTypeUnionTypeDef",
     "UpdateFleetMetricRequestRequestTypeDef",
     "AllowedTypeDef",
     "ExplicitDenyTypeDef",
     "ImplicitDenyTypeDef",
+    "AssetPropertyValueTypeDef",
+    "AssociateTargetsWithJobResponseTypeDef",
+    "CancelJobResponseTypeDef",
+    "CreateAuthorizerResponseTypeDef",
+    "CreateBillingGroupResponseTypeDef",
+    "CreateCertificateFromCsrResponseTypeDef",
+    "CreateCustomMetricResponseTypeDef",
+    "CreateDimensionResponseTypeDef",
+    "CreateDomainConfigurationResponseTypeDef",
+    "CreateDynamicThingGroupResponseTypeDef",
+    "CreateFleetMetricResponseTypeDef",
+    "CreateJobResponseTypeDef",
+    "CreateJobTemplateResponseTypeDef",
+    "CreateMitigationActionResponseTypeDef",
+    "CreateOTAUpdateResponseTypeDef",
+    "CreatePackageResponseTypeDef",
+    "CreatePackageVersionResponseTypeDef",
+    "CreatePolicyResponseTypeDef",
+    "CreatePolicyVersionResponseTypeDef",
+    "CreateProvisioningTemplateResponseTypeDef",
+    "CreateProvisioningTemplateVersionResponseTypeDef",
+    "CreateRoleAliasResponseTypeDef",
+    "CreateScheduledAuditResponseTypeDef",
+    "CreateSecurityProfileResponseTypeDef",
+    "CreateStreamResponseTypeDef",
+    "CreateThingGroupResponseTypeDef",
+    "CreateThingResponseTypeDef",
+    "CreateThingTypeResponseTypeDef",
+    "DescribeCustomMetricResponseTypeDef",
+    "DescribeDimensionResponseTypeDef",
+    "DescribeEndpointResponseTypeDef",
+    "DescribeFleetMetricResponseTypeDef",
+    "DescribeIndexResponseTypeDef",
+    "DescribeProvisioningTemplateVersionResponseTypeDef",
+    "DescribeScheduledAuditResponseTypeDef",
+    "DescribeThingRegistrationTaskResponseTypeDef",
+    "DescribeThingResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetCardinalityResponseTypeDef",
+    "GetJobDocumentResponseTypeDef",
+    "GetLoggingOptionsResponseTypeDef",
+    "GetPackageResponseTypeDef",
+    "GetPackageVersionResponseTypeDef",
+    "GetPolicyResponseTypeDef",
+    "GetPolicyVersionResponseTypeDef",
+    "GetRegistrationCodeResponseTypeDef",
+    "GetV2LoggingOptionsResponseTypeDef",
     "ListAttachedPoliciesResponseTypeDef",
+    "ListCustomMetricsResponseTypeDef",
+    "ListDimensionsResponseTypeDef",
+    "ListIndicesResponseTypeDef",
     "ListPoliciesResponseTypeDef",
+    "ListPolicyPrincipalsResponseTypeDef",
     "ListPrincipalPoliciesResponseTypeDef",
-    "AssetPropertyValueTypeDef",
+    "ListPrincipalThingsResponseTypeDef",
+    "ListRoleAliasesResponseTypeDef",
+    "ListTargetsForPolicyResponseTypeDef",
+    "ListThingPrincipalsResponseTypeDef",
+    "ListThingRegistrationTaskReportsResponseTypeDef",
+    "ListThingRegistrationTasksResponseTypeDef",
+    "ListThingsInBillingGroupResponseTypeDef",
+    "ListThingsInThingGroupResponseTypeDef",
+    "RegisterCACertificateResponseTypeDef",
+    "RegisterCertificateResponseTypeDef",
+    "RegisterCertificateWithoutCAResponseTypeDef",
+    "RegisterThingResponseTypeDef",
+    "SetDefaultAuthorizerResponseTypeDef",
+    "StartAuditMitigationActionsTaskResponseTypeDef",
+    "StartDetectMitigationActionsTaskResponseTypeDef",
+    "StartOnDemandAuditTaskResponseTypeDef",
+    "StartThingRegistrationTaskResponseTypeDef",
+    "TestInvokeAuthorizerResponseTypeDef",
+    "TransferCertificateResponseTypeDef",
+    "UpdateAuthorizerResponseTypeDef",
+    "UpdateBillingGroupResponseTypeDef",
+    "UpdateCustomMetricResponseTypeDef",
+    "UpdateDimensionResponseTypeDef",
+    "UpdateDomainConfigurationResponseTypeDef",
+    "UpdateDynamicThingGroupResponseTypeDef",
+    "UpdateMitigationActionResponseTypeDef",
+    "UpdateRoleAliasResponseTypeDef",
+    "UpdateScheduledAuditResponseTypeDef",
+    "UpdateStreamResponseTypeDef",
+    "UpdateThingGroupResponseTypeDef",
+    "ThingGroupPropertiesOutputTypeDef",
+    "AttributePayloadUnionTypeDef",
     "CreateThingRequestRequestTypeDef",
     "ThingGroupPropertiesTypeDef",
     "UpdateThingRequestRequestTypeDef",
     "ListAuditMitigationActionsExecutionsResponseTypeDef",
     "ListAuditMitigationActionsTasksResponseTypeDef",
+    "AuditMitigationActionsTaskTargetUnionTypeDef",
     "StartAuditMitigationActionsTaskRequestRequestTypeDef",
     "DescribeAccountAuditConfigurationResponseTypeDef",
     "UpdateAccountAuditConfigurationRequestRequestTypeDef",
     "ListAuditTasksResponseTypeDef",
-    "TestAuthorizationRequestRequestTypeDef",
+    "AuthInfoUnionTypeDef",
     "DescribeAuthorizerResponseTypeDef",
     "DescribeDefaultAuthorizerResponseTypeDef",
     "ListAuthorizersResponseTypeDef",
     "AwsJobAbortConfigTypeDef",
     "AwsJobExponentialRolloutRateTypeDef",
+    "BehaviorCriteriaOutputTypeDef",
     "BehaviorCriteriaTypeDef",
     "GetBehaviorModelTrainingSummariesResponseTypeDef",
     "MetricToRetainTypeDef",
     "DescribeBillingGroupResponseTypeDef",
     "UpdateBillingGroupRequestRequestTypeDef",
+    "CodeSigningSignatureTypeDef",
+    "MqttContextTypeDef",
     "GetBucketsAggregationResponseTypeDef",
     "BucketsAggregationTypeTypeDef",
     "CACertificateDescriptionTypeDef",
     "ListCACertificatesResponseTypeDef",
     "CertificateDescriptionTypeDef",
     "ListCertificatesByCAResponseTypeDef",
     "ListCertificatesResponseTypeDef",
-    "CustomCodeSigningTypeDef",
+    "CustomCodeSigningOutputTypeDef",
     "DescribeEventConfigurationsResponseTypeDef",
     "UpdateEventConfigurationsRequestRequestTypeDef",
+    "ListAuditMitigationActionsTasksRequestRequestTypeDef",
+    "ListAuditTasksRequestRequestTypeDef",
+    "ListDetectMitigationActionsExecutionsRequestRequestTypeDef",
+    "ListDetectMitigationActionsTasksRequestRequestTypeDef",
+    "ListMetricValuesRequestRequestTypeDef",
+    "ListViolationEventsRequestRequestTypeDef",
+    "ViolationEventOccurrenceRangeTypeDef",
     "CreateAuthorizerRequestRequestTypeDef",
     "CreateBillingGroupRequestRequestTypeDef",
     "CreateCustomMetricRequestRequestTypeDef",
     "CreateDimensionRequestRequestTypeDef",
     "CreateFleetMetricRequestRequestTypeDef",
     "CreatePolicyRequestRequestTypeDef",
     "CreateRoleAliasRequestRequestTypeDef",
     "CreateScheduledAuditRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDomainConfigurationRequestRequestTypeDef",
     "UpdateDomainConfigurationRequestRequestTypeDef",
+    "SchedulingConfigOutputTypeDef",
     "SchedulingConfigTypeDef",
     "CreateKeysAndCertificateResponseTypeDef",
     "CreateProvisioningClaimResponseTypeDef",
     "CreateProvisioningTemplateRequestRequestTypeDef",
     "DescribeProvisioningTemplateResponseTypeDef",
     "UpdateProvisioningTemplateRequestRequestTypeDef",
     "CreateThingTypeRequestRequestTypeDef",
@@ -620,38 +584,99 @@
     "RegisterCACertificateRequestRequestTypeDef",
     "UpdateCACertificateRequestRequestTypeDef",
     "DescribeDomainConfigurationResponseTypeDef",
     "DescribeManagedJobTemplateResponseTypeDef",
     "DescribeRoleAliasResponseTypeDef",
     "DescribeThingTypeResponseTypeDef",
     "ThingTypeDefinitionTypeDef",
+    "ThingTypePropertiesUnionTypeDef",
     "DestinationTypeDef",
     "ListDetectMitigationActionsExecutionsResponseTypeDef",
-    "StartDetectMitigationActionsTaskRequestRequestTypeDef",
+    "DetectMitigationActionsTaskTargetUnionTypeDef",
     "ListDomainConfigurationsResponseTypeDef",
     "DynamoDBv2ActionTypeDef",
     "GetEffectivePoliciesResponseTypeDef",
     "ExponentialRolloutRateTypeDef",
+    "ThingGroupIndexingConfigurationOutputTypeDef",
     "ThingGroupIndexingConfigurationTypeDef",
     "StreamFileTypeDef",
     "FileLocationTypeDef",
     "ListFleetMetricsResponseTypeDef",
+    "GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef",
+    "ListActiveViolationsRequestListActiveViolationsPaginateTypeDef",
+    "ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef",
+    "ListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef",
+    "ListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef",
+    "ListAuditTasksRequestListAuditTasksPaginateTypeDef",
+    "ListAuthorizersRequestListAuthorizersPaginateTypeDef",
+    "ListBillingGroupsRequestListBillingGroupsPaginateTypeDef",
+    "ListCACertificatesRequestListCACertificatesPaginateTypeDef",
+    "ListCertificatesByCARequestListCertificatesByCAPaginateTypeDef",
+    "ListCertificatesRequestListCertificatesPaginateTypeDef",
+    "ListCustomMetricsRequestListCustomMetricsPaginateTypeDef",
+    "ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef",
+    "ListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef",
+    "ListDimensionsRequestListDimensionsPaginateTypeDef",
+    "ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef",
+    "ListFleetMetricsRequestListFleetMetricsPaginateTypeDef",
+    "ListIndicesRequestListIndicesPaginateTypeDef",
+    "ListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef",
+    "ListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef",
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
+    "ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef",
+    "ListMetricValuesRequestListMetricValuesPaginateTypeDef",
+    "ListMitigationActionsRequestListMitigationActionsPaginateTypeDef",
+    "ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef",
+    "ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef",
+    "ListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
+    "ListPackagesRequestListPackagesPaginateTypeDef",
+    "ListPoliciesRequestListPoliciesPaginateTypeDef",
+    "ListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef",
+    "ListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef",
+    "ListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef",
+    "ListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef",
+    "ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef",
+    "ListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef",
+    "ListRoleAliasesRequestListRoleAliasesPaginateTypeDef",
+    "ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef",
+    "ListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef",
+    "ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef",
+    "ListStreamsRequestListStreamsPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef",
+    "ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef",
+    "ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef",
+    "ListThingGroupsRequestListThingGroupsPaginateTypeDef",
+    "ListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef",
+    "ListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef",
+    "ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef",
+    "ListThingTypesRequestListThingTypesPaginateTypeDef",
+    "ListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef",
+    "ListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef",
+    "ListThingsRequestListThingsPaginateTypeDef",
+    "ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef",
+    "ListTopicRulesRequestListTopicRulesPaginateTypeDef",
+    "ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef",
+    "ListViolationEventsRequestListViolationEventsPaginateTypeDef",
     "GetPackageConfigurationResponseTypeDef",
     "UpdatePackageConfigurationRequestRequestTypeDef",
     "GetPercentilesResponseTypeDef",
     "GetStatisticsResponseTypeDef",
     "ListBillingGroupsResponseTypeDef",
     "ListThingGroupsForThingResponseTypeDef",
     "ListThingGroupsResponseTypeDef",
     "ThingGroupMetadataTypeDef",
     "HttpAuthorizationTypeDef",
+    "ThingIndexingConfigurationOutputTypeDef",
     "ThingIndexingConfigurationTypeDef",
     "JobExecutionTypeDef",
     "JobExecutionSummaryForJobTypeDef",
     "JobExecutionSummaryForThingTypeDef",
+    "JobExecutionsRetryConfigOutputTypeDef",
     "JobExecutionsRetryConfigTypeDef",
     "ListJobsResponseTypeDef",
     "ListJobTemplatesResponseTypeDef",
     "ListManagedJobTemplatesResponseTypeDef",
     "ListMitigationActionsResponseTypeDef",
     "ListOTAUpdatesResponseTypeDef",
     "ListOutgoingCertificatesResponseTypeDef",
@@ -667,55 +692,73 @@
     "SecurityProfileTargetMappingTypeDef",
     "ListThingsResponseTypeDef",
     "ListTopicRulesResponseTypeDef",
     "LocationActionTypeDef",
     "LogTargetConfigurationTypeDef",
     "SetV2LoggingLevelRequestRequestTypeDef",
     "SetLoggingOptionsRequestRequestTypeDef",
+    "MitigationActionParamsOutputTypeDef",
     "MitigationActionParamsTypeDef",
+    "MqttHeadersOutputTypeDef",
     "MqttHeadersTypeDef",
     "ResourceIdentifierTypeDef",
-    "TestInvokeAuthorizerRequestRequestTypeDef",
     "ThingDocumentTypeDef",
+    "TimestreamActionOutputTypeDef",
     "TimestreamActionTypeDef",
     "TopicRuleDestinationConfigurationTypeDef",
     "TopicRuleDestinationSummaryTypeDef",
     "TopicRuleDestinationTypeDef",
     "ValidateSecurityProfileBehaviorsResponseTypeDef",
+    "AbortConfigUnionTypeDef",
     "ListMetricValuesResponseTypeDef",
     "DeniedTypeDef",
+    "PutAssetPropertyValueEntryOutputTypeDef",
     "PutAssetPropertyValueEntryTypeDef",
     "CreateDynamicThingGroupRequestRequestTypeDef",
     "CreateThingGroupRequestRequestTypeDef",
+    "ThingGroupPropertiesUnionTypeDef",
     "UpdateDynamicThingGroupRequestRequestTypeDef",
     "UpdateThingGroupRequestRequestTypeDef",
+    "TestAuthorizationRequestRequestTypeDef",
     "AwsJobExecutionsRolloutConfigTypeDef",
+    "BehaviorOutputTypeDef",
     "BehaviorTypeDef",
+    "CustomCodeSigningTypeDef",
+    "TestInvokeAuthorizerRequestRequestTypeDef",
     "GetBucketsAggregationRequestRequestTypeDef",
     "DescribeCACertificateResponseTypeDef",
     "DescribeCertificateResponseTypeDef",
+    "StartDetectMitigationActionsTaskRequestRequestTypeDef",
+    "ViolationEventOccurrenceRangeUnionTypeDef",
+    "SchedulingConfigUnionTypeDef",
     "ListThingTypesResponseTypeDef",
     "StartSigningJobParameterTypeDef",
     "JobExecutionsRolloutConfigTypeDef",
+    "ThingGroupIndexingConfigurationUnionTypeDef",
     "CreateStreamRequestRequestTypeDef",
     "StreamInfoTypeDef",
     "UpdateStreamRequestRequestTypeDef",
     "DescribeThingGroupResponseTypeDef",
+    "HttpActionOutputTypeDef",
     "HttpActionTypeDef",
     "GetIndexingConfigurationResponseTypeDef",
+    "ThingIndexingConfigurationUnionTypeDef",
     "UpdateIndexingConfigurationRequestRequestTypeDef",
     "DescribeJobExecutionResponseTypeDef",
     "ListJobExecutionsForJobResponseTypeDef",
     "ListJobExecutionsForThingResponseTypeDef",
+    "JobExecutionsRetryConfigUnionTypeDef",
     "ListSecurityProfilesForTargetResponseTypeDef",
     "ListV2LoggingLevelsResponseTypeDef",
-    "CreateMitigationActionRequestRequestTypeDef",
     "DescribeMitigationActionResponseTypeDef",
     "MitigationActionTypeDef",
+    "CreateMitigationActionRequestRequestTypeDef",
+    "MitigationActionParamsUnionTypeDef",
     "UpdateMitigationActionRequestRequestTypeDef",
+    "RepublishActionOutputTypeDef",
     "RepublishActionTypeDef",
     "AuditSuppressionTypeDef",
     "CreateAuditSuppressionRequestRequestTypeDef",
     "DeleteAuditSuppressionRequestRequestTypeDef",
     "DescribeAuditSuppressionRequestRequestTypeDef",
     "DescribeAuditSuppressionResponseTypeDef",
     "ListAuditFindingsRequestListAuditFindingsPaginateTypeDef",
@@ -727,52 +770,58 @@
     "UpdateAuditSuppressionRequestRequestTypeDef",
     "SearchIndexResponseTypeDef",
     "CreateTopicRuleDestinationRequestRequestTypeDef",
     "ListTopicRuleDestinationsResponseTypeDef",
     "CreateTopicRuleDestinationResponseTypeDef",
     "GetTopicRuleDestinationResponseTypeDef",
     "AuthResultTypeDef",
+    "IotSiteWiseActionOutputTypeDef",
     "IotSiteWiseActionTypeDef",
     "ActiveViolationTypeDef",
-    "CreateSecurityProfileRequestRequestTypeDef",
     "DescribeSecurityProfileResponseTypeDef",
-    "UpdateSecurityProfileRequestRequestTypeDef",
     "UpdateSecurityProfileResponseTypeDef",
-    "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
     "ViolationEventTypeDef",
+    "BehaviorUnionTypeDef",
+    "CodeSigningOutputTypeDef",
     "CodeSigningTypeDef",
     "CreateJobRequestRequestTypeDef",
     "CreateJobTemplateRequestRequestTypeDef",
     "DescribeJobTemplateResponseTypeDef",
     "JobTypeDef",
     "UpdateJobRequestRequestTypeDef",
     "DescribeStreamResponseTypeDef",
     "DescribeAuditMitigationActionsTaskResponseTypeDef",
     "DetectMitigationActionsTaskSummaryTypeDef",
     "ListAuditSuppressionsResponseTypeDef",
     "AuditFindingTypeDef",
     "ListRelatedResourcesForAuditFindingResponseTypeDef",
     "TestAuthorizationResponseTypeDef",
+    "ActionOutputTypeDef",
     "ActionTypeDef",
     "ListActiveViolationsResponseTypeDef",
     "ListViolationEventsResponseTypeDef",
+    "CreateSecurityProfileRequestRequestTypeDef",
+    "UpdateSecurityProfileRequestRequestTypeDef",
+    "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
+    "OTAUpdateFileOutputTypeDef",
     "OTAUpdateFileTypeDef",
     "DescribeJobResponseTypeDef",
     "DescribeDetectMitigationActionsTaskResponseTypeDef",
     "ListDetectMitigationActionsTasksResponseTypeDef",
     "DescribeAuditFindingResponseTypeDef",
     "ListAuditFindingsResponseTypeDef",
-    "TopicRulePayloadTypeDef",
     "TopicRuleTypeDef",
-    "CreateOTAUpdateRequestRequestTypeDef",
+    "TopicRulePayloadTypeDef",
     "OTAUpdateInfoTypeDef",
+    "OTAUpdateFileUnionTypeDef",
+    "GetTopicRuleResponseTypeDef",
     "CreateTopicRuleRequestRequestTypeDef",
     "ReplaceTopicRuleRequestRequestTypeDef",
-    "GetTopicRuleResponseTypeDef",
     "GetOTAUpdateResponseTypeDef",
+    "CreateOTAUpdateRequestRequestTypeDef",
 )
 
 AbortCriteriaTypeDef = TypedDict(
     "AbortCriteriaTypeDef",
     {
         "failureType": JobExecutionFailureTypeType,
         "action": Literal["CANCEL"],
@@ -935,32 +984,34 @@
     },
     total=False,
 )
 
 class IotEventsActionTypeDef(_RequiredIotEventsActionTypeDef, _OptionalIotEventsActionTypeDef):
     pass
 
-_RequiredKafkaActionTypeDef = TypedDict(
-    "_RequiredKafkaActionTypeDef",
+_RequiredKafkaActionOutputTypeDef = TypedDict(
+    "_RequiredKafkaActionOutputTypeDef",
     {
         "destinationArn": str,
         "topic": str,
-        "clientProperties": Mapping[str, str],
+        "clientProperties": Dict[str, str],
     },
 )
-_OptionalKafkaActionTypeDef = TypedDict(
-    "_OptionalKafkaActionTypeDef",
+_OptionalKafkaActionOutputTypeDef = TypedDict(
+    "_OptionalKafkaActionOutputTypeDef",
     {
         "key": str,
         "partition": str,
     },
     total=False,
 )
 
-class KafkaActionTypeDef(_RequiredKafkaActionTypeDef, _OptionalKafkaActionTypeDef):
+class KafkaActionOutputTypeDef(
+    _RequiredKafkaActionOutputTypeDef, _OptionalKafkaActionOutputTypeDef
+):
     pass
 
 _RequiredKinesisActionTypeDef = TypedDict(
     "_RequiredKinesisActionTypeDef",
     {
         "roleArn": str,
         "streamName": str,
@@ -1074,23 +1125,43 @@
 )
 
 class StepFunctionsActionTypeDef(
     _RequiredStepFunctionsActionTypeDef, _OptionalStepFunctionsActionTypeDef
 ):
     pass
 
-MetricValueTypeDef = TypedDict(
-    "MetricValueTypeDef",
+_RequiredKafkaActionTypeDef = TypedDict(
+    "_RequiredKafkaActionTypeDef",
+    {
+        "destinationArn": str,
+        "topic": str,
+        "clientProperties": Mapping[str, str],
+    },
+)
+_OptionalKafkaActionTypeDef = TypedDict(
+    "_OptionalKafkaActionTypeDef",
+    {
+        "key": str,
+        "partition": str,
+    },
+    total=False,
+)
+
+class KafkaActionTypeDef(_RequiredKafkaActionTypeDef, _OptionalKafkaActionTypeDef):
+    pass
+
+MetricValueOutputTypeDef = TypedDict(
+    "MetricValueOutputTypeDef",
     {
         "count": int,
-        "cidrs": Sequence[str],
-        "ports": Sequence[int],
+        "cidrs": List[str],
+        "ports": List[int],
         "number": float,
-        "numbers": Sequence[float],
-        "strings": Sequence[str],
+        "numbers": List[float],
+        "strings": List[str],
     },
     total=False,
 )
 
 ViolationEventAdditionalInfoTypeDef = TypedDict(
     "ViolationEventAdditionalInfoTypeDef",
     {
@@ -1118,14 +1189,34 @@
         "thingName": str,
         "thingArn": str,
         "overrideDynamicGroups": bool,
     },
     total=False,
 )
 
+_RequiredAddThingsToThingGroupParamsOutputTypeDef = TypedDict(
+    "_RequiredAddThingsToThingGroupParamsOutputTypeDef",
+    {
+        "thingGroupNames": List[str],
+    },
+)
+_OptionalAddThingsToThingGroupParamsOutputTypeDef = TypedDict(
+    "_OptionalAddThingsToThingGroupParamsOutputTypeDef",
+    {
+        "overrideDynamicGroups": bool,
+    },
+    total=False,
+)
+
+class AddThingsToThingGroupParamsOutputTypeDef(
+    _RequiredAddThingsToThingGroupParamsOutputTypeDef,
+    _OptionalAddThingsToThingGroupParamsOutputTypeDef,
+):
+    pass
+
 _RequiredAddThingsToThingGroupParamsTypeDef = TypedDict(
     "_RequiredAddThingsToThingGroupParamsTypeDef",
     {
         "thingGroupNames": Sequence[str],
     },
 )
 _OptionalAddThingsToThingGroupParamsTypeDef = TypedDict(
@@ -1137,14 +1228,33 @@
 )
 
 class AddThingsToThingGroupParamsTypeDef(
     _RequiredAddThingsToThingGroupParamsTypeDef, _OptionalAddThingsToThingGroupParamsTypeDef
 ):
     pass
 
+_RequiredAggregationTypeOutputTypeDef = TypedDict(
+    "_RequiredAggregationTypeOutputTypeDef",
+    {
+        "name": AggregationTypeNameType,
+    },
+)
+_OptionalAggregationTypeOutputTypeDef = TypedDict(
+    "_OptionalAggregationTypeOutputTypeDef",
+    {
+        "values": List[str],
+    },
+    total=False,
+)
+
+class AggregationTypeOutputTypeDef(
+    _RequiredAggregationTypeOutputTypeDef, _OptionalAggregationTypeOutputTypeDef
+):
+    pass
+
 _RequiredAggregationTypeTypeDef = TypedDict(
     "_RequiredAggregationTypeTypeDef",
     {
         "name": AggregationTypeNameType,
     },
 )
 _OptionalAggregationTypeTypeDef = TypedDict(
@@ -1223,21 +1333,22 @@
 
 class AssociateTargetsWithJobRequestRequestTypeDef(
     _RequiredAssociateTargetsWithJobRequestRequestTypeDef,
     _OptionalAssociateTargetsWithJobRequestRequestTypeDef,
 ):
     pass
 
-AssociateTargetsWithJobResponseTypeDef = TypedDict(
-    "AssociateTargetsWithJobResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "jobArn": str,
-        "jobId": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AttachPolicyRequestRequestTypeDef = TypedDict(
     "AttachPolicyRequestRequestTypeDef",
     {
         "policyName": str,
@@ -1265,14 +1376,23 @@
     "AttachThingPrincipalRequestRequestTypeDef",
     {
         "thingName": str,
         "principal": str,
     },
 )
 
+AttributePayloadOutputTypeDef = TypedDict(
+    "AttributePayloadOutputTypeDef",
+    {
+        "attributes": Dict[str, str],
+        "merge": bool,
+    },
+    total=False,
+)
+
 AttributePayloadTypeDef = TypedDict(
     "AttributePayloadTypeDef",
     {
         "attributes": Mapping[str, str],
         "merge": bool,
     },
     total=False,
@@ -1322,24 +1442,34 @@
         "taskId": str,
         "startTime": datetime,
         "taskStatus": AuditMitigationActionsTaskStatusType,
     },
     total=False,
 )
 
-AuditMitigationActionsTaskTargetTypeDef = TypedDict(
-    "AuditMitigationActionsTaskTargetTypeDef",
+AuditMitigationActionsTaskTargetOutputTypeDef = TypedDict(
+    "AuditMitigationActionsTaskTargetOutputTypeDef",
     {
         "auditTaskId": str,
         "findingIds": List[str],
         "auditCheckToReasonCodeFilter": Dict[str, List[str]],
     },
     total=False,
 )
 
+AuditMitigationActionsTaskTargetTypeDef = TypedDict(
+    "AuditMitigationActionsTaskTargetTypeDef",
+    {
+        "auditTaskId": str,
+        "findingIds": Sequence[str],
+        "auditCheckToReasonCodeFilter": Mapping[str, Sequence[str]],
+    },
+    total=False,
+)
+
 AuditNotificationTargetTypeDef = TypedDict(
     "AuditNotificationTargetTypeDef",
     {
         "targetArn": str,
         "roleArn": str,
         "enabled": bool,
     },
@@ -1352,14 +1482,31 @@
         "taskId": str,
         "taskStatus": AuditTaskStatusType,
         "taskType": AuditTaskTypeType,
     },
     total=False,
 )
 
+_RequiredAuthInfoOutputTypeDef = TypedDict(
+    "_RequiredAuthInfoOutputTypeDef",
+    {
+        "resources": List[str],
+    },
+)
+_OptionalAuthInfoOutputTypeDef = TypedDict(
+    "_OptionalAuthInfoOutputTypeDef",
+    {
+        "actionType": ActionTypeType,
+    },
+    total=False,
+)
+
+class AuthInfoOutputTypeDef(_RequiredAuthInfoOutputTypeDef, _OptionalAuthInfoOutputTypeDef):
+    pass
+
 _RequiredAuthInfoTypeDef = TypedDict(
     "_RequiredAuthInfoTypeDef",
     {
         "resources": Sequence[str],
     },
 )
 _OptionalAuthInfoTypeDef = TypedDict(
@@ -1454,14 +1601,27 @@
     "StatisticalThresholdTypeDef",
     {
         "statistic": str,
     },
     total=False,
 )
 
+MetricValueTypeDef = TypedDict(
+    "MetricValueTypeDef",
+    {
+        "count": int,
+        "cidrs": Sequence[str],
+        "ports": Sequence[int],
+        "number": float,
+        "numbers": Sequence[float],
+        "strings": Sequence[str],
+    },
+    total=False,
+)
+
 BehaviorModelTrainingSummaryTypeDef = TypedDict(
     "BehaviorModelTrainingSummaryTypeDef",
     {
         "securityProfileName": str,
         "behaviorName": str,
         "trainingDataCollectionStartDate": datetime,
         "modelStatus": ModelStatusType,
@@ -1500,14 +1660,15 @@
     "BillingGroupPropertiesTypeDef",
     {
         "billingGroupDescription": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BucketTypeDef = TypedDict(
     "BucketTypeDef",
     {
         "keyValue": str,
         "count": int,
     },
     total=False,
@@ -1609,24 +1770,14 @@
 )
 
 class CancelJobRequestRequestTypeDef(
     _RequiredCancelJobRequestRequestTypeDef, _OptionalCancelJobRequestRequestTypeDef
 ):
     pass
 
-CancelJobResponseTypeDef = TypedDict(
-    "CancelJobResponseTypeDef",
-    {
-        "jobArn": str,
-        "jobId": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TransferDataTypeDef = TypedDict(
     "TransferDataTypeDef",
     {
         "transferMessage": str,
         "rejectReason": str,
         "transferDate": datetime,
         "acceptDate": datetime,
@@ -1652,18 +1803,18 @@
     {
         "certificateName": str,
         "inlineDocument": str,
     },
     total=False,
 )
 
-CodeSigningSignatureTypeDef = TypedDict(
-    "CodeSigningSignatureTypeDef",
+CodeSigningSignatureOutputTypeDef = TypedDict(
+    "CodeSigningSignatureOutputTypeDef",
     {
-        "inlineDocument": Union[str, bytes, IO[Any], StreamingBody],
+        "inlineDocument": bytes,
     },
     total=False,
 )
 
 ConfigurationTypeDef = TypedDict(
     "ConfigurationTypeDef",
     {
@@ -1675,14 +1826,15 @@
 ConfirmTopicRuleDestinationRequestRequestTypeDef = TypedDict(
     "ConfirmTopicRuleDestinationRequestRequestTypeDef",
     {
         "confirmationToken": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalTagTypeDef = TypedDict(
@@ -1692,33 +1844,14 @@
     },
     total=False,
 )
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
-CreateAuthorizerResponseTypeDef = TypedDict(
-    "CreateAuthorizerResponseTypeDef",
-    {
-        "authorizerName": str,
-        "authorizerArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateBillingGroupResponseTypeDef = TypedDict(
-    "CreateBillingGroupResponseTypeDef",
-    {
-        "billingGroupName": str,
-        "billingGroupArn": str,
-        "billingGroupId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateCertificateFromCsrRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCertificateFromCsrRequestRequestTypeDef",
     {
         "certificateSigningRequest": str,
     },
 )
 _OptionalCreateCertificateFromCsrRequestRequestTypeDef = TypedDict(
@@ -1731,81 +1864,22 @@
 
 class CreateCertificateFromCsrRequestRequestTypeDef(
     _RequiredCreateCertificateFromCsrRequestRequestTypeDef,
     _OptionalCreateCertificateFromCsrRequestRequestTypeDef,
 ):
     pass
 
-CreateCertificateFromCsrResponseTypeDef = TypedDict(
-    "CreateCertificateFromCsrResponseTypeDef",
-    {
-        "certificateArn": str,
-        "certificateId": str,
-        "certificatePem": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateCustomMetricResponseTypeDef = TypedDict(
-    "CreateCustomMetricResponseTypeDef",
-    {
-        "metricName": str,
-        "metricArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDimensionResponseTypeDef = TypedDict(
-    "CreateDimensionResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TlsConfigTypeDef = TypedDict(
     "TlsConfigTypeDef",
     {
         "securityPolicy": str,
     },
     total=False,
 )
 
-CreateDomainConfigurationResponseTypeDef = TypedDict(
-    "CreateDomainConfigurationResponseTypeDef",
-    {
-        "domainConfigurationName": str,
-        "domainConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDynamicThingGroupResponseTypeDef = TypedDict(
-    "CreateDynamicThingGroupResponseTypeDef",
-    {
-        "thingGroupName": str,
-        "thingGroupArn": str,
-        "thingGroupId": str,
-        "indexName": str,
-        "queryString": str,
-        "queryVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFleetMetricResponseTypeDef = TypedDict(
-    "CreateFleetMetricResponseTypeDef",
-    {
-        "metricName": str,
-        "metricArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PresignedUrlConfigTypeDef = TypedDict(
     "PresignedUrlConfigTypeDef",
     {
         "roleArn": str,
         "expiresInSec": int,
     },
     total=False,
@@ -1815,41 +1889,22 @@
     "TimeoutConfigTypeDef",
     {
         "inProgressTimeoutInMinutes": int,
     },
     total=False,
 )
 
-CreateJobResponseTypeDef = TypedDict(
-    "CreateJobResponseTypeDef",
-    {
-        "jobArn": str,
-        "jobId": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MaintenanceWindowTypeDef = TypedDict(
     "MaintenanceWindowTypeDef",
     {
         "startTime": str,
         "durationInMinutes": int,
     },
 )
 
-CreateJobTemplateResponseTypeDef = TypedDict(
-    "CreateJobTemplateResponseTypeDef",
-    {
-        "jobTemplateArn": str,
-        "jobTemplateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateKeysAndCertificateRequestRequestTypeDef = TypedDict(
     "CreateKeysAndCertificateRequestRequestTypeDef",
     {
         "setAsActive": bool,
     },
     total=False,
 )
@@ -1859,35 +1914,14 @@
     {
         "PublicKey": str,
         "PrivateKey": str,
     },
     total=False,
 )
 
-CreateMitigationActionResponseTypeDef = TypedDict(
-    "CreateMitigationActionResponseTypeDef",
-    {
-        "actionArn": str,
-        "actionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateOTAUpdateResponseTypeDef = TypedDict(
-    "CreateOTAUpdateResponseTypeDef",
-    {
-        "otaUpdateId": str,
-        "awsIotJobId": str,
-        "otaUpdateArn": str,
-        "awsIotJobArn": str,
-        "otaUpdateStatus": OTAUpdateStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePackageRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackageRequestRequestTypeDef",
     {
         "packageName": str,
     },
 )
 _OptionalCreatePackageRequestRequestTypeDef = TypedDict(
@@ -1901,24 +1935,14 @@
 )
 
 class CreatePackageRequestRequestTypeDef(
     _RequiredCreatePackageRequestRequestTypeDef, _OptionalCreatePackageRequestRequestTypeDef
 ):
     pass
 
-CreatePackageResponseTypeDef = TypedDict(
-    "CreatePackageResponseTypeDef",
-    {
-        "packageName": str,
-        "packageArn": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePackageVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackageVersionRequestRequestTypeDef",
     {
         "packageName": str,
         "versionName": str,
     },
 )
@@ -1935,39 +1959,14 @@
 
 class CreatePackageVersionRequestRequestTypeDef(
     _RequiredCreatePackageVersionRequestRequestTypeDef,
     _OptionalCreatePackageVersionRequestRequestTypeDef,
 ):
     pass
 
-CreatePackageVersionResponseTypeDef = TypedDict(
-    "CreatePackageVersionResponseTypeDef",
-    {
-        "packageVersionArn": str,
-        "packageName": str,
-        "versionName": str,
-        "description": str,
-        "attributes": Dict[str, str],
-        "status": PackageVersionStatusType,
-        "errorReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePolicyResponseTypeDef = TypedDict(
-    "CreatePolicyResponseTypeDef",
-    {
-        "policyName": str,
-        "policyArn": str,
-        "policyDocument": str,
-        "policyVersionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePolicyVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePolicyVersionRequestRequestTypeDef",
     {
         "policyName": str,
         "policyDocument": str,
     },
 )
@@ -1981,25 +1980,14 @@
 
 class CreatePolicyVersionRequestRequestTypeDef(
     _RequiredCreatePolicyVersionRequestRequestTypeDef,
     _OptionalCreatePolicyVersionRequestRequestTypeDef,
 ):
     pass
 
-CreatePolicyVersionResponseTypeDef = TypedDict(
-    "CreatePolicyVersionResponseTypeDef",
-    {
-        "policyArn": str,
-        "policyDocument": str,
-        "policyVersionId": str,
-        "isDefaultVersion": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateProvisioningClaimRequestRequestTypeDef = TypedDict(
     "CreateProvisioningClaimRequestRequestTypeDef",
     {
         "templateName": str,
     },
 )
 
@@ -2016,24 +2004,14 @@
     },
     total=False,
 )
 
 class ProvisioningHookTypeDef(_RequiredProvisioningHookTypeDef, _OptionalProvisioningHookTypeDef):
     pass
 
-CreateProvisioningTemplateResponseTypeDef = TypedDict(
-    "CreateProvisioningTemplateResponseTypeDef",
-    {
-        "templateArn": str,
-        "templateName": str,
-        "defaultVersionId": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateProvisioningTemplateVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProvisioningTemplateVersionRequestRequestTypeDef",
     {
         "templateName": str,
         "templateBody": str,
     },
 )
@@ -2047,101 +2025,23 @@
 
 class CreateProvisioningTemplateVersionRequestRequestTypeDef(
     _RequiredCreateProvisioningTemplateVersionRequestRequestTypeDef,
     _OptionalCreateProvisioningTemplateVersionRequestRequestTypeDef,
 ):
     pass
 
-CreateProvisioningTemplateVersionResponseTypeDef = TypedDict(
-    "CreateProvisioningTemplateVersionResponseTypeDef",
-    {
-        "templateArn": str,
-        "templateName": str,
-        "versionId": int,
-        "isDefaultVersion": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateRoleAliasResponseTypeDef = TypedDict(
-    "CreateRoleAliasResponseTypeDef",
-    {
-        "roleAlias": str,
-        "roleAliasArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateScheduledAuditResponseTypeDef = TypedDict(
-    "CreateScheduledAuditResponseTypeDef",
-    {
-        "scheduledAuditArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSecurityProfileResponseTypeDef = TypedDict(
-    "CreateSecurityProfileResponseTypeDef",
-    {
-        "securityProfileName": str,
-        "securityProfileArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateStreamResponseTypeDef = TypedDict(
-    "CreateStreamResponseTypeDef",
-    {
-        "streamId": str,
-        "streamArn": str,
-        "description": str,
-        "streamVersion": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateThingGroupResponseTypeDef = TypedDict(
-    "CreateThingGroupResponseTypeDef",
-    {
-        "thingGroupName": str,
-        "thingGroupArn": str,
-        "thingGroupId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateThingResponseTypeDef = TypedDict(
-    "CreateThingResponseTypeDef",
-    {
-        "thingName": str,
-        "thingArn": str,
-        "thingId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ThingTypePropertiesTypeDef = TypedDict(
     "ThingTypePropertiesTypeDef",
     {
         "thingTypeDescription": str,
         "searchableAttributes": Sequence[str],
     },
     total=False,
 )
 
-CreateThingTypeResponseTypeDef = TypedDict(
-    "CreateThingTypeResponseTypeDef",
-    {
-        "thingTypeName": str,
-        "thingTypeArn": str,
-        "thingTypeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteAccountAuditConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteAccountAuditConfigurationRequestRequestTypeDef",
     {
         "deleteScheduledAudits": bool,
     },
     total=False,
 )
@@ -2622,54 +2522,28 @@
 DescribeCustomMetricRequestRequestTypeDef = TypedDict(
     "DescribeCustomMetricRequestRequestTypeDef",
     {
         "metricName": str,
     },
 )
 
-DescribeCustomMetricResponseTypeDef = TypedDict(
-    "DescribeCustomMetricResponseTypeDef",
-    {
-        "metricName": str,
-        "metricArn": str,
-        "metricType": CustomMetricTypeType,
-        "displayName": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
     "DescribeDetectMitigationActionsTaskRequestRequestTypeDef",
     {
         "taskId": str,
     },
 )
 
 DescribeDimensionRequestRequestTypeDef = TypedDict(
     "DescribeDimensionRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-DescribeDimensionResponseTypeDef = TypedDict(
-    "DescribeDimensionResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "type": Literal["TOPIC_FILTER"],
-        "stringValues": List[str],
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDomainConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeDomainConfigurationRequestRequestTypeDef",
     {
         "domainConfigurationName": str,
     },
 )
 
@@ -2687,46 +2561,28 @@
     "DescribeEndpointRequestRequestTypeDef",
     {
         "endpointType": str,
     },
     total=False,
 )
 
-DescribeEndpointResponseTypeDef = TypedDict(
-    "DescribeEndpointResponseTypeDef",
-    {
-        "endpointAddress": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeFleetMetricRequestRequestTypeDef = TypedDict(
     "DescribeFleetMetricRequestRequestTypeDef",
     {
         "metricName": str,
     },
 )
 
 DescribeIndexRequestRequestTypeDef = TypedDict(
     "DescribeIndexRequestRequestTypeDef",
     {
         "indexName": str,
     },
 )
 
-DescribeIndexResponseTypeDef = TypedDict(
-    "DescribeIndexResponseTypeDef",
-    {
-        "indexName": str,
-        "indexStatus": IndexStatusType,
-        "schema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeJobExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeJobExecutionRequestRequestTypeDef",
     {
         "jobId": str,
         "thingName": str,
     },
 )
@@ -2808,25 +2664,14 @@
     "DescribeProvisioningTemplateVersionRequestRequestTypeDef",
     {
         "templateName": str,
         "versionId": int,
     },
 )
 
-DescribeProvisioningTemplateVersionResponseTypeDef = TypedDict(
-    "DescribeProvisioningTemplateVersionResponseTypeDef",
-    {
-        "versionId": int,
-        "creationDate": datetime,
-        "templateBody": str,
-        "isDefaultVersion": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeRoleAliasRequestRequestTypeDef = TypedDict(
     "DescribeRoleAliasRequestRequestTypeDef",
     {
         "roleAlias": str,
     },
 )
 
@@ -2847,27 +2692,14 @@
 DescribeScheduledAuditRequestRequestTypeDef = TypedDict(
     "DescribeScheduledAuditRequestRequestTypeDef",
     {
         "scheduledAuditName": str,
     },
 )
 
-DescribeScheduledAuditResponseTypeDef = TypedDict(
-    "DescribeScheduledAuditResponseTypeDef",
-    {
-        "frequency": AuditFrequencyType,
-        "dayOfMonth": str,
-        "dayOfWeek": DayOfWeekType,
-        "targetCheckNames": List[str],
-        "scheduledAuditName": str,
-        "scheduledAuditArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeSecurityProfileRequestRequestTypeDef = TypedDict(
     "DescribeSecurityProfileRequestRequestTypeDef",
     {
         "securityProfileName": str,
     },
 )
 
@@ -2888,55 +2720,21 @@
 DescribeThingRegistrationTaskRequestRequestTypeDef = TypedDict(
     "DescribeThingRegistrationTaskRequestRequestTypeDef",
     {
         "taskId": str,
     },
 )
 
-DescribeThingRegistrationTaskResponseTypeDef = TypedDict(
-    "DescribeThingRegistrationTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "templateBody": str,
-        "inputFileBucket": str,
-        "inputFileKey": str,
-        "roleArn": str,
-        "status": StatusType,
-        "message": str,
-        "successCount": int,
-        "failureCount": int,
-        "percentageProgress": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeThingRequestRequestTypeDef = TypedDict(
     "DescribeThingRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 
-DescribeThingResponseTypeDef = TypedDict(
-    "DescribeThingResponseTypeDef",
-    {
-        "defaultClientId": str,
-        "thingName": str,
-        "thingId": str,
-        "thingArn": str,
-        "thingTypeName": str,
-        "attributes": Dict[str, str],
-        "version": int,
-        "billingGroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeThingTypeRequestRequestTypeDef = TypedDict(
     "DescribeThingTypeRequestRequestTypeDef",
     {
         "thingTypeName": str,
     },
 )
 
@@ -2946,14 +2744,23 @@
         "deprecated": bool,
         "deprecationDate": datetime,
         "creationDate": datetime,
     },
     total=False,
 )
 
+ThingTypePropertiesOutputTypeDef = TypedDict(
+    "ThingTypePropertiesOutputTypeDef",
+    {
+        "thingTypeDescription": str,
+        "searchableAttributes": List[str],
+    },
+    total=False,
+)
+
 S3DestinationTypeDef = TypedDict(
     "S3DestinationTypeDef",
     {
         "bucket": str,
         "prefix": str,
     },
     total=False,
@@ -3013,32 +2820,42 @@
         "actionsExecuted": int,
         "actionsSkipped": int,
         "actionsFailed": int,
     },
     total=False,
 )
 
-DetectMitigationActionsTaskTargetTypeDef = TypedDict(
-    "DetectMitigationActionsTaskTargetTypeDef",
+DetectMitigationActionsTaskTargetOutputTypeDef = TypedDict(
+    "DetectMitigationActionsTaskTargetOutputTypeDef",
     {
         "violationIds": List[str],
         "securityProfileName": str,
         "behaviorName": str,
     },
     total=False,
 )
 
-ViolationEventOccurrenceRangeTypeDef = TypedDict(
-    "ViolationEventOccurrenceRangeTypeDef",
+ViolationEventOccurrenceRangeOutputTypeDef = TypedDict(
+    "ViolationEventOccurrenceRangeOutputTypeDef",
     {
         "startTime": datetime,
         "endTime": datetime,
     },
 )
 
+DetectMitigationActionsTaskTargetTypeDef = TypedDict(
+    "DetectMitigationActionsTaskTargetTypeDef",
+    {
+        "violationIds": Sequence[str],
+        "securityProfileName": str,
+        "behaviorName": str,
+    },
+    total=False,
+)
+
 DisableTopicRuleRequestRequestTypeDef = TypedDict(
     "DisableTopicRuleRequestRequestTypeDef",
     {
         "ruleName": str,
     },
 )
 
@@ -3065,21 +2882,14 @@
         "policyName": str,
         "policyArn": str,
         "policyDocument": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnableIoTLoggingParamsTypeDef = TypedDict(
     "EnableIoTLoggingParamsTypeDef",
     {
         "roleArnForLogging": str,
         "logLevel": LogLevelType,
     },
 )
@@ -3142,23 +2952,22 @@
     {
         "metricName": str,
         "metricArn": str,
     },
     total=False,
 )
 
-GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef = (
-    TypedDict(
-        "GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef",
-        {
-            "securityProfileName": str,
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
 )
 
 GetBehaviorModelTrainingSummariesRequestRequestTypeDef = TypedDict(
     "GetBehaviorModelTrainingSummariesRequestRequestTypeDef",
     {
         "securityProfileName": str,
         "maxResults": int,
@@ -3184,22 +2993,14 @@
 )
 
 class GetCardinalityRequestRequestTypeDef(
     _RequiredGetCardinalityRequestRequestTypeDef, _OptionalGetCardinalityRequestRequestTypeDef
 ):
     pass
 
-GetCardinalityResponseTypeDef = TypedDict(
-    "GetCardinalityResponseTypeDef",
-    {
-        "cardinality": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetEffectivePoliciesRequestRequestTypeDef = TypedDict(
     "GetEffectivePoliciesRequestRequestTypeDef",
     {
         "principal": str,
         "cognitoIdentityPoolId": str,
         "thingName": str,
     },
@@ -3209,31 +3010,14 @@
 GetJobDocumentRequestRequestTypeDef = TypedDict(
     "GetJobDocumentRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 
-GetJobDocumentResponseTypeDef = TypedDict(
-    "GetJobDocumentResponseTypeDef",
-    {
-        "document": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetLoggingOptionsResponseTypeDef = TypedDict(
-    "GetLoggingOptionsResponseTypeDef",
-    {
-        "roleArn": str,
-        "logLevel": LogLevelType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetOTAUpdateRequestRequestTypeDef = TypedDict(
     "GetOTAUpdateRequestRequestTypeDef",
     {
         "otaUpdateId": str,
     },
 )
 
@@ -3249,51 +3033,22 @@
 GetPackageRequestRequestTypeDef = TypedDict(
     "GetPackageRequestRequestTypeDef",
     {
         "packageName": str,
     },
 )
 
-GetPackageResponseTypeDef = TypedDict(
-    "GetPackageResponseTypeDef",
-    {
-        "packageName": str,
-        "packageArn": str,
-        "description": str,
-        "defaultVersionName": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPackageVersionRequestRequestTypeDef = TypedDict(
     "GetPackageVersionRequestRequestTypeDef",
     {
         "packageName": str,
         "versionName": str,
     },
 )
 
-GetPackageVersionResponseTypeDef = TypedDict(
-    "GetPackageVersionResponseTypeDef",
-    {
-        "packageVersionArn": str,
-        "packageName": str,
-        "versionName": str,
-        "description": str,
-        "attributes": Dict[str, str],
-        "status": PackageVersionStatusType,
-        "errorReason": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetPercentilesRequestRequestTypeDef = TypedDict(
     "_RequiredGetPercentilesRequestRequestTypeDef",
     {
         "queryString": str,
     },
 )
 _OptionalGetPercentilesRequestRequestTypeDef = TypedDict(
@@ -3324,59 +3079,22 @@
 GetPolicyRequestRequestTypeDef = TypedDict(
     "GetPolicyRequestRequestTypeDef",
     {
         "policyName": str,
     },
 )
 
-GetPolicyResponseTypeDef = TypedDict(
-    "GetPolicyResponseTypeDef",
-    {
-        "policyName": str,
-        "policyArn": str,
-        "policyDocument": str,
-        "defaultVersionId": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "generationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPolicyVersionRequestRequestTypeDef = TypedDict(
     "GetPolicyVersionRequestRequestTypeDef",
     {
         "policyName": str,
         "policyVersionId": str,
     },
 )
 
-GetPolicyVersionResponseTypeDef = TypedDict(
-    "GetPolicyVersionResponseTypeDef",
-    {
-        "policyArn": str,
-        "policyName": str,
-        "policyDocument": str,
-        "policyVersionId": str,
-        "isDefaultVersion": bool,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "generationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetRegistrationCodeResponseTypeDef = TypedDict(
-    "GetRegistrationCodeResponseTypeDef",
-    {
-        "registrationCode": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetStatisticsRequestRequestTypeDef",
     {
         "queryString": str,
     },
 )
 _OptionalGetStatisticsRequestRequestTypeDef = TypedDict(
@@ -3419,24 +3137,14 @@
 GetTopicRuleRequestRequestTypeDef = TypedDict(
     "GetTopicRuleRequestRequestTypeDef",
     {
         "ruleName": str,
     },
 )
 
-GetV2LoggingOptionsResponseTypeDef = TypedDict(
-    "GetV2LoggingOptionsResponseTypeDef",
-    {
-        "roleArn": str,
-        "defaultLogLevel": LogLevelType,
-        "disableAllLogs": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GroupNameAndArnTypeDef = TypedDict(
     "GroupNameAndArnTypeDef",
     {
         "groupName": str,
         "groupArn": str,
     },
     total=False,
@@ -3487,18 +3195,26 @@
     "HttpUrlDestinationSummaryTypeDef",
     {
         "confirmationUrl": str,
     },
     total=False,
 )
 
+IndexingFilterOutputTypeDef = TypedDict(
+    "IndexingFilterOutputTypeDef",
+    {
+        "namedShadowNames": List[str],
+    },
+    total=False,
+)
+
 IndexingFilterTypeDef = TypedDict(
     "IndexingFilterTypeDef",
     {
-        "namedShadowNames": List[str],
+        "namedShadowNames": Sequence[str],
     },
     total=False,
 )
 
 IssuerCertificateIdentifierTypeDef = TypedDict(
     "IssuerCertificateIdentifierTypeDef",
     {
@@ -3585,62 +3301,28 @@
     "ScheduledJobRolloutTypeDef",
     {
         "startTime": str,
     },
     total=False,
 )
 
-ListActiveViolationsRequestListActiveViolationsPaginateTypeDef = TypedDict(
-    "ListActiveViolationsRequestListActiveViolationsPaginateTypeDef",
-    {
-        "thingName": str,
-        "securityProfileName": str,
-        "behaviorCriteriaType": BehaviorCriteriaTypeType,
-        "listSuppressedAlerts": bool,
-        "verificationState": VerificationStateType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListActiveViolationsRequestRequestTypeDef = TypedDict(
     "ListActiveViolationsRequestRequestTypeDef",
     {
         "thingName": str,
         "securityProfileName": str,
         "behaviorCriteriaType": BehaviorCriteriaTypeType,
         "listSuppressedAlerts": bool,
         "verificationState": VerificationStateType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef",
-    {
-        "target": str,
-    },
-)
-_OptionalListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef",
-    {
-        "recursive": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef(
-    _RequiredListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef,
-    _OptionalListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef,
-):
-    pass
-
 _RequiredListAttachedPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListAttachedPoliciesRequestRequestTypeDef",
     {
         "target": str,
     },
 )
 _OptionalListAttachedPoliciesRequestRequestTypeDef = TypedDict(
@@ -3655,36 +3337,14 @@
 
 class ListAttachedPoliciesRequestRequestTypeDef(
     _RequiredListAttachedPoliciesRequestRequestTypeDef,
     _OptionalListAttachedPoliciesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef",
-    {
-        "taskId": str,
-        "findingId": str,
-    },
-)
-_OptionalListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef",
-    {
-        "actionStatus": AuditMitigationActionsExecutionStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef(
-    _RequiredListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef,
-    _OptionalListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListAuditMitigationActionsExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredListAuditMitigationActionsExecutionsRequestRequestTypeDef",
     {
         "taskId": str,
         "findingId": str,
     },
 )
@@ -3700,191 +3360,46 @@
 
 class ListAuditMitigationActionsExecutionsRequestRequestTypeDef(
     _RequiredListAuditMitigationActionsExecutionsRequestRequestTypeDef,
     _OptionalListAuditMitigationActionsExecutionsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef = TypedDict(
-    "_RequiredListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef = TypedDict(
-    "_OptionalListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef",
-    {
-        "auditTaskId": str,
-        "findingId": str,
-        "taskStatus": AuditMitigationActionsTaskStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef(
-    _RequiredListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef,
-    _OptionalListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef,
-):
-    pass
-
-_RequiredListAuditMitigationActionsTasksRequestRequestTypeDef = TypedDict(
-    "_RequiredListAuditMitigationActionsTasksRequestRequestTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListAuditMitigationActionsTasksRequestRequestTypeDef = TypedDict(
-    "_OptionalListAuditMitigationActionsTasksRequestRequestTypeDef",
-    {
-        "auditTaskId": str,
-        "findingId": str,
-        "taskStatus": AuditMitigationActionsTaskStatusType,
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-class ListAuditMitigationActionsTasksRequestRequestTypeDef(
-    _RequiredListAuditMitigationActionsTasksRequestRequestTypeDef,
-    _OptionalListAuditMitigationActionsTasksRequestRequestTypeDef,
-):
-    pass
-
-_RequiredListAuditTasksRequestListAuditTasksPaginateTypeDef = TypedDict(
-    "_RequiredListAuditTasksRequestListAuditTasksPaginateTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListAuditTasksRequestListAuditTasksPaginateTypeDef = TypedDict(
-    "_OptionalListAuditTasksRequestListAuditTasksPaginateTypeDef",
-    {
-        "taskType": AuditTaskTypeType,
-        "taskStatus": AuditTaskStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAuditTasksRequestListAuditTasksPaginateTypeDef(
-    _RequiredListAuditTasksRequestListAuditTasksPaginateTypeDef,
-    _OptionalListAuditTasksRequestListAuditTasksPaginateTypeDef,
-):
-    pass
-
-_RequiredListAuditTasksRequestRequestTypeDef = TypedDict(
-    "_RequiredListAuditTasksRequestRequestTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListAuditTasksRequestRequestTypeDef = TypedDict(
-    "_OptionalListAuditTasksRequestRequestTypeDef",
-    {
-        "taskType": AuditTaskTypeType,
-        "taskStatus": AuditTaskStatusType,
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-class ListAuditTasksRequestRequestTypeDef(
-    _RequiredListAuditTasksRequestRequestTypeDef, _OptionalListAuditTasksRequestRequestTypeDef
-):
-    pass
-
-ListAuthorizersRequestListAuthorizersPaginateTypeDef = TypedDict(
-    "ListAuthorizersRequestListAuthorizersPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "status": AuthorizerStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAuthorizersRequestRequestTypeDef = TypedDict(
     "ListAuthorizersRequestRequestTypeDef",
     {
         "pageSize": int,
         "marker": str,
         "ascendingOrder": bool,
         "status": AuthorizerStatusType,
     },
     total=False,
 )
 
-ListBillingGroupsRequestListBillingGroupsPaginateTypeDef = TypedDict(
-    "ListBillingGroupsRequestListBillingGroupsPaginateTypeDef",
-    {
-        "namePrefixFilter": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListBillingGroupsRequestRequestTypeDef = TypedDict(
     "ListBillingGroupsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "namePrefixFilter": str,
     },
     total=False,
 )
 
-ListCACertificatesRequestListCACertificatesPaginateTypeDef = TypedDict(
-    "ListCACertificatesRequestListCACertificatesPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "templateName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCACertificatesRequestRequestTypeDef = TypedDict(
     "ListCACertificatesRequestRequestTypeDef",
     {
         "pageSize": int,
         "marker": str,
         "ascendingOrder": bool,
         "templateName": str,
     },
     total=False,
 )
 
-_RequiredListCertificatesByCARequestListCertificatesByCAPaginateTypeDef = TypedDict(
-    "_RequiredListCertificatesByCARequestListCertificatesByCAPaginateTypeDef",
-    {
-        "caCertificateId": str,
-    },
-)
-_OptionalListCertificatesByCARequestListCertificatesByCAPaginateTypeDef = TypedDict(
-    "_OptionalListCertificatesByCARequestListCertificatesByCAPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListCertificatesByCARequestListCertificatesByCAPaginateTypeDef(
-    _RequiredListCertificatesByCARequestListCertificatesByCAPaginateTypeDef,
-    _OptionalListCertificatesByCARequestListCertificatesByCAPaginateTypeDef,
-):
-    pass
-
 _RequiredListCertificatesByCARequestRequestTypeDef = TypedDict(
     "_RequiredListCertificatesByCARequestRequestTypeDef",
     {
         "caCertificateId": str,
     },
 )
 _OptionalListCertificatesByCARequestRequestTypeDef = TypedDict(
@@ -3899,238 +3414,70 @@
 
 class ListCertificatesByCARequestRequestTypeDef(
     _RequiredListCertificatesByCARequestRequestTypeDef,
     _OptionalListCertificatesByCARequestRequestTypeDef,
 ):
     pass
 
-ListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
-    "ListCertificatesRequestListCertificatesPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCertificatesRequestRequestTypeDef = TypedDict(
     "ListCertificatesRequestRequestTypeDef",
     {
         "pageSize": int,
         "marker": str,
         "ascendingOrder": bool,
     },
     total=False,
 )
 
-ListCustomMetricsRequestListCustomMetricsPaginateTypeDef = TypedDict(
-    "ListCustomMetricsRequestListCustomMetricsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCustomMetricsRequestRequestTypeDef = TypedDict(
     "ListCustomMetricsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListCustomMetricsResponseTypeDef = TypedDict(
-    "ListCustomMetricsResponseTypeDef",
-    {
-        "metricNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef = TypedDict(
-    "ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef",
-    {
-        "taskId": str,
-        "violationId": str,
-        "thingName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListDetectMitigationActionsExecutionsRequestRequestTypeDef = TypedDict(
-    "ListDetectMitigationActionsExecutionsRequestRequestTypeDef",
-    {
-        "taskId": str,
-        "violationId": str,
-        "thingName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-_RequiredListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef = TypedDict(
-    "_RequiredListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef = TypedDict(
-    "_OptionalListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef(
-    _RequiredListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef,
-    _OptionalListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef,
-):
-    pass
-
-_RequiredListDetectMitigationActionsTasksRequestRequestTypeDef = TypedDict(
-    "_RequiredListDetectMitigationActionsTasksRequestRequestTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListDetectMitigationActionsTasksRequestRequestTypeDef = TypedDict(
-    "_OptionalListDetectMitigationActionsTasksRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-class ListDetectMitigationActionsTasksRequestRequestTypeDef(
-    _RequiredListDetectMitigationActionsTasksRequestRequestTypeDef,
-    _OptionalListDetectMitigationActionsTasksRequestRequestTypeDef,
-):
-    pass
-
-ListDimensionsRequestListDimensionsPaginateTypeDef = TypedDict(
-    "ListDimensionsRequestListDimensionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDimensionsRequestRequestTypeDef = TypedDict(
     "ListDimensionsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListDimensionsResponseTypeDef = TypedDict(
-    "ListDimensionsResponseTypeDef",
-    {
-        "dimensionNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef = TypedDict(
-    "ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef",
-    {
-        "serviceType": ServiceTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDomainConfigurationsRequestRequestTypeDef = TypedDict(
     "ListDomainConfigurationsRequestRequestTypeDef",
     {
         "marker": str,
         "pageSize": int,
         "serviceType": ServiceTypeType,
     },
     total=False,
 )
 
-ListFleetMetricsRequestListFleetMetricsPaginateTypeDef = TypedDict(
-    "ListFleetMetricsRequestListFleetMetricsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFleetMetricsRequestRequestTypeDef = TypedDict(
     "ListFleetMetricsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListIndicesRequestListIndicesPaginateTypeDef = TypedDict(
-    "ListIndicesRequestListIndicesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListIndicesRequestRequestTypeDef = TypedDict(
     "ListIndicesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListIndicesResponseTypeDef = TypedDict(
-    "ListIndicesResponseTypeDef",
-    {
-        "indexNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef = TypedDict(
-    "_RequiredListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef",
-    {
-        "jobId": str,
-    },
-)
-_OptionalListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef = TypedDict(
-    "_OptionalListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef",
-    {
-        "status": JobExecutionStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef(
-    _RequiredListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef,
-    _OptionalListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef,
-):
-    pass
-
 _RequiredListJobExecutionsForJobRequestRequestTypeDef = TypedDict(
     "_RequiredListJobExecutionsForJobRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 _OptionalListJobExecutionsForJobRequestRequestTypeDef = TypedDict(
@@ -4145,37 +3492,14 @@
 
 class ListJobExecutionsForJobRequestRequestTypeDef(
     _RequiredListJobExecutionsForJobRequestRequestTypeDef,
     _OptionalListJobExecutionsForJobRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef = TypedDict(
-    "_RequiredListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef",
-    {
-        "thingName": str,
-    },
-)
-_OptionalListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef = TypedDict(
-    "_OptionalListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef",
-    {
-        "status": JobExecutionStatusType,
-        "namespaceId": str,
-        "jobId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef(
-    _RequiredListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef,
-    _OptionalListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef,
-):
-    pass
-
 _RequiredListJobExecutionsForThingRequestRequestTypeDef = TypedDict(
     "_RequiredListJobExecutionsForThingRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 _OptionalListJobExecutionsForThingRequestRequestTypeDef = TypedDict(
@@ -4192,67 +3516,37 @@
 
 class ListJobExecutionsForThingRequestRequestTypeDef(
     _RequiredListJobExecutionsForThingRequestRequestTypeDef,
     _OptionalListJobExecutionsForThingRequestRequestTypeDef,
 ):
     pass
 
-ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListJobTemplatesRequestRequestTypeDef = TypedDict(
     "ListJobTemplatesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "ListJobsRequestListJobsPaginateTypeDef",
-    {
-        "status": JobStatusType,
-        "targetSelection": TargetSelectionType,
-        "thingGroupName": str,
-        "thingGroupId": str,
-        "namespaceId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "status": JobStatusType,
         "targetSelection": TargetSelectionType,
         "maxResults": int,
         "nextToken": str,
         "thingGroupName": str,
         "thingGroupId": str,
         "namespaceId": str,
     },
     total=False,
 )
 
-ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef = TypedDict(
-    "ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef",
-    {
-        "templateName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListManagedJobTemplatesRequestRequestTypeDef = TypedDict(
     "ListManagedJobTemplatesRequestRequestTypeDef",
     {
         "templateName": str,
         "maxResults": int,
         "nextToken": str,
     },
@@ -4267,73 +3561,14 @@
         "description": str,
         "environments": List[str],
         "templateVersion": str,
     },
     total=False,
 )
 
-_RequiredListMetricValuesRequestListMetricValuesPaginateTypeDef = TypedDict(
-    "_RequiredListMetricValuesRequestListMetricValuesPaginateTypeDef",
-    {
-        "thingName": str,
-        "metricName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListMetricValuesRequestListMetricValuesPaginateTypeDef = TypedDict(
-    "_OptionalListMetricValuesRequestListMetricValuesPaginateTypeDef",
-    {
-        "dimensionName": str,
-        "dimensionValueOperator": DimensionValueOperatorType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListMetricValuesRequestListMetricValuesPaginateTypeDef(
-    _RequiredListMetricValuesRequestListMetricValuesPaginateTypeDef,
-    _OptionalListMetricValuesRequestListMetricValuesPaginateTypeDef,
-):
-    pass
-
-_RequiredListMetricValuesRequestRequestTypeDef = TypedDict(
-    "_RequiredListMetricValuesRequestRequestTypeDef",
-    {
-        "thingName": str,
-        "metricName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListMetricValuesRequestRequestTypeDef = TypedDict(
-    "_OptionalListMetricValuesRequestRequestTypeDef",
-    {
-        "dimensionName": str,
-        "dimensionValueOperator": DimensionValueOperatorType,
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-class ListMetricValuesRequestRequestTypeDef(
-    _RequiredListMetricValuesRequestRequestTypeDef, _OptionalListMetricValuesRequestRequestTypeDef
-):
-    pass
-
-ListMitigationActionsRequestListMitigationActionsPaginateTypeDef = TypedDict(
-    "ListMitigationActionsRequestListMitigationActionsPaginateTypeDef",
-    {
-        "actionType": MitigationActionTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMitigationActionsRequestRequestTypeDef = TypedDict(
     "ListMitigationActionsRequestRequestTypeDef",
     {
         "actionType": MitigationActionTypeType,
         "maxResults": int,
         "nextToken": str,
     },
@@ -4346,23 +3581,14 @@
         "actionName": str,
         "actionArn": str,
         "creationDate": datetime,
     },
     total=False,
 )
 
-ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef = TypedDict(
-    "ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef",
-    {
-        "otaUpdateStatus": OTAUpdateStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOTAUpdatesRequestRequestTypeDef = TypedDict(
     "ListOTAUpdatesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "otaUpdateStatus": OTAUpdateStatusType,
     },
@@ -4375,23 +3601,14 @@
         "otaUpdateId": str,
         "otaUpdateArn": str,
         "creationDate": datetime,
     },
     total=False,
 )
 
-ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef = TypedDict(
-    "ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOutgoingCertificatesRequestRequestTypeDef = TypedDict(
     "ListOutgoingCertificatesRequestRequestTypeDef",
     {
         "pageSize": int,
         "marker": str,
         "ascendingOrder": bool,
     },
@@ -4407,35 +3624,14 @@
         "transferDate": datetime,
         "transferMessage": str,
         "creationDate": datetime,
     },
     total=False,
 )
 
-_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
-    {
-        "packageName": str,
-    },
-)
-_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
-    {
-        "status": PackageVersionStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPackageVersionsRequestListPackageVersionsPaginateTypeDef(
-    _RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
-    _OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListPackageVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListPackageVersionsRequestRequestTypeDef",
     {
         "packageName": str,
     },
 )
 _OptionalListPackageVersionsRequestRequestTypeDef = TypedDict(
@@ -4462,22 +3658,14 @@
         "status": PackageVersionStatusType,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
     },
     total=False,
 )
 
-ListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
-    "ListPackagesRequestListPackagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPackagesRequestRequestTypeDef = TypedDict(
     "ListPackagesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -4490,54 +3678,24 @@
         "defaultVersionName": str,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
     },
     total=False,
 )
 
-ListPoliciesRequestListPoliciesPaginateTypeDef = TypedDict(
-    "ListPoliciesRequestListPoliciesPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPoliciesRequestRequestTypeDef = TypedDict(
     "ListPoliciesRequestRequestTypeDef",
     {
         "marker": str,
         "pageSize": int,
         "ascendingOrder": bool,
     },
     total=False,
 )
 
-_RequiredListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef = TypedDict(
-    "_RequiredListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef",
-    {
-        "policyName": str,
-    },
-)
-_OptionalListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef = TypedDict(
-    "_OptionalListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef(
-    _RequiredListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef,
-    _OptionalListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef,
-):
-    pass
-
 _RequiredListPolicyPrincipalsRequestRequestTypeDef = TypedDict(
     "_RequiredListPolicyPrincipalsRequestRequestTypeDef",
     {
         "policyName": str,
     },
 )
 _OptionalListPolicyPrincipalsRequestRequestTypeDef = TypedDict(
@@ -4552,23 +3710,14 @@
 
 class ListPolicyPrincipalsRequestRequestTypeDef(
     _RequiredListPolicyPrincipalsRequestRequestTypeDef,
     _OptionalListPolicyPrincipalsRequestRequestTypeDef,
 ):
     pass
 
-ListPolicyPrincipalsResponseTypeDef = TypedDict(
-    "ListPolicyPrincipalsResponseTypeDef",
-    {
-        "principals": List[str],
-        "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListPolicyVersionsRequestRequestTypeDef = TypedDict(
     "ListPolicyVersionsRequestRequestTypeDef",
     {
         "policyName": str,
     },
 )
 
@@ -4578,35 +3727,14 @@
         "versionId": str,
         "isDefaultVersion": bool,
         "createDate": datetime,
     },
     total=False,
 )
 
-_RequiredListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef",
-    {
-        "principal": str,
-    },
-)
-_OptionalListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef(
-    _RequiredListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef,
-    _OptionalListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef,
-):
-    pass
-
 _RequiredListPrincipalPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListPrincipalPoliciesRequestRequestTypeDef",
     {
         "principal": str,
     },
 )
 _OptionalListPrincipalPoliciesRequestRequestTypeDef = TypedDict(
@@ -4621,34 +3749,14 @@
 
 class ListPrincipalPoliciesRequestRequestTypeDef(
     _RequiredListPrincipalPoliciesRequestRequestTypeDef,
     _OptionalListPrincipalPoliciesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef = TypedDict(
-    "_RequiredListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef",
-    {
-        "principal": str,
-    },
-)
-_OptionalListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef = TypedDict(
-    "_OptionalListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef(
-    _RequiredListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef,
-    _OptionalListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef,
-):
-    pass
-
 _RequiredListPrincipalThingsRequestRequestTypeDef = TypedDict(
     "_RequiredListPrincipalThingsRequestRequestTypeDef",
     {
         "principal": str,
     },
 )
 _OptionalListPrincipalThingsRequestRequestTypeDef = TypedDict(
@@ -4662,43 +3770,14 @@
 
 class ListPrincipalThingsRequestRequestTypeDef(
     _RequiredListPrincipalThingsRequestRequestTypeDef,
     _OptionalListPrincipalThingsRequestRequestTypeDef,
 ):
     pass
 
-ListPrincipalThingsResponseTypeDef = TypedDict(
-    "ListPrincipalThingsResponseTypeDef",
-    {
-        "things": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef",
-    {
-        "templateName": str,
-    },
-)
-_OptionalListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef(
-    _RequiredListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef,
-    _OptionalListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListProvisioningTemplateVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListProvisioningTemplateVersionsRequestRequestTypeDef",
     {
         "templateName": str,
     },
 )
 _OptionalListProvisioningTemplateVersionsRequestRequestTypeDef = TypedDict(
@@ -4722,22 +3801,14 @@
         "versionId": int,
         "creationDate": datetime,
         "isDefaultVersion": bool,
     },
     total=False,
 )
 
-ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef = TypedDict(
-    "ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProvisioningTemplatesRequestRequestTypeDef = TypedDict(
     "ListProvisioningTemplatesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -4753,34 +3824,14 @@
         "lastModifiedDate": datetime,
         "enabled": bool,
         "type": TemplateTypeType,
     },
     total=False,
 )
 
-_RequiredListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef = TypedDict(
-    "_RequiredListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef",
-    {
-        "findingId": str,
-    },
-)
-_OptionalListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef = TypedDict(
-    "_OptionalListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef(
-    _RequiredListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef,
-    _OptionalListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef,
-):
-    pass
-
 _RequiredListRelatedResourcesForAuditFindingRequestRequestTypeDef = TypedDict(
     "_RequiredListRelatedResourcesForAuditFindingRequestRequestTypeDef",
     {
         "findingId": str,
     },
 )
 _OptionalListRelatedResourcesForAuditFindingRequestRequestTypeDef = TypedDict(
@@ -4794,50 +3845,24 @@
 
 class ListRelatedResourcesForAuditFindingRequestRequestTypeDef(
     _RequiredListRelatedResourcesForAuditFindingRequestRequestTypeDef,
     _OptionalListRelatedResourcesForAuditFindingRequestRequestTypeDef,
 ):
     pass
 
-ListRoleAliasesRequestListRoleAliasesPaginateTypeDef = TypedDict(
-    "ListRoleAliasesRequestListRoleAliasesPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRoleAliasesRequestRequestTypeDef = TypedDict(
     "ListRoleAliasesRequestRequestTypeDef",
     {
         "pageSize": int,
         "marker": str,
         "ascendingOrder": bool,
     },
     total=False,
 )
 
-ListRoleAliasesResponseTypeDef = TypedDict(
-    "ListRoleAliasesResponseTypeDef",
-    {
-        "roleAliases": List[str],
-        "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef = TypedDict(
-    "ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListScheduledAuditsRequestRequestTypeDef = TypedDict(
     "ListScheduledAuditsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -4851,39 +3876,14 @@
         "frequency": AuditFrequencyType,
         "dayOfMonth": str,
         "dayOfWeek": DayOfWeekType,
     },
     total=False,
 )
 
-_RequiredListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef",
-        {
-            "securityProfileTargetArn": str,
-        },
-    )
-)
-_OptionalListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef",
-        {
-            "recursive": bool,
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-class ListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef(
-    _RequiredListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef,
-    _OptionalListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef,
-):
-    pass
-
 _RequiredListSecurityProfilesForTargetRequestRequestTypeDef = TypedDict(
     "_RequiredListSecurityProfilesForTargetRequestRequestTypeDef",
     {
         "securityProfileTargetArn": str,
     },
 )
 _OptionalListSecurityProfilesForTargetRequestRequestTypeDef = TypedDict(
@@ -4898,24 +3898,14 @@
 
 class ListSecurityProfilesForTargetRequestRequestTypeDef(
     _RequiredListSecurityProfilesForTargetRequestRequestTypeDef,
     _OptionalListSecurityProfilesForTargetRequestRequestTypeDef,
 ):
     pass
 
-ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef = TypedDict(
-    "ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef",
-    {
-        "dimensionName": str,
-        "metricName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSecurityProfilesRequestRequestTypeDef = TypedDict(
     "ListSecurityProfilesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "dimensionName": str,
         "metricName": str,
@@ -4927,23 +3917,14 @@
     "SecurityProfileIdentifierTypeDef",
     {
         "name": str,
         "arn": str,
     },
 )
 
-ListStreamsRequestListStreamsPaginateTypeDef = TypedDict(
-    "ListStreamsRequestListStreamsPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStreamsRequestRequestTypeDef = TypedDict(
     "ListStreamsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "ascendingOrder": bool,
     },
@@ -4957,34 +3938,14 @@
         "streamArn": str,
         "streamVersion": int,
         "description": str,
     },
     total=False,
 )
 
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -4997,34 +3958,14 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef = TypedDict(
-    "_RequiredListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef",
-    {
-        "policyName": str,
-    },
-)
-_OptionalListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef = TypedDict(
-    "_OptionalListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef(
-    _RequiredListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
-    _OptionalListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
-):
-    pass
-
 _RequiredListTargetsForPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredListTargetsForPolicyRequestRequestTypeDef",
     {
         "policyName": str,
     },
 )
 _OptionalListTargetsForPolicyRequestRequestTypeDef = TypedDict(
@@ -5038,47 +3979,14 @@
 
 class ListTargetsForPolicyRequestRequestTypeDef(
     _RequiredListTargetsForPolicyRequestRequestTypeDef,
     _OptionalListTargetsForPolicyRequestRequestTypeDef,
 ):
     pass
 
-ListTargetsForPolicyResponseTypeDef = TypedDict(
-    "ListTargetsForPolicyResponseTypeDef",
-    {
-        "targets": List[str],
-        "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef = (
-    TypedDict(
-        "_RequiredListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef",
-        {
-            "securityProfileName": str,
-        },
-    )
-)
-_OptionalListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef = (
-    TypedDict(
-        "_OptionalListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef",
-        {
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-class ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef(
-    _RequiredListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef,
-    _OptionalListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef,
-):
-    pass
-
 _RequiredListTargetsForSecurityProfileRequestRequestTypeDef = TypedDict(
     "_RequiredListTargetsForSecurityProfileRequestRequestTypeDef",
     {
         "securityProfileName": str,
     },
 )
 _OptionalListTargetsForSecurityProfileRequestRequestTypeDef = TypedDict(
@@ -5099,34 +4007,14 @@
 SecurityProfileTargetTypeDef = TypedDict(
     "SecurityProfileTargetTypeDef",
     {
         "arn": str,
     },
 )
 
-_RequiredListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef = TypedDict(
-    "_RequiredListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef",
-    {
-        "thingName": str,
-    },
-)
-_OptionalListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef = TypedDict(
-    "_OptionalListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef(
-    _RequiredListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef,
-    _OptionalListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef,
-):
-    pass
-
 _RequiredListThingGroupsForThingRequestRequestTypeDef = TypedDict(
     "_RequiredListThingGroupsForThingRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 _OptionalListThingGroupsForThingRequestRequestTypeDef = TypedDict(
@@ -5140,57 +4028,26 @@
 
 class ListThingGroupsForThingRequestRequestTypeDef(
     _RequiredListThingGroupsForThingRequestRequestTypeDef,
     _OptionalListThingGroupsForThingRequestRequestTypeDef,
 ):
     pass
 
-ListThingGroupsRequestListThingGroupsPaginateTypeDef = TypedDict(
-    "ListThingGroupsRequestListThingGroupsPaginateTypeDef",
-    {
-        "parentGroup": str,
-        "namePrefixFilter": str,
-        "recursive": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListThingGroupsRequestRequestTypeDef = TypedDict(
     "ListThingGroupsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "parentGroup": str,
         "namePrefixFilter": str,
         "recursive": bool,
     },
     total=False,
 )
 
-_RequiredListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef = TypedDict(
-    "_RequiredListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef",
-    {
-        "thingName": str,
-    },
-)
-_OptionalListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef = TypedDict(
-    "_OptionalListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef(
-    _RequiredListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef,
-    _OptionalListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef,
-):
-    pass
-
 _RequiredListThingPrincipalsRequestRequestTypeDef = TypedDict(
     "_RequiredListThingPrincipalsRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 _OptionalListThingPrincipalsRequestRequestTypeDef = TypedDict(
@@ -5204,44 +4061,14 @@
 
 class ListThingPrincipalsRequestRequestTypeDef(
     _RequiredListThingPrincipalsRequestRequestTypeDef,
     _OptionalListThingPrincipalsRequestRequestTypeDef,
 ):
     pass
 
-ListThingPrincipalsResponseTypeDef = TypedDict(
-    "ListThingPrincipalsResponseTypeDef",
-    {
-        "principals": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef = TypedDict(
-    "_RequiredListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef",
-    {
-        "taskId": str,
-        "reportType": ReportTypeType,
-    },
-)
-_OptionalListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef = TypedDict(
-    "_OptionalListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef(
-    _RequiredListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef,
-    _OptionalListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef,
-):
-    pass
-
 _RequiredListThingRegistrationTaskReportsRequestRequestTypeDef = TypedDict(
     "_RequiredListThingRegistrationTaskReportsRequestRequestTypeDef",
     {
         "taskId": str,
         "reportType": ReportTypeType,
     },
 )
@@ -5256,91 +4083,34 @@
 
 class ListThingRegistrationTaskReportsRequestRequestTypeDef(
     _RequiredListThingRegistrationTaskReportsRequestRequestTypeDef,
     _OptionalListThingRegistrationTaskReportsRequestRequestTypeDef,
 ):
     pass
 
-ListThingRegistrationTaskReportsResponseTypeDef = TypedDict(
-    "ListThingRegistrationTaskReportsResponseTypeDef",
-    {
-        "resourceLinks": List[str],
-        "reportType": ReportTypeType,
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef = TypedDict(
-    "ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef",
-    {
-        "status": StatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListThingRegistrationTasksRequestRequestTypeDef = TypedDict(
     "ListThingRegistrationTasksRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "status": StatusType,
     },
     total=False,
 )
 
-ListThingRegistrationTasksResponseTypeDef = TypedDict(
-    "ListThingRegistrationTasksResponseTypeDef",
-    {
-        "taskIds": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListThingTypesRequestListThingTypesPaginateTypeDef = TypedDict(
-    "ListThingTypesRequestListThingTypesPaginateTypeDef",
-    {
-        "thingTypeName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListThingTypesRequestRequestTypeDef = TypedDict(
     "ListThingTypesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "thingTypeName": str,
     },
     total=False,
 )
 
-_RequiredListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef = TypedDict(
-    "_RequiredListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef",
-    {
-        "billingGroupName": str,
-    },
-)
-_OptionalListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef = TypedDict(
-    "_OptionalListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef(
-    _RequiredListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef,
-    _OptionalListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef,
-):
-    pass
-
 _RequiredListThingsInBillingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredListThingsInBillingGroupRequestRequestTypeDef",
     {
         "billingGroupName": str,
     },
 )
 _OptionalListThingsInBillingGroupRequestRequestTypeDef = TypedDict(
@@ -5354,44 +4124,14 @@
 
 class ListThingsInBillingGroupRequestRequestTypeDef(
     _RequiredListThingsInBillingGroupRequestRequestTypeDef,
     _OptionalListThingsInBillingGroupRequestRequestTypeDef,
 ):
     pass
 
-ListThingsInBillingGroupResponseTypeDef = TypedDict(
-    "ListThingsInBillingGroupResponseTypeDef",
-    {
-        "things": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef = TypedDict(
-    "_RequiredListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef",
-    {
-        "thingGroupName": str,
-    },
-)
-_OptionalListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef = TypedDict(
-    "_OptionalListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef",
-    {
-        "recursive": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef(
-    _RequiredListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef,
-    _OptionalListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef,
-):
-    pass
-
 _RequiredListThingsInThingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredListThingsInThingGroupRequestRequestTypeDef",
     {
         "thingGroupName": str,
     },
 )
 _OptionalListThingsInThingGroupRequestRequestTypeDef = TypedDict(
@@ -5406,35 +4146,14 @@
 
 class ListThingsInThingGroupRequestRequestTypeDef(
     _RequiredListThingsInThingGroupRequestRequestTypeDef,
     _OptionalListThingsInThingGroupRequestRequestTypeDef,
 ):
     pass
 
-ListThingsInThingGroupResponseTypeDef = TypedDict(
-    "ListThingsInThingGroupResponseTypeDef",
-    {
-        "things": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListThingsRequestListThingsPaginateTypeDef = TypedDict(
-    "ListThingsRequestListThingsPaginateTypeDef",
-    {
-        "attributeName": str,
-        "attributeValue": str,
-        "thingTypeName": str,
-        "usePrefixAttributeValue": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListThingsRequestRequestTypeDef = TypedDict(
     "ListThingsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "attributeName": str,
         "attributeValue": str,
@@ -5452,41 +4171,23 @@
         "thingArn": str,
         "attributes": Dict[str, str],
         "version": int,
     },
     total=False,
 )
 
-ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef = TypedDict(
-    "ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTopicRuleDestinationsRequestRequestTypeDef = TypedDict(
     "ListTopicRuleDestinationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListTopicRulesRequestListTopicRulesPaginateTypeDef = TypedDict(
-    "ListTopicRulesRequestListTopicRulesPaginateTypeDef",
-    {
-        "topic": str,
-        "ruleDisabled": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTopicRulesRequestRequestTypeDef = TypedDict(
     "ListTopicRulesRequestRequestTypeDef",
     {
         "topic": str,
         "maxResults": int,
         "nextToken": str,
         "ruleDisabled": bool,
@@ -5502,86 +4203,24 @@
         "topicPattern": str,
         "createdAt": datetime,
         "ruleDisabled": bool,
     },
     total=False,
 )
 
-ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef = TypedDict(
-    "ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef",
-    {
-        "targetType": LogTargetTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListV2LoggingLevelsRequestRequestTypeDef = TypedDict(
     "ListV2LoggingLevelsRequestRequestTypeDef",
     {
         "targetType": LogTargetTypeType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListViolationEventsRequestListViolationEventsPaginateTypeDef = TypedDict(
-    "_RequiredListViolationEventsRequestListViolationEventsPaginateTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListViolationEventsRequestListViolationEventsPaginateTypeDef = TypedDict(
-    "_OptionalListViolationEventsRequestListViolationEventsPaginateTypeDef",
-    {
-        "thingName": str,
-        "securityProfileName": str,
-        "behaviorCriteriaType": BehaviorCriteriaTypeType,
-        "listSuppressedAlerts": bool,
-        "verificationState": VerificationStateType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListViolationEventsRequestListViolationEventsPaginateTypeDef(
-    _RequiredListViolationEventsRequestListViolationEventsPaginateTypeDef,
-    _OptionalListViolationEventsRequestListViolationEventsPaginateTypeDef,
-):
-    pass
-
-_RequiredListViolationEventsRequestRequestTypeDef = TypedDict(
-    "_RequiredListViolationEventsRequestRequestTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListViolationEventsRequestRequestTypeDef = TypedDict(
-    "_OptionalListViolationEventsRequestRequestTypeDef",
-    {
-        "thingName": str,
-        "securityProfileName": str,
-        "behaviorCriteriaType": BehaviorCriteriaTypeType,
-        "listSuppressedAlerts": bool,
-        "verificationState": VerificationStateType,
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-class ListViolationEventsRequestRequestTypeDef(
-    _RequiredListViolationEventsRequestRequestTypeDef,
-    _OptionalListViolationEventsRequestRequestTypeDef,
-):
-    pass
-
 _RequiredLocationTimestampTypeDef = TypedDict(
     "_RequiredLocationTimestampTypeDef",
     {
         "value": str,
     },
 )
 _OptionalLocationTimestampTypeDef = TypedDict(
@@ -5657,42 +4296,22 @@
 UpdateDeviceCertificateParamsTypeDef = TypedDict(
     "UpdateDeviceCertificateParamsTypeDef",
     {
         "action": Literal["DEACTIVATE"],
     },
 )
 
-MqttContextTypeDef = TypedDict(
-    "MqttContextTypeDef",
-    {
-        "username": str,
-        "password": Union[str, bytes, IO[Any], StreamingBody],
-        "clientId": str,
-    },
-    total=False,
-)
-
 UserPropertyTypeDef = TypedDict(
     "UserPropertyTypeDef",
     {
         "key": str,
         "value": str,
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
 PolicyVersionIdentifierTypeDef = TypedDict(
     "PolicyVersionIdentifierTypeDef",
     {
         "policyName": str,
         "policyVersionId": str,
     },
     total=False,
@@ -5715,23 +4334,14 @@
 
 class PutVerificationStateOnViolationRequestRequestTypeDef(
     _RequiredPutVerificationStateOnViolationRequestRequestTypeDef,
     _OptionalPutVerificationStateOnViolationRequestRequestTypeDef,
 ):
     pass
 
-RegisterCACertificateResponseTypeDef = TypedDict(
-    "RegisterCACertificateResponseTypeDef",
-    {
-        "certificateArn": str,
-        "certificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRegisterCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterCertificateRequestRequestTypeDef",
     {
         "certificatePem": str,
     },
 )
 _OptionalRegisterCertificateRequestRequestTypeDef = TypedDict(
@@ -5746,23 +4356,14 @@
 
 class RegisterCertificateRequestRequestTypeDef(
     _RequiredRegisterCertificateRequestRequestTypeDef,
     _OptionalRegisterCertificateRequestRequestTypeDef,
 ):
     pass
 
-RegisterCertificateResponseTypeDef = TypedDict(
-    "RegisterCertificateResponseTypeDef",
-    {
-        "certificateArn": str,
-        "certificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRegisterCertificateWithoutCARequestRequestTypeDef = TypedDict(
     "_RequiredRegisterCertificateWithoutCARequestRequestTypeDef",
     {
         "certificatePem": str,
     },
 )
 _OptionalRegisterCertificateWithoutCARequestRequestTypeDef = TypedDict(
@@ -5775,23 +4376,14 @@
 
 class RegisterCertificateWithoutCARequestRequestTypeDef(
     _RequiredRegisterCertificateWithoutCARequestRequestTypeDef,
     _OptionalRegisterCertificateWithoutCARequestRequestTypeDef,
 ):
     pass
 
-RegisterCertificateWithoutCAResponseTypeDef = TypedDict(
-    "RegisterCertificateWithoutCAResponseTypeDef",
-    {
-        "certificateArn": str,
-        "certificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRegisterThingRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterThingRequestRequestTypeDef",
     {
         "templateBody": str,
     },
 )
 _OptionalRegisterThingRequestRequestTypeDef = TypedDict(
@@ -5803,23 +4395,14 @@
 )
 
 class RegisterThingRequestRequestTypeDef(
     _RequiredRegisterThingRequestRequestTypeDef, _OptionalRegisterThingRequestRequestTypeDef
 ):
     pass
 
-RegisterThingResponseTypeDef = TypedDict(
-    "RegisterThingResponseTypeDef",
-    {
-        "certificatePem": str,
-        "resourceArns": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRejectCertificateTransferRequestRequestTypeDef = TypedDict(
     "_RequiredRejectCertificateTransferRequestRequestTypeDef",
     {
         "certificateId": str,
     },
 )
 _OptionalRejectCertificateTransferRequestRequestTypeDef = TypedDict(
@@ -5854,25 +4437,14 @@
         "thingGroupArn": str,
         "thingName": str,
         "thingArn": str,
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
 _RequiredSearchIndexRequestRequestTypeDef = TypedDict(
     "_RequiredSearchIndexRequestRequestTypeDef",
     {
         "queryString": str,
     },
 )
 _OptionalSearchIndexRequestRequestTypeDef = TypedDict(
@@ -5906,23 +4478,14 @@
 SetDefaultAuthorizerRequestRequestTypeDef = TypedDict(
     "SetDefaultAuthorizerRequestRequestTypeDef",
     {
         "authorizerName": str,
     },
 )
 
-SetDefaultAuthorizerResponseTypeDef = TypedDict(
-    "SetDefaultAuthorizerResponseTypeDef",
-    {
-        "authorizerName": str,
-        "authorizerArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetDefaultPolicyVersionRequestRequestTypeDef = TypedDict(
     "SetDefaultPolicyVersionRequestRequestTypeDef",
     {
         "policyName": str,
         "policyVersionId": str,
     },
 )
@@ -5943,63 +4506,31 @@
         "certificateArn": str,
         "platform": str,
         "certificatePathOnDevice": str,
     },
     total=False,
 )
 
-StartAuditMitigationActionsTaskResponseTypeDef = TypedDict(
-    "StartAuditMitigationActionsTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartDetectMitigationActionsTaskResponseTypeDef = TypedDict(
-    "StartDetectMitigationActionsTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartOnDemandAuditTaskRequestRequestTypeDef = TypedDict(
     "StartOnDemandAuditTaskRequestRequestTypeDef",
     {
         "targetCheckNames": Sequence[str],
     },
 )
 
-StartOnDemandAuditTaskResponseTypeDef = TypedDict(
-    "StartOnDemandAuditTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartThingRegistrationTaskRequestRequestTypeDef = TypedDict(
     "StartThingRegistrationTaskRequestRequestTypeDef",
     {
         "templateBody": str,
         "inputFileBucket": str,
         "inputFileKey": str,
         "roleArn": str,
     },
 )
 
-StartThingRegistrationTaskResponseTypeDef = TypedDict(
-    "StartThingRegistrationTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopThingRegistrationTaskRequestRequestTypeDef = TypedDict(
     "StopThingRegistrationTaskRequestRequestTypeDef",
     {
         "taskId": str,
     },
 )
 
@@ -6007,26 +4538,14 @@
     "TlsContextTypeDef",
     {
         "serverName": str,
     },
     total=False,
 )
 
-TestInvokeAuthorizerResponseTypeDef = TypedDict(
-    "TestInvokeAuthorizerResponseTypeDef",
-    {
-        "isAuthenticated": bool,
-        "principalId": str,
-        "policyDocuments": List[str],
-        "refreshAfterInSeconds": int,
-        "disconnectAfterInSeconds": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ThingConnectivityTypeDef = TypedDict(
     "ThingConnectivityTypeDef",
     {
         "connected": bool,
         "timestamp": int,
         "disconnectReason": str,
     },
@@ -6109,22 +4628,14 @@
 
 class TransferCertificateRequestRequestTypeDef(
     _RequiredTransferCertificateRequestRequestTypeDef,
     _OptionalTransferCertificateRequestRequestTypeDef,
 ):
     pass
 
-TransferCertificateResponseTypeDef = TypedDict(
-    "TransferCertificateResponseTypeDef",
-    {
-        "transferredCertificateArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -6148,31 +4659,14 @@
 )
 
 class UpdateAuthorizerRequestRequestTypeDef(
     _RequiredUpdateAuthorizerRequestRequestTypeDef, _OptionalUpdateAuthorizerRequestRequestTypeDef
 ):
     pass
 
-UpdateAuthorizerResponseTypeDef = TypedDict(
-    "UpdateAuthorizerResponseTypeDef",
-    {
-        "authorizerName": str,
-        "authorizerArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateBillingGroupResponseTypeDef = TypedDict(
-    "UpdateBillingGroupResponseTypeDef",
-    {
-        "version": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateCertificateRequestRequestTypeDef = TypedDict(
     "UpdateCertificateRequestRequestTypeDef",
     {
         "certificateId": str,
         "newStatus": CertificateStatusType,
     },
 )
@@ -6181,74 +4675,22 @@
     "UpdateCustomMetricRequestRequestTypeDef",
     {
         "metricName": str,
         "displayName": str,
     },
 )
 
-UpdateCustomMetricResponseTypeDef = TypedDict(
-    "UpdateCustomMetricResponseTypeDef",
-    {
-        "metricName": str,
-        "metricArn": str,
-        "metricType": CustomMetricTypeType,
-        "displayName": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateDimensionRequestRequestTypeDef = TypedDict(
     "UpdateDimensionRequestRequestTypeDef",
     {
         "name": str,
         "stringValues": Sequence[str],
     },
 )
 
-UpdateDimensionResponseTypeDef = TypedDict(
-    "UpdateDimensionResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "type": Literal["TOPIC_FILTER"],
-        "stringValues": List[str],
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateDomainConfigurationResponseTypeDef = TypedDict(
-    "UpdateDomainConfigurationResponseTypeDef",
-    {
-        "domainConfigurationName": str,
-        "domainConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateDynamicThingGroupResponseTypeDef = TypedDict(
-    "UpdateDynamicThingGroupResponseTypeDef",
-    {
-        "version": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateMitigationActionResponseTypeDef = TypedDict(
-    "UpdateMitigationActionResponseTypeDef",
-    {
-        "actionArn": str,
-        "actionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdatePackageRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePackageRequestRequestTypeDef",
     {
         "packageName": str,
     },
 )
 _OptionalUpdatePackageRequestRequestTypeDef = TypedDict(
@@ -6307,23 +4749,14 @@
 )
 
 class UpdateRoleAliasRequestRequestTypeDef(
     _RequiredUpdateRoleAliasRequestRequestTypeDef, _OptionalUpdateRoleAliasRequestRequestTypeDef
 ):
     pass
 
-UpdateRoleAliasResponseTypeDef = TypedDict(
-    "UpdateRoleAliasResponseTypeDef",
-    {
-        "roleAlias": str,
-        "roleAliasArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateScheduledAuditRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateScheduledAuditRequestRequestTypeDef",
     {
         "scheduledAuditName": str,
     },
 )
 _OptionalUpdateScheduledAuditRequestRequestTypeDef = TypedDict(
@@ -6339,41 +4772,14 @@
 
 class UpdateScheduledAuditRequestRequestTypeDef(
     _RequiredUpdateScheduledAuditRequestRequestTypeDef,
     _OptionalUpdateScheduledAuditRequestRequestTypeDef,
 ):
     pass
 
-UpdateScheduledAuditResponseTypeDef = TypedDict(
-    "UpdateScheduledAuditResponseTypeDef",
-    {
-        "scheduledAuditArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateStreamResponseTypeDef = TypedDict(
-    "UpdateStreamResponseTypeDef",
-    {
-        "streamId": str,
-        "streamArn": str,
-        "description": str,
-        "streamVersion": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateThingGroupResponseTypeDef = TypedDict(
-    "UpdateThingGroupResponseTypeDef",
-    {
-        "version": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateThingGroupsForThingRequestRequestTypeDef = TypedDict(
     "UpdateThingGroupsForThingRequestRequestTypeDef",
     {
         "thingName": str,
         "thingGroupsToAdd": Sequence[str],
         "thingGroupsToRemove": Sequence[str],
         "overrideDynamicGroups": bool,
@@ -6393,50 +4799,38 @@
     "ValidationErrorTypeDef",
     {
         "errorMessage": str,
     },
     total=False,
 )
 
+AbortConfigOutputTypeDef = TypedDict(
+    "AbortConfigOutputTypeDef",
+    {
+        "criteriaList": List[AbortCriteriaTypeDef],
+    },
+)
+
 AbortConfigTypeDef = TypedDict(
     "AbortConfigTypeDef",
     {
         "criteriaList": Sequence[AbortCriteriaTypeDef],
     },
 )
 
 MetricDatumTypeDef = TypedDict(
     "MetricDatumTypeDef",
     {
         "timestamp": datetime,
-        "value": MetricValueTypeDef,
+        "value": MetricValueOutputTypeDef,
     },
     total=False,
 )
 
-DescribeFleetMetricResponseTypeDef = TypedDict(
-    "DescribeFleetMetricResponseTypeDef",
-    {
-        "metricName": str,
-        "queryString": str,
-        "aggregationType": AggregationTypeTypeDef,
-        "period": int,
-        "aggregationField": str,
-        "description": str,
-        "queryVersion": str,
-        "indexName": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "unit": FleetMetricUnitType,
-        "version": int,
-        "metricArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+AggregationTypeUnionTypeDef = Union[AggregationTypeTypeDef, AggregationTypeOutputTypeDef]
 _RequiredUpdateFleetMetricRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFleetMetricRequestRequestTypeDef",
     {
         "metricName": str,
         "indexName": str,
     },
 )
@@ -6480,61 +4874,884 @@
     "ImplicitDenyTypeDef",
     {
         "policies": List[PolicyTypeDef],
     },
     total=False,
 )
 
+_RequiredAssetPropertyValueTypeDef = TypedDict(
+    "_RequiredAssetPropertyValueTypeDef",
+    {
+        "value": AssetPropertyVariantTypeDef,
+        "timestamp": AssetPropertyTimestampTypeDef,
+    },
+)
+_OptionalAssetPropertyValueTypeDef = TypedDict(
+    "_OptionalAssetPropertyValueTypeDef",
+    {
+        "quality": str,
+    },
+    total=False,
+)
+
+class AssetPropertyValueTypeDef(
+    _RequiredAssetPropertyValueTypeDef, _OptionalAssetPropertyValueTypeDef
+):
+    pass
+
+AssociateTargetsWithJobResponseTypeDef = TypedDict(
+    "AssociateTargetsWithJobResponseTypeDef",
+    {
+        "jobArn": str,
+        "jobId": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelJobResponseTypeDef = TypedDict(
+    "CancelJobResponseTypeDef",
+    {
+        "jobArn": str,
+        "jobId": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAuthorizerResponseTypeDef = TypedDict(
+    "CreateAuthorizerResponseTypeDef",
+    {
+        "authorizerName": str,
+        "authorizerArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateBillingGroupResponseTypeDef = TypedDict(
+    "CreateBillingGroupResponseTypeDef",
+    {
+        "billingGroupName": str,
+        "billingGroupArn": str,
+        "billingGroupId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCertificateFromCsrResponseTypeDef = TypedDict(
+    "CreateCertificateFromCsrResponseTypeDef",
+    {
+        "certificateArn": str,
+        "certificateId": str,
+        "certificatePem": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCustomMetricResponseTypeDef = TypedDict(
+    "CreateCustomMetricResponseTypeDef",
+    {
+        "metricName": str,
+        "metricArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDimensionResponseTypeDef = TypedDict(
+    "CreateDimensionResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDomainConfigurationResponseTypeDef = TypedDict(
+    "CreateDomainConfigurationResponseTypeDef",
+    {
+        "domainConfigurationName": str,
+        "domainConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDynamicThingGroupResponseTypeDef = TypedDict(
+    "CreateDynamicThingGroupResponseTypeDef",
+    {
+        "thingGroupName": str,
+        "thingGroupArn": str,
+        "thingGroupId": str,
+        "indexName": str,
+        "queryString": str,
+        "queryVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFleetMetricResponseTypeDef = TypedDict(
+    "CreateFleetMetricResponseTypeDef",
+    {
+        "metricName": str,
+        "metricArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateJobResponseTypeDef = TypedDict(
+    "CreateJobResponseTypeDef",
+    {
+        "jobArn": str,
+        "jobId": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateJobTemplateResponseTypeDef = TypedDict(
+    "CreateJobTemplateResponseTypeDef",
+    {
+        "jobTemplateArn": str,
+        "jobTemplateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMitigationActionResponseTypeDef = TypedDict(
+    "CreateMitigationActionResponseTypeDef",
+    {
+        "actionArn": str,
+        "actionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateOTAUpdateResponseTypeDef = TypedDict(
+    "CreateOTAUpdateResponseTypeDef",
+    {
+        "otaUpdateId": str,
+        "awsIotJobId": str,
+        "otaUpdateArn": str,
+        "awsIotJobArn": str,
+        "otaUpdateStatus": OTAUpdateStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePackageResponseTypeDef = TypedDict(
+    "CreatePackageResponseTypeDef",
+    {
+        "packageName": str,
+        "packageArn": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePackageVersionResponseTypeDef = TypedDict(
+    "CreatePackageVersionResponseTypeDef",
+    {
+        "packageVersionArn": str,
+        "packageName": str,
+        "versionName": str,
+        "description": str,
+        "attributes": Dict[str, str],
+        "status": PackageVersionStatusType,
+        "errorReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePolicyResponseTypeDef = TypedDict(
+    "CreatePolicyResponseTypeDef",
+    {
+        "policyName": str,
+        "policyArn": str,
+        "policyDocument": str,
+        "policyVersionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePolicyVersionResponseTypeDef = TypedDict(
+    "CreatePolicyVersionResponseTypeDef",
+    {
+        "policyArn": str,
+        "policyDocument": str,
+        "policyVersionId": str,
+        "isDefaultVersion": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProvisioningTemplateResponseTypeDef = TypedDict(
+    "CreateProvisioningTemplateResponseTypeDef",
+    {
+        "templateArn": str,
+        "templateName": str,
+        "defaultVersionId": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProvisioningTemplateVersionResponseTypeDef = TypedDict(
+    "CreateProvisioningTemplateVersionResponseTypeDef",
+    {
+        "templateArn": str,
+        "templateName": str,
+        "versionId": int,
+        "isDefaultVersion": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRoleAliasResponseTypeDef = TypedDict(
+    "CreateRoleAliasResponseTypeDef",
+    {
+        "roleAlias": str,
+        "roleAliasArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateScheduledAuditResponseTypeDef = TypedDict(
+    "CreateScheduledAuditResponseTypeDef",
+    {
+        "scheduledAuditArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSecurityProfileResponseTypeDef = TypedDict(
+    "CreateSecurityProfileResponseTypeDef",
+    {
+        "securityProfileName": str,
+        "securityProfileArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStreamResponseTypeDef = TypedDict(
+    "CreateStreamResponseTypeDef",
+    {
+        "streamId": str,
+        "streamArn": str,
+        "description": str,
+        "streamVersion": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateThingGroupResponseTypeDef = TypedDict(
+    "CreateThingGroupResponseTypeDef",
+    {
+        "thingGroupName": str,
+        "thingGroupArn": str,
+        "thingGroupId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateThingResponseTypeDef = TypedDict(
+    "CreateThingResponseTypeDef",
+    {
+        "thingName": str,
+        "thingArn": str,
+        "thingId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateThingTypeResponseTypeDef = TypedDict(
+    "CreateThingTypeResponseTypeDef",
+    {
+        "thingTypeName": str,
+        "thingTypeArn": str,
+        "thingTypeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeCustomMetricResponseTypeDef = TypedDict(
+    "DescribeCustomMetricResponseTypeDef",
+    {
+        "metricName": str,
+        "metricArn": str,
+        "metricType": CustomMetricTypeType,
+        "displayName": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDimensionResponseTypeDef = TypedDict(
+    "DescribeDimensionResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "type": Literal["TOPIC_FILTER"],
+        "stringValues": List[str],
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEndpointResponseTypeDef = TypedDict(
+    "DescribeEndpointResponseTypeDef",
+    {
+        "endpointAddress": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeFleetMetricResponseTypeDef = TypedDict(
+    "DescribeFleetMetricResponseTypeDef",
+    {
+        "metricName": str,
+        "queryString": str,
+        "aggregationType": AggregationTypeOutputTypeDef,
+        "period": int,
+        "aggregationField": str,
+        "description": str,
+        "queryVersion": str,
+        "indexName": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "unit": FleetMetricUnitType,
+        "version": int,
+        "metricArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeIndexResponseTypeDef = TypedDict(
+    "DescribeIndexResponseTypeDef",
+    {
+        "indexName": str,
+        "indexStatus": IndexStatusType,
+        "schema": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeProvisioningTemplateVersionResponseTypeDef = TypedDict(
+    "DescribeProvisioningTemplateVersionResponseTypeDef",
+    {
+        "versionId": int,
+        "creationDate": datetime,
+        "templateBody": str,
+        "isDefaultVersion": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeScheduledAuditResponseTypeDef = TypedDict(
+    "DescribeScheduledAuditResponseTypeDef",
+    {
+        "frequency": AuditFrequencyType,
+        "dayOfMonth": str,
+        "dayOfWeek": DayOfWeekType,
+        "targetCheckNames": List[str],
+        "scheduledAuditName": str,
+        "scheduledAuditArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeThingRegistrationTaskResponseTypeDef = TypedDict(
+    "DescribeThingRegistrationTaskResponseTypeDef",
+    {
+        "taskId": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "templateBody": str,
+        "inputFileBucket": str,
+        "inputFileKey": str,
+        "roleArn": str,
+        "status": StatusType,
+        "message": str,
+        "successCount": int,
+        "failureCount": int,
+        "percentageProgress": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeThingResponseTypeDef = TypedDict(
+    "DescribeThingResponseTypeDef",
+    {
+        "defaultClientId": str,
+        "thingName": str,
+        "thingId": str,
+        "thingArn": str,
+        "thingTypeName": str,
+        "attributes": Dict[str, str],
+        "version": int,
+        "billingGroupName": str,
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
+GetCardinalityResponseTypeDef = TypedDict(
+    "GetCardinalityResponseTypeDef",
+    {
+        "cardinality": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetJobDocumentResponseTypeDef = TypedDict(
+    "GetJobDocumentResponseTypeDef",
+    {
+        "document": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetLoggingOptionsResponseTypeDef = TypedDict(
+    "GetLoggingOptionsResponseTypeDef",
+    {
+        "roleArn": str,
+        "logLevel": LogLevelType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPackageResponseTypeDef = TypedDict(
+    "GetPackageResponseTypeDef",
+    {
+        "packageName": str,
+        "packageArn": str,
+        "description": str,
+        "defaultVersionName": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPackageVersionResponseTypeDef = TypedDict(
+    "GetPackageVersionResponseTypeDef",
+    {
+        "packageVersionArn": str,
+        "packageName": str,
+        "versionName": str,
+        "description": str,
+        "attributes": Dict[str, str],
+        "status": PackageVersionStatusType,
+        "errorReason": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPolicyResponseTypeDef = TypedDict(
+    "GetPolicyResponseTypeDef",
+    {
+        "policyName": str,
+        "policyArn": str,
+        "policyDocument": str,
+        "defaultVersionId": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "generationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPolicyVersionResponseTypeDef = TypedDict(
+    "GetPolicyVersionResponseTypeDef",
+    {
+        "policyArn": str,
+        "policyName": str,
+        "policyDocument": str,
+        "policyVersionId": str,
+        "isDefaultVersion": bool,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "generationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRegistrationCodeResponseTypeDef = TypedDict(
+    "GetRegistrationCodeResponseTypeDef",
+    {
+        "registrationCode": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetV2LoggingOptionsResponseTypeDef = TypedDict(
+    "GetV2LoggingOptionsResponseTypeDef",
+    {
+        "roleArn": str,
+        "defaultLogLevel": LogLevelType,
+        "disableAllLogs": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListAttachedPoliciesResponseTypeDef = TypedDict(
     "ListAttachedPoliciesResponseTypeDef",
     {
         "policies": List[PolicyTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCustomMetricsResponseTypeDef = TypedDict(
+    "ListCustomMetricsResponseTypeDef",
+    {
+        "metricNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDimensionsResponseTypeDef = TypedDict(
+    "ListDimensionsResponseTypeDef",
+    {
+        "dimensionNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListIndicesResponseTypeDef = TypedDict(
+    "ListIndicesResponseTypeDef",
+    {
+        "indexNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPoliciesResponseTypeDef = TypedDict(
     "ListPoliciesResponseTypeDef",
     {
         "policies": List[PolicyTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPolicyPrincipalsResponseTypeDef = TypedDict(
+    "ListPolicyPrincipalsResponseTypeDef",
+    {
+        "principals": List[str],
+        "nextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPrincipalPoliciesResponseTypeDef = TypedDict(
     "ListPrincipalPoliciesResponseTypeDef",
     {
         "policies": List[PolicyTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredAssetPropertyValueTypeDef = TypedDict(
-    "_RequiredAssetPropertyValueTypeDef",
+ListPrincipalThingsResponseTypeDef = TypedDict(
+    "ListPrincipalThingsResponseTypeDef",
     {
-        "value": AssetPropertyVariantTypeDef,
-        "timestamp": AssetPropertyTimestampTypeDef,
+        "things": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalAssetPropertyValueTypeDef = TypedDict(
-    "_OptionalAssetPropertyValueTypeDef",
+
+ListRoleAliasesResponseTypeDef = TypedDict(
+    "ListRoleAliasesResponseTypeDef",
     {
-        "quality": str,
+        "roleAliases": List[str],
+        "nextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class AssetPropertyValueTypeDef(
-    _RequiredAssetPropertyValueTypeDef, _OptionalAssetPropertyValueTypeDef
-):
-    pass
+ListTargetsForPolicyResponseTypeDef = TypedDict(
+    "ListTargetsForPolicyResponseTypeDef",
+    {
+        "targets": List[str],
+        "nextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListThingPrincipalsResponseTypeDef = TypedDict(
+    "ListThingPrincipalsResponseTypeDef",
+    {
+        "principals": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListThingRegistrationTaskReportsResponseTypeDef = TypedDict(
+    "ListThingRegistrationTaskReportsResponseTypeDef",
+    {
+        "resourceLinks": List[str],
+        "reportType": ReportTypeType,
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListThingRegistrationTasksResponseTypeDef = TypedDict(
+    "ListThingRegistrationTasksResponseTypeDef",
+    {
+        "taskIds": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListThingsInBillingGroupResponseTypeDef = TypedDict(
+    "ListThingsInBillingGroupResponseTypeDef",
+    {
+        "things": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListThingsInThingGroupResponseTypeDef = TypedDict(
+    "ListThingsInThingGroupResponseTypeDef",
+    {
+        "things": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterCACertificateResponseTypeDef = TypedDict(
+    "RegisterCACertificateResponseTypeDef",
+    {
+        "certificateArn": str,
+        "certificateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterCertificateResponseTypeDef = TypedDict(
+    "RegisterCertificateResponseTypeDef",
+    {
+        "certificateArn": str,
+        "certificateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterCertificateWithoutCAResponseTypeDef = TypedDict(
+    "RegisterCertificateWithoutCAResponseTypeDef",
+    {
+        "certificateArn": str,
+        "certificateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterThingResponseTypeDef = TypedDict(
+    "RegisterThingResponseTypeDef",
+    {
+        "certificatePem": str,
+        "resourceArns": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetDefaultAuthorizerResponseTypeDef = TypedDict(
+    "SetDefaultAuthorizerResponseTypeDef",
+    {
+        "authorizerName": str,
+        "authorizerArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartAuditMitigationActionsTaskResponseTypeDef = TypedDict(
+    "StartAuditMitigationActionsTaskResponseTypeDef",
+    {
+        "taskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartDetectMitigationActionsTaskResponseTypeDef = TypedDict(
+    "StartDetectMitigationActionsTaskResponseTypeDef",
+    {
+        "taskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartOnDemandAuditTaskResponseTypeDef = TypedDict(
+    "StartOnDemandAuditTaskResponseTypeDef",
+    {
+        "taskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartThingRegistrationTaskResponseTypeDef = TypedDict(
+    "StartThingRegistrationTaskResponseTypeDef",
+    {
+        "taskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestInvokeAuthorizerResponseTypeDef = TypedDict(
+    "TestInvokeAuthorizerResponseTypeDef",
+    {
+        "isAuthenticated": bool,
+        "principalId": str,
+        "policyDocuments": List[str],
+        "refreshAfterInSeconds": int,
+        "disconnectAfterInSeconds": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TransferCertificateResponseTypeDef = TypedDict(
+    "TransferCertificateResponseTypeDef",
+    {
+        "transferredCertificateArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAuthorizerResponseTypeDef = TypedDict(
+    "UpdateAuthorizerResponseTypeDef",
+    {
+        "authorizerName": str,
+        "authorizerArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBillingGroupResponseTypeDef = TypedDict(
+    "UpdateBillingGroupResponseTypeDef",
+    {
+        "version": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateCustomMetricResponseTypeDef = TypedDict(
+    "UpdateCustomMetricResponseTypeDef",
+    {
+        "metricName": str,
+        "metricArn": str,
+        "metricType": CustomMetricTypeType,
+        "displayName": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDimensionResponseTypeDef = TypedDict(
+    "UpdateDimensionResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "type": Literal["TOPIC_FILTER"],
+        "stringValues": List[str],
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDomainConfigurationResponseTypeDef = TypedDict(
+    "UpdateDomainConfigurationResponseTypeDef",
+    {
+        "domainConfigurationName": str,
+        "domainConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+UpdateDynamicThingGroupResponseTypeDef = TypedDict(
+    "UpdateDynamicThingGroupResponseTypeDef",
+    {
+        "version": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateMitigationActionResponseTypeDef = TypedDict(
+    "UpdateMitigationActionResponseTypeDef",
+    {
+        "actionArn": str,
+        "actionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRoleAliasResponseTypeDef = TypedDict(
+    "UpdateRoleAliasResponseTypeDef",
+    {
+        "roleAlias": str,
+        "roleAliasArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateScheduledAuditResponseTypeDef = TypedDict(
+    "UpdateScheduledAuditResponseTypeDef",
+    {
+        "scheduledAuditArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateStreamResponseTypeDef = TypedDict(
+    "UpdateStreamResponseTypeDef",
+    {
+        "streamId": str,
+        "streamArn": str,
+        "description": str,
+        "streamVersion": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateThingGroupResponseTypeDef = TypedDict(
+    "UpdateThingGroupResponseTypeDef",
+    {
+        "version": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ThingGroupPropertiesOutputTypeDef = TypedDict(
+    "ThingGroupPropertiesOutputTypeDef",
+    {
+        "thingGroupDescription": str,
+        "attributePayload": AttributePayloadOutputTypeDef,
+    },
+    total=False,
+)
+
+AttributePayloadUnionTypeDef = Union[AttributePayloadTypeDef, AttributePayloadOutputTypeDef]
 _RequiredCreateThingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateThingRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 _OptionalCreateThingRequestRequestTypeDef = TypedDict(
@@ -6584,27 +5801,30 @@
     pass
 
 ListAuditMitigationActionsExecutionsResponseTypeDef = TypedDict(
     "ListAuditMitigationActionsExecutionsResponseTypeDef",
     {
         "actionsExecutions": List[AuditMitigationActionExecutionMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAuditMitigationActionsTasksResponseTypeDef = TypedDict(
     "ListAuditMitigationActionsTasksResponseTypeDef",
     {
         "tasks": List[AuditMitigationActionsTaskMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AuditMitigationActionsTaskTargetUnionTypeDef = Union[
+    AuditMitigationActionsTaskTargetTypeDef, AuditMitigationActionsTaskTargetOutputTypeDef
+]
 StartAuditMitigationActionsTaskRequestRequestTypeDef = TypedDict(
     "StartAuditMitigationActionsTaskRequestRequestTypeDef",
     {
         "taskId": str,
         "target": AuditMitigationActionsTaskTargetTypeDef,
         "auditCheckToActionsMapping": Mapping[str, Sequence[str]],
         "clientRequestToken": str,
@@ -6615,15 +5835,15 @@
     "DescribeAccountAuditConfigurationResponseTypeDef",
     {
         "roleArn": str,
         "auditNotificationTargetConfigurations": Dict[
             Literal["SNS"], AuditNotificationTargetTypeDef
         ],
         "auditCheckConfigurations": Dict[str, AuditCheckConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAccountAuditConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateAccountAuditConfigurationRequestRequestTypeDef",
     {
         "roleArn": str,
@@ -6636,63 +5856,41 @@
 )
 
 ListAuditTasksResponseTypeDef = TypedDict(
     "ListAuditTasksResponseTypeDef",
     {
         "tasks": List[AuditTaskMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredTestAuthorizationRequestRequestTypeDef = TypedDict(
-    "_RequiredTestAuthorizationRequestRequestTypeDef",
-    {
-        "authInfos": Sequence[AuthInfoTypeDef],
-    },
-)
-_OptionalTestAuthorizationRequestRequestTypeDef = TypedDict(
-    "_OptionalTestAuthorizationRequestRequestTypeDef",
-    {
-        "principal": str,
-        "cognitoIdentityPoolId": str,
-        "clientId": str,
-        "policyNamesToAdd": Sequence[str],
-        "policyNamesToSkip": Sequence[str],
-    },
-    total=False,
-)
-
-class TestAuthorizationRequestRequestTypeDef(
-    _RequiredTestAuthorizationRequestRequestTypeDef, _OptionalTestAuthorizationRequestRequestTypeDef
-):
-    pass
-
+AuthInfoUnionTypeDef = Union[AuthInfoTypeDef, AuthInfoOutputTypeDef]
 DescribeAuthorizerResponseTypeDef = TypedDict(
     "DescribeAuthorizerResponseTypeDef",
     {
         "authorizerDescription": AuthorizerDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDefaultAuthorizerResponseTypeDef = TypedDict(
     "DescribeDefaultAuthorizerResponseTypeDef",
     {
         "authorizerDescription": AuthorizerDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAuthorizersResponseTypeDef = TypedDict(
     "ListAuthorizersResponseTypeDef",
     {
         "authorizers": List[AuthorizerSummaryTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AwsJobAbortConfigTypeDef = TypedDict(
     "AwsJobAbortConfigTypeDef",
     {
         "abortCriteriaList": Sequence[AwsJobAbortCriteriaTypeDef],
@@ -6704,14 +5902,28 @@
     {
         "baseRatePerMinute": int,
         "incrementFactor": float,
         "rateIncreaseCriteria": AwsJobRateIncreaseCriteriaTypeDef,
     },
 )
 
+BehaviorCriteriaOutputTypeDef = TypedDict(
+    "BehaviorCriteriaOutputTypeDef",
+    {
+        "comparisonOperator": ComparisonOperatorType,
+        "value": MetricValueOutputTypeDef,
+        "durationSeconds": int,
+        "consecutiveDatapointsToAlarm": int,
+        "consecutiveDatapointsToClear": int,
+        "statisticalThreshold": StatisticalThresholdTypeDef,
+        "mlDetectionConfig": MachineLearningDetectionConfigTypeDef,
+    },
+    total=False,
+)
+
 BehaviorCriteriaTypeDef = TypedDict(
     "BehaviorCriteriaTypeDef",
     {
         "comparisonOperator": ComparisonOperatorType,
         "value": MetricValueTypeDef,
         "durationSeconds": int,
         "consecutiveDatapointsToAlarm": int,
@@ -6723,15 +5935,15 @@
 )
 
 GetBehaviorModelTrainingSummariesResponseTypeDef = TypedDict(
     "GetBehaviorModelTrainingSummariesResponseTypeDef",
     {
         "summaries": List[BehaviorModelTrainingSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredMetricToRetainTypeDef = TypedDict(
     "_RequiredMetricToRetainTypeDef",
     {
         "metric": str,
@@ -6753,15 +5965,15 @@
     {
         "billingGroupName": str,
         "billingGroupId": str,
         "billingGroupArn": str,
         "version": int,
         "billingGroupProperties": BillingGroupPropertiesTypeDef,
         "billingGroupMetadata": BillingGroupMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateBillingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBillingGroupRequestRequestTypeDef",
     {
         "billingGroupName": str,
@@ -6778,20 +5990,38 @@
 
 class UpdateBillingGroupRequestRequestTypeDef(
     _RequiredUpdateBillingGroupRequestRequestTypeDef,
     _OptionalUpdateBillingGroupRequestRequestTypeDef,
 ):
     pass
 
+CodeSigningSignatureTypeDef = TypedDict(
+    "CodeSigningSignatureTypeDef",
+    {
+        "inlineDocument": BlobTypeDef,
+    },
+    total=False,
+)
+
+MqttContextTypeDef = TypedDict(
+    "MqttContextTypeDef",
+    {
+        "username": str,
+        "password": BlobTypeDef,
+        "clientId": str,
+    },
+    total=False,
+)
+
 GetBucketsAggregationResponseTypeDef = TypedDict(
     "GetBucketsAggregationResponseTypeDef",
     {
         "totalCount": int,
         "buckets": List[BucketTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BucketsAggregationTypeTypeDef = TypedDict(
     "BucketsAggregationTypeTypeDef",
     {
         "termsAggregation": TermsAggregationTypeDef,
@@ -6819,15 +6049,15 @@
 )
 
 ListCACertificatesResponseTypeDef = TypedDict(
     "ListCACertificatesResponseTypeDef",
     {
         "certificates": List[CACertificateTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CertificateDescriptionTypeDef = TypedDict(
     "CertificateDescriptionTypeDef",
     {
         "certificateArn": str,
@@ -6849,56 +6079,200 @@
 )
 
 ListCertificatesByCAResponseTypeDef = TypedDict(
     "ListCertificatesByCAResponseTypeDef",
     {
         "certificates": List[CertificateTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCertificatesResponseTypeDef = TypedDict(
     "ListCertificatesResponseTypeDef",
     {
         "certificates": List[CertificateTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CustomCodeSigningTypeDef = TypedDict(
-    "CustomCodeSigningTypeDef",
+CustomCodeSigningOutputTypeDef = TypedDict(
+    "CustomCodeSigningOutputTypeDef",
     {
-        "signature": CodeSigningSignatureTypeDef,
+        "signature": CodeSigningSignatureOutputTypeDef,
         "certificateChain": CodeSigningCertificateChainTypeDef,
         "hashAlgorithm": str,
         "signatureAlgorithm": str,
     },
     total=False,
 )
 
 DescribeEventConfigurationsResponseTypeDef = TypedDict(
     "DescribeEventConfigurationsResponseTypeDef",
     {
         "eventConfigurations": Dict[EventTypeType, ConfigurationTypeDef],
         "creationDate": datetime,
         "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEventConfigurationsRequestRequestTypeDef = TypedDict(
     "UpdateEventConfigurationsRequestRequestTypeDef",
     {
         "eventConfigurations": Mapping[EventTypeType, ConfigurationTypeDef],
     },
     total=False,
 )
 
+_RequiredListAuditMitigationActionsTasksRequestRequestTypeDef = TypedDict(
+    "_RequiredListAuditMitigationActionsTasksRequestRequestTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListAuditMitigationActionsTasksRequestRequestTypeDef = TypedDict(
+    "_OptionalListAuditMitigationActionsTasksRequestRequestTypeDef",
+    {
+        "auditTaskId": str,
+        "findingId": str,
+        "taskStatus": AuditMitigationActionsTaskStatusType,
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+class ListAuditMitigationActionsTasksRequestRequestTypeDef(
+    _RequiredListAuditMitigationActionsTasksRequestRequestTypeDef,
+    _OptionalListAuditMitigationActionsTasksRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListAuditTasksRequestRequestTypeDef = TypedDict(
+    "_RequiredListAuditTasksRequestRequestTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListAuditTasksRequestRequestTypeDef = TypedDict(
+    "_OptionalListAuditTasksRequestRequestTypeDef",
+    {
+        "taskType": AuditTaskTypeType,
+        "taskStatus": AuditTaskStatusType,
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+class ListAuditTasksRequestRequestTypeDef(
+    _RequiredListAuditTasksRequestRequestTypeDef, _OptionalListAuditTasksRequestRequestTypeDef
+):
+    pass
+
+ListDetectMitigationActionsExecutionsRequestRequestTypeDef = TypedDict(
+    "ListDetectMitigationActionsExecutionsRequestRequestTypeDef",
+    {
+        "taskId": str,
+        "violationId": str,
+        "thingName": str,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+_RequiredListDetectMitigationActionsTasksRequestRequestTypeDef = TypedDict(
+    "_RequiredListDetectMitigationActionsTasksRequestRequestTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListDetectMitigationActionsTasksRequestRequestTypeDef = TypedDict(
+    "_OptionalListDetectMitigationActionsTasksRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+class ListDetectMitigationActionsTasksRequestRequestTypeDef(
+    _RequiredListDetectMitigationActionsTasksRequestRequestTypeDef,
+    _OptionalListDetectMitigationActionsTasksRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListMetricValuesRequestRequestTypeDef = TypedDict(
+    "_RequiredListMetricValuesRequestRequestTypeDef",
+    {
+        "thingName": str,
+        "metricName": str,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListMetricValuesRequestRequestTypeDef = TypedDict(
+    "_OptionalListMetricValuesRequestRequestTypeDef",
+    {
+        "dimensionName": str,
+        "dimensionValueOperator": DimensionValueOperatorType,
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+class ListMetricValuesRequestRequestTypeDef(
+    _RequiredListMetricValuesRequestRequestTypeDef, _OptionalListMetricValuesRequestRequestTypeDef
+):
+    pass
+
+_RequiredListViolationEventsRequestRequestTypeDef = TypedDict(
+    "_RequiredListViolationEventsRequestRequestTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListViolationEventsRequestRequestTypeDef = TypedDict(
+    "_OptionalListViolationEventsRequestRequestTypeDef",
+    {
+        "thingName": str,
+        "securityProfileName": str,
+        "behaviorCriteriaType": BehaviorCriteriaTypeType,
+        "listSuppressedAlerts": bool,
+        "verificationState": VerificationStateType,
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+class ListViolationEventsRequestRequestTypeDef(
+    _RequiredListViolationEventsRequestRequestTypeDef,
+    _OptionalListViolationEventsRequestRequestTypeDef,
+):
+    pass
+
+ViolationEventOccurrenceRangeTypeDef = TypedDict(
+    "ViolationEventOccurrenceRangeTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+
 _RequiredCreateAuthorizerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAuthorizerRequestRequestTypeDef",
     {
         "authorizerName": str,
         "authorizerFunctionArn": str,
     },
 )
@@ -7079,15 +6453,15 @@
     pass
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -7140,14 +6514,25 @@
 
 class UpdateDomainConfigurationRequestRequestTypeDef(
     _RequiredUpdateDomainConfigurationRequestRequestTypeDef,
     _OptionalUpdateDomainConfigurationRequestRequestTypeDef,
 ):
     pass
 
+SchedulingConfigOutputTypeDef = TypedDict(
+    "SchedulingConfigOutputTypeDef",
+    {
+        "startTime": str,
+        "endTime": str,
+        "endBehavior": JobEndBehaviorType,
+        "maintenanceWindows": List[MaintenanceWindowTypeDef],
+    },
+    total=False,
+)
+
 SchedulingConfigTypeDef = TypedDict(
     "SchedulingConfigTypeDef",
     {
         "startTime": str,
         "endTime": str,
         "endBehavior": JobEndBehaviorType,
         "maintenanceWindows": Sequence[MaintenanceWindowTypeDef],
@@ -7158,26 +6543,26 @@
 CreateKeysAndCertificateResponseTypeDef = TypedDict(
     "CreateKeysAndCertificateResponseTypeDef",
     {
         "certificateArn": str,
         "certificateId": str,
         "certificatePem": str,
         "keyPair": KeyPairTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateProvisioningClaimResponseTypeDef = TypedDict(
     "CreateProvisioningClaimResponseTypeDef",
     {
         "certificateId": str,
         "certificatePem": str,
         "keyPair": KeyPairTypeDef,
         "expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateProvisioningTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProvisioningTemplateRequestRequestTypeDef",
     {
         "templateName": str,
@@ -7213,15 +6598,15 @@
         "lastModifiedDate": datetime,
         "defaultVersionId": int,
         "templateBody": str,
         "enabled": bool,
         "provisioningRoleArn": str,
         "preProvisioningHook": ProvisioningHookTypeDef,
         "type": TemplateTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateProvisioningTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProvisioningTemplateRequestRequestTypeDef",
     {
         "templateName": str,
@@ -7271,15 +6656,15 @@
     {
         "taskStatus": AuditTaskStatusType,
         "taskType": AuditTaskTypeType,
         "taskStartTime": datetime,
         "taskStatistics": TaskStatisticsTypeDef,
         "scheduledAuditName": str,
         "auditDetails": Dict[str, AuditCheckDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRegisterCACertificateRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterCACertificateRequestRequestTypeDef",
     {
         "caCertificate": str,
@@ -7336,111 +6721,92 @@
         "serverCertificates": List[ServerCertificateSummaryTypeDef],
         "authorizerConfig": AuthorizerConfigTypeDef,
         "domainConfigurationStatus": DomainConfigurationStatusType,
         "serviceType": ServiceTypeType,
         "domainType": DomainTypeType,
         "lastStatusChangeDate": datetime,
         "tlsConfig": TlsConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeManagedJobTemplateResponseTypeDef = TypedDict(
     "DescribeManagedJobTemplateResponseTypeDef",
     {
         "templateName": str,
         "templateArn": str,
         "description": str,
         "templateVersion": str,
         "environments": List[str],
         "documentParameters": List[DocumentParameterTypeDef],
         "document": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRoleAliasResponseTypeDef = TypedDict(
     "DescribeRoleAliasResponseTypeDef",
     {
         "roleAliasDescription": RoleAliasDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeThingTypeResponseTypeDef = TypedDict(
     "DescribeThingTypeResponseTypeDef",
     {
         "thingTypeName": str,
         "thingTypeId": str,
         "thingTypeArn": str,
-        "thingTypeProperties": ThingTypePropertiesTypeDef,
+        "thingTypeProperties": ThingTypePropertiesOutputTypeDef,
         "thingTypeMetadata": ThingTypeMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ThingTypeDefinitionTypeDef = TypedDict(
     "ThingTypeDefinitionTypeDef",
     {
         "thingTypeName": str,
         "thingTypeArn": str,
-        "thingTypeProperties": ThingTypePropertiesTypeDef,
+        "thingTypeProperties": ThingTypePropertiesOutputTypeDef,
         "thingTypeMetadata": ThingTypeMetadataTypeDef,
     },
     total=False,
 )
 
+ThingTypePropertiesUnionTypeDef = Union[
+    ThingTypePropertiesTypeDef, ThingTypePropertiesOutputTypeDef
+]
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "s3Destination": S3DestinationTypeDef,
     },
     total=False,
 )
 
 ListDetectMitigationActionsExecutionsResponseTypeDef = TypedDict(
     "ListDetectMitigationActionsExecutionsResponseTypeDef",
     {
         "actionsExecutions": List[DetectMitigationActionExecutionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
-    "_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef",
-    {
-        "taskId": str,
-        "target": DetectMitigationActionsTaskTargetTypeDef,
-        "actions": Sequence[str],
-        "clientRequestToken": str,
-    },
-)
-_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
-    "_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef",
-    {
-        "violationEventOccurrenceRange": ViolationEventOccurrenceRangeTypeDef,
-        "includeOnlyActiveViolations": bool,
-        "includeSuppressedAlerts": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class StartDetectMitigationActionsTaskRequestRequestTypeDef(
-    _RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef,
-    _OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef,
-):
-    pass
-
+DetectMitigationActionsTaskTargetUnionTypeDef = Union[
+    DetectMitigationActionsTaskTargetTypeDef, DetectMitigationActionsTaskTargetOutputTypeDef
+]
 ListDomainConfigurationsResponseTypeDef = TypedDict(
     "ListDomainConfigurationsResponseTypeDef",
     {
         "domainConfigurations": List[DomainConfigurationSummaryTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DynamoDBv2ActionTypeDef = TypedDict(
     "DynamoDBv2ActionTypeDef",
     {
         "roleArn": str,
@@ -7448,38 +6814,59 @@
     },
 )
 
 GetEffectivePoliciesResponseTypeDef = TypedDict(
     "GetEffectivePoliciesResponseTypeDef",
     {
         "effectivePolicies": List[EffectivePolicyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExponentialRolloutRateTypeDef = TypedDict(
     "ExponentialRolloutRateTypeDef",
     {
         "baseRatePerMinute": int,
         "incrementFactor": float,
         "rateIncreaseCriteria": RateIncreaseCriteriaTypeDef,
     },
 )
 
+_RequiredThingGroupIndexingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredThingGroupIndexingConfigurationOutputTypeDef",
+    {
+        "thingGroupIndexingMode": ThingGroupIndexingModeType,
+    },
+)
+_OptionalThingGroupIndexingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalThingGroupIndexingConfigurationOutputTypeDef",
+    {
+        "managedFields": List[FieldTypeDef],
+        "customFields": List[FieldTypeDef],
+    },
+    total=False,
+)
+
+class ThingGroupIndexingConfigurationOutputTypeDef(
+    _RequiredThingGroupIndexingConfigurationOutputTypeDef,
+    _OptionalThingGroupIndexingConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredThingGroupIndexingConfigurationTypeDef = TypedDict(
     "_RequiredThingGroupIndexingConfigurationTypeDef",
     {
         "thingGroupIndexingMode": ThingGroupIndexingModeType,
     },
 )
 _OptionalThingGroupIndexingConfigurationTypeDef = TypedDict(
     "_OptionalThingGroupIndexingConfigurationTypeDef",
     {
-        "managedFields": List[FieldTypeDef],
-        "customFields": List[FieldTypeDef],
+        "managedFields": Sequence[FieldTypeDef],
+        "customFields": Sequence[FieldTypeDef],
     },
     total=False,
 )
 
 class ThingGroupIndexingConfigurationTypeDef(
     _RequiredThingGroupIndexingConfigurationTypeDef, _OptionalThingGroupIndexingConfigurationTypeDef
 ):
@@ -7504,23 +6891,866 @@
 )
 
 ListFleetMetricsResponseTypeDef = TypedDict(
     "ListFleetMetricsResponseTypeDef",
     {
         "fleetMetrics": List[FleetMetricNameAndArnTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef = (
+    TypedDict(
+        "GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef",
+        {
+            "securityProfileName": str,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+ListActiveViolationsRequestListActiveViolationsPaginateTypeDef = TypedDict(
+    "ListActiveViolationsRequestListActiveViolationsPaginateTypeDef",
+    {
+        "thingName": str,
+        "securityProfileName": str,
+        "behaviorCriteriaType": BehaviorCriteriaTypeType,
+        "listSuppressedAlerts": bool,
+        "verificationState": VerificationStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef",
+    {
+        "target": str,
+    },
+)
+_OptionalListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef",
+    {
+        "recursive": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef(
+    _RequiredListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef,
+    _OptionalListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef,
+):
+    pass
+
+_RequiredListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef",
+    {
+        "taskId": str,
+        "findingId": str,
+    },
+)
+_OptionalListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef",
+    {
+        "actionStatus": AuditMitigationActionsExecutionStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef(
+    _RequiredListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef,
+    _OptionalListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef,
+):
+    pass
+
+_RequiredListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef = TypedDict(
+    "_RequiredListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef = TypedDict(
+    "_OptionalListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef",
+    {
+        "auditTaskId": str,
+        "findingId": str,
+        "taskStatus": AuditMitigationActionsTaskStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef(
+    _RequiredListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef,
+    _OptionalListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef,
+):
+    pass
+
+_RequiredListAuditTasksRequestListAuditTasksPaginateTypeDef = TypedDict(
+    "_RequiredListAuditTasksRequestListAuditTasksPaginateTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListAuditTasksRequestListAuditTasksPaginateTypeDef = TypedDict(
+    "_OptionalListAuditTasksRequestListAuditTasksPaginateTypeDef",
+    {
+        "taskType": AuditTaskTypeType,
+        "taskStatus": AuditTaskStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAuditTasksRequestListAuditTasksPaginateTypeDef(
+    _RequiredListAuditTasksRequestListAuditTasksPaginateTypeDef,
+    _OptionalListAuditTasksRequestListAuditTasksPaginateTypeDef,
+):
+    pass
+
+ListAuthorizersRequestListAuthorizersPaginateTypeDef = TypedDict(
+    "ListAuthorizersRequestListAuthorizersPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "status": AuthorizerStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListBillingGroupsRequestListBillingGroupsPaginateTypeDef = TypedDict(
+    "ListBillingGroupsRequestListBillingGroupsPaginateTypeDef",
+    {
+        "namePrefixFilter": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCACertificatesRequestListCACertificatesPaginateTypeDef = TypedDict(
+    "ListCACertificatesRequestListCACertificatesPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "templateName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListCertificatesByCARequestListCertificatesByCAPaginateTypeDef = TypedDict(
+    "_RequiredListCertificatesByCARequestListCertificatesByCAPaginateTypeDef",
+    {
+        "caCertificateId": str,
     },
 )
+_OptionalListCertificatesByCARequestListCertificatesByCAPaginateTypeDef = TypedDict(
+    "_OptionalListCertificatesByCARequestListCertificatesByCAPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListCertificatesByCARequestListCertificatesByCAPaginateTypeDef(
+    _RequiredListCertificatesByCARequestListCertificatesByCAPaginateTypeDef,
+    _OptionalListCertificatesByCARequestListCertificatesByCAPaginateTypeDef,
+):
+    pass
+
+ListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
+    "ListCertificatesRequestListCertificatesPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCustomMetricsRequestListCustomMetricsPaginateTypeDef = TypedDict(
+    "ListCustomMetricsRequestListCustomMetricsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef = TypedDict(
+    "ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef",
+    {
+        "taskId": str,
+        "violationId": str,
+        "thingName": str,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef = TypedDict(
+    "_RequiredListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef = TypedDict(
+    "_OptionalListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef(
+    _RequiredListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef,
+    _OptionalListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef,
+):
+    pass
+
+ListDimensionsRequestListDimensionsPaginateTypeDef = TypedDict(
+    "ListDimensionsRequestListDimensionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef = TypedDict(
+    "ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef",
+    {
+        "serviceType": ServiceTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListFleetMetricsRequestListFleetMetricsPaginateTypeDef = TypedDict(
+    "ListFleetMetricsRequestListFleetMetricsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListIndicesRequestListIndicesPaginateTypeDef = TypedDict(
+    "ListIndicesRequestListIndicesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef = TypedDict(
+    "_RequiredListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef",
+    {
+        "jobId": str,
+    },
+)
+_OptionalListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef = TypedDict(
+    "_OptionalListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef",
+    {
+        "status": JobExecutionStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef(
+    _RequiredListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef,
+    _OptionalListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef,
+):
+    pass
+
+_RequiredListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef = TypedDict(
+    "_RequiredListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef",
+    {
+        "thingName": str,
+    },
+)
+_OptionalListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef = TypedDict(
+    "_OptionalListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef",
+    {
+        "status": JobExecutionStatusType,
+        "namespaceId": str,
+        "jobId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef(
+    _RequiredListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef,
+    _OptionalListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef,
+):
+    pass
+
+ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "ListJobsRequestListJobsPaginateTypeDef",
+    {
+        "status": JobStatusType,
+        "targetSelection": TargetSelectionType,
+        "thingGroupName": str,
+        "thingGroupId": str,
+        "namespaceId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef = TypedDict(
+    "ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef",
+    {
+        "templateName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListMetricValuesRequestListMetricValuesPaginateTypeDef = TypedDict(
+    "_RequiredListMetricValuesRequestListMetricValuesPaginateTypeDef",
+    {
+        "thingName": str,
+        "metricName": str,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListMetricValuesRequestListMetricValuesPaginateTypeDef = TypedDict(
+    "_OptionalListMetricValuesRequestListMetricValuesPaginateTypeDef",
+    {
+        "dimensionName": str,
+        "dimensionValueOperator": DimensionValueOperatorType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListMetricValuesRequestListMetricValuesPaginateTypeDef(
+    _RequiredListMetricValuesRequestListMetricValuesPaginateTypeDef,
+    _OptionalListMetricValuesRequestListMetricValuesPaginateTypeDef,
+):
+    pass
+
+ListMitigationActionsRequestListMitigationActionsPaginateTypeDef = TypedDict(
+    "ListMitigationActionsRequestListMitigationActionsPaginateTypeDef",
+    {
+        "actionType": MitigationActionTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef = TypedDict(
+    "ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef",
+    {
+        "otaUpdateStatus": OTAUpdateStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef = TypedDict(
+    "ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
+    {
+        "packageName": str,
+    },
+)
+_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
+    {
+        "status": PackageVersionStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPackageVersionsRequestListPackageVersionsPaginateTypeDef(
+    _RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+    _OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+):
+    pass
+
+ListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
+    "ListPackagesRequestListPackagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPoliciesRequestListPoliciesPaginateTypeDef = TypedDict(
+    "ListPoliciesRequestListPoliciesPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef = TypedDict(
+    "_RequiredListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef",
+    {
+        "policyName": str,
+    },
+)
+_OptionalListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef = TypedDict(
+    "_OptionalListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef(
+    _RequiredListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef,
+    _OptionalListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef,
+):
+    pass
+
+_RequiredListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef",
+    {
+        "principal": str,
+    },
+)
+_OptionalListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef(
+    _RequiredListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef,
+    _OptionalListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef,
+):
+    pass
+
+_RequiredListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef = TypedDict(
+    "_RequiredListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef",
+    {
+        "principal": str,
+    },
+)
+_OptionalListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef = TypedDict(
+    "_OptionalListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef(
+    _RequiredListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef,
+    _OptionalListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef,
+):
+    pass
+
+_RequiredListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef",
+    {
+        "templateName": str,
+    },
+)
+_OptionalListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef(
+    _RequiredListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef,
+    _OptionalListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef,
+):
+    pass
+
+ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef = TypedDict(
+    "ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef = TypedDict(
+    "_RequiredListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef",
+    {
+        "findingId": str,
+    },
+)
+_OptionalListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef = TypedDict(
+    "_OptionalListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef(
+    _RequiredListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef,
+    _OptionalListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef,
+):
+    pass
+
+ListRoleAliasesRequestListRoleAliasesPaginateTypeDef = TypedDict(
+    "ListRoleAliasesRequestListRoleAliasesPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef = TypedDict(
+    "ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef",
+        {
+            "securityProfileTargetArn": str,
+        },
+    )
+)
+_OptionalListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef",
+        {
+            "recursive": bool,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+class ListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef(
+    _RequiredListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef,
+    _OptionalListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef,
+):
+    pass
+
+ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef = TypedDict(
+    "ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef",
+    {
+        "dimensionName": str,
+        "metricName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListStreamsRequestListStreamsPaginateTypeDef = TypedDict(
+    "ListStreamsRequestListStreamsPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+_RequiredListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef = TypedDict(
+    "_RequiredListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef",
+    {
+        "policyName": str,
+    },
+)
+_OptionalListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef = TypedDict(
+    "_OptionalListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef(
+    _RequiredListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
+    _OptionalListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
+):
+    pass
+
+_RequiredListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef = (
+    TypedDict(
+        "_RequiredListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef",
+        {
+            "securityProfileName": str,
+        },
+    )
+)
+_OptionalListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef = (
+    TypedDict(
+        "_OptionalListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef",
+        {
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+class ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef(
+    _RequiredListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef,
+    _OptionalListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef,
+):
+    pass
+
+_RequiredListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef = TypedDict(
+    "_RequiredListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef",
+    {
+        "thingName": str,
+    },
+)
+_OptionalListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef = TypedDict(
+    "_OptionalListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef(
+    _RequiredListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef,
+    _OptionalListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef,
+):
+    pass
+
+ListThingGroupsRequestListThingGroupsPaginateTypeDef = TypedDict(
+    "ListThingGroupsRequestListThingGroupsPaginateTypeDef",
+    {
+        "parentGroup": str,
+        "namePrefixFilter": str,
+        "recursive": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef = TypedDict(
+    "_RequiredListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef",
+    {
+        "thingName": str,
+    },
+)
+_OptionalListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef = TypedDict(
+    "_OptionalListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef(
+    _RequiredListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef,
+    _OptionalListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef,
+):
+    pass
+
+_RequiredListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef = TypedDict(
+    "_RequiredListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef",
+    {
+        "taskId": str,
+        "reportType": ReportTypeType,
+    },
+)
+_OptionalListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef = TypedDict(
+    "_OptionalListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef(
+    _RequiredListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef,
+    _OptionalListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef,
+):
+    pass
+
+ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef = TypedDict(
+    "ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef",
+    {
+        "status": StatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListThingTypesRequestListThingTypesPaginateTypeDef = TypedDict(
+    "ListThingTypesRequestListThingTypesPaginateTypeDef",
+    {
+        "thingTypeName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef = TypedDict(
+    "_RequiredListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef",
+    {
+        "billingGroupName": str,
+    },
+)
+_OptionalListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef = TypedDict(
+    "_OptionalListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef(
+    _RequiredListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef,
+    _OptionalListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef,
+):
+    pass
+
+_RequiredListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef = TypedDict(
+    "_RequiredListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef",
+    {
+        "thingGroupName": str,
+    },
+)
+_OptionalListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef = TypedDict(
+    "_OptionalListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef",
+    {
+        "recursive": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef(
+    _RequiredListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef,
+    _OptionalListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef,
+):
+    pass
+
+ListThingsRequestListThingsPaginateTypeDef = TypedDict(
+    "ListThingsRequestListThingsPaginateTypeDef",
+    {
+        "attributeName": str,
+        "attributeValue": str,
+        "thingTypeName": str,
+        "usePrefixAttributeValue": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef = TypedDict(
+    "ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTopicRulesRequestListTopicRulesPaginateTypeDef = TypedDict(
+    "ListTopicRulesRequestListTopicRulesPaginateTypeDef",
+    {
+        "topic": str,
+        "ruleDisabled": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef = TypedDict(
+    "ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef",
+    {
+        "targetType": LogTargetTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListViolationEventsRequestListViolationEventsPaginateTypeDef = TypedDict(
+    "_RequiredListViolationEventsRequestListViolationEventsPaginateTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalListViolationEventsRequestListViolationEventsPaginateTypeDef = TypedDict(
+    "_OptionalListViolationEventsRequestListViolationEventsPaginateTypeDef",
+    {
+        "thingName": str,
+        "securityProfileName": str,
+        "behaviorCriteriaType": BehaviorCriteriaTypeType,
+        "listSuppressedAlerts": bool,
+        "verificationState": VerificationStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListViolationEventsRequestListViolationEventsPaginateTypeDef(
+    _RequiredListViolationEventsRequestListViolationEventsPaginateTypeDef,
+    _OptionalListViolationEventsRequestListViolationEventsPaginateTypeDef,
+):
+    pass
 
 GetPackageConfigurationResponseTypeDef = TypedDict(
     "GetPackageConfigurationResponseTypeDef",
     {
         "versionUpdateByJobsConfig": VersionUpdateByJobsConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePackageConfigurationRequestRequestTypeDef = TypedDict(
     "UpdatePackageConfigurationRequestRequestTypeDef",
     {
         "versionUpdateByJobsConfig": VersionUpdateByJobsConfigTypeDef,
@@ -7529,50 +7759,50 @@
     total=False,
 )
 
 GetPercentilesResponseTypeDef = TypedDict(
     "GetPercentilesResponseTypeDef",
     {
         "percentiles": List[PercentPairTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStatisticsResponseTypeDef = TypedDict(
     "GetStatisticsResponseTypeDef",
     {
         "statistics": StatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBillingGroupsResponseTypeDef = TypedDict(
     "ListBillingGroupsResponseTypeDef",
     {
         "billingGroups": List[GroupNameAndArnTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListThingGroupsForThingResponseTypeDef = TypedDict(
     "ListThingGroupsForThingResponseTypeDef",
     {
         "thingGroups": List[GroupNameAndArnTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListThingGroupsResponseTypeDef = TypedDict(
     "ListThingGroupsResponseTypeDef",
     {
         "thingGroups": List[GroupNameAndArnTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ThingGroupMetadataTypeDef = TypedDict(
     "ThingGroupMetadataTypeDef",
     {
         "parentGroupName": str,
@@ -7586,28 +7816,53 @@
     "HttpAuthorizationTypeDef",
     {
         "sigv4": SigV4AuthorizationTypeDef,
     },
     total=False,
 )
 
+_RequiredThingIndexingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredThingIndexingConfigurationOutputTypeDef",
+    {
+        "thingIndexingMode": ThingIndexingModeType,
+    },
+)
+_OptionalThingIndexingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalThingIndexingConfigurationOutputTypeDef",
+    {
+        "thingConnectivityIndexingMode": ThingConnectivityIndexingModeType,
+        "deviceDefenderIndexingMode": DeviceDefenderIndexingModeType,
+        "namedShadowIndexingMode": NamedShadowIndexingModeType,
+        "managedFields": List[FieldTypeDef],
+        "customFields": List[FieldTypeDef],
+        "filter": IndexingFilterOutputTypeDef,
+    },
+    total=False,
+)
+
+class ThingIndexingConfigurationOutputTypeDef(
+    _RequiredThingIndexingConfigurationOutputTypeDef,
+    _OptionalThingIndexingConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredThingIndexingConfigurationTypeDef = TypedDict(
     "_RequiredThingIndexingConfigurationTypeDef",
     {
         "thingIndexingMode": ThingIndexingModeType,
     },
 )
 _OptionalThingIndexingConfigurationTypeDef = TypedDict(
     "_OptionalThingIndexingConfigurationTypeDef",
     {
         "thingConnectivityIndexingMode": ThingConnectivityIndexingModeType,
         "deviceDefenderIndexingMode": DeviceDefenderIndexingModeType,
         "namedShadowIndexingMode": NamedShadowIndexingModeType,
-        "managedFields": List[FieldTypeDef],
-        "customFields": List[FieldTypeDef],
+        "managedFields": Sequence[FieldTypeDef],
+        "customFields": Sequence[FieldTypeDef],
         "filter": IndexingFilterTypeDef,
     },
     total=False,
 )
 
 class ThingIndexingConfigurationTypeDef(
     _RequiredThingIndexingConfigurationTypeDef, _OptionalThingIndexingConfigurationTypeDef
@@ -7646,152 +7901,159 @@
     {
         "jobId": str,
         "jobExecutionSummary": JobExecutionSummaryTypeDef,
     },
     total=False,
 )
 
+JobExecutionsRetryConfigOutputTypeDef = TypedDict(
+    "JobExecutionsRetryConfigOutputTypeDef",
+    {
+        "criteriaList": List[RetryCriteriaTypeDef],
+    },
+)
+
 JobExecutionsRetryConfigTypeDef = TypedDict(
     "JobExecutionsRetryConfigTypeDef",
     {
         "criteriaList": Sequence[RetryCriteriaTypeDef],
     },
 )
 
 ListJobsResponseTypeDef = TypedDict(
     "ListJobsResponseTypeDef",
     {
         "jobs": List[JobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobTemplatesResponseTypeDef = TypedDict(
     "ListJobTemplatesResponseTypeDef",
     {
         "jobTemplates": List[JobTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListManagedJobTemplatesResponseTypeDef = TypedDict(
     "ListManagedJobTemplatesResponseTypeDef",
     {
         "managedJobTemplates": List[ManagedJobTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMitigationActionsResponseTypeDef = TypedDict(
     "ListMitigationActionsResponseTypeDef",
     {
         "actionIdentifiers": List[MitigationActionIdentifierTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOTAUpdatesResponseTypeDef = TypedDict(
     "ListOTAUpdatesResponseTypeDef",
     {
         "otaUpdates": List[OTAUpdateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOutgoingCertificatesResponseTypeDef = TypedDict(
     "ListOutgoingCertificatesResponseTypeDef",
     {
         "outgoingCertificates": List[OutgoingCertificateTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPackageVersionsResponseTypeDef = TypedDict(
     "ListPackageVersionsResponseTypeDef",
     {
         "packageVersionSummaries": List[PackageVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPackagesResponseTypeDef = TypedDict(
     "ListPackagesResponseTypeDef",
     {
         "packageSummaries": List[PackageSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPolicyVersionsResponseTypeDef = TypedDict(
     "ListPolicyVersionsResponseTypeDef",
     {
         "policyVersions": List[PolicyVersionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProvisioningTemplateVersionsResponseTypeDef = TypedDict(
     "ListProvisioningTemplateVersionsResponseTypeDef",
     {
         "versions": List[ProvisioningTemplateVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProvisioningTemplatesResponseTypeDef = TypedDict(
     "ListProvisioningTemplatesResponseTypeDef",
     {
         "templates": List[ProvisioningTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListScheduledAuditsResponseTypeDef = TypedDict(
     "ListScheduledAuditsResponseTypeDef",
     {
         "scheduledAudits": List[ScheduledAuditMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSecurityProfilesResponseTypeDef = TypedDict(
     "ListSecurityProfilesResponseTypeDef",
     {
         "securityProfileIdentifiers": List[SecurityProfileIdentifierTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamsResponseTypeDef = TypedDict(
     "ListStreamsResponseTypeDef",
     {
         "streams": List[StreamSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTargetsForSecurityProfileResponseTypeDef = TypedDict(
     "ListTargetsForSecurityProfileResponseTypeDef",
     {
         "securityProfileTargets": List[SecurityProfileTargetTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SecurityProfileTargetMappingTypeDef = TypedDict(
     "SecurityProfileTargetMappingTypeDef",
     {
         "securityProfileIdentifier": SecurityProfileIdentifierTypeDef,
@@ -7801,24 +8063,24 @@
 )
 
 ListThingsResponseTypeDef = TypedDict(
     "ListThingsResponseTypeDef",
     {
         "things": List[ThingAttributeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTopicRulesResponseTypeDef = TypedDict(
     "ListTopicRulesResponseTypeDef",
     {
         "rules": List[TopicRuleListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredLocationActionTypeDef = TypedDict(
     "_RequiredLocationActionTypeDef",
     {
         "roleArn": str,
@@ -7859,27 +8121,53 @@
 SetLoggingOptionsRequestRequestTypeDef = TypedDict(
     "SetLoggingOptionsRequestRequestTypeDef",
     {
         "loggingOptionsPayload": LoggingOptionsPayloadTypeDef,
     },
 )
 
+MitigationActionParamsOutputTypeDef = TypedDict(
+    "MitigationActionParamsOutputTypeDef",
+    {
+        "updateDeviceCertificateParams": UpdateDeviceCertificateParamsTypeDef,
+        "updateCACertificateParams": UpdateCACertificateParamsTypeDef,
+        "addThingsToThingGroupParams": AddThingsToThingGroupParamsOutputTypeDef,
+        "replaceDefaultPolicyVersionParams": ReplaceDefaultPolicyVersionParamsTypeDef,
+        "enableIoTLoggingParams": EnableIoTLoggingParamsTypeDef,
+        "publishFindingToSnsParams": PublishFindingToSnsParamsTypeDef,
+    },
+    total=False,
+)
+
 MitigationActionParamsTypeDef = TypedDict(
     "MitigationActionParamsTypeDef",
     {
         "updateDeviceCertificateParams": UpdateDeviceCertificateParamsTypeDef,
         "updateCACertificateParams": UpdateCACertificateParamsTypeDef,
         "addThingsToThingGroupParams": AddThingsToThingGroupParamsTypeDef,
         "replaceDefaultPolicyVersionParams": ReplaceDefaultPolicyVersionParamsTypeDef,
         "enableIoTLoggingParams": EnableIoTLoggingParamsTypeDef,
         "publishFindingToSnsParams": PublishFindingToSnsParamsTypeDef,
     },
     total=False,
 )
 
+MqttHeadersOutputTypeDef = TypedDict(
+    "MqttHeadersOutputTypeDef",
+    {
+        "payloadFormatIndicator": str,
+        "contentType": str,
+        "responseTopic": str,
+        "correlationData": str,
+        "messageExpiry": str,
+        "userProperties": List[UserPropertyTypeDef],
+    },
+    total=False,
+)
+
 MqttHeadersTypeDef = TypedDict(
     "MqttHeadersTypeDef",
     {
         "payloadFormatIndicator": str,
         "contentType": str,
         "responseTopic": str,
         "correlationData": str,
@@ -7902,38 +8190,14 @@
         "roleAliasArn": str,
         "issuerCertificateIdentifier": IssuerCertificateIdentifierTypeDef,
         "deviceCertificateArn": str,
     },
     total=False,
 )
 
-_RequiredTestInvokeAuthorizerRequestRequestTypeDef = TypedDict(
-    "_RequiredTestInvokeAuthorizerRequestRequestTypeDef",
-    {
-        "authorizerName": str,
-    },
-)
-_OptionalTestInvokeAuthorizerRequestRequestTypeDef = TypedDict(
-    "_OptionalTestInvokeAuthorizerRequestRequestTypeDef",
-    {
-        "token": str,
-        "tokenSignature": str,
-        "httpContext": HttpContextTypeDef,
-        "mqttContext": MqttContextTypeDef,
-        "tlsContext": TlsContextTypeDef,
-    },
-    total=False,
-)
-
-class TestInvokeAuthorizerRequestRequestTypeDef(
-    _RequiredTestInvokeAuthorizerRequestRequestTypeDef,
-    _OptionalTestInvokeAuthorizerRequestRequestTypeDef,
-):
-    pass
-
 ThingDocumentTypeDef = TypedDict(
     "ThingDocumentTypeDef",
     {
         "thingName": str,
         "thingId": str,
         "thingTypeName": str,
         "thingGroupNames": List[str],
@@ -7941,14 +8205,36 @@
         "shadow": str,
         "deviceDefender": str,
         "connectivity": ThingConnectivityTypeDef,
     },
     total=False,
 )
 
+_RequiredTimestreamActionOutputTypeDef = TypedDict(
+    "_RequiredTimestreamActionOutputTypeDef",
+    {
+        "roleArn": str,
+        "databaseName": str,
+        "tableName": str,
+        "dimensions": List[TimestreamDimensionTypeDef],
+    },
+)
+_OptionalTimestreamActionOutputTypeDef = TypedDict(
+    "_OptionalTimestreamActionOutputTypeDef",
+    {
+        "timestamp": TimestreamTimestampTypeDef,
+    },
+    total=False,
+)
+
+class TimestreamActionOutputTypeDef(
+    _RequiredTimestreamActionOutputTypeDef, _OptionalTimestreamActionOutputTypeDef
+):
+    pass
+
 _RequiredTimestreamActionTypeDef = TypedDict(
     "_RequiredTimestreamActionTypeDef",
     {
         "roleArn": str,
         "databaseName": str,
         "tableName": str,
         "dimensions": Sequence[TimestreamDimensionTypeDef],
@@ -8003,36 +8289,60 @@
 )
 
 ValidateSecurityProfileBehaviorsResponseTypeDef = TypedDict(
     "ValidateSecurityProfileBehaviorsResponseTypeDef",
     {
         "valid": bool,
         "validationErrors": List[ValidationErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AbortConfigUnionTypeDef = Union[AbortConfigTypeDef, AbortConfigOutputTypeDef]
 ListMetricValuesResponseTypeDef = TypedDict(
     "ListMetricValuesResponseTypeDef",
     {
         "metricDatumList": List[MetricDatumTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeniedTypeDef = TypedDict(
     "DeniedTypeDef",
     {
         "implicitDeny": ImplicitDenyTypeDef,
         "explicitDeny": ExplicitDenyTypeDef,
     },
     total=False,
 )
 
+_RequiredPutAssetPropertyValueEntryOutputTypeDef = TypedDict(
+    "_RequiredPutAssetPropertyValueEntryOutputTypeDef",
+    {
+        "propertyValues": List[AssetPropertyValueTypeDef],
+    },
+)
+_OptionalPutAssetPropertyValueEntryOutputTypeDef = TypedDict(
+    "_OptionalPutAssetPropertyValueEntryOutputTypeDef",
+    {
+        "entryId": str,
+        "assetId": str,
+        "propertyId": str,
+        "propertyAlias": str,
+    },
+    total=False,
+)
+
+class PutAssetPropertyValueEntryOutputTypeDef(
+    _RequiredPutAssetPropertyValueEntryOutputTypeDef,
+    _OptionalPutAssetPropertyValueEntryOutputTypeDef,
+):
+    pass
+
 _RequiredPutAssetPropertyValueEntryTypeDef = TypedDict(
     "_RequiredPutAssetPropertyValueEntryTypeDef",
     {
         "propertyValues": Sequence[AssetPropertyValueTypeDef],
     },
 )
 _OptionalPutAssetPropertyValueEntryTypeDef = TypedDict(
@@ -8092,14 +8402,17 @@
 )
 
 class CreateThingGroupRequestRequestTypeDef(
     _RequiredCreateThingGroupRequestRequestTypeDef, _OptionalCreateThingGroupRequestRequestTypeDef
 ):
     pass
 
+ThingGroupPropertiesUnionTypeDef = Union[
+    ThingGroupPropertiesTypeDef, ThingGroupPropertiesOutputTypeDef
+]
 _RequiredUpdateDynamicThingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDynamicThingGroupRequestRequestTypeDef",
     {
         "thingGroupName": str,
         "thingGroupProperties": ThingGroupPropertiesTypeDef,
     },
 )
@@ -8136,23 +8449,66 @@
 )
 
 class UpdateThingGroupRequestRequestTypeDef(
     _RequiredUpdateThingGroupRequestRequestTypeDef, _OptionalUpdateThingGroupRequestRequestTypeDef
 ):
     pass
 
+_RequiredTestAuthorizationRequestRequestTypeDef = TypedDict(
+    "_RequiredTestAuthorizationRequestRequestTypeDef",
+    {
+        "authInfos": Sequence[AuthInfoUnionTypeDef],
+    },
+)
+_OptionalTestAuthorizationRequestRequestTypeDef = TypedDict(
+    "_OptionalTestAuthorizationRequestRequestTypeDef",
+    {
+        "principal": str,
+        "cognitoIdentityPoolId": str,
+        "clientId": str,
+        "policyNamesToAdd": Sequence[str],
+        "policyNamesToSkip": Sequence[str],
+    },
+    total=False,
+)
+
+class TestAuthorizationRequestRequestTypeDef(
+    _RequiredTestAuthorizationRequestRequestTypeDef, _OptionalTestAuthorizationRequestRequestTypeDef
+):
+    pass
+
 AwsJobExecutionsRolloutConfigTypeDef = TypedDict(
     "AwsJobExecutionsRolloutConfigTypeDef",
     {
         "maximumPerMinute": int,
         "exponentialRate": AwsJobExponentialRolloutRateTypeDef,
     },
     total=False,
 )
 
+_RequiredBehaviorOutputTypeDef = TypedDict(
+    "_RequiredBehaviorOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalBehaviorOutputTypeDef = TypedDict(
+    "_OptionalBehaviorOutputTypeDef",
+    {
+        "metric": str,
+        "metricDimension": MetricDimensionTypeDef,
+        "criteria": BehaviorCriteriaOutputTypeDef,
+        "suppressAlerts": bool,
+    },
+    total=False,
+)
+
+class BehaviorOutputTypeDef(_RequiredBehaviorOutputTypeDef, _OptionalBehaviorOutputTypeDef):
+    pass
+
 _RequiredBehaviorTypeDef = TypedDict(
     "_RequiredBehaviorTypeDef",
     {
         "name": str,
     },
 )
 _OptionalBehaviorTypeDef = TypedDict(
@@ -8165,14 +8521,49 @@
     },
     total=False,
 )
 
 class BehaviorTypeDef(_RequiredBehaviorTypeDef, _OptionalBehaviorTypeDef):
     pass
 
+CustomCodeSigningTypeDef = TypedDict(
+    "CustomCodeSigningTypeDef",
+    {
+        "signature": CodeSigningSignatureTypeDef,
+        "certificateChain": CodeSigningCertificateChainTypeDef,
+        "hashAlgorithm": str,
+        "signatureAlgorithm": str,
+    },
+    total=False,
+)
+
+_RequiredTestInvokeAuthorizerRequestRequestTypeDef = TypedDict(
+    "_RequiredTestInvokeAuthorizerRequestRequestTypeDef",
+    {
+        "authorizerName": str,
+    },
+)
+_OptionalTestInvokeAuthorizerRequestRequestTypeDef = TypedDict(
+    "_OptionalTestInvokeAuthorizerRequestRequestTypeDef",
+    {
+        "token": str,
+        "tokenSignature": str,
+        "httpContext": HttpContextTypeDef,
+        "mqttContext": MqttContextTypeDef,
+        "tlsContext": TlsContextTypeDef,
+    },
+    total=False,
+)
+
+class TestInvokeAuthorizerRequestRequestTypeDef(
+    _RequiredTestInvokeAuthorizerRequestRequestTypeDef,
+    _OptionalTestInvokeAuthorizerRequestRequestTypeDef,
+):
+    pass
+
 _RequiredGetBucketsAggregationRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketsAggregationRequestRequestTypeDef",
     {
         "queryString": str,
         "aggregationField": str,
         "bucketsAggregationType": BucketsAggregationTypeTypeDef,
     },
@@ -8193,32 +8584,61 @@
     pass
 
 DescribeCACertificateResponseTypeDef = TypedDict(
     "DescribeCACertificateResponseTypeDef",
     {
         "certificateDescription": CACertificateDescriptionTypeDef,
         "registrationConfig": RegistrationConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCertificateResponseTypeDef = TypedDict(
     "DescribeCertificateResponseTypeDef",
     {
         "certificateDescription": CertificateDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
+    "_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef",
+    {
+        "taskId": str,
+        "target": DetectMitigationActionsTaskTargetTypeDef,
+        "actions": Sequence[str],
+        "clientRequestToken": str,
+    },
+)
+_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
+    "_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef",
+    {
+        "violationEventOccurrenceRange": ViolationEventOccurrenceRangeTypeDef,
+        "includeOnlyActiveViolations": bool,
+        "includeSuppressedAlerts": bool,
     },
+    total=False,
 )
 
+class StartDetectMitigationActionsTaskRequestRequestTypeDef(
+    _RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef,
+    _OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef,
+):
+    pass
+
+ViolationEventOccurrenceRangeUnionTypeDef = Union[
+    ViolationEventOccurrenceRangeTypeDef, ViolationEventOccurrenceRangeOutputTypeDef
+]
+SchedulingConfigUnionTypeDef = Union[SchedulingConfigTypeDef, SchedulingConfigOutputTypeDef]
 ListThingTypesResponseTypeDef = TypedDict(
     "ListThingTypesResponseTypeDef",
     {
         "thingTypes": List[ThingTypeDefinitionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartSigningJobParameterTypeDef = TypedDict(
     "StartSigningJobParameterTypeDef",
     {
         "signingProfileParameter": SigningProfileParameterTypeDef,
@@ -8233,14 +8653,17 @@
     {
         "maximumPerMinute": int,
         "exponentialRate": ExponentialRolloutRateTypeDef,
     },
     total=False,
 )
 
+ThingGroupIndexingConfigurationUnionTypeDef = Union[
+    ThingGroupIndexingConfigurationTypeDef, ThingGroupIndexingConfigurationOutputTypeDef
+]
 _RequiredCreateStreamRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStreamRequestRequestTypeDef",
     {
         "streamId": str,
         "files": Sequence[StreamFileTypeDef],
         "roleArn": str,
     },
@@ -8298,24 +8721,43 @@
 DescribeThingGroupResponseTypeDef = TypedDict(
     "DescribeThingGroupResponseTypeDef",
     {
         "thingGroupName": str,
         "thingGroupId": str,
         "thingGroupArn": str,
         "version": int,
-        "thingGroupProperties": ThingGroupPropertiesTypeDef,
+        "thingGroupProperties": ThingGroupPropertiesOutputTypeDef,
         "thingGroupMetadata": ThingGroupMetadataTypeDef,
         "indexName": str,
         "queryString": str,
         "queryVersion": str,
         "status": DynamicGroupStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredHttpActionOutputTypeDef = TypedDict(
+    "_RequiredHttpActionOutputTypeDef",
+    {
+        "url": str,
+    },
+)
+_OptionalHttpActionOutputTypeDef = TypedDict(
+    "_OptionalHttpActionOutputTypeDef",
+    {
+        "confirmationUrl": str,
+        "headers": List[HttpActionHeaderTypeDef],
+        "auth": HttpAuthorizationTypeDef,
+    },
+    total=False,
+)
+
+class HttpActionOutputTypeDef(_RequiredHttpActionOutputTypeDef, _OptionalHttpActionOutputTypeDef):
+    pass
+
 _RequiredHttpActionTypeDef = TypedDict(
     "_RequiredHttpActionTypeDef",
     {
         "url": str,
     },
 )
 _OptionalHttpActionTypeDef = TypedDict(
@@ -8330,121 +8772,130 @@
 
 class HttpActionTypeDef(_RequiredHttpActionTypeDef, _OptionalHttpActionTypeDef):
     pass
 
 GetIndexingConfigurationResponseTypeDef = TypedDict(
     "GetIndexingConfigurationResponseTypeDef",
     {
-        "thingIndexingConfiguration": ThingIndexingConfigurationTypeDef,
-        "thingGroupIndexingConfiguration": ThingGroupIndexingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "thingIndexingConfiguration": ThingIndexingConfigurationOutputTypeDef,
+        "thingGroupIndexingConfiguration": ThingGroupIndexingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ThingIndexingConfigurationUnionTypeDef = Union[
+    ThingIndexingConfigurationTypeDef, ThingIndexingConfigurationOutputTypeDef
+]
 UpdateIndexingConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateIndexingConfigurationRequestRequestTypeDef",
     {
         "thingIndexingConfiguration": ThingIndexingConfigurationTypeDef,
         "thingGroupIndexingConfiguration": ThingGroupIndexingConfigurationTypeDef,
     },
     total=False,
 )
 
 DescribeJobExecutionResponseTypeDef = TypedDict(
     "DescribeJobExecutionResponseTypeDef",
     {
         "execution": JobExecutionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobExecutionsForJobResponseTypeDef = TypedDict(
     "ListJobExecutionsForJobResponseTypeDef",
     {
         "executionSummaries": List[JobExecutionSummaryForJobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobExecutionsForThingResponseTypeDef = TypedDict(
     "ListJobExecutionsForThingResponseTypeDef",
     {
         "executionSummaries": List[JobExecutionSummaryForThingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+JobExecutionsRetryConfigUnionTypeDef = Union[
+    JobExecutionsRetryConfigTypeDef, JobExecutionsRetryConfigOutputTypeDef
+]
 ListSecurityProfilesForTargetResponseTypeDef = TypedDict(
     "ListSecurityProfilesForTargetResponseTypeDef",
     {
         "securityProfileTargetMappings": List[SecurityProfileTargetMappingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListV2LoggingLevelsResponseTypeDef = TypedDict(
     "ListV2LoggingLevelsResponseTypeDef",
     {
         "logTargetConfigurations": List[LogTargetConfigurationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateMitigationActionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateMitigationActionRequestRequestTypeDef",
-    {
-        "actionName": str,
-        "roleArn": str,
-        "actionParams": MitigationActionParamsTypeDef,
-    },
-)
-_OptionalCreateMitigationActionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateMitigationActionRequestRequestTypeDef",
-    {
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateMitigationActionRequestRequestTypeDef(
-    _RequiredCreateMitigationActionRequestRequestTypeDef,
-    _OptionalCreateMitigationActionRequestRequestTypeDef,
-):
-    pass
-
 DescribeMitigationActionResponseTypeDef = TypedDict(
     "DescribeMitigationActionResponseTypeDef",
     {
         "actionName": str,
         "actionType": MitigationActionTypeType,
         "actionArn": str,
         "actionId": str,
         "roleArn": str,
-        "actionParams": MitigationActionParamsTypeDef,
+        "actionParams": MitigationActionParamsOutputTypeDef,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MitigationActionTypeDef = TypedDict(
     "MitigationActionTypeDef",
     {
         "name": str,
         "id": str,
         "roleArn": str,
+        "actionParams": MitigationActionParamsOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredCreateMitigationActionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateMitigationActionRequestRequestTypeDef",
+    {
+        "actionName": str,
+        "roleArn": str,
         "actionParams": MitigationActionParamsTypeDef,
     },
+)
+_OptionalCreateMitigationActionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateMitigationActionRequestRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
     total=False,
 )
 
+class CreateMitigationActionRequestRequestTypeDef(
+    _RequiredCreateMitigationActionRequestRequestTypeDef,
+    _OptionalCreateMitigationActionRequestRequestTypeDef,
+):
+    pass
+
+MitigationActionParamsUnionTypeDef = Union[
+    MitigationActionParamsTypeDef, MitigationActionParamsOutputTypeDef
+]
 _RequiredUpdateMitigationActionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMitigationActionRequestRequestTypeDef",
     {
         "actionName": str,
     },
 )
 _OptionalUpdateMitigationActionRequestRequestTypeDef = TypedDict(
@@ -8458,14 +8909,35 @@
 
 class UpdateMitigationActionRequestRequestTypeDef(
     _RequiredUpdateMitigationActionRequestRequestTypeDef,
     _OptionalUpdateMitigationActionRequestRequestTypeDef,
 ):
     pass
 
+_RequiredRepublishActionOutputTypeDef = TypedDict(
+    "_RequiredRepublishActionOutputTypeDef",
+    {
+        "roleArn": str,
+        "topic": str,
+    },
+)
+_OptionalRepublishActionOutputTypeDef = TypedDict(
+    "_OptionalRepublishActionOutputTypeDef",
+    {
+        "qos": int,
+        "headers": MqttHeadersOutputTypeDef,
+    },
+    total=False,
+)
+
+class RepublishActionOutputTypeDef(
+    _RequiredRepublishActionOutputTypeDef, _OptionalRepublishActionOutputTypeDef
+):
+    pass
+
 _RequiredRepublishActionTypeDef = TypedDict(
     "_RequiredRepublishActionTypeDef",
     {
         "roleArn": str,
         "topic": str,
     },
 )
@@ -8508,15 +8980,15 @@
         "resourceIdentifier": ResourceIdentifierTypeDef,
         "clientRequestToken": str,
     },
 )
 _OptionalCreateAuditSuppressionRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAuditSuppressionRequestRequestTypeDef",
     {
-        "expirationDate": Union[datetime, str],
+        "expirationDate": TimestampTypeDef,
         "suppressIndefinitely": bool,
         "description": str,
     },
     total=False,
 )
 
 class CreateAuditSuppressionRequestRequestTypeDef(
@@ -8545,54 +9017,54 @@
     "DescribeAuditSuppressionResponseTypeDef",
     {
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
         "expirationDate": datetime,
         "suppressIndefinitely": bool,
         "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAuditFindingsRequestListAuditFindingsPaginateTypeDef = TypedDict(
     "ListAuditFindingsRequestListAuditFindingsPaginateTypeDef",
     {
         "taskId": str,
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
         "listSuppressedFindings": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListAuditFindingsRequestRequestTypeDef = TypedDict(
     "ListAuditFindingsRequestRequestTypeDef",
     {
         "taskId": str,
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
         "maxResults": int,
         "nextToken": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
         "listSuppressedFindings": bool,
     },
     total=False,
 )
 
 ListAuditSuppressionsRequestListAuditSuppressionsPaginateTypeDef = TypedDict(
     "ListAuditSuppressionsRequestListAuditSuppressionsPaginateTypeDef",
     {
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
         "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListAuditSuppressionsRequestRequestTypeDef = TypedDict(
     "ListAuditSuppressionsRequestRequestTypeDef",
     {
@@ -8631,15 +9103,15 @@
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
     },
 )
 _OptionalUpdateAuditSuppressionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateAuditSuppressionRequestRequestTypeDef",
     {
-        "expirationDate": Union[datetime, str],
+        "expirationDate": TimestampTypeDef,
         "suppressIndefinitely": bool,
         "description": str,
     },
     total=False,
 )
 
 class UpdateAuditSuppressionRequestRequestTypeDef(
@@ -8650,15 +9122,15 @@
 
 SearchIndexResponseTypeDef = TypedDict(
     "SearchIndexResponseTypeDef",
     {
         "nextToken": str,
         "things": List[ThingDocumentTypeDef],
         "thingGroups": List[ThingGroupDocumentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTopicRuleDestinationRequestRequestTypeDef = TypedDict(
     "CreateTopicRuleDestinationRequestRequestTypeDef",
     {
         "destinationConfiguration": TopicRuleDestinationConfigurationTypeDef,
@@ -8666,182 +9138,141 @@
 )
 
 ListTopicRuleDestinationsResponseTypeDef = TypedDict(
     "ListTopicRuleDestinationsResponseTypeDef",
     {
         "destinationSummaries": List[TopicRuleDestinationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTopicRuleDestinationResponseTypeDef = TypedDict(
     "CreateTopicRuleDestinationResponseTypeDef",
     {
         "topicRuleDestination": TopicRuleDestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTopicRuleDestinationResponseTypeDef = TypedDict(
     "GetTopicRuleDestinationResponseTypeDef",
     {
         "topicRuleDestination": TopicRuleDestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AuthResultTypeDef = TypedDict(
     "AuthResultTypeDef",
     {
-        "authInfo": AuthInfoTypeDef,
+        "authInfo": AuthInfoOutputTypeDef,
         "allowed": AllowedTypeDef,
         "denied": DeniedTypeDef,
         "authDecision": AuthDecisionType,
         "missingContextValues": List[str],
     },
     total=False,
 )
 
+IotSiteWiseActionOutputTypeDef = TypedDict(
+    "IotSiteWiseActionOutputTypeDef",
+    {
+        "putAssetPropertyValueEntries": List[PutAssetPropertyValueEntryOutputTypeDef],
+        "roleArn": str,
+    },
+)
+
 IotSiteWiseActionTypeDef = TypedDict(
     "IotSiteWiseActionTypeDef",
     {
         "putAssetPropertyValueEntries": Sequence[PutAssetPropertyValueEntryTypeDef],
         "roleArn": str,
     },
 )
 
 ActiveViolationTypeDef = TypedDict(
     "ActiveViolationTypeDef",
     {
         "violationId": str,
         "thingName": str,
         "securityProfileName": str,
-        "behavior": BehaviorTypeDef,
-        "lastViolationValue": MetricValueTypeDef,
+        "behavior": BehaviorOutputTypeDef,
+        "lastViolationValue": MetricValueOutputTypeDef,
         "violationEventAdditionalInfo": ViolationEventAdditionalInfoTypeDef,
         "verificationState": VerificationStateType,
         "verificationStateDescription": str,
         "lastViolationTime": datetime,
         "violationStartTime": datetime,
     },
     total=False,
 )
 
-_RequiredCreateSecurityProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSecurityProfileRequestRequestTypeDef",
-    {
-        "securityProfileName": str,
-    },
-)
-_OptionalCreateSecurityProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSecurityProfileRequestRequestTypeDef",
-    {
-        "securityProfileDescription": str,
-        "behaviors": Sequence[BehaviorTypeDef],
-        "alertTargets": Mapping[Literal["SNS"], AlertTargetTypeDef],
-        "additionalMetricsToRetain": Sequence[str],
-        "additionalMetricsToRetainV2": Sequence[MetricToRetainTypeDef],
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateSecurityProfileRequestRequestTypeDef(
-    _RequiredCreateSecurityProfileRequestRequestTypeDef,
-    _OptionalCreateSecurityProfileRequestRequestTypeDef,
-):
-    pass
-
 DescribeSecurityProfileResponseTypeDef = TypedDict(
     "DescribeSecurityProfileResponseTypeDef",
     {
         "securityProfileName": str,
         "securityProfileArn": str,
         "securityProfileDescription": str,
-        "behaviors": List[BehaviorTypeDef],
+        "behaviors": List[BehaviorOutputTypeDef],
         "alertTargets": Dict[Literal["SNS"], AlertTargetTypeDef],
         "additionalMetricsToRetain": List[str],
         "additionalMetricsToRetainV2": List[MetricToRetainTypeDef],
         "version": int,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSecurityProfileRequestRequestTypeDef",
-    {
-        "securityProfileName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSecurityProfileRequestRequestTypeDef",
-    {
-        "securityProfileDescription": str,
-        "behaviors": Sequence[BehaviorTypeDef],
-        "alertTargets": Mapping[Literal["SNS"], AlertTargetTypeDef],
-        "additionalMetricsToRetain": Sequence[str],
-        "additionalMetricsToRetainV2": Sequence[MetricToRetainTypeDef],
-        "deleteBehaviors": bool,
-        "deleteAlertTargets": bool,
-        "deleteAdditionalMetricsToRetain": bool,
-        "expectedVersion": int,
-    },
-    total=False,
-)
-
-class UpdateSecurityProfileRequestRequestTypeDef(
-    _RequiredUpdateSecurityProfileRequestRequestTypeDef,
-    _OptionalUpdateSecurityProfileRequestRequestTypeDef,
-):
-    pass
 
 UpdateSecurityProfileResponseTypeDef = TypedDict(
     "UpdateSecurityProfileResponseTypeDef",
     {
         "securityProfileName": str,
         "securityProfileArn": str,
         "securityProfileDescription": str,
-        "behaviors": List[BehaviorTypeDef],
+        "behaviors": List[BehaviorOutputTypeDef],
         "alertTargets": Dict[Literal["SNS"], AlertTargetTypeDef],
         "additionalMetricsToRetain": List[str],
         "additionalMetricsToRetainV2": List[MetricToRetainTypeDef],
         "version": int,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ValidateSecurityProfileBehaviorsRequestRequestTypeDef = TypedDict(
-    "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
-    {
-        "behaviors": Sequence[BehaviorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ViolationEventTypeDef = TypedDict(
     "ViolationEventTypeDef",
     {
         "violationId": str,
         "thingName": str,
         "securityProfileName": str,
-        "behavior": BehaviorTypeDef,
-        "metricValue": MetricValueTypeDef,
+        "behavior": BehaviorOutputTypeDef,
+        "metricValue": MetricValueOutputTypeDef,
         "violationEventAdditionalInfo": ViolationEventAdditionalInfoTypeDef,
         "violationEventType": ViolationEventTypeType,
         "verificationState": VerificationStateType,
         "verificationStateDescription": str,
         "violationEventTime": datetime,
     },
     total=False,
 )
 
+BehaviorUnionTypeDef = Union[BehaviorTypeDef, BehaviorOutputTypeDef]
+CodeSigningOutputTypeDef = TypedDict(
+    "CodeSigningOutputTypeDef",
+    {
+        "awsSignerJobId": str,
+        "startSigningJobParameter": StartSigningJobParameterTypeDef,
+        "customCodeSigning": CustomCodeSigningOutputTypeDef,
+    },
+    total=False,
+)
+
 CodeSigningTypeDef = TypedDict(
     "CodeSigningTypeDef",
     {
         "awsSignerJobId": str,
         "startSigningJobParameter": StartSigningJobParameterTypeDef,
         "customCodeSigning": CustomCodeSigningTypeDef,
     },
@@ -8919,20 +9350,20 @@
         "jobTemplateId": str,
         "description": str,
         "documentSource": str,
         "document": str,
         "createdAt": datetime,
         "presignedUrlConfig": PresignedUrlConfigTypeDef,
         "jobExecutionsRolloutConfig": JobExecutionsRolloutConfigTypeDef,
-        "abortConfig": AbortConfigTypeDef,
+        "abortConfig": AbortConfigOutputTypeDef,
         "timeoutConfig": TimeoutConfigTypeDef,
-        "jobExecutionsRetryConfig": JobExecutionsRetryConfigTypeDef,
+        "jobExecutionsRetryConfig": JobExecutionsRetryConfigOutputTypeDef,
         "maintenanceWindows": List[MaintenanceWindowTypeDef],
         "destinationPackageVersions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
         "jobArn": str,
@@ -8942,26 +9373,26 @@
         "forceCanceled": bool,
         "reasonCode": str,
         "comment": str,
         "targets": List[str],
         "description": str,
         "presignedUrlConfig": PresignedUrlConfigTypeDef,
         "jobExecutionsRolloutConfig": JobExecutionsRolloutConfigTypeDef,
-        "abortConfig": AbortConfigTypeDef,
+        "abortConfig": AbortConfigOutputTypeDef,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "completedAt": datetime,
         "jobProcessDetails": JobProcessDetailsTypeDef,
         "timeoutConfig": TimeoutConfigTypeDef,
         "namespaceId": str,
         "jobTemplateArn": str,
-        "jobExecutionsRetryConfig": JobExecutionsRetryConfigTypeDef,
+        "jobExecutionsRetryConfig": JobExecutionsRetryConfigOutputTypeDef,
         "documentParameters": Dict[str, str],
         "isConcurrent": bool,
-        "schedulingConfig": SchedulingConfigTypeDef,
+        "schedulingConfig": SchedulingConfigOutputTypeDef,
         "scheduledJobRollouts": List[ScheduledJobRolloutTypeDef],
         "destinationPackageVersions": List[str],
     },
     total=False,
 )
 
 _RequiredUpdateJobRequestRequestTypeDef = TypedDict(
@@ -8989,55 +9420,55 @@
 ):
     pass
 
 DescribeStreamResponseTypeDef = TypedDict(
     "DescribeStreamResponseTypeDef",
     {
         "streamInfo": StreamInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAuditMitigationActionsTaskResponseTypeDef = TypedDict(
     "DescribeAuditMitigationActionsTaskResponseTypeDef",
     {
         "taskStatus": AuditMitigationActionsTaskStatusType,
         "startTime": datetime,
         "endTime": datetime,
         "taskStatistics": Dict[str, TaskStatisticsForAuditCheckTypeDef],
-        "target": AuditMitigationActionsTaskTargetTypeDef,
+        "target": AuditMitigationActionsTaskTargetOutputTypeDef,
         "auditCheckToActionsMapping": Dict[str, List[str]],
         "actionsDefinition": List[MitigationActionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectMitigationActionsTaskSummaryTypeDef = TypedDict(
     "DetectMitigationActionsTaskSummaryTypeDef",
     {
         "taskId": str,
         "taskStatus": DetectMitigationActionsTaskStatusType,
         "taskStartTime": datetime,
         "taskEndTime": datetime,
-        "target": DetectMitigationActionsTaskTargetTypeDef,
-        "violationEventOccurrenceRange": ViolationEventOccurrenceRangeTypeDef,
+        "target": DetectMitigationActionsTaskTargetOutputTypeDef,
+        "violationEventOccurrenceRange": ViolationEventOccurrenceRangeOutputTypeDef,
         "onlyActiveViolationsIncluded": bool,
         "suppressedAlertsIncluded": bool,
         "actionsDefinition": List[MitigationActionTypeDef],
         "taskStatistics": DetectMitigationActionsTaskStatisticsTypeDef,
     },
     total=False,
 )
 
 ListAuditSuppressionsResponseTypeDef = TypedDict(
     "ListAuditSuppressionsResponseTypeDef",
     {
         "suppressions": List[AuditSuppressionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AuditFindingTypeDef = TypedDict(
     "AuditFindingTypeDef",
     {
         "findingId": str,
@@ -9056,26 +9487,56 @@
 )
 
 ListRelatedResourcesForAuditFindingResponseTypeDef = TypedDict(
     "ListRelatedResourcesForAuditFindingResponseTypeDef",
     {
         "relatedResources": List[RelatedResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestAuthorizationResponseTypeDef = TypedDict(
     "TestAuthorizationResponseTypeDef",
     {
         "authResults": List[AuthResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ActionOutputTypeDef = TypedDict(
+    "ActionOutputTypeDef",
+    {
+        "dynamoDB": DynamoDBActionTypeDef,
+        "dynamoDBv2": DynamoDBv2ActionTypeDef,
+        "lambda": LambdaActionTypeDef,
+        "sns": SnsActionTypeDef,
+        "sqs": SqsActionTypeDef,
+        "kinesis": KinesisActionTypeDef,
+        "republish": RepublishActionOutputTypeDef,
+        "s3": S3ActionTypeDef,
+        "firehose": FirehoseActionTypeDef,
+        "cloudwatchMetric": CloudwatchMetricActionTypeDef,
+        "cloudwatchAlarm": CloudwatchAlarmActionTypeDef,
+        "cloudwatchLogs": CloudwatchLogsActionTypeDef,
+        "elasticsearch": ElasticsearchActionTypeDef,
+        "salesforce": SalesforceActionTypeDef,
+        "iotAnalytics": IotAnalyticsActionTypeDef,
+        "iotEvents": IotEventsActionTypeDef,
+        "iotSiteWise": IotSiteWiseActionOutputTypeDef,
+        "stepFunctions": StepFunctionsActionTypeDef,
+        "timestream": TimestreamActionOutputTypeDef,
+        "http": HttpActionOutputTypeDef,
+        "kafka": KafkaActionOutputTypeDef,
+        "openSearch": OpenSearchActionTypeDef,
+        "location": LocationActionTypeDef,
+    },
+    total=False,
+)
+
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "dynamoDB": DynamoDBActionTypeDef,
         "dynamoDBv2": DynamoDBv2ActionTypeDef,
         "lambda": LambdaActionTypeDef,
         "sns": SnsActionTypeDef,
@@ -9103,27 +9564,100 @@
 )
 
 ListActiveViolationsResponseTypeDef = TypedDict(
     "ListActiveViolationsResponseTypeDef",
     {
         "activeViolations": List[ActiveViolationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListViolationEventsResponseTypeDef = TypedDict(
     "ListViolationEventsResponseTypeDef",
     {
         "violationEvents": List[ViolationEventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateSecurityProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSecurityProfileRequestRequestTypeDef",
+    {
+        "securityProfileName": str,
+    },
+)
+_OptionalCreateSecurityProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSecurityProfileRequestRequestTypeDef",
+    {
+        "securityProfileDescription": str,
+        "behaviors": Sequence[BehaviorUnionTypeDef],
+        "alertTargets": Mapping[Literal["SNS"], AlertTargetTypeDef],
+        "additionalMetricsToRetain": Sequence[str],
+        "additionalMetricsToRetainV2": Sequence[MetricToRetainTypeDef],
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateSecurityProfileRequestRequestTypeDef(
+    _RequiredCreateSecurityProfileRequestRequestTypeDef,
+    _OptionalCreateSecurityProfileRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSecurityProfileRequestRequestTypeDef",
+    {
+        "securityProfileName": str,
+    },
+)
+_OptionalUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSecurityProfileRequestRequestTypeDef",
+    {
+        "securityProfileDescription": str,
+        "behaviors": Sequence[BehaviorUnionTypeDef],
+        "alertTargets": Mapping[Literal["SNS"], AlertTargetTypeDef],
+        "additionalMetricsToRetain": Sequence[str],
+        "additionalMetricsToRetainV2": Sequence[MetricToRetainTypeDef],
+        "deleteBehaviors": bool,
+        "deleteAlertTargets": bool,
+        "deleteAdditionalMetricsToRetain": bool,
+        "expectedVersion": int,
+    },
+    total=False,
+)
+
+class UpdateSecurityProfileRequestRequestTypeDef(
+    _RequiredUpdateSecurityProfileRequestRequestTypeDef,
+    _OptionalUpdateSecurityProfileRequestRequestTypeDef,
+):
+    pass
+
+ValidateSecurityProfileBehaviorsRequestRequestTypeDef = TypedDict(
+    "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
+    {
+        "behaviors": Sequence[BehaviorUnionTypeDef],
     },
 )
 
+OTAUpdateFileOutputTypeDef = TypedDict(
+    "OTAUpdateFileOutputTypeDef",
+    {
+        "fileName": str,
+        "fileType": int,
+        "fileVersion": str,
+        "fileLocation": FileLocationTypeDef,
+        "codeSigning": CodeSigningOutputTypeDef,
+        "attributes": Dict[str, str],
+    },
+    total=False,
+)
+
 OTAUpdateFileTypeDef = TypedDict(
     "OTAUpdateFileTypeDef",
     {
         "fileName": str,
         "fileType": int,
         "fileVersion": str,
         "fileLocation": FileLocationTypeDef,
@@ -9134,116 +9668,86 @@
 )
 
 DescribeJobResponseTypeDef = TypedDict(
     "DescribeJobResponseTypeDef",
     {
         "documentSource": str,
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDetectMitigationActionsTaskResponseTypeDef = TypedDict(
     "DescribeDetectMitigationActionsTaskResponseTypeDef",
     {
         "taskSummary": DetectMitigationActionsTaskSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDetectMitigationActionsTasksResponseTypeDef = TypedDict(
     "ListDetectMitigationActionsTasksResponseTypeDef",
     {
         "tasks": List[DetectMitigationActionsTaskSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAuditFindingResponseTypeDef = TypedDict(
     "DescribeAuditFindingResponseTypeDef",
     {
         "finding": AuditFindingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAuditFindingsResponseTypeDef = TypedDict(
     "ListAuditFindingsResponseTypeDef",
     {
         "findings": List[AuditFindingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredTopicRulePayloadTypeDef = TypedDict(
-    "_RequiredTopicRulePayloadTypeDef",
-    {
-        "sql": str,
-        "actions": Sequence[ActionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalTopicRulePayloadTypeDef = TypedDict(
-    "_OptionalTopicRulePayloadTypeDef",
-    {
-        "description": str,
-        "ruleDisabled": bool,
-        "awsIotSqlVersion": str,
-        "errorAction": ActionTypeDef,
-    },
-    total=False,
-)
-
-class TopicRulePayloadTypeDef(_RequiredTopicRulePayloadTypeDef, _OptionalTopicRulePayloadTypeDef):
-    pass
 
 TopicRuleTypeDef = TypedDict(
     "TopicRuleTypeDef",
     {
         "ruleName": str,
         "sql": str,
         "description": str,
         "createdAt": datetime,
-        "actions": List[ActionTypeDef],
+        "actions": List[ActionOutputTypeDef],
         "ruleDisabled": bool,
         "awsIotSqlVersion": str,
-        "errorAction": ActionTypeDef,
+        "errorAction": ActionOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateOTAUpdateRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateOTAUpdateRequestRequestTypeDef",
+_RequiredTopicRulePayloadTypeDef = TypedDict(
+    "_RequiredTopicRulePayloadTypeDef",
     {
-        "otaUpdateId": str,
-        "targets": Sequence[str],
-        "files": Sequence[OTAUpdateFileTypeDef],
-        "roleArn": str,
+        "sql": str,
+        "actions": Sequence[ActionTypeDef],
     },
 )
-_OptionalCreateOTAUpdateRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateOTAUpdateRequestRequestTypeDef",
+_OptionalTopicRulePayloadTypeDef = TypedDict(
+    "_OptionalTopicRulePayloadTypeDef",
     {
         "description": str,
-        "protocols": Sequence[ProtocolType],
-        "targetSelection": TargetSelectionType,
-        "awsJobExecutionsRolloutConfig": AwsJobExecutionsRolloutConfigTypeDef,
-        "awsJobPresignedUrlConfig": AwsJobPresignedUrlConfigTypeDef,
-        "awsJobAbortConfig": AwsJobAbortConfigTypeDef,
-        "awsJobTimeoutConfig": AwsJobTimeoutConfigTypeDef,
-        "additionalParameters": Mapping[str, str],
-        "tags": Sequence[TagTypeDef],
+        "ruleDisabled": bool,
+        "awsIotSqlVersion": str,
+        "errorAction": ActionTypeDef,
     },
     total=False,
 )
 
-class CreateOTAUpdateRequestRequestTypeDef(
-    _RequiredCreateOTAUpdateRequestRequestTypeDef, _OptionalCreateOTAUpdateRequestRequestTypeDef
-):
+class TopicRulePayloadTypeDef(_RequiredTopicRulePayloadTypeDef, _OptionalTopicRulePayloadTypeDef):
     pass
 
 OTAUpdateInfoTypeDef = TypedDict(
     "OTAUpdateInfoTypeDef",
     {
         "otaUpdateId": str,
         "otaUpdateArn": str,
@@ -9251,24 +9755,34 @@
         "lastModifiedDate": datetime,
         "description": str,
         "targets": List[str],
         "protocols": List[ProtocolType],
         "awsJobExecutionsRolloutConfig": AwsJobExecutionsRolloutConfigTypeDef,
         "awsJobPresignedUrlConfig": AwsJobPresignedUrlConfigTypeDef,
         "targetSelection": TargetSelectionType,
-        "otaUpdateFiles": List[OTAUpdateFileTypeDef],
+        "otaUpdateFiles": List[OTAUpdateFileOutputTypeDef],
         "otaUpdateStatus": OTAUpdateStatusType,
         "awsIotJobId": str,
         "awsIotJobArn": str,
         "errorInfo": ErrorInfoTypeDef,
         "additionalParameters": Dict[str, str],
     },
     total=False,
 )
 
+OTAUpdateFileUnionTypeDef = Union[OTAUpdateFileTypeDef, OTAUpdateFileOutputTypeDef]
+GetTopicRuleResponseTypeDef = TypedDict(
+    "GetTopicRuleResponseTypeDef",
+    {
+        "ruleArn": str,
+        "rule": TopicRuleTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateTopicRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTopicRuleRequestRequestTypeDef",
     {
         "ruleName": str,
         "topicRulePayload": TopicRulePayloadTypeDef,
     },
 )
@@ -9289,23 +9803,44 @@
     "ReplaceTopicRuleRequestRequestTypeDef",
     {
         "ruleName": str,
         "topicRulePayload": TopicRulePayloadTypeDef,
     },
 )
 
-GetTopicRuleResponseTypeDef = TypedDict(
-    "GetTopicRuleResponseTypeDef",
+GetOTAUpdateResponseTypeDef = TypedDict(
+    "GetOTAUpdateResponseTypeDef",
     {
-        "ruleArn": str,
-        "rule": TopicRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "otaUpdateInfo": OTAUpdateInfoTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetOTAUpdateResponseTypeDef = TypedDict(
-    "GetOTAUpdateResponseTypeDef",
+_RequiredCreateOTAUpdateRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateOTAUpdateRequestRequestTypeDef",
     {
-        "otaUpdateInfo": OTAUpdateInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "otaUpdateId": str,
+        "targets": Sequence[str],
+        "files": Sequence[OTAUpdateFileUnionTypeDef],
+        "roleArn": str,
+    },
+)
+_OptionalCreateOTAUpdateRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateOTAUpdateRequestRequestTypeDef",
+    {
+        "description": str,
+        "protocols": Sequence[ProtocolType],
+        "targetSelection": TargetSelectionType,
+        "awsJobExecutionsRolloutConfig": AwsJobExecutionsRolloutConfigTypeDef,
+        "awsJobPresignedUrlConfig": AwsJobPresignedUrlConfigTypeDef,
+        "awsJobAbortConfig": AwsJobAbortConfigTypeDef,
+        "awsJobTimeoutConfig": AwsJobTimeoutConfigTypeDef,
+        "additionalParameters": Mapping[str, str],
+        "tags": Sequence[TagTypeDef],
     },
+    total=False,
 )
+
+class CreateOTAUpdateRequestRequestTypeDef(
+    _RequiredCreateOTAUpdateRequestRequestTypeDef, _OptionalCreateOTAUpdateRequestRequestTypeDef
+):
+    pass
```

### Comparing `types-aiobotocore-iot-2.5.2/types_aiobotocore_iot.egg-info/PKG-INFO` & `types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iot
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IoT 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IoT 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iot type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore iot type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iot"></a>
 
 # types-aiobotocore-iot
 
 [![PyPI - types-aiobotocore-iot](https://img.shields.io/pypi/v/types-aiobotocore-iot.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iot?color=blue)](https://pypistats.org/packages/types-aiobotocore-iot)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot)](https://pepy.tech/project/types-aiobotocore-iot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoT 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
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
 [types-aiobotocore-iot docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/).
 
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
@@ -643,137 +642,120 @@
 )
 
 
 def check_value(value: AbortActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iot.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iot.type_defs import (
     AbortCriteriaTypeDef,
     AcceptCertificateTransferRequestRequestTypeDef,
     CloudwatchAlarmActionTypeDef,
     CloudwatchLogsActionTypeDef,
     CloudwatchMetricActionTypeDef,
     DynamoDBActionTypeDef,
     ElasticsearchActionTypeDef,
     FirehoseActionTypeDef,
     IotAnalyticsActionTypeDef,
     IotEventsActionTypeDef,
-    KafkaActionTypeDef,
+    KafkaActionOutputTypeDef,
     KinesisActionTypeDef,
     LambdaActionTypeDef,
     OpenSearchActionTypeDef,
     S3ActionTypeDef,
     SalesforceActionTypeDef,
     SnsActionTypeDef,
     SqsActionTypeDef,
     StepFunctionsActionTypeDef,
-    MetricValueTypeDef,
+    KafkaActionTypeDef,
+    MetricValueOutputTypeDef,
     ViolationEventAdditionalInfoTypeDef,
     AddThingToBillingGroupRequestRequestTypeDef,
     AddThingToThingGroupRequestRequestTypeDef,
+    AddThingsToThingGroupParamsOutputTypeDef,
     AddThingsToThingGroupParamsTypeDef,
+    AggregationTypeOutputTypeDef,
     AggregationTypeTypeDef,
     AlertTargetTypeDef,
     PolicyTypeDef,
     AssetPropertyTimestampTypeDef,
     AssetPropertyVariantTypeDef,
     AssociateTargetsWithJobRequestRequestTypeDef,
-    AssociateTargetsWithJobResponseTypeDef,
+    ResponseMetadataTypeDef,
     AttachPolicyRequestRequestTypeDef,
     AttachPrincipalPolicyRequestRequestTypeDef,
     AttachSecurityProfileRequestRequestTypeDef,
     AttachThingPrincipalRequestRequestTypeDef,
+    AttributePayloadOutputTypeDef,
     AttributePayloadTypeDef,
     AuditCheckConfigurationTypeDef,
     AuditCheckDetailsTypeDef,
     AuditMitigationActionExecutionMetadataTypeDef,
     AuditMitigationActionsTaskMetadataTypeDef,
+    AuditMitigationActionsTaskTargetOutputTypeDef,
     AuditMitigationActionsTaskTargetTypeDef,
     AuditNotificationTargetTypeDef,
     AuditTaskMetadataTypeDef,
+    AuthInfoOutputTypeDef,
     AuthInfoTypeDef,
     AuthorizerConfigTypeDef,
     AuthorizerDescriptionTypeDef,
     AuthorizerSummaryTypeDef,
     AwsJobAbortCriteriaTypeDef,
     AwsJobRateIncreaseCriteriaTypeDef,
     AwsJobPresignedUrlConfigTypeDef,
     AwsJobTimeoutConfigTypeDef,
     MachineLearningDetectionConfigTypeDef,
     StatisticalThresholdTypeDef,
+    MetricValueTypeDef,
     BehaviorModelTrainingSummaryTypeDef,
     MetricDimensionTypeDef,
     BillingGroupMetadataTypeDef,
     BillingGroupPropertiesTypeDef,
+    BlobTypeDef,
     BucketTypeDef,
     TermsAggregationTypeDef,
     CertificateValidityTypeDef,
     CACertificateTypeDef,
     CancelAuditMitigationActionsTaskRequestRequestTypeDef,
     CancelAuditTaskRequestRequestTypeDef,
     CancelCertificateTransferRequestRequestTypeDef,
     CancelDetectMitigationActionsTaskRequestRequestTypeDef,
     CancelJobExecutionRequestRequestTypeDef,
     CancelJobRequestRequestTypeDef,
-    CancelJobResponseTypeDef,
     TransferDataTypeDef,
     CertificateTypeDef,
     CodeSigningCertificateChainTypeDef,
-    CodeSigningSignatureTypeDef,
+    CodeSigningSignatureOutputTypeDef,
     ConfigurationTypeDef,
     ConfirmTopicRuleDestinationRequestRequestTypeDef,
+    TimestampTypeDef,
     TagTypeDef,
-    CreateAuthorizerResponseTypeDef,
-    CreateBillingGroupResponseTypeDef,
     CreateCertificateFromCsrRequestRequestTypeDef,
-    CreateCertificateFromCsrResponseTypeDef,
-    CreateCustomMetricResponseTypeDef,
-    CreateDimensionResponseTypeDef,
     TlsConfigTypeDef,
-    CreateDomainConfigurationResponseTypeDef,
-    CreateDynamicThingGroupResponseTypeDef,
-    CreateFleetMetricResponseTypeDef,
     PresignedUrlConfigTypeDef,
     TimeoutConfigTypeDef,
-    CreateJobResponseTypeDef,
     MaintenanceWindowTypeDef,
-    CreateJobTemplateResponseTypeDef,
     CreateKeysAndCertificateRequestRequestTypeDef,
     KeyPairTypeDef,
-    CreateMitigationActionResponseTypeDef,
-    CreateOTAUpdateResponseTypeDef,
     CreatePackageRequestRequestTypeDef,
-    CreatePackageResponseTypeDef,
     CreatePackageVersionRequestRequestTypeDef,
-    CreatePackageVersionResponseTypeDef,
-    CreatePolicyResponseTypeDef,
     CreatePolicyVersionRequestRequestTypeDef,
-    CreatePolicyVersionResponseTypeDef,
     CreateProvisioningClaimRequestRequestTypeDef,
     ProvisioningHookTypeDef,
-    CreateProvisioningTemplateResponseTypeDef,
     CreateProvisioningTemplateVersionRequestRequestTypeDef,
-    CreateProvisioningTemplateVersionResponseTypeDef,
-    CreateRoleAliasResponseTypeDef,
-    CreateScheduledAuditResponseTypeDef,
-    CreateSecurityProfileResponseTypeDef,
-    CreateStreamResponseTypeDef,
-    CreateThingGroupResponseTypeDef,
-    CreateThingResponseTypeDef,
     ThingTypePropertiesTypeDef,
-    CreateThingTypeResponseTypeDef,
     DeleteAccountAuditConfigurationRequestRequestTypeDef,
     DeleteAuthorizerRequestRequestTypeDef,
     DeleteBillingGroupRequestRequestTypeDef,
     DeleteCACertificateRequestRequestTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     DeleteCustomMetricRequestRequestTypeDef,
     DeleteDimensionRequestRequestTypeDef,
@@ -809,374 +791,355 @@
     TaskStatisticsTypeDef,
     DescribeAuthorizerRequestRequestTypeDef,
     DescribeBillingGroupRequestRequestTypeDef,
     DescribeCACertificateRequestRequestTypeDef,
     RegistrationConfigTypeDef,
     DescribeCertificateRequestRequestTypeDef,
     DescribeCustomMetricRequestRequestTypeDef,
-    DescribeCustomMetricResponseTypeDef,
     DescribeDetectMitigationActionsTaskRequestRequestTypeDef,
     DescribeDimensionRequestRequestTypeDef,
-    DescribeDimensionResponseTypeDef,
     DescribeDomainConfigurationRequestRequestTypeDef,
     ServerCertificateSummaryTypeDef,
     DescribeEndpointRequestRequestTypeDef,
-    DescribeEndpointResponseTypeDef,
     DescribeFleetMetricRequestRequestTypeDef,
     DescribeIndexRequestRequestTypeDef,
-    DescribeIndexResponseTypeDef,
     DescribeJobExecutionRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeJobTemplateRequestRequestTypeDef,
     DescribeManagedJobTemplateRequestRequestTypeDef,
     DocumentParameterTypeDef,
     DescribeMitigationActionRequestRequestTypeDef,
     DescribeProvisioningTemplateRequestRequestTypeDef,
     DescribeProvisioningTemplateVersionRequestRequestTypeDef,
-    DescribeProvisioningTemplateVersionResponseTypeDef,
     DescribeRoleAliasRequestRequestTypeDef,
     RoleAliasDescriptionTypeDef,
     DescribeScheduledAuditRequestRequestTypeDef,
-    DescribeScheduledAuditResponseTypeDef,
     DescribeSecurityProfileRequestRequestTypeDef,
     DescribeStreamRequestRequestTypeDef,
     DescribeThingGroupRequestRequestTypeDef,
     DescribeThingRegistrationTaskRequestRequestTypeDef,
-    DescribeThingRegistrationTaskResponseTypeDef,
     DescribeThingRequestRequestTypeDef,
-    DescribeThingResponseTypeDef,
     DescribeThingTypeRequestRequestTypeDef,
     ThingTypeMetadataTypeDef,
+    ThingTypePropertiesOutputTypeDef,
     S3DestinationTypeDef,
     DetachPolicyRequestRequestTypeDef,
     DetachPrincipalPolicyRequestRequestTypeDef,
     DetachSecurityProfileRequestRequestTypeDef,
     DetachThingPrincipalRequestRequestTypeDef,
     DetectMitigationActionExecutionTypeDef,
     DetectMitigationActionsTaskStatisticsTypeDef,
+    DetectMitigationActionsTaskTargetOutputTypeDef,
+    ViolationEventOccurrenceRangeOutputTypeDef,
     DetectMitigationActionsTaskTargetTypeDef,
-    ViolationEventOccurrenceRangeTypeDef,
     DisableTopicRuleRequestRequestTypeDef,
     DomainConfigurationSummaryTypeDef,
     PutItemInputTypeDef,
     EffectivePolicyTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableIoTLoggingParamsTypeDef,
     EnableTopicRuleRequestRequestTypeDef,
     ErrorInfoTypeDef,
     RateIncreaseCriteriaTypeDef,
     FieldTypeDef,
     S3LocationTypeDef,
     StreamTypeDef,
     FleetMetricNameAndArnTypeDef,
-    GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetBehaviorModelTrainingSummariesRequestRequestTypeDef,
     GetCardinalityRequestRequestTypeDef,
-    GetCardinalityResponseTypeDef,
     GetEffectivePoliciesRequestRequestTypeDef,
     GetJobDocumentRequestRequestTypeDef,
-    GetJobDocumentResponseTypeDef,
-    GetLoggingOptionsResponseTypeDef,
     GetOTAUpdateRequestRequestTypeDef,
     VersionUpdateByJobsConfigTypeDef,
     GetPackageRequestRequestTypeDef,
-    GetPackageResponseTypeDef,
     GetPackageVersionRequestRequestTypeDef,
-    GetPackageVersionResponseTypeDef,
     GetPercentilesRequestRequestTypeDef,
     PercentPairTypeDef,
     GetPolicyRequestRequestTypeDef,
-    GetPolicyResponseTypeDef,
     GetPolicyVersionRequestRequestTypeDef,
-    GetPolicyVersionResponseTypeDef,
-    GetRegistrationCodeResponseTypeDef,
     GetStatisticsRequestRequestTypeDef,
     StatisticsTypeDef,
     GetTopicRuleDestinationRequestRequestTypeDef,
     GetTopicRuleRequestRequestTypeDef,
-    GetV2LoggingOptionsResponseTypeDef,
     GroupNameAndArnTypeDef,
     HttpActionHeaderTypeDef,
     SigV4AuthorizationTypeDef,
     HttpContextTypeDef,
     HttpUrlDestinationConfigurationTypeDef,
     HttpUrlDestinationPropertiesTypeDef,
     HttpUrlDestinationSummaryTypeDef,
+    IndexingFilterOutputTypeDef,
     IndexingFilterTypeDef,
     IssuerCertificateIdentifierTypeDef,
     JobExecutionStatusDetailsTypeDef,
     JobExecutionSummaryTypeDef,
     RetryCriteriaTypeDef,
     JobProcessDetailsTypeDef,
     JobSummaryTypeDef,
     JobTemplateSummaryTypeDef,
     ScheduledJobRolloutTypeDef,
-    ListActiveViolationsRequestListActiveViolationsPaginateTypeDef,
     ListActiveViolationsRequestRequestTypeDef,
-    ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef,
     ListAttachedPoliciesRequestRequestTypeDef,
-    ListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef,
     ListAuditMitigationActionsExecutionsRequestRequestTypeDef,
-    ListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef,
-    ListAuditMitigationActionsTasksRequestRequestTypeDef,
-    ListAuditTasksRequestListAuditTasksPaginateTypeDef,
-    ListAuditTasksRequestRequestTypeDef,
-    ListAuthorizersRequestListAuthorizersPaginateTypeDef,
     ListAuthorizersRequestRequestTypeDef,
-    ListBillingGroupsRequestListBillingGroupsPaginateTypeDef,
     ListBillingGroupsRequestRequestTypeDef,
-    ListCACertificatesRequestListCACertificatesPaginateTypeDef,
     ListCACertificatesRequestRequestTypeDef,
-    ListCertificatesByCARequestListCertificatesByCAPaginateTypeDef,
     ListCertificatesByCARequestRequestTypeDef,
-    ListCertificatesRequestListCertificatesPaginateTypeDef,
     ListCertificatesRequestRequestTypeDef,
-    ListCustomMetricsRequestListCustomMetricsPaginateTypeDef,
     ListCustomMetricsRequestRequestTypeDef,
-    ListCustomMetricsResponseTypeDef,
-    ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef,
-    ListDetectMitigationActionsExecutionsRequestRequestTypeDef,
-    ListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef,
-    ListDetectMitigationActionsTasksRequestRequestTypeDef,
-    ListDimensionsRequestListDimensionsPaginateTypeDef,
     ListDimensionsRequestRequestTypeDef,
-    ListDimensionsResponseTypeDef,
-    ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef,
     ListDomainConfigurationsRequestRequestTypeDef,
-    ListFleetMetricsRequestListFleetMetricsPaginateTypeDef,
     ListFleetMetricsRequestRequestTypeDef,
-    ListIndicesRequestListIndicesPaginateTypeDef,
     ListIndicesRequestRequestTypeDef,
-    ListIndicesResponseTypeDef,
-    ListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef,
     ListJobExecutionsForJobRequestRequestTypeDef,
-    ListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef,
     ListJobExecutionsForThingRequestRequestTypeDef,
-    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
-    ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef,
     ListManagedJobTemplatesRequestRequestTypeDef,
     ManagedJobTemplateSummaryTypeDef,
-    ListMetricValuesRequestListMetricValuesPaginateTypeDef,
-    ListMetricValuesRequestRequestTypeDef,
-    ListMitigationActionsRequestListMitigationActionsPaginateTypeDef,
     ListMitigationActionsRequestRequestTypeDef,
     MitigationActionIdentifierTypeDef,
-    ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef,
     ListOTAUpdatesRequestRequestTypeDef,
     OTAUpdateSummaryTypeDef,
-    ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef,
     ListOutgoingCertificatesRequestRequestTypeDef,
     OutgoingCertificateTypeDef,
-    ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
     ListPackageVersionsRequestRequestTypeDef,
     PackageVersionSummaryTypeDef,
-    ListPackagesRequestListPackagesPaginateTypeDef,
     ListPackagesRequestRequestTypeDef,
     PackageSummaryTypeDef,
-    ListPoliciesRequestListPoliciesPaginateTypeDef,
     ListPoliciesRequestRequestTypeDef,
-    ListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef,
     ListPolicyPrincipalsRequestRequestTypeDef,
-    ListPolicyPrincipalsResponseTypeDef,
     ListPolicyVersionsRequestRequestTypeDef,
     PolicyVersionTypeDef,
-    ListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef,
     ListPrincipalPoliciesRequestRequestTypeDef,
-    ListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef,
     ListPrincipalThingsRequestRequestTypeDef,
-    ListPrincipalThingsResponseTypeDef,
-    ListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef,
     ListProvisioningTemplateVersionsRequestRequestTypeDef,
     ProvisioningTemplateVersionSummaryTypeDef,
-    ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef,
     ListProvisioningTemplatesRequestRequestTypeDef,
     ProvisioningTemplateSummaryTypeDef,
-    ListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef,
     ListRelatedResourcesForAuditFindingRequestRequestTypeDef,
-    ListRoleAliasesRequestListRoleAliasesPaginateTypeDef,
     ListRoleAliasesRequestRequestTypeDef,
-    ListRoleAliasesResponseTypeDef,
-    ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef,
     ListScheduledAuditsRequestRequestTypeDef,
     ScheduledAuditMetadataTypeDef,
-    ListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef,
     ListSecurityProfilesForTargetRequestRequestTypeDef,
-    ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef,
     ListSecurityProfilesRequestRequestTypeDef,
     SecurityProfileIdentifierTypeDef,
-    ListStreamsRequestListStreamsPaginateTypeDef,
     ListStreamsRequestRequestTypeDef,
     StreamSummaryTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
     ListTargetsForPolicyRequestRequestTypeDef,
-    ListTargetsForPolicyResponseTypeDef,
-    ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef,
     ListTargetsForSecurityProfileRequestRequestTypeDef,
     SecurityProfileTargetTypeDef,
-    ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef,
     ListThingGroupsForThingRequestRequestTypeDef,
-    ListThingGroupsRequestListThingGroupsPaginateTypeDef,
     ListThingGroupsRequestRequestTypeDef,
-    ListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef,
     ListThingPrincipalsRequestRequestTypeDef,
-    ListThingPrincipalsResponseTypeDef,
-    ListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef,
     ListThingRegistrationTaskReportsRequestRequestTypeDef,
-    ListThingRegistrationTaskReportsResponseTypeDef,
-    ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef,
     ListThingRegistrationTasksRequestRequestTypeDef,
-    ListThingRegistrationTasksResponseTypeDef,
-    ListThingTypesRequestListThingTypesPaginateTypeDef,
     ListThingTypesRequestRequestTypeDef,
-    ListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef,
     ListThingsInBillingGroupRequestRequestTypeDef,
-    ListThingsInBillingGroupResponseTypeDef,
-    ListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef,
     ListThingsInThingGroupRequestRequestTypeDef,
-    ListThingsInThingGroupResponseTypeDef,
-    ListThingsRequestListThingsPaginateTypeDef,
     ListThingsRequestRequestTypeDef,
     ThingAttributeTypeDef,
-    ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef,
     ListTopicRuleDestinationsRequestRequestTypeDef,
-    ListTopicRulesRequestListTopicRulesPaginateTypeDef,
     ListTopicRulesRequestRequestTypeDef,
     TopicRuleListItemTypeDef,
-    ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef,
     ListV2LoggingLevelsRequestRequestTypeDef,
-    ListViolationEventsRequestListViolationEventsPaginateTypeDef,
-    ListViolationEventsRequestRequestTypeDef,
     LocationTimestampTypeDef,
     LogTargetTypeDef,
     LoggingOptionsPayloadTypeDef,
     PublishFindingToSnsParamsTypeDef,
     ReplaceDefaultPolicyVersionParamsTypeDef,
     UpdateCACertificateParamsTypeDef,
     UpdateDeviceCertificateParamsTypeDef,
-    MqttContextTypeDef,
     UserPropertyTypeDef,
-    PaginatorConfigTypeDef,
     PolicyVersionIdentifierTypeDef,
     PutVerificationStateOnViolationRequestRequestTypeDef,
-    RegisterCACertificateResponseTypeDef,
     RegisterCertificateRequestRequestTypeDef,
-    RegisterCertificateResponseTypeDef,
     RegisterCertificateWithoutCARequestRequestTypeDef,
-    RegisterCertificateWithoutCAResponseTypeDef,
     RegisterThingRequestRequestTypeDef,
-    RegisterThingResponseTypeDef,
     RejectCertificateTransferRequestRequestTypeDef,
     RemoveThingFromBillingGroupRequestRequestTypeDef,
     RemoveThingFromThingGroupRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     SearchIndexRequestRequestTypeDef,
     ThingGroupDocumentTypeDef,
     SetDefaultAuthorizerRequestRequestTypeDef,
-    SetDefaultAuthorizerResponseTypeDef,
     SetDefaultPolicyVersionRequestRequestTypeDef,
     SetV2LoggingOptionsRequestRequestTypeDef,
     SigningProfileParameterTypeDef,
-    StartAuditMitigationActionsTaskResponseTypeDef,
-    StartDetectMitigationActionsTaskResponseTypeDef,
     StartOnDemandAuditTaskRequestRequestTypeDef,
-    StartOnDemandAuditTaskResponseTypeDef,
     StartThingRegistrationTaskRequestRequestTypeDef,
-    StartThingRegistrationTaskResponseTypeDef,
     StopThingRegistrationTaskRequestRequestTypeDef,
     TlsContextTypeDef,
-    TestInvokeAuthorizerResponseTypeDef,
     ThingConnectivityTypeDef,
     TimestreamDimensionTypeDef,
     TimestreamTimestampTypeDef,
     VpcDestinationConfigurationTypeDef,
     VpcDestinationSummaryTypeDef,
     VpcDestinationPropertiesTypeDef,
     TransferCertificateRequestRequestTypeDef,
-    TransferCertificateResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAuthorizerRequestRequestTypeDef,
-    UpdateAuthorizerResponseTypeDef,
-    UpdateBillingGroupResponseTypeDef,
     UpdateCertificateRequestRequestTypeDef,
     UpdateCustomMetricRequestRequestTypeDef,
-    UpdateCustomMetricResponseTypeDef,
     UpdateDimensionRequestRequestTypeDef,
-    UpdateDimensionResponseTypeDef,
-    UpdateDomainConfigurationResponseTypeDef,
-    UpdateDynamicThingGroupResponseTypeDef,
-    UpdateMitigationActionResponseTypeDef,
     UpdatePackageRequestRequestTypeDef,
     UpdatePackageVersionRequestRequestTypeDef,
     UpdateRoleAliasRequestRequestTypeDef,
-    UpdateRoleAliasResponseTypeDef,
     UpdateScheduledAuditRequestRequestTypeDef,
-    UpdateScheduledAuditResponseTypeDef,
-    UpdateStreamResponseTypeDef,
-    UpdateThingGroupResponseTypeDef,
     UpdateThingGroupsForThingRequestRequestTypeDef,
     UpdateTopicRuleDestinationRequestRequestTypeDef,
     ValidationErrorTypeDef,
+    AbortConfigOutputTypeDef,
     AbortConfigTypeDef,
     MetricDatumTypeDef,
-    DescribeFleetMetricResponseTypeDef,
+    AggregationTypeUnionTypeDef,
     UpdateFleetMetricRequestRequestTypeDef,
     AllowedTypeDef,
     ExplicitDenyTypeDef,
     ImplicitDenyTypeDef,
+    AssetPropertyValueTypeDef,
+    AssociateTargetsWithJobResponseTypeDef,
+    CancelJobResponseTypeDef,
+    CreateAuthorizerResponseTypeDef,
+    CreateBillingGroupResponseTypeDef,
+    CreateCertificateFromCsrResponseTypeDef,
+    CreateCustomMetricResponseTypeDef,
+    CreateDimensionResponseTypeDef,
+    CreateDomainConfigurationResponseTypeDef,
+    CreateDynamicThingGroupResponseTypeDef,
+    CreateFleetMetricResponseTypeDef,
+    CreateJobResponseTypeDef,
+    CreateJobTemplateResponseTypeDef,
+    CreateMitigationActionResponseTypeDef,
+    CreateOTAUpdateResponseTypeDef,
+    CreatePackageResponseTypeDef,
+    CreatePackageVersionResponseTypeDef,
+    CreatePolicyResponseTypeDef,
+    CreatePolicyVersionResponseTypeDef,
+    CreateProvisioningTemplateResponseTypeDef,
+    CreateProvisioningTemplateVersionResponseTypeDef,
+    CreateRoleAliasResponseTypeDef,
+    CreateScheduledAuditResponseTypeDef,
+    CreateSecurityProfileResponseTypeDef,
+    CreateStreamResponseTypeDef,
+    CreateThingGroupResponseTypeDef,
+    CreateThingResponseTypeDef,
+    CreateThingTypeResponseTypeDef,
+    DescribeCustomMetricResponseTypeDef,
+    DescribeDimensionResponseTypeDef,
+    DescribeEndpointResponseTypeDef,
+    DescribeFleetMetricResponseTypeDef,
+    DescribeIndexResponseTypeDef,
+    DescribeProvisioningTemplateVersionResponseTypeDef,
+    DescribeScheduledAuditResponseTypeDef,
+    DescribeThingRegistrationTaskResponseTypeDef,
+    DescribeThingResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCardinalityResponseTypeDef,
+    GetJobDocumentResponseTypeDef,
+    GetLoggingOptionsResponseTypeDef,
+    GetPackageResponseTypeDef,
+    GetPackageVersionResponseTypeDef,
+    GetPolicyResponseTypeDef,
+    GetPolicyVersionResponseTypeDef,
+    GetRegistrationCodeResponseTypeDef,
+    GetV2LoggingOptionsResponseTypeDef,
     ListAttachedPoliciesResponseTypeDef,
+    ListCustomMetricsResponseTypeDef,
+    ListDimensionsResponseTypeDef,
+    ListIndicesResponseTypeDef,
     ListPoliciesResponseTypeDef,
+    ListPolicyPrincipalsResponseTypeDef,
     ListPrincipalPoliciesResponseTypeDef,
-    AssetPropertyValueTypeDef,
+    ListPrincipalThingsResponseTypeDef,
+    ListRoleAliasesResponseTypeDef,
+    ListTargetsForPolicyResponseTypeDef,
+    ListThingPrincipalsResponseTypeDef,
+    ListThingRegistrationTaskReportsResponseTypeDef,
+    ListThingRegistrationTasksResponseTypeDef,
+    ListThingsInBillingGroupResponseTypeDef,
+    ListThingsInThingGroupResponseTypeDef,
+    RegisterCACertificateResponseTypeDef,
+    RegisterCertificateResponseTypeDef,
+    RegisterCertificateWithoutCAResponseTypeDef,
+    RegisterThingResponseTypeDef,
+    SetDefaultAuthorizerResponseTypeDef,
+    StartAuditMitigationActionsTaskResponseTypeDef,
+    StartDetectMitigationActionsTaskResponseTypeDef,
+    StartOnDemandAuditTaskResponseTypeDef,
+    StartThingRegistrationTaskResponseTypeDef,
+    TestInvokeAuthorizerResponseTypeDef,
+    TransferCertificateResponseTypeDef,
+    UpdateAuthorizerResponseTypeDef,
+    UpdateBillingGroupResponseTypeDef,
+    UpdateCustomMetricResponseTypeDef,
+    UpdateDimensionResponseTypeDef,
+    UpdateDomainConfigurationResponseTypeDef,
+    UpdateDynamicThingGroupResponseTypeDef,
+    UpdateMitigationActionResponseTypeDef,
+    UpdateRoleAliasResponseTypeDef,
+    UpdateScheduledAuditResponseTypeDef,
+    UpdateStreamResponseTypeDef,
+    UpdateThingGroupResponseTypeDef,
+    ThingGroupPropertiesOutputTypeDef,
+    AttributePayloadUnionTypeDef,
     CreateThingRequestRequestTypeDef,
     ThingGroupPropertiesTypeDef,
     UpdateThingRequestRequestTypeDef,
     ListAuditMitigationActionsExecutionsResponseTypeDef,
     ListAuditMitigationActionsTasksResponseTypeDef,
+    AuditMitigationActionsTaskTargetUnionTypeDef,
     StartAuditMitigationActionsTaskRequestRequestTypeDef,
     DescribeAccountAuditConfigurationResponseTypeDef,
     UpdateAccountAuditConfigurationRequestRequestTypeDef,
     ListAuditTasksResponseTypeDef,
-    TestAuthorizationRequestRequestTypeDef,
+    AuthInfoUnionTypeDef,
     DescribeAuthorizerResponseTypeDef,
     DescribeDefaultAuthorizerResponseTypeDef,
     ListAuthorizersResponseTypeDef,
     AwsJobAbortConfigTypeDef,
     AwsJobExponentialRolloutRateTypeDef,
+    BehaviorCriteriaOutputTypeDef,
     BehaviorCriteriaTypeDef,
     GetBehaviorModelTrainingSummariesResponseTypeDef,
     MetricToRetainTypeDef,
     DescribeBillingGroupResponseTypeDef,
     UpdateBillingGroupRequestRequestTypeDef,
+    CodeSigningSignatureTypeDef,
+    MqttContextTypeDef,
     GetBucketsAggregationResponseTypeDef,
     BucketsAggregationTypeTypeDef,
     CACertificateDescriptionTypeDef,
     ListCACertificatesResponseTypeDef,
     CertificateDescriptionTypeDef,
     ListCertificatesByCAResponseTypeDef,
     ListCertificatesResponseTypeDef,
-    CustomCodeSigningTypeDef,
+    CustomCodeSigningOutputTypeDef,
     DescribeEventConfigurationsResponseTypeDef,
     UpdateEventConfigurationsRequestRequestTypeDef,
+    ListAuditMitigationActionsTasksRequestRequestTypeDef,
+    ListAuditTasksRequestRequestTypeDef,
+    ListDetectMitigationActionsExecutionsRequestRequestTypeDef,
+    ListDetectMitigationActionsTasksRequestRequestTypeDef,
+    ListMetricValuesRequestRequestTypeDef,
+    ListViolationEventsRequestRequestTypeDef,
+    ViolationEventOccurrenceRangeTypeDef,
     CreateAuthorizerRequestRequestTypeDef,
     CreateBillingGroupRequestRequestTypeDef,
     CreateCustomMetricRequestRequestTypeDef,
     CreateDimensionRequestRequestTypeDef,
     CreateFleetMetricRequestRequestTypeDef,
     CreatePolicyRequestRequestTypeDef,
     CreateRoleAliasRequestRequestTypeDef,
     CreateScheduledAuditRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDomainConfigurationRequestRequestTypeDef,
     UpdateDomainConfigurationRequestRequestTypeDef,
+    SchedulingConfigOutputTypeDef,
     SchedulingConfigTypeDef,
     CreateKeysAndCertificateResponseTypeDef,
     CreateProvisioningClaimResponseTypeDef,
     CreateProvisioningTemplateRequestRequestTypeDef,
     DescribeProvisioningTemplateResponseTypeDef,
     UpdateProvisioningTemplateRequestRequestTypeDef,
     CreateThingTypeRequestRequestTypeDef,
@@ -1184,38 +1147,99 @@
     RegisterCACertificateRequestRequestTypeDef,
     UpdateCACertificateRequestRequestTypeDef,
     DescribeDomainConfigurationResponseTypeDef,
     DescribeManagedJobTemplateResponseTypeDef,
     DescribeRoleAliasResponseTypeDef,
     DescribeThingTypeResponseTypeDef,
     ThingTypeDefinitionTypeDef,
+    ThingTypePropertiesUnionTypeDef,
     DestinationTypeDef,
     ListDetectMitigationActionsExecutionsResponseTypeDef,
-    StartDetectMitigationActionsTaskRequestRequestTypeDef,
+    DetectMitigationActionsTaskTargetUnionTypeDef,
     ListDomainConfigurationsResponseTypeDef,
     DynamoDBv2ActionTypeDef,
     GetEffectivePoliciesResponseTypeDef,
     ExponentialRolloutRateTypeDef,
+    ThingGroupIndexingConfigurationOutputTypeDef,
     ThingGroupIndexingConfigurationTypeDef,
     StreamFileTypeDef,
     FileLocationTypeDef,
     ListFleetMetricsResponseTypeDef,
+    GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef,
+    ListActiveViolationsRequestListActiveViolationsPaginateTypeDef,
+    ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef,
+    ListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef,
+    ListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef,
+    ListAuditTasksRequestListAuditTasksPaginateTypeDef,
+    ListAuthorizersRequestListAuthorizersPaginateTypeDef,
+    ListBillingGroupsRequestListBillingGroupsPaginateTypeDef,
+    ListCACertificatesRequestListCACertificatesPaginateTypeDef,
+    ListCertificatesByCARequestListCertificatesByCAPaginateTypeDef,
+    ListCertificatesRequestListCertificatesPaginateTypeDef,
+    ListCustomMetricsRequestListCustomMetricsPaginateTypeDef,
+    ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef,
+    ListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef,
+    ListDimensionsRequestListDimensionsPaginateTypeDef,
+    ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef,
+    ListFleetMetricsRequestListFleetMetricsPaginateTypeDef,
+    ListIndicesRequestListIndicesPaginateTypeDef,
+    ListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef,
+    ListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef,
+    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
+    ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef,
+    ListMetricValuesRequestListMetricValuesPaginateTypeDef,
+    ListMitigationActionsRequestListMitigationActionsPaginateTypeDef,
+    ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef,
+    ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef,
+    ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+    ListPackagesRequestListPackagesPaginateTypeDef,
+    ListPoliciesRequestListPoliciesPaginateTypeDef,
+    ListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef,
+    ListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef,
+    ListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef,
+    ListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef,
+    ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef,
+    ListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef,
+    ListRoleAliasesRequestListRoleAliasesPaginateTypeDef,
+    ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef,
+    ListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef,
+    ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef,
+    ListStreamsRequestListStreamsPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
+    ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef,
+    ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef,
+    ListThingGroupsRequestListThingGroupsPaginateTypeDef,
+    ListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef,
+    ListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef,
+    ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef,
+    ListThingTypesRequestListThingTypesPaginateTypeDef,
+    ListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef,
+    ListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef,
+    ListThingsRequestListThingsPaginateTypeDef,
+    ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef,
+    ListTopicRulesRequestListTopicRulesPaginateTypeDef,
+    ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef,
+    ListViolationEventsRequestListViolationEventsPaginateTypeDef,
     GetPackageConfigurationResponseTypeDef,
     UpdatePackageConfigurationRequestRequestTypeDef,
     GetPercentilesResponseTypeDef,
     GetStatisticsResponseTypeDef,
     ListBillingGroupsResponseTypeDef,
     ListThingGroupsForThingResponseTypeDef,
     ListThingGroupsResponseTypeDef,
     ThingGroupMetadataTypeDef,
     HttpAuthorizationTypeDef,
+    ThingIndexingConfigurationOutputTypeDef,
     ThingIndexingConfigurationTypeDef,
     JobExecutionTypeDef,
     JobExecutionSummaryForJobTypeDef,
     JobExecutionSummaryForThingTypeDef,
+    JobExecutionsRetryConfigOutputTypeDef,
     JobExecutionsRetryConfigTypeDef,
     ListJobsResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     ListManagedJobTemplatesResponseTypeDef,
     ListMitigationActionsResponseTypeDef,
     ListOTAUpdatesResponseTypeDef,
     ListOutgoingCertificatesResponseTypeDef,
@@ -1231,55 +1255,73 @@
     SecurityProfileTargetMappingTypeDef,
     ListThingsResponseTypeDef,
     ListTopicRulesResponseTypeDef,
     LocationActionTypeDef,
     LogTargetConfigurationTypeDef,
     SetV2LoggingLevelRequestRequestTypeDef,
     SetLoggingOptionsRequestRequestTypeDef,
+    MitigationActionParamsOutputTypeDef,
     MitigationActionParamsTypeDef,
+    MqttHeadersOutputTypeDef,
     MqttHeadersTypeDef,
     ResourceIdentifierTypeDef,
-    TestInvokeAuthorizerRequestRequestTypeDef,
     ThingDocumentTypeDef,
+    TimestreamActionOutputTypeDef,
     TimestreamActionTypeDef,
     TopicRuleDestinationConfigurationTypeDef,
     TopicRuleDestinationSummaryTypeDef,
     TopicRuleDestinationTypeDef,
     ValidateSecurityProfileBehaviorsResponseTypeDef,
+    AbortConfigUnionTypeDef,
     ListMetricValuesResponseTypeDef,
     DeniedTypeDef,
+    PutAssetPropertyValueEntryOutputTypeDef,
     PutAssetPropertyValueEntryTypeDef,
     CreateDynamicThingGroupRequestRequestTypeDef,
     CreateThingGroupRequestRequestTypeDef,
+    ThingGroupPropertiesUnionTypeDef,
     UpdateDynamicThingGroupRequestRequestTypeDef,
     UpdateThingGroupRequestRequestTypeDef,
+    TestAuthorizationRequestRequestTypeDef,
     AwsJobExecutionsRolloutConfigTypeDef,
+    BehaviorOutputTypeDef,
     BehaviorTypeDef,
+    CustomCodeSigningTypeDef,
+    TestInvokeAuthorizerRequestRequestTypeDef,
     GetBucketsAggregationRequestRequestTypeDef,
     DescribeCACertificateResponseTypeDef,
     DescribeCertificateResponseTypeDef,
+    StartDetectMitigationActionsTaskRequestRequestTypeDef,
+    ViolationEventOccurrenceRangeUnionTypeDef,
+    SchedulingConfigUnionTypeDef,
     ListThingTypesResponseTypeDef,
     StartSigningJobParameterTypeDef,
     JobExecutionsRolloutConfigTypeDef,
+    ThingGroupIndexingConfigurationUnionTypeDef,
     CreateStreamRequestRequestTypeDef,
     StreamInfoTypeDef,
     UpdateStreamRequestRequestTypeDef,
     DescribeThingGroupResponseTypeDef,
+    HttpActionOutputTypeDef,
     HttpActionTypeDef,
     GetIndexingConfigurationResponseTypeDef,
+    ThingIndexingConfigurationUnionTypeDef,
     UpdateIndexingConfigurationRequestRequestTypeDef,
     DescribeJobExecutionResponseTypeDef,
     ListJobExecutionsForJobResponseTypeDef,
     ListJobExecutionsForThingResponseTypeDef,
+    JobExecutionsRetryConfigUnionTypeDef,
     ListSecurityProfilesForTargetResponseTypeDef,
     ListV2LoggingLevelsResponseTypeDef,
-    CreateMitigationActionRequestRequestTypeDef,
     DescribeMitigationActionResponseTypeDef,
     MitigationActionTypeDef,
+    CreateMitigationActionRequestRequestTypeDef,
+    MitigationActionParamsUnionTypeDef,
     UpdateMitigationActionRequestRequestTypeDef,
+    RepublishActionOutputTypeDef,
     RepublishActionTypeDef,
     AuditSuppressionTypeDef,
     CreateAuditSuppressionRequestRequestTypeDef,
     DeleteAuditSuppressionRequestRequestTypeDef,
     DescribeAuditSuppressionRequestRequestTypeDef,
     DescribeAuditSuppressionResponseTypeDef,
     ListAuditFindingsRequestListAuditFindingsPaginateTypeDef,
@@ -1291,56 +1333,62 @@
     UpdateAuditSuppressionRequestRequestTypeDef,
     SearchIndexResponseTypeDef,
     CreateTopicRuleDestinationRequestRequestTypeDef,
     ListTopicRuleDestinationsResponseTypeDef,
     CreateTopicRuleDestinationResponseTypeDef,
     GetTopicRuleDestinationResponseTypeDef,
     AuthResultTypeDef,
+    IotSiteWiseActionOutputTypeDef,
     IotSiteWiseActionTypeDef,
     ActiveViolationTypeDef,
-    CreateSecurityProfileRequestRequestTypeDef,
     DescribeSecurityProfileResponseTypeDef,
-    UpdateSecurityProfileRequestRequestTypeDef,
     UpdateSecurityProfileResponseTypeDef,
-    ValidateSecurityProfileBehaviorsRequestRequestTypeDef,
     ViolationEventTypeDef,
+    BehaviorUnionTypeDef,
+    CodeSigningOutputTypeDef,
     CodeSigningTypeDef,
     CreateJobRequestRequestTypeDef,
     CreateJobTemplateRequestRequestTypeDef,
     DescribeJobTemplateResponseTypeDef,
     JobTypeDef,
     UpdateJobRequestRequestTypeDef,
     DescribeStreamResponseTypeDef,
     DescribeAuditMitigationActionsTaskResponseTypeDef,
     DetectMitigationActionsTaskSummaryTypeDef,
     ListAuditSuppressionsResponseTypeDef,
     AuditFindingTypeDef,
     ListRelatedResourcesForAuditFindingResponseTypeDef,
     TestAuthorizationResponseTypeDef,
+    ActionOutputTypeDef,
     ActionTypeDef,
     ListActiveViolationsResponseTypeDef,
     ListViolationEventsResponseTypeDef,
+    CreateSecurityProfileRequestRequestTypeDef,
+    UpdateSecurityProfileRequestRequestTypeDef,
+    ValidateSecurityProfileBehaviorsRequestRequestTypeDef,
+    OTAUpdateFileOutputTypeDef,
     OTAUpdateFileTypeDef,
     DescribeJobResponseTypeDef,
     DescribeDetectMitigationActionsTaskResponseTypeDef,
     ListDetectMitigationActionsTasksResponseTypeDef,
     DescribeAuditFindingResponseTypeDef,
     ListAuditFindingsResponseTypeDef,
-    TopicRulePayloadTypeDef,
     TopicRuleTypeDef,
-    CreateOTAUpdateRequestRequestTypeDef,
+    TopicRulePayloadTypeDef,
     OTAUpdateInfoTypeDef,
+    OTAUpdateFileUnionTypeDef,
+    GetTopicRuleResponseTypeDef,
     CreateTopicRuleRequestRequestTypeDef,
     ReplaceTopicRuleRequestRequestTypeDef,
-    GetTopicRuleResponseTypeDef,
     GetOTAUpdateResponseTypeDef,
+    CreateOTAUpdateRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AbortCriteriaTypeDef:
+def get_value() -> AbortCriteriaTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iot-2.5.2/types_aiobotocore_iot.egg-info/SOURCES.txt` & `types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot.egg-info/SOURCES.txt`

 * *Files identical despite different names*


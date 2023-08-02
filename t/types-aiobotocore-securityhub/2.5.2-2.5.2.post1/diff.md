# Comparing `tmp/types-aiobotocore-securityhub-2.5.2.tar.gz` & `tmp/types-aiobotocore-securityhub-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-securityhub-2.5.2.tar", last modified: Sat Jul  8 01:44:18 2023, max compression
+gzip compressed data, was "types-aiobotocore-securityhub-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:59 2023, max compression
```

## Comparing `types-aiobotocore-securityhub-2.5.2.tar` & `types-aiobotocore-securityhub-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:18.038880 types-aiobotocore-securityhub-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:40:39.000000 types-aiobotocore-securityhub-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    51423 2023-07-08 01:44:18.038880 types-aiobotocore-securityhub-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    49842 2023-07-08 01:40:39.000000 types-aiobotocore-securityhub-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:18.038880 types-aiobotocore-securityhub-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-08 01:40:39.000000 types-aiobotocore-securityhub-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:18.038880 types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub/
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-07-08 01:40:39.000000 types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-07-08 01:40:39.000000 types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-08 01:40:39.000000 types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54849 2023-07-08 01:40:40.000000 types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    54758 2023-07-08 01:40:40.000000 types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14068 2023-07-08 01:40:40.000000 types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14066 2023-07-08 01:40:40.000000 types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19141 2023-07-08 01:40:40.000000 types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19124 2023-07-08 01:40:40.000000 types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:40:39.000000 types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   279900 2023-07-08 01:40:45.000000 types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   279833 2023-07-08 01:40:43.000000 types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:40:39.000000 types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:18.038880 types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    51423 2023-07-08 01:44:17.000000 types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-08 01:44:17.000000 types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:17.000000 types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:17.000000 types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:17.000000 types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-08 01:44:17.000000 types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.369462 types-aiobotocore-securityhub-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:17.000000 types-aiobotocore-securityhub-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    61760 2023-08-02 14:52:59.369462 types-aiobotocore-securityhub-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    60226 2023-08-02 14:49:17.000000 types-aiobotocore-securityhub-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:59.369462 types-aiobotocore-securityhub-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-02 14:49:14.000000 types-aiobotocore-securityhub-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.365462 types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub/
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-08-02 14:49:17.000000 types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-08-02 14:49:17.000000 types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-02 14:49:17.000000 types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54881 2023-08-02 14:49:17.000000 types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54790 2023-08-02 14:49:17.000000 types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14068 2023-08-02 14:49:18.000000 types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14066 2023-08-02 14:49:18.000000 types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-08-02 14:49:18.000000 types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19081 2023-08-02 14:49:18.000000 types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:17.000000 types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   401063 2023-08-02 14:49:27.000000 types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   400990 2023-08-02 14:49:21.000000 types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:17.000000 types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.369462 types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    61760 2023-08-02 14:52:59.000000 types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-02 14:52:59.000000 types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:59.000000 types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:59.000000 types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:59.000000 types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 14:52:59.000000 types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-securityhub-2.5.2/LICENSE` & `types-aiobotocore-securityhub-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securityhub-2.5.2/PKG-INFO` & `types-aiobotocore-securityhub-2.5.2.post1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-securityhub
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SecurityHub 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SecurityHub 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore securityhub type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore securityhub type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-securityhub"></a>
 
 # types-aiobotocore-securityhub
 
 [![PyPI - types-aiobotocore-securityhub](https://img.shields.io/pypi/v/types-aiobotocore-securityhub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-securityhub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-securityhub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-securityhub)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-securityhub?color=blue)](https://pypistats.org/packages/types-aiobotocore-securityhub)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-securityhub)](https://pepy.tech/project/types-aiobotocore-securityhub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SecurityHub 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
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
 [types-aiobotocore-securityhub docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/).
 
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
@@ -404,107 +403,117 @@
 )
 
 
 def check_value(value: AdminStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_securityhub.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_securityhub.type_defs import (
     AcceptAdministratorInvitationRequestRequestTypeDef,
     AcceptInvitationRequestRequestTypeDef,
     AccountDetailsTypeDef,
     ActionLocalIpDetailsTypeDef,
     ActionLocalPortDetailsTypeDef,
+    DnsRequestActionTypeDef,
     CityTypeDef,
     CountryTypeDef,
     GeoLocationTypeDef,
     IpOrganizationDetailsTypeDef,
     ActionRemotePortDetailsTypeDef,
     ActionTargetTypeDef,
-    DnsRequestActionTypeDef,
     AdjustmentTypeDef,
     AdminAccountTypeDef,
     AssociatedStandardTypeDef,
     AssociationStateDetailsTypeDef,
     NoteUpdateTypeDef,
     RelatedFindingTypeDef,
     SeverityUpdateTypeDef,
     WorkflowUpdateTypeDef,
     MapFilterTypeDef,
     NumberFilterTypeDef,
     StringFilterTypeDef,
     AutomationRulesMetadataTypeDef,
     AvailabilityZoneTypeDef,
     AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef,
-    AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef,
+    AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef,
     AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef,
     AwsAmazonMqBrokerUsersDetailsTypeDef,
+    AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef,
     AwsAmazonMqBrokerLogsPendingDetailsTypeDef,
     AwsApiCallActionDomainDetailsTypeDef,
     AwsApiGatewayAccessLogSettingsTypeDef,
+    AwsApiGatewayCanarySettingsOutputTypeDef,
     AwsApiGatewayCanarySettingsTypeDef,
+    AwsApiGatewayEndpointConfigurationOutputTypeDef,
     AwsApiGatewayEndpointConfigurationTypeDef,
     AwsApiGatewayMethodSettingsTypeDef,
+    AwsCorsConfigurationOutputTypeDef,
     AwsCorsConfigurationTypeDef,
     AwsApiGatewayV2RouteSettingsTypeDef,
     AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef,
     AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef,
     AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef,
     AwsAppSyncGraphQlApiLogConfigDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationMetadataOptionsTypeDef,
+    AwsBackupBackupPlanAdvancedBackupSettingsDetailsOutputTypeDef,
     AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef,
     AwsBackupBackupPlanLifecycleDetailsTypeDef,
+    AwsBackupBackupVaultNotificationsDetailsOutputTypeDef,
     AwsBackupBackupVaultNotificationsDetailsTypeDef,
     AwsBackupRecoveryPointCalculatedLifecycleDetailsTypeDef,
     AwsBackupRecoveryPointCreatedByDetailsTypeDef,
     AwsBackupRecoveryPointLifecycleDetailsTypeDef,
     AwsCertificateManagerCertificateExtendedKeyUsageTypeDef,
     AwsCertificateManagerCertificateKeyUsageTypeDef,
     AwsCertificateManagerCertificateOptionsTypeDef,
     AwsCertificateManagerCertificateResourceRecordTypeDef,
     AwsCloudFormationStackDriftInformationDetailsTypeDef,
     AwsCloudFormationStackOutputsDetailsTypeDef,
     AwsCloudFrontDistributionCacheBehaviorTypeDef,
     AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef,
     AwsCloudFrontDistributionLoggingTypeDef,
     AwsCloudFrontDistributionViewerCertificateTypeDef,
+    AwsCloudFrontDistributionOriginSslProtocolsOutputTypeDef,
     AwsCloudFrontDistributionOriginSslProtocolsTypeDef,
+    AwsCloudFrontDistributionOriginGroupFailoverStatusCodesOutputTypeDef,
     AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef,
     AwsCloudFrontDistributionOriginS3OriginConfigTypeDef,
     AwsCloudTrailTrailDetailsTypeDef,
     AwsCloudWatchAlarmDimensionsDetailsTypeDef,
     AwsCodeBuildProjectArtifactsDetailsTypeDef,
     AwsCodeBuildProjectSourceTypeDef,
+    AwsCodeBuildProjectVpcConfigOutputTypeDef,
     AwsCodeBuildProjectVpcConfigTypeDef,
     AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef,
     AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef,
     AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef,
     AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef,
     AwsDynamoDbTableAttributeDefinitionTypeDef,
     AwsDynamoDbTableBillingModeSummaryTypeDef,
     AwsDynamoDbTableKeySchemaTypeDef,
     AwsDynamoDbTableProvisionedThroughputTypeDef,
     AwsDynamoDbTableRestoreSummaryTypeDef,
     AwsDynamoDbTableSseDescriptionTypeDef,
     AwsDynamoDbTableStreamSpecificationTypeDef,
+    AwsDynamoDbTableProjectionOutputTypeDef,
     AwsDynamoDbTableProjectionTypeDef,
     AwsDynamoDbTableProvisionedThroughputOverrideTypeDef,
     AwsEc2EipDetailsTypeDef,
     AwsEc2InstanceMetadataOptionsTypeDef,
     AwsEc2InstanceMonitoringDetailsTypeDef,
     AwsEc2InstanceNetworkInterfacesDetailsTypeDef,
     AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef,
@@ -545,86 +554,101 @@
     PropagatingVgwSetDetailsTypeDef,
     RouteSetDetailsTypeDef,
     AwsEc2SecurityGroupIpRangeTypeDef,
     AwsEc2SecurityGroupIpv6RangeTypeDef,
     AwsEc2SecurityGroupPrefixListIdTypeDef,
     AwsEc2SecurityGroupUserIdGroupPairTypeDef,
     Ipv6CidrBlockAssociationTypeDef,
+    AwsEc2TransitGatewayDetailsOutputTypeDef,
     AwsEc2TransitGatewayDetailsTypeDef,
     AwsEc2VolumeAttachmentTypeDef,
     CidrBlockAssociationTypeDef,
     AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef,
     AwsEc2VpcPeeringConnectionStatusDetailsTypeDef,
     VpcInfoCidrBlockSetDetailsTypeDef,
     VpcInfoIpv6CidrBlockSetDetailsTypeDef,
     VpcInfoPeeringOptionsDetailsTypeDef,
     AwsEc2VpnConnectionRoutesDetailsTypeDef,
     AwsEc2VpnConnectionVgwTelemetryDetailsTypeDef,
+    AwsEc2VpnConnectionOptionsTunnelOptionsDetailsOutputTypeDef,
     AwsEc2VpnConnectionOptionsTunnelOptionsDetailsTypeDef,
+    AwsEcrContainerImageDetailsOutputTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     AwsEcrRepositoryImageScanningConfigurationDetailsTypeDef,
     AwsEcrRepositoryLifecyclePolicyDetailsTypeDef,
     AwsEcsClusterClusterSettingsDetailsTypeDef,
     AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef,
     AwsEcsClusterDefaultCapacityProviderStrategyDetailsTypeDef,
     AwsMountPointTypeDef,
     AwsEcsServiceCapacityProviderStrategyDetailsTypeDef,
     AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef,
     AwsEcsServiceDeploymentControllerDetailsTypeDef,
     AwsEcsServiceLoadBalancersDetailsTypeDef,
     AwsEcsServicePlacementConstraintsDetailsTypeDef,
     AwsEcsServicePlacementStrategiesDetailsTypeDef,
     AwsEcsServiceServiceRegistriesDetailsTypeDef,
+    AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsOutputTypeDef,
     AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsOutputTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef,
     AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef,
     AwsEcsTaskDefinitionPlacementConstraintsDetailsTypeDef,
     AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef,
-    AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef,
+    AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsOutputTypeDef,
     AwsEcsTaskDefinitionVolumesHostDetailsTypeDef,
+    AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef,
     AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef,
     AwsEcsTaskVolumeHostDetailsTypeDef,
+    AwsEfsAccessPointPosixUserDetailsOutputTypeDef,
     AwsEfsAccessPointPosixUserDetailsTypeDef,
     AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef,
+    AwsEksClusterResourcesVpcConfigDetailsOutputTypeDef,
     AwsEksClusterResourcesVpcConfigDetailsTypeDef,
+    AwsEksClusterLoggingClusterLoggingDetailsOutputTypeDef,
     AwsEksClusterLoggingClusterLoggingDetailsTypeDef,
     AwsElasticBeanstalkEnvironmentEnvironmentLinkTypeDef,
     AwsElasticBeanstalkEnvironmentOptionSettingTypeDef,
     AwsElasticBeanstalkEnvironmentTierTypeDef,
     AwsElasticsearchDomainDomainEndpointOptionsTypeDef,
     AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef,
     AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef,
     AwsElasticsearchDomainServiceSoftwareOptionsTypeDef,
+    AwsElasticsearchDomainVPCOptionsOutputTypeDef,
     AwsElasticsearchDomainVPCOptionsTypeDef,
     AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef,
     AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef,
     AwsElbAppCookieStickinessPolicyTypeDef,
     AwsElbLbCookieStickinessPolicyTypeDef,
     AwsElbLoadBalancerAccessLogTypeDef,
     AwsElbLoadBalancerAdditionalAttributeTypeDef,
     AwsElbLoadBalancerConnectionDrainingTypeDef,
     AwsElbLoadBalancerConnectionSettingsTypeDef,
     AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef,
+    AwsElbLoadBalancerBackendServerDescriptionOutputTypeDef,
     AwsElbLoadBalancerBackendServerDescriptionTypeDef,
     AwsElbLoadBalancerHealthCheckTypeDef,
     AwsElbLoadBalancerInstanceTypeDef,
     AwsElbLoadBalancerSourceSecurityGroupTypeDef,
     AwsElbLoadBalancerListenerTypeDef,
     AwsElbv2LoadBalancerAttributeTypeDef,
     LoadBalancerStateTypeDef,
@@ -647,42 +671,48 @@
     AwsIamUserPolicyTypeDef,
     AwsKinesisStreamStreamEncryptionDetailsTypeDef,
     AwsKmsKeyDetailsTypeDef,
     AwsLambdaFunctionCodeTypeDef,
     AwsLambdaFunctionDeadLetterConfigTypeDef,
     AwsLambdaFunctionLayerTypeDef,
     AwsLambdaFunctionTracingConfigTypeDef,
+    AwsLambdaFunctionVpcConfigOutputTypeDef,
     AwsLambdaFunctionVpcConfigTypeDef,
     AwsLambdaFunctionEnvironmentErrorTypeDef,
+    AwsLambdaLayerVersionDetailsOutputTypeDef,
     AwsLambdaLayerVersionDetailsTypeDef,
     AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef,
     AwsOpenSearchServiceDomainMasterUserOptionsDetailsTypeDef,
     AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef,
     AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef,
     AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsTypeDef,
     AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsTypeDef,
     AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsTypeDef,
+    AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef,
     AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef,
     AwsOpenSearchServiceDomainLogPublishingOptionTypeDef,
     AwsRdsDbClusterAssociatedRoleTypeDef,
     AwsRdsDbClusterMemberTypeDef,
     AwsRdsDbClusterOptionGroupMembershipTypeDef,
     AwsRdsDbDomainMembershipTypeDef,
     AwsRdsDbInstanceVpcSecurityGroupTypeDef,
+    AwsRdsDbClusterSnapshotDetailsOutputTypeDef,
     AwsRdsDbClusterSnapshotDetailsTypeDef,
     AwsRdsDbInstanceAssociatedRoleTypeDef,
     AwsRdsDbInstanceEndpointTypeDef,
     AwsRdsDbOptionGroupMembershipTypeDef,
     AwsRdsDbParameterGroupTypeDef,
     AwsRdsDbProcessorFeatureTypeDef,
     AwsRdsDbStatusInfoTypeDef,
+    AwsRdsPendingCloudWatchLogsExportsOutputTypeDef,
     AwsRdsPendingCloudWatchLogsExportsTypeDef,
     AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef,
     AwsRdsDbSecurityGroupIpRangeTypeDef,
     AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef,
+    AwsRdsEventSubscriptionDetailsOutputTypeDef,
     AwsRdsEventSubscriptionDetailsTypeDef,
     AwsRedshiftClusterClusterNodeTypeDef,
     AwsRedshiftClusterClusterParameterStatusTypeDef,
     AwsRedshiftClusterClusterSecurityGroupTypeDef,
     AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef,
     AwsRedshiftClusterDeferredMaintenanceWindowTypeDef,
     AwsRedshiftClusterElasticIpStatusTypeDef,
@@ -739,14 +769,15 @@
     WafExcludedRuleTypeDef,
     WafOverrideActionTypeDef,
     AwsWafv2CustomHttpHeaderTypeDef,
     AwsWafv2VisibilityConfigDetailsTypeDef,
     AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef,
     AwsXrayEncryptionConfigDetailsTypeDef,
     BatchDeleteAutomationRulesRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UnprocessedAutomationRuleTypeDef,
     BatchDisableStandardsRequestRequestTypeDef,
     StandardsSubscriptionRequestTypeDef,
     BatchGetAutomationRulesRequestRequestTypeDef,
     BatchGetSecurityControlsRequestRequestTypeDef,
     SecurityControlTypeDef,
     UnprocessedSecurityControlTypeDef,
@@ -755,400 +786,575 @@
     ImportFindingsErrorTypeDef,
     StandardsControlAssociationUpdateTypeDef,
     CellTypeDef,
     ClassificationStatusTypeDef,
     StatusReasonTypeDef,
     VolumeMountTypeDef,
     CreateActionTargetRequestRequestTypeDef,
-    CreateActionTargetResponseTypeDef,
-    CreateAutomationRuleResponseTypeDef,
     CreateFindingAggregatorRequestRequestTypeDef,
-    CreateFindingAggregatorResponseTypeDef,
-    CreateInsightResponseTypeDef,
     ResultTypeDef,
     DateRangeTypeDef,
     DeclineInvitationsRequestRequestTypeDef,
     DeleteActionTargetRequestRequestTypeDef,
-    DeleteActionTargetResponseTypeDef,
     DeleteFindingAggregatorRequestRequestTypeDef,
     DeleteInsightRequestRequestTypeDef,
-    DeleteInsightResponseTypeDef,
     DeleteInvitationsRequestRequestTypeDef,
     DeleteMembersRequestRequestTypeDef,
-    DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeActionTargetsRequestRequestTypeDef,
     DescribeHubRequestRequestTypeDef,
-    DescribeHubResponseTypeDef,
-    DescribeOrganizationConfigurationResponseTypeDef,
-    DescribeProductsRequestDescribeProductsPaginateTypeDef,
     DescribeProductsRequestRequestTypeDef,
     ProductTypeDef,
-    DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
     DescribeStandardsControlsRequestRequestTypeDef,
     StandardsControlTypeDef,
-    DescribeStandardsRequestDescribeStandardsPaginateTypeDef,
     DescribeStandardsRequestRequestTypeDef,
     DisableImportFindingsForProductRequestRequestTypeDef,
     DisableOrganizationAdminAccountRequestRequestTypeDef,
     DisassociateMembersRequestRequestTypeDef,
     EnableImportFindingsForProductRequestRequestTypeDef,
-    EnableImportFindingsForProductResponseTypeDef,
     EnableOrganizationAdminAccountRequestRequestTypeDef,
     EnableSecurityHubRequestRequestTypeDef,
     FilePathsTypeDef,
     FindingAggregatorTypeDef,
     FindingHistoryUpdateSourceTypeDef,
     FindingHistoryUpdateTypeDef,
     FindingProviderSeverityTypeDef,
     FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef,
     FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef,
     InvitationTypeDef,
-    GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef,
     GetEnabledStandardsRequestRequestTypeDef,
     GetFindingAggregatorRequestRequestTypeDef,
-    GetFindingAggregatorResponseTypeDef,
+    TimestampTypeDef,
     SortCriterionTypeDef,
     GetInsightResultsRequestRequestTypeDef,
-    GetInsightsRequestGetInsightsPaginateTypeDef,
     GetInsightsRequestRequestTypeDef,
-    GetInvitationsCountResponseTypeDef,
     GetMembersRequestRequestTypeDef,
     MemberTypeDef,
     InsightResultValueTypeDef,
     InviteMembersRequestRequestTypeDef,
     ListAutomationRulesRequestRequestTypeDef,
-    ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef,
     ListEnabledProductsForImportRequestRequestTypeDef,
-    ListEnabledProductsForImportResponseTypeDef,
-    ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef,
     ListFindingAggregatorsRequestRequestTypeDef,
-    ListInvitationsRequestListInvitationsPaginateTypeDef,
     ListInvitationsRequestRequestTypeDef,
-    ListMembersRequestListMembersPaginateTypeDef,
     ListMembersRequestRequestTypeDef,
-    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
     ListOrganizationAdminAccountsRequestRequestTypeDef,
-    ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef,
     ListSecurityControlDefinitionsRequestRequestTypeDef,
     SecurityControlDefinitionTypeDef,
-    ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef,
     ListStandardsControlAssociationsRequestRequestTypeDef,
     StandardsControlAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PortRangeTypeDef,
     RangeTypeDef,
     RecordTypeDef,
-    PaginatorConfigTypeDef,
     RecommendationTypeDef,
-    ResponseMetadataTypeDef,
+    RuleGroupSourceListDetailsOutputTypeDef,
     RuleGroupSourceListDetailsTypeDef,
     RuleGroupSourceStatefulRulesHeaderDetailsTypeDef,
+    RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef,
     RuleGroupSourceStatefulRulesOptionsDetailsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef,
+    RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef,
+    RuleGroupVariablesIpSetsDetailsOutputTypeDef,
     RuleGroupVariablesIpSetsDetailsTypeDef,
+    RuleGroupVariablesPortSetsDetailsOutputTypeDef,
     RuleGroupVariablesPortSetsDetailsTypeDef,
     SoftwarePackageTypeDef,
     StandardsManagedByTypeDef,
     StandardsStatusReasonTypeDef,
     StatelessCustomPublishMetricActionDimensionTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateActionTargetRequestRequestTypeDef,
     UpdateFindingAggregatorRequestRequestTypeDef,
-    UpdateFindingAggregatorResponseTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
     UpdateSecurityHubConfigurationRequestRequestTypeDef,
     UpdateStandardsControlRequestRequestTypeDef,
     VulnerabilityVendorTypeDef,
     CreateMembersRequestRequestTypeDef,
     ActionRemoteIpDetailsTypeDef,
-    DescribeActionTargetsResponseTypeDef,
+    CvssOutputTypeDef,
     CvssTypeDef,
-    ListOrganizationAdminAccountsResponseTypeDef,
     AssociationSetDetailsTypeDef,
+    AutomationRulesFindingFieldsUpdateOutputTypeDef,
     AutomationRulesFindingFieldsUpdateTypeDef,
-    ListAutomationRulesResponseTypeDef,
     AwsAmazonMqBrokerLogsDetailsTypeDef,
+    AwsApiGatewayRestApiDetailsOutputTypeDef,
     AwsApiGatewayRestApiDetailsTypeDef,
+    AwsApiGatewayStageDetailsOutputTypeDef,
     AwsApiGatewayStageDetailsTypeDef,
+    AwsApiGatewayV2ApiDetailsOutputTypeDef,
     AwsApiGatewayV2ApiDetailsTypeDef,
+    AwsApiGatewayV2StageDetailsOutputTypeDef,
     AwsApiGatewayV2StageDetailsTypeDef,
     AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef,
+    AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef,
     AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef,
+    AwsBackupBackupVaultDetailsOutputTypeDef,
     AwsBackupBackupVaultDetailsTypeDef,
     AwsBackupRecoveryPointDetailsTypeDef,
+    AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef,
     AwsCertificateManagerCertificateDomainValidationOptionTypeDef,
+    AwsCloudFormationStackDetailsOutputTypeDef,
     AwsCloudFormationStackDetailsTypeDef,
+    AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef,
     AwsCloudFrontDistributionCacheBehaviorsTypeDef,
+    AwsCloudFrontDistributionOriginCustomOriginConfigOutputTypeDef,
     AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef,
+    AwsCloudFrontDistributionOriginGroupFailoverOutputTypeDef,
     AwsCloudFrontDistributionOriginGroupFailoverTypeDef,
+    AwsCloudWatchAlarmDetailsOutputTypeDef,
     AwsCloudWatchAlarmDetailsTypeDef,
+    AwsCodeBuildProjectEnvironmentOutputTypeDef,
     AwsCodeBuildProjectEnvironmentTypeDef,
     AwsCodeBuildProjectLogsConfigDetailsTypeDef,
+    AwsDynamoDbTableGlobalSecondaryIndexOutputTypeDef,
+    AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef,
     AwsDynamoDbTableGlobalSecondaryIndexTypeDef,
     AwsDynamoDbTableLocalSecondaryIndexTypeDef,
     AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef,
+    AwsEc2InstanceDetailsOutputTypeDef,
     AwsEc2InstanceDetailsTypeDef,
     AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef,
     AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef,
     AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceRequirementsDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef,
     AwsEc2NetworkAclEntryTypeDef,
+    AwsEc2NetworkInterfaceDetailsOutputTypeDef,
     AwsEc2NetworkInterfaceDetailsTypeDef,
+    AwsEc2SecurityGroupIpPermissionOutputTypeDef,
     AwsEc2SecurityGroupIpPermissionTypeDef,
+    AwsEc2SubnetDetailsOutputTypeDef,
     AwsEc2SubnetDetailsTypeDef,
+    AwsEc2VolumeDetailsOutputTypeDef,
     AwsEc2VolumeDetailsTypeDef,
+    AwsEc2VpcDetailsOutputTypeDef,
     AwsEc2VpcDetailsTypeDef,
+    AwsEc2VpcEndpointServiceDetailsOutputTypeDef,
     AwsEc2VpcEndpointServiceDetailsTypeDef,
+    AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef,
     AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef,
+    AwsEc2VpnConnectionOptionsDetailsOutputTypeDef,
     AwsEc2VpnConnectionOptionsDetailsTypeDef,
     AwsEcrRepositoryDetailsTypeDef,
     AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef,
+    AwsEcsContainerDetailsOutputTypeDef,
     AwsEcsContainerDetailsTypeDef,
     AwsEcsServiceDeploymentConfigurationDetailsTypeDef,
+    AwsEcsServiceNetworkConfigurationDetailsOutputTypeDef,
     AwsEcsServiceNetworkConfigurationDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef,
+    AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef,
     AwsEcsTaskDefinitionProxyConfigurationDetailsTypeDef,
     AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef,
     AwsEcsTaskVolumeDetailsTypeDef,
     AwsEfsAccessPointRootDirectoryDetailsTypeDef,
+    AwsEksClusterLoggingDetailsOutputTypeDef,
     AwsEksClusterLoggingDetailsTypeDef,
+    AwsElasticBeanstalkEnvironmentDetailsOutputTypeDef,
     AwsElasticBeanstalkEnvironmentDetailsTypeDef,
     AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef,
     AwsElasticsearchDomainLogPublishingOptionsTypeDef,
+    AwsElbLoadBalancerPoliciesOutputTypeDef,
     AwsElbLoadBalancerPoliciesTypeDef,
+    AwsElbLoadBalancerAttributesOutputTypeDef,
     AwsElbLoadBalancerAttributesTypeDef,
+    AwsElbLoadBalancerListenerDescriptionOutputTypeDef,
     AwsElbLoadBalancerListenerDescriptionTypeDef,
+    AwsElbv2LoadBalancerDetailsOutputTypeDef,
     AwsElbv2LoadBalancerDetailsTypeDef,
     AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef,
     AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef,
     AwsIamAccessKeySessionContextTypeDef,
+    AwsIamGroupDetailsOutputTypeDef,
     AwsIamGroupDetailsTypeDef,
+    AwsIamInstanceProfileOutputTypeDef,
     AwsIamInstanceProfileTypeDef,
+    AwsIamPolicyDetailsOutputTypeDef,
     AwsIamPolicyDetailsTypeDef,
+    AwsIamUserDetailsOutputTypeDef,
     AwsIamUserDetailsTypeDef,
     AwsKinesisStreamDetailsTypeDef,
+    AwsLambdaFunctionEnvironmentOutputTypeDef,
     AwsLambdaFunctionEnvironmentTypeDef,
+    AwsNetworkFirewallFirewallDetailsOutputTypeDef,
     AwsNetworkFirewallFirewallDetailsTypeDef,
     AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef,
     AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef,
     AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef,
+    AwsRdsDbClusterDetailsOutputTypeDef,
     AwsRdsDbClusterDetailsTypeDef,
+    AwsRdsDbSnapshotDetailsOutputTypeDef,
     AwsRdsDbSnapshotDetailsTypeDef,
+    AwsRdsDbPendingModifiedValuesOutputTypeDef,
     AwsRdsDbPendingModifiedValuesTypeDef,
+    AwsRdsDbSecurityGroupDetailsOutputTypeDef,
     AwsRdsDbSecurityGroupDetailsTypeDef,
     AwsRdsDbSubnetGroupSubnetTypeDef,
+    AwsRedshiftClusterClusterParameterGroupOutputTypeDef,
     AwsRedshiftClusterClusterParameterGroupTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef,
+    AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef,
     AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef,
     AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef,
     AwsS3BucketServerSideEncryptionRuleTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef,
+    AwsSageMakerNotebookInstanceDetailsOutputTypeDef,
     AwsSageMakerNotebookInstanceDetailsTypeDef,
     AwsSecretsManagerSecretDetailsTypeDef,
     BatchUpdateFindingsRequestRequestTypeDef,
     BatchUpdateFindingsUnprocessedFindingTypeDef,
-    GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
-    GetFindingHistoryRequestRequestTypeDef,
+    AwsSnsTopicDetailsOutputTypeDef,
     AwsSnsTopicDetailsTypeDef,
     AwsSsmPatchTypeDef,
     AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef,
+    AwsWafRateBasedRuleDetailsOutputTypeDef,
     AwsWafRateBasedRuleDetailsTypeDef,
+    AwsWafRegionalRateBasedRuleDetailsOutputTypeDef,
     AwsWafRegionalRateBasedRuleDetailsTypeDef,
+    AwsWafRegionalRuleDetailsOutputTypeDef,
     AwsWafRegionalRuleDetailsTypeDef,
     AwsWafRegionalRuleGroupRulesDetailsTypeDef,
     AwsWafRegionalWebAclRulesListDetailsTypeDef,
+    AwsWafRuleDetailsOutputTypeDef,
     AwsWafRuleDetailsTypeDef,
     AwsWafRuleGroupRulesDetailsTypeDef,
+    AwsWafWebAclRuleOutputTypeDef,
     AwsWafWebAclRuleTypeDef,
+    AwsWafv2CustomRequestHandlingDetailsOutputTypeDef,
     AwsWafv2CustomRequestHandlingDetailsTypeDef,
+    AwsWafv2CustomResponseDetailsOutputTypeDef,
     AwsWafv2CustomResponseDetailsTypeDef,
     AwsWafv2WebAclCaptchaConfigDetailsTypeDef,
+    CreateActionTargetResponseTypeDef,
+    CreateAutomationRuleResponseTypeDef,
+    CreateFindingAggregatorResponseTypeDef,
+    CreateInsightResponseTypeDef,
+    DeleteActionTargetResponseTypeDef,
+    DeleteInsightResponseTypeDef,
+    DescribeActionTargetsResponseTypeDef,
+    DescribeHubResponseTypeDef,
+    DescribeOrganizationConfigurationResponseTypeDef,
+    EnableImportFindingsForProductResponseTypeDef,
+    GetFindingAggregatorResponseTypeDef,
+    GetInvitationsCountResponseTypeDef,
+    ListAutomationRulesResponseTypeDef,
+    ListEnabledProductsForImportResponseTypeDef,
+    ListOrganizationAdminAccountsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateFindingAggregatorResponseTypeDef,
     BatchDeleteAutomationRulesResponseTypeDef,
     BatchUpdateAutomationRulesResponseTypeDef,
     BatchEnableStandardsRequestRequestTypeDef,
     BatchGetSecurityControlsResponseTypeDef,
     BatchGetStandardsControlAssociationsRequestRequestTypeDef,
     UnprocessedStandardsControlAssociationTypeDef,
     BatchImportFindingsResponseTypeDef,
     BatchUpdateStandardsControlAssociationsRequestRequestTypeDef,
     UnprocessedStandardsControlAssociationUpdateTypeDef,
+    ComplianceOutputTypeDef,
     ComplianceTypeDef,
+    ContainerDetailsOutputTypeDef,
     ContainerDetailsTypeDef,
     CreateMembersResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     DeleteMembersResponseTypeDef,
     InviteMembersResponseTypeDef,
     DateFilterTypeDef,
+    DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef,
+    DescribeProductsRequestDescribeProductsPaginateTypeDef,
+    DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
+    DescribeStandardsRequestDescribeStandardsPaginateTypeDef,
+    GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef,
+    GetInsightsRequestGetInsightsPaginateTypeDef,
+    ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef,
+    ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef,
+    ListInvitationsRequestListInvitationsPaginateTypeDef,
+    ListMembersRequestListMembersPaginateTypeDef,
+    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
+    ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef,
+    ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef,
     DescribeProductsResponseTypeDef,
     DescribeStandardsControlsResponseTypeDef,
+    ThreatOutputTypeDef,
     ThreatTypeDef,
     ListFindingAggregatorsResponseTypeDef,
     FindingHistoryRecordTypeDef,
+    FindingProviderFieldsOutputTypeDef,
     FindingProviderFieldsTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetMasterAccountResponseTypeDef,
     ListInvitationsResponseTypeDef,
+    GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
+    GetFindingHistoryRequestRequestTypeDef,
     GetMembersResponseTypeDef,
     ListMembersResponseTypeDef,
     InsightResultsTypeDef,
     ListSecurityControlDefinitionsResponseTypeDef,
     ListStandardsControlAssociationsResponseTypeDef,
+    NetworkPathComponentDetailsOutputTypeDef,
     NetworkPathComponentDetailsTypeDef,
     NetworkTypeDef,
     PageTypeDef,
     RemediationTypeDef,
+    RuleGroupSourceStatefulRulesDetailsOutputTypeDef,
     RuleGroupSourceStatefulRulesDetailsTypeDef,
+    RuleGroupSourceStatelessRuleMatchAttributesOutputTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesTypeDef,
+    RuleGroupVariablesOutputTypeDef,
     RuleGroupVariablesTypeDef,
     StandardTypeDef,
     StandardsSubscriptionTypeDef,
+    StatelessCustomPublishMetricActionOutputTypeDef,
     StatelessCustomPublishMetricActionTypeDef,
+    AwsApiCallActionOutputTypeDef,
     AwsApiCallActionTypeDef,
     NetworkConnectionActionTypeDef,
     PortProbeDetailTypeDef,
+    VulnerabilityOutputTypeDef,
     VulnerabilityTypeDef,
+    AwsEc2RouteTableDetailsOutputTypeDef,
     AwsEc2RouteTableDetailsTypeDef,
+    AutomationRulesActionOutputTypeDef,
     AutomationRulesActionTypeDef,
+    AwsAmazonMqBrokerDetailsOutputTypeDef,
     AwsAmazonMqBrokerDetailsTypeDef,
+    AwsAppSyncGraphQlApiDetailsOutputTypeDef,
     AwsAppSyncGraphQlApiDetailsTypeDef,
+    AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef,
+    AwsAutoScalingLaunchConfigurationDetailsOutputTypeDef,
     AwsAutoScalingLaunchConfigurationDetailsTypeDef,
+    AwsBackupBackupPlanRuleDetailsOutputTypeDef,
     AwsBackupBackupPlanRuleDetailsTypeDef,
+    AwsCertificateManagerCertificateRenewalSummaryOutputTypeDef,
     AwsCertificateManagerCertificateRenewalSummaryTypeDef,
+    AwsCloudFrontDistributionOriginItemOutputTypeDef,
     AwsCloudFrontDistributionOriginItemTypeDef,
+    AwsCloudFrontDistributionOriginGroupOutputTypeDef,
     AwsCloudFrontDistributionOriginGroupTypeDef,
+    AwsCodeBuildProjectDetailsOutputTypeDef,
     AwsCodeBuildProjectDetailsTypeDef,
+    AwsDynamoDbTableReplicaOutputTypeDef,
     AwsDynamoDbTableReplicaTypeDef,
+    AwsEc2LaunchTemplateDataDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataDetailsTypeDef,
+    AwsEc2NetworkAclDetailsOutputTypeDef,
     AwsEc2NetworkAclDetailsTypeDef,
+    AwsEc2SecurityGroupDetailsOutputTypeDef,
     AwsEc2SecurityGroupDetailsTypeDef,
+    AwsEc2VpcPeeringConnectionDetailsOutputTypeDef,
     AwsEc2VpcPeeringConnectionDetailsTypeDef,
+    AwsEc2VpnConnectionDetailsOutputTypeDef,
     AwsEc2VpnConnectionDetailsTypeDef,
     AwsEcsClusterConfigurationDetailsTypeDef,
+    AwsEcsServiceDetailsOutputTypeDef,
     AwsEcsServiceDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef,
+    AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef,
     AwsEcsTaskDefinitionVolumesDetailsTypeDef,
+    AwsEcsTaskDetailsOutputTypeDef,
     AwsEcsTaskDetailsTypeDef,
+    AwsEfsAccessPointDetailsOutputTypeDef,
     AwsEfsAccessPointDetailsTypeDef,
+    AwsEksClusterDetailsOutputTypeDef,
     AwsEksClusterDetailsTypeDef,
+    AwsElasticsearchDomainDetailsOutputTypeDef,
     AwsElasticsearchDomainDetailsTypeDef,
+    AwsElbLoadBalancerDetailsOutputTypeDef,
     AwsElbLoadBalancerDetailsTypeDef,
     AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef,
     AwsIamAccessKeyDetailsTypeDef,
+    AwsIamRoleDetailsOutputTypeDef,
     AwsIamRoleDetailsTypeDef,
+    AwsLambdaFunctionDetailsOutputTypeDef,
     AwsLambdaFunctionDetailsTypeDef,
+    AwsOpenSearchServiceDomainDetailsOutputTypeDef,
     AwsOpenSearchServiceDomainDetailsTypeDef,
+    AwsRdsDbSubnetGroupOutputTypeDef,
     AwsRdsDbSubnetGroupTypeDef,
+    AwsRedshiftClusterDetailsOutputTypeDef,
     AwsRedshiftClusterDetailsTypeDef,
+    AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef,
+    AwsS3BucketNotificationConfigurationFilterOutputTypeDef,
     AwsS3BucketNotificationConfigurationFilterTypeDef,
     AwsS3BucketObjectLockConfigurationTypeDef,
+    AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef,
     AwsS3BucketServerSideEncryptionConfigurationTypeDef,
+    AwsS3BucketWebsiteConfigurationOutputTypeDef,
     AwsS3BucketWebsiteConfigurationTypeDef,
     BatchUpdateFindingsResponseTypeDef,
     AwsSsmPatchComplianceDetailsTypeDef,
+    AwsStepFunctionStateMachineLoggingConfigurationDetailsOutputTypeDef,
     AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef,
+    AwsWafRegionalRuleGroupDetailsOutputTypeDef,
     AwsWafRegionalRuleGroupDetailsTypeDef,
+    AwsWafRegionalWebAclDetailsOutputTypeDef,
     AwsWafRegionalWebAclDetailsTypeDef,
+    AwsWafRuleGroupDetailsOutputTypeDef,
     AwsWafRuleGroupDetailsTypeDef,
+    AwsWafWebAclDetailsOutputTypeDef,
     AwsWafWebAclDetailsTypeDef,
+    AwsWafv2ActionAllowDetailsOutputTypeDef,
+    AwsWafv2RulesActionCaptchaDetailsOutputTypeDef,
+    AwsWafv2RulesActionCountDetailsOutputTypeDef,
     AwsWafv2ActionAllowDetailsTypeDef,
     AwsWafv2RulesActionCaptchaDetailsTypeDef,
     AwsWafv2RulesActionCountDetailsTypeDef,
+    AwsWafv2ActionBlockDetailsOutputTypeDef,
     AwsWafv2ActionBlockDetailsTypeDef,
     BatchGetStandardsControlAssociationsResponseTypeDef,
     BatchUpdateStandardsControlAssociationsResponseTypeDef,
+    AutomationRulesFindingFiltersOutputTypeDef,
     AutomationRulesFindingFiltersTypeDef,
+    AwsSecurityFindingFiltersOutputTypeDef,
     AwsSecurityFindingFiltersTypeDef,
     GetFindingHistoryResponseTypeDef,
     GetInsightResultsResponseTypeDef,
+    NetworkHeaderOutputTypeDef,
     NetworkHeaderTypeDef,
+    OccurrencesOutputTypeDef,
     OccurrencesTypeDef,
+    RuleGroupSourceStatelessRuleDefinitionOutputTypeDef,
     RuleGroupSourceStatelessRuleDefinitionTypeDef,
     DescribeStandardsResponseTypeDef,
     BatchDisableStandardsResponseTypeDef,
     BatchEnableStandardsResponseTypeDef,
     GetEnabledStandardsResponseTypeDef,
+    StatelessCustomActionDefinitionOutputTypeDef,
     StatelessCustomActionDefinitionTypeDef,
+    PortProbeActionOutputTypeDef,
     PortProbeActionTypeDef,
+    AutomationRulesActionUnionTypeDef,
+    AwsAutoScalingAutoScalingGroupDetailsOutputTypeDef,
     AwsAutoScalingAutoScalingGroupDetailsTypeDef,
+    AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef,
     AwsBackupBackupPlanBackupPlanDetailsTypeDef,
+    AwsCertificateManagerCertificateDetailsOutputTypeDef,
     AwsCertificateManagerCertificateDetailsTypeDef,
+    AwsCloudFrontDistributionOriginsOutputTypeDef,
     AwsCloudFrontDistributionOriginsTypeDef,
+    AwsCloudFrontDistributionOriginGroupsOutputTypeDef,
     AwsCloudFrontDistributionOriginGroupsTypeDef,
+    AwsDynamoDbTableDetailsOutputTypeDef,
     AwsDynamoDbTableDetailsTypeDef,
+    AwsEc2LaunchTemplateDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDetailsTypeDef,
+    AwsEcsClusterDetailsOutputTypeDef,
     AwsEcsClusterDetailsTypeDef,
+    AwsEcsTaskDefinitionDetailsOutputTypeDef,
     AwsEcsTaskDefinitionDetailsTypeDef,
     AwsGuardDutyDetectorDataSourcesDetailsTypeDef,
+    AwsRdsDbInstanceDetailsOutputTypeDef,
     AwsRdsDbInstanceDetailsTypeDef,
+    AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef,
+    AwsS3BucketNotificationConfigurationDetailOutputTypeDef,
     AwsS3BucketNotificationConfigurationDetailTypeDef,
+    AwsStepFunctionStateMachineDetailsOutputTypeDef,
     AwsStepFunctionStateMachineDetailsTypeDef,
+    AwsWafv2RulesActionDetailsOutputTypeDef,
+    AwsWafv2WebAclActionDetailsOutputTypeDef,
     AwsWafv2RulesActionDetailsTypeDef,
     AwsWafv2WebAclActionDetailsTypeDef,
     AutomationRulesConfigTypeDef,
-    CreateAutomationRuleRequestRequestTypeDef,
+    AutomationRulesFindingFiltersUnionTypeDef,
     UpdateAutomationRulesRequestItemTypeDef,
+    InsightTypeDef,
+    AwsSecurityFindingFiltersUnionTypeDef,
     CreateInsightRequestRequestTypeDef,
     GetFindingsRequestGetFindingsPaginateTypeDef,
     GetFindingsRequestRequestTypeDef,
-    InsightTypeDef,
     UpdateFindingsRequestRequestTypeDef,
     UpdateInsightRequestRequestTypeDef,
+    NetworkPathComponentOutputTypeDef,
     NetworkPathComponentTypeDef,
+    CustomDataIdentifiersDetectionsOutputTypeDef,
+    SensitiveDataDetectionsOutputTypeDef,
     CustomDataIdentifiersDetectionsTypeDef,
     SensitiveDataDetectionsTypeDef,
+    RuleGroupSourceStatelessRulesDetailsOutputTypeDef,
     RuleGroupSourceStatelessRulesDetailsTypeDef,
+    FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef,
+    RuleGroupSourceCustomActionsDetailsOutputTypeDef,
     FirewallPolicyStatelessCustomActionsDetailsTypeDef,
     RuleGroupSourceCustomActionsDetailsTypeDef,
+    ActionOutputTypeDef,
     ActionTypeDef,
+    CreateAutomationRuleRequestRequestTypeDef,
+    AwsBackupBackupPlanDetailsOutputTypeDef,
     AwsBackupBackupPlanDetailsTypeDef,
+    AwsCloudFrontDistributionDetailsOutputTypeDef,
     AwsCloudFrontDistributionDetailsTypeDef,
+    AwsGuardDutyDetectorDetailsOutputTypeDef,
     AwsGuardDutyDetectorDetailsTypeDef,
+    AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef,
+    AwsS3BucketNotificationConfigurationOutputTypeDef,
     AwsS3BucketNotificationConfigurationTypeDef,
+    AwsWafv2RulesDetailsOutputTypeDef,
     AwsWafv2RulesDetailsTypeDef,
     BatchGetAutomationRulesResponseTypeDef,
     BatchUpdateAutomationRulesRequestRequestTypeDef,
     GetInsightsResponseTypeDef,
+    CustomDataIdentifiersResultOutputTypeDef,
+    SensitiveDataResultOutputTypeDef,
     CustomDataIdentifiersResultTypeDef,
     SensitiveDataResultTypeDef,
+    FirewallPolicyDetailsOutputTypeDef,
+    RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef,
     FirewallPolicyDetailsTypeDef,
     RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef,
+    AwsS3BucketBucketLifecycleConfigurationDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef,
+    AwsWafv2RuleGroupDetailsOutputTypeDef,
+    AwsWafv2WebAclDetailsOutputTypeDef,
     AwsWafv2RuleGroupDetailsTypeDef,
     AwsWafv2WebAclDetailsTypeDef,
+    ClassificationResultOutputTypeDef,
     ClassificationResultTypeDef,
+    AwsNetworkFirewallFirewallPolicyDetailsOutputTypeDef,
+    RuleGroupSourceOutputTypeDef,
     AwsNetworkFirewallFirewallPolicyDetailsTypeDef,
     RuleGroupSourceTypeDef,
+    AwsS3BucketDetailsOutputTypeDef,
     AwsS3BucketDetailsTypeDef,
+    DataClassificationDetailsOutputTypeDef,
     DataClassificationDetailsTypeDef,
+    RuleGroupDetailsOutputTypeDef,
     RuleGroupDetailsTypeDef,
+    AwsNetworkFirewallRuleGroupDetailsOutputTypeDef,
     AwsNetworkFirewallRuleGroupDetailsTypeDef,
+    ResourceDetailsOutputTypeDef,
     ResourceDetailsTypeDef,
+    ResourceOutputTypeDef,
     ResourceTypeDef,
+    AwsSecurityFindingOutputTypeDef,
     AwsSecurityFindingTypeDef,
-    BatchImportFindingsRequestRequestTypeDef,
     GetFindingsResponseTypeDef,
+    AwsSecurityFindingUnionTypeDef,
+    BatchImportFindingsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AcceptAdministratorInvitationRequestRequestTypeDef:
+def get_value() -> AcceptAdministratorInvitationRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-securityhub-2.5.2/README.md` & `types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-securityhub
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SecurityHub 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore securityhub type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-securityhub"></a>
 
 # types-aiobotocore-securityhub
 
 [![PyPI - types-aiobotocore-securityhub](https://img.shields.io/pypi/v/types-aiobotocore-securityhub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-securityhub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-securityhub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-securityhub)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-securityhub?color=blue)](https://pypistats.org/packages/types-aiobotocore-securityhub)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-securityhub)](https://pepy.tech/project/types-aiobotocore-securityhub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SecurityHub 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
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
 [types-aiobotocore-securityhub docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/).
 
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
@@ -371,107 +403,117 @@
 )
 
 
 def check_value(value: AdminStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_securityhub.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_securityhub.type_defs import (
     AcceptAdministratorInvitationRequestRequestTypeDef,
     AcceptInvitationRequestRequestTypeDef,
     AccountDetailsTypeDef,
     ActionLocalIpDetailsTypeDef,
     ActionLocalPortDetailsTypeDef,
+    DnsRequestActionTypeDef,
     CityTypeDef,
     CountryTypeDef,
     GeoLocationTypeDef,
     IpOrganizationDetailsTypeDef,
     ActionRemotePortDetailsTypeDef,
     ActionTargetTypeDef,
-    DnsRequestActionTypeDef,
     AdjustmentTypeDef,
     AdminAccountTypeDef,
     AssociatedStandardTypeDef,
     AssociationStateDetailsTypeDef,
     NoteUpdateTypeDef,
     RelatedFindingTypeDef,
     SeverityUpdateTypeDef,
     WorkflowUpdateTypeDef,
     MapFilterTypeDef,
     NumberFilterTypeDef,
     StringFilterTypeDef,
     AutomationRulesMetadataTypeDef,
     AvailabilityZoneTypeDef,
     AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef,
-    AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef,
+    AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef,
     AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef,
     AwsAmazonMqBrokerUsersDetailsTypeDef,
+    AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef,
     AwsAmazonMqBrokerLogsPendingDetailsTypeDef,
     AwsApiCallActionDomainDetailsTypeDef,
     AwsApiGatewayAccessLogSettingsTypeDef,
+    AwsApiGatewayCanarySettingsOutputTypeDef,
     AwsApiGatewayCanarySettingsTypeDef,
+    AwsApiGatewayEndpointConfigurationOutputTypeDef,
     AwsApiGatewayEndpointConfigurationTypeDef,
     AwsApiGatewayMethodSettingsTypeDef,
+    AwsCorsConfigurationOutputTypeDef,
     AwsCorsConfigurationTypeDef,
     AwsApiGatewayV2RouteSettingsTypeDef,
     AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef,
     AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef,
     AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef,
     AwsAppSyncGraphQlApiLogConfigDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationMetadataOptionsTypeDef,
+    AwsBackupBackupPlanAdvancedBackupSettingsDetailsOutputTypeDef,
     AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef,
     AwsBackupBackupPlanLifecycleDetailsTypeDef,
+    AwsBackupBackupVaultNotificationsDetailsOutputTypeDef,
     AwsBackupBackupVaultNotificationsDetailsTypeDef,
     AwsBackupRecoveryPointCalculatedLifecycleDetailsTypeDef,
     AwsBackupRecoveryPointCreatedByDetailsTypeDef,
     AwsBackupRecoveryPointLifecycleDetailsTypeDef,
     AwsCertificateManagerCertificateExtendedKeyUsageTypeDef,
     AwsCertificateManagerCertificateKeyUsageTypeDef,
     AwsCertificateManagerCertificateOptionsTypeDef,
     AwsCertificateManagerCertificateResourceRecordTypeDef,
     AwsCloudFormationStackDriftInformationDetailsTypeDef,
     AwsCloudFormationStackOutputsDetailsTypeDef,
     AwsCloudFrontDistributionCacheBehaviorTypeDef,
     AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef,
     AwsCloudFrontDistributionLoggingTypeDef,
     AwsCloudFrontDistributionViewerCertificateTypeDef,
+    AwsCloudFrontDistributionOriginSslProtocolsOutputTypeDef,
     AwsCloudFrontDistributionOriginSslProtocolsTypeDef,
+    AwsCloudFrontDistributionOriginGroupFailoverStatusCodesOutputTypeDef,
     AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef,
     AwsCloudFrontDistributionOriginS3OriginConfigTypeDef,
     AwsCloudTrailTrailDetailsTypeDef,
     AwsCloudWatchAlarmDimensionsDetailsTypeDef,
     AwsCodeBuildProjectArtifactsDetailsTypeDef,
     AwsCodeBuildProjectSourceTypeDef,
+    AwsCodeBuildProjectVpcConfigOutputTypeDef,
     AwsCodeBuildProjectVpcConfigTypeDef,
     AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef,
     AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef,
     AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef,
     AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef,
     AwsDynamoDbTableAttributeDefinitionTypeDef,
     AwsDynamoDbTableBillingModeSummaryTypeDef,
     AwsDynamoDbTableKeySchemaTypeDef,
     AwsDynamoDbTableProvisionedThroughputTypeDef,
     AwsDynamoDbTableRestoreSummaryTypeDef,
     AwsDynamoDbTableSseDescriptionTypeDef,
     AwsDynamoDbTableStreamSpecificationTypeDef,
+    AwsDynamoDbTableProjectionOutputTypeDef,
     AwsDynamoDbTableProjectionTypeDef,
     AwsDynamoDbTableProvisionedThroughputOverrideTypeDef,
     AwsEc2EipDetailsTypeDef,
     AwsEc2InstanceMetadataOptionsTypeDef,
     AwsEc2InstanceMonitoringDetailsTypeDef,
     AwsEc2InstanceNetworkInterfacesDetailsTypeDef,
     AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef,
@@ -512,86 +554,101 @@
     PropagatingVgwSetDetailsTypeDef,
     RouteSetDetailsTypeDef,
     AwsEc2SecurityGroupIpRangeTypeDef,
     AwsEc2SecurityGroupIpv6RangeTypeDef,
     AwsEc2SecurityGroupPrefixListIdTypeDef,
     AwsEc2SecurityGroupUserIdGroupPairTypeDef,
     Ipv6CidrBlockAssociationTypeDef,
+    AwsEc2TransitGatewayDetailsOutputTypeDef,
     AwsEc2TransitGatewayDetailsTypeDef,
     AwsEc2VolumeAttachmentTypeDef,
     CidrBlockAssociationTypeDef,
     AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef,
     AwsEc2VpcPeeringConnectionStatusDetailsTypeDef,
     VpcInfoCidrBlockSetDetailsTypeDef,
     VpcInfoIpv6CidrBlockSetDetailsTypeDef,
     VpcInfoPeeringOptionsDetailsTypeDef,
     AwsEc2VpnConnectionRoutesDetailsTypeDef,
     AwsEc2VpnConnectionVgwTelemetryDetailsTypeDef,
+    AwsEc2VpnConnectionOptionsTunnelOptionsDetailsOutputTypeDef,
     AwsEc2VpnConnectionOptionsTunnelOptionsDetailsTypeDef,
+    AwsEcrContainerImageDetailsOutputTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     AwsEcrRepositoryImageScanningConfigurationDetailsTypeDef,
     AwsEcrRepositoryLifecyclePolicyDetailsTypeDef,
     AwsEcsClusterClusterSettingsDetailsTypeDef,
     AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef,
     AwsEcsClusterDefaultCapacityProviderStrategyDetailsTypeDef,
     AwsMountPointTypeDef,
     AwsEcsServiceCapacityProviderStrategyDetailsTypeDef,
     AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef,
     AwsEcsServiceDeploymentControllerDetailsTypeDef,
     AwsEcsServiceLoadBalancersDetailsTypeDef,
     AwsEcsServicePlacementConstraintsDetailsTypeDef,
     AwsEcsServicePlacementStrategiesDetailsTypeDef,
     AwsEcsServiceServiceRegistriesDetailsTypeDef,
+    AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsOutputTypeDef,
     AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsOutputTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef,
     AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef,
     AwsEcsTaskDefinitionPlacementConstraintsDetailsTypeDef,
     AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef,
-    AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef,
+    AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsOutputTypeDef,
     AwsEcsTaskDefinitionVolumesHostDetailsTypeDef,
+    AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef,
     AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef,
     AwsEcsTaskVolumeHostDetailsTypeDef,
+    AwsEfsAccessPointPosixUserDetailsOutputTypeDef,
     AwsEfsAccessPointPosixUserDetailsTypeDef,
     AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef,
+    AwsEksClusterResourcesVpcConfigDetailsOutputTypeDef,
     AwsEksClusterResourcesVpcConfigDetailsTypeDef,
+    AwsEksClusterLoggingClusterLoggingDetailsOutputTypeDef,
     AwsEksClusterLoggingClusterLoggingDetailsTypeDef,
     AwsElasticBeanstalkEnvironmentEnvironmentLinkTypeDef,
     AwsElasticBeanstalkEnvironmentOptionSettingTypeDef,
     AwsElasticBeanstalkEnvironmentTierTypeDef,
     AwsElasticsearchDomainDomainEndpointOptionsTypeDef,
     AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef,
     AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef,
     AwsElasticsearchDomainServiceSoftwareOptionsTypeDef,
+    AwsElasticsearchDomainVPCOptionsOutputTypeDef,
     AwsElasticsearchDomainVPCOptionsTypeDef,
     AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef,
     AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef,
     AwsElbAppCookieStickinessPolicyTypeDef,
     AwsElbLbCookieStickinessPolicyTypeDef,
     AwsElbLoadBalancerAccessLogTypeDef,
     AwsElbLoadBalancerAdditionalAttributeTypeDef,
     AwsElbLoadBalancerConnectionDrainingTypeDef,
     AwsElbLoadBalancerConnectionSettingsTypeDef,
     AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef,
+    AwsElbLoadBalancerBackendServerDescriptionOutputTypeDef,
     AwsElbLoadBalancerBackendServerDescriptionTypeDef,
     AwsElbLoadBalancerHealthCheckTypeDef,
     AwsElbLoadBalancerInstanceTypeDef,
     AwsElbLoadBalancerSourceSecurityGroupTypeDef,
     AwsElbLoadBalancerListenerTypeDef,
     AwsElbv2LoadBalancerAttributeTypeDef,
     LoadBalancerStateTypeDef,
@@ -614,42 +671,48 @@
     AwsIamUserPolicyTypeDef,
     AwsKinesisStreamStreamEncryptionDetailsTypeDef,
     AwsKmsKeyDetailsTypeDef,
     AwsLambdaFunctionCodeTypeDef,
     AwsLambdaFunctionDeadLetterConfigTypeDef,
     AwsLambdaFunctionLayerTypeDef,
     AwsLambdaFunctionTracingConfigTypeDef,
+    AwsLambdaFunctionVpcConfigOutputTypeDef,
     AwsLambdaFunctionVpcConfigTypeDef,
     AwsLambdaFunctionEnvironmentErrorTypeDef,
+    AwsLambdaLayerVersionDetailsOutputTypeDef,
     AwsLambdaLayerVersionDetailsTypeDef,
     AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef,
     AwsOpenSearchServiceDomainMasterUserOptionsDetailsTypeDef,
     AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef,
     AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef,
     AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsTypeDef,
     AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsTypeDef,
     AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsTypeDef,
+    AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef,
     AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef,
     AwsOpenSearchServiceDomainLogPublishingOptionTypeDef,
     AwsRdsDbClusterAssociatedRoleTypeDef,
     AwsRdsDbClusterMemberTypeDef,
     AwsRdsDbClusterOptionGroupMembershipTypeDef,
     AwsRdsDbDomainMembershipTypeDef,
     AwsRdsDbInstanceVpcSecurityGroupTypeDef,
+    AwsRdsDbClusterSnapshotDetailsOutputTypeDef,
     AwsRdsDbClusterSnapshotDetailsTypeDef,
     AwsRdsDbInstanceAssociatedRoleTypeDef,
     AwsRdsDbInstanceEndpointTypeDef,
     AwsRdsDbOptionGroupMembershipTypeDef,
     AwsRdsDbParameterGroupTypeDef,
     AwsRdsDbProcessorFeatureTypeDef,
     AwsRdsDbStatusInfoTypeDef,
+    AwsRdsPendingCloudWatchLogsExportsOutputTypeDef,
     AwsRdsPendingCloudWatchLogsExportsTypeDef,
     AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef,
     AwsRdsDbSecurityGroupIpRangeTypeDef,
     AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef,
+    AwsRdsEventSubscriptionDetailsOutputTypeDef,
     AwsRdsEventSubscriptionDetailsTypeDef,
     AwsRedshiftClusterClusterNodeTypeDef,
     AwsRedshiftClusterClusterParameterStatusTypeDef,
     AwsRedshiftClusterClusterSecurityGroupTypeDef,
     AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef,
     AwsRedshiftClusterDeferredMaintenanceWindowTypeDef,
     AwsRedshiftClusterElasticIpStatusTypeDef,
@@ -706,14 +769,15 @@
     WafExcludedRuleTypeDef,
     WafOverrideActionTypeDef,
     AwsWafv2CustomHttpHeaderTypeDef,
     AwsWafv2VisibilityConfigDetailsTypeDef,
     AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef,
     AwsXrayEncryptionConfigDetailsTypeDef,
     BatchDeleteAutomationRulesRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UnprocessedAutomationRuleTypeDef,
     BatchDisableStandardsRequestRequestTypeDef,
     StandardsSubscriptionRequestTypeDef,
     BatchGetAutomationRulesRequestRequestTypeDef,
     BatchGetSecurityControlsRequestRequestTypeDef,
     SecurityControlTypeDef,
     UnprocessedSecurityControlTypeDef,
@@ -722,400 +786,575 @@
     ImportFindingsErrorTypeDef,
     StandardsControlAssociationUpdateTypeDef,
     CellTypeDef,
     ClassificationStatusTypeDef,
     StatusReasonTypeDef,
     VolumeMountTypeDef,
     CreateActionTargetRequestRequestTypeDef,
-    CreateActionTargetResponseTypeDef,
-    CreateAutomationRuleResponseTypeDef,
     CreateFindingAggregatorRequestRequestTypeDef,
-    CreateFindingAggregatorResponseTypeDef,
-    CreateInsightResponseTypeDef,
     ResultTypeDef,
     DateRangeTypeDef,
     DeclineInvitationsRequestRequestTypeDef,
     DeleteActionTargetRequestRequestTypeDef,
-    DeleteActionTargetResponseTypeDef,
     DeleteFindingAggregatorRequestRequestTypeDef,
     DeleteInsightRequestRequestTypeDef,
-    DeleteInsightResponseTypeDef,
     DeleteInvitationsRequestRequestTypeDef,
     DeleteMembersRequestRequestTypeDef,
-    DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeActionTargetsRequestRequestTypeDef,
     DescribeHubRequestRequestTypeDef,
-    DescribeHubResponseTypeDef,
-    DescribeOrganizationConfigurationResponseTypeDef,
-    DescribeProductsRequestDescribeProductsPaginateTypeDef,
     DescribeProductsRequestRequestTypeDef,
     ProductTypeDef,
-    DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
     DescribeStandardsControlsRequestRequestTypeDef,
     StandardsControlTypeDef,
-    DescribeStandardsRequestDescribeStandardsPaginateTypeDef,
     DescribeStandardsRequestRequestTypeDef,
     DisableImportFindingsForProductRequestRequestTypeDef,
     DisableOrganizationAdminAccountRequestRequestTypeDef,
     DisassociateMembersRequestRequestTypeDef,
     EnableImportFindingsForProductRequestRequestTypeDef,
-    EnableImportFindingsForProductResponseTypeDef,
     EnableOrganizationAdminAccountRequestRequestTypeDef,
     EnableSecurityHubRequestRequestTypeDef,
     FilePathsTypeDef,
     FindingAggregatorTypeDef,
     FindingHistoryUpdateSourceTypeDef,
     FindingHistoryUpdateTypeDef,
     FindingProviderSeverityTypeDef,
     FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef,
     FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef,
     InvitationTypeDef,
-    GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef,
     GetEnabledStandardsRequestRequestTypeDef,
     GetFindingAggregatorRequestRequestTypeDef,
-    GetFindingAggregatorResponseTypeDef,
+    TimestampTypeDef,
     SortCriterionTypeDef,
     GetInsightResultsRequestRequestTypeDef,
-    GetInsightsRequestGetInsightsPaginateTypeDef,
     GetInsightsRequestRequestTypeDef,
-    GetInvitationsCountResponseTypeDef,
     GetMembersRequestRequestTypeDef,
     MemberTypeDef,
     InsightResultValueTypeDef,
     InviteMembersRequestRequestTypeDef,
     ListAutomationRulesRequestRequestTypeDef,
-    ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef,
     ListEnabledProductsForImportRequestRequestTypeDef,
-    ListEnabledProductsForImportResponseTypeDef,
-    ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef,
     ListFindingAggregatorsRequestRequestTypeDef,
-    ListInvitationsRequestListInvitationsPaginateTypeDef,
     ListInvitationsRequestRequestTypeDef,
-    ListMembersRequestListMembersPaginateTypeDef,
     ListMembersRequestRequestTypeDef,
-    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
     ListOrganizationAdminAccountsRequestRequestTypeDef,
-    ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef,
     ListSecurityControlDefinitionsRequestRequestTypeDef,
     SecurityControlDefinitionTypeDef,
-    ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef,
     ListStandardsControlAssociationsRequestRequestTypeDef,
     StandardsControlAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PortRangeTypeDef,
     RangeTypeDef,
     RecordTypeDef,
-    PaginatorConfigTypeDef,
     RecommendationTypeDef,
-    ResponseMetadataTypeDef,
+    RuleGroupSourceListDetailsOutputTypeDef,
     RuleGroupSourceListDetailsTypeDef,
     RuleGroupSourceStatefulRulesHeaderDetailsTypeDef,
+    RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef,
     RuleGroupSourceStatefulRulesOptionsDetailsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef,
+    RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef,
+    RuleGroupVariablesIpSetsDetailsOutputTypeDef,
     RuleGroupVariablesIpSetsDetailsTypeDef,
+    RuleGroupVariablesPortSetsDetailsOutputTypeDef,
     RuleGroupVariablesPortSetsDetailsTypeDef,
     SoftwarePackageTypeDef,
     StandardsManagedByTypeDef,
     StandardsStatusReasonTypeDef,
     StatelessCustomPublishMetricActionDimensionTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateActionTargetRequestRequestTypeDef,
     UpdateFindingAggregatorRequestRequestTypeDef,
-    UpdateFindingAggregatorResponseTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
     UpdateSecurityHubConfigurationRequestRequestTypeDef,
     UpdateStandardsControlRequestRequestTypeDef,
     VulnerabilityVendorTypeDef,
     CreateMembersRequestRequestTypeDef,
     ActionRemoteIpDetailsTypeDef,
-    DescribeActionTargetsResponseTypeDef,
+    CvssOutputTypeDef,
     CvssTypeDef,
-    ListOrganizationAdminAccountsResponseTypeDef,
     AssociationSetDetailsTypeDef,
+    AutomationRulesFindingFieldsUpdateOutputTypeDef,
     AutomationRulesFindingFieldsUpdateTypeDef,
-    ListAutomationRulesResponseTypeDef,
     AwsAmazonMqBrokerLogsDetailsTypeDef,
+    AwsApiGatewayRestApiDetailsOutputTypeDef,
     AwsApiGatewayRestApiDetailsTypeDef,
+    AwsApiGatewayStageDetailsOutputTypeDef,
     AwsApiGatewayStageDetailsTypeDef,
+    AwsApiGatewayV2ApiDetailsOutputTypeDef,
     AwsApiGatewayV2ApiDetailsTypeDef,
+    AwsApiGatewayV2StageDetailsOutputTypeDef,
     AwsApiGatewayV2StageDetailsTypeDef,
     AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef,
+    AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef,
     AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef,
+    AwsBackupBackupVaultDetailsOutputTypeDef,
     AwsBackupBackupVaultDetailsTypeDef,
     AwsBackupRecoveryPointDetailsTypeDef,
+    AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef,
     AwsCertificateManagerCertificateDomainValidationOptionTypeDef,
+    AwsCloudFormationStackDetailsOutputTypeDef,
     AwsCloudFormationStackDetailsTypeDef,
+    AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef,
     AwsCloudFrontDistributionCacheBehaviorsTypeDef,
+    AwsCloudFrontDistributionOriginCustomOriginConfigOutputTypeDef,
     AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef,
+    AwsCloudFrontDistributionOriginGroupFailoverOutputTypeDef,
     AwsCloudFrontDistributionOriginGroupFailoverTypeDef,
+    AwsCloudWatchAlarmDetailsOutputTypeDef,
     AwsCloudWatchAlarmDetailsTypeDef,
+    AwsCodeBuildProjectEnvironmentOutputTypeDef,
     AwsCodeBuildProjectEnvironmentTypeDef,
     AwsCodeBuildProjectLogsConfigDetailsTypeDef,
+    AwsDynamoDbTableGlobalSecondaryIndexOutputTypeDef,
+    AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef,
     AwsDynamoDbTableGlobalSecondaryIndexTypeDef,
     AwsDynamoDbTableLocalSecondaryIndexTypeDef,
     AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef,
+    AwsEc2InstanceDetailsOutputTypeDef,
     AwsEc2InstanceDetailsTypeDef,
     AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef,
     AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef,
     AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceRequirementsDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef,
     AwsEc2NetworkAclEntryTypeDef,
+    AwsEc2NetworkInterfaceDetailsOutputTypeDef,
     AwsEc2NetworkInterfaceDetailsTypeDef,
+    AwsEc2SecurityGroupIpPermissionOutputTypeDef,
     AwsEc2SecurityGroupIpPermissionTypeDef,
+    AwsEc2SubnetDetailsOutputTypeDef,
     AwsEc2SubnetDetailsTypeDef,
+    AwsEc2VolumeDetailsOutputTypeDef,
     AwsEc2VolumeDetailsTypeDef,
+    AwsEc2VpcDetailsOutputTypeDef,
     AwsEc2VpcDetailsTypeDef,
+    AwsEc2VpcEndpointServiceDetailsOutputTypeDef,
     AwsEc2VpcEndpointServiceDetailsTypeDef,
+    AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef,
     AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef,
+    AwsEc2VpnConnectionOptionsDetailsOutputTypeDef,
     AwsEc2VpnConnectionOptionsDetailsTypeDef,
     AwsEcrRepositoryDetailsTypeDef,
     AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef,
+    AwsEcsContainerDetailsOutputTypeDef,
     AwsEcsContainerDetailsTypeDef,
     AwsEcsServiceDeploymentConfigurationDetailsTypeDef,
+    AwsEcsServiceNetworkConfigurationDetailsOutputTypeDef,
     AwsEcsServiceNetworkConfigurationDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef,
+    AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef,
     AwsEcsTaskDefinitionProxyConfigurationDetailsTypeDef,
     AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef,
     AwsEcsTaskVolumeDetailsTypeDef,
     AwsEfsAccessPointRootDirectoryDetailsTypeDef,
+    AwsEksClusterLoggingDetailsOutputTypeDef,
     AwsEksClusterLoggingDetailsTypeDef,
+    AwsElasticBeanstalkEnvironmentDetailsOutputTypeDef,
     AwsElasticBeanstalkEnvironmentDetailsTypeDef,
     AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef,
     AwsElasticsearchDomainLogPublishingOptionsTypeDef,
+    AwsElbLoadBalancerPoliciesOutputTypeDef,
     AwsElbLoadBalancerPoliciesTypeDef,
+    AwsElbLoadBalancerAttributesOutputTypeDef,
     AwsElbLoadBalancerAttributesTypeDef,
+    AwsElbLoadBalancerListenerDescriptionOutputTypeDef,
     AwsElbLoadBalancerListenerDescriptionTypeDef,
+    AwsElbv2LoadBalancerDetailsOutputTypeDef,
     AwsElbv2LoadBalancerDetailsTypeDef,
     AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef,
     AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef,
     AwsIamAccessKeySessionContextTypeDef,
+    AwsIamGroupDetailsOutputTypeDef,
     AwsIamGroupDetailsTypeDef,
+    AwsIamInstanceProfileOutputTypeDef,
     AwsIamInstanceProfileTypeDef,
+    AwsIamPolicyDetailsOutputTypeDef,
     AwsIamPolicyDetailsTypeDef,
+    AwsIamUserDetailsOutputTypeDef,
     AwsIamUserDetailsTypeDef,
     AwsKinesisStreamDetailsTypeDef,
+    AwsLambdaFunctionEnvironmentOutputTypeDef,
     AwsLambdaFunctionEnvironmentTypeDef,
+    AwsNetworkFirewallFirewallDetailsOutputTypeDef,
     AwsNetworkFirewallFirewallDetailsTypeDef,
     AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef,
     AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef,
     AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef,
+    AwsRdsDbClusterDetailsOutputTypeDef,
     AwsRdsDbClusterDetailsTypeDef,
+    AwsRdsDbSnapshotDetailsOutputTypeDef,
     AwsRdsDbSnapshotDetailsTypeDef,
+    AwsRdsDbPendingModifiedValuesOutputTypeDef,
     AwsRdsDbPendingModifiedValuesTypeDef,
+    AwsRdsDbSecurityGroupDetailsOutputTypeDef,
     AwsRdsDbSecurityGroupDetailsTypeDef,
     AwsRdsDbSubnetGroupSubnetTypeDef,
+    AwsRedshiftClusterClusterParameterGroupOutputTypeDef,
     AwsRedshiftClusterClusterParameterGroupTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef,
+    AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef,
     AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef,
     AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef,
     AwsS3BucketServerSideEncryptionRuleTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef,
+    AwsSageMakerNotebookInstanceDetailsOutputTypeDef,
     AwsSageMakerNotebookInstanceDetailsTypeDef,
     AwsSecretsManagerSecretDetailsTypeDef,
     BatchUpdateFindingsRequestRequestTypeDef,
     BatchUpdateFindingsUnprocessedFindingTypeDef,
-    GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
-    GetFindingHistoryRequestRequestTypeDef,
+    AwsSnsTopicDetailsOutputTypeDef,
     AwsSnsTopicDetailsTypeDef,
     AwsSsmPatchTypeDef,
     AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef,
+    AwsWafRateBasedRuleDetailsOutputTypeDef,
     AwsWafRateBasedRuleDetailsTypeDef,
+    AwsWafRegionalRateBasedRuleDetailsOutputTypeDef,
     AwsWafRegionalRateBasedRuleDetailsTypeDef,
+    AwsWafRegionalRuleDetailsOutputTypeDef,
     AwsWafRegionalRuleDetailsTypeDef,
     AwsWafRegionalRuleGroupRulesDetailsTypeDef,
     AwsWafRegionalWebAclRulesListDetailsTypeDef,
+    AwsWafRuleDetailsOutputTypeDef,
     AwsWafRuleDetailsTypeDef,
     AwsWafRuleGroupRulesDetailsTypeDef,
+    AwsWafWebAclRuleOutputTypeDef,
     AwsWafWebAclRuleTypeDef,
+    AwsWafv2CustomRequestHandlingDetailsOutputTypeDef,
     AwsWafv2CustomRequestHandlingDetailsTypeDef,
+    AwsWafv2CustomResponseDetailsOutputTypeDef,
     AwsWafv2CustomResponseDetailsTypeDef,
     AwsWafv2WebAclCaptchaConfigDetailsTypeDef,
+    CreateActionTargetResponseTypeDef,
+    CreateAutomationRuleResponseTypeDef,
+    CreateFindingAggregatorResponseTypeDef,
+    CreateInsightResponseTypeDef,
+    DeleteActionTargetResponseTypeDef,
+    DeleteInsightResponseTypeDef,
+    DescribeActionTargetsResponseTypeDef,
+    DescribeHubResponseTypeDef,
+    DescribeOrganizationConfigurationResponseTypeDef,
+    EnableImportFindingsForProductResponseTypeDef,
+    GetFindingAggregatorResponseTypeDef,
+    GetInvitationsCountResponseTypeDef,
+    ListAutomationRulesResponseTypeDef,
+    ListEnabledProductsForImportResponseTypeDef,
+    ListOrganizationAdminAccountsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateFindingAggregatorResponseTypeDef,
     BatchDeleteAutomationRulesResponseTypeDef,
     BatchUpdateAutomationRulesResponseTypeDef,
     BatchEnableStandardsRequestRequestTypeDef,
     BatchGetSecurityControlsResponseTypeDef,
     BatchGetStandardsControlAssociationsRequestRequestTypeDef,
     UnprocessedStandardsControlAssociationTypeDef,
     BatchImportFindingsResponseTypeDef,
     BatchUpdateStandardsControlAssociationsRequestRequestTypeDef,
     UnprocessedStandardsControlAssociationUpdateTypeDef,
+    ComplianceOutputTypeDef,
     ComplianceTypeDef,
+    ContainerDetailsOutputTypeDef,
     ContainerDetailsTypeDef,
     CreateMembersResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     DeleteMembersResponseTypeDef,
     InviteMembersResponseTypeDef,
     DateFilterTypeDef,
+    DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef,
+    DescribeProductsRequestDescribeProductsPaginateTypeDef,
+    DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
+    DescribeStandardsRequestDescribeStandardsPaginateTypeDef,
+    GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef,
+    GetInsightsRequestGetInsightsPaginateTypeDef,
+    ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef,
+    ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef,
+    ListInvitationsRequestListInvitationsPaginateTypeDef,
+    ListMembersRequestListMembersPaginateTypeDef,
+    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
+    ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef,
+    ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef,
     DescribeProductsResponseTypeDef,
     DescribeStandardsControlsResponseTypeDef,
+    ThreatOutputTypeDef,
     ThreatTypeDef,
     ListFindingAggregatorsResponseTypeDef,
     FindingHistoryRecordTypeDef,
+    FindingProviderFieldsOutputTypeDef,
     FindingProviderFieldsTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetMasterAccountResponseTypeDef,
     ListInvitationsResponseTypeDef,
+    GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
+    GetFindingHistoryRequestRequestTypeDef,
     GetMembersResponseTypeDef,
     ListMembersResponseTypeDef,
     InsightResultsTypeDef,
     ListSecurityControlDefinitionsResponseTypeDef,
     ListStandardsControlAssociationsResponseTypeDef,
+    NetworkPathComponentDetailsOutputTypeDef,
     NetworkPathComponentDetailsTypeDef,
     NetworkTypeDef,
     PageTypeDef,
     RemediationTypeDef,
+    RuleGroupSourceStatefulRulesDetailsOutputTypeDef,
     RuleGroupSourceStatefulRulesDetailsTypeDef,
+    RuleGroupSourceStatelessRuleMatchAttributesOutputTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesTypeDef,
+    RuleGroupVariablesOutputTypeDef,
     RuleGroupVariablesTypeDef,
     StandardTypeDef,
     StandardsSubscriptionTypeDef,
+    StatelessCustomPublishMetricActionOutputTypeDef,
     StatelessCustomPublishMetricActionTypeDef,
+    AwsApiCallActionOutputTypeDef,
     AwsApiCallActionTypeDef,
     NetworkConnectionActionTypeDef,
     PortProbeDetailTypeDef,
+    VulnerabilityOutputTypeDef,
     VulnerabilityTypeDef,
+    AwsEc2RouteTableDetailsOutputTypeDef,
     AwsEc2RouteTableDetailsTypeDef,
+    AutomationRulesActionOutputTypeDef,
     AutomationRulesActionTypeDef,
+    AwsAmazonMqBrokerDetailsOutputTypeDef,
     AwsAmazonMqBrokerDetailsTypeDef,
+    AwsAppSyncGraphQlApiDetailsOutputTypeDef,
     AwsAppSyncGraphQlApiDetailsTypeDef,
+    AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef,
+    AwsAutoScalingLaunchConfigurationDetailsOutputTypeDef,
     AwsAutoScalingLaunchConfigurationDetailsTypeDef,
+    AwsBackupBackupPlanRuleDetailsOutputTypeDef,
     AwsBackupBackupPlanRuleDetailsTypeDef,
+    AwsCertificateManagerCertificateRenewalSummaryOutputTypeDef,
     AwsCertificateManagerCertificateRenewalSummaryTypeDef,
+    AwsCloudFrontDistributionOriginItemOutputTypeDef,
     AwsCloudFrontDistributionOriginItemTypeDef,
+    AwsCloudFrontDistributionOriginGroupOutputTypeDef,
     AwsCloudFrontDistributionOriginGroupTypeDef,
+    AwsCodeBuildProjectDetailsOutputTypeDef,
     AwsCodeBuildProjectDetailsTypeDef,
+    AwsDynamoDbTableReplicaOutputTypeDef,
     AwsDynamoDbTableReplicaTypeDef,
+    AwsEc2LaunchTemplateDataDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataDetailsTypeDef,
+    AwsEc2NetworkAclDetailsOutputTypeDef,
     AwsEc2NetworkAclDetailsTypeDef,
+    AwsEc2SecurityGroupDetailsOutputTypeDef,
     AwsEc2SecurityGroupDetailsTypeDef,
+    AwsEc2VpcPeeringConnectionDetailsOutputTypeDef,
     AwsEc2VpcPeeringConnectionDetailsTypeDef,
+    AwsEc2VpnConnectionDetailsOutputTypeDef,
     AwsEc2VpnConnectionDetailsTypeDef,
     AwsEcsClusterConfigurationDetailsTypeDef,
+    AwsEcsServiceDetailsOutputTypeDef,
     AwsEcsServiceDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef,
+    AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef,
     AwsEcsTaskDefinitionVolumesDetailsTypeDef,
+    AwsEcsTaskDetailsOutputTypeDef,
     AwsEcsTaskDetailsTypeDef,
+    AwsEfsAccessPointDetailsOutputTypeDef,
     AwsEfsAccessPointDetailsTypeDef,
+    AwsEksClusterDetailsOutputTypeDef,
     AwsEksClusterDetailsTypeDef,
+    AwsElasticsearchDomainDetailsOutputTypeDef,
     AwsElasticsearchDomainDetailsTypeDef,
+    AwsElbLoadBalancerDetailsOutputTypeDef,
     AwsElbLoadBalancerDetailsTypeDef,
     AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef,
     AwsIamAccessKeyDetailsTypeDef,
+    AwsIamRoleDetailsOutputTypeDef,
     AwsIamRoleDetailsTypeDef,
+    AwsLambdaFunctionDetailsOutputTypeDef,
     AwsLambdaFunctionDetailsTypeDef,
+    AwsOpenSearchServiceDomainDetailsOutputTypeDef,
     AwsOpenSearchServiceDomainDetailsTypeDef,
+    AwsRdsDbSubnetGroupOutputTypeDef,
     AwsRdsDbSubnetGroupTypeDef,
+    AwsRedshiftClusterDetailsOutputTypeDef,
     AwsRedshiftClusterDetailsTypeDef,
+    AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef,
+    AwsS3BucketNotificationConfigurationFilterOutputTypeDef,
     AwsS3BucketNotificationConfigurationFilterTypeDef,
     AwsS3BucketObjectLockConfigurationTypeDef,
+    AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef,
     AwsS3BucketServerSideEncryptionConfigurationTypeDef,
+    AwsS3BucketWebsiteConfigurationOutputTypeDef,
     AwsS3BucketWebsiteConfigurationTypeDef,
     BatchUpdateFindingsResponseTypeDef,
     AwsSsmPatchComplianceDetailsTypeDef,
+    AwsStepFunctionStateMachineLoggingConfigurationDetailsOutputTypeDef,
     AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef,
+    AwsWafRegionalRuleGroupDetailsOutputTypeDef,
     AwsWafRegionalRuleGroupDetailsTypeDef,
+    AwsWafRegionalWebAclDetailsOutputTypeDef,
     AwsWafRegionalWebAclDetailsTypeDef,
+    AwsWafRuleGroupDetailsOutputTypeDef,
     AwsWafRuleGroupDetailsTypeDef,
+    AwsWafWebAclDetailsOutputTypeDef,
     AwsWafWebAclDetailsTypeDef,
+    AwsWafv2ActionAllowDetailsOutputTypeDef,
+    AwsWafv2RulesActionCaptchaDetailsOutputTypeDef,
+    AwsWafv2RulesActionCountDetailsOutputTypeDef,
     AwsWafv2ActionAllowDetailsTypeDef,
     AwsWafv2RulesActionCaptchaDetailsTypeDef,
     AwsWafv2RulesActionCountDetailsTypeDef,
+    AwsWafv2ActionBlockDetailsOutputTypeDef,
     AwsWafv2ActionBlockDetailsTypeDef,
     BatchGetStandardsControlAssociationsResponseTypeDef,
     BatchUpdateStandardsControlAssociationsResponseTypeDef,
+    AutomationRulesFindingFiltersOutputTypeDef,
     AutomationRulesFindingFiltersTypeDef,
+    AwsSecurityFindingFiltersOutputTypeDef,
     AwsSecurityFindingFiltersTypeDef,
     GetFindingHistoryResponseTypeDef,
     GetInsightResultsResponseTypeDef,
+    NetworkHeaderOutputTypeDef,
     NetworkHeaderTypeDef,
+    OccurrencesOutputTypeDef,
     OccurrencesTypeDef,
+    RuleGroupSourceStatelessRuleDefinitionOutputTypeDef,
     RuleGroupSourceStatelessRuleDefinitionTypeDef,
     DescribeStandardsResponseTypeDef,
     BatchDisableStandardsResponseTypeDef,
     BatchEnableStandardsResponseTypeDef,
     GetEnabledStandardsResponseTypeDef,
+    StatelessCustomActionDefinitionOutputTypeDef,
     StatelessCustomActionDefinitionTypeDef,
+    PortProbeActionOutputTypeDef,
     PortProbeActionTypeDef,
+    AutomationRulesActionUnionTypeDef,
+    AwsAutoScalingAutoScalingGroupDetailsOutputTypeDef,
     AwsAutoScalingAutoScalingGroupDetailsTypeDef,
+    AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef,
     AwsBackupBackupPlanBackupPlanDetailsTypeDef,
+    AwsCertificateManagerCertificateDetailsOutputTypeDef,
     AwsCertificateManagerCertificateDetailsTypeDef,
+    AwsCloudFrontDistributionOriginsOutputTypeDef,
     AwsCloudFrontDistributionOriginsTypeDef,
+    AwsCloudFrontDistributionOriginGroupsOutputTypeDef,
     AwsCloudFrontDistributionOriginGroupsTypeDef,
+    AwsDynamoDbTableDetailsOutputTypeDef,
     AwsDynamoDbTableDetailsTypeDef,
+    AwsEc2LaunchTemplateDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDetailsTypeDef,
+    AwsEcsClusterDetailsOutputTypeDef,
     AwsEcsClusterDetailsTypeDef,
+    AwsEcsTaskDefinitionDetailsOutputTypeDef,
     AwsEcsTaskDefinitionDetailsTypeDef,
     AwsGuardDutyDetectorDataSourcesDetailsTypeDef,
+    AwsRdsDbInstanceDetailsOutputTypeDef,
     AwsRdsDbInstanceDetailsTypeDef,
+    AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef,
+    AwsS3BucketNotificationConfigurationDetailOutputTypeDef,
     AwsS3BucketNotificationConfigurationDetailTypeDef,
+    AwsStepFunctionStateMachineDetailsOutputTypeDef,
     AwsStepFunctionStateMachineDetailsTypeDef,
+    AwsWafv2RulesActionDetailsOutputTypeDef,
+    AwsWafv2WebAclActionDetailsOutputTypeDef,
     AwsWafv2RulesActionDetailsTypeDef,
     AwsWafv2WebAclActionDetailsTypeDef,
     AutomationRulesConfigTypeDef,
-    CreateAutomationRuleRequestRequestTypeDef,
+    AutomationRulesFindingFiltersUnionTypeDef,
     UpdateAutomationRulesRequestItemTypeDef,
+    InsightTypeDef,
+    AwsSecurityFindingFiltersUnionTypeDef,
     CreateInsightRequestRequestTypeDef,
     GetFindingsRequestGetFindingsPaginateTypeDef,
     GetFindingsRequestRequestTypeDef,
-    InsightTypeDef,
     UpdateFindingsRequestRequestTypeDef,
     UpdateInsightRequestRequestTypeDef,
+    NetworkPathComponentOutputTypeDef,
     NetworkPathComponentTypeDef,
+    CustomDataIdentifiersDetectionsOutputTypeDef,
+    SensitiveDataDetectionsOutputTypeDef,
     CustomDataIdentifiersDetectionsTypeDef,
     SensitiveDataDetectionsTypeDef,
+    RuleGroupSourceStatelessRulesDetailsOutputTypeDef,
     RuleGroupSourceStatelessRulesDetailsTypeDef,
+    FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef,
+    RuleGroupSourceCustomActionsDetailsOutputTypeDef,
     FirewallPolicyStatelessCustomActionsDetailsTypeDef,
     RuleGroupSourceCustomActionsDetailsTypeDef,
+    ActionOutputTypeDef,
     ActionTypeDef,
+    CreateAutomationRuleRequestRequestTypeDef,
+    AwsBackupBackupPlanDetailsOutputTypeDef,
     AwsBackupBackupPlanDetailsTypeDef,
+    AwsCloudFrontDistributionDetailsOutputTypeDef,
     AwsCloudFrontDistributionDetailsTypeDef,
+    AwsGuardDutyDetectorDetailsOutputTypeDef,
     AwsGuardDutyDetectorDetailsTypeDef,
+    AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef,
+    AwsS3BucketNotificationConfigurationOutputTypeDef,
     AwsS3BucketNotificationConfigurationTypeDef,
+    AwsWafv2RulesDetailsOutputTypeDef,
     AwsWafv2RulesDetailsTypeDef,
     BatchGetAutomationRulesResponseTypeDef,
     BatchUpdateAutomationRulesRequestRequestTypeDef,
     GetInsightsResponseTypeDef,
+    CustomDataIdentifiersResultOutputTypeDef,
+    SensitiveDataResultOutputTypeDef,
     CustomDataIdentifiersResultTypeDef,
     SensitiveDataResultTypeDef,
+    FirewallPolicyDetailsOutputTypeDef,
+    RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef,
     FirewallPolicyDetailsTypeDef,
     RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef,
+    AwsS3BucketBucketLifecycleConfigurationDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef,
+    AwsWafv2RuleGroupDetailsOutputTypeDef,
+    AwsWafv2WebAclDetailsOutputTypeDef,
     AwsWafv2RuleGroupDetailsTypeDef,
     AwsWafv2WebAclDetailsTypeDef,
+    ClassificationResultOutputTypeDef,
     ClassificationResultTypeDef,
+    AwsNetworkFirewallFirewallPolicyDetailsOutputTypeDef,
+    RuleGroupSourceOutputTypeDef,
     AwsNetworkFirewallFirewallPolicyDetailsTypeDef,
     RuleGroupSourceTypeDef,
+    AwsS3BucketDetailsOutputTypeDef,
     AwsS3BucketDetailsTypeDef,
+    DataClassificationDetailsOutputTypeDef,
     DataClassificationDetailsTypeDef,
+    RuleGroupDetailsOutputTypeDef,
     RuleGroupDetailsTypeDef,
+    AwsNetworkFirewallRuleGroupDetailsOutputTypeDef,
     AwsNetworkFirewallRuleGroupDetailsTypeDef,
+    ResourceDetailsOutputTypeDef,
     ResourceDetailsTypeDef,
+    ResourceOutputTypeDef,
     ResourceTypeDef,
+    AwsSecurityFindingOutputTypeDef,
     AwsSecurityFindingTypeDef,
-    BatchImportFindingsRequestRequestTypeDef,
     GetFindingsResponseTypeDef,
+    AwsSecurityFindingUnionTypeDef,
+    BatchImportFindingsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AcceptAdministratorInvitationRequestRequestTypeDef:
+def get_value() -> AcceptAdministratorInvitationRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-securityhub-2.5.2/setup.py` & `types-aiobotocore-securityhub-2.5.2.post1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-securityhub",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_securityhub"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SecurityHub 2.5.2 service generated with"
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
-    keywords="aiobotocore securityhub type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore securityhub type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_securityhub": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/"
```

### Comparing `types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub/__init__.py` & `types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub/__init__.pyi` & `types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub/__main__.py` & `types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SecurityHub 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.SecurityHub 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub\nOther"
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

### Comparing `types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub/client.py` & `types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("securityhub") as client:
         client: SecurityHubClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     AutoEnableStandardsType,
     ControlFindingGeneratorType,
@@ -44,19 +43,19 @@
     ListMembersPaginator,
     ListOrganizationAdminAccountsPaginator,
     ListSecurityControlDefinitionsPaginator,
     ListStandardsControlAssociationsPaginator,
 )
 from .type_defs import (
     AccountDetailsTypeDef,
-    AutomationRulesActionTypeDef,
-    AutomationRulesFindingFiltersTypeDef,
-    AwsSecurityFindingFiltersTypeDef,
+    AutomationRulesActionUnionTypeDef,
+    AutomationRulesFindingFiltersUnionTypeDef,
+    AwsSecurityFindingFiltersUnionTypeDef,
     AwsSecurityFindingIdentifierTypeDef,
-    AwsSecurityFindingTypeDef,
+    AwsSecurityFindingUnionTypeDef,
     BatchDeleteAutomationRulesResponseTypeDef,
     BatchDisableStandardsResponseTypeDef,
     BatchEnableStandardsResponseTypeDef,
     BatchGetAutomationRulesResponseTypeDef,
     BatchGetSecurityControlsResponseTypeDef,
     BatchGetStandardsControlAssociationsResponseTypeDef,
     BatchImportFindingsResponseTypeDef,
@@ -103,14 +102,15 @@
     NoteUpdateTypeDef,
     RelatedFindingTypeDef,
     SeverityUpdateTypeDef,
     SortCriterionTypeDef,
     StandardsControlAssociationIdTypeDef,
     StandardsControlAssociationUpdateTypeDef,
     StandardsSubscriptionRequestTypeDef,
+    TimestampTypeDef,
     UpdateAutomationRulesRequestItemTypeDef,
     UpdateFindingAggregatorResponseTypeDef,
     WorkflowUpdateTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -236,15 +236,15 @@
         is currently enabled or disabled in a standard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_get_standards_control_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#batch_get_standards_control_associations)
         """
 
     async def batch_import_findings(
-        self, *, Findings: Sequence[AwsSecurityFindingTypeDef]
+        self, *, Findings: Sequence[AwsSecurityFindingUnionTypeDef]
     ) -> BatchImportFindingsResponseTypeDef:
         """
         Imports security findings generated by a finding provider into Security Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_import_findings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#batch_import_findings)
         """
@@ -325,16 +325,16 @@
 
     async def create_automation_rule(
         self,
         *,
         RuleOrder: int,
         RuleName: str,
         Description: str,
-        Criteria: AutomationRulesFindingFiltersTypeDef,
-        Actions: Sequence[AutomationRulesActionTypeDef],
+        Criteria: AutomationRulesFindingFiltersUnionTypeDef,
+        Actions: Sequence[AutomationRulesActionUnionTypeDef],
         Tags: Mapping[str, str] = ...,
         RuleStatus: RuleStatusType = ...,
         IsTerminal: bool = ...
     ) -> CreateAutomationRuleResponseTypeDef:
         """
         Creates an automation rule based on input parameters.
 
@@ -349,15 +349,15 @@
         Used to enable finding aggregation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_finding_aggregator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#create_finding_aggregator)
         """
 
     async def create_insight(
-        self, *, Name: str, Filters: AwsSecurityFindingFiltersTypeDef, GroupByAttribute: str
+        self, *, Name: str, Filters: AwsSecurityFindingFiltersUnionTypeDef, GroupByAttribute: str
     ) -> CreateInsightResponseTypeDef:
         """
         Creates a custom insight in Security Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_insight)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#create_insight)
         """
@@ -619,30 +619,30 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#get_finding_aggregator)
         """
 
     async def get_finding_history(
         self,
         *,
         FindingIdentifier: AwsSecurityFindingIdentifierTypeDef,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> GetFindingHistoryResponseTypeDef:
         """
         Returns history for a Security Hub finding in the last 90 days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_finding_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#get_finding_history)
         """
 
     async def get_findings(
         self,
         *,
-        Filters: AwsSecurityFindingFiltersTypeDef = ...,
+        Filters: AwsSecurityFindingFiltersUnionTypeDef = ...,
         SortCriteria: Sequence[SortCriterionTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> GetFindingsResponseTypeDef:
         """
         Returns a list of findings that match the specified criteria.
 
@@ -833,15 +833,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_finding_aggregator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#update_finding_aggregator)
         """
 
     async def update_findings(
         self,
         *,
-        Filters: AwsSecurityFindingFiltersTypeDef,
+        Filters: AwsSecurityFindingFiltersUnionTypeDef,
         Note: NoteUpdateTypeDef = ...,
         RecordState: RecordStateType = ...
     ) -> Dict[str, Any]:
         """
         `UpdateFindings` is deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_findings)
@@ -849,15 +849,15 @@
         """
 
     async def update_insight(
         self,
         *,
         InsightArn: str,
         Name: str = ...,
-        Filters: AwsSecurityFindingFiltersTypeDef = ...,
+        Filters: AwsSecurityFindingFiltersUnionTypeDef = ...,
         GroupByAttribute: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the Security Hub insight identified by the specified insight ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_insight)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#update_insight)
```

### Comparing `types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub/client.pyi` & `types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("securityhub") as client:
         client: SecurityHubClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     AutoEnableStandardsType,
     ControlFindingGeneratorType,
@@ -44,19 +43,19 @@
     ListMembersPaginator,
     ListOrganizationAdminAccountsPaginator,
     ListSecurityControlDefinitionsPaginator,
     ListStandardsControlAssociationsPaginator,
 )
 from .type_defs import (
     AccountDetailsTypeDef,
-    AutomationRulesActionTypeDef,
-    AutomationRulesFindingFiltersTypeDef,
-    AwsSecurityFindingFiltersTypeDef,
+    AutomationRulesActionUnionTypeDef,
+    AutomationRulesFindingFiltersUnionTypeDef,
+    AwsSecurityFindingFiltersUnionTypeDef,
     AwsSecurityFindingIdentifierTypeDef,
-    AwsSecurityFindingTypeDef,
+    AwsSecurityFindingUnionTypeDef,
     BatchDeleteAutomationRulesResponseTypeDef,
     BatchDisableStandardsResponseTypeDef,
     BatchEnableStandardsResponseTypeDef,
     BatchGetAutomationRulesResponseTypeDef,
     BatchGetSecurityControlsResponseTypeDef,
     BatchGetStandardsControlAssociationsResponseTypeDef,
     BatchImportFindingsResponseTypeDef,
@@ -103,14 +102,15 @@
     NoteUpdateTypeDef,
     RelatedFindingTypeDef,
     SeverityUpdateTypeDef,
     SortCriterionTypeDef,
     StandardsControlAssociationIdTypeDef,
     StandardsControlAssociationUpdateTypeDef,
     StandardsSubscriptionRequestTypeDef,
+    TimestampTypeDef,
     UpdateAutomationRulesRequestItemTypeDef,
     UpdateFindingAggregatorResponseTypeDef,
     WorkflowUpdateTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -223,15 +223,15 @@
         For a batch of security controls and standards, identifies whether each control
         is currently enabled or disabled in a standard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_get_standards_control_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#batch_get_standards_control_associations)
         """
     async def batch_import_findings(
-        self, *, Findings: Sequence[AwsSecurityFindingTypeDef]
+        self, *, Findings: Sequence[AwsSecurityFindingUnionTypeDef]
     ) -> BatchImportFindingsResponseTypeDef:
         """
         Imports security findings generated by a finding provider into Security Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_import_findings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#batch_import_findings)
         """
@@ -305,16 +305,16 @@
         """
     async def create_automation_rule(
         self,
         *,
         RuleOrder: int,
         RuleName: str,
         Description: str,
-        Criteria: AutomationRulesFindingFiltersTypeDef,
-        Actions: Sequence[AutomationRulesActionTypeDef],
+        Criteria: AutomationRulesFindingFiltersUnionTypeDef,
+        Actions: Sequence[AutomationRulesActionUnionTypeDef],
         Tags: Mapping[str, str] = ...,
         RuleStatus: RuleStatusType = ...,
         IsTerminal: bool = ...
     ) -> CreateAutomationRuleResponseTypeDef:
         """
         Creates an automation rule based on input parameters.
 
@@ -327,15 +327,15 @@
         """
         Used to enable finding aggregation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_finding_aggregator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#create_finding_aggregator)
         """
     async def create_insight(
-        self, *, Name: str, Filters: AwsSecurityFindingFiltersTypeDef, GroupByAttribute: str
+        self, *, Name: str, Filters: AwsSecurityFindingFiltersUnionTypeDef, GroupByAttribute: str
     ) -> CreateInsightResponseTypeDef:
         """
         Creates a custom insight in Security Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_insight)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#create_insight)
         """
@@ -570,29 +570,29 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_finding_aggregator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#get_finding_aggregator)
         """
     async def get_finding_history(
         self,
         *,
         FindingIdentifier: AwsSecurityFindingIdentifierTypeDef,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> GetFindingHistoryResponseTypeDef:
         """
         Returns history for a Security Hub finding in the last 90 days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_finding_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#get_finding_history)
         """
     async def get_findings(
         self,
         *,
-        Filters: AwsSecurityFindingFiltersTypeDef = ...,
+        Filters: AwsSecurityFindingFiltersUnionTypeDef = ...,
         SortCriteria: Sequence[SortCriterionTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> GetFindingsResponseTypeDef:
         """
         Returns a list of findings that match the specified criteria.
 
@@ -763,30 +763,30 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_finding_aggregator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#update_finding_aggregator)
         """
     async def update_findings(
         self,
         *,
-        Filters: AwsSecurityFindingFiltersTypeDef,
+        Filters: AwsSecurityFindingFiltersUnionTypeDef,
         Note: NoteUpdateTypeDef = ...,
         RecordState: RecordStateType = ...
     ) -> Dict[str, Any]:
         """
         `UpdateFindings` is deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_findings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#update_findings)
         """
     async def update_insight(
         self,
         *,
         InsightArn: str,
         Name: str = ...,
-        Filters: AwsSecurityFindingFiltersTypeDef = ...,
+        Filters: AwsSecurityFindingFiltersUnionTypeDef = ...,
         GroupByAttribute: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the Security Hub insight identified by the specified insight ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_insight)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/client/#update_insight)
```

### Comparing `types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub/literals.py` & `types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub/literals.pyi` & `types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub/paginator.py` & `types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,22 +44,21 @@
         list_invitations_paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")
         list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
         list_organization_admin_accounts_paginator: ListOrganizationAdminAccountsPaginator = client.get_paginator("list_organization_admin_accounts")
         list_security_control_definitions_paginator: ListSecurityControlDefinitionsPaginator = client.get_paginator("list_security_control_definitions")
         list_standards_control_associations_paginator: ListStandardsControlAssociationsPaginator = client.get_paginator("list_standards_control_associations")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import (
-    AwsSecurityFindingFiltersTypeDef,
+    AwsSecurityFindingFiltersUnionTypeDef,
     AwsSecurityFindingIdentifierTypeDef,
     DescribeActionTargetsResponseTypeDef,
     DescribeProductsResponseTypeDef,
     DescribeStandardsControlsResponseTypeDef,
     DescribeStandardsResponseTypeDef,
     GetEnabledStandardsResponseTypeDef,
     GetFindingHistoryResponseTypeDef,
@@ -70,14 +69,15 @@
     ListInvitationsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListOrganizationAdminAccountsResponseTypeDef,
     ListSecurityControlDefinitionsResponseTypeDef,
     ListStandardsControlAssociationsResponseTypeDef,
     PaginatorConfigTypeDef,
     SortCriterionTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeActionTargetsPaginator",
     "DescribeProductsPaginator",
     "DescribeStandardsPaginator",
     "DescribeStandardsControlsPaginator",
@@ -111,60 +111,60 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#describeactiontargetspaginator)
     """
 
     def paginate(
         self,
         *,
         ActionTargetArns: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeActionTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeActionTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#describeactiontargetspaginator)
         """
 
 
 class DescribeProductsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeProducts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#describeproductspaginator)
     """
 
     def paginate(
-        self, *, ProductArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ProductArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeProductsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeProducts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#describeproductspaginator)
         """
 
 
 class DescribeStandardsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandards)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#describestandardspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeStandardsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandards.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#describestandardspaginator)
         """
 
 
 class DescribeStandardsControlsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandardsControls)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#describestandardscontrolspaginator)
     """
 
     def paginate(
-        self, *, StandardsSubscriptionArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StandardsSubscriptionArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeStandardsControlsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandardsControls.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#describestandardscontrolspaginator)
         """
 
 
@@ -174,15 +174,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#getenabledstandardspaginator)
     """
 
     def paginate(
         self,
         *,
         StandardsSubscriptionArns: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetEnabledStandardsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetEnabledStandards.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#getenabledstandardspaginator)
         """
 
 
@@ -192,17 +192,17 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#getfindinghistorypaginator)
     """
 
     def paginate(
         self,
         *,
         FindingIdentifier: AwsSecurityFindingIdentifierTypeDef,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetFindingHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindingHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#getfindinghistorypaginator)
         """
 
 
@@ -211,135 +211,135 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindings)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#getfindingspaginator)
     """
 
     def paginate(
         self,
         *,
-        Filters: AwsSecurityFindingFiltersTypeDef = ...,
+        Filters: AwsSecurityFindingFiltersUnionTypeDef = ...,
         SortCriteria: Sequence[SortCriterionTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#getfindingspaginator)
         """
 
 
 class GetInsightsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetInsights)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#getinsightspaginator)
     """
 
     def paginate(
-        self, *, InsightArns: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, InsightArns: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetInsights.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#getinsightspaginator)
         """
 
 
 class ListEnabledProductsForImportPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListEnabledProductsForImport)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#listenabledproductsforimportpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEnabledProductsForImportResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListEnabledProductsForImport.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#listenabledproductsforimportpaginator)
         """
 
 
 class ListFindingAggregatorsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListFindingAggregators)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#listfindingaggregatorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFindingAggregatorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListFindingAggregators.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#listfindingaggregatorspaginator)
         """
 
 
 class ListInvitationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListInvitations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#listinvitationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListInvitationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListInvitations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#listinvitationspaginator)
         """
 
 
 class ListMembersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListMembers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#listmemberspaginator)
     """
 
     def paginate(
-        self, *, OnlyAssociated: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, OnlyAssociated: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListMembers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#listmemberspaginator)
         """
 
 
 class ListOrganizationAdminAccountsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListOrganizationAdminAccounts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#listorganizationadminaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListOrganizationAdminAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListOrganizationAdminAccounts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#listorganizationadminaccountspaginator)
         """
 
 
 class ListSecurityControlDefinitionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListSecurityControlDefinitions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#listsecuritycontroldefinitionspaginator)
     """
 
     def paginate(
-        self, *, StandardsArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StandardsArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSecurityControlDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListSecurityControlDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#listsecuritycontroldefinitionspaginator)
         """
 
 
 class ListStandardsControlAssociationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListStandardsControlAssociations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#liststandardscontrolassociationspaginator)
     """
 
     def paginate(
-        self, *, SecurityControlId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SecurityControlId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStandardsControlAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListStandardsControlAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#liststandardscontrolassociationspaginator)
         """
```

### Comparing `types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub/paginator.pyi` & `types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -44,22 +44,21 @@
         list_invitations_paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")
         list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
         list_organization_admin_accounts_paginator: ListOrganizationAdminAccountsPaginator = client.get_paginator("list_organization_admin_accounts")
         list_security_control_definitions_paginator: ListSecurityControlDefinitionsPaginator = client.get_paginator("list_security_control_definitions")
         list_standards_control_associations_paginator: ListStandardsControlAssociationsPaginator = client.get_paginator("list_standards_control_associations")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import (
-    AwsSecurityFindingFiltersTypeDef,
+    AwsSecurityFindingFiltersUnionTypeDef,
     AwsSecurityFindingIdentifierTypeDef,
     DescribeActionTargetsResponseTypeDef,
     DescribeProductsResponseTypeDef,
     DescribeStandardsControlsResponseTypeDef,
     DescribeStandardsResponseTypeDef,
     GetEnabledStandardsResponseTypeDef,
     GetFindingHistoryResponseTypeDef,
@@ -70,14 +69,15 @@
     ListInvitationsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListOrganizationAdminAccountsResponseTypeDef,
     ListSecurityControlDefinitionsResponseTypeDef,
     ListStandardsControlAssociationsResponseTypeDef,
     PaginatorConfigTypeDef,
     SortCriterionTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeActionTargetsPaginator",
     "DescribeProductsPaginator",
     "DescribeStandardsPaginator",
     "DescribeStandardsControlsPaginator",
@@ -108,57 +108,57 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#describeactiontargetspaginator)
     """
 
     def paginate(
         self,
         *,
         ActionTargetArns: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeActionTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeActionTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#describeactiontargetspaginator)
         """
 
 class DescribeProductsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeProducts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#describeproductspaginator)
     """
 
     def paginate(
-        self, *, ProductArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ProductArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeProductsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeProducts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#describeproductspaginator)
         """
 
 class DescribeStandardsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandards)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#describestandardspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeStandardsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandards.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#describestandardspaginator)
         """
 
 class DescribeStandardsControlsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandardsControls)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#describestandardscontrolspaginator)
     """
 
     def paginate(
-        self, *, StandardsSubscriptionArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StandardsSubscriptionArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeStandardsControlsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandardsControls.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#describestandardscontrolspaginator)
         """
 
 class GetEnabledStandardsPaginator(AioPaginator):
@@ -167,15 +167,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#getenabledstandardspaginator)
     """
 
     def paginate(
         self,
         *,
         StandardsSubscriptionArns: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetEnabledStandardsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetEnabledStandards.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#getenabledstandardspaginator)
         """
 
 class GetFindingHistoryPaginator(AioPaginator):
@@ -184,17 +184,17 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#getfindinghistorypaginator)
     """
 
     def paginate(
         self,
         *,
         FindingIdentifier: AwsSecurityFindingIdentifierTypeDef,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetFindingHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindingHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#getfindinghistorypaginator)
         """
 
 class GetFindingsPaginator(AioPaginator):
@@ -202,127 +202,127 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindings)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#getfindingspaginator)
     """
 
     def paginate(
         self,
         *,
-        Filters: AwsSecurityFindingFiltersTypeDef = ...,
+        Filters: AwsSecurityFindingFiltersUnionTypeDef = ...,
         SortCriteria: Sequence[SortCriterionTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#getfindingspaginator)
         """
 
 class GetInsightsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetInsights)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#getinsightspaginator)
     """
 
     def paginate(
-        self, *, InsightArns: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, InsightArns: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetInsights.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#getinsightspaginator)
         """
 
 class ListEnabledProductsForImportPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListEnabledProductsForImport)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#listenabledproductsforimportpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEnabledProductsForImportResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListEnabledProductsForImport.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#listenabledproductsforimportpaginator)
         """
 
 class ListFindingAggregatorsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListFindingAggregators)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#listfindingaggregatorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFindingAggregatorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListFindingAggregators.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#listfindingaggregatorspaginator)
         """
 
 class ListInvitationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListInvitations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#listinvitationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListInvitationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListInvitations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#listinvitationspaginator)
         """
 
 class ListMembersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListMembers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#listmemberspaginator)
     """
 
     def paginate(
-        self, *, OnlyAssociated: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, OnlyAssociated: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListMembers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#listmemberspaginator)
         """
 
 class ListOrganizationAdminAccountsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListOrganizationAdminAccounts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#listorganizationadminaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListOrganizationAdminAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListOrganizationAdminAccounts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#listorganizationadminaccountspaginator)
         """
 
 class ListSecurityControlDefinitionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListSecurityControlDefinitions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#listsecuritycontroldefinitionspaginator)
     """
 
     def paginate(
-        self, *, StandardsArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StandardsArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSecurityControlDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListSecurityControlDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#listsecuritycontroldefinitionspaginator)
         """
 
 class ListStandardsControlAssociationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListStandardsControlAssociations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#liststandardscontrolassociationspaginator)
     """
 
     def paginate(
-        self, *, SecurityControlId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SecurityControlId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStandardsControlAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListStandardsControlAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/paginators/#liststandardscontrolassociationspaginator)
         """
```

### Comparing `types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub/type_defs.py` & `types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub/type_defs.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_securityhub.type_defs import AcceptAdministratorInvitationRequestRequestTypeDef
 
-    data: AcceptAdministratorInvitationRequestRequestTypeDef = {...}
+    data: AcceptAdministratorInvitationRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -61,93 +61,103 @@
 
 __all__ = (
     "AcceptAdministratorInvitationRequestRequestTypeDef",
     "AcceptInvitationRequestRequestTypeDef",
     "AccountDetailsTypeDef",
     "ActionLocalIpDetailsTypeDef",
     "ActionLocalPortDetailsTypeDef",
+    "DnsRequestActionTypeDef",
     "CityTypeDef",
     "CountryTypeDef",
     "GeoLocationTypeDef",
     "IpOrganizationDetailsTypeDef",
     "ActionRemotePortDetailsTypeDef",
     "ActionTargetTypeDef",
-    "DnsRequestActionTypeDef",
     "AdjustmentTypeDef",
     "AdminAccountTypeDef",
     "AssociatedStandardTypeDef",
     "AssociationStateDetailsTypeDef",
     "NoteUpdateTypeDef",
     "RelatedFindingTypeDef",
     "SeverityUpdateTypeDef",
     "WorkflowUpdateTypeDef",
     "MapFilterTypeDef",
     "NumberFilterTypeDef",
     "StringFilterTypeDef",
     "AutomationRulesMetadataTypeDef",
     "AvailabilityZoneTypeDef",
     "AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef",
-    "AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef",
+    "AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef",
     "AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef",
     "AwsAmazonMqBrokerUsersDetailsTypeDef",
+    "AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef",
     "AwsAmazonMqBrokerLogsPendingDetailsTypeDef",
     "AwsApiCallActionDomainDetailsTypeDef",
     "AwsApiGatewayAccessLogSettingsTypeDef",
+    "AwsApiGatewayCanarySettingsOutputTypeDef",
     "AwsApiGatewayCanarySettingsTypeDef",
+    "AwsApiGatewayEndpointConfigurationOutputTypeDef",
     "AwsApiGatewayEndpointConfigurationTypeDef",
     "AwsApiGatewayMethodSettingsTypeDef",
+    "AwsCorsConfigurationOutputTypeDef",
     "AwsCorsConfigurationTypeDef",
     "AwsApiGatewayV2RouteSettingsTypeDef",
     "AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef",
     "AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef",
     "AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef",
     "AwsAppSyncGraphQlApiLogConfigDetailsTypeDef",
     "AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef",
     "AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef",
     "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef",
     "AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef",
     "AwsAutoScalingLaunchConfigurationMetadataOptionsTypeDef",
+    "AwsBackupBackupPlanAdvancedBackupSettingsDetailsOutputTypeDef",
     "AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef",
     "AwsBackupBackupPlanLifecycleDetailsTypeDef",
+    "AwsBackupBackupVaultNotificationsDetailsOutputTypeDef",
     "AwsBackupBackupVaultNotificationsDetailsTypeDef",
     "AwsBackupRecoveryPointCalculatedLifecycleDetailsTypeDef",
     "AwsBackupRecoveryPointCreatedByDetailsTypeDef",
     "AwsBackupRecoveryPointLifecycleDetailsTypeDef",
     "AwsCertificateManagerCertificateExtendedKeyUsageTypeDef",
     "AwsCertificateManagerCertificateKeyUsageTypeDef",
     "AwsCertificateManagerCertificateOptionsTypeDef",
     "AwsCertificateManagerCertificateResourceRecordTypeDef",
     "AwsCloudFormationStackDriftInformationDetailsTypeDef",
     "AwsCloudFormationStackOutputsDetailsTypeDef",
     "AwsCloudFrontDistributionCacheBehaviorTypeDef",
     "AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef",
     "AwsCloudFrontDistributionLoggingTypeDef",
     "AwsCloudFrontDistributionViewerCertificateTypeDef",
+    "AwsCloudFrontDistributionOriginSslProtocolsOutputTypeDef",
     "AwsCloudFrontDistributionOriginSslProtocolsTypeDef",
+    "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesOutputTypeDef",
     "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef",
     "AwsCloudFrontDistributionOriginS3OriginConfigTypeDef",
     "AwsCloudTrailTrailDetailsTypeDef",
     "AwsCloudWatchAlarmDimensionsDetailsTypeDef",
     "AwsCodeBuildProjectArtifactsDetailsTypeDef",
     "AwsCodeBuildProjectSourceTypeDef",
+    "AwsCodeBuildProjectVpcConfigOutputTypeDef",
     "AwsCodeBuildProjectVpcConfigTypeDef",
     "AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef",
     "AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef",
     "AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef",
     "AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef",
     "AwsDynamoDbTableAttributeDefinitionTypeDef",
     "AwsDynamoDbTableBillingModeSummaryTypeDef",
     "AwsDynamoDbTableKeySchemaTypeDef",
     "AwsDynamoDbTableProvisionedThroughputTypeDef",
     "AwsDynamoDbTableRestoreSummaryTypeDef",
     "AwsDynamoDbTableSseDescriptionTypeDef",
     "AwsDynamoDbTableStreamSpecificationTypeDef",
+    "AwsDynamoDbTableProjectionOutputTypeDef",
     "AwsDynamoDbTableProjectionTypeDef",
     "AwsDynamoDbTableProvisionedThroughputOverrideTypeDef",
     "AwsEc2EipDetailsTypeDef",
     "AwsEc2InstanceMetadataOptionsTypeDef",
     "AwsEc2InstanceMonitoringDetailsTypeDef",
     "AwsEc2InstanceNetworkInterfacesDetailsTypeDef",
     "AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef",
@@ -188,86 +198,101 @@
     "PropagatingVgwSetDetailsTypeDef",
     "RouteSetDetailsTypeDef",
     "AwsEc2SecurityGroupIpRangeTypeDef",
     "AwsEc2SecurityGroupIpv6RangeTypeDef",
     "AwsEc2SecurityGroupPrefixListIdTypeDef",
     "AwsEc2SecurityGroupUserIdGroupPairTypeDef",
     "Ipv6CidrBlockAssociationTypeDef",
+    "AwsEc2TransitGatewayDetailsOutputTypeDef",
     "AwsEc2TransitGatewayDetailsTypeDef",
     "AwsEc2VolumeAttachmentTypeDef",
     "CidrBlockAssociationTypeDef",
     "AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef",
     "AwsEc2VpcPeeringConnectionStatusDetailsTypeDef",
     "VpcInfoCidrBlockSetDetailsTypeDef",
     "VpcInfoIpv6CidrBlockSetDetailsTypeDef",
     "VpcInfoPeeringOptionsDetailsTypeDef",
     "AwsEc2VpnConnectionRoutesDetailsTypeDef",
     "AwsEc2VpnConnectionVgwTelemetryDetailsTypeDef",
+    "AwsEc2VpnConnectionOptionsTunnelOptionsDetailsOutputTypeDef",
     "AwsEc2VpnConnectionOptionsTunnelOptionsDetailsTypeDef",
+    "AwsEcrContainerImageDetailsOutputTypeDef",
     "AwsEcrContainerImageDetailsTypeDef",
     "AwsEcrRepositoryImageScanningConfigurationDetailsTypeDef",
     "AwsEcrRepositoryLifecyclePolicyDetailsTypeDef",
     "AwsEcsClusterClusterSettingsDetailsTypeDef",
     "AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef",
     "AwsEcsClusterDefaultCapacityProviderStrategyDetailsTypeDef",
     "AwsMountPointTypeDef",
     "AwsEcsServiceCapacityProviderStrategyDetailsTypeDef",
     "AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef",
     "AwsEcsServiceDeploymentControllerDetailsTypeDef",
     "AwsEcsServiceLoadBalancersDetailsTypeDef",
     "AwsEcsServicePlacementConstraintsDetailsTypeDef",
     "AwsEcsServicePlacementStrategiesDetailsTypeDef",
     "AwsEcsServiceServiceRegistriesDetailsTypeDef",
+    "AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsOutputTypeDef",
     "AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsOutputTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef",
     "AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef",
     "AwsEcsTaskDefinitionPlacementConstraintsDetailsTypeDef",
     "AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef",
-    "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef",
+    "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionVolumesHostDetailsTypeDef",
+    "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef",
     "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef",
     "AwsEcsTaskVolumeHostDetailsTypeDef",
+    "AwsEfsAccessPointPosixUserDetailsOutputTypeDef",
     "AwsEfsAccessPointPosixUserDetailsTypeDef",
     "AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef",
+    "AwsEksClusterResourcesVpcConfigDetailsOutputTypeDef",
     "AwsEksClusterResourcesVpcConfigDetailsTypeDef",
+    "AwsEksClusterLoggingClusterLoggingDetailsOutputTypeDef",
     "AwsEksClusterLoggingClusterLoggingDetailsTypeDef",
     "AwsElasticBeanstalkEnvironmentEnvironmentLinkTypeDef",
     "AwsElasticBeanstalkEnvironmentOptionSettingTypeDef",
     "AwsElasticBeanstalkEnvironmentTierTypeDef",
     "AwsElasticsearchDomainDomainEndpointOptionsTypeDef",
     "AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef",
     "AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef",
     "AwsElasticsearchDomainServiceSoftwareOptionsTypeDef",
+    "AwsElasticsearchDomainVPCOptionsOutputTypeDef",
     "AwsElasticsearchDomainVPCOptionsTypeDef",
     "AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef",
     "AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef",
     "AwsElbAppCookieStickinessPolicyTypeDef",
     "AwsElbLbCookieStickinessPolicyTypeDef",
     "AwsElbLoadBalancerAccessLogTypeDef",
     "AwsElbLoadBalancerAdditionalAttributeTypeDef",
     "AwsElbLoadBalancerConnectionDrainingTypeDef",
     "AwsElbLoadBalancerConnectionSettingsTypeDef",
     "AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef",
+    "AwsElbLoadBalancerBackendServerDescriptionOutputTypeDef",
     "AwsElbLoadBalancerBackendServerDescriptionTypeDef",
     "AwsElbLoadBalancerHealthCheckTypeDef",
     "AwsElbLoadBalancerInstanceTypeDef",
     "AwsElbLoadBalancerSourceSecurityGroupTypeDef",
     "AwsElbLoadBalancerListenerTypeDef",
     "AwsElbv2LoadBalancerAttributeTypeDef",
     "LoadBalancerStateTypeDef",
@@ -290,42 +315,48 @@
     "AwsIamUserPolicyTypeDef",
     "AwsKinesisStreamStreamEncryptionDetailsTypeDef",
     "AwsKmsKeyDetailsTypeDef",
     "AwsLambdaFunctionCodeTypeDef",
     "AwsLambdaFunctionDeadLetterConfigTypeDef",
     "AwsLambdaFunctionLayerTypeDef",
     "AwsLambdaFunctionTracingConfigTypeDef",
+    "AwsLambdaFunctionVpcConfigOutputTypeDef",
     "AwsLambdaFunctionVpcConfigTypeDef",
     "AwsLambdaFunctionEnvironmentErrorTypeDef",
+    "AwsLambdaLayerVersionDetailsOutputTypeDef",
     "AwsLambdaLayerVersionDetailsTypeDef",
     "AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef",
     "AwsOpenSearchServiceDomainMasterUserOptionsDetailsTypeDef",
     "AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef",
     "AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef",
     "AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsTypeDef",
     "AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsTypeDef",
     "AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsTypeDef",
+    "AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef",
     "AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef",
     "AwsOpenSearchServiceDomainLogPublishingOptionTypeDef",
     "AwsRdsDbClusterAssociatedRoleTypeDef",
     "AwsRdsDbClusterMemberTypeDef",
     "AwsRdsDbClusterOptionGroupMembershipTypeDef",
     "AwsRdsDbDomainMembershipTypeDef",
     "AwsRdsDbInstanceVpcSecurityGroupTypeDef",
+    "AwsRdsDbClusterSnapshotDetailsOutputTypeDef",
     "AwsRdsDbClusterSnapshotDetailsTypeDef",
     "AwsRdsDbInstanceAssociatedRoleTypeDef",
     "AwsRdsDbInstanceEndpointTypeDef",
     "AwsRdsDbOptionGroupMembershipTypeDef",
     "AwsRdsDbParameterGroupTypeDef",
     "AwsRdsDbProcessorFeatureTypeDef",
     "AwsRdsDbStatusInfoTypeDef",
+    "AwsRdsPendingCloudWatchLogsExportsOutputTypeDef",
     "AwsRdsPendingCloudWatchLogsExportsTypeDef",
     "AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef",
     "AwsRdsDbSecurityGroupIpRangeTypeDef",
     "AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef",
+    "AwsRdsEventSubscriptionDetailsOutputTypeDef",
     "AwsRdsEventSubscriptionDetailsTypeDef",
     "AwsRedshiftClusterClusterNodeTypeDef",
     "AwsRedshiftClusterClusterParameterStatusTypeDef",
     "AwsRedshiftClusterClusterSecurityGroupTypeDef",
     "AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef",
     "AwsRedshiftClusterDeferredMaintenanceWindowTypeDef",
     "AwsRedshiftClusterElasticIpStatusTypeDef",
@@ -382,14 +413,15 @@
     "WafExcludedRuleTypeDef",
     "WafOverrideActionTypeDef",
     "AwsWafv2CustomHttpHeaderTypeDef",
     "AwsWafv2VisibilityConfigDetailsTypeDef",
     "AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef",
     "AwsXrayEncryptionConfigDetailsTypeDef",
     "BatchDeleteAutomationRulesRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "UnprocessedAutomationRuleTypeDef",
     "BatchDisableStandardsRequestRequestTypeDef",
     "StandardsSubscriptionRequestTypeDef",
     "BatchGetAutomationRulesRequestRequestTypeDef",
     "BatchGetSecurityControlsRequestRequestTypeDef",
     "SecurityControlTypeDef",
     "UnprocessedSecurityControlTypeDef",
@@ -398,396 +430,571 @@
     "ImportFindingsErrorTypeDef",
     "StandardsControlAssociationUpdateTypeDef",
     "CellTypeDef",
     "ClassificationStatusTypeDef",
     "StatusReasonTypeDef",
     "VolumeMountTypeDef",
     "CreateActionTargetRequestRequestTypeDef",
-    "CreateActionTargetResponseTypeDef",
-    "CreateAutomationRuleResponseTypeDef",
     "CreateFindingAggregatorRequestRequestTypeDef",
-    "CreateFindingAggregatorResponseTypeDef",
-    "CreateInsightResponseTypeDef",
     "ResultTypeDef",
     "DateRangeTypeDef",
     "DeclineInvitationsRequestRequestTypeDef",
     "DeleteActionTargetRequestRequestTypeDef",
-    "DeleteActionTargetResponseTypeDef",
     "DeleteFindingAggregatorRequestRequestTypeDef",
     "DeleteInsightRequestRequestTypeDef",
-    "DeleteInsightResponseTypeDef",
     "DeleteInvitationsRequestRequestTypeDef",
     "DeleteMembersRequestRequestTypeDef",
-    "DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeActionTargetsRequestRequestTypeDef",
     "DescribeHubRequestRequestTypeDef",
-    "DescribeHubResponseTypeDef",
-    "DescribeOrganizationConfigurationResponseTypeDef",
-    "DescribeProductsRequestDescribeProductsPaginateTypeDef",
     "DescribeProductsRequestRequestTypeDef",
     "ProductTypeDef",
-    "DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef",
     "DescribeStandardsControlsRequestRequestTypeDef",
     "StandardsControlTypeDef",
-    "DescribeStandardsRequestDescribeStandardsPaginateTypeDef",
     "DescribeStandardsRequestRequestTypeDef",
     "DisableImportFindingsForProductRequestRequestTypeDef",
     "DisableOrganizationAdminAccountRequestRequestTypeDef",
     "DisassociateMembersRequestRequestTypeDef",
     "EnableImportFindingsForProductRequestRequestTypeDef",
-    "EnableImportFindingsForProductResponseTypeDef",
     "EnableOrganizationAdminAccountRequestRequestTypeDef",
     "EnableSecurityHubRequestRequestTypeDef",
     "FilePathsTypeDef",
     "FindingAggregatorTypeDef",
     "FindingHistoryUpdateSourceTypeDef",
     "FindingHistoryUpdateTypeDef",
     "FindingProviderSeverityTypeDef",
     "FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef",
     "FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef",
     "InvitationTypeDef",
-    "GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef",
     "GetEnabledStandardsRequestRequestTypeDef",
     "GetFindingAggregatorRequestRequestTypeDef",
-    "GetFindingAggregatorResponseTypeDef",
+    "TimestampTypeDef",
     "SortCriterionTypeDef",
     "GetInsightResultsRequestRequestTypeDef",
-    "GetInsightsRequestGetInsightsPaginateTypeDef",
     "GetInsightsRequestRequestTypeDef",
-    "GetInvitationsCountResponseTypeDef",
     "GetMembersRequestRequestTypeDef",
     "MemberTypeDef",
     "InsightResultValueTypeDef",
     "InviteMembersRequestRequestTypeDef",
     "ListAutomationRulesRequestRequestTypeDef",
-    "ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef",
     "ListEnabledProductsForImportRequestRequestTypeDef",
-    "ListEnabledProductsForImportResponseTypeDef",
-    "ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef",
     "ListFindingAggregatorsRequestRequestTypeDef",
-    "ListInvitationsRequestListInvitationsPaginateTypeDef",
     "ListInvitationsRequestRequestTypeDef",
-    "ListMembersRequestListMembersPaginateTypeDef",
     "ListMembersRequestRequestTypeDef",
-    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
-    "ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef",
     "ListSecurityControlDefinitionsRequestRequestTypeDef",
     "SecurityControlDefinitionTypeDef",
-    "ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef",
     "ListStandardsControlAssociationsRequestRequestTypeDef",
     "StandardsControlAssociationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "PortRangeTypeDef",
     "RangeTypeDef",
     "RecordTypeDef",
-    "PaginatorConfigTypeDef",
     "RecommendationTypeDef",
-    "ResponseMetadataTypeDef",
+    "RuleGroupSourceListDetailsOutputTypeDef",
     "RuleGroupSourceListDetailsTypeDef",
     "RuleGroupSourceStatefulRulesHeaderDetailsTypeDef",
+    "RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef",
     "RuleGroupSourceStatefulRulesOptionsDetailsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef",
+    "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef",
+    "RuleGroupVariablesIpSetsDetailsOutputTypeDef",
     "RuleGroupVariablesIpSetsDetailsTypeDef",
+    "RuleGroupVariablesPortSetsDetailsOutputTypeDef",
     "RuleGroupVariablesPortSetsDetailsTypeDef",
     "SoftwarePackageTypeDef",
     "StandardsManagedByTypeDef",
     "StandardsStatusReasonTypeDef",
     "StatelessCustomPublishMetricActionDimensionTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateActionTargetRequestRequestTypeDef",
     "UpdateFindingAggregatorRequestRequestTypeDef",
-    "UpdateFindingAggregatorResponseTypeDef",
     "UpdateOrganizationConfigurationRequestRequestTypeDef",
     "UpdateSecurityHubConfigurationRequestRequestTypeDef",
     "UpdateStandardsControlRequestRequestTypeDef",
     "VulnerabilityVendorTypeDef",
     "CreateMembersRequestRequestTypeDef",
     "ActionRemoteIpDetailsTypeDef",
-    "DescribeActionTargetsResponseTypeDef",
+    "CvssOutputTypeDef",
     "CvssTypeDef",
-    "ListOrganizationAdminAccountsResponseTypeDef",
     "AssociationSetDetailsTypeDef",
+    "AutomationRulesFindingFieldsUpdateOutputTypeDef",
     "AutomationRulesFindingFieldsUpdateTypeDef",
-    "ListAutomationRulesResponseTypeDef",
     "AwsAmazonMqBrokerLogsDetailsTypeDef",
+    "AwsApiGatewayRestApiDetailsOutputTypeDef",
     "AwsApiGatewayRestApiDetailsTypeDef",
+    "AwsApiGatewayStageDetailsOutputTypeDef",
     "AwsApiGatewayStageDetailsTypeDef",
+    "AwsApiGatewayV2ApiDetailsOutputTypeDef",
     "AwsApiGatewayV2ApiDetailsTypeDef",
+    "AwsApiGatewayV2StageDetailsOutputTypeDef",
     "AwsApiGatewayV2StageDetailsTypeDef",
     "AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef",
+    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef",
     "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef",
     "AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef",
+    "AwsBackupBackupVaultDetailsOutputTypeDef",
     "AwsBackupBackupVaultDetailsTypeDef",
     "AwsBackupRecoveryPointDetailsTypeDef",
+    "AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef",
     "AwsCertificateManagerCertificateDomainValidationOptionTypeDef",
+    "AwsCloudFormationStackDetailsOutputTypeDef",
     "AwsCloudFormationStackDetailsTypeDef",
+    "AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef",
     "AwsCloudFrontDistributionCacheBehaviorsTypeDef",
+    "AwsCloudFrontDistributionOriginCustomOriginConfigOutputTypeDef",
     "AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef",
+    "AwsCloudFrontDistributionOriginGroupFailoverOutputTypeDef",
     "AwsCloudFrontDistributionOriginGroupFailoverTypeDef",
+    "AwsCloudWatchAlarmDetailsOutputTypeDef",
     "AwsCloudWatchAlarmDetailsTypeDef",
+    "AwsCodeBuildProjectEnvironmentOutputTypeDef",
     "AwsCodeBuildProjectEnvironmentTypeDef",
     "AwsCodeBuildProjectLogsConfigDetailsTypeDef",
+    "AwsDynamoDbTableGlobalSecondaryIndexOutputTypeDef",
+    "AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef",
     "AwsDynamoDbTableGlobalSecondaryIndexTypeDef",
     "AwsDynamoDbTableLocalSecondaryIndexTypeDef",
     "AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef",
+    "AwsEc2InstanceDetailsOutputTypeDef",
     "AwsEc2InstanceDetailsTypeDef",
     "AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef",
     "AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef",
     "AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef",
     "AwsEc2NetworkAclEntryTypeDef",
+    "AwsEc2NetworkInterfaceDetailsOutputTypeDef",
     "AwsEc2NetworkInterfaceDetailsTypeDef",
+    "AwsEc2SecurityGroupIpPermissionOutputTypeDef",
     "AwsEc2SecurityGroupIpPermissionTypeDef",
+    "AwsEc2SubnetDetailsOutputTypeDef",
     "AwsEc2SubnetDetailsTypeDef",
+    "AwsEc2VolumeDetailsOutputTypeDef",
     "AwsEc2VolumeDetailsTypeDef",
+    "AwsEc2VpcDetailsOutputTypeDef",
     "AwsEc2VpcDetailsTypeDef",
+    "AwsEc2VpcEndpointServiceDetailsOutputTypeDef",
     "AwsEc2VpcEndpointServiceDetailsTypeDef",
+    "AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef",
     "AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef",
+    "AwsEc2VpnConnectionOptionsDetailsOutputTypeDef",
     "AwsEc2VpnConnectionOptionsDetailsTypeDef",
     "AwsEcrRepositoryDetailsTypeDef",
     "AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef",
+    "AwsEcsContainerDetailsOutputTypeDef",
     "AwsEcsContainerDetailsTypeDef",
     "AwsEcsServiceDeploymentConfigurationDetailsTypeDef",
+    "AwsEcsServiceNetworkConfigurationDetailsOutputTypeDef",
     "AwsEcsServiceNetworkConfigurationDetailsTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef",
+    "AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionProxyConfigurationDetailsTypeDef",
     "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef",
     "AwsEcsTaskVolumeDetailsTypeDef",
     "AwsEfsAccessPointRootDirectoryDetailsTypeDef",
+    "AwsEksClusterLoggingDetailsOutputTypeDef",
     "AwsEksClusterLoggingDetailsTypeDef",
+    "AwsElasticBeanstalkEnvironmentDetailsOutputTypeDef",
     "AwsElasticBeanstalkEnvironmentDetailsTypeDef",
     "AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef",
     "AwsElasticsearchDomainLogPublishingOptionsTypeDef",
+    "AwsElbLoadBalancerPoliciesOutputTypeDef",
     "AwsElbLoadBalancerPoliciesTypeDef",
+    "AwsElbLoadBalancerAttributesOutputTypeDef",
     "AwsElbLoadBalancerAttributesTypeDef",
+    "AwsElbLoadBalancerListenerDescriptionOutputTypeDef",
     "AwsElbLoadBalancerListenerDescriptionTypeDef",
+    "AwsElbv2LoadBalancerDetailsOutputTypeDef",
     "AwsElbv2LoadBalancerDetailsTypeDef",
     "AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef",
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef",
     "AwsIamAccessKeySessionContextTypeDef",
+    "AwsIamGroupDetailsOutputTypeDef",
     "AwsIamGroupDetailsTypeDef",
+    "AwsIamInstanceProfileOutputTypeDef",
     "AwsIamInstanceProfileTypeDef",
+    "AwsIamPolicyDetailsOutputTypeDef",
     "AwsIamPolicyDetailsTypeDef",
+    "AwsIamUserDetailsOutputTypeDef",
     "AwsIamUserDetailsTypeDef",
     "AwsKinesisStreamDetailsTypeDef",
+    "AwsLambdaFunctionEnvironmentOutputTypeDef",
     "AwsLambdaFunctionEnvironmentTypeDef",
+    "AwsNetworkFirewallFirewallDetailsOutputTypeDef",
     "AwsNetworkFirewallFirewallDetailsTypeDef",
     "AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef",
     "AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef",
     "AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef",
+    "AwsRdsDbClusterDetailsOutputTypeDef",
     "AwsRdsDbClusterDetailsTypeDef",
+    "AwsRdsDbSnapshotDetailsOutputTypeDef",
     "AwsRdsDbSnapshotDetailsTypeDef",
+    "AwsRdsDbPendingModifiedValuesOutputTypeDef",
     "AwsRdsDbPendingModifiedValuesTypeDef",
+    "AwsRdsDbSecurityGroupDetailsOutputTypeDef",
     "AwsRdsDbSecurityGroupDetailsTypeDef",
     "AwsRdsDbSubnetGroupSubnetTypeDef",
+    "AwsRedshiftClusterClusterParameterGroupOutputTypeDef",
     "AwsRedshiftClusterClusterParameterGroupTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef",
+    "AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef",
     "AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef",
     "AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef",
     "AwsS3BucketServerSideEncryptionRuleTypeDef",
     "AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef",
+    "AwsSageMakerNotebookInstanceDetailsOutputTypeDef",
     "AwsSageMakerNotebookInstanceDetailsTypeDef",
     "AwsSecretsManagerSecretDetailsTypeDef",
     "BatchUpdateFindingsRequestRequestTypeDef",
     "BatchUpdateFindingsUnprocessedFindingTypeDef",
-    "GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
-    "GetFindingHistoryRequestRequestTypeDef",
+    "AwsSnsTopicDetailsOutputTypeDef",
     "AwsSnsTopicDetailsTypeDef",
     "AwsSsmPatchTypeDef",
     "AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef",
+    "AwsWafRateBasedRuleDetailsOutputTypeDef",
     "AwsWafRateBasedRuleDetailsTypeDef",
+    "AwsWafRegionalRateBasedRuleDetailsOutputTypeDef",
     "AwsWafRegionalRateBasedRuleDetailsTypeDef",
+    "AwsWafRegionalRuleDetailsOutputTypeDef",
     "AwsWafRegionalRuleDetailsTypeDef",
     "AwsWafRegionalRuleGroupRulesDetailsTypeDef",
     "AwsWafRegionalWebAclRulesListDetailsTypeDef",
+    "AwsWafRuleDetailsOutputTypeDef",
     "AwsWafRuleDetailsTypeDef",
     "AwsWafRuleGroupRulesDetailsTypeDef",
+    "AwsWafWebAclRuleOutputTypeDef",
     "AwsWafWebAclRuleTypeDef",
+    "AwsWafv2CustomRequestHandlingDetailsOutputTypeDef",
     "AwsWafv2CustomRequestHandlingDetailsTypeDef",
+    "AwsWafv2CustomResponseDetailsOutputTypeDef",
     "AwsWafv2CustomResponseDetailsTypeDef",
     "AwsWafv2WebAclCaptchaConfigDetailsTypeDef",
+    "CreateActionTargetResponseTypeDef",
+    "CreateAutomationRuleResponseTypeDef",
+    "CreateFindingAggregatorResponseTypeDef",
+    "CreateInsightResponseTypeDef",
+    "DeleteActionTargetResponseTypeDef",
+    "DeleteInsightResponseTypeDef",
+    "DescribeActionTargetsResponseTypeDef",
+    "DescribeHubResponseTypeDef",
+    "DescribeOrganizationConfigurationResponseTypeDef",
+    "EnableImportFindingsForProductResponseTypeDef",
+    "GetFindingAggregatorResponseTypeDef",
+    "GetInvitationsCountResponseTypeDef",
+    "ListAutomationRulesResponseTypeDef",
+    "ListEnabledProductsForImportResponseTypeDef",
+    "ListOrganizationAdminAccountsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateFindingAggregatorResponseTypeDef",
     "BatchDeleteAutomationRulesResponseTypeDef",
     "BatchUpdateAutomationRulesResponseTypeDef",
     "BatchEnableStandardsRequestRequestTypeDef",
     "BatchGetSecurityControlsResponseTypeDef",
     "BatchGetStandardsControlAssociationsRequestRequestTypeDef",
     "UnprocessedStandardsControlAssociationTypeDef",
     "BatchImportFindingsResponseTypeDef",
     "BatchUpdateStandardsControlAssociationsRequestRequestTypeDef",
     "UnprocessedStandardsControlAssociationUpdateTypeDef",
+    "ComplianceOutputTypeDef",
     "ComplianceTypeDef",
+    "ContainerDetailsOutputTypeDef",
     "ContainerDetailsTypeDef",
     "CreateMembersResponseTypeDef",
     "DeclineInvitationsResponseTypeDef",
     "DeleteInvitationsResponseTypeDef",
     "DeleteMembersResponseTypeDef",
     "InviteMembersResponseTypeDef",
     "DateFilterTypeDef",
+    "DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef",
+    "DescribeProductsRequestDescribeProductsPaginateTypeDef",
+    "DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef",
+    "DescribeStandardsRequestDescribeStandardsPaginateTypeDef",
+    "GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef",
+    "GetInsightsRequestGetInsightsPaginateTypeDef",
+    "ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef",
+    "ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef",
+    "ListInvitationsRequestListInvitationsPaginateTypeDef",
+    "ListMembersRequestListMembersPaginateTypeDef",
+    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
+    "ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef",
+    "ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef",
     "DescribeProductsResponseTypeDef",
     "DescribeStandardsControlsResponseTypeDef",
+    "ThreatOutputTypeDef",
     "ThreatTypeDef",
     "ListFindingAggregatorsResponseTypeDef",
     "FindingHistoryRecordTypeDef",
+    "FindingProviderFieldsOutputTypeDef",
     "FindingProviderFieldsTypeDef",
     "GetAdministratorAccountResponseTypeDef",
     "GetMasterAccountResponseTypeDef",
     "ListInvitationsResponseTypeDef",
+    "GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
+    "GetFindingHistoryRequestRequestTypeDef",
     "GetMembersResponseTypeDef",
     "ListMembersResponseTypeDef",
     "InsightResultsTypeDef",
     "ListSecurityControlDefinitionsResponseTypeDef",
     "ListStandardsControlAssociationsResponseTypeDef",
+    "NetworkPathComponentDetailsOutputTypeDef",
     "NetworkPathComponentDetailsTypeDef",
     "NetworkTypeDef",
     "PageTypeDef",
     "RemediationTypeDef",
+    "RuleGroupSourceStatefulRulesDetailsOutputTypeDef",
     "RuleGroupSourceStatefulRulesDetailsTypeDef",
+    "RuleGroupSourceStatelessRuleMatchAttributesOutputTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesTypeDef",
+    "RuleGroupVariablesOutputTypeDef",
     "RuleGroupVariablesTypeDef",
     "StandardTypeDef",
     "StandardsSubscriptionTypeDef",
+    "StatelessCustomPublishMetricActionOutputTypeDef",
     "StatelessCustomPublishMetricActionTypeDef",
+    "AwsApiCallActionOutputTypeDef",
     "AwsApiCallActionTypeDef",
     "NetworkConnectionActionTypeDef",
     "PortProbeDetailTypeDef",
+    "VulnerabilityOutputTypeDef",
     "VulnerabilityTypeDef",
+    "AwsEc2RouteTableDetailsOutputTypeDef",
     "AwsEc2RouteTableDetailsTypeDef",
+    "AutomationRulesActionOutputTypeDef",
     "AutomationRulesActionTypeDef",
+    "AwsAmazonMqBrokerDetailsOutputTypeDef",
     "AwsAmazonMqBrokerDetailsTypeDef",
+    "AwsAppSyncGraphQlApiDetailsOutputTypeDef",
     "AwsAppSyncGraphQlApiDetailsTypeDef",
+    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef",
+    "AwsAutoScalingLaunchConfigurationDetailsOutputTypeDef",
     "AwsAutoScalingLaunchConfigurationDetailsTypeDef",
+    "AwsBackupBackupPlanRuleDetailsOutputTypeDef",
     "AwsBackupBackupPlanRuleDetailsTypeDef",
+    "AwsCertificateManagerCertificateRenewalSummaryOutputTypeDef",
     "AwsCertificateManagerCertificateRenewalSummaryTypeDef",
+    "AwsCloudFrontDistributionOriginItemOutputTypeDef",
     "AwsCloudFrontDistributionOriginItemTypeDef",
+    "AwsCloudFrontDistributionOriginGroupOutputTypeDef",
     "AwsCloudFrontDistributionOriginGroupTypeDef",
+    "AwsCodeBuildProjectDetailsOutputTypeDef",
     "AwsCodeBuildProjectDetailsTypeDef",
+    "AwsDynamoDbTableReplicaOutputTypeDef",
     "AwsDynamoDbTableReplicaTypeDef",
+    "AwsEc2LaunchTemplateDataDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataDetailsTypeDef",
+    "AwsEc2NetworkAclDetailsOutputTypeDef",
     "AwsEc2NetworkAclDetailsTypeDef",
+    "AwsEc2SecurityGroupDetailsOutputTypeDef",
     "AwsEc2SecurityGroupDetailsTypeDef",
+    "AwsEc2VpcPeeringConnectionDetailsOutputTypeDef",
     "AwsEc2VpcPeeringConnectionDetailsTypeDef",
+    "AwsEc2VpnConnectionDetailsOutputTypeDef",
     "AwsEc2VpnConnectionDetailsTypeDef",
     "AwsEcsClusterConfigurationDetailsTypeDef",
+    "AwsEcsServiceDetailsOutputTypeDef",
     "AwsEcsServiceDetailsTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef",
+    "AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionVolumesDetailsTypeDef",
+    "AwsEcsTaskDetailsOutputTypeDef",
     "AwsEcsTaskDetailsTypeDef",
+    "AwsEfsAccessPointDetailsOutputTypeDef",
     "AwsEfsAccessPointDetailsTypeDef",
+    "AwsEksClusterDetailsOutputTypeDef",
     "AwsEksClusterDetailsTypeDef",
+    "AwsElasticsearchDomainDetailsOutputTypeDef",
     "AwsElasticsearchDomainDetailsTypeDef",
+    "AwsElbLoadBalancerDetailsOutputTypeDef",
     "AwsElbLoadBalancerDetailsTypeDef",
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef",
     "AwsIamAccessKeyDetailsTypeDef",
+    "AwsIamRoleDetailsOutputTypeDef",
     "AwsIamRoleDetailsTypeDef",
+    "AwsLambdaFunctionDetailsOutputTypeDef",
     "AwsLambdaFunctionDetailsTypeDef",
+    "AwsOpenSearchServiceDomainDetailsOutputTypeDef",
     "AwsOpenSearchServiceDomainDetailsTypeDef",
+    "AwsRdsDbSubnetGroupOutputTypeDef",
     "AwsRdsDbSubnetGroupTypeDef",
+    "AwsRedshiftClusterDetailsOutputTypeDef",
     "AwsRedshiftClusterDetailsTypeDef",
+    "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef",
+    "AwsS3BucketNotificationConfigurationFilterOutputTypeDef",
     "AwsS3BucketNotificationConfigurationFilterTypeDef",
     "AwsS3BucketObjectLockConfigurationTypeDef",
+    "AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef",
     "AwsS3BucketServerSideEncryptionConfigurationTypeDef",
+    "AwsS3BucketWebsiteConfigurationOutputTypeDef",
     "AwsS3BucketWebsiteConfigurationTypeDef",
     "BatchUpdateFindingsResponseTypeDef",
     "AwsSsmPatchComplianceDetailsTypeDef",
+    "AwsStepFunctionStateMachineLoggingConfigurationDetailsOutputTypeDef",
     "AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef",
+    "AwsWafRegionalRuleGroupDetailsOutputTypeDef",
     "AwsWafRegionalRuleGroupDetailsTypeDef",
+    "AwsWafRegionalWebAclDetailsOutputTypeDef",
     "AwsWafRegionalWebAclDetailsTypeDef",
+    "AwsWafRuleGroupDetailsOutputTypeDef",
     "AwsWafRuleGroupDetailsTypeDef",
+    "AwsWafWebAclDetailsOutputTypeDef",
     "AwsWafWebAclDetailsTypeDef",
+    "AwsWafv2ActionAllowDetailsOutputTypeDef",
+    "AwsWafv2RulesActionCaptchaDetailsOutputTypeDef",
+    "AwsWafv2RulesActionCountDetailsOutputTypeDef",
     "AwsWafv2ActionAllowDetailsTypeDef",
     "AwsWafv2RulesActionCaptchaDetailsTypeDef",
     "AwsWafv2RulesActionCountDetailsTypeDef",
+    "AwsWafv2ActionBlockDetailsOutputTypeDef",
     "AwsWafv2ActionBlockDetailsTypeDef",
     "BatchGetStandardsControlAssociationsResponseTypeDef",
     "BatchUpdateStandardsControlAssociationsResponseTypeDef",
+    "AutomationRulesFindingFiltersOutputTypeDef",
     "AutomationRulesFindingFiltersTypeDef",
+    "AwsSecurityFindingFiltersOutputTypeDef",
     "AwsSecurityFindingFiltersTypeDef",
     "GetFindingHistoryResponseTypeDef",
     "GetInsightResultsResponseTypeDef",
+    "NetworkHeaderOutputTypeDef",
     "NetworkHeaderTypeDef",
+    "OccurrencesOutputTypeDef",
     "OccurrencesTypeDef",
+    "RuleGroupSourceStatelessRuleDefinitionOutputTypeDef",
     "RuleGroupSourceStatelessRuleDefinitionTypeDef",
     "DescribeStandardsResponseTypeDef",
     "BatchDisableStandardsResponseTypeDef",
     "BatchEnableStandardsResponseTypeDef",
     "GetEnabledStandardsResponseTypeDef",
+    "StatelessCustomActionDefinitionOutputTypeDef",
     "StatelessCustomActionDefinitionTypeDef",
+    "PortProbeActionOutputTypeDef",
     "PortProbeActionTypeDef",
+    "AutomationRulesActionUnionTypeDef",
+    "AwsAutoScalingAutoScalingGroupDetailsOutputTypeDef",
     "AwsAutoScalingAutoScalingGroupDetailsTypeDef",
+    "AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef",
     "AwsBackupBackupPlanBackupPlanDetailsTypeDef",
+    "AwsCertificateManagerCertificateDetailsOutputTypeDef",
     "AwsCertificateManagerCertificateDetailsTypeDef",
+    "AwsCloudFrontDistributionOriginsOutputTypeDef",
     "AwsCloudFrontDistributionOriginsTypeDef",
+    "AwsCloudFrontDistributionOriginGroupsOutputTypeDef",
     "AwsCloudFrontDistributionOriginGroupsTypeDef",
+    "AwsDynamoDbTableDetailsOutputTypeDef",
     "AwsDynamoDbTableDetailsTypeDef",
+    "AwsEc2LaunchTemplateDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDetailsTypeDef",
+    "AwsEcsClusterDetailsOutputTypeDef",
     "AwsEcsClusterDetailsTypeDef",
+    "AwsEcsTaskDefinitionDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionDetailsTypeDef",
     "AwsGuardDutyDetectorDataSourcesDetailsTypeDef",
+    "AwsRdsDbInstanceDetailsOutputTypeDef",
     "AwsRdsDbInstanceDetailsTypeDef",
+    "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef",
+    "AwsS3BucketNotificationConfigurationDetailOutputTypeDef",
     "AwsS3BucketNotificationConfigurationDetailTypeDef",
+    "AwsStepFunctionStateMachineDetailsOutputTypeDef",
     "AwsStepFunctionStateMachineDetailsTypeDef",
+    "AwsWafv2RulesActionDetailsOutputTypeDef",
+    "AwsWafv2WebAclActionDetailsOutputTypeDef",
     "AwsWafv2RulesActionDetailsTypeDef",
     "AwsWafv2WebAclActionDetailsTypeDef",
     "AutomationRulesConfigTypeDef",
-    "CreateAutomationRuleRequestRequestTypeDef",
+    "AutomationRulesFindingFiltersUnionTypeDef",
     "UpdateAutomationRulesRequestItemTypeDef",
+    "InsightTypeDef",
+    "AwsSecurityFindingFiltersUnionTypeDef",
     "CreateInsightRequestRequestTypeDef",
     "GetFindingsRequestGetFindingsPaginateTypeDef",
     "GetFindingsRequestRequestTypeDef",
-    "InsightTypeDef",
     "UpdateFindingsRequestRequestTypeDef",
     "UpdateInsightRequestRequestTypeDef",
+    "NetworkPathComponentOutputTypeDef",
     "NetworkPathComponentTypeDef",
+    "CustomDataIdentifiersDetectionsOutputTypeDef",
+    "SensitiveDataDetectionsOutputTypeDef",
     "CustomDataIdentifiersDetectionsTypeDef",
     "SensitiveDataDetectionsTypeDef",
+    "RuleGroupSourceStatelessRulesDetailsOutputTypeDef",
     "RuleGroupSourceStatelessRulesDetailsTypeDef",
+    "FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef",
+    "RuleGroupSourceCustomActionsDetailsOutputTypeDef",
     "FirewallPolicyStatelessCustomActionsDetailsTypeDef",
     "RuleGroupSourceCustomActionsDetailsTypeDef",
+    "ActionOutputTypeDef",
     "ActionTypeDef",
+    "CreateAutomationRuleRequestRequestTypeDef",
+    "AwsBackupBackupPlanDetailsOutputTypeDef",
     "AwsBackupBackupPlanDetailsTypeDef",
+    "AwsCloudFrontDistributionDetailsOutputTypeDef",
     "AwsCloudFrontDistributionDetailsTypeDef",
+    "AwsGuardDutyDetectorDetailsOutputTypeDef",
     "AwsGuardDutyDetectorDetailsTypeDef",
+    "AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef",
+    "AwsS3BucketNotificationConfigurationOutputTypeDef",
     "AwsS3BucketNotificationConfigurationTypeDef",
+    "AwsWafv2RulesDetailsOutputTypeDef",
     "AwsWafv2RulesDetailsTypeDef",
     "BatchGetAutomationRulesResponseTypeDef",
     "BatchUpdateAutomationRulesRequestRequestTypeDef",
     "GetInsightsResponseTypeDef",
+    "CustomDataIdentifiersResultOutputTypeDef",
+    "SensitiveDataResultOutputTypeDef",
     "CustomDataIdentifiersResultTypeDef",
     "SensitiveDataResultTypeDef",
+    "FirewallPolicyDetailsOutputTypeDef",
+    "RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef",
     "FirewallPolicyDetailsTypeDef",
     "RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef",
+    "AwsS3BucketBucketLifecycleConfigurationDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef",
+    "AwsWafv2RuleGroupDetailsOutputTypeDef",
+    "AwsWafv2WebAclDetailsOutputTypeDef",
     "AwsWafv2RuleGroupDetailsTypeDef",
     "AwsWafv2WebAclDetailsTypeDef",
+    "ClassificationResultOutputTypeDef",
     "ClassificationResultTypeDef",
+    "AwsNetworkFirewallFirewallPolicyDetailsOutputTypeDef",
+    "RuleGroupSourceOutputTypeDef",
     "AwsNetworkFirewallFirewallPolicyDetailsTypeDef",
     "RuleGroupSourceTypeDef",
+    "AwsS3BucketDetailsOutputTypeDef",
     "AwsS3BucketDetailsTypeDef",
+    "DataClassificationDetailsOutputTypeDef",
     "DataClassificationDetailsTypeDef",
+    "RuleGroupDetailsOutputTypeDef",
     "RuleGroupDetailsTypeDef",
+    "AwsNetworkFirewallRuleGroupDetailsOutputTypeDef",
     "AwsNetworkFirewallRuleGroupDetailsTypeDef",
+    "ResourceDetailsOutputTypeDef",
     "ResourceDetailsTypeDef",
+    "ResourceOutputTypeDef",
     "ResourceTypeDef",
+    "AwsSecurityFindingOutputTypeDef",
     "AwsSecurityFindingTypeDef",
-    "BatchImportFindingsRequestRequestTypeDef",
     "GetFindingsResponseTypeDef",
+    "AwsSecurityFindingUnionTypeDef",
+    "BatchImportFindingsRequestRequestTypeDef",
 )
 
 AcceptAdministratorInvitationRequestRequestTypeDef = TypedDict(
     "AcceptAdministratorInvitationRequestRequestTypeDef",
     {
         "AdministratorId": str,
         "InvitationId": str,
@@ -834,14 +1041,24 @@
     {
         "Port": int,
         "PortName": str,
     },
     total=False,
 )
 
+DnsRequestActionTypeDef = TypedDict(
+    "DnsRequestActionTypeDef",
+    {
+        "Domain": str,
+        "Protocol": str,
+        "Blocked": bool,
+    },
+    total=False,
+)
+
 CityTypeDef = TypedDict(
     "CityTypeDef",
     {
         "CityName": str,
     },
     total=False,
 )
@@ -889,24 +1106,14 @@
     {
         "ActionTargetArn": str,
         "Name": str,
         "Description": str,
     },
 )
 
-DnsRequestActionTypeDef = TypedDict(
-    "DnsRequestActionTypeDef",
-    {
-        "Domain": str,
-        "Protocol": str,
-        "Blocked": bool,
-    },
-    total=False,
-)
-
 AdjustmentTypeDef = TypedDict(
     "AdjustmentTypeDef",
     {
         "Metric": str,
         "Reason": str,
     },
     total=False,
@@ -1031,18 +1238,18 @@
     {
         "KmsKeyId": str,
         "UseAwsOwnedKey": bool,
     },
     total=False,
 )
 
-AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef = TypedDict(
-    "AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef",
+AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef = TypedDict(
+    "AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef",
     {
-        "Hosts": Sequence[str],
+        "Hosts": List[str],
         "RoleBase": str,
         "RoleName": str,
         "RoleSearchMatching": str,
         "RoleSearchSubtree": bool,
         "ServiceAccountUsername": str,
         "UserBase": str,
         "UserRoleName": str,
@@ -1067,14 +1274,31 @@
     {
         "PendingChange": str,
         "Username": str,
     },
     total=False,
 )
 
+AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef = TypedDict(
+    "AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef",
+    {
+        "Hosts": Sequence[str],
+        "RoleBase": str,
+        "RoleName": str,
+        "RoleSearchMatching": str,
+        "RoleSearchSubtree": bool,
+        "ServiceAccountUsername": str,
+        "UserBase": str,
+        "UserRoleName": str,
+        "UserSearchMatching": str,
+        "UserSearchSubtree": bool,
+    },
+    total=False,
+)
+
 AwsAmazonMqBrokerLogsPendingDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerLogsPendingDetailsTypeDef",
     {
         "Audit": bool,
         "General": bool,
     },
     total=False,
@@ -1093,25 +1317,44 @@
     {
         "Format": str,
         "DestinationArn": str,
     },
     total=False,
 )
 
+AwsApiGatewayCanarySettingsOutputTypeDef = TypedDict(
+    "AwsApiGatewayCanarySettingsOutputTypeDef",
+    {
+        "PercentTraffic": float,
+        "DeploymentId": str,
+        "StageVariableOverrides": Dict[str, str],
+        "UseStageCache": bool,
+    },
+    total=False,
+)
+
 AwsApiGatewayCanarySettingsTypeDef = TypedDict(
     "AwsApiGatewayCanarySettingsTypeDef",
     {
         "PercentTraffic": float,
         "DeploymentId": str,
         "StageVariableOverrides": Mapping[str, str],
         "UseStageCache": bool,
     },
     total=False,
 )
 
+AwsApiGatewayEndpointConfigurationOutputTypeDef = TypedDict(
+    "AwsApiGatewayEndpointConfigurationOutputTypeDef",
+    {
+        "Types": List[str],
+    },
+    total=False,
+)
+
 AwsApiGatewayEndpointConfigurationTypeDef = TypedDict(
     "AwsApiGatewayEndpointConfigurationTypeDef",
     {
         "Types": Sequence[str],
     },
     total=False,
 )
@@ -1131,14 +1374,27 @@
         "UnauthorizedCacheControlHeaderStrategy": str,
         "HttpMethod": str,
         "ResourcePath": str,
     },
     total=False,
 )
 
+AwsCorsConfigurationOutputTypeDef = TypedDict(
+    "AwsCorsConfigurationOutputTypeDef",
+    {
+        "AllowOrigins": List[str],
+        "AllowCredentials": bool,
+        "ExposeHeaders": List[str],
+        "MaxAge": int,
+        "AllowMethods": List[str],
+        "AllowHeaders": List[str],
+    },
+    total=False,
+)
+
 AwsCorsConfigurationTypeDef = TypedDict(
     "AwsCorsConfigurationTypeDef",
     {
         "AllowOrigins": Sequence[str],
         "AllowCredentials": bool,
         "ExposeHeaders": Sequence[str],
         "MaxAge": int,
@@ -1279,14 +1535,23 @@
         "HttpEndpoint": str,
         "HttpPutResponseHopLimit": int,
         "HttpTokens": str,
     },
     total=False,
 )
 
+AwsBackupBackupPlanAdvancedBackupSettingsDetailsOutputTypeDef = TypedDict(
+    "AwsBackupBackupPlanAdvancedBackupSettingsDetailsOutputTypeDef",
+    {
+        "BackupOptions": Dict[str, str],
+        "ResourceType": str,
+    },
+    total=False,
+)
+
 AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef",
     {
         "BackupOptions": Mapping[str, str],
         "ResourceType": str,
     },
     total=False,
@@ -1297,14 +1562,23 @@
     {
         "DeleteAfterDays": int,
         "MoveToColdStorageAfterDays": int,
     },
     total=False,
 )
 
+AwsBackupBackupVaultNotificationsDetailsOutputTypeDef = TypedDict(
+    "AwsBackupBackupVaultNotificationsDetailsOutputTypeDef",
+    {
+        "BackupVaultEvents": List[str],
+        "SnsTopicArn": str,
+    },
+    total=False,
+)
+
 AwsBackupBackupVaultNotificationsDetailsTypeDef = TypedDict(
     "AwsBackupBackupVaultNotificationsDetailsTypeDef",
     {
         "BackupVaultEvents": Sequence[str],
         "SnsTopicArn": str,
     },
     total=False,
@@ -1429,23 +1703,41 @@
         "IamCertificateId": str,
         "MinimumProtocolVersion": str,
         "SslSupportMethod": str,
     },
     total=False,
 )
 
+AwsCloudFrontDistributionOriginSslProtocolsOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginSslProtocolsOutputTypeDef",
+    {
+        "Items": List[str],
+        "Quantity": int,
+    },
+    total=False,
+)
+
 AwsCloudFrontDistributionOriginSslProtocolsTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginSslProtocolsTypeDef",
     {
         "Items": Sequence[str],
         "Quantity": int,
     },
     total=False,
 )
 
+AwsCloudFrontDistributionOriginGroupFailoverStatusCodesOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesOutputTypeDef",
+    {
+        "Items": List[int],
+        "Quantity": int,
+    },
+    total=False,
+)
+
 AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef",
     {
         "Items": Sequence[int],
         "Quantity": int,
     },
     total=False,
@@ -1513,14 +1805,24 @@
         "Location": str,
         "GitCloneDepth": int,
         "InsecureSsl": bool,
     },
     total=False,
 )
 
+AwsCodeBuildProjectVpcConfigOutputTypeDef = TypedDict(
+    "AwsCodeBuildProjectVpcConfigOutputTypeDef",
+    {
+        "VpcId": str,
+        "Subnets": List[str],
+        "SecurityGroupIds": List[str],
+    },
+    total=False,
+)
+
 AwsCodeBuildProjectVpcConfigTypeDef = TypedDict(
     "AwsCodeBuildProjectVpcConfigTypeDef",
     {
         "VpcId": str,
         "Subnets": Sequence[str],
         "SecurityGroupIds": Sequence[str],
     },
@@ -1632,14 +1934,23 @@
     {
         "StreamEnabled": bool,
         "StreamViewType": str,
     },
     total=False,
 )
 
+AwsDynamoDbTableProjectionOutputTypeDef = TypedDict(
+    "AwsDynamoDbTableProjectionOutputTypeDef",
+    {
+        "NonKeyAttributes": List[str],
+        "ProjectionType": str,
+    },
+    total=False,
+)
+
 AwsDynamoDbTableProjectionTypeDef = TypedDict(
     "AwsDynamoDbTableProjectionTypeDef",
     {
         "NonKeyAttributes": Sequence[str],
         "ProjectionType": str,
     },
     total=False,
@@ -2101,14 +2412,33 @@
         "AssociationId": str,
         "Ipv6CidrBlock": str,
         "CidrBlockState": str,
     },
     total=False,
 )
 
+AwsEc2TransitGatewayDetailsOutputTypeDef = TypedDict(
+    "AwsEc2TransitGatewayDetailsOutputTypeDef",
+    {
+        "Id": str,
+        "Description": str,
+        "DefaultRouteTablePropagation": str,
+        "AutoAcceptSharedAttachments": str,
+        "DefaultRouteTableAssociation": str,
+        "TransitGatewayCidrBlocks": List[str],
+        "AssociationDefaultRouteTableId": str,
+        "PropagationDefaultRouteTableId": str,
+        "VpnEcmpSupport": str,
+        "DnsSupport": str,
+        "MulticastSupport": str,
+        "AmazonSideAsn": int,
+    },
+    total=False,
+)
+
 AwsEc2TransitGatewayDetailsTypeDef = TypedDict(
     "AwsEc2TransitGatewayDetailsTypeDef",
     {
         "Id": str,
         "Description": str,
         "DefaultRouteTablePropagation": str,
         "AutoAcceptSharedAttachments": str,
@@ -2206,14 +2536,37 @@
         "OutsideIpAddress": str,
         "Status": str,
         "StatusMessage": str,
     },
     total=False,
 )
 
+AwsEc2VpnConnectionOptionsTunnelOptionsDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VpnConnectionOptionsTunnelOptionsDetailsOutputTypeDef",
+    {
+        "DpdTimeoutSeconds": int,
+        "IkeVersions": List[str],
+        "OutsideIpAddress": str,
+        "Phase1DhGroupNumbers": List[int],
+        "Phase1EncryptionAlgorithms": List[str],
+        "Phase1IntegrityAlgorithms": List[str],
+        "Phase1LifetimeSeconds": int,
+        "Phase2DhGroupNumbers": List[int],
+        "Phase2EncryptionAlgorithms": List[str],
+        "Phase2IntegrityAlgorithms": List[str],
+        "Phase2LifetimeSeconds": int,
+        "PreSharedKey": str,
+        "RekeyFuzzPercentage": int,
+        "RekeyMarginTimeSeconds": int,
+        "ReplayWindowSize": int,
+        "TunnelInsideCidr": str,
+    },
+    total=False,
+)
+
 AwsEc2VpnConnectionOptionsTunnelOptionsDetailsTypeDef = TypedDict(
     "AwsEc2VpnConnectionOptionsTunnelOptionsDetailsTypeDef",
     {
         "DpdTimeoutSeconds": int,
         "IkeVersions": Sequence[str],
         "OutsideIpAddress": str,
         "Phase1DhGroupNumbers": Sequence[int],
@@ -2229,14 +2582,27 @@
         "RekeyMarginTimeSeconds": int,
         "ReplayWindowSize": int,
         "TunnelInsideCidr": str,
     },
     total=False,
 )
 
+AwsEcrContainerImageDetailsOutputTypeDef = TypedDict(
+    "AwsEcrContainerImageDetailsOutputTypeDef",
+    {
+        "RegistryId": str,
+        "RepositoryName": str,
+        "Architecture": str,
+        "ImageDigest": str,
+        "ImageTags": List[str],
+        "ImagePublishedAt": str,
+    },
+    total=False,
+)
+
 AwsEcrContainerImageDetailsTypeDef = TypedDict(
     "AwsEcrContainerImageDetailsTypeDef",
     {
         "RegistryId": str,
         "RepositoryName": str,
         "Architecture": str,
         "ImageDigest": str,
@@ -2366,14 +2732,24 @@
         "ContainerPort": int,
         "Port": int,
         "RegistryArn": str,
     },
     total=False,
 )
 
+AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsOutputTypeDef",
+    {
+        "AssignPublicIp": str,
+        "SecurityGroups": List[str],
+        "Subnets": List[str],
+    },
+    total=False,
+)
+
 AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef",
     {
         "AssignPublicIp": str,
         "SecurityGroups": Sequence[str],
         "Subnets": Sequence[str],
     },
@@ -2412,27 +2788,27 @@
     {
         "Hostname": str,
         "IpAddress": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef",
     {
-        "Options": Mapping[str, str],
+        "Options": Dict[str, str],
         "Type": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef",
     {
-        "Command": Sequence[str],
+        "Command": List[str],
         "Interval": int,
         "Retries": int,
         "StartPeriod": int,
         "Timeout": int,
     },
     total=False,
 )
@@ -2507,23 +2883,73 @@
     {
         "ReadOnly": bool,
         "SourceContainer": str,
     },
     total=False,
 )
 
+AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef",
+    {
+        "Options": Mapping[str, str],
+        "Type": str,
+    },
+    total=False,
+)
+
+AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef",
+    {
+        "Command": Sequence[str],
+        "Interval": int,
+        "Retries": int,
+        "StartPeriod": int,
+        "Timeout": int,
+    },
+    total=False,
+)
+
+AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef",
+    {
+        "Add": List[str],
+        "Drop": List[str],
+    },
+    total=False,
+)
+
 AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef",
     {
         "Add": Sequence[str],
         "Drop": Sequence[str],
     },
     total=False,
 )
 
+AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsOutputTypeDef",
+    {
+        "ContainerPath": str,
+        "HostPath": str,
+        "Permissions": List[str],
+    },
+    total=False,
+)
+
+AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsOutputTypeDef",
+    {
+        "ContainerPath": str,
+        "MountOptions": List[str],
+        "Size": int,
+    },
+    total=False,
+)
+
 AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsTypeDef",
     {
         "ContainerPath": str,
         "HostPath": str,
         "Permissions": Sequence[str],
     },
@@ -2572,34 +2998,46 @@
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef",
+AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsOutputTypeDef",
     {
         "Autoprovision": bool,
         "Driver": str,
-        "DriverOpts": Mapping[str, str],
-        "Labels": Mapping[str, str],
+        "DriverOpts": Dict[str, str],
+        "Labels": Dict[str, str],
         "Scope": str,
     },
     total=False,
 )
 
 AwsEcsTaskDefinitionVolumesHostDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesHostDetailsTypeDef",
     {
         "SourcePath": str,
     },
     total=False,
 )
 
+AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef",
+    {
+        "Autoprovision": bool,
+        "Driver": str,
+        "DriverOpts": Mapping[str, str],
+        "Labels": Mapping[str, str],
+        "Scope": str,
+    },
+    total=False,
+)
+
 AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef",
     {
         "AccessPointId": str,
         "Iam": str,
     },
     total=False,
@@ -2609,14 +3047,24 @@
     "AwsEcsTaskVolumeHostDetailsTypeDef",
     {
         "SourcePath": str,
     },
     total=False,
 )
 
+AwsEfsAccessPointPosixUserDetailsOutputTypeDef = TypedDict(
+    "AwsEfsAccessPointPosixUserDetailsOutputTypeDef",
+    {
+        "Gid": str,
+        "SecondaryGids": List[str],
+        "Uid": str,
+    },
+    total=False,
+)
+
 AwsEfsAccessPointPosixUserDetailsTypeDef = TypedDict(
     "AwsEfsAccessPointPosixUserDetailsTypeDef",
     {
         "Gid": str,
         "SecondaryGids": Sequence[str],
         "Uid": str,
     },
@@ -2629,24 +3077,43 @@
         "OwnerGid": str,
         "OwnerUid": str,
         "Permissions": str,
     },
     total=False,
 )
 
+AwsEksClusterResourcesVpcConfigDetailsOutputTypeDef = TypedDict(
+    "AwsEksClusterResourcesVpcConfigDetailsOutputTypeDef",
+    {
+        "SecurityGroupIds": List[str],
+        "SubnetIds": List[str],
+        "EndpointPublicAccess": bool,
+    },
+    total=False,
+)
+
 AwsEksClusterResourcesVpcConfigDetailsTypeDef = TypedDict(
     "AwsEksClusterResourcesVpcConfigDetailsTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "SubnetIds": Sequence[str],
         "EndpointPublicAccess": bool,
     },
     total=False,
 )
 
+AwsEksClusterLoggingClusterLoggingDetailsOutputTypeDef = TypedDict(
+    "AwsEksClusterLoggingClusterLoggingDetailsOutputTypeDef",
+    {
+        "Enabled": bool,
+        "Types": List[str],
+    },
+    total=False,
+)
+
 AwsEksClusterLoggingClusterLoggingDetailsTypeDef = TypedDict(
     "AwsEksClusterLoggingClusterLoggingDetailsTypeDef",
     {
         "Enabled": bool,
         "Types": Sequence[str],
     },
     total=False,
@@ -2718,14 +3185,25 @@
         "NewVersion": str,
         "UpdateAvailable": bool,
         "UpdateStatus": str,
     },
     total=False,
 )
 
+AwsElasticsearchDomainVPCOptionsOutputTypeDef = TypedDict(
+    "AwsElasticsearchDomainVPCOptionsOutputTypeDef",
+    {
+        "AvailabilityZones": List[str],
+        "SecurityGroupIds": List[str],
+        "SubnetIds": List[str],
+        "VPCId": str,
+    },
+    total=False,
+)
+
 AwsElasticsearchDomainVPCOptionsTypeDef = TypedDict(
     "AwsElasticsearchDomainVPCOptionsTypeDef",
     {
         "AvailabilityZones": Sequence[str],
         "SecurityGroupIds": Sequence[str],
         "SubnetIds": Sequence[str],
         "VPCId": str,
@@ -2809,14 +3287,23 @@
     "AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
+AwsElbLoadBalancerBackendServerDescriptionOutputTypeDef = TypedDict(
+    "AwsElbLoadBalancerBackendServerDescriptionOutputTypeDef",
+    {
+        "InstancePort": int,
+        "PolicyNames": List[str],
+    },
+    total=False,
+)
+
 AwsElbLoadBalancerBackendServerDescriptionTypeDef = TypedDict(
     "AwsElbLoadBalancerBackendServerDescriptionTypeDef",
     {
         "InstancePort": int,
         "PolicyNames": Sequence[str],
     },
     total=False,
@@ -3091,14 +3578,24 @@
     "AwsLambdaFunctionTracingConfigTypeDef",
     {
         "Mode": str,
     },
     total=False,
 )
 
+AwsLambdaFunctionVpcConfigOutputTypeDef = TypedDict(
+    "AwsLambdaFunctionVpcConfigOutputTypeDef",
+    {
+        "SecurityGroupIds": List[str],
+        "SubnetIds": List[str],
+        "VpcId": str,
+    },
+    total=False,
+)
+
 AwsLambdaFunctionVpcConfigTypeDef = TypedDict(
     "AwsLambdaFunctionVpcConfigTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "SubnetIds": Sequence[str],
         "VpcId": str,
     },
@@ -3110,14 +3607,24 @@
     {
         "ErrorCode": str,
         "Message": str,
     },
     total=False,
 )
 
+AwsLambdaLayerVersionDetailsOutputTypeDef = TypedDict(
+    "AwsLambdaLayerVersionDetailsOutputTypeDef",
+    {
+        "Version": int,
+        "CompatibleRuntimes": List[str],
+        "CreatedDate": str,
+    },
+    total=False,
+)
+
 AwsLambdaLayerVersionDetailsTypeDef = TypedDict(
     "AwsLambdaLayerVersionDetailsTypeDef",
     {
         "Version": int,
         "CompatibleRuntimes": Sequence[str],
         "CreatedDate": str,
     },
@@ -3190,14 +3697,23 @@
         "UpdateAvailable": bool,
         "UpdateStatus": str,
         "OptionalDeployment": bool,
     },
     total=False,
 )
 
+AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef = TypedDict(
+    "AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef",
+    {
+        "SecurityGroupIds": List[str],
+        "SubnetIds": List[str],
+    },
+    total=False,
+)
+
 AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "SubnetIds": Sequence[str],
     },
     total=False,
@@ -3257,14 +3773,39 @@
     {
         "VpcSecurityGroupId": str,
         "Status": str,
     },
     total=False,
 )
 
+AwsRdsDbClusterSnapshotDetailsOutputTypeDef = TypedDict(
+    "AwsRdsDbClusterSnapshotDetailsOutputTypeDef",
+    {
+        "AvailabilityZones": List[str],
+        "SnapshotCreateTime": str,
+        "Engine": str,
+        "AllocatedStorage": int,
+        "Status": str,
+        "Port": int,
+        "VpcId": str,
+        "ClusterCreateTime": str,
+        "MasterUsername": str,
+        "EngineVersion": str,
+        "LicenseModel": str,
+        "SnapshotType": str,
+        "PercentProgress": int,
+        "StorageEncrypted": bool,
+        "KmsKeyId": str,
+        "DbClusterIdentifier": str,
+        "DbClusterSnapshotIdentifier": str,
+        "IamDatabaseAuthenticationEnabled": bool,
+    },
+    total=False,
+)
+
 AwsRdsDbClusterSnapshotDetailsTypeDef = TypedDict(
     "AwsRdsDbClusterSnapshotDetailsTypeDef",
     {
         "AvailabilityZones": Sequence[str],
         "SnapshotCreateTime": str,
         "Engine": str,
         "AllocatedStorage": int,
@@ -3340,14 +3881,23 @@
         "Normal": bool,
         "Status": str,
         "Message": str,
     },
     total=False,
 )
 
+AwsRdsPendingCloudWatchLogsExportsOutputTypeDef = TypedDict(
+    "AwsRdsPendingCloudWatchLogsExportsOutputTypeDef",
+    {
+        "LogTypesToEnable": List[str],
+        "LogTypesToDisable": List[str],
+    },
+    total=False,
+)
+
 AwsRdsPendingCloudWatchLogsExportsTypeDef = TypedDict(
     "AwsRdsPendingCloudWatchLogsExportsTypeDef",
     {
         "LogTypesToEnable": Sequence[str],
         "LogTypesToDisable": Sequence[str],
     },
     total=False,
@@ -3377,14 +3927,31 @@
     "AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+AwsRdsEventSubscriptionDetailsOutputTypeDef = TypedDict(
+    "AwsRdsEventSubscriptionDetailsOutputTypeDef",
+    {
+        "CustSubscriptionId": str,
+        "CustomerAwsId": str,
+        "Enabled": bool,
+        "EventCategoriesList": List[str],
+        "EventSubscriptionArn": str,
+        "SnsTopicArn": str,
+        "SourceIdsList": List[str],
+        "SourceType": str,
+        "Status": str,
+        "SubscriptionCreationTime": str,
+    },
+    total=False,
+)
+
 AwsRdsEventSubscriptionDetailsTypeDef = TypedDict(
     "AwsRdsEventSubscriptionDetailsTypeDef",
     {
         "CustSubscriptionId": str,
         "CustomerAwsId": str,
         "Enabled": bool,
         "EventCategoriesList": Sequence[str],
@@ -4042,14 +4609,25 @@
 BatchDeleteAutomationRulesRequestRequestTypeDef = TypedDict(
     "BatchDeleteAutomationRulesRequestRequestTypeDef",
     {
         "AutomationRulesArns": Sequence[str],
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
 UnprocessedAutomationRuleTypeDef = TypedDict(
     "UnprocessedAutomationRuleTypeDef",
     {
         "RuleArn": str,
         "ErrorCode": int,
         "ErrorMessage": str,
     },
@@ -4257,30 +4835,14 @@
     {
         "Name": str,
         "Description": str,
         "Id": str,
     },
 )
 
-CreateActionTargetResponseTypeDef = TypedDict(
-    "CreateActionTargetResponseTypeDef",
-    {
-        "ActionTargetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateAutomationRuleResponseTypeDef = TypedDict(
-    "CreateAutomationRuleResponseTypeDef",
-    {
-        "RuleArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateFindingAggregatorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFindingAggregatorRequestRequestTypeDef",
     {
         "RegionLinkingMode": str,
     },
 )
 _OptionalCreateFindingAggregatorRequestRequestTypeDef = TypedDict(
@@ -4295,33 +4857,14 @@
 class CreateFindingAggregatorRequestRequestTypeDef(
     _RequiredCreateFindingAggregatorRequestRequestTypeDef,
     _OptionalCreateFindingAggregatorRequestRequestTypeDef,
 ):
     pass
 
 
-CreateFindingAggregatorResponseTypeDef = TypedDict(
-    "CreateFindingAggregatorResponseTypeDef",
-    {
-        "FindingAggregatorArn": str,
-        "FindingAggregationRegion": str,
-        "RegionLinkingMode": str,
-        "Regions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateInsightResponseTypeDef = TypedDict(
-    "CreateInsightResponseTypeDef",
-    {
-        "InsightArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResultTypeDef = TypedDict(
     "ResultTypeDef",
     {
         "AccountId": str,
         "ProcessingResult": str,
     },
     total=False,
@@ -4346,63 +4889,48 @@
 DeleteActionTargetRequestRequestTypeDef = TypedDict(
     "DeleteActionTargetRequestRequestTypeDef",
     {
         "ActionTargetArn": str,
     },
 )
 
-DeleteActionTargetResponseTypeDef = TypedDict(
-    "DeleteActionTargetResponseTypeDef",
-    {
-        "ActionTargetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteFindingAggregatorRequestRequestTypeDef = TypedDict(
     "DeleteFindingAggregatorRequestRequestTypeDef",
     {
         "FindingAggregatorArn": str,
     },
 )
 
 DeleteInsightRequestRequestTypeDef = TypedDict(
     "DeleteInsightRequestRequestTypeDef",
     {
         "InsightArn": str,
     },
 )
 
-DeleteInsightResponseTypeDef = TypedDict(
-    "DeleteInsightResponseTypeDef",
-    {
-        "InsightArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteInvitationsRequestRequestTypeDef = TypedDict(
     "DeleteInvitationsRequestRequestTypeDef",
     {
         "AccountIds": Sequence[str],
     },
 )
 
 DeleteMembersRequestRequestTypeDef = TypedDict(
     "DeleteMembersRequestRequestTypeDef",
     {
         "AccountIds": Sequence[str],
     },
 )
 
-DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef = TypedDict(
-    "DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ActionTargetArns": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeActionTargetsRequestRequestTypeDef = TypedDict(
     "DescribeActionTargetsRequestRequestTypeDef",
     {
@@ -4417,44 +4945,14 @@
     "DescribeHubRequestRequestTypeDef",
     {
         "HubArn": str,
     },
     total=False,
 )
 
-DescribeHubResponseTypeDef = TypedDict(
-    "DescribeHubResponseTypeDef",
-    {
-        "HubArn": str,
-        "SubscribedAt": str,
-        "AutoEnableControls": bool,
-        "ControlFindingGenerator": ControlFindingGeneratorType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
-    "DescribeOrganizationConfigurationResponseTypeDef",
-    {
-        "AutoEnable": bool,
-        "MemberAccountLimitReached": bool,
-        "AutoEnableStandards": AutoEnableStandardsType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeProductsRequestDescribeProductsPaginateTypeDef = TypedDict(
-    "DescribeProductsRequestDescribeProductsPaginateTypeDef",
-    {
-        "ProductArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeProductsRequestRequestTypeDef = TypedDict(
     "DescribeProductsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ProductArn": str,
     },
@@ -4483,36 +4981,14 @@
 )
 
 
 class ProductTypeDef(_RequiredProductTypeDef, _OptionalProductTypeDef):
     pass
 
 
-_RequiredDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef",
-    {
-        "StandardsSubscriptionArn": str,
-    },
-)
-_OptionalDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef(
-    _RequiredDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
-    _OptionalDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeStandardsControlsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeStandardsControlsRequestRequestTypeDef",
     {
         "StandardsSubscriptionArn": str,
     },
 )
 _OptionalDescribeStandardsControlsRequestRequestTypeDef = TypedDict(
@@ -4545,22 +5021,14 @@
         "RemediationUrl": str,
         "SeverityRating": SeverityRatingType,
         "RelatedRequirements": List[str],
     },
     total=False,
 )
 
-DescribeStandardsRequestDescribeStandardsPaginateTypeDef = TypedDict(
-    "DescribeStandardsRequestDescribeStandardsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeStandardsRequestRequestTypeDef = TypedDict(
     "DescribeStandardsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -4590,22 +5058,14 @@
 EnableImportFindingsForProductRequestRequestTypeDef = TypedDict(
     "EnableImportFindingsForProductRequestRequestTypeDef",
     {
         "ProductArn": str,
     },
 )
 
-EnableImportFindingsForProductResponseTypeDef = TypedDict(
-    "EnableImportFindingsForProductResponseTypeDef",
-    {
-        "ProductSubscriptionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnableOrganizationAdminAccountRequestRequestTypeDef = TypedDict(
     "EnableOrganizationAdminAccountRequestRequestTypeDef",
     {
         "AdminAccountId": str,
     },
 )
 
@@ -4690,23 +5150,14 @@
         "InvitationId": str,
         "InvitedAt": datetime,
         "MemberStatus": str,
     },
     total=False,
 )
 
-GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef = TypedDict(
-    "GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef",
-    {
-        "StandardsSubscriptionArns": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetEnabledStandardsRequestRequestTypeDef = TypedDict(
     "GetEnabledStandardsRequestRequestTypeDef",
     {
         "StandardsSubscriptionArns": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
@@ -4716,25 +5167,15 @@
 GetFindingAggregatorRequestRequestTypeDef = TypedDict(
     "GetFindingAggregatorRequestRequestTypeDef",
     {
         "FindingAggregatorArn": str,
     },
 )
 
-GetFindingAggregatorResponseTypeDef = TypedDict(
-    "GetFindingAggregatorResponseTypeDef",
-    {
-        "FindingAggregatorArn": str,
-        "FindingAggregationRegion": str,
-        "RegionLinkingMode": str,
-        "Regions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 SortCriterionTypeDef = TypedDict(
     "SortCriterionTypeDef",
     {
         "Field": str,
         "SortOrder": SortOrderType,
     },
     total=False,
@@ -4743,41 +5184,24 @@
 GetInsightResultsRequestRequestTypeDef = TypedDict(
     "GetInsightResultsRequestRequestTypeDef",
     {
         "InsightArn": str,
     },
 )
 
-GetInsightsRequestGetInsightsPaginateTypeDef = TypedDict(
-    "GetInsightsRequestGetInsightsPaginateTypeDef",
-    {
-        "InsightArns": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetInsightsRequestRequestTypeDef = TypedDict(
     "GetInsightsRequestRequestTypeDef",
     {
         "InsightArns": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-GetInvitationsCountResponseTypeDef = TypedDict(
-    "GetInvitationsCountResponseTypeDef",
-    {
-        "InvitationsCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetMembersRequestRequestTypeDef = TypedDict(
     "GetMembersRequestRequestTypeDef",
     {
         "AccountIds": Sequence[str],
     },
 )
 
@@ -4815,119 +5239,60 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef = TypedDict(
-    "ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListEnabledProductsForImportRequestRequestTypeDef = TypedDict(
     "ListEnabledProductsForImportRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListEnabledProductsForImportResponseTypeDef = TypedDict(
-    "ListEnabledProductsForImportResponseTypeDef",
-    {
-        "ProductSubscriptions": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef = TypedDict(
-    "ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFindingAggregatorsRequestRequestTypeDef = TypedDict(
     "ListFindingAggregatorsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListInvitationsRequestListInvitationsPaginateTypeDef = TypedDict(
-    "ListInvitationsRequestListInvitationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListInvitationsRequestRequestTypeDef = TypedDict(
     "ListInvitationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListMembersRequestListMembersPaginateTypeDef = TypedDict(
-    "ListMembersRequestListMembersPaginateTypeDef",
-    {
-        "OnlyAssociated": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMembersRequestRequestTypeDef = TypedDict(
     "ListMembersRequestRequestTypeDef",
     {
         "OnlyAssociated": bool,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef = TypedDict(
-    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOrganizationAdminAccountsRequestRequestTypeDef = TypedDict(
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef = TypedDict(
-    "ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef",
-    {
-        "StandardsArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSecurityControlDefinitionsRequestRequestTypeDef = TypedDict(
     "ListSecurityControlDefinitionsRequestRequestTypeDef",
     {
         "StandardsArn": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -4942,36 +5307,14 @@
         "Description": str,
         "RemediationUrl": str,
         "SeverityRating": SeverityRatingType,
         "CurrentRegionAvailability": RegionAvailabilityStatusType,
     },
 )
 
-_RequiredListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef",
-    {
-        "SecurityControlId": str,
-    },
-)
-_OptionalListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef(
-    _RequiredListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef,
-    _OptionalListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListStandardsControlAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredListStandardsControlAssociationsRequestRequestTypeDef",
     {
         "SecurityControlId": str,
     },
 )
 _OptionalListStandardsControlAssociationsRequestRequestTypeDef = TypedDict(
@@ -5023,22 +5366,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PortRangeTypeDef = TypedDict(
     "PortRangeTypeDef",
     {
         "Begin": int,
         "End": int,
     },
     total=False,
@@ -5059,42 +5394,31 @@
     {
         "JsonPath": str,
         "RecordIndex": int,
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
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "Text": str,
         "Url": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+RuleGroupSourceListDetailsOutputTypeDef = TypedDict(
+    "RuleGroupSourceListDetailsOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "GeneratedRulesType": str,
+        "TargetTypes": List[str],
+        "Targets": List[str],
     },
+    total=False,
 )
 
 RuleGroupSourceListDetailsTypeDef = TypedDict(
     "RuleGroupSourceListDetailsTypeDef",
     {
         "GeneratedRulesType": str,
         "TargetTypes": Sequence[str],
@@ -5112,14 +5436,23 @@
         "Protocol": str,
         "Source": str,
         "SourcePort": str,
     },
     total=False,
 )
 
+RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef",
+    {
+        "Keyword": str,
+        "Settings": List[str],
+    },
+    total=False,
+)
+
 RuleGroupSourceStatefulRulesOptionsDetailsTypeDef = TypedDict(
     "RuleGroupSourceStatefulRulesOptionsDetailsTypeDef",
     {
         "Keyword": str,
         "Settings": Sequence[str],
     },
     total=False,
@@ -5155,31 +5488,56 @@
     "RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef",
     {
         "AddressDefinition": str,
     },
     total=False,
 )
 
+RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef",
+    {
+        "Flags": List[str],
+        "Masks": List[str],
+    },
+    total=False,
+)
+
 RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef",
     {
         "Flags": Sequence[str],
         "Masks": Sequence[str],
     },
     total=False,
 )
 
+RuleGroupVariablesIpSetsDetailsOutputTypeDef = TypedDict(
+    "RuleGroupVariablesIpSetsDetailsOutputTypeDef",
+    {
+        "Definition": List[str],
+    },
+    total=False,
+)
+
 RuleGroupVariablesIpSetsDetailsTypeDef = TypedDict(
     "RuleGroupVariablesIpSetsDetailsTypeDef",
     {
         "Definition": Sequence[str],
     },
     total=False,
 )
 
+RuleGroupVariablesPortSetsDetailsOutputTypeDef = TypedDict(
+    "RuleGroupVariablesPortSetsDetailsOutputTypeDef",
+    {
+        "Definition": List[str],
+    },
+    total=False,
+)
+
 RuleGroupVariablesPortSetsDetailsTypeDef = TypedDict(
     "RuleGroupVariablesPortSetsDetailsTypeDef",
     {
         "Definition": Sequence[str],
     },
     total=False,
 )
@@ -5284,25 +5642,14 @@
 class UpdateFindingAggregatorRequestRequestTypeDef(
     _RequiredUpdateFindingAggregatorRequestRequestTypeDef,
     _OptionalUpdateFindingAggregatorRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateFindingAggregatorResponseTypeDef = TypedDict(
-    "UpdateFindingAggregatorResponseTypeDef",
-    {
-        "FindingAggregatorArn": str,
-        "FindingAggregationRegion": str,
-        "RegionLinkingMode": str,
-        "Regions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateOrganizationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOrganizationConfigurationRequestRequestTypeDef",
     {
         "AutoEnable": bool,
     },
 )
 _OptionalUpdateOrganizationConfigurationRequestRequestTypeDef = TypedDict(
@@ -5392,94 +5739,111 @@
         "Country": CountryTypeDef,
         "City": CityTypeDef,
         "GeoLocation": GeoLocationTypeDef,
     },
     total=False,
 )
 
-DescribeActionTargetsResponseTypeDef = TypedDict(
-    "DescribeActionTargetsResponseTypeDef",
+CvssOutputTypeDef = TypedDict(
+    "CvssOutputTypeDef",
     {
-        "ActionTargets": List[ActionTargetTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Version": str,
+        "BaseScore": float,
+        "BaseVector": str,
+        "Source": str,
+        "Adjustments": List[AdjustmentTypeDef],
     },
+    total=False,
 )
 
 CvssTypeDef = TypedDict(
     "CvssTypeDef",
     {
         "Version": str,
         "BaseScore": float,
         "BaseVector": str,
         "Source": str,
         "Adjustments": Sequence[AdjustmentTypeDef],
     },
     total=False,
 )
 
-ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
-    "ListOrganizationAdminAccountsResponseTypeDef",
-    {
-        "AdminAccounts": List[AdminAccountTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssociationSetDetailsTypeDef = TypedDict(
     "AssociationSetDetailsTypeDef",
     {
         "AssociationState": AssociationStateDetailsTypeDef,
         "GatewayId": str,
         "Main": bool,
         "RouteTableAssociationId": str,
         "RouteTableId": str,
         "SubnetId": str,
     },
     total=False,
 )
 
-AutomationRulesFindingFieldsUpdateTypeDef = TypedDict(
-    "AutomationRulesFindingFieldsUpdateTypeDef",
+AutomationRulesFindingFieldsUpdateOutputTypeDef = TypedDict(
+    "AutomationRulesFindingFieldsUpdateOutputTypeDef",
     {
         "Note": NoteUpdateTypeDef,
         "Severity": SeverityUpdateTypeDef,
         "VerificationState": VerificationStateType,
         "Confidence": int,
         "Criticality": int,
         "Types": List[str],
         "UserDefinedFields": Dict[str, str],
         "Workflow": WorkflowUpdateTypeDef,
         "RelatedFindings": List[RelatedFindingTypeDef],
     },
     total=False,
 )
 
-ListAutomationRulesResponseTypeDef = TypedDict(
-    "ListAutomationRulesResponseTypeDef",
+AutomationRulesFindingFieldsUpdateTypeDef = TypedDict(
+    "AutomationRulesFindingFieldsUpdateTypeDef",
     {
-        "AutomationRulesMetadata": List[AutomationRulesMetadataTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Note": NoteUpdateTypeDef,
+        "Severity": SeverityUpdateTypeDef,
+        "VerificationState": VerificationStateType,
+        "Confidence": int,
+        "Criticality": int,
+        "Types": Sequence[str],
+        "UserDefinedFields": Mapping[str, str],
+        "Workflow": WorkflowUpdateTypeDef,
+        "RelatedFindings": Sequence[RelatedFindingTypeDef],
     },
+    total=False,
 )
 
 AwsAmazonMqBrokerLogsDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerLogsDetailsTypeDef",
     {
         "Audit": bool,
         "General": bool,
         "AuditLogGroup": str,
         "GeneralLogGroup": str,
         "Pending": AwsAmazonMqBrokerLogsPendingDetailsTypeDef,
     },
     total=False,
 )
 
+AwsApiGatewayRestApiDetailsOutputTypeDef = TypedDict(
+    "AwsApiGatewayRestApiDetailsOutputTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "CreatedDate": str,
+        "Version": str,
+        "BinaryMediaTypes": List[str],
+        "MinimumCompressionSize": int,
+        "ApiKeySource": str,
+        "EndpointConfiguration": AwsApiGatewayEndpointConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 AwsApiGatewayRestApiDetailsTypeDef = TypedDict(
     "AwsApiGatewayRestApiDetailsTypeDef",
     {
         "Id": str,
         "Name": str,
         "Description": str,
         "CreatedDate": str,
@@ -5488,14 +5852,37 @@
         "MinimumCompressionSize": int,
         "ApiKeySource": str,
         "EndpointConfiguration": AwsApiGatewayEndpointConfigurationTypeDef,
     },
     total=False,
 )
 
+AwsApiGatewayStageDetailsOutputTypeDef = TypedDict(
+    "AwsApiGatewayStageDetailsOutputTypeDef",
+    {
+        "DeploymentId": str,
+        "ClientCertificateId": str,
+        "StageName": str,
+        "Description": str,
+        "CacheClusterEnabled": bool,
+        "CacheClusterSize": str,
+        "CacheClusterStatus": str,
+        "MethodSettings": List[AwsApiGatewayMethodSettingsTypeDef],
+        "Variables": Dict[str, str],
+        "DocumentationVersion": str,
+        "AccessLogSettings": AwsApiGatewayAccessLogSettingsTypeDef,
+        "CanarySettings": AwsApiGatewayCanarySettingsOutputTypeDef,
+        "TracingEnabled": bool,
+        "CreatedDate": str,
+        "LastUpdatedDate": str,
+        "WebAclArn": str,
+    },
+    total=False,
+)
+
 AwsApiGatewayStageDetailsTypeDef = TypedDict(
     "AwsApiGatewayStageDetailsTypeDef",
     {
         "DeploymentId": str,
         "ClientCertificateId": str,
         "StageName": str,
         "Description": str,
@@ -5511,14 +5898,31 @@
         "CreatedDate": str,
         "LastUpdatedDate": str,
         "WebAclArn": str,
     },
     total=False,
 )
 
+AwsApiGatewayV2ApiDetailsOutputTypeDef = TypedDict(
+    "AwsApiGatewayV2ApiDetailsOutputTypeDef",
+    {
+        "ApiEndpoint": str,
+        "ApiId": str,
+        "ApiKeySelectionExpression": str,
+        "CreatedDate": str,
+        "Description": str,
+        "Version": str,
+        "Name": str,
+        "ProtocolType": str,
+        "RouteSelectionExpression": str,
+        "CorsConfiguration": AwsCorsConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 AwsApiGatewayV2ApiDetailsTypeDef = TypedDict(
     "AwsApiGatewayV2ApiDetailsTypeDef",
     {
         "ApiEndpoint": str,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
         "CreatedDate": str,
@@ -5528,14 +5932,34 @@
         "ProtocolType": str,
         "RouteSelectionExpression": str,
         "CorsConfiguration": AwsCorsConfigurationTypeDef,
     },
     total=False,
 )
 
+AwsApiGatewayV2StageDetailsOutputTypeDef = TypedDict(
+    "AwsApiGatewayV2StageDetailsOutputTypeDef",
+    {
+        "ClientCertificateId": str,
+        "CreatedDate": str,
+        "Description": str,
+        "DefaultRouteSettings": AwsApiGatewayV2RouteSettingsTypeDef,
+        "DeploymentId": str,
+        "LastUpdatedDate": str,
+        "RouteSettings": AwsApiGatewayV2RouteSettingsTypeDef,
+        "StageName": str,
+        "StageVariables": Dict[str, str],
+        "AccessLogSettings": AwsApiGatewayAccessLogSettingsTypeDef,
+        "AutoDeploy": bool,
+        "LastDeploymentStatusMessage": str,
+        "ApiGatewayManaged": bool,
+    },
+    total=False,
+)
+
 AwsApiGatewayV2StageDetailsTypeDef = TypedDict(
     "AwsApiGatewayV2StageDetailsTypeDef",
     {
         "ClientCertificateId": str,
         "CreatedDate": str,
         "Description": str,
         "DefaultRouteSettings": AwsApiGatewayV2RouteSettingsTypeDef,
@@ -5559,14 +5983,25 @@
         "LambdaAuthorizerConfig": AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef,
         "OpenIdConnectConfig": AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef,
         "UserPoolConfig": AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef,
     },
     total=False,
 )
 
+AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef = TypedDict(
+    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef",
+    {
+        "LaunchTemplateSpecification": AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef,
+        "Overrides": List[
+            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef
+        ],
+    },
+    total=False,
+)
+
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef",
     {
         "LaunchTemplateSpecification": AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef,
         "Overrides": Sequence[
             AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef
         ],
@@ -5590,14 +6025,26 @@
     {
         "DestinationBackupVaultArn": str,
         "Lifecycle": AwsBackupBackupPlanLifecycleDetailsTypeDef,
     },
     total=False,
 )
 
+AwsBackupBackupVaultDetailsOutputTypeDef = TypedDict(
+    "AwsBackupBackupVaultDetailsOutputTypeDef",
+    {
+        "BackupVaultArn": str,
+        "BackupVaultName": str,
+        "EncryptionKeyArn": str,
+        "Notifications": AwsBackupBackupVaultNotificationsDetailsOutputTypeDef,
+        "AccessPolicy": str,
+    },
+    total=False,
+)
+
 AwsBackupBackupVaultDetailsTypeDef = TypedDict(
     "AwsBackupBackupVaultDetailsTypeDef",
     {
         "BackupVaultArn": str,
         "BackupVaultName": str,
         "EncryptionKeyArn": str,
         "Notifications": AwsBackupBackupVaultNotificationsDetailsTypeDef,
@@ -5628,27 +6075,62 @@
         "Status": str,
         "StatusMessage": str,
         "StorageClass": str,
     },
     total=False,
 )
 
+AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef = TypedDict(
+    "AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef",
+    {
+        "DomainName": str,
+        "ResourceRecord": AwsCertificateManagerCertificateResourceRecordTypeDef,
+        "ValidationDomain": str,
+        "ValidationEmails": List[str],
+        "ValidationMethod": str,
+        "ValidationStatus": str,
+    },
+    total=False,
+)
+
 AwsCertificateManagerCertificateDomainValidationOptionTypeDef = TypedDict(
     "AwsCertificateManagerCertificateDomainValidationOptionTypeDef",
     {
         "DomainName": str,
         "ResourceRecord": AwsCertificateManagerCertificateResourceRecordTypeDef,
         "ValidationDomain": str,
         "ValidationEmails": Sequence[str],
         "ValidationMethod": str,
         "ValidationStatus": str,
     },
     total=False,
 )
 
+AwsCloudFormationStackDetailsOutputTypeDef = TypedDict(
+    "AwsCloudFormationStackDetailsOutputTypeDef",
+    {
+        "Capabilities": List[str],
+        "CreationTime": str,
+        "Description": str,
+        "DisableRollback": bool,
+        "DriftInformation": AwsCloudFormationStackDriftInformationDetailsTypeDef,
+        "EnableTerminationProtection": bool,
+        "LastUpdatedTime": str,
+        "NotificationArns": List[str],
+        "Outputs": List[AwsCloudFormationStackOutputsDetailsTypeDef],
+        "RoleArn": str,
+        "StackId": str,
+        "StackName": str,
+        "StackStatus": str,
+        "StackStatusReason": str,
+        "TimeoutInMinutes": int,
+    },
+    total=False,
+)
+
 AwsCloudFormationStackDetailsTypeDef = TypedDict(
     "AwsCloudFormationStackDetailsTypeDef",
     {
         "Capabilities": Sequence[str],
         "CreationTime": str,
         "Description": str,
         "DisableRollback": bool,
@@ -5663,43 +6145,101 @@
         "StackStatus": str,
         "StackStatusReason": str,
         "TimeoutInMinutes": int,
     },
     total=False,
 )
 
+AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef",
+    {
+        "Items": List[AwsCloudFrontDistributionCacheBehaviorTypeDef],
+    },
+    total=False,
+)
+
 AwsCloudFrontDistributionCacheBehaviorsTypeDef = TypedDict(
     "AwsCloudFrontDistributionCacheBehaviorsTypeDef",
     {
         "Items": Sequence[AwsCloudFrontDistributionCacheBehaviorTypeDef],
     },
     total=False,
 )
 
+AwsCloudFrontDistributionOriginCustomOriginConfigOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginCustomOriginConfigOutputTypeDef",
+    {
+        "HttpPort": int,
+        "HttpsPort": int,
+        "OriginKeepaliveTimeout": int,
+        "OriginProtocolPolicy": str,
+        "OriginReadTimeout": int,
+        "OriginSslProtocols": AwsCloudFrontDistributionOriginSslProtocolsOutputTypeDef,
+    },
+    total=False,
+)
+
 AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef",
     {
         "HttpPort": int,
         "HttpsPort": int,
         "OriginKeepaliveTimeout": int,
         "OriginProtocolPolicy": str,
         "OriginReadTimeout": int,
         "OriginSslProtocols": AwsCloudFrontDistributionOriginSslProtocolsTypeDef,
     },
     total=False,
 )
 
+AwsCloudFrontDistributionOriginGroupFailoverOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginGroupFailoverOutputTypeDef",
+    {
+        "StatusCodes": AwsCloudFrontDistributionOriginGroupFailoverStatusCodesOutputTypeDef,
+    },
+    total=False,
+)
+
 AwsCloudFrontDistributionOriginGroupFailoverTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupFailoverTypeDef",
     {
         "StatusCodes": AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef,
     },
     total=False,
 )
 
+AwsCloudWatchAlarmDetailsOutputTypeDef = TypedDict(
+    "AwsCloudWatchAlarmDetailsOutputTypeDef",
+    {
+        "ActionsEnabled": bool,
+        "AlarmActions": List[str],
+        "AlarmArn": str,
+        "AlarmConfigurationUpdatedTimestamp": str,
+        "AlarmDescription": str,
+        "AlarmName": str,
+        "ComparisonOperator": str,
+        "DatapointsToAlarm": int,
+        "Dimensions": List[AwsCloudWatchAlarmDimensionsDetailsTypeDef],
+        "EvaluateLowSampleCountPercentile": str,
+        "EvaluationPeriods": int,
+        "ExtendedStatistic": str,
+        "InsufficientDataActions": List[str],
+        "MetricName": str,
+        "Namespace": str,
+        "OkActions": List[str],
+        "Period": int,
+        "Statistic": str,
+        "Threshold": float,
+        "ThresholdMetricId": str,
+        "TreatMissingData": str,
+        "Unit": str,
+    },
+    total=False,
+)
+
 AwsCloudWatchAlarmDetailsTypeDef = TypedDict(
     "AwsCloudWatchAlarmDetailsTypeDef",
     {
         "ActionsEnabled": bool,
         "AlarmActions": Sequence[str],
         "AlarmArn": str,
         "AlarmConfigurationUpdatedTimestamp": str,
@@ -5721,14 +6261,29 @@
         "ThresholdMetricId": str,
         "TreatMissingData": str,
         "Unit": str,
     },
     total=False,
 )
 
+AwsCodeBuildProjectEnvironmentOutputTypeDef = TypedDict(
+    "AwsCodeBuildProjectEnvironmentOutputTypeDef",
+    {
+        "Certificate": str,
+        "EnvironmentVariables": List[
+            AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef
+        ],
+        "PrivilegedMode": bool,
+        "ImagePullCredentialsType": str,
+        "RegistryCredential": AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef,
+        "Type": str,
+    },
+    total=False,
+)
+
 AwsCodeBuildProjectEnvironmentTypeDef = TypedDict(
     "AwsCodeBuildProjectEnvironmentTypeDef",
     {
         "Certificate": str,
         "EnvironmentVariables": Sequence[
             AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef
         ],
@@ -5745,14 +6300,41 @@
     {
         "CloudWatchLogs": AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef,
         "S3Logs": AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef,
     },
     total=False,
 )
 
+AwsDynamoDbTableGlobalSecondaryIndexOutputTypeDef = TypedDict(
+    "AwsDynamoDbTableGlobalSecondaryIndexOutputTypeDef",
+    {
+        "Backfilling": bool,
+        "IndexArn": str,
+        "IndexName": str,
+        "IndexSizeBytes": int,
+        "IndexStatus": str,
+        "ItemCount": int,
+        "KeySchema": List[AwsDynamoDbTableKeySchemaTypeDef],
+        "Projection": AwsDynamoDbTableProjectionOutputTypeDef,
+        "ProvisionedThroughput": AwsDynamoDbTableProvisionedThroughputTypeDef,
+    },
+    total=False,
+)
+
+AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef = TypedDict(
+    "AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef",
+    {
+        "IndexArn": str,
+        "IndexName": str,
+        "KeySchema": List[AwsDynamoDbTableKeySchemaTypeDef],
+        "Projection": AwsDynamoDbTableProjectionOutputTypeDef,
+    },
+    total=False,
+)
+
 AwsDynamoDbTableGlobalSecondaryIndexTypeDef = TypedDict(
     "AwsDynamoDbTableGlobalSecondaryIndexTypeDef",
     {
         "Backfilling": bool,
         "IndexArn": str,
         "IndexName": str,
         "IndexSizeBytes": int,
@@ -5781,14 +6363,34 @@
     {
         "IndexName": str,
         "ProvisionedThroughputOverride": AwsDynamoDbTableProvisionedThroughputOverrideTypeDef,
     },
     total=False,
 )
 
+AwsEc2InstanceDetailsOutputTypeDef = TypedDict(
+    "AwsEc2InstanceDetailsOutputTypeDef",
+    {
+        "Type": str,
+        "ImageId": str,
+        "IpV4Addresses": List[str],
+        "IpV6Addresses": List[str],
+        "KeyName": str,
+        "IamInstanceProfileArn": str,
+        "VpcId": str,
+        "SubnetId": str,
+        "LaunchedAt": str,
+        "NetworkInterfaces": List[AwsEc2InstanceNetworkInterfacesDetailsTypeDef],
+        "VirtualizationType": str,
+        "MetadataOptions": AwsEc2InstanceMetadataOptionsTypeDef,
+        "Monitoring": AwsEc2InstanceMonitoringDetailsTypeDef,
+    },
+    total=False,
+)
+
 AwsEc2InstanceDetailsTypeDef = TypedDict(
     "AwsEc2InstanceDetailsTypeDef",
     {
         "Type": str,
         "ImageId": str,
         "IpV4Addresses": Sequence[str],
         "IpV6Addresses": Sequence[str],
@@ -5830,14 +6432,54 @@
     {
         "MarketType": str,
         "SpotOptions": AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef,
     },
     total=False,
 )
 
+AwsEc2LaunchTemplateDataInstanceRequirementsDetailsOutputTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsOutputTypeDef",
+    {
+        "AcceleratorCount": (
+            AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef
+        ),
+        "AcceleratorManufacturers": List[str],
+        "AcceleratorNames": List[str],
+        "AcceleratorTotalMemoryMiB": (
+            AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef
+        ),
+        "AcceleratorTypes": List[str],
+        "BareMetal": str,
+        "BaselineEbsBandwidthMbps": (
+            AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef
+        ),
+        "BurstablePerformance": str,
+        "CpuManufacturers": List[str],
+        "ExcludedInstanceTypes": List[str],
+        "InstanceGenerations": List[str],
+        "LocalStorage": str,
+        "LocalStorageTypes": List[str],
+        "MemoryGiBPerVCpu": (
+            AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef
+        ),
+        "MemoryMiB": AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef,
+        "NetworkInterfaceCount": (
+            AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef
+        ),
+        "OnDemandMaxPricePercentageOverLowestPrice": int,
+        "RequireHibernateSupport": bool,
+        "SpotMaxPricePercentageOverLowestPrice": int,
+        "TotalLocalStorageGB": (
+            AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef
+        ),
+        "VCpuCount": AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef,
+    },
+    total=False,
+)
+
 AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef",
     {
         "AcceleratorCount": (
             AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef
         ),
         "AcceleratorManufacturers": Sequence[str],
@@ -5870,14 +6512,44 @@
             AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef
         ),
         "VCpuCount": AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef,
     },
     total=False,
 )
 
+AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsOutputTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsOutputTypeDef",
+    {
+        "AssociateCarrierIpAddress": bool,
+        "AssociatePublicIpAddress": bool,
+        "DeleteOnTermination": bool,
+        "Description": str,
+        "DeviceIndex": int,
+        "Groups": List[str],
+        "InterfaceType": str,
+        "Ipv4PrefixCount": int,
+        "Ipv4Prefixes": List[AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef],
+        "Ipv6AddressCount": int,
+        "Ipv6Addresses": List[
+            AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef
+        ],
+        "Ipv6PrefixCount": int,
+        "Ipv6Prefixes": List[AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef],
+        "NetworkCardIndex": int,
+        "NetworkInterfaceId": str,
+        "PrivateIpAddress": str,
+        "PrivateIpAddresses": List[
+            AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef
+        ],
+        "SecondaryPrivateIpAddressCount": int,
+        "SubnetId": str,
+    },
+    total=False,
+)
+
 AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef",
     {
         "AssociateCarrierIpAddress": bool,
         "AssociatePublicIpAddress": bool,
         "DeleteOnTermination": bool,
         "Description": str,
@@ -5919,14 +6591,29 @@
         "Protocol": str,
         "RuleAction": str,
         "RuleNumber": int,
     },
     total=False,
 )
 
+AwsEc2NetworkInterfaceDetailsOutputTypeDef = TypedDict(
+    "AwsEc2NetworkInterfaceDetailsOutputTypeDef",
+    {
+        "Attachment": AwsEc2NetworkInterfaceAttachmentTypeDef,
+        "NetworkInterfaceId": str,
+        "SecurityGroups": List[AwsEc2NetworkInterfaceSecurityGroupTypeDef],
+        "SourceDestCheck": bool,
+        "IpV6Addresses": List[AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef],
+        "PrivateIpAddresses": List[AwsEc2NetworkInterfacePrivateIpAddressDetailTypeDef],
+        "PublicDnsName": str,
+        "PublicIp": str,
+    },
+    total=False,
+)
+
 AwsEc2NetworkInterfaceDetailsTypeDef = TypedDict(
     "AwsEc2NetworkInterfaceDetailsTypeDef",
     {
         "Attachment": AwsEc2NetworkInterfaceAttachmentTypeDef,
         "NetworkInterfaceId": str,
         "SecurityGroups": Sequence[AwsEc2NetworkInterfaceSecurityGroupTypeDef],
         "SourceDestCheck": bool,
@@ -5934,28 +6621,62 @@
         "PrivateIpAddresses": Sequence[AwsEc2NetworkInterfacePrivateIpAddressDetailTypeDef],
         "PublicDnsName": str,
         "PublicIp": str,
     },
     total=False,
 )
 
+AwsEc2SecurityGroupIpPermissionOutputTypeDef = TypedDict(
+    "AwsEc2SecurityGroupIpPermissionOutputTypeDef",
+    {
+        "IpProtocol": str,
+        "FromPort": int,
+        "ToPort": int,
+        "UserIdGroupPairs": List[AwsEc2SecurityGroupUserIdGroupPairTypeDef],
+        "IpRanges": List[AwsEc2SecurityGroupIpRangeTypeDef],
+        "Ipv6Ranges": List[AwsEc2SecurityGroupIpv6RangeTypeDef],
+        "PrefixListIds": List[AwsEc2SecurityGroupPrefixListIdTypeDef],
+    },
+    total=False,
+)
+
 AwsEc2SecurityGroupIpPermissionTypeDef = TypedDict(
     "AwsEc2SecurityGroupIpPermissionTypeDef",
     {
         "IpProtocol": str,
         "FromPort": int,
         "ToPort": int,
         "UserIdGroupPairs": Sequence[AwsEc2SecurityGroupUserIdGroupPairTypeDef],
         "IpRanges": Sequence[AwsEc2SecurityGroupIpRangeTypeDef],
         "Ipv6Ranges": Sequence[AwsEc2SecurityGroupIpv6RangeTypeDef],
         "PrefixListIds": Sequence[AwsEc2SecurityGroupPrefixListIdTypeDef],
     },
     total=False,
 )
 
+AwsEc2SubnetDetailsOutputTypeDef = TypedDict(
+    "AwsEc2SubnetDetailsOutputTypeDef",
+    {
+        "AssignIpv6AddressOnCreation": bool,
+        "AvailabilityZone": str,
+        "AvailabilityZoneId": str,
+        "AvailableIpAddressCount": int,
+        "CidrBlock": str,
+        "DefaultForAz": bool,
+        "MapPublicIpOnLaunch": bool,
+        "OwnerId": str,
+        "State": str,
+        "SubnetArn": str,
+        "SubnetId": str,
+        "VpcId": str,
+        "Ipv6CidrBlockAssociationSet": List[Ipv6CidrBlockAssociationTypeDef],
+    },
+    total=False,
+)
+
 AwsEc2SubnetDetailsTypeDef = TypedDict(
     "AwsEc2SubnetDetailsTypeDef",
     {
         "AssignIpv6AddressOnCreation": bool,
         "AvailabilityZone": str,
         "AvailabilityZoneId": str,
         "AvailableIpAddressCount": int,
@@ -5968,14 +6689,32 @@
         "SubnetId": str,
         "VpcId": str,
         "Ipv6CidrBlockAssociationSet": Sequence[Ipv6CidrBlockAssociationTypeDef],
     },
     total=False,
 )
 
+AwsEc2VolumeDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VolumeDetailsOutputTypeDef",
+    {
+        "CreateTime": str,
+        "DeviceName": str,
+        "Encrypted": bool,
+        "Size": int,
+        "SnapshotId": str,
+        "Status": str,
+        "KmsKeyId": str,
+        "Attachments": List[AwsEc2VolumeAttachmentTypeDef],
+        "VolumeId": str,
+        "VolumeType": str,
+        "VolumeScanStatus": str,
+    },
+    total=False,
+)
+
 AwsEc2VolumeDetailsTypeDef = TypedDict(
     "AwsEc2VolumeDetailsTypeDef",
     {
         "CreateTime": str,
         "DeviceName": str,
         "Encrypted": bool,
         "Size": int,
@@ -5986,25 +6725,54 @@
         "VolumeId": str,
         "VolumeType": str,
         "VolumeScanStatus": str,
     },
     total=False,
 )
 
+AwsEc2VpcDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VpcDetailsOutputTypeDef",
+    {
+        "CidrBlockAssociationSet": List[CidrBlockAssociationTypeDef],
+        "Ipv6CidrBlockAssociationSet": List[Ipv6CidrBlockAssociationTypeDef],
+        "DhcpOptionsId": str,
+        "State": str,
+    },
+    total=False,
+)
+
 AwsEc2VpcDetailsTypeDef = TypedDict(
     "AwsEc2VpcDetailsTypeDef",
     {
         "CidrBlockAssociationSet": Sequence[CidrBlockAssociationTypeDef],
         "Ipv6CidrBlockAssociationSet": Sequence[Ipv6CidrBlockAssociationTypeDef],
         "DhcpOptionsId": str,
         "State": str,
     },
     total=False,
 )
 
+AwsEc2VpcEndpointServiceDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VpcEndpointServiceDetailsOutputTypeDef",
+    {
+        "AcceptanceRequired": bool,
+        "AvailabilityZones": List[str],
+        "BaseEndpointDnsNames": List[str],
+        "ManagesVpcEndpoints": bool,
+        "GatewayLoadBalancerArns": List[str],
+        "NetworkLoadBalancerArns": List[str],
+        "PrivateDnsName": str,
+        "ServiceId": str,
+        "ServiceName": str,
+        "ServiceState": str,
+        "ServiceType": List[AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef],
+    },
+    total=False,
+)
+
 AwsEc2VpcEndpointServiceDetailsTypeDef = TypedDict(
     "AwsEc2VpcEndpointServiceDetailsTypeDef",
     {
         "AcceptanceRequired": bool,
         "AvailabilityZones": Sequence[str],
         "BaseEndpointDnsNames": Sequence[str],
         "ManagesVpcEndpoints": bool,
@@ -6015,28 +6783,51 @@
         "ServiceName": str,
         "ServiceState": str,
         "ServiceType": Sequence[AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef],
     },
     total=False,
 )
 
+AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef",
+    {
+        "CidrBlock": str,
+        "CidrBlockSet": List[VpcInfoCidrBlockSetDetailsTypeDef],
+        "Ipv6CidrBlockSet": List[VpcInfoIpv6CidrBlockSetDetailsTypeDef],
+        "OwnerId": str,
+        "PeeringOptions": VpcInfoPeeringOptionsDetailsTypeDef,
+        "Region": str,
+        "VpcId": str,
+    },
+    total=False,
+)
+
 AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef = TypedDict(
     "AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef",
     {
         "CidrBlock": str,
         "CidrBlockSet": Sequence[VpcInfoCidrBlockSetDetailsTypeDef],
         "Ipv6CidrBlockSet": Sequence[VpcInfoIpv6CidrBlockSetDetailsTypeDef],
         "OwnerId": str,
         "PeeringOptions": VpcInfoPeeringOptionsDetailsTypeDef,
         "Region": str,
         "VpcId": str,
     },
     total=False,
 )
 
+AwsEc2VpnConnectionOptionsDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VpnConnectionOptionsDetailsOutputTypeDef",
+    {
+        "StaticRoutesOnly": bool,
+        "TunnelOptions": List[AwsEc2VpnConnectionOptionsTunnelOptionsDetailsOutputTypeDef],
+    },
+    total=False,
+)
+
 AwsEc2VpnConnectionOptionsDetailsTypeDef = TypedDict(
     "AwsEc2VpnConnectionOptionsDetailsTypeDef",
     {
         "StaticRoutesOnly": bool,
         "TunnelOptions": Sequence[AwsEc2VpnConnectionOptionsTunnelOptionsDetailsTypeDef],
     },
     total=False,
@@ -6063,14 +6854,25 @@
             AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef
         ),
         "Logging": str,
     },
     total=False,
 )
 
+AwsEcsContainerDetailsOutputTypeDef = TypedDict(
+    "AwsEcsContainerDetailsOutputTypeDef",
+    {
+        "Name": str,
+        "Image": str,
+        "MountPoints": List[AwsMountPointTypeDef],
+        "Privileged": bool,
+    },
+    total=False,
+)
+
 AwsEcsContainerDetailsTypeDef = TypedDict(
     "AwsEcsContainerDetailsTypeDef",
     {
         "Name": str,
         "Image": str,
         "MountPoints": Sequence[AwsMountPointTypeDef],
         "Privileged": bool,
@@ -6086,22 +6888,52 @@
         ),
         "MaximumPercent": int,
         "MinimumHealthyPercent": int,
     },
     total=False,
 )
 
+AwsEcsServiceNetworkConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsEcsServiceNetworkConfigurationDetailsOutputTypeDef",
+    {
+        "AwsVpcConfiguration": (
+            AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsOutputTypeDef
+        ),
+    },
+    total=False,
+)
+
 AwsEcsServiceNetworkConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsServiceNetworkConfigurationDetailsTypeDef",
     {
         "AwsVpcConfiguration": AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef,
     },
     total=False,
 )
 
+AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsOutputTypeDef",
+    {
+        "Capabilities": (
+            AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef
+        ),
+        "Devices": List[
+            AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsOutputTypeDef
+        ],
+        "InitProcessEnabled": bool,
+        "MaxSwap": int,
+        "SharedMemorySize": int,
+        "Swappiness": int,
+        "Tmpfs": List[
+            AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsOutputTypeDef
+        ],
+    },
+    total=False,
+)
+
 AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef",
     {
         "Capabilities": (
             AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef
         ),
         "Devices": Sequence[
@@ -6114,26 +6946,50 @@
         "Tmpfs": Sequence[
             AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsTypeDef
         ],
     },
     total=False,
 )
 
+AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsOutputTypeDef",
+    {
+        "LogDriver": str,
+        "Options": Dict[str, str],
+        "SecretOptions": List[
+            AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef
+        ],
+    },
+    total=False,
+)
+
 AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef",
     {
         "LogDriver": str,
         "Options": Mapping[str, str],
         "SecretOptions": Sequence[
             AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef
         ],
     },
     total=False,
 )
 
+AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef",
+    {
+        "ContainerName": str,
+        "ProxyConfigurationProperties": List[
+            AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef
+        ],
+        "Type": str,
+    },
+    total=False,
+)
+
 AwsEcsTaskDefinitionProxyConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionProxyConfigurationDetailsTypeDef",
     {
         "ContainerName": str,
         "ProxyConfigurationProperties": Sequence[
             AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef
         ],
@@ -6170,22 +7026,53 @@
     {
         "CreationInfo": AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef,
         "Path": str,
     },
     total=False,
 )
 
+AwsEksClusterLoggingDetailsOutputTypeDef = TypedDict(
+    "AwsEksClusterLoggingDetailsOutputTypeDef",
+    {
+        "ClusterLogging": List[AwsEksClusterLoggingClusterLoggingDetailsOutputTypeDef],
+    },
+    total=False,
+)
+
 AwsEksClusterLoggingDetailsTypeDef = TypedDict(
     "AwsEksClusterLoggingDetailsTypeDef",
     {
         "ClusterLogging": Sequence[AwsEksClusterLoggingClusterLoggingDetailsTypeDef],
     },
     total=False,
 )
 
+AwsElasticBeanstalkEnvironmentDetailsOutputTypeDef = TypedDict(
+    "AwsElasticBeanstalkEnvironmentDetailsOutputTypeDef",
+    {
+        "ApplicationName": str,
+        "Cname": str,
+        "DateCreated": str,
+        "DateUpdated": str,
+        "Description": str,
+        "EndpointUrl": str,
+        "EnvironmentArn": str,
+        "EnvironmentId": str,
+        "EnvironmentLinks": List[AwsElasticBeanstalkEnvironmentEnvironmentLinkTypeDef],
+        "EnvironmentName": str,
+        "OptionSettings": List[AwsElasticBeanstalkEnvironmentOptionSettingTypeDef],
+        "PlatformArn": str,
+        "SolutionStackName": str,
+        "Status": str,
+        "Tier": AwsElasticBeanstalkEnvironmentTierTypeDef,
+        "VersionLabel": str,
+    },
+    total=False,
+)
+
 AwsElasticBeanstalkEnvironmentDetailsTypeDef = TypedDict(
     "AwsElasticBeanstalkEnvironmentDetailsTypeDef",
     {
         "ApplicationName": str,
         "Cname": str,
         "DateCreated": str,
         "DateUpdated": str,
@@ -6227,45 +7114,94 @@
         "IndexSlowLogs": AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef,
         "SearchSlowLogs": AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef,
         "AuditLogs": AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef,
     },
     total=False,
 )
 
+AwsElbLoadBalancerPoliciesOutputTypeDef = TypedDict(
+    "AwsElbLoadBalancerPoliciesOutputTypeDef",
+    {
+        "AppCookieStickinessPolicies": List[AwsElbAppCookieStickinessPolicyTypeDef],
+        "LbCookieStickinessPolicies": List[AwsElbLbCookieStickinessPolicyTypeDef],
+        "OtherPolicies": List[str],
+    },
+    total=False,
+)
+
 AwsElbLoadBalancerPoliciesTypeDef = TypedDict(
     "AwsElbLoadBalancerPoliciesTypeDef",
     {
         "AppCookieStickinessPolicies": Sequence[AwsElbAppCookieStickinessPolicyTypeDef],
         "LbCookieStickinessPolicies": Sequence[AwsElbLbCookieStickinessPolicyTypeDef],
         "OtherPolicies": Sequence[str],
     },
     total=False,
 )
 
+AwsElbLoadBalancerAttributesOutputTypeDef = TypedDict(
+    "AwsElbLoadBalancerAttributesOutputTypeDef",
+    {
+        "AccessLog": AwsElbLoadBalancerAccessLogTypeDef,
+        "ConnectionDraining": AwsElbLoadBalancerConnectionDrainingTypeDef,
+        "ConnectionSettings": AwsElbLoadBalancerConnectionSettingsTypeDef,
+        "CrossZoneLoadBalancing": AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef,
+        "AdditionalAttributes": List[AwsElbLoadBalancerAdditionalAttributeTypeDef],
+    },
+    total=False,
+)
+
 AwsElbLoadBalancerAttributesTypeDef = TypedDict(
     "AwsElbLoadBalancerAttributesTypeDef",
     {
         "AccessLog": AwsElbLoadBalancerAccessLogTypeDef,
         "ConnectionDraining": AwsElbLoadBalancerConnectionDrainingTypeDef,
         "ConnectionSettings": AwsElbLoadBalancerConnectionSettingsTypeDef,
         "CrossZoneLoadBalancing": AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef,
         "AdditionalAttributes": Sequence[AwsElbLoadBalancerAdditionalAttributeTypeDef],
     },
     total=False,
 )
 
+AwsElbLoadBalancerListenerDescriptionOutputTypeDef = TypedDict(
+    "AwsElbLoadBalancerListenerDescriptionOutputTypeDef",
+    {
+        "Listener": AwsElbLoadBalancerListenerTypeDef,
+        "PolicyNames": List[str],
+    },
+    total=False,
+)
+
 AwsElbLoadBalancerListenerDescriptionTypeDef = TypedDict(
     "AwsElbLoadBalancerListenerDescriptionTypeDef",
     {
         "Listener": AwsElbLoadBalancerListenerTypeDef,
         "PolicyNames": Sequence[str],
     },
     total=False,
 )
 
+AwsElbv2LoadBalancerDetailsOutputTypeDef = TypedDict(
+    "AwsElbv2LoadBalancerDetailsOutputTypeDef",
+    {
+        "AvailabilityZones": List[AvailabilityZoneTypeDef],
+        "CanonicalHostedZoneId": str,
+        "CreatedTime": str,
+        "DNSName": str,
+        "IpAddressType": str,
+        "Scheme": str,
+        "SecurityGroups": List[str],
+        "State": LoadBalancerStateTypeDef,
+        "Type": str,
+        "VpcId": str,
+        "LoadBalancerAttributes": List[AwsElbv2LoadBalancerAttributeTypeDef],
+    },
+    total=False,
+)
+
 AwsElbv2LoadBalancerDetailsTypeDef = TypedDict(
     "AwsElbv2LoadBalancerDetailsTypeDef",
     {
         "AvailabilityZones": Sequence[AvailabilityZoneTypeDef],
         "CanonicalHostedZoneId": str,
         "CreatedTime": str,
         "DNSName": str,
@@ -6301,40 +7237,84 @@
     {
         "Attributes": AwsIamAccessKeySessionContextAttributesTypeDef,
         "SessionIssuer": AwsIamAccessKeySessionContextSessionIssuerTypeDef,
     },
     total=False,
 )
 
+AwsIamGroupDetailsOutputTypeDef = TypedDict(
+    "AwsIamGroupDetailsOutputTypeDef",
+    {
+        "AttachedManagedPolicies": List[AwsIamAttachedManagedPolicyTypeDef],
+        "CreateDate": str,
+        "GroupId": str,
+        "GroupName": str,
+        "GroupPolicyList": List[AwsIamGroupPolicyTypeDef],
+        "Path": str,
+    },
+    total=False,
+)
+
 AwsIamGroupDetailsTypeDef = TypedDict(
     "AwsIamGroupDetailsTypeDef",
     {
         "AttachedManagedPolicies": Sequence[AwsIamAttachedManagedPolicyTypeDef],
         "CreateDate": str,
         "GroupId": str,
         "GroupName": str,
         "GroupPolicyList": Sequence[AwsIamGroupPolicyTypeDef],
         "Path": str,
     },
     total=False,
 )
 
+AwsIamInstanceProfileOutputTypeDef = TypedDict(
+    "AwsIamInstanceProfileOutputTypeDef",
+    {
+        "Arn": str,
+        "CreateDate": str,
+        "InstanceProfileId": str,
+        "InstanceProfileName": str,
+        "Path": str,
+        "Roles": List[AwsIamInstanceProfileRoleTypeDef],
+    },
+    total=False,
+)
+
 AwsIamInstanceProfileTypeDef = TypedDict(
     "AwsIamInstanceProfileTypeDef",
     {
         "Arn": str,
         "CreateDate": str,
         "InstanceProfileId": str,
         "InstanceProfileName": str,
         "Path": str,
         "Roles": Sequence[AwsIamInstanceProfileRoleTypeDef],
     },
     total=False,
 )
 
+AwsIamPolicyDetailsOutputTypeDef = TypedDict(
+    "AwsIamPolicyDetailsOutputTypeDef",
+    {
+        "AttachmentCount": int,
+        "CreateDate": str,
+        "DefaultVersionId": str,
+        "Description": str,
+        "IsAttachable": bool,
+        "Path": str,
+        "PermissionsBoundaryUsageCount": int,
+        "PolicyId": str,
+        "PolicyName": str,
+        "PolicyVersionList": List[AwsIamPolicyVersionTypeDef],
+        "UpdateDate": str,
+    },
+    total=False,
+)
+
 AwsIamPolicyDetailsTypeDef = TypedDict(
     "AwsIamPolicyDetailsTypeDef",
     {
         "AttachmentCount": int,
         "CreateDate": str,
         "DefaultVersionId": str,
         "Description": str,
@@ -6345,14 +7325,29 @@
         "PolicyName": str,
         "PolicyVersionList": Sequence[AwsIamPolicyVersionTypeDef],
         "UpdateDate": str,
     },
     total=False,
 )
 
+AwsIamUserDetailsOutputTypeDef = TypedDict(
+    "AwsIamUserDetailsOutputTypeDef",
+    {
+        "AttachedManagedPolicies": List[AwsIamAttachedManagedPolicyTypeDef],
+        "CreateDate": str,
+        "GroupList": List[str],
+        "Path": str,
+        "PermissionsBoundary": AwsIamPermissionsBoundaryTypeDef,
+        "UserId": str,
+        "UserName": str,
+        "UserPolicyList": List[AwsIamUserPolicyTypeDef],
+    },
+    total=False,
+)
+
 AwsIamUserDetailsTypeDef = TypedDict(
     "AwsIamUserDetailsTypeDef",
     {
         "AttachedManagedPolicies": Sequence[AwsIamAttachedManagedPolicyTypeDef],
         "CreateDate": str,
         "GroupList": Sequence[str],
         "Path": str,
@@ -6372,23 +7367,49 @@
         "StreamEncryption": AwsKinesisStreamStreamEncryptionDetailsTypeDef,
         "ShardCount": int,
         "RetentionPeriodHours": int,
     },
     total=False,
 )
 
+AwsLambdaFunctionEnvironmentOutputTypeDef = TypedDict(
+    "AwsLambdaFunctionEnvironmentOutputTypeDef",
+    {
+        "Variables": Dict[str, str],
+        "Error": AwsLambdaFunctionEnvironmentErrorTypeDef,
+    },
+    total=False,
+)
+
 AwsLambdaFunctionEnvironmentTypeDef = TypedDict(
     "AwsLambdaFunctionEnvironmentTypeDef",
     {
         "Variables": Mapping[str, str],
         "Error": AwsLambdaFunctionEnvironmentErrorTypeDef,
     },
     total=False,
 )
 
+AwsNetworkFirewallFirewallDetailsOutputTypeDef = TypedDict(
+    "AwsNetworkFirewallFirewallDetailsOutputTypeDef",
+    {
+        "DeleteProtection": bool,
+        "Description": str,
+        "FirewallArn": str,
+        "FirewallId": str,
+        "FirewallName": str,
+        "FirewallPolicyArn": str,
+        "FirewallPolicyChangeProtection": bool,
+        "SubnetChangeProtection": bool,
+        "SubnetMappings": List[AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef],
+        "VpcId": str,
+    },
+    total=False,
+)
+
 AwsNetworkFirewallFirewallDetailsTypeDef = TypedDict(
     "AwsNetworkFirewallFirewallDetailsTypeDef",
     {
         "DeleteProtection": bool,
         "Description": str,
         "FirewallArn": str,
         "FirewallId": str,
@@ -6437,14 +7458,58 @@
         "IndexSlowLogs": AwsOpenSearchServiceDomainLogPublishingOptionTypeDef,
         "SearchSlowLogs": AwsOpenSearchServiceDomainLogPublishingOptionTypeDef,
         "AuditLogs": AwsOpenSearchServiceDomainLogPublishingOptionTypeDef,
     },
     total=False,
 )
 
+AwsRdsDbClusterDetailsOutputTypeDef = TypedDict(
+    "AwsRdsDbClusterDetailsOutputTypeDef",
+    {
+        "AllocatedStorage": int,
+        "AvailabilityZones": List[str],
+        "BackupRetentionPeriod": int,
+        "DatabaseName": str,
+        "Status": str,
+        "Endpoint": str,
+        "ReaderEndpoint": str,
+        "CustomEndpoints": List[str],
+        "MultiAz": bool,
+        "Engine": str,
+        "EngineVersion": str,
+        "Port": int,
+        "MasterUsername": str,
+        "PreferredBackupWindow": str,
+        "PreferredMaintenanceWindow": str,
+        "ReadReplicaIdentifiers": List[str],
+        "VpcSecurityGroups": List[AwsRdsDbInstanceVpcSecurityGroupTypeDef],
+        "HostedZoneId": str,
+        "StorageEncrypted": bool,
+        "KmsKeyId": str,
+        "DbClusterResourceId": str,
+        "AssociatedRoles": List[AwsRdsDbClusterAssociatedRoleTypeDef],
+        "ClusterCreateTime": str,
+        "EnabledCloudWatchLogsExports": List[str],
+        "EngineMode": str,
+        "DeletionProtection": bool,
+        "HttpEndpointEnabled": bool,
+        "ActivityStreamStatus": str,
+        "CopyTagsToSnapshot": bool,
+        "CrossAccountClone": bool,
+        "DomainMemberships": List[AwsRdsDbDomainMembershipTypeDef],
+        "DbClusterParameterGroup": str,
+        "DbSubnetGroup": str,
+        "DbClusterOptionGroupMemberships": List[AwsRdsDbClusterOptionGroupMembershipTypeDef],
+        "DbClusterIdentifier": str,
+        "DbClusterMembers": List[AwsRdsDbClusterMemberTypeDef],
+        "IamDatabaseAuthenticationEnabled": bool,
+    },
+    total=False,
+)
+
 AwsRdsDbClusterDetailsTypeDef = TypedDict(
     "AwsRdsDbClusterDetailsTypeDef",
     {
         "AllocatedStorage": int,
         "AvailabilityZones": Sequence[str],
         "BackupRetentionPeriod": int,
         "DatabaseName": str,
@@ -6481,14 +7546,48 @@
         "DbClusterIdentifier": str,
         "DbClusterMembers": Sequence[AwsRdsDbClusterMemberTypeDef],
         "IamDatabaseAuthenticationEnabled": bool,
     },
     total=False,
 )
 
+AwsRdsDbSnapshotDetailsOutputTypeDef = TypedDict(
+    "AwsRdsDbSnapshotDetailsOutputTypeDef",
+    {
+        "DbSnapshotIdentifier": str,
+        "DbInstanceIdentifier": str,
+        "SnapshotCreateTime": str,
+        "Engine": str,
+        "AllocatedStorage": int,
+        "Status": str,
+        "Port": int,
+        "AvailabilityZone": str,
+        "VpcId": str,
+        "InstanceCreateTime": str,
+        "MasterUsername": str,
+        "EngineVersion": str,
+        "LicenseModel": str,
+        "SnapshotType": str,
+        "Iops": int,
+        "OptionGroupName": str,
+        "PercentProgress": int,
+        "SourceRegion": str,
+        "SourceDbSnapshotIdentifier": str,
+        "StorageType": str,
+        "TdeCredentialArn": str,
+        "Encrypted": bool,
+        "KmsKeyId": str,
+        "Timezone": str,
+        "IamDatabaseAuthenticationEnabled": bool,
+        "ProcessorFeatures": List[AwsRdsDbProcessorFeatureTypeDef],
+        "DbiResourceId": str,
+    },
+    total=False,
+)
+
 AwsRdsDbSnapshotDetailsTypeDef = TypedDict(
     "AwsRdsDbSnapshotDetailsTypeDef",
     {
         "DbSnapshotIdentifier": str,
         "DbInstanceIdentifier": str,
         "SnapshotCreateTime": str,
         "Engine": str,
@@ -6515,14 +7614,36 @@
         "IamDatabaseAuthenticationEnabled": bool,
         "ProcessorFeatures": Sequence[AwsRdsDbProcessorFeatureTypeDef],
         "DbiResourceId": str,
     },
     total=False,
 )
 
+AwsRdsDbPendingModifiedValuesOutputTypeDef = TypedDict(
+    "AwsRdsDbPendingModifiedValuesOutputTypeDef",
+    {
+        "DbInstanceClass": str,
+        "AllocatedStorage": int,
+        "MasterUserPassword": str,
+        "Port": int,
+        "BackupRetentionPeriod": int,
+        "MultiAZ": bool,
+        "EngineVersion": str,
+        "LicenseModel": str,
+        "Iops": int,
+        "DbInstanceIdentifier": str,
+        "StorageType": str,
+        "CaCertificateIdentifier": str,
+        "DbSubnetGroupName": str,
+        "PendingCloudWatchLogsExports": AwsRdsPendingCloudWatchLogsExportsOutputTypeDef,
+        "ProcessorFeatures": List[AwsRdsDbProcessorFeatureTypeDef],
+    },
+    total=False,
+)
+
 AwsRdsDbPendingModifiedValuesTypeDef = TypedDict(
     "AwsRdsDbPendingModifiedValuesTypeDef",
     {
         "DbInstanceClass": str,
         "AllocatedStorage": int,
         "MasterUserPassword": str,
         "Port": int,
@@ -6537,14 +7658,28 @@
         "DbSubnetGroupName": str,
         "PendingCloudWatchLogsExports": AwsRdsPendingCloudWatchLogsExportsTypeDef,
         "ProcessorFeatures": Sequence[AwsRdsDbProcessorFeatureTypeDef],
     },
     total=False,
 )
 
+AwsRdsDbSecurityGroupDetailsOutputTypeDef = TypedDict(
+    "AwsRdsDbSecurityGroupDetailsOutputTypeDef",
+    {
+        "DbSecurityGroupArn": str,
+        "DbSecurityGroupDescription": str,
+        "DbSecurityGroupName": str,
+        "Ec2SecurityGroups": List[AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef],
+        "IpRanges": List[AwsRdsDbSecurityGroupIpRangeTypeDef],
+        "OwnerId": str,
+        "VpcId": str,
+    },
+    total=False,
+)
+
 AwsRdsDbSecurityGroupDetailsTypeDef = TypedDict(
     "AwsRdsDbSecurityGroupDetailsTypeDef",
     {
         "DbSecurityGroupArn": str,
         "DbSecurityGroupDescription": str,
         "DbSecurityGroupName": str,
         "Ec2SecurityGroups": Sequence[AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef],
@@ -6561,14 +7696,24 @@
         "SubnetIdentifier": str,
         "SubnetAvailabilityZone": AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef,
         "SubnetStatus": str,
     },
     total=False,
 )
 
+AwsRedshiftClusterClusterParameterGroupOutputTypeDef = TypedDict(
+    "AwsRedshiftClusterClusterParameterGroupOutputTypeDef",
+    {
+        "ClusterParameterStatusList": List[AwsRedshiftClusterClusterParameterStatusTypeDef],
+        "ParameterApplyStatus": str,
+        "ParameterGroupName": str,
+    },
+    total=False,
+)
+
 AwsRedshiftClusterClusterParameterGroupTypeDef = TypedDict(
     "AwsRedshiftClusterClusterParameterGroupTypeDef",
     {
         "ClusterParameterStatusList": Sequence[AwsRedshiftClusterClusterParameterStatusTypeDef],
         "ParameterApplyStatus": str,
         "ParameterGroupName": str,
     },
@@ -6581,14 +7726,22 @@
         "Prefix": str,
         "Tag": AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsTypeDef,
         "Type": str,
     },
     total=False,
 )
 
+AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef = TypedDict(
+    "AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef",
+    {
+        "FilterRules": List[AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef],
+    },
+    total=False,
+)
+
 AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef",
     {
         "FilterRules": Sequence[AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef],
     },
     total=False,
 )
@@ -6614,14 +7767,43 @@
     {
         "Condition": AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef,
         "Redirect": AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef,
     },
     total=False,
 )
 
+AwsSageMakerNotebookInstanceDetailsOutputTypeDef = TypedDict(
+    "AwsSageMakerNotebookInstanceDetailsOutputTypeDef",
+    {
+        "AcceleratorTypes": List[str],
+        "AdditionalCodeRepositories": List[str],
+        "DefaultCodeRepository": str,
+        "DirectInternetAccess": str,
+        "FailureReason": str,
+        "InstanceMetadataServiceConfiguration": (
+            AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef
+        ),
+        "InstanceType": str,
+        "KmsKeyId": str,
+        "NetworkInterfaceId": str,
+        "NotebookInstanceArn": str,
+        "NotebookInstanceLifecycleConfigName": str,
+        "NotebookInstanceName": str,
+        "NotebookInstanceStatus": str,
+        "PlatformIdentifier": str,
+        "RoleArn": str,
+        "RootAccess": str,
+        "SecurityGroups": List[str],
+        "SubnetId": str,
+        "Url": str,
+        "VolumeSizeInGB": int,
+    },
+    total=False,
+)
+
 AwsSageMakerNotebookInstanceDetailsTypeDef = TypedDict(
     "AwsSageMakerNotebookInstanceDetailsTypeDef",
     {
         "AcceleratorTypes": Sequence[str],
         "AdditionalCodeRepositories": Sequence[str],
         "DefaultCodeRepository": str,
         "DirectInternetAccess": str,
@@ -6697,62 +7879,32 @@
     {
         "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
 )
 
-_RequiredGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
-    {
-        "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
-    },
-)
-_OptionalGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef(
-    _RequiredGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
-    _OptionalGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetFindingHistoryRequestRequestTypeDef = TypedDict(
-    "_RequiredGetFindingHistoryRequestRequestTypeDef",
-    {
-        "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
-    },
-)
-_OptionalGetFindingHistoryRequestRequestTypeDef = TypedDict(
-    "_OptionalGetFindingHistoryRequestRequestTypeDef",
+AwsSnsTopicDetailsOutputTypeDef = TypedDict(
+    "AwsSnsTopicDetailsOutputTypeDef",
     {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "NextToken": str,
-        "MaxResults": int,
+        "KmsMasterKeyId": str,
+        "Subscription": List[AwsSnsTopicSubscriptionTypeDef],
+        "TopicName": str,
+        "Owner": str,
+        "SqsSuccessFeedbackRoleArn": str,
+        "SqsFailureFeedbackRoleArn": str,
+        "ApplicationSuccessFeedbackRoleArn": str,
+        "FirehoseSuccessFeedbackRoleArn": str,
+        "FirehoseFailureFeedbackRoleArn": str,
+        "HttpSuccessFeedbackRoleArn": str,
+        "HttpFailureFeedbackRoleArn": str,
     },
     total=False,
 )
 
-
-class GetFindingHistoryRequestRequestTypeDef(
-    _RequiredGetFindingHistoryRequestRequestTypeDef, _OptionalGetFindingHistoryRequestRequestTypeDef
-):
-    pass
-
-
 AwsSnsTopicDetailsTypeDef = TypedDict(
     "AwsSnsTopicDetailsTypeDef",
     {
         "KmsMasterKeyId": str,
         "Subscription": Sequence[AwsSnsTopicSubscriptionTypeDef],
         "TopicName": str,
         "Owner": str,
@@ -6779,40 +7931,77 @@
     "AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef",
     {
         "CloudWatchLogsLogGroup": AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef,
     },
     total=False,
 )
 
+AwsWafRateBasedRuleDetailsOutputTypeDef = TypedDict(
+    "AwsWafRateBasedRuleDetailsOutputTypeDef",
+    {
+        "MetricName": str,
+        "Name": str,
+        "RateKey": str,
+        "RateLimit": int,
+        "RuleId": str,
+        "MatchPredicates": List[AwsWafRateBasedRuleMatchPredicateTypeDef],
+    },
+    total=False,
+)
+
 AwsWafRateBasedRuleDetailsTypeDef = TypedDict(
     "AwsWafRateBasedRuleDetailsTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "RateKey": str,
         "RateLimit": int,
         "RuleId": str,
         "MatchPredicates": Sequence[AwsWafRateBasedRuleMatchPredicateTypeDef],
     },
     total=False,
 )
 
+AwsWafRegionalRateBasedRuleDetailsOutputTypeDef = TypedDict(
+    "AwsWafRegionalRateBasedRuleDetailsOutputTypeDef",
+    {
+        "MetricName": str,
+        "Name": str,
+        "RateKey": str,
+        "RateLimit": int,
+        "RuleId": str,
+        "MatchPredicates": List[AwsWafRegionalRateBasedRuleMatchPredicateTypeDef],
+    },
+    total=False,
+)
+
 AwsWafRegionalRateBasedRuleDetailsTypeDef = TypedDict(
     "AwsWafRegionalRateBasedRuleDetailsTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "RateKey": str,
         "RateLimit": int,
         "RuleId": str,
         "MatchPredicates": Sequence[AwsWafRegionalRateBasedRuleMatchPredicateTypeDef],
     },
     total=False,
 )
 
+AwsWafRegionalRuleDetailsOutputTypeDef = TypedDict(
+    "AwsWafRegionalRuleDetailsOutputTypeDef",
+    {
+        "MetricName": str,
+        "Name": str,
+        "PredicateList": List[AwsWafRegionalRulePredicateListDetailsTypeDef],
+        "RuleId": str,
+    },
+    total=False,
+)
+
 AwsWafRegionalRuleDetailsTypeDef = TypedDict(
     "AwsWafRegionalRuleDetailsTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "PredicateList": Sequence[AwsWafRegionalRulePredicateListDetailsTypeDef],
         "RuleId": str,
@@ -6839,14 +8028,25 @@
         "Priority": int,
         "RuleId": str,
         "Type": str,
     },
     total=False,
 )
 
+AwsWafRuleDetailsOutputTypeDef = TypedDict(
+    "AwsWafRuleDetailsOutputTypeDef",
+    {
+        "MetricName": str,
+        "Name": str,
+        "PredicateList": List[AwsWafRulePredicateListDetailsTypeDef],
+        "RuleId": str,
+    },
+    total=False,
+)
+
 AwsWafRuleDetailsTypeDef = TypedDict(
     "AwsWafRuleDetailsTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "PredicateList": Sequence[AwsWafRulePredicateListDetailsTypeDef],
         "RuleId": str,
@@ -6861,35 +8061,66 @@
         "Priority": int,
         "RuleId": str,
         "Type": str,
     },
     total=False,
 )
 
+AwsWafWebAclRuleOutputTypeDef = TypedDict(
+    "AwsWafWebAclRuleOutputTypeDef",
+    {
+        "Action": WafActionTypeDef,
+        "ExcludedRules": List[WafExcludedRuleTypeDef],
+        "OverrideAction": WafOverrideActionTypeDef,
+        "Priority": int,
+        "RuleId": str,
+        "Type": str,
+    },
+    total=False,
+)
+
 AwsWafWebAclRuleTypeDef = TypedDict(
     "AwsWafWebAclRuleTypeDef",
     {
         "Action": WafActionTypeDef,
         "ExcludedRules": Sequence[WafExcludedRuleTypeDef],
         "OverrideAction": WafOverrideActionTypeDef,
         "Priority": int,
         "RuleId": str,
         "Type": str,
     },
     total=False,
 )
 
+AwsWafv2CustomRequestHandlingDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2CustomRequestHandlingDetailsOutputTypeDef",
+    {
+        "InsertHeaders": List[AwsWafv2CustomHttpHeaderTypeDef],
+    },
+    total=False,
+)
+
 AwsWafv2CustomRequestHandlingDetailsTypeDef = TypedDict(
     "AwsWafv2CustomRequestHandlingDetailsTypeDef",
     {
         "InsertHeaders": Sequence[AwsWafv2CustomHttpHeaderTypeDef],
     },
     total=False,
 )
 
+AwsWafv2CustomResponseDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2CustomResponseDetailsOutputTypeDef",
+    {
+        "CustomResponseBodyKey": str,
+        "ResponseCode": int,
+        "ResponseHeaders": List[AwsWafv2CustomHttpHeaderTypeDef],
+    },
+    total=False,
+)
+
 AwsWafv2CustomResponseDetailsTypeDef = TypedDict(
     "AwsWafv2CustomResponseDetailsTypeDef",
     {
         "CustomResponseBodyKey": str,
         "ResponseCode": int,
         "ResponseHeaders": Sequence[AwsWafv2CustomHttpHeaderTypeDef],
     },
@@ -6900,29 +8131,183 @@
     "AwsWafv2WebAclCaptchaConfigDetailsTypeDef",
     {
         "ImmunityTimeProperty": AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef,
     },
     total=False,
 )
 
+CreateActionTargetResponseTypeDef = TypedDict(
+    "CreateActionTargetResponseTypeDef",
+    {
+        "ActionTargetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAutomationRuleResponseTypeDef = TypedDict(
+    "CreateAutomationRuleResponseTypeDef",
+    {
+        "RuleArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFindingAggregatorResponseTypeDef = TypedDict(
+    "CreateFindingAggregatorResponseTypeDef",
+    {
+        "FindingAggregatorArn": str,
+        "FindingAggregationRegion": str,
+        "RegionLinkingMode": str,
+        "Regions": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateInsightResponseTypeDef = TypedDict(
+    "CreateInsightResponseTypeDef",
+    {
+        "InsightArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteActionTargetResponseTypeDef = TypedDict(
+    "DeleteActionTargetResponseTypeDef",
+    {
+        "ActionTargetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteInsightResponseTypeDef = TypedDict(
+    "DeleteInsightResponseTypeDef",
+    {
+        "InsightArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeActionTargetsResponseTypeDef = TypedDict(
+    "DescribeActionTargetsResponseTypeDef",
+    {
+        "ActionTargets": List[ActionTargetTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeHubResponseTypeDef = TypedDict(
+    "DescribeHubResponseTypeDef",
+    {
+        "HubArn": str,
+        "SubscribedAt": str,
+        "AutoEnableControls": bool,
+        "ControlFindingGenerator": ControlFindingGeneratorType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
+    "DescribeOrganizationConfigurationResponseTypeDef",
+    {
+        "AutoEnable": bool,
+        "MemberAccountLimitReached": bool,
+        "AutoEnableStandards": AutoEnableStandardsType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EnableImportFindingsForProductResponseTypeDef = TypedDict(
+    "EnableImportFindingsForProductResponseTypeDef",
+    {
+        "ProductSubscriptionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFindingAggregatorResponseTypeDef = TypedDict(
+    "GetFindingAggregatorResponseTypeDef",
+    {
+        "FindingAggregatorArn": str,
+        "FindingAggregationRegion": str,
+        "RegionLinkingMode": str,
+        "Regions": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetInvitationsCountResponseTypeDef = TypedDict(
+    "GetInvitationsCountResponseTypeDef",
+    {
+        "InvitationsCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAutomationRulesResponseTypeDef = TypedDict(
+    "ListAutomationRulesResponseTypeDef",
+    {
+        "AutomationRulesMetadata": List[AutomationRulesMetadataTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListEnabledProductsForImportResponseTypeDef = TypedDict(
+    "ListEnabledProductsForImportResponseTypeDef",
+    {
+        "ProductSubscriptions": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
+    "ListOrganizationAdminAccountsResponseTypeDef",
+    {
+        "AdminAccounts": List[AdminAccountTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFindingAggregatorResponseTypeDef = TypedDict(
+    "UpdateFindingAggregatorResponseTypeDef",
+    {
+        "FindingAggregatorArn": str,
+        "FindingAggregationRegion": str,
+        "RegionLinkingMode": str,
+        "Regions": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 BatchDeleteAutomationRulesResponseTypeDef = TypedDict(
     "BatchDeleteAutomationRulesResponseTypeDef",
     {
         "ProcessedAutomationRules": List[str],
         "UnprocessedAutomationRules": List[UnprocessedAutomationRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateAutomationRulesResponseTypeDef = TypedDict(
     "BatchUpdateAutomationRulesResponseTypeDef",
     {
         "ProcessedAutomationRules": List[str],
         "UnprocessedAutomationRules": List[UnprocessedAutomationRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchEnableStandardsRequestRequestTypeDef = TypedDict(
     "BatchEnableStandardsRequestRequestTypeDef",
     {
         "StandardsSubscriptionRequests": Sequence[StandardsSubscriptionRequestTypeDef],
@@ -6930,15 +8315,15 @@
 )
 
 BatchGetSecurityControlsResponseTypeDef = TypedDict(
     "BatchGetSecurityControlsResponseTypeDef",
     {
         "SecurityControls": List[SecurityControlTypeDef],
         "UnprocessedIds": List[UnprocessedSecurityControlTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetStandardsControlAssociationsRequestRequestTypeDef = TypedDict(
     "BatchGetStandardsControlAssociationsRequestRequestTypeDef",
     {
         "StandardsControlAssociationIds": Sequence[StandardsControlAssociationIdTypeDef],
@@ -6970,15 +8355,15 @@
 
 BatchImportFindingsResponseTypeDef = TypedDict(
     "BatchImportFindingsResponseTypeDef",
     {
         "FailedCount": int,
         "SuccessCount": int,
         "FailedFindings": List[ImportFindingsErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateStandardsControlAssociationsRequestRequestTypeDef = TypedDict(
     "BatchUpdateStandardsControlAssociationsRequestRequestTypeDef",
     {
         "StandardsControlAssociationUpdates": Sequence[StandardsControlAssociationUpdateTypeDef],
@@ -7004,26 +8389,52 @@
 class UnprocessedStandardsControlAssociationUpdateTypeDef(
     _RequiredUnprocessedStandardsControlAssociationUpdateTypeDef,
     _OptionalUnprocessedStandardsControlAssociationUpdateTypeDef,
 ):
     pass
 
 
+ComplianceOutputTypeDef = TypedDict(
+    "ComplianceOutputTypeDef",
+    {
+        "Status": ComplianceStatusType,
+        "RelatedRequirements": List[str],
+        "StatusReasons": List[StatusReasonTypeDef],
+        "SecurityControlId": str,
+        "AssociatedStandards": List[AssociatedStandardTypeDef],
+    },
+    total=False,
+)
+
 ComplianceTypeDef = TypedDict(
     "ComplianceTypeDef",
     {
         "Status": ComplianceStatusType,
         "RelatedRequirements": Sequence[str],
         "StatusReasons": Sequence[StatusReasonTypeDef],
         "SecurityControlId": str,
         "AssociatedStandards": Sequence[AssociatedStandardTypeDef],
     },
     total=False,
 )
 
+ContainerDetailsOutputTypeDef = TypedDict(
+    "ContainerDetailsOutputTypeDef",
+    {
+        "ContainerRuntime": str,
+        "Name": str,
+        "ImageId": str,
+        "ImageName": str,
+        "LaunchedAt": str,
+        "VolumeMounts": List[VolumeMountTypeDef],
+        "Privileged": bool,
+    },
+    total=False,
+)
+
 ContainerDetailsTypeDef = TypedDict(
     "ContainerDetailsTypeDef",
     {
         "ContainerRuntime": str,
         "Name": str,
         "ImageId": str,
         "ImageName": str,
@@ -7034,76 +8445,225 @@
     total=False,
 )
 
 CreateMembersResponseTypeDef = TypedDict(
     "CreateMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[ResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeclineInvitationsResponseTypeDef = TypedDict(
     "DeclineInvitationsResponseTypeDef",
     {
         "UnprocessedAccounts": List[ResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteInvitationsResponseTypeDef = TypedDict(
     "DeleteInvitationsResponseTypeDef",
     {
         "UnprocessedAccounts": List[ResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteMembersResponseTypeDef = TypedDict(
     "DeleteMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[ResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InviteMembersResponseTypeDef = TypedDict(
     "InviteMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[ResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DateFilterTypeDef = TypedDict(
     "DateFilterTypeDef",
     {
         "Start": str,
         "End": str,
         "DateRange": DateRangeTypeDef,
     },
     total=False,
 )
 
+DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef = TypedDict(
+    "DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef",
+    {
+        "ActionTargetArns": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeProductsRequestDescribeProductsPaginateTypeDef = TypedDict(
+    "DescribeProductsRequestDescribeProductsPaginateTypeDef",
+    {
+        "ProductArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef",
+    {
+        "StandardsSubscriptionArn": str,
+    },
+)
+_OptionalDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef(
+    _RequiredDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
+    _OptionalDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
+):
+    pass
+
+
+DescribeStandardsRequestDescribeStandardsPaginateTypeDef = TypedDict(
+    "DescribeStandardsRequestDescribeStandardsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef = TypedDict(
+    "GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef",
+    {
+        "StandardsSubscriptionArns": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetInsightsRequestGetInsightsPaginateTypeDef = TypedDict(
+    "GetInsightsRequestGetInsightsPaginateTypeDef",
+    {
+        "InsightArns": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef = TypedDict(
+    "ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef = TypedDict(
+    "ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListInvitationsRequestListInvitationsPaginateTypeDef = TypedDict(
+    "ListInvitationsRequestListInvitationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListMembersRequestListMembersPaginateTypeDef = TypedDict(
+    "ListMembersRequestListMembersPaginateTypeDef",
+    {
+        "OnlyAssociated": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef = TypedDict(
+    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef = TypedDict(
+    "ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef",
+    {
+        "StandardsArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef",
+    {
+        "SecurityControlId": str,
+    },
+)
+_OptionalListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef(
+    _RequiredListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef,
+    _OptionalListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef,
+):
+    pass
+
+
 DescribeProductsResponseTypeDef = TypedDict(
     "DescribeProductsResponseTypeDef",
     {
         "Products": List[ProductTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStandardsControlsResponseTypeDef = TypedDict(
     "DescribeStandardsControlsResponseTypeDef",
     {
         "Controls": List[StandardsControlTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ThreatOutputTypeDef = TypedDict(
+    "ThreatOutputTypeDef",
+    {
+        "Name": str,
+        "Severity": str,
+        "ItemCount": int,
+        "FilePaths": List[FilePathsTypeDef],
     },
+    total=False,
 )
 
 ThreatTypeDef = TypedDict(
     "ThreatTypeDef",
     {
         "Name": str,
         "Severity": str,
@@ -7114,15 +8674,15 @@
 )
 
 ListFindingAggregatorsResponseTypeDef = TypedDict(
     "ListFindingAggregatorsResponseTypeDef",
     {
         "FindingAggregators": List[FindingAggregatorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FindingHistoryRecordTypeDef = TypedDict(
     "FindingHistoryRecordTypeDef",
     {
         "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
@@ -7131,14 +8691,26 @@
         "UpdateSource": FindingHistoryUpdateSourceTypeDef,
         "Updates": List[FindingHistoryUpdateTypeDef],
         "NextToken": str,
     },
     total=False,
 )
 
+FindingProviderFieldsOutputTypeDef = TypedDict(
+    "FindingProviderFieldsOutputTypeDef",
+    {
+        "Confidence": int,
+        "Criticality": int,
+        "RelatedFindings": List[RelatedFindingTypeDef],
+        "Severity": FindingProviderSeverityTypeDef,
+        "Types": List[str],
+    },
+    total=False,
+)
+
 FindingProviderFieldsTypeDef = TypedDict(
     "FindingProviderFieldsTypeDef",
     {
         "Confidence": int,
         "Criticality": int,
         "RelatedFindings": Sequence[RelatedFindingTypeDef],
         "Severity": FindingProviderSeverityTypeDef,
@@ -7147,50 +8719,98 @@
     total=False,
 )
 
 GetAdministratorAccountResponseTypeDef = TypedDict(
     "GetAdministratorAccountResponseTypeDef",
     {
         "Administrator": InvitationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMasterAccountResponseTypeDef = TypedDict(
     "GetMasterAccountResponseTypeDef",
     {
         "Master": InvitationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInvitationsResponseTypeDef = TypedDict(
     "ListInvitationsResponseTypeDef",
     {
         "Invitations": List[InvitationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
+    {
+        "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
+    },
+)
+_OptionalGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef(
+    _RequiredGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
+    _OptionalGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetFindingHistoryRequestRequestTypeDef = TypedDict(
+    "_RequiredGetFindingHistoryRequestRequestTypeDef",
+    {
+        "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
+    },
+)
+_OptionalGetFindingHistoryRequestRequestTypeDef = TypedDict(
+    "_OptionalGetFindingHistoryRequestRequestTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
     },
+    total=False,
 )
 
+
+class GetFindingHistoryRequestRequestTypeDef(
+    _RequiredGetFindingHistoryRequestRequestTypeDef, _OptionalGetFindingHistoryRequestRequestTypeDef
+):
+    pass
+
+
 GetMembersResponseTypeDef = TypedDict(
     "GetMembersResponseTypeDef",
     {
         "Members": List[MemberTypeDef],
         "UnprocessedAccounts": List[ResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMembersResponseTypeDef = TypedDict(
     "ListMembersResponseTypeDef",
     {
         "Members": List[MemberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InsightResultsTypeDef = TypedDict(
     "InsightResultsTypeDef",
     {
         "InsightArn": str,
@@ -7200,25 +8820,34 @@
 )
 
 ListSecurityControlDefinitionsResponseTypeDef = TypedDict(
     "ListSecurityControlDefinitionsResponseTypeDef",
     {
         "SecurityControlDefinitions": List[SecurityControlDefinitionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStandardsControlAssociationsResponseTypeDef = TypedDict(
     "ListStandardsControlAssociationsResponseTypeDef",
     {
         "StandardsControlAssociationSummaries": List[StandardsControlAssociationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+NetworkPathComponentDetailsOutputTypeDef = TypedDict(
+    "NetworkPathComponentDetailsOutputTypeDef",
+    {
+        "Address": List[str],
+        "PortRanges": List[PortRangeTypeDef],
     },
+    total=False,
 )
 
 NetworkPathComponentDetailsTypeDef = TypedDict(
     "NetworkPathComponentDetailsTypeDef",
     {
         "Address": Sequence[str],
         "PortRanges": Sequence[PortRangeTypeDef],
@@ -7259,24 +8888,49 @@
     "RemediationTypeDef",
     {
         "Recommendation": RecommendationTypeDef,
     },
     total=False,
 )
 
+RuleGroupSourceStatefulRulesDetailsOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatefulRulesDetailsOutputTypeDef",
+    {
+        "Action": str,
+        "Header": RuleGroupSourceStatefulRulesHeaderDetailsTypeDef,
+        "RuleOptions": List[RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef],
+    },
+    total=False,
+)
+
 RuleGroupSourceStatefulRulesDetailsTypeDef = TypedDict(
     "RuleGroupSourceStatefulRulesDetailsTypeDef",
     {
         "Action": str,
         "Header": RuleGroupSourceStatefulRulesHeaderDetailsTypeDef,
         "RuleOptions": Sequence[RuleGroupSourceStatefulRulesOptionsDetailsTypeDef],
     },
     total=False,
 )
 
+RuleGroupSourceStatelessRuleMatchAttributesOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRuleMatchAttributesOutputTypeDef",
+    {
+        "DestinationPorts": List[
+            RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef
+        ],
+        "Destinations": List[RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef],
+        "Protocols": List[int],
+        "SourcePorts": List[RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef],
+        "Sources": List[RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef],
+        "TcpFlags": List[RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef],
+    },
+    total=False,
+)
+
 RuleGroupSourceStatelessRuleMatchAttributesTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesTypeDef",
     {
         "DestinationPorts": Sequence[
             RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef
         ],
         "Destinations": Sequence[RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef],
@@ -7284,14 +8938,23 @@
         "SourcePorts": Sequence[RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef],
         "Sources": Sequence[RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef],
         "TcpFlags": Sequence[RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef],
     },
     total=False,
 )
 
+RuleGroupVariablesOutputTypeDef = TypedDict(
+    "RuleGroupVariablesOutputTypeDef",
+    {
+        "IpSets": RuleGroupVariablesIpSetsDetailsOutputTypeDef,
+        "PortSets": RuleGroupVariablesPortSetsDetailsOutputTypeDef,
+    },
+    total=False,
+)
+
 RuleGroupVariablesTypeDef = TypedDict(
     "RuleGroupVariablesTypeDef",
     {
         "IpSets": RuleGroupVariablesIpSetsDetailsTypeDef,
         "PortSets": RuleGroupVariablesPortSetsDetailsTypeDef,
     },
     total=False,
@@ -7329,22 +8992,45 @@
 
 class StandardsSubscriptionTypeDef(
     _RequiredStandardsSubscriptionTypeDef, _OptionalStandardsSubscriptionTypeDef
 ):
     pass
 
 
+StatelessCustomPublishMetricActionOutputTypeDef = TypedDict(
+    "StatelessCustomPublishMetricActionOutputTypeDef",
+    {
+        "Dimensions": List[StatelessCustomPublishMetricActionDimensionTypeDef],
+    },
+    total=False,
+)
+
 StatelessCustomPublishMetricActionTypeDef = TypedDict(
     "StatelessCustomPublishMetricActionTypeDef",
     {
         "Dimensions": Sequence[StatelessCustomPublishMetricActionDimensionTypeDef],
     },
     total=False,
 )
 
+AwsApiCallActionOutputTypeDef = TypedDict(
+    "AwsApiCallActionOutputTypeDef",
+    {
+        "Api": str,
+        "ServiceName": str,
+        "CallerType": str,
+        "RemoteIpDetails": ActionRemoteIpDetailsTypeDef,
+        "DomainDetails": AwsApiCallActionDomainDetailsTypeDef,
+        "AffectedResources": Dict[str, str],
+        "FirstSeen": str,
+        "LastSeen": str,
+    },
+    total=False,
+)
+
 AwsApiCallActionTypeDef = TypedDict(
     "AwsApiCallActionTypeDef",
     {
         "Api": str,
         "ServiceName": str,
         "CallerType": str,
         "RemoteIpDetails": ActionRemoteIpDetailsTypeDef,
@@ -7375,14 +9061,40 @@
         "LocalPortDetails": ActionLocalPortDetailsTypeDef,
         "LocalIpDetails": ActionLocalIpDetailsTypeDef,
         "RemoteIpDetails": ActionRemoteIpDetailsTypeDef,
     },
     total=False,
 )
 
+_RequiredVulnerabilityOutputTypeDef = TypedDict(
+    "_RequiredVulnerabilityOutputTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalVulnerabilityOutputTypeDef = TypedDict(
+    "_OptionalVulnerabilityOutputTypeDef",
+    {
+        "VulnerablePackages": List[SoftwarePackageTypeDef],
+        "Cvss": List[CvssOutputTypeDef],
+        "RelatedVulnerabilities": List[str],
+        "Vendor": VulnerabilityVendorTypeDef,
+        "ReferenceUrls": List[str],
+        "FixAvailable": VulnerabilityFixAvailableType,
+    },
+    total=False,
+)
+
+
+class VulnerabilityOutputTypeDef(
+    _RequiredVulnerabilityOutputTypeDef, _OptionalVulnerabilityOutputTypeDef
+):
+    pass
+
+
 _RequiredVulnerabilityTypeDef = TypedDict(
     "_RequiredVulnerabilityTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalVulnerabilityTypeDef = TypedDict(
@@ -7399,36 +9111,83 @@
 )
 
 
 class VulnerabilityTypeDef(_RequiredVulnerabilityTypeDef, _OptionalVulnerabilityTypeDef):
     pass
 
 
+AwsEc2RouteTableDetailsOutputTypeDef = TypedDict(
+    "AwsEc2RouteTableDetailsOutputTypeDef",
+    {
+        "AssociationSet": List[AssociationSetDetailsTypeDef],
+        "OwnerId": str,
+        "PropagatingVgwSet": List[PropagatingVgwSetDetailsTypeDef],
+        "RouteTableId": str,
+        "RouteSet": List[RouteSetDetailsTypeDef],
+        "VpcId": str,
+    },
+    total=False,
+)
+
 AwsEc2RouteTableDetailsTypeDef = TypedDict(
     "AwsEc2RouteTableDetailsTypeDef",
     {
         "AssociationSet": Sequence[AssociationSetDetailsTypeDef],
         "OwnerId": str,
         "PropagatingVgwSet": Sequence[PropagatingVgwSetDetailsTypeDef],
         "RouteTableId": str,
         "RouteSet": Sequence[RouteSetDetailsTypeDef],
         "VpcId": str,
     },
     total=False,
 )
 
+AutomationRulesActionOutputTypeDef = TypedDict(
+    "AutomationRulesActionOutputTypeDef",
+    {
+        "Type": Literal["FINDING_FIELDS_UPDATE"],
+        "FindingFieldsUpdate": AutomationRulesFindingFieldsUpdateOutputTypeDef,
+    },
+    total=False,
+)
+
 AutomationRulesActionTypeDef = TypedDict(
     "AutomationRulesActionTypeDef",
     {
         "Type": Literal["FINDING_FIELDS_UPDATE"],
         "FindingFieldsUpdate": AutomationRulesFindingFieldsUpdateTypeDef,
     },
     total=False,
 )
 
+AwsAmazonMqBrokerDetailsOutputTypeDef = TypedDict(
+    "AwsAmazonMqBrokerDetailsOutputTypeDef",
+    {
+        "AuthenticationStrategy": str,
+        "AutoMinorVersionUpgrade": bool,
+        "BrokerArn": str,
+        "BrokerName": str,
+        "DeploymentMode": str,
+        "EncryptionOptions": AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef,
+        "EngineType": str,
+        "EngineVersion": str,
+        "HostInstanceType": str,
+        "BrokerId": str,
+        "LdapServerMetadata": AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef,
+        "Logs": AwsAmazonMqBrokerLogsDetailsTypeDef,
+        "MaintenanceWindowStartTime": AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef,
+        "PubliclyAccessible": bool,
+        "SecurityGroups": List[str],
+        "StorageType": str,
+        "SubnetIds": List[str],
+        "Users": List[AwsAmazonMqBrokerUsersDetailsTypeDef],
+    },
+    total=False,
+)
+
 AwsAmazonMqBrokerDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerDetailsTypeDef",
     {
         "AuthenticationStrategy": str,
         "AutoMinorVersionUpgrade": bool,
         "BrokerArn": str,
         "BrokerName": str,
@@ -7446,14 +9205,35 @@
         "StorageType": str,
         "SubnetIds": Sequence[str],
         "Users": Sequence[AwsAmazonMqBrokerUsersDetailsTypeDef],
     },
     total=False,
 )
 
+AwsAppSyncGraphQlApiDetailsOutputTypeDef = TypedDict(
+    "AwsAppSyncGraphQlApiDetailsOutputTypeDef",
+    {
+        "ApiId": str,
+        "Id": str,
+        "OpenIdConnectConfig": AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef,
+        "Name": str,
+        "LambdaAuthorizerConfig": AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef,
+        "XrayEnabled": bool,
+        "Arn": str,
+        "UserPoolConfig": AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef,
+        "AuthenticationType": str,
+        "LogConfig": AwsAppSyncGraphQlApiLogConfigDetailsTypeDef,
+        "AdditionalAuthenticationProviders": List[
+            AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef
+        ],
+        "WafWebAclArn": str,
+    },
+    total=False,
+)
+
 AwsAppSyncGraphQlApiDetailsTypeDef = TypedDict(
     "AwsAppSyncGraphQlApiDetailsTypeDef",
     {
         "ApiId": str,
         "Id": str,
         "OpenIdConnectConfig": AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef,
         "Name": str,
@@ -7467,27 +9247,68 @@
             AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef
         ],
         "WafWebAclArn": str,
     },
     total=False,
 )
 
+AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef = TypedDict(
+    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef",
+    {
+        "InstancesDistribution": (
+            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef
+        ),
+        "LaunchTemplate": (
+            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef
+        ),
+    },
+    total=False,
+)
+
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef",
     {
         "InstancesDistribution": (
             AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef
         ),
         "LaunchTemplate": (
             AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef
         ),
     },
     total=False,
 )
 
+AwsAutoScalingLaunchConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsAutoScalingLaunchConfigurationDetailsOutputTypeDef",
+    {
+        "AssociatePublicIpAddress": bool,
+        "BlockDeviceMappings": List[
+            AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef
+        ],
+        "ClassicLinkVpcId": str,
+        "ClassicLinkVpcSecurityGroups": List[str],
+        "CreatedTime": str,
+        "EbsOptimized": bool,
+        "IamInstanceProfile": str,
+        "ImageId": str,
+        "InstanceMonitoring": AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef,
+        "InstanceType": str,
+        "KernelId": str,
+        "KeyName": str,
+        "LaunchConfigurationName": str,
+        "PlacementTenancy": str,
+        "RamdiskId": str,
+        "SecurityGroups": List[str],
+        "SpotPrice": str,
+        "UserData": str,
+        "MetadataOptions": AwsAutoScalingLaunchConfigurationMetadataOptionsTypeDef,
+    },
+    total=False,
+)
+
 AwsAutoScalingLaunchConfigurationDetailsTypeDef = TypedDict(
     "AwsAutoScalingLaunchConfigurationDetailsTypeDef",
     {
         "AssociatePublicIpAddress": bool,
         "BlockDeviceMappings": Sequence[
             AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef
         ],
@@ -7508,14 +9329,30 @@
         "SpotPrice": str,
         "UserData": str,
         "MetadataOptions": AwsAutoScalingLaunchConfigurationMetadataOptionsTypeDef,
     },
     total=False,
 )
 
+AwsBackupBackupPlanRuleDetailsOutputTypeDef = TypedDict(
+    "AwsBackupBackupPlanRuleDetailsOutputTypeDef",
+    {
+        "TargetBackupVault": str,
+        "StartWindowMinutes": int,
+        "ScheduleExpression": str,
+        "RuleName": str,
+        "RuleId": str,
+        "EnableContinuousBackup": bool,
+        "CompletionWindowMinutes": int,
+        "CopyActions": List[AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef],
+        "Lifecycle": AwsBackupBackupPlanLifecycleDetailsTypeDef,
+    },
+    total=False,
+)
+
 AwsBackupBackupPlanRuleDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanRuleDetailsTypeDef",
     {
         "TargetBackupVault": str,
         "StartWindowMinutes": int,
         "ScheduleExpression": str,
         "RuleName": str,
@@ -7524,47 +9361,96 @@
         "CompletionWindowMinutes": int,
         "CopyActions": Sequence[AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef],
         "Lifecycle": AwsBackupBackupPlanLifecycleDetailsTypeDef,
     },
     total=False,
 )
 
+AwsCertificateManagerCertificateRenewalSummaryOutputTypeDef = TypedDict(
+    "AwsCertificateManagerCertificateRenewalSummaryOutputTypeDef",
+    {
+        "DomainValidationOptions": List[
+            AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef
+        ],
+        "RenewalStatus": str,
+        "RenewalStatusReason": str,
+        "UpdatedAt": str,
+    },
+    total=False,
+)
+
 AwsCertificateManagerCertificateRenewalSummaryTypeDef = TypedDict(
     "AwsCertificateManagerCertificateRenewalSummaryTypeDef",
     {
         "DomainValidationOptions": Sequence[
             AwsCertificateManagerCertificateDomainValidationOptionTypeDef
         ],
         "RenewalStatus": str,
         "RenewalStatusReason": str,
         "UpdatedAt": str,
     },
     total=False,
 )
 
+AwsCloudFrontDistributionOriginItemOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginItemOutputTypeDef",
+    {
+        "DomainName": str,
+        "Id": str,
+        "OriginPath": str,
+        "S3OriginConfig": AwsCloudFrontDistributionOriginS3OriginConfigTypeDef,
+        "CustomOriginConfig": AwsCloudFrontDistributionOriginCustomOriginConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 AwsCloudFrontDistributionOriginItemTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginItemTypeDef",
     {
         "DomainName": str,
         "Id": str,
         "OriginPath": str,
         "S3OriginConfig": AwsCloudFrontDistributionOriginS3OriginConfigTypeDef,
         "CustomOriginConfig": AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef,
     },
     total=False,
 )
 
+AwsCloudFrontDistributionOriginGroupOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginGroupOutputTypeDef",
+    {
+        "FailoverCriteria": AwsCloudFrontDistributionOriginGroupFailoverOutputTypeDef,
+    },
+    total=False,
+)
+
 AwsCloudFrontDistributionOriginGroupTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupTypeDef",
     {
         "FailoverCriteria": AwsCloudFrontDistributionOriginGroupFailoverTypeDef,
     },
     total=False,
 )
 
+AwsCodeBuildProjectDetailsOutputTypeDef = TypedDict(
+    "AwsCodeBuildProjectDetailsOutputTypeDef",
+    {
+        "EncryptionKey": str,
+        "Artifacts": List[AwsCodeBuildProjectArtifactsDetailsTypeDef],
+        "Environment": AwsCodeBuildProjectEnvironmentOutputTypeDef,
+        "Name": str,
+        "Source": AwsCodeBuildProjectSourceTypeDef,
+        "ServiceRole": str,
+        "LogsConfig": AwsCodeBuildProjectLogsConfigDetailsTypeDef,
+        "VpcConfig": AwsCodeBuildProjectVpcConfigOutputTypeDef,
+        "SecondaryArtifacts": List[AwsCodeBuildProjectArtifactsDetailsTypeDef],
+    },
+    total=False,
+)
+
 AwsCodeBuildProjectDetailsTypeDef = TypedDict(
     "AwsCodeBuildProjectDetailsTypeDef",
     {
         "EncryptionKey": str,
         "Artifacts": Sequence[AwsCodeBuildProjectArtifactsDetailsTypeDef],
         "Environment": AwsCodeBuildProjectEnvironmentTypeDef,
         "Name": str,
@@ -7573,27 +9459,85 @@
         "LogsConfig": AwsCodeBuildProjectLogsConfigDetailsTypeDef,
         "VpcConfig": AwsCodeBuildProjectVpcConfigTypeDef,
         "SecondaryArtifacts": Sequence[AwsCodeBuildProjectArtifactsDetailsTypeDef],
     },
     total=False,
 )
 
+AwsDynamoDbTableReplicaOutputTypeDef = TypedDict(
+    "AwsDynamoDbTableReplicaOutputTypeDef",
+    {
+        "GlobalSecondaryIndexes": List[AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef],
+        "KmsMasterKeyId": str,
+        "ProvisionedThroughputOverride": AwsDynamoDbTableProvisionedThroughputOverrideTypeDef,
+        "RegionName": str,
+        "ReplicaStatus": str,
+        "ReplicaStatusDescription": str,
+    },
+    total=False,
+)
+
 AwsDynamoDbTableReplicaTypeDef = TypedDict(
     "AwsDynamoDbTableReplicaTypeDef",
     {
         "GlobalSecondaryIndexes": Sequence[AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef],
         "KmsMasterKeyId": str,
         "ProvisionedThroughputOverride": AwsDynamoDbTableProvisionedThroughputOverrideTypeDef,
         "RegionName": str,
         "ReplicaStatus": str,
         "ReplicaStatusDescription": str,
     },
     total=False,
 )
 
+AwsEc2LaunchTemplateDataDetailsOutputTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataDetailsOutputTypeDef",
+    {
+        "BlockDeviceMappingSet": List[AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef],
+        "CapacityReservationSpecification": (
+            AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef
+        ),
+        "CpuOptions": AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef,
+        "CreditSpecification": AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef,
+        "DisableApiStop": bool,
+        "DisableApiTermination": bool,
+        "EbsOptimized": bool,
+        "ElasticGpuSpecificationSet": List[
+            AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef
+        ],
+        "ElasticInferenceAcceleratorSet": List[
+            AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef
+        ],
+        "EnclaveOptions": AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef,
+        "HibernationOptions": AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef,
+        "IamInstanceProfile": AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef,
+        "ImageId": str,
+        "InstanceInitiatedShutdownBehavior": str,
+        "InstanceMarketOptions": AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef,
+        "InstanceRequirements": AwsEc2LaunchTemplateDataInstanceRequirementsDetailsOutputTypeDef,
+        "InstanceType": str,
+        "KernelId": str,
+        "KeyName": str,
+        "LicenseSet": List[AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef],
+        "MaintenanceOptions": AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef,
+        "MetadataOptions": AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef,
+        "Monitoring": AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef,
+        "NetworkInterfaceSet": List[
+            AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsOutputTypeDef
+        ],
+        "Placement": AwsEc2LaunchTemplateDataPlacementDetailsTypeDef,
+        "PrivateDnsNameOptions": AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef,
+        "RamDiskId": str,
+        "SecurityGroupIdSet": List[str],
+        "SecurityGroupSet": List[str],
+        "UserData": str,
+    },
+    total=False,
+)
+
 AwsEc2LaunchTemplateDataDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataDetailsTypeDef",
     {
         "BlockDeviceMappingSet": Sequence[
             AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef
         ],
         "CapacityReservationSpecification": (
@@ -7631,52 +9575,108 @@
         "SecurityGroupIdSet": Sequence[str],
         "SecurityGroupSet": Sequence[str],
         "UserData": str,
     },
     total=False,
 )
 
+AwsEc2NetworkAclDetailsOutputTypeDef = TypedDict(
+    "AwsEc2NetworkAclDetailsOutputTypeDef",
+    {
+        "IsDefault": bool,
+        "NetworkAclId": str,
+        "OwnerId": str,
+        "VpcId": str,
+        "Associations": List[AwsEc2NetworkAclAssociationTypeDef],
+        "Entries": List[AwsEc2NetworkAclEntryTypeDef],
+    },
+    total=False,
+)
+
 AwsEc2NetworkAclDetailsTypeDef = TypedDict(
     "AwsEc2NetworkAclDetailsTypeDef",
     {
         "IsDefault": bool,
         "NetworkAclId": str,
         "OwnerId": str,
         "VpcId": str,
         "Associations": Sequence[AwsEc2NetworkAclAssociationTypeDef],
         "Entries": Sequence[AwsEc2NetworkAclEntryTypeDef],
     },
     total=False,
 )
 
+AwsEc2SecurityGroupDetailsOutputTypeDef = TypedDict(
+    "AwsEc2SecurityGroupDetailsOutputTypeDef",
+    {
+        "GroupName": str,
+        "GroupId": str,
+        "OwnerId": str,
+        "VpcId": str,
+        "IpPermissions": List[AwsEc2SecurityGroupIpPermissionOutputTypeDef],
+        "IpPermissionsEgress": List[AwsEc2SecurityGroupIpPermissionOutputTypeDef],
+    },
+    total=False,
+)
+
 AwsEc2SecurityGroupDetailsTypeDef = TypedDict(
     "AwsEc2SecurityGroupDetailsTypeDef",
     {
         "GroupName": str,
         "GroupId": str,
         "OwnerId": str,
         "VpcId": str,
         "IpPermissions": Sequence[AwsEc2SecurityGroupIpPermissionTypeDef],
         "IpPermissionsEgress": Sequence[AwsEc2SecurityGroupIpPermissionTypeDef],
     },
     total=False,
 )
 
+AwsEc2VpcPeeringConnectionDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VpcPeeringConnectionDetailsOutputTypeDef",
+    {
+        "AccepterVpcInfo": AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef,
+        "ExpirationTime": str,
+        "RequesterVpcInfo": AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef,
+        "Status": AwsEc2VpcPeeringConnectionStatusDetailsTypeDef,
+        "VpcPeeringConnectionId": str,
+    },
+    total=False,
+)
+
 AwsEc2VpcPeeringConnectionDetailsTypeDef = TypedDict(
     "AwsEc2VpcPeeringConnectionDetailsTypeDef",
     {
         "AccepterVpcInfo": AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef,
         "ExpirationTime": str,
         "RequesterVpcInfo": AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef,
         "Status": AwsEc2VpcPeeringConnectionStatusDetailsTypeDef,
         "VpcPeeringConnectionId": str,
     },
     total=False,
 )
 
+AwsEc2VpnConnectionDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VpnConnectionDetailsOutputTypeDef",
+    {
+        "VpnConnectionId": str,
+        "State": str,
+        "CustomerGatewayId": str,
+        "CustomerGatewayConfiguration": str,
+        "Type": str,
+        "VpnGatewayId": str,
+        "Category": str,
+        "VgwTelemetry": List[AwsEc2VpnConnectionVgwTelemetryDetailsTypeDef],
+        "Options": AwsEc2VpnConnectionOptionsDetailsOutputTypeDef,
+        "Routes": List[AwsEc2VpnConnectionRoutesDetailsTypeDef],
+        "TransitGatewayId": str,
+    },
+    total=False,
+)
+
 AwsEc2VpnConnectionDetailsTypeDef = TypedDict(
     "AwsEc2VpnConnectionDetailsTypeDef",
     {
         "VpnConnectionId": str,
         "State": str,
         "CustomerGatewayId": str,
         "CustomerGatewayConfiguration": str,
@@ -7697,14 +9697,43 @@
         "ExecuteCommandConfiguration": (
             AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef
         ),
     },
     total=False,
 )
 
+AwsEcsServiceDetailsOutputTypeDef = TypedDict(
+    "AwsEcsServiceDetailsOutputTypeDef",
+    {
+        "CapacityProviderStrategy": List[AwsEcsServiceCapacityProviderStrategyDetailsTypeDef],
+        "Cluster": str,
+        "DeploymentConfiguration": AwsEcsServiceDeploymentConfigurationDetailsTypeDef,
+        "DeploymentController": AwsEcsServiceDeploymentControllerDetailsTypeDef,
+        "DesiredCount": int,
+        "EnableEcsManagedTags": bool,
+        "EnableExecuteCommand": bool,
+        "HealthCheckGracePeriodSeconds": int,
+        "LaunchType": str,
+        "LoadBalancers": List[AwsEcsServiceLoadBalancersDetailsTypeDef],
+        "Name": str,
+        "NetworkConfiguration": AwsEcsServiceNetworkConfigurationDetailsOutputTypeDef,
+        "PlacementConstraints": List[AwsEcsServicePlacementConstraintsDetailsTypeDef],
+        "PlacementStrategies": List[AwsEcsServicePlacementStrategiesDetailsTypeDef],
+        "PlatformVersion": str,
+        "PropagateTags": str,
+        "Role": str,
+        "SchedulingStrategy": str,
+        "ServiceArn": str,
+        "ServiceName": str,
+        "ServiceRegistries": List[AwsEcsServiceServiceRegistriesDetailsTypeDef],
+        "TaskDefinition": str,
+    },
+    total=False,
+)
+
 AwsEcsServiceDetailsTypeDef = TypedDict(
     "AwsEcsServiceDetailsTypeDef",
     {
         "CapacityProviderStrategy": Sequence[AwsEcsServiceCapacityProviderStrategyDetailsTypeDef],
         "Cluster": str,
         "DeploymentConfiguration": AwsEcsServiceDeploymentConfigurationDetailsTypeDef,
         "DeploymentController": AwsEcsServiceDeploymentControllerDetailsTypeDef,
@@ -7726,14 +9755,74 @@
         "ServiceName": str,
         "ServiceRegistries": Sequence[AwsEcsServiceServiceRegistriesDetailsTypeDef],
         "TaskDefinition": str,
     },
     total=False,
 )
 
+AwsEcsTaskDefinitionContainerDefinitionsDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsDetailsOutputTypeDef",
+    {
+        "Command": List[str],
+        "Cpu": int,
+        "DependsOn": List[AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef],
+        "DisableNetworking": bool,
+        "DnsSearchDomains": List[str],
+        "DnsServers": List[str],
+        "DockerLabels": Dict[str, str],
+        "DockerSecurityOptions": List[str],
+        "EntryPoint": List[str],
+        "Environment": List[AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef],
+        "EnvironmentFiles": List[
+            AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef
+        ],
+        "Essential": bool,
+        "ExtraHosts": List[AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef],
+        "FirelensConfiguration": (
+            AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef
+        ),
+        "HealthCheck": AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef,
+        "Hostname": str,
+        "Image": str,
+        "Interactive": bool,
+        "Links": List[str],
+        "LinuxParameters": (
+            AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsOutputTypeDef
+        ),
+        "LogConfiguration": (
+            AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsOutputTypeDef
+        ),
+        "Memory": int,
+        "MemoryReservation": int,
+        "MountPoints": List[AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef],
+        "Name": str,
+        "PortMappings": List[AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef],
+        "Privileged": bool,
+        "PseudoTerminal": bool,
+        "ReadonlyRootFilesystem": bool,
+        "RepositoryCredentials": (
+            AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef
+        ),
+        "ResourceRequirements": List[
+            AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef
+        ],
+        "Secrets": List[AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef],
+        "StartTimeout": int,
+        "StopTimeout": int,
+        "SystemControls": List[
+            AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsTypeDef
+        ],
+        "Ulimits": List[AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsTypeDef],
+        "User": str,
+        "VolumesFrom": List[AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef],
+        "WorkingDirectory": str,
+    },
+    total=False,
+)
+
 AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef",
     {
         "Command": Sequence[str],
         "Cpu": int,
         "DependsOn": Sequence[AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef],
         "DisableNetworking": bool,
@@ -7784,27 +9873,56 @@
         "User": str,
         "VolumesFrom": Sequence[AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef],
         "WorkingDirectory": str,
     },
     total=False,
 )
 
+AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef",
+    {
+        "DockerVolumeConfiguration": (
+            AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsOutputTypeDef
+        ),
+        "EfsVolumeConfiguration": AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef,
+        "Host": AwsEcsTaskDefinitionVolumesHostDetailsTypeDef,
+        "Name": str,
+    },
+    total=False,
+)
+
 AwsEcsTaskDefinitionVolumesDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesDetailsTypeDef",
     {
         "DockerVolumeConfiguration": (
             AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef
         ),
         "EfsVolumeConfiguration": AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef,
         "Host": AwsEcsTaskDefinitionVolumesHostDetailsTypeDef,
         "Name": str,
     },
     total=False,
 )
 
+AwsEcsTaskDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDetailsOutputTypeDef",
+    {
+        "ClusterArn": str,
+        "TaskDefinitionArn": str,
+        "Version": str,
+        "CreatedAt": str,
+        "StartedAt": str,
+        "StartedBy": str,
+        "Group": str,
+        "Volumes": List[AwsEcsTaskVolumeDetailsTypeDef],
+        "Containers": List[AwsEcsContainerDetailsOutputTypeDef],
+    },
+    total=False,
+)
+
 AwsEcsTaskDetailsTypeDef = TypedDict(
     "AwsEcsTaskDetailsTypeDef",
     {
         "ClusterArn": str,
         "TaskDefinitionArn": str,
         "Version": str,
         "CreatedAt": str,
@@ -7813,27 +9931,56 @@
         "Group": str,
         "Volumes": Sequence[AwsEcsTaskVolumeDetailsTypeDef],
         "Containers": Sequence[AwsEcsContainerDetailsTypeDef],
     },
     total=False,
 )
 
+AwsEfsAccessPointDetailsOutputTypeDef = TypedDict(
+    "AwsEfsAccessPointDetailsOutputTypeDef",
+    {
+        "AccessPointId": str,
+        "Arn": str,
+        "ClientToken": str,
+        "FileSystemId": str,
+        "PosixUser": AwsEfsAccessPointPosixUserDetailsOutputTypeDef,
+        "RootDirectory": AwsEfsAccessPointRootDirectoryDetailsTypeDef,
+    },
+    total=False,
+)
+
 AwsEfsAccessPointDetailsTypeDef = TypedDict(
     "AwsEfsAccessPointDetailsTypeDef",
     {
         "AccessPointId": str,
         "Arn": str,
         "ClientToken": str,
         "FileSystemId": str,
         "PosixUser": AwsEfsAccessPointPosixUserDetailsTypeDef,
         "RootDirectory": AwsEfsAccessPointRootDirectoryDetailsTypeDef,
     },
     total=False,
 )
 
+AwsEksClusterDetailsOutputTypeDef = TypedDict(
+    "AwsEksClusterDetailsOutputTypeDef",
+    {
+        "Arn": str,
+        "CertificateAuthorityData": str,
+        "ClusterStatus": str,
+        "Endpoint": str,
+        "Name": str,
+        "ResourcesVpcConfig": AwsEksClusterResourcesVpcConfigDetailsOutputTypeDef,
+        "RoleArn": str,
+        "Version": str,
+        "Logging": AwsEksClusterLoggingDetailsOutputTypeDef,
+    },
+    total=False,
+)
+
 AwsEksClusterDetailsTypeDef = TypedDict(
     "AwsEksClusterDetailsTypeDef",
     {
         "Arn": str,
         "CertificateAuthorityData": str,
         "ClusterStatus": str,
         "Endpoint": str,
@@ -7842,14 +9989,36 @@
         "RoleArn": str,
         "Version": str,
         "Logging": AwsEksClusterLoggingDetailsTypeDef,
     },
     total=False,
 )
 
+AwsElasticsearchDomainDetailsOutputTypeDef = TypedDict(
+    "AwsElasticsearchDomainDetailsOutputTypeDef",
+    {
+        "AccessPolicies": str,
+        "DomainEndpointOptions": AwsElasticsearchDomainDomainEndpointOptionsTypeDef,
+        "DomainId": str,
+        "DomainName": str,
+        "Endpoint": str,
+        "Endpoints": Dict[str, str],
+        "ElasticsearchVersion": str,
+        "ElasticsearchClusterConfig": (
+            AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef
+        ),
+        "EncryptionAtRestOptions": AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef,
+        "LogPublishingOptions": AwsElasticsearchDomainLogPublishingOptionsTypeDef,
+        "NodeToNodeEncryptionOptions": AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef,
+        "ServiceSoftwareOptions": AwsElasticsearchDomainServiceSoftwareOptionsTypeDef,
+        "VPCOptions": AwsElasticsearchDomainVPCOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
 AwsElasticsearchDomainDetailsTypeDef = TypedDict(
     "AwsElasticsearchDomainDetailsTypeDef",
     {
         "AccessPolicies": str,
         "DomainEndpointOptions": AwsElasticsearchDomainDomainEndpointOptionsTypeDef,
         "DomainId": str,
         "DomainName": str,
@@ -7864,14 +10033,38 @@
         "NodeToNodeEncryptionOptions": AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef,
         "ServiceSoftwareOptions": AwsElasticsearchDomainServiceSoftwareOptionsTypeDef,
         "VPCOptions": AwsElasticsearchDomainVPCOptionsTypeDef,
     },
     total=False,
 )
 
+AwsElbLoadBalancerDetailsOutputTypeDef = TypedDict(
+    "AwsElbLoadBalancerDetailsOutputTypeDef",
+    {
+        "AvailabilityZones": List[str],
+        "BackendServerDescriptions": List[AwsElbLoadBalancerBackendServerDescriptionOutputTypeDef],
+        "CanonicalHostedZoneName": str,
+        "CanonicalHostedZoneNameID": str,
+        "CreatedTime": str,
+        "DnsName": str,
+        "HealthCheck": AwsElbLoadBalancerHealthCheckTypeDef,
+        "Instances": List[AwsElbLoadBalancerInstanceTypeDef],
+        "ListenerDescriptions": List[AwsElbLoadBalancerListenerDescriptionOutputTypeDef],
+        "LoadBalancerAttributes": AwsElbLoadBalancerAttributesOutputTypeDef,
+        "LoadBalancerName": str,
+        "Policies": AwsElbLoadBalancerPoliciesOutputTypeDef,
+        "Scheme": str,
+        "SecurityGroups": List[str],
+        "SourceSecurityGroup": AwsElbLoadBalancerSourceSecurityGroupTypeDef,
+        "Subnets": List[str],
+        "VpcId": str,
+    },
+    total=False,
+)
+
 AwsElbLoadBalancerDetailsTypeDef = TypedDict(
     "AwsElbLoadBalancerDetailsTypeDef",
     {
         "AvailabilityZones": Sequence[str],
         "BackendServerDescriptions": Sequence[AwsElbLoadBalancerBackendServerDescriptionTypeDef],
         "CanonicalHostedZoneName": str,
         "CanonicalHostedZoneNameID": str,
@@ -7913,14 +10106,31 @@
         "AccountId": str,
         "AccessKeyId": str,
         "SessionContext": AwsIamAccessKeySessionContextTypeDef,
     },
     total=False,
 )
 
+AwsIamRoleDetailsOutputTypeDef = TypedDict(
+    "AwsIamRoleDetailsOutputTypeDef",
+    {
+        "AssumeRolePolicyDocument": str,
+        "AttachedManagedPolicies": List[AwsIamAttachedManagedPolicyTypeDef],
+        "CreateDate": str,
+        "InstanceProfileList": List[AwsIamInstanceProfileOutputTypeDef],
+        "PermissionsBoundary": AwsIamPermissionsBoundaryTypeDef,
+        "RoleId": str,
+        "RoleName": str,
+        "RolePolicyList": List[AwsIamRolePolicyTypeDef],
+        "MaxSessionDuration": int,
+        "Path": str,
+    },
+    total=False,
+)
+
 AwsIamRoleDetailsTypeDef = TypedDict(
     "AwsIamRoleDetailsTypeDef",
     {
         "AssumeRolePolicyDocument": str,
         "AttachedManagedPolicies": Sequence[AwsIamAttachedManagedPolicyTypeDef],
         "CreateDate": str,
         "InstanceProfileList": Sequence[AwsIamInstanceProfileTypeDef],
@@ -7930,14 +10140,41 @@
         "RolePolicyList": Sequence[AwsIamRolePolicyTypeDef],
         "MaxSessionDuration": int,
         "Path": str,
     },
     total=False,
 )
 
+AwsLambdaFunctionDetailsOutputTypeDef = TypedDict(
+    "AwsLambdaFunctionDetailsOutputTypeDef",
+    {
+        "Code": AwsLambdaFunctionCodeTypeDef,
+        "CodeSha256": str,
+        "DeadLetterConfig": AwsLambdaFunctionDeadLetterConfigTypeDef,
+        "Environment": AwsLambdaFunctionEnvironmentOutputTypeDef,
+        "FunctionName": str,
+        "Handler": str,
+        "KmsKeyArn": str,
+        "LastModified": str,
+        "Layers": List[AwsLambdaFunctionLayerTypeDef],
+        "MasterArn": str,
+        "MemorySize": int,
+        "RevisionId": str,
+        "Role": str,
+        "Runtime": str,
+        "Timeout": int,
+        "TracingConfig": AwsLambdaFunctionTracingConfigTypeDef,
+        "VpcConfig": AwsLambdaFunctionVpcConfigOutputTypeDef,
+        "Version": str,
+        "Architectures": List[str],
+        "PackageType": str,
+    },
+    total=False,
+)
+
 AwsLambdaFunctionDetailsTypeDef = TypedDict(
     "AwsLambdaFunctionDetailsTypeDef",
     {
         "Code": AwsLambdaFunctionCodeTypeDef,
         "CodeSha256": str,
         "DeadLetterConfig": AwsLambdaFunctionDeadLetterConfigTypeDef,
         "Environment": AwsLambdaFunctionEnvironmentTypeDef,
@@ -7957,14 +10194,38 @@
         "Version": str,
         "Architectures": Sequence[str],
         "PackageType": str,
     },
     total=False,
 )
 
+AwsOpenSearchServiceDomainDetailsOutputTypeDef = TypedDict(
+    "AwsOpenSearchServiceDomainDetailsOutputTypeDef",
+    {
+        "Arn": str,
+        "AccessPolicies": str,
+        "DomainName": str,
+        "Id": str,
+        "DomainEndpoint": str,
+        "EngineVersion": str,
+        "EncryptionAtRestOptions": AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsTypeDef,
+        "NodeToNodeEncryptionOptions": (
+            AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsTypeDef
+        ),
+        "ServiceSoftwareOptions": AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsTypeDef,
+        "ClusterConfig": AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef,
+        "DomainEndpointOptions": AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef,
+        "VpcOptions": AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef,
+        "LogPublishingOptions": AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef,
+        "DomainEndpoints": Dict[str, str],
+        "AdvancedSecurityOptions": AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef,
+    },
+    total=False,
+)
+
 AwsOpenSearchServiceDomainDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainDetailsTypeDef",
     {
         "Arn": str,
         "AccessPolicies": str,
         "DomainName": str,
         "Id": str,
@@ -7981,27 +10242,91 @@
         "LogPublishingOptions": AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef,
         "DomainEndpoints": Mapping[str, str],
         "AdvancedSecurityOptions": AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef,
     },
     total=False,
 )
 
+AwsRdsDbSubnetGroupOutputTypeDef = TypedDict(
+    "AwsRdsDbSubnetGroupOutputTypeDef",
+    {
+        "DbSubnetGroupName": str,
+        "DbSubnetGroupDescription": str,
+        "VpcId": str,
+        "SubnetGroupStatus": str,
+        "Subnets": List[AwsRdsDbSubnetGroupSubnetTypeDef],
+        "DbSubnetGroupArn": str,
+    },
+    total=False,
+)
+
 AwsRdsDbSubnetGroupTypeDef = TypedDict(
     "AwsRdsDbSubnetGroupTypeDef",
     {
         "DbSubnetGroupName": str,
         "DbSubnetGroupDescription": str,
         "VpcId": str,
         "SubnetGroupStatus": str,
         "Subnets": Sequence[AwsRdsDbSubnetGroupSubnetTypeDef],
         "DbSubnetGroupArn": str,
     },
     total=False,
 )
 
+AwsRedshiftClusterDetailsOutputTypeDef = TypedDict(
+    "AwsRedshiftClusterDetailsOutputTypeDef",
+    {
+        "AllowVersionUpgrade": bool,
+        "AutomatedSnapshotRetentionPeriod": int,
+        "AvailabilityZone": str,
+        "ClusterAvailabilityStatus": str,
+        "ClusterCreateTime": str,
+        "ClusterIdentifier": str,
+        "ClusterNodes": List[AwsRedshiftClusterClusterNodeTypeDef],
+        "ClusterParameterGroups": List[AwsRedshiftClusterClusterParameterGroupOutputTypeDef],
+        "ClusterPublicKey": str,
+        "ClusterRevisionNumber": str,
+        "ClusterSecurityGroups": List[AwsRedshiftClusterClusterSecurityGroupTypeDef],
+        "ClusterSnapshotCopyStatus": AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef,
+        "ClusterStatus": str,
+        "ClusterSubnetGroupName": str,
+        "ClusterVersion": str,
+        "DBName": str,
+        "DeferredMaintenanceWindows": List[AwsRedshiftClusterDeferredMaintenanceWindowTypeDef],
+        "ElasticIpStatus": AwsRedshiftClusterElasticIpStatusTypeDef,
+        "ElasticResizeNumberOfNodeOptions": str,
+        "Encrypted": bool,
+        "Endpoint": AwsRedshiftClusterEndpointTypeDef,
+        "EnhancedVpcRouting": bool,
+        "ExpectedNextSnapshotScheduleTime": str,
+        "ExpectedNextSnapshotScheduleTimeStatus": str,
+        "HsmStatus": AwsRedshiftClusterHsmStatusTypeDef,
+        "IamRoles": List[AwsRedshiftClusterIamRoleTypeDef],
+        "KmsKeyId": str,
+        "MaintenanceTrackName": str,
+        "ManualSnapshotRetentionPeriod": int,
+        "MasterUsername": str,
+        "NextMaintenanceWindowStartTime": str,
+        "NodeType": str,
+        "NumberOfNodes": int,
+        "PendingActions": List[str],
+        "PendingModifiedValues": AwsRedshiftClusterPendingModifiedValuesTypeDef,
+        "PreferredMaintenanceWindow": str,
+        "PubliclyAccessible": bool,
+        "ResizeInfo": AwsRedshiftClusterResizeInfoTypeDef,
+        "RestoreStatus": AwsRedshiftClusterRestoreStatusTypeDef,
+        "SnapshotScheduleIdentifier": str,
+        "SnapshotScheduleState": str,
+        "VpcId": str,
+        "VpcSecurityGroups": List[AwsRedshiftClusterVpcSecurityGroupTypeDef],
+        "LoggingStatus": AwsRedshiftClusterLoggingStatusTypeDef,
+    },
+    total=False,
+)
+
 AwsRedshiftClusterDetailsTypeDef = TypedDict(
     "AwsRedshiftClusterDetailsTypeDef",
     {
         "AllowVersionUpgrade": bool,
         "AutomatedSnapshotRetentionPeriod": int,
         "AvailabilityZone": str,
         "ClusterAvailabilityStatus": str,
@@ -8045,27 +10370,48 @@
         "VpcId": str,
         "VpcSecurityGroups": Sequence[AwsRedshiftClusterVpcSecurityGroupTypeDef],
         "LoggingStatus": AwsRedshiftClusterLoggingStatusTypeDef,
     },
     total=False,
 )
 
+AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsOutputTypeDef = TypedDict(
+    "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsOutputTypeDef",
+    {
+        "Operands": List[
+            AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef
+        ],
+        "Prefix": str,
+        "Tag": AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef,
+        "Type": str,
+    },
+    total=False,
+)
+
 AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef",
     {
         "Operands": Sequence[
             AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef
         ],
         "Prefix": str,
         "Tag": AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef,
         "Type": str,
     },
     total=False,
 )
 
+AwsS3BucketNotificationConfigurationFilterOutputTypeDef = TypedDict(
+    "AwsS3BucketNotificationConfigurationFilterOutputTypeDef",
+    {
+        "S3KeyFilter": AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef,
+    },
+    total=False,
+)
+
 AwsS3BucketNotificationConfigurationFilterTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationFilterTypeDef",
     {
         "S3KeyFilter": AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef,
     },
     total=False,
 )
@@ -8075,22 +10421,41 @@
     {
         "ObjectLockEnabled": str,
         "Rule": AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef,
     },
     total=False,
 )
 
+AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef = TypedDict(
+    "AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef",
+    {
+        "Rules": List[AwsS3BucketServerSideEncryptionRuleTypeDef],
+    },
+    total=False,
+)
+
 AwsS3BucketServerSideEncryptionConfigurationTypeDef = TypedDict(
     "AwsS3BucketServerSideEncryptionConfigurationTypeDef",
     {
         "Rules": Sequence[AwsS3BucketServerSideEncryptionRuleTypeDef],
     },
     total=False,
 )
 
+AwsS3BucketWebsiteConfigurationOutputTypeDef = TypedDict(
+    "AwsS3BucketWebsiteConfigurationOutputTypeDef",
+    {
+        "ErrorDocument": str,
+        "IndexDocumentSuffix": str,
+        "RedirectAllRequestsTo": AwsS3BucketWebsiteConfigurationRedirectToTypeDef,
+        "RoutingRules": List[AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef],
+    },
+    total=False,
+)
+
 AwsS3BucketWebsiteConfigurationTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationTypeDef",
     {
         "ErrorDocument": str,
         "IndexDocumentSuffix": str,
         "RedirectAllRequestsTo": AwsS3BucketWebsiteConfigurationRedirectToTypeDef,
         "RoutingRules": Sequence[AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef],
@@ -8099,83 +10464,164 @@
 )
 
 BatchUpdateFindingsResponseTypeDef = TypedDict(
     "BatchUpdateFindingsResponseTypeDef",
     {
         "ProcessedFindings": List[AwsSecurityFindingIdentifierTypeDef],
         "UnprocessedFindings": List[BatchUpdateFindingsUnprocessedFindingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AwsSsmPatchComplianceDetailsTypeDef = TypedDict(
     "AwsSsmPatchComplianceDetailsTypeDef",
     {
         "Patch": AwsSsmPatchTypeDef,
     },
     total=False,
 )
 
+AwsStepFunctionStateMachineLoggingConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsStepFunctionStateMachineLoggingConfigurationDetailsOutputTypeDef",
+    {
+        "Destinations": List[
+            AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef
+        ],
+        "IncludeExecutionData": bool,
+        "Level": str,
+    },
+    total=False,
+)
+
 AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef = TypedDict(
     "AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef",
     {
         "Destinations": Sequence[
             AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef
         ],
         "IncludeExecutionData": bool,
         "Level": str,
     },
     total=False,
 )
 
+AwsWafRegionalRuleGroupDetailsOutputTypeDef = TypedDict(
+    "AwsWafRegionalRuleGroupDetailsOutputTypeDef",
+    {
+        "MetricName": str,
+        "Name": str,
+        "RuleGroupId": str,
+        "Rules": List[AwsWafRegionalRuleGroupRulesDetailsTypeDef],
+    },
+    total=False,
+)
+
 AwsWafRegionalRuleGroupDetailsTypeDef = TypedDict(
     "AwsWafRegionalRuleGroupDetailsTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "RuleGroupId": str,
         "Rules": Sequence[AwsWafRegionalRuleGroupRulesDetailsTypeDef],
     },
     total=False,
 )
 
+AwsWafRegionalWebAclDetailsOutputTypeDef = TypedDict(
+    "AwsWafRegionalWebAclDetailsOutputTypeDef",
+    {
+        "DefaultAction": str,
+        "MetricName": str,
+        "Name": str,
+        "RulesList": List[AwsWafRegionalWebAclRulesListDetailsTypeDef],
+        "WebAclId": str,
+    },
+    total=False,
+)
+
 AwsWafRegionalWebAclDetailsTypeDef = TypedDict(
     "AwsWafRegionalWebAclDetailsTypeDef",
     {
         "DefaultAction": str,
         "MetricName": str,
         "Name": str,
         "RulesList": Sequence[AwsWafRegionalWebAclRulesListDetailsTypeDef],
         "WebAclId": str,
     },
     total=False,
 )
 
+AwsWafRuleGroupDetailsOutputTypeDef = TypedDict(
+    "AwsWafRuleGroupDetailsOutputTypeDef",
+    {
+        "MetricName": str,
+        "Name": str,
+        "RuleGroupId": str,
+        "Rules": List[AwsWafRuleGroupRulesDetailsTypeDef],
+    },
+    total=False,
+)
+
 AwsWafRuleGroupDetailsTypeDef = TypedDict(
     "AwsWafRuleGroupDetailsTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "RuleGroupId": str,
         "Rules": Sequence[AwsWafRuleGroupRulesDetailsTypeDef],
     },
     total=False,
 )
 
+AwsWafWebAclDetailsOutputTypeDef = TypedDict(
+    "AwsWafWebAclDetailsOutputTypeDef",
+    {
+        "Name": str,
+        "DefaultAction": str,
+        "Rules": List[AwsWafWebAclRuleOutputTypeDef],
+        "WebAclId": str,
+    },
+    total=False,
+)
+
 AwsWafWebAclDetailsTypeDef = TypedDict(
     "AwsWafWebAclDetailsTypeDef",
     {
         "Name": str,
         "DefaultAction": str,
         "Rules": Sequence[AwsWafWebAclRuleTypeDef],
         "WebAclId": str,
     },
     total=False,
 )
 
+AwsWafv2ActionAllowDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2ActionAllowDetailsOutputTypeDef",
+    {
+        "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsOutputTypeDef,
+    },
+    total=False,
+)
+
+AwsWafv2RulesActionCaptchaDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2RulesActionCaptchaDetailsOutputTypeDef",
+    {
+        "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsOutputTypeDef,
+    },
+    total=False,
+)
+
+AwsWafv2RulesActionCountDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2RulesActionCountDetailsOutputTypeDef",
+    {
+        "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsOutputTypeDef,
+    },
+    total=False,
+)
+
 AwsWafv2ActionAllowDetailsTypeDef = TypedDict(
     "AwsWafv2ActionAllowDetailsTypeDef",
     {
         "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsTypeDef,
     },
     total=False,
 )
@@ -8192,41 +10638,49 @@
     "AwsWafv2RulesActionCountDetailsTypeDef",
     {
         "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsTypeDef,
     },
     total=False,
 )
 
+AwsWafv2ActionBlockDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2ActionBlockDetailsOutputTypeDef",
+    {
+        "CustomResponse": AwsWafv2CustomResponseDetailsOutputTypeDef,
+    },
+    total=False,
+)
+
 AwsWafv2ActionBlockDetailsTypeDef = TypedDict(
     "AwsWafv2ActionBlockDetailsTypeDef",
     {
         "CustomResponse": AwsWafv2CustomResponseDetailsTypeDef,
     },
     total=False,
 )
 
 BatchGetStandardsControlAssociationsResponseTypeDef = TypedDict(
     "BatchGetStandardsControlAssociationsResponseTypeDef",
     {
         "StandardsControlAssociationDetails": List[StandardsControlAssociationDetailTypeDef],
         "UnprocessedAssociations": List[UnprocessedStandardsControlAssociationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateStandardsControlAssociationsResponseTypeDef = TypedDict(
     "BatchUpdateStandardsControlAssociationsResponseTypeDef",
     {
         "UnprocessedAssociationUpdates": List[UnprocessedStandardsControlAssociationUpdateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AutomationRulesFindingFiltersTypeDef = TypedDict(
-    "AutomationRulesFindingFiltersTypeDef",
+AutomationRulesFindingFiltersOutputTypeDef = TypedDict(
+    "AutomationRulesFindingFiltersOutputTypeDef",
     {
         "ProductArn": List[StringFilterTypeDef],
         "AwsAccountId": List[StringFilterTypeDef],
         "Id": List[StringFilterTypeDef],
         "GeneratorId": List[StringFilterTypeDef],
         "Type": List[StringFilterTypeDef],
         "FirstObservedAt": List[DateFilterTypeDef],
@@ -8259,14 +10713,160 @@
         "NoteUpdatedAt": List[DateFilterTypeDef],
         "NoteUpdatedBy": List[StringFilterTypeDef],
         "UserDefinedFields": List[MapFilterTypeDef],
     },
     total=False,
 )
 
+AutomationRulesFindingFiltersTypeDef = TypedDict(
+    "AutomationRulesFindingFiltersTypeDef",
+    {
+        "ProductArn": Sequence[StringFilterTypeDef],
+        "AwsAccountId": Sequence[StringFilterTypeDef],
+        "Id": Sequence[StringFilterTypeDef],
+        "GeneratorId": Sequence[StringFilterTypeDef],
+        "Type": Sequence[StringFilterTypeDef],
+        "FirstObservedAt": Sequence[DateFilterTypeDef],
+        "LastObservedAt": Sequence[DateFilterTypeDef],
+        "CreatedAt": Sequence[DateFilterTypeDef],
+        "UpdatedAt": Sequence[DateFilterTypeDef],
+        "Confidence": Sequence[NumberFilterTypeDef],
+        "Criticality": Sequence[NumberFilterTypeDef],
+        "Title": Sequence[StringFilterTypeDef],
+        "Description": Sequence[StringFilterTypeDef],
+        "SourceUrl": Sequence[StringFilterTypeDef],
+        "ProductName": Sequence[StringFilterTypeDef],
+        "CompanyName": Sequence[StringFilterTypeDef],
+        "SeverityLabel": Sequence[StringFilterTypeDef],
+        "ResourceType": Sequence[StringFilterTypeDef],
+        "ResourceId": Sequence[StringFilterTypeDef],
+        "ResourcePartition": Sequence[StringFilterTypeDef],
+        "ResourceRegion": Sequence[StringFilterTypeDef],
+        "ResourceTags": Sequence[MapFilterTypeDef],
+        "ResourceDetailsOther": Sequence[MapFilterTypeDef],
+        "ComplianceStatus": Sequence[StringFilterTypeDef],
+        "ComplianceSecurityControlId": Sequence[StringFilterTypeDef],
+        "ComplianceAssociatedStandardsId": Sequence[StringFilterTypeDef],
+        "VerificationState": Sequence[StringFilterTypeDef],
+        "WorkflowStatus": Sequence[StringFilterTypeDef],
+        "RecordState": Sequence[StringFilterTypeDef],
+        "RelatedFindingsProductArn": Sequence[StringFilterTypeDef],
+        "RelatedFindingsId": Sequence[StringFilterTypeDef],
+        "NoteText": Sequence[StringFilterTypeDef],
+        "NoteUpdatedAt": Sequence[DateFilterTypeDef],
+        "NoteUpdatedBy": Sequence[StringFilterTypeDef],
+        "UserDefinedFields": Sequence[MapFilterTypeDef],
+    },
+    total=False,
+)
+
+AwsSecurityFindingFiltersOutputTypeDef = TypedDict(
+    "AwsSecurityFindingFiltersOutputTypeDef",
+    {
+        "ProductArn": List[StringFilterTypeDef],
+        "AwsAccountId": List[StringFilterTypeDef],
+        "Id": List[StringFilterTypeDef],
+        "GeneratorId": List[StringFilterTypeDef],
+        "Region": List[StringFilterTypeDef],
+        "Type": List[StringFilterTypeDef],
+        "FirstObservedAt": List[DateFilterTypeDef],
+        "LastObservedAt": List[DateFilterTypeDef],
+        "CreatedAt": List[DateFilterTypeDef],
+        "UpdatedAt": List[DateFilterTypeDef],
+        "SeverityProduct": List[NumberFilterTypeDef],
+        "SeverityNormalized": List[NumberFilterTypeDef],
+        "SeverityLabel": List[StringFilterTypeDef],
+        "Confidence": List[NumberFilterTypeDef],
+        "Criticality": List[NumberFilterTypeDef],
+        "Title": List[StringFilterTypeDef],
+        "Description": List[StringFilterTypeDef],
+        "RecommendationText": List[StringFilterTypeDef],
+        "SourceUrl": List[StringFilterTypeDef],
+        "ProductFields": List[MapFilterTypeDef],
+        "ProductName": List[StringFilterTypeDef],
+        "CompanyName": List[StringFilterTypeDef],
+        "UserDefinedFields": List[MapFilterTypeDef],
+        "MalwareName": List[StringFilterTypeDef],
+        "MalwareType": List[StringFilterTypeDef],
+        "MalwarePath": List[StringFilterTypeDef],
+        "MalwareState": List[StringFilterTypeDef],
+        "NetworkDirection": List[StringFilterTypeDef],
+        "NetworkProtocol": List[StringFilterTypeDef],
+        "NetworkSourceIpV4": List[IpFilterTypeDef],
+        "NetworkSourceIpV6": List[IpFilterTypeDef],
+        "NetworkSourcePort": List[NumberFilterTypeDef],
+        "NetworkSourceDomain": List[StringFilterTypeDef],
+        "NetworkSourceMac": List[StringFilterTypeDef],
+        "NetworkDestinationIpV4": List[IpFilterTypeDef],
+        "NetworkDestinationIpV6": List[IpFilterTypeDef],
+        "NetworkDestinationPort": List[NumberFilterTypeDef],
+        "NetworkDestinationDomain": List[StringFilterTypeDef],
+        "ProcessName": List[StringFilterTypeDef],
+        "ProcessPath": List[StringFilterTypeDef],
+        "ProcessPid": List[NumberFilterTypeDef],
+        "ProcessParentPid": List[NumberFilterTypeDef],
+        "ProcessLaunchedAt": List[DateFilterTypeDef],
+        "ProcessTerminatedAt": List[DateFilterTypeDef],
+        "ThreatIntelIndicatorType": List[StringFilterTypeDef],
+        "ThreatIntelIndicatorValue": List[StringFilterTypeDef],
+        "ThreatIntelIndicatorCategory": List[StringFilterTypeDef],
+        "ThreatIntelIndicatorLastObservedAt": List[DateFilterTypeDef],
+        "ThreatIntelIndicatorSource": List[StringFilterTypeDef],
+        "ThreatIntelIndicatorSourceUrl": List[StringFilterTypeDef],
+        "ResourceType": List[StringFilterTypeDef],
+        "ResourceId": List[StringFilterTypeDef],
+        "ResourcePartition": List[StringFilterTypeDef],
+        "ResourceRegion": List[StringFilterTypeDef],
+        "ResourceTags": List[MapFilterTypeDef],
+        "ResourceAwsEc2InstanceType": List[StringFilterTypeDef],
+        "ResourceAwsEc2InstanceImageId": List[StringFilterTypeDef],
+        "ResourceAwsEc2InstanceIpV4Addresses": List[IpFilterTypeDef],
+        "ResourceAwsEc2InstanceIpV6Addresses": List[IpFilterTypeDef],
+        "ResourceAwsEc2InstanceKeyName": List[StringFilterTypeDef],
+        "ResourceAwsEc2InstanceIamInstanceProfileArn": List[StringFilterTypeDef],
+        "ResourceAwsEc2InstanceVpcId": List[StringFilterTypeDef],
+        "ResourceAwsEc2InstanceSubnetId": List[StringFilterTypeDef],
+        "ResourceAwsEc2InstanceLaunchedAt": List[DateFilterTypeDef],
+        "ResourceAwsS3BucketOwnerId": List[StringFilterTypeDef],
+        "ResourceAwsS3BucketOwnerName": List[StringFilterTypeDef],
+        "ResourceAwsIamAccessKeyUserName": List[StringFilterTypeDef],
+        "ResourceAwsIamAccessKeyPrincipalName": List[StringFilterTypeDef],
+        "ResourceAwsIamAccessKeyStatus": List[StringFilterTypeDef],
+        "ResourceAwsIamAccessKeyCreatedAt": List[DateFilterTypeDef],
+        "ResourceAwsIamUserUserName": List[StringFilterTypeDef],
+        "ResourceContainerName": List[StringFilterTypeDef],
+        "ResourceContainerImageId": List[StringFilterTypeDef],
+        "ResourceContainerImageName": List[StringFilterTypeDef],
+        "ResourceContainerLaunchedAt": List[DateFilterTypeDef],
+        "ResourceDetailsOther": List[MapFilterTypeDef],
+        "ComplianceStatus": List[StringFilterTypeDef],
+        "VerificationState": List[StringFilterTypeDef],
+        "WorkflowState": List[StringFilterTypeDef],
+        "WorkflowStatus": List[StringFilterTypeDef],
+        "RecordState": List[StringFilterTypeDef],
+        "RelatedFindingsProductArn": List[StringFilterTypeDef],
+        "RelatedFindingsId": List[StringFilterTypeDef],
+        "NoteText": List[StringFilterTypeDef],
+        "NoteUpdatedAt": List[DateFilterTypeDef],
+        "NoteUpdatedBy": List[StringFilterTypeDef],
+        "Keyword": List[KeywordFilterTypeDef],
+        "FindingProviderFieldsConfidence": List[NumberFilterTypeDef],
+        "FindingProviderFieldsCriticality": List[NumberFilterTypeDef],
+        "FindingProviderFieldsRelatedFindingsId": List[StringFilterTypeDef],
+        "FindingProviderFieldsRelatedFindingsProductArn": List[StringFilterTypeDef],
+        "FindingProviderFieldsSeverityLabel": List[StringFilterTypeDef],
+        "FindingProviderFieldsSeverityOriginal": List[StringFilterTypeDef],
+        "FindingProviderFieldsTypes": List[StringFilterTypeDef],
+        "Sample": List[BooleanFilterTypeDef],
+        "ComplianceSecurityControlId": List[StringFilterTypeDef],
+        "ComplianceAssociatedStandardsId": List[StringFilterTypeDef],
+    },
+    total=False,
+)
+
 AwsSecurityFindingFiltersTypeDef = TypedDict(
     "AwsSecurityFindingFiltersTypeDef",
     {
         "ProductArn": Sequence[StringFilterTypeDef],
         "AwsAccountId": Sequence[StringFilterTypeDef],
         "Id": Sequence[StringFilterTypeDef],
         "GeneratorId": Sequence[StringFilterTypeDef],
@@ -8368,108 +10968,181 @@
 )
 
 GetFindingHistoryResponseTypeDef = TypedDict(
     "GetFindingHistoryResponseTypeDef",
     {
         "Records": List[FindingHistoryRecordTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInsightResultsResponseTypeDef = TypedDict(
     "GetInsightResultsResponseTypeDef",
     {
         "InsightResults": InsightResultsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+NetworkHeaderOutputTypeDef = TypedDict(
+    "NetworkHeaderOutputTypeDef",
+    {
+        "Protocol": str,
+        "Destination": NetworkPathComponentDetailsOutputTypeDef,
+        "Source": NetworkPathComponentDetailsOutputTypeDef,
+    },
+    total=False,
+)
+
 NetworkHeaderTypeDef = TypedDict(
     "NetworkHeaderTypeDef",
     {
         "Protocol": str,
         "Destination": NetworkPathComponentDetailsTypeDef,
         "Source": NetworkPathComponentDetailsTypeDef,
     },
     total=False,
 )
 
+OccurrencesOutputTypeDef = TypedDict(
+    "OccurrencesOutputTypeDef",
+    {
+        "LineRanges": List[RangeTypeDef],
+        "OffsetRanges": List[RangeTypeDef],
+        "Pages": List[PageTypeDef],
+        "Records": List[RecordTypeDef],
+        "Cells": List[CellTypeDef],
+    },
+    total=False,
+)
+
 OccurrencesTypeDef = TypedDict(
     "OccurrencesTypeDef",
     {
         "LineRanges": Sequence[RangeTypeDef],
         "OffsetRanges": Sequence[RangeTypeDef],
         "Pages": Sequence[PageTypeDef],
         "Records": Sequence[RecordTypeDef],
         "Cells": Sequence[CellTypeDef],
     },
     total=False,
 )
 
+RuleGroupSourceStatelessRuleDefinitionOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRuleDefinitionOutputTypeDef",
+    {
+        "Actions": List[str],
+        "MatchAttributes": RuleGroupSourceStatelessRuleMatchAttributesOutputTypeDef,
+    },
+    total=False,
+)
+
 RuleGroupSourceStatelessRuleDefinitionTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleDefinitionTypeDef",
     {
         "Actions": Sequence[str],
         "MatchAttributes": RuleGroupSourceStatelessRuleMatchAttributesTypeDef,
     },
     total=False,
 )
 
 DescribeStandardsResponseTypeDef = TypedDict(
     "DescribeStandardsResponseTypeDef",
     {
         "Standards": List[StandardTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDisableStandardsResponseTypeDef = TypedDict(
     "BatchDisableStandardsResponseTypeDef",
     {
         "StandardsSubscriptions": List[StandardsSubscriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchEnableStandardsResponseTypeDef = TypedDict(
     "BatchEnableStandardsResponseTypeDef",
     {
         "StandardsSubscriptions": List[StandardsSubscriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEnabledStandardsResponseTypeDef = TypedDict(
     "GetEnabledStandardsResponseTypeDef",
     {
         "StandardsSubscriptions": List[StandardsSubscriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StatelessCustomActionDefinitionOutputTypeDef = TypedDict(
+    "StatelessCustomActionDefinitionOutputTypeDef",
+    {
+        "PublishMetricAction": StatelessCustomPublishMetricActionOutputTypeDef,
     },
+    total=False,
 )
 
 StatelessCustomActionDefinitionTypeDef = TypedDict(
     "StatelessCustomActionDefinitionTypeDef",
     {
         "PublishMetricAction": StatelessCustomPublishMetricActionTypeDef,
     },
     total=False,
 )
 
+PortProbeActionOutputTypeDef = TypedDict(
+    "PortProbeActionOutputTypeDef",
+    {
+        "PortProbeDetails": List[PortProbeDetailTypeDef],
+        "Blocked": bool,
+    },
+    total=False,
+)
+
 PortProbeActionTypeDef = TypedDict(
     "PortProbeActionTypeDef",
     {
         "PortProbeDetails": Sequence[PortProbeDetailTypeDef],
         "Blocked": bool,
     },
     total=False,
 )
 
+AutomationRulesActionUnionTypeDef = Union[
+    AutomationRulesActionTypeDef, AutomationRulesActionOutputTypeDef
+]
+AwsAutoScalingAutoScalingGroupDetailsOutputTypeDef = TypedDict(
+    "AwsAutoScalingAutoScalingGroupDetailsOutputTypeDef",
+    {
+        "LaunchConfigurationName": str,
+        "LoadBalancerNames": List[str],
+        "HealthCheckType": str,
+        "HealthCheckGracePeriod": int,
+        "CreatedTime": str,
+        "MixedInstancesPolicy": (
+            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef
+        ),
+        "AvailabilityZones": List[
+            AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef
+        ],
+        "LaunchTemplate": (
+            AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef
+        ),
+        "CapacityRebalance": bool,
+    },
+    total=False,
+)
+
 AwsAutoScalingAutoScalingGroupDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupDetailsTypeDef",
     {
         "LaunchConfigurationName": str,
         "LoadBalancerNames": Sequence[str],
         "HealthCheckType": str,
         "HealthCheckGracePeriod": int,
@@ -8482,24 +11155,68 @@
             AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef
         ),
         "CapacityRebalance": bool,
     },
     total=False,
 )
 
+AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef = TypedDict(
+    "AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef",
+    {
+        "BackupPlanName": str,
+        "AdvancedBackupSettings": List[
+            AwsBackupBackupPlanAdvancedBackupSettingsDetailsOutputTypeDef
+        ],
+        "BackupPlanRule": List[AwsBackupBackupPlanRuleDetailsOutputTypeDef],
+    },
+    total=False,
+)
+
 AwsBackupBackupPlanBackupPlanDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanBackupPlanDetailsTypeDef",
     {
         "BackupPlanName": str,
         "AdvancedBackupSettings": Sequence[AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef],
         "BackupPlanRule": Sequence[AwsBackupBackupPlanRuleDetailsTypeDef],
     },
     total=False,
 )
 
+AwsCertificateManagerCertificateDetailsOutputTypeDef = TypedDict(
+    "AwsCertificateManagerCertificateDetailsOutputTypeDef",
+    {
+        "CertificateAuthorityArn": str,
+        "CreatedAt": str,
+        "DomainName": str,
+        "DomainValidationOptions": List[
+            AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef
+        ],
+        "ExtendedKeyUsages": List[AwsCertificateManagerCertificateExtendedKeyUsageTypeDef],
+        "FailureReason": str,
+        "ImportedAt": str,
+        "InUseBy": List[str],
+        "IssuedAt": str,
+        "Issuer": str,
+        "KeyAlgorithm": str,
+        "KeyUsages": List[AwsCertificateManagerCertificateKeyUsageTypeDef],
+        "NotAfter": str,
+        "NotBefore": str,
+        "Options": AwsCertificateManagerCertificateOptionsTypeDef,
+        "RenewalEligibility": str,
+        "RenewalSummary": AwsCertificateManagerCertificateRenewalSummaryOutputTypeDef,
+        "Serial": str,
+        "SignatureAlgorithm": str,
+        "Status": str,
+        "Subject": str,
+        "SubjectAlternativeNames": List[str],
+        "Type": str,
+    },
+    total=False,
+)
+
 AwsCertificateManagerCertificateDetailsTypeDef = TypedDict(
     "AwsCertificateManagerCertificateDetailsTypeDef",
     {
         "CertificateAuthorityArn": str,
         "CreatedAt": str,
         "DomainName": str,
         "DomainValidationOptions": Sequence[
@@ -8524,30 +11241,72 @@
         "Subject": str,
         "SubjectAlternativeNames": Sequence[str],
         "Type": str,
     },
     total=False,
 )
 
+AwsCloudFrontDistributionOriginsOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginsOutputTypeDef",
+    {
+        "Items": List[AwsCloudFrontDistributionOriginItemOutputTypeDef],
+    },
+    total=False,
+)
+
 AwsCloudFrontDistributionOriginsTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginsTypeDef",
     {
         "Items": Sequence[AwsCloudFrontDistributionOriginItemTypeDef],
     },
     total=False,
 )
 
+AwsCloudFrontDistributionOriginGroupsOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginGroupsOutputTypeDef",
+    {
+        "Items": List[AwsCloudFrontDistributionOriginGroupOutputTypeDef],
+    },
+    total=False,
+)
+
 AwsCloudFrontDistributionOriginGroupsTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupsTypeDef",
     {
         "Items": Sequence[AwsCloudFrontDistributionOriginGroupTypeDef],
     },
     total=False,
 )
 
+AwsDynamoDbTableDetailsOutputTypeDef = TypedDict(
+    "AwsDynamoDbTableDetailsOutputTypeDef",
+    {
+        "AttributeDefinitions": List[AwsDynamoDbTableAttributeDefinitionTypeDef],
+        "BillingModeSummary": AwsDynamoDbTableBillingModeSummaryTypeDef,
+        "CreationDateTime": str,
+        "GlobalSecondaryIndexes": List[AwsDynamoDbTableGlobalSecondaryIndexOutputTypeDef],
+        "GlobalTableVersion": str,
+        "ItemCount": int,
+        "KeySchema": List[AwsDynamoDbTableKeySchemaTypeDef],
+        "LatestStreamArn": str,
+        "LatestStreamLabel": str,
+        "LocalSecondaryIndexes": List[AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef],
+        "ProvisionedThroughput": AwsDynamoDbTableProvisionedThroughputTypeDef,
+        "Replicas": List[AwsDynamoDbTableReplicaOutputTypeDef],
+        "RestoreSummary": AwsDynamoDbTableRestoreSummaryTypeDef,
+        "SseDescription": AwsDynamoDbTableSseDescriptionTypeDef,
+        "StreamSpecification": AwsDynamoDbTableStreamSpecificationTypeDef,
+        "TableId": str,
+        "TableName": str,
+        "TableSizeBytes": int,
+        "TableStatus": str,
+    },
+    total=False,
+)
+
 AwsDynamoDbTableDetailsTypeDef = TypedDict(
     "AwsDynamoDbTableDetailsTypeDef",
     {
         "AttributeDefinitions": Sequence[AwsDynamoDbTableAttributeDefinitionTypeDef],
         "BillingModeSummary": AwsDynamoDbTableBillingModeSummaryTypeDef,
         "CreationDateTime": str,
         "GlobalSecondaryIndexes": Sequence[AwsDynamoDbTableGlobalSecondaryIndexTypeDef],
@@ -8566,26 +11325,57 @@
         "TableName": str,
         "TableSizeBytes": int,
         "TableStatus": str,
     },
     total=False,
 )
 
+AwsEc2LaunchTemplateDetailsOutputTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDetailsOutputTypeDef",
+    {
+        "LaunchTemplateName": str,
+        "Id": str,
+        "LaunchTemplateData": AwsEc2LaunchTemplateDataDetailsOutputTypeDef,
+        "DefaultVersionNumber": int,
+        "LatestVersionNumber": int,
+    },
+    total=False,
+)
+
 AwsEc2LaunchTemplateDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDetailsTypeDef",
     {
         "LaunchTemplateName": str,
         "Id": str,
         "LaunchTemplateData": AwsEc2LaunchTemplateDataDetailsTypeDef,
         "DefaultVersionNumber": int,
         "LatestVersionNumber": int,
     },
     total=False,
 )
 
+AwsEcsClusterDetailsOutputTypeDef = TypedDict(
+    "AwsEcsClusterDetailsOutputTypeDef",
+    {
+        "ClusterArn": str,
+        "ActiveServicesCount": int,
+        "CapacityProviders": List[str],
+        "ClusterSettings": List[AwsEcsClusterClusterSettingsDetailsTypeDef],
+        "Configuration": AwsEcsClusterConfigurationDetailsTypeDef,
+        "DefaultCapacityProviderStrategy": List[
+            AwsEcsClusterDefaultCapacityProviderStrategyDetailsTypeDef
+        ],
+        "ClusterName": str,
+        "RegisteredContainerInstancesCount": int,
+        "RunningTasksCount": int,
+        "Status": str,
+    },
+    total=False,
+)
+
 AwsEcsClusterDetailsTypeDef = TypedDict(
     "AwsEcsClusterDetailsTypeDef",
     {
         "ClusterArn": str,
         "ActiveServicesCount": int,
         "CapacityProviders": Sequence[str],
         "ClusterSettings": Sequence[AwsEcsClusterClusterSettingsDetailsTypeDef],
@@ -8597,14 +11387,35 @@
         "RegisteredContainerInstancesCount": int,
         "RunningTasksCount": int,
         "Status": str,
     },
     total=False,
 )
 
+AwsEcsTaskDefinitionDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionDetailsOutputTypeDef",
+    {
+        "ContainerDefinitions": List[AwsEcsTaskDefinitionContainerDefinitionsDetailsOutputTypeDef],
+        "Cpu": str,
+        "ExecutionRoleArn": str,
+        "Family": str,
+        "InferenceAccelerators": List[AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef],
+        "IpcMode": str,
+        "Memory": str,
+        "NetworkMode": str,
+        "PidMode": str,
+        "PlacementConstraints": List[AwsEcsTaskDefinitionPlacementConstraintsDetailsTypeDef],
+        "ProxyConfiguration": AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef,
+        "RequiresCompatibilities": List[str],
+        "TaskRoleArn": str,
+        "Volumes": List[AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef],
+    },
+    total=False,
+)
+
 AwsEcsTaskDefinitionDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionDetailsTypeDef",
     {
         "ContainerDefinitions": Sequence[AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef],
         "Cpu": str,
         "ExecutionRoleArn": str,
         "Family": str,
@@ -8631,14 +11442,78 @@
         "Kubernetes": AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef,
         "MalwareProtection": AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef,
         "S3Logs": AwsGuardDutyDetectorDataSourcesS3LogsDetailsTypeDef,
     },
     total=False,
 )
 
+AwsRdsDbInstanceDetailsOutputTypeDef = TypedDict(
+    "AwsRdsDbInstanceDetailsOutputTypeDef",
+    {
+        "AssociatedRoles": List[AwsRdsDbInstanceAssociatedRoleTypeDef],
+        "CACertificateIdentifier": str,
+        "DBClusterIdentifier": str,
+        "DBInstanceIdentifier": str,
+        "DBInstanceClass": str,
+        "DbInstancePort": int,
+        "DbiResourceId": str,
+        "DBName": str,
+        "DeletionProtection": bool,
+        "Endpoint": AwsRdsDbInstanceEndpointTypeDef,
+        "Engine": str,
+        "EngineVersion": str,
+        "IAMDatabaseAuthenticationEnabled": bool,
+        "InstanceCreateTime": str,
+        "KmsKeyId": str,
+        "PubliclyAccessible": bool,
+        "StorageEncrypted": bool,
+        "TdeCredentialArn": str,
+        "VpcSecurityGroups": List[AwsRdsDbInstanceVpcSecurityGroupTypeDef],
+        "MultiAz": bool,
+        "EnhancedMonitoringResourceArn": str,
+        "DbInstanceStatus": str,
+        "MasterUsername": str,
+        "AllocatedStorage": int,
+        "PreferredBackupWindow": str,
+        "BackupRetentionPeriod": int,
+        "DbSecurityGroups": List[str],
+        "DbParameterGroups": List[AwsRdsDbParameterGroupTypeDef],
+        "AvailabilityZone": str,
+        "DbSubnetGroup": AwsRdsDbSubnetGroupOutputTypeDef,
+        "PreferredMaintenanceWindow": str,
+        "PendingModifiedValues": AwsRdsDbPendingModifiedValuesOutputTypeDef,
+        "LatestRestorableTime": str,
+        "AutoMinorVersionUpgrade": bool,
+        "ReadReplicaSourceDBInstanceIdentifier": str,
+        "ReadReplicaDBInstanceIdentifiers": List[str],
+        "ReadReplicaDBClusterIdentifiers": List[str],
+        "LicenseModel": str,
+        "Iops": int,
+        "OptionGroupMemberships": List[AwsRdsDbOptionGroupMembershipTypeDef],
+        "CharacterSetName": str,
+        "SecondaryAvailabilityZone": str,
+        "StatusInfos": List[AwsRdsDbStatusInfoTypeDef],
+        "StorageType": str,
+        "DomainMemberships": List[AwsRdsDbDomainMembershipTypeDef],
+        "CopyTagsToSnapshot": bool,
+        "MonitoringInterval": int,
+        "MonitoringRoleArn": str,
+        "PromotionTier": int,
+        "Timezone": str,
+        "PerformanceInsightsEnabled": bool,
+        "PerformanceInsightsKmsKeyId": str,
+        "PerformanceInsightsRetentionPeriod": int,
+        "EnabledCloudWatchLogsExports": List[str],
+        "ProcessorFeatures": List[AwsRdsDbProcessorFeatureTypeDef],
+        "ListenerEndpoint": AwsRdsDbInstanceEndpointTypeDef,
+        "MaxAllocatedStorage": int,
+    },
+    total=False,
+)
+
 AwsRdsDbInstanceDetailsTypeDef = TypedDict(
     "AwsRdsDbInstanceDetailsTypeDef",
     {
         "AssociatedRoles": Sequence[AwsRdsDbInstanceAssociatedRoleTypeDef],
         "CACertificateIdentifier": str,
         "DBClusterIdentifier": str,
         "DBInstanceIdentifier": str,
@@ -8695,33 +11570,69 @@
         "ProcessorFeatures": Sequence[AwsRdsDbProcessorFeatureTypeDef],
         "ListenerEndpoint": AwsRdsDbInstanceEndpointTypeDef,
         "MaxAllocatedStorage": int,
     },
     total=False,
 )
 
+AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsOutputTypeDef = TypedDict(
+    "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsOutputTypeDef",
+    {
+        "Predicate": (
+            AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsOutputTypeDef
+        ),
+    },
+    total=False,
+)
+
 AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef",
     {
         "Predicate": AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef,
     },
     total=False,
 )
 
+AwsS3BucketNotificationConfigurationDetailOutputTypeDef = TypedDict(
+    "AwsS3BucketNotificationConfigurationDetailOutputTypeDef",
+    {
+        "Events": List[str],
+        "Filter": AwsS3BucketNotificationConfigurationFilterOutputTypeDef,
+        "Destination": str,
+        "Type": str,
+    },
+    total=False,
+)
+
 AwsS3BucketNotificationConfigurationDetailTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationDetailTypeDef",
     {
         "Events": Sequence[str],
         "Filter": AwsS3BucketNotificationConfigurationFilterTypeDef,
         "Destination": str,
         "Type": str,
     },
     total=False,
 )
 
+AwsStepFunctionStateMachineDetailsOutputTypeDef = TypedDict(
+    "AwsStepFunctionStateMachineDetailsOutputTypeDef",
+    {
+        "Label": str,
+        "LoggingConfiguration": AwsStepFunctionStateMachineLoggingConfigurationDetailsOutputTypeDef,
+        "Name": str,
+        "RoleArn": str,
+        "StateMachineArn": str,
+        "Status": str,
+        "TracingConfiguration": AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef,
+        "Type": str,
+    },
+    total=False,
+)
+
 AwsStepFunctionStateMachineDetailsTypeDef = TypedDict(
     "AwsStepFunctionStateMachineDetailsTypeDef",
     {
         "Label": str,
         "LoggingConfiguration": AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef,
         "Name": str,
         "RoleArn": str,
@@ -8729,14 +11640,34 @@
         "Status": str,
         "TracingConfiguration": AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef,
         "Type": str,
     },
     total=False,
 )
 
+AwsWafv2RulesActionDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2RulesActionDetailsOutputTypeDef",
+    {
+        "Allow": AwsWafv2ActionAllowDetailsOutputTypeDef,
+        "Block": AwsWafv2ActionBlockDetailsOutputTypeDef,
+        "Captcha": AwsWafv2RulesActionCaptchaDetailsOutputTypeDef,
+        "Count": AwsWafv2RulesActionCountDetailsOutputTypeDef,
+    },
+    total=False,
+)
+
+AwsWafv2WebAclActionDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2WebAclActionDetailsOutputTypeDef",
+    {
+        "Allow": AwsWafv2ActionAllowDetailsOutputTypeDef,
+        "Block": AwsWafv2ActionBlockDetailsOutputTypeDef,
+    },
+    total=False,
+)
+
 AwsWafv2RulesActionDetailsTypeDef = TypedDict(
     "AwsWafv2RulesActionDetailsTypeDef",
     {
         "Allow": AwsWafv2ActionAllowDetailsTypeDef,
         "Block": AwsWafv2ActionBlockDetailsTypeDef,
         "Captcha": AwsWafv2RulesActionCaptchaDetailsTypeDef,
         "Count": AwsWafv2RulesActionCountDetailsTypeDef,
@@ -8758,51 +11689,26 @@
     {
         "RuleArn": str,
         "RuleStatus": RuleStatusType,
         "RuleOrder": int,
         "RuleName": str,
         "Description": str,
         "IsTerminal": bool,
-        "Criteria": AutomationRulesFindingFiltersTypeDef,
-        "Actions": List[AutomationRulesActionTypeDef],
+        "Criteria": AutomationRulesFindingFiltersOutputTypeDef,
+        "Actions": List[AutomationRulesActionOutputTypeDef],
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
         "CreatedBy": str,
     },
     total=False,
 )
 
-_RequiredCreateAutomationRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAutomationRuleRequestRequestTypeDef",
-    {
-        "RuleOrder": int,
-        "RuleName": str,
-        "Description": str,
-        "Criteria": AutomationRulesFindingFiltersTypeDef,
-        "Actions": Sequence[AutomationRulesActionTypeDef],
-    },
-)
-_OptionalCreateAutomationRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAutomationRuleRequestRequestTypeDef",
-    {
-        "Tags": Mapping[str, str],
-        "RuleStatus": RuleStatusType,
-        "IsTerminal": bool,
-    },
-    total=False,
-)
-
-
-class CreateAutomationRuleRequestRequestTypeDef(
-    _RequiredCreateAutomationRuleRequestRequestTypeDef,
-    _OptionalCreateAutomationRuleRequestRequestTypeDef,
-):
-    pass
-
-
+AutomationRulesFindingFiltersUnionTypeDef = Union[
+    AutomationRulesFindingFiltersTypeDef, AutomationRulesFindingFiltersOutputTypeDef
+]
 _RequiredUpdateAutomationRulesRequestItemTypeDef = TypedDict(
     "_RequiredUpdateAutomationRulesRequestItemTypeDef",
     {
         "RuleArn": str,
     },
 )
 _OptionalUpdateAutomationRulesRequestItemTypeDef = TypedDict(
@@ -8823,29 +11729,42 @@
 class UpdateAutomationRulesRequestItemTypeDef(
     _RequiredUpdateAutomationRulesRequestItemTypeDef,
     _OptionalUpdateAutomationRulesRequestItemTypeDef,
 ):
     pass
 
 
+InsightTypeDef = TypedDict(
+    "InsightTypeDef",
+    {
+        "InsightArn": str,
+        "Name": str,
+        "Filters": AwsSecurityFindingFiltersOutputTypeDef,
+        "GroupByAttribute": str,
+    },
+)
+
+AwsSecurityFindingFiltersUnionTypeDef = Union[
+    AwsSecurityFindingFiltersTypeDef, AwsSecurityFindingFiltersOutputTypeDef
+]
 CreateInsightRequestRequestTypeDef = TypedDict(
     "CreateInsightRequestRequestTypeDef",
     {
         "Name": str,
         "Filters": AwsSecurityFindingFiltersTypeDef,
         "GroupByAttribute": str,
     },
 )
 
 GetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
     "GetFindingsRequestGetFindingsPaginateTypeDef",
     {
         "Filters": AwsSecurityFindingFiltersTypeDef,
         "SortCriteria": Sequence[SortCriterionTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetFindingsRequestRequestTypeDef = TypedDict(
     "GetFindingsRequestRequestTypeDef",
     {
@@ -8853,24 +11772,14 @@
         "SortCriteria": Sequence[SortCriterionTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-InsightTypeDef = TypedDict(
-    "InsightTypeDef",
-    {
-        "InsightArn": str,
-        "Name": str,
-        "Filters": AwsSecurityFindingFiltersTypeDef,
-        "GroupByAttribute": str,
-    },
-)
-
 _RequiredUpdateFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFindingsRequestRequestTypeDef",
     {
         "Filters": AwsSecurityFindingFiltersTypeDef,
     },
 )
 _OptionalUpdateFindingsRequestRequestTypeDef = TypedDict(
@@ -8908,25 +11817,57 @@
 
 class UpdateInsightRequestRequestTypeDef(
     _RequiredUpdateInsightRequestRequestTypeDef, _OptionalUpdateInsightRequestRequestTypeDef
 ):
     pass
 
 
+NetworkPathComponentOutputTypeDef = TypedDict(
+    "NetworkPathComponentOutputTypeDef",
+    {
+        "ComponentId": str,
+        "ComponentType": str,
+        "Egress": NetworkHeaderOutputTypeDef,
+        "Ingress": NetworkHeaderOutputTypeDef,
+    },
+    total=False,
+)
+
 NetworkPathComponentTypeDef = TypedDict(
     "NetworkPathComponentTypeDef",
     {
         "ComponentId": str,
         "ComponentType": str,
         "Egress": NetworkHeaderTypeDef,
         "Ingress": NetworkHeaderTypeDef,
     },
     total=False,
 )
 
+CustomDataIdentifiersDetectionsOutputTypeDef = TypedDict(
+    "CustomDataIdentifiersDetectionsOutputTypeDef",
+    {
+        "Count": int,
+        "Arn": str,
+        "Name": str,
+        "Occurrences": OccurrencesOutputTypeDef,
+    },
+    total=False,
+)
+
+SensitiveDataDetectionsOutputTypeDef = TypedDict(
+    "SensitiveDataDetectionsOutputTypeDef",
+    {
+        "Count": int,
+        "Type": str,
+        "Occurrences": OccurrencesOutputTypeDef,
+    },
+    total=False,
+)
+
 CustomDataIdentifiersDetectionsTypeDef = TypedDict(
     "CustomDataIdentifiersDetectionsTypeDef",
     {
         "Count": int,
         "Arn": str,
         "Name": str,
         "Occurrences": OccurrencesTypeDef,
@@ -8940,23 +11881,50 @@
         "Count": int,
         "Type": str,
         "Occurrences": OccurrencesTypeDef,
     },
     total=False,
 )
 
+RuleGroupSourceStatelessRulesDetailsOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRulesDetailsOutputTypeDef",
+    {
+        "Priority": int,
+        "RuleDefinition": RuleGroupSourceStatelessRuleDefinitionOutputTypeDef,
+    },
+    total=False,
+)
+
 RuleGroupSourceStatelessRulesDetailsTypeDef = TypedDict(
     "RuleGroupSourceStatelessRulesDetailsTypeDef",
     {
         "Priority": int,
         "RuleDefinition": RuleGroupSourceStatelessRuleDefinitionTypeDef,
     },
     total=False,
 )
 
+FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef = TypedDict(
+    "FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef",
+    {
+        "ActionDefinition": StatelessCustomActionDefinitionOutputTypeDef,
+        "ActionName": str,
+    },
+    total=False,
+)
+
+RuleGroupSourceCustomActionsDetailsOutputTypeDef = TypedDict(
+    "RuleGroupSourceCustomActionsDetailsOutputTypeDef",
+    {
+        "ActionDefinition": StatelessCustomActionDefinitionOutputTypeDef,
+        "ActionName": str,
+    },
+    total=False,
+)
+
 FirewallPolicyStatelessCustomActionsDetailsTypeDef = TypedDict(
     "FirewallPolicyStatelessCustomActionsDetailsTypeDef",
     {
         "ActionDefinition": StatelessCustomActionDefinitionTypeDef,
         "ActionName": str,
     },
     total=False,
@@ -8967,37 +11935,107 @@
     {
         "ActionDefinition": StatelessCustomActionDefinitionTypeDef,
         "ActionName": str,
     },
     total=False,
 )
 
+ActionOutputTypeDef = TypedDict(
+    "ActionOutputTypeDef",
+    {
+        "ActionType": str,
+        "NetworkConnectionAction": NetworkConnectionActionTypeDef,
+        "AwsApiCallAction": AwsApiCallActionOutputTypeDef,
+        "DnsRequestAction": DnsRequestActionTypeDef,
+        "PortProbeAction": PortProbeActionOutputTypeDef,
+    },
+    total=False,
+)
+
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "ActionType": str,
         "NetworkConnectionAction": NetworkConnectionActionTypeDef,
         "AwsApiCallAction": AwsApiCallActionTypeDef,
         "DnsRequestAction": DnsRequestActionTypeDef,
         "PortProbeAction": PortProbeActionTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateAutomationRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAutomationRuleRequestRequestTypeDef",
+    {
+        "RuleOrder": int,
+        "RuleName": str,
+        "Description": str,
+        "Criteria": AutomationRulesFindingFiltersTypeDef,
+        "Actions": Sequence[AutomationRulesActionUnionTypeDef],
+    },
+)
+_OptionalCreateAutomationRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAutomationRuleRequestRequestTypeDef",
+    {
+        "Tags": Mapping[str, str],
+        "RuleStatus": RuleStatusType,
+        "IsTerminal": bool,
+    },
+    total=False,
+)
+
+
+class CreateAutomationRuleRequestRequestTypeDef(
+    _RequiredCreateAutomationRuleRequestRequestTypeDef,
+    _OptionalCreateAutomationRuleRequestRequestTypeDef,
+):
+    pass
+
+
+AwsBackupBackupPlanDetailsOutputTypeDef = TypedDict(
+    "AwsBackupBackupPlanDetailsOutputTypeDef",
+    {
+        "BackupPlan": AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef,
+        "BackupPlanArn": str,
+        "BackupPlanId": str,
+        "VersionId": str,
+    },
+    total=False,
+)
+
 AwsBackupBackupPlanDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanDetailsTypeDef",
     {
         "BackupPlan": AwsBackupBackupPlanBackupPlanDetailsTypeDef,
         "BackupPlanArn": str,
         "BackupPlanId": str,
         "VersionId": str,
     },
     total=False,
 )
 
+AwsCloudFrontDistributionDetailsOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionDetailsOutputTypeDef",
+    {
+        "CacheBehaviors": AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef,
+        "DefaultCacheBehavior": AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef,
+        "DefaultRootObject": str,
+        "DomainName": str,
+        "ETag": str,
+        "LastModifiedTime": str,
+        "Logging": AwsCloudFrontDistributionLoggingTypeDef,
+        "Origins": AwsCloudFrontDistributionOriginsOutputTypeDef,
+        "OriginGroups": AwsCloudFrontDistributionOriginGroupsOutputTypeDef,
+        "ViewerCertificate": AwsCloudFrontDistributionViewerCertificateTypeDef,
+        "Status": str,
+        "WebAclId": str,
+    },
+    total=False,
+)
+
 AwsCloudFrontDistributionDetailsTypeDef = TypedDict(
     "AwsCloudFrontDistributionDetailsTypeDef",
     {
         "CacheBehaviors": AwsCloudFrontDistributionCacheBehaviorsTypeDef,
         "DefaultCacheBehavior": AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef,
         "DefaultRootObject": str,
         "DomainName": str,
@@ -9009,26 +12047,60 @@
         "ViewerCertificate": AwsCloudFrontDistributionViewerCertificateTypeDef,
         "Status": str,
         "WebAclId": str,
     },
     total=False,
 )
 
+AwsGuardDutyDetectorDetailsOutputTypeDef = TypedDict(
+    "AwsGuardDutyDetectorDetailsOutputTypeDef",
+    {
+        "DataSources": AwsGuardDutyDetectorDataSourcesDetailsTypeDef,
+        "Features": List[AwsGuardDutyDetectorFeaturesDetailsTypeDef],
+        "FindingPublishingFrequency": str,
+        "ServiceRole": str,
+        "Status": str,
+    },
+    total=False,
+)
+
 AwsGuardDutyDetectorDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDetailsTypeDef",
     {
         "DataSources": AwsGuardDutyDetectorDataSourcesDetailsTypeDef,
         "Features": Sequence[AwsGuardDutyDetectorFeaturesDetailsTypeDef],
         "FindingPublishingFrequency": str,
         "ServiceRole": str,
         "Status": str,
     },
     total=False,
 )
 
+AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef = TypedDict(
+    "AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef",
+    {
+        "AbortIncompleteMultipartUpload": (
+            AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef
+        ),
+        "ExpirationDate": str,
+        "ExpirationInDays": int,
+        "ExpiredObjectDeleteMarker": bool,
+        "Filter": AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsOutputTypeDef,
+        "ID": str,
+        "NoncurrentVersionExpirationInDays": int,
+        "NoncurrentVersionTransitions": List[
+            AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsTypeDef
+        ],
+        "Prefix": str,
+        "Status": str,
+        "Transitions": List[AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsTypeDef],
+    },
+    total=False,
+)
+
 AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef",
     {
         "AbortIncompleteMultipartUpload": (
             AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef
         ),
         "ExpirationDate": str,
@@ -9045,22 +12117,42 @@
         "Transitions": Sequence[
             AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsTypeDef
         ],
     },
     total=False,
 )
 
+AwsS3BucketNotificationConfigurationOutputTypeDef = TypedDict(
+    "AwsS3BucketNotificationConfigurationOutputTypeDef",
+    {
+        "Configurations": List[AwsS3BucketNotificationConfigurationDetailOutputTypeDef],
+    },
+    total=False,
+)
+
 AwsS3BucketNotificationConfigurationTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationTypeDef",
     {
         "Configurations": Sequence[AwsS3BucketNotificationConfigurationDetailTypeDef],
     },
     total=False,
 )
 
+AwsWafv2RulesDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2RulesDetailsOutputTypeDef",
+    {
+        "Action": AwsWafv2RulesActionDetailsOutputTypeDef,
+        "Name": str,
+        "OverrideAction": str,
+        "Priority": int,
+        "VisibilityConfig": AwsWafv2VisibilityConfigDetailsTypeDef,
+    },
+    total=False,
+)
+
 AwsWafv2RulesDetailsTypeDef = TypedDict(
     "AwsWafv2RulesDetailsTypeDef",
     {
         "Action": AwsWafv2RulesActionDetailsTypeDef,
         "Name": str,
         "OverrideAction": str,
         "Priority": int,
@@ -9070,15 +12162,15 @@
 )
 
 BatchGetAutomationRulesResponseTypeDef = TypedDict(
     "BatchGetAutomationRulesResponseTypeDef",
     {
         "Rules": List[AutomationRulesConfigTypeDef],
         "UnprocessedAutomationRules": List[UnprocessedAutomationRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateAutomationRulesRequestRequestTypeDef = TypedDict(
     "BatchUpdateAutomationRulesRequestRequestTypeDef",
     {
         "UpdateAutomationRulesRequestItems": Sequence[UpdateAutomationRulesRequestItemTypeDef],
@@ -9086,16 +12178,35 @@
 )
 
 GetInsightsResponseTypeDef = TypedDict(
     "GetInsightsResponseTypeDef",
     {
         "Insights": List[InsightTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CustomDataIdentifiersResultOutputTypeDef = TypedDict(
+    "CustomDataIdentifiersResultOutputTypeDef",
+    {
+        "Detections": List[CustomDataIdentifiersDetectionsOutputTypeDef],
+        "TotalCount": int,
+    },
+    total=False,
+)
+
+SensitiveDataResultOutputTypeDef = TypedDict(
+    "SensitiveDataResultOutputTypeDef",
+    {
+        "Category": str,
+        "Detections": List[SensitiveDataDetectionsOutputTypeDef],
+        "TotalCount": int,
     },
+    total=False,
 )
 
 CustomDataIdentifiersResultTypeDef = TypedDict(
     "CustomDataIdentifiersResultTypeDef",
     {
         "Detections": Sequence[CustomDataIdentifiersDetectionsTypeDef],
         "TotalCount": int,
@@ -9109,14 +12220,39 @@
         "Category": str,
         "Detections": Sequence[SensitiveDataDetectionsTypeDef],
         "TotalCount": int,
     },
     total=False,
 )
 
+FirewallPolicyDetailsOutputTypeDef = TypedDict(
+    "FirewallPolicyDetailsOutputTypeDef",
+    {
+        "StatefulRuleGroupReferences": List[
+            FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef
+        ],
+        "StatelessCustomActions": List[FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef],
+        "StatelessDefaultActions": List[str],
+        "StatelessFragmentDefaultActions": List[str],
+        "StatelessRuleGroupReferences": List[
+            FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef
+        ],
+    },
+    total=False,
+)
+
+RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef",
+    {
+        "CustomActions": List[RuleGroupSourceCustomActionsDetailsOutputTypeDef],
+        "StatelessRules": List[RuleGroupSourceStatelessRulesDetailsOutputTypeDef],
+    },
+    total=False,
+)
+
 FirewallPolicyDetailsTypeDef = TypedDict(
     "FirewallPolicyDetailsTypeDef",
     {
         "StatefulRuleGroupReferences": Sequence[
             FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef
         ],
         "StatelessCustomActions": Sequence[FirewallPolicyStatelessCustomActionsDetailsTypeDef],
@@ -9134,22 +12270,62 @@
     {
         "CustomActions": Sequence[RuleGroupSourceCustomActionsDetailsTypeDef],
         "StatelessRules": Sequence[RuleGroupSourceStatelessRulesDetailsTypeDef],
     },
     total=False,
 )
 
+AwsS3BucketBucketLifecycleConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsS3BucketBucketLifecycleConfigurationDetailsOutputTypeDef",
+    {
+        "Rules": List[AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef],
+    },
+    total=False,
+)
+
 AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef",
     {
         "Rules": Sequence[AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef],
     },
     total=False,
 )
 
+AwsWafv2RuleGroupDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2RuleGroupDetailsOutputTypeDef",
+    {
+        "Capacity": int,
+        "Description": str,
+        "Id": str,
+        "Name": str,
+        "Arn": str,
+        "Rules": List[AwsWafv2RulesDetailsOutputTypeDef],
+        "Scope": str,
+        "VisibilityConfig": AwsWafv2VisibilityConfigDetailsTypeDef,
+    },
+    total=False,
+)
+
+AwsWafv2WebAclDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2WebAclDetailsOutputTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "ManagedbyFirewallManager": bool,
+        "Id": str,
+        "Capacity": int,
+        "CaptchaConfig": AwsWafv2WebAclCaptchaConfigDetailsTypeDef,
+        "DefaultAction": AwsWafv2WebAclActionDetailsOutputTypeDef,
+        "Description": str,
+        "Rules": List[AwsWafv2RulesDetailsOutputTypeDef],
+        "VisibilityConfig": AwsWafv2VisibilityConfigDetailsTypeDef,
+    },
+    total=False,
+)
+
 AwsWafv2RuleGroupDetailsTypeDef = TypedDict(
     "AwsWafv2RuleGroupDetailsTypeDef",
     {
         "Capacity": int,
         "Description": str,
         "Id": str,
         "Name": str,
@@ -9174,27 +12350,65 @@
         "Description": str,
         "Rules": Sequence[AwsWafv2RulesDetailsTypeDef],
         "VisibilityConfig": AwsWafv2VisibilityConfigDetailsTypeDef,
     },
     total=False,
 )
 
+ClassificationResultOutputTypeDef = TypedDict(
+    "ClassificationResultOutputTypeDef",
+    {
+        "MimeType": str,
+        "SizeClassified": int,
+        "AdditionalOccurrences": bool,
+        "Status": ClassificationStatusTypeDef,
+        "SensitiveData": List[SensitiveDataResultOutputTypeDef],
+        "CustomDataIdentifiers": CustomDataIdentifiersResultOutputTypeDef,
+    },
+    total=False,
+)
+
 ClassificationResultTypeDef = TypedDict(
     "ClassificationResultTypeDef",
     {
         "MimeType": str,
         "SizeClassified": int,
         "AdditionalOccurrences": bool,
         "Status": ClassificationStatusTypeDef,
         "SensitiveData": Sequence[SensitiveDataResultTypeDef],
         "CustomDataIdentifiers": CustomDataIdentifiersResultTypeDef,
     },
     total=False,
 )
 
+AwsNetworkFirewallFirewallPolicyDetailsOutputTypeDef = TypedDict(
+    "AwsNetworkFirewallFirewallPolicyDetailsOutputTypeDef",
+    {
+        "FirewallPolicy": FirewallPolicyDetailsOutputTypeDef,
+        "FirewallPolicyArn": str,
+        "FirewallPolicyId": str,
+        "FirewallPolicyName": str,
+        "Description": str,
+    },
+    total=False,
+)
+
+RuleGroupSourceOutputTypeDef = TypedDict(
+    "RuleGroupSourceOutputTypeDef",
+    {
+        "RulesSourceList": RuleGroupSourceListDetailsOutputTypeDef,
+        "RulesString": str,
+        "StatefulRules": List[RuleGroupSourceStatefulRulesDetailsOutputTypeDef],
+        "StatelessRulesAndCustomActions": (
+            RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef
+        ),
+    },
+    total=False,
+)
+
 AwsNetworkFirewallFirewallPolicyDetailsTypeDef = TypedDict(
     "AwsNetworkFirewallFirewallPolicyDetailsTypeDef",
     {
         "FirewallPolicy": FirewallPolicyDetailsTypeDef,
         "FirewallPolicyArn": str,
         "FirewallPolicyId": str,
         "FirewallPolicyName": str,
@@ -9212,14 +12426,36 @@
         "StatelessRulesAndCustomActions": (
             RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef
         ),
     },
     total=False,
 )
 
+AwsS3BucketDetailsOutputTypeDef = TypedDict(
+    "AwsS3BucketDetailsOutputTypeDef",
+    {
+        "OwnerId": str,
+        "OwnerName": str,
+        "OwnerAccountId": str,
+        "CreatedAt": str,
+        "ServerSideEncryptionConfiguration": (
+            AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef
+        ),
+        "BucketLifecycleConfiguration": AwsS3BucketBucketLifecycleConfigurationDetailsOutputTypeDef,
+        "PublicAccessBlockConfiguration": AwsS3AccountPublicAccessBlockDetailsTypeDef,
+        "AccessControlList": str,
+        "BucketLoggingConfiguration": AwsS3BucketLoggingConfigurationTypeDef,
+        "BucketWebsiteConfiguration": AwsS3BucketWebsiteConfigurationOutputTypeDef,
+        "BucketNotificationConfiguration": AwsS3BucketNotificationConfigurationOutputTypeDef,
+        "BucketVersioningConfiguration": AwsS3BucketBucketVersioningConfigurationTypeDef,
+        "ObjectLockConfiguration": AwsS3BucketObjectLockConfigurationTypeDef,
+    },
+    total=False,
+)
+
 AwsS3BucketDetailsTypeDef = TypedDict(
     "AwsS3BucketDetailsTypeDef",
     {
         "OwnerId": str,
         "OwnerName": str,
         "OwnerAccountId": str,
         "CreatedAt": str,
@@ -9232,46 +12468,174 @@
         "BucketNotificationConfiguration": AwsS3BucketNotificationConfigurationTypeDef,
         "BucketVersioningConfiguration": AwsS3BucketBucketVersioningConfigurationTypeDef,
         "ObjectLockConfiguration": AwsS3BucketObjectLockConfigurationTypeDef,
     },
     total=False,
 )
 
+DataClassificationDetailsOutputTypeDef = TypedDict(
+    "DataClassificationDetailsOutputTypeDef",
+    {
+        "DetailedResultsLocation": str,
+        "Result": ClassificationResultOutputTypeDef,
+    },
+    total=False,
+)
+
 DataClassificationDetailsTypeDef = TypedDict(
     "DataClassificationDetailsTypeDef",
     {
         "DetailedResultsLocation": str,
         "Result": ClassificationResultTypeDef,
     },
     total=False,
 )
 
+RuleGroupDetailsOutputTypeDef = TypedDict(
+    "RuleGroupDetailsOutputTypeDef",
+    {
+        "RuleVariables": RuleGroupVariablesOutputTypeDef,
+        "RulesSource": RuleGroupSourceOutputTypeDef,
+    },
+    total=False,
+)
+
 RuleGroupDetailsTypeDef = TypedDict(
     "RuleGroupDetailsTypeDef",
     {
         "RuleVariables": RuleGroupVariablesTypeDef,
         "RulesSource": RuleGroupSourceTypeDef,
     },
     total=False,
 )
 
+AwsNetworkFirewallRuleGroupDetailsOutputTypeDef = TypedDict(
+    "AwsNetworkFirewallRuleGroupDetailsOutputTypeDef",
+    {
+        "Capacity": int,
+        "Description": str,
+        "RuleGroup": RuleGroupDetailsOutputTypeDef,
+        "RuleGroupArn": str,
+        "RuleGroupId": str,
+        "RuleGroupName": str,
+        "Type": str,
+    },
+    total=False,
+)
+
 AwsNetworkFirewallRuleGroupDetailsTypeDef = TypedDict(
     "AwsNetworkFirewallRuleGroupDetailsTypeDef",
     {
         "Capacity": int,
         "Description": str,
         "RuleGroup": RuleGroupDetailsTypeDef,
         "RuleGroupArn": str,
         "RuleGroupId": str,
         "RuleGroupName": str,
         "Type": str,
     },
     total=False,
 )
 
+ResourceDetailsOutputTypeDef = TypedDict(
+    "ResourceDetailsOutputTypeDef",
+    {
+        "AwsAutoScalingAutoScalingGroup": AwsAutoScalingAutoScalingGroupDetailsOutputTypeDef,
+        "AwsCodeBuildProject": AwsCodeBuildProjectDetailsOutputTypeDef,
+        "AwsCloudFrontDistribution": AwsCloudFrontDistributionDetailsOutputTypeDef,
+        "AwsEc2Instance": AwsEc2InstanceDetailsOutputTypeDef,
+        "AwsEc2NetworkInterface": AwsEc2NetworkInterfaceDetailsOutputTypeDef,
+        "AwsEc2SecurityGroup": AwsEc2SecurityGroupDetailsOutputTypeDef,
+        "AwsEc2Volume": AwsEc2VolumeDetailsOutputTypeDef,
+        "AwsEc2Vpc": AwsEc2VpcDetailsOutputTypeDef,
+        "AwsEc2Eip": AwsEc2EipDetailsTypeDef,
+        "AwsEc2Subnet": AwsEc2SubnetDetailsOutputTypeDef,
+        "AwsEc2NetworkAcl": AwsEc2NetworkAclDetailsOutputTypeDef,
+        "AwsElbv2LoadBalancer": AwsElbv2LoadBalancerDetailsOutputTypeDef,
+        "AwsElasticBeanstalkEnvironment": AwsElasticBeanstalkEnvironmentDetailsOutputTypeDef,
+        "AwsElasticsearchDomain": AwsElasticsearchDomainDetailsOutputTypeDef,
+        "AwsS3Bucket": AwsS3BucketDetailsOutputTypeDef,
+        "AwsS3AccountPublicAccessBlock": AwsS3AccountPublicAccessBlockDetailsTypeDef,
+        "AwsS3Object": AwsS3ObjectDetailsTypeDef,
+        "AwsSecretsManagerSecret": AwsSecretsManagerSecretDetailsTypeDef,
+        "AwsIamAccessKey": AwsIamAccessKeyDetailsTypeDef,
+        "AwsIamUser": AwsIamUserDetailsOutputTypeDef,
+        "AwsIamPolicy": AwsIamPolicyDetailsOutputTypeDef,
+        "AwsApiGatewayV2Stage": AwsApiGatewayV2StageDetailsOutputTypeDef,
+        "AwsApiGatewayV2Api": AwsApiGatewayV2ApiDetailsOutputTypeDef,
+        "AwsDynamoDbTable": AwsDynamoDbTableDetailsOutputTypeDef,
+        "AwsApiGatewayStage": AwsApiGatewayStageDetailsOutputTypeDef,
+        "AwsApiGatewayRestApi": AwsApiGatewayRestApiDetailsOutputTypeDef,
+        "AwsCloudTrailTrail": AwsCloudTrailTrailDetailsTypeDef,
+        "AwsSsmPatchCompliance": AwsSsmPatchComplianceDetailsTypeDef,
+        "AwsCertificateManagerCertificate": AwsCertificateManagerCertificateDetailsOutputTypeDef,
+        "AwsRedshiftCluster": AwsRedshiftClusterDetailsOutputTypeDef,
+        "AwsElbLoadBalancer": AwsElbLoadBalancerDetailsOutputTypeDef,
+        "AwsIamGroup": AwsIamGroupDetailsOutputTypeDef,
+        "AwsIamRole": AwsIamRoleDetailsOutputTypeDef,
+        "AwsKmsKey": AwsKmsKeyDetailsTypeDef,
+        "AwsLambdaFunction": AwsLambdaFunctionDetailsOutputTypeDef,
+        "AwsLambdaLayerVersion": AwsLambdaLayerVersionDetailsOutputTypeDef,
+        "AwsRdsDbInstance": AwsRdsDbInstanceDetailsOutputTypeDef,
+        "AwsSnsTopic": AwsSnsTopicDetailsOutputTypeDef,
+        "AwsSqsQueue": AwsSqsQueueDetailsTypeDef,
+        "AwsWafWebAcl": AwsWafWebAclDetailsOutputTypeDef,
+        "AwsRdsDbSnapshot": AwsRdsDbSnapshotDetailsOutputTypeDef,
+        "AwsRdsDbClusterSnapshot": AwsRdsDbClusterSnapshotDetailsOutputTypeDef,
+        "AwsRdsDbCluster": AwsRdsDbClusterDetailsOutputTypeDef,
+        "AwsEcsCluster": AwsEcsClusterDetailsOutputTypeDef,
+        "AwsEcsContainer": AwsEcsContainerDetailsOutputTypeDef,
+        "AwsEcsTaskDefinition": AwsEcsTaskDefinitionDetailsOutputTypeDef,
+        "Container": ContainerDetailsOutputTypeDef,
+        "Other": Dict[str, str],
+        "AwsRdsEventSubscription": AwsRdsEventSubscriptionDetailsOutputTypeDef,
+        "AwsEcsService": AwsEcsServiceDetailsOutputTypeDef,
+        "AwsAutoScalingLaunchConfiguration": AwsAutoScalingLaunchConfigurationDetailsOutputTypeDef,
+        "AwsEc2VpnConnection": AwsEc2VpnConnectionDetailsOutputTypeDef,
+        "AwsEcrContainerImage": AwsEcrContainerImageDetailsOutputTypeDef,
+        "AwsOpenSearchServiceDomain": AwsOpenSearchServiceDomainDetailsOutputTypeDef,
+        "AwsEc2VpcEndpointService": AwsEc2VpcEndpointServiceDetailsOutputTypeDef,
+        "AwsXrayEncryptionConfig": AwsXrayEncryptionConfigDetailsTypeDef,
+        "AwsWafRateBasedRule": AwsWafRateBasedRuleDetailsOutputTypeDef,
+        "AwsWafRegionalRateBasedRule": AwsWafRegionalRateBasedRuleDetailsOutputTypeDef,
+        "AwsEcrRepository": AwsEcrRepositoryDetailsTypeDef,
+        "AwsEksCluster": AwsEksClusterDetailsOutputTypeDef,
+        "AwsNetworkFirewallFirewallPolicy": AwsNetworkFirewallFirewallPolicyDetailsOutputTypeDef,
+        "AwsNetworkFirewallFirewall": AwsNetworkFirewallFirewallDetailsOutputTypeDef,
+        "AwsNetworkFirewallRuleGroup": AwsNetworkFirewallRuleGroupDetailsOutputTypeDef,
+        "AwsRdsDbSecurityGroup": AwsRdsDbSecurityGroupDetailsOutputTypeDef,
+        "AwsKinesisStream": AwsKinesisStreamDetailsTypeDef,
+        "AwsEc2TransitGateway": AwsEc2TransitGatewayDetailsOutputTypeDef,
+        "AwsEfsAccessPoint": AwsEfsAccessPointDetailsOutputTypeDef,
+        "AwsCloudFormationStack": AwsCloudFormationStackDetailsOutputTypeDef,
+        "AwsCloudWatchAlarm": AwsCloudWatchAlarmDetailsOutputTypeDef,
+        "AwsEc2VpcPeeringConnection": AwsEc2VpcPeeringConnectionDetailsOutputTypeDef,
+        "AwsWafRegionalRuleGroup": AwsWafRegionalRuleGroupDetailsOutputTypeDef,
+        "AwsWafRegionalRule": AwsWafRegionalRuleDetailsOutputTypeDef,
+        "AwsWafRegionalWebAcl": AwsWafRegionalWebAclDetailsOutputTypeDef,
+        "AwsWafRule": AwsWafRuleDetailsOutputTypeDef,
+        "AwsWafRuleGroup": AwsWafRuleGroupDetailsOutputTypeDef,
+        "AwsEcsTask": AwsEcsTaskDetailsOutputTypeDef,
+        "AwsBackupBackupVault": AwsBackupBackupVaultDetailsOutputTypeDef,
+        "AwsBackupBackupPlan": AwsBackupBackupPlanDetailsOutputTypeDef,
+        "AwsBackupRecoveryPoint": AwsBackupRecoveryPointDetailsTypeDef,
+        "AwsEc2LaunchTemplate": AwsEc2LaunchTemplateDetailsOutputTypeDef,
+        "AwsSageMakerNotebookInstance": AwsSageMakerNotebookInstanceDetailsOutputTypeDef,
+        "AwsWafv2WebAcl": AwsWafv2WebAclDetailsOutputTypeDef,
+        "AwsWafv2RuleGroup": AwsWafv2RuleGroupDetailsOutputTypeDef,
+        "AwsEc2RouteTable": AwsEc2RouteTableDetailsOutputTypeDef,
+        "AwsAmazonMqBroker": AwsAmazonMqBrokerDetailsOutputTypeDef,
+        "AwsAppSyncGraphQlApi": AwsAppSyncGraphQlApiDetailsOutputTypeDef,
+        "AwsEventSchemasRegistry": AwsEventSchemasRegistryDetailsTypeDef,
+        "AwsGuardDutyDetector": AwsGuardDutyDetectorDetailsOutputTypeDef,
+        "AwsStepFunctionStateMachine": AwsStepFunctionStateMachineDetailsOutputTypeDef,
+    },
+    total=False,
+)
+
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "AwsAutoScalingAutoScalingGroup": AwsAutoScalingAutoScalingGroupDetailsTypeDef,
         "AwsCodeBuildProject": AwsCodeBuildProjectDetailsTypeDef,
         "AwsCloudFrontDistribution": AwsCloudFrontDistributionDetailsTypeDef,
         "AwsEc2Instance": AwsEc2InstanceDetailsTypeDef,
@@ -9360,14 +12724,39 @@
         "AwsEventSchemasRegistry": AwsEventSchemasRegistryDetailsTypeDef,
         "AwsGuardDutyDetector": AwsGuardDutyDetectorDetailsTypeDef,
         "AwsStepFunctionStateMachine": AwsStepFunctionStateMachineDetailsTypeDef,
     },
     total=False,
 )
 
+_RequiredResourceOutputTypeDef = TypedDict(
+    "_RequiredResourceOutputTypeDef",
+    {
+        "Type": str,
+        "Id": str,
+    },
+)
+_OptionalResourceOutputTypeDef = TypedDict(
+    "_OptionalResourceOutputTypeDef",
+    {
+        "Partition": PartitionType,
+        "Region": str,
+        "ResourceRole": str,
+        "Tags": Dict[str, str],
+        "DataClassification": DataClassificationDetailsOutputTypeDef,
+        "Details": ResourceDetailsOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class ResourceOutputTypeDef(_RequiredResourceOutputTypeDef, _OptionalResourceOutputTypeDef):
+    pass
+
+
 _RequiredResourceTypeDef = TypedDict(
     "_RequiredResourceTypeDef",
     {
         "Type": str,
         "Id": str,
     },
 )
@@ -9385,14 +12774,74 @@
 )
 
 
 class ResourceTypeDef(_RequiredResourceTypeDef, _OptionalResourceTypeDef):
     pass
 
 
+_RequiredAwsSecurityFindingOutputTypeDef = TypedDict(
+    "_RequiredAwsSecurityFindingOutputTypeDef",
+    {
+        "SchemaVersion": str,
+        "Id": str,
+        "ProductArn": str,
+        "GeneratorId": str,
+        "AwsAccountId": str,
+        "CreatedAt": str,
+        "UpdatedAt": str,
+        "Title": str,
+        "Description": str,
+        "Resources": List[ResourceOutputTypeDef],
+    },
+)
+_OptionalAwsSecurityFindingOutputTypeDef = TypedDict(
+    "_OptionalAwsSecurityFindingOutputTypeDef",
+    {
+        "ProductName": str,
+        "CompanyName": str,
+        "Region": str,
+        "Types": List[str],
+        "FirstObservedAt": str,
+        "LastObservedAt": str,
+        "Severity": SeverityTypeDef,
+        "Confidence": int,
+        "Criticality": int,
+        "Remediation": RemediationTypeDef,
+        "SourceUrl": str,
+        "ProductFields": Dict[str, str],
+        "UserDefinedFields": Dict[str, str],
+        "Malware": List[MalwareTypeDef],
+        "Network": NetworkTypeDef,
+        "NetworkPath": List[NetworkPathComponentOutputTypeDef],
+        "Process": ProcessDetailsTypeDef,
+        "Threats": List[ThreatOutputTypeDef],
+        "ThreatIntelIndicators": List[ThreatIntelIndicatorTypeDef],
+        "Compliance": ComplianceOutputTypeDef,
+        "VerificationState": VerificationStateType,
+        "WorkflowState": WorkflowStateType,
+        "Workflow": WorkflowTypeDef,
+        "RecordState": RecordStateType,
+        "RelatedFindings": List[RelatedFindingTypeDef],
+        "Note": NoteTypeDef,
+        "Vulnerabilities": List[VulnerabilityOutputTypeDef],
+        "PatchSummary": PatchSummaryTypeDef,
+        "Action": ActionOutputTypeDef,
+        "FindingProviderFields": FindingProviderFieldsOutputTypeDef,
+        "Sample": bool,
+    },
+    total=False,
+)
+
+
+class AwsSecurityFindingOutputTypeDef(
+    _RequiredAwsSecurityFindingOutputTypeDef, _OptionalAwsSecurityFindingOutputTypeDef
+):
+    pass
+
+
 _RequiredAwsSecurityFindingTypeDef = TypedDict(
     "_RequiredAwsSecurityFindingTypeDef",
     {
         "SchemaVersion": str,
         "Id": str,
         "ProductArn": str,
         "GeneratorId": str,
@@ -9445,22 +12894,23 @@
 
 class AwsSecurityFindingTypeDef(
     _RequiredAwsSecurityFindingTypeDef, _OptionalAwsSecurityFindingTypeDef
 ):
     pass
 
 
-BatchImportFindingsRequestRequestTypeDef = TypedDict(
-    "BatchImportFindingsRequestRequestTypeDef",
+GetFindingsResponseTypeDef = TypedDict(
+    "GetFindingsResponseTypeDef",
     {
-        "Findings": Sequence[AwsSecurityFindingTypeDef],
+        "Findings": List[AwsSecurityFindingOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetFindingsResponseTypeDef = TypedDict(
-    "GetFindingsResponseTypeDef",
+AwsSecurityFindingUnionTypeDef = Union[AwsSecurityFindingTypeDef, AwsSecurityFindingOutputTypeDef]
+BatchImportFindingsRequestRequestTypeDef = TypedDict(
+    "BatchImportFindingsRequestRequestTypeDef",
     {
-        "Findings": List[AwsSecurityFindingTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Findings": Sequence[AwsSecurityFindingUnionTypeDef],
     },
 )
```

### Comparing `types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub/type_defs.pyi` & `types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub/type_defs.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_securityhub.type_defs import AcceptAdministratorInvitationRequestRequestTypeDef
 
-    data: AcceptAdministratorInvitationRequestRequestTypeDef = {...}
+    data: AcceptAdministratorInvitationRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -60,93 +60,103 @@
 
 __all__ = (
     "AcceptAdministratorInvitationRequestRequestTypeDef",
     "AcceptInvitationRequestRequestTypeDef",
     "AccountDetailsTypeDef",
     "ActionLocalIpDetailsTypeDef",
     "ActionLocalPortDetailsTypeDef",
+    "DnsRequestActionTypeDef",
     "CityTypeDef",
     "CountryTypeDef",
     "GeoLocationTypeDef",
     "IpOrganizationDetailsTypeDef",
     "ActionRemotePortDetailsTypeDef",
     "ActionTargetTypeDef",
-    "DnsRequestActionTypeDef",
     "AdjustmentTypeDef",
     "AdminAccountTypeDef",
     "AssociatedStandardTypeDef",
     "AssociationStateDetailsTypeDef",
     "NoteUpdateTypeDef",
     "RelatedFindingTypeDef",
     "SeverityUpdateTypeDef",
     "WorkflowUpdateTypeDef",
     "MapFilterTypeDef",
     "NumberFilterTypeDef",
     "StringFilterTypeDef",
     "AutomationRulesMetadataTypeDef",
     "AvailabilityZoneTypeDef",
     "AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef",
-    "AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef",
+    "AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef",
     "AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef",
     "AwsAmazonMqBrokerUsersDetailsTypeDef",
+    "AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef",
     "AwsAmazonMqBrokerLogsPendingDetailsTypeDef",
     "AwsApiCallActionDomainDetailsTypeDef",
     "AwsApiGatewayAccessLogSettingsTypeDef",
+    "AwsApiGatewayCanarySettingsOutputTypeDef",
     "AwsApiGatewayCanarySettingsTypeDef",
+    "AwsApiGatewayEndpointConfigurationOutputTypeDef",
     "AwsApiGatewayEndpointConfigurationTypeDef",
     "AwsApiGatewayMethodSettingsTypeDef",
+    "AwsCorsConfigurationOutputTypeDef",
     "AwsCorsConfigurationTypeDef",
     "AwsApiGatewayV2RouteSettingsTypeDef",
     "AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef",
     "AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef",
     "AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef",
     "AwsAppSyncGraphQlApiLogConfigDetailsTypeDef",
     "AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef",
     "AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef",
     "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef",
     "AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef",
     "AwsAutoScalingLaunchConfigurationMetadataOptionsTypeDef",
+    "AwsBackupBackupPlanAdvancedBackupSettingsDetailsOutputTypeDef",
     "AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef",
     "AwsBackupBackupPlanLifecycleDetailsTypeDef",
+    "AwsBackupBackupVaultNotificationsDetailsOutputTypeDef",
     "AwsBackupBackupVaultNotificationsDetailsTypeDef",
     "AwsBackupRecoveryPointCalculatedLifecycleDetailsTypeDef",
     "AwsBackupRecoveryPointCreatedByDetailsTypeDef",
     "AwsBackupRecoveryPointLifecycleDetailsTypeDef",
     "AwsCertificateManagerCertificateExtendedKeyUsageTypeDef",
     "AwsCertificateManagerCertificateKeyUsageTypeDef",
     "AwsCertificateManagerCertificateOptionsTypeDef",
     "AwsCertificateManagerCertificateResourceRecordTypeDef",
     "AwsCloudFormationStackDriftInformationDetailsTypeDef",
     "AwsCloudFormationStackOutputsDetailsTypeDef",
     "AwsCloudFrontDistributionCacheBehaviorTypeDef",
     "AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef",
     "AwsCloudFrontDistributionLoggingTypeDef",
     "AwsCloudFrontDistributionViewerCertificateTypeDef",
+    "AwsCloudFrontDistributionOriginSslProtocolsOutputTypeDef",
     "AwsCloudFrontDistributionOriginSslProtocolsTypeDef",
+    "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesOutputTypeDef",
     "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef",
     "AwsCloudFrontDistributionOriginS3OriginConfigTypeDef",
     "AwsCloudTrailTrailDetailsTypeDef",
     "AwsCloudWatchAlarmDimensionsDetailsTypeDef",
     "AwsCodeBuildProjectArtifactsDetailsTypeDef",
     "AwsCodeBuildProjectSourceTypeDef",
+    "AwsCodeBuildProjectVpcConfigOutputTypeDef",
     "AwsCodeBuildProjectVpcConfigTypeDef",
     "AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef",
     "AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef",
     "AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef",
     "AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef",
     "AwsDynamoDbTableAttributeDefinitionTypeDef",
     "AwsDynamoDbTableBillingModeSummaryTypeDef",
     "AwsDynamoDbTableKeySchemaTypeDef",
     "AwsDynamoDbTableProvisionedThroughputTypeDef",
     "AwsDynamoDbTableRestoreSummaryTypeDef",
     "AwsDynamoDbTableSseDescriptionTypeDef",
     "AwsDynamoDbTableStreamSpecificationTypeDef",
+    "AwsDynamoDbTableProjectionOutputTypeDef",
     "AwsDynamoDbTableProjectionTypeDef",
     "AwsDynamoDbTableProvisionedThroughputOverrideTypeDef",
     "AwsEc2EipDetailsTypeDef",
     "AwsEc2InstanceMetadataOptionsTypeDef",
     "AwsEc2InstanceMonitoringDetailsTypeDef",
     "AwsEc2InstanceNetworkInterfacesDetailsTypeDef",
     "AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef",
@@ -187,86 +197,101 @@
     "PropagatingVgwSetDetailsTypeDef",
     "RouteSetDetailsTypeDef",
     "AwsEc2SecurityGroupIpRangeTypeDef",
     "AwsEc2SecurityGroupIpv6RangeTypeDef",
     "AwsEc2SecurityGroupPrefixListIdTypeDef",
     "AwsEc2SecurityGroupUserIdGroupPairTypeDef",
     "Ipv6CidrBlockAssociationTypeDef",
+    "AwsEc2TransitGatewayDetailsOutputTypeDef",
     "AwsEc2TransitGatewayDetailsTypeDef",
     "AwsEc2VolumeAttachmentTypeDef",
     "CidrBlockAssociationTypeDef",
     "AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef",
     "AwsEc2VpcPeeringConnectionStatusDetailsTypeDef",
     "VpcInfoCidrBlockSetDetailsTypeDef",
     "VpcInfoIpv6CidrBlockSetDetailsTypeDef",
     "VpcInfoPeeringOptionsDetailsTypeDef",
     "AwsEc2VpnConnectionRoutesDetailsTypeDef",
     "AwsEc2VpnConnectionVgwTelemetryDetailsTypeDef",
+    "AwsEc2VpnConnectionOptionsTunnelOptionsDetailsOutputTypeDef",
     "AwsEc2VpnConnectionOptionsTunnelOptionsDetailsTypeDef",
+    "AwsEcrContainerImageDetailsOutputTypeDef",
     "AwsEcrContainerImageDetailsTypeDef",
     "AwsEcrRepositoryImageScanningConfigurationDetailsTypeDef",
     "AwsEcrRepositoryLifecyclePolicyDetailsTypeDef",
     "AwsEcsClusterClusterSettingsDetailsTypeDef",
     "AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef",
     "AwsEcsClusterDefaultCapacityProviderStrategyDetailsTypeDef",
     "AwsMountPointTypeDef",
     "AwsEcsServiceCapacityProviderStrategyDetailsTypeDef",
     "AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef",
     "AwsEcsServiceDeploymentControllerDetailsTypeDef",
     "AwsEcsServiceLoadBalancersDetailsTypeDef",
     "AwsEcsServicePlacementConstraintsDetailsTypeDef",
     "AwsEcsServicePlacementStrategiesDetailsTypeDef",
     "AwsEcsServiceServiceRegistriesDetailsTypeDef",
+    "AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsOutputTypeDef",
     "AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsOutputTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef",
     "AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef",
     "AwsEcsTaskDefinitionPlacementConstraintsDetailsTypeDef",
     "AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef",
-    "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef",
+    "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionVolumesHostDetailsTypeDef",
+    "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef",
     "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef",
     "AwsEcsTaskVolumeHostDetailsTypeDef",
+    "AwsEfsAccessPointPosixUserDetailsOutputTypeDef",
     "AwsEfsAccessPointPosixUserDetailsTypeDef",
     "AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef",
+    "AwsEksClusterResourcesVpcConfigDetailsOutputTypeDef",
     "AwsEksClusterResourcesVpcConfigDetailsTypeDef",
+    "AwsEksClusterLoggingClusterLoggingDetailsOutputTypeDef",
     "AwsEksClusterLoggingClusterLoggingDetailsTypeDef",
     "AwsElasticBeanstalkEnvironmentEnvironmentLinkTypeDef",
     "AwsElasticBeanstalkEnvironmentOptionSettingTypeDef",
     "AwsElasticBeanstalkEnvironmentTierTypeDef",
     "AwsElasticsearchDomainDomainEndpointOptionsTypeDef",
     "AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef",
     "AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef",
     "AwsElasticsearchDomainServiceSoftwareOptionsTypeDef",
+    "AwsElasticsearchDomainVPCOptionsOutputTypeDef",
     "AwsElasticsearchDomainVPCOptionsTypeDef",
     "AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef",
     "AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef",
     "AwsElbAppCookieStickinessPolicyTypeDef",
     "AwsElbLbCookieStickinessPolicyTypeDef",
     "AwsElbLoadBalancerAccessLogTypeDef",
     "AwsElbLoadBalancerAdditionalAttributeTypeDef",
     "AwsElbLoadBalancerConnectionDrainingTypeDef",
     "AwsElbLoadBalancerConnectionSettingsTypeDef",
     "AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef",
+    "AwsElbLoadBalancerBackendServerDescriptionOutputTypeDef",
     "AwsElbLoadBalancerBackendServerDescriptionTypeDef",
     "AwsElbLoadBalancerHealthCheckTypeDef",
     "AwsElbLoadBalancerInstanceTypeDef",
     "AwsElbLoadBalancerSourceSecurityGroupTypeDef",
     "AwsElbLoadBalancerListenerTypeDef",
     "AwsElbv2LoadBalancerAttributeTypeDef",
     "LoadBalancerStateTypeDef",
@@ -289,42 +314,48 @@
     "AwsIamUserPolicyTypeDef",
     "AwsKinesisStreamStreamEncryptionDetailsTypeDef",
     "AwsKmsKeyDetailsTypeDef",
     "AwsLambdaFunctionCodeTypeDef",
     "AwsLambdaFunctionDeadLetterConfigTypeDef",
     "AwsLambdaFunctionLayerTypeDef",
     "AwsLambdaFunctionTracingConfigTypeDef",
+    "AwsLambdaFunctionVpcConfigOutputTypeDef",
     "AwsLambdaFunctionVpcConfigTypeDef",
     "AwsLambdaFunctionEnvironmentErrorTypeDef",
+    "AwsLambdaLayerVersionDetailsOutputTypeDef",
     "AwsLambdaLayerVersionDetailsTypeDef",
     "AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef",
     "AwsOpenSearchServiceDomainMasterUserOptionsDetailsTypeDef",
     "AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef",
     "AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef",
     "AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsTypeDef",
     "AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsTypeDef",
     "AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsTypeDef",
+    "AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef",
     "AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef",
     "AwsOpenSearchServiceDomainLogPublishingOptionTypeDef",
     "AwsRdsDbClusterAssociatedRoleTypeDef",
     "AwsRdsDbClusterMemberTypeDef",
     "AwsRdsDbClusterOptionGroupMembershipTypeDef",
     "AwsRdsDbDomainMembershipTypeDef",
     "AwsRdsDbInstanceVpcSecurityGroupTypeDef",
+    "AwsRdsDbClusterSnapshotDetailsOutputTypeDef",
     "AwsRdsDbClusterSnapshotDetailsTypeDef",
     "AwsRdsDbInstanceAssociatedRoleTypeDef",
     "AwsRdsDbInstanceEndpointTypeDef",
     "AwsRdsDbOptionGroupMembershipTypeDef",
     "AwsRdsDbParameterGroupTypeDef",
     "AwsRdsDbProcessorFeatureTypeDef",
     "AwsRdsDbStatusInfoTypeDef",
+    "AwsRdsPendingCloudWatchLogsExportsOutputTypeDef",
     "AwsRdsPendingCloudWatchLogsExportsTypeDef",
     "AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef",
     "AwsRdsDbSecurityGroupIpRangeTypeDef",
     "AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef",
+    "AwsRdsEventSubscriptionDetailsOutputTypeDef",
     "AwsRdsEventSubscriptionDetailsTypeDef",
     "AwsRedshiftClusterClusterNodeTypeDef",
     "AwsRedshiftClusterClusterParameterStatusTypeDef",
     "AwsRedshiftClusterClusterSecurityGroupTypeDef",
     "AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef",
     "AwsRedshiftClusterDeferredMaintenanceWindowTypeDef",
     "AwsRedshiftClusterElasticIpStatusTypeDef",
@@ -381,14 +412,15 @@
     "WafExcludedRuleTypeDef",
     "WafOverrideActionTypeDef",
     "AwsWafv2CustomHttpHeaderTypeDef",
     "AwsWafv2VisibilityConfigDetailsTypeDef",
     "AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef",
     "AwsXrayEncryptionConfigDetailsTypeDef",
     "BatchDeleteAutomationRulesRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "UnprocessedAutomationRuleTypeDef",
     "BatchDisableStandardsRequestRequestTypeDef",
     "StandardsSubscriptionRequestTypeDef",
     "BatchGetAutomationRulesRequestRequestTypeDef",
     "BatchGetSecurityControlsRequestRequestTypeDef",
     "SecurityControlTypeDef",
     "UnprocessedSecurityControlTypeDef",
@@ -397,396 +429,571 @@
     "ImportFindingsErrorTypeDef",
     "StandardsControlAssociationUpdateTypeDef",
     "CellTypeDef",
     "ClassificationStatusTypeDef",
     "StatusReasonTypeDef",
     "VolumeMountTypeDef",
     "CreateActionTargetRequestRequestTypeDef",
-    "CreateActionTargetResponseTypeDef",
-    "CreateAutomationRuleResponseTypeDef",
     "CreateFindingAggregatorRequestRequestTypeDef",
-    "CreateFindingAggregatorResponseTypeDef",
-    "CreateInsightResponseTypeDef",
     "ResultTypeDef",
     "DateRangeTypeDef",
     "DeclineInvitationsRequestRequestTypeDef",
     "DeleteActionTargetRequestRequestTypeDef",
-    "DeleteActionTargetResponseTypeDef",
     "DeleteFindingAggregatorRequestRequestTypeDef",
     "DeleteInsightRequestRequestTypeDef",
-    "DeleteInsightResponseTypeDef",
     "DeleteInvitationsRequestRequestTypeDef",
     "DeleteMembersRequestRequestTypeDef",
-    "DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeActionTargetsRequestRequestTypeDef",
     "DescribeHubRequestRequestTypeDef",
-    "DescribeHubResponseTypeDef",
-    "DescribeOrganizationConfigurationResponseTypeDef",
-    "DescribeProductsRequestDescribeProductsPaginateTypeDef",
     "DescribeProductsRequestRequestTypeDef",
     "ProductTypeDef",
-    "DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef",
     "DescribeStandardsControlsRequestRequestTypeDef",
     "StandardsControlTypeDef",
-    "DescribeStandardsRequestDescribeStandardsPaginateTypeDef",
     "DescribeStandardsRequestRequestTypeDef",
     "DisableImportFindingsForProductRequestRequestTypeDef",
     "DisableOrganizationAdminAccountRequestRequestTypeDef",
     "DisassociateMembersRequestRequestTypeDef",
     "EnableImportFindingsForProductRequestRequestTypeDef",
-    "EnableImportFindingsForProductResponseTypeDef",
     "EnableOrganizationAdminAccountRequestRequestTypeDef",
     "EnableSecurityHubRequestRequestTypeDef",
     "FilePathsTypeDef",
     "FindingAggregatorTypeDef",
     "FindingHistoryUpdateSourceTypeDef",
     "FindingHistoryUpdateTypeDef",
     "FindingProviderSeverityTypeDef",
     "FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef",
     "FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef",
     "InvitationTypeDef",
-    "GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef",
     "GetEnabledStandardsRequestRequestTypeDef",
     "GetFindingAggregatorRequestRequestTypeDef",
-    "GetFindingAggregatorResponseTypeDef",
+    "TimestampTypeDef",
     "SortCriterionTypeDef",
     "GetInsightResultsRequestRequestTypeDef",
-    "GetInsightsRequestGetInsightsPaginateTypeDef",
     "GetInsightsRequestRequestTypeDef",
-    "GetInvitationsCountResponseTypeDef",
     "GetMembersRequestRequestTypeDef",
     "MemberTypeDef",
     "InsightResultValueTypeDef",
     "InviteMembersRequestRequestTypeDef",
     "ListAutomationRulesRequestRequestTypeDef",
-    "ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef",
     "ListEnabledProductsForImportRequestRequestTypeDef",
-    "ListEnabledProductsForImportResponseTypeDef",
-    "ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef",
     "ListFindingAggregatorsRequestRequestTypeDef",
-    "ListInvitationsRequestListInvitationsPaginateTypeDef",
     "ListInvitationsRequestRequestTypeDef",
-    "ListMembersRequestListMembersPaginateTypeDef",
     "ListMembersRequestRequestTypeDef",
-    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
-    "ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef",
     "ListSecurityControlDefinitionsRequestRequestTypeDef",
     "SecurityControlDefinitionTypeDef",
-    "ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef",
     "ListStandardsControlAssociationsRequestRequestTypeDef",
     "StandardsControlAssociationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "PortRangeTypeDef",
     "RangeTypeDef",
     "RecordTypeDef",
-    "PaginatorConfigTypeDef",
     "RecommendationTypeDef",
-    "ResponseMetadataTypeDef",
+    "RuleGroupSourceListDetailsOutputTypeDef",
     "RuleGroupSourceListDetailsTypeDef",
     "RuleGroupSourceStatefulRulesHeaderDetailsTypeDef",
+    "RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef",
     "RuleGroupSourceStatefulRulesOptionsDetailsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef",
+    "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef",
+    "RuleGroupVariablesIpSetsDetailsOutputTypeDef",
     "RuleGroupVariablesIpSetsDetailsTypeDef",
+    "RuleGroupVariablesPortSetsDetailsOutputTypeDef",
     "RuleGroupVariablesPortSetsDetailsTypeDef",
     "SoftwarePackageTypeDef",
     "StandardsManagedByTypeDef",
     "StandardsStatusReasonTypeDef",
     "StatelessCustomPublishMetricActionDimensionTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateActionTargetRequestRequestTypeDef",
     "UpdateFindingAggregatorRequestRequestTypeDef",
-    "UpdateFindingAggregatorResponseTypeDef",
     "UpdateOrganizationConfigurationRequestRequestTypeDef",
     "UpdateSecurityHubConfigurationRequestRequestTypeDef",
     "UpdateStandardsControlRequestRequestTypeDef",
     "VulnerabilityVendorTypeDef",
     "CreateMembersRequestRequestTypeDef",
     "ActionRemoteIpDetailsTypeDef",
-    "DescribeActionTargetsResponseTypeDef",
+    "CvssOutputTypeDef",
     "CvssTypeDef",
-    "ListOrganizationAdminAccountsResponseTypeDef",
     "AssociationSetDetailsTypeDef",
+    "AutomationRulesFindingFieldsUpdateOutputTypeDef",
     "AutomationRulesFindingFieldsUpdateTypeDef",
-    "ListAutomationRulesResponseTypeDef",
     "AwsAmazonMqBrokerLogsDetailsTypeDef",
+    "AwsApiGatewayRestApiDetailsOutputTypeDef",
     "AwsApiGatewayRestApiDetailsTypeDef",
+    "AwsApiGatewayStageDetailsOutputTypeDef",
     "AwsApiGatewayStageDetailsTypeDef",
+    "AwsApiGatewayV2ApiDetailsOutputTypeDef",
     "AwsApiGatewayV2ApiDetailsTypeDef",
+    "AwsApiGatewayV2StageDetailsOutputTypeDef",
     "AwsApiGatewayV2StageDetailsTypeDef",
     "AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef",
+    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef",
     "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef",
     "AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef",
+    "AwsBackupBackupVaultDetailsOutputTypeDef",
     "AwsBackupBackupVaultDetailsTypeDef",
     "AwsBackupRecoveryPointDetailsTypeDef",
+    "AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef",
     "AwsCertificateManagerCertificateDomainValidationOptionTypeDef",
+    "AwsCloudFormationStackDetailsOutputTypeDef",
     "AwsCloudFormationStackDetailsTypeDef",
+    "AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef",
     "AwsCloudFrontDistributionCacheBehaviorsTypeDef",
+    "AwsCloudFrontDistributionOriginCustomOriginConfigOutputTypeDef",
     "AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef",
+    "AwsCloudFrontDistributionOriginGroupFailoverOutputTypeDef",
     "AwsCloudFrontDistributionOriginGroupFailoverTypeDef",
+    "AwsCloudWatchAlarmDetailsOutputTypeDef",
     "AwsCloudWatchAlarmDetailsTypeDef",
+    "AwsCodeBuildProjectEnvironmentOutputTypeDef",
     "AwsCodeBuildProjectEnvironmentTypeDef",
     "AwsCodeBuildProjectLogsConfigDetailsTypeDef",
+    "AwsDynamoDbTableGlobalSecondaryIndexOutputTypeDef",
+    "AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef",
     "AwsDynamoDbTableGlobalSecondaryIndexTypeDef",
     "AwsDynamoDbTableLocalSecondaryIndexTypeDef",
     "AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef",
+    "AwsEc2InstanceDetailsOutputTypeDef",
     "AwsEc2InstanceDetailsTypeDef",
     "AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef",
     "AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef",
     "AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef",
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef",
     "AwsEc2NetworkAclEntryTypeDef",
+    "AwsEc2NetworkInterfaceDetailsOutputTypeDef",
     "AwsEc2NetworkInterfaceDetailsTypeDef",
+    "AwsEc2SecurityGroupIpPermissionOutputTypeDef",
     "AwsEc2SecurityGroupIpPermissionTypeDef",
+    "AwsEc2SubnetDetailsOutputTypeDef",
     "AwsEc2SubnetDetailsTypeDef",
+    "AwsEc2VolumeDetailsOutputTypeDef",
     "AwsEc2VolumeDetailsTypeDef",
+    "AwsEc2VpcDetailsOutputTypeDef",
     "AwsEc2VpcDetailsTypeDef",
+    "AwsEc2VpcEndpointServiceDetailsOutputTypeDef",
     "AwsEc2VpcEndpointServiceDetailsTypeDef",
+    "AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef",
     "AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef",
+    "AwsEc2VpnConnectionOptionsDetailsOutputTypeDef",
     "AwsEc2VpnConnectionOptionsDetailsTypeDef",
     "AwsEcrRepositoryDetailsTypeDef",
     "AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef",
+    "AwsEcsContainerDetailsOutputTypeDef",
     "AwsEcsContainerDetailsTypeDef",
     "AwsEcsServiceDeploymentConfigurationDetailsTypeDef",
+    "AwsEcsServiceNetworkConfigurationDetailsOutputTypeDef",
     "AwsEcsServiceNetworkConfigurationDetailsTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef",
+    "AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionProxyConfigurationDetailsTypeDef",
     "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef",
     "AwsEcsTaskVolumeDetailsTypeDef",
     "AwsEfsAccessPointRootDirectoryDetailsTypeDef",
+    "AwsEksClusterLoggingDetailsOutputTypeDef",
     "AwsEksClusterLoggingDetailsTypeDef",
+    "AwsElasticBeanstalkEnvironmentDetailsOutputTypeDef",
     "AwsElasticBeanstalkEnvironmentDetailsTypeDef",
     "AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef",
     "AwsElasticsearchDomainLogPublishingOptionsTypeDef",
+    "AwsElbLoadBalancerPoliciesOutputTypeDef",
     "AwsElbLoadBalancerPoliciesTypeDef",
+    "AwsElbLoadBalancerAttributesOutputTypeDef",
     "AwsElbLoadBalancerAttributesTypeDef",
+    "AwsElbLoadBalancerListenerDescriptionOutputTypeDef",
     "AwsElbLoadBalancerListenerDescriptionTypeDef",
+    "AwsElbv2LoadBalancerDetailsOutputTypeDef",
     "AwsElbv2LoadBalancerDetailsTypeDef",
     "AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef",
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef",
     "AwsIamAccessKeySessionContextTypeDef",
+    "AwsIamGroupDetailsOutputTypeDef",
     "AwsIamGroupDetailsTypeDef",
+    "AwsIamInstanceProfileOutputTypeDef",
     "AwsIamInstanceProfileTypeDef",
+    "AwsIamPolicyDetailsOutputTypeDef",
     "AwsIamPolicyDetailsTypeDef",
+    "AwsIamUserDetailsOutputTypeDef",
     "AwsIamUserDetailsTypeDef",
     "AwsKinesisStreamDetailsTypeDef",
+    "AwsLambdaFunctionEnvironmentOutputTypeDef",
     "AwsLambdaFunctionEnvironmentTypeDef",
+    "AwsNetworkFirewallFirewallDetailsOutputTypeDef",
     "AwsNetworkFirewallFirewallDetailsTypeDef",
     "AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef",
     "AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef",
     "AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef",
+    "AwsRdsDbClusterDetailsOutputTypeDef",
     "AwsRdsDbClusterDetailsTypeDef",
+    "AwsRdsDbSnapshotDetailsOutputTypeDef",
     "AwsRdsDbSnapshotDetailsTypeDef",
+    "AwsRdsDbPendingModifiedValuesOutputTypeDef",
     "AwsRdsDbPendingModifiedValuesTypeDef",
+    "AwsRdsDbSecurityGroupDetailsOutputTypeDef",
     "AwsRdsDbSecurityGroupDetailsTypeDef",
     "AwsRdsDbSubnetGroupSubnetTypeDef",
+    "AwsRedshiftClusterClusterParameterGroupOutputTypeDef",
     "AwsRedshiftClusterClusterParameterGroupTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef",
+    "AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef",
     "AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef",
     "AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef",
     "AwsS3BucketServerSideEncryptionRuleTypeDef",
     "AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef",
+    "AwsSageMakerNotebookInstanceDetailsOutputTypeDef",
     "AwsSageMakerNotebookInstanceDetailsTypeDef",
     "AwsSecretsManagerSecretDetailsTypeDef",
     "BatchUpdateFindingsRequestRequestTypeDef",
     "BatchUpdateFindingsUnprocessedFindingTypeDef",
-    "GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
-    "GetFindingHistoryRequestRequestTypeDef",
+    "AwsSnsTopicDetailsOutputTypeDef",
     "AwsSnsTopicDetailsTypeDef",
     "AwsSsmPatchTypeDef",
     "AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef",
+    "AwsWafRateBasedRuleDetailsOutputTypeDef",
     "AwsWafRateBasedRuleDetailsTypeDef",
+    "AwsWafRegionalRateBasedRuleDetailsOutputTypeDef",
     "AwsWafRegionalRateBasedRuleDetailsTypeDef",
+    "AwsWafRegionalRuleDetailsOutputTypeDef",
     "AwsWafRegionalRuleDetailsTypeDef",
     "AwsWafRegionalRuleGroupRulesDetailsTypeDef",
     "AwsWafRegionalWebAclRulesListDetailsTypeDef",
+    "AwsWafRuleDetailsOutputTypeDef",
     "AwsWafRuleDetailsTypeDef",
     "AwsWafRuleGroupRulesDetailsTypeDef",
+    "AwsWafWebAclRuleOutputTypeDef",
     "AwsWafWebAclRuleTypeDef",
+    "AwsWafv2CustomRequestHandlingDetailsOutputTypeDef",
     "AwsWafv2CustomRequestHandlingDetailsTypeDef",
+    "AwsWafv2CustomResponseDetailsOutputTypeDef",
     "AwsWafv2CustomResponseDetailsTypeDef",
     "AwsWafv2WebAclCaptchaConfigDetailsTypeDef",
+    "CreateActionTargetResponseTypeDef",
+    "CreateAutomationRuleResponseTypeDef",
+    "CreateFindingAggregatorResponseTypeDef",
+    "CreateInsightResponseTypeDef",
+    "DeleteActionTargetResponseTypeDef",
+    "DeleteInsightResponseTypeDef",
+    "DescribeActionTargetsResponseTypeDef",
+    "DescribeHubResponseTypeDef",
+    "DescribeOrganizationConfigurationResponseTypeDef",
+    "EnableImportFindingsForProductResponseTypeDef",
+    "GetFindingAggregatorResponseTypeDef",
+    "GetInvitationsCountResponseTypeDef",
+    "ListAutomationRulesResponseTypeDef",
+    "ListEnabledProductsForImportResponseTypeDef",
+    "ListOrganizationAdminAccountsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateFindingAggregatorResponseTypeDef",
     "BatchDeleteAutomationRulesResponseTypeDef",
     "BatchUpdateAutomationRulesResponseTypeDef",
     "BatchEnableStandardsRequestRequestTypeDef",
     "BatchGetSecurityControlsResponseTypeDef",
     "BatchGetStandardsControlAssociationsRequestRequestTypeDef",
     "UnprocessedStandardsControlAssociationTypeDef",
     "BatchImportFindingsResponseTypeDef",
     "BatchUpdateStandardsControlAssociationsRequestRequestTypeDef",
     "UnprocessedStandardsControlAssociationUpdateTypeDef",
+    "ComplianceOutputTypeDef",
     "ComplianceTypeDef",
+    "ContainerDetailsOutputTypeDef",
     "ContainerDetailsTypeDef",
     "CreateMembersResponseTypeDef",
     "DeclineInvitationsResponseTypeDef",
     "DeleteInvitationsResponseTypeDef",
     "DeleteMembersResponseTypeDef",
     "InviteMembersResponseTypeDef",
     "DateFilterTypeDef",
+    "DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef",
+    "DescribeProductsRequestDescribeProductsPaginateTypeDef",
+    "DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef",
+    "DescribeStandardsRequestDescribeStandardsPaginateTypeDef",
+    "GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef",
+    "GetInsightsRequestGetInsightsPaginateTypeDef",
+    "ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef",
+    "ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef",
+    "ListInvitationsRequestListInvitationsPaginateTypeDef",
+    "ListMembersRequestListMembersPaginateTypeDef",
+    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
+    "ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef",
+    "ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef",
     "DescribeProductsResponseTypeDef",
     "DescribeStandardsControlsResponseTypeDef",
+    "ThreatOutputTypeDef",
     "ThreatTypeDef",
     "ListFindingAggregatorsResponseTypeDef",
     "FindingHistoryRecordTypeDef",
+    "FindingProviderFieldsOutputTypeDef",
     "FindingProviderFieldsTypeDef",
     "GetAdministratorAccountResponseTypeDef",
     "GetMasterAccountResponseTypeDef",
     "ListInvitationsResponseTypeDef",
+    "GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
+    "GetFindingHistoryRequestRequestTypeDef",
     "GetMembersResponseTypeDef",
     "ListMembersResponseTypeDef",
     "InsightResultsTypeDef",
     "ListSecurityControlDefinitionsResponseTypeDef",
     "ListStandardsControlAssociationsResponseTypeDef",
+    "NetworkPathComponentDetailsOutputTypeDef",
     "NetworkPathComponentDetailsTypeDef",
     "NetworkTypeDef",
     "PageTypeDef",
     "RemediationTypeDef",
+    "RuleGroupSourceStatefulRulesDetailsOutputTypeDef",
     "RuleGroupSourceStatefulRulesDetailsTypeDef",
+    "RuleGroupSourceStatelessRuleMatchAttributesOutputTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesTypeDef",
+    "RuleGroupVariablesOutputTypeDef",
     "RuleGroupVariablesTypeDef",
     "StandardTypeDef",
     "StandardsSubscriptionTypeDef",
+    "StatelessCustomPublishMetricActionOutputTypeDef",
     "StatelessCustomPublishMetricActionTypeDef",
+    "AwsApiCallActionOutputTypeDef",
     "AwsApiCallActionTypeDef",
     "NetworkConnectionActionTypeDef",
     "PortProbeDetailTypeDef",
+    "VulnerabilityOutputTypeDef",
     "VulnerabilityTypeDef",
+    "AwsEc2RouteTableDetailsOutputTypeDef",
     "AwsEc2RouteTableDetailsTypeDef",
+    "AutomationRulesActionOutputTypeDef",
     "AutomationRulesActionTypeDef",
+    "AwsAmazonMqBrokerDetailsOutputTypeDef",
     "AwsAmazonMqBrokerDetailsTypeDef",
+    "AwsAppSyncGraphQlApiDetailsOutputTypeDef",
     "AwsAppSyncGraphQlApiDetailsTypeDef",
+    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef",
+    "AwsAutoScalingLaunchConfigurationDetailsOutputTypeDef",
     "AwsAutoScalingLaunchConfigurationDetailsTypeDef",
+    "AwsBackupBackupPlanRuleDetailsOutputTypeDef",
     "AwsBackupBackupPlanRuleDetailsTypeDef",
+    "AwsCertificateManagerCertificateRenewalSummaryOutputTypeDef",
     "AwsCertificateManagerCertificateRenewalSummaryTypeDef",
+    "AwsCloudFrontDistributionOriginItemOutputTypeDef",
     "AwsCloudFrontDistributionOriginItemTypeDef",
+    "AwsCloudFrontDistributionOriginGroupOutputTypeDef",
     "AwsCloudFrontDistributionOriginGroupTypeDef",
+    "AwsCodeBuildProjectDetailsOutputTypeDef",
     "AwsCodeBuildProjectDetailsTypeDef",
+    "AwsDynamoDbTableReplicaOutputTypeDef",
     "AwsDynamoDbTableReplicaTypeDef",
+    "AwsEc2LaunchTemplateDataDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataDetailsTypeDef",
+    "AwsEc2NetworkAclDetailsOutputTypeDef",
     "AwsEc2NetworkAclDetailsTypeDef",
+    "AwsEc2SecurityGroupDetailsOutputTypeDef",
     "AwsEc2SecurityGroupDetailsTypeDef",
+    "AwsEc2VpcPeeringConnectionDetailsOutputTypeDef",
     "AwsEc2VpcPeeringConnectionDetailsTypeDef",
+    "AwsEc2VpnConnectionDetailsOutputTypeDef",
     "AwsEc2VpnConnectionDetailsTypeDef",
     "AwsEcsClusterConfigurationDetailsTypeDef",
+    "AwsEcsServiceDetailsOutputTypeDef",
     "AwsEcsServiceDetailsTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef",
+    "AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionVolumesDetailsTypeDef",
+    "AwsEcsTaskDetailsOutputTypeDef",
     "AwsEcsTaskDetailsTypeDef",
+    "AwsEfsAccessPointDetailsOutputTypeDef",
     "AwsEfsAccessPointDetailsTypeDef",
+    "AwsEksClusterDetailsOutputTypeDef",
     "AwsEksClusterDetailsTypeDef",
+    "AwsElasticsearchDomainDetailsOutputTypeDef",
     "AwsElasticsearchDomainDetailsTypeDef",
+    "AwsElbLoadBalancerDetailsOutputTypeDef",
     "AwsElbLoadBalancerDetailsTypeDef",
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef",
     "AwsIamAccessKeyDetailsTypeDef",
+    "AwsIamRoleDetailsOutputTypeDef",
     "AwsIamRoleDetailsTypeDef",
+    "AwsLambdaFunctionDetailsOutputTypeDef",
     "AwsLambdaFunctionDetailsTypeDef",
+    "AwsOpenSearchServiceDomainDetailsOutputTypeDef",
     "AwsOpenSearchServiceDomainDetailsTypeDef",
+    "AwsRdsDbSubnetGroupOutputTypeDef",
     "AwsRdsDbSubnetGroupTypeDef",
+    "AwsRedshiftClusterDetailsOutputTypeDef",
     "AwsRedshiftClusterDetailsTypeDef",
+    "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef",
+    "AwsS3BucketNotificationConfigurationFilterOutputTypeDef",
     "AwsS3BucketNotificationConfigurationFilterTypeDef",
     "AwsS3BucketObjectLockConfigurationTypeDef",
+    "AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef",
     "AwsS3BucketServerSideEncryptionConfigurationTypeDef",
+    "AwsS3BucketWebsiteConfigurationOutputTypeDef",
     "AwsS3BucketWebsiteConfigurationTypeDef",
     "BatchUpdateFindingsResponseTypeDef",
     "AwsSsmPatchComplianceDetailsTypeDef",
+    "AwsStepFunctionStateMachineLoggingConfigurationDetailsOutputTypeDef",
     "AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef",
+    "AwsWafRegionalRuleGroupDetailsOutputTypeDef",
     "AwsWafRegionalRuleGroupDetailsTypeDef",
+    "AwsWafRegionalWebAclDetailsOutputTypeDef",
     "AwsWafRegionalWebAclDetailsTypeDef",
+    "AwsWafRuleGroupDetailsOutputTypeDef",
     "AwsWafRuleGroupDetailsTypeDef",
+    "AwsWafWebAclDetailsOutputTypeDef",
     "AwsWafWebAclDetailsTypeDef",
+    "AwsWafv2ActionAllowDetailsOutputTypeDef",
+    "AwsWafv2RulesActionCaptchaDetailsOutputTypeDef",
+    "AwsWafv2RulesActionCountDetailsOutputTypeDef",
     "AwsWafv2ActionAllowDetailsTypeDef",
     "AwsWafv2RulesActionCaptchaDetailsTypeDef",
     "AwsWafv2RulesActionCountDetailsTypeDef",
+    "AwsWafv2ActionBlockDetailsOutputTypeDef",
     "AwsWafv2ActionBlockDetailsTypeDef",
     "BatchGetStandardsControlAssociationsResponseTypeDef",
     "BatchUpdateStandardsControlAssociationsResponseTypeDef",
+    "AutomationRulesFindingFiltersOutputTypeDef",
     "AutomationRulesFindingFiltersTypeDef",
+    "AwsSecurityFindingFiltersOutputTypeDef",
     "AwsSecurityFindingFiltersTypeDef",
     "GetFindingHistoryResponseTypeDef",
     "GetInsightResultsResponseTypeDef",
+    "NetworkHeaderOutputTypeDef",
     "NetworkHeaderTypeDef",
+    "OccurrencesOutputTypeDef",
     "OccurrencesTypeDef",
+    "RuleGroupSourceStatelessRuleDefinitionOutputTypeDef",
     "RuleGroupSourceStatelessRuleDefinitionTypeDef",
     "DescribeStandardsResponseTypeDef",
     "BatchDisableStandardsResponseTypeDef",
     "BatchEnableStandardsResponseTypeDef",
     "GetEnabledStandardsResponseTypeDef",
+    "StatelessCustomActionDefinitionOutputTypeDef",
     "StatelessCustomActionDefinitionTypeDef",
+    "PortProbeActionOutputTypeDef",
     "PortProbeActionTypeDef",
+    "AutomationRulesActionUnionTypeDef",
+    "AwsAutoScalingAutoScalingGroupDetailsOutputTypeDef",
     "AwsAutoScalingAutoScalingGroupDetailsTypeDef",
+    "AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef",
     "AwsBackupBackupPlanBackupPlanDetailsTypeDef",
+    "AwsCertificateManagerCertificateDetailsOutputTypeDef",
     "AwsCertificateManagerCertificateDetailsTypeDef",
+    "AwsCloudFrontDistributionOriginsOutputTypeDef",
     "AwsCloudFrontDistributionOriginsTypeDef",
+    "AwsCloudFrontDistributionOriginGroupsOutputTypeDef",
     "AwsCloudFrontDistributionOriginGroupsTypeDef",
+    "AwsDynamoDbTableDetailsOutputTypeDef",
     "AwsDynamoDbTableDetailsTypeDef",
+    "AwsEc2LaunchTemplateDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDetailsTypeDef",
+    "AwsEcsClusterDetailsOutputTypeDef",
     "AwsEcsClusterDetailsTypeDef",
+    "AwsEcsTaskDefinitionDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionDetailsTypeDef",
     "AwsGuardDutyDetectorDataSourcesDetailsTypeDef",
+    "AwsRdsDbInstanceDetailsOutputTypeDef",
     "AwsRdsDbInstanceDetailsTypeDef",
+    "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef",
+    "AwsS3BucketNotificationConfigurationDetailOutputTypeDef",
     "AwsS3BucketNotificationConfigurationDetailTypeDef",
+    "AwsStepFunctionStateMachineDetailsOutputTypeDef",
     "AwsStepFunctionStateMachineDetailsTypeDef",
+    "AwsWafv2RulesActionDetailsOutputTypeDef",
+    "AwsWafv2WebAclActionDetailsOutputTypeDef",
     "AwsWafv2RulesActionDetailsTypeDef",
     "AwsWafv2WebAclActionDetailsTypeDef",
     "AutomationRulesConfigTypeDef",
-    "CreateAutomationRuleRequestRequestTypeDef",
+    "AutomationRulesFindingFiltersUnionTypeDef",
     "UpdateAutomationRulesRequestItemTypeDef",
+    "InsightTypeDef",
+    "AwsSecurityFindingFiltersUnionTypeDef",
     "CreateInsightRequestRequestTypeDef",
     "GetFindingsRequestGetFindingsPaginateTypeDef",
     "GetFindingsRequestRequestTypeDef",
-    "InsightTypeDef",
     "UpdateFindingsRequestRequestTypeDef",
     "UpdateInsightRequestRequestTypeDef",
+    "NetworkPathComponentOutputTypeDef",
     "NetworkPathComponentTypeDef",
+    "CustomDataIdentifiersDetectionsOutputTypeDef",
+    "SensitiveDataDetectionsOutputTypeDef",
     "CustomDataIdentifiersDetectionsTypeDef",
     "SensitiveDataDetectionsTypeDef",
+    "RuleGroupSourceStatelessRulesDetailsOutputTypeDef",
     "RuleGroupSourceStatelessRulesDetailsTypeDef",
+    "FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef",
+    "RuleGroupSourceCustomActionsDetailsOutputTypeDef",
     "FirewallPolicyStatelessCustomActionsDetailsTypeDef",
     "RuleGroupSourceCustomActionsDetailsTypeDef",
+    "ActionOutputTypeDef",
     "ActionTypeDef",
+    "CreateAutomationRuleRequestRequestTypeDef",
+    "AwsBackupBackupPlanDetailsOutputTypeDef",
     "AwsBackupBackupPlanDetailsTypeDef",
+    "AwsCloudFrontDistributionDetailsOutputTypeDef",
     "AwsCloudFrontDistributionDetailsTypeDef",
+    "AwsGuardDutyDetectorDetailsOutputTypeDef",
     "AwsGuardDutyDetectorDetailsTypeDef",
+    "AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef",
+    "AwsS3BucketNotificationConfigurationOutputTypeDef",
     "AwsS3BucketNotificationConfigurationTypeDef",
+    "AwsWafv2RulesDetailsOutputTypeDef",
     "AwsWafv2RulesDetailsTypeDef",
     "BatchGetAutomationRulesResponseTypeDef",
     "BatchUpdateAutomationRulesRequestRequestTypeDef",
     "GetInsightsResponseTypeDef",
+    "CustomDataIdentifiersResultOutputTypeDef",
+    "SensitiveDataResultOutputTypeDef",
     "CustomDataIdentifiersResultTypeDef",
     "SensitiveDataResultTypeDef",
+    "FirewallPolicyDetailsOutputTypeDef",
+    "RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef",
     "FirewallPolicyDetailsTypeDef",
     "RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef",
+    "AwsS3BucketBucketLifecycleConfigurationDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef",
+    "AwsWafv2RuleGroupDetailsOutputTypeDef",
+    "AwsWafv2WebAclDetailsOutputTypeDef",
     "AwsWafv2RuleGroupDetailsTypeDef",
     "AwsWafv2WebAclDetailsTypeDef",
+    "ClassificationResultOutputTypeDef",
     "ClassificationResultTypeDef",
+    "AwsNetworkFirewallFirewallPolicyDetailsOutputTypeDef",
+    "RuleGroupSourceOutputTypeDef",
     "AwsNetworkFirewallFirewallPolicyDetailsTypeDef",
     "RuleGroupSourceTypeDef",
+    "AwsS3BucketDetailsOutputTypeDef",
     "AwsS3BucketDetailsTypeDef",
+    "DataClassificationDetailsOutputTypeDef",
     "DataClassificationDetailsTypeDef",
+    "RuleGroupDetailsOutputTypeDef",
     "RuleGroupDetailsTypeDef",
+    "AwsNetworkFirewallRuleGroupDetailsOutputTypeDef",
     "AwsNetworkFirewallRuleGroupDetailsTypeDef",
+    "ResourceDetailsOutputTypeDef",
     "ResourceDetailsTypeDef",
+    "ResourceOutputTypeDef",
     "ResourceTypeDef",
+    "AwsSecurityFindingOutputTypeDef",
     "AwsSecurityFindingTypeDef",
-    "BatchImportFindingsRequestRequestTypeDef",
     "GetFindingsResponseTypeDef",
+    "AwsSecurityFindingUnionTypeDef",
+    "BatchImportFindingsRequestRequestTypeDef",
 )
 
 AcceptAdministratorInvitationRequestRequestTypeDef = TypedDict(
     "AcceptAdministratorInvitationRequestRequestTypeDef",
     {
         "AdministratorId": str,
         "InvitationId": str,
@@ -831,14 +1038,24 @@
     {
         "Port": int,
         "PortName": str,
     },
     total=False,
 )
 
+DnsRequestActionTypeDef = TypedDict(
+    "DnsRequestActionTypeDef",
+    {
+        "Domain": str,
+        "Protocol": str,
+        "Blocked": bool,
+    },
+    total=False,
+)
+
 CityTypeDef = TypedDict(
     "CityTypeDef",
     {
         "CityName": str,
     },
     total=False,
 )
@@ -886,24 +1103,14 @@
     {
         "ActionTargetArn": str,
         "Name": str,
         "Description": str,
     },
 )
 
-DnsRequestActionTypeDef = TypedDict(
-    "DnsRequestActionTypeDef",
-    {
-        "Domain": str,
-        "Protocol": str,
-        "Blocked": bool,
-    },
-    total=False,
-)
-
 AdjustmentTypeDef = TypedDict(
     "AdjustmentTypeDef",
     {
         "Metric": str,
         "Reason": str,
     },
     total=False,
@@ -1028,18 +1235,18 @@
     {
         "KmsKeyId": str,
         "UseAwsOwnedKey": bool,
     },
     total=False,
 )
 
-AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef = TypedDict(
-    "AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef",
+AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef = TypedDict(
+    "AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef",
     {
-        "Hosts": Sequence[str],
+        "Hosts": List[str],
         "RoleBase": str,
         "RoleName": str,
         "RoleSearchMatching": str,
         "RoleSearchSubtree": bool,
         "ServiceAccountUsername": str,
         "UserBase": str,
         "UserRoleName": str,
@@ -1064,14 +1271,31 @@
     {
         "PendingChange": str,
         "Username": str,
     },
     total=False,
 )
 
+AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef = TypedDict(
+    "AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef",
+    {
+        "Hosts": Sequence[str],
+        "RoleBase": str,
+        "RoleName": str,
+        "RoleSearchMatching": str,
+        "RoleSearchSubtree": bool,
+        "ServiceAccountUsername": str,
+        "UserBase": str,
+        "UserRoleName": str,
+        "UserSearchMatching": str,
+        "UserSearchSubtree": bool,
+    },
+    total=False,
+)
+
 AwsAmazonMqBrokerLogsPendingDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerLogsPendingDetailsTypeDef",
     {
         "Audit": bool,
         "General": bool,
     },
     total=False,
@@ -1090,25 +1314,44 @@
     {
         "Format": str,
         "DestinationArn": str,
     },
     total=False,
 )
 
+AwsApiGatewayCanarySettingsOutputTypeDef = TypedDict(
+    "AwsApiGatewayCanarySettingsOutputTypeDef",
+    {
+        "PercentTraffic": float,
+        "DeploymentId": str,
+        "StageVariableOverrides": Dict[str, str],
+        "UseStageCache": bool,
+    },
+    total=False,
+)
+
 AwsApiGatewayCanarySettingsTypeDef = TypedDict(
     "AwsApiGatewayCanarySettingsTypeDef",
     {
         "PercentTraffic": float,
         "DeploymentId": str,
         "StageVariableOverrides": Mapping[str, str],
         "UseStageCache": bool,
     },
     total=False,
 )
 
+AwsApiGatewayEndpointConfigurationOutputTypeDef = TypedDict(
+    "AwsApiGatewayEndpointConfigurationOutputTypeDef",
+    {
+        "Types": List[str],
+    },
+    total=False,
+)
+
 AwsApiGatewayEndpointConfigurationTypeDef = TypedDict(
     "AwsApiGatewayEndpointConfigurationTypeDef",
     {
         "Types": Sequence[str],
     },
     total=False,
 )
@@ -1128,14 +1371,27 @@
         "UnauthorizedCacheControlHeaderStrategy": str,
         "HttpMethod": str,
         "ResourcePath": str,
     },
     total=False,
 )
 
+AwsCorsConfigurationOutputTypeDef = TypedDict(
+    "AwsCorsConfigurationOutputTypeDef",
+    {
+        "AllowOrigins": List[str],
+        "AllowCredentials": bool,
+        "ExposeHeaders": List[str],
+        "MaxAge": int,
+        "AllowMethods": List[str],
+        "AllowHeaders": List[str],
+    },
+    total=False,
+)
+
 AwsCorsConfigurationTypeDef = TypedDict(
     "AwsCorsConfigurationTypeDef",
     {
         "AllowOrigins": Sequence[str],
         "AllowCredentials": bool,
         "ExposeHeaders": Sequence[str],
         "MaxAge": int,
@@ -1276,14 +1532,23 @@
         "HttpEndpoint": str,
         "HttpPutResponseHopLimit": int,
         "HttpTokens": str,
     },
     total=False,
 )
 
+AwsBackupBackupPlanAdvancedBackupSettingsDetailsOutputTypeDef = TypedDict(
+    "AwsBackupBackupPlanAdvancedBackupSettingsDetailsOutputTypeDef",
+    {
+        "BackupOptions": Dict[str, str],
+        "ResourceType": str,
+    },
+    total=False,
+)
+
 AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef",
     {
         "BackupOptions": Mapping[str, str],
         "ResourceType": str,
     },
     total=False,
@@ -1294,14 +1559,23 @@
     {
         "DeleteAfterDays": int,
         "MoveToColdStorageAfterDays": int,
     },
     total=False,
 )
 
+AwsBackupBackupVaultNotificationsDetailsOutputTypeDef = TypedDict(
+    "AwsBackupBackupVaultNotificationsDetailsOutputTypeDef",
+    {
+        "BackupVaultEvents": List[str],
+        "SnsTopicArn": str,
+    },
+    total=False,
+)
+
 AwsBackupBackupVaultNotificationsDetailsTypeDef = TypedDict(
     "AwsBackupBackupVaultNotificationsDetailsTypeDef",
     {
         "BackupVaultEvents": Sequence[str],
         "SnsTopicArn": str,
     },
     total=False,
@@ -1426,23 +1700,41 @@
         "IamCertificateId": str,
         "MinimumProtocolVersion": str,
         "SslSupportMethod": str,
     },
     total=False,
 )
 
+AwsCloudFrontDistributionOriginSslProtocolsOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginSslProtocolsOutputTypeDef",
+    {
+        "Items": List[str],
+        "Quantity": int,
+    },
+    total=False,
+)
+
 AwsCloudFrontDistributionOriginSslProtocolsTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginSslProtocolsTypeDef",
     {
         "Items": Sequence[str],
         "Quantity": int,
     },
     total=False,
 )
 
+AwsCloudFrontDistributionOriginGroupFailoverStatusCodesOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesOutputTypeDef",
+    {
+        "Items": List[int],
+        "Quantity": int,
+    },
+    total=False,
+)
+
 AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef",
     {
         "Items": Sequence[int],
         "Quantity": int,
     },
     total=False,
@@ -1510,14 +1802,24 @@
         "Location": str,
         "GitCloneDepth": int,
         "InsecureSsl": bool,
     },
     total=False,
 )
 
+AwsCodeBuildProjectVpcConfigOutputTypeDef = TypedDict(
+    "AwsCodeBuildProjectVpcConfigOutputTypeDef",
+    {
+        "VpcId": str,
+        "Subnets": List[str],
+        "SecurityGroupIds": List[str],
+    },
+    total=False,
+)
+
 AwsCodeBuildProjectVpcConfigTypeDef = TypedDict(
     "AwsCodeBuildProjectVpcConfigTypeDef",
     {
         "VpcId": str,
         "Subnets": Sequence[str],
         "SecurityGroupIds": Sequence[str],
     },
@@ -1629,14 +1931,23 @@
     {
         "StreamEnabled": bool,
         "StreamViewType": str,
     },
     total=False,
 )
 
+AwsDynamoDbTableProjectionOutputTypeDef = TypedDict(
+    "AwsDynamoDbTableProjectionOutputTypeDef",
+    {
+        "NonKeyAttributes": List[str],
+        "ProjectionType": str,
+    },
+    total=False,
+)
+
 AwsDynamoDbTableProjectionTypeDef = TypedDict(
     "AwsDynamoDbTableProjectionTypeDef",
     {
         "NonKeyAttributes": Sequence[str],
         "ProjectionType": str,
     },
     total=False,
@@ -2098,14 +2409,33 @@
         "AssociationId": str,
         "Ipv6CidrBlock": str,
         "CidrBlockState": str,
     },
     total=False,
 )
 
+AwsEc2TransitGatewayDetailsOutputTypeDef = TypedDict(
+    "AwsEc2TransitGatewayDetailsOutputTypeDef",
+    {
+        "Id": str,
+        "Description": str,
+        "DefaultRouteTablePropagation": str,
+        "AutoAcceptSharedAttachments": str,
+        "DefaultRouteTableAssociation": str,
+        "TransitGatewayCidrBlocks": List[str],
+        "AssociationDefaultRouteTableId": str,
+        "PropagationDefaultRouteTableId": str,
+        "VpnEcmpSupport": str,
+        "DnsSupport": str,
+        "MulticastSupport": str,
+        "AmazonSideAsn": int,
+    },
+    total=False,
+)
+
 AwsEc2TransitGatewayDetailsTypeDef = TypedDict(
     "AwsEc2TransitGatewayDetailsTypeDef",
     {
         "Id": str,
         "Description": str,
         "DefaultRouteTablePropagation": str,
         "AutoAcceptSharedAttachments": str,
@@ -2203,14 +2533,37 @@
         "OutsideIpAddress": str,
         "Status": str,
         "StatusMessage": str,
     },
     total=False,
 )
 
+AwsEc2VpnConnectionOptionsTunnelOptionsDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VpnConnectionOptionsTunnelOptionsDetailsOutputTypeDef",
+    {
+        "DpdTimeoutSeconds": int,
+        "IkeVersions": List[str],
+        "OutsideIpAddress": str,
+        "Phase1DhGroupNumbers": List[int],
+        "Phase1EncryptionAlgorithms": List[str],
+        "Phase1IntegrityAlgorithms": List[str],
+        "Phase1LifetimeSeconds": int,
+        "Phase2DhGroupNumbers": List[int],
+        "Phase2EncryptionAlgorithms": List[str],
+        "Phase2IntegrityAlgorithms": List[str],
+        "Phase2LifetimeSeconds": int,
+        "PreSharedKey": str,
+        "RekeyFuzzPercentage": int,
+        "RekeyMarginTimeSeconds": int,
+        "ReplayWindowSize": int,
+        "TunnelInsideCidr": str,
+    },
+    total=False,
+)
+
 AwsEc2VpnConnectionOptionsTunnelOptionsDetailsTypeDef = TypedDict(
     "AwsEc2VpnConnectionOptionsTunnelOptionsDetailsTypeDef",
     {
         "DpdTimeoutSeconds": int,
         "IkeVersions": Sequence[str],
         "OutsideIpAddress": str,
         "Phase1DhGroupNumbers": Sequence[int],
@@ -2226,14 +2579,27 @@
         "RekeyMarginTimeSeconds": int,
         "ReplayWindowSize": int,
         "TunnelInsideCidr": str,
     },
     total=False,
 )
 
+AwsEcrContainerImageDetailsOutputTypeDef = TypedDict(
+    "AwsEcrContainerImageDetailsOutputTypeDef",
+    {
+        "RegistryId": str,
+        "RepositoryName": str,
+        "Architecture": str,
+        "ImageDigest": str,
+        "ImageTags": List[str],
+        "ImagePublishedAt": str,
+    },
+    total=False,
+)
+
 AwsEcrContainerImageDetailsTypeDef = TypedDict(
     "AwsEcrContainerImageDetailsTypeDef",
     {
         "RegistryId": str,
         "RepositoryName": str,
         "Architecture": str,
         "ImageDigest": str,
@@ -2363,14 +2729,24 @@
         "ContainerPort": int,
         "Port": int,
         "RegistryArn": str,
     },
     total=False,
 )
 
+AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsOutputTypeDef",
+    {
+        "AssignPublicIp": str,
+        "SecurityGroups": List[str],
+        "Subnets": List[str],
+    },
+    total=False,
+)
+
 AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef",
     {
         "AssignPublicIp": str,
         "SecurityGroups": Sequence[str],
         "Subnets": Sequence[str],
     },
@@ -2409,27 +2785,27 @@
     {
         "Hostname": str,
         "IpAddress": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef",
     {
-        "Options": Mapping[str, str],
+        "Options": Dict[str, str],
         "Type": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef",
     {
-        "Command": Sequence[str],
+        "Command": List[str],
         "Interval": int,
         "Retries": int,
         "StartPeriod": int,
         "Timeout": int,
     },
     total=False,
 )
@@ -2504,23 +2880,73 @@
     {
         "ReadOnly": bool,
         "SourceContainer": str,
     },
     total=False,
 )
 
+AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef",
+    {
+        "Options": Mapping[str, str],
+        "Type": str,
+    },
+    total=False,
+)
+
+AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef",
+    {
+        "Command": Sequence[str],
+        "Interval": int,
+        "Retries": int,
+        "StartPeriod": int,
+        "Timeout": int,
+    },
+    total=False,
+)
+
+AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef",
+    {
+        "Add": List[str],
+        "Drop": List[str],
+    },
+    total=False,
+)
+
 AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef",
     {
         "Add": Sequence[str],
         "Drop": Sequence[str],
     },
     total=False,
 )
 
+AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsOutputTypeDef",
+    {
+        "ContainerPath": str,
+        "HostPath": str,
+        "Permissions": List[str],
+    },
+    total=False,
+)
+
+AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsOutputTypeDef",
+    {
+        "ContainerPath": str,
+        "MountOptions": List[str],
+        "Size": int,
+    },
+    total=False,
+)
+
 AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsTypeDef",
     {
         "ContainerPath": str,
         "HostPath": str,
         "Permissions": Sequence[str],
     },
@@ -2569,34 +2995,46 @@
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef",
+AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsOutputTypeDef",
     {
         "Autoprovision": bool,
         "Driver": str,
-        "DriverOpts": Mapping[str, str],
-        "Labels": Mapping[str, str],
+        "DriverOpts": Dict[str, str],
+        "Labels": Dict[str, str],
         "Scope": str,
     },
     total=False,
 )
 
 AwsEcsTaskDefinitionVolumesHostDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesHostDetailsTypeDef",
     {
         "SourcePath": str,
     },
     total=False,
 )
 
+AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef",
+    {
+        "Autoprovision": bool,
+        "Driver": str,
+        "DriverOpts": Mapping[str, str],
+        "Labels": Mapping[str, str],
+        "Scope": str,
+    },
+    total=False,
+)
+
 AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef",
     {
         "AccessPointId": str,
         "Iam": str,
     },
     total=False,
@@ -2606,14 +3044,24 @@
     "AwsEcsTaskVolumeHostDetailsTypeDef",
     {
         "SourcePath": str,
     },
     total=False,
 )
 
+AwsEfsAccessPointPosixUserDetailsOutputTypeDef = TypedDict(
+    "AwsEfsAccessPointPosixUserDetailsOutputTypeDef",
+    {
+        "Gid": str,
+        "SecondaryGids": List[str],
+        "Uid": str,
+    },
+    total=False,
+)
+
 AwsEfsAccessPointPosixUserDetailsTypeDef = TypedDict(
     "AwsEfsAccessPointPosixUserDetailsTypeDef",
     {
         "Gid": str,
         "SecondaryGids": Sequence[str],
         "Uid": str,
     },
@@ -2626,24 +3074,43 @@
         "OwnerGid": str,
         "OwnerUid": str,
         "Permissions": str,
     },
     total=False,
 )
 
+AwsEksClusterResourcesVpcConfigDetailsOutputTypeDef = TypedDict(
+    "AwsEksClusterResourcesVpcConfigDetailsOutputTypeDef",
+    {
+        "SecurityGroupIds": List[str],
+        "SubnetIds": List[str],
+        "EndpointPublicAccess": bool,
+    },
+    total=False,
+)
+
 AwsEksClusterResourcesVpcConfigDetailsTypeDef = TypedDict(
     "AwsEksClusterResourcesVpcConfigDetailsTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "SubnetIds": Sequence[str],
         "EndpointPublicAccess": bool,
     },
     total=False,
 )
 
+AwsEksClusterLoggingClusterLoggingDetailsOutputTypeDef = TypedDict(
+    "AwsEksClusterLoggingClusterLoggingDetailsOutputTypeDef",
+    {
+        "Enabled": bool,
+        "Types": List[str],
+    },
+    total=False,
+)
+
 AwsEksClusterLoggingClusterLoggingDetailsTypeDef = TypedDict(
     "AwsEksClusterLoggingClusterLoggingDetailsTypeDef",
     {
         "Enabled": bool,
         "Types": Sequence[str],
     },
     total=False,
@@ -2715,14 +3182,25 @@
         "NewVersion": str,
         "UpdateAvailable": bool,
         "UpdateStatus": str,
     },
     total=False,
 )
 
+AwsElasticsearchDomainVPCOptionsOutputTypeDef = TypedDict(
+    "AwsElasticsearchDomainVPCOptionsOutputTypeDef",
+    {
+        "AvailabilityZones": List[str],
+        "SecurityGroupIds": List[str],
+        "SubnetIds": List[str],
+        "VPCId": str,
+    },
+    total=False,
+)
+
 AwsElasticsearchDomainVPCOptionsTypeDef = TypedDict(
     "AwsElasticsearchDomainVPCOptionsTypeDef",
     {
         "AvailabilityZones": Sequence[str],
         "SecurityGroupIds": Sequence[str],
         "SubnetIds": Sequence[str],
         "VPCId": str,
@@ -2806,14 +3284,23 @@
     "AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
+AwsElbLoadBalancerBackendServerDescriptionOutputTypeDef = TypedDict(
+    "AwsElbLoadBalancerBackendServerDescriptionOutputTypeDef",
+    {
+        "InstancePort": int,
+        "PolicyNames": List[str],
+    },
+    total=False,
+)
+
 AwsElbLoadBalancerBackendServerDescriptionTypeDef = TypedDict(
     "AwsElbLoadBalancerBackendServerDescriptionTypeDef",
     {
         "InstancePort": int,
         "PolicyNames": Sequence[str],
     },
     total=False,
@@ -3088,14 +3575,24 @@
     "AwsLambdaFunctionTracingConfigTypeDef",
     {
         "Mode": str,
     },
     total=False,
 )
 
+AwsLambdaFunctionVpcConfigOutputTypeDef = TypedDict(
+    "AwsLambdaFunctionVpcConfigOutputTypeDef",
+    {
+        "SecurityGroupIds": List[str],
+        "SubnetIds": List[str],
+        "VpcId": str,
+    },
+    total=False,
+)
+
 AwsLambdaFunctionVpcConfigTypeDef = TypedDict(
     "AwsLambdaFunctionVpcConfigTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "SubnetIds": Sequence[str],
         "VpcId": str,
     },
@@ -3107,14 +3604,24 @@
     {
         "ErrorCode": str,
         "Message": str,
     },
     total=False,
 )
 
+AwsLambdaLayerVersionDetailsOutputTypeDef = TypedDict(
+    "AwsLambdaLayerVersionDetailsOutputTypeDef",
+    {
+        "Version": int,
+        "CompatibleRuntimes": List[str],
+        "CreatedDate": str,
+    },
+    total=False,
+)
+
 AwsLambdaLayerVersionDetailsTypeDef = TypedDict(
     "AwsLambdaLayerVersionDetailsTypeDef",
     {
         "Version": int,
         "CompatibleRuntimes": Sequence[str],
         "CreatedDate": str,
     },
@@ -3187,14 +3694,23 @@
         "UpdateAvailable": bool,
         "UpdateStatus": str,
         "OptionalDeployment": bool,
     },
     total=False,
 )
 
+AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef = TypedDict(
+    "AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef",
+    {
+        "SecurityGroupIds": List[str],
+        "SubnetIds": List[str],
+    },
+    total=False,
+)
+
 AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "SubnetIds": Sequence[str],
     },
     total=False,
@@ -3254,14 +3770,39 @@
     {
         "VpcSecurityGroupId": str,
         "Status": str,
     },
     total=False,
 )
 
+AwsRdsDbClusterSnapshotDetailsOutputTypeDef = TypedDict(
+    "AwsRdsDbClusterSnapshotDetailsOutputTypeDef",
+    {
+        "AvailabilityZones": List[str],
+        "SnapshotCreateTime": str,
+        "Engine": str,
+        "AllocatedStorage": int,
+        "Status": str,
+        "Port": int,
+        "VpcId": str,
+        "ClusterCreateTime": str,
+        "MasterUsername": str,
+        "EngineVersion": str,
+        "LicenseModel": str,
+        "SnapshotType": str,
+        "PercentProgress": int,
+        "StorageEncrypted": bool,
+        "KmsKeyId": str,
+        "DbClusterIdentifier": str,
+        "DbClusterSnapshotIdentifier": str,
+        "IamDatabaseAuthenticationEnabled": bool,
+    },
+    total=False,
+)
+
 AwsRdsDbClusterSnapshotDetailsTypeDef = TypedDict(
     "AwsRdsDbClusterSnapshotDetailsTypeDef",
     {
         "AvailabilityZones": Sequence[str],
         "SnapshotCreateTime": str,
         "Engine": str,
         "AllocatedStorage": int,
@@ -3337,14 +3878,23 @@
         "Normal": bool,
         "Status": str,
         "Message": str,
     },
     total=False,
 )
 
+AwsRdsPendingCloudWatchLogsExportsOutputTypeDef = TypedDict(
+    "AwsRdsPendingCloudWatchLogsExportsOutputTypeDef",
+    {
+        "LogTypesToEnable": List[str],
+        "LogTypesToDisable": List[str],
+    },
+    total=False,
+)
+
 AwsRdsPendingCloudWatchLogsExportsTypeDef = TypedDict(
     "AwsRdsPendingCloudWatchLogsExportsTypeDef",
     {
         "LogTypesToEnable": Sequence[str],
         "LogTypesToDisable": Sequence[str],
     },
     total=False,
@@ -3374,14 +3924,31 @@
     "AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+AwsRdsEventSubscriptionDetailsOutputTypeDef = TypedDict(
+    "AwsRdsEventSubscriptionDetailsOutputTypeDef",
+    {
+        "CustSubscriptionId": str,
+        "CustomerAwsId": str,
+        "Enabled": bool,
+        "EventCategoriesList": List[str],
+        "EventSubscriptionArn": str,
+        "SnsTopicArn": str,
+        "SourceIdsList": List[str],
+        "SourceType": str,
+        "Status": str,
+        "SubscriptionCreationTime": str,
+    },
+    total=False,
+)
+
 AwsRdsEventSubscriptionDetailsTypeDef = TypedDict(
     "AwsRdsEventSubscriptionDetailsTypeDef",
     {
         "CustSubscriptionId": str,
         "CustomerAwsId": str,
         "Enabled": bool,
         "EventCategoriesList": Sequence[str],
@@ -4035,14 +4602,25 @@
 BatchDeleteAutomationRulesRequestRequestTypeDef = TypedDict(
     "BatchDeleteAutomationRulesRequestRequestTypeDef",
     {
         "AutomationRulesArns": Sequence[str],
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
 UnprocessedAutomationRuleTypeDef = TypedDict(
     "UnprocessedAutomationRuleTypeDef",
     {
         "RuleArn": str,
         "ErrorCode": int,
         "ErrorMessage": str,
     },
@@ -4240,30 +4818,14 @@
     {
         "Name": str,
         "Description": str,
         "Id": str,
     },
 )
 
-CreateActionTargetResponseTypeDef = TypedDict(
-    "CreateActionTargetResponseTypeDef",
-    {
-        "ActionTargetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateAutomationRuleResponseTypeDef = TypedDict(
-    "CreateAutomationRuleResponseTypeDef",
-    {
-        "RuleArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateFindingAggregatorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFindingAggregatorRequestRequestTypeDef",
     {
         "RegionLinkingMode": str,
     },
 )
 _OptionalCreateFindingAggregatorRequestRequestTypeDef = TypedDict(
@@ -4276,33 +4838,14 @@
 
 class CreateFindingAggregatorRequestRequestTypeDef(
     _RequiredCreateFindingAggregatorRequestRequestTypeDef,
     _OptionalCreateFindingAggregatorRequestRequestTypeDef,
 ):
     pass
 
-CreateFindingAggregatorResponseTypeDef = TypedDict(
-    "CreateFindingAggregatorResponseTypeDef",
-    {
-        "FindingAggregatorArn": str,
-        "FindingAggregationRegion": str,
-        "RegionLinkingMode": str,
-        "Regions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateInsightResponseTypeDef = TypedDict(
-    "CreateInsightResponseTypeDef",
-    {
-        "InsightArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResultTypeDef = TypedDict(
     "ResultTypeDef",
     {
         "AccountId": str,
         "ProcessingResult": str,
     },
     total=False,
@@ -4327,63 +4870,48 @@
 DeleteActionTargetRequestRequestTypeDef = TypedDict(
     "DeleteActionTargetRequestRequestTypeDef",
     {
         "ActionTargetArn": str,
     },
 )
 
-DeleteActionTargetResponseTypeDef = TypedDict(
-    "DeleteActionTargetResponseTypeDef",
-    {
-        "ActionTargetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteFindingAggregatorRequestRequestTypeDef = TypedDict(
     "DeleteFindingAggregatorRequestRequestTypeDef",
     {
         "FindingAggregatorArn": str,
     },
 )
 
 DeleteInsightRequestRequestTypeDef = TypedDict(
     "DeleteInsightRequestRequestTypeDef",
     {
         "InsightArn": str,
     },
 )
 
-DeleteInsightResponseTypeDef = TypedDict(
-    "DeleteInsightResponseTypeDef",
-    {
-        "InsightArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteInvitationsRequestRequestTypeDef = TypedDict(
     "DeleteInvitationsRequestRequestTypeDef",
     {
         "AccountIds": Sequence[str],
     },
 )
 
 DeleteMembersRequestRequestTypeDef = TypedDict(
     "DeleteMembersRequestRequestTypeDef",
     {
         "AccountIds": Sequence[str],
     },
 )
 
-DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef = TypedDict(
-    "DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ActionTargetArns": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeActionTargetsRequestRequestTypeDef = TypedDict(
     "DescribeActionTargetsRequestRequestTypeDef",
     {
@@ -4398,44 +4926,14 @@
     "DescribeHubRequestRequestTypeDef",
     {
         "HubArn": str,
     },
     total=False,
 )
 
-DescribeHubResponseTypeDef = TypedDict(
-    "DescribeHubResponseTypeDef",
-    {
-        "HubArn": str,
-        "SubscribedAt": str,
-        "AutoEnableControls": bool,
-        "ControlFindingGenerator": ControlFindingGeneratorType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
-    "DescribeOrganizationConfigurationResponseTypeDef",
-    {
-        "AutoEnable": bool,
-        "MemberAccountLimitReached": bool,
-        "AutoEnableStandards": AutoEnableStandardsType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeProductsRequestDescribeProductsPaginateTypeDef = TypedDict(
-    "DescribeProductsRequestDescribeProductsPaginateTypeDef",
-    {
-        "ProductArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeProductsRequestRequestTypeDef = TypedDict(
     "DescribeProductsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ProductArn": str,
     },
@@ -4462,34 +4960,14 @@
     },
     total=False,
 )
 
 class ProductTypeDef(_RequiredProductTypeDef, _OptionalProductTypeDef):
     pass
 
-_RequiredDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef",
-    {
-        "StandardsSubscriptionArn": str,
-    },
-)
-_OptionalDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef(
-    _RequiredDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
-    _OptionalDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeStandardsControlsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeStandardsControlsRequestRequestTypeDef",
     {
         "StandardsSubscriptionArn": str,
     },
 )
 _OptionalDescribeStandardsControlsRequestRequestTypeDef = TypedDict(
@@ -4520,22 +4998,14 @@
         "RemediationUrl": str,
         "SeverityRating": SeverityRatingType,
         "RelatedRequirements": List[str],
     },
     total=False,
 )
 
-DescribeStandardsRequestDescribeStandardsPaginateTypeDef = TypedDict(
-    "DescribeStandardsRequestDescribeStandardsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeStandardsRequestRequestTypeDef = TypedDict(
     "DescribeStandardsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -4565,22 +5035,14 @@
 EnableImportFindingsForProductRequestRequestTypeDef = TypedDict(
     "EnableImportFindingsForProductRequestRequestTypeDef",
     {
         "ProductArn": str,
     },
 )
 
-EnableImportFindingsForProductResponseTypeDef = TypedDict(
-    "EnableImportFindingsForProductResponseTypeDef",
-    {
-        "ProductSubscriptionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnableOrganizationAdminAccountRequestRequestTypeDef = TypedDict(
     "EnableOrganizationAdminAccountRequestRequestTypeDef",
     {
         "AdminAccountId": str,
     },
 )
 
@@ -4665,23 +5127,14 @@
         "InvitationId": str,
         "InvitedAt": datetime,
         "MemberStatus": str,
     },
     total=False,
 )
 
-GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef = TypedDict(
-    "GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef",
-    {
-        "StandardsSubscriptionArns": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetEnabledStandardsRequestRequestTypeDef = TypedDict(
     "GetEnabledStandardsRequestRequestTypeDef",
     {
         "StandardsSubscriptionArns": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
@@ -4691,25 +5144,15 @@
 GetFindingAggregatorRequestRequestTypeDef = TypedDict(
     "GetFindingAggregatorRequestRequestTypeDef",
     {
         "FindingAggregatorArn": str,
     },
 )
 
-GetFindingAggregatorResponseTypeDef = TypedDict(
-    "GetFindingAggregatorResponseTypeDef",
-    {
-        "FindingAggregatorArn": str,
-        "FindingAggregationRegion": str,
-        "RegionLinkingMode": str,
-        "Regions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 SortCriterionTypeDef = TypedDict(
     "SortCriterionTypeDef",
     {
         "Field": str,
         "SortOrder": SortOrderType,
     },
     total=False,
@@ -4718,41 +5161,24 @@
 GetInsightResultsRequestRequestTypeDef = TypedDict(
     "GetInsightResultsRequestRequestTypeDef",
     {
         "InsightArn": str,
     },
 )
 
-GetInsightsRequestGetInsightsPaginateTypeDef = TypedDict(
-    "GetInsightsRequestGetInsightsPaginateTypeDef",
-    {
-        "InsightArns": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetInsightsRequestRequestTypeDef = TypedDict(
     "GetInsightsRequestRequestTypeDef",
     {
         "InsightArns": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-GetInvitationsCountResponseTypeDef = TypedDict(
-    "GetInvitationsCountResponseTypeDef",
-    {
-        "InvitationsCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetMembersRequestRequestTypeDef = TypedDict(
     "GetMembersRequestRequestTypeDef",
     {
         "AccountIds": Sequence[str],
     },
 )
 
@@ -4790,119 +5216,60 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef = TypedDict(
-    "ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListEnabledProductsForImportRequestRequestTypeDef = TypedDict(
     "ListEnabledProductsForImportRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListEnabledProductsForImportResponseTypeDef = TypedDict(
-    "ListEnabledProductsForImportResponseTypeDef",
-    {
-        "ProductSubscriptions": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef = TypedDict(
-    "ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFindingAggregatorsRequestRequestTypeDef = TypedDict(
     "ListFindingAggregatorsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListInvitationsRequestListInvitationsPaginateTypeDef = TypedDict(
-    "ListInvitationsRequestListInvitationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListInvitationsRequestRequestTypeDef = TypedDict(
     "ListInvitationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListMembersRequestListMembersPaginateTypeDef = TypedDict(
-    "ListMembersRequestListMembersPaginateTypeDef",
-    {
-        "OnlyAssociated": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMembersRequestRequestTypeDef = TypedDict(
     "ListMembersRequestRequestTypeDef",
     {
         "OnlyAssociated": bool,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef = TypedDict(
-    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOrganizationAdminAccountsRequestRequestTypeDef = TypedDict(
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef = TypedDict(
-    "ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef",
-    {
-        "StandardsArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSecurityControlDefinitionsRequestRequestTypeDef = TypedDict(
     "ListSecurityControlDefinitionsRequestRequestTypeDef",
     {
         "StandardsArn": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -4917,34 +5284,14 @@
         "Description": str,
         "RemediationUrl": str,
         "SeverityRating": SeverityRatingType,
         "CurrentRegionAvailability": RegionAvailabilityStatusType,
     },
 )
 
-_RequiredListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef",
-    {
-        "SecurityControlId": str,
-    },
-)
-_OptionalListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef(
-    _RequiredListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef,
-    _OptionalListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef,
-):
-    pass
-
 _RequiredListStandardsControlAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredListStandardsControlAssociationsRequestRequestTypeDef",
     {
         "SecurityControlId": str,
     },
 )
 _OptionalListStandardsControlAssociationsRequestRequestTypeDef = TypedDict(
@@ -4992,22 +5339,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PortRangeTypeDef = TypedDict(
     "PortRangeTypeDef",
     {
         "Begin": int,
         "End": int,
     },
     total=False,
@@ -5028,42 +5367,31 @@
     {
         "JsonPath": str,
         "RecordIndex": int,
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
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "Text": str,
         "Url": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+RuleGroupSourceListDetailsOutputTypeDef = TypedDict(
+    "RuleGroupSourceListDetailsOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "GeneratedRulesType": str,
+        "TargetTypes": List[str],
+        "Targets": List[str],
     },
+    total=False,
 )
 
 RuleGroupSourceListDetailsTypeDef = TypedDict(
     "RuleGroupSourceListDetailsTypeDef",
     {
         "GeneratedRulesType": str,
         "TargetTypes": Sequence[str],
@@ -5081,14 +5409,23 @@
         "Protocol": str,
         "Source": str,
         "SourcePort": str,
     },
     total=False,
 )
 
+RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef",
+    {
+        "Keyword": str,
+        "Settings": List[str],
+    },
+    total=False,
+)
+
 RuleGroupSourceStatefulRulesOptionsDetailsTypeDef = TypedDict(
     "RuleGroupSourceStatefulRulesOptionsDetailsTypeDef",
     {
         "Keyword": str,
         "Settings": Sequence[str],
     },
     total=False,
@@ -5124,31 +5461,56 @@
     "RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef",
     {
         "AddressDefinition": str,
     },
     total=False,
 )
 
+RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef",
+    {
+        "Flags": List[str],
+        "Masks": List[str],
+    },
+    total=False,
+)
+
 RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef",
     {
         "Flags": Sequence[str],
         "Masks": Sequence[str],
     },
     total=False,
 )
 
+RuleGroupVariablesIpSetsDetailsOutputTypeDef = TypedDict(
+    "RuleGroupVariablesIpSetsDetailsOutputTypeDef",
+    {
+        "Definition": List[str],
+    },
+    total=False,
+)
+
 RuleGroupVariablesIpSetsDetailsTypeDef = TypedDict(
     "RuleGroupVariablesIpSetsDetailsTypeDef",
     {
         "Definition": Sequence[str],
     },
     total=False,
 )
 
+RuleGroupVariablesPortSetsDetailsOutputTypeDef = TypedDict(
+    "RuleGroupVariablesPortSetsDetailsOutputTypeDef",
+    {
+        "Definition": List[str],
+    },
+    total=False,
+)
+
 RuleGroupVariablesPortSetsDetailsTypeDef = TypedDict(
     "RuleGroupVariablesPortSetsDetailsTypeDef",
     {
         "Definition": Sequence[str],
     },
     total=False,
 )
@@ -5249,25 +5611,14 @@
 
 class UpdateFindingAggregatorRequestRequestTypeDef(
     _RequiredUpdateFindingAggregatorRequestRequestTypeDef,
     _OptionalUpdateFindingAggregatorRequestRequestTypeDef,
 ):
     pass
 
-UpdateFindingAggregatorResponseTypeDef = TypedDict(
-    "UpdateFindingAggregatorResponseTypeDef",
-    {
-        "FindingAggregatorArn": str,
-        "FindingAggregationRegion": str,
-        "RegionLinkingMode": str,
-        "Regions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateOrganizationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOrganizationConfigurationRequestRequestTypeDef",
     {
         "AutoEnable": bool,
     },
 )
 _OptionalUpdateOrganizationConfigurationRequestRequestTypeDef = TypedDict(
@@ -5351,94 +5702,111 @@
         "Country": CountryTypeDef,
         "City": CityTypeDef,
         "GeoLocation": GeoLocationTypeDef,
     },
     total=False,
 )
 
-DescribeActionTargetsResponseTypeDef = TypedDict(
-    "DescribeActionTargetsResponseTypeDef",
+CvssOutputTypeDef = TypedDict(
+    "CvssOutputTypeDef",
     {
-        "ActionTargets": List[ActionTargetTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Version": str,
+        "BaseScore": float,
+        "BaseVector": str,
+        "Source": str,
+        "Adjustments": List[AdjustmentTypeDef],
     },
+    total=False,
 )
 
 CvssTypeDef = TypedDict(
     "CvssTypeDef",
     {
         "Version": str,
         "BaseScore": float,
         "BaseVector": str,
         "Source": str,
         "Adjustments": Sequence[AdjustmentTypeDef],
     },
     total=False,
 )
 
-ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
-    "ListOrganizationAdminAccountsResponseTypeDef",
-    {
-        "AdminAccounts": List[AdminAccountTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssociationSetDetailsTypeDef = TypedDict(
     "AssociationSetDetailsTypeDef",
     {
         "AssociationState": AssociationStateDetailsTypeDef,
         "GatewayId": str,
         "Main": bool,
         "RouteTableAssociationId": str,
         "RouteTableId": str,
         "SubnetId": str,
     },
     total=False,
 )
 
-AutomationRulesFindingFieldsUpdateTypeDef = TypedDict(
-    "AutomationRulesFindingFieldsUpdateTypeDef",
+AutomationRulesFindingFieldsUpdateOutputTypeDef = TypedDict(
+    "AutomationRulesFindingFieldsUpdateOutputTypeDef",
     {
         "Note": NoteUpdateTypeDef,
         "Severity": SeverityUpdateTypeDef,
         "VerificationState": VerificationStateType,
         "Confidence": int,
         "Criticality": int,
         "Types": List[str],
         "UserDefinedFields": Dict[str, str],
         "Workflow": WorkflowUpdateTypeDef,
         "RelatedFindings": List[RelatedFindingTypeDef],
     },
     total=False,
 )
 
-ListAutomationRulesResponseTypeDef = TypedDict(
-    "ListAutomationRulesResponseTypeDef",
+AutomationRulesFindingFieldsUpdateTypeDef = TypedDict(
+    "AutomationRulesFindingFieldsUpdateTypeDef",
     {
-        "AutomationRulesMetadata": List[AutomationRulesMetadataTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Note": NoteUpdateTypeDef,
+        "Severity": SeverityUpdateTypeDef,
+        "VerificationState": VerificationStateType,
+        "Confidence": int,
+        "Criticality": int,
+        "Types": Sequence[str],
+        "UserDefinedFields": Mapping[str, str],
+        "Workflow": WorkflowUpdateTypeDef,
+        "RelatedFindings": Sequence[RelatedFindingTypeDef],
     },
+    total=False,
 )
 
 AwsAmazonMqBrokerLogsDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerLogsDetailsTypeDef",
     {
         "Audit": bool,
         "General": bool,
         "AuditLogGroup": str,
         "GeneralLogGroup": str,
         "Pending": AwsAmazonMqBrokerLogsPendingDetailsTypeDef,
     },
     total=False,
 )
 
+AwsApiGatewayRestApiDetailsOutputTypeDef = TypedDict(
+    "AwsApiGatewayRestApiDetailsOutputTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "CreatedDate": str,
+        "Version": str,
+        "BinaryMediaTypes": List[str],
+        "MinimumCompressionSize": int,
+        "ApiKeySource": str,
+        "EndpointConfiguration": AwsApiGatewayEndpointConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 AwsApiGatewayRestApiDetailsTypeDef = TypedDict(
     "AwsApiGatewayRestApiDetailsTypeDef",
     {
         "Id": str,
         "Name": str,
         "Description": str,
         "CreatedDate": str,
@@ -5447,14 +5815,37 @@
         "MinimumCompressionSize": int,
         "ApiKeySource": str,
         "EndpointConfiguration": AwsApiGatewayEndpointConfigurationTypeDef,
     },
     total=False,
 )
 
+AwsApiGatewayStageDetailsOutputTypeDef = TypedDict(
+    "AwsApiGatewayStageDetailsOutputTypeDef",
+    {
+        "DeploymentId": str,
+        "ClientCertificateId": str,
+        "StageName": str,
+        "Description": str,
+        "CacheClusterEnabled": bool,
+        "CacheClusterSize": str,
+        "CacheClusterStatus": str,
+        "MethodSettings": List[AwsApiGatewayMethodSettingsTypeDef],
+        "Variables": Dict[str, str],
+        "DocumentationVersion": str,
+        "AccessLogSettings": AwsApiGatewayAccessLogSettingsTypeDef,
+        "CanarySettings": AwsApiGatewayCanarySettingsOutputTypeDef,
+        "TracingEnabled": bool,
+        "CreatedDate": str,
+        "LastUpdatedDate": str,
+        "WebAclArn": str,
+    },
+    total=False,
+)
+
 AwsApiGatewayStageDetailsTypeDef = TypedDict(
     "AwsApiGatewayStageDetailsTypeDef",
     {
         "DeploymentId": str,
         "ClientCertificateId": str,
         "StageName": str,
         "Description": str,
@@ -5470,14 +5861,31 @@
         "CreatedDate": str,
         "LastUpdatedDate": str,
         "WebAclArn": str,
     },
     total=False,
 )
 
+AwsApiGatewayV2ApiDetailsOutputTypeDef = TypedDict(
+    "AwsApiGatewayV2ApiDetailsOutputTypeDef",
+    {
+        "ApiEndpoint": str,
+        "ApiId": str,
+        "ApiKeySelectionExpression": str,
+        "CreatedDate": str,
+        "Description": str,
+        "Version": str,
+        "Name": str,
+        "ProtocolType": str,
+        "RouteSelectionExpression": str,
+        "CorsConfiguration": AwsCorsConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 AwsApiGatewayV2ApiDetailsTypeDef = TypedDict(
     "AwsApiGatewayV2ApiDetailsTypeDef",
     {
         "ApiEndpoint": str,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
         "CreatedDate": str,
@@ -5487,14 +5895,34 @@
         "ProtocolType": str,
         "RouteSelectionExpression": str,
         "CorsConfiguration": AwsCorsConfigurationTypeDef,
     },
     total=False,
 )
 
+AwsApiGatewayV2StageDetailsOutputTypeDef = TypedDict(
+    "AwsApiGatewayV2StageDetailsOutputTypeDef",
+    {
+        "ClientCertificateId": str,
+        "CreatedDate": str,
+        "Description": str,
+        "DefaultRouteSettings": AwsApiGatewayV2RouteSettingsTypeDef,
+        "DeploymentId": str,
+        "LastUpdatedDate": str,
+        "RouteSettings": AwsApiGatewayV2RouteSettingsTypeDef,
+        "StageName": str,
+        "StageVariables": Dict[str, str],
+        "AccessLogSettings": AwsApiGatewayAccessLogSettingsTypeDef,
+        "AutoDeploy": bool,
+        "LastDeploymentStatusMessage": str,
+        "ApiGatewayManaged": bool,
+    },
+    total=False,
+)
+
 AwsApiGatewayV2StageDetailsTypeDef = TypedDict(
     "AwsApiGatewayV2StageDetailsTypeDef",
     {
         "ClientCertificateId": str,
         "CreatedDate": str,
         "Description": str,
         "DefaultRouteSettings": AwsApiGatewayV2RouteSettingsTypeDef,
@@ -5518,14 +5946,25 @@
         "LambdaAuthorizerConfig": AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef,
         "OpenIdConnectConfig": AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef,
         "UserPoolConfig": AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef,
     },
     total=False,
 )
 
+AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef = TypedDict(
+    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef",
+    {
+        "LaunchTemplateSpecification": AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef,
+        "Overrides": List[
+            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef
+        ],
+    },
+    total=False,
+)
+
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef",
     {
         "LaunchTemplateSpecification": AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef,
         "Overrides": Sequence[
             AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef
         ],
@@ -5549,14 +5988,26 @@
     {
         "DestinationBackupVaultArn": str,
         "Lifecycle": AwsBackupBackupPlanLifecycleDetailsTypeDef,
     },
     total=False,
 )
 
+AwsBackupBackupVaultDetailsOutputTypeDef = TypedDict(
+    "AwsBackupBackupVaultDetailsOutputTypeDef",
+    {
+        "BackupVaultArn": str,
+        "BackupVaultName": str,
+        "EncryptionKeyArn": str,
+        "Notifications": AwsBackupBackupVaultNotificationsDetailsOutputTypeDef,
+        "AccessPolicy": str,
+    },
+    total=False,
+)
+
 AwsBackupBackupVaultDetailsTypeDef = TypedDict(
     "AwsBackupBackupVaultDetailsTypeDef",
     {
         "BackupVaultArn": str,
         "BackupVaultName": str,
         "EncryptionKeyArn": str,
         "Notifications": AwsBackupBackupVaultNotificationsDetailsTypeDef,
@@ -5587,27 +6038,62 @@
         "Status": str,
         "StatusMessage": str,
         "StorageClass": str,
     },
     total=False,
 )
 
+AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef = TypedDict(
+    "AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef",
+    {
+        "DomainName": str,
+        "ResourceRecord": AwsCertificateManagerCertificateResourceRecordTypeDef,
+        "ValidationDomain": str,
+        "ValidationEmails": List[str],
+        "ValidationMethod": str,
+        "ValidationStatus": str,
+    },
+    total=False,
+)
+
 AwsCertificateManagerCertificateDomainValidationOptionTypeDef = TypedDict(
     "AwsCertificateManagerCertificateDomainValidationOptionTypeDef",
     {
         "DomainName": str,
         "ResourceRecord": AwsCertificateManagerCertificateResourceRecordTypeDef,
         "ValidationDomain": str,
         "ValidationEmails": Sequence[str],
         "ValidationMethod": str,
         "ValidationStatus": str,
     },
     total=False,
 )
 
+AwsCloudFormationStackDetailsOutputTypeDef = TypedDict(
+    "AwsCloudFormationStackDetailsOutputTypeDef",
+    {
+        "Capabilities": List[str],
+        "CreationTime": str,
+        "Description": str,
+        "DisableRollback": bool,
+        "DriftInformation": AwsCloudFormationStackDriftInformationDetailsTypeDef,
+        "EnableTerminationProtection": bool,
+        "LastUpdatedTime": str,
+        "NotificationArns": List[str],
+        "Outputs": List[AwsCloudFormationStackOutputsDetailsTypeDef],
+        "RoleArn": str,
+        "StackId": str,
+        "StackName": str,
+        "StackStatus": str,
+        "StackStatusReason": str,
+        "TimeoutInMinutes": int,
+    },
+    total=False,
+)
+
 AwsCloudFormationStackDetailsTypeDef = TypedDict(
     "AwsCloudFormationStackDetailsTypeDef",
     {
         "Capabilities": Sequence[str],
         "CreationTime": str,
         "Description": str,
         "DisableRollback": bool,
@@ -5622,43 +6108,101 @@
         "StackStatus": str,
         "StackStatusReason": str,
         "TimeoutInMinutes": int,
     },
     total=False,
 )
 
+AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef",
+    {
+        "Items": List[AwsCloudFrontDistributionCacheBehaviorTypeDef],
+    },
+    total=False,
+)
+
 AwsCloudFrontDistributionCacheBehaviorsTypeDef = TypedDict(
     "AwsCloudFrontDistributionCacheBehaviorsTypeDef",
     {
         "Items": Sequence[AwsCloudFrontDistributionCacheBehaviorTypeDef],
     },
     total=False,
 )
 
+AwsCloudFrontDistributionOriginCustomOriginConfigOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginCustomOriginConfigOutputTypeDef",
+    {
+        "HttpPort": int,
+        "HttpsPort": int,
+        "OriginKeepaliveTimeout": int,
+        "OriginProtocolPolicy": str,
+        "OriginReadTimeout": int,
+        "OriginSslProtocols": AwsCloudFrontDistributionOriginSslProtocolsOutputTypeDef,
+    },
+    total=False,
+)
+
 AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef",
     {
         "HttpPort": int,
         "HttpsPort": int,
         "OriginKeepaliveTimeout": int,
         "OriginProtocolPolicy": str,
         "OriginReadTimeout": int,
         "OriginSslProtocols": AwsCloudFrontDistributionOriginSslProtocolsTypeDef,
     },
     total=False,
 )
 
+AwsCloudFrontDistributionOriginGroupFailoverOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginGroupFailoverOutputTypeDef",
+    {
+        "StatusCodes": AwsCloudFrontDistributionOriginGroupFailoverStatusCodesOutputTypeDef,
+    },
+    total=False,
+)
+
 AwsCloudFrontDistributionOriginGroupFailoverTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupFailoverTypeDef",
     {
         "StatusCodes": AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef,
     },
     total=False,
 )
 
+AwsCloudWatchAlarmDetailsOutputTypeDef = TypedDict(
+    "AwsCloudWatchAlarmDetailsOutputTypeDef",
+    {
+        "ActionsEnabled": bool,
+        "AlarmActions": List[str],
+        "AlarmArn": str,
+        "AlarmConfigurationUpdatedTimestamp": str,
+        "AlarmDescription": str,
+        "AlarmName": str,
+        "ComparisonOperator": str,
+        "DatapointsToAlarm": int,
+        "Dimensions": List[AwsCloudWatchAlarmDimensionsDetailsTypeDef],
+        "EvaluateLowSampleCountPercentile": str,
+        "EvaluationPeriods": int,
+        "ExtendedStatistic": str,
+        "InsufficientDataActions": List[str],
+        "MetricName": str,
+        "Namespace": str,
+        "OkActions": List[str],
+        "Period": int,
+        "Statistic": str,
+        "Threshold": float,
+        "ThresholdMetricId": str,
+        "TreatMissingData": str,
+        "Unit": str,
+    },
+    total=False,
+)
+
 AwsCloudWatchAlarmDetailsTypeDef = TypedDict(
     "AwsCloudWatchAlarmDetailsTypeDef",
     {
         "ActionsEnabled": bool,
         "AlarmActions": Sequence[str],
         "AlarmArn": str,
         "AlarmConfigurationUpdatedTimestamp": str,
@@ -5680,14 +6224,29 @@
         "ThresholdMetricId": str,
         "TreatMissingData": str,
         "Unit": str,
     },
     total=False,
 )
 
+AwsCodeBuildProjectEnvironmentOutputTypeDef = TypedDict(
+    "AwsCodeBuildProjectEnvironmentOutputTypeDef",
+    {
+        "Certificate": str,
+        "EnvironmentVariables": List[
+            AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef
+        ],
+        "PrivilegedMode": bool,
+        "ImagePullCredentialsType": str,
+        "RegistryCredential": AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef,
+        "Type": str,
+    },
+    total=False,
+)
+
 AwsCodeBuildProjectEnvironmentTypeDef = TypedDict(
     "AwsCodeBuildProjectEnvironmentTypeDef",
     {
         "Certificate": str,
         "EnvironmentVariables": Sequence[
             AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef
         ],
@@ -5704,14 +6263,41 @@
     {
         "CloudWatchLogs": AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef,
         "S3Logs": AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef,
     },
     total=False,
 )
 
+AwsDynamoDbTableGlobalSecondaryIndexOutputTypeDef = TypedDict(
+    "AwsDynamoDbTableGlobalSecondaryIndexOutputTypeDef",
+    {
+        "Backfilling": bool,
+        "IndexArn": str,
+        "IndexName": str,
+        "IndexSizeBytes": int,
+        "IndexStatus": str,
+        "ItemCount": int,
+        "KeySchema": List[AwsDynamoDbTableKeySchemaTypeDef],
+        "Projection": AwsDynamoDbTableProjectionOutputTypeDef,
+        "ProvisionedThroughput": AwsDynamoDbTableProvisionedThroughputTypeDef,
+    },
+    total=False,
+)
+
+AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef = TypedDict(
+    "AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef",
+    {
+        "IndexArn": str,
+        "IndexName": str,
+        "KeySchema": List[AwsDynamoDbTableKeySchemaTypeDef],
+        "Projection": AwsDynamoDbTableProjectionOutputTypeDef,
+    },
+    total=False,
+)
+
 AwsDynamoDbTableGlobalSecondaryIndexTypeDef = TypedDict(
     "AwsDynamoDbTableGlobalSecondaryIndexTypeDef",
     {
         "Backfilling": bool,
         "IndexArn": str,
         "IndexName": str,
         "IndexSizeBytes": int,
@@ -5740,14 +6326,34 @@
     {
         "IndexName": str,
         "ProvisionedThroughputOverride": AwsDynamoDbTableProvisionedThroughputOverrideTypeDef,
     },
     total=False,
 )
 
+AwsEc2InstanceDetailsOutputTypeDef = TypedDict(
+    "AwsEc2InstanceDetailsOutputTypeDef",
+    {
+        "Type": str,
+        "ImageId": str,
+        "IpV4Addresses": List[str],
+        "IpV6Addresses": List[str],
+        "KeyName": str,
+        "IamInstanceProfileArn": str,
+        "VpcId": str,
+        "SubnetId": str,
+        "LaunchedAt": str,
+        "NetworkInterfaces": List[AwsEc2InstanceNetworkInterfacesDetailsTypeDef],
+        "VirtualizationType": str,
+        "MetadataOptions": AwsEc2InstanceMetadataOptionsTypeDef,
+        "Monitoring": AwsEc2InstanceMonitoringDetailsTypeDef,
+    },
+    total=False,
+)
+
 AwsEc2InstanceDetailsTypeDef = TypedDict(
     "AwsEc2InstanceDetailsTypeDef",
     {
         "Type": str,
         "ImageId": str,
         "IpV4Addresses": Sequence[str],
         "IpV6Addresses": Sequence[str],
@@ -5789,14 +6395,54 @@
     {
         "MarketType": str,
         "SpotOptions": AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef,
     },
     total=False,
 )
 
+AwsEc2LaunchTemplateDataInstanceRequirementsDetailsOutputTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsOutputTypeDef",
+    {
+        "AcceleratorCount": (
+            AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef
+        ),
+        "AcceleratorManufacturers": List[str],
+        "AcceleratorNames": List[str],
+        "AcceleratorTotalMemoryMiB": (
+            AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef
+        ),
+        "AcceleratorTypes": List[str],
+        "BareMetal": str,
+        "BaselineEbsBandwidthMbps": (
+            AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef
+        ),
+        "BurstablePerformance": str,
+        "CpuManufacturers": List[str],
+        "ExcludedInstanceTypes": List[str],
+        "InstanceGenerations": List[str],
+        "LocalStorage": str,
+        "LocalStorageTypes": List[str],
+        "MemoryGiBPerVCpu": (
+            AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef
+        ),
+        "MemoryMiB": AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef,
+        "NetworkInterfaceCount": (
+            AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef
+        ),
+        "OnDemandMaxPricePercentageOverLowestPrice": int,
+        "RequireHibernateSupport": bool,
+        "SpotMaxPricePercentageOverLowestPrice": int,
+        "TotalLocalStorageGB": (
+            AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef
+        ),
+        "VCpuCount": AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef,
+    },
+    total=False,
+)
+
 AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef",
     {
         "AcceleratorCount": (
             AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef
         ),
         "AcceleratorManufacturers": Sequence[str],
@@ -5829,14 +6475,44 @@
             AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef
         ),
         "VCpuCount": AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef,
     },
     total=False,
 )
 
+AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsOutputTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsOutputTypeDef",
+    {
+        "AssociateCarrierIpAddress": bool,
+        "AssociatePublicIpAddress": bool,
+        "DeleteOnTermination": bool,
+        "Description": str,
+        "DeviceIndex": int,
+        "Groups": List[str],
+        "InterfaceType": str,
+        "Ipv4PrefixCount": int,
+        "Ipv4Prefixes": List[AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef],
+        "Ipv6AddressCount": int,
+        "Ipv6Addresses": List[
+            AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef
+        ],
+        "Ipv6PrefixCount": int,
+        "Ipv6Prefixes": List[AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef],
+        "NetworkCardIndex": int,
+        "NetworkInterfaceId": str,
+        "PrivateIpAddress": str,
+        "PrivateIpAddresses": List[
+            AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef
+        ],
+        "SecondaryPrivateIpAddressCount": int,
+        "SubnetId": str,
+    },
+    total=False,
+)
+
 AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef",
     {
         "AssociateCarrierIpAddress": bool,
         "AssociatePublicIpAddress": bool,
         "DeleteOnTermination": bool,
         "Description": str,
@@ -5878,14 +6554,29 @@
         "Protocol": str,
         "RuleAction": str,
         "RuleNumber": int,
     },
     total=False,
 )
 
+AwsEc2NetworkInterfaceDetailsOutputTypeDef = TypedDict(
+    "AwsEc2NetworkInterfaceDetailsOutputTypeDef",
+    {
+        "Attachment": AwsEc2NetworkInterfaceAttachmentTypeDef,
+        "NetworkInterfaceId": str,
+        "SecurityGroups": List[AwsEc2NetworkInterfaceSecurityGroupTypeDef],
+        "SourceDestCheck": bool,
+        "IpV6Addresses": List[AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef],
+        "PrivateIpAddresses": List[AwsEc2NetworkInterfacePrivateIpAddressDetailTypeDef],
+        "PublicDnsName": str,
+        "PublicIp": str,
+    },
+    total=False,
+)
+
 AwsEc2NetworkInterfaceDetailsTypeDef = TypedDict(
     "AwsEc2NetworkInterfaceDetailsTypeDef",
     {
         "Attachment": AwsEc2NetworkInterfaceAttachmentTypeDef,
         "NetworkInterfaceId": str,
         "SecurityGroups": Sequence[AwsEc2NetworkInterfaceSecurityGroupTypeDef],
         "SourceDestCheck": bool,
@@ -5893,28 +6584,62 @@
         "PrivateIpAddresses": Sequence[AwsEc2NetworkInterfacePrivateIpAddressDetailTypeDef],
         "PublicDnsName": str,
         "PublicIp": str,
     },
     total=False,
 )
 
+AwsEc2SecurityGroupIpPermissionOutputTypeDef = TypedDict(
+    "AwsEc2SecurityGroupIpPermissionOutputTypeDef",
+    {
+        "IpProtocol": str,
+        "FromPort": int,
+        "ToPort": int,
+        "UserIdGroupPairs": List[AwsEc2SecurityGroupUserIdGroupPairTypeDef],
+        "IpRanges": List[AwsEc2SecurityGroupIpRangeTypeDef],
+        "Ipv6Ranges": List[AwsEc2SecurityGroupIpv6RangeTypeDef],
+        "PrefixListIds": List[AwsEc2SecurityGroupPrefixListIdTypeDef],
+    },
+    total=False,
+)
+
 AwsEc2SecurityGroupIpPermissionTypeDef = TypedDict(
     "AwsEc2SecurityGroupIpPermissionTypeDef",
     {
         "IpProtocol": str,
         "FromPort": int,
         "ToPort": int,
         "UserIdGroupPairs": Sequence[AwsEc2SecurityGroupUserIdGroupPairTypeDef],
         "IpRanges": Sequence[AwsEc2SecurityGroupIpRangeTypeDef],
         "Ipv6Ranges": Sequence[AwsEc2SecurityGroupIpv6RangeTypeDef],
         "PrefixListIds": Sequence[AwsEc2SecurityGroupPrefixListIdTypeDef],
     },
     total=False,
 )
 
+AwsEc2SubnetDetailsOutputTypeDef = TypedDict(
+    "AwsEc2SubnetDetailsOutputTypeDef",
+    {
+        "AssignIpv6AddressOnCreation": bool,
+        "AvailabilityZone": str,
+        "AvailabilityZoneId": str,
+        "AvailableIpAddressCount": int,
+        "CidrBlock": str,
+        "DefaultForAz": bool,
+        "MapPublicIpOnLaunch": bool,
+        "OwnerId": str,
+        "State": str,
+        "SubnetArn": str,
+        "SubnetId": str,
+        "VpcId": str,
+        "Ipv6CidrBlockAssociationSet": List[Ipv6CidrBlockAssociationTypeDef],
+    },
+    total=False,
+)
+
 AwsEc2SubnetDetailsTypeDef = TypedDict(
     "AwsEc2SubnetDetailsTypeDef",
     {
         "AssignIpv6AddressOnCreation": bool,
         "AvailabilityZone": str,
         "AvailabilityZoneId": str,
         "AvailableIpAddressCount": int,
@@ -5927,14 +6652,32 @@
         "SubnetId": str,
         "VpcId": str,
         "Ipv6CidrBlockAssociationSet": Sequence[Ipv6CidrBlockAssociationTypeDef],
     },
     total=False,
 )
 
+AwsEc2VolumeDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VolumeDetailsOutputTypeDef",
+    {
+        "CreateTime": str,
+        "DeviceName": str,
+        "Encrypted": bool,
+        "Size": int,
+        "SnapshotId": str,
+        "Status": str,
+        "KmsKeyId": str,
+        "Attachments": List[AwsEc2VolumeAttachmentTypeDef],
+        "VolumeId": str,
+        "VolumeType": str,
+        "VolumeScanStatus": str,
+    },
+    total=False,
+)
+
 AwsEc2VolumeDetailsTypeDef = TypedDict(
     "AwsEc2VolumeDetailsTypeDef",
     {
         "CreateTime": str,
         "DeviceName": str,
         "Encrypted": bool,
         "Size": int,
@@ -5945,25 +6688,54 @@
         "VolumeId": str,
         "VolumeType": str,
         "VolumeScanStatus": str,
     },
     total=False,
 )
 
+AwsEc2VpcDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VpcDetailsOutputTypeDef",
+    {
+        "CidrBlockAssociationSet": List[CidrBlockAssociationTypeDef],
+        "Ipv6CidrBlockAssociationSet": List[Ipv6CidrBlockAssociationTypeDef],
+        "DhcpOptionsId": str,
+        "State": str,
+    },
+    total=False,
+)
+
 AwsEc2VpcDetailsTypeDef = TypedDict(
     "AwsEc2VpcDetailsTypeDef",
     {
         "CidrBlockAssociationSet": Sequence[CidrBlockAssociationTypeDef],
         "Ipv6CidrBlockAssociationSet": Sequence[Ipv6CidrBlockAssociationTypeDef],
         "DhcpOptionsId": str,
         "State": str,
     },
     total=False,
 )
 
+AwsEc2VpcEndpointServiceDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VpcEndpointServiceDetailsOutputTypeDef",
+    {
+        "AcceptanceRequired": bool,
+        "AvailabilityZones": List[str],
+        "BaseEndpointDnsNames": List[str],
+        "ManagesVpcEndpoints": bool,
+        "GatewayLoadBalancerArns": List[str],
+        "NetworkLoadBalancerArns": List[str],
+        "PrivateDnsName": str,
+        "ServiceId": str,
+        "ServiceName": str,
+        "ServiceState": str,
+        "ServiceType": List[AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef],
+    },
+    total=False,
+)
+
 AwsEc2VpcEndpointServiceDetailsTypeDef = TypedDict(
     "AwsEc2VpcEndpointServiceDetailsTypeDef",
     {
         "AcceptanceRequired": bool,
         "AvailabilityZones": Sequence[str],
         "BaseEndpointDnsNames": Sequence[str],
         "ManagesVpcEndpoints": bool,
@@ -5974,28 +6746,51 @@
         "ServiceName": str,
         "ServiceState": str,
         "ServiceType": Sequence[AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef],
     },
     total=False,
 )
 
+AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef",
+    {
+        "CidrBlock": str,
+        "CidrBlockSet": List[VpcInfoCidrBlockSetDetailsTypeDef],
+        "Ipv6CidrBlockSet": List[VpcInfoIpv6CidrBlockSetDetailsTypeDef],
+        "OwnerId": str,
+        "PeeringOptions": VpcInfoPeeringOptionsDetailsTypeDef,
+        "Region": str,
+        "VpcId": str,
+    },
+    total=False,
+)
+
 AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef = TypedDict(
     "AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef",
     {
         "CidrBlock": str,
         "CidrBlockSet": Sequence[VpcInfoCidrBlockSetDetailsTypeDef],
         "Ipv6CidrBlockSet": Sequence[VpcInfoIpv6CidrBlockSetDetailsTypeDef],
         "OwnerId": str,
         "PeeringOptions": VpcInfoPeeringOptionsDetailsTypeDef,
         "Region": str,
         "VpcId": str,
     },
     total=False,
 )
 
+AwsEc2VpnConnectionOptionsDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VpnConnectionOptionsDetailsOutputTypeDef",
+    {
+        "StaticRoutesOnly": bool,
+        "TunnelOptions": List[AwsEc2VpnConnectionOptionsTunnelOptionsDetailsOutputTypeDef],
+    },
+    total=False,
+)
+
 AwsEc2VpnConnectionOptionsDetailsTypeDef = TypedDict(
     "AwsEc2VpnConnectionOptionsDetailsTypeDef",
     {
         "StaticRoutesOnly": bool,
         "TunnelOptions": Sequence[AwsEc2VpnConnectionOptionsTunnelOptionsDetailsTypeDef],
     },
     total=False,
@@ -6022,14 +6817,25 @@
             AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef
         ),
         "Logging": str,
     },
     total=False,
 )
 
+AwsEcsContainerDetailsOutputTypeDef = TypedDict(
+    "AwsEcsContainerDetailsOutputTypeDef",
+    {
+        "Name": str,
+        "Image": str,
+        "MountPoints": List[AwsMountPointTypeDef],
+        "Privileged": bool,
+    },
+    total=False,
+)
+
 AwsEcsContainerDetailsTypeDef = TypedDict(
     "AwsEcsContainerDetailsTypeDef",
     {
         "Name": str,
         "Image": str,
         "MountPoints": Sequence[AwsMountPointTypeDef],
         "Privileged": bool,
@@ -6045,22 +6851,52 @@
         ),
         "MaximumPercent": int,
         "MinimumHealthyPercent": int,
     },
     total=False,
 )
 
+AwsEcsServiceNetworkConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsEcsServiceNetworkConfigurationDetailsOutputTypeDef",
+    {
+        "AwsVpcConfiguration": (
+            AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsOutputTypeDef
+        ),
+    },
+    total=False,
+)
+
 AwsEcsServiceNetworkConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsServiceNetworkConfigurationDetailsTypeDef",
     {
         "AwsVpcConfiguration": AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef,
     },
     total=False,
 )
 
+AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsOutputTypeDef",
+    {
+        "Capabilities": (
+            AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef
+        ),
+        "Devices": List[
+            AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsOutputTypeDef
+        ],
+        "InitProcessEnabled": bool,
+        "MaxSwap": int,
+        "SharedMemorySize": int,
+        "Swappiness": int,
+        "Tmpfs": List[
+            AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsOutputTypeDef
+        ],
+    },
+    total=False,
+)
+
 AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef",
     {
         "Capabilities": (
             AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef
         ),
         "Devices": Sequence[
@@ -6073,26 +6909,50 @@
         "Tmpfs": Sequence[
             AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsTypeDef
         ],
     },
     total=False,
 )
 
+AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsOutputTypeDef",
+    {
+        "LogDriver": str,
+        "Options": Dict[str, str],
+        "SecretOptions": List[
+            AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef
+        ],
+    },
+    total=False,
+)
+
 AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef",
     {
         "LogDriver": str,
         "Options": Mapping[str, str],
         "SecretOptions": Sequence[
             AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef
         ],
     },
     total=False,
 )
 
+AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef",
+    {
+        "ContainerName": str,
+        "ProxyConfigurationProperties": List[
+            AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef
+        ],
+        "Type": str,
+    },
+    total=False,
+)
+
 AwsEcsTaskDefinitionProxyConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionProxyConfigurationDetailsTypeDef",
     {
         "ContainerName": str,
         "ProxyConfigurationProperties": Sequence[
             AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef
         ],
@@ -6129,22 +6989,53 @@
     {
         "CreationInfo": AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef,
         "Path": str,
     },
     total=False,
 )
 
+AwsEksClusterLoggingDetailsOutputTypeDef = TypedDict(
+    "AwsEksClusterLoggingDetailsOutputTypeDef",
+    {
+        "ClusterLogging": List[AwsEksClusterLoggingClusterLoggingDetailsOutputTypeDef],
+    },
+    total=False,
+)
+
 AwsEksClusterLoggingDetailsTypeDef = TypedDict(
     "AwsEksClusterLoggingDetailsTypeDef",
     {
         "ClusterLogging": Sequence[AwsEksClusterLoggingClusterLoggingDetailsTypeDef],
     },
     total=False,
 )
 
+AwsElasticBeanstalkEnvironmentDetailsOutputTypeDef = TypedDict(
+    "AwsElasticBeanstalkEnvironmentDetailsOutputTypeDef",
+    {
+        "ApplicationName": str,
+        "Cname": str,
+        "DateCreated": str,
+        "DateUpdated": str,
+        "Description": str,
+        "EndpointUrl": str,
+        "EnvironmentArn": str,
+        "EnvironmentId": str,
+        "EnvironmentLinks": List[AwsElasticBeanstalkEnvironmentEnvironmentLinkTypeDef],
+        "EnvironmentName": str,
+        "OptionSettings": List[AwsElasticBeanstalkEnvironmentOptionSettingTypeDef],
+        "PlatformArn": str,
+        "SolutionStackName": str,
+        "Status": str,
+        "Tier": AwsElasticBeanstalkEnvironmentTierTypeDef,
+        "VersionLabel": str,
+    },
+    total=False,
+)
+
 AwsElasticBeanstalkEnvironmentDetailsTypeDef = TypedDict(
     "AwsElasticBeanstalkEnvironmentDetailsTypeDef",
     {
         "ApplicationName": str,
         "Cname": str,
         "DateCreated": str,
         "DateUpdated": str,
@@ -6186,45 +7077,94 @@
         "IndexSlowLogs": AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef,
         "SearchSlowLogs": AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef,
         "AuditLogs": AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef,
     },
     total=False,
 )
 
+AwsElbLoadBalancerPoliciesOutputTypeDef = TypedDict(
+    "AwsElbLoadBalancerPoliciesOutputTypeDef",
+    {
+        "AppCookieStickinessPolicies": List[AwsElbAppCookieStickinessPolicyTypeDef],
+        "LbCookieStickinessPolicies": List[AwsElbLbCookieStickinessPolicyTypeDef],
+        "OtherPolicies": List[str],
+    },
+    total=False,
+)
+
 AwsElbLoadBalancerPoliciesTypeDef = TypedDict(
     "AwsElbLoadBalancerPoliciesTypeDef",
     {
         "AppCookieStickinessPolicies": Sequence[AwsElbAppCookieStickinessPolicyTypeDef],
         "LbCookieStickinessPolicies": Sequence[AwsElbLbCookieStickinessPolicyTypeDef],
         "OtherPolicies": Sequence[str],
     },
     total=False,
 )
 
+AwsElbLoadBalancerAttributesOutputTypeDef = TypedDict(
+    "AwsElbLoadBalancerAttributesOutputTypeDef",
+    {
+        "AccessLog": AwsElbLoadBalancerAccessLogTypeDef,
+        "ConnectionDraining": AwsElbLoadBalancerConnectionDrainingTypeDef,
+        "ConnectionSettings": AwsElbLoadBalancerConnectionSettingsTypeDef,
+        "CrossZoneLoadBalancing": AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef,
+        "AdditionalAttributes": List[AwsElbLoadBalancerAdditionalAttributeTypeDef],
+    },
+    total=False,
+)
+
 AwsElbLoadBalancerAttributesTypeDef = TypedDict(
     "AwsElbLoadBalancerAttributesTypeDef",
     {
         "AccessLog": AwsElbLoadBalancerAccessLogTypeDef,
         "ConnectionDraining": AwsElbLoadBalancerConnectionDrainingTypeDef,
         "ConnectionSettings": AwsElbLoadBalancerConnectionSettingsTypeDef,
         "CrossZoneLoadBalancing": AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef,
         "AdditionalAttributes": Sequence[AwsElbLoadBalancerAdditionalAttributeTypeDef],
     },
     total=False,
 )
 
+AwsElbLoadBalancerListenerDescriptionOutputTypeDef = TypedDict(
+    "AwsElbLoadBalancerListenerDescriptionOutputTypeDef",
+    {
+        "Listener": AwsElbLoadBalancerListenerTypeDef,
+        "PolicyNames": List[str],
+    },
+    total=False,
+)
+
 AwsElbLoadBalancerListenerDescriptionTypeDef = TypedDict(
     "AwsElbLoadBalancerListenerDescriptionTypeDef",
     {
         "Listener": AwsElbLoadBalancerListenerTypeDef,
         "PolicyNames": Sequence[str],
     },
     total=False,
 )
 
+AwsElbv2LoadBalancerDetailsOutputTypeDef = TypedDict(
+    "AwsElbv2LoadBalancerDetailsOutputTypeDef",
+    {
+        "AvailabilityZones": List[AvailabilityZoneTypeDef],
+        "CanonicalHostedZoneId": str,
+        "CreatedTime": str,
+        "DNSName": str,
+        "IpAddressType": str,
+        "Scheme": str,
+        "SecurityGroups": List[str],
+        "State": LoadBalancerStateTypeDef,
+        "Type": str,
+        "VpcId": str,
+        "LoadBalancerAttributes": List[AwsElbv2LoadBalancerAttributeTypeDef],
+    },
+    total=False,
+)
+
 AwsElbv2LoadBalancerDetailsTypeDef = TypedDict(
     "AwsElbv2LoadBalancerDetailsTypeDef",
     {
         "AvailabilityZones": Sequence[AvailabilityZoneTypeDef],
         "CanonicalHostedZoneId": str,
         "CreatedTime": str,
         "DNSName": str,
@@ -6260,40 +7200,84 @@
     {
         "Attributes": AwsIamAccessKeySessionContextAttributesTypeDef,
         "SessionIssuer": AwsIamAccessKeySessionContextSessionIssuerTypeDef,
     },
     total=False,
 )
 
+AwsIamGroupDetailsOutputTypeDef = TypedDict(
+    "AwsIamGroupDetailsOutputTypeDef",
+    {
+        "AttachedManagedPolicies": List[AwsIamAttachedManagedPolicyTypeDef],
+        "CreateDate": str,
+        "GroupId": str,
+        "GroupName": str,
+        "GroupPolicyList": List[AwsIamGroupPolicyTypeDef],
+        "Path": str,
+    },
+    total=False,
+)
+
 AwsIamGroupDetailsTypeDef = TypedDict(
     "AwsIamGroupDetailsTypeDef",
     {
         "AttachedManagedPolicies": Sequence[AwsIamAttachedManagedPolicyTypeDef],
         "CreateDate": str,
         "GroupId": str,
         "GroupName": str,
         "GroupPolicyList": Sequence[AwsIamGroupPolicyTypeDef],
         "Path": str,
     },
     total=False,
 )
 
+AwsIamInstanceProfileOutputTypeDef = TypedDict(
+    "AwsIamInstanceProfileOutputTypeDef",
+    {
+        "Arn": str,
+        "CreateDate": str,
+        "InstanceProfileId": str,
+        "InstanceProfileName": str,
+        "Path": str,
+        "Roles": List[AwsIamInstanceProfileRoleTypeDef],
+    },
+    total=False,
+)
+
 AwsIamInstanceProfileTypeDef = TypedDict(
     "AwsIamInstanceProfileTypeDef",
     {
         "Arn": str,
         "CreateDate": str,
         "InstanceProfileId": str,
         "InstanceProfileName": str,
         "Path": str,
         "Roles": Sequence[AwsIamInstanceProfileRoleTypeDef],
     },
     total=False,
 )
 
+AwsIamPolicyDetailsOutputTypeDef = TypedDict(
+    "AwsIamPolicyDetailsOutputTypeDef",
+    {
+        "AttachmentCount": int,
+        "CreateDate": str,
+        "DefaultVersionId": str,
+        "Description": str,
+        "IsAttachable": bool,
+        "Path": str,
+        "PermissionsBoundaryUsageCount": int,
+        "PolicyId": str,
+        "PolicyName": str,
+        "PolicyVersionList": List[AwsIamPolicyVersionTypeDef],
+        "UpdateDate": str,
+    },
+    total=False,
+)
+
 AwsIamPolicyDetailsTypeDef = TypedDict(
     "AwsIamPolicyDetailsTypeDef",
     {
         "AttachmentCount": int,
         "CreateDate": str,
         "DefaultVersionId": str,
         "Description": str,
@@ -6304,14 +7288,29 @@
         "PolicyName": str,
         "PolicyVersionList": Sequence[AwsIamPolicyVersionTypeDef],
         "UpdateDate": str,
     },
     total=False,
 )
 
+AwsIamUserDetailsOutputTypeDef = TypedDict(
+    "AwsIamUserDetailsOutputTypeDef",
+    {
+        "AttachedManagedPolicies": List[AwsIamAttachedManagedPolicyTypeDef],
+        "CreateDate": str,
+        "GroupList": List[str],
+        "Path": str,
+        "PermissionsBoundary": AwsIamPermissionsBoundaryTypeDef,
+        "UserId": str,
+        "UserName": str,
+        "UserPolicyList": List[AwsIamUserPolicyTypeDef],
+    },
+    total=False,
+)
+
 AwsIamUserDetailsTypeDef = TypedDict(
     "AwsIamUserDetailsTypeDef",
     {
         "AttachedManagedPolicies": Sequence[AwsIamAttachedManagedPolicyTypeDef],
         "CreateDate": str,
         "GroupList": Sequence[str],
         "Path": str,
@@ -6331,23 +7330,49 @@
         "StreamEncryption": AwsKinesisStreamStreamEncryptionDetailsTypeDef,
         "ShardCount": int,
         "RetentionPeriodHours": int,
     },
     total=False,
 )
 
+AwsLambdaFunctionEnvironmentOutputTypeDef = TypedDict(
+    "AwsLambdaFunctionEnvironmentOutputTypeDef",
+    {
+        "Variables": Dict[str, str],
+        "Error": AwsLambdaFunctionEnvironmentErrorTypeDef,
+    },
+    total=False,
+)
+
 AwsLambdaFunctionEnvironmentTypeDef = TypedDict(
     "AwsLambdaFunctionEnvironmentTypeDef",
     {
         "Variables": Mapping[str, str],
         "Error": AwsLambdaFunctionEnvironmentErrorTypeDef,
     },
     total=False,
 )
 
+AwsNetworkFirewallFirewallDetailsOutputTypeDef = TypedDict(
+    "AwsNetworkFirewallFirewallDetailsOutputTypeDef",
+    {
+        "DeleteProtection": bool,
+        "Description": str,
+        "FirewallArn": str,
+        "FirewallId": str,
+        "FirewallName": str,
+        "FirewallPolicyArn": str,
+        "FirewallPolicyChangeProtection": bool,
+        "SubnetChangeProtection": bool,
+        "SubnetMappings": List[AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef],
+        "VpcId": str,
+    },
+    total=False,
+)
+
 AwsNetworkFirewallFirewallDetailsTypeDef = TypedDict(
     "AwsNetworkFirewallFirewallDetailsTypeDef",
     {
         "DeleteProtection": bool,
         "Description": str,
         "FirewallArn": str,
         "FirewallId": str,
@@ -6396,14 +7421,58 @@
         "IndexSlowLogs": AwsOpenSearchServiceDomainLogPublishingOptionTypeDef,
         "SearchSlowLogs": AwsOpenSearchServiceDomainLogPublishingOptionTypeDef,
         "AuditLogs": AwsOpenSearchServiceDomainLogPublishingOptionTypeDef,
     },
     total=False,
 )
 
+AwsRdsDbClusterDetailsOutputTypeDef = TypedDict(
+    "AwsRdsDbClusterDetailsOutputTypeDef",
+    {
+        "AllocatedStorage": int,
+        "AvailabilityZones": List[str],
+        "BackupRetentionPeriod": int,
+        "DatabaseName": str,
+        "Status": str,
+        "Endpoint": str,
+        "ReaderEndpoint": str,
+        "CustomEndpoints": List[str],
+        "MultiAz": bool,
+        "Engine": str,
+        "EngineVersion": str,
+        "Port": int,
+        "MasterUsername": str,
+        "PreferredBackupWindow": str,
+        "PreferredMaintenanceWindow": str,
+        "ReadReplicaIdentifiers": List[str],
+        "VpcSecurityGroups": List[AwsRdsDbInstanceVpcSecurityGroupTypeDef],
+        "HostedZoneId": str,
+        "StorageEncrypted": bool,
+        "KmsKeyId": str,
+        "DbClusterResourceId": str,
+        "AssociatedRoles": List[AwsRdsDbClusterAssociatedRoleTypeDef],
+        "ClusterCreateTime": str,
+        "EnabledCloudWatchLogsExports": List[str],
+        "EngineMode": str,
+        "DeletionProtection": bool,
+        "HttpEndpointEnabled": bool,
+        "ActivityStreamStatus": str,
+        "CopyTagsToSnapshot": bool,
+        "CrossAccountClone": bool,
+        "DomainMemberships": List[AwsRdsDbDomainMembershipTypeDef],
+        "DbClusterParameterGroup": str,
+        "DbSubnetGroup": str,
+        "DbClusterOptionGroupMemberships": List[AwsRdsDbClusterOptionGroupMembershipTypeDef],
+        "DbClusterIdentifier": str,
+        "DbClusterMembers": List[AwsRdsDbClusterMemberTypeDef],
+        "IamDatabaseAuthenticationEnabled": bool,
+    },
+    total=False,
+)
+
 AwsRdsDbClusterDetailsTypeDef = TypedDict(
     "AwsRdsDbClusterDetailsTypeDef",
     {
         "AllocatedStorage": int,
         "AvailabilityZones": Sequence[str],
         "BackupRetentionPeriod": int,
         "DatabaseName": str,
@@ -6440,14 +7509,48 @@
         "DbClusterIdentifier": str,
         "DbClusterMembers": Sequence[AwsRdsDbClusterMemberTypeDef],
         "IamDatabaseAuthenticationEnabled": bool,
     },
     total=False,
 )
 
+AwsRdsDbSnapshotDetailsOutputTypeDef = TypedDict(
+    "AwsRdsDbSnapshotDetailsOutputTypeDef",
+    {
+        "DbSnapshotIdentifier": str,
+        "DbInstanceIdentifier": str,
+        "SnapshotCreateTime": str,
+        "Engine": str,
+        "AllocatedStorage": int,
+        "Status": str,
+        "Port": int,
+        "AvailabilityZone": str,
+        "VpcId": str,
+        "InstanceCreateTime": str,
+        "MasterUsername": str,
+        "EngineVersion": str,
+        "LicenseModel": str,
+        "SnapshotType": str,
+        "Iops": int,
+        "OptionGroupName": str,
+        "PercentProgress": int,
+        "SourceRegion": str,
+        "SourceDbSnapshotIdentifier": str,
+        "StorageType": str,
+        "TdeCredentialArn": str,
+        "Encrypted": bool,
+        "KmsKeyId": str,
+        "Timezone": str,
+        "IamDatabaseAuthenticationEnabled": bool,
+        "ProcessorFeatures": List[AwsRdsDbProcessorFeatureTypeDef],
+        "DbiResourceId": str,
+    },
+    total=False,
+)
+
 AwsRdsDbSnapshotDetailsTypeDef = TypedDict(
     "AwsRdsDbSnapshotDetailsTypeDef",
     {
         "DbSnapshotIdentifier": str,
         "DbInstanceIdentifier": str,
         "SnapshotCreateTime": str,
         "Engine": str,
@@ -6474,14 +7577,36 @@
         "IamDatabaseAuthenticationEnabled": bool,
         "ProcessorFeatures": Sequence[AwsRdsDbProcessorFeatureTypeDef],
         "DbiResourceId": str,
     },
     total=False,
 )
 
+AwsRdsDbPendingModifiedValuesOutputTypeDef = TypedDict(
+    "AwsRdsDbPendingModifiedValuesOutputTypeDef",
+    {
+        "DbInstanceClass": str,
+        "AllocatedStorage": int,
+        "MasterUserPassword": str,
+        "Port": int,
+        "BackupRetentionPeriod": int,
+        "MultiAZ": bool,
+        "EngineVersion": str,
+        "LicenseModel": str,
+        "Iops": int,
+        "DbInstanceIdentifier": str,
+        "StorageType": str,
+        "CaCertificateIdentifier": str,
+        "DbSubnetGroupName": str,
+        "PendingCloudWatchLogsExports": AwsRdsPendingCloudWatchLogsExportsOutputTypeDef,
+        "ProcessorFeatures": List[AwsRdsDbProcessorFeatureTypeDef],
+    },
+    total=False,
+)
+
 AwsRdsDbPendingModifiedValuesTypeDef = TypedDict(
     "AwsRdsDbPendingModifiedValuesTypeDef",
     {
         "DbInstanceClass": str,
         "AllocatedStorage": int,
         "MasterUserPassword": str,
         "Port": int,
@@ -6496,14 +7621,28 @@
         "DbSubnetGroupName": str,
         "PendingCloudWatchLogsExports": AwsRdsPendingCloudWatchLogsExportsTypeDef,
         "ProcessorFeatures": Sequence[AwsRdsDbProcessorFeatureTypeDef],
     },
     total=False,
 )
 
+AwsRdsDbSecurityGroupDetailsOutputTypeDef = TypedDict(
+    "AwsRdsDbSecurityGroupDetailsOutputTypeDef",
+    {
+        "DbSecurityGroupArn": str,
+        "DbSecurityGroupDescription": str,
+        "DbSecurityGroupName": str,
+        "Ec2SecurityGroups": List[AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef],
+        "IpRanges": List[AwsRdsDbSecurityGroupIpRangeTypeDef],
+        "OwnerId": str,
+        "VpcId": str,
+    },
+    total=False,
+)
+
 AwsRdsDbSecurityGroupDetailsTypeDef = TypedDict(
     "AwsRdsDbSecurityGroupDetailsTypeDef",
     {
         "DbSecurityGroupArn": str,
         "DbSecurityGroupDescription": str,
         "DbSecurityGroupName": str,
         "Ec2SecurityGroups": Sequence[AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef],
@@ -6520,14 +7659,24 @@
         "SubnetIdentifier": str,
         "SubnetAvailabilityZone": AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef,
         "SubnetStatus": str,
     },
     total=False,
 )
 
+AwsRedshiftClusterClusterParameterGroupOutputTypeDef = TypedDict(
+    "AwsRedshiftClusterClusterParameterGroupOutputTypeDef",
+    {
+        "ClusterParameterStatusList": List[AwsRedshiftClusterClusterParameterStatusTypeDef],
+        "ParameterApplyStatus": str,
+        "ParameterGroupName": str,
+    },
+    total=False,
+)
+
 AwsRedshiftClusterClusterParameterGroupTypeDef = TypedDict(
     "AwsRedshiftClusterClusterParameterGroupTypeDef",
     {
         "ClusterParameterStatusList": Sequence[AwsRedshiftClusterClusterParameterStatusTypeDef],
         "ParameterApplyStatus": str,
         "ParameterGroupName": str,
     },
@@ -6540,14 +7689,22 @@
         "Prefix": str,
         "Tag": AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsTypeDef,
         "Type": str,
     },
     total=False,
 )
 
+AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef = TypedDict(
+    "AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef",
+    {
+        "FilterRules": List[AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef],
+    },
+    total=False,
+)
+
 AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef",
     {
         "FilterRules": Sequence[AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef],
     },
     total=False,
 )
@@ -6573,14 +7730,43 @@
     {
         "Condition": AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef,
         "Redirect": AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef,
     },
     total=False,
 )
 
+AwsSageMakerNotebookInstanceDetailsOutputTypeDef = TypedDict(
+    "AwsSageMakerNotebookInstanceDetailsOutputTypeDef",
+    {
+        "AcceleratorTypes": List[str],
+        "AdditionalCodeRepositories": List[str],
+        "DefaultCodeRepository": str,
+        "DirectInternetAccess": str,
+        "FailureReason": str,
+        "InstanceMetadataServiceConfiguration": (
+            AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef
+        ),
+        "InstanceType": str,
+        "KmsKeyId": str,
+        "NetworkInterfaceId": str,
+        "NotebookInstanceArn": str,
+        "NotebookInstanceLifecycleConfigName": str,
+        "NotebookInstanceName": str,
+        "NotebookInstanceStatus": str,
+        "PlatformIdentifier": str,
+        "RoleArn": str,
+        "RootAccess": str,
+        "SecurityGroups": List[str],
+        "SubnetId": str,
+        "Url": str,
+        "VolumeSizeInGB": int,
+    },
+    total=False,
+)
+
 AwsSageMakerNotebookInstanceDetailsTypeDef = TypedDict(
     "AwsSageMakerNotebookInstanceDetailsTypeDef",
     {
         "AcceleratorTypes": Sequence[str],
         "AdditionalCodeRepositories": Sequence[str],
         "DefaultCodeRepository": str,
         "DirectInternetAccess": str,
@@ -6654,58 +7840,32 @@
     {
         "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
 )
 
-_RequiredGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
+AwsSnsTopicDetailsOutputTypeDef = TypedDict(
+    "AwsSnsTopicDetailsOutputTypeDef",
     {
-        "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
-    },
-)
-_OptionalGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef(
-    _RequiredGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
-    _OptionalGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
-):
-    pass
-
-_RequiredGetFindingHistoryRequestRequestTypeDef = TypedDict(
-    "_RequiredGetFindingHistoryRequestRequestTypeDef",
-    {
-        "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
-    },
-)
-_OptionalGetFindingHistoryRequestRequestTypeDef = TypedDict(
-    "_OptionalGetFindingHistoryRequestRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "NextToken": str,
-        "MaxResults": int,
+        "KmsMasterKeyId": str,
+        "Subscription": List[AwsSnsTopicSubscriptionTypeDef],
+        "TopicName": str,
+        "Owner": str,
+        "SqsSuccessFeedbackRoleArn": str,
+        "SqsFailureFeedbackRoleArn": str,
+        "ApplicationSuccessFeedbackRoleArn": str,
+        "FirehoseSuccessFeedbackRoleArn": str,
+        "FirehoseFailureFeedbackRoleArn": str,
+        "HttpSuccessFeedbackRoleArn": str,
+        "HttpFailureFeedbackRoleArn": str,
     },
     total=False,
 )
 
-class GetFindingHistoryRequestRequestTypeDef(
-    _RequiredGetFindingHistoryRequestRequestTypeDef, _OptionalGetFindingHistoryRequestRequestTypeDef
-):
-    pass
-
 AwsSnsTopicDetailsTypeDef = TypedDict(
     "AwsSnsTopicDetailsTypeDef",
     {
         "KmsMasterKeyId": str,
         "Subscription": Sequence[AwsSnsTopicSubscriptionTypeDef],
         "TopicName": str,
         "Owner": str,
@@ -6732,40 +7892,77 @@
     "AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef",
     {
         "CloudWatchLogsLogGroup": AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef,
     },
     total=False,
 )
 
+AwsWafRateBasedRuleDetailsOutputTypeDef = TypedDict(
+    "AwsWafRateBasedRuleDetailsOutputTypeDef",
+    {
+        "MetricName": str,
+        "Name": str,
+        "RateKey": str,
+        "RateLimit": int,
+        "RuleId": str,
+        "MatchPredicates": List[AwsWafRateBasedRuleMatchPredicateTypeDef],
+    },
+    total=False,
+)
+
 AwsWafRateBasedRuleDetailsTypeDef = TypedDict(
     "AwsWafRateBasedRuleDetailsTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "RateKey": str,
         "RateLimit": int,
         "RuleId": str,
         "MatchPredicates": Sequence[AwsWafRateBasedRuleMatchPredicateTypeDef],
     },
     total=False,
 )
 
+AwsWafRegionalRateBasedRuleDetailsOutputTypeDef = TypedDict(
+    "AwsWafRegionalRateBasedRuleDetailsOutputTypeDef",
+    {
+        "MetricName": str,
+        "Name": str,
+        "RateKey": str,
+        "RateLimit": int,
+        "RuleId": str,
+        "MatchPredicates": List[AwsWafRegionalRateBasedRuleMatchPredicateTypeDef],
+    },
+    total=False,
+)
+
 AwsWafRegionalRateBasedRuleDetailsTypeDef = TypedDict(
     "AwsWafRegionalRateBasedRuleDetailsTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "RateKey": str,
         "RateLimit": int,
         "RuleId": str,
         "MatchPredicates": Sequence[AwsWafRegionalRateBasedRuleMatchPredicateTypeDef],
     },
     total=False,
 )
 
+AwsWafRegionalRuleDetailsOutputTypeDef = TypedDict(
+    "AwsWafRegionalRuleDetailsOutputTypeDef",
+    {
+        "MetricName": str,
+        "Name": str,
+        "PredicateList": List[AwsWafRegionalRulePredicateListDetailsTypeDef],
+        "RuleId": str,
+    },
+    total=False,
+)
+
 AwsWafRegionalRuleDetailsTypeDef = TypedDict(
     "AwsWafRegionalRuleDetailsTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "PredicateList": Sequence[AwsWafRegionalRulePredicateListDetailsTypeDef],
         "RuleId": str,
@@ -6792,14 +7989,25 @@
         "Priority": int,
         "RuleId": str,
         "Type": str,
     },
     total=False,
 )
 
+AwsWafRuleDetailsOutputTypeDef = TypedDict(
+    "AwsWafRuleDetailsOutputTypeDef",
+    {
+        "MetricName": str,
+        "Name": str,
+        "PredicateList": List[AwsWafRulePredicateListDetailsTypeDef],
+        "RuleId": str,
+    },
+    total=False,
+)
+
 AwsWafRuleDetailsTypeDef = TypedDict(
     "AwsWafRuleDetailsTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "PredicateList": Sequence[AwsWafRulePredicateListDetailsTypeDef],
         "RuleId": str,
@@ -6814,35 +8022,66 @@
         "Priority": int,
         "RuleId": str,
         "Type": str,
     },
     total=False,
 )
 
+AwsWafWebAclRuleOutputTypeDef = TypedDict(
+    "AwsWafWebAclRuleOutputTypeDef",
+    {
+        "Action": WafActionTypeDef,
+        "ExcludedRules": List[WafExcludedRuleTypeDef],
+        "OverrideAction": WafOverrideActionTypeDef,
+        "Priority": int,
+        "RuleId": str,
+        "Type": str,
+    },
+    total=False,
+)
+
 AwsWafWebAclRuleTypeDef = TypedDict(
     "AwsWafWebAclRuleTypeDef",
     {
         "Action": WafActionTypeDef,
         "ExcludedRules": Sequence[WafExcludedRuleTypeDef],
         "OverrideAction": WafOverrideActionTypeDef,
         "Priority": int,
         "RuleId": str,
         "Type": str,
     },
     total=False,
 )
 
+AwsWafv2CustomRequestHandlingDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2CustomRequestHandlingDetailsOutputTypeDef",
+    {
+        "InsertHeaders": List[AwsWafv2CustomHttpHeaderTypeDef],
+    },
+    total=False,
+)
+
 AwsWafv2CustomRequestHandlingDetailsTypeDef = TypedDict(
     "AwsWafv2CustomRequestHandlingDetailsTypeDef",
     {
         "InsertHeaders": Sequence[AwsWafv2CustomHttpHeaderTypeDef],
     },
     total=False,
 )
 
+AwsWafv2CustomResponseDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2CustomResponseDetailsOutputTypeDef",
+    {
+        "CustomResponseBodyKey": str,
+        "ResponseCode": int,
+        "ResponseHeaders": List[AwsWafv2CustomHttpHeaderTypeDef],
+    },
+    total=False,
+)
+
 AwsWafv2CustomResponseDetailsTypeDef = TypedDict(
     "AwsWafv2CustomResponseDetailsTypeDef",
     {
         "CustomResponseBodyKey": str,
         "ResponseCode": int,
         "ResponseHeaders": Sequence[AwsWafv2CustomHttpHeaderTypeDef],
     },
@@ -6853,29 +8092,183 @@
     "AwsWafv2WebAclCaptchaConfigDetailsTypeDef",
     {
         "ImmunityTimeProperty": AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef,
     },
     total=False,
 )
 
+CreateActionTargetResponseTypeDef = TypedDict(
+    "CreateActionTargetResponseTypeDef",
+    {
+        "ActionTargetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAutomationRuleResponseTypeDef = TypedDict(
+    "CreateAutomationRuleResponseTypeDef",
+    {
+        "RuleArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFindingAggregatorResponseTypeDef = TypedDict(
+    "CreateFindingAggregatorResponseTypeDef",
+    {
+        "FindingAggregatorArn": str,
+        "FindingAggregationRegion": str,
+        "RegionLinkingMode": str,
+        "Regions": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateInsightResponseTypeDef = TypedDict(
+    "CreateInsightResponseTypeDef",
+    {
+        "InsightArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteActionTargetResponseTypeDef = TypedDict(
+    "DeleteActionTargetResponseTypeDef",
+    {
+        "ActionTargetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteInsightResponseTypeDef = TypedDict(
+    "DeleteInsightResponseTypeDef",
+    {
+        "InsightArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeActionTargetsResponseTypeDef = TypedDict(
+    "DescribeActionTargetsResponseTypeDef",
+    {
+        "ActionTargets": List[ActionTargetTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeHubResponseTypeDef = TypedDict(
+    "DescribeHubResponseTypeDef",
+    {
+        "HubArn": str,
+        "SubscribedAt": str,
+        "AutoEnableControls": bool,
+        "ControlFindingGenerator": ControlFindingGeneratorType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
+    "DescribeOrganizationConfigurationResponseTypeDef",
+    {
+        "AutoEnable": bool,
+        "MemberAccountLimitReached": bool,
+        "AutoEnableStandards": AutoEnableStandardsType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EnableImportFindingsForProductResponseTypeDef = TypedDict(
+    "EnableImportFindingsForProductResponseTypeDef",
+    {
+        "ProductSubscriptionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFindingAggregatorResponseTypeDef = TypedDict(
+    "GetFindingAggregatorResponseTypeDef",
+    {
+        "FindingAggregatorArn": str,
+        "FindingAggregationRegion": str,
+        "RegionLinkingMode": str,
+        "Regions": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetInvitationsCountResponseTypeDef = TypedDict(
+    "GetInvitationsCountResponseTypeDef",
+    {
+        "InvitationsCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAutomationRulesResponseTypeDef = TypedDict(
+    "ListAutomationRulesResponseTypeDef",
+    {
+        "AutomationRulesMetadata": List[AutomationRulesMetadataTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListEnabledProductsForImportResponseTypeDef = TypedDict(
+    "ListEnabledProductsForImportResponseTypeDef",
+    {
+        "ProductSubscriptions": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
+    "ListOrganizationAdminAccountsResponseTypeDef",
+    {
+        "AdminAccounts": List[AdminAccountTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFindingAggregatorResponseTypeDef = TypedDict(
+    "UpdateFindingAggregatorResponseTypeDef",
+    {
+        "FindingAggregatorArn": str,
+        "FindingAggregationRegion": str,
+        "RegionLinkingMode": str,
+        "Regions": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 BatchDeleteAutomationRulesResponseTypeDef = TypedDict(
     "BatchDeleteAutomationRulesResponseTypeDef",
     {
         "ProcessedAutomationRules": List[str],
         "UnprocessedAutomationRules": List[UnprocessedAutomationRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateAutomationRulesResponseTypeDef = TypedDict(
     "BatchUpdateAutomationRulesResponseTypeDef",
     {
         "ProcessedAutomationRules": List[str],
         "UnprocessedAutomationRules": List[UnprocessedAutomationRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchEnableStandardsRequestRequestTypeDef = TypedDict(
     "BatchEnableStandardsRequestRequestTypeDef",
     {
         "StandardsSubscriptionRequests": Sequence[StandardsSubscriptionRequestTypeDef],
@@ -6883,15 +8276,15 @@
 )
 
 BatchGetSecurityControlsResponseTypeDef = TypedDict(
     "BatchGetSecurityControlsResponseTypeDef",
     {
         "SecurityControls": List[SecurityControlTypeDef],
         "UnprocessedIds": List[UnprocessedSecurityControlTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetStandardsControlAssociationsRequestRequestTypeDef = TypedDict(
     "BatchGetStandardsControlAssociationsRequestRequestTypeDef",
     {
         "StandardsControlAssociationIds": Sequence[StandardsControlAssociationIdTypeDef],
@@ -6921,15 +8314,15 @@
 
 BatchImportFindingsResponseTypeDef = TypedDict(
     "BatchImportFindingsResponseTypeDef",
     {
         "FailedCount": int,
         "SuccessCount": int,
         "FailedFindings": List[ImportFindingsErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateStandardsControlAssociationsRequestRequestTypeDef = TypedDict(
     "BatchUpdateStandardsControlAssociationsRequestRequestTypeDef",
     {
         "StandardsControlAssociationUpdates": Sequence[StandardsControlAssociationUpdateTypeDef],
@@ -6953,26 +8346,52 @@
 
 class UnprocessedStandardsControlAssociationUpdateTypeDef(
     _RequiredUnprocessedStandardsControlAssociationUpdateTypeDef,
     _OptionalUnprocessedStandardsControlAssociationUpdateTypeDef,
 ):
     pass
 
+ComplianceOutputTypeDef = TypedDict(
+    "ComplianceOutputTypeDef",
+    {
+        "Status": ComplianceStatusType,
+        "RelatedRequirements": List[str],
+        "StatusReasons": List[StatusReasonTypeDef],
+        "SecurityControlId": str,
+        "AssociatedStandards": List[AssociatedStandardTypeDef],
+    },
+    total=False,
+)
+
 ComplianceTypeDef = TypedDict(
     "ComplianceTypeDef",
     {
         "Status": ComplianceStatusType,
         "RelatedRequirements": Sequence[str],
         "StatusReasons": Sequence[StatusReasonTypeDef],
         "SecurityControlId": str,
         "AssociatedStandards": Sequence[AssociatedStandardTypeDef],
     },
     total=False,
 )
 
+ContainerDetailsOutputTypeDef = TypedDict(
+    "ContainerDetailsOutputTypeDef",
+    {
+        "ContainerRuntime": str,
+        "Name": str,
+        "ImageId": str,
+        "ImageName": str,
+        "LaunchedAt": str,
+        "VolumeMounts": List[VolumeMountTypeDef],
+        "Privileged": bool,
+    },
+    total=False,
+)
+
 ContainerDetailsTypeDef = TypedDict(
     "ContainerDetailsTypeDef",
     {
         "ContainerRuntime": str,
         "Name": str,
         "ImageId": str,
         "ImageName": str,
@@ -6983,78 +8402,223 @@
     total=False,
 )
 
 CreateMembersResponseTypeDef = TypedDict(
     "CreateMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[ResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeclineInvitationsResponseTypeDef = TypedDict(
     "DeclineInvitationsResponseTypeDef",
     {
         "UnprocessedAccounts": List[ResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteInvitationsResponseTypeDef = TypedDict(
     "DeleteInvitationsResponseTypeDef",
     {
         "UnprocessedAccounts": List[ResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteMembersResponseTypeDef = TypedDict(
     "DeleteMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[ResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InviteMembersResponseTypeDef = TypedDict(
     "InviteMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[ResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DateFilterTypeDef = TypedDict(
     "DateFilterTypeDef",
     {
         "Start": str,
         "End": str,
         "DateRange": DateRangeTypeDef,
     },
     total=False,
 )
 
+DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef = TypedDict(
+    "DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef",
+    {
+        "ActionTargetArns": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeProductsRequestDescribeProductsPaginateTypeDef = TypedDict(
+    "DescribeProductsRequestDescribeProductsPaginateTypeDef",
+    {
+        "ProductArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef",
+    {
+        "StandardsSubscriptionArn": str,
+    },
+)
+_OptionalDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef(
+    _RequiredDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
+    _OptionalDescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
+):
+    pass
+
+DescribeStandardsRequestDescribeStandardsPaginateTypeDef = TypedDict(
+    "DescribeStandardsRequestDescribeStandardsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef = TypedDict(
+    "GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef",
+    {
+        "StandardsSubscriptionArns": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetInsightsRequestGetInsightsPaginateTypeDef = TypedDict(
+    "GetInsightsRequestGetInsightsPaginateTypeDef",
+    {
+        "InsightArns": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef = TypedDict(
+    "ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef = TypedDict(
+    "ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListInvitationsRequestListInvitationsPaginateTypeDef = TypedDict(
+    "ListInvitationsRequestListInvitationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListMembersRequestListMembersPaginateTypeDef = TypedDict(
+    "ListMembersRequestListMembersPaginateTypeDef",
+    {
+        "OnlyAssociated": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef = TypedDict(
+    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef = TypedDict(
+    "ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef",
+    {
+        "StandardsArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef",
+    {
+        "SecurityControlId": str,
+    },
+)
+_OptionalListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef(
+    _RequiredListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef,
+    _OptionalListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef,
+):
+    pass
+
 DescribeProductsResponseTypeDef = TypedDict(
     "DescribeProductsResponseTypeDef",
     {
         "Products": List[ProductTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStandardsControlsResponseTypeDef = TypedDict(
     "DescribeStandardsControlsResponseTypeDef",
     {
         "Controls": List[StandardsControlTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ThreatOutputTypeDef = TypedDict(
+    "ThreatOutputTypeDef",
+    {
+        "Name": str,
+        "Severity": str,
+        "ItemCount": int,
+        "FilePaths": List[FilePathsTypeDef],
+    },
+    total=False,
+)
+
 ThreatTypeDef = TypedDict(
     "ThreatTypeDef",
     {
         "Name": str,
         "Severity": str,
         "ItemCount": int,
         "FilePaths": Sequence[FilePathsTypeDef],
@@ -7063,15 +8627,15 @@
 )
 
 ListFindingAggregatorsResponseTypeDef = TypedDict(
     "ListFindingAggregatorsResponseTypeDef",
     {
         "FindingAggregators": List[FindingAggregatorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FindingHistoryRecordTypeDef = TypedDict(
     "FindingHistoryRecordTypeDef",
     {
         "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
@@ -7080,14 +8644,26 @@
         "UpdateSource": FindingHistoryUpdateSourceTypeDef,
         "Updates": List[FindingHistoryUpdateTypeDef],
         "NextToken": str,
     },
     total=False,
 )
 
+FindingProviderFieldsOutputTypeDef = TypedDict(
+    "FindingProviderFieldsOutputTypeDef",
+    {
+        "Confidence": int,
+        "Criticality": int,
+        "RelatedFindings": List[RelatedFindingTypeDef],
+        "Severity": FindingProviderSeverityTypeDef,
+        "Types": List[str],
+    },
+    total=False,
+)
+
 FindingProviderFieldsTypeDef = TypedDict(
     "FindingProviderFieldsTypeDef",
     {
         "Confidence": int,
         "Criticality": int,
         "RelatedFindings": Sequence[RelatedFindingTypeDef],
         "Severity": FindingProviderSeverityTypeDef,
@@ -7096,50 +8672,94 @@
     total=False,
 )
 
 GetAdministratorAccountResponseTypeDef = TypedDict(
     "GetAdministratorAccountResponseTypeDef",
     {
         "Administrator": InvitationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMasterAccountResponseTypeDef = TypedDict(
     "GetMasterAccountResponseTypeDef",
     {
         "Master": InvitationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInvitationsResponseTypeDef = TypedDict(
     "ListInvitationsResponseTypeDef",
     {
         "Invitations": List[InvitationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
+    {
+        "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
+    },
+)
+_OptionalGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef(
+    _RequiredGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
+    _OptionalGetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
+):
+    pass
+
+_RequiredGetFindingHistoryRequestRequestTypeDef = TypedDict(
+    "_RequiredGetFindingHistoryRequestRequestTypeDef",
+    {
+        "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
+    },
+)
+_OptionalGetFindingHistoryRequestRequestTypeDef = TypedDict(
+    "_OptionalGetFindingHistoryRequestRequestTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
     },
+    total=False,
 )
 
+class GetFindingHistoryRequestRequestTypeDef(
+    _RequiredGetFindingHistoryRequestRequestTypeDef, _OptionalGetFindingHistoryRequestRequestTypeDef
+):
+    pass
+
 GetMembersResponseTypeDef = TypedDict(
     "GetMembersResponseTypeDef",
     {
         "Members": List[MemberTypeDef],
         "UnprocessedAccounts": List[ResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMembersResponseTypeDef = TypedDict(
     "ListMembersResponseTypeDef",
     {
         "Members": List[MemberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InsightResultsTypeDef = TypedDict(
     "InsightResultsTypeDef",
     {
         "InsightArn": str,
@@ -7149,27 +8769,36 @@
 )
 
 ListSecurityControlDefinitionsResponseTypeDef = TypedDict(
     "ListSecurityControlDefinitionsResponseTypeDef",
     {
         "SecurityControlDefinitions": List[SecurityControlDefinitionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStandardsControlAssociationsResponseTypeDef = TypedDict(
     "ListStandardsControlAssociationsResponseTypeDef",
     {
         "StandardsControlAssociationSummaries": List[StandardsControlAssociationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+NetworkPathComponentDetailsOutputTypeDef = TypedDict(
+    "NetworkPathComponentDetailsOutputTypeDef",
+    {
+        "Address": List[str],
+        "PortRanges": List[PortRangeTypeDef],
+    },
+    total=False,
+)
+
 NetworkPathComponentDetailsTypeDef = TypedDict(
     "NetworkPathComponentDetailsTypeDef",
     {
         "Address": Sequence[str],
         "PortRanges": Sequence[PortRangeTypeDef],
     },
     total=False,
@@ -7208,24 +8837,49 @@
     "RemediationTypeDef",
     {
         "Recommendation": RecommendationTypeDef,
     },
     total=False,
 )
 
+RuleGroupSourceStatefulRulesDetailsOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatefulRulesDetailsOutputTypeDef",
+    {
+        "Action": str,
+        "Header": RuleGroupSourceStatefulRulesHeaderDetailsTypeDef,
+        "RuleOptions": List[RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef],
+    },
+    total=False,
+)
+
 RuleGroupSourceStatefulRulesDetailsTypeDef = TypedDict(
     "RuleGroupSourceStatefulRulesDetailsTypeDef",
     {
         "Action": str,
         "Header": RuleGroupSourceStatefulRulesHeaderDetailsTypeDef,
         "RuleOptions": Sequence[RuleGroupSourceStatefulRulesOptionsDetailsTypeDef],
     },
     total=False,
 )
 
+RuleGroupSourceStatelessRuleMatchAttributesOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRuleMatchAttributesOutputTypeDef",
+    {
+        "DestinationPorts": List[
+            RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef
+        ],
+        "Destinations": List[RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef],
+        "Protocols": List[int],
+        "SourcePorts": List[RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef],
+        "Sources": List[RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef],
+        "TcpFlags": List[RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef],
+    },
+    total=False,
+)
+
 RuleGroupSourceStatelessRuleMatchAttributesTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesTypeDef",
     {
         "DestinationPorts": Sequence[
             RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef
         ],
         "Destinations": Sequence[RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef],
@@ -7233,14 +8887,23 @@
         "SourcePorts": Sequence[RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef],
         "Sources": Sequence[RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef],
         "TcpFlags": Sequence[RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef],
     },
     total=False,
 )
 
+RuleGroupVariablesOutputTypeDef = TypedDict(
+    "RuleGroupVariablesOutputTypeDef",
+    {
+        "IpSets": RuleGroupVariablesIpSetsDetailsOutputTypeDef,
+        "PortSets": RuleGroupVariablesPortSetsDetailsOutputTypeDef,
+    },
+    total=False,
+)
+
 RuleGroupVariablesTypeDef = TypedDict(
     "RuleGroupVariablesTypeDef",
     {
         "IpSets": RuleGroupVariablesIpSetsDetailsTypeDef,
         "PortSets": RuleGroupVariablesPortSetsDetailsTypeDef,
     },
     total=False,
@@ -7276,22 +8939,45 @@
 )
 
 class StandardsSubscriptionTypeDef(
     _RequiredStandardsSubscriptionTypeDef, _OptionalStandardsSubscriptionTypeDef
 ):
     pass
 
+StatelessCustomPublishMetricActionOutputTypeDef = TypedDict(
+    "StatelessCustomPublishMetricActionOutputTypeDef",
+    {
+        "Dimensions": List[StatelessCustomPublishMetricActionDimensionTypeDef],
+    },
+    total=False,
+)
+
 StatelessCustomPublishMetricActionTypeDef = TypedDict(
     "StatelessCustomPublishMetricActionTypeDef",
     {
         "Dimensions": Sequence[StatelessCustomPublishMetricActionDimensionTypeDef],
     },
     total=False,
 )
 
+AwsApiCallActionOutputTypeDef = TypedDict(
+    "AwsApiCallActionOutputTypeDef",
+    {
+        "Api": str,
+        "ServiceName": str,
+        "CallerType": str,
+        "RemoteIpDetails": ActionRemoteIpDetailsTypeDef,
+        "DomainDetails": AwsApiCallActionDomainDetailsTypeDef,
+        "AffectedResources": Dict[str, str],
+        "FirstSeen": str,
+        "LastSeen": str,
+    },
+    total=False,
+)
+
 AwsApiCallActionTypeDef = TypedDict(
     "AwsApiCallActionTypeDef",
     {
         "Api": str,
         "ServiceName": str,
         "CallerType": str,
         "RemoteIpDetails": ActionRemoteIpDetailsTypeDef,
@@ -7322,14 +9008,38 @@
         "LocalPortDetails": ActionLocalPortDetailsTypeDef,
         "LocalIpDetails": ActionLocalIpDetailsTypeDef,
         "RemoteIpDetails": ActionRemoteIpDetailsTypeDef,
     },
     total=False,
 )
 
+_RequiredVulnerabilityOutputTypeDef = TypedDict(
+    "_RequiredVulnerabilityOutputTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalVulnerabilityOutputTypeDef = TypedDict(
+    "_OptionalVulnerabilityOutputTypeDef",
+    {
+        "VulnerablePackages": List[SoftwarePackageTypeDef],
+        "Cvss": List[CvssOutputTypeDef],
+        "RelatedVulnerabilities": List[str],
+        "Vendor": VulnerabilityVendorTypeDef,
+        "ReferenceUrls": List[str],
+        "FixAvailable": VulnerabilityFixAvailableType,
+    },
+    total=False,
+)
+
+class VulnerabilityOutputTypeDef(
+    _RequiredVulnerabilityOutputTypeDef, _OptionalVulnerabilityOutputTypeDef
+):
+    pass
+
 _RequiredVulnerabilityTypeDef = TypedDict(
     "_RequiredVulnerabilityTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalVulnerabilityTypeDef = TypedDict(
@@ -7344,36 +9054,83 @@
     },
     total=False,
 )
 
 class VulnerabilityTypeDef(_RequiredVulnerabilityTypeDef, _OptionalVulnerabilityTypeDef):
     pass
 
+AwsEc2RouteTableDetailsOutputTypeDef = TypedDict(
+    "AwsEc2RouteTableDetailsOutputTypeDef",
+    {
+        "AssociationSet": List[AssociationSetDetailsTypeDef],
+        "OwnerId": str,
+        "PropagatingVgwSet": List[PropagatingVgwSetDetailsTypeDef],
+        "RouteTableId": str,
+        "RouteSet": List[RouteSetDetailsTypeDef],
+        "VpcId": str,
+    },
+    total=False,
+)
+
 AwsEc2RouteTableDetailsTypeDef = TypedDict(
     "AwsEc2RouteTableDetailsTypeDef",
     {
         "AssociationSet": Sequence[AssociationSetDetailsTypeDef],
         "OwnerId": str,
         "PropagatingVgwSet": Sequence[PropagatingVgwSetDetailsTypeDef],
         "RouteTableId": str,
         "RouteSet": Sequence[RouteSetDetailsTypeDef],
         "VpcId": str,
     },
     total=False,
 )
 
+AutomationRulesActionOutputTypeDef = TypedDict(
+    "AutomationRulesActionOutputTypeDef",
+    {
+        "Type": Literal["FINDING_FIELDS_UPDATE"],
+        "FindingFieldsUpdate": AutomationRulesFindingFieldsUpdateOutputTypeDef,
+    },
+    total=False,
+)
+
 AutomationRulesActionTypeDef = TypedDict(
     "AutomationRulesActionTypeDef",
     {
         "Type": Literal["FINDING_FIELDS_UPDATE"],
         "FindingFieldsUpdate": AutomationRulesFindingFieldsUpdateTypeDef,
     },
     total=False,
 )
 
+AwsAmazonMqBrokerDetailsOutputTypeDef = TypedDict(
+    "AwsAmazonMqBrokerDetailsOutputTypeDef",
+    {
+        "AuthenticationStrategy": str,
+        "AutoMinorVersionUpgrade": bool,
+        "BrokerArn": str,
+        "BrokerName": str,
+        "DeploymentMode": str,
+        "EncryptionOptions": AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef,
+        "EngineType": str,
+        "EngineVersion": str,
+        "HostInstanceType": str,
+        "BrokerId": str,
+        "LdapServerMetadata": AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef,
+        "Logs": AwsAmazonMqBrokerLogsDetailsTypeDef,
+        "MaintenanceWindowStartTime": AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef,
+        "PubliclyAccessible": bool,
+        "SecurityGroups": List[str],
+        "StorageType": str,
+        "SubnetIds": List[str],
+        "Users": List[AwsAmazonMqBrokerUsersDetailsTypeDef],
+    },
+    total=False,
+)
+
 AwsAmazonMqBrokerDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerDetailsTypeDef",
     {
         "AuthenticationStrategy": str,
         "AutoMinorVersionUpgrade": bool,
         "BrokerArn": str,
         "BrokerName": str,
@@ -7391,14 +9148,35 @@
         "StorageType": str,
         "SubnetIds": Sequence[str],
         "Users": Sequence[AwsAmazonMqBrokerUsersDetailsTypeDef],
     },
     total=False,
 )
 
+AwsAppSyncGraphQlApiDetailsOutputTypeDef = TypedDict(
+    "AwsAppSyncGraphQlApiDetailsOutputTypeDef",
+    {
+        "ApiId": str,
+        "Id": str,
+        "OpenIdConnectConfig": AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef,
+        "Name": str,
+        "LambdaAuthorizerConfig": AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef,
+        "XrayEnabled": bool,
+        "Arn": str,
+        "UserPoolConfig": AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef,
+        "AuthenticationType": str,
+        "LogConfig": AwsAppSyncGraphQlApiLogConfigDetailsTypeDef,
+        "AdditionalAuthenticationProviders": List[
+            AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef
+        ],
+        "WafWebAclArn": str,
+    },
+    total=False,
+)
+
 AwsAppSyncGraphQlApiDetailsTypeDef = TypedDict(
     "AwsAppSyncGraphQlApiDetailsTypeDef",
     {
         "ApiId": str,
         "Id": str,
         "OpenIdConnectConfig": AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef,
         "Name": str,
@@ -7412,27 +9190,68 @@
             AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef
         ],
         "WafWebAclArn": str,
     },
     total=False,
 )
 
+AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef = TypedDict(
+    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef",
+    {
+        "InstancesDistribution": (
+            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef
+        ),
+        "LaunchTemplate": (
+            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef
+        ),
+    },
+    total=False,
+)
+
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef",
     {
         "InstancesDistribution": (
             AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef
         ),
         "LaunchTemplate": (
             AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef
         ),
     },
     total=False,
 )
 
+AwsAutoScalingLaunchConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsAutoScalingLaunchConfigurationDetailsOutputTypeDef",
+    {
+        "AssociatePublicIpAddress": bool,
+        "BlockDeviceMappings": List[
+            AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef
+        ],
+        "ClassicLinkVpcId": str,
+        "ClassicLinkVpcSecurityGroups": List[str],
+        "CreatedTime": str,
+        "EbsOptimized": bool,
+        "IamInstanceProfile": str,
+        "ImageId": str,
+        "InstanceMonitoring": AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef,
+        "InstanceType": str,
+        "KernelId": str,
+        "KeyName": str,
+        "LaunchConfigurationName": str,
+        "PlacementTenancy": str,
+        "RamdiskId": str,
+        "SecurityGroups": List[str],
+        "SpotPrice": str,
+        "UserData": str,
+        "MetadataOptions": AwsAutoScalingLaunchConfigurationMetadataOptionsTypeDef,
+    },
+    total=False,
+)
+
 AwsAutoScalingLaunchConfigurationDetailsTypeDef = TypedDict(
     "AwsAutoScalingLaunchConfigurationDetailsTypeDef",
     {
         "AssociatePublicIpAddress": bool,
         "BlockDeviceMappings": Sequence[
             AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef
         ],
@@ -7453,14 +9272,30 @@
         "SpotPrice": str,
         "UserData": str,
         "MetadataOptions": AwsAutoScalingLaunchConfigurationMetadataOptionsTypeDef,
     },
     total=False,
 )
 
+AwsBackupBackupPlanRuleDetailsOutputTypeDef = TypedDict(
+    "AwsBackupBackupPlanRuleDetailsOutputTypeDef",
+    {
+        "TargetBackupVault": str,
+        "StartWindowMinutes": int,
+        "ScheduleExpression": str,
+        "RuleName": str,
+        "RuleId": str,
+        "EnableContinuousBackup": bool,
+        "CompletionWindowMinutes": int,
+        "CopyActions": List[AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef],
+        "Lifecycle": AwsBackupBackupPlanLifecycleDetailsTypeDef,
+    },
+    total=False,
+)
+
 AwsBackupBackupPlanRuleDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanRuleDetailsTypeDef",
     {
         "TargetBackupVault": str,
         "StartWindowMinutes": int,
         "ScheduleExpression": str,
         "RuleName": str,
@@ -7469,47 +9304,96 @@
         "CompletionWindowMinutes": int,
         "CopyActions": Sequence[AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef],
         "Lifecycle": AwsBackupBackupPlanLifecycleDetailsTypeDef,
     },
     total=False,
 )
 
+AwsCertificateManagerCertificateRenewalSummaryOutputTypeDef = TypedDict(
+    "AwsCertificateManagerCertificateRenewalSummaryOutputTypeDef",
+    {
+        "DomainValidationOptions": List[
+            AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef
+        ],
+        "RenewalStatus": str,
+        "RenewalStatusReason": str,
+        "UpdatedAt": str,
+    },
+    total=False,
+)
+
 AwsCertificateManagerCertificateRenewalSummaryTypeDef = TypedDict(
     "AwsCertificateManagerCertificateRenewalSummaryTypeDef",
     {
         "DomainValidationOptions": Sequence[
             AwsCertificateManagerCertificateDomainValidationOptionTypeDef
         ],
         "RenewalStatus": str,
         "RenewalStatusReason": str,
         "UpdatedAt": str,
     },
     total=False,
 )
 
+AwsCloudFrontDistributionOriginItemOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginItemOutputTypeDef",
+    {
+        "DomainName": str,
+        "Id": str,
+        "OriginPath": str,
+        "S3OriginConfig": AwsCloudFrontDistributionOriginS3OriginConfigTypeDef,
+        "CustomOriginConfig": AwsCloudFrontDistributionOriginCustomOriginConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 AwsCloudFrontDistributionOriginItemTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginItemTypeDef",
     {
         "DomainName": str,
         "Id": str,
         "OriginPath": str,
         "S3OriginConfig": AwsCloudFrontDistributionOriginS3OriginConfigTypeDef,
         "CustomOriginConfig": AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef,
     },
     total=False,
 )
 
+AwsCloudFrontDistributionOriginGroupOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginGroupOutputTypeDef",
+    {
+        "FailoverCriteria": AwsCloudFrontDistributionOriginGroupFailoverOutputTypeDef,
+    },
+    total=False,
+)
+
 AwsCloudFrontDistributionOriginGroupTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupTypeDef",
     {
         "FailoverCriteria": AwsCloudFrontDistributionOriginGroupFailoverTypeDef,
     },
     total=False,
 )
 
+AwsCodeBuildProjectDetailsOutputTypeDef = TypedDict(
+    "AwsCodeBuildProjectDetailsOutputTypeDef",
+    {
+        "EncryptionKey": str,
+        "Artifacts": List[AwsCodeBuildProjectArtifactsDetailsTypeDef],
+        "Environment": AwsCodeBuildProjectEnvironmentOutputTypeDef,
+        "Name": str,
+        "Source": AwsCodeBuildProjectSourceTypeDef,
+        "ServiceRole": str,
+        "LogsConfig": AwsCodeBuildProjectLogsConfigDetailsTypeDef,
+        "VpcConfig": AwsCodeBuildProjectVpcConfigOutputTypeDef,
+        "SecondaryArtifacts": List[AwsCodeBuildProjectArtifactsDetailsTypeDef],
+    },
+    total=False,
+)
+
 AwsCodeBuildProjectDetailsTypeDef = TypedDict(
     "AwsCodeBuildProjectDetailsTypeDef",
     {
         "EncryptionKey": str,
         "Artifacts": Sequence[AwsCodeBuildProjectArtifactsDetailsTypeDef],
         "Environment": AwsCodeBuildProjectEnvironmentTypeDef,
         "Name": str,
@@ -7518,27 +9402,85 @@
         "LogsConfig": AwsCodeBuildProjectLogsConfigDetailsTypeDef,
         "VpcConfig": AwsCodeBuildProjectVpcConfigTypeDef,
         "SecondaryArtifacts": Sequence[AwsCodeBuildProjectArtifactsDetailsTypeDef],
     },
     total=False,
 )
 
+AwsDynamoDbTableReplicaOutputTypeDef = TypedDict(
+    "AwsDynamoDbTableReplicaOutputTypeDef",
+    {
+        "GlobalSecondaryIndexes": List[AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef],
+        "KmsMasterKeyId": str,
+        "ProvisionedThroughputOverride": AwsDynamoDbTableProvisionedThroughputOverrideTypeDef,
+        "RegionName": str,
+        "ReplicaStatus": str,
+        "ReplicaStatusDescription": str,
+    },
+    total=False,
+)
+
 AwsDynamoDbTableReplicaTypeDef = TypedDict(
     "AwsDynamoDbTableReplicaTypeDef",
     {
         "GlobalSecondaryIndexes": Sequence[AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef],
         "KmsMasterKeyId": str,
         "ProvisionedThroughputOverride": AwsDynamoDbTableProvisionedThroughputOverrideTypeDef,
         "RegionName": str,
         "ReplicaStatus": str,
         "ReplicaStatusDescription": str,
     },
     total=False,
 )
 
+AwsEc2LaunchTemplateDataDetailsOutputTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataDetailsOutputTypeDef",
+    {
+        "BlockDeviceMappingSet": List[AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef],
+        "CapacityReservationSpecification": (
+            AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef
+        ),
+        "CpuOptions": AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef,
+        "CreditSpecification": AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef,
+        "DisableApiStop": bool,
+        "DisableApiTermination": bool,
+        "EbsOptimized": bool,
+        "ElasticGpuSpecificationSet": List[
+            AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef
+        ],
+        "ElasticInferenceAcceleratorSet": List[
+            AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef
+        ],
+        "EnclaveOptions": AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef,
+        "HibernationOptions": AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef,
+        "IamInstanceProfile": AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef,
+        "ImageId": str,
+        "InstanceInitiatedShutdownBehavior": str,
+        "InstanceMarketOptions": AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef,
+        "InstanceRequirements": AwsEc2LaunchTemplateDataInstanceRequirementsDetailsOutputTypeDef,
+        "InstanceType": str,
+        "KernelId": str,
+        "KeyName": str,
+        "LicenseSet": List[AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef],
+        "MaintenanceOptions": AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef,
+        "MetadataOptions": AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef,
+        "Monitoring": AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef,
+        "NetworkInterfaceSet": List[
+            AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsOutputTypeDef
+        ],
+        "Placement": AwsEc2LaunchTemplateDataPlacementDetailsTypeDef,
+        "PrivateDnsNameOptions": AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef,
+        "RamDiskId": str,
+        "SecurityGroupIdSet": List[str],
+        "SecurityGroupSet": List[str],
+        "UserData": str,
+    },
+    total=False,
+)
+
 AwsEc2LaunchTemplateDataDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataDetailsTypeDef",
     {
         "BlockDeviceMappingSet": Sequence[
             AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef
         ],
         "CapacityReservationSpecification": (
@@ -7576,52 +9518,108 @@
         "SecurityGroupIdSet": Sequence[str],
         "SecurityGroupSet": Sequence[str],
         "UserData": str,
     },
     total=False,
 )
 
+AwsEc2NetworkAclDetailsOutputTypeDef = TypedDict(
+    "AwsEc2NetworkAclDetailsOutputTypeDef",
+    {
+        "IsDefault": bool,
+        "NetworkAclId": str,
+        "OwnerId": str,
+        "VpcId": str,
+        "Associations": List[AwsEc2NetworkAclAssociationTypeDef],
+        "Entries": List[AwsEc2NetworkAclEntryTypeDef],
+    },
+    total=False,
+)
+
 AwsEc2NetworkAclDetailsTypeDef = TypedDict(
     "AwsEc2NetworkAclDetailsTypeDef",
     {
         "IsDefault": bool,
         "NetworkAclId": str,
         "OwnerId": str,
         "VpcId": str,
         "Associations": Sequence[AwsEc2NetworkAclAssociationTypeDef],
         "Entries": Sequence[AwsEc2NetworkAclEntryTypeDef],
     },
     total=False,
 )
 
+AwsEc2SecurityGroupDetailsOutputTypeDef = TypedDict(
+    "AwsEc2SecurityGroupDetailsOutputTypeDef",
+    {
+        "GroupName": str,
+        "GroupId": str,
+        "OwnerId": str,
+        "VpcId": str,
+        "IpPermissions": List[AwsEc2SecurityGroupIpPermissionOutputTypeDef],
+        "IpPermissionsEgress": List[AwsEc2SecurityGroupIpPermissionOutputTypeDef],
+    },
+    total=False,
+)
+
 AwsEc2SecurityGroupDetailsTypeDef = TypedDict(
     "AwsEc2SecurityGroupDetailsTypeDef",
     {
         "GroupName": str,
         "GroupId": str,
         "OwnerId": str,
         "VpcId": str,
         "IpPermissions": Sequence[AwsEc2SecurityGroupIpPermissionTypeDef],
         "IpPermissionsEgress": Sequence[AwsEc2SecurityGroupIpPermissionTypeDef],
     },
     total=False,
 )
 
+AwsEc2VpcPeeringConnectionDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VpcPeeringConnectionDetailsOutputTypeDef",
+    {
+        "AccepterVpcInfo": AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef,
+        "ExpirationTime": str,
+        "RequesterVpcInfo": AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef,
+        "Status": AwsEc2VpcPeeringConnectionStatusDetailsTypeDef,
+        "VpcPeeringConnectionId": str,
+    },
+    total=False,
+)
+
 AwsEc2VpcPeeringConnectionDetailsTypeDef = TypedDict(
     "AwsEc2VpcPeeringConnectionDetailsTypeDef",
     {
         "AccepterVpcInfo": AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef,
         "ExpirationTime": str,
         "RequesterVpcInfo": AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef,
         "Status": AwsEc2VpcPeeringConnectionStatusDetailsTypeDef,
         "VpcPeeringConnectionId": str,
     },
     total=False,
 )
 
+AwsEc2VpnConnectionDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VpnConnectionDetailsOutputTypeDef",
+    {
+        "VpnConnectionId": str,
+        "State": str,
+        "CustomerGatewayId": str,
+        "CustomerGatewayConfiguration": str,
+        "Type": str,
+        "VpnGatewayId": str,
+        "Category": str,
+        "VgwTelemetry": List[AwsEc2VpnConnectionVgwTelemetryDetailsTypeDef],
+        "Options": AwsEc2VpnConnectionOptionsDetailsOutputTypeDef,
+        "Routes": List[AwsEc2VpnConnectionRoutesDetailsTypeDef],
+        "TransitGatewayId": str,
+    },
+    total=False,
+)
+
 AwsEc2VpnConnectionDetailsTypeDef = TypedDict(
     "AwsEc2VpnConnectionDetailsTypeDef",
     {
         "VpnConnectionId": str,
         "State": str,
         "CustomerGatewayId": str,
         "CustomerGatewayConfiguration": str,
@@ -7642,14 +9640,43 @@
         "ExecuteCommandConfiguration": (
             AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef
         ),
     },
     total=False,
 )
 
+AwsEcsServiceDetailsOutputTypeDef = TypedDict(
+    "AwsEcsServiceDetailsOutputTypeDef",
+    {
+        "CapacityProviderStrategy": List[AwsEcsServiceCapacityProviderStrategyDetailsTypeDef],
+        "Cluster": str,
+        "DeploymentConfiguration": AwsEcsServiceDeploymentConfigurationDetailsTypeDef,
+        "DeploymentController": AwsEcsServiceDeploymentControllerDetailsTypeDef,
+        "DesiredCount": int,
+        "EnableEcsManagedTags": bool,
+        "EnableExecuteCommand": bool,
+        "HealthCheckGracePeriodSeconds": int,
+        "LaunchType": str,
+        "LoadBalancers": List[AwsEcsServiceLoadBalancersDetailsTypeDef],
+        "Name": str,
+        "NetworkConfiguration": AwsEcsServiceNetworkConfigurationDetailsOutputTypeDef,
+        "PlacementConstraints": List[AwsEcsServicePlacementConstraintsDetailsTypeDef],
+        "PlacementStrategies": List[AwsEcsServicePlacementStrategiesDetailsTypeDef],
+        "PlatformVersion": str,
+        "PropagateTags": str,
+        "Role": str,
+        "SchedulingStrategy": str,
+        "ServiceArn": str,
+        "ServiceName": str,
+        "ServiceRegistries": List[AwsEcsServiceServiceRegistriesDetailsTypeDef],
+        "TaskDefinition": str,
+    },
+    total=False,
+)
+
 AwsEcsServiceDetailsTypeDef = TypedDict(
     "AwsEcsServiceDetailsTypeDef",
     {
         "CapacityProviderStrategy": Sequence[AwsEcsServiceCapacityProviderStrategyDetailsTypeDef],
         "Cluster": str,
         "DeploymentConfiguration": AwsEcsServiceDeploymentConfigurationDetailsTypeDef,
         "DeploymentController": AwsEcsServiceDeploymentControllerDetailsTypeDef,
@@ -7671,14 +9698,74 @@
         "ServiceName": str,
         "ServiceRegistries": Sequence[AwsEcsServiceServiceRegistriesDetailsTypeDef],
         "TaskDefinition": str,
     },
     total=False,
 )
 
+AwsEcsTaskDefinitionContainerDefinitionsDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsDetailsOutputTypeDef",
+    {
+        "Command": List[str],
+        "Cpu": int,
+        "DependsOn": List[AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef],
+        "DisableNetworking": bool,
+        "DnsSearchDomains": List[str],
+        "DnsServers": List[str],
+        "DockerLabels": Dict[str, str],
+        "DockerSecurityOptions": List[str],
+        "EntryPoint": List[str],
+        "Environment": List[AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef],
+        "EnvironmentFiles": List[
+            AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef
+        ],
+        "Essential": bool,
+        "ExtraHosts": List[AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef],
+        "FirelensConfiguration": (
+            AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef
+        ),
+        "HealthCheck": AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef,
+        "Hostname": str,
+        "Image": str,
+        "Interactive": bool,
+        "Links": List[str],
+        "LinuxParameters": (
+            AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsOutputTypeDef
+        ),
+        "LogConfiguration": (
+            AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsOutputTypeDef
+        ),
+        "Memory": int,
+        "MemoryReservation": int,
+        "MountPoints": List[AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef],
+        "Name": str,
+        "PortMappings": List[AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef],
+        "Privileged": bool,
+        "PseudoTerminal": bool,
+        "ReadonlyRootFilesystem": bool,
+        "RepositoryCredentials": (
+            AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef
+        ),
+        "ResourceRequirements": List[
+            AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef
+        ],
+        "Secrets": List[AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef],
+        "StartTimeout": int,
+        "StopTimeout": int,
+        "SystemControls": List[
+            AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsTypeDef
+        ],
+        "Ulimits": List[AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsTypeDef],
+        "User": str,
+        "VolumesFrom": List[AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef],
+        "WorkingDirectory": str,
+    },
+    total=False,
+)
+
 AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef",
     {
         "Command": Sequence[str],
         "Cpu": int,
         "DependsOn": Sequence[AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef],
         "DisableNetworking": bool,
@@ -7729,27 +9816,56 @@
         "User": str,
         "VolumesFrom": Sequence[AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef],
         "WorkingDirectory": str,
     },
     total=False,
 )
 
+AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef",
+    {
+        "DockerVolumeConfiguration": (
+            AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsOutputTypeDef
+        ),
+        "EfsVolumeConfiguration": AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef,
+        "Host": AwsEcsTaskDefinitionVolumesHostDetailsTypeDef,
+        "Name": str,
+    },
+    total=False,
+)
+
 AwsEcsTaskDefinitionVolumesDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesDetailsTypeDef",
     {
         "DockerVolumeConfiguration": (
             AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef
         ),
         "EfsVolumeConfiguration": AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef,
         "Host": AwsEcsTaskDefinitionVolumesHostDetailsTypeDef,
         "Name": str,
     },
     total=False,
 )
 
+AwsEcsTaskDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDetailsOutputTypeDef",
+    {
+        "ClusterArn": str,
+        "TaskDefinitionArn": str,
+        "Version": str,
+        "CreatedAt": str,
+        "StartedAt": str,
+        "StartedBy": str,
+        "Group": str,
+        "Volumes": List[AwsEcsTaskVolumeDetailsTypeDef],
+        "Containers": List[AwsEcsContainerDetailsOutputTypeDef],
+    },
+    total=False,
+)
+
 AwsEcsTaskDetailsTypeDef = TypedDict(
     "AwsEcsTaskDetailsTypeDef",
     {
         "ClusterArn": str,
         "TaskDefinitionArn": str,
         "Version": str,
         "CreatedAt": str,
@@ -7758,27 +9874,56 @@
         "Group": str,
         "Volumes": Sequence[AwsEcsTaskVolumeDetailsTypeDef],
         "Containers": Sequence[AwsEcsContainerDetailsTypeDef],
     },
     total=False,
 )
 
+AwsEfsAccessPointDetailsOutputTypeDef = TypedDict(
+    "AwsEfsAccessPointDetailsOutputTypeDef",
+    {
+        "AccessPointId": str,
+        "Arn": str,
+        "ClientToken": str,
+        "FileSystemId": str,
+        "PosixUser": AwsEfsAccessPointPosixUserDetailsOutputTypeDef,
+        "RootDirectory": AwsEfsAccessPointRootDirectoryDetailsTypeDef,
+    },
+    total=False,
+)
+
 AwsEfsAccessPointDetailsTypeDef = TypedDict(
     "AwsEfsAccessPointDetailsTypeDef",
     {
         "AccessPointId": str,
         "Arn": str,
         "ClientToken": str,
         "FileSystemId": str,
         "PosixUser": AwsEfsAccessPointPosixUserDetailsTypeDef,
         "RootDirectory": AwsEfsAccessPointRootDirectoryDetailsTypeDef,
     },
     total=False,
 )
 
+AwsEksClusterDetailsOutputTypeDef = TypedDict(
+    "AwsEksClusterDetailsOutputTypeDef",
+    {
+        "Arn": str,
+        "CertificateAuthorityData": str,
+        "ClusterStatus": str,
+        "Endpoint": str,
+        "Name": str,
+        "ResourcesVpcConfig": AwsEksClusterResourcesVpcConfigDetailsOutputTypeDef,
+        "RoleArn": str,
+        "Version": str,
+        "Logging": AwsEksClusterLoggingDetailsOutputTypeDef,
+    },
+    total=False,
+)
+
 AwsEksClusterDetailsTypeDef = TypedDict(
     "AwsEksClusterDetailsTypeDef",
     {
         "Arn": str,
         "CertificateAuthorityData": str,
         "ClusterStatus": str,
         "Endpoint": str,
@@ -7787,14 +9932,36 @@
         "RoleArn": str,
         "Version": str,
         "Logging": AwsEksClusterLoggingDetailsTypeDef,
     },
     total=False,
 )
 
+AwsElasticsearchDomainDetailsOutputTypeDef = TypedDict(
+    "AwsElasticsearchDomainDetailsOutputTypeDef",
+    {
+        "AccessPolicies": str,
+        "DomainEndpointOptions": AwsElasticsearchDomainDomainEndpointOptionsTypeDef,
+        "DomainId": str,
+        "DomainName": str,
+        "Endpoint": str,
+        "Endpoints": Dict[str, str],
+        "ElasticsearchVersion": str,
+        "ElasticsearchClusterConfig": (
+            AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef
+        ),
+        "EncryptionAtRestOptions": AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef,
+        "LogPublishingOptions": AwsElasticsearchDomainLogPublishingOptionsTypeDef,
+        "NodeToNodeEncryptionOptions": AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef,
+        "ServiceSoftwareOptions": AwsElasticsearchDomainServiceSoftwareOptionsTypeDef,
+        "VPCOptions": AwsElasticsearchDomainVPCOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
 AwsElasticsearchDomainDetailsTypeDef = TypedDict(
     "AwsElasticsearchDomainDetailsTypeDef",
     {
         "AccessPolicies": str,
         "DomainEndpointOptions": AwsElasticsearchDomainDomainEndpointOptionsTypeDef,
         "DomainId": str,
         "DomainName": str,
@@ -7809,14 +9976,38 @@
         "NodeToNodeEncryptionOptions": AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef,
         "ServiceSoftwareOptions": AwsElasticsearchDomainServiceSoftwareOptionsTypeDef,
         "VPCOptions": AwsElasticsearchDomainVPCOptionsTypeDef,
     },
     total=False,
 )
 
+AwsElbLoadBalancerDetailsOutputTypeDef = TypedDict(
+    "AwsElbLoadBalancerDetailsOutputTypeDef",
+    {
+        "AvailabilityZones": List[str],
+        "BackendServerDescriptions": List[AwsElbLoadBalancerBackendServerDescriptionOutputTypeDef],
+        "CanonicalHostedZoneName": str,
+        "CanonicalHostedZoneNameID": str,
+        "CreatedTime": str,
+        "DnsName": str,
+        "HealthCheck": AwsElbLoadBalancerHealthCheckTypeDef,
+        "Instances": List[AwsElbLoadBalancerInstanceTypeDef],
+        "ListenerDescriptions": List[AwsElbLoadBalancerListenerDescriptionOutputTypeDef],
+        "LoadBalancerAttributes": AwsElbLoadBalancerAttributesOutputTypeDef,
+        "LoadBalancerName": str,
+        "Policies": AwsElbLoadBalancerPoliciesOutputTypeDef,
+        "Scheme": str,
+        "SecurityGroups": List[str],
+        "SourceSecurityGroup": AwsElbLoadBalancerSourceSecurityGroupTypeDef,
+        "Subnets": List[str],
+        "VpcId": str,
+    },
+    total=False,
+)
+
 AwsElbLoadBalancerDetailsTypeDef = TypedDict(
     "AwsElbLoadBalancerDetailsTypeDef",
     {
         "AvailabilityZones": Sequence[str],
         "BackendServerDescriptions": Sequence[AwsElbLoadBalancerBackendServerDescriptionTypeDef],
         "CanonicalHostedZoneName": str,
         "CanonicalHostedZoneNameID": str,
@@ -7858,14 +10049,31 @@
         "AccountId": str,
         "AccessKeyId": str,
         "SessionContext": AwsIamAccessKeySessionContextTypeDef,
     },
     total=False,
 )
 
+AwsIamRoleDetailsOutputTypeDef = TypedDict(
+    "AwsIamRoleDetailsOutputTypeDef",
+    {
+        "AssumeRolePolicyDocument": str,
+        "AttachedManagedPolicies": List[AwsIamAttachedManagedPolicyTypeDef],
+        "CreateDate": str,
+        "InstanceProfileList": List[AwsIamInstanceProfileOutputTypeDef],
+        "PermissionsBoundary": AwsIamPermissionsBoundaryTypeDef,
+        "RoleId": str,
+        "RoleName": str,
+        "RolePolicyList": List[AwsIamRolePolicyTypeDef],
+        "MaxSessionDuration": int,
+        "Path": str,
+    },
+    total=False,
+)
+
 AwsIamRoleDetailsTypeDef = TypedDict(
     "AwsIamRoleDetailsTypeDef",
     {
         "AssumeRolePolicyDocument": str,
         "AttachedManagedPolicies": Sequence[AwsIamAttachedManagedPolicyTypeDef],
         "CreateDate": str,
         "InstanceProfileList": Sequence[AwsIamInstanceProfileTypeDef],
@@ -7875,14 +10083,41 @@
         "RolePolicyList": Sequence[AwsIamRolePolicyTypeDef],
         "MaxSessionDuration": int,
         "Path": str,
     },
     total=False,
 )
 
+AwsLambdaFunctionDetailsOutputTypeDef = TypedDict(
+    "AwsLambdaFunctionDetailsOutputTypeDef",
+    {
+        "Code": AwsLambdaFunctionCodeTypeDef,
+        "CodeSha256": str,
+        "DeadLetterConfig": AwsLambdaFunctionDeadLetterConfigTypeDef,
+        "Environment": AwsLambdaFunctionEnvironmentOutputTypeDef,
+        "FunctionName": str,
+        "Handler": str,
+        "KmsKeyArn": str,
+        "LastModified": str,
+        "Layers": List[AwsLambdaFunctionLayerTypeDef],
+        "MasterArn": str,
+        "MemorySize": int,
+        "RevisionId": str,
+        "Role": str,
+        "Runtime": str,
+        "Timeout": int,
+        "TracingConfig": AwsLambdaFunctionTracingConfigTypeDef,
+        "VpcConfig": AwsLambdaFunctionVpcConfigOutputTypeDef,
+        "Version": str,
+        "Architectures": List[str],
+        "PackageType": str,
+    },
+    total=False,
+)
+
 AwsLambdaFunctionDetailsTypeDef = TypedDict(
     "AwsLambdaFunctionDetailsTypeDef",
     {
         "Code": AwsLambdaFunctionCodeTypeDef,
         "CodeSha256": str,
         "DeadLetterConfig": AwsLambdaFunctionDeadLetterConfigTypeDef,
         "Environment": AwsLambdaFunctionEnvironmentTypeDef,
@@ -7902,14 +10137,38 @@
         "Version": str,
         "Architectures": Sequence[str],
         "PackageType": str,
     },
     total=False,
 )
 
+AwsOpenSearchServiceDomainDetailsOutputTypeDef = TypedDict(
+    "AwsOpenSearchServiceDomainDetailsOutputTypeDef",
+    {
+        "Arn": str,
+        "AccessPolicies": str,
+        "DomainName": str,
+        "Id": str,
+        "DomainEndpoint": str,
+        "EngineVersion": str,
+        "EncryptionAtRestOptions": AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsTypeDef,
+        "NodeToNodeEncryptionOptions": (
+            AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsTypeDef
+        ),
+        "ServiceSoftwareOptions": AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsTypeDef,
+        "ClusterConfig": AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef,
+        "DomainEndpointOptions": AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef,
+        "VpcOptions": AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef,
+        "LogPublishingOptions": AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef,
+        "DomainEndpoints": Dict[str, str],
+        "AdvancedSecurityOptions": AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef,
+    },
+    total=False,
+)
+
 AwsOpenSearchServiceDomainDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainDetailsTypeDef",
     {
         "Arn": str,
         "AccessPolicies": str,
         "DomainName": str,
         "Id": str,
@@ -7926,27 +10185,91 @@
         "LogPublishingOptions": AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef,
         "DomainEndpoints": Mapping[str, str],
         "AdvancedSecurityOptions": AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef,
     },
     total=False,
 )
 
+AwsRdsDbSubnetGroupOutputTypeDef = TypedDict(
+    "AwsRdsDbSubnetGroupOutputTypeDef",
+    {
+        "DbSubnetGroupName": str,
+        "DbSubnetGroupDescription": str,
+        "VpcId": str,
+        "SubnetGroupStatus": str,
+        "Subnets": List[AwsRdsDbSubnetGroupSubnetTypeDef],
+        "DbSubnetGroupArn": str,
+    },
+    total=False,
+)
+
 AwsRdsDbSubnetGroupTypeDef = TypedDict(
     "AwsRdsDbSubnetGroupTypeDef",
     {
         "DbSubnetGroupName": str,
         "DbSubnetGroupDescription": str,
         "VpcId": str,
         "SubnetGroupStatus": str,
         "Subnets": Sequence[AwsRdsDbSubnetGroupSubnetTypeDef],
         "DbSubnetGroupArn": str,
     },
     total=False,
 )
 
+AwsRedshiftClusterDetailsOutputTypeDef = TypedDict(
+    "AwsRedshiftClusterDetailsOutputTypeDef",
+    {
+        "AllowVersionUpgrade": bool,
+        "AutomatedSnapshotRetentionPeriod": int,
+        "AvailabilityZone": str,
+        "ClusterAvailabilityStatus": str,
+        "ClusterCreateTime": str,
+        "ClusterIdentifier": str,
+        "ClusterNodes": List[AwsRedshiftClusterClusterNodeTypeDef],
+        "ClusterParameterGroups": List[AwsRedshiftClusterClusterParameterGroupOutputTypeDef],
+        "ClusterPublicKey": str,
+        "ClusterRevisionNumber": str,
+        "ClusterSecurityGroups": List[AwsRedshiftClusterClusterSecurityGroupTypeDef],
+        "ClusterSnapshotCopyStatus": AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef,
+        "ClusterStatus": str,
+        "ClusterSubnetGroupName": str,
+        "ClusterVersion": str,
+        "DBName": str,
+        "DeferredMaintenanceWindows": List[AwsRedshiftClusterDeferredMaintenanceWindowTypeDef],
+        "ElasticIpStatus": AwsRedshiftClusterElasticIpStatusTypeDef,
+        "ElasticResizeNumberOfNodeOptions": str,
+        "Encrypted": bool,
+        "Endpoint": AwsRedshiftClusterEndpointTypeDef,
+        "EnhancedVpcRouting": bool,
+        "ExpectedNextSnapshotScheduleTime": str,
+        "ExpectedNextSnapshotScheduleTimeStatus": str,
+        "HsmStatus": AwsRedshiftClusterHsmStatusTypeDef,
+        "IamRoles": List[AwsRedshiftClusterIamRoleTypeDef],
+        "KmsKeyId": str,
+        "MaintenanceTrackName": str,
+        "ManualSnapshotRetentionPeriod": int,
+        "MasterUsername": str,
+        "NextMaintenanceWindowStartTime": str,
+        "NodeType": str,
+        "NumberOfNodes": int,
+        "PendingActions": List[str],
+        "PendingModifiedValues": AwsRedshiftClusterPendingModifiedValuesTypeDef,
+        "PreferredMaintenanceWindow": str,
+        "PubliclyAccessible": bool,
+        "ResizeInfo": AwsRedshiftClusterResizeInfoTypeDef,
+        "RestoreStatus": AwsRedshiftClusterRestoreStatusTypeDef,
+        "SnapshotScheduleIdentifier": str,
+        "SnapshotScheduleState": str,
+        "VpcId": str,
+        "VpcSecurityGroups": List[AwsRedshiftClusterVpcSecurityGroupTypeDef],
+        "LoggingStatus": AwsRedshiftClusterLoggingStatusTypeDef,
+    },
+    total=False,
+)
+
 AwsRedshiftClusterDetailsTypeDef = TypedDict(
     "AwsRedshiftClusterDetailsTypeDef",
     {
         "AllowVersionUpgrade": bool,
         "AutomatedSnapshotRetentionPeriod": int,
         "AvailabilityZone": str,
         "ClusterAvailabilityStatus": str,
@@ -7990,27 +10313,48 @@
         "VpcId": str,
         "VpcSecurityGroups": Sequence[AwsRedshiftClusterVpcSecurityGroupTypeDef],
         "LoggingStatus": AwsRedshiftClusterLoggingStatusTypeDef,
     },
     total=False,
 )
 
+AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsOutputTypeDef = TypedDict(
+    "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsOutputTypeDef",
+    {
+        "Operands": List[
+            AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef
+        ],
+        "Prefix": str,
+        "Tag": AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef,
+        "Type": str,
+    },
+    total=False,
+)
+
 AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef",
     {
         "Operands": Sequence[
             AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef
         ],
         "Prefix": str,
         "Tag": AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef,
         "Type": str,
     },
     total=False,
 )
 
+AwsS3BucketNotificationConfigurationFilterOutputTypeDef = TypedDict(
+    "AwsS3BucketNotificationConfigurationFilterOutputTypeDef",
+    {
+        "S3KeyFilter": AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef,
+    },
+    total=False,
+)
+
 AwsS3BucketNotificationConfigurationFilterTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationFilterTypeDef",
     {
         "S3KeyFilter": AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef,
     },
     total=False,
 )
@@ -8020,22 +10364,41 @@
     {
         "ObjectLockEnabled": str,
         "Rule": AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef,
     },
     total=False,
 )
 
+AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef = TypedDict(
+    "AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef",
+    {
+        "Rules": List[AwsS3BucketServerSideEncryptionRuleTypeDef],
+    },
+    total=False,
+)
+
 AwsS3BucketServerSideEncryptionConfigurationTypeDef = TypedDict(
     "AwsS3BucketServerSideEncryptionConfigurationTypeDef",
     {
         "Rules": Sequence[AwsS3BucketServerSideEncryptionRuleTypeDef],
     },
     total=False,
 )
 
+AwsS3BucketWebsiteConfigurationOutputTypeDef = TypedDict(
+    "AwsS3BucketWebsiteConfigurationOutputTypeDef",
+    {
+        "ErrorDocument": str,
+        "IndexDocumentSuffix": str,
+        "RedirectAllRequestsTo": AwsS3BucketWebsiteConfigurationRedirectToTypeDef,
+        "RoutingRules": List[AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef],
+    },
+    total=False,
+)
+
 AwsS3BucketWebsiteConfigurationTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationTypeDef",
     {
         "ErrorDocument": str,
         "IndexDocumentSuffix": str,
         "RedirectAllRequestsTo": AwsS3BucketWebsiteConfigurationRedirectToTypeDef,
         "RoutingRules": Sequence[AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef],
@@ -8044,83 +10407,164 @@
 )
 
 BatchUpdateFindingsResponseTypeDef = TypedDict(
     "BatchUpdateFindingsResponseTypeDef",
     {
         "ProcessedFindings": List[AwsSecurityFindingIdentifierTypeDef],
         "UnprocessedFindings": List[BatchUpdateFindingsUnprocessedFindingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AwsSsmPatchComplianceDetailsTypeDef = TypedDict(
     "AwsSsmPatchComplianceDetailsTypeDef",
     {
         "Patch": AwsSsmPatchTypeDef,
     },
     total=False,
 )
 
+AwsStepFunctionStateMachineLoggingConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsStepFunctionStateMachineLoggingConfigurationDetailsOutputTypeDef",
+    {
+        "Destinations": List[
+            AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef
+        ],
+        "IncludeExecutionData": bool,
+        "Level": str,
+    },
+    total=False,
+)
+
 AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef = TypedDict(
     "AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef",
     {
         "Destinations": Sequence[
             AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef
         ],
         "IncludeExecutionData": bool,
         "Level": str,
     },
     total=False,
 )
 
+AwsWafRegionalRuleGroupDetailsOutputTypeDef = TypedDict(
+    "AwsWafRegionalRuleGroupDetailsOutputTypeDef",
+    {
+        "MetricName": str,
+        "Name": str,
+        "RuleGroupId": str,
+        "Rules": List[AwsWafRegionalRuleGroupRulesDetailsTypeDef],
+    },
+    total=False,
+)
+
 AwsWafRegionalRuleGroupDetailsTypeDef = TypedDict(
     "AwsWafRegionalRuleGroupDetailsTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "RuleGroupId": str,
         "Rules": Sequence[AwsWafRegionalRuleGroupRulesDetailsTypeDef],
     },
     total=False,
 )
 
+AwsWafRegionalWebAclDetailsOutputTypeDef = TypedDict(
+    "AwsWafRegionalWebAclDetailsOutputTypeDef",
+    {
+        "DefaultAction": str,
+        "MetricName": str,
+        "Name": str,
+        "RulesList": List[AwsWafRegionalWebAclRulesListDetailsTypeDef],
+        "WebAclId": str,
+    },
+    total=False,
+)
+
 AwsWafRegionalWebAclDetailsTypeDef = TypedDict(
     "AwsWafRegionalWebAclDetailsTypeDef",
     {
         "DefaultAction": str,
         "MetricName": str,
         "Name": str,
         "RulesList": Sequence[AwsWafRegionalWebAclRulesListDetailsTypeDef],
         "WebAclId": str,
     },
     total=False,
 )
 
+AwsWafRuleGroupDetailsOutputTypeDef = TypedDict(
+    "AwsWafRuleGroupDetailsOutputTypeDef",
+    {
+        "MetricName": str,
+        "Name": str,
+        "RuleGroupId": str,
+        "Rules": List[AwsWafRuleGroupRulesDetailsTypeDef],
+    },
+    total=False,
+)
+
 AwsWafRuleGroupDetailsTypeDef = TypedDict(
     "AwsWafRuleGroupDetailsTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "RuleGroupId": str,
         "Rules": Sequence[AwsWafRuleGroupRulesDetailsTypeDef],
     },
     total=False,
 )
 
+AwsWafWebAclDetailsOutputTypeDef = TypedDict(
+    "AwsWafWebAclDetailsOutputTypeDef",
+    {
+        "Name": str,
+        "DefaultAction": str,
+        "Rules": List[AwsWafWebAclRuleOutputTypeDef],
+        "WebAclId": str,
+    },
+    total=False,
+)
+
 AwsWafWebAclDetailsTypeDef = TypedDict(
     "AwsWafWebAclDetailsTypeDef",
     {
         "Name": str,
         "DefaultAction": str,
         "Rules": Sequence[AwsWafWebAclRuleTypeDef],
         "WebAclId": str,
     },
     total=False,
 )
 
+AwsWafv2ActionAllowDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2ActionAllowDetailsOutputTypeDef",
+    {
+        "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsOutputTypeDef,
+    },
+    total=False,
+)
+
+AwsWafv2RulesActionCaptchaDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2RulesActionCaptchaDetailsOutputTypeDef",
+    {
+        "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsOutputTypeDef,
+    },
+    total=False,
+)
+
+AwsWafv2RulesActionCountDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2RulesActionCountDetailsOutputTypeDef",
+    {
+        "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsOutputTypeDef,
+    },
+    total=False,
+)
+
 AwsWafv2ActionAllowDetailsTypeDef = TypedDict(
     "AwsWafv2ActionAllowDetailsTypeDef",
     {
         "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsTypeDef,
     },
     total=False,
 )
@@ -8137,41 +10581,49 @@
     "AwsWafv2RulesActionCountDetailsTypeDef",
     {
         "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsTypeDef,
     },
     total=False,
 )
 
+AwsWafv2ActionBlockDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2ActionBlockDetailsOutputTypeDef",
+    {
+        "CustomResponse": AwsWafv2CustomResponseDetailsOutputTypeDef,
+    },
+    total=False,
+)
+
 AwsWafv2ActionBlockDetailsTypeDef = TypedDict(
     "AwsWafv2ActionBlockDetailsTypeDef",
     {
         "CustomResponse": AwsWafv2CustomResponseDetailsTypeDef,
     },
     total=False,
 )
 
 BatchGetStandardsControlAssociationsResponseTypeDef = TypedDict(
     "BatchGetStandardsControlAssociationsResponseTypeDef",
     {
         "StandardsControlAssociationDetails": List[StandardsControlAssociationDetailTypeDef],
         "UnprocessedAssociations": List[UnprocessedStandardsControlAssociationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateStandardsControlAssociationsResponseTypeDef = TypedDict(
     "BatchUpdateStandardsControlAssociationsResponseTypeDef",
     {
         "UnprocessedAssociationUpdates": List[UnprocessedStandardsControlAssociationUpdateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AutomationRulesFindingFiltersTypeDef = TypedDict(
-    "AutomationRulesFindingFiltersTypeDef",
+AutomationRulesFindingFiltersOutputTypeDef = TypedDict(
+    "AutomationRulesFindingFiltersOutputTypeDef",
     {
         "ProductArn": List[StringFilterTypeDef],
         "AwsAccountId": List[StringFilterTypeDef],
         "Id": List[StringFilterTypeDef],
         "GeneratorId": List[StringFilterTypeDef],
         "Type": List[StringFilterTypeDef],
         "FirstObservedAt": List[DateFilterTypeDef],
@@ -8204,14 +10656,160 @@
         "NoteUpdatedAt": List[DateFilterTypeDef],
         "NoteUpdatedBy": List[StringFilterTypeDef],
         "UserDefinedFields": List[MapFilterTypeDef],
     },
     total=False,
 )
 
+AutomationRulesFindingFiltersTypeDef = TypedDict(
+    "AutomationRulesFindingFiltersTypeDef",
+    {
+        "ProductArn": Sequence[StringFilterTypeDef],
+        "AwsAccountId": Sequence[StringFilterTypeDef],
+        "Id": Sequence[StringFilterTypeDef],
+        "GeneratorId": Sequence[StringFilterTypeDef],
+        "Type": Sequence[StringFilterTypeDef],
+        "FirstObservedAt": Sequence[DateFilterTypeDef],
+        "LastObservedAt": Sequence[DateFilterTypeDef],
+        "CreatedAt": Sequence[DateFilterTypeDef],
+        "UpdatedAt": Sequence[DateFilterTypeDef],
+        "Confidence": Sequence[NumberFilterTypeDef],
+        "Criticality": Sequence[NumberFilterTypeDef],
+        "Title": Sequence[StringFilterTypeDef],
+        "Description": Sequence[StringFilterTypeDef],
+        "SourceUrl": Sequence[StringFilterTypeDef],
+        "ProductName": Sequence[StringFilterTypeDef],
+        "CompanyName": Sequence[StringFilterTypeDef],
+        "SeverityLabel": Sequence[StringFilterTypeDef],
+        "ResourceType": Sequence[StringFilterTypeDef],
+        "ResourceId": Sequence[StringFilterTypeDef],
+        "ResourcePartition": Sequence[StringFilterTypeDef],
+        "ResourceRegion": Sequence[StringFilterTypeDef],
+        "ResourceTags": Sequence[MapFilterTypeDef],
+        "ResourceDetailsOther": Sequence[MapFilterTypeDef],
+        "ComplianceStatus": Sequence[StringFilterTypeDef],
+        "ComplianceSecurityControlId": Sequence[StringFilterTypeDef],
+        "ComplianceAssociatedStandardsId": Sequence[StringFilterTypeDef],
+        "VerificationState": Sequence[StringFilterTypeDef],
+        "WorkflowStatus": Sequence[StringFilterTypeDef],
+        "RecordState": Sequence[StringFilterTypeDef],
+        "RelatedFindingsProductArn": Sequence[StringFilterTypeDef],
+        "RelatedFindingsId": Sequence[StringFilterTypeDef],
+        "NoteText": Sequence[StringFilterTypeDef],
+        "NoteUpdatedAt": Sequence[DateFilterTypeDef],
+        "NoteUpdatedBy": Sequence[StringFilterTypeDef],
+        "UserDefinedFields": Sequence[MapFilterTypeDef],
+    },
+    total=False,
+)
+
+AwsSecurityFindingFiltersOutputTypeDef = TypedDict(
+    "AwsSecurityFindingFiltersOutputTypeDef",
+    {
+        "ProductArn": List[StringFilterTypeDef],
+        "AwsAccountId": List[StringFilterTypeDef],
+        "Id": List[StringFilterTypeDef],
+        "GeneratorId": List[StringFilterTypeDef],
+        "Region": List[StringFilterTypeDef],
+        "Type": List[StringFilterTypeDef],
+        "FirstObservedAt": List[DateFilterTypeDef],
+        "LastObservedAt": List[DateFilterTypeDef],
+        "CreatedAt": List[DateFilterTypeDef],
+        "UpdatedAt": List[DateFilterTypeDef],
+        "SeverityProduct": List[NumberFilterTypeDef],
+        "SeverityNormalized": List[NumberFilterTypeDef],
+        "SeverityLabel": List[StringFilterTypeDef],
+        "Confidence": List[NumberFilterTypeDef],
+        "Criticality": List[NumberFilterTypeDef],
+        "Title": List[StringFilterTypeDef],
+        "Description": List[StringFilterTypeDef],
+        "RecommendationText": List[StringFilterTypeDef],
+        "SourceUrl": List[StringFilterTypeDef],
+        "ProductFields": List[MapFilterTypeDef],
+        "ProductName": List[StringFilterTypeDef],
+        "CompanyName": List[StringFilterTypeDef],
+        "UserDefinedFields": List[MapFilterTypeDef],
+        "MalwareName": List[StringFilterTypeDef],
+        "MalwareType": List[StringFilterTypeDef],
+        "MalwarePath": List[StringFilterTypeDef],
+        "MalwareState": List[StringFilterTypeDef],
+        "NetworkDirection": List[StringFilterTypeDef],
+        "NetworkProtocol": List[StringFilterTypeDef],
+        "NetworkSourceIpV4": List[IpFilterTypeDef],
+        "NetworkSourceIpV6": List[IpFilterTypeDef],
+        "NetworkSourcePort": List[NumberFilterTypeDef],
+        "NetworkSourceDomain": List[StringFilterTypeDef],
+        "NetworkSourceMac": List[StringFilterTypeDef],
+        "NetworkDestinationIpV4": List[IpFilterTypeDef],
+        "NetworkDestinationIpV6": List[IpFilterTypeDef],
+        "NetworkDestinationPort": List[NumberFilterTypeDef],
+        "NetworkDestinationDomain": List[StringFilterTypeDef],
+        "ProcessName": List[StringFilterTypeDef],
+        "ProcessPath": List[StringFilterTypeDef],
+        "ProcessPid": List[NumberFilterTypeDef],
+        "ProcessParentPid": List[NumberFilterTypeDef],
+        "ProcessLaunchedAt": List[DateFilterTypeDef],
+        "ProcessTerminatedAt": List[DateFilterTypeDef],
+        "ThreatIntelIndicatorType": List[StringFilterTypeDef],
+        "ThreatIntelIndicatorValue": List[StringFilterTypeDef],
+        "ThreatIntelIndicatorCategory": List[StringFilterTypeDef],
+        "ThreatIntelIndicatorLastObservedAt": List[DateFilterTypeDef],
+        "ThreatIntelIndicatorSource": List[StringFilterTypeDef],
+        "ThreatIntelIndicatorSourceUrl": List[StringFilterTypeDef],
+        "ResourceType": List[StringFilterTypeDef],
+        "ResourceId": List[StringFilterTypeDef],
+        "ResourcePartition": List[StringFilterTypeDef],
+        "ResourceRegion": List[StringFilterTypeDef],
+        "ResourceTags": List[MapFilterTypeDef],
+        "ResourceAwsEc2InstanceType": List[StringFilterTypeDef],
+        "ResourceAwsEc2InstanceImageId": List[StringFilterTypeDef],
+        "ResourceAwsEc2InstanceIpV4Addresses": List[IpFilterTypeDef],
+        "ResourceAwsEc2InstanceIpV6Addresses": List[IpFilterTypeDef],
+        "ResourceAwsEc2InstanceKeyName": List[StringFilterTypeDef],
+        "ResourceAwsEc2InstanceIamInstanceProfileArn": List[StringFilterTypeDef],
+        "ResourceAwsEc2InstanceVpcId": List[StringFilterTypeDef],
+        "ResourceAwsEc2InstanceSubnetId": List[StringFilterTypeDef],
+        "ResourceAwsEc2InstanceLaunchedAt": List[DateFilterTypeDef],
+        "ResourceAwsS3BucketOwnerId": List[StringFilterTypeDef],
+        "ResourceAwsS3BucketOwnerName": List[StringFilterTypeDef],
+        "ResourceAwsIamAccessKeyUserName": List[StringFilterTypeDef],
+        "ResourceAwsIamAccessKeyPrincipalName": List[StringFilterTypeDef],
+        "ResourceAwsIamAccessKeyStatus": List[StringFilterTypeDef],
+        "ResourceAwsIamAccessKeyCreatedAt": List[DateFilterTypeDef],
+        "ResourceAwsIamUserUserName": List[StringFilterTypeDef],
+        "ResourceContainerName": List[StringFilterTypeDef],
+        "ResourceContainerImageId": List[StringFilterTypeDef],
+        "ResourceContainerImageName": List[StringFilterTypeDef],
+        "ResourceContainerLaunchedAt": List[DateFilterTypeDef],
+        "ResourceDetailsOther": List[MapFilterTypeDef],
+        "ComplianceStatus": List[StringFilterTypeDef],
+        "VerificationState": List[StringFilterTypeDef],
+        "WorkflowState": List[StringFilterTypeDef],
+        "WorkflowStatus": List[StringFilterTypeDef],
+        "RecordState": List[StringFilterTypeDef],
+        "RelatedFindingsProductArn": List[StringFilterTypeDef],
+        "RelatedFindingsId": List[StringFilterTypeDef],
+        "NoteText": List[StringFilterTypeDef],
+        "NoteUpdatedAt": List[DateFilterTypeDef],
+        "NoteUpdatedBy": List[StringFilterTypeDef],
+        "Keyword": List[KeywordFilterTypeDef],
+        "FindingProviderFieldsConfidence": List[NumberFilterTypeDef],
+        "FindingProviderFieldsCriticality": List[NumberFilterTypeDef],
+        "FindingProviderFieldsRelatedFindingsId": List[StringFilterTypeDef],
+        "FindingProviderFieldsRelatedFindingsProductArn": List[StringFilterTypeDef],
+        "FindingProviderFieldsSeverityLabel": List[StringFilterTypeDef],
+        "FindingProviderFieldsSeverityOriginal": List[StringFilterTypeDef],
+        "FindingProviderFieldsTypes": List[StringFilterTypeDef],
+        "Sample": List[BooleanFilterTypeDef],
+        "ComplianceSecurityControlId": List[StringFilterTypeDef],
+        "ComplianceAssociatedStandardsId": List[StringFilterTypeDef],
+    },
+    total=False,
+)
+
 AwsSecurityFindingFiltersTypeDef = TypedDict(
     "AwsSecurityFindingFiltersTypeDef",
     {
         "ProductArn": Sequence[StringFilterTypeDef],
         "AwsAccountId": Sequence[StringFilterTypeDef],
         "Id": Sequence[StringFilterTypeDef],
         "GeneratorId": Sequence[StringFilterTypeDef],
@@ -8313,108 +10911,181 @@
 )
 
 GetFindingHistoryResponseTypeDef = TypedDict(
     "GetFindingHistoryResponseTypeDef",
     {
         "Records": List[FindingHistoryRecordTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInsightResultsResponseTypeDef = TypedDict(
     "GetInsightResultsResponseTypeDef",
     {
         "InsightResults": InsightResultsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+NetworkHeaderOutputTypeDef = TypedDict(
+    "NetworkHeaderOutputTypeDef",
+    {
+        "Protocol": str,
+        "Destination": NetworkPathComponentDetailsOutputTypeDef,
+        "Source": NetworkPathComponentDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 NetworkHeaderTypeDef = TypedDict(
     "NetworkHeaderTypeDef",
     {
         "Protocol": str,
         "Destination": NetworkPathComponentDetailsTypeDef,
         "Source": NetworkPathComponentDetailsTypeDef,
     },
     total=False,
 )
 
+OccurrencesOutputTypeDef = TypedDict(
+    "OccurrencesOutputTypeDef",
+    {
+        "LineRanges": List[RangeTypeDef],
+        "OffsetRanges": List[RangeTypeDef],
+        "Pages": List[PageTypeDef],
+        "Records": List[RecordTypeDef],
+        "Cells": List[CellTypeDef],
+    },
+    total=False,
+)
+
 OccurrencesTypeDef = TypedDict(
     "OccurrencesTypeDef",
     {
         "LineRanges": Sequence[RangeTypeDef],
         "OffsetRanges": Sequence[RangeTypeDef],
         "Pages": Sequence[PageTypeDef],
         "Records": Sequence[RecordTypeDef],
         "Cells": Sequence[CellTypeDef],
     },
     total=False,
 )
 
+RuleGroupSourceStatelessRuleDefinitionOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRuleDefinitionOutputTypeDef",
+    {
+        "Actions": List[str],
+        "MatchAttributes": RuleGroupSourceStatelessRuleMatchAttributesOutputTypeDef,
+    },
+    total=False,
+)
+
 RuleGroupSourceStatelessRuleDefinitionTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleDefinitionTypeDef",
     {
         "Actions": Sequence[str],
         "MatchAttributes": RuleGroupSourceStatelessRuleMatchAttributesTypeDef,
     },
     total=False,
 )
 
 DescribeStandardsResponseTypeDef = TypedDict(
     "DescribeStandardsResponseTypeDef",
     {
         "Standards": List[StandardTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDisableStandardsResponseTypeDef = TypedDict(
     "BatchDisableStandardsResponseTypeDef",
     {
         "StandardsSubscriptions": List[StandardsSubscriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchEnableStandardsResponseTypeDef = TypedDict(
     "BatchEnableStandardsResponseTypeDef",
     {
         "StandardsSubscriptions": List[StandardsSubscriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEnabledStandardsResponseTypeDef = TypedDict(
     "GetEnabledStandardsResponseTypeDef",
     {
         "StandardsSubscriptions": List[StandardsSubscriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+StatelessCustomActionDefinitionOutputTypeDef = TypedDict(
+    "StatelessCustomActionDefinitionOutputTypeDef",
+    {
+        "PublishMetricAction": StatelessCustomPublishMetricActionOutputTypeDef,
+    },
+    total=False,
+)
+
 StatelessCustomActionDefinitionTypeDef = TypedDict(
     "StatelessCustomActionDefinitionTypeDef",
     {
         "PublishMetricAction": StatelessCustomPublishMetricActionTypeDef,
     },
     total=False,
 )
 
+PortProbeActionOutputTypeDef = TypedDict(
+    "PortProbeActionOutputTypeDef",
+    {
+        "PortProbeDetails": List[PortProbeDetailTypeDef],
+        "Blocked": bool,
+    },
+    total=False,
+)
+
 PortProbeActionTypeDef = TypedDict(
     "PortProbeActionTypeDef",
     {
         "PortProbeDetails": Sequence[PortProbeDetailTypeDef],
         "Blocked": bool,
     },
     total=False,
 )
 
+AutomationRulesActionUnionTypeDef = Union[
+    AutomationRulesActionTypeDef, AutomationRulesActionOutputTypeDef
+]
+AwsAutoScalingAutoScalingGroupDetailsOutputTypeDef = TypedDict(
+    "AwsAutoScalingAutoScalingGroupDetailsOutputTypeDef",
+    {
+        "LaunchConfigurationName": str,
+        "LoadBalancerNames": List[str],
+        "HealthCheckType": str,
+        "HealthCheckGracePeriod": int,
+        "CreatedTime": str,
+        "MixedInstancesPolicy": (
+            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef
+        ),
+        "AvailabilityZones": List[
+            AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef
+        ],
+        "LaunchTemplate": (
+            AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef
+        ),
+        "CapacityRebalance": bool,
+    },
+    total=False,
+)
+
 AwsAutoScalingAutoScalingGroupDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupDetailsTypeDef",
     {
         "LaunchConfigurationName": str,
         "LoadBalancerNames": Sequence[str],
         "HealthCheckType": str,
         "HealthCheckGracePeriod": int,
@@ -8427,24 +11098,68 @@
             AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef
         ),
         "CapacityRebalance": bool,
     },
     total=False,
 )
 
+AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef = TypedDict(
+    "AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef",
+    {
+        "BackupPlanName": str,
+        "AdvancedBackupSettings": List[
+            AwsBackupBackupPlanAdvancedBackupSettingsDetailsOutputTypeDef
+        ],
+        "BackupPlanRule": List[AwsBackupBackupPlanRuleDetailsOutputTypeDef],
+    },
+    total=False,
+)
+
 AwsBackupBackupPlanBackupPlanDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanBackupPlanDetailsTypeDef",
     {
         "BackupPlanName": str,
         "AdvancedBackupSettings": Sequence[AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef],
         "BackupPlanRule": Sequence[AwsBackupBackupPlanRuleDetailsTypeDef],
     },
     total=False,
 )
 
+AwsCertificateManagerCertificateDetailsOutputTypeDef = TypedDict(
+    "AwsCertificateManagerCertificateDetailsOutputTypeDef",
+    {
+        "CertificateAuthorityArn": str,
+        "CreatedAt": str,
+        "DomainName": str,
+        "DomainValidationOptions": List[
+            AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef
+        ],
+        "ExtendedKeyUsages": List[AwsCertificateManagerCertificateExtendedKeyUsageTypeDef],
+        "FailureReason": str,
+        "ImportedAt": str,
+        "InUseBy": List[str],
+        "IssuedAt": str,
+        "Issuer": str,
+        "KeyAlgorithm": str,
+        "KeyUsages": List[AwsCertificateManagerCertificateKeyUsageTypeDef],
+        "NotAfter": str,
+        "NotBefore": str,
+        "Options": AwsCertificateManagerCertificateOptionsTypeDef,
+        "RenewalEligibility": str,
+        "RenewalSummary": AwsCertificateManagerCertificateRenewalSummaryOutputTypeDef,
+        "Serial": str,
+        "SignatureAlgorithm": str,
+        "Status": str,
+        "Subject": str,
+        "SubjectAlternativeNames": List[str],
+        "Type": str,
+    },
+    total=False,
+)
+
 AwsCertificateManagerCertificateDetailsTypeDef = TypedDict(
     "AwsCertificateManagerCertificateDetailsTypeDef",
     {
         "CertificateAuthorityArn": str,
         "CreatedAt": str,
         "DomainName": str,
         "DomainValidationOptions": Sequence[
@@ -8469,30 +11184,72 @@
         "Subject": str,
         "SubjectAlternativeNames": Sequence[str],
         "Type": str,
     },
     total=False,
 )
 
+AwsCloudFrontDistributionOriginsOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginsOutputTypeDef",
+    {
+        "Items": List[AwsCloudFrontDistributionOriginItemOutputTypeDef],
+    },
+    total=False,
+)
+
 AwsCloudFrontDistributionOriginsTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginsTypeDef",
     {
         "Items": Sequence[AwsCloudFrontDistributionOriginItemTypeDef],
     },
     total=False,
 )
 
+AwsCloudFrontDistributionOriginGroupsOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginGroupsOutputTypeDef",
+    {
+        "Items": List[AwsCloudFrontDistributionOriginGroupOutputTypeDef],
+    },
+    total=False,
+)
+
 AwsCloudFrontDistributionOriginGroupsTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupsTypeDef",
     {
         "Items": Sequence[AwsCloudFrontDistributionOriginGroupTypeDef],
     },
     total=False,
 )
 
+AwsDynamoDbTableDetailsOutputTypeDef = TypedDict(
+    "AwsDynamoDbTableDetailsOutputTypeDef",
+    {
+        "AttributeDefinitions": List[AwsDynamoDbTableAttributeDefinitionTypeDef],
+        "BillingModeSummary": AwsDynamoDbTableBillingModeSummaryTypeDef,
+        "CreationDateTime": str,
+        "GlobalSecondaryIndexes": List[AwsDynamoDbTableGlobalSecondaryIndexOutputTypeDef],
+        "GlobalTableVersion": str,
+        "ItemCount": int,
+        "KeySchema": List[AwsDynamoDbTableKeySchemaTypeDef],
+        "LatestStreamArn": str,
+        "LatestStreamLabel": str,
+        "LocalSecondaryIndexes": List[AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef],
+        "ProvisionedThroughput": AwsDynamoDbTableProvisionedThroughputTypeDef,
+        "Replicas": List[AwsDynamoDbTableReplicaOutputTypeDef],
+        "RestoreSummary": AwsDynamoDbTableRestoreSummaryTypeDef,
+        "SseDescription": AwsDynamoDbTableSseDescriptionTypeDef,
+        "StreamSpecification": AwsDynamoDbTableStreamSpecificationTypeDef,
+        "TableId": str,
+        "TableName": str,
+        "TableSizeBytes": int,
+        "TableStatus": str,
+    },
+    total=False,
+)
+
 AwsDynamoDbTableDetailsTypeDef = TypedDict(
     "AwsDynamoDbTableDetailsTypeDef",
     {
         "AttributeDefinitions": Sequence[AwsDynamoDbTableAttributeDefinitionTypeDef],
         "BillingModeSummary": AwsDynamoDbTableBillingModeSummaryTypeDef,
         "CreationDateTime": str,
         "GlobalSecondaryIndexes": Sequence[AwsDynamoDbTableGlobalSecondaryIndexTypeDef],
@@ -8511,26 +11268,57 @@
         "TableName": str,
         "TableSizeBytes": int,
         "TableStatus": str,
     },
     total=False,
 )
 
+AwsEc2LaunchTemplateDetailsOutputTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDetailsOutputTypeDef",
+    {
+        "LaunchTemplateName": str,
+        "Id": str,
+        "LaunchTemplateData": AwsEc2LaunchTemplateDataDetailsOutputTypeDef,
+        "DefaultVersionNumber": int,
+        "LatestVersionNumber": int,
+    },
+    total=False,
+)
+
 AwsEc2LaunchTemplateDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDetailsTypeDef",
     {
         "LaunchTemplateName": str,
         "Id": str,
         "LaunchTemplateData": AwsEc2LaunchTemplateDataDetailsTypeDef,
         "DefaultVersionNumber": int,
         "LatestVersionNumber": int,
     },
     total=False,
 )
 
+AwsEcsClusterDetailsOutputTypeDef = TypedDict(
+    "AwsEcsClusterDetailsOutputTypeDef",
+    {
+        "ClusterArn": str,
+        "ActiveServicesCount": int,
+        "CapacityProviders": List[str],
+        "ClusterSettings": List[AwsEcsClusterClusterSettingsDetailsTypeDef],
+        "Configuration": AwsEcsClusterConfigurationDetailsTypeDef,
+        "DefaultCapacityProviderStrategy": List[
+            AwsEcsClusterDefaultCapacityProviderStrategyDetailsTypeDef
+        ],
+        "ClusterName": str,
+        "RegisteredContainerInstancesCount": int,
+        "RunningTasksCount": int,
+        "Status": str,
+    },
+    total=False,
+)
+
 AwsEcsClusterDetailsTypeDef = TypedDict(
     "AwsEcsClusterDetailsTypeDef",
     {
         "ClusterArn": str,
         "ActiveServicesCount": int,
         "CapacityProviders": Sequence[str],
         "ClusterSettings": Sequence[AwsEcsClusterClusterSettingsDetailsTypeDef],
@@ -8542,14 +11330,35 @@
         "RegisteredContainerInstancesCount": int,
         "RunningTasksCount": int,
         "Status": str,
     },
     total=False,
 )
 
+AwsEcsTaskDefinitionDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionDetailsOutputTypeDef",
+    {
+        "ContainerDefinitions": List[AwsEcsTaskDefinitionContainerDefinitionsDetailsOutputTypeDef],
+        "Cpu": str,
+        "ExecutionRoleArn": str,
+        "Family": str,
+        "InferenceAccelerators": List[AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef],
+        "IpcMode": str,
+        "Memory": str,
+        "NetworkMode": str,
+        "PidMode": str,
+        "PlacementConstraints": List[AwsEcsTaskDefinitionPlacementConstraintsDetailsTypeDef],
+        "ProxyConfiguration": AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef,
+        "RequiresCompatibilities": List[str],
+        "TaskRoleArn": str,
+        "Volumes": List[AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef],
+    },
+    total=False,
+)
+
 AwsEcsTaskDefinitionDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionDetailsTypeDef",
     {
         "ContainerDefinitions": Sequence[AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef],
         "Cpu": str,
         "ExecutionRoleArn": str,
         "Family": str,
@@ -8576,14 +11385,78 @@
         "Kubernetes": AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef,
         "MalwareProtection": AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef,
         "S3Logs": AwsGuardDutyDetectorDataSourcesS3LogsDetailsTypeDef,
     },
     total=False,
 )
 
+AwsRdsDbInstanceDetailsOutputTypeDef = TypedDict(
+    "AwsRdsDbInstanceDetailsOutputTypeDef",
+    {
+        "AssociatedRoles": List[AwsRdsDbInstanceAssociatedRoleTypeDef],
+        "CACertificateIdentifier": str,
+        "DBClusterIdentifier": str,
+        "DBInstanceIdentifier": str,
+        "DBInstanceClass": str,
+        "DbInstancePort": int,
+        "DbiResourceId": str,
+        "DBName": str,
+        "DeletionProtection": bool,
+        "Endpoint": AwsRdsDbInstanceEndpointTypeDef,
+        "Engine": str,
+        "EngineVersion": str,
+        "IAMDatabaseAuthenticationEnabled": bool,
+        "InstanceCreateTime": str,
+        "KmsKeyId": str,
+        "PubliclyAccessible": bool,
+        "StorageEncrypted": bool,
+        "TdeCredentialArn": str,
+        "VpcSecurityGroups": List[AwsRdsDbInstanceVpcSecurityGroupTypeDef],
+        "MultiAz": bool,
+        "EnhancedMonitoringResourceArn": str,
+        "DbInstanceStatus": str,
+        "MasterUsername": str,
+        "AllocatedStorage": int,
+        "PreferredBackupWindow": str,
+        "BackupRetentionPeriod": int,
+        "DbSecurityGroups": List[str],
+        "DbParameterGroups": List[AwsRdsDbParameterGroupTypeDef],
+        "AvailabilityZone": str,
+        "DbSubnetGroup": AwsRdsDbSubnetGroupOutputTypeDef,
+        "PreferredMaintenanceWindow": str,
+        "PendingModifiedValues": AwsRdsDbPendingModifiedValuesOutputTypeDef,
+        "LatestRestorableTime": str,
+        "AutoMinorVersionUpgrade": bool,
+        "ReadReplicaSourceDBInstanceIdentifier": str,
+        "ReadReplicaDBInstanceIdentifiers": List[str],
+        "ReadReplicaDBClusterIdentifiers": List[str],
+        "LicenseModel": str,
+        "Iops": int,
+        "OptionGroupMemberships": List[AwsRdsDbOptionGroupMembershipTypeDef],
+        "CharacterSetName": str,
+        "SecondaryAvailabilityZone": str,
+        "StatusInfos": List[AwsRdsDbStatusInfoTypeDef],
+        "StorageType": str,
+        "DomainMemberships": List[AwsRdsDbDomainMembershipTypeDef],
+        "CopyTagsToSnapshot": bool,
+        "MonitoringInterval": int,
+        "MonitoringRoleArn": str,
+        "PromotionTier": int,
+        "Timezone": str,
+        "PerformanceInsightsEnabled": bool,
+        "PerformanceInsightsKmsKeyId": str,
+        "PerformanceInsightsRetentionPeriod": int,
+        "EnabledCloudWatchLogsExports": List[str],
+        "ProcessorFeatures": List[AwsRdsDbProcessorFeatureTypeDef],
+        "ListenerEndpoint": AwsRdsDbInstanceEndpointTypeDef,
+        "MaxAllocatedStorage": int,
+    },
+    total=False,
+)
+
 AwsRdsDbInstanceDetailsTypeDef = TypedDict(
     "AwsRdsDbInstanceDetailsTypeDef",
     {
         "AssociatedRoles": Sequence[AwsRdsDbInstanceAssociatedRoleTypeDef],
         "CACertificateIdentifier": str,
         "DBClusterIdentifier": str,
         "DBInstanceIdentifier": str,
@@ -8640,33 +11513,69 @@
         "ProcessorFeatures": Sequence[AwsRdsDbProcessorFeatureTypeDef],
         "ListenerEndpoint": AwsRdsDbInstanceEndpointTypeDef,
         "MaxAllocatedStorage": int,
     },
     total=False,
 )
 
+AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsOutputTypeDef = TypedDict(
+    "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsOutputTypeDef",
+    {
+        "Predicate": (
+            AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsOutputTypeDef
+        ),
+    },
+    total=False,
+)
+
 AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef",
     {
         "Predicate": AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef,
     },
     total=False,
 )
 
+AwsS3BucketNotificationConfigurationDetailOutputTypeDef = TypedDict(
+    "AwsS3BucketNotificationConfigurationDetailOutputTypeDef",
+    {
+        "Events": List[str],
+        "Filter": AwsS3BucketNotificationConfigurationFilterOutputTypeDef,
+        "Destination": str,
+        "Type": str,
+    },
+    total=False,
+)
+
 AwsS3BucketNotificationConfigurationDetailTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationDetailTypeDef",
     {
         "Events": Sequence[str],
         "Filter": AwsS3BucketNotificationConfigurationFilterTypeDef,
         "Destination": str,
         "Type": str,
     },
     total=False,
 )
 
+AwsStepFunctionStateMachineDetailsOutputTypeDef = TypedDict(
+    "AwsStepFunctionStateMachineDetailsOutputTypeDef",
+    {
+        "Label": str,
+        "LoggingConfiguration": AwsStepFunctionStateMachineLoggingConfigurationDetailsOutputTypeDef,
+        "Name": str,
+        "RoleArn": str,
+        "StateMachineArn": str,
+        "Status": str,
+        "TracingConfiguration": AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef,
+        "Type": str,
+    },
+    total=False,
+)
+
 AwsStepFunctionStateMachineDetailsTypeDef = TypedDict(
     "AwsStepFunctionStateMachineDetailsTypeDef",
     {
         "Label": str,
         "LoggingConfiguration": AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef,
         "Name": str,
         "RoleArn": str,
@@ -8674,14 +11583,34 @@
         "Status": str,
         "TracingConfiguration": AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef,
         "Type": str,
     },
     total=False,
 )
 
+AwsWafv2RulesActionDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2RulesActionDetailsOutputTypeDef",
+    {
+        "Allow": AwsWafv2ActionAllowDetailsOutputTypeDef,
+        "Block": AwsWafv2ActionBlockDetailsOutputTypeDef,
+        "Captcha": AwsWafv2RulesActionCaptchaDetailsOutputTypeDef,
+        "Count": AwsWafv2RulesActionCountDetailsOutputTypeDef,
+    },
+    total=False,
+)
+
+AwsWafv2WebAclActionDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2WebAclActionDetailsOutputTypeDef",
+    {
+        "Allow": AwsWafv2ActionAllowDetailsOutputTypeDef,
+        "Block": AwsWafv2ActionBlockDetailsOutputTypeDef,
+    },
+    total=False,
+)
+
 AwsWafv2RulesActionDetailsTypeDef = TypedDict(
     "AwsWafv2RulesActionDetailsTypeDef",
     {
         "Allow": AwsWafv2ActionAllowDetailsTypeDef,
         "Block": AwsWafv2ActionBlockDetailsTypeDef,
         "Captcha": AwsWafv2RulesActionCaptchaDetailsTypeDef,
         "Count": AwsWafv2RulesActionCountDetailsTypeDef,
@@ -8703,49 +11632,26 @@
     {
         "RuleArn": str,
         "RuleStatus": RuleStatusType,
         "RuleOrder": int,
         "RuleName": str,
         "Description": str,
         "IsTerminal": bool,
-        "Criteria": AutomationRulesFindingFiltersTypeDef,
-        "Actions": List[AutomationRulesActionTypeDef],
+        "Criteria": AutomationRulesFindingFiltersOutputTypeDef,
+        "Actions": List[AutomationRulesActionOutputTypeDef],
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
         "CreatedBy": str,
     },
     total=False,
 )
 
-_RequiredCreateAutomationRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAutomationRuleRequestRequestTypeDef",
-    {
-        "RuleOrder": int,
-        "RuleName": str,
-        "Description": str,
-        "Criteria": AutomationRulesFindingFiltersTypeDef,
-        "Actions": Sequence[AutomationRulesActionTypeDef],
-    },
-)
-_OptionalCreateAutomationRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAutomationRuleRequestRequestTypeDef",
-    {
-        "Tags": Mapping[str, str],
-        "RuleStatus": RuleStatusType,
-        "IsTerminal": bool,
-    },
-    total=False,
-)
-
-class CreateAutomationRuleRequestRequestTypeDef(
-    _RequiredCreateAutomationRuleRequestRequestTypeDef,
-    _OptionalCreateAutomationRuleRequestRequestTypeDef,
-):
-    pass
-
+AutomationRulesFindingFiltersUnionTypeDef = Union[
+    AutomationRulesFindingFiltersTypeDef, AutomationRulesFindingFiltersOutputTypeDef
+]
 _RequiredUpdateAutomationRulesRequestItemTypeDef = TypedDict(
     "_RequiredUpdateAutomationRulesRequestItemTypeDef",
     {
         "RuleArn": str,
     },
 )
 _OptionalUpdateAutomationRulesRequestItemTypeDef = TypedDict(
@@ -8764,29 +11670,42 @@
 
 class UpdateAutomationRulesRequestItemTypeDef(
     _RequiredUpdateAutomationRulesRequestItemTypeDef,
     _OptionalUpdateAutomationRulesRequestItemTypeDef,
 ):
     pass
 
+InsightTypeDef = TypedDict(
+    "InsightTypeDef",
+    {
+        "InsightArn": str,
+        "Name": str,
+        "Filters": AwsSecurityFindingFiltersOutputTypeDef,
+        "GroupByAttribute": str,
+    },
+)
+
+AwsSecurityFindingFiltersUnionTypeDef = Union[
+    AwsSecurityFindingFiltersTypeDef, AwsSecurityFindingFiltersOutputTypeDef
+]
 CreateInsightRequestRequestTypeDef = TypedDict(
     "CreateInsightRequestRequestTypeDef",
     {
         "Name": str,
         "Filters": AwsSecurityFindingFiltersTypeDef,
         "GroupByAttribute": str,
     },
 )
 
 GetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
     "GetFindingsRequestGetFindingsPaginateTypeDef",
     {
         "Filters": AwsSecurityFindingFiltersTypeDef,
         "SortCriteria": Sequence[SortCriterionTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetFindingsRequestRequestTypeDef = TypedDict(
     "GetFindingsRequestRequestTypeDef",
     {
@@ -8794,24 +11713,14 @@
         "SortCriteria": Sequence[SortCriterionTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-InsightTypeDef = TypedDict(
-    "InsightTypeDef",
-    {
-        "InsightArn": str,
-        "Name": str,
-        "Filters": AwsSecurityFindingFiltersTypeDef,
-        "GroupByAttribute": str,
-    },
-)
-
 _RequiredUpdateFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFindingsRequestRequestTypeDef",
     {
         "Filters": AwsSecurityFindingFiltersTypeDef,
     },
 )
 _OptionalUpdateFindingsRequestRequestTypeDef = TypedDict(
@@ -8845,25 +11754,57 @@
 )
 
 class UpdateInsightRequestRequestTypeDef(
     _RequiredUpdateInsightRequestRequestTypeDef, _OptionalUpdateInsightRequestRequestTypeDef
 ):
     pass
 
+NetworkPathComponentOutputTypeDef = TypedDict(
+    "NetworkPathComponentOutputTypeDef",
+    {
+        "ComponentId": str,
+        "ComponentType": str,
+        "Egress": NetworkHeaderOutputTypeDef,
+        "Ingress": NetworkHeaderOutputTypeDef,
+    },
+    total=False,
+)
+
 NetworkPathComponentTypeDef = TypedDict(
     "NetworkPathComponentTypeDef",
     {
         "ComponentId": str,
         "ComponentType": str,
         "Egress": NetworkHeaderTypeDef,
         "Ingress": NetworkHeaderTypeDef,
     },
     total=False,
 )
 
+CustomDataIdentifiersDetectionsOutputTypeDef = TypedDict(
+    "CustomDataIdentifiersDetectionsOutputTypeDef",
+    {
+        "Count": int,
+        "Arn": str,
+        "Name": str,
+        "Occurrences": OccurrencesOutputTypeDef,
+    },
+    total=False,
+)
+
+SensitiveDataDetectionsOutputTypeDef = TypedDict(
+    "SensitiveDataDetectionsOutputTypeDef",
+    {
+        "Count": int,
+        "Type": str,
+        "Occurrences": OccurrencesOutputTypeDef,
+    },
+    total=False,
+)
+
 CustomDataIdentifiersDetectionsTypeDef = TypedDict(
     "CustomDataIdentifiersDetectionsTypeDef",
     {
         "Count": int,
         "Arn": str,
         "Name": str,
         "Occurrences": OccurrencesTypeDef,
@@ -8877,23 +11818,50 @@
         "Count": int,
         "Type": str,
         "Occurrences": OccurrencesTypeDef,
     },
     total=False,
 )
 
+RuleGroupSourceStatelessRulesDetailsOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRulesDetailsOutputTypeDef",
+    {
+        "Priority": int,
+        "RuleDefinition": RuleGroupSourceStatelessRuleDefinitionOutputTypeDef,
+    },
+    total=False,
+)
+
 RuleGroupSourceStatelessRulesDetailsTypeDef = TypedDict(
     "RuleGroupSourceStatelessRulesDetailsTypeDef",
     {
         "Priority": int,
         "RuleDefinition": RuleGroupSourceStatelessRuleDefinitionTypeDef,
     },
     total=False,
 )
 
+FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef = TypedDict(
+    "FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef",
+    {
+        "ActionDefinition": StatelessCustomActionDefinitionOutputTypeDef,
+        "ActionName": str,
+    },
+    total=False,
+)
+
+RuleGroupSourceCustomActionsDetailsOutputTypeDef = TypedDict(
+    "RuleGroupSourceCustomActionsDetailsOutputTypeDef",
+    {
+        "ActionDefinition": StatelessCustomActionDefinitionOutputTypeDef,
+        "ActionName": str,
+    },
+    total=False,
+)
+
 FirewallPolicyStatelessCustomActionsDetailsTypeDef = TypedDict(
     "FirewallPolicyStatelessCustomActionsDetailsTypeDef",
     {
         "ActionDefinition": StatelessCustomActionDefinitionTypeDef,
         "ActionName": str,
     },
     total=False,
@@ -8904,37 +11872,105 @@
     {
         "ActionDefinition": StatelessCustomActionDefinitionTypeDef,
         "ActionName": str,
     },
     total=False,
 )
 
+ActionOutputTypeDef = TypedDict(
+    "ActionOutputTypeDef",
+    {
+        "ActionType": str,
+        "NetworkConnectionAction": NetworkConnectionActionTypeDef,
+        "AwsApiCallAction": AwsApiCallActionOutputTypeDef,
+        "DnsRequestAction": DnsRequestActionTypeDef,
+        "PortProbeAction": PortProbeActionOutputTypeDef,
+    },
+    total=False,
+)
+
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "ActionType": str,
         "NetworkConnectionAction": NetworkConnectionActionTypeDef,
         "AwsApiCallAction": AwsApiCallActionTypeDef,
         "DnsRequestAction": DnsRequestActionTypeDef,
         "PortProbeAction": PortProbeActionTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateAutomationRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAutomationRuleRequestRequestTypeDef",
+    {
+        "RuleOrder": int,
+        "RuleName": str,
+        "Description": str,
+        "Criteria": AutomationRulesFindingFiltersTypeDef,
+        "Actions": Sequence[AutomationRulesActionUnionTypeDef],
+    },
+)
+_OptionalCreateAutomationRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAutomationRuleRequestRequestTypeDef",
+    {
+        "Tags": Mapping[str, str],
+        "RuleStatus": RuleStatusType,
+        "IsTerminal": bool,
+    },
+    total=False,
+)
+
+class CreateAutomationRuleRequestRequestTypeDef(
+    _RequiredCreateAutomationRuleRequestRequestTypeDef,
+    _OptionalCreateAutomationRuleRequestRequestTypeDef,
+):
+    pass
+
+AwsBackupBackupPlanDetailsOutputTypeDef = TypedDict(
+    "AwsBackupBackupPlanDetailsOutputTypeDef",
+    {
+        "BackupPlan": AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef,
+        "BackupPlanArn": str,
+        "BackupPlanId": str,
+        "VersionId": str,
+    },
+    total=False,
+)
+
 AwsBackupBackupPlanDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanDetailsTypeDef",
     {
         "BackupPlan": AwsBackupBackupPlanBackupPlanDetailsTypeDef,
         "BackupPlanArn": str,
         "BackupPlanId": str,
         "VersionId": str,
     },
     total=False,
 )
 
+AwsCloudFrontDistributionDetailsOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionDetailsOutputTypeDef",
+    {
+        "CacheBehaviors": AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef,
+        "DefaultCacheBehavior": AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef,
+        "DefaultRootObject": str,
+        "DomainName": str,
+        "ETag": str,
+        "LastModifiedTime": str,
+        "Logging": AwsCloudFrontDistributionLoggingTypeDef,
+        "Origins": AwsCloudFrontDistributionOriginsOutputTypeDef,
+        "OriginGroups": AwsCloudFrontDistributionOriginGroupsOutputTypeDef,
+        "ViewerCertificate": AwsCloudFrontDistributionViewerCertificateTypeDef,
+        "Status": str,
+        "WebAclId": str,
+    },
+    total=False,
+)
+
 AwsCloudFrontDistributionDetailsTypeDef = TypedDict(
     "AwsCloudFrontDistributionDetailsTypeDef",
     {
         "CacheBehaviors": AwsCloudFrontDistributionCacheBehaviorsTypeDef,
         "DefaultCacheBehavior": AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef,
         "DefaultRootObject": str,
         "DomainName": str,
@@ -8946,26 +11982,60 @@
         "ViewerCertificate": AwsCloudFrontDistributionViewerCertificateTypeDef,
         "Status": str,
         "WebAclId": str,
     },
     total=False,
 )
 
+AwsGuardDutyDetectorDetailsOutputTypeDef = TypedDict(
+    "AwsGuardDutyDetectorDetailsOutputTypeDef",
+    {
+        "DataSources": AwsGuardDutyDetectorDataSourcesDetailsTypeDef,
+        "Features": List[AwsGuardDutyDetectorFeaturesDetailsTypeDef],
+        "FindingPublishingFrequency": str,
+        "ServiceRole": str,
+        "Status": str,
+    },
+    total=False,
+)
+
 AwsGuardDutyDetectorDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDetailsTypeDef",
     {
         "DataSources": AwsGuardDutyDetectorDataSourcesDetailsTypeDef,
         "Features": Sequence[AwsGuardDutyDetectorFeaturesDetailsTypeDef],
         "FindingPublishingFrequency": str,
         "ServiceRole": str,
         "Status": str,
     },
     total=False,
 )
 
+AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef = TypedDict(
+    "AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef",
+    {
+        "AbortIncompleteMultipartUpload": (
+            AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef
+        ),
+        "ExpirationDate": str,
+        "ExpirationInDays": int,
+        "ExpiredObjectDeleteMarker": bool,
+        "Filter": AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsOutputTypeDef,
+        "ID": str,
+        "NoncurrentVersionExpirationInDays": int,
+        "NoncurrentVersionTransitions": List[
+            AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsTypeDef
+        ],
+        "Prefix": str,
+        "Status": str,
+        "Transitions": List[AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsTypeDef],
+    },
+    total=False,
+)
+
 AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef",
     {
         "AbortIncompleteMultipartUpload": (
             AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef
         ),
         "ExpirationDate": str,
@@ -8982,22 +12052,42 @@
         "Transitions": Sequence[
             AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsTypeDef
         ],
     },
     total=False,
 )
 
+AwsS3BucketNotificationConfigurationOutputTypeDef = TypedDict(
+    "AwsS3BucketNotificationConfigurationOutputTypeDef",
+    {
+        "Configurations": List[AwsS3BucketNotificationConfigurationDetailOutputTypeDef],
+    },
+    total=False,
+)
+
 AwsS3BucketNotificationConfigurationTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationTypeDef",
     {
         "Configurations": Sequence[AwsS3BucketNotificationConfigurationDetailTypeDef],
     },
     total=False,
 )
 
+AwsWafv2RulesDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2RulesDetailsOutputTypeDef",
+    {
+        "Action": AwsWafv2RulesActionDetailsOutputTypeDef,
+        "Name": str,
+        "OverrideAction": str,
+        "Priority": int,
+        "VisibilityConfig": AwsWafv2VisibilityConfigDetailsTypeDef,
+    },
+    total=False,
+)
+
 AwsWafv2RulesDetailsTypeDef = TypedDict(
     "AwsWafv2RulesDetailsTypeDef",
     {
         "Action": AwsWafv2RulesActionDetailsTypeDef,
         "Name": str,
         "OverrideAction": str,
         "Priority": int,
@@ -9007,15 +12097,15 @@
 )
 
 BatchGetAutomationRulesResponseTypeDef = TypedDict(
     "BatchGetAutomationRulesResponseTypeDef",
     {
         "Rules": List[AutomationRulesConfigTypeDef],
         "UnprocessedAutomationRules": List[UnprocessedAutomationRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateAutomationRulesRequestRequestTypeDef = TypedDict(
     "BatchUpdateAutomationRulesRequestRequestTypeDef",
     {
         "UpdateAutomationRulesRequestItems": Sequence[UpdateAutomationRulesRequestItemTypeDef],
@@ -9023,18 +12113,37 @@
 )
 
 GetInsightsResponseTypeDef = TypedDict(
     "GetInsightsResponseTypeDef",
     {
         "Insights": List[InsightTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CustomDataIdentifiersResultOutputTypeDef = TypedDict(
+    "CustomDataIdentifiersResultOutputTypeDef",
+    {
+        "Detections": List[CustomDataIdentifiersDetectionsOutputTypeDef],
+        "TotalCount": int,
+    },
+    total=False,
+)
+
+SensitiveDataResultOutputTypeDef = TypedDict(
+    "SensitiveDataResultOutputTypeDef",
+    {
+        "Category": str,
+        "Detections": List[SensitiveDataDetectionsOutputTypeDef],
+        "TotalCount": int,
+    },
+    total=False,
+)
+
 CustomDataIdentifiersResultTypeDef = TypedDict(
     "CustomDataIdentifiersResultTypeDef",
     {
         "Detections": Sequence[CustomDataIdentifiersDetectionsTypeDef],
         "TotalCount": int,
     },
     total=False,
@@ -9046,14 +12155,39 @@
         "Category": str,
         "Detections": Sequence[SensitiveDataDetectionsTypeDef],
         "TotalCount": int,
     },
     total=False,
 )
 
+FirewallPolicyDetailsOutputTypeDef = TypedDict(
+    "FirewallPolicyDetailsOutputTypeDef",
+    {
+        "StatefulRuleGroupReferences": List[
+            FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef
+        ],
+        "StatelessCustomActions": List[FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef],
+        "StatelessDefaultActions": List[str],
+        "StatelessFragmentDefaultActions": List[str],
+        "StatelessRuleGroupReferences": List[
+            FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef
+        ],
+    },
+    total=False,
+)
+
+RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef",
+    {
+        "CustomActions": List[RuleGroupSourceCustomActionsDetailsOutputTypeDef],
+        "StatelessRules": List[RuleGroupSourceStatelessRulesDetailsOutputTypeDef],
+    },
+    total=False,
+)
+
 FirewallPolicyDetailsTypeDef = TypedDict(
     "FirewallPolicyDetailsTypeDef",
     {
         "StatefulRuleGroupReferences": Sequence[
             FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef
         ],
         "StatelessCustomActions": Sequence[FirewallPolicyStatelessCustomActionsDetailsTypeDef],
@@ -9071,22 +12205,62 @@
     {
         "CustomActions": Sequence[RuleGroupSourceCustomActionsDetailsTypeDef],
         "StatelessRules": Sequence[RuleGroupSourceStatelessRulesDetailsTypeDef],
     },
     total=False,
 )
 
+AwsS3BucketBucketLifecycleConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsS3BucketBucketLifecycleConfigurationDetailsOutputTypeDef",
+    {
+        "Rules": List[AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef],
+    },
+    total=False,
+)
+
 AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef",
     {
         "Rules": Sequence[AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef],
     },
     total=False,
 )
 
+AwsWafv2RuleGroupDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2RuleGroupDetailsOutputTypeDef",
+    {
+        "Capacity": int,
+        "Description": str,
+        "Id": str,
+        "Name": str,
+        "Arn": str,
+        "Rules": List[AwsWafv2RulesDetailsOutputTypeDef],
+        "Scope": str,
+        "VisibilityConfig": AwsWafv2VisibilityConfigDetailsTypeDef,
+    },
+    total=False,
+)
+
+AwsWafv2WebAclDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2WebAclDetailsOutputTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "ManagedbyFirewallManager": bool,
+        "Id": str,
+        "Capacity": int,
+        "CaptchaConfig": AwsWafv2WebAclCaptchaConfigDetailsTypeDef,
+        "DefaultAction": AwsWafv2WebAclActionDetailsOutputTypeDef,
+        "Description": str,
+        "Rules": List[AwsWafv2RulesDetailsOutputTypeDef],
+        "VisibilityConfig": AwsWafv2VisibilityConfigDetailsTypeDef,
+    },
+    total=False,
+)
+
 AwsWafv2RuleGroupDetailsTypeDef = TypedDict(
     "AwsWafv2RuleGroupDetailsTypeDef",
     {
         "Capacity": int,
         "Description": str,
         "Id": str,
         "Name": str,
@@ -9111,27 +12285,65 @@
         "Description": str,
         "Rules": Sequence[AwsWafv2RulesDetailsTypeDef],
         "VisibilityConfig": AwsWafv2VisibilityConfigDetailsTypeDef,
     },
     total=False,
 )
 
+ClassificationResultOutputTypeDef = TypedDict(
+    "ClassificationResultOutputTypeDef",
+    {
+        "MimeType": str,
+        "SizeClassified": int,
+        "AdditionalOccurrences": bool,
+        "Status": ClassificationStatusTypeDef,
+        "SensitiveData": List[SensitiveDataResultOutputTypeDef],
+        "CustomDataIdentifiers": CustomDataIdentifiersResultOutputTypeDef,
+    },
+    total=False,
+)
+
 ClassificationResultTypeDef = TypedDict(
     "ClassificationResultTypeDef",
     {
         "MimeType": str,
         "SizeClassified": int,
         "AdditionalOccurrences": bool,
         "Status": ClassificationStatusTypeDef,
         "SensitiveData": Sequence[SensitiveDataResultTypeDef],
         "CustomDataIdentifiers": CustomDataIdentifiersResultTypeDef,
     },
     total=False,
 )
 
+AwsNetworkFirewallFirewallPolicyDetailsOutputTypeDef = TypedDict(
+    "AwsNetworkFirewallFirewallPolicyDetailsOutputTypeDef",
+    {
+        "FirewallPolicy": FirewallPolicyDetailsOutputTypeDef,
+        "FirewallPolicyArn": str,
+        "FirewallPolicyId": str,
+        "FirewallPolicyName": str,
+        "Description": str,
+    },
+    total=False,
+)
+
+RuleGroupSourceOutputTypeDef = TypedDict(
+    "RuleGroupSourceOutputTypeDef",
+    {
+        "RulesSourceList": RuleGroupSourceListDetailsOutputTypeDef,
+        "RulesString": str,
+        "StatefulRules": List[RuleGroupSourceStatefulRulesDetailsOutputTypeDef],
+        "StatelessRulesAndCustomActions": (
+            RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef
+        ),
+    },
+    total=False,
+)
+
 AwsNetworkFirewallFirewallPolicyDetailsTypeDef = TypedDict(
     "AwsNetworkFirewallFirewallPolicyDetailsTypeDef",
     {
         "FirewallPolicy": FirewallPolicyDetailsTypeDef,
         "FirewallPolicyArn": str,
         "FirewallPolicyId": str,
         "FirewallPolicyName": str,
@@ -9149,14 +12361,36 @@
         "StatelessRulesAndCustomActions": (
             RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef
         ),
     },
     total=False,
 )
 
+AwsS3BucketDetailsOutputTypeDef = TypedDict(
+    "AwsS3BucketDetailsOutputTypeDef",
+    {
+        "OwnerId": str,
+        "OwnerName": str,
+        "OwnerAccountId": str,
+        "CreatedAt": str,
+        "ServerSideEncryptionConfiguration": (
+            AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef
+        ),
+        "BucketLifecycleConfiguration": AwsS3BucketBucketLifecycleConfigurationDetailsOutputTypeDef,
+        "PublicAccessBlockConfiguration": AwsS3AccountPublicAccessBlockDetailsTypeDef,
+        "AccessControlList": str,
+        "BucketLoggingConfiguration": AwsS3BucketLoggingConfigurationTypeDef,
+        "BucketWebsiteConfiguration": AwsS3BucketWebsiteConfigurationOutputTypeDef,
+        "BucketNotificationConfiguration": AwsS3BucketNotificationConfigurationOutputTypeDef,
+        "BucketVersioningConfiguration": AwsS3BucketBucketVersioningConfigurationTypeDef,
+        "ObjectLockConfiguration": AwsS3BucketObjectLockConfigurationTypeDef,
+    },
+    total=False,
+)
+
 AwsS3BucketDetailsTypeDef = TypedDict(
     "AwsS3BucketDetailsTypeDef",
     {
         "OwnerId": str,
         "OwnerName": str,
         "OwnerAccountId": str,
         "CreatedAt": str,
@@ -9169,46 +12403,174 @@
         "BucketNotificationConfiguration": AwsS3BucketNotificationConfigurationTypeDef,
         "BucketVersioningConfiguration": AwsS3BucketBucketVersioningConfigurationTypeDef,
         "ObjectLockConfiguration": AwsS3BucketObjectLockConfigurationTypeDef,
     },
     total=False,
 )
 
+DataClassificationDetailsOutputTypeDef = TypedDict(
+    "DataClassificationDetailsOutputTypeDef",
+    {
+        "DetailedResultsLocation": str,
+        "Result": ClassificationResultOutputTypeDef,
+    },
+    total=False,
+)
+
 DataClassificationDetailsTypeDef = TypedDict(
     "DataClassificationDetailsTypeDef",
     {
         "DetailedResultsLocation": str,
         "Result": ClassificationResultTypeDef,
     },
     total=False,
 )
 
+RuleGroupDetailsOutputTypeDef = TypedDict(
+    "RuleGroupDetailsOutputTypeDef",
+    {
+        "RuleVariables": RuleGroupVariablesOutputTypeDef,
+        "RulesSource": RuleGroupSourceOutputTypeDef,
+    },
+    total=False,
+)
+
 RuleGroupDetailsTypeDef = TypedDict(
     "RuleGroupDetailsTypeDef",
     {
         "RuleVariables": RuleGroupVariablesTypeDef,
         "RulesSource": RuleGroupSourceTypeDef,
     },
     total=False,
 )
 
+AwsNetworkFirewallRuleGroupDetailsOutputTypeDef = TypedDict(
+    "AwsNetworkFirewallRuleGroupDetailsOutputTypeDef",
+    {
+        "Capacity": int,
+        "Description": str,
+        "RuleGroup": RuleGroupDetailsOutputTypeDef,
+        "RuleGroupArn": str,
+        "RuleGroupId": str,
+        "RuleGroupName": str,
+        "Type": str,
+    },
+    total=False,
+)
+
 AwsNetworkFirewallRuleGroupDetailsTypeDef = TypedDict(
     "AwsNetworkFirewallRuleGroupDetailsTypeDef",
     {
         "Capacity": int,
         "Description": str,
         "RuleGroup": RuleGroupDetailsTypeDef,
         "RuleGroupArn": str,
         "RuleGroupId": str,
         "RuleGroupName": str,
         "Type": str,
     },
     total=False,
 )
 
+ResourceDetailsOutputTypeDef = TypedDict(
+    "ResourceDetailsOutputTypeDef",
+    {
+        "AwsAutoScalingAutoScalingGroup": AwsAutoScalingAutoScalingGroupDetailsOutputTypeDef,
+        "AwsCodeBuildProject": AwsCodeBuildProjectDetailsOutputTypeDef,
+        "AwsCloudFrontDistribution": AwsCloudFrontDistributionDetailsOutputTypeDef,
+        "AwsEc2Instance": AwsEc2InstanceDetailsOutputTypeDef,
+        "AwsEc2NetworkInterface": AwsEc2NetworkInterfaceDetailsOutputTypeDef,
+        "AwsEc2SecurityGroup": AwsEc2SecurityGroupDetailsOutputTypeDef,
+        "AwsEc2Volume": AwsEc2VolumeDetailsOutputTypeDef,
+        "AwsEc2Vpc": AwsEc2VpcDetailsOutputTypeDef,
+        "AwsEc2Eip": AwsEc2EipDetailsTypeDef,
+        "AwsEc2Subnet": AwsEc2SubnetDetailsOutputTypeDef,
+        "AwsEc2NetworkAcl": AwsEc2NetworkAclDetailsOutputTypeDef,
+        "AwsElbv2LoadBalancer": AwsElbv2LoadBalancerDetailsOutputTypeDef,
+        "AwsElasticBeanstalkEnvironment": AwsElasticBeanstalkEnvironmentDetailsOutputTypeDef,
+        "AwsElasticsearchDomain": AwsElasticsearchDomainDetailsOutputTypeDef,
+        "AwsS3Bucket": AwsS3BucketDetailsOutputTypeDef,
+        "AwsS3AccountPublicAccessBlock": AwsS3AccountPublicAccessBlockDetailsTypeDef,
+        "AwsS3Object": AwsS3ObjectDetailsTypeDef,
+        "AwsSecretsManagerSecret": AwsSecretsManagerSecretDetailsTypeDef,
+        "AwsIamAccessKey": AwsIamAccessKeyDetailsTypeDef,
+        "AwsIamUser": AwsIamUserDetailsOutputTypeDef,
+        "AwsIamPolicy": AwsIamPolicyDetailsOutputTypeDef,
+        "AwsApiGatewayV2Stage": AwsApiGatewayV2StageDetailsOutputTypeDef,
+        "AwsApiGatewayV2Api": AwsApiGatewayV2ApiDetailsOutputTypeDef,
+        "AwsDynamoDbTable": AwsDynamoDbTableDetailsOutputTypeDef,
+        "AwsApiGatewayStage": AwsApiGatewayStageDetailsOutputTypeDef,
+        "AwsApiGatewayRestApi": AwsApiGatewayRestApiDetailsOutputTypeDef,
+        "AwsCloudTrailTrail": AwsCloudTrailTrailDetailsTypeDef,
+        "AwsSsmPatchCompliance": AwsSsmPatchComplianceDetailsTypeDef,
+        "AwsCertificateManagerCertificate": AwsCertificateManagerCertificateDetailsOutputTypeDef,
+        "AwsRedshiftCluster": AwsRedshiftClusterDetailsOutputTypeDef,
+        "AwsElbLoadBalancer": AwsElbLoadBalancerDetailsOutputTypeDef,
+        "AwsIamGroup": AwsIamGroupDetailsOutputTypeDef,
+        "AwsIamRole": AwsIamRoleDetailsOutputTypeDef,
+        "AwsKmsKey": AwsKmsKeyDetailsTypeDef,
+        "AwsLambdaFunction": AwsLambdaFunctionDetailsOutputTypeDef,
+        "AwsLambdaLayerVersion": AwsLambdaLayerVersionDetailsOutputTypeDef,
+        "AwsRdsDbInstance": AwsRdsDbInstanceDetailsOutputTypeDef,
+        "AwsSnsTopic": AwsSnsTopicDetailsOutputTypeDef,
+        "AwsSqsQueue": AwsSqsQueueDetailsTypeDef,
+        "AwsWafWebAcl": AwsWafWebAclDetailsOutputTypeDef,
+        "AwsRdsDbSnapshot": AwsRdsDbSnapshotDetailsOutputTypeDef,
+        "AwsRdsDbClusterSnapshot": AwsRdsDbClusterSnapshotDetailsOutputTypeDef,
+        "AwsRdsDbCluster": AwsRdsDbClusterDetailsOutputTypeDef,
+        "AwsEcsCluster": AwsEcsClusterDetailsOutputTypeDef,
+        "AwsEcsContainer": AwsEcsContainerDetailsOutputTypeDef,
+        "AwsEcsTaskDefinition": AwsEcsTaskDefinitionDetailsOutputTypeDef,
+        "Container": ContainerDetailsOutputTypeDef,
+        "Other": Dict[str, str],
+        "AwsRdsEventSubscription": AwsRdsEventSubscriptionDetailsOutputTypeDef,
+        "AwsEcsService": AwsEcsServiceDetailsOutputTypeDef,
+        "AwsAutoScalingLaunchConfiguration": AwsAutoScalingLaunchConfigurationDetailsOutputTypeDef,
+        "AwsEc2VpnConnection": AwsEc2VpnConnectionDetailsOutputTypeDef,
+        "AwsEcrContainerImage": AwsEcrContainerImageDetailsOutputTypeDef,
+        "AwsOpenSearchServiceDomain": AwsOpenSearchServiceDomainDetailsOutputTypeDef,
+        "AwsEc2VpcEndpointService": AwsEc2VpcEndpointServiceDetailsOutputTypeDef,
+        "AwsXrayEncryptionConfig": AwsXrayEncryptionConfigDetailsTypeDef,
+        "AwsWafRateBasedRule": AwsWafRateBasedRuleDetailsOutputTypeDef,
+        "AwsWafRegionalRateBasedRule": AwsWafRegionalRateBasedRuleDetailsOutputTypeDef,
+        "AwsEcrRepository": AwsEcrRepositoryDetailsTypeDef,
+        "AwsEksCluster": AwsEksClusterDetailsOutputTypeDef,
+        "AwsNetworkFirewallFirewallPolicy": AwsNetworkFirewallFirewallPolicyDetailsOutputTypeDef,
+        "AwsNetworkFirewallFirewall": AwsNetworkFirewallFirewallDetailsOutputTypeDef,
+        "AwsNetworkFirewallRuleGroup": AwsNetworkFirewallRuleGroupDetailsOutputTypeDef,
+        "AwsRdsDbSecurityGroup": AwsRdsDbSecurityGroupDetailsOutputTypeDef,
+        "AwsKinesisStream": AwsKinesisStreamDetailsTypeDef,
+        "AwsEc2TransitGateway": AwsEc2TransitGatewayDetailsOutputTypeDef,
+        "AwsEfsAccessPoint": AwsEfsAccessPointDetailsOutputTypeDef,
+        "AwsCloudFormationStack": AwsCloudFormationStackDetailsOutputTypeDef,
+        "AwsCloudWatchAlarm": AwsCloudWatchAlarmDetailsOutputTypeDef,
+        "AwsEc2VpcPeeringConnection": AwsEc2VpcPeeringConnectionDetailsOutputTypeDef,
+        "AwsWafRegionalRuleGroup": AwsWafRegionalRuleGroupDetailsOutputTypeDef,
+        "AwsWafRegionalRule": AwsWafRegionalRuleDetailsOutputTypeDef,
+        "AwsWafRegionalWebAcl": AwsWafRegionalWebAclDetailsOutputTypeDef,
+        "AwsWafRule": AwsWafRuleDetailsOutputTypeDef,
+        "AwsWafRuleGroup": AwsWafRuleGroupDetailsOutputTypeDef,
+        "AwsEcsTask": AwsEcsTaskDetailsOutputTypeDef,
+        "AwsBackupBackupVault": AwsBackupBackupVaultDetailsOutputTypeDef,
+        "AwsBackupBackupPlan": AwsBackupBackupPlanDetailsOutputTypeDef,
+        "AwsBackupRecoveryPoint": AwsBackupRecoveryPointDetailsTypeDef,
+        "AwsEc2LaunchTemplate": AwsEc2LaunchTemplateDetailsOutputTypeDef,
+        "AwsSageMakerNotebookInstance": AwsSageMakerNotebookInstanceDetailsOutputTypeDef,
+        "AwsWafv2WebAcl": AwsWafv2WebAclDetailsOutputTypeDef,
+        "AwsWafv2RuleGroup": AwsWafv2RuleGroupDetailsOutputTypeDef,
+        "AwsEc2RouteTable": AwsEc2RouteTableDetailsOutputTypeDef,
+        "AwsAmazonMqBroker": AwsAmazonMqBrokerDetailsOutputTypeDef,
+        "AwsAppSyncGraphQlApi": AwsAppSyncGraphQlApiDetailsOutputTypeDef,
+        "AwsEventSchemasRegistry": AwsEventSchemasRegistryDetailsTypeDef,
+        "AwsGuardDutyDetector": AwsGuardDutyDetectorDetailsOutputTypeDef,
+        "AwsStepFunctionStateMachine": AwsStepFunctionStateMachineDetailsOutputTypeDef,
+    },
+    total=False,
+)
+
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "AwsAutoScalingAutoScalingGroup": AwsAutoScalingAutoScalingGroupDetailsTypeDef,
         "AwsCodeBuildProject": AwsCodeBuildProjectDetailsTypeDef,
         "AwsCloudFrontDistribution": AwsCloudFrontDistributionDetailsTypeDef,
         "AwsEc2Instance": AwsEc2InstanceDetailsTypeDef,
@@ -9297,14 +12659,37 @@
         "AwsEventSchemasRegistry": AwsEventSchemasRegistryDetailsTypeDef,
         "AwsGuardDutyDetector": AwsGuardDutyDetectorDetailsTypeDef,
         "AwsStepFunctionStateMachine": AwsStepFunctionStateMachineDetailsTypeDef,
     },
     total=False,
 )
 
+_RequiredResourceOutputTypeDef = TypedDict(
+    "_RequiredResourceOutputTypeDef",
+    {
+        "Type": str,
+        "Id": str,
+    },
+)
+_OptionalResourceOutputTypeDef = TypedDict(
+    "_OptionalResourceOutputTypeDef",
+    {
+        "Partition": PartitionType,
+        "Region": str,
+        "ResourceRole": str,
+        "Tags": Dict[str, str],
+        "DataClassification": DataClassificationDetailsOutputTypeDef,
+        "Details": ResourceDetailsOutputTypeDef,
+    },
+    total=False,
+)
+
+class ResourceOutputTypeDef(_RequiredResourceOutputTypeDef, _OptionalResourceOutputTypeDef):
+    pass
+
 _RequiredResourceTypeDef = TypedDict(
     "_RequiredResourceTypeDef",
     {
         "Type": str,
         "Id": str,
     },
 )
@@ -9320,14 +12705,72 @@
     },
     total=False,
 )
 
 class ResourceTypeDef(_RequiredResourceTypeDef, _OptionalResourceTypeDef):
     pass
 
+_RequiredAwsSecurityFindingOutputTypeDef = TypedDict(
+    "_RequiredAwsSecurityFindingOutputTypeDef",
+    {
+        "SchemaVersion": str,
+        "Id": str,
+        "ProductArn": str,
+        "GeneratorId": str,
+        "AwsAccountId": str,
+        "CreatedAt": str,
+        "UpdatedAt": str,
+        "Title": str,
+        "Description": str,
+        "Resources": List[ResourceOutputTypeDef],
+    },
+)
+_OptionalAwsSecurityFindingOutputTypeDef = TypedDict(
+    "_OptionalAwsSecurityFindingOutputTypeDef",
+    {
+        "ProductName": str,
+        "CompanyName": str,
+        "Region": str,
+        "Types": List[str],
+        "FirstObservedAt": str,
+        "LastObservedAt": str,
+        "Severity": SeverityTypeDef,
+        "Confidence": int,
+        "Criticality": int,
+        "Remediation": RemediationTypeDef,
+        "SourceUrl": str,
+        "ProductFields": Dict[str, str],
+        "UserDefinedFields": Dict[str, str],
+        "Malware": List[MalwareTypeDef],
+        "Network": NetworkTypeDef,
+        "NetworkPath": List[NetworkPathComponentOutputTypeDef],
+        "Process": ProcessDetailsTypeDef,
+        "Threats": List[ThreatOutputTypeDef],
+        "ThreatIntelIndicators": List[ThreatIntelIndicatorTypeDef],
+        "Compliance": ComplianceOutputTypeDef,
+        "VerificationState": VerificationStateType,
+        "WorkflowState": WorkflowStateType,
+        "Workflow": WorkflowTypeDef,
+        "RecordState": RecordStateType,
+        "RelatedFindings": List[RelatedFindingTypeDef],
+        "Note": NoteTypeDef,
+        "Vulnerabilities": List[VulnerabilityOutputTypeDef],
+        "PatchSummary": PatchSummaryTypeDef,
+        "Action": ActionOutputTypeDef,
+        "FindingProviderFields": FindingProviderFieldsOutputTypeDef,
+        "Sample": bool,
+    },
+    total=False,
+)
+
+class AwsSecurityFindingOutputTypeDef(
+    _RequiredAwsSecurityFindingOutputTypeDef, _OptionalAwsSecurityFindingOutputTypeDef
+):
+    pass
+
 _RequiredAwsSecurityFindingTypeDef = TypedDict(
     "_RequiredAwsSecurityFindingTypeDef",
     {
         "SchemaVersion": str,
         "Id": str,
         "ProductArn": str,
         "GeneratorId": str,
@@ -9378,22 +12821,23 @@
 )
 
 class AwsSecurityFindingTypeDef(
     _RequiredAwsSecurityFindingTypeDef, _OptionalAwsSecurityFindingTypeDef
 ):
     pass
 
-BatchImportFindingsRequestRequestTypeDef = TypedDict(
-    "BatchImportFindingsRequestRequestTypeDef",
+GetFindingsResponseTypeDef = TypedDict(
+    "GetFindingsResponseTypeDef",
     {
-        "Findings": Sequence[AwsSecurityFindingTypeDef],
+        "Findings": List[AwsSecurityFindingOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetFindingsResponseTypeDef = TypedDict(
-    "GetFindingsResponseTypeDef",
+AwsSecurityFindingUnionTypeDef = Union[AwsSecurityFindingTypeDef, AwsSecurityFindingOutputTypeDef]
+BatchImportFindingsRequestRequestTypeDef = TypedDict(
+    "BatchImportFindingsRequestRequestTypeDef",
     {
-        "Findings": List[AwsSecurityFindingTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Findings": Sequence[AwsSecurityFindingUnionTypeDef],
     },
 )
```

### Comparing `types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub.egg-info/PKG-INFO` & `types-aiobotocore-securityhub-2.5.2.post1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,62 +1,29 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-securityhub
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SecurityHub 2.5.2 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore securityhub type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="types-aiobotocore-securityhub"></a>
 
 # types-aiobotocore-securityhub
 
 [![PyPI - types-aiobotocore-securityhub](https://img.shields.io/pypi/v/types-aiobotocore-securityhub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-securityhub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-securityhub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-securityhub)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-securityhub?color=blue)](https://pypistats.org/packages/types-aiobotocore-securityhub)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-securityhub)](https://pepy.tech/project/types-aiobotocore-securityhub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SecurityHub 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
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
 [types-aiobotocore-securityhub docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securityhub/).
 
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
@@ -404,107 +371,117 @@
 )
 
 
 def check_value(value: AdminStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_securityhub.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_securityhub.type_defs import (
     AcceptAdministratorInvitationRequestRequestTypeDef,
     AcceptInvitationRequestRequestTypeDef,
     AccountDetailsTypeDef,
     ActionLocalIpDetailsTypeDef,
     ActionLocalPortDetailsTypeDef,
+    DnsRequestActionTypeDef,
     CityTypeDef,
     CountryTypeDef,
     GeoLocationTypeDef,
     IpOrganizationDetailsTypeDef,
     ActionRemotePortDetailsTypeDef,
     ActionTargetTypeDef,
-    DnsRequestActionTypeDef,
     AdjustmentTypeDef,
     AdminAccountTypeDef,
     AssociatedStandardTypeDef,
     AssociationStateDetailsTypeDef,
     NoteUpdateTypeDef,
     RelatedFindingTypeDef,
     SeverityUpdateTypeDef,
     WorkflowUpdateTypeDef,
     MapFilterTypeDef,
     NumberFilterTypeDef,
     StringFilterTypeDef,
     AutomationRulesMetadataTypeDef,
     AvailabilityZoneTypeDef,
     AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef,
-    AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef,
+    AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef,
     AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef,
     AwsAmazonMqBrokerUsersDetailsTypeDef,
+    AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef,
     AwsAmazonMqBrokerLogsPendingDetailsTypeDef,
     AwsApiCallActionDomainDetailsTypeDef,
     AwsApiGatewayAccessLogSettingsTypeDef,
+    AwsApiGatewayCanarySettingsOutputTypeDef,
     AwsApiGatewayCanarySettingsTypeDef,
+    AwsApiGatewayEndpointConfigurationOutputTypeDef,
     AwsApiGatewayEndpointConfigurationTypeDef,
     AwsApiGatewayMethodSettingsTypeDef,
+    AwsCorsConfigurationOutputTypeDef,
     AwsCorsConfigurationTypeDef,
     AwsApiGatewayV2RouteSettingsTypeDef,
     AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef,
     AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef,
     AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef,
     AwsAppSyncGraphQlApiLogConfigDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationMetadataOptionsTypeDef,
+    AwsBackupBackupPlanAdvancedBackupSettingsDetailsOutputTypeDef,
     AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef,
     AwsBackupBackupPlanLifecycleDetailsTypeDef,
+    AwsBackupBackupVaultNotificationsDetailsOutputTypeDef,
     AwsBackupBackupVaultNotificationsDetailsTypeDef,
     AwsBackupRecoveryPointCalculatedLifecycleDetailsTypeDef,
     AwsBackupRecoveryPointCreatedByDetailsTypeDef,
     AwsBackupRecoveryPointLifecycleDetailsTypeDef,
     AwsCertificateManagerCertificateExtendedKeyUsageTypeDef,
     AwsCertificateManagerCertificateKeyUsageTypeDef,
     AwsCertificateManagerCertificateOptionsTypeDef,
     AwsCertificateManagerCertificateResourceRecordTypeDef,
     AwsCloudFormationStackDriftInformationDetailsTypeDef,
     AwsCloudFormationStackOutputsDetailsTypeDef,
     AwsCloudFrontDistributionCacheBehaviorTypeDef,
     AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef,
     AwsCloudFrontDistributionLoggingTypeDef,
     AwsCloudFrontDistributionViewerCertificateTypeDef,
+    AwsCloudFrontDistributionOriginSslProtocolsOutputTypeDef,
     AwsCloudFrontDistributionOriginSslProtocolsTypeDef,
+    AwsCloudFrontDistributionOriginGroupFailoverStatusCodesOutputTypeDef,
     AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef,
     AwsCloudFrontDistributionOriginS3OriginConfigTypeDef,
     AwsCloudTrailTrailDetailsTypeDef,
     AwsCloudWatchAlarmDimensionsDetailsTypeDef,
     AwsCodeBuildProjectArtifactsDetailsTypeDef,
     AwsCodeBuildProjectSourceTypeDef,
+    AwsCodeBuildProjectVpcConfigOutputTypeDef,
     AwsCodeBuildProjectVpcConfigTypeDef,
     AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef,
     AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef,
     AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef,
     AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef,
     AwsDynamoDbTableAttributeDefinitionTypeDef,
     AwsDynamoDbTableBillingModeSummaryTypeDef,
     AwsDynamoDbTableKeySchemaTypeDef,
     AwsDynamoDbTableProvisionedThroughputTypeDef,
     AwsDynamoDbTableRestoreSummaryTypeDef,
     AwsDynamoDbTableSseDescriptionTypeDef,
     AwsDynamoDbTableStreamSpecificationTypeDef,
+    AwsDynamoDbTableProjectionOutputTypeDef,
     AwsDynamoDbTableProjectionTypeDef,
     AwsDynamoDbTableProvisionedThroughputOverrideTypeDef,
     AwsEc2EipDetailsTypeDef,
     AwsEc2InstanceMetadataOptionsTypeDef,
     AwsEc2InstanceMonitoringDetailsTypeDef,
     AwsEc2InstanceNetworkInterfacesDetailsTypeDef,
     AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef,
@@ -545,86 +522,101 @@
     PropagatingVgwSetDetailsTypeDef,
     RouteSetDetailsTypeDef,
     AwsEc2SecurityGroupIpRangeTypeDef,
     AwsEc2SecurityGroupIpv6RangeTypeDef,
     AwsEc2SecurityGroupPrefixListIdTypeDef,
     AwsEc2SecurityGroupUserIdGroupPairTypeDef,
     Ipv6CidrBlockAssociationTypeDef,
+    AwsEc2TransitGatewayDetailsOutputTypeDef,
     AwsEc2TransitGatewayDetailsTypeDef,
     AwsEc2VolumeAttachmentTypeDef,
     CidrBlockAssociationTypeDef,
     AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef,
     AwsEc2VpcPeeringConnectionStatusDetailsTypeDef,
     VpcInfoCidrBlockSetDetailsTypeDef,
     VpcInfoIpv6CidrBlockSetDetailsTypeDef,
     VpcInfoPeeringOptionsDetailsTypeDef,
     AwsEc2VpnConnectionRoutesDetailsTypeDef,
     AwsEc2VpnConnectionVgwTelemetryDetailsTypeDef,
+    AwsEc2VpnConnectionOptionsTunnelOptionsDetailsOutputTypeDef,
     AwsEc2VpnConnectionOptionsTunnelOptionsDetailsTypeDef,
+    AwsEcrContainerImageDetailsOutputTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     AwsEcrRepositoryImageScanningConfigurationDetailsTypeDef,
     AwsEcrRepositoryLifecyclePolicyDetailsTypeDef,
     AwsEcsClusterClusterSettingsDetailsTypeDef,
     AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef,
     AwsEcsClusterDefaultCapacityProviderStrategyDetailsTypeDef,
     AwsMountPointTypeDef,
     AwsEcsServiceCapacityProviderStrategyDetailsTypeDef,
     AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef,
     AwsEcsServiceDeploymentControllerDetailsTypeDef,
     AwsEcsServiceLoadBalancersDetailsTypeDef,
     AwsEcsServicePlacementConstraintsDetailsTypeDef,
     AwsEcsServicePlacementStrategiesDetailsTypeDef,
     AwsEcsServiceServiceRegistriesDetailsTypeDef,
+    AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsOutputTypeDef,
     AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsOutputTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef,
     AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef,
     AwsEcsTaskDefinitionPlacementConstraintsDetailsTypeDef,
     AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef,
-    AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef,
+    AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsOutputTypeDef,
     AwsEcsTaskDefinitionVolumesHostDetailsTypeDef,
+    AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef,
     AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef,
     AwsEcsTaskVolumeHostDetailsTypeDef,
+    AwsEfsAccessPointPosixUserDetailsOutputTypeDef,
     AwsEfsAccessPointPosixUserDetailsTypeDef,
     AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef,
+    AwsEksClusterResourcesVpcConfigDetailsOutputTypeDef,
     AwsEksClusterResourcesVpcConfigDetailsTypeDef,
+    AwsEksClusterLoggingClusterLoggingDetailsOutputTypeDef,
     AwsEksClusterLoggingClusterLoggingDetailsTypeDef,
     AwsElasticBeanstalkEnvironmentEnvironmentLinkTypeDef,
     AwsElasticBeanstalkEnvironmentOptionSettingTypeDef,
     AwsElasticBeanstalkEnvironmentTierTypeDef,
     AwsElasticsearchDomainDomainEndpointOptionsTypeDef,
     AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef,
     AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef,
     AwsElasticsearchDomainServiceSoftwareOptionsTypeDef,
+    AwsElasticsearchDomainVPCOptionsOutputTypeDef,
     AwsElasticsearchDomainVPCOptionsTypeDef,
     AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef,
     AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef,
     AwsElbAppCookieStickinessPolicyTypeDef,
     AwsElbLbCookieStickinessPolicyTypeDef,
     AwsElbLoadBalancerAccessLogTypeDef,
     AwsElbLoadBalancerAdditionalAttributeTypeDef,
     AwsElbLoadBalancerConnectionDrainingTypeDef,
     AwsElbLoadBalancerConnectionSettingsTypeDef,
     AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef,
+    AwsElbLoadBalancerBackendServerDescriptionOutputTypeDef,
     AwsElbLoadBalancerBackendServerDescriptionTypeDef,
     AwsElbLoadBalancerHealthCheckTypeDef,
     AwsElbLoadBalancerInstanceTypeDef,
     AwsElbLoadBalancerSourceSecurityGroupTypeDef,
     AwsElbLoadBalancerListenerTypeDef,
     AwsElbv2LoadBalancerAttributeTypeDef,
     LoadBalancerStateTypeDef,
@@ -647,42 +639,48 @@
     AwsIamUserPolicyTypeDef,
     AwsKinesisStreamStreamEncryptionDetailsTypeDef,
     AwsKmsKeyDetailsTypeDef,
     AwsLambdaFunctionCodeTypeDef,
     AwsLambdaFunctionDeadLetterConfigTypeDef,
     AwsLambdaFunctionLayerTypeDef,
     AwsLambdaFunctionTracingConfigTypeDef,
+    AwsLambdaFunctionVpcConfigOutputTypeDef,
     AwsLambdaFunctionVpcConfigTypeDef,
     AwsLambdaFunctionEnvironmentErrorTypeDef,
+    AwsLambdaLayerVersionDetailsOutputTypeDef,
     AwsLambdaLayerVersionDetailsTypeDef,
     AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef,
     AwsOpenSearchServiceDomainMasterUserOptionsDetailsTypeDef,
     AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef,
     AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef,
     AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsTypeDef,
     AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsTypeDef,
     AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsTypeDef,
+    AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef,
     AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef,
     AwsOpenSearchServiceDomainLogPublishingOptionTypeDef,
     AwsRdsDbClusterAssociatedRoleTypeDef,
     AwsRdsDbClusterMemberTypeDef,
     AwsRdsDbClusterOptionGroupMembershipTypeDef,
     AwsRdsDbDomainMembershipTypeDef,
     AwsRdsDbInstanceVpcSecurityGroupTypeDef,
+    AwsRdsDbClusterSnapshotDetailsOutputTypeDef,
     AwsRdsDbClusterSnapshotDetailsTypeDef,
     AwsRdsDbInstanceAssociatedRoleTypeDef,
     AwsRdsDbInstanceEndpointTypeDef,
     AwsRdsDbOptionGroupMembershipTypeDef,
     AwsRdsDbParameterGroupTypeDef,
     AwsRdsDbProcessorFeatureTypeDef,
     AwsRdsDbStatusInfoTypeDef,
+    AwsRdsPendingCloudWatchLogsExportsOutputTypeDef,
     AwsRdsPendingCloudWatchLogsExportsTypeDef,
     AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef,
     AwsRdsDbSecurityGroupIpRangeTypeDef,
     AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef,
+    AwsRdsEventSubscriptionDetailsOutputTypeDef,
     AwsRdsEventSubscriptionDetailsTypeDef,
     AwsRedshiftClusterClusterNodeTypeDef,
     AwsRedshiftClusterClusterParameterStatusTypeDef,
     AwsRedshiftClusterClusterSecurityGroupTypeDef,
     AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef,
     AwsRedshiftClusterDeferredMaintenanceWindowTypeDef,
     AwsRedshiftClusterElasticIpStatusTypeDef,
@@ -739,14 +737,15 @@
     WafExcludedRuleTypeDef,
     WafOverrideActionTypeDef,
     AwsWafv2CustomHttpHeaderTypeDef,
     AwsWafv2VisibilityConfigDetailsTypeDef,
     AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef,
     AwsXrayEncryptionConfigDetailsTypeDef,
     BatchDeleteAutomationRulesRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UnprocessedAutomationRuleTypeDef,
     BatchDisableStandardsRequestRequestTypeDef,
     StandardsSubscriptionRequestTypeDef,
     BatchGetAutomationRulesRequestRequestTypeDef,
     BatchGetSecurityControlsRequestRequestTypeDef,
     SecurityControlTypeDef,
     UnprocessedSecurityControlTypeDef,
@@ -755,400 +754,575 @@
     ImportFindingsErrorTypeDef,
     StandardsControlAssociationUpdateTypeDef,
     CellTypeDef,
     ClassificationStatusTypeDef,
     StatusReasonTypeDef,
     VolumeMountTypeDef,
     CreateActionTargetRequestRequestTypeDef,
-    CreateActionTargetResponseTypeDef,
-    CreateAutomationRuleResponseTypeDef,
     CreateFindingAggregatorRequestRequestTypeDef,
-    CreateFindingAggregatorResponseTypeDef,
-    CreateInsightResponseTypeDef,
     ResultTypeDef,
     DateRangeTypeDef,
     DeclineInvitationsRequestRequestTypeDef,
     DeleteActionTargetRequestRequestTypeDef,
-    DeleteActionTargetResponseTypeDef,
     DeleteFindingAggregatorRequestRequestTypeDef,
     DeleteInsightRequestRequestTypeDef,
-    DeleteInsightResponseTypeDef,
     DeleteInvitationsRequestRequestTypeDef,
     DeleteMembersRequestRequestTypeDef,
-    DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeActionTargetsRequestRequestTypeDef,
     DescribeHubRequestRequestTypeDef,
-    DescribeHubResponseTypeDef,
-    DescribeOrganizationConfigurationResponseTypeDef,
-    DescribeProductsRequestDescribeProductsPaginateTypeDef,
     DescribeProductsRequestRequestTypeDef,
     ProductTypeDef,
-    DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
     DescribeStandardsControlsRequestRequestTypeDef,
     StandardsControlTypeDef,
-    DescribeStandardsRequestDescribeStandardsPaginateTypeDef,
     DescribeStandardsRequestRequestTypeDef,
     DisableImportFindingsForProductRequestRequestTypeDef,
     DisableOrganizationAdminAccountRequestRequestTypeDef,
     DisassociateMembersRequestRequestTypeDef,
     EnableImportFindingsForProductRequestRequestTypeDef,
-    EnableImportFindingsForProductResponseTypeDef,
     EnableOrganizationAdminAccountRequestRequestTypeDef,
     EnableSecurityHubRequestRequestTypeDef,
     FilePathsTypeDef,
     FindingAggregatorTypeDef,
     FindingHistoryUpdateSourceTypeDef,
     FindingHistoryUpdateTypeDef,
     FindingProviderSeverityTypeDef,
     FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef,
     FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef,
     InvitationTypeDef,
-    GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef,
     GetEnabledStandardsRequestRequestTypeDef,
     GetFindingAggregatorRequestRequestTypeDef,
-    GetFindingAggregatorResponseTypeDef,
+    TimestampTypeDef,
     SortCriterionTypeDef,
     GetInsightResultsRequestRequestTypeDef,
-    GetInsightsRequestGetInsightsPaginateTypeDef,
     GetInsightsRequestRequestTypeDef,
-    GetInvitationsCountResponseTypeDef,
     GetMembersRequestRequestTypeDef,
     MemberTypeDef,
     InsightResultValueTypeDef,
     InviteMembersRequestRequestTypeDef,
     ListAutomationRulesRequestRequestTypeDef,
-    ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef,
     ListEnabledProductsForImportRequestRequestTypeDef,
-    ListEnabledProductsForImportResponseTypeDef,
-    ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef,
     ListFindingAggregatorsRequestRequestTypeDef,
-    ListInvitationsRequestListInvitationsPaginateTypeDef,
     ListInvitationsRequestRequestTypeDef,
-    ListMembersRequestListMembersPaginateTypeDef,
     ListMembersRequestRequestTypeDef,
-    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
     ListOrganizationAdminAccountsRequestRequestTypeDef,
-    ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef,
     ListSecurityControlDefinitionsRequestRequestTypeDef,
     SecurityControlDefinitionTypeDef,
-    ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef,
     ListStandardsControlAssociationsRequestRequestTypeDef,
     StandardsControlAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PortRangeTypeDef,
     RangeTypeDef,
     RecordTypeDef,
-    PaginatorConfigTypeDef,
     RecommendationTypeDef,
-    ResponseMetadataTypeDef,
+    RuleGroupSourceListDetailsOutputTypeDef,
     RuleGroupSourceListDetailsTypeDef,
     RuleGroupSourceStatefulRulesHeaderDetailsTypeDef,
+    RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef,
     RuleGroupSourceStatefulRulesOptionsDetailsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef,
+    RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef,
+    RuleGroupVariablesIpSetsDetailsOutputTypeDef,
     RuleGroupVariablesIpSetsDetailsTypeDef,
+    RuleGroupVariablesPortSetsDetailsOutputTypeDef,
     RuleGroupVariablesPortSetsDetailsTypeDef,
     SoftwarePackageTypeDef,
     StandardsManagedByTypeDef,
     StandardsStatusReasonTypeDef,
     StatelessCustomPublishMetricActionDimensionTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateActionTargetRequestRequestTypeDef,
     UpdateFindingAggregatorRequestRequestTypeDef,
-    UpdateFindingAggregatorResponseTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
     UpdateSecurityHubConfigurationRequestRequestTypeDef,
     UpdateStandardsControlRequestRequestTypeDef,
     VulnerabilityVendorTypeDef,
     CreateMembersRequestRequestTypeDef,
     ActionRemoteIpDetailsTypeDef,
-    DescribeActionTargetsResponseTypeDef,
+    CvssOutputTypeDef,
     CvssTypeDef,
-    ListOrganizationAdminAccountsResponseTypeDef,
     AssociationSetDetailsTypeDef,
+    AutomationRulesFindingFieldsUpdateOutputTypeDef,
     AutomationRulesFindingFieldsUpdateTypeDef,
-    ListAutomationRulesResponseTypeDef,
     AwsAmazonMqBrokerLogsDetailsTypeDef,
+    AwsApiGatewayRestApiDetailsOutputTypeDef,
     AwsApiGatewayRestApiDetailsTypeDef,
+    AwsApiGatewayStageDetailsOutputTypeDef,
     AwsApiGatewayStageDetailsTypeDef,
+    AwsApiGatewayV2ApiDetailsOutputTypeDef,
     AwsApiGatewayV2ApiDetailsTypeDef,
+    AwsApiGatewayV2StageDetailsOutputTypeDef,
     AwsApiGatewayV2StageDetailsTypeDef,
     AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef,
+    AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef,
     AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef,
+    AwsBackupBackupVaultDetailsOutputTypeDef,
     AwsBackupBackupVaultDetailsTypeDef,
     AwsBackupRecoveryPointDetailsTypeDef,
+    AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef,
     AwsCertificateManagerCertificateDomainValidationOptionTypeDef,
+    AwsCloudFormationStackDetailsOutputTypeDef,
     AwsCloudFormationStackDetailsTypeDef,
+    AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef,
     AwsCloudFrontDistributionCacheBehaviorsTypeDef,
+    AwsCloudFrontDistributionOriginCustomOriginConfigOutputTypeDef,
     AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef,
+    AwsCloudFrontDistributionOriginGroupFailoverOutputTypeDef,
     AwsCloudFrontDistributionOriginGroupFailoverTypeDef,
+    AwsCloudWatchAlarmDetailsOutputTypeDef,
     AwsCloudWatchAlarmDetailsTypeDef,
+    AwsCodeBuildProjectEnvironmentOutputTypeDef,
     AwsCodeBuildProjectEnvironmentTypeDef,
     AwsCodeBuildProjectLogsConfigDetailsTypeDef,
+    AwsDynamoDbTableGlobalSecondaryIndexOutputTypeDef,
+    AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef,
     AwsDynamoDbTableGlobalSecondaryIndexTypeDef,
     AwsDynamoDbTableLocalSecondaryIndexTypeDef,
     AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef,
+    AwsEc2InstanceDetailsOutputTypeDef,
     AwsEc2InstanceDetailsTypeDef,
     AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef,
     AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef,
     AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataInstanceRequirementsDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef,
+    AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef,
     AwsEc2NetworkAclEntryTypeDef,
+    AwsEc2NetworkInterfaceDetailsOutputTypeDef,
     AwsEc2NetworkInterfaceDetailsTypeDef,
+    AwsEc2SecurityGroupIpPermissionOutputTypeDef,
     AwsEc2SecurityGroupIpPermissionTypeDef,
+    AwsEc2SubnetDetailsOutputTypeDef,
     AwsEc2SubnetDetailsTypeDef,
+    AwsEc2VolumeDetailsOutputTypeDef,
     AwsEc2VolumeDetailsTypeDef,
+    AwsEc2VpcDetailsOutputTypeDef,
     AwsEc2VpcDetailsTypeDef,
+    AwsEc2VpcEndpointServiceDetailsOutputTypeDef,
     AwsEc2VpcEndpointServiceDetailsTypeDef,
+    AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef,
     AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef,
+    AwsEc2VpnConnectionOptionsDetailsOutputTypeDef,
     AwsEc2VpnConnectionOptionsDetailsTypeDef,
     AwsEcrRepositoryDetailsTypeDef,
     AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef,
+    AwsEcsContainerDetailsOutputTypeDef,
     AwsEcsContainerDetailsTypeDef,
     AwsEcsServiceDeploymentConfigurationDetailsTypeDef,
+    AwsEcsServiceNetworkConfigurationDetailsOutputTypeDef,
     AwsEcsServiceNetworkConfigurationDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef,
+    AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef,
     AwsEcsTaskDefinitionProxyConfigurationDetailsTypeDef,
     AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef,
     AwsEcsTaskVolumeDetailsTypeDef,
     AwsEfsAccessPointRootDirectoryDetailsTypeDef,
+    AwsEksClusterLoggingDetailsOutputTypeDef,
     AwsEksClusterLoggingDetailsTypeDef,
+    AwsElasticBeanstalkEnvironmentDetailsOutputTypeDef,
     AwsElasticBeanstalkEnvironmentDetailsTypeDef,
     AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef,
     AwsElasticsearchDomainLogPublishingOptionsTypeDef,
+    AwsElbLoadBalancerPoliciesOutputTypeDef,
     AwsElbLoadBalancerPoliciesTypeDef,
+    AwsElbLoadBalancerAttributesOutputTypeDef,
     AwsElbLoadBalancerAttributesTypeDef,
+    AwsElbLoadBalancerListenerDescriptionOutputTypeDef,
     AwsElbLoadBalancerListenerDescriptionTypeDef,
+    AwsElbv2LoadBalancerDetailsOutputTypeDef,
     AwsElbv2LoadBalancerDetailsTypeDef,
     AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef,
     AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef,
     AwsIamAccessKeySessionContextTypeDef,
+    AwsIamGroupDetailsOutputTypeDef,
     AwsIamGroupDetailsTypeDef,
+    AwsIamInstanceProfileOutputTypeDef,
     AwsIamInstanceProfileTypeDef,
+    AwsIamPolicyDetailsOutputTypeDef,
     AwsIamPolicyDetailsTypeDef,
+    AwsIamUserDetailsOutputTypeDef,
     AwsIamUserDetailsTypeDef,
     AwsKinesisStreamDetailsTypeDef,
+    AwsLambdaFunctionEnvironmentOutputTypeDef,
     AwsLambdaFunctionEnvironmentTypeDef,
+    AwsNetworkFirewallFirewallDetailsOutputTypeDef,
     AwsNetworkFirewallFirewallDetailsTypeDef,
     AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef,
     AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef,
     AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef,
+    AwsRdsDbClusterDetailsOutputTypeDef,
     AwsRdsDbClusterDetailsTypeDef,
+    AwsRdsDbSnapshotDetailsOutputTypeDef,
     AwsRdsDbSnapshotDetailsTypeDef,
+    AwsRdsDbPendingModifiedValuesOutputTypeDef,
     AwsRdsDbPendingModifiedValuesTypeDef,
+    AwsRdsDbSecurityGroupDetailsOutputTypeDef,
     AwsRdsDbSecurityGroupDetailsTypeDef,
     AwsRdsDbSubnetGroupSubnetTypeDef,
+    AwsRedshiftClusterClusterParameterGroupOutputTypeDef,
     AwsRedshiftClusterClusterParameterGroupTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef,
+    AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef,
     AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef,
     AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef,
     AwsS3BucketServerSideEncryptionRuleTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef,
+    AwsSageMakerNotebookInstanceDetailsOutputTypeDef,
     AwsSageMakerNotebookInstanceDetailsTypeDef,
     AwsSecretsManagerSecretDetailsTypeDef,
     BatchUpdateFindingsRequestRequestTypeDef,
     BatchUpdateFindingsUnprocessedFindingTypeDef,
-    GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
-    GetFindingHistoryRequestRequestTypeDef,
+    AwsSnsTopicDetailsOutputTypeDef,
     AwsSnsTopicDetailsTypeDef,
     AwsSsmPatchTypeDef,
     AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef,
+    AwsWafRateBasedRuleDetailsOutputTypeDef,
     AwsWafRateBasedRuleDetailsTypeDef,
+    AwsWafRegionalRateBasedRuleDetailsOutputTypeDef,
     AwsWafRegionalRateBasedRuleDetailsTypeDef,
+    AwsWafRegionalRuleDetailsOutputTypeDef,
     AwsWafRegionalRuleDetailsTypeDef,
     AwsWafRegionalRuleGroupRulesDetailsTypeDef,
     AwsWafRegionalWebAclRulesListDetailsTypeDef,
+    AwsWafRuleDetailsOutputTypeDef,
     AwsWafRuleDetailsTypeDef,
     AwsWafRuleGroupRulesDetailsTypeDef,
+    AwsWafWebAclRuleOutputTypeDef,
     AwsWafWebAclRuleTypeDef,
+    AwsWafv2CustomRequestHandlingDetailsOutputTypeDef,
     AwsWafv2CustomRequestHandlingDetailsTypeDef,
+    AwsWafv2CustomResponseDetailsOutputTypeDef,
     AwsWafv2CustomResponseDetailsTypeDef,
     AwsWafv2WebAclCaptchaConfigDetailsTypeDef,
+    CreateActionTargetResponseTypeDef,
+    CreateAutomationRuleResponseTypeDef,
+    CreateFindingAggregatorResponseTypeDef,
+    CreateInsightResponseTypeDef,
+    DeleteActionTargetResponseTypeDef,
+    DeleteInsightResponseTypeDef,
+    DescribeActionTargetsResponseTypeDef,
+    DescribeHubResponseTypeDef,
+    DescribeOrganizationConfigurationResponseTypeDef,
+    EnableImportFindingsForProductResponseTypeDef,
+    GetFindingAggregatorResponseTypeDef,
+    GetInvitationsCountResponseTypeDef,
+    ListAutomationRulesResponseTypeDef,
+    ListEnabledProductsForImportResponseTypeDef,
+    ListOrganizationAdminAccountsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateFindingAggregatorResponseTypeDef,
     BatchDeleteAutomationRulesResponseTypeDef,
     BatchUpdateAutomationRulesResponseTypeDef,
     BatchEnableStandardsRequestRequestTypeDef,
     BatchGetSecurityControlsResponseTypeDef,
     BatchGetStandardsControlAssociationsRequestRequestTypeDef,
     UnprocessedStandardsControlAssociationTypeDef,
     BatchImportFindingsResponseTypeDef,
     BatchUpdateStandardsControlAssociationsRequestRequestTypeDef,
     UnprocessedStandardsControlAssociationUpdateTypeDef,
+    ComplianceOutputTypeDef,
     ComplianceTypeDef,
+    ContainerDetailsOutputTypeDef,
     ContainerDetailsTypeDef,
     CreateMembersResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     DeleteMembersResponseTypeDef,
     InviteMembersResponseTypeDef,
     DateFilterTypeDef,
+    DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef,
+    DescribeProductsRequestDescribeProductsPaginateTypeDef,
+    DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
+    DescribeStandardsRequestDescribeStandardsPaginateTypeDef,
+    GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef,
+    GetInsightsRequestGetInsightsPaginateTypeDef,
+    ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef,
+    ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef,
+    ListInvitationsRequestListInvitationsPaginateTypeDef,
+    ListMembersRequestListMembersPaginateTypeDef,
+    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
+    ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef,
+    ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef,
     DescribeProductsResponseTypeDef,
     DescribeStandardsControlsResponseTypeDef,
+    ThreatOutputTypeDef,
     ThreatTypeDef,
     ListFindingAggregatorsResponseTypeDef,
     FindingHistoryRecordTypeDef,
+    FindingProviderFieldsOutputTypeDef,
     FindingProviderFieldsTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetMasterAccountResponseTypeDef,
     ListInvitationsResponseTypeDef,
+    GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
+    GetFindingHistoryRequestRequestTypeDef,
     GetMembersResponseTypeDef,
     ListMembersResponseTypeDef,
     InsightResultsTypeDef,
     ListSecurityControlDefinitionsResponseTypeDef,
     ListStandardsControlAssociationsResponseTypeDef,
+    NetworkPathComponentDetailsOutputTypeDef,
     NetworkPathComponentDetailsTypeDef,
     NetworkTypeDef,
     PageTypeDef,
     RemediationTypeDef,
+    RuleGroupSourceStatefulRulesDetailsOutputTypeDef,
     RuleGroupSourceStatefulRulesDetailsTypeDef,
+    RuleGroupSourceStatelessRuleMatchAttributesOutputTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesTypeDef,
+    RuleGroupVariablesOutputTypeDef,
     RuleGroupVariablesTypeDef,
     StandardTypeDef,
     StandardsSubscriptionTypeDef,
+    StatelessCustomPublishMetricActionOutputTypeDef,
     StatelessCustomPublishMetricActionTypeDef,
+    AwsApiCallActionOutputTypeDef,
     AwsApiCallActionTypeDef,
     NetworkConnectionActionTypeDef,
     PortProbeDetailTypeDef,
+    VulnerabilityOutputTypeDef,
     VulnerabilityTypeDef,
+    AwsEc2RouteTableDetailsOutputTypeDef,
     AwsEc2RouteTableDetailsTypeDef,
+    AutomationRulesActionOutputTypeDef,
     AutomationRulesActionTypeDef,
+    AwsAmazonMqBrokerDetailsOutputTypeDef,
     AwsAmazonMqBrokerDetailsTypeDef,
+    AwsAppSyncGraphQlApiDetailsOutputTypeDef,
     AwsAppSyncGraphQlApiDetailsTypeDef,
+    AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef,
+    AwsAutoScalingLaunchConfigurationDetailsOutputTypeDef,
     AwsAutoScalingLaunchConfigurationDetailsTypeDef,
+    AwsBackupBackupPlanRuleDetailsOutputTypeDef,
     AwsBackupBackupPlanRuleDetailsTypeDef,
+    AwsCertificateManagerCertificateRenewalSummaryOutputTypeDef,
     AwsCertificateManagerCertificateRenewalSummaryTypeDef,
+    AwsCloudFrontDistributionOriginItemOutputTypeDef,
     AwsCloudFrontDistributionOriginItemTypeDef,
+    AwsCloudFrontDistributionOriginGroupOutputTypeDef,
     AwsCloudFrontDistributionOriginGroupTypeDef,
+    AwsCodeBuildProjectDetailsOutputTypeDef,
     AwsCodeBuildProjectDetailsTypeDef,
+    AwsDynamoDbTableReplicaOutputTypeDef,
     AwsDynamoDbTableReplicaTypeDef,
+    AwsEc2LaunchTemplateDataDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataDetailsTypeDef,
+    AwsEc2NetworkAclDetailsOutputTypeDef,
     AwsEc2NetworkAclDetailsTypeDef,
+    AwsEc2SecurityGroupDetailsOutputTypeDef,
     AwsEc2SecurityGroupDetailsTypeDef,
+    AwsEc2VpcPeeringConnectionDetailsOutputTypeDef,
     AwsEc2VpcPeeringConnectionDetailsTypeDef,
+    AwsEc2VpnConnectionDetailsOutputTypeDef,
     AwsEc2VpnConnectionDetailsTypeDef,
     AwsEcsClusterConfigurationDetailsTypeDef,
+    AwsEcsServiceDetailsOutputTypeDef,
     AwsEcsServiceDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef,
+    AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef,
     AwsEcsTaskDefinitionVolumesDetailsTypeDef,
+    AwsEcsTaskDetailsOutputTypeDef,
     AwsEcsTaskDetailsTypeDef,
+    AwsEfsAccessPointDetailsOutputTypeDef,
     AwsEfsAccessPointDetailsTypeDef,
+    AwsEksClusterDetailsOutputTypeDef,
     AwsEksClusterDetailsTypeDef,
+    AwsElasticsearchDomainDetailsOutputTypeDef,
     AwsElasticsearchDomainDetailsTypeDef,
+    AwsElbLoadBalancerDetailsOutputTypeDef,
     AwsElbLoadBalancerDetailsTypeDef,
     AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef,
     AwsIamAccessKeyDetailsTypeDef,
+    AwsIamRoleDetailsOutputTypeDef,
     AwsIamRoleDetailsTypeDef,
+    AwsLambdaFunctionDetailsOutputTypeDef,
     AwsLambdaFunctionDetailsTypeDef,
+    AwsOpenSearchServiceDomainDetailsOutputTypeDef,
     AwsOpenSearchServiceDomainDetailsTypeDef,
+    AwsRdsDbSubnetGroupOutputTypeDef,
     AwsRdsDbSubnetGroupTypeDef,
+    AwsRedshiftClusterDetailsOutputTypeDef,
     AwsRedshiftClusterDetailsTypeDef,
+    AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef,
+    AwsS3BucketNotificationConfigurationFilterOutputTypeDef,
     AwsS3BucketNotificationConfigurationFilterTypeDef,
     AwsS3BucketObjectLockConfigurationTypeDef,
+    AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef,
     AwsS3BucketServerSideEncryptionConfigurationTypeDef,
+    AwsS3BucketWebsiteConfigurationOutputTypeDef,
     AwsS3BucketWebsiteConfigurationTypeDef,
     BatchUpdateFindingsResponseTypeDef,
     AwsSsmPatchComplianceDetailsTypeDef,
+    AwsStepFunctionStateMachineLoggingConfigurationDetailsOutputTypeDef,
     AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef,
+    AwsWafRegionalRuleGroupDetailsOutputTypeDef,
     AwsWafRegionalRuleGroupDetailsTypeDef,
+    AwsWafRegionalWebAclDetailsOutputTypeDef,
     AwsWafRegionalWebAclDetailsTypeDef,
+    AwsWafRuleGroupDetailsOutputTypeDef,
     AwsWafRuleGroupDetailsTypeDef,
+    AwsWafWebAclDetailsOutputTypeDef,
     AwsWafWebAclDetailsTypeDef,
+    AwsWafv2ActionAllowDetailsOutputTypeDef,
+    AwsWafv2RulesActionCaptchaDetailsOutputTypeDef,
+    AwsWafv2RulesActionCountDetailsOutputTypeDef,
     AwsWafv2ActionAllowDetailsTypeDef,
     AwsWafv2RulesActionCaptchaDetailsTypeDef,
     AwsWafv2RulesActionCountDetailsTypeDef,
+    AwsWafv2ActionBlockDetailsOutputTypeDef,
     AwsWafv2ActionBlockDetailsTypeDef,
     BatchGetStandardsControlAssociationsResponseTypeDef,
     BatchUpdateStandardsControlAssociationsResponseTypeDef,
+    AutomationRulesFindingFiltersOutputTypeDef,
     AutomationRulesFindingFiltersTypeDef,
+    AwsSecurityFindingFiltersOutputTypeDef,
     AwsSecurityFindingFiltersTypeDef,
     GetFindingHistoryResponseTypeDef,
     GetInsightResultsResponseTypeDef,
+    NetworkHeaderOutputTypeDef,
     NetworkHeaderTypeDef,
+    OccurrencesOutputTypeDef,
     OccurrencesTypeDef,
+    RuleGroupSourceStatelessRuleDefinitionOutputTypeDef,
     RuleGroupSourceStatelessRuleDefinitionTypeDef,
     DescribeStandardsResponseTypeDef,
     BatchDisableStandardsResponseTypeDef,
     BatchEnableStandardsResponseTypeDef,
     GetEnabledStandardsResponseTypeDef,
+    StatelessCustomActionDefinitionOutputTypeDef,
     StatelessCustomActionDefinitionTypeDef,
+    PortProbeActionOutputTypeDef,
     PortProbeActionTypeDef,
+    AutomationRulesActionUnionTypeDef,
+    AwsAutoScalingAutoScalingGroupDetailsOutputTypeDef,
     AwsAutoScalingAutoScalingGroupDetailsTypeDef,
+    AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef,
     AwsBackupBackupPlanBackupPlanDetailsTypeDef,
+    AwsCertificateManagerCertificateDetailsOutputTypeDef,
     AwsCertificateManagerCertificateDetailsTypeDef,
+    AwsCloudFrontDistributionOriginsOutputTypeDef,
     AwsCloudFrontDistributionOriginsTypeDef,
+    AwsCloudFrontDistributionOriginGroupsOutputTypeDef,
     AwsCloudFrontDistributionOriginGroupsTypeDef,
+    AwsDynamoDbTableDetailsOutputTypeDef,
     AwsDynamoDbTableDetailsTypeDef,
+    AwsEc2LaunchTemplateDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDetailsTypeDef,
+    AwsEcsClusterDetailsOutputTypeDef,
     AwsEcsClusterDetailsTypeDef,
+    AwsEcsTaskDefinitionDetailsOutputTypeDef,
     AwsEcsTaskDefinitionDetailsTypeDef,
     AwsGuardDutyDetectorDataSourcesDetailsTypeDef,
+    AwsRdsDbInstanceDetailsOutputTypeDef,
     AwsRdsDbInstanceDetailsTypeDef,
+    AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef,
+    AwsS3BucketNotificationConfigurationDetailOutputTypeDef,
     AwsS3BucketNotificationConfigurationDetailTypeDef,
+    AwsStepFunctionStateMachineDetailsOutputTypeDef,
     AwsStepFunctionStateMachineDetailsTypeDef,
+    AwsWafv2RulesActionDetailsOutputTypeDef,
+    AwsWafv2WebAclActionDetailsOutputTypeDef,
     AwsWafv2RulesActionDetailsTypeDef,
     AwsWafv2WebAclActionDetailsTypeDef,
     AutomationRulesConfigTypeDef,
-    CreateAutomationRuleRequestRequestTypeDef,
+    AutomationRulesFindingFiltersUnionTypeDef,
     UpdateAutomationRulesRequestItemTypeDef,
+    InsightTypeDef,
+    AwsSecurityFindingFiltersUnionTypeDef,
     CreateInsightRequestRequestTypeDef,
     GetFindingsRequestGetFindingsPaginateTypeDef,
     GetFindingsRequestRequestTypeDef,
-    InsightTypeDef,
     UpdateFindingsRequestRequestTypeDef,
     UpdateInsightRequestRequestTypeDef,
+    NetworkPathComponentOutputTypeDef,
     NetworkPathComponentTypeDef,
+    CustomDataIdentifiersDetectionsOutputTypeDef,
+    SensitiveDataDetectionsOutputTypeDef,
     CustomDataIdentifiersDetectionsTypeDef,
     SensitiveDataDetectionsTypeDef,
+    RuleGroupSourceStatelessRulesDetailsOutputTypeDef,
     RuleGroupSourceStatelessRulesDetailsTypeDef,
+    FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef,
+    RuleGroupSourceCustomActionsDetailsOutputTypeDef,
     FirewallPolicyStatelessCustomActionsDetailsTypeDef,
     RuleGroupSourceCustomActionsDetailsTypeDef,
+    ActionOutputTypeDef,
     ActionTypeDef,
+    CreateAutomationRuleRequestRequestTypeDef,
+    AwsBackupBackupPlanDetailsOutputTypeDef,
     AwsBackupBackupPlanDetailsTypeDef,
+    AwsCloudFrontDistributionDetailsOutputTypeDef,
     AwsCloudFrontDistributionDetailsTypeDef,
+    AwsGuardDutyDetectorDetailsOutputTypeDef,
     AwsGuardDutyDetectorDetailsTypeDef,
+    AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef,
+    AwsS3BucketNotificationConfigurationOutputTypeDef,
     AwsS3BucketNotificationConfigurationTypeDef,
+    AwsWafv2RulesDetailsOutputTypeDef,
     AwsWafv2RulesDetailsTypeDef,
     BatchGetAutomationRulesResponseTypeDef,
     BatchUpdateAutomationRulesRequestRequestTypeDef,
     GetInsightsResponseTypeDef,
+    CustomDataIdentifiersResultOutputTypeDef,
+    SensitiveDataResultOutputTypeDef,
     CustomDataIdentifiersResultTypeDef,
     SensitiveDataResultTypeDef,
+    FirewallPolicyDetailsOutputTypeDef,
+    RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef,
     FirewallPolicyDetailsTypeDef,
     RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef,
+    AwsS3BucketBucketLifecycleConfigurationDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef,
+    AwsWafv2RuleGroupDetailsOutputTypeDef,
+    AwsWafv2WebAclDetailsOutputTypeDef,
     AwsWafv2RuleGroupDetailsTypeDef,
     AwsWafv2WebAclDetailsTypeDef,
+    ClassificationResultOutputTypeDef,
     ClassificationResultTypeDef,
+    AwsNetworkFirewallFirewallPolicyDetailsOutputTypeDef,
+    RuleGroupSourceOutputTypeDef,
     AwsNetworkFirewallFirewallPolicyDetailsTypeDef,
     RuleGroupSourceTypeDef,
+    AwsS3BucketDetailsOutputTypeDef,
     AwsS3BucketDetailsTypeDef,
+    DataClassificationDetailsOutputTypeDef,
     DataClassificationDetailsTypeDef,
+    RuleGroupDetailsOutputTypeDef,
     RuleGroupDetailsTypeDef,
+    AwsNetworkFirewallRuleGroupDetailsOutputTypeDef,
     AwsNetworkFirewallRuleGroupDetailsTypeDef,
+    ResourceDetailsOutputTypeDef,
     ResourceDetailsTypeDef,
+    ResourceOutputTypeDef,
     ResourceTypeDef,
+    AwsSecurityFindingOutputTypeDef,
     AwsSecurityFindingTypeDef,
-    BatchImportFindingsRequestRequestTypeDef,
     GetFindingsResponseTypeDef,
+    AwsSecurityFindingUnionTypeDef,
+    BatchImportFindingsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AcceptAdministratorInvitationRequestRequestTypeDef:
+def get_value() -> AcceptAdministratorInvitationRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-securityhub-2.5.2/types_aiobotocore_securityhub.egg-info/SOURCES.txt` & `types-aiobotocore-securityhub-2.5.2.post1/types_aiobotocore_securityhub.egg-info/SOURCES.txt`

 * *Files identical despite different names*


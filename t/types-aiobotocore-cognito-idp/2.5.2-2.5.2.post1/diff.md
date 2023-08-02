# Comparing `tmp/types-aiobotocore-cognito-idp-2.5.2.tar.gz` & `tmp/types-aiobotocore-cognito-idp-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cognito-idp-2.5.2.tar", last modified: Sat Jul  8 01:43:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-cognito-idp-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:05 2023, max compression
```

## Comparing `types-aiobotocore-cognito-idp-2.5.2.tar` & `types-aiobotocore-cognito-idp-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:26.137913 types-aiobotocore-cognito-idp-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:45.000000 types-aiobotocore-cognito-idp-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25561 2023-07-08 01:43:26.133913 types-aiobotocore-cognito-idp-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23968 2023-07-08 01:27:45.000000 types-aiobotocore-cognito-idp-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:26.137913 types-aiobotocore-cognito-idp-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-08 01:27:45.000000 types-aiobotocore-cognito-idp-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:26.129913 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-08 01:27:45.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-08 01:27:45.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-08 01:27:45.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    82577 2023-07-08 01:27:47.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    82458 2023-07-08 01:27:46.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-07-08 01:27:47.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-07-08 01:27:47.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-07-08 01:27:47.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-07-08 01:27:47.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:45.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    97467 2023-07-08 01:27:50.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    97328 2023-07-08 01:27:48.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:45.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:26.133913 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25561 2023-07-08 01:43:25.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-08 01:43:25.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:25.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:25.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:25.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-08 01:43:25.000000 types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.993618 types-aiobotocore-cognito-idp-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:20.000000 types-aiobotocore-cognito-idp-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25922 2023-08-02 14:52:04.993618 types-aiobotocore-cognito-idp-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24376 2023-08-02 14:35:20.000000 types-aiobotocore-cognito-idp-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:04.993618 types-aiobotocore-cognito-idp-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-08-02 14:35:20.000000 types-aiobotocore-cognito-idp-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.993618 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-08-02 14:35:20.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-08-02 14:35:20.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-02 14:35:20.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82516 2023-08-02 14:35:20.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82397 2023-08-02 14:35:20.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-08-02 14:35:21.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-08-02 14:35:21.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11573 2023-08-02 14:35:21.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-08-02 14:35:20.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:20.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    99761 2023-08-02 14:35:24.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99620 2023-08-02 14:35:23.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:20.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.993618 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25922 2023-08-02 14:52:04.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-02 14:52:04.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:04.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 14:52:04.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cognito-idp-2.5.2/LICENSE` & `types-aiobotocore-cognito-idp-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-idp-2.5.2/PKG-INFO` & `types-aiobotocore-cognito-idp-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cognito-idp
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CognitoIdentityProvider 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CognitoIdentityProvider 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore cognito-idp type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore cognito-idp type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cognito-idp"></a>
 
 # types-aiobotocore-cognito-idp
 
 [![PyPI - types-aiobotocore-cognito-idp](https://img.shields.io/pypi/v/types-aiobotocore-cognito-idp.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-idp)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cognito-idp.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-idp)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cognito-idp?color=blue)](https://pypistats.org/packages/types-aiobotocore-cognito-idp)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cognito-idp)](https://pepy.tech/project/types-aiobotocore-cognito-idp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CognitoIdentityProvider 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
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
 [types-aiobotocore-cognito-idp docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/).
 
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
@@ -380,77 +379,75 @@
 )
 
 
 def check_value(value: AccountTakeoverEventActionTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cognito_idp.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cognito_idp.type_defs import (
     RecoveryOptionTypeTypeDef,
     AccountTakeoverActionTypeTypeDef,
     AdminAddUserToGroupRequestRequestTypeDef,
     AdminConfirmSignUpRequestRequestTypeDef,
     MessageTemplateTypeTypeDef,
     AttributeTypeTypeDef,
+    ResponseMetadataTypeDef,
     AdminDeleteUserAttributesRequestRequestTypeDef,
     AdminDeleteUserRequestRequestTypeDef,
     ProviderUserIdentifierTypeTypeDef,
     AdminDisableUserRequestRequestTypeDef,
     AdminEnableUserRequestRequestTypeDef,
     AdminForgetDeviceRequestRequestTypeDef,
     AdminGetDeviceRequestRequestTypeDef,
     AdminGetUserRequestRequestTypeDef,
     MFAOptionTypeTypeDef,
     AnalyticsMetadataTypeTypeDef,
     AdminListDevicesRequestRequestTypeDef,
-    AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
+    PaginatorConfigTypeDef,
     AdminListGroupsForUserRequestRequestTypeDef,
     GroupTypeTypeDef,
-    AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
     AdminListUserAuthEventsRequestRequestTypeDef,
     AdminRemoveUserFromGroupRequestRequestTypeDef,
     AdminResetUserPasswordRequestRequestTypeDef,
     SMSMfaSettingsTypeTypeDef,
     SoftwareTokenMfaSettingsTypeTypeDef,
     AdminSetUserPasswordRequestRequestTypeDef,
     AdminUpdateAuthEventFeedbackRequestRequestTypeDef,
     AdminUpdateDeviceStatusRequestRequestTypeDef,
     AdminUserGlobalSignOutRequestRequestTypeDef,
     AnalyticsConfigurationTypeTypeDef,
     AssociateSoftwareTokenRequestRequestTypeDef,
-    AssociateSoftwareTokenResponseTypeDef,
     ChallengeResponseTypeTypeDef,
     EventContextDataTypeTypeDef,
     EventFeedbackTypeTypeDef,
     EventRiskTypeTypeDef,
     NewDeviceMetadataTypeTypeDef,
+    BlobTypeDef,
     ChangePasswordRequestRequestTypeDef,
     CodeDeliveryDetailsTypeTypeDef,
     CompromisedCredentialsActionsTypeTypeDef,
     DeviceSecretVerifierConfigTypeTypeDef,
-    ConfirmDeviceResponseTypeDef,
     UserContextDataTypeTypeDef,
     HttpHeaderTypeDef,
     CreateGroupRequestRequestTypeDef,
     CreateIdentityProviderRequestRequestTypeDef,
     IdentityProviderTypeTypeDef,
     ResourceServerScopeTypeTypeDef,
     CreateUserImportJobRequestRequestTypeDef,
     UserImportJobTypeTypeDef,
     TokenValidityUnitsTypeTypeDef,
     CustomDomainConfigTypeTypeDef,
-    CreateUserPoolDomainResponseTypeDef,
     DeviceConfigurationTypeTypeDef,
     EmailConfigurationTypeTypeDef,
     SmsConfigurationTypeTypeDef,
     UserAttributeUpdateSettingsTypeTypeDef,
     UserPoolAddOnsTypeTypeDef,
     UsernameConfigurationTypeTypeDef,
     VerificationMessageTemplateTypeTypeDef,
@@ -467,99 +464,106 @@
     DescribeIdentityProviderRequestRequestTypeDef,
     DescribeResourceServerRequestRequestTypeDef,
     DescribeRiskConfigurationRequestRequestTypeDef,
     DescribeUserImportJobRequestRequestTypeDef,
     DescribeUserPoolClientRequestRequestTypeDef,
     DescribeUserPoolDomainRequestRequestTypeDef,
     DescribeUserPoolRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ForgetDeviceRequestRequestTypeDef,
     GetCSVHeaderRequestRequestTypeDef,
-    GetCSVHeaderResponseTypeDef,
     GetDeviceRequestRequestTypeDef,
     GetGroupRequestRequestTypeDef,
     GetIdentityProviderByIdentifierRequestRequestTypeDef,
     GetSigningCertificateRequestRequestTypeDef,
-    GetSigningCertificateResponseTypeDef,
     GetUICustomizationRequestRequestTypeDef,
     UICustomizationTypeTypeDef,
     GetUserAttributeVerificationCodeRequestRequestTypeDef,
     GetUserPoolMfaConfigRequestRequestTypeDef,
     SoftwareTokenMfaConfigTypeTypeDef,
     GetUserRequestRequestTypeDef,
     GlobalSignOutRequestRequestTypeDef,
     ListDevicesRequestRequestTypeDef,
-    ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
-    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
     ListIdentityProvidersRequestRequestTypeDef,
     ProviderDescriptionTypeDef,
-    ListResourceServersRequestListResourceServersPaginateTypeDef,
     ListResourceServersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListUserImportJobsRequestRequestTypeDef,
-    ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
     ListUserPoolClientsRequestRequestTypeDef,
     UserPoolClientDescriptionTypeDef,
-    ListUserPoolsRequestListUserPoolsPaginateTypeDef,
     ListUserPoolsRequestRequestTypeDef,
-    ListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
     ListUsersInGroupRequestRequestTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     NotifyEmailTypeTypeDef,
     NumberAttributeConstraintsTypeTypeDef,
-    PaginatorConfigTypeDef,
     PasswordPolicyTypeTypeDef,
-    ResponseMetadataTypeDef,
     RevokeTokenRequestRequestTypeDef,
+    RiskExceptionConfigurationTypeOutputTypeDef,
     RiskExceptionConfigurationTypeTypeDef,
     StringAttributeConstraintsTypeTypeDef,
-    SetUICustomizationRequestRequestTypeDef,
     StartUserImportJobRequestRequestTypeDef,
     StopUserImportJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAuthEventFeedbackRequestRequestTypeDef,
     UpdateDeviceStatusRequestRequestTypeDef,
     UpdateGroupRequestRequestTypeDef,
     UpdateIdentityProviderRequestRequestTypeDef,
-    UpdateUserPoolDomainResponseTypeDef,
+    UserAttributeUpdateSettingsTypeOutputTypeDef,
     VerifySoftwareTokenRequestRequestTypeDef,
-    VerifySoftwareTokenResponseTypeDef,
     VerifyUserAttributeRequestRequestTypeDef,
+    AccountRecoverySettingTypeOutputTypeDef,
     AccountRecoverySettingTypeTypeDef,
     AccountTakeoverActionsTypeTypeDef,
     AdminCreateUserConfigTypeTypeDef,
     AdminCreateUserRequestRequestTypeDef,
     AdminUpdateUserAttributesRequestRequestTypeDef,
     DeviceTypeTypeDef,
     UpdateUserAttributesRequestRequestTypeDef,
+    AssociateSoftwareTokenResponseTypeDef,
+    ConfirmDeviceResponseTypeDef,
+    CreateUserPoolDomainResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCSVHeaderResponseTypeDef,
+    GetSigningCertificateResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateUserPoolDomainResponseTypeDef,
+    VerifySoftwareTokenResponseTypeDef,
     AdminDisableProviderForUserRequestRequestTypeDef,
     AdminLinkProviderForUserRequestRequestTypeDef,
     AdminGetUserResponseTypeDef,
     AdminSetUserSettingsRequestRequestTypeDef,
     GetUserResponseTypeDef,
     SetUserSettingsRequestRequestTypeDef,
     UserTypeTypeDef,
+    AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
+    AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
+    ListGroupsRequestListGroupsPaginateTypeDef,
+    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
+    ListResourceServersRequestListResourceServersPaginateTypeDef,
+    ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
+    ListUserPoolsRequestListUserPoolsPaginateTypeDef,
+    ListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
     AdminListGroupsForUserResponseTypeDef,
     CreateGroupResponseTypeDef,
     GetGroupResponseTypeDef,
     ListGroupsResponseTypeDef,
     UpdateGroupResponseTypeDef,
     AdminSetUserMFAPreferenceRequestRequestTypeDef,
     SetUserMFAPreferenceRequestRequestTypeDef,
     AuthEventTypeTypeDef,
     AuthenticationResultTypeTypeDef,
+    SetUICustomizationRequestRequestTypeDef,
     ForgotPasswordResponseTypeDef,
     GetUserAttributeVerificationCodeResponseTypeDef,
     ResendConfirmationCodeResponseTypeDef,
     SignUpResponseTypeDef,
     UpdateUserAttributesResponseTypeDef,
+    CompromisedCredentialsRiskConfigurationTypeOutputTypeDef,
     CompromisedCredentialsRiskConfigurationTypeTypeDef,
     ConfirmDeviceRequestRequestTypeDef,
     ConfirmForgotPasswordRequestRequestTypeDef,
     ConfirmSignUpRequestRequestTypeDef,
     ForgotPasswordRequestRequestTypeDef,
     InitiateAuthRequestRequestTypeDef,
     ResendConfirmationCodeRequestRequestTypeDef,
@@ -588,27 +592,31 @@
     LambdaConfigTypeTypeDef,
     GetUICustomizationResponseTypeDef,
     SetUICustomizationResponseTypeDef,
     ListIdentityProvidersResponseTypeDef,
     ListUserPoolClientsResponseTypeDef,
     NotifyConfigurationTypeTypeDef,
     UserPoolPolicyTypeTypeDef,
+    RiskExceptionConfigurationTypeUnionTypeDef,
     SchemaAttributeTypeTypeDef,
+    UserAttributeUpdateSettingsTypeUnionTypeDef,
+    AccountRecoverySettingTypeUnionTypeDef,
     AdminGetDeviceResponseTypeDef,
     AdminListDevicesResponseTypeDef,
     GetDeviceResponseTypeDef,
     ListDevicesResponseTypeDef,
     AdminCreateUserResponseTypeDef,
     ListUsersInGroupResponseTypeDef,
     ListUsersResponseTypeDef,
     AdminListUserAuthEventsResponseTypeDef,
     AdminInitiateAuthResponseTypeDef,
     AdminRespondToAuthChallengeResponseTypeDef,
     InitiateAuthResponseTypeDef,
     RespondToAuthChallengeResponseTypeDef,
+    CompromisedCredentialsRiskConfigurationTypeUnionTypeDef,
     AdminInitiateAuthRequestRequestTypeDef,
     AdminRespondToAuthChallengeRequestRequestTypeDef,
     CreateResourceServerResponseTypeDef,
     DescribeResourceServerResponseTypeDef,
     ListResourceServersResponseTypeDef,
     UpdateResourceServerResponseTypeDef,
     CreateUserPoolClientResponseTypeDef,
@@ -630,15 +638,15 @@
     CreateUserPoolResponseTypeDef,
     DescribeUserPoolResponseTypeDef,
     DescribeRiskConfigurationResponseTypeDef,
     SetRiskConfigurationResponseTypeDef,
 )
 
 
-def get_structure() -> RecoveryOptionTypeTypeDef:
+def get_value() -> RecoveryOptionTypeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cognito-idp-2.5.2/README.md` & `types-aiobotocore-cognito-idp-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-cognito-idp"></a>
 
 # types-aiobotocore-cognito-idp
 
 [![PyPI - types-aiobotocore-cognito-idp](https://img.shields.io/pypi/v/types-aiobotocore-cognito-idp.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-idp)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cognito-idp.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-idp)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cognito-idp?color=blue)](https://pypistats.org/packages/types-aiobotocore-cognito-idp)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cognito-idp)](https://pepy.tech/project/types-aiobotocore-cognito-idp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CognitoIdentityProvider 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
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
 [types-aiobotocore-cognito-idp docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/).
 
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
@@ -347,77 +347,75 @@
 )
 
 
 def check_value(value: AccountTakeoverEventActionTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cognito_idp.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cognito_idp.type_defs import (
     RecoveryOptionTypeTypeDef,
     AccountTakeoverActionTypeTypeDef,
     AdminAddUserToGroupRequestRequestTypeDef,
     AdminConfirmSignUpRequestRequestTypeDef,
     MessageTemplateTypeTypeDef,
     AttributeTypeTypeDef,
+    ResponseMetadataTypeDef,
     AdminDeleteUserAttributesRequestRequestTypeDef,
     AdminDeleteUserRequestRequestTypeDef,
     ProviderUserIdentifierTypeTypeDef,
     AdminDisableUserRequestRequestTypeDef,
     AdminEnableUserRequestRequestTypeDef,
     AdminForgetDeviceRequestRequestTypeDef,
     AdminGetDeviceRequestRequestTypeDef,
     AdminGetUserRequestRequestTypeDef,
     MFAOptionTypeTypeDef,
     AnalyticsMetadataTypeTypeDef,
     AdminListDevicesRequestRequestTypeDef,
-    AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
+    PaginatorConfigTypeDef,
     AdminListGroupsForUserRequestRequestTypeDef,
     GroupTypeTypeDef,
-    AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
     AdminListUserAuthEventsRequestRequestTypeDef,
     AdminRemoveUserFromGroupRequestRequestTypeDef,
     AdminResetUserPasswordRequestRequestTypeDef,
     SMSMfaSettingsTypeTypeDef,
     SoftwareTokenMfaSettingsTypeTypeDef,
     AdminSetUserPasswordRequestRequestTypeDef,
     AdminUpdateAuthEventFeedbackRequestRequestTypeDef,
     AdminUpdateDeviceStatusRequestRequestTypeDef,
     AdminUserGlobalSignOutRequestRequestTypeDef,
     AnalyticsConfigurationTypeTypeDef,
     AssociateSoftwareTokenRequestRequestTypeDef,
-    AssociateSoftwareTokenResponseTypeDef,
     ChallengeResponseTypeTypeDef,
     EventContextDataTypeTypeDef,
     EventFeedbackTypeTypeDef,
     EventRiskTypeTypeDef,
     NewDeviceMetadataTypeTypeDef,
+    BlobTypeDef,
     ChangePasswordRequestRequestTypeDef,
     CodeDeliveryDetailsTypeTypeDef,
     CompromisedCredentialsActionsTypeTypeDef,
     DeviceSecretVerifierConfigTypeTypeDef,
-    ConfirmDeviceResponseTypeDef,
     UserContextDataTypeTypeDef,
     HttpHeaderTypeDef,
     CreateGroupRequestRequestTypeDef,
     CreateIdentityProviderRequestRequestTypeDef,
     IdentityProviderTypeTypeDef,
     ResourceServerScopeTypeTypeDef,
     CreateUserImportJobRequestRequestTypeDef,
     UserImportJobTypeTypeDef,
     TokenValidityUnitsTypeTypeDef,
     CustomDomainConfigTypeTypeDef,
-    CreateUserPoolDomainResponseTypeDef,
     DeviceConfigurationTypeTypeDef,
     EmailConfigurationTypeTypeDef,
     SmsConfigurationTypeTypeDef,
     UserAttributeUpdateSettingsTypeTypeDef,
     UserPoolAddOnsTypeTypeDef,
     UsernameConfigurationTypeTypeDef,
     VerificationMessageTemplateTypeTypeDef,
@@ -434,99 +432,106 @@
     DescribeIdentityProviderRequestRequestTypeDef,
     DescribeResourceServerRequestRequestTypeDef,
     DescribeRiskConfigurationRequestRequestTypeDef,
     DescribeUserImportJobRequestRequestTypeDef,
     DescribeUserPoolClientRequestRequestTypeDef,
     DescribeUserPoolDomainRequestRequestTypeDef,
     DescribeUserPoolRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ForgetDeviceRequestRequestTypeDef,
     GetCSVHeaderRequestRequestTypeDef,
-    GetCSVHeaderResponseTypeDef,
     GetDeviceRequestRequestTypeDef,
     GetGroupRequestRequestTypeDef,
     GetIdentityProviderByIdentifierRequestRequestTypeDef,
     GetSigningCertificateRequestRequestTypeDef,
-    GetSigningCertificateResponseTypeDef,
     GetUICustomizationRequestRequestTypeDef,
     UICustomizationTypeTypeDef,
     GetUserAttributeVerificationCodeRequestRequestTypeDef,
     GetUserPoolMfaConfigRequestRequestTypeDef,
     SoftwareTokenMfaConfigTypeTypeDef,
     GetUserRequestRequestTypeDef,
     GlobalSignOutRequestRequestTypeDef,
     ListDevicesRequestRequestTypeDef,
-    ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
-    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
     ListIdentityProvidersRequestRequestTypeDef,
     ProviderDescriptionTypeDef,
-    ListResourceServersRequestListResourceServersPaginateTypeDef,
     ListResourceServersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListUserImportJobsRequestRequestTypeDef,
-    ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
     ListUserPoolClientsRequestRequestTypeDef,
     UserPoolClientDescriptionTypeDef,
-    ListUserPoolsRequestListUserPoolsPaginateTypeDef,
     ListUserPoolsRequestRequestTypeDef,
-    ListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
     ListUsersInGroupRequestRequestTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     NotifyEmailTypeTypeDef,
     NumberAttributeConstraintsTypeTypeDef,
-    PaginatorConfigTypeDef,
     PasswordPolicyTypeTypeDef,
-    ResponseMetadataTypeDef,
     RevokeTokenRequestRequestTypeDef,
+    RiskExceptionConfigurationTypeOutputTypeDef,
     RiskExceptionConfigurationTypeTypeDef,
     StringAttributeConstraintsTypeTypeDef,
-    SetUICustomizationRequestRequestTypeDef,
     StartUserImportJobRequestRequestTypeDef,
     StopUserImportJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAuthEventFeedbackRequestRequestTypeDef,
     UpdateDeviceStatusRequestRequestTypeDef,
     UpdateGroupRequestRequestTypeDef,
     UpdateIdentityProviderRequestRequestTypeDef,
-    UpdateUserPoolDomainResponseTypeDef,
+    UserAttributeUpdateSettingsTypeOutputTypeDef,
     VerifySoftwareTokenRequestRequestTypeDef,
-    VerifySoftwareTokenResponseTypeDef,
     VerifyUserAttributeRequestRequestTypeDef,
+    AccountRecoverySettingTypeOutputTypeDef,
     AccountRecoverySettingTypeTypeDef,
     AccountTakeoverActionsTypeTypeDef,
     AdminCreateUserConfigTypeTypeDef,
     AdminCreateUserRequestRequestTypeDef,
     AdminUpdateUserAttributesRequestRequestTypeDef,
     DeviceTypeTypeDef,
     UpdateUserAttributesRequestRequestTypeDef,
+    AssociateSoftwareTokenResponseTypeDef,
+    ConfirmDeviceResponseTypeDef,
+    CreateUserPoolDomainResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCSVHeaderResponseTypeDef,
+    GetSigningCertificateResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateUserPoolDomainResponseTypeDef,
+    VerifySoftwareTokenResponseTypeDef,
     AdminDisableProviderForUserRequestRequestTypeDef,
     AdminLinkProviderForUserRequestRequestTypeDef,
     AdminGetUserResponseTypeDef,
     AdminSetUserSettingsRequestRequestTypeDef,
     GetUserResponseTypeDef,
     SetUserSettingsRequestRequestTypeDef,
     UserTypeTypeDef,
+    AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
+    AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
+    ListGroupsRequestListGroupsPaginateTypeDef,
+    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
+    ListResourceServersRequestListResourceServersPaginateTypeDef,
+    ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
+    ListUserPoolsRequestListUserPoolsPaginateTypeDef,
+    ListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
     AdminListGroupsForUserResponseTypeDef,
     CreateGroupResponseTypeDef,
     GetGroupResponseTypeDef,
     ListGroupsResponseTypeDef,
     UpdateGroupResponseTypeDef,
     AdminSetUserMFAPreferenceRequestRequestTypeDef,
     SetUserMFAPreferenceRequestRequestTypeDef,
     AuthEventTypeTypeDef,
     AuthenticationResultTypeTypeDef,
+    SetUICustomizationRequestRequestTypeDef,
     ForgotPasswordResponseTypeDef,
     GetUserAttributeVerificationCodeResponseTypeDef,
     ResendConfirmationCodeResponseTypeDef,
     SignUpResponseTypeDef,
     UpdateUserAttributesResponseTypeDef,
+    CompromisedCredentialsRiskConfigurationTypeOutputTypeDef,
     CompromisedCredentialsRiskConfigurationTypeTypeDef,
     ConfirmDeviceRequestRequestTypeDef,
     ConfirmForgotPasswordRequestRequestTypeDef,
     ConfirmSignUpRequestRequestTypeDef,
     ForgotPasswordRequestRequestTypeDef,
     InitiateAuthRequestRequestTypeDef,
     ResendConfirmationCodeRequestRequestTypeDef,
@@ -555,27 +560,31 @@
     LambdaConfigTypeTypeDef,
     GetUICustomizationResponseTypeDef,
     SetUICustomizationResponseTypeDef,
     ListIdentityProvidersResponseTypeDef,
     ListUserPoolClientsResponseTypeDef,
     NotifyConfigurationTypeTypeDef,
     UserPoolPolicyTypeTypeDef,
+    RiskExceptionConfigurationTypeUnionTypeDef,
     SchemaAttributeTypeTypeDef,
+    UserAttributeUpdateSettingsTypeUnionTypeDef,
+    AccountRecoverySettingTypeUnionTypeDef,
     AdminGetDeviceResponseTypeDef,
     AdminListDevicesResponseTypeDef,
     GetDeviceResponseTypeDef,
     ListDevicesResponseTypeDef,
     AdminCreateUserResponseTypeDef,
     ListUsersInGroupResponseTypeDef,
     ListUsersResponseTypeDef,
     AdminListUserAuthEventsResponseTypeDef,
     AdminInitiateAuthResponseTypeDef,
     AdminRespondToAuthChallengeResponseTypeDef,
     InitiateAuthResponseTypeDef,
     RespondToAuthChallengeResponseTypeDef,
+    CompromisedCredentialsRiskConfigurationTypeUnionTypeDef,
     AdminInitiateAuthRequestRequestTypeDef,
     AdminRespondToAuthChallengeRequestRequestTypeDef,
     CreateResourceServerResponseTypeDef,
     DescribeResourceServerResponseTypeDef,
     ListResourceServersResponseTypeDef,
     UpdateResourceServerResponseTypeDef,
     CreateUserPoolClientResponseTypeDef,
@@ -597,15 +606,15 @@
     CreateUserPoolResponseTypeDef,
     DescribeUserPoolResponseTypeDef,
     DescribeRiskConfigurationResponseTypeDef,
     SetRiskConfigurationResponseTypeDef,
 )
 
 
-def get_structure() -> RecoveryOptionTypeTypeDef:
+def get_value() -> RecoveryOptionTypeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cognito-idp-2.5.2/setup.py` & `types-aiobotocore-cognito-idp-2.5.2.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cognito-idp",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_cognito_idp"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CognitoIdentityProvider 2.5.2 service generated with"
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
-    keywords="aiobotocore cognito-idp type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore cognito-idp type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_cognito_idp": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/"
```

### Comparing `types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/__init__.py` & `types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/__init__.pyi` & `types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/__main__.py` & `types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.CognitoIdentityProvider 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider\nOther"
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

### Comparing `types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/client.py` & `types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 
     session = get_session()
     async with session.create_client("cognito-idp") as client:
         client: CognitoIdentityProviderClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import (
     AliasAttributeTypeType,
     AuthFlowTypeType,
     ChallengeNameTypeType,
     DeletionProtectionTypeType,
@@ -46,30 +45,31 @@
     ListResourceServersPaginator,
     ListUserPoolClientsPaginator,
     ListUserPoolsPaginator,
     ListUsersInGroupPaginator,
     ListUsersPaginator,
 )
 from .type_defs import (
-    AccountRecoverySettingTypeTypeDef,
+    AccountRecoverySettingTypeUnionTypeDef,
     AccountTakeoverRiskConfigurationTypeTypeDef,
     AdminCreateUserConfigTypeTypeDef,
     AdminCreateUserResponseTypeDef,
     AdminGetDeviceResponseTypeDef,
     AdminGetUserResponseTypeDef,
     AdminInitiateAuthResponseTypeDef,
     AdminListDevicesResponseTypeDef,
     AdminListGroupsForUserResponseTypeDef,
     AdminListUserAuthEventsResponseTypeDef,
     AdminRespondToAuthChallengeResponseTypeDef,
     AnalyticsConfigurationTypeTypeDef,
     AnalyticsMetadataTypeTypeDef,
     AssociateSoftwareTokenResponseTypeDef,
     AttributeTypeTypeDef,
-    CompromisedCredentialsRiskConfigurationTypeTypeDef,
+    BlobTypeDef,
+    CompromisedCredentialsRiskConfigurationTypeUnionTypeDef,
     ConfirmDeviceResponseTypeDef,
     ContextDataTypeTypeDef,
     CreateGroupResponseTypeDef,
     CreateIdentityProviderResponseTypeDef,
     CreateResourceServerResponseTypeDef,
     CreateUserImportJobResponseTypeDef,
     CreateUserPoolClientResponseTypeDef,
@@ -110,15 +110,15 @@
     ListUsersInGroupResponseTypeDef,
     ListUsersResponseTypeDef,
     MFAOptionTypeTypeDef,
     ProviderUserIdentifierTypeTypeDef,
     ResendConfirmationCodeResponseTypeDef,
     ResourceServerScopeTypeTypeDef,
     RespondToAuthChallengeResponseTypeDef,
-    RiskExceptionConfigurationTypeTypeDef,
+    RiskExceptionConfigurationTypeUnionTypeDef,
     SchemaAttributeTypeTypeDef,
     SetRiskConfigurationResponseTypeDef,
     SetUICustomizationResponseTypeDef,
     SetUserPoolMfaConfigResponseTypeDef,
     SignUpResponseTypeDef,
     SmsConfigurationTypeTypeDef,
     SmsMfaConfigTypeTypeDef,
@@ -130,15 +130,15 @@
     TokenValidityUnitsTypeTypeDef,
     UpdateGroupResponseTypeDef,
     UpdateIdentityProviderResponseTypeDef,
     UpdateResourceServerResponseTypeDef,
     UpdateUserAttributesResponseTypeDef,
     UpdateUserPoolClientResponseTypeDef,
     UpdateUserPoolDomainResponseTypeDef,
-    UserAttributeUpdateSettingsTypeTypeDef,
+    UserAttributeUpdateSettingsTypeUnionTypeDef,
     UserContextDataTypeTypeDef,
     UsernameConfigurationTypeTypeDef,
     UserPoolAddOnsTypeTypeDef,
     UserPoolPolicyTypeTypeDef,
     VerificationMessageTemplateTypeTypeDef,
     VerifySoftwareTokenResponseTypeDef,
 )
@@ -700,24 +700,24 @@
         UsernameAttributes: Sequence[UsernameAttributeTypeType] = ...,
         SmsVerificationMessage: str = ...,
         EmailVerificationMessage: str = ...,
         EmailVerificationSubject: str = ...,
         VerificationMessageTemplate: VerificationMessageTemplateTypeTypeDef = ...,
         SmsAuthenticationMessage: str = ...,
         MfaConfiguration: UserPoolMfaTypeType = ...,
-        UserAttributeUpdateSettings: UserAttributeUpdateSettingsTypeTypeDef = ...,
+        UserAttributeUpdateSettings: UserAttributeUpdateSettingsTypeUnionTypeDef = ...,
         DeviceConfiguration: DeviceConfigurationTypeTypeDef = ...,
         EmailConfiguration: EmailConfigurationTypeTypeDef = ...,
         SmsConfiguration: SmsConfigurationTypeTypeDef = ...,
         UserPoolTags: Mapping[str, str] = ...,
         AdminCreateUserConfig: AdminCreateUserConfigTypeTypeDef = ...,
         Schema: Sequence[SchemaAttributeTypeTypeDef] = ...,
         UserPoolAddOns: UserPoolAddOnsTypeTypeDef = ...,
         UsernameConfiguration: UsernameConfigurationTypeTypeDef = ...,
-        AccountRecoverySetting: AccountRecoverySettingTypeTypeDef = ...
+        AccountRecoverySetting: AccountRecoverySettingTypeUnionTypeDef = ...
     ) -> CreateUserPoolResponseTypeDef:
         """
         Creates a new Amazon Cognito user pool and sets the password policy for the
         pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#create_user_pool)
@@ -1221,32 +1221,27 @@
         """
 
     async def set_risk_configuration(
         self,
         *,
         UserPoolId: str,
         ClientId: str = ...,
-        CompromisedCredentialsRiskConfiguration: CompromisedCredentialsRiskConfigurationTypeTypeDef = ...,
+        CompromisedCredentialsRiskConfiguration: CompromisedCredentialsRiskConfigurationTypeUnionTypeDef = ...,
         AccountTakeoverRiskConfiguration: AccountTakeoverRiskConfigurationTypeTypeDef = ...,
-        RiskExceptionConfiguration: RiskExceptionConfigurationTypeTypeDef = ...
+        RiskExceptionConfiguration: RiskExceptionConfigurationTypeUnionTypeDef = ...
     ) -> SetRiskConfigurationResponseTypeDef:
         """
         Configures actions on detected risks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_risk_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#set_risk_configuration)
         """
 
     async def set_ui_customization(
-        self,
-        *,
-        UserPoolId: str,
-        ClientId: str = ...,
-        CSS: str = ...,
-        ImageFile: Union[str, bytes, IO[Any], StreamingBody] = ...
+        self, *, UserPoolId: str, ClientId: str = ..., CSS: str = ..., ImageFile: BlobTypeDef = ...
     ) -> SetUICustomizationResponseTypeDef:
         """
         Sets the user interface (UI) customization information for a user pool's built-
         in app UI.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_ui_customization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#set_ui_customization)
@@ -1450,23 +1445,23 @@
         LambdaConfig: LambdaConfigTypeTypeDef = ...,
         AutoVerifiedAttributes: Sequence[VerifiedAttributeTypeType] = ...,
         SmsVerificationMessage: str = ...,
         EmailVerificationMessage: str = ...,
         EmailVerificationSubject: str = ...,
         VerificationMessageTemplate: VerificationMessageTemplateTypeTypeDef = ...,
         SmsAuthenticationMessage: str = ...,
-        UserAttributeUpdateSettings: UserAttributeUpdateSettingsTypeTypeDef = ...,
+        UserAttributeUpdateSettings: UserAttributeUpdateSettingsTypeUnionTypeDef = ...,
         MfaConfiguration: UserPoolMfaTypeType = ...,
         DeviceConfiguration: DeviceConfigurationTypeTypeDef = ...,
         EmailConfiguration: EmailConfigurationTypeTypeDef = ...,
         SmsConfiguration: SmsConfigurationTypeTypeDef = ...,
         UserPoolTags: Mapping[str, str] = ...,
         AdminCreateUserConfig: AdminCreateUserConfigTypeTypeDef = ...,
         UserPoolAddOns: UserPoolAddOnsTypeTypeDef = ...,
-        AccountRecoverySetting: AccountRecoverySettingTypeTypeDef = ...
+        AccountRecoverySetting: AccountRecoverySettingTypeUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the specified user pool with the specified attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_user_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#update_user_pool)
         """
```

### Comparing `types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/client.pyi` & `types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 
     session = get_session()
     async with session.create_client("cognito-idp") as client:
         client: CognitoIdentityProviderClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import (
     AliasAttributeTypeType,
     AuthFlowTypeType,
     ChallengeNameTypeType,
     DeletionProtectionTypeType,
@@ -46,30 +45,31 @@
     ListResourceServersPaginator,
     ListUserPoolClientsPaginator,
     ListUserPoolsPaginator,
     ListUsersInGroupPaginator,
     ListUsersPaginator,
 )
 from .type_defs import (
-    AccountRecoverySettingTypeTypeDef,
+    AccountRecoverySettingTypeUnionTypeDef,
     AccountTakeoverRiskConfigurationTypeTypeDef,
     AdminCreateUserConfigTypeTypeDef,
     AdminCreateUserResponseTypeDef,
     AdminGetDeviceResponseTypeDef,
     AdminGetUserResponseTypeDef,
     AdminInitiateAuthResponseTypeDef,
     AdminListDevicesResponseTypeDef,
     AdminListGroupsForUserResponseTypeDef,
     AdminListUserAuthEventsResponseTypeDef,
     AdminRespondToAuthChallengeResponseTypeDef,
     AnalyticsConfigurationTypeTypeDef,
     AnalyticsMetadataTypeTypeDef,
     AssociateSoftwareTokenResponseTypeDef,
     AttributeTypeTypeDef,
-    CompromisedCredentialsRiskConfigurationTypeTypeDef,
+    BlobTypeDef,
+    CompromisedCredentialsRiskConfigurationTypeUnionTypeDef,
     ConfirmDeviceResponseTypeDef,
     ContextDataTypeTypeDef,
     CreateGroupResponseTypeDef,
     CreateIdentityProviderResponseTypeDef,
     CreateResourceServerResponseTypeDef,
     CreateUserImportJobResponseTypeDef,
     CreateUserPoolClientResponseTypeDef,
@@ -110,15 +110,15 @@
     ListUsersInGroupResponseTypeDef,
     ListUsersResponseTypeDef,
     MFAOptionTypeTypeDef,
     ProviderUserIdentifierTypeTypeDef,
     ResendConfirmationCodeResponseTypeDef,
     ResourceServerScopeTypeTypeDef,
     RespondToAuthChallengeResponseTypeDef,
-    RiskExceptionConfigurationTypeTypeDef,
+    RiskExceptionConfigurationTypeUnionTypeDef,
     SchemaAttributeTypeTypeDef,
     SetRiskConfigurationResponseTypeDef,
     SetUICustomizationResponseTypeDef,
     SetUserPoolMfaConfigResponseTypeDef,
     SignUpResponseTypeDef,
     SmsConfigurationTypeTypeDef,
     SmsMfaConfigTypeTypeDef,
@@ -130,15 +130,15 @@
     TokenValidityUnitsTypeTypeDef,
     UpdateGroupResponseTypeDef,
     UpdateIdentityProviderResponseTypeDef,
     UpdateResourceServerResponseTypeDef,
     UpdateUserAttributesResponseTypeDef,
     UpdateUserPoolClientResponseTypeDef,
     UpdateUserPoolDomainResponseTypeDef,
-    UserAttributeUpdateSettingsTypeTypeDef,
+    UserAttributeUpdateSettingsTypeUnionTypeDef,
     UserContextDataTypeTypeDef,
     UsernameConfigurationTypeTypeDef,
     UserPoolAddOnsTypeTypeDef,
     UserPoolPolicyTypeTypeDef,
     VerificationMessageTemplateTypeTypeDef,
     VerifySoftwareTokenResponseTypeDef,
 )
@@ -657,24 +657,24 @@
         UsernameAttributes: Sequence[UsernameAttributeTypeType] = ...,
         SmsVerificationMessage: str = ...,
         EmailVerificationMessage: str = ...,
         EmailVerificationSubject: str = ...,
         VerificationMessageTemplate: VerificationMessageTemplateTypeTypeDef = ...,
         SmsAuthenticationMessage: str = ...,
         MfaConfiguration: UserPoolMfaTypeType = ...,
-        UserAttributeUpdateSettings: UserAttributeUpdateSettingsTypeTypeDef = ...,
+        UserAttributeUpdateSettings: UserAttributeUpdateSettingsTypeUnionTypeDef = ...,
         DeviceConfiguration: DeviceConfigurationTypeTypeDef = ...,
         EmailConfiguration: EmailConfigurationTypeTypeDef = ...,
         SmsConfiguration: SmsConfigurationTypeTypeDef = ...,
         UserPoolTags: Mapping[str, str] = ...,
         AdminCreateUserConfig: AdminCreateUserConfigTypeTypeDef = ...,
         Schema: Sequence[SchemaAttributeTypeTypeDef] = ...,
         UserPoolAddOns: UserPoolAddOnsTypeTypeDef = ...,
         UsernameConfiguration: UsernameConfigurationTypeTypeDef = ...,
-        AccountRecoverySetting: AccountRecoverySettingTypeTypeDef = ...
+        AccountRecoverySetting: AccountRecoverySettingTypeUnionTypeDef = ...
     ) -> CreateUserPoolResponseTypeDef:
         """
         Creates a new Amazon Cognito user pool and sets the password policy for the
         pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#create_user_pool)
@@ -1133,31 +1133,26 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#revoke_token)
         """
     async def set_risk_configuration(
         self,
         *,
         UserPoolId: str,
         ClientId: str = ...,
-        CompromisedCredentialsRiskConfiguration: CompromisedCredentialsRiskConfigurationTypeTypeDef = ...,
+        CompromisedCredentialsRiskConfiguration: CompromisedCredentialsRiskConfigurationTypeUnionTypeDef = ...,
         AccountTakeoverRiskConfiguration: AccountTakeoverRiskConfigurationTypeTypeDef = ...,
-        RiskExceptionConfiguration: RiskExceptionConfigurationTypeTypeDef = ...
+        RiskExceptionConfiguration: RiskExceptionConfigurationTypeUnionTypeDef = ...
     ) -> SetRiskConfigurationResponseTypeDef:
         """
         Configures actions on detected risks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_risk_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#set_risk_configuration)
         """
     async def set_ui_customization(
-        self,
-        *,
-        UserPoolId: str,
-        ClientId: str = ...,
-        CSS: str = ...,
-        ImageFile: Union[str, bytes, IO[Any], StreamingBody] = ...
+        self, *, UserPoolId: str, ClientId: str = ..., CSS: str = ..., ImageFile: BlobTypeDef = ...
     ) -> SetUICustomizationResponseTypeDef:
         """
         Sets the user interface (UI) customization information for a user pool's built-
         in app UI.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_ui_customization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#set_ui_customization)
@@ -1346,23 +1341,23 @@
         LambdaConfig: LambdaConfigTypeTypeDef = ...,
         AutoVerifiedAttributes: Sequence[VerifiedAttributeTypeType] = ...,
         SmsVerificationMessage: str = ...,
         EmailVerificationMessage: str = ...,
         EmailVerificationSubject: str = ...,
         VerificationMessageTemplate: VerificationMessageTemplateTypeTypeDef = ...,
         SmsAuthenticationMessage: str = ...,
-        UserAttributeUpdateSettings: UserAttributeUpdateSettingsTypeTypeDef = ...,
+        UserAttributeUpdateSettings: UserAttributeUpdateSettingsTypeUnionTypeDef = ...,
         MfaConfiguration: UserPoolMfaTypeType = ...,
         DeviceConfiguration: DeviceConfigurationTypeTypeDef = ...,
         EmailConfiguration: EmailConfigurationTypeTypeDef = ...,
         SmsConfiguration: SmsConfigurationTypeTypeDef = ...,
         UserPoolTags: Mapping[str, str] = ...,
         AdminCreateUserConfig: AdminCreateUserConfigTypeTypeDef = ...,
         UserPoolAddOns: UserPoolAddOnsTypeTypeDef = ...,
-        AccountRecoverySetting: AccountRecoverySettingTypeTypeDef = ...
+        AccountRecoverySetting: AccountRecoverySettingTypeUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the specified user pool with the specified attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_user_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#update_user_pool)
         """
```

### Comparing `types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/literals.py` & `types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/literals.pyi` & `types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/paginator.py` & `types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,105 +80,105 @@
 class AdminListGroupsForUserPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListGroupsForUser)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#adminlistgroupsforuserpaginator)
     """
 
     def paginate(
-        self, *, Username: str, UserPoolId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Username: str, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[AdminListGroupsForUserResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListGroupsForUser.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#adminlistgroupsforuserpaginator)
         """
 
 
 class AdminListUserAuthEventsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListUserAuthEvents)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#adminlistuserautheventspaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, Username: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserPoolId: str, Username: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[AdminListUserAuthEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListUserAuthEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#adminlistuserautheventspaginator)
         """
 
 
 class ListGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#listgroupspaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#listgroupspaginator)
         """
 
 
 class ListIdentityProvidersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListIdentityProviders)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#listidentityproviderspaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListIdentityProvidersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListIdentityProviders.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#listidentityproviderspaginator)
         """
 
 
 class ListResourceServersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListResourceServers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#listresourceserverspaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListResourceServers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#listresourceserverspaginator)
         """
 
 
 class ListUserPoolClientsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPoolClients)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#listuserpoolclientspaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUserPoolClientsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPoolClients.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#listuserpoolclientspaginator)
         """
 
 
 class ListUserPoolsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPools)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#listuserpoolspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUserPoolsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPools.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#listuserpoolspaginator)
         """
 
 
@@ -190,28 +190,28 @@
 
     def paginate(
         self,
         *,
         UserPoolId: str,
         AttributesToGet: Sequence[str] = ...,
         Filter: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#listuserspaginator)
         """
 
 
 class ListUsersInGroupPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsersInGroup)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#listusersingrouppaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, GroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserPoolId: str, GroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUsersInGroupResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsersInGroup.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#listusersingrouppaginator)
         """
```

### Comparing `types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/paginator.pyi` & `types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -77,99 +77,99 @@
 class AdminListGroupsForUserPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListGroupsForUser)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#adminlistgroupsforuserpaginator)
     """
 
     def paginate(
-        self, *, Username: str, UserPoolId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Username: str, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[AdminListGroupsForUserResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListGroupsForUser.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#adminlistgroupsforuserpaginator)
         """
 
 class AdminListUserAuthEventsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListUserAuthEvents)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#adminlistuserautheventspaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, Username: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserPoolId: str, Username: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[AdminListUserAuthEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListUserAuthEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#adminlistuserautheventspaginator)
         """
 
 class ListGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#listgroupspaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#listgroupspaginator)
         """
 
 class ListIdentityProvidersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListIdentityProviders)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#listidentityproviderspaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListIdentityProvidersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListIdentityProviders.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#listidentityproviderspaginator)
         """
 
 class ListResourceServersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListResourceServers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#listresourceserverspaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListResourceServers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#listresourceserverspaginator)
         """
 
 class ListUserPoolClientsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPoolClients)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#listuserpoolclientspaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUserPoolClientsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPoolClients.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#listuserpoolclientspaginator)
         """
 
 class ListUserPoolsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPools)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#listuserpoolspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUserPoolsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPools.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#listuserpoolspaginator)
         """
 
 class ListUsersPaginator(AioPaginator):
@@ -180,27 +180,27 @@
 
     def paginate(
         self,
         *,
         UserPoolId: str,
         AttributesToGet: Sequence[str] = ...,
         Filter: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#listuserspaginator)
         """
 
 class ListUsersInGroupPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsersInGroup)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#listusersingrouppaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, GroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserPoolId: str, GroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUsersInGroupResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsersInGroup.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/paginators/#listusersingrouppaginator)
         """
```

### Comparing `types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/type_defs.py` & `types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_cognito_idp.type_defs import RecoveryOptionTypeTypeDef
 
-    data: RecoveryOptionTypeTypeDef = {...}
+    data: RecoveryOptionTypeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -68,62 +68,60 @@
 __all__ = (
     "RecoveryOptionTypeTypeDef",
     "AccountTakeoverActionTypeTypeDef",
     "AdminAddUserToGroupRequestRequestTypeDef",
     "AdminConfirmSignUpRequestRequestTypeDef",
     "MessageTemplateTypeTypeDef",
     "AttributeTypeTypeDef",
+    "ResponseMetadataTypeDef",
     "AdminDeleteUserAttributesRequestRequestTypeDef",
     "AdminDeleteUserRequestRequestTypeDef",
     "ProviderUserIdentifierTypeTypeDef",
     "AdminDisableUserRequestRequestTypeDef",
     "AdminEnableUserRequestRequestTypeDef",
     "AdminForgetDeviceRequestRequestTypeDef",
     "AdminGetDeviceRequestRequestTypeDef",
     "AdminGetUserRequestRequestTypeDef",
     "MFAOptionTypeTypeDef",
     "AnalyticsMetadataTypeTypeDef",
     "AdminListDevicesRequestRequestTypeDef",
-    "AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "AdminListGroupsForUserRequestRequestTypeDef",
     "GroupTypeTypeDef",
-    "AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
     "AdminListUserAuthEventsRequestRequestTypeDef",
     "AdminRemoveUserFromGroupRequestRequestTypeDef",
     "AdminResetUserPasswordRequestRequestTypeDef",
     "SMSMfaSettingsTypeTypeDef",
     "SoftwareTokenMfaSettingsTypeTypeDef",
     "AdminSetUserPasswordRequestRequestTypeDef",
     "AdminUpdateAuthEventFeedbackRequestRequestTypeDef",
     "AdminUpdateDeviceStatusRequestRequestTypeDef",
     "AdminUserGlobalSignOutRequestRequestTypeDef",
     "AnalyticsConfigurationTypeTypeDef",
     "AssociateSoftwareTokenRequestRequestTypeDef",
-    "AssociateSoftwareTokenResponseTypeDef",
     "ChallengeResponseTypeTypeDef",
     "EventContextDataTypeTypeDef",
     "EventFeedbackTypeTypeDef",
     "EventRiskTypeTypeDef",
     "NewDeviceMetadataTypeTypeDef",
+    "BlobTypeDef",
     "ChangePasswordRequestRequestTypeDef",
     "CodeDeliveryDetailsTypeTypeDef",
     "CompromisedCredentialsActionsTypeTypeDef",
     "DeviceSecretVerifierConfigTypeTypeDef",
-    "ConfirmDeviceResponseTypeDef",
     "UserContextDataTypeTypeDef",
     "HttpHeaderTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "CreateIdentityProviderRequestRequestTypeDef",
     "IdentityProviderTypeTypeDef",
     "ResourceServerScopeTypeTypeDef",
     "CreateUserImportJobRequestRequestTypeDef",
     "UserImportJobTypeTypeDef",
     "TokenValidityUnitsTypeTypeDef",
     "CustomDomainConfigTypeTypeDef",
-    "CreateUserPoolDomainResponseTypeDef",
     "DeviceConfigurationTypeTypeDef",
     "EmailConfigurationTypeTypeDef",
     "SmsConfigurationTypeTypeDef",
     "UserAttributeUpdateSettingsTypeTypeDef",
     "UserPoolAddOnsTypeTypeDef",
     "UsernameConfigurationTypeTypeDef",
     "VerificationMessageTemplateTypeTypeDef",
@@ -140,99 +138,106 @@
     "DescribeIdentityProviderRequestRequestTypeDef",
     "DescribeResourceServerRequestRequestTypeDef",
     "DescribeRiskConfigurationRequestRequestTypeDef",
     "DescribeUserImportJobRequestRequestTypeDef",
     "DescribeUserPoolClientRequestRequestTypeDef",
     "DescribeUserPoolDomainRequestRequestTypeDef",
     "DescribeUserPoolRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ForgetDeviceRequestRequestTypeDef",
     "GetCSVHeaderRequestRequestTypeDef",
-    "GetCSVHeaderResponseTypeDef",
     "GetDeviceRequestRequestTypeDef",
     "GetGroupRequestRequestTypeDef",
     "GetIdentityProviderByIdentifierRequestRequestTypeDef",
     "GetSigningCertificateRequestRequestTypeDef",
-    "GetSigningCertificateResponseTypeDef",
     "GetUICustomizationRequestRequestTypeDef",
     "UICustomizationTypeTypeDef",
     "GetUserAttributeVerificationCodeRequestRequestTypeDef",
     "GetUserPoolMfaConfigRequestRequestTypeDef",
     "SoftwareTokenMfaConfigTypeTypeDef",
     "GetUserRequestRequestTypeDef",
     "GlobalSignOutRequestRequestTypeDef",
     "ListDevicesRequestRequestTypeDef",
-    "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListGroupsRequestRequestTypeDef",
-    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
     "ListIdentityProvidersRequestRequestTypeDef",
     "ProviderDescriptionTypeDef",
-    "ListResourceServersRequestListResourceServersPaginateTypeDef",
     "ListResourceServersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListUserImportJobsRequestRequestTypeDef",
-    "ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
     "ListUserPoolClientsRequestRequestTypeDef",
     "UserPoolClientDescriptionTypeDef",
-    "ListUserPoolsRequestListUserPoolsPaginateTypeDef",
     "ListUserPoolsRequestRequestTypeDef",
-    "ListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
     "ListUsersInGroupRequestRequestTypeDef",
-    "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
     "NotifyEmailTypeTypeDef",
     "NumberAttributeConstraintsTypeTypeDef",
-    "PaginatorConfigTypeDef",
     "PasswordPolicyTypeTypeDef",
-    "ResponseMetadataTypeDef",
     "RevokeTokenRequestRequestTypeDef",
+    "RiskExceptionConfigurationTypeOutputTypeDef",
     "RiskExceptionConfigurationTypeTypeDef",
     "StringAttributeConstraintsTypeTypeDef",
-    "SetUICustomizationRequestRequestTypeDef",
     "StartUserImportJobRequestRequestTypeDef",
     "StopUserImportJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAuthEventFeedbackRequestRequestTypeDef",
     "UpdateDeviceStatusRequestRequestTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "UpdateIdentityProviderRequestRequestTypeDef",
-    "UpdateUserPoolDomainResponseTypeDef",
+    "UserAttributeUpdateSettingsTypeOutputTypeDef",
     "VerifySoftwareTokenRequestRequestTypeDef",
-    "VerifySoftwareTokenResponseTypeDef",
     "VerifyUserAttributeRequestRequestTypeDef",
+    "AccountRecoverySettingTypeOutputTypeDef",
     "AccountRecoverySettingTypeTypeDef",
     "AccountTakeoverActionsTypeTypeDef",
     "AdminCreateUserConfigTypeTypeDef",
     "AdminCreateUserRequestRequestTypeDef",
     "AdminUpdateUserAttributesRequestRequestTypeDef",
     "DeviceTypeTypeDef",
     "UpdateUserAttributesRequestRequestTypeDef",
+    "AssociateSoftwareTokenResponseTypeDef",
+    "ConfirmDeviceResponseTypeDef",
+    "CreateUserPoolDomainResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetCSVHeaderResponseTypeDef",
+    "GetSigningCertificateResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateUserPoolDomainResponseTypeDef",
+    "VerifySoftwareTokenResponseTypeDef",
     "AdminDisableProviderForUserRequestRequestTypeDef",
     "AdminLinkProviderForUserRequestRequestTypeDef",
     "AdminGetUserResponseTypeDef",
     "AdminSetUserSettingsRequestRequestTypeDef",
     "GetUserResponseTypeDef",
     "SetUserSettingsRequestRequestTypeDef",
     "UserTypeTypeDef",
+    "AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
+    "AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
+    "ListGroupsRequestListGroupsPaginateTypeDef",
+    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
+    "ListResourceServersRequestListResourceServersPaginateTypeDef",
+    "ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
+    "ListUserPoolsRequestListUserPoolsPaginateTypeDef",
+    "ListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
     "AdminListGroupsForUserResponseTypeDef",
     "CreateGroupResponseTypeDef",
     "GetGroupResponseTypeDef",
     "ListGroupsResponseTypeDef",
     "UpdateGroupResponseTypeDef",
     "AdminSetUserMFAPreferenceRequestRequestTypeDef",
     "SetUserMFAPreferenceRequestRequestTypeDef",
     "AuthEventTypeTypeDef",
     "AuthenticationResultTypeTypeDef",
+    "SetUICustomizationRequestRequestTypeDef",
     "ForgotPasswordResponseTypeDef",
     "GetUserAttributeVerificationCodeResponseTypeDef",
     "ResendConfirmationCodeResponseTypeDef",
     "SignUpResponseTypeDef",
     "UpdateUserAttributesResponseTypeDef",
+    "CompromisedCredentialsRiskConfigurationTypeOutputTypeDef",
     "CompromisedCredentialsRiskConfigurationTypeTypeDef",
     "ConfirmDeviceRequestRequestTypeDef",
     "ConfirmForgotPasswordRequestRequestTypeDef",
     "ConfirmSignUpRequestRequestTypeDef",
     "ForgotPasswordRequestRequestTypeDef",
     "InitiateAuthRequestRequestTypeDef",
     "ResendConfirmationCodeRequestRequestTypeDef",
@@ -261,27 +266,31 @@
     "LambdaConfigTypeTypeDef",
     "GetUICustomizationResponseTypeDef",
     "SetUICustomizationResponseTypeDef",
     "ListIdentityProvidersResponseTypeDef",
     "ListUserPoolClientsResponseTypeDef",
     "NotifyConfigurationTypeTypeDef",
     "UserPoolPolicyTypeTypeDef",
+    "RiskExceptionConfigurationTypeUnionTypeDef",
     "SchemaAttributeTypeTypeDef",
+    "UserAttributeUpdateSettingsTypeUnionTypeDef",
+    "AccountRecoverySettingTypeUnionTypeDef",
     "AdminGetDeviceResponseTypeDef",
     "AdminListDevicesResponseTypeDef",
     "GetDeviceResponseTypeDef",
     "ListDevicesResponseTypeDef",
     "AdminCreateUserResponseTypeDef",
     "ListUsersInGroupResponseTypeDef",
     "ListUsersResponseTypeDef",
     "AdminListUserAuthEventsResponseTypeDef",
     "AdminInitiateAuthResponseTypeDef",
     "AdminRespondToAuthChallengeResponseTypeDef",
     "InitiateAuthResponseTypeDef",
     "RespondToAuthChallengeResponseTypeDef",
+    "CompromisedCredentialsRiskConfigurationTypeUnionTypeDef",
     "AdminInitiateAuthRequestRequestTypeDef",
     "AdminRespondToAuthChallengeRequestRequestTypeDef",
     "CreateResourceServerResponseTypeDef",
     "DescribeResourceServerResponseTypeDef",
     "ListResourceServersResponseTypeDef",
     "UpdateResourceServerResponseTypeDef",
     "CreateUserPoolClientResponseTypeDef",
@@ -379,14 +388,25 @@
 )
 
 
 class AttributeTypeTypeDef(_RequiredAttributeTypeTypeDef, _OptionalAttributeTypeTypeDef):
     pass
 
 
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
 AdminDeleteUserAttributesRequestRequestTypeDef = TypedDict(
     "AdminDeleteUserAttributesRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Username": str,
         "UserAttributeNames": Sequence[str],
     },
@@ -488,37 +508,24 @@
 
 class AdminListDevicesRequestRequestTypeDef(
     _RequiredAdminListDevicesRequestRequestTypeDef, _OptionalAdminListDevicesRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef = TypedDict(
-    "_RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
-    {
-        "Username": str,
-        "UserPoolId": str,
-    },
-)
-_OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef = TypedDict(
-    "_OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
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
-class AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef(
-    _RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
-    _OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
-):
-    pass
-
-
 _RequiredAdminListGroupsForUserRequestRequestTypeDef = TypedDict(
     "_RequiredAdminListGroupsForUserRequestRequestTypeDef",
     {
         "Username": str,
         "UserPoolId": str,
     },
 )
@@ -549,37 +556,14 @@
         "Precedence": int,
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
     },
     total=False,
 )
 
-_RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef = TypedDict(
-    "_RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
-    {
-        "UserPoolId": str,
-        "Username": str,
-    },
-)
-_OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef = TypedDict(
-    "_OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef(
-    _RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
-    _OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredAdminListUserAuthEventsRequestRequestTypeDef = TypedDict(
     "_RequiredAdminListUserAuthEventsRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Username": str,
     },
 )
@@ -733,23 +717,14 @@
     {
         "AccessToken": str,
         "Session": str,
     },
     total=False,
 )
 
-AssociateSoftwareTokenResponseTypeDef = TypedDict(
-    "AssociateSoftwareTokenResponseTypeDef",
-    {
-        "SecretCode": str,
-        "Session": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ChallengeResponseTypeTypeDef = TypedDict(
     "ChallengeResponseTypeTypeDef",
     {
         "ChallengeName": ChallengeNameType,
         "ChallengeResponse": ChallengeResponseType,
     },
     total=False,
@@ -804,14 +779,15 @@
     {
         "DeviceKey": str,
         "DeviceGroupKey": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ChangePasswordRequestRequestTypeDef = TypedDict(
     "ChangePasswordRequestRequestTypeDef",
     {
         "PreviousPassword": str,
         "ProposedPassword": str,
         "AccessToken": str,
     },
@@ -839,22 +815,14 @@
     {
         "PasswordVerifier": str,
         "Salt": str,
     },
     total=False,
 )
 
-ConfirmDeviceResponseTypeDef = TypedDict(
-    "ConfirmDeviceResponseTypeDef",
-    {
-        "UserConfirmationNecessary": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UserContextDataTypeTypeDef = TypedDict(
     "UserContextDataTypeTypeDef",
     {
         "IpAddress": str,
         "EncodedData": str,
     },
     total=False,
@@ -984,22 +952,14 @@
 CustomDomainConfigTypeTypeDef = TypedDict(
     "CustomDomainConfigTypeTypeDef",
     {
         "CertificateArn": str,
     },
 )
 
-CreateUserPoolDomainResponseTypeDef = TypedDict(
-    "CreateUserPoolDomainResponseTypeDef",
-    {
-        "CloudFrontDomain": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeviceConfigurationTypeTypeDef = TypedDict(
     "DeviceConfigurationTypeTypeDef",
     {
         "ChallengeRequiredOnNewDevice": bool,
         "DeviceOnlyRememberedOnUserPrompt": bool,
     },
     total=False,
@@ -1216,21 +1176,14 @@
 DescribeUserPoolRequestRequestTypeDef = TypedDict(
     "DescribeUserPoolRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredForgetDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredForgetDeviceRequestRequestTypeDef",
     {
         "DeviceKey": str,
     },
 )
 _OptionalForgetDeviceRequestRequestTypeDef = TypedDict(
@@ -1251,23 +1204,14 @@
 GetCSVHeaderRequestRequestTypeDef = TypedDict(
     "GetCSVHeaderRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 
-GetCSVHeaderResponseTypeDef = TypedDict(
-    "GetCSVHeaderResponseTypeDef",
-    {
-        "UserPoolId": str,
-        "CSVHeader": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredGetDeviceRequestRequestTypeDef",
     {
         "DeviceKey": str,
     },
 )
 _OptionalGetDeviceRequestRequestTypeDef = TypedDict(
@@ -1304,22 +1248,14 @@
 GetSigningCertificateRequestRequestTypeDef = TypedDict(
     "GetSigningCertificateRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 
-GetSigningCertificateResponseTypeDef = TypedDict(
-    "GetSigningCertificateResponseTypeDef",
-    {
-        "Certificate": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetUICustomizationRequestRequestTypeDef = TypedDict(
     "_RequiredGetUICustomizationRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalGetUICustomizationRequestRequestTypeDef = TypedDict(
@@ -1422,36 +1358,14 @@
 
 class ListDevicesRequestRequestTypeDef(
     _RequiredListDevicesRequestRequestTypeDef, _OptionalListDevicesRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListGroupsRequestListGroupsPaginateTypeDef(
-    _RequiredListGroupsRequestListGroupsPaginateTypeDef,
-    _OptionalListGroupsRequestListGroupsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupsRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalListGroupsRequestRequestTypeDef = TypedDict(
@@ -1466,36 +1380,14 @@
 
 class ListGroupsRequestRequestTypeDef(
     _RequiredListGroupsRequestRequestTypeDef, _OptionalListGroupsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
-    "_RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
-    "_OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef(
-    _RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
-    _OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListIdentityProvidersRequestRequestTypeDef = TypedDict(
     "_RequiredListIdentityProvidersRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalListIdentityProvidersRequestRequestTypeDef = TypedDict(
@@ -1522,36 +1414,14 @@
         "ProviderType": IdentityProviderTypeTypeType,
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
     },
     total=False,
 )
 
-_RequiredListResourceServersRequestListResourceServersPaginateTypeDef = TypedDict(
-    "_RequiredListResourceServersRequestListResourceServersPaginateTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalListResourceServersRequestListResourceServersPaginateTypeDef = TypedDict(
-    "_OptionalListResourceServersRequestListResourceServersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListResourceServersRequestListResourceServersPaginateTypeDef(
-    _RequiredListResourceServersRequestListResourceServersPaginateTypeDef,
-    _OptionalListResourceServersRequestListResourceServersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListResourceServersRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceServersRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalListResourceServersRequestRequestTypeDef = TypedDict(
@@ -1574,22 +1444,14 @@
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
 _RequiredListUserImportJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListUserImportJobsRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "MaxResults": int,
     },
 )
@@ -1605,36 +1467,14 @@
 class ListUserImportJobsRequestRequestTypeDef(
     _RequiredListUserImportJobsRequestRequestTypeDef,
     _OptionalListUserImportJobsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef = TypedDict(
-    "_RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef = TypedDict(
-    "_OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef(
-    _RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
-    _OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListUserPoolClientsRequestRequestTypeDef = TypedDict(
     "_RequiredListUserPoolClientsRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalListUserPoolClientsRequestRequestTypeDef = TypedDict(
@@ -1660,22 +1500,14 @@
         "ClientId": str,
         "UserPoolId": str,
         "ClientName": str,
     },
     total=False,
 )
 
-ListUserPoolsRequestListUserPoolsPaginateTypeDef = TypedDict(
-    "ListUserPoolsRequestListUserPoolsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 _RequiredListUserPoolsRequestRequestTypeDef = TypedDict(
     "_RequiredListUserPoolsRequestRequestTypeDef",
     {
         "MaxResults": int,
     },
 )
 _OptionalListUserPoolsRequestRequestTypeDef = TypedDict(
@@ -1689,37 +1521,14 @@
 
 class ListUserPoolsRequestRequestTypeDef(
     _RequiredListUserPoolsRequestRequestTypeDef, _OptionalListUserPoolsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef = TypedDict(
-    "_RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
-    {
-        "UserPoolId": str,
-        "GroupName": str,
-    },
-)
-_OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef = TypedDict(
-    "_OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListUsersInGroupRequestListUsersInGroupPaginateTypeDef(
-    _RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
-    _OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListUsersInGroupRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersInGroupRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "GroupName": str,
     },
 )
@@ -1735,38 +1544,14 @@
 
 class ListUsersInGroupRequestRequestTypeDef(
     _RequiredListUsersInGroupRequestRequestTypeDef, _OptionalListUsersInGroupRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_RequiredListUsersRequestListUsersPaginateTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_OptionalListUsersRequestListUsersPaginateTypeDef",
-    {
-        "AttributesToGet": Sequence[str],
-        "Filter": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListUsersRequestListUsersPaginateTypeDef(
-    _RequiredListUsersRequestListUsersPaginateTypeDef,
-    _OptionalListUsersRequestListUsersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -1812,48 +1597,27 @@
     {
         "MinValue": str,
         "MaxValue": str,
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
 PasswordPolicyTypeTypeDef = TypedDict(
     "PasswordPolicyTypeTypeDef",
     {
         "MinimumLength": int,
         "RequireUppercase": bool,
         "RequireLowercase": bool,
         "RequireNumbers": bool,
         "RequireSymbols": bool,
         "TemporaryPasswordValidityDays": int,
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
 _RequiredRevokeTokenRequestRequestTypeDef = TypedDict(
     "_RequiredRevokeTokenRequestRequestTypeDef",
     {
         "Token": str,
         "ClientId": str,
     },
 )
@@ -1868,56 +1632,41 @@
 
 class RevokeTokenRequestRequestTypeDef(
     _RequiredRevokeTokenRequestRequestTypeDef, _OptionalRevokeTokenRequestRequestTypeDef
 ):
     pass
 
 
-RiskExceptionConfigurationTypeTypeDef = TypedDict(
-    "RiskExceptionConfigurationTypeTypeDef",
+RiskExceptionConfigurationTypeOutputTypeDef = TypedDict(
+    "RiskExceptionConfigurationTypeOutputTypeDef",
     {
         "BlockedIPRangeList": List[str],
         "SkippedIPRangeList": List[str],
     },
     total=False,
 )
 
-StringAttributeConstraintsTypeTypeDef = TypedDict(
-    "StringAttributeConstraintsTypeTypeDef",
+RiskExceptionConfigurationTypeTypeDef = TypedDict(
+    "RiskExceptionConfigurationTypeTypeDef",
     {
-        "MinLength": str,
-        "MaxLength": str,
+        "BlockedIPRangeList": Sequence[str],
+        "SkippedIPRangeList": Sequence[str],
     },
     total=False,
 )
 
-_RequiredSetUICustomizationRequestRequestTypeDef = TypedDict(
-    "_RequiredSetUICustomizationRequestRequestTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalSetUICustomizationRequestRequestTypeDef = TypedDict(
-    "_OptionalSetUICustomizationRequestRequestTypeDef",
+StringAttributeConstraintsTypeTypeDef = TypedDict(
+    "StringAttributeConstraintsTypeTypeDef",
     {
-        "ClientId": str,
-        "CSS": str,
-        "ImageFile": Union[str, bytes, IO[Any], StreamingBody],
+        "MinLength": str,
+        "MaxLength": str,
     },
     total=False,
 )
 
-
-class SetUICustomizationRequestRequestTypeDef(
-    _RequiredSetUICustomizationRequestRequestTypeDef,
-    _OptionalSetUICustomizationRequestRequestTypeDef,
-):
-    pass
-
-
 StartUserImportJobRequestRequestTypeDef = TypedDict(
     "StartUserImportJobRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "JobId": str,
     },
 )
@@ -2025,20 +1774,20 @@
 class UpdateIdentityProviderRequestRequestTypeDef(
     _RequiredUpdateIdentityProviderRequestRequestTypeDef,
     _OptionalUpdateIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateUserPoolDomainResponseTypeDef = TypedDict(
-    "UpdateUserPoolDomainResponseTypeDef",
+UserAttributeUpdateSettingsTypeOutputTypeDef = TypedDict(
+    "UserAttributeUpdateSettingsTypeOutputTypeDef",
     {
-        "CloudFrontDomain": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AttributesRequireVerificationBeforeUpdate": List[VerifiedAttributeTypeType],
     },
+    total=False,
 )
 
 _RequiredVerifySoftwareTokenRequestRequestTypeDef = TypedDict(
     "_RequiredVerifySoftwareTokenRequestRequestTypeDef",
     {
         "UserCode": str,
     },
@@ -2057,32 +1806,31 @@
 class VerifySoftwareTokenRequestRequestTypeDef(
     _RequiredVerifySoftwareTokenRequestRequestTypeDef,
     _OptionalVerifySoftwareTokenRequestRequestTypeDef,
 ):
     pass
 
 
-VerifySoftwareTokenResponseTypeDef = TypedDict(
-    "VerifySoftwareTokenResponseTypeDef",
-    {
-        "Status": VerifySoftwareTokenResponseTypeType,
-        "Session": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VerifyUserAttributeRequestRequestTypeDef = TypedDict(
     "VerifyUserAttributeRequestRequestTypeDef",
     {
         "AccessToken": str,
         "AttributeName": str,
         "Code": str,
     },
 )
 
+AccountRecoverySettingTypeOutputTypeDef = TypedDict(
+    "AccountRecoverySettingTypeOutputTypeDef",
+    {
+        "RecoveryMechanisms": List[RecoveryOptionTypeTypeDef],
+    },
+    total=False,
+)
+
 AccountRecoverySettingTypeTypeDef = TypedDict(
     "AccountRecoverySettingTypeTypeDef",
     {
         "RecoveryMechanisms": Sequence[RecoveryOptionTypeTypeDef],
     },
     total=False,
 )
@@ -2190,14 +1938,88 @@
 class UpdateUserAttributesRequestRequestTypeDef(
     _RequiredUpdateUserAttributesRequestRequestTypeDef,
     _OptionalUpdateUserAttributesRequestRequestTypeDef,
 ):
     pass
 
 
+AssociateSoftwareTokenResponseTypeDef = TypedDict(
+    "AssociateSoftwareTokenResponseTypeDef",
+    {
+        "SecretCode": str,
+        "Session": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConfirmDeviceResponseTypeDef = TypedDict(
+    "ConfirmDeviceResponseTypeDef",
+    {
+        "UserConfirmationNecessary": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUserPoolDomainResponseTypeDef = TypedDict(
+    "CreateUserPoolDomainResponseTypeDef",
+    {
+        "CloudFrontDomain": str,
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
+GetCSVHeaderResponseTypeDef = TypedDict(
+    "GetCSVHeaderResponseTypeDef",
+    {
+        "UserPoolId": str,
+        "CSVHeader": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSigningCertificateResponseTypeDef = TypedDict(
+    "GetSigningCertificateResponseTypeDef",
+    {
+        "Certificate": str,
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
+UpdateUserPoolDomainResponseTypeDef = TypedDict(
+    "UpdateUserPoolDomainResponseTypeDef",
+    {
+        "CloudFrontDomain": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VerifySoftwareTokenResponseTypeDef = TypedDict(
+    "VerifySoftwareTokenResponseTypeDef",
+    {
+        "Status": VerifySoftwareTokenResponseTypeType,
+        "Session": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AdminDisableProviderForUserRequestRequestTypeDef = TypedDict(
     "AdminDisableProviderForUserRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "User": ProviderUserIdentifierTypeTypeDef,
     },
 )
@@ -2219,15 +2041,15 @@
         "UserCreateDate": datetime,
         "UserLastModifiedDate": datetime,
         "Enabled": bool,
         "UserStatus": UserStatusTypeType,
         "MFAOptions": List[MFAOptionTypeTypeDef],
         "PreferredMfaSetting": str,
         "UserMFASettingList": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AdminSetUserSettingsRequestRequestTypeDef = TypedDict(
     "AdminSetUserSettingsRequestRequestTypeDef",
     {
         "UserPoolId": str,
@@ -2240,15 +2062,15 @@
     "GetUserResponseTypeDef",
     {
         "Username": str,
         "UserAttributes": List[AttributeTypeTypeDef],
         "MFAOptions": List[MFAOptionTypeTypeDef],
         "PreferredMfaSetting": str,
         "UserMFASettingList": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SetUserSettingsRequestRequestTypeDef = TypedDict(
     "SetUserSettingsRequestRequestTypeDef",
     {
         "AccessToken": str,
@@ -2266,53 +2088,242 @@
         "Enabled": bool,
         "UserStatus": UserStatusTypeType,
         "MFAOptions": List[MFAOptionTypeTypeDef],
     },
     total=False,
 )
 
+_RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef = TypedDict(
+    "_RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
+    {
+        "Username": str,
+        "UserPoolId": str,
+    },
+)
+_OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef = TypedDict(
+    "_OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef(
+    _RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
+    _OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
+):
+    pass
+
+
+_RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef = TypedDict(
+    "_RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
+    {
+        "UserPoolId": str,
+        "Username": str,
+    },
+)
+_OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef = TypedDict(
+    "_OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef(
+    _RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
+    _OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListGroupsRequestListGroupsPaginateTypeDef(
+    _RequiredListGroupsRequestListGroupsPaginateTypeDef,
+    _OptionalListGroupsRequestListGroupsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
+    "_RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
+    "_OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef(
+    _RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
+    _OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListResourceServersRequestListResourceServersPaginateTypeDef = TypedDict(
+    "_RequiredListResourceServersRequestListResourceServersPaginateTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalListResourceServersRequestListResourceServersPaginateTypeDef = TypedDict(
+    "_OptionalListResourceServersRequestListResourceServersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListResourceServersRequestListResourceServersPaginateTypeDef(
+    _RequiredListResourceServersRequestListResourceServersPaginateTypeDef,
+    _OptionalListResourceServersRequestListResourceServersPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef = TypedDict(
+    "_RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef = TypedDict(
+    "_OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef(
+    _RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
+    _OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
+):
+    pass
+
+
+ListUserPoolsRequestListUserPoolsPaginateTypeDef = TypedDict(
+    "ListUserPoolsRequestListUserPoolsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef = TypedDict(
+    "_RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
+    {
+        "UserPoolId": str,
+        "GroupName": str,
+    },
+)
+_OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef = TypedDict(
+    "_OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListUsersInGroupRequestListUsersInGroupPaginateTypeDef(
+    _RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
+    _OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_RequiredListUsersRequestListUsersPaginateTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_OptionalListUsersRequestListUsersPaginateTypeDef",
+    {
+        "AttributesToGet": Sequence[str],
+        "Filter": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListUsersRequestListUsersPaginateTypeDef(
+    _RequiredListUsersRequestListUsersPaginateTypeDef,
+    _OptionalListUsersRequestListUsersPaginateTypeDef,
+):
+    pass
+
+
 AdminListGroupsForUserResponseTypeDef = TypedDict(
     "AdminListGroupsForUserResponseTypeDef",
     {
         "Groups": List[GroupTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateGroupResponseTypeDef = TypedDict(
     "CreateGroupResponseTypeDef",
     {
         "Group": GroupTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGroupResponseTypeDef = TypedDict(
     "GetGroupResponseTypeDef",
     {
         "Group": GroupTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGroupsResponseTypeDef = TypedDict(
     "ListGroupsResponseTypeDef",
     {
         "Groups": List[GroupTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGroupResponseTypeDef = TypedDict(
     "UpdateGroupResponseTypeDef",
     {
         "Group": GroupTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAdminSetUserMFAPreferenceRequestRequestTypeDef = TypedDict(
     "_RequiredAdminSetUserMFAPreferenceRequestRequestTypeDef",
     {
         "Username": str,
@@ -2383,66 +2394,112 @@
         "RefreshToken": str,
         "IdToken": str,
         "NewDeviceMetadata": NewDeviceMetadataTypeTypeDef,
     },
     total=False,
 )
 
+_RequiredSetUICustomizationRequestRequestTypeDef = TypedDict(
+    "_RequiredSetUICustomizationRequestRequestTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalSetUICustomizationRequestRequestTypeDef = TypedDict(
+    "_OptionalSetUICustomizationRequestRequestTypeDef",
+    {
+        "ClientId": str,
+        "CSS": str,
+        "ImageFile": BlobTypeDef,
+    },
+    total=False,
+)
+
+
+class SetUICustomizationRequestRequestTypeDef(
+    _RequiredSetUICustomizationRequestRequestTypeDef,
+    _OptionalSetUICustomizationRequestRequestTypeDef,
+):
+    pass
+
+
 ForgotPasswordResponseTypeDef = TypedDict(
     "ForgotPasswordResponseTypeDef",
     {
         "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserAttributeVerificationCodeResponseTypeDef = TypedDict(
     "GetUserAttributeVerificationCodeResponseTypeDef",
     {
         "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResendConfirmationCodeResponseTypeDef = TypedDict(
     "ResendConfirmationCodeResponseTypeDef",
     {
         "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SignUpResponseTypeDef = TypedDict(
     "SignUpResponseTypeDef",
     {
         "UserConfirmed": bool,
         "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
         "UserSub": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUserAttributesResponseTypeDef = TypedDict(
     "UpdateUserAttributesResponseTypeDef",
     {
         "CodeDeliveryDetailsList": List[CodeDeliveryDetailsTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCompromisedCredentialsRiskConfigurationTypeOutputTypeDef = TypedDict(
+    "_RequiredCompromisedCredentialsRiskConfigurationTypeOutputTypeDef",
+    {
+        "Actions": CompromisedCredentialsActionsTypeTypeDef,
+    },
+)
+_OptionalCompromisedCredentialsRiskConfigurationTypeOutputTypeDef = TypedDict(
+    "_OptionalCompromisedCredentialsRiskConfigurationTypeOutputTypeDef",
+    {
+        "EventFilter": List[EventFilterTypeType],
+    },
+    total=False,
+)
+
+
+class CompromisedCredentialsRiskConfigurationTypeOutputTypeDef(
+    _RequiredCompromisedCredentialsRiskConfigurationTypeOutputTypeDef,
+    _OptionalCompromisedCredentialsRiskConfigurationTypeOutputTypeDef,
+):
+    pass
+
+
 _RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef = TypedDict(
     "_RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef",
     {
         "Actions": CompromisedCredentialsActionsTypeTypeDef,
     },
 )
 _OptionalCompromisedCredentialsRiskConfigurationTypeTypeDef = TypedDict(
     "_OptionalCompromisedCredentialsRiskConfigurationTypeTypeDef",
     {
-        "EventFilter": List[EventFilterTypeType],
+        "EventFilter": Sequence[EventFilterTypeType],
     },
     total=False,
 )
 
 
 class CompromisedCredentialsRiskConfigurationTypeTypeDef(
     _RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef,
@@ -2682,39 +2739,39 @@
     pass
 
 
 CreateIdentityProviderResponseTypeDef = TypedDict(
     "CreateIdentityProviderResponseTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeIdentityProviderResponseTypeDef = TypedDict(
     "DescribeIdentityProviderResponseTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIdentityProviderByIdentifierResponseTypeDef = TypedDict(
     "GetIdentityProviderByIdentifierResponseTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateIdentityProviderResponseTypeDef = TypedDict(
     "UpdateIdentityProviderResponseTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateResourceServerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResourceServerRequestRequestTypeDef",
     {
         "UserPoolId": str,
@@ -2773,48 +2830,48 @@
     pass
 
 
 CreateUserImportJobResponseTypeDef = TypedDict(
     "CreateUserImportJobResponseTypeDef",
     {
         "UserImportJob": UserImportJobTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUserImportJobResponseTypeDef = TypedDict(
     "DescribeUserImportJobResponseTypeDef",
     {
         "UserImportJob": UserImportJobTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUserImportJobsResponseTypeDef = TypedDict(
     "ListUserImportJobsResponseTypeDef",
     {
         "UserImportJobs": List[UserImportJobTypeTypeDef],
         "PaginationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartUserImportJobResponseTypeDef = TypedDict(
     "StartUserImportJobResponseTypeDef",
     {
         "UserImportJob": UserImportJobTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopUserImportJobResponseTypeDef = TypedDict(
     "StopUserImportJobResponseTypeDef",
     {
         "UserImportJob": UserImportJobTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateUserPoolClientRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserPoolClientRequestRequestTypeDef",
     {
         "UserPoolId": str,
@@ -3006,41 +3063,41 @@
     total=False,
 )
 
 GetUICustomizationResponseTypeDef = TypedDict(
     "GetUICustomizationResponseTypeDef",
     {
         "UICustomization": UICustomizationTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SetUICustomizationResponseTypeDef = TypedDict(
     "SetUICustomizationResponseTypeDef",
     {
         "UICustomization": UICustomizationTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIdentityProvidersResponseTypeDef = TypedDict(
     "ListIdentityProvidersResponseTypeDef",
     {
         "Providers": List[ProviderDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUserPoolClientsResponseTypeDef = TypedDict(
     "ListUserPoolClientsResponseTypeDef",
     {
         "UserPoolClients": List[UserPoolClientDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredNotifyConfigurationTypeTypeDef = TypedDict(
     "_RequiredNotifyConfigurationTypeTypeDef",
     {
         "SourceArn": str,
@@ -3069,141 +3126,154 @@
     "UserPoolPolicyTypeTypeDef",
     {
         "PasswordPolicy": PasswordPolicyTypeTypeDef,
     },
     total=False,
 )
 
+RiskExceptionConfigurationTypeUnionTypeDef = Union[
+    RiskExceptionConfigurationTypeTypeDef, RiskExceptionConfigurationTypeOutputTypeDef
+]
 SchemaAttributeTypeTypeDef = TypedDict(
     "SchemaAttributeTypeTypeDef",
     {
         "Name": str,
         "AttributeDataType": AttributeDataTypeType,
         "DeveloperOnlyAttribute": bool,
         "Mutable": bool,
         "Required": bool,
         "NumberAttributeConstraints": NumberAttributeConstraintsTypeTypeDef,
         "StringAttributeConstraints": StringAttributeConstraintsTypeTypeDef,
     },
     total=False,
 )
 
+UserAttributeUpdateSettingsTypeUnionTypeDef = Union[
+    UserAttributeUpdateSettingsTypeTypeDef, UserAttributeUpdateSettingsTypeOutputTypeDef
+]
+AccountRecoverySettingTypeUnionTypeDef = Union[
+    AccountRecoverySettingTypeTypeDef, AccountRecoverySettingTypeOutputTypeDef
+]
 AdminGetDeviceResponseTypeDef = TypedDict(
     "AdminGetDeviceResponseTypeDef",
     {
         "Device": DeviceTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AdminListDevicesResponseTypeDef = TypedDict(
     "AdminListDevicesResponseTypeDef",
     {
         "Devices": List[DeviceTypeTypeDef],
         "PaginationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeviceResponseTypeDef = TypedDict(
     "GetDeviceResponseTypeDef",
     {
         "Device": DeviceTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDevicesResponseTypeDef = TypedDict(
     "ListDevicesResponseTypeDef",
     {
         "Devices": List[DeviceTypeTypeDef],
         "PaginationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AdminCreateUserResponseTypeDef = TypedDict(
     "AdminCreateUserResponseTypeDef",
     {
         "User": UserTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsersInGroupResponseTypeDef = TypedDict(
     "ListUsersInGroupResponseTypeDef",
     {
         "Users": List[UserTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "Users": List[UserTypeTypeDef],
         "PaginationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AdminListUserAuthEventsResponseTypeDef = TypedDict(
     "AdminListUserAuthEventsResponseTypeDef",
     {
         "AuthEvents": List[AuthEventTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AdminInitiateAuthResponseTypeDef = TypedDict(
     "AdminInitiateAuthResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
         "AuthenticationResult": AuthenticationResultTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AdminRespondToAuthChallengeResponseTypeDef = TypedDict(
     "AdminRespondToAuthChallengeResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
         "AuthenticationResult": AuthenticationResultTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InitiateAuthResponseTypeDef = TypedDict(
     "InitiateAuthResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
         "AuthenticationResult": AuthenticationResultTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RespondToAuthChallengeResponseTypeDef = TypedDict(
     "RespondToAuthChallengeResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
         "AuthenticationResult": AuthenticationResultTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CompromisedCredentialsRiskConfigurationTypeUnionTypeDef = Union[
+    CompromisedCredentialsRiskConfigurationTypeTypeDef,
+    CompromisedCredentialsRiskConfigurationTypeOutputTypeDef,
+]
 _RequiredAdminInitiateAuthRequestRequestTypeDef = TypedDict(
     "_RequiredAdminInitiateAuthRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "ClientId": str,
         "AuthFlow": AuthFlowTypeType,
     },
@@ -3254,82 +3324,82 @@
     pass
 
 
 CreateResourceServerResponseTypeDef = TypedDict(
     "CreateResourceServerResponseTypeDef",
     {
         "ResourceServer": ResourceServerTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeResourceServerResponseTypeDef = TypedDict(
     "DescribeResourceServerResponseTypeDef",
     {
         "ResourceServer": ResourceServerTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceServersResponseTypeDef = TypedDict(
     "ListResourceServersResponseTypeDef",
     {
         "ResourceServers": List[ResourceServerTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResourceServerResponseTypeDef = TypedDict(
     "UpdateResourceServerResponseTypeDef",
     {
         "ResourceServer": ResourceServerTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateUserPoolClientResponseTypeDef = TypedDict(
     "CreateUserPoolClientResponseTypeDef",
     {
         "UserPoolClient": UserPoolClientTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUserPoolClientResponseTypeDef = TypedDict(
     "DescribeUserPoolClientResponseTypeDef",
     {
         "UserPoolClient": UserPoolClientTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUserPoolClientResponseTypeDef = TypedDict(
     "UpdateUserPoolClientResponseTypeDef",
     {
         "UserPoolClient": UserPoolClientTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUserPoolDomainResponseTypeDef = TypedDict(
     "DescribeUserPoolDomainResponseTypeDef",
     {
         "DomainDescription": DomainDescriptionTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserPoolMfaConfigResponseTypeDef = TypedDict(
     "GetUserPoolMfaConfigResponseTypeDef",
     {
         "SmsMfaConfiguration": SmsMfaConfigTypeTypeDef,
         "SoftwareTokenMfaConfiguration": SoftwareTokenMfaConfigTypeTypeDef,
         "MfaConfiguration": UserPoolMfaTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSetUserPoolMfaConfigRequestRequestTypeDef = TypedDict(
     "_RequiredSetUserPoolMfaConfigRequestRequestTypeDef",
     {
         "UserPoolId": str,
@@ -3355,15 +3425,15 @@
 
 SetUserPoolMfaConfigResponseTypeDef = TypedDict(
     "SetUserPoolMfaConfigResponseTypeDef",
     {
         "SmsMfaConfiguration": SmsMfaConfigTypeTypeDef,
         "SoftwareTokenMfaConfiguration": SoftwareTokenMfaConfigTypeTypeDef,
         "MfaConfiguration": UserPoolMfaTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UserPoolDescriptionTypeTypeDef = TypedDict(
     "UserPoolDescriptionTypeTypeDef",
     {
         "Id": str,
@@ -3502,53 +3572,53 @@
         "AliasAttributes": List[AliasAttributeTypeType],
         "UsernameAttributes": List[UsernameAttributeTypeType],
         "SmsVerificationMessage": str,
         "EmailVerificationMessage": str,
         "EmailVerificationSubject": str,
         "VerificationMessageTemplate": VerificationMessageTemplateTypeTypeDef,
         "SmsAuthenticationMessage": str,
-        "UserAttributeUpdateSettings": UserAttributeUpdateSettingsTypeTypeDef,
+        "UserAttributeUpdateSettings": UserAttributeUpdateSettingsTypeOutputTypeDef,
         "MfaConfiguration": UserPoolMfaTypeType,
         "DeviceConfiguration": DeviceConfigurationTypeTypeDef,
         "EstimatedNumberOfUsers": int,
         "EmailConfiguration": EmailConfigurationTypeTypeDef,
         "SmsConfiguration": SmsConfigurationTypeTypeDef,
         "UserPoolTags": Dict[str, str],
         "SmsConfigurationFailure": str,
         "EmailConfigurationFailure": str,
         "Domain": str,
         "CustomDomain": str,
         "AdminCreateUserConfig": AdminCreateUserConfigTypeTypeDef,
         "UserPoolAddOns": UserPoolAddOnsTypeTypeDef,
         "UsernameConfiguration": UsernameConfigurationTypeTypeDef,
         "Arn": str,
-        "AccountRecoverySetting": AccountRecoverySettingTypeTypeDef,
+        "AccountRecoverySetting": AccountRecoverySettingTypeOutputTypeDef,
     },
     total=False,
 )
 
 ListUserPoolsResponseTypeDef = TypedDict(
     "ListUserPoolsResponseTypeDef",
     {
         "UserPools": List[UserPoolDescriptionTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RiskConfigurationTypeTypeDef = TypedDict(
     "RiskConfigurationTypeTypeDef",
     {
         "UserPoolId": str,
         "ClientId": str,
         "CompromisedCredentialsRiskConfiguration": (
-            CompromisedCredentialsRiskConfigurationTypeTypeDef
+            CompromisedCredentialsRiskConfigurationTypeOutputTypeDef
         ),
         "AccountTakeoverRiskConfiguration": AccountTakeoverRiskConfigurationTypeTypeDef,
-        "RiskExceptionConfiguration": RiskExceptionConfigurationTypeTypeDef,
+        "RiskExceptionConfiguration": RiskExceptionConfigurationTypeOutputTypeDef,
         "LastModifiedDate": datetime,
     },
     total=False,
 )
 
 _RequiredSetRiskConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredSetRiskConfigurationRequestRequestTypeDef",
@@ -3577,34 +3647,34 @@
     pass
 
 
 CreateUserPoolResponseTypeDef = TypedDict(
     "CreateUserPoolResponseTypeDef",
     {
         "UserPool": UserPoolTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUserPoolResponseTypeDef = TypedDict(
     "DescribeUserPoolResponseTypeDef",
     {
         "UserPool": UserPoolTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRiskConfigurationResponseTypeDef = TypedDict(
     "DescribeRiskConfigurationResponseTypeDef",
     {
         "RiskConfiguration": RiskConfigurationTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SetRiskConfigurationResponseTypeDef = TypedDict(
     "SetRiskConfigurationResponseTypeDef",
     {
         "RiskConfiguration": RiskConfigurationTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp/type_defs.pyi` & `types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_cognito_idp.type_defs import RecoveryOptionTypeTypeDef
 
-    data: RecoveryOptionTypeTypeDef = {...}
+    data: RecoveryOptionTypeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -67,62 +67,60 @@
 __all__ = (
     "RecoveryOptionTypeTypeDef",
     "AccountTakeoverActionTypeTypeDef",
     "AdminAddUserToGroupRequestRequestTypeDef",
     "AdminConfirmSignUpRequestRequestTypeDef",
     "MessageTemplateTypeTypeDef",
     "AttributeTypeTypeDef",
+    "ResponseMetadataTypeDef",
     "AdminDeleteUserAttributesRequestRequestTypeDef",
     "AdminDeleteUserRequestRequestTypeDef",
     "ProviderUserIdentifierTypeTypeDef",
     "AdminDisableUserRequestRequestTypeDef",
     "AdminEnableUserRequestRequestTypeDef",
     "AdminForgetDeviceRequestRequestTypeDef",
     "AdminGetDeviceRequestRequestTypeDef",
     "AdminGetUserRequestRequestTypeDef",
     "MFAOptionTypeTypeDef",
     "AnalyticsMetadataTypeTypeDef",
     "AdminListDevicesRequestRequestTypeDef",
-    "AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "AdminListGroupsForUserRequestRequestTypeDef",
     "GroupTypeTypeDef",
-    "AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
     "AdminListUserAuthEventsRequestRequestTypeDef",
     "AdminRemoveUserFromGroupRequestRequestTypeDef",
     "AdminResetUserPasswordRequestRequestTypeDef",
     "SMSMfaSettingsTypeTypeDef",
     "SoftwareTokenMfaSettingsTypeTypeDef",
     "AdminSetUserPasswordRequestRequestTypeDef",
     "AdminUpdateAuthEventFeedbackRequestRequestTypeDef",
     "AdminUpdateDeviceStatusRequestRequestTypeDef",
     "AdminUserGlobalSignOutRequestRequestTypeDef",
     "AnalyticsConfigurationTypeTypeDef",
     "AssociateSoftwareTokenRequestRequestTypeDef",
-    "AssociateSoftwareTokenResponseTypeDef",
     "ChallengeResponseTypeTypeDef",
     "EventContextDataTypeTypeDef",
     "EventFeedbackTypeTypeDef",
     "EventRiskTypeTypeDef",
     "NewDeviceMetadataTypeTypeDef",
+    "BlobTypeDef",
     "ChangePasswordRequestRequestTypeDef",
     "CodeDeliveryDetailsTypeTypeDef",
     "CompromisedCredentialsActionsTypeTypeDef",
     "DeviceSecretVerifierConfigTypeTypeDef",
-    "ConfirmDeviceResponseTypeDef",
     "UserContextDataTypeTypeDef",
     "HttpHeaderTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "CreateIdentityProviderRequestRequestTypeDef",
     "IdentityProviderTypeTypeDef",
     "ResourceServerScopeTypeTypeDef",
     "CreateUserImportJobRequestRequestTypeDef",
     "UserImportJobTypeTypeDef",
     "TokenValidityUnitsTypeTypeDef",
     "CustomDomainConfigTypeTypeDef",
-    "CreateUserPoolDomainResponseTypeDef",
     "DeviceConfigurationTypeTypeDef",
     "EmailConfigurationTypeTypeDef",
     "SmsConfigurationTypeTypeDef",
     "UserAttributeUpdateSettingsTypeTypeDef",
     "UserPoolAddOnsTypeTypeDef",
     "UsernameConfigurationTypeTypeDef",
     "VerificationMessageTemplateTypeTypeDef",
@@ -139,99 +137,106 @@
     "DescribeIdentityProviderRequestRequestTypeDef",
     "DescribeResourceServerRequestRequestTypeDef",
     "DescribeRiskConfigurationRequestRequestTypeDef",
     "DescribeUserImportJobRequestRequestTypeDef",
     "DescribeUserPoolClientRequestRequestTypeDef",
     "DescribeUserPoolDomainRequestRequestTypeDef",
     "DescribeUserPoolRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ForgetDeviceRequestRequestTypeDef",
     "GetCSVHeaderRequestRequestTypeDef",
-    "GetCSVHeaderResponseTypeDef",
     "GetDeviceRequestRequestTypeDef",
     "GetGroupRequestRequestTypeDef",
     "GetIdentityProviderByIdentifierRequestRequestTypeDef",
     "GetSigningCertificateRequestRequestTypeDef",
-    "GetSigningCertificateResponseTypeDef",
     "GetUICustomizationRequestRequestTypeDef",
     "UICustomizationTypeTypeDef",
     "GetUserAttributeVerificationCodeRequestRequestTypeDef",
     "GetUserPoolMfaConfigRequestRequestTypeDef",
     "SoftwareTokenMfaConfigTypeTypeDef",
     "GetUserRequestRequestTypeDef",
     "GlobalSignOutRequestRequestTypeDef",
     "ListDevicesRequestRequestTypeDef",
-    "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListGroupsRequestRequestTypeDef",
-    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
     "ListIdentityProvidersRequestRequestTypeDef",
     "ProviderDescriptionTypeDef",
-    "ListResourceServersRequestListResourceServersPaginateTypeDef",
     "ListResourceServersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListUserImportJobsRequestRequestTypeDef",
-    "ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
     "ListUserPoolClientsRequestRequestTypeDef",
     "UserPoolClientDescriptionTypeDef",
-    "ListUserPoolsRequestListUserPoolsPaginateTypeDef",
     "ListUserPoolsRequestRequestTypeDef",
-    "ListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
     "ListUsersInGroupRequestRequestTypeDef",
-    "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
     "NotifyEmailTypeTypeDef",
     "NumberAttributeConstraintsTypeTypeDef",
-    "PaginatorConfigTypeDef",
     "PasswordPolicyTypeTypeDef",
-    "ResponseMetadataTypeDef",
     "RevokeTokenRequestRequestTypeDef",
+    "RiskExceptionConfigurationTypeOutputTypeDef",
     "RiskExceptionConfigurationTypeTypeDef",
     "StringAttributeConstraintsTypeTypeDef",
-    "SetUICustomizationRequestRequestTypeDef",
     "StartUserImportJobRequestRequestTypeDef",
     "StopUserImportJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAuthEventFeedbackRequestRequestTypeDef",
     "UpdateDeviceStatusRequestRequestTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "UpdateIdentityProviderRequestRequestTypeDef",
-    "UpdateUserPoolDomainResponseTypeDef",
+    "UserAttributeUpdateSettingsTypeOutputTypeDef",
     "VerifySoftwareTokenRequestRequestTypeDef",
-    "VerifySoftwareTokenResponseTypeDef",
     "VerifyUserAttributeRequestRequestTypeDef",
+    "AccountRecoverySettingTypeOutputTypeDef",
     "AccountRecoverySettingTypeTypeDef",
     "AccountTakeoverActionsTypeTypeDef",
     "AdminCreateUserConfigTypeTypeDef",
     "AdminCreateUserRequestRequestTypeDef",
     "AdminUpdateUserAttributesRequestRequestTypeDef",
     "DeviceTypeTypeDef",
     "UpdateUserAttributesRequestRequestTypeDef",
+    "AssociateSoftwareTokenResponseTypeDef",
+    "ConfirmDeviceResponseTypeDef",
+    "CreateUserPoolDomainResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetCSVHeaderResponseTypeDef",
+    "GetSigningCertificateResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateUserPoolDomainResponseTypeDef",
+    "VerifySoftwareTokenResponseTypeDef",
     "AdminDisableProviderForUserRequestRequestTypeDef",
     "AdminLinkProviderForUserRequestRequestTypeDef",
     "AdminGetUserResponseTypeDef",
     "AdminSetUserSettingsRequestRequestTypeDef",
     "GetUserResponseTypeDef",
     "SetUserSettingsRequestRequestTypeDef",
     "UserTypeTypeDef",
+    "AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
+    "AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
+    "ListGroupsRequestListGroupsPaginateTypeDef",
+    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
+    "ListResourceServersRequestListResourceServersPaginateTypeDef",
+    "ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
+    "ListUserPoolsRequestListUserPoolsPaginateTypeDef",
+    "ListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
     "AdminListGroupsForUserResponseTypeDef",
     "CreateGroupResponseTypeDef",
     "GetGroupResponseTypeDef",
     "ListGroupsResponseTypeDef",
     "UpdateGroupResponseTypeDef",
     "AdminSetUserMFAPreferenceRequestRequestTypeDef",
     "SetUserMFAPreferenceRequestRequestTypeDef",
     "AuthEventTypeTypeDef",
     "AuthenticationResultTypeTypeDef",
+    "SetUICustomizationRequestRequestTypeDef",
     "ForgotPasswordResponseTypeDef",
     "GetUserAttributeVerificationCodeResponseTypeDef",
     "ResendConfirmationCodeResponseTypeDef",
     "SignUpResponseTypeDef",
     "UpdateUserAttributesResponseTypeDef",
+    "CompromisedCredentialsRiskConfigurationTypeOutputTypeDef",
     "CompromisedCredentialsRiskConfigurationTypeTypeDef",
     "ConfirmDeviceRequestRequestTypeDef",
     "ConfirmForgotPasswordRequestRequestTypeDef",
     "ConfirmSignUpRequestRequestTypeDef",
     "ForgotPasswordRequestRequestTypeDef",
     "InitiateAuthRequestRequestTypeDef",
     "ResendConfirmationCodeRequestRequestTypeDef",
@@ -260,27 +265,31 @@
     "LambdaConfigTypeTypeDef",
     "GetUICustomizationResponseTypeDef",
     "SetUICustomizationResponseTypeDef",
     "ListIdentityProvidersResponseTypeDef",
     "ListUserPoolClientsResponseTypeDef",
     "NotifyConfigurationTypeTypeDef",
     "UserPoolPolicyTypeTypeDef",
+    "RiskExceptionConfigurationTypeUnionTypeDef",
     "SchemaAttributeTypeTypeDef",
+    "UserAttributeUpdateSettingsTypeUnionTypeDef",
+    "AccountRecoverySettingTypeUnionTypeDef",
     "AdminGetDeviceResponseTypeDef",
     "AdminListDevicesResponseTypeDef",
     "GetDeviceResponseTypeDef",
     "ListDevicesResponseTypeDef",
     "AdminCreateUserResponseTypeDef",
     "ListUsersInGroupResponseTypeDef",
     "ListUsersResponseTypeDef",
     "AdminListUserAuthEventsResponseTypeDef",
     "AdminInitiateAuthResponseTypeDef",
     "AdminRespondToAuthChallengeResponseTypeDef",
     "InitiateAuthResponseTypeDef",
     "RespondToAuthChallengeResponseTypeDef",
+    "CompromisedCredentialsRiskConfigurationTypeUnionTypeDef",
     "AdminInitiateAuthRequestRequestTypeDef",
     "AdminRespondToAuthChallengeRequestRequestTypeDef",
     "CreateResourceServerResponseTypeDef",
     "DescribeResourceServerResponseTypeDef",
     "ListResourceServersResponseTypeDef",
     "UpdateResourceServerResponseTypeDef",
     "CreateUserPoolClientResponseTypeDef",
@@ -374,14 +383,25 @@
     },
     total=False,
 )
 
 class AttributeTypeTypeDef(_RequiredAttributeTypeTypeDef, _OptionalAttributeTypeTypeDef):
     pass
 
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
 AdminDeleteUserAttributesRequestRequestTypeDef = TypedDict(
     "AdminDeleteUserAttributesRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Username": str,
         "UserAttributeNames": Sequence[str],
     },
@@ -481,35 +501,24 @@
 )
 
 class AdminListDevicesRequestRequestTypeDef(
     _RequiredAdminListDevicesRequestRequestTypeDef, _OptionalAdminListDevicesRequestRequestTypeDef
 ):
     pass
 
-_RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef = TypedDict(
-    "_RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
-    {
-        "Username": str,
-        "UserPoolId": str,
-    },
-)
-_OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef = TypedDict(
-    "_OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
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
 
-class AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef(
-    _RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
-    _OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
-):
-    pass
-
 _RequiredAdminListGroupsForUserRequestRequestTypeDef = TypedDict(
     "_RequiredAdminListGroupsForUserRequestRequestTypeDef",
     {
         "Username": str,
         "UserPoolId": str,
     },
 )
@@ -538,35 +547,14 @@
         "Precedence": int,
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
     },
     total=False,
 )
 
-_RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef = TypedDict(
-    "_RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
-    {
-        "UserPoolId": str,
-        "Username": str,
-    },
-)
-_OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef = TypedDict(
-    "_OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef(
-    _RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
-    _OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
-):
-    pass
-
 _RequiredAdminListUserAuthEventsRequestRequestTypeDef = TypedDict(
     "_RequiredAdminListUserAuthEventsRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Username": str,
     },
 )
@@ -712,23 +700,14 @@
     {
         "AccessToken": str,
         "Session": str,
     },
     total=False,
 )
 
-AssociateSoftwareTokenResponseTypeDef = TypedDict(
-    "AssociateSoftwareTokenResponseTypeDef",
-    {
-        "SecretCode": str,
-        "Session": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ChallengeResponseTypeTypeDef = TypedDict(
     "ChallengeResponseTypeTypeDef",
     {
         "ChallengeName": ChallengeNameType,
         "ChallengeResponse": ChallengeResponseType,
     },
     total=False,
@@ -781,14 +760,15 @@
     {
         "DeviceKey": str,
         "DeviceGroupKey": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ChangePasswordRequestRequestTypeDef = TypedDict(
     "ChangePasswordRequestRequestTypeDef",
     {
         "PreviousPassword": str,
         "ProposedPassword": str,
         "AccessToken": str,
     },
@@ -816,22 +796,14 @@
     {
         "PasswordVerifier": str,
         "Salt": str,
     },
     total=False,
 )
 
-ConfirmDeviceResponseTypeDef = TypedDict(
-    "ConfirmDeviceResponseTypeDef",
-    {
-        "UserConfirmationNecessary": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UserContextDataTypeTypeDef = TypedDict(
     "UserContextDataTypeTypeDef",
     {
         "IpAddress": str,
         "EncodedData": str,
     },
     total=False,
@@ -957,22 +929,14 @@
 CustomDomainConfigTypeTypeDef = TypedDict(
     "CustomDomainConfigTypeTypeDef",
     {
         "CertificateArn": str,
     },
 )
 
-CreateUserPoolDomainResponseTypeDef = TypedDict(
-    "CreateUserPoolDomainResponseTypeDef",
-    {
-        "CloudFrontDomain": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeviceConfigurationTypeTypeDef = TypedDict(
     "DeviceConfigurationTypeTypeDef",
     {
         "ChallengeRequiredOnNewDevice": bool,
         "DeviceOnlyRememberedOnUserPrompt": bool,
     },
     total=False,
@@ -1185,21 +1149,14 @@
 DescribeUserPoolRequestRequestTypeDef = TypedDict(
     "DescribeUserPoolRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredForgetDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredForgetDeviceRequestRequestTypeDef",
     {
         "DeviceKey": str,
     },
 )
 _OptionalForgetDeviceRequestRequestTypeDef = TypedDict(
@@ -1218,23 +1175,14 @@
 GetCSVHeaderRequestRequestTypeDef = TypedDict(
     "GetCSVHeaderRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 
-GetCSVHeaderResponseTypeDef = TypedDict(
-    "GetCSVHeaderResponseTypeDef",
-    {
-        "UserPoolId": str,
-        "CSVHeader": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredGetDeviceRequestRequestTypeDef",
     {
         "DeviceKey": str,
     },
 )
 _OptionalGetDeviceRequestRequestTypeDef = TypedDict(
@@ -1269,22 +1217,14 @@
 GetSigningCertificateRequestRequestTypeDef = TypedDict(
     "GetSigningCertificateRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 
-GetSigningCertificateResponseTypeDef = TypedDict(
-    "GetSigningCertificateResponseTypeDef",
-    {
-        "Certificate": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetUICustomizationRequestRequestTypeDef = TypedDict(
     "_RequiredGetUICustomizationRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalGetUICustomizationRequestRequestTypeDef = TypedDict(
@@ -1381,34 +1321,14 @@
 )
 
 class ListDevicesRequestRequestTypeDef(
     _RequiredListDevicesRequestRequestTypeDef, _OptionalListDevicesRequestRequestTypeDef
 ):
     pass
 
-_RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListGroupsRequestListGroupsPaginateTypeDef(
-    _RequiredListGroupsRequestListGroupsPaginateTypeDef,
-    _OptionalListGroupsRequestListGroupsPaginateTypeDef,
-):
-    pass
-
 _RequiredListGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupsRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalListGroupsRequestRequestTypeDef = TypedDict(
@@ -1421,34 +1341,14 @@
 )
 
 class ListGroupsRequestRequestTypeDef(
     _RequiredListGroupsRequestRequestTypeDef, _OptionalListGroupsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
-    "_RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
-    "_OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef(
-    _RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
-    _OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
-):
-    pass
-
 _RequiredListIdentityProvidersRequestRequestTypeDef = TypedDict(
     "_RequiredListIdentityProvidersRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalListIdentityProvidersRequestRequestTypeDef = TypedDict(
@@ -1473,34 +1373,14 @@
         "ProviderType": IdentityProviderTypeTypeType,
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
     },
     total=False,
 )
 
-_RequiredListResourceServersRequestListResourceServersPaginateTypeDef = TypedDict(
-    "_RequiredListResourceServersRequestListResourceServersPaginateTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalListResourceServersRequestListResourceServersPaginateTypeDef = TypedDict(
-    "_OptionalListResourceServersRequestListResourceServersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListResourceServersRequestListResourceServersPaginateTypeDef(
-    _RequiredListResourceServersRequestListResourceServersPaginateTypeDef,
-    _OptionalListResourceServersRequestListResourceServersPaginateTypeDef,
-):
-    pass
-
 _RequiredListResourceServersRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceServersRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalListResourceServersRequestRequestTypeDef = TypedDict(
@@ -1521,22 +1401,14 @@
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
 _RequiredListUserImportJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListUserImportJobsRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "MaxResults": int,
     },
 )
@@ -1550,34 +1422,14 @@
 
 class ListUserImportJobsRequestRequestTypeDef(
     _RequiredListUserImportJobsRequestRequestTypeDef,
     _OptionalListUserImportJobsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef = TypedDict(
-    "_RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef = TypedDict(
-    "_OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef(
-    _RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
-    _OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
-):
-    pass
-
 _RequiredListUserPoolClientsRequestRequestTypeDef = TypedDict(
     "_RequiredListUserPoolClientsRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalListUserPoolClientsRequestRequestTypeDef = TypedDict(
@@ -1601,22 +1453,14 @@
         "ClientId": str,
         "UserPoolId": str,
         "ClientName": str,
     },
     total=False,
 )
 
-ListUserPoolsRequestListUserPoolsPaginateTypeDef = TypedDict(
-    "ListUserPoolsRequestListUserPoolsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 _RequiredListUserPoolsRequestRequestTypeDef = TypedDict(
     "_RequiredListUserPoolsRequestRequestTypeDef",
     {
         "MaxResults": int,
     },
 )
 _OptionalListUserPoolsRequestRequestTypeDef = TypedDict(
@@ -1628,35 +1472,14 @@
 )
 
 class ListUserPoolsRequestRequestTypeDef(
     _RequiredListUserPoolsRequestRequestTypeDef, _OptionalListUserPoolsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef = TypedDict(
-    "_RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
-    {
-        "UserPoolId": str,
-        "GroupName": str,
-    },
-)
-_OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef = TypedDict(
-    "_OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListUsersInGroupRequestListUsersInGroupPaginateTypeDef(
-    _RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
-    _OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
-):
-    pass
-
 _RequiredListUsersInGroupRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersInGroupRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "GroupName": str,
     },
 )
@@ -1670,36 +1493,14 @@
 )
 
 class ListUsersInGroupRequestRequestTypeDef(
     _RequiredListUsersInGroupRequestRequestTypeDef, _OptionalListUsersInGroupRequestRequestTypeDef
 ):
     pass
 
-_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_RequiredListUsersRequestListUsersPaginateTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_OptionalListUsersRequestListUsersPaginateTypeDef",
-    {
-        "AttributesToGet": Sequence[str],
-        "Filter": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListUsersRequestListUsersPaginateTypeDef(
-    _RequiredListUsersRequestListUsersPaginateTypeDef,
-    _OptionalListUsersRequestListUsersPaginateTypeDef,
-):
-    pass
-
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -1741,48 +1542,27 @@
     {
         "MinValue": str,
         "MaxValue": str,
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
 PasswordPolicyTypeTypeDef = TypedDict(
     "PasswordPolicyTypeTypeDef",
     {
         "MinimumLength": int,
         "RequireUppercase": bool,
         "RequireLowercase": bool,
         "RequireNumbers": bool,
         "RequireSymbols": bool,
         "TemporaryPasswordValidityDays": int,
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
 _RequiredRevokeTokenRequestRequestTypeDef = TypedDict(
     "_RequiredRevokeTokenRequestRequestTypeDef",
     {
         "Token": str,
         "ClientId": str,
     },
 )
@@ -1795,54 +1575,41 @@
 )
 
 class RevokeTokenRequestRequestTypeDef(
     _RequiredRevokeTokenRequestRequestTypeDef, _OptionalRevokeTokenRequestRequestTypeDef
 ):
     pass
 
-RiskExceptionConfigurationTypeTypeDef = TypedDict(
-    "RiskExceptionConfigurationTypeTypeDef",
+RiskExceptionConfigurationTypeOutputTypeDef = TypedDict(
+    "RiskExceptionConfigurationTypeOutputTypeDef",
     {
         "BlockedIPRangeList": List[str],
         "SkippedIPRangeList": List[str],
     },
     total=False,
 )
 
-StringAttributeConstraintsTypeTypeDef = TypedDict(
-    "StringAttributeConstraintsTypeTypeDef",
+RiskExceptionConfigurationTypeTypeDef = TypedDict(
+    "RiskExceptionConfigurationTypeTypeDef",
     {
-        "MinLength": str,
-        "MaxLength": str,
+        "BlockedIPRangeList": Sequence[str],
+        "SkippedIPRangeList": Sequence[str],
     },
     total=False,
 )
 
-_RequiredSetUICustomizationRequestRequestTypeDef = TypedDict(
-    "_RequiredSetUICustomizationRequestRequestTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalSetUICustomizationRequestRequestTypeDef = TypedDict(
-    "_OptionalSetUICustomizationRequestRequestTypeDef",
+StringAttributeConstraintsTypeTypeDef = TypedDict(
+    "StringAttributeConstraintsTypeTypeDef",
     {
-        "ClientId": str,
-        "CSS": str,
-        "ImageFile": Union[str, bytes, IO[Any], StreamingBody],
+        "MinLength": str,
+        "MaxLength": str,
     },
     total=False,
 )
 
-class SetUICustomizationRequestRequestTypeDef(
-    _RequiredSetUICustomizationRequestRequestTypeDef,
-    _OptionalSetUICustomizationRequestRequestTypeDef,
-):
-    pass
-
 StartUserImportJobRequestRequestTypeDef = TypedDict(
     "StartUserImportJobRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "JobId": str,
     },
 )
@@ -1944,20 +1711,20 @@
 
 class UpdateIdentityProviderRequestRequestTypeDef(
     _RequiredUpdateIdentityProviderRequestRequestTypeDef,
     _OptionalUpdateIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
-UpdateUserPoolDomainResponseTypeDef = TypedDict(
-    "UpdateUserPoolDomainResponseTypeDef",
+UserAttributeUpdateSettingsTypeOutputTypeDef = TypedDict(
+    "UserAttributeUpdateSettingsTypeOutputTypeDef",
     {
-        "CloudFrontDomain": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AttributesRequireVerificationBeforeUpdate": List[VerifiedAttributeTypeType],
     },
+    total=False,
 )
 
 _RequiredVerifySoftwareTokenRequestRequestTypeDef = TypedDict(
     "_RequiredVerifySoftwareTokenRequestRequestTypeDef",
     {
         "UserCode": str,
     },
@@ -1974,32 +1741,31 @@
 
 class VerifySoftwareTokenRequestRequestTypeDef(
     _RequiredVerifySoftwareTokenRequestRequestTypeDef,
     _OptionalVerifySoftwareTokenRequestRequestTypeDef,
 ):
     pass
 
-VerifySoftwareTokenResponseTypeDef = TypedDict(
-    "VerifySoftwareTokenResponseTypeDef",
-    {
-        "Status": VerifySoftwareTokenResponseTypeType,
-        "Session": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VerifyUserAttributeRequestRequestTypeDef = TypedDict(
     "VerifyUserAttributeRequestRequestTypeDef",
     {
         "AccessToken": str,
         "AttributeName": str,
         "Code": str,
     },
 )
 
+AccountRecoverySettingTypeOutputTypeDef = TypedDict(
+    "AccountRecoverySettingTypeOutputTypeDef",
+    {
+        "RecoveryMechanisms": List[RecoveryOptionTypeTypeDef],
+    },
+    total=False,
+)
+
 AccountRecoverySettingTypeTypeDef = TypedDict(
     "AccountRecoverySettingTypeTypeDef",
     {
         "RecoveryMechanisms": Sequence[RecoveryOptionTypeTypeDef],
     },
     total=False,
 )
@@ -2101,14 +1867,88 @@
 
 class UpdateUserAttributesRequestRequestTypeDef(
     _RequiredUpdateUserAttributesRequestRequestTypeDef,
     _OptionalUpdateUserAttributesRequestRequestTypeDef,
 ):
     pass
 
+AssociateSoftwareTokenResponseTypeDef = TypedDict(
+    "AssociateSoftwareTokenResponseTypeDef",
+    {
+        "SecretCode": str,
+        "Session": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConfirmDeviceResponseTypeDef = TypedDict(
+    "ConfirmDeviceResponseTypeDef",
+    {
+        "UserConfirmationNecessary": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUserPoolDomainResponseTypeDef = TypedDict(
+    "CreateUserPoolDomainResponseTypeDef",
+    {
+        "CloudFrontDomain": str,
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
+GetCSVHeaderResponseTypeDef = TypedDict(
+    "GetCSVHeaderResponseTypeDef",
+    {
+        "UserPoolId": str,
+        "CSVHeader": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSigningCertificateResponseTypeDef = TypedDict(
+    "GetSigningCertificateResponseTypeDef",
+    {
+        "Certificate": str,
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
+UpdateUserPoolDomainResponseTypeDef = TypedDict(
+    "UpdateUserPoolDomainResponseTypeDef",
+    {
+        "CloudFrontDomain": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VerifySoftwareTokenResponseTypeDef = TypedDict(
+    "VerifySoftwareTokenResponseTypeDef",
+    {
+        "Status": VerifySoftwareTokenResponseTypeType,
+        "Session": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AdminDisableProviderForUserRequestRequestTypeDef = TypedDict(
     "AdminDisableProviderForUserRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "User": ProviderUserIdentifierTypeTypeDef,
     },
 )
@@ -2130,15 +1970,15 @@
         "UserCreateDate": datetime,
         "UserLastModifiedDate": datetime,
         "Enabled": bool,
         "UserStatus": UserStatusTypeType,
         "MFAOptions": List[MFAOptionTypeTypeDef],
         "PreferredMfaSetting": str,
         "UserMFASettingList": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AdminSetUserSettingsRequestRequestTypeDef = TypedDict(
     "AdminSetUserSettingsRequestRequestTypeDef",
     {
         "UserPoolId": str,
@@ -2151,15 +1991,15 @@
     "GetUserResponseTypeDef",
     {
         "Username": str,
         "UserAttributes": List[AttributeTypeTypeDef],
         "MFAOptions": List[MFAOptionTypeTypeDef],
         "PreferredMfaSetting": str,
         "UserMFASettingList": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SetUserSettingsRequestRequestTypeDef = TypedDict(
     "SetUserSettingsRequestRequestTypeDef",
     {
         "AccessToken": str,
@@ -2177,53 +2017,226 @@
         "Enabled": bool,
         "UserStatus": UserStatusTypeType,
         "MFAOptions": List[MFAOptionTypeTypeDef],
     },
     total=False,
 )
 
+_RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef = TypedDict(
+    "_RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
+    {
+        "Username": str,
+        "UserPoolId": str,
+    },
+)
+_OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef = TypedDict(
+    "_OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef(
+    _RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
+    _OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
+):
+    pass
+
+_RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef = TypedDict(
+    "_RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
+    {
+        "UserPoolId": str,
+        "Username": str,
+    },
+)
+_OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef = TypedDict(
+    "_OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef(
+    _RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
+    _OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
+):
+    pass
+
+_RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListGroupsRequestListGroupsPaginateTypeDef(
+    _RequiredListGroupsRequestListGroupsPaginateTypeDef,
+    _OptionalListGroupsRequestListGroupsPaginateTypeDef,
+):
+    pass
+
+_RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
+    "_RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
+    "_OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef(
+    _RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
+    _OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
+):
+    pass
+
+_RequiredListResourceServersRequestListResourceServersPaginateTypeDef = TypedDict(
+    "_RequiredListResourceServersRequestListResourceServersPaginateTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalListResourceServersRequestListResourceServersPaginateTypeDef = TypedDict(
+    "_OptionalListResourceServersRequestListResourceServersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListResourceServersRequestListResourceServersPaginateTypeDef(
+    _RequiredListResourceServersRequestListResourceServersPaginateTypeDef,
+    _OptionalListResourceServersRequestListResourceServersPaginateTypeDef,
+):
+    pass
+
+_RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef = TypedDict(
+    "_RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef = TypedDict(
+    "_OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef(
+    _RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
+    _OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
+):
+    pass
+
+ListUserPoolsRequestListUserPoolsPaginateTypeDef = TypedDict(
+    "ListUserPoolsRequestListUserPoolsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef = TypedDict(
+    "_RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
+    {
+        "UserPoolId": str,
+        "GroupName": str,
+    },
+)
+_OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef = TypedDict(
+    "_OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListUsersInGroupRequestListUsersInGroupPaginateTypeDef(
+    _RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
+    _OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
+):
+    pass
+
+_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_RequiredListUsersRequestListUsersPaginateTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_OptionalListUsersRequestListUsersPaginateTypeDef",
+    {
+        "AttributesToGet": Sequence[str],
+        "Filter": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListUsersRequestListUsersPaginateTypeDef(
+    _RequiredListUsersRequestListUsersPaginateTypeDef,
+    _OptionalListUsersRequestListUsersPaginateTypeDef,
+):
+    pass
+
 AdminListGroupsForUserResponseTypeDef = TypedDict(
     "AdminListGroupsForUserResponseTypeDef",
     {
         "Groups": List[GroupTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateGroupResponseTypeDef = TypedDict(
     "CreateGroupResponseTypeDef",
     {
         "Group": GroupTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGroupResponseTypeDef = TypedDict(
     "GetGroupResponseTypeDef",
     {
         "Group": GroupTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGroupsResponseTypeDef = TypedDict(
     "ListGroupsResponseTypeDef",
     {
         "Groups": List[GroupTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGroupResponseTypeDef = TypedDict(
     "UpdateGroupResponseTypeDef",
     {
         "Group": GroupTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAdminSetUserMFAPreferenceRequestRequestTypeDef = TypedDict(
     "_RequiredAdminSetUserMFAPreferenceRequestRequestTypeDef",
     {
         "Username": str,
@@ -2290,66 +2303,108 @@
         "RefreshToken": str,
         "IdToken": str,
         "NewDeviceMetadata": NewDeviceMetadataTypeTypeDef,
     },
     total=False,
 )
 
+_RequiredSetUICustomizationRequestRequestTypeDef = TypedDict(
+    "_RequiredSetUICustomizationRequestRequestTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalSetUICustomizationRequestRequestTypeDef = TypedDict(
+    "_OptionalSetUICustomizationRequestRequestTypeDef",
+    {
+        "ClientId": str,
+        "CSS": str,
+        "ImageFile": BlobTypeDef,
+    },
+    total=False,
+)
+
+class SetUICustomizationRequestRequestTypeDef(
+    _RequiredSetUICustomizationRequestRequestTypeDef,
+    _OptionalSetUICustomizationRequestRequestTypeDef,
+):
+    pass
+
 ForgotPasswordResponseTypeDef = TypedDict(
     "ForgotPasswordResponseTypeDef",
     {
         "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserAttributeVerificationCodeResponseTypeDef = TypedDict(
     "GetUserAttributeVerificationCodeResponseTypeDef",
     {
         "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResendConfirmationCodeResponseTypeDef = TypedDict(
     "ResendConfirmationCodeResponseTypeDef",
     {
         "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SignUpResponseTypeDef = TypedDict(
     "SignUpResponseTypeDef",
     {
         "UserConfirmed": bool,
         "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
         "UserSub": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUserAttributesResponseTypeDef = TypedDict(
     "UpdateUserAttributesResponseTypeDef",
     {
         "CodeDeliveryDetailsList": List[CodeDeliveryDetailsTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCompromisedCredentialsRiskConfigurationTypeOutputTypeDef = TypedDict(
+    "_RequiredCompromisedCredentialsRiskConfigurationTypeOutputTypeDef",
+    {
+        "Actions": CompromisedCredentialsActionsTypeTypeDef,
+    },
+)
+_OptionalCompromisedCredentialsRiskConfigurationTypeOutputTypeDef = TypedDict(
+    "_OptionalCompromisedCredentialsRiskConfigurationTypeOutputTypeDef",
+    {
+        "EventFilter": List[EventFilterTypeType],
+    },
+    total=False,
+)
+
+class CompromisedCredentialsRiskConfigurationTypeOutputTypeDef(
+    _RequiredCompromisedCredentialsRiskConfigurationTypeOutputTypeDef,
+    _OptionalCompromisedCredentialsRiskConfigurationTypeOutputTypeDef,
+):
+    pass
+
 _RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef = TypedDict(
     "_RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef",
     {
         "Actions": CompromisedCredentialsActionsTypeTypeDef,
     },
 )
 _OptionalCompromisedCredentialsRiskConfigurationTypeTypeDef = TypedDict(
     "_OptionalCompromisedCredentialsRiskConfigurationTypeTypeDef",
     {
-        "EventFilter": List[EventFilterTypeType],
+        "EventFilter": Sequence[EventFilterTypeType],
     },
     total=False,
 )
 
 class CompromisedCredentialsRiskConfigurationTypeTypeDef(
     _RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef,
     _OptionalCompromisedCredentialsRiskConfigurationTypeTypeDef,
@@ -2569,39 +2624,39 @@
 class ContextDataTypeTypeDef(_RequiredContextDataTypeTypeDef, _OptionalContextDataTypeTypeDef):
     pass
 
 CreateIdentityProviderResponseTypeDef = TypedDict(
     "CreateIdentityProviderResponseTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeIdentityProviderResponseTypeDef = TypedDict(
     "DescribeIdentityProviderResponseTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIdentityProviderByIdentifierResponseTypeDef = TypedDict(
     "GetIdentityProviderByIdentifierResponseTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateIdentityProviderResponseTypeDef = TypedDict(
     "UpdateIdentityProviderResponseTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateResourceServerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResourceServerRequestRequestTypeDef",
     {
         "UserPoolId": str,
@@ -2656,48 +2711,48 @@
 ):
     pass
 
 CreateUserImportJobResponseTypeDef = TypedDict(
     "CreateUserImportJobResponseTypeDef",
     {
         "UserImportJob": UserImportJobTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUserImportJobResponseTypeDef = TypedDict(
     "DescribeUserImportJobResponseTypeDef",
     {
         "UserImportJob": UserImportJobTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUserImportJobsResponseTypeDef = TypedDict(
     "ListUserImportJobsResponseTypeDef",
     {
         "UserImportJobs": List[UserImportJobTypeTypeDef],
         "PaginationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartUserImportJobResponseTypeDef = TypedDict(
     "StartUserImportJobResponseTypeDef",
     {
         "UserImportJob": UserImportJobTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopUserImportJobResponseTypeDef = TypedDict(
     "StopUserImportJobResponseTypeDef",
     {
         "UserImportJob": UserImportJobTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateUserPoolClientRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserPoolClientRequestRequestTypeDef",
     {
         "UserPoolId": str,
@@ -2883,41 +2938,41 @@
     total=False,
 )
 
 GetUICustomizationResponseTypeDef = TypedDict(
     "GetUICustomizationResponseTypeDef",
     {
         "UICustomization": UICustomizationTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SetUICustomizationResponseTypeDef = TypedDict(
     "SetUICustomizationResponseTypeDef",
     {
         "UICustomization": UICustomizationTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIdentityProvidersResponseTypeDef = TypedDict(
     "ListIdentityProvidersResponseTypeDef",
     {
         "Providers": List[ProviderDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUserPoolClientsResponseTypeDef = TypedDict(
     "ListUserPoolClientsResponseTypeDef",
     {
         "UserPoolClients": List[UserPoolClientDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredNotifyConfigurationTypeTypeDef = TypedDict(
     "_RequiredNotifyConfigurationTypeTypeDef",
     {
         "SourceArn": str,
@@ -2944,141 +2999,154 @@
     "UserPoolPolicyTypeTypeDef",
     {
         "PasswordPolicy": PasswordPolicyTypeTypeDef,
     },
     total=False,
 )
 
+RiskExceptionConfigurationTypeUnionTypeDef = Union[
+    RiskExceptionConfigurationTypeTypeDef, RiskExceptionConfigurationTypeOutputTypeDef
+]
 SchemaAttributeTypeTypeDef = TypedDict(
     "SchemaAttributeTypeTypeDef",
     {
         "Name": str,
         "AttributeDataType": AttributeDataTypeType,
         "DeveloperOnlyAttribute": bool,
         "Mutable": bool,
         "Required": bool,
         "NumberAttributeConstraints": NumberAttributeConstraintsTypeTypeDef,
         "StringAttributeConstraints": StringAttributeConstraintsTypeTypeDef,
     },
     total=False,
 )
 
+UserAttributeUpdateSettingsTypeUnionTypeDef = Union[
+    UserAttributeUpdateSettingsTypeTypeDef, UserAttributeUpdateSettingsTypeOutputTypeDef
+]
+AccountRecoverySettingTypeUnionTypeDef = Union[
+    AccountRecoverySettingTypeTypeDef, AccountRecoverySettingTypeOutputTypeDef
+]
 AdminGetDeviceResponseTypeDef = TypedDict(
     "AdminGetDeviceResponseTypeDef",
     {
         "Device": DeviceTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AdminListDevicesResponseTypeDef = TypedDict(
     "AdminListDevicesResponseTypeDef",
     {
         "Devices": List[DeviceTypeTypeDef],
         "PaginationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeviceResponseTypeDef = TypedDict(
     "GetDeviceResponseTypeDef",
     {
         "Device": DeviceTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDevicesResponseTypeDef = TypedDict(
     "ListDevicesResponseTypeDef",
     {
         "Devices": List[DeviceTypeTypeDef],
         "PaginationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AdminCreateUserResponseTypeDef = TypedDict(
     "AdminCreateUserResponseTypeDef",
     {
         "User": UserTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsersInGroupResponseTypeDef = TypedDict(
     "ListUsersInGroupResponseTypeDef",
     {
         "Users": List[UserTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "Users": List[UserTypeTypeDef],
         "PaginationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AdminListUserAuthEventsResponseTypeDef = TypedDict(
     "AdminListUserAuthEventsResponseTypeDef",
     {
         "AuthEvents": List[AuthEventTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AdminInitiateAuthResponseTypeDef = TypedDict(
     "AdminInitiateAuthResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
         "AuthenticationResult": AuthenticationResultTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AdminRespondToAuthChallengeResponseTypeDef = TypedDict(
     "AdminRespondToAuthChallengeResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
         "AuthenticationResult": AuthenticationResultTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InitiateAuthResponseTypeDef = TypedDict(
     "InitiateAuthResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
         "AuthenticationResult": AuthenticationResultTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RespondToAuthChallengeResponseTypeDef = TypedDict(
     "RespondToAuthChallengeResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
         "AuthenticationResult": AuthenticationResultTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CompromisedCredentialsRiskConfigurationTypeUnionTypeDef = Union[
+    CompromisedCredentialsRiskConfigurationTypeTypeDef,
+    CompromisedCredentialsRiskConfigurationTypeOutputTypeDef,
+]
 _RequiredAdminInitiateAuthRequestRequestTypeDef = TypedDict(
     "_RequiredAdminInitiateAuthRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "ClientId": str,
         "AuthFlow": AuthFlowTypeType,
     },
@@ -3125,82 +3193,82 @@
 ):
     pass
 
 CreateResourceServerResponseTypeDef = TypedDict(
     "CreateResourceServerResponseTypeDef",
     {
         "ResourceServer": ResourceServerTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeResourceServerResponseTypeDef = TypedDict(
     "DescribeResourceServerResponseTypeDef",
     {
         "ResourceServer": ResourceServerTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceServersResponseTypeDef = TypedDict(
     "ListResourceServersResponseTypeDef",
     {
         "ResourceServers": List[ResourceServerTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResourceServerResponseTypeDef = TypedDict(
     "UpdateResourceServerResponseTypeDef",
     {
         "ResourceServer": ResourceServerTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateUserPoolClientResponseTypeDef = TypedDict(
     "CreateUserPoolClientResponseTypeDef",
     {
         "UserPoolClient": UserPoolClientTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUserPoolClientResponseTypeDef = TypedDict(
     "DescribeUserPoolClientResponseTypeDef",
     {
         "UserPoolClient": UserPoolClientTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUserPoolClientResponseTypeDef = TypedDict(
     "UpdateUserPoolClientResponseTypeDef",
     {
         "UserPoolClient": UserPoolClientTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUserPoolDomainResponseTypeDef = TypedDict(
     "DescribeUserPoolDomainResponseTypeDef",
     {
         "DomainDescription": DomainDescriptionTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserPoolMfaConfigResponseTypeDef = TypedDict(
     "GetUserPoolMfaConfigResponseTypeDef",
     {
         "SmsMfaConfiguration": SmsMfaConfigTypeTypeDef,
         "SoftwareTokenMfaConfiguration": SoftwareTokenMfaConfigTypeTypeDef,
         "MfaConfiguration": UserPoolMfaTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSetUserPoolMfaConfigRequestRequestTypeDef = TypedDict(
     "_RequiredSetUserPoolMfaConfigRequestRequestTypeDef",
     {
         "UserPoolId": str,
@@ -3224,15 +3292,15 @@
 
 SetUserPoolMfaConfigResponseTypeDef = TypedDict(
     "SetUserPoolMfaConfigResponseTypeDef",
     {
         "SmsMfaConfiguration": SmsMfaConfigTypeTypeDef,
         "SoftwareTokenMfaConfiguration": SoftwareTokenMfaConfigTypeTypeDef,
         "MfaConfiguration": UserPoolMfaTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UserPoolDescriptionTypeTypeDef = TypedDict(
     "UserPoolDescriptionTypeTypeDef",
     {
         "Id": str,
@@ -3365,53 +3433,53 @@
         "AliasAttributes": List[AliasAttributeTypeType],
         "UsernameAttributes": List[UsernameAttributeTypeType],
         "SmsVerificationMessage": str,
         "EmailVerificationMessage": str,
         "EmailVerificationSubject": str,
         "VerificationMessageTemplate": VerificationMessageTemplateTypeTypeDef,
         "SmsAuthenticationMessage": str,
-        "UserAttributeUpdateSettings": UserAttributeUpdateSettingsTypeTypeDef,
+        "UserAttributeUpdateSettings": UserAttributeUpdateSettingsTypeOutputTypeDef,
         "MfaConfiguration": UserPoolMfaTypeType,
         "DeviceConfiguration": DeviceConfigurationTypeTypeDef,
         "EstimatedNumberOfUsers": int,
         "EmailConfiguration": EmailConfigurationTypeTypeDef,
         "SmsConfiguration": SmsConfigurationTypeTypeDef,
         "UserPoolTags": Dict[str, str],
         "SmsConfigurationFailure": str,
         "EmailConfigurationFailure": str,
         "Domain": str,
         "CustomDomain": str,
         "AdminCreateUserConfig": AdminCreateUserConfigTypeTypeDef,
         "UserPoolAddOns": UserPoolAddOnsTypeTypeDef,
         "UsernameConfiguration": UsernameConfigurationTypeTypeDef,
         "Arn": str,
-        "AccountRecoverySetting": AccountRecoverySettingTypeTypeDef,
+        "AccountRecoverySetting": AccountRecoverySettingTypeOutputTypeDef,
     },
     total=False,
 )
 
 ListUserPoolsResponseTypeDef = TypedDict(
     "ListUserPoolsResponseTypeDef",
     {
         "UserPools": List[UserPoolDescriptionTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RiskConfigurationTypeTypeDef = TypedDict(
     "RiskConfigurationTypeTypeDef",
     {
         "UserPoolId": str,
         "ClientId": str,
         "CompromisedCredentialsRiskConfiguration": (
-            CompromisedCredentialsRiskConfigurationTypeTypeDef
+            CompromisedCredentialsRiskConfigurationTypeOutputTypeDef
         ),
         "AccountTakeoverRiskConfiguration": AccountTakeoverRiskConfigurationTypeTypeDef,
-        "RiskExceptionConfiguration": RiskExceptionConfigurationTypeTypeDef,
+        "RiskExceptionConfiguration": RiskExceptionConfigurationTypeOutputTypeDef,
         "LastModifiedDate": datetime,
     },
     total=False,
 )
 
 _RequiredSetRiskConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredSetRiskConfigurationRequestRequestTypeDef",
@@ -3438,34 +3506,34 @@
 ):
     pass
 
 CreateUserPoolResponseTypeDef = TypedDict(
     "CreateUserPoolResponseTypeDef",
     {
         "UserPool": UserPoolTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUserPoolResponseTypeDef = TypedDict(
     "DescribeUserPoolResponseTypeDef",
     {
         "UserPool": UserPoolTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRiskConfigurationResponseTypeDef = TypedDict(
     "DescribeRiskConfigurationResponseTypeDef",
     {
         "RiskConfiguration": RiskConfigurationTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SetRiskConfigurationResponseTypeDef = TypedDict(
     "SetRiskConfigurationResponseTypeDef",
     {
         "RiskConfiguration": RiskConfigurationTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp.egg-info/PKG-INFO` & `types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cognito-idp
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CognitoIdentityProvider 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CognitoIdentityProvider 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore cognito-idp type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore cognito-idp type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cognito-idp"></a>
 
 # types-aiobotocore-cognito-idp
 
 [![PyPI - types-aiobotocore-cognito-idp](https://img.shields.io/pypi/v/types-aiobotocore-cognito-idp.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-idp)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cognito-idp.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-idp)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cognito-idp?color=blue)](https://pypistats.org/packages/types-aiobotocore-cognito-idp)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cognito-idp)](https://pepy.tech/project/types-aiobotocore-cognito-idp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CognitoIdentityProvider 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
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
 [types-aiobotocore-cognito-idp docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/).
 
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
@@ -380,77 +379,75 @@
 )
 
 
 def check_value(value: AccountTakeoverEventActionTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cognito_idp.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cognito_idp.type_defs import (
     RecoveryOptionTypeTypeDef,
     AccountTakeoverActionTypeTypeDef,
     AdminAddUserToGroupRequestRequestTypeDef,
     AdminConfirmSignUpRequestRequestTypeDef,
     MessageTemplateTypeTypeDef,
     AttributeTypeTypeDef,
+    ResponseMetadataTypeDef,
     AdminDeleteUserAttributesRequestRequestTypeDef,
     AdminDeleteUserRequestRequestTypeDef,
     ProviderUserIdentifierTypeTypeDef,
     AdminDisableUserRequestRequestTypeDef,
     AdminEnableUserRequestRequestTypeDef,
     AdminForgetDeviceRequestRequestTypeDef,
     AdminGetDeviceRequestRequestTypeDef,
     AdminGetUserRequestRequestTypeDef,
     MFAOptionTypeTypeDef,
     AnalyticsMetadataTypeTypeDef,
     AdminListDevicesRequestRequestTypeDef,
-    AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
+    PaginatorConfigTypeDef,
     AdminListGroupsForUserRequestRequestTypeDef,
     GroupTypeTypeDef,
-    AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
     AdminListUserAuthEventsRequestRequestTypeDef,
     AdminRemoveUserFromGroupRequestRequestTypeDef,
     AdminResetUserPasswordRequestRequestTypeDef,
     SMSMfaSettingsTypeTypeDef,
     SoftwareTokenMfaSettingsTypeTypeDef,
     AdminSetUserPasswordRequestRequestTypeDef,
     AdminUpdateAuthEventFeedbackRequestRequestTypeDef,
     AdminUpdateDeviceStatusRequestRequestTypeDef,
     AdminUserGlobalSignOutRequestRequestTypeDef,
     AnalyticsConfigurationTypeTypeDef,
     AssociateSoftwareTokenRequestRequestTypeDef,
-    AssociateSoftwareTokenResponseTypeDef,
     ChallengeResponseTypeTypeDef,
     EventContextDataTypeTypeDef,
     EventFeedbackTypeTypeDef,
     EventRiskTypeTypeDef,
     NewDeviceMetadataTypeTypeDef,
+    BlobTypeDef,
     ChangePasswordRequestRequestTypeDef,
     CodeDeliveryDetailsTypeTypeDef,
     CompromisedCredentialsActionsTypeTypeDef,
     DeviceSecretVerifierConfigTypeTypeDef,
-    ConfirmDeviceResponseTypeDef,
     UserContextDataTypeTypeDef,
     HttpHeaderTypeDef,
     CreateGroupRequestRequestTypeDef,
     CreateIdentityProviderRequestRequestTypeDef,
     IdentityProviderTypeTypeDef,
     ResourceServerScopeTypeTypeDef,
     CreateUserImportJobRequestRequestTypeDef,
     UserImportJobTypeTypeDef,
     TokenValidityUnitsTypeTypeDef,
     CustomDomainConfigTypeTypeDef,
-    CreateUserPoolDomainResponseTypeDef,
     DeviceConfigurationTypeTypeDef,
     EmailConfigurationTypeTypeDef,
     SmsConfigurationTypeTypeDef,
     UserAttributeUpdateSettingsTypeTypeDef,
     UserPoolAddOnsTypeTypeDef,
     UsernameConfigurationTypeTypeDef,
     VerificationMessageTemplateTypeTypeDef,
@@ -467,99 +464,106 @@
     DescribeIdentityProviderRequestRequestTypeDef,
     DescribeResourceServerRequestRequestTypeDef,
     DescribeRiskConfigurationRequestRequestTypeDef,
     DescribeUserImportJobRequestRequestTypeDef,
     DescribeUserPoolClientRequestRequestTypeDef,
     DescribeUserPoolDomainRequestRequestTypeDef,
     DescribeUserPoolRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ForgetDeviceRequestRequestTypeDef,
     GetCSVHeaderRequestRequestTypeDef,
-    GetCSVHeaderResponseTypeDef,
     GetDeviceRequestRequestTypeDef,
     GetGroupRequestRequestTypeDef,
     GetIdentityProviderByIdentifierRequestRequestTypeDef,
     GetSigningCertificateRequestRequestTypeDef,
-    GetSigningCertificateResponseTypeDef,
     GetUICustomizationRequestRequestTypeDef,
     UICustomizationTypeTypeDef,
     GetUserAttributeVerificationCodeRequestRequestTypeDef,
     GetUserPoolMfaConfigRequestRequestTypeDef,
     SoftwareTokenMfaConfigTypeTypeDef,
     GetUserRequestRequestTypeDef,
     GlobalSignOutRequestRequestTypeDef,
     ListDevicesRequestRequestTypeDef,
-    ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
-    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
     ListIdentityProvidersRequestRequestTypeDef,
     ProviderDescriptionTypeDef,
-    ListResourceServersRequestListResourceServersPaginateTypeDef,
     ListResourceServersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListUserImportJobsRequestRequestTypeDef,
-    ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
     ListUserPoolClientsRequestRequestTypeDef,
     UserPoolClientDescriptionTypeDef,
-    ListUserPoolsRequestListUserPoolsPaginateTypeDef,
     ListUserPoolsRequestRequestTypeDef,
-    ListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
     ListUsersInGroupRequestRequestTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     NotifyEmailTypeTypeDef,
     NumberAttributeConstraintsTypeTypeDef,
-    PaginatorConfigTypeDef,
     PasswordPolicyTypeTypeDef,
-    ResponseMetadataTypeDef,
     RevokeTokenRequestRequestTypeDef,
+    RiskExceptionConfigurationTypeOutputTypeDef,
     RiskExceptionConfigurationTypeTypeDef,
     StringAttributeConstraintsTypeTypeDef,
-    SetUICustomizationRequestRequestTypeDef,
     StartUserImportJobRequestRequestTypeDef,
     StopUserImportJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAuthEventFeedbackRequestRequestTypeDef,
     UpdateDeviceStatusRequestRequestTypeDef,
     UpdateGroupRequestRequestTypeDef,
     UpdateIdentityProviderRequestRequestTypeDef,
-    UpdateUserPoolDomainResponseTypeDef,
+    UserAttributeUpdateSettingsTypeOutputTypeDef,
     VerifySoftwareTokenRequestRequestTypeDef,
-    VerifySoftwareTokenResponseTypeDef,
     VerifyUserAttributeRequestRequestTypeDef,
+    AccountRecoverySettingTypeOutputTypeDef,
     AccountRecoverySettingTypeTypeDef,
     AccountTakeoverActionsTypeTypeDef,
     AdminCreateUserConfigTypeTypeDef,
     AdminCreateUserRequestRequestTypeDef,
     AdminUpdateUserAttributesRequestRequestTypeDef,
     DeviceTypeTypeDef,
     UpdateUserAttributesRequestRequestTypeDef,
+    AssociateSoftwareTokenResponseTypeDef,
+    ConfirmDeviceResponseTypeDef,
+    CreateUserPoolDomainResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCSVHeaderResponseTypeDef,
+    GetSigningCertificateResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateUserPoolDomainResponseTypeDef,
+    VerifySoftwareTokenResponseTypeDef,
     AdminDisableProviderForUserRequestRequestTypeDef,
     AdminLinkProviderForUserRequestRequestTypeDef,
     AdminGetUserResponseTypeDef,
     AdminSetUserSettingsRequestRequestTypeDef,
     GetUserResponseTypeDef,
     SetUserSettingsRequestRequestTypeDef,
     UserTypeTypeDef,
+    AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
+    AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
+    ListGroupsRequestListGroupsPaginateTypeDef,
+    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
+    ListResourceServersRequestListResourceServersPaginateTypeDef,
+    ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
+    ListUserPoolsRequestListUserPoolsPaginateTypeDef,
+    ListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
     AdminListGroupsForUserResponseTypeDef,
     CreateGroupResponseTypeDef,
     GetGroupResponseTypeDef,
     ListGroupsResponseTypeDef,
     UpdateGroupResponseTypeDef,
     AdminSetUserMFAPreferenceRequestRequestTypeDef,
     SetUserMFAPreferenceRequestRequestTypeDef,
     AuthEventTypeTypeDef,
     AuthenticationResultTypeTypeDef,
+    SetUICustomizationRequestRequestTypeDef,
     ForgotPasswordResponseTypeDef,
     GetUserAttributeVerificationCodeResponseTypeDef,
     ResendConfirmationCodeResponseTypeDef,
     SignUpResponseTypeDef,
     UpdateUserAttributesResponseTypeDef,
+    CompromisedCredentialsRiskConfigurationTypeOutputTypeDef,
     CompromisedCredentialsRiskConfigurationTypeTypeDef,
     ConfirmDeviceRequestRequestTypeDef,
     ConfirmForgotPasswordRequestRequestTypeDef,
     ConfirmSignUpRequestRequestTypeDef,
     ForgotPasswordRequestRequestTypeDef,
     InitiateAuthRequestRequestTypeDef,
     ResendConfirmationCodeRequestRequestTypeDef,
@@ -588,27 +592,31 @@
     LambdaConfigTypeTypeDef,
     GetUICustomizationResponseTypeDef,
     SetUICustomizationResponseTypeDef,
     ListIdentityProvidersResponseTypeDef,
     ListUserPoolClientsResponseTypeDef,
     NotifyConfigurationTypeTypeDef,
     UserPoolPolicyTypeTypeDef,
+    RiskExceptionConfigurationTypeUnionTypeDef,
     SchemaAttributeTypeTypeDef,
+    UserAttributeUpdateSettingsTypeUnionTypeDef,
+    AccountRecoverySettingTypeUnionTypeDef,
     AdminGetDeviceResponseTypeDef,
     AdminListDevicesResponseTypeDef,
     GetDeviceResponseTypeDef,
     ListDevicesResponseTypeDef,
     AdminCreateUserResponseTypeDef,
     ListUsersInGroupResponseTypeDef,
     ListUsersResponseTypeDef,
     AdminListUserAuthEventsResponseTypeDef,
     AdminInitiateAuthResponseTypeDef,
     AdminRespondToAuthChallengeResponseTypeDef,
     InitiateAuthResponseTypeDef,
     RespondToAuthChallengeResponseTypeDef,
+    CompromisedCredentialsRiskConfigurationTypeUnionTypeDef,
     AdminInitiateAuthRequestRequestTypeDef,
     AdminRespondToAuthChallengeRequestRequestTypeDef,
     CreateResourceServerResponseTypeDef,
     DescribeResourceServerResponseTypeDef,
     ListResourceServersResponseTypeDef,
     UpdateResourceServerResponseTypeDef,
     CreateUserPoolClientResponseTypeDef,
@@ -630,15 +638,15 @@
     CreateUserPoolResponseTypeDef,
     DescribeUserPoolResponseTypeDef,
     DescribeRiskConfigurationResponseTypeDef,
     SetRiskConfigurationResponseTypeDef,
 )
 
 
-def get_structure() -> RecoveryOptionTypeTypeDef:
+def get_value() -> RecoveryOptionTypeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cognito-idp-2.5.2/types_aiobotocore_cognito_idp.egg-info/SOURCES.txt` & `types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp.egg-info/SOURCES.txt`

 * *Files identical despite different names*


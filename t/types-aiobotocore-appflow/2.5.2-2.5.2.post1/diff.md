# Comparing `tmp/types-aiobotocore-appflow-2.5.2.tar.gz` & `tmp/types-aiobotocore-appflow-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-appflow-2.5.2.tar", last modified: Sat Jul  8 01:43:12 2023, max compression
+gzip compressed data, was "types-aiobotocore-appflow-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:50 2023, max compression
```

## Comparing `types-aiobotocore-appflow-2.5.2.tar` & `types-aiobotocore-appflow-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:12.369652 types-aiobotocore-appflow-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:25:43.000000 types-aiobotocore-appflow-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19966 2023-07-08 01:43:12.369652 types-aiobotocore-appflow-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18401 2023-07-08 01:25:43.000000 types-aiobotocore-appflow-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:12.389653 types-aiobotocore-appflow-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-08 01:25:43.000000 types-aiobotocore-appflow-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:12.369652 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-08 01:25:43.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-08 01:25:43.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-08 01:25:43.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21145 2023-07-08 01:25:43.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-07-08 01:25:43.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18362 2023-07-08 01:25:43.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    18360 2023-07-08 01:25:43.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:25:43.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    71147 2023-07-08 01:25:45.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    71045 2023-07-08 01:25:44.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:25:43.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:12.369652 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19966 2023-07-08 01:43:12.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-08 01:43:12.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:12.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:12.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:12.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-08 01:43:12.000000 types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.545660 types-aiobotocore-appflow-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:09.000000 types-aiobotocore-appflow-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21029 2023-08-02 14:51:50.545660 types-aiobotocore-appflow-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19511 2023-08-02 14:33:09.000000 types-aiobotocore-appflow-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:50.545660 types-aiobotocore-appflow-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-02 14:33:09.000000 types-aiobotocore-appflow-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.541660 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-02 14:33:09.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-08-02 14:33:09.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-02 14:33:09.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21205 2023-08-02 14:33:09.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21171 2023-08-02 14:33:09.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18362 2023-08-02 14:33:09.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18360 2023-08-02 14:33:09.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:09.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    86507 2023-08-02 14:33:11.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86375 2023-08-02 14:33:10.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:09.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.545660 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21029 2023-08-02 14:51:50.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-02 14:51:50.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:50.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:50.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:50.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 14:51:50.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-appflow-2.5.2/LICENSE` & `types-aiobotocore-appflow-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appflow-2.5.2/PKG-INFO` & `types-aiobotocore-appflow-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appflow
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Appflow 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Appflow 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore appflow type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore appflow type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-appflow"></a>
 
 # types-aiobotocore-appflow
 
 [![PyPI - types-aiobotocore-appflow](https://img.shields.io/pypi/v/types-aiobotocore-appflow.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appflow)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appflow.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appflow)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-appflow?color=blue)](https://pypistats.org/packages/types-aiobotocore-appflow)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appflow)](https://pepy.tech/project/types-aiobotocore-appflow)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Appflow 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
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
 [types-aiobotocore-appflow docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/).
 
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
@@ -323,31 +322,31 @@
 )
 
 
 def check_value(value: AggregationTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_appflow.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_appflow.type_defs import (
     AggregationConfigTypeDef,
     AmplitudeConnectorProfileCredentialsTypeDef,
     AmplitudeSourcePropertiesTypeDef,
     ApiKeyCredentialsTypeDef,
     AuthParameterTypeDef,
     BasicAuthCredentialsTypeDef,
     CancelFlowExecutionsRequestRequestTypeDef,
-    CancelFlowExecutionsResponseTypeDef,
+    ResponseMetadataTypeDef,
     ConnectorRuntimeSettingTypeDef,
     DataTransferApiTypeDef,
     ConnectorDetailTypeDef,
     DestinationFieldPropertiesTypeDef,
     SourceFieldPropertiesTypeDef,
     ConnectorEntityTypeDef,
     GoogleAnalyticsMetadataTypeDef,
@@ -377,18 +376,17 @@
     ServiceNowConnectorProfilePropertiesTypeDef,
     SlackConnectorProfilePropertiesTypeDef,
     SnowflakeConnectorProfilePropertiesTypeDef,
     VeevaConnectorProfilePropertiesTypeDef,
     ZendeskConnectorProfilePropertiesTypeDef,
     PrivateConnectionProvisioningStateTypeDef,
     LambdaConnectorProvisioningConfigTypeDef,
-    CreateConnectorProfileResponseTypeDef,
-    CreateFlowResponseTypeDef,
     CustomAuthCredentialsTypeDef,
     ErrorHandlingConfigTypeDef,
+    OAuth2PropertiesOutputTypeDef,
     OAuth2PropertiesTypeDef,
     CustomerProfilesDestinationPropertiesTypeDef,
     DatadogSourcePropertiesTypeDef,
     DeleteConnectorProfileRequestRequestTypeDef,
     DeleteFlowRequestRequestTypeDef,
     DescribeConnectorEntityRequestRequestTypeDef,
     DescribeConnectorProfilesRequestRequestTypeDef,
@@ -404,117 +402,146 @@
     GoogleAnalyticsSourcePropertiesTypeDef,
     IncrementalPullConfigTypeDef,
     InforNexusSourcePropertiesTypeDef,
     ListConnectorEntitiesRequestRequestTypeDef,
     ListConnectorsRequestRequestTypeDef,
     ListFlowsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     MarketoSourcePropertiesTypeDef,
     RegistrationOutputTypeDef,
     OAuth2CustomParameterTypeDef,
+    OAuthPropertiesOutputTypeDef,
     OAuthPropertiesTypeDef,
     PardotSourcePropertiesTypeDef,
+    PrefixConfigOutputTypeDef,
     PrefixConfigTypeDef,
-    RegisterConnectorResponseTypeDef,
     ResetConnectorMetadataCacheRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     S3InputFormatConfigTypeDef,
     SuccessResponseHandlingConfigTypeDef,
     SAPODataSourcePropertiesTypeDef,
     SalesforceSourcePropertiesTypeDef,
-    ScheduledTriggerPropertiesTypeDef,
+    ScheduledTriggerPropertiesOutputTypeDef,
+    TimestampTypeDef,
     ServiceNowSourcePropertiesTypeDef,
     SingularSourcePropertiesTypeDef,
     SlackSourcePropertiesTypeDef,
     TrendmicroSourcePropertiesTypeDef,
     VeevaSourcePropertiesTypeDef,
     ZendeskSourcePropertiesTypeDef,
     StartFlowRequestRequestTypeDef,
-    StartFlowResponseTypeDef,
     StopFlowRequestRequestTypeDef,
-    StopFlowResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UnregisterConnectorRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    CustomAuthConfigTypeDef,
+    CancelFlowExecutionsResponseTypeDef,
+    CreateConnectorProfileResponseTypeDef,
+    CreateFlowResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RegisterConnectorResponseTypeDef,
+    StartFlowResponseTypeDef,
+    StopFlowResponseTypeDef,
     UpdateConnectorProfileResponseTypeDef,
     UpdateConnectorRegistrationResponseTypeDef,
     UpdateFlowResponseTypeDef,
-    CustomAuthConfigTypeDef,
+    CustomConnectorSourcePropertiesOutputTypeDef,
     CustomConnectorSourcePropertiesTypeDef,
     ListConnectorsResponseTypeDef,
     ListConnectorEntitiesResponseTypeDef,
     ConnectorMetadataTypeDef,
     GoogleAnalyticsConnectorProfileCredentialsTypeDef,
     HoneycodeConnectorProfileCredentialsTypeDef,
     MarketoConnectorProfileCredentialsTypeDef,
     OAuth2CredentialsTypeDef,
     OAuthCredentialsTypeDef,
     PardotConnectorProfileCredentialsTypeDef,
     SalesforceConnectorProfileCredentialsTypeDef,
     SlackConnectorProfileCredentialsTypeDef,
     ZendeskConnectorProfileCredentialsTypeDef,
+    TaskOutputTypeDef,
     TaskTypeDef,
     ConnectorProvisioningConfigTypeDef,
+    CustomConnectorDestinationPropertiesOutputTypeDef,
     CustomConnectorDestinationPropertiesTypeDef,
     EventBridgeDestinationPropertiesTypeDef,
     HoneycodeDestinationPropertiesTypeDef,
     MarketoDestinationPropertiesTypeDef,
     RedshiftDestinationPropertiesTypeDef,
+    SalesforceDestinationPropertiesOutputTypeDef,
     SalesforceDestinationPropertiesTypeDef,
     SnowflakeDestinationPropertiesTypeDef,
+    ZendeskDestinationPropertiesOutputTypeDef,
     ZendeskDestinationPropertiesTypeDef,
+    CustomConnectorProfilePropertiesOutputTypeDef,
     CustomConnectorProfilePropertiesTypeDef,
     FlowDefinitionTypeDef,
     ExecutionResultTypeDef,
     FieldTypeDetailsTypeDef,
     MetadataCatalogConfigTypeDef,
     MetadataCatalogDetailTypeDef,
     OAuth2DefaultsTypeDef,
+    SAPODataConnectorProfilePropertiesOutputTypeDef,
     SAPODataConnectorProfilePropertiesTypeDef,
+    S3OutputFormatConfigOutputTypeDef,
+    UpsolverS3OutputFormatConfigOutputTypeDef,
     S3OutputFormatConfigTypeDef,
     UpsolverS3OutputFormatConfigTypeDef,
     S3SourcePropertiesTypeDef,
+    SAPODataDestinationPropertiesOutputTypeDef,
     SAPODataDestinationPropertiesTypeDef,
-    TriggerPropertiesTypeDef,
+    TriggerPropertiesOutputTypeDef,
+    ScheduledTriggerPropertiesTypeDef,
     CustomConnectorProfileCredentialsTypeDef,
     SAPODataConnectorProfileCredentialsTypeDef,
+    TaskUnionTypeDef,
     RegisterConnectorRequestRequestTypeDef,
     UpdateConnectorRegistrationRequestRequestTypeDef,
     ListFlowsResponseTypeDef,
     SupportedFieldTypeDetailsTypeDef,
     ExecutionRecordTypeDef,
     AuthenticationConfigTypeDef,
+    ConnectorProfilePropertiesOutputTypeDef,
     ConnectorProfilePropertiesTypeDef,
+    S3DestinationPropertiesOutputTypeDef,
+    UpsolverDestinationPropertiesOutputTypeDef,
     S3DestinationPropertiesTypeDef,
     UpsolverDestinationPropertiesTypeDef,
+    SourceConnectorPropertiesOutputTypeDef,
     SourceConnectorPropertiesTypeDef,
-    TriggerConfigTypeDef,
+    TriggerConfigOutputTypeDef,
+    TriggerPropertiesTypeDef,
     ConnectorProfileCredentialsTypeDef,
     ConnectorEntityFieldTypeDef,
     DescribeFlowExecutionRecordsResponseTypeDef,
     ConnectorConfigurationTypeDef,
     ConnectorProfileTypeDef,
+    DestinationConnectorPropertiesOutputTypeDef,
     DestinationConnectorPropertiesTypeDef,
+    SourceFlowConfigOutputTypeDef,
     SourceFlowConfigTypeDef,
+    TriggerConfigTypeDef,
     ConnectorProfileConfigTypeDef,
     DescribeConnectorEntityResponseTypeDef,
     DescribeConnectorResponseTypeDef,
     DescribeConnectorsResponseTypeDef,
     DescribeConnectorProfilesResponseTypeDef,
+    DestinationFlowConfigOutputTypeDef,
     DestinationFlowConfigTypeDef,
+    SourceFlowConfigUnionTypeDef,
+    TriggerConfigUnionTypeDef,
     CreateConnectorProfileRequestRequestTypeDef,
     UpdateConnectorProfileRequestRequestTypeDef,
-    CreateFlowRequestRequestTypeDef,
     DescribeFlowResponseTypeDef,
+    DestinationFlowConfigUnionTypeDef,
+    CreateFlowRequestRequestTypeDef,
     UpdateFlowRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AggregationConfigTypeDef:
+def get_value() -> AggregationConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-appflow-2.5.2/README.md` & `types-aiobotocore-appflow-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-appflow"></a>
 
 # types-aiobotocore-appflow
 
 [![PyPI - types-aiobotocore-appflow](https://img.shields.io/pypi/v/types-aiobotocore-appflow.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appflow)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appflow.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appflow)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-appflow?color=blue)](https://pypistats.org/packages/types-aiobotocore-appflow)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appflow)](https://pepy.tech/project/types-aiobotocore-appflow)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Appflow 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
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
 [types-aiobotocore-appflow docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/).
 
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
@@ -290,31 +290,31 @@
 )
 
 
 def check_value(value: AggregationTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_appflow.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_appflow.type_defs import (
     AggregationConfigTypeDef,
     AmplitudeConnectorProfileCredentialsTypeDef,
     AmplitudeSourcePropertiesTypeDef,
     ApiKeyCredentialsTypeDef,
     AuthParameterTypeDef,
     BasicAuthCredentialsTypeDef,
     CancelFlowExecutionsRequestRequestTypeDef,
-    CancelFlowExecutionsResponseTypeDef,
+    ResponseMetadataTypeDef,
     ConnectorRuntimeSettingTypeDef,
     DataTransferApiTypeDef,
     ConnectorDetailTypeDef,
     DestinationFieldPropertiesTypeDef,
     SourceFieldPropertiesTypeDef,
     ConnectorEntityTypeDef,
     GoogleAnalyticsMetadataTypeDef,
@@ -344,18 +344,17 @@
     ServiceNowConnectorProfilePropertiesTypeDef,
     SlackConnectorProfilePropertiesTypeDef,
     SnowflakeConnectorProfilePropertiesTypeDef,
     VeevaConnectorProfilePropertiesTypeDef,
     ZendeskConnectorProfilePropertiesTypeDef,
     PrivateConnectionProvisioningStateTypeDef,
     LambdaConnectorProvisioningConfigTypeDef,
-    CreateConnectorProfileResponseTypeDef,
-    CreateFlowResponseTypeDef,
     CustomAuthCredentialsTypeDef,
     ErrorHandlingConfigTypeDef,
+    OAuth2PropertiesOutputTypeDef,
     OAuth2PropertiesTypeDef,
     CustomerProfilesDestinationPropertiesTypeDef,
     DatadogSourcePropertiesTypeDef,
     DeleteConnectorProfileRequestRequestTypeDef,
     DeleteFlowRequestRequestTypeDef,
     DescribeConnectorEntityRequestRequestTypeDef,
     DescribeConnectorProfilesRequestRequestTypeDef,
@@ -371,117 +370,146 @@
     GoogleAnalyticsSourcePropertiesTypeDef,
     IncrementalPullConfigTypeDef,
     InforNexusSourcePropertiesTypeDef,
     ListConnectorEntitiesRequestRequestTypeDef,
     ListConnectorsRequestRequestTypeDef,
     ListFlowsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     MarketoSourcePropertiesTypeDef,
     RegistrationOutputTypeDef,
     OAuth2CustomParameterTypeDef,
+    OAuthPropertiesOutputTypeDef,
     OAuthPropertiesTypeDef,
     PardotSourcePropertiesTypeDef,
+    PrefixConfigOutputTypeDef,
     PrefixConfigTypeDef,
-    RegisterConnectorResponseTypeDef,
     ResetConnectorMetadataCacheRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     S3InputFormatConfigTypeDef,
     SuccessResponseHandlingConfigTypeDef,
     SAPODataSourcePropertiesTypeDef,
     SalesforceSourcePropertiesTypeDef,
-    ScheduledTriggerPropertiesTypeDef,
+    ScheduledTriggerPropertiesOutputTypeDef,
+    TimestampTypeDef,
     ServiceNowSourcePropertiesTypeDef,
     SingularSourcePropertiesTypeDef,
     SlackSourcePropertiesTypeDef,
     TrendmicroSourcePropertiesTypeDef,
     VeevaSourcePropertiesTypeDef,
     ZendeskSourcePropertiesTypeDef,
     StartFlowRequestRequestTypeDef,
-    StartFlowResponseTypeDef,
     StopFlowRequestRequestTypeDef,
-    StopFlowResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UnregisterConnectorRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    CustomAuthConfigTypeDef,
+    CancelFlowExecutionsResponseTypeDef,
+    CreateConnectorProfileResponseTypeDef,
+    CreateFlowResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RegisterConnectorResponseTypeDef,
+    StartFlowResponseTypeDef,
+    StopFlowResponseTypeDef,
     UpdateConnectorProfileResponseTypeDef,
     UpdateConnectorRegistrationResponseTypeDef,
     UpdateFlowResponseTypeDef,
-    CustomAuthConfigTypeDef,
+    CustomConnectorSourcePropertiesOutputTypeDef,
     CustomConnectorSourcePropertiesTypeDef,
     ListConnectorsResponseTypeDef,
     ListConnectorEntitiesResponseTypeDef,
     ConnectorMetadataTypeDef,
     GoogleAnalyticsConnectorProfileCredentialsTypeDef,
     HoneycodeConnectorProfileCredentialsTypeDef,
     MarketoConnectorProfileCredentialsTypeDef,
     OAuth2CredentialsTypeDef,
     OAuthCredentialsTypeDef,
     PardotConnectorProfileCredentialsTypeDef,
     SalesforceConnectorProfileCredentialsTypeDef,
     SlackConnectorProfileCredentialsTypeDef,
     ZendeskConnectorProfileCredentialsTypeDef,
+    TaskOutputTypeDef,
     TaskTypeDef,
     ConnectorProvisioningConfigTypeDef,
+    CustomConnectorDestinationPropertiesOutputTypeDef,
     CustomConnectorDestinationPropertiesTypeDef,
     EventBridgeDestinationPropertiesTypeDef,
     HoneycodeDestinationPropertiesTypeDef,
     MarketoDestinationPropertiesTypeDef,
     RedshiftDestinationPropertiesTypeDef,
+    SalesforceDestinationPropertiesOutputTypeDef,
     SalesforceDestinationPropertiesTypeDef,
     SnowflakeDestinationPropertiesTypeDef,
+    ZendeskDestinationPropertiesOutputTypeDef,
     ZendeskDestinationPropertiesTypeDef,
+    CustomConnectorProfilePropertiesOutputTypeDef,
     CustomConnectorProfilePropertiesTypeDef,
     FlowDefinitionTypeDef,
     ExecutionResultTypeDef,
     FieldTypeDetailsTypeDef,
     MetadataCatalogConfigTypeDef,
     MetadataCatalogDetailTypeDef,
     OAuth2DefaultsTypeDef,
+    SAPODataConnectorProfilePropertiesOutputTypeDef,
     SAPODataConnectorProfilePropertiesTypeDef,
+    S3OutputFormatConfigOutputTypeDef,
+    UpsolverS3OutputFormatConfigOutputTypeDef,
     S3OutputFormatConfigTypeDef,
     UpsolverS3OutputFormatConfigTypeDef,
     S3SourcePropertiesTypeDef,
+    SAPODataDestinationPropertiesOutputTypeDef,
     SAPODataDestinationPropertiesTypeDef,
-    TriggerPropertiesTypeDef,
+    TriggerPropertiesOutputTypeDef,
+    ScheduledTriggerPropertiesTypeDef,
     CustomConnectorProfileCredentialsTypeDef,
     SAPODataConnectorProfileCredentialsTypeDef,
+    TaskUnionTypeDef,
     RegisterConnectorRequestRequestTypeDef,
     UpdateConnectorRegistrationRequestRequestTypeDef,
     ListFlowsResponseTypeDef,
     SupportedFieldTypeDetailsTypeDef,
     ExecutionRecordTypeDef,
     AuthenticationConfigTypeDef,
+    ConnectorProfilePropertiesOutputTypeDef,
     ConnectorProfilePropertiesTypeDef,
+    S3DestinationPropertiesOutputTypeDef,
+    UpsolverDestinationPropertiesOutputTypeDef,
     S3DestinationPropertiesTypeDef,
     UpsolverDestinationPropertiesTypeDef,
+    SourceConnectorPropertiesOutputTypeDef,
     SourceConnectorPropertiesTypeDef,
-    TriggerConfigTypeDef,
+    TriggerConfigOutputTypeDef,
+    TriggerPropertiesTypeDef,
     ConnectorProfileCredentialsTypeDef,
     ConnectorEntityFieldTypeDef,
     DescribeFlowExecutionRecordsResponseTypeDef,
     ConnectorConfigurationTypeDef,
     ConnectorProfileTypeDef,
+    DestinationConnectorPropertiesOutputTypeDef,
     DestinationConnectorPropertiesTypeDef,
+    SourceFlowConfigOutputTypeDef,
     SourceFlowConfigTypeDef,
+    TriggerConfigTypeDef,
     ConnectorProfileConfigTypeDef,
     DescribeConnectorEntityResponseTypeDef,
     DescribeConnectorResponseTypeDef,
     DescribeConnectorsResponseTypeDef,
     DescribeConnectorProfilesResponseTypeDef,
+    DestinationFlowConfigOutputTypeDef,
     DestinationFlowConfigTypeDef,
+    SourceFlowConfigUnionTypeDef,
+    TriggerConfigUnionTypeDef,
     CreateConnectorProfileRequestRequestTypeDef,
     UpdateConnectorProfileRequestRequestTypeDef,
-    CreateFlowRequestRequestTypeDef,
     DescribeFlowResponseTypeDef,
+    DestinationFlowConfigUnionTypeDef,
+    CreateFlowRequestRequestTypeDef,
     UpdateFlowRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AggregationConfigTypeDef:
+def get_value() -> AggregationConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-appflow-2.5.2/setup.py` & `types-aiobotocore-appflow-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-appflow",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_appflow"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Appflow 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore appflow type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore appflow type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_appflow": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/"
```

### Comparing `types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/__main__.py` & `types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Appflow 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Appflow 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow\nOther"
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

### Comparing `types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/client.py` & `types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,26 +29,26 @@
     CreateFlowResponseTypeDef,
     DescribeConnectorEntityResponseTypeDef,
     DescribeConnectorProfilesResponseTypeDef,
     DescribeConnectorResponseTypeDef,
     DescribeConnectorsResponseTypeDef,
     DescribeFlowExecutionRecordsResponseTypeDef,
     DescribeFlowResponseTypeDef,
-    DestinationFlowConfigTypeDef,
+    DestinationFlowConfigUnionTypeDef,
     ListConnectorEntitiesResponseTypeDef,
     ListConnectorsResponseTypeDef,
     ListFlowsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MetadataCatalogConfigTypeDef,
     RegisterConnectorResponseTypeDef,
-    SourceFlowConfigTypeDef,
+    SourceFlowConfigUnionTypeDef,
     StartFlowResponseTypeDef,
     StopFlowResponseTypeDef,
-    TaskTypeDef,
-    TriggerConfigTypeDef,
+    TaskUnionTypeDef,
+    TriggerConfigUnionTypeDef,
     UpdateConnectorProfileResponseTypeDef,
     UpdateConnectorRegistrationResponseTypeDef,
     UpdateFlowResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -143,18 +143,18 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/client/#create_connector_profile)
         """
 
     async def create_flow(
         self,
         *,
         flowName: str,
-        triggerConfig: TriggerConfigTypeDef,
-        sourceFlowConfig: SourceFlowConfigTypeDef,
-        destinationFlowConfigList: Sequence[DestinationFlowConfigTypeDef],
-        tasks: Sequence[TaskTypeDef],
+        triggerConfig: TriggerConfigUnionTypeDef,
+        sourceFlowConfig: SourceFlowConfigUnionTypeDef,
+        destinationFlowConfigList: Sequence[DestinationFlowConfigUnionTypeDef],
+        tasks: Sequence[TaskUnionTypeDef],
         description: str = ...,
         kmsArn: str = ...,
         tags: Mapping[str, str] = ...,
         metadataCatalogConfig: MetadataCatalogConfigTypeDef = ...,
         clientToken: str = ...
     ) -> CreateFlowResponseTypeDef:
         """
@@ -428,18 +428,18 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/client/#update_connector_registration)
         """
 
     async def update_flow(
         self,
         *,
         flowName: str,
-        triggerConfig: TriggerConfigTypeDef,
-        sourceFlowConfig: SourceFlowConfigTypeDef,
-        destinationFlowConfigList: Sequence[DestinationFlowConfigTypeDef],
-        tasks: Sequence[TaskTypeDef],
+        triggerConfig: TriggerConfigUnionTypeDef,
+        sourceFlowConfig: SourceFlowConfigUnionTypeDef,
+        destinationFlowConfigList: Sequence[DestinationFlowConfigUnionTypeDef],
+        tasks: Sequence[TaskUnionTypeDef],
         description: str = ...,
         metadataCatalogConfig: MetadataCatalogConfigTypeDef = ...,
         clientToken: str = ...
     ) -> UpdateFlowResponseTypeDef:
         """
         Updates an existing flow.
```

### Comparing `types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/client.pyi` & `types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -29,26 +29,26 @@
     CreateFlowResponseTypeDef,
     DescribeConnectorEntityResponseTypeDef,
     DescribeConnectorProfilesResponseTypeDef,
     DescribeConnectorResponseTypeDef,
     DescribeConnectorsResponseTypeDef,
     DescribeFlowExecutionRecordsResponseTypeDef,
     DescribeFlowResponseTypeDef,
-    DestinationFlowConfigTypeDef,
+    DestinationFlowConfigUnionTypeDef,
     ListConnectorEntitiesResponseTypeDef,
     ListConnectorsResponseTypeDef,
     ListFlowsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MetadataCatalogConfigTypeDef,
     RegisterConnectorResponseTypeDef,
-    SourceFlowConfigTypeDef,
+    SourceFlowConfigUnionTypeDef,
     StartFlowResponseTypeDef,
     StopFlowResponseTypeDef,
-    TaskTypeDef,
-    TriggerConfigTypeDef,
+    TaskUnionTypeDef,
+    TriggerConfigUnionTypeDef,
     UpdateConnectorProfileResponseTypeDef,
     UpdateConnectorRegistrationResponseTypeDef,
     UpdateFlowResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -134,18 +134,18 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.create_connector_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/client/#create_connector_profile)
         """
     async def create_flow(
         self,
         *,
         flowName: str,
-        triggerConfig: TriggerConfigTypeDef,
-        sourceFlowConfig: SourceFlowConfigTypeDef,
-        destinationFlowConfigList: Sequence[DestinationFlowConfigTypeDef],
-        tasks: Sequence[TaskTypeDef],
+        triggerConfig: TriggerConfigUnionTypeDef,
+        sourceFlowConfig: SourceFlowConfigUnionTypeDef,
+        destinationFlowConfigList: Sequence[DestinationFlowConfigUnionTypeDef],
+        tasks: Sequence[TaskUnionTypeDef],
         description: str = ...,
         kmsArn: str = ...,
         tags: Mapping[str, str] = ...,
         metadataCatalogConfig: MetadataCatalogConfigTypeDef = ...,
         clientToken: str = ...
     ) -> CreateFlowResponseTypeDef:
         """
@@ -396,18 +396,18 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.update_connector_registration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/client/#update_connector_registration)
         """
     async def update_flow(
         self,
         *,
         flowName: str,
-        triggerConfig: TriggerConfigTypeDef,
-        sourceFlowConfig: SourceFlowConfigTypeDef,
-        destinationFlowConfigList: Sequence[DestinationFlowConfigTypeDef],
-        tasks: Sequence[TaskTypeDef],
+        triggerConfig: TriggerConfigUnionTypeDef,
+        sourceFlowConfig: SourceFlowConfigUnionTypeDef,
+        destinationFlowConfigList: Sequence[DestinationFlowConfigUnionTypeDef],
+        tasks: Sequence[TaskUnionTypeDef],
         description: str = ...,
         metadataCatalogConfig: MetadataCatalogConfigTypeDef = ...,
         clientToken: str = ...
     ) -> UpdateFlowResponseTypeDef:
         """
         Updates an existing flow.
```

### Comparing `types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/literals.py` & `types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/literals.pyi` & `types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/type_defs.py` & `types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_appflow.type_defs import AggregationConfigTypeDef
 
-    data: AggregationConfigTypeDef = {...}
+    data: AggregationConfigTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -64,24 +64,23 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AggregationConfigTypeDef",
     "AmplitudeConnectorProfileCredentialsTypeDef",
     "AmplitudeSourcePropertiesTypeDef",
     "ApiKeyCredentialsTypeDef",
     "AuthParameterTypeDef",
     "BasicAuthCredentialsTypeDef",
     "CancelFlowExecutionsRequestRequestTypeDef",
-    "CancelFlowExecutionsResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ConnectorRuntimeSettingTypeDef",
     "DataTransferApiTypeDef",
     "ConnectorDetailTypeDef",
     "DestinationFieldPropertiesTypeDef",
     "SourceFieldPropertiesTypeDef",
     "ConnectorEntityTypeDef",
     "GoogleAnalyticsMetadataTypeDef",
@@ -111,18 +110,17 @@
     "ServiceNowConnectorProfilePropertiesTypeDef",
     "SlackConnectorProfilePropertiesTypeDef",
     "SnowflakeConnectorProfilePropertiesTypeDef",
     "VeevaConnectorProfilePropertiesTypeDef",
     "ZendeskConnectorProfilePropertiesTypeDef",
     "PrivateConnectionProvisioningStateTypeDef",
     "LambdaConnectorProvisioningConfigTypeDef",
-    "CreateConnectorProfileResponseTypeDef",
-    "CreateFlowResponseTypeDef",
     "CustomAuthCredentialsTypeDef",
     "ErrorHandlingConfigTypeDef",
+    "OAuth2PropertiesOutputTypeDef",
     "OAuth2PropertiesTypeDef",
     "CustomerProfilesDestinationPropertiesTypeDef",
     "DatadogSourcePropertiesTypeDef",
     "DeleteConnectorProfileRequestRequestTypeDef",
     "DeleteFlowRequestRequestTypeDef",
     "DescribeConnectorEntityRequestRequestTypeDef",
     "DescribeConnectorProfilesRequestRequestTypeDef",
@@ -138,112 +136,141 @@
     "GoogleAnalyticsSourcePropertiesTypeDef",
     "IncrementalPullConfigTypeDef",
     "InforNexusSourcePropertiesTypeDef",
     "ListConnectorEntitiesRequestRequestTypeDef",
     "ListConnectorsRequestRequestTypeDef",
     "ListFlowsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "MarketoSourcePropertiesTypeDef",
     "RegistrationOutputTypeDef",
     "OAuth2CustomParameterTypeDef",
+    "OAuthPropertiesOutputTypeDef",
     "OAuthPropertiesTypeDef",
     "PardotSourcePropertiesTypeDef",
+    "PrefixConfigOutputTypeDef",
     "PrefixConfigTypeDef",
-    "RegisterConnectorResponseTypeDef",
     "ResetConnectorMetadataCacheRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "S3InputFormatConfigTypeDef",
     "SuccessResponseHandlingConfigTypeDef",
     "SAPODataSourcePropertiesTypeDef",
     "SalesforceSourcePropertiesTypeDef",
-    "ScheduledTriggerPropertiesTypeDef",
+    "ScheduledTriggerPropertiesOutputTypeDef",
+    "TimestampTypeDef",
     "ServiceNowSourcePropertiesTypeDef",
     "SingularSourcePropertiesTypeDef",
     "SlackSourcePropertiesTypeDef",
     "TrendmicroSourcePropertiesTypeDef",
     "VeevaSourcePropertiesTypeDef",
     "ZendeskSourcePropertiesTypeDef",
     "StartFlowRequestRequestTypeDef",
-    "StartFlowResponseTypeDef",
     "StopFlowRequestRequestTypeDef",
-    "StopFlowResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UnregisterConnectorRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "CustomAuthConfigTypeDef",
+    "CancelFlowExecutionsResponseTypeDef",
+    "CreateConnectorProfileResponseTypeDef",
+    "CreateFlowResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "RegisterConnectorResponseTypeDef",
+    "StartFlowResponseTypeDef",
+    "StopFlowResponseTypeDef",
     "UpdateConnectorProfileResponseTypeDef",
     "UpdateConnectorRegistrationResponseTypeDef",
     "UpdateFlowResponseTypeDef",
-    "CustomAuthConfigTypeDef",
+    "CustomConnectorSourcePropertiesOutputTypeDef",
     "CustomConnectorSourcePropertiesTypeDef",
     "ListConnectorsResponseTypeDef",
     "ListConnectorEntitiesResponseTypeDef",
     "ConnectorMetadataTypeDef",
     "GoogleAnalyticsConnectorProfileCredentialsTypeDef",
     "HoneycodeConnectorProfileCredentialsTypeDef",
     "MarketoConnectorProfileCredentialsTypeDef",
     "OAuth2CredentialsTypeDef",
     "OAuthCredentialsTypeDef",
     "PardotConnectorProfileCredentialsTypeDef",
     "SalesforceConnectorProfileCredentialsTypeDef",
     "SlackConnectorProfileCredentialsTypeDef",
     "ZendeskConnectorProfileCredentialsTypeDef",
+    "TaskOutputTypeDef",
     "TaskTypeDef",
     "ConnectorProvisioningConfigTypeDef",
+    "CustomConnectorDestinationPropertiesOutputTypeDef",
     "CustomConnectorDestinationPropertiesTypeDef",
     "EventBridgeDestinationPropertiesTypeDef",
     "HoneycodeDestinationPropertiesTypeDef",
     "MarketoDestinationPropertiesTypeDef",
     "RedshiftDestinationPropertiesTypeDef",
+    "SalesforceDestinationPropertiesOutputTypeDef",
     "SalesforceDestinationPropertiesTypeDef",
     "SnowflakeDestinationPropertiesTypeDef",
+    "ZendeskDestinationPropertiesOutputTypeDef",
     "ZendeskDestinationPropertiesTypeDef",
+    "CustomConnectorProfilePropertiesOutputTypeDef",
     "CustomConnectorProfilePropertiesTypeDef",
     "FlowDefinitionTypeDef",
     "ExecutionResultTypeDef",
     "FieldTypeDetailsTypeDef",
     "MetadataCatalogConfigTypeDef",
     "MetadataCatalogDetailTypeDef",
     "OAuth2DefaultsTypeDef",
+    "SAPODataConnectorProfilePropertiesOutputTypeDef",
     "SAPODataConnectorProfilePropertiesTypeDef",
+    "S3OutputFormatConfigOutputTypeDef",
+    "UpsolverS3OutputFormatConfigOutputTypeDef",
     "S3OutputFormatConfigTypeDef",
     "UpsolverS3OutputFormatConfigTypeDef",
     "S3SourcePropertiesTypeDef",
+    "SAPODataDestinationPropertiesOutputTypeDef",
     "SAPODataDestinationPropertiesTypeDef",
-    "TriggerPropertiesTypeDef",
+    "TriggerPropertiesOutputTypeDef",
+    "ScheduledTriggerPropertiesTypeDef",
     "CustomConnectorProfileCredentialsTypeDef",
     "SAPODataConnectorProfileCredentialsTypeDef",
+    "TaskUnionTypeDef",
     "RegisterConnectorRequestRequestTypeDef",
     "UpdateConnectorRegistrationRequestRequestTypeDef",
     "ListFlowsResponseTypeDef",
     "SupportedFieldTypeDetailsTypeDef",
     "ExecutionRecordTypeDef",
     "AuthenticationConfigTypeDef",
+    "ConnectorProfilePropertiesOutputTypeDef",
     "ConnectorProfilePropertiesTypeDef",
+    "S3DestinationPropertiesOutputTypeDef",
+    "UpsolverDestinationPropertiesOutputTypeDef",
     "S3DestinationPropertiesTypeDef",
     "UpsolverDestinationPropertiesTypeDef",
+    "SourceConnectorPropertiesOutputTypeDef",
     "SourceConnectorPropertiesTypeDef",
-    "TriggerConfigTypeDef",
+    "TriggerConfigOutputTypeDef",
+    "TriggerPropertiesTypeDef",
     "ConnectorProfileCredentialsTypeDef",
     "ConnectorEntityFieldTypeDef",
     "DescribeFlowExecutionRecordsResponseTypeDef",
     "ConnectorConfigurationTypeDef",
     "ConnectorProfileTypeDef",
+    "DestinationConnectorPropertiesOutputTypeDef",
     "DestinationConnectorPropertiesTypeDef",
+    "SourceFlowConfigOutputTypeDef",
     "SourceFlowConfigTypeDef",
+    "TriggerConfigTypeDef",
     "ConnectorProfileConfigTypeDef",
     "DescribeConnectorEntityResponseTypeDef",
     "DescribeConnectorResponseTypeDef",
     "DescribeConnectorsResponseTypeDef",
     "DescribeConnectorProfilesResponseTypeDef",
+    "DestinationFlowConfigOutputTypeDef",
     "DestinationFlowConfigTypeDef",
+    "SourceFlowConfigUnionTypeDef",
+    "TriggerConfigUnionTypeDef",
     "CreateConnectorProfileRequestRequestTypeDef",
     "UpdateConnectorProfileRequestRequestTypeDef",
-    "CreateFlowRequestRequestTypeDef",
     "DescribeFlowResponseTypeDef",
+    "DestinationFlowConfigUnionTypeDef",
+    "CreateFlowRequestRequestTypeDef",
     "UpdateFlowRequestRequestTypeDef",
 )
 
 AggregationConfigTypeDef = TypedDict(
     "AggregationConfigTypeDef",
     {
         "aggregationType": AggregationTypeType,
@@ -277,21 +304,19 @@
     "_OptionalApiKeyCredentialsTypeDef",
     {
         "apiSecretKey": str,
     },
     total=False,
 )
 
-
 class ApiKeyCredentialsTypeDef(
     _RequiredApiKeyCredentialsTypeDef, _OptionalApiKeyCredentialsTypeDef
 ):
     pass
 
-
 AuthParameterTypeDef = TypedDict(
     "AuthParameterTypeDef",
     {
         "key": str,
         "isRequired": bool,
         "label": str,
         "description": str,
@@ -319,27 +344,28 @@
     "_OptionalCancelFlowExecutionsRequestRequestTypeDef",
     {
         "executionIds": Sequence[str],
     },
     total=False,
 )
 
-
 class CancelFlowExecutionsRequestRequestTypeDef(
     _RequiredCancelFlowExecutionsRequestRequestTypeDef,
     _OptionalCancelFlowExecutionsRequestRequestTypeDef,
 ):
     pass
 
-
-CancelFlowExecutionsResponseTypeDef = TypedDict(
-    "CancelFlowExecutionsResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "invalidExecutions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ConnectorRuntimeSettingTypeDef = TypedDict(
     "ConnectorRuntimeSettingTypeDef",
     {
         "key": str,
@@ -415,19 +441,17 @@
     {
         "label": str,
         "hasNestedEntities": bool,
     },
     total=False,
 )
 
-
 class ConnectorEntityTypeDef(_RequiredConnectorEntityTypeDef, _OptionalConnectorEntityTypeDef):
     pass
 
-
 GoogleAnalyticsMetadataTypeDef = TypedDict(
     "GoogleAnalyticsMetadataTypeDef",
     {
         "oAuthScopes": List[str],
     },
     total=False,
 )
@@ -634,22 +658,20 @@
         "clusterIdentifier": str,
         "workgroupName": str,
         "databaseName": str,
     },
     total=False,
 )
 
-
 class RedshiftConnectorProfilePropertiesTypeDef(
     _RequiredRedshiftConnectorProfilePropertiesTypeDef,
     _OptionalRedshiftConnectorProfilePropertiesTypeDef,
 ):
     pass
 
-
 SalesforceConnectorProfilePropertiesTypeDef = TypedDict(
     "SalesforceConnectorProfilePropertiesTypeDef",
     {
         "instanceUrl": str,
         "isSandboxEnvironment": bool,
         "usePrivateLinkForMetadataAndAuthorization": bool,
     },
@@ -685,22 +707,20 @@
         "privateLinkServiceName": str,
         "accountName": str,
         "region": str,
     },
     total=False,
 )
 
-
 class SnowflakeConnectorProfilePropertiesTypeDef(
     _RequiredSnowflakeConnectorProfilePropertiesTypeDef,
     _OptionalSnowflakeConnectorProfilePropertiesTypeDef,
 ):
     pass
 
-
 VeevaConnectorProfilePropertiesTypeDef = TypedDict(
     "VeevaConnectorProfilePropertiesTypeDef",
     {
         "instanceUrl": str,
     },
 )
 
@@ -724,62 +744,63 @@
 LambdaConnectorProvisioningConfigTypeDef = TypedDict(
     "LambdaConnectorProvisioningConfigTypeDef",
     {
         "lambdaArn": str,
     },
 )
 
-CreateConnectorProfileResponseTypeDef = TypedDict(
-    "CreateConnectorProfileResponseTypeDef",
-    {
-        "connectorProfileArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFlowResponseTypeDef = TypedDict(
-    "CreateFlowResponseTypeDef",
-    {
-        "flowArn": str,
-        "flowStatus": FlowStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCustomAuthCredentialsTypeDef = TypedDict(
     "_RequiredCustomAuthCredentialsTypeDef",
     {
         "customAuthenticationType": str,
     },
 )
 _OptionalCustomAuthCredentialsTypeDef = TypedDict(
     "_OptionalCustomAuthCredentialsTypeDef",
     {
         "credentialsMap": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CustomAuthCredentialsTypeDef(
     _RequiredCustomAuthCredentialsTypeDef, _OptionalCustomAuthCredentialsTypeDef
 ):
     pass
 
-
 ErrorHandlingConfigTypeDef = TypedDict(
     "ErrorHandlingConfigTypeDef",
     {
         "failOnFirstDestinationError": bool,
         "bucketPrefix": str,
         "bucketName": str,
     },
     total=False,
 )
 
+_RequiredOAuth2PropertiesOutputTypeDef = TypedDict(
+    "_RequiredOAuth2PropertiesOutputTypeDef",
+    {
+        "tokenUrl": str,
+        "oAuth2GrantType": OAuth2GrantTypeType,
+    },
+)
+_OptionalOAuth2PropertiesOutputTypeDef = TypedDict(
+    "_OptionalOAuth2PropertiesOutputTypeDef",
+    {
+        "tokenUrlCustomProperties": Dict[str, str],
+    },
+    total=False,
+)
+
+class OAuth2PropertiesOutputTypeDef(
+    _RequiredOAuth2PropertiesOutputTypeDef, _OptionalOAuth2PropertiesOutputTypeDef
+):
+    pass
+
 _RequiredOAuth2PropertiesTypeDef = TypedDict(
     "_RequiredOAuth2PropertiesTypeDef",
     {
         "tokenUrl": str,
         "oAuth2GrantType": OAuth2GrantTypeType,
     },
 )
@@ -787,41 +808,37 @@
     "_OptionalOAuth2PropertiesTypeDef",
     {
         "tokenUrlCustomProperties": Mapping[str, str],
     },
     total=False,
 )
 
-
 class OAuth2PropertiesTypeDef(_RequiredOAuth2PropertiesTypeDef, _OptionalOAuth2PropertiesTypeDef):
     pass
 
-
 _RequiredCustomerProfilesDestinationPropertiesTypeDef = TypedDict(
     "_RequiredCustomerProfilesDestinationPropertiesTypeDef",
     {
         "domainName": str,
     },
 )
 _OptionalCustomerProfilesDestinationPropertiesTypeDef = TypedDict(
     "_OptionalCustomerProfilesDestinationPropertiesTypeDef",
     {
         "objectTypeName": str,
     },
     total=False,
 )
 
-
 class CustomerProfilesDestinationPropertiesTypeDef(
     _RequiredCustomerProfilesDestinationPropertiesTypeDef,
     _OptionalCustomerProfilesDestinationPropertiesTypeDef,
 ):
     pass
 
-
 DatadogSourcePropertiesTypeDef = TypedDict(
     "DatadogSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -835,43 +852,39 @@
     "_OptionalDeleteConnectorProfileRequestRequestTypeDef",
     {
         "forceDelete": bool,
     },
     total=False,
 )
 
-
 class DeleteConnectorProfileRequestRequestTypeDef(
     _RequiredDeleteConnectorProfileRequestRequestTypeDef,
     _OptionalDeleteConnectorProfileRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteFlowRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFlowRequestRequestTypeDef",
     {
         "flowName": str,
     },
 )
 _OptionalDeleteFlowRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteFlowRequestRequestTypeDef",
     {
         "forceDelete": bool,
     },
     total=False,
 )
 
-
 class DeleteFlowRequestRequestTypeDef(
     _RequiredDeleteFlowRequestRequestTypeDef, _OptionalDeleteFlowRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDescribeConnectorEntityRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConnectorEntityRequestRequestTypeDef",
     {
         "connectorEntityName": str,
     },
 )
 _OptionalDescribeConnectorEntityRequestRequestTypeDef = TypedDict(
@@ -880,22 +893,20 @@
         "connectorType": ConnectorTypeType,
         "connectorProfileName": str,
         "apiVersion": str,
     },
     total=False,
 )
 
-
 class DescribeConnectorEntityRequestRequestTypeDef(
     _RequiredDescribeConnectorEntityRequestRequestTypeDef,
     _OptionalDescribeConnectorEntityRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeConnectorProfilesRequestRequestTypeDef = TypedDict(
     "DescribeConnectorProfilesRequestRequestTypeDef",
     {
         "connectorProfileNames": Sequence[str],
         "connectorType": ConnectorTypeType,
         "connectorLabel": str,
         "maxResults": int,
@@ -914,21 +925,19 @@
     "_OptionalDescribeConnectorRequestRequestTypeDef",
     {
         "connectorLabel": str,
     },
     total=False,
 )
 
-
 class DescribeConnectorRequestRequestTypeDef(
     _RequiredDescribeConnectorRequestRequestTypeDef, _OptionalDescribeConnectorRequestRequestTypeDef
 ):
     pass
 
-
 DescribeConnectorsRequestRequestTypeDef = TypedDict(
     "DescribeConnectorsRequestRequestTypeDef",
     {
         "connectorTypes": Sequence[ConnectorTypeType],
         "maxResults": int,
         "nextToken": str,
     },
@@ -946,22 +955,20 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class DescribeFlowExecutionRecordsRequestRequestTypeDef(
     _RequiredDescribeFlowExecutionRecordsRequestRequestTypeDef,
     _OptionalDescribeFlowExecutionRecordsRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeFlowRequestRequestTypeDef = TypedDict(
     "DescribeFlowRequestRequestTypeDef",
     {
         "flowName": str,
     },
 )
 
@@ -1065,22 +1072,14 @@
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
 MarketoSourcePropertiesTypeDef = TypedDict(
     "MarketoSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -1104,14 +1103,23 @@
         "isSensitiveField": bool,
         "connectorSuppliedValues": List[str],
         "type": OAuth2CustomPropTypeType,
     },
     total=False,
 )
 
+OAuthPropertiesOutputTypeDef = TypedDict(
+    "OAuthPropertiesOutputTypeDef",
+    {
+        "tokenUrl": str,
+        "authCodeUrl": str,
+        "oAuthScopes": List[str],
+    },
+)
+
 OAuthPropertiesTypeDef = TypedDict(
     "OAuthPropertiesTypeDef",
     {
         "tokenUrl": str,
         "authCodeUrl": str,
         "oAuthScopes": Sequence[str],
     },
@@ -1120,55 +1128,46 @@
 PardotSourcePropertiesTypeDef = TypedDict(
     "PardotSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
-PrefixConfigTypeDef = TypedDict(
-    "PrefixConfigTypeDef",
+PrefixConfigOutputTypeDef = TypedDict(
+    "PrefixConfigOutputTypeDef",
     {
         "prefixType": PrefixTypeType,
         "prefixFormat": PrefixFormatType,
-        "pathPrefixHierarchy": Sequence[PathPrefixType],
+        "pathPrefixHierarchy": List[PathPrefixType],
     },
     total=False,
 )
 
-RegisterConnectorResponseTypeDef = TypedDict(
-    "RegisterConnectorResponseTypeDef",
+PrefixConfigTypeDef = TypedDict(
+    "PrefixConfigTypeDef",
     {
-        "connectorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "prefixType": PrefixTypeType,
+        "prefixFormat": PrefixFormatType,
+        "pathPrefixHierarchy": Sequence[PathPrefixType],
     },
+    total=False,
 )
 
 ResetConnectorMetadataCacheRequestRequestTypeDef = TypedDict(
     "ResetConnectorMetadataCacheRequestRequestTypeDef",
     {
         "connectorProfileName": str,
         "connectorType": ConnectorTypeType,
         "connectorEntityName": str,
         "entitiesPath": str,
         "apiVersion": str,
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
 S3InputFormatConfigTypeDef = TypedDict(
     "S3InputFormatConfigTypeDef",
     {
         "s3InputFileType": S3InputFileTypeType,
     },
     total=False,
 )
@@ -1202,48 +1201,46 @@
         "enableDynamicFieldUpdate": bool,
         "includeDeletedRecords": bool,
         "dataTransferApi": SalesforceDataTransferApiType,
     },
     total=False,
 )
 
-
 class SalesforceSourcePropertiesTypeDef(
     _RequiredSalesforceSourcePropertiesTypeDef, _OptionalSalesforceSourcePropertiesTypeDef
 ):
     pass
 
-
-_RequiredScheduledTriggerPropertiesTypeDef = TypedDict(
-    "_RequiredScheduledTriggerPropertiesTypeDef",
+_RequiredScheduledTriggerPropertiesOutputTypeDef = TypedDict(
+    "_RequiredScheduledTriggerPropertiesOutputTypeDef",
     {
         "scheduleExpression": str,
     },
 )
-_OptionalScheduledTriggerPropertiesTypeDef = TypedDict(
-    "_OptionalScheduledTriggerPropertiesTypeDef",
+_OptionalScheduledTriggerPropertiesOutputTypeDef = TypedDict(
+    "_OptionalScheduledTriggerPropertiesOutputTypeDef",
     {
         "dataPullMode": DataPullModeType,
-        "scheduleStartTime": Union[datetime, str],
-        "scheduleEndTime": Union[datetime, str],
+        "scheduleStartTime": datetime,
+        "scheduleEndTime": datetime,
         "timezone": str,
         "scheduleOffset": int,
-        "firstExecutionFrom": Union[datetime, str],
+        "firstExecutionFrom": datetime,
         "flowErrorDeactivationThreshold": int,
     },
     total=False,
 )
 
-
-class ScheduledTriggerPropertiesTypeDef(
-    _RequiredScheduledTriggerPropertiesTypeDef, _OptionalScheduledTriggerPropertiesTypeDef
+class ScheduledTriggerPropertiesOutputTypeDef(
+    _RequiredScheduledTriggerPropertiesOutputTypeDef,
+    _OptionalScheduledTriggerPropertiesOutputTypeDef,
 ):
     pass
 
-
+TimestampTypeDef = Union[datetime, str]
 ServiceNowSourcePropertiesTypeDef = TypedDict(
     "ServiceNowSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -1281,21 +1278,19 @@
         "includeSourceFiles": bool,
         "includeRenditions": bool,
         "includeAllVersions": bool,
     },
     total=False,
 )
 
-
 class VeevaSourcePropertiesTypeDef(
     _RequiredVeevaSourcePropertiesTypeDef, _OptionalVeevaSourcePropertiesTypeDef
 ):
     pass
 
-
 ZendeskSourcePropertiesTypeDef = TypedDict(
     "ZendeskSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -1309,47 +1304,26 @@
     "_OptionalStartFlowRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class StartFlowRequestRequestTypeDef(
     _RequiredStartFlowRequestRequestTypeDef, _OptionalStartFlowRequestRequestTypeDef
 ):
     pass
 
-
-StartFlowResponseTypeDef = TypedDict(
-    "StartFlowResponseTypeDef",
-    {
-        "flowArn": str,
-        "flowStatus": FlowStatusType,
-        "executionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopFlowRequestRequestTypeDef = TypedDict(
     "StopFlowRequestRequestTypeDef",
     {
         "flowName": str,
     },
 )
 
-StopFlowResponseTypeDef = TypedDict(
-    "StopFlowResponseTypeDef",
-    {
-        "flowArn": str,
-        "flowStatus": FlowStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1364,63 +1338,142 @@
     "_OptionalUnregisterConnectorRequestRequestTypeDef",
     {
         "forceDelete": bool,
     },
     total=False,
 )
 
-
 class UnregisterConnectorRequestRequestTypeDef(
     _RequiredUnregisterConnectorRequestRequestTypeDef,
     _OptionalUnregisterConnectorRequestRequestTypeDef,
 ):
     pass
 
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+CustomAuthConfigTypeDef = TypedDict(
+    "CustomAuthConfigTypeDef",
+    {
+        "customAuthenticationType": str,
+        "authParameters": List[AuthParameterTypeDef],
+    },
+    total=False,
+)
+
+CancelFlowExecutionsResponseTypeDef = TypedDict(
+    "CancelFlowExecutionsResponseTypeDef",
+    {
+        "invalidExecutions": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateConnectorProfileResponseTypeDef = TypedDict(
+    "CreateConnectorProfileResponseTypeDef",
+    {
+        "connectorProfileArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFlowResponseTypeDef = TypedDict(
+    "CreateFlowResponseTypeDef",
+    {
+        "flowArn": str,
+        "flowStatus": FlowStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterConnectorResponseTypeDef = TypedDict(
+    "RegisterConnectorResponseTypeDef",
+    {
+        "connectorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartFlowResponseTypeDef = TypedDict(
+    "StartFlowResponseTypeDef",
+    {
+        "flowArn": str,
+        "flowStatus": FlowStatusType,
+        "executionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopFlowResponseTypeDef = TypedDict(
+    "StopFlowResponseTypeDef",
+    {
+        "flowArn": str,
+        "flowStatus": FlowStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateConnectorProfileResponseTypeDef = TypedDict(
     "UpdateConnectorProfileResponseTypeDef",
     {
         "connectorProfileArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConnectorRegistrationResponseTypeDef = TypedDict(
     "UpdateConnectorRegistrationResponseTypeDef",
     {
         "connectorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFlowResponseTypeDef = TypedDict(
     "UpdateFlowResponseTypeDef",
     {
         "flowStatus": FlowStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CustomAuthConfigTypeDef = TypedDict(
-    "CustomAuthConfigTypeDef",
+_RequiredCustomConnectorSourcePropertiesOutputTypeDef = TypedDict(
+    "_RequiredCustomConnectorSourcePropertiesOutputTypeDef",
     {
-        "customAuthenticationType": str,
-        "authParameters": List[AuthParameterTypeDef],
+        "entityName": str,
+    },
+)
+_OptionalCustomConnectorSourcePropertiesOutputTypeDef = TypedDict(
+    "_OptionalCustomConnectorSourcePropertiesOutputTypeDef",
+    {
+        "customProperties": Dict[str, str],
+        "dataTransferApi": DataTransferApiTypeDef,
     },
     total=False,
 )
 
+class CustomConnectorSourcePropertiesOutputTypeDef(
+    _RequiredCustomConnectorSourcePropertiesOutputTypeDef,
+    _OptionalCustomConnectorSourcePropertiesOutputTypeDef,
+):
+    pass
+
 _RequiredCustomConnectorSourcePropertiesTypeDef = TypedDict(
     "_RequiredCustomConnectorSourcePropertiesTypeDef",
     {
         "entityName": str,
     },
 )
 _OptionalCustomConnectorSourcePropertiesTypeDef = TypedDict(
@@ -1428,36 +1481,34 @@
     {
         "customProperties": Mapping[str, str],
         "dataTransferApi": DataTransferApiTypeDef,
     },
     total=False,
 )
 
-
 class CustomConnectorSourcePropertiesTypeDef(
     _RequiredCustomConnectorSourcePropertiesTypeDef, _OptionalCustomConnectorSourcePropertiesTypeDef
 ):
     pass
 
-
 ListConnectorsResponseTypeDef = TypedDict(
     "ListConnectorsResponseTypeDef",
     {
         "connectors": List[ConnectorDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConnectorEntitiesResponseTypeDef = TypedDict(
     "ListConnectorEntitiesResponseTypeDef",
     {
         "connectorEntityMap": Dict[str, List[ConnectorEntityTypeDef]],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConnectorMetadataTypeDef = TypedDict(
     "ConnectorMetadataTypeDef",
     {
         "Amplitude": Dict[str, Any],
@@ -1499,22 +1550,20 @@
         "accessToken": str,
         "refreshToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
     total=False,
 )
 
-
 class GoogleAnalyticsConnectorProfileCredentialsTypeDef(
     _RequiredGoogleAnalyticsConnectorProfileCredentialsTypeDef,
     _OptionalGoogleAnalyticsConnectorProfileCredentialsTypeDef,
 ):
     pass
 
-
 HoneycodeConnectorProfileCredentialsTypeDef = TypedDict(
     "HoneycodeConnectorProfileCredentialsTypeDef",
     {
         "accessToken": str,
         "refreshToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
@@ -1533,22 +1582,20 @@
     {
         "accessToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
     total=False,
 )
 
-
 class MarketoConnectorProfileCredentialsTypeDef(
     _RequiredMarketoConnectorProfileCredentialsTypeDef,
     _OptionalMarketoConnectorProfileCredentialsTypeDef,
 ):
     pass
 
-
 OAuth2CredentialsTypeDef = TypedDict(
     "OAuth2CredentialsTypeDef",
     {
         "clientId": str,
         "clientSecret": str,
         "accessToken": str,
         "refreshToken": str,
@@ -1570,19 +1617,17 @@
         "accessToken": str,
         "refreshToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
     total=False,
 )
 
-
 class OAuthCredentialsTypeDef(_RequiredOAuthCredentialsTypeDef, _OptionalOAuthCredentialsTypeDef):
     pass
 
-
 PardotConnectorProfileCredentialsTypeDef = TypedDict(
     "PardotConnectorProfileCredentialsTypeDef",
     {
         "accessToken": str,
         "refreshToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
         "clientCredentialsArn": str,
@@ -1615,22 +1660,20 @@
     {
         "accessToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
     total=False,
 )
 
-
 class SlackConnectorProfileCredentialsTypeDef(
     _RequiredSlackConnectorProfileCredentialsTypeDef,
     _OptionalSlackConnectorProfileCredentialsTypeDef,
 ):
     pass
 
-
 _RequiredZendeskConnectorProfileCredentialsTypeDef = TypedDict(
     "_RequiredZendeskConnectorProfileCredentialsTypeDef",
     {
         "clientId": str,
         "clientSecret": str,
     },
 )
@@ -1639,21 +1682,39 @@
     {
         "accessToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
     total=False,
 )
 
-
 class ZendeskConnectorProfileCredentialsTypeDef(
     _RequiredZendeskConnectorProfileCredentialsTypeDef,
     _OptionalZendeskConnectorProfileCredentialsTypeDef,
 ):
     pass
 
+_RequiredTaskOutputTypeDef = TypedDict(
+    "_RequiredTaskOutputTypeDef",
+    {
+        "sourceFields": List[str],
+        "taskType": TaskTypeType,
+    },
+)
+_OptionalTaskOutputTypeDef = TypedDict(
+    "_OptionalTaskOutputTypeDef",
+    {
+        "connectorOperator": ConnectorOperatorTypeDef,
+        "destinationField": str,
+        "taskProperties": Dict[OperatorPropertiesKeysType, str],
+    },
+    total=False,
+)
+
+class TaskOutputTypeDef(_RequiredTaskOutputTypeDef, _OptionalTaskOutputTypeDef):
+    pass
 
 _RequiredTaskTypeDef = TypedDict(
     "_RequiredTaskTypeDef",
     {
         "sourceFields": Sequence[str],
         "taskType": TaskTypeType,
     },
@@ -1664,27 +1725,48 @@
         "connectorOperator": ConnectorOperatorTypeDef,
         "destinationField": str,
         "taskProperties": Mapping[OperatorPropertiesKeysType, str],
     },
     total=False,
 )
 
-
 class TaskTypeDef(_RequiredTaskTypeDef, _OptionalTaskTypeDef):
     pass
 
-
 ConnectorProvisioningConfigTypeDef = TypedDict(
     "ConnectorProvisioningConfigTypeDef",
     {
         "lambda": LambdaConnectorProvisioningConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredCustomConnectorDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredCustomConnectorDestinationPropertiesOutputTypeDef",
+    {
+        "entityName": str,
+    },
+)
+_OptionalCustomConnectorDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalCustomConnectorDestinationPropertiesOutputTypeDef",
+    {
+        "errorHandlingConfig": ErrorHandlingConfigTypeDef,
+        "writeOperationType": WriteOperationTypeType,
+        "idFieldNames": List[str],
+        "customProperties": Dict[str, str],
+    },
+    total=False,
+)
+
+class CustomConnectorDestinationPropertiesOutputTypeDef(
+    _RequiredCustomConnectorDestinationPropertiesOutputTypeDef,
+    _OptionalCustomConnectorDestinationPropertiesOutputTypeDef,
+):
+    pass
+
 _RequiredCustomConnectorDestinationPropertiesTypeDef = TypedDict(
     "_RequiredCustomConnectorDestinationPropertiesTypeDef",
     {
         "entityName": str,
     },
 )
 _OptionalCustomConnectorDestinationPropertiesTypeDef = TypedDict(
@@ -1694,86 +1776,78 @@
         "writeOperationType": WriteOperationTypeType,
         "idFieldNames": Sequence[str],
         "customProperties": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CustomConnectorDestinationPropertiesTypeDef(
     _RequiredCustomConnectorDestinationPropertiesTypeDef,
     _OptionalCustomConnectorDestinationPropertiesTypeDef,
 ):
     pass
 
-
 _RequiredEventBridgeDestinationPropertiesTypeDef = TypedDict(
     "_RequiredEventBridgeDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalEventBridgeDestinationPropertiesTypeDef = TypedDict(
     "_OptionalEventBridgeDestinationPropertiesTypeDef",
     {
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
     },
     total=False,
 )
 
-
 class EventBridgeDestinationPropertiesTypeDef(
     _RequiredEventBridgeDestinationPropertiesTypeDef,
     _OptionalEventBridgeDestinationPropertiesTypeDef,
 ):
     pass
 
-
 _RequiredHoneycodeDestinationPropertiesTypeDef = TypedDict(
     "_RequiredHoneycodeDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalHoneycodeDestinationPropertiesTypeDef = TypedDict(
     "_OptionalHoneycodeDestinationPropertiesTypeDef",
     {
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
     },
     total=False,
 )
 
-
 class HoneycodeDestinationPropertiesTypeDef(
     _RequiredHoneycodeDestinationPropertiesTypeDef, _OptionalHoneycodeDestinationPropertiesTypeDef
 ):
     pass
 
-
 _RequiredMarketoDestinationPropertiesTypeDef = TypedDict(
     "_RequiredMarketoDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalMarketoDestinationPropertiesTypeDef = TypedDict(
     "_OptionalMarketoDestinationPropertiesTypeDef",
     {
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
     },
     total=False,
 )
 
-
 class MarketoDestinationPropertiesTypeDef(
     _RequiredMarketoDestinationPropertiesTypeDef, _OptionalMarketoDestinationPropertiesTypeDef
 ):
     pass
 
-
 _RequiredRedshiftDestinationPropertiesTypeDef = TypedDict(
     "_RequiredRedshiftDestinationPropertiesTypeDef",
     {
         "object": str,
         "intermediateBucketName": str,
     },
 )
@@ -1782,20 +1856,41 @@
     {
         "bucketPrefix": str,
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
     },
     total=False,
 )
 
-
 class RedshiftDestinationPropertiesTypeDef(
     _RequiredRedshiftDestinationPropertiesTypeDef, _OptionalRedshiftDestinationPropertiesTypeDef
 ):
     pass
 
+_RequiredSalesforceDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredSalesforceDestinationPropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+_OptionalSalesforceDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalSalesforceDestinationPropertiesOutputTypeDef",
+    {
+        "idFieldNames": List[str],
+        "errorHandlingConfig": ErrorHandlingConfigTypeDef,
+        "writeOperationType": WriteOperationTypeType,
+        "dataTransferApi": SalesforceDataTransferApiType,
+    },
+    total=False,
+)
+
+class SalesforceDestinationPropertiesOutputTypeDef(
+    _RequiredSalesforceDestinationPropertiesOutputTypeDef,
+    _OptionalSalesforceDestinationPropertiesOutputTypeDef,
+):
+    pass
 
 _RequiredSalesforceDestinationPropertiesTypeDef = TypedDict(
     "_RequiredSalesforceDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
@@ -1806,21 +1901,19 @@
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
         "writeOperationType": WriteOperationTypeType,
         "dataTransferApi": SalesforceDataTransferApiType,
     },
     total=False,
 )
 
-
 class SalesforceDestinationPropertiesTypeDef(
     _RequiredSalesforceDestinationPropertiesTypeDef, _OptionalSalesforceDestinationPropertiesTypeDef
 ):
     pass
 
-
 _RequiredSnowflakeDestinationPropertiesTypeDef = TypedDict(
     "_RequiredSnowflakeDestinationPropertiesTypeDef",
     {
         "object": str,
         "intermediateBucketName": str,
     },
 )
@@ -1829,20 +1922,40 @@
     {
         "bucketPrefix": str,
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
     },
     total=False,
 )
 
-
 class SnowflakeDestinationPropertiesTypeDef(
     _RequiredSnowflakeDestinationPropertiesTypeDef, _OptionalSnowflakeDestinationPropertiesTypeDef
 ):
     pass
 
+_RequiredZendeskDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredZendeskDestinationPropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+_OptionalZendeskDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalZendeskDestinationPropertiesOutputTypeDef",
+    {
+        "idFieldNames": List[str],
+        "errorHandlingConfig": ErrorHandlingConfigTypeDef,
+        "writeOperationType": WriteOperationTypeType,
+    },
+    total=False,
+)
+
+class ZendeskDestinationPropertiesOutputTypeDef(
+    _RequiredZendeskDestinationPropertiesOutputTypeDef,
+    _OptionalZendeskDestinationPropertiesOutputTypeDef,
+):
+    pass
 
 _RequiredZendeskDestinationPropertiesTypeDef = TypedDict(
     "_RequiredZendeskDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
@@ -1852,20 +1965,27 @@
         "idFieldNames": Sequence[str],
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
         "writeOperationType": WriteOperationTypeType,
     },
     total=False,
 )
 
-
 class ZendeskDestinationPropertiesTypeDef(
     _RequiredZendeskDestinationPropertiesTypeDef, _OptionalZendeskDestinationPropertiesTypeDef
 ):
     pass
 
+CustomConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "CustomConnectorProfilePropertiesOutputTypeDef",
+    {
+        "profileProperties": Dict[str, str],
+        "oAuth2Properties": OAuth2PropertiesOutputTypeDef,
+    },
+    total=False,
+)
 
 CustomConnectorProfilePropertiesTypeDef = TypedDict(
     "CustomConnectorProfilePropertiesTypeDef",
     {
         "profileProperties": Mapping[str, str],
         "oAuth2Properties": OAuth2PropertiesTypeDef,
     },
@@ -1920,19 +2040,17 @@
         "supportedDateFormat": str,
         "fieldValueRange": RangeTypeDef,
         "fieldLengthRange": RangeTypeDef,
     },
     total=False,
 )
 
-
 class FieldTypeDetailsTypeDef(_RequiredFieldTypeDetailsTypeDef, _OptionalFieldTypeDetailsTypeDef):
     pass
 
-
 MetadataCatalogConfigTypeDef = TypedDict(
     "MetadataCatalogConfigTypeDef",
     {
         "glueDataCatalog": GlueDataCatalogConfigTypeDef,
     },
     total=False,
 )
@@ -1956,14 +2074,39 @@
         "authCodeUrls": List[str],
         "oauth2GrantTypesSupported": List[OAuth2GrantTypeType],
         "oauth2CustomProperties": List[OAuth2CustomParameterTypeDef],
     },
     total=False,
 )
 
+_RequiredSAPODataConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "_RequiredSAPODataConnectorProfilePropertiesOutputTypeDef",
+    {
+        "applicationHostUrl": str,
+        "applicationServicePath": str,
+        "portNumber": int,
+        "clientNumber": str,
+    },
+)
+_OptionalSAPODataConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "_OptionalSAPODataConnectorProfilePropertiesOutputTypeDef",
+    {
+        "logonLanguage": str,
+        "privateLinkServiceName": str,
+        "oAuthProperties": OAuthPropertiesOutputTypeDef,
+    },
+    total=False,
+)
+
+class SAPODataConnectorProfilePropertiesOutputTypeDef(
+    _RequiredSAPODataConnectorProfilePropertiesOutputTypeDef,
+    _OptionalSAPODataConnectorProfilePropertiesOutputTypeDef,
+):
+    pass
+
 _RequiredSAPODataConnectorProfilePropertiesTypeDef = TypedDict(
     "_RequiredSAPODataConnectorProfilePropertiesTypeDef",
     {
         "applicationHostUrl": str,
         "applicationServicePath": str,
         "portNumber": int,
         "clientNumber": str,
@@ -1975,21 +2118,51 @@
         "logonLanguage": str,
         "privateLinkServiceName": str,
         "oAuthProperties": OAuthPropertiesTypeDef,
     },
     total=False,
 )
 
-
 class SAPODataConnectorProfilePropertiesTypeDef(
     _RequiredSAPODataConnectorProfilePropertiesTypeDef,
     _OptionalSAPODataConnectorProfilePropertiesTypeDef,
 ):
     pass
 
+S3OutputFormatConfigOutputTypeDef = TypedDict(
+    "S3OutputFormatConfigOutputTypeDef",
+    {
+        "fileType": FileTypeType,
+        "prefixConfig": PrefixConfigOutputTypeDef,
+        "aggregationConfig": AggregationConfigTypeDef,
+        "preserveSourceDataTyping": bool,
+    },
+    total=False,
+)
+
+_RequiredUpsolverS3OutputFormatConfigOutputTypeDef = TypedDict(
+    "_RequiredUpsolverS3OutputFormatConfigOutputTypeDef",
+    {
+        "prefixConfig": PrefixConfigOutputTypeDef,
+    },
+)
+_OptionalUpsolverS3OutputFormatConfigOutputTypeDef = TypedDict(
+    "_OptionalUpsolverS3OutputFormatConfigOutputTypeDef",
+    {
+        "fileType": FileTypeType,
+        "aggregationConfig": AggregationConfigTypeDef,
+    },
+    total=False,
+)
+
+class UpsolverS3OutputFormatConfigOutputTypeDef(
+    _RequiredUpsolverS3OutputFormatConfigOutputTypeDef,
+    _OptionalUpsolverS3OutputFormatConfigOutputTypeDef,
+):
+    pass
 
 S3OutputFormatConfigTypeDef = TypedDict(
     "S3OutputFormatConfigTypeDef",
     {
         "fileType": FileTypeType,
         "prefixConfig": PrefixConfigTypeDef,
         "aggregationConfig": AggregationConfigTypeDef,
@@ -2009,21 +2182,19 @@
     {
         "fileType": FileTypeType,
         "aggregationConfig": AggregationConfigTypeDef,
     },
     total=False,
 )
 
-
 class UpsolverS3OutputFormatConfigTypeDef(
     _RequiredUpsolverS3OutputFormatConfigTypeDef, _OptionalUpsolverS3OutputFormatConfigTypeDef
 ):
     pass
 
-
 _RequiredS3SourcePropertiesTypeDef = TypedDict(
     "_RequiredS3SourcePropertiesTypeDef",
     {
         "bucketName": str,
     },
 )
 _OptionalS3SourcePropertiesTypeDef = TypedDict(
@@ -2031,20 +2202,41 @@
     {
         "bucketPrefix": str,
         "s3InputFormatConfig": S3InputFormatConfigTypeDef,
     },
     total=False,
 )
 
-
 class S3SourcePropertiesTypeDef(
     _RequiredS3SourcePropertiesTypeDef, _OptionalS3SourcePropertiesTypeDef
 ):
     pass
 
+_RequiredSAPODataDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredSAPODataDestinationPropertiesOutputTypeDef",
+    {
+        "objectPath": str,
+    },
+)
+_OptionalSAPODataDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalSAPODataDestinationPropertiesOutputTypeDef",
+    {
+        "successResponseHandlingConfig": SuccessResponseHandlingConfigTypeDef,
+        "idFieldNames": List[str],
+        "errorHandlingConfig": ErrorHandlingConfigTypeDef,
+        "writeOperationType": WriteOperationTypeType,
+    },
+    total=False,
+)
+
+class SAPODataDestinationPropertiesOutputTypeDef(
+    _RequiredSAPODataDestinationPropertiesOutputTypeDef,
+    _OptionalSAPODataDestinationPropertiesOutputTypeDef,
+):
+    pass
 
 _RequiredSAPODataDestinationPropertiesTypeDef = TypedDict(
     "_RequiredSAPODataDestinationPropertiesTypeDef",
     {
         "objectPath": str,
     },
 )
@@ -2055,29 +2247,52 @@
         "idFieldNames": Sequence[str],
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
         "writeOperationType": WriteOperationTypeType,
     },
     total=False,
 )
 
-
 class SAPODataDestinationPropertiesTypeDef(
     _RequiredSAPODataDestinationPropertiesTypeDef, _OptionalSAPODataDestinationPropertiesTypeDef
 ):
     pass
 
+TriggerPropertiesOutputTypeDef = TypedDict(
+    "TriggerPropertiesOutputTypeDef",
+    {
+        "Scheduled": ScheduledTriggerPropertiesOutputTypeDef,
+    },
+    total=False,
+)
 
-TriggerPropertiesTypeDef = TypedDict(
-    "TriggerPropertiesTypeDef",
+_RequiredScheduledTriggerPropertiesTypeDef = TypedDict(
+    "_RequiredScheduledTriggerPropertiesTypeDef",
     {
-        "Scheduled": ScheduledTriggerPropertiesTypeDef,
+        "scheduleExpression": str,
+    },
+)
+_OptionalScheduledTriggerPropertiesTypeDef = TypedDict(
+    "_OptionalScheduledTriggerPropertiesTypeDef",
+    {
+        "dataPullMode": DataPullModeType,
+        "scheduleStartTime": TimestampTypeDef,
+        "scheduleEndTime": TimestampTypeDef,
+        "timezone": str,
+        "scheduleOffset": int,
+        "firstExecutionFrom": TimestampTypeDef,
+        "flowErrorDeactivationThreshold": int,
     },
     total=False,
 )
 
+class ScheduledTriggerPropertiesTypeDef(
+    _RequiredScheduledTriggerPropertiesTypeDef, _OptionalScheduledTriggerPropertiesTypeDef
+):
+    pass
+
 _RequiredCustomConnectorProfileCredentialsTypeDef = TypedDict(
     "_RequiredCustomConnectorProfileCredentialsTypeDef",
     {
         "authenticationType": AuthenticationTypeType,
     },
 )
 _OptionalCustomConnectorProfileCredentialsTypeDef = TypedDict(
@@ -2087,31 +2302,30 @@
         "oauth2": OAuth2CredentialsTypeDef,
         "apiKey": ApiKeyCredentialsTypeDef,
         "custom": CustomAuthCredentialsTypeDef,
     },
     total=False,
 )
 
-
 class CustomConnectorProfileCredentialsTypeDef(
     _RequiredCustomConnectorProfileCredentialsTypeDef,
     _OptionalCustomConnectorProfileCredentialsTypeDef,
 ):
     pass
 
-
 SAPODataConnectorProfileCredentialsTypeDef = TypedDict(
     "SAPODataConnectorProfileCredentialsTypeDef",
     {
         "basicAuthCredentials": BasicAuthCredentialsTypeDef,
         "oAuthCredentials": OAuthCredentialsTypeDef,
     },
     total=False,
 )
 
+TaskUnionTypeDef = Union[TaskTypeDef, TaskOutputTypeDef]
 RegisterConnectorRequestRequestTypeDef = TypedDict(
     "RegisterConnectorRequestRequestTypeDef",
     {
         "connectorLabel": str,
         "description": str,
         "connectorProvisioningType": Literal["LAMBDA"],
         "connectorProvisioningConfig": ConnectorProvisioningConfigTypeDef,
@@ -2132,28 +2346,26 @@
         "description": str,
         "connectorProvisioningConfig": ConnectorProvisioningConfigTypeDef,
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateConnectorRegistrationRequestRequestTypeDef(
     _RequiredUpdateConnectorRegistrationRequestRequestTypeDef,
     _OptionalUpdateConnectorRegistrationRequestRequestTypeDef,
 ):
     pass
 
-
 ListFlowsResponseTypeDef = TypedDict(
     "ListFlowsResponseTypeDef",
     {
         "flows": List[FlowDefinitionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SupportedFieldTypeDetailsTypeDef = TypedDict(
     "SupportedFieldTypeDetailsTypeDef",
     {
         "v1": FieldTypeDetailsTypeDef,
@@ -2184,14 +2396,40 @@
         "isCustomAuthSupported": bool,
         "oAuth2Defaults": OAuth2DefaultsTypeDef,
         "customAuthConfigs": List[CustomAuthConfigTypeDef],
     },
     total=False,
 )
 
+ConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "ConnectorProfilePropertiesOutputTypeDef",
+    {
+        "Amplitude": Dict[str, Any],
+        "Datadog": DatadogConnectorProfilePropertiesTypeDef,
+        "Dynatrace": DynatraceConnectorProfilePropertiesTypeDef,
+        "GoogleAnalytics": Dict[str, Any],
+        "Honeycode": Dict[str, Any],
+        "InforNexus": InforNexusConnectorProfilePropertiesTypeDef,
+        "Marketo": MarketoConnectorProfilePropertiesTypeDef,
+        "Redshift": RedshiftConnectorProfilePropertiesTypeDef,
+        "Salesforce": SalesforceConnectorProfilePropertiesTypeDef,
+        "ServiceNow": ServiceNowConnectorProfilePropertiesTypeDef,
+        "Singular": Dict[str, Any],
+        "Slack": SlackConnectorProfilePropertiesTypeDef,
+        "Snowflake": SnowflakeConnectorProfilePropertiesTypeDef,
+        "Trendmicro": Dict[str, Any],
+        "Veeva": VeevaConnectorProfilePropertiesTypeDef,
+        "Zendesk": ZendeskConnectorProfilePropertiesTypeDef,
+        "SAPOData": SAPODataConnectorProfilePropertiesOutputTypeDef,
+        "CustomConnector": CustomConnectorProfilePropertiesOutputTypeDef,
+        "Pardot": PardotConnectorProfilePropertiesTypeDef,
+    },
+    total=False,
+)
+
 ConnectorProfilePropertiesTypeDef = TypedDict(
     "ConnectorProfilePropertiesTypeDef",
     {
         "Amplitude": Mapping[str, Any],
         "Datadog": DatadogConnectorProfilePropertiesTypeDef,
         "Dynatrace": DynatraceConnectorProfilePropertiesTypeDef,
         "GoogleAnalytics": Mapping[str, Any],
@@ -2210,14 +2448,55 @@
         "SAPOData": SAPODataConnectorProfilePropertiesTypeDef,
         "CustomConnector": CustomConnectorProfilePropertiesTypeDef,
         "Pardot": PardotConnectorProfilePropertiesTypeDef,
     },
     total=False,
 )
 
+_RequiredS3DestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredS3DestinationPropertiesOutputTypeDef",
+    {
+        "bucketName": str,
+    },
+)
+_OptionalS3DestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalS3DestinationPropertiesOutputTypeDef",
+    {
+        "bucketPrefix": str,
+        "s3OutputFormatConfig": S3OutputFormatConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class S3DestinationPropertiesOutputTypeDef(
+    _RequiredS3DestinationPropertiesOutputTypeDef, _OptionalS3DestinationPropertiesOutputTypeDef
+):
+    pass
+
+_RequiredUpsolverDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredUpsolverDestinationPropertiesOutputTypeDef",
+    {
+        "bucketName": str,
+        "s3OutputFormatConfig": UpsolverS3OutputFormatConfigOutputTypeDef,
+    },
+)
+_OptionalUpsolverDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalUpsolverDestinationPropertiesOutputTypeDef",
+    {
+        "bucketPrefix": str,
+    },
+    total=False,
+)
+
+class UpsolverDestinationPropertiesOutputTypeDef(
+    _RequiredUpsolverDestinationPropertiesOutputTypeDef,
+    _OptionalUpsolverDestinationPropertiesOutputTypeDef,
+):
+    pass
+
 _RequiredS3DestinationPropertiesTypeDef = TypedDict(
     "_RequiredS3DestinationPropertiesTypeDef",
     {
         "bucketName": str,
     },
 )
 _OptionalS3DestinationPropertiesTypeDef = TypedDict(
@@ -2225,21 +2504,19 @@
     {
         "bucketPrefix": str,
         "s3OutputFormatConfig": S3OutputFormatConfigTypeDef,
     },
     total=False,
 )
 
-
 class S3DestinationPropertiesTypeDef(
     _RequiredS3DestinationPropertiesTypeDef, _OptionalS3DestinationPropertiesTypeDef
 ):
     pass
 
-
 _RequiredUpsolverDestinationPropertiesTypeDef = TypedDict(
     "_RequiredUpsolverDestinationPropertiesTypeDef",
     {
         "bucketName": str,
         "s3OutputFormatConfig": UpsolverS3OutputFormatConfigTypeDef,
     },
 )
@@ -2247,20 +2524,42 @@
     "_OptionalUpsolverDestinationPropertiesTypeDef",
     {
         "bucketPrefix": str,
     },
     total=False,
 )
 
-
 class UpsolverDestinationPropertiesTypeDef(
     _RequiredUpsolverDestinationPropertiesTypeDef, _OptionalUpsolverDestinationPropertiesTypeDef
 ):
     pass
 
+SourceConnectorPropertiesOutputTypeDef = TypedDict(
+    "SourceConnectorPropertiesOutputTypeDef",
+    {
+        "Amplitude": AmplitudeSourcePropertiesTypeDef,
+        "Datadog": DatadogSourcePropertiesTypeDef,
+        "Dynatrace": DynatraceSourcePropertiesTypeDef,
+        "GoogleAnalytics": GoogleAnalyticsSourcePropertiesTypeDef,
+        "InforNexus": InforNexusSourcePropertiesTypeDef,
+        "Marketo": MarketoSourcePropertiesTypeDef,
+        "S3": S3SourcePropertiesTypeDef,
+        "Salesforce": SalesforceSourcePropertiesTypeDef,
+        "ServiceNow": ServiceNowSourcePropertiesTypeDef,
+        "Singular": SingularSourcePropertiesTypeDef,
+        "Slack": SlackSourcePropertiesTypeDef,
+        "Trendmicro": TrendmicroSourcePropertiesTypeDef,
+        "Veeva": VeevaSourcePropertiesTypeDef,
+        "Zendesk": ZendeskSourcePropertiesTypeDef,
+        "SAPOData": SAPODataSourcePropertiesTypeDef,
+        "CustomConnector": CustomConnectorSourcePropertiesOutputTypeDef,
+        "Pardot": PardotSourcePropertiesTypeDef,
+    },
+    total=False,
+)
 
 SourceConnectorPropertiesTypeDef = TypedDict(
     "SourceConnectorPropertiesTypeDef",
     {
         "Amplitude": AmplitudeSourcePropertiesTypeDef,
         "Datadog": DatadogSourcePropertiesTypeDef,
         "Dynatrace": DynatraceSourcePropertiesTypeDef,
@@ -2278,32 +2577,40 @@
         "SAPOData": SAPODataSourcePropertiesTypeDef,
         "CustomConnector": CustomConnectorSourcePropertiesTypeDef,
         "Pardot": PardotSourcePropertiesTypeDef,
     },
     total=False,
 )
 
-_RequiredTriggerConfigTypeDef = TypedDict(
-    "_RequiredTriggerConfigTypeDef",
+_RequiredTriggerConfigOutputTypeDef = TypedDict(
+    "_RequiredTriggerConfigOutputTypeDef",
     {
         "triggerType": TriggerTypeType,
     },
 )
-_OptionalTriggerConfigTypeDef = TypedDict(
-    "_OptionalTriggerConfigTypeDef",
+_OptionalTriggerConfigOutputTypeDef = TypedDict(
+    "_OptionalTriggerConfigOutputTypeDef",
     {
-        "triggerProperties": TriggerPropertiesTypeDef,
+        "triggerProperties": TriggerPropertiesOutputTypeDef,
     },
     total=False,
 )
 
-
-class TriggerConfigTypeDef(_RequiredTriggerConfigTypeDef, _OptionalTriggerConfigTypeDef):
+class TriggerConfigOutputTypeDef(
+    _RequiredTriggerConfigOutputTypeDef, _OptionalTriggerConfigOutputTypeDef
+):
     pass
 
+TriggerPropertiesTypeDef = TypedDict(
+    "TriggerPropertiesTypeDef",
+    {
+        "Scheduled": ScheduledTriggerPropertiesTypeDef,
+    },
+    total=False,
+)
 
 ConnectorProfileCredentialsTypeDef = TypedDict(
     "ConnectorProfileCredentialsTypeDef",
     {
         "Amplitude": AmplitudeConnectorProfileCredentialsTypeDef,
         "Datadog": DatadogConnectorProfileCredentialsTypeDef,
         "Dynatrace": DynatraceConnectorProfileCredentialsTypeDef,
@@ -2346,27 +2653,25 @@
         "sourceProperties": SourceFieldPropertiesTypeDef,
         "destinationProperties": DestinationFieldPropertiesTypeDef,
         "customProperties": Dict[str, str],
     },
     total=False,
 )
 
-
 class ConnectorEntityFieldTypeDef(
     _RequiredConnectorEntityFieldTypeDef, _OptionalConnectorEntityFieldTypeDef
 ):
     pass
 
-
 DescribeFlowExecutionRecordsResponseTypeDef = TypedDict(
     "DescribeFlowExecutionRecordsResponseTypeDef",
     {
         "flowExecutions": List[ExecutionRecordTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConnectorConfigurationTypeDef = TypedDict(
     "ConnectorConfigurationTypeDef",
     {
         "canUseAsSource": bool,
@@ -2406,22 +2711,42 @@
     {
         "connectorProfileArn": str,
         "connectorProfileName": str,
         "connectorType": ConnectorTypeType,
         "connectorLabel": str,
         "connectionMode": ConnectionModeType,
         "credentialsArn": str,
-        "connectorProfileProperties": ConnectorProfilePropertiesTypeDef,
+        "connectorProfileProperties": ConnectorProfilePropertiesOutputTypeDef,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "privateConnectionProvisioningState": PrivateConnectionProvisioningStateTypeDef,
     },
     total=False,
 )
 
+DestinationConnectorPropertiesOutputTypeDef = TypedDict(
+    "DestinationConnectorPropertiesOutputTypeDef",
+    {
+        "Redshift": RedshiftDestinationPropertiesTypeDef,
+        "S3": S3DestinationPropertiesOutputTypeDef,
+        "Salesforce": SalesforceDestinationPropertiesOutputTypeDef,
+        "Snowflake": SnowflakeDestinationPropertiesTypeDef,
+        "EventBridge": EventBridgeDestinationPropertiesTypeDef,
+        "LookoutMetrics": Dict[str, Any],
+        "Upsolver": UpsolverDestinationPropertiesOutputTypeDef,
+        "Honeycode": HoneycodeDestinationPropertiesTypeDef,
+        "CustomerProfiles": CustomerProfilesDestinationPropertiesTypeDef,
+        "Zendesk": ZendeskDestinationPropertiesOutputTypeDef,
+        "Marketo": MarketoDestinationPropertiesTypeDef,
+        "CustomConnector": CustomConnectorDestinationPropertiesOutputTypeDef,
+        "SAPOData": SAPODataDestinationPropertiesOutputTypeDef,
+    },
+    total=False,
+)
+
 DestinationConnectorPropertiesTypeDef = TypedDict(
     "DestinationConnectorPropertiesTypeDef",
     {
         "Redshift": RedshiftDestinationPropertiesTypeDef,
         "S3": S3DestinationPropertiesTypeDef,
         "Salesforce": SalesforceDestinationPropertiesTypeDef,
         "Snowflake": SnowflakeDestinationPropertiesTypeDef,
@@ -2434,14 +2759,36 @@
         "Marketo": MarketoDestinationPropertiesTypeDef,
         "CustomConnector": CustomConnectorDestinationPropertiesTypeDef,
         "SAPOData": SAPODataDestinationPropertiesTypeDef,
     },
     total=False,
 )
 
+_RequiredSourceFlowConfigOutputTypeDef = TypedDict(
+    "_RequiredSourceFlowConfigOutputTypeDef",
+    {
+        "connectorType": ConnectorTypeType,
+        "sourceConnectorProperties": SourceConnectorPropertiesOutputTypeDef,
+    },
+)
+_OptionalSourceFlowConfigOutputTypeDef = TypedDict(
+    "_OptionalSourceFlowConfigOutputTypeDef",
+    {
+        "apiVersion": str,
+        "connectorProfileName": str,
+        "incrementalPullConfig": IncrementalPullConfigTypeDef,
+    },
+    total=False,
+)
+
+class SourceFlowConfigOutputTypeDef(
+    _RequiredSourceFlowConfigOutputTypeDef, _OptionalSourceFlowConfigOutputTypeDef
+):
+    pass
+
 _RequiredSourceFlowConfigTypeDef = TypedDict(
     "_RequiredSourceFlowConfigTypeDef",
     {
         "connectorType": ConnectorTypeType,
         "sourceConnectorProperties": SourceConnectorPropertiesTypeDef,
     },
 )
@@ -2451,18 +2798,33 @@
         "apiVersion": str,
         "connectorProfileName": str,
         "incrementalPullConfig": IncrementalPullConfigTypeDef,
     },
     total=False,
 )
 
-
 class SourceFlowConfigTypeDef(_RequiredSourceFlowConfigTypeDef, _OptionalSourceFlowConfigTypeDef):
     pass
 
+_RequiredTriggerConfigTypeDef = TypedDict(
+    "_RequiredTriggerConfigTypeDef",
+    {
+        "triggerType": TriggerTypeType,
+    },
+)
+_OptionalTriggerConfigTypeDef = TypedDict(
+    "_OptionalTriggerConfigTypeDef",
+    {
+        "triggerProperties": TriggerPropertiesTypeDef,
+    },
+    total=False,
+)
+
+class TriggerConfigTypeDef(_RequiredTriggerConfigTypeDef, _OptionalTriggerConfigTypeDef):
+    pass
 
 _RequiredConnectorProfileConfigTypeDef = TypedDict(
     "_RequiredConnectorProfileConfigTypeDef",
     {
         "connectorProfileProperties": ConnectorProfilePropertiesTypeDef,
     },
 )
@@ -2470,56 +2832,75 @@
     "_OptionalConnectorProfileConfigTypeDef",
     {
         "connectorProfileCredentials": ConnectorProfileCredentialsTypeDef,
     },
     total=False,
 )
 
-
 class ConnectorProfileConfigTypeDef(
     _RequiredConnectorProfileConfigTypeDef, _OptionalConnectorProfileConfigTypeDef
 ):
     pass
 
-
 DescribeConnectorEntityResponseTypeDef = TypedDict(
     "DescribeConnectorEntityResponseTypeDef",
     {
         "connectorEntityFields": List[ConnectorEntityFieldTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConnectorResponseTypeDef = TypedDict(
     "DescribeConnectorResponseTypeDef",
     {
         "connectorConfiguration": ConnectorConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConnectorsResponseTypeDef = TypedDict(
     "DescribeConnectorsResponseTypeDef",
     {
         "connectorConfigurations": Dict[ConnectorTypeType, ConnectorConfigurationTypeDef],
         "connectors": List[ConnectorDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConnectorProfilesResponseTypeDef = TypedDict(
     "DescribeConnectorProfilesResponseTypeDef",
     {
         "connectorProfileDetails": List[ConnectorProfileTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredDestinationFlowConfigOutputTypeDef = TypedDict(
+    "_RequiredDestinationFlowConfigOutputTypeDef",
+    {
+        "connectorType": ConnectorTypeType,
+        "destinationConnectorProperties": DestinationConnectorPropertiesOutputTypeDef,
+    },
+)
+_OptionalDestinationFlowConfigOutputTypeDef = TypedDict(
+    "_OptionalDestinationFlowConfigOutputTypeDef",
+    {
+        "apiVersion": str,
+        "connectorProfileName": str,
     },
+    total=False,
 )
 
+class DestinationFlowConfigOutputTypeDef(
+    _RequiredDestinationFlowConfigOutputTypeDef, _OptionalDestinationFlowConfigOutputTypeDef
+):
+    pass
+
 _RequiredDestinationFlowConfigTypeDef = TypedDict(
     "_RequiredDestinationFlowConfigTypeDef",
     {
         "connectorType": ConnectorTypeType,
         "destinationConnectorProperties": DestinationConnectorPropertiesTypeDef,
     },
 )
@@ -2528,21 +2909,21 @@
     {
         "apiVersion": str,
         "connectorProfileName": str,
     },
     total=False,
 )
 
-
 class DestinationFlowConfigTypeDef(
     _RequiredDestinationFlowConfigTypeDef, _OptionalDestinationFlowConfigTypeDef
 ):
     pass
 
-
+SourceFlowConfigUnionTypeDef = Union[SourceFlowConfigTypeDef, SourceFlowConfigOutputTypeDef]
+TriggerConfigUnionTypeDef = Union[TriggerConfigTypeDef, TriggerConfigOutputTypeDef]
 _RequiredCreateConnectorProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectorProfileRequestRequestTypeDef",
     {
         "connectorProfileName": str,
         "connectorType": ConnectorTypeType,
         "connectionMode": ConnectionModeType,
         "connectorProfileConfig": ConnectorProfileConfigTypeDef,
@@ -2554,22 +2935,20 @@
         "kmsArn": str,
         "connectorLabel": str,
         "clientToken": str,
     },
     total=False,
 )
 
-
 class CreateConnectorProfileRequestRequestTypeDef(
     _RequiredCreateConnectorProfileRequestRequestTypeDef,
     _OptionalCreateConnectorProfileRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateConnectorProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateConnectorProfileRequestRequestTypeDef",
     {
         "connectorProfileName": str,
         "connectionMode": ConnectionModeType,
         "connectorProfileConfig": ConnectorProfileConfigTypeDef,
     },
@@ -2578,95 +2957,93 @@
     "_OptionalUpdateConnectorProfileRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateConnectorProfileRequestRequestTypeDef(
     _RequiredUpdateConnectorProfileRequestRequestTypeDef,
     _OptionalUpdateConnectorProfileRequestRequestTypeDef,
 ):
     pass
 
+DescribeFlowResponseTypeDef = TypedDict(
+    "DescribeFlowResponseTypeDef",
+    {
+        "flowArn": str,
+        "description": str,
+        "flowName": str,
+        "kmsArn": str,
+        "flowStatus": FlowStatusType,
+        "flowStatusMessage": str,
+        "sourceFlowConfig": SourceFlowConfigOutputTypeDef,
+        "destinationFlowConfigList": List[DestinationFlowConfigOutputTypeDef],
+        "lastRunExecutionDetails": ExecutionDetailsTypeDef,
+        "triggerConfig": TriggerConfigOutputTypeDef,
+        "tasks": List[TaskOutputTypeDef],
+        "createdAt": datetime,
+        "lastUpdatedAt": datetime,
+        "createdBy": str,
+        "lastUpdatedBy": str,
+        "tags": Dict[str, str],
+        "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
+        "lastRunMetadataCatalogDetails": List[MetadataCatalogDetailTypeDef],
+        "schemaVersion": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+DestinationFlowConfigUnionTypeDef = Union[
+    DestinationFlowConfigTypeDef, DestinationFlowConfigOutputTypeDef
+]
 _RequiredCreateFlowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFlowRequestRequestTypeDef",
     {
         "flowName": str,
         "triggerConfig": TriggerConfigTypeDef,
         "sourceFlowConfig": SourceFlowConfigTypeDef,
-        "destinationFlowConfigList": Sequence[DestinationFlowConfigTypeDef],
-        "tasks": Sequence[TaskTypeDef],
+        "destinationFlowConfigList": Sequence[DestinationFlowConfigUnionTypeDef],
+        "tasks": Sequence[TaskUnionTypeDef],
     },
 )
 _OptionalCreateFlowRequestRequestTypeDef = TypedDict(
     "_OptionalCreateFlowRequestRequestTypeDef",
     {
         "description": str,
         "kmsArn": str,
         "tags": Mapping[str, str],
         "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
         "clientToken": str,
     },
     total=False,
 )
 
-
 class CreateFlowRequestRequestTypeDef(
     _RequiredCreateFlowRequestRequestTypeDef, _OptionalCreateFlowRequestRequestTypeDef
 ):
     pass
 
-
-DescribeFlowResponseTypeDef = TypedDict(
-    "DescribeFlowResponseTypeDef",
-    {
-        "flowArn": str,
-        "description": str,
-        "flowName": str,
-        "kmsArn": str,
-        "flowStatus": FlowStatusType,
-        "flowStatusMessage": str,
-        "sourceFlowConfig": SourceFlowConfigTypeDef,
-        "destinationFlowConfigList": List[DestinationFlowConfigTypeDef],
-        "lastRunExecutionDetails": ExecutionDetailsTypeDef,
-        "triggerConfig": TriggerConfigTypeDef,
-        "tasks": List[TaskTypeDef],
-        "createdAt": datetime,
-        "lastUpdatedAt": datetime,
-        "createdBy": str,
-        "lastUpdatedBy": str,
-        "tags": Dict[str, str],
-        "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
-        "lastRunMetadataCatalogDetails": List[MetadataCatalogDetailTypeDef],
-        "schemaVersion": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateFlowRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFlowRequestRequestTypeDef",
     {
         "flowName": str,
         "triggerConfig": TriggerConfigTypeDef,
         "sourceFlowConfig": SourceFlowConfigTypeDef,
-        "destinationFlowConfigList": Sequence[DestinationFlowConfigTypeDef],
-        "tasks": Sequence[TaskTypeDef],
+        "destinationFlowConfigList": Sequence[DestinationFlowConfigUnionTypeDef],
+        "tasks": Sequence[TaskUnionTypeDef],
     },
 )
 _OptionalUpdateFlowRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateFlowRequestRequestTypeDef",
     {
         "description": str,
         "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateFlowRequestRequestTypeDef(
     _RequiredUpdateFlowRequestRequestTypeDef, _OptionalUpdateFlowRequestRequestTypeDef
 ):
     pass
```

### Comparing `types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow/type_defs.pyi` & `types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_appflow.type_defs import AggregationConfigTypeDef
 
-    data: AggregationConfigTypeDef = {...}
+    data: AggregationConfigTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -64,23 +64,24 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AggregationConfigTypeDef",
     "AmplitudeConnectorProfileCredentialsTypeDef",
     "AmplitudeSourcePropertiesTypeDef",
     "ApiKeyCredentialsTypeDef",
     "AuthParameterTypeDef",
     "BasicAuthCredentialsTypeDef",
     "CancelFlowExecutionsRequestRequestTypeDef",
-    "CancelFlowExecutionsResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ConnectorRuntimeSettingTypeDef",
     "DataTransferApiTypeDef",
     "ConnectorDetailTypeDef",
     "DestinationFieldPropertiesTypeDef",
     "SourceFieldPropertiesTypeDef",
     "ConnectorEntityTypeDef",
     "GoogleAnalyticsMetadataTypeDef",
@@ -110,18 +111,17 @@
     "ServiceNowConnectorProfilePropertiesTypeDef",
     "SlackConnectorProfilePropertiesTypeDef",
     "SnowflakeConnectorProfilePropertiesTypeDef",
     "VeevaConnectorProfilePropertiesTypeDef",
     "ZendeskConnectorProfilePropertiesTypeDef",
     "PrivateConnectionProvisioningStateTypeDef",
     "LambdaConnectorProvisioningConfigTypeDef",
-    "CreateConnectorProfileResponseTypeDef",
-    "CreateFlowResponseTypeDef",
     "CustomAuthCredentialsTypeDef",
     "ErrorHandlingConfigTypeDef",
+    "OAuth2PropertiesOutputTypeDef",
     "OAuth2PropertiesTypeDef",
     "CustomerProfilesDestinationPropertiesTypeDef",
     "DatadogSourcePropertiesTypeDef",
     "DeleteConnectorProfileRequestRequestTypeDef",
     "DeleteFlowRequestRequestTypeDef",
     "DescribeConnectorEntityRequestRequestTypeDef",
     "DescribeConnectorProfilesRequestRequestTypeDef",
@@ -137,112 +137,141 @@
     "GoogleAnalyticsSourcePropertiesTypeDef",
     "IncrementalPullConfigTypeDef",
     "InforNexusSourcePropertiesTypeDef",
     "ListConnectorEntitiesRequestRequestTypeDef",
     "ListConnectorsRequestRequestTypeDef",
     "ListFlowsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "MarketoSourcePropertiesTypeDef",
     "RegistrationOutputTypeDef",
     "OAuth2CustomParameterTypeDef",
+    "OAuthPropertiesOutputTypeDef",
     "OAuthPropertiesTypeDef",
     "PardotSourcePropertiesTypeDef",
+    "PrefixConfigOutputTypeDef",
     "PrefixConfigTypeDef",
-    "RegisterConnectorResponseTypeDef",
     "ResetConnectorMetadataCacheRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "S3InputFormatConfigTypeDef",
     "SuccessResponseHandlingConfigTypeDef",
     "SAPODataSourcePropertiesTypeDef",
     "SalesforceSourcePropertiesTypeDef",
-    "ScheduledTriggerPropertiesTypeDef",
+    "ScheduledTriggerPropertiesOutputTypeDef",
+    "TimestampTypeDef",
     "ServiceNowSourcePropertiesTypeDef",
     "SingularSourcePropertiesTypeDef",
     "SlackSourcePropertiesTypeDef",
     "TrendmicroSourcePropertiesTypeDef",
     "VeevaSourcePropertiesTypeDef",
     "ZendeskSourcePropertiesTypeDef",
     "StartFlowRequestRequestTypeDef",
-    "StartFlowResponseTypeDef",
     "StopFlowRequestRequestTypeDef",
-    "StopFlowResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UnregisterConnectorRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "CustomAuthConfigTypeDef",
+    "CancelFlowExecutionsResponseTypeDef",
+    "CreateConnectorProfileResponseTypeDef",
+    "CreateFlowResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "RegisterConnectorResponseTypeDef",
+    "StartFlowResponseTypeDef",
+    "StopFlowResponseTypeDef",
     "UpdateConnectorProfileResponseTypeDef",
     "UpdateConnectorRegistrationResponseTypeDef",
     "UpdateFlowResponseTypeDef",
-    "CustomAuthConfigTypeDef",
+    "CustomConnectorSourcePropertiesOutputTypeDef",
     "CustomConnectorSourcePropertiesTypeDef",
     "ListConnectorsResponseTypeDef",
     "ListConnectorEntitiesResponseTypeDef",
     "ConnectorMetadataTypeDef",
     "GoogleAnalyticsConnectorProfileCredentialsTypeDef",
     "HoneycodeConnectorProfileCredentialsTypeDef",
     "MarketoConnectorProfileCredentialsTypeDef",
     "OAuth2CredentialsTypeDef",
     "OAuthCredentialsTypeDef",
     "PardotConnectorProfileCredentialsTypeDef",
     "SalesforceConnectorProfileCredentialsTypeDef",
     "SlackConnectorProfileCredentialsTypeDef",
     "ZendeskConnectorProfileCredentialsTypeDef",
+    "TaskOutputTypeDef",
     "TaskTypeDef",
     "ConnectorProvisioningConfigTypeDef",
+    "CustomConnectorDestinationPropertiesOutputTypeDef",
     "CustomConnectorDestinationPropertiesTypeDef",
     "EventBridgeDestinationPropertiesTypeDef",
     "HoneycodeDestinationPropertiesTypeDef",
     "MarketoDestinationPropertiesTypeDef",
     "RedshiftDestinationPropertiesTypeDef",
+    "SalesforceDestinationPropertiesOutputTypeDef",
     "SalesforceDestinationPropertiesTypeDef",
     "SnowflakeDestinationPropertiesTypeDef",
+    "ZendeskDestinationPropertiesOutputTypeDef",
     "ZendeskDestinationPropertiesTypeDef",
+    "CustomConnectorProfilePropertiesOutputTypeDef",
     "CustomConnectorProfilePropertiesTypeDef",
     "FlowDefinitionTypeDef",
     "ExecutionResultTypeDef",
     "FieldTypeDetailsTypeDef",
     "MetadataCatalogConfigTypeDef",
     "MetadataCatalogDetailTypeDef",
     "OAuth2DefaultsTypeDef",
+    "SAPODataConnectorProfilePropertiesOutputTypeDef",
     "SAPODataConnectorProfilePropertiesTypeDef",
+    "S3OutputFormatConfigOutputTypeDef",
+    "UpsolverS3OutputFormatConfigOutputTypeDef",
     "S3OutputFormatConfigTypeDef",
     "UpsolverS3OutputFormatConfigTypeDef",
     "S3SourcePropertiesTypeDef",
+    "SAPODataDestinationPropertiesOutputTypeDef",
     "SAPODataDestinationPropertiesTypeDef",
-    "TriggerPropertiesTypeDef",
+    "TriggerPropertiesOutputTypeDef",
+    "ScheduledTriggerPropertiesTypeDef",
     "CustomConnectorProfileCredentialsTypeDef",
     "SAPODataConnectorProfileCredentialsTypeDef",
+    "TaskUnionTypeDef",
     "RegisterConnectorRequestRequestTypeDef",
     "UpdateConnectorRegistrationRequestRequestTypeDef",
     "ListFlowsResponseTypeDef",
     "SupportedFieldTypeDetailsTypeDef",
     "ExecutionRecordTypeDef",
     "AuthenticationConfigTypeDef",
+    "ConnectorProfilePropertiesOutputTypeDef",
     "ConnectorProfilePropertiesTypeDef",
+    "S3DestinationPropertiesOutputTypeDef",
+    "UpsolverDestinationPropertiesOutputTypeDef",
     "S3DestinationPropertiesTypeDef",
     "UpsolverDestinationPropertiesTypeDef",
+    "SourceConnectorPropertiesOutputTypeDef",
     "SourceConnectorPropertiesTypeDef",
-    "TriggerConfigTypeDef",
+    "TriggerConfigOutputTypeDef",
+    "TriggerPropertiesTypeDef",
     "ConnectorProfileCredentialsTypeDef",
     "ConnectorEntityFieldTypeDef",
     "DescribeFlowExecutionRecordsResponseTypeDef",
     "ConnectorConfigurationTypeDef",
     "ConnectorProfileTypeDef",
+    "DestinationConnectorPropertiesOutputTypeDef",
     "DestinationConnectorPropertiesTypeDef",
+    "SourceFlowConfigOutputTypeDef",
     "SourceFlowConfigTypeDef",
+    "TriggerConfigTypeDef",
     "ConnectorProfileConfigTypeDef",
     "DescribeConnectorEntityResponseTypeDef",
     "DescribeConnectorResponseTypeDef",
     "DescribeConnectorsResponseTypeDef",
     "DescribeConnectorProfilesResponseTypeDef",
+    "DestinationFlowConfigOutputTypeDef",
     "DestinationFlowConfigTypeDef",
+    "SourceFlowConfigUnionTypeDef",
+    "TriggerConfigUnionTypeDef",
     "CreateConnectorProfileRequestRequestTypeDef",
     "UpdateConnectorProfileRequestRequestTypeDef",
-    "CreateFlowRequestRequestTypeDef",
     "DescribeFlowResponseTypeDef",
+    "DestinationFlowConfigUnionTypeDef",
+    "CreateFlowRequestRequestTypeDef",
     "UpdateFlowRequestRequestTypeDef",
 )
 
 AggregationConfigTypeDef = TypedDict(
     "AggregationConfigTypeDef",
     {
         "aggregationType": AggregationTypeType,
@@ -276,19 +305,21 @@
     "_OptionalApiKeyCredentialsTypeDef",
     {
         "apiSecretKey": str,
     },
     total=False,
 )
 
+
 class ApiKeyCredentialsTypeDef(
     _RequiredApiKeyCredentialsTypeDef, _OptionalApiKeyCredentialsTypeDef
 ):
     pass
 
+
 AuthParameterTypeDef = TypedDict(
     "AuthParameterTypeDef",
     {
         "key": str,
         "isRequired": bool,
         "label": str,
         "description": str,
@@ -316,25 +347,30 @@
     "_OptionalCancelFlowExecutionsRequestRequestTypeDef",
     {
         "executionIds": Sequence[str],
     },
     total=False,
 )
 
+
 class CancelFlowExecutionsRequestRequestTypeDef(
     _RequiredCancelFlowExecutionsRequestRequestTypeDef,
     _OptionalCancelFlowExecutionsRequestRequestTypeDef,
 ):
     pass
 
-CancelFlowExecutionsResponseTypeDef = TypedDict(
-    "CancelFlowExecutionsResponseTypeDef",
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "invalidExecutions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ConnectorRuntimeSettingTypeDef = TypedDict(
     "ConnectorRuntimeSettingTypeDef",
     {
         "key": str,
@@ -410,17 +446,19 @@
     {
         "label": str,
         "hasNestedEntities": bool,
     },
     total=False,
 )
 
+
 class ConnectorEntityTypeDef(_RequiredConnectorEntityTypeDef, _OptionalConnectorEntityTypeDef):
     pass
 
+
 GoogleAnalyticsMetadataTypeDef = TypedDict(
     "GoogleAnalyticsMetadataTypeDef",
     {
         "oAuthScopes": List[str],
     },
     total=False,
 )
@@ -627,20 +665,22 @@
         "clusterIdentifier": str,
         "workgroupName": str,
         "databaseName": str,
     },
     total=False,
 )
 
+
 class RedshiftConnectorProfilePropertiesTypeDef(
     _RequiredRedshiftConnectorProfilePropertiesTypeDef,
     _OptionalRedshiftConnectorProfilePropertiesTypeDef,
 ):
     pass
 
+
 SalesforceConnectorProfilePropertiesTypeDef = TypedDict(
     "SalesforceConnectorProfilePropertiesTypeDef",
     {
         "instanceUrl": str,
         "isSandboxEnvironment": bool,
         "usePrivateLinkForMetadataAndAuthorization": bool,
     },
@@ -676,20 +716,22 @@
         "privateLinkServiceName": str,
         "accountName": str,
         "region": str,
     },
     total=False,
 )
 
+
 class SnowflakeConnectorProfilePropertiesTypeDef(
     _RequiredSnowflakeConnectorProfilePropertiesTypeDef,
     _OptionalSnowflakeConnectorProfilePropertiesTypeDef,
 ):
     pass
 
+
 VeevaConnectorProfilePropertiesTypeDef = TypedDict(
     "VeevaConnectorProfilePropertiesTypeDef",
     {
         "instanceUrl": str,
     },
 )
 
@@ -713,60 +755,67 @@
 LambdaConnectorProvisioningConfigTypeDef = TypedDict(
     "LambdaConnectorProvisioningConfigTypeDef",
     {
         "lambdaArn": str,
     },
 )
 
-CreateConnectorProfileResponseTypeDef = TypedDict(
-    "CreateConnectorProfileResponseTypeDef",
-    {
-        "connectorProfileArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFlowResponseTypeDef = TypedDict(
-    "CreateFlowResponseTypeDef",
-    {
-        "flowArn": str,
-        "flowStatus": FlowStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCustomAuthCredentialsTypeDef = TypedDict(
     "_RequiredCustomAuthCredentialsTypeDef",
     {
         "customAuthenticationType": str,
     },
 )
 _OptionalCustomAuthCredentialsTypeDef = TypedDict(
     "_OptionalCustomAuthCredentialsTypeDef",
     {
         "credentialsMap": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CustomAuthCredentialsTypeDef(
     _RequiredCustomAuthCredentialsTypeDef, _OptionalCustomAuthCredentialsTypeDef
 ):
     pass
 
+
 ErrorHandlingConfigTypeDef = TypedDict(
     "ErrorHandlingConfigTypeDef",
     {
         "failOnFirstDestinationError": bool,
         "bucketPrefix": str,
         "bucketName": str,
     },
     total=False,
 )
 
+_RequiredOAuth2PropertiesOutputTypeDef = TypedDict(
+    "_RequiredOAuth2PropertiesOutputTypeDef",
+    {
+        "tokenUrl": str,
+        "oAuth2GrantType": OAuth2GrantTypeType,
+    },
+)
+_OptionalOAuth2PropertiesOutputTypeDef = TypedDict(
+    "_OptionalOAuth2PropertiesOutputTypeDef",
+    {
+        "tokenUrlCustomProperties": Dict[str, str],
+    },
+    total=False,
+)
+
+
+class OAuth2PropertiesOutputTypeDef(
+    _RequiredOAuth2PropertiesOutputTypeDef, _OptionalOAuth2PropertiesOutputTypeDef
+):
+    pass
+
+
 _RequiredOAuth2PropertiesTypeDef = TypedDict(
     "_RequiredOAuth2PropertiesTypeDef",
     {
         "tokenUrl": str,
         "oAuth2GrantType": OAuth2GrantTypeType,
     },
 )
@@ -774,37 +823,41 @@
     "_OptionalOAuth2PropertiesTypeDef",
     {
         "tokenUrlCustomProperties": Mapping[str, str],
     },
     total=False,
 )
 
+
 class OAuth2PropertiesTypeDef(_RequiredOAuth2PropertiesTypeDef, _OptionalOAuth2PropertiesTypeDef):
     pass
 
+
 _RequiredCustomerProfilesDestinationPropertiesTypeDef = TypedDict(
     "_RequiredCustomerProfilesDestinationPropertiesTypeDef",
     {
         "domainName": str,
     },
 )
 _OptionalCustomerProfilesDestinationPropertiesTypeDef = TypedDict(
     "_OptionalCustomerProfilesDestinationPropertiesTypeDef",
     {
         "objectTypeName": str,
     },
     total=False,
 )
 
+
 class CustomerProfilesDestinationPropertiesTypeDef(
     _RequiredCustomerProfilesDestinationPropertiesTypeDef,
     _OptionalCustomerProfilesDestinationPropertiesTypeDef,
 ):
     pass
 
+
 DatadogSourcePropertiesTypeDef = TypedDict(
     "DatadogSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -818,39 +871,43 @@
     "_OptionalDeleteConnectorProfileRequestRequestTypeDef",
     {
         "forceDelete": bool,
     },
     total=False,
 )
 
+
 class DeleteConnectorProfileRequestRequestTypeDef(
     _RequiredDeleteConnectorProfileRequestRequestTypeDef,
     _OptionalDeleteConnectorProfileRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteFlowRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFlowRequestRequestTypeDef",
     {
         "flowName": str,
     },
 )
 _OptionalDeleteFlowRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteFlowRequestRequestTypeDef",
     {
         "forceDelete": bool,
     },
     total=False,
 )
 
+
 class DeleteFlowRequestRequestTypeDef(
     _RequiredDeleteFlowRequestRequestTypeDef, _OptionalDeleteFlowRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDescribeConnectorEntityRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConnectorEntityRequestRequestTypeDef",
     {
         "connectorEntityName": str,
     },
 )
 _OptionalDescribeConnectorEntityRequestRequestTypeDef = TypedDict(
@@ -859,20 +916,22 @@
         "connectorType": ConnectorTypeType,
         "connectorProfileName": str,
         "apiVersion": str,
     },
     total=False,
 )
 
+
 class DescribeConnectorEntityRequestRequestTypeDef(
     _RequiredDescribeConnectorEntityRequestRequestTypeDef,
     _OptionalDescribeConnectorEntityRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeConnectorProfilesRequestRequestTypeDef = TypedDict(
     "DescribeConnectorProfilesRequestRequestTypeDef",
     {
         "connectorProfileNames": Sequence[str],
         "connectorType": ConnectorTypeType,
         "connectorLabel": str,
         "maxResults": int,
@@ -891,19 +950,21 @@
     "_OptionalDescribeConnectorRequestRequestTypeDef",
     {
         "connectorLabel": str,
     },
     total=False,
 )
 
+
 class DescribeConnectorRequestRequestTypeDef(
     _RequiredDescribeConnectorRequestRequestTypeDef, _OptionalDescribeConnectorRequestRequestTypeDef
 ):
     pass
 
+
 DescribeConnectorsRequestRequestTypeDef = TypedDict(
     "DescribeConnectorsRequestRequestTypeDef",
     {
         "connectorTypes": Sequence[ConnectorTypeType],
         "maxResults": int,
         "nextToken": str,
     },
@@ -921,20 +982,22 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class DescribeFlowExecutionRecordsRequestRequestTypeDef(
     _RequiredDescribeFlowExecutionRecordsRequestRequestTypeDef,
     _OptionalDescribeFlowExecutionRecordsRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeFlowRequestRequestTypeDef = TypedDict(
     "DescribeFlowRequestRequestTypeDef",
     {
         "flowName": str,
     },
 )
 
@@ -1038,22 +1101,14 @@
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
 MarketoSourcePropertiesTypeDef = TypedDict(
     "MarketoSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -1077,14 +1132,23 @@
         "isSensitiveField": bool,
         "connectorSuppliedValues": List[str],
         "type": OAuth2CustomPropTypeType,
     },
     total=False,
 )
 
+OAuthPropertiesOutputTypeDef = TypedDict(
+    "OAuthPropertiesOutputTypeDef",
+    {
+        "tokenUrl": str,
+        "authCodeUrl": str,
+        "oAuthScopes": List[str],
+    },
+)
+
 OAuthPropertiesTypeDef = TypedDict(
     "OAuthPropertiesTypeDef",
     {
         "tokenUrl": str,
         "authCodeUrl": str,
         "oAuthScopes": Sequence[str],
     },
@@ -1093,55 +1157,46 @@
 PardotSourcePropertiesTypeDef = TypedDict(
     "PardotSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
-PrefixConfigTypeDef = TypedDict(
-    "PrefixConfigTypeDef",
+PrefixConfigOutputTypeDef = TypedDict(
+    "PrefixConfigOutputTypeDef",
     {
         "prefixType": PrefixTypeType,
         "prefixFormat": PrefixFormatType,
-        "pathPrefixHierarchy": Sequence[PathPrefixType],
+        "pathPrefixHierarchy": List[PathPrefixType],
     },
     total=False,
 )
 
-RegisterConnectorResponseTypeDef = TypedDict(
-    "RegisterConnectorResponseTypeDef",
+PrefixConfigTypeDef = TypedDict(
+    "PrefixConfigTypeDef",
     {
-        "connectorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "prefixType": PrefixTypeType,
+        "prefixFormat": PrefixFormatType,
+        "pathPrefixHierarchy": Sequence[PathPrefixType],
     },
+    total=False,
 )
 
 ResetConnectorMetadataCacheRequestRequestTypeDef = TypedDict(
     "ResetConnectorMetadataCacheRequestRequestTypeDef",
     {
         "connectorProfileName": str,
         "connectorType": ConnectorTypeType,
         "connectorEntityName": str,
         "entitiesPath": str,
         "apiVersion": str,
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
 S3InputFormatConfigTypeDef = TypedDict(
     "S3InputFormatConfigTypeDef",
     {
         "s3InputFileType": S3InputFileTypeType,
     },
     total=False,
 )
@@ -1175,44 +1230,50 @@
         "enableDynamicFieldUpdate": bool,
         "includeDeletedRecords": bool,
         "dataTransferApi": SalesforceDataTransferApiType,
     },
     total=False,
 )
 
+
 class SalesforceSourcePropertiesTypeDef(
     _RequiredSalesforceSourcePropertiesTypeDef, _OptionalSalesforceSourcePropertiesTypeDef
 ):
     pass
 
-_RequiredScheduledTriggerPropertiesTypeDef = TypedDict(
-    "_RequiredScheduledTriggerPropertiesTypeDef",
+
+_RequiredScheduledTriggerPropertiesOutputTypeDef = TypedDict(
+    "_RequiredScheduledTriggerPropertiesOutputTypeDef",
     {
         "scheduleExpression": str,
     },
 )
-_OptionalScheduledTriggerPropertiesTypeDef = TypedDict(
-    "_OptionalScheduledTriggerPropertiesTypeDef",
+_OptionalScheduledTriggerPropertiesOutputTypeDef = TypedDict(
+    "_OptionalScheduledTriggerPropertiesOutputTypeDef",
     {
         "dataPullMode": DataPullModeType,
-        "scheduleStartTime": Union[datetime, str],
-        "scheduleEndTime": Union[datetime, str],
+        "scheduleStartTime": datetime,
+        "scheduleEndTime": datetime,
         "timezone": str,
         "scheduleOffset": int,
-        "firstExecutionFrom": Union[datetime, str],
+        "firstExecutionFrom": datetime,
         "flowErrorDeactivationThreshold": int,
     },
     total=False,
 )
 
-class ScheduledTriggerPropertiesTypeDef(
-    _RequiredScheduledTriggerPropertiesTypeDef, _OptionalScheduledTriggerPropertiesTypeDef
+
+class ScheduledTriggerPropertiesOutputTypeDef(
+    _RequiredScheduledTriggerPropertiesOutputTypeDef,
+    _OptionalScheduledTriggerPropertiesOutputTypeDef,
 ):
     pass
 
+
+TimestampTypeDef = Union[datetime, str]
 ServiceNowSourcePropertiesTypeDef = TypedDict(
     "ServiceNowSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -1250,19 +1311,21 @@
         "includeSourceFiles": bool,
         "includeRenditions": bool,
         "includeAllVersions": bool,
     },
     total=False,
 )
 
+
 class VeevaSourcePropertiesTypeDef(
     _RequiredVeevaSourcePropertiesTypeDef, _OptionalVeevaSourcePropertiesTypeDef
 ):
     pass
 
+
 ZendeskSourcePropertiesTypeDef = TypedDict(
     "ZendeskSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -1276,45 +1339,28 @@
     "_OptionalStartFlowRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class StartFlowRequestRequestTypeDef(
     _RequiredStartFlowRequestRequestTypeDef, _OptionalStartFlowRequestRequestTypeDef
 ):
     pass
 
-StartFlowResponseTypeDef = TypedDict(
-    "StartFlowResponseTypeDef",
-    {
-        "flowArn": str,
-        "flowStatus": FlowStatusType,
-        "executionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 StopFlowRequestRequestTypeDef = TypedDict(
     "StopFlowRequestRequestTypeDef",
     {
         "flowName": str,
     },
 )
 
-StopFlowResponseTypeDef = TypedDict(
-    "StopFlowResponseTypeDef",
-    {
-        "flowArn": str,
-        "flowStatus": FlowStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1329,61 +1375,146 @@
     "_OptionalUnregisterConnectorRequestRequestTypeDef",
     {
         "forceDelete": bool,
     },
     total=False,
 )
 
+
 class UnregisterConnectorRequestRequestTypeDef(
     _RequiredUnregisterConnectorRequestRequestTypeDef,
     _OptionalUnregisterConnectorRequestRequestTypeDef,
 ):
     pass
 
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+CustomAuthConfigTypeDef = TypedDict(
+    "CustomAuthConfigTypeDef",
+    {
+        "customAuthenticationType": str,
+        "authParameters": List[AuthParameterTypeDef],
+    },
+    total=False,
+)
+
+CancelFlowExecutionsResponseTypeDef = TypedDict(
+    "CancelFlowExecutionsResponseTypeDef",
+    {
+        "invalidExecutions": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateConnectorProfileResponseTypeDef = TypedDict(
+    "CreateConnectorProfileResponseTypeDef",
+    {
+        "connectorProfileArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFlowResponseTypeDef = TypedDict(
+    "CreateFlowResponseTypeDef",
+    {
+        "flowArn": str,
+        "flowStatus": FlowStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterConnectorResponseTypeDef = TypedDict(
+    "RegisterConnectorResponseTypeDef",
+    {
+        "connectorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartFlowResponseTypeDef = TypedDict(
+    "StartFlowResponseTypeDef",
+    {
+        "flowArn": str,
+        "flowStatus": FlowStatusType,
+        "executionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopFlowResponseTypeDef = TypedDict(
+    "StopFlowResponseTypeDef",
+    {
+        "flowArn": str,
+        "flowStatus": FlowStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateConnectorProfileResponseTypeDef = TypedDict(
     "UpdateConnectorProfileResponseTypeDef",
     {
         "connectorProfileArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConnectorRegistrationResponseTypeDef = TypedDict(
     "UpdateConnectorRegistrationResponseTypeDef",
     {
         "connectorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFlowResponseTypeDef = TypedDict(
     "UpdateFlowResponseTypeDef",
     {
         "flowStatus": FlowStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CustomAuthConfigTypeDef = TypedDict(
-    "CustomAuthConfigTypeDef",
+_RequiredCustomConnectorSourcePropertiesOutputTypeDef = TypedDict(
+    "_RequiredCustomConnectorSourcePropertiesOutputTypeDef",
     {
-        "customAuthenticationType": str,
-        "authParameters": List[AuthParameterTypeDef],
+        "entityName": str,
+    },
+)
+_OptionalCustomConnectorSourcePropertiesOutputTypeDef = TypedDict(
+    "_OptionalCustomConnectorSourcePropertiesOutputTypeDef",
+    {
+        "customProperties": Dict[str, str],
+        "dataTransferApi": DataTransferApiTypeDef,
     },
     total=False,
 )
 
+
+class CustomConnectorSourcePropertiesOutputTypeDef(
+    _RequiredCustomConnectorSourcePropertiesOutputTypeDef,
+    _OptionalCustomConnectorSourcePropertiesOutputTypeDef,
+):
+    pass
+
+
 _RequiredCustomConnectorSourcePropertiesTypeDef = TypedDict(
     "_RequiredCustomConnectorSourcePropertiesTypeDef",
     {
         "entityName": str,
     },
 )
 _OptionalCustomConnectorSourcePropertiesTypeDef = TypedDict(
@@ -1391,34 +1522,36 @@
     {
         "customProperties": Mapping[str, str],
         "dataTransferApi": DataTransferApiTypeDef,
     },
     total=False,
 )
 
+
 class CustomConnectorSourcePropertiesTypeDef(
     _RequiredCustomConnectorSourcePropertiesTypeDef, _OptionalCustomConnectorSourcePropertiesTypeDef
 ):
     pass
 
+
 ListConnectorsResponseTypeDef = TypedDict(
     "ListConnectorsResponseTypeDef",
     {
         "connectors": List[ConnectorDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConnectorEntitiesResponseTypeDef = TypedDict(
     "ListConnectorEntitiesResponseTypeDef",
     {
         "connectorEntityMap": Dict[str, List[ConnectorEntityTypeDef]],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConnectorMetadataTypeDef = TypedDict(
     "ConnectorMetadataTypeDef",
     {
         "Amplitude": Dict[str, Any],
@@ -1460,20 +1593,22 @@
         "accessToken": str,
         "refreshToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
     total=False,
 )
 
+
 class GoogleAnalyticsConnectorProfileCredentialsTypeDef(
     _RequiredGoogleAnalyticsConnectorProfileCredentialsTypeDef,
     _OptionalGoogleAnalyticsConnectorProfileCredentialsTypeDef,
 ):
     pass
 
+
 HoneycodeConnectorProfileCredentialsTypeDef = TypedDict(
     "HoneycodeConnectorProfileCredentialsTypeDef",
     {
         "accessToken": str,
         "refreshToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
@@ -1492,20 +1627,22 @@
     {
         "accessToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
     total=False,
 )
 
+
 class MarketoConnectorProfileCredentialsTypeDef(
     _RequiredMarketoConnectorProfileCredentialsTypeDef,
     _OptionalMarketoConnectorProfileCredentialsTypeDef,
 ):
     pass
 
+
 OAuth2CredentialsTypeDef = TypedDict(
     "OAuth2CredentialsTypeDef",
     {
         "clientId": str,
         "clientSecret": str,
         "accessToken": str,
         "refreshToken": str,
@@ -1527,17 +1664,19 @@
         "accessToken": str,
         "refreshToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
     total=False,
 )
 
+
 class OAuthCredentialsTypeDef(_RequiredOAuthCredentialsTypeDef, _OptionalOAuthCredentialsTypeDef):
     pass
 
+
 PardotConnectorProfileCredentialsTypeDef = TypedDict(
     "PardotConnectorProfileCredentialsTypeDef",
     {
         "accessToken": str,
         "refreshToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
         "clientCredentialsArn": str,
@@ -1570,20 +1709,22 @@
     {
         "accessToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
     total=False,
 )
 
+
 class SlackConnectorProfileCredentialsTypeDef(
     _RequiredSlackConnectorProfileCredentialsTypeDef,
     _OptionalSlackConnectorProfileCredentialsTypeDef,
 ):
     pass
 
+
 _RequiredZendeskConnectorProfileCredentialsTypeDef = TypedDict(
     "_RequiredZendeskConnectorProfileCredentialsTypeDef",
     {
         "clientId": str,
         "clientSecret": str,
     },
 )
@@ -1592,20 +1733,44 @@
     {
         "accessToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
     total=False,
 )
 
+
 class ZendeskConnectorProfileCredentialsTypeDef(
     _RequiredZendeskConnectorProfileCredentialsTypeDef,
     _OptionalZendeskConnectorProfileCredentialsTypeDef,
 ):
     pass
 
+
+_RequiredTaskOutputTypeDef = TypedDict(
+    "_RequiredTaskOutputTypeDef",
+    {
+        "sourceFields": List[str],
+        "taskType": TaskTypeType,
+    },
+)
+_OptionalTaskOutputTypeDef = TypedDict(
+    "_OptionalTaskOutputTypeDef",
+    {
+        "connectorOperator": ConnectorOperatorTypeDef,
+        "destinationField": str,
+        "taskProperties": Dict[OperatorPropertiesKeysType, str],
+    },
+    total=False,
+)
+
+
+class TaskOutputTypeDef(_RequiredTaskOutputTypeDef, _OptionalTaskOutputTypeDef):
+    pass
+
+
 _RequiredTaskTypeDef = TypedDict(
     "_RequiredTaskTypeDef",
     {
         "sourceFields": Sequence[str],
         "taskType": TaskTypeType,
     },
 )
@@ -1615,25 +1780,52 @@
         "connectorOperator": ConnectorOperatorTypeDef,
         "destinationField": str,
         "taskProperties": Mapping[OperatorPropertiesKeysType, str],
     },
     total=False,
 )
 
+
 class TaskTypeDef(_RequiredTaskTypeDef, _OptionalTaskTypeDef):
     pass
 
+
 ConnectorProvisioningConfigTypeDef = TypedDict(
     "ConnectorProvisioningConfigTypeDef",
     {
         "lambda": LambdaConnectorProvisioningConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredCustomConnectorDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredCustomConnectorDestinationPropertiesOutputTypeDef",
+    {
+        "entityName": str,
+    },
+)
+_OptionalCustomConnectorDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalCustomConnectorDestinationPropertiesOutputTypeDef",
+    {
+        "errorHandlingConfig": ErrorHandlingConfigTypeDef,
+        "writeOperationType": WriteOperationTypeType,
+        "idFieldNames": List[str],
+        "customProperties": Dict[str, str],
+    },
+    total=False,
+)
+
+
+class CustomConnectorDestinationPropertiesOutputTypeDef(
+    _RequiredCustomConnectorDestinationPropertiesOutputTypeDef,
+    _OptionalCustomConnectorDestinationPropertiesOutputTypeDef,
+):
+    pass
+
+
 _RequiredCustomConnectorDestinationPropertiesTypeDef = TypedDict(
     "_RequiredCustomConnectorDestinationPropertiesTypeDef",
     {
         "entityName": str,
     },
 )
 _OptionalCustomConnectorDestinationPropertiesTypeDef = TypedDict(
@@ -1643,78 +1835,86 @@
         "writeOperationType": WriteOperationTypeType,
         "idFieldNames": Sequence[str],
         "customProperties": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CustomConnectorDestinationPropertiesTypeDef(
     _RequiredCustomConnectorDestinationPropertiesTypeDef,
     _OptionalCustomConnectorDestinationPropertiesTypeDef,
 ):
     pass
 
+
 _RequiredEventBridgeDestinationPropertiesTypeDef = TypedDict(
     "_RequiredEventBridgeDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalEventBridgeDestinationPropertiesTypeDef = TypedDict(
     "_OptionalEventBridgeDestinationPropertiesTypeDef",
     {
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
     },
     total=False,
 )
 
+
 class EventBridgeDestinationPropertiesTypeDef(
     _RequiredEventBridgeDestinationPropertiesTypeDef,
     _OptionalEventBridgeDestinationPropertiesTypeDef,
 ):
     pass
 
+
 _RequiredHoneycodeDestinationPropertiesTypeDef = TypedDict(
     "_RequiredHoneycodeDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalHoneycodeDestinationPropertiesTypeDef = TypedDict(
     "_OptionalHoneycodeDestinationPropertiesTypeDef",
     {
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
     },
     total=False,
 )
 
+
 class HoneycodeDestinationPropertiesTypeDef(
     _RequiredHoneycodeDestinationPropertiesTypeDef, _OptionalHoneycodeDestinationPropertiesTypeDef
 ):
     pass
 
+
 _RequiredMarketoDestinationPropertiesTypeDef = TypedDict(
     "_RequiredMarketoDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalMarketoDestinationPropertiesTypeDef = TypedDict(
     "_OptionalMarketoDestinationPropertiesTypeDef",
     {
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
     },
     total=False,
 )
 
+
 class MarketoDestinationPropertiesTypeDef(
     _RequiredMarketoDestinationPropertiesTypeDef, _OptionalMarketoDestinationPropertiesTypeDef
 ):
     pass
 
+
 _RequiredRedshiftDestinationPropertiesTypeDef = TypedDict(
     "_RequiredRedshiftDestinationPropertiesTypeDef",
     {
         "object": str,
         "intermediateBucketName": str,
     },
 )
@@ -1723,19 +1923,46 @@
     {
         "bucketPrefix": str,
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
     },
     total=False,
 )
 
+
 class RedshiftDestinationPropertiesTypeDef(
     _RequiredRedshiftDestinationPropertiesTypeDef, _OptionalRedshiftDestinationPropertiesTypeDef
 ):
     pass
 
+
+_RequiredSalesforceDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredSalesforceDestinationPropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+_OptionalSalesforceDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalSalesforceDestinationPropertiesOutputTypeDef",
+    {
+        "idFieldNames": List[str],
+        "errorHandlingConfig": ErrorHandlingConfigTypeDef,
+        "writeOperationType": WriteOperationTypeType,
+        "dataTransferApi": SalesforceDataTransferApiType,
+    },
+    total=False,
+)
+
+
+class SalesforceDestinationPropertiesOutputTypeDef(
+    _RequiredSalesforceDestinationPropertiesOutputTypeDef,
+    _OptionalSalesforceDestinationPropertiesOutputTypeDef,
+):
+    pass
+
+
 _RequiredSalesforceDestinationPropertiesTypeDef = TypedDict(
     "_RequiredSalesforceDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalSalesforceDestinationPropertiesTypeDef = TypedDict(
@@ -1745,19 +1972,21 @@
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
         "writeOperationType": WriteOperationTypeType,
         "dataTransferApi": SalesforceDataTransferApiType,
     },
     total=False,
 )
 
+
 class SalesforceDestinationPropertiesTypeDef(
     _RequiredSalesforceDestinationPropertiesTypeDef, _OptionalSalesforceDestinationPropertiesTypeDef
 ):
     pass
 
+
 _RequiredSnowflakeDestinationPropertiesTypeDef = TypedDict(
     "_RequiredSnowflakeDestinationPropertiesTypeDef",
     {
         "object": str,
         "intermediateBucketName": str,
     },
 )
@@ -1766,19 +1995,45 @@
     {
         "bucketPrefix": str,
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
     },
     total=False,
 )
 
+
 class SnowflakeDestinationPropertiesTypeDef(
     _RequiredSnowflakeDestinationPropertiesTypeDef, _OptionalSnowflakeDestinationPropertiesTypeDef
 ):
     pass
 
+
+_RequiredZendeskDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredZendeskDestinationPropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+_OptionalZendeskDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalZendeskDestinationPropertiesOutputTypeDef",
+    {
+        "idFieldNames": List[str],
+        "errorHandlingConfig": ErrorHandlingConfigTypeDef,
+        "writeOperationType": WriteOperationTypeType,
+    },
+    total=False,
+)
+
+
+class ZendeskDestinationPropertiesOutputTypeDef(
+    _RequiredZendeskDestinationPropertiesOutputTypeDef,
+    _OptionalZendeskDestinationPropertiesOutputTypeDef,
+):
+    pass
+
+
 _RequiredZendeskDestinationPropertiesTypeDef = TypedDict(
     "_RequiredZendeskDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalZendeskDestinationPropertiesTypeDef = TypedDict(
@@ -1787,19 +2042,30 @@
         "idFieldNames": Sequence[str],
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
         "writeOperationType": WriteOperationTypeType,
     },
     total=False,
 )
 
+
 class ZendeskDestinationPropertiesTypeDef(
     _RequiredZendeskDestinationPropertiesTypeDef, _OptionalZendeskDestinationPropertiesTypeDef
 ):
     pass
 
+
+CustomConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "CustomConnectorProfilePropertiesOutputTypeDef",
+    {
+        "profileProperties": Dict[str, str],
+        "oAuth2Properties": OAuth2PropertiesOutputTypeDef,
+    },
+    total=False,
+)
+
 CustomConnectorProfilePropertiesTypeDef = TypedDict(
     "CustomConnectorProfilePropertiesTypeDef",
     {
         "profileProperties": Mapping[str, str],
         "oAuth2Properties": OAuth2PropertiesTypeDef,
     },
     total=False,
@@ -1853,17 +2119,19 @@
         "supportedDateFormat": str,
         "fieldValueRange": RangeTypeDef,
         "fieldLengthRange": RangeTypeDef,
     },
     total=False,
 )
 
+
 class FieldTypeDetailsTypeDef(_RequiredFieldTypeDetailsTypeDef, _OptionalFieldTypeDetailsTypeDef):
     pass
 
+
 MetadataCatalogConfigTypeDef = TypedDict(
     "MetadataCatalogConfigTypeDef",
     {
         "glueDataCatalog": GlueDataCatalogConfigTypeDef,
     },
     total=False,
 )
@@ -1887,14 +2155,41 @@
         "authCodeUrls": List[str],
         "oauth2GrantTypesSupported": List[OAuth2GrantTypeType],
         "oauth2CustomProperties": List[OAuth2CustomParameterTypeDef],
     },
     total=False,
 )
 
+_RequiredSAPODataConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "_RequiredSAPODataConnectorProfilePropertiesOutputTypeDef",
+    {
+        "applicationHostUrl": str,
+        "applicationServicePath": str,
+        "portNumber": int,
+        "clientNumber": str,
+    },
+)
+_OptionalSAPODataConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "_OptionalSAPODataConnectorProfilePropertiesOutputTypeDef",
+    {
+        "logonLanguage": str,
+        "privateLinkServiceName": str,
+        "oAuthProperties": OAuthPropertiesOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class SAPODataConnectorProfilePropertiesOutputTypeDef(
+    _RequiredSAPODataConnectorProfilePropertiesOutputTypeDef,
+    _OptionalSAPODataConnectorProfilePropertiesOutputTypeDef,
+):
+    pass
+
+
 _RequiredSAPODataConnectorProfilePropertiesTypeDef = TypedDict(
     "_RequiredSAPODataConnectorProfilePropertiesTypeDef",
     {
         "applicationHostUrl": str,
         "applicationServicePath": str,
         "portNumber": int,
         "clientNumber": str,
@@ -1906,20 +2201,56 @@
         "logonLanguage": str,
         "privateLinkServiceName": str,
         "oAuthProperties": OAuthPropertiesTypeDef,
     },
     total=False,
 )
 
+
 class SAPODataConnectorProfilePropertiesTypeDef(
     _RequiredSAPODataConnectorProfilePropertiesTypeDef,
     _OptionalSAPODataConnectorProfilePropertiesTypeDef,
 ):
     pass
 
+
+S3OutputFormatConfigOutputTypeDef = TypedDict(
+    "S3OutputFormatConfigOutputTypeDef",
+    {
+        "fileType": FileTypeType,
+        "prefixConfig": PrefixConfigOutputTypeDef,
+        "aggregationConfig": AggregationConfigTypeDef,
+        "preserveSourceDataTyping": bool,
+    },
+    total=False,
+)
+
+_RequiredUpsolverS3OutputFormatConfigOutputTypeDef = TypedDict(
+    "_RequiredUpsolverS3OutputFormatConfigOutputTypeDef",
+    {
+        "prefixConfig": PrefixConfigOutputTypeDef,
+    },
+)
+_OptionalUpsolverS3OutputFormatConfigOutputTypeDef = TypedDict(
+    "_OptionalUpsolverS3OutputFormatConfigOutputTypeDef",
+    {
+        "fileType": FileTypeType,
+        "aggregationConfig": AggregationConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class UpsolverS3OutputFormatConfigOutputTypeDef(
+    _RequiredUpsolverS3OutputFormatConfigOutputTypeDef,
+    _OptionalUpsolverS3OutputFormatConfigOutputTypeDef,
+):
+    pass
+
+
 S3OutputFormatConfigTypeDef = TypedDict(
     "S3OutputFormatConfigTypeDef",
     {
         "fileType": FileTypeType,
         "prefixConfig": PrefixConfigTypeDef,
         "aggregationConfig": AggregationConfigTypeDef,
         "preserveSourceDataTyping": bool,
@@ -1938,19 +2269,21 @@
     {
         "fileType": FileTypeType,
         "aggregationConfig": AggregationConfigTypeDef,
     },
     total=False,
 )
 
+
 class UpsolverS3OutputFormatConfigTypeDef(
     _RequiredUpsolverS3OutputFormatConfigTypeDef, _OptionalUpsolverS3OutputFormatConfigTypeDef
 ):
     pass
 
+
 _RequiredS3SourcePropertiesTypeDef = TypedDict(
     "_RequiredS3SourcePropertiesTypeDef",
     {
         "bucketName": str,
     },
 )
 _OptionalS3SourcePropertiesTypeDef = TypedDict(
@@ -1958,19 +2291,46 @@
     {
         "bucketPrefix": str,
         "s3InputFormatConfig": S3InputFormatConfigTypeDef,
     },
     total=False,
 )
 
+
 class S3SourcePropertiesTypeDef(
     _RequiredS3SourcePropertiesTypeDef, _OptionalS3SourcePropertiesTypeDef
 ):
     pass
 
+
+_RequiredSAPODataDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredSAPODataDestinationPropertiesOutputTypeDef",
+    {
+        "objectPath": str,
+    },
+)
+_OptionalSAPODataDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalSAPODataDestinationPropertiesOutputTypeDef",
+    {
+        "successResponseHandlingConfig": SuccessResponseHandlingConfigTypeDef,
+        "idFieldNames": List[str],
+        "errorHandlingConfig": ErrorHandlingConfigTypeDef,
+        "writeOperationType": WriteOperationTypeType,
+    },
+    total=False,
+)
+
+
+class SAPODataDestinationPropertiesOutputTypeDef(
+    _RequiredSAPODataDestinationPropertiesOutputTypeDef,
+    _OptionalSAPODataDestinationPropertiesOutputTypeDef,
+):
+    pass
+
+
 _RequiredSAPODataDestinationPropertiesTypeDef = TypedDict(
     "_RequiredSAPODataDestinationPropertiesTypeDef",
     {
         "objectPath": str,
     },
 )
 _OptionalSAPODataDestinationPropertiesTypeDef = TypedDict(
@@ -1980,27 +2340,56 @@
         "idFieldNames": Sequence[str],
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
         "writeOperationType": WriteOperationTypeType,
     },
     total=False,
 )
 
+
 class SAPODataDestinationPropertiesTypeDef(
     _RequiredSAPODataDestinationPropertiesTypeDef, _OptionalSAPODataDestinationPropertiesTypeDef
 ):
     pass
 
-TriggerPropertiesTypeDef = TypedDict(
-    "TriggerPropertiesTypeDef",
+
+TriggerPropertiesOutputTypeDef = TypedDict(
+    "TriggerPropertiesOutputTypeDef",
     {
-        "Scheduled": ScheduledTriggerPropertiesTypeDef,
+        "Scheduled": ScheduledTriggerPropertiesOutputTypeDef,
     },
     total=False,
 )
 
+_RequiredScheduledTriggerPropertiesTypeDef = TypedDict(
+    "_RequiredScheduledTriggerPropertiesTypeDef",
+    {
+        "scheduleExpression": str,
+    },
+)
+_OptionalScheduledTriggerPropertiesTypeDef = TypedDict(
+    "_OptionalScheduledTriggerPropertiesTypeDef",
+    {
+        "dataPullMode": DataPullModeType,
+        "scheduleStartTime": TimestampTypeDef,
+        "scheduleEndTime": TimestampTypeDef,
+        "timezone": str,
+        "scheduleOffset": int,
+        "firstExecutionFrom": TimestampTypeDef,
+        "flowErrorDeactivationThreshold": int,
+    },
+    total=False,
+)
+
+
+class ScheduledTriggerPropertiesTypeDef(
+    _RequiredScheduledTriggerPropertiesTypeDef, _OptionalScheduledTriggerPropertiesTypeDef
+):
+    pass
+
+
 _RequiredCustomConnectorProfileCredentialsTypeDef = TypedDict(
     "_RequiredCustomConnectorProfileCredentialsTypeDef",
     {
         "authenticationType": AuthenticationTypeType,
     },
 )
 _OptionalCustomConnectorProfileCredentialsTypeDef = TypedDict(
@@ -2010,29 +2399,32 @@
         "oauth2": OAuth2CredentialsTypeDef,
         "apiKey": ApiKeyCredentialsTypeDef,
         "custom": CustomAuthCredentialsTypeDef,
     },
     total=False,
 )
 
+
 class CustomConnectorProfileCredentialsTypeDef(
     _RequiredCustomConnectorProfileCredentialsTypeDef,
     _OptionalCustomConnectorProfileCredentialsTypeDef,
 ):
     pass
 
+
 SAPODataConnectorProfileCredentialsTypeDef = TypedDict(
     "SAPODataConnectorProfileCredentialsTypeDef",
     {
         "basicAuthCredentials": BasicAuthCredentialsTypeDef,
         "oAuthCredentials": OAuthCredentialsTypeDef,
     },
     total=False,
 )
 
+TaskUnionTypeDef = Union[TaskTypeDef, TaskOutputTypeDef]
 RegisterConnectorRequestRequestTypeDef = TypedDict(
     "RegisterConnectorRequestRequestTypeDef",
     {
         "connectorLabel": str,
         "description": str,
         "connectorProvisioningType": Literal["LAMBDA"],
         "connectorProvisioningConfig": ConnectorProvisioningConfigTypeDef,
@@ -2053,26 +2445,28 @@
         "description": str,
         "connectorProvisioningConfig": ConnectorProvisioningConfigTypeDef,
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateConnectorRegistrationRequestRequestTypeDef(
     _RequiredUpdateConnectorRegistrationRequestRequestTypeDef,
     _OptionalUpdateConnectorRegistrationRequestRequestTypeDef,
 ):
     pass
 
+
 ListFlowsResponseTypeDef = TypedDict(
     "ListFlowsResponseTypeDef",
     {
         "flows": List[FlowDefinitionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SupportedFieldTypeDetailsTypeDef = TypedDict(
     "SupportedFieldTypeDetailsTypeDef",
     {
         "v1": FieldTypeDetailsTypeDef,
@@ -2103,14 +2497,40 @@
         "isCustomAuthSupported": bool,
         "oAuth2Defaults": OAuth2DefaultsTypeDef,
         "customAuthConfigs": List[CustomAuthConfigTypeDef],
     },
     total=False,
 )
 
+ConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "ConnectorProfilePropertiesOutputTypeDef",
+    {
+        "Amplitude": Dict[str, Any],
+        "Datadog": DatadogConnectorProfilePropertiesTypeDef,
+        "Dynatrace": DynatraceConnectorProfilePropertiesTypeDef,
+        "GoogleAnalytics": Dict[str, Any],
+        "Honeycode": Dict[str, Any],
+        "InforNexus": InforNexusConnectorProfilePropertiesTypeDef,
+        "Marketo": MarketoConnectorProfilePropertiesTypeDef,
+        "Redshift": RedshiftConnectorProfilePropertiesTypeDef,
+        "Salesforce": SalesforceConnectorProfilePropertiesTypeDef,
+        "ServiceNow": ServiceNowConnectorProfilePropertiesTypeDef,
+        "Singular": Dict[str, Any],
+        "Slack": SlackConnectorProfilePropertiesTypeDef,
+        "Snowflake": SnowflakeConnectorProfilePropertiesTypeDef,
+        "Trendmicro": Dict[str, Any],
+        "Veeva": VeevaConnectorProfilePropertiesTypeDef,
+        "Zendesk": ZendeskConnectorProfilePropertiesTypeDef,
+        "SAPOData": SAPODataConnectorProfilePropertiesOutputTypeDef,
+        "CustomConnector": CustomConnectorProfilePropertiesOutputTypeDef,
+        "Pardot": PardotConnectorProfilePropertiesTypeDef,
+    },
+    total=False,
+)
+
 ConnectorProfilePropertiesTypeDef = TypedDict(
     "ConnectorProfilePropertiesTypeDef",
     {
         "Amplitude": Mapping[str, Any],
         "Datadog": DatadogConnectorProfilePropertiesTypeDef,
         "Dynatrace": DynatraceConnectorProfilePropertiesTypeDef,
         "GoogleAnalytics": Mapping[str, Any],
@@ -2129,14 +2549,59 @@
         "SAPOData": SAPODataConnectorProfilePropertiesTypeDef,
         "CustomConnector": CustomConnectorProfilePropertiesTypeDef,
         "Pardot": PardotConnectorProfilePropertiesTypeDef,
     },
     total=False,
 )
 
+_RequiredS3DestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredS3DestinationPropertiesOutputTypeDef",
+    {
+        "bucketName": str,
+    },
+)
+_OptionalS3DestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalS3DestinationPropertiesOutputTypeDef",
+    {
+        "bucketPrefix": str,
+        "s3OutputFormatConfig": S3OutputFormatConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class S3DestinationPropertiesOutputTypeDef(
+    _RequiredS3DestinationPropertiesOutputTypeDef, _OptionalS3DestinationPropertiesOutputTypeDef
+):
+    pass
+
+
+_RequiredUpsolverDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredUpsolverDestinationPropertiesOutputTypeDef",
+    {
+        "bucketName": str,
+        "s3OutputFormatConfig": UpsolverS3OutputFormatConfigOutputTypeDef,
+    },
+)
+_OptionalUpsolverDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalUpsolverDestinationPropertiesOutputTypeDef",
+    {
+        "bucketPrefix": str,
+    },
+    total=False,
+)
+
+
+class UpsolverDestinationPropertiesOutputTypeDef(
+    _RequiredUpsolverDestinationPropertiesOutputTypeDef,
+    _OptionalUpsolverDestinationPropertiesOutputTypeDef,
+):
+    pass
+
+
 _RequiredS3DestinationPropertiesTypeDef = TypedDict(
     "_RequiredS3DestinationPropertiesTypeDef",
     {
         "bucketName": str,
     },
 )
 _OptionalS3DestinationPropertiesTypeDef = TypedDict(
@@ -2144,19 +2609,21 @@
     {
         "bucketPrefix": str,
         "s3OutputFormatConfig": S3OutputFormatConfigTypeDef,
     },
     total=False,
 )
 
+
 class S3DestinationPropertiesTypeDef(
     _RequiredS3DestinationPropertiesTypeDef, _OptionalS3DestinationPropertiesTypeDef
 ):
     pass
 
+
 _RequiredUpsolverDestinationPropertiesTypeDef = TypedDict(
     "_RequiredUpsolverDestinationPropertiesTypeDef",
     {
         "bucketName": str,
         "s3OutputFormatConfig": UpsolverS3OutputFormatConfigTypeDef,
     },
 )
@@ -2164,19 +2631,45 @@
     "_OptionalUpsolverDestinationPropertiesTypeDef",
     {
         "bucketPrefix": str,
     },
     total=False,
 )
 
+
 class UpsolverDestinationPropertiesTypeDef(
     _RequiredUpsolverDestinationPropertiesTypeDef, _OptionalUpsolverDestinationPropertiesTypeDef
 ):
     pass
 
+
+SourceConnectorPropertiesOutputTypeDef = TypedDict(
+    "SourceConnectorPropertiesOutputTypeDef",
+    {
+        "Amplitude": AmplitudeSourcePropertiesTypeDef,
+        "Datadog": DatadogSourcePropertiesTypeDef,
+        "Dynatrace": DynatraceSourcePropertiesTypeDef,
+        "GoogleAnalytics": GoogleAnalyticsSourcePropertiesTypeDef,
+        "InforNexus": InforNexusSourcePropertiesTypeDef,
+        "Marketo": MarketoSourcePropertiesTypeDef,
+        "S3": S3SourcePropertiesTypeDef,
+        "Salesforce": SalesforceSourcePropertiesTypeDef,
+        "ServiceNow": ServiceNowSourcePropertiesTypeDef,
+        "Singular": SingularSourcePropertiesTypeDef,
+        "Slack": SlackSourcePropertiesTypeDef,
+        "Trendmicro": TrendmicroSourcePropertiesTypeDef,
+        "Veeva": VeevaSourcePropertiesTypeDef,
+        "Zendesk": ZendeskSourcePropertiesTypeDef,
+        "SAPOData": SAPODataSourcePropertiesTypeDef,
+        "CustomConnector": CustomConnectorSourcePropertiesOutputTypeDef,
+        "Pardot": PardotSourcePropertiesTypeDef,
+    },
+    total=False,
+)
+
 SourceConnectorPropertiesTypeDef = TypedDict(
     "SourceConnectorPropertiesTypeDef",
     {
         "Amplitude": AmplitudeSourcePropertiesTypeDef,
         "Datadog": DatadogSourcePropertiesTypeDef,
         "Dynatrace": DynatraceSourcePropertiesTypeDef,
         "GoogleAnalytics": GoogleAnalyticsSourcePropertiesTypeDef,
@@ -2193,31 +2686,43 @@
         "SAPOData": SAPODataSourcePropertiesTypeDef,
         "CustomConnector": CustomConnectorSourcePropertiesTypeDef,
         "Pardot": PardotSourcePropertiesTypeDef,
     },
     total=False,
 )
 
-_RequiredTriggerConfigTypeDef = TypedDict(
-    "_RequiredTriggerConfigTypeDef",
+_RequiredTriggerConfigOutputTypeDef = TypedDict(
+    "_RequiredTriggerConfigOutputTypeDef",
     {
         "triggerType": TriggerTypeType,
     },
 )
-_OptionalTriggerConfigTypeDef = TypedDict(
-    "_OptionalTriggerConfigTypeDef",
+_OptionalTriggerConfigOutputTypeDef = TypedDict(
+    "_OptionalTriggerConfigOutputTypeDef",
     {
-        "triggerProperties": TriggerPropertiesTypeDef,
+        "triggerProperties": TriggerPropertiesOutputTypeDef,
     },
     total=False,
 )
 
-class TriggerConfigTypeDef(_RequiredTriggerConfigTypeDef, _OptionalTriggerConfigTypeDef):
+
+class TriggerConfigOutputTypeDef(
+    _RequiredTriggerConfigOutputTypeDef, _OptionalTriggerConfigOutputTypeDef
+):
     pass
 
+
+TriggerPropertiesTypeDef = TypedDict(
+    "TriggerPropertiesTypeDef",
+    {
+        "Scheduled": ScheduledTriggerPropertiesTypeDef,
+    },
+    total=False,
+)
+
 ConnectorProfileCredentialsTypeDef = TypedDict(
     "ConnectorProfileCredentialsTypeDef",
     {
         "Amplitude": AmplitudeConnectorProfileCredentialsTypeDef,
         "Datadog": DatadogConnectorProfileCredentialsTypeDef,
         "Dynatrace": DynatraceConnectorProfileCredentialsTypeDef,
         "GoogleAnalytics": GoogleAnalyticsConnectorProfileCredentialsTypeDef,
@@ -2259,25 +2764,27 @@
         "sourceProperties": SourceFieldPropertiesTypeDef,
         "destinationProperties": DestinationFieldPropertiesTypeDef,
         "customProperties": Dict[str, str],
     },
     total=False,
 )
 
+
 class ConnectorEntityFieldTypeDef(
     _RequiredConnectorEntityFieldTypeDef, _OptionalConnectorEntityFieldTypeDef
 ):
     pass
 
+
 DescribeFlowExecutionRecordsResponseTypeDef = TypedDict(
     "DescribeFlowExecutionRecordsResponseTypeDef",
     {
         "flowExecutions": List[ExecutionRecordTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConnectorConfigurationTypeDef = TypedDict(
     "ConnectorConfigurationTypeDef",
     {
         "canUseAsSource": bool,
@@ -2317,22 +2824,42 @@
     {
         "connectorProfileArn": str,
         "connectorProfileName": str,
         "connectorType": ConnectorTypeType,
         "connectorLabel": str,
         "connectionMode": ConnectionModeType,
         "credentialsArn": str,
-        "connectorProfileProperties": ConnectorProfilePropertiesTypeDef,
+        "connectorProfileProperties": ConnectorProfilePropertiesOutputTypeDef,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "privateConnectionProvisioningState": PrivateConnectionProvisioningStateTypeDef,
     },
     total=False,
 )
 
+DestinationConnectorPropertiesOutputTypeDef = TypedDict(
+    "DestinationConnectorPropertiesOutputTypeDef",
+    {
+        "Redshift": RedshiftDestinationPropertiesTypeDef,
+        "S3": S3DestinationPropertiesOutputTypeDef,
+        "Salesforce": SalesforceDestinationPropertiesOutputTypeDef,
+        "Snowflake": SnowflakeDestinationPropertiesTypeDef,
+        "EventBridge": EventBridgeDestinationPropertiesTypeDef,
+        "LookoutMetrics": Dict[str, Any],
+        "Upsolver": UpsolverDestinationPropertiesOutputTypeDef,
+        "Honeycode": HoneycodeDestinationPropertiesTypeDef,
+        "CustomerProfiles": CustomerProfilesDestinationPropertiesTypeDef,
+        "Zendesk": ZendeskDestinationPropertiesOutputTypeDef,
+        "Marketo": MarketoDestinationPropertiesTypeDef,
+        "CustomConnector": CustomConnectorDestinationPropertiesOutputTypeDef,
+        "SAPOData": SAPODataDestinationPropertiesOutputTypeDef,
+    },
+    total=False,
+)
+
 DestinationConnectorPropertiesTypeDef = TypedDict(
     "DestinationConnectorPropertiesTypeDef",
     {
         "Redshift": RedshiftDestinationPropertiesTypeDef,
         "S3": S3DestinationPropertiesTypeDef,
         "Salesforce": SalesforceDestinationPropertiesTypeDef,
         "Snowflake": SnowflakeDestinationPropertiesTypeDef,
@@ -2345,14 +2872,38 @@
         "Marketo": MarketoDestinationPropertiesTypeDef,
         "CustomConnector": CustomConnectorDestinationPropertiesTypeDef,
         "SAPOData": SAPODataDestinationPropertiesTypeDef,
     },
     total=False,
 )
 
+_RequiredSourceFlowConfigOutputTypeDef = TypedDict(
+    "_RequiredSourceFlowConfigOutputTypeDef",
+    {
+        "connectorType": ConnectorTypeType,
+        "sourceConnectorProperties": SourceConnectorPropertiesOutputTypeDef,
+    },
+)
+_OptionalSourceFlowConfigOutputTypeDef = TypedDict(
+    "_OptionalSourceFlowConfigOutputTypeDef",
+    {
+        "apiVersion": str,
+        "connectorProfileName": str,
+        "incrementalPullConfig": IncrementalPullConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class SourceFlowConfigOutputTypeDef(
+    _RequiredSourceFlowConfigOutputTypeDef, _OptionalSourceFlowConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredSourceFlowConfigTypeDef = TypedDict(
     "_RequiredSourceFlowConfigTypeDef",
     {
         "connectorType": ConnectorTypeType,
         "sourceConnectorProperties": SourceConnectorPropertiesTypeDef,
     },
 )
@@ -2362,71 +2913,117 @@
         "apiVersion": str,
         "connectorProfileName": str,
         "incrementalPullConfig": IncrementalPullConfigTypeDef,
     },
     total=False,
 )
 
+
 class SourceFlowConfigTypeDef(_RequiredSourceFlowConfigTypeDef, _OptionalSourceFlowConfigTypeDef):
     pass
 
+
+_RequiredTriggerConfigTypeDef = TypedDict(
+    "_RequiredTriggerConfigTypeDef",
+    {
+        "triggerType": TriggerTypeType,
+    },
+)
+_OptionalTriggerConfigTypeDef = TypedDict(
+    "_OptionalTriggerConfigTypeDef",
+    {
+        "triggerProperties": TriggerPropertiesTypeDef,
+    },
+    total=False,
+)
+
+
+class TriggerConfigTypeDef(_RequiredTriggerConfigTypeDef, _OptionalTriggerConfigTypeDef):
+    pass
+
+
 _RequiredConnectorProfileConfigTypeDef = TypedDict(
     "_RequiredConnectorProfileConfigTypeDef",
     {
         "connectorProfileProperties": ConnectorProfilePropertiesTypeDef,
     },
 )
 _OptionalConnectorProfileConfigTypeDef = TypedDict(
     "_OptionalConnectorProfileConfigTypeDef",
     {
         "connectorProfileCredentials": ConnectorProfileCredentialsTypeDef,
     },
     total=False,
 )
 
+
 class ConnectorProfileConfigTypeDef(
     _RequiredConnectorProfileConfigTypeDef, _OptionalConnectorProfileConfigTypeDef
 ):
     pass
 
+
 DescribeConnectorEntityResponseTypeDef = TypedDict(
     "DescribeConnectorEntityResponseTypeDef",
     {
         "connectorEntityFields": List[ConnectorEntityFieldTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConnectorResponseTypeDef = TypedDict(
     "DescribeConnectorResponseTypeDef",
     {
         "connectorConfiguration": ConnectorConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConnectorsResponseTypeDef = TypedDict(
     "DescribeConnectorsResponseTypeDef",
     {
         "connectorConfigurations": Dict[ConnectorTypeType, ConnectorConfigurationTypeDef],
         "connectors": List[ConnectorDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConnectorProfilesResponseTypeDef = TypedDict(
     "DescribeConnectorProfilesResponseTypeDef",
     {
         "connectorProfileDetails": List[ConnectorProfileTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredDestinationFlowConfigOutputTypeDef = TypedDict(
+    "_RequiredDestinationFlowConfigOutputTypeDef",
+    {
+        "connectorType": ConnectorTypeType,
+        "destinationConnectorProperties": DestinationConnectorPropertiesOutputTypeDef,
+    },
+)
+_OptionalDestinationFlowConfigOutputTypeDef = TypedDict(
+    "_OptionalDestinationFlowConfigOutputTypeDef",
+    {
+        "apiVersion": str,
+        "connectorProfileName": str,
+    },
+    total=False,
+)
+
+
+class DestinationFlowConfigOutputTypeDef(
+    _RequiredDestinationFlowConfigOutputTypeDef, _OptionalDestinationFlowConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredDestinationFlowConfigTypeDef = TypedDict(
     "_RequiredDestinationFlowConfigTypeDef",
     {
         "connectorType": ConnectorTypeType,
         "destinationConnectorProperties": DestinationConnectorPropertiesTypeDef,
     },
 )
@@ -2435,19 +3032,23 @@
     {
         "apiVersion": str,
         "connectorProfileName": str,
     },
     total=False,
 )
 
+
 class DestinationFlowConfigTypeDef(
     _RequiredDestinationFlowConfigTypeDef, _OptionalDestinationFlowConfigTypeDef
 ):
     pass
 
+
+SourceFlowConfigUnionTypeDef = Union[SourceFlowConfigTypeDef, SourceFlowConfigOutputTypeDef]
+TriggerConfigUnionTypeDef = Union[TriggerConfigTypeDef, TriggerConfigOutputTypeDef]
 _RequiredCreateConnectorProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectorProfileRequestRequestTypeDef",
     {
         "connectorProfileName": str,
         "connectorType": ConnectorTypeType,
         "connectionMode": ConnectionModeType,
         "connectorProfileConfig": ConnectorProfileConfigTypeDef,
@@ -2459,20 +3060,22 @@
         "kmsArn": str,
         "connectorLabel": str,
         "clientToken": str,
     },
     total=False,
 )
 
+
 class CreateConnectorProfileRequestRequestTypeDef(
     _RequiredCreateConnectorProfileRequestRequestTypeDef,
     _OptionalCreateConnectorProfileRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateConnectorProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateConnectorProfileRequestRequestTypeDef",
     {
         "connectorProfileName": str,
         "connectionMode": ConnectionModeType,
         "connectorProfileConfig": ConnectorProfileConfigTypeDef,
     },
@@ -2481,90 +3084,98 @@
     "_OptionalUpdateConnectorProfileRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateConnectorProfileRequestRequestTypeDef(
     _RequiredUpdateConnectorProfileRequestRequestTypeDef,
     _OptionalUpdateConnectorProfileRequestRequestTypeDef,
 ):
     pass
 
+
+DescribeFlowResponseTypeDef = TypedDict(
+    "DescribeFlowResponseTypeDef",
+    {
+        "flowArn": str,
+        "description": str,
+        "flowName": str,
+        "kmsArn": str,
+        "flowStatus": FlowStatusType,
+        "flowStatusMessage": str,
+        "sourceFlowConfig": SourceFlowConfigOutputTypeDef,
+        "destinationFlowConfigList": List[DestinationFlowConfigOutputTypeDef],
+        "lastRunExecutionDetails": ExecutionDetailsTypeDef,
+        "triggerConfig": TriggerConfigOutputTypeDef,
+        "tasks": List[TaskOutputTypeDef],
+        "createdAt": datetime,
+        "lastUpdatedAt": datetime,
+        "createdBy": str,
+        "lastUpdatedBy": str,
+        "tags": Dict[str, str],
+        "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
+        "lastRunMetadataCatalogDetails": List[MetadataCatalogDetailTypeDef],
+        "schemaVersion": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DestinationFlowConfigUnionTypeDef = Union[
+    DestinationFlowConfigTypeDef, DestinationFlowConfigOutputTypeDef
+]
 _RequiredCreateFlowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFlowRequestRequestTypeDef",
     {
         "flowName": str,
         "triggerConfig": TriggerConfigTypeDef,
         "sourceFlowConfig": SourceFlowConfigTypeDef,
-        "destinationFlowConfigList": Sequence[DestinationFlowConfigTypeDef],
-        "tasks": Sequence[TaskTypeDef],
+        "destinationFlowConfigList": Sequence[DestinationFlowConfigUnionTypeDef],
+        "tasks": Sequence[TaskUnionTypeDef],
     },
 )
 _OptionalCreateFlowRequestRequestTypeDef = TypedDict(
     "_OptionalCreateFlowRequestRequestTypeDef",
     {
         "description": str,
         "kmsArn": str,
         "tags": Mapping[str, str],
         "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
         "clientToken": str,
     },
     total=False,
 )
 
+
 class CreateFlowRequestRequestTypeDef(
     _RequiredCreateFlowRequestRequestTypeDef, _OptionalCreateFlowRequestRequestTypeDef
 ):
     pass
 
-DescribeFlowResponseTypeDef = TypedDict(
-    "DescribeFlowResponseTypeDef",
-    {
-        "flowArn": str,
-        "description": str,
-        "flowName": str,
-        "kmsArn": str,
-        "flowStatus": FlowStatusType,
-        "flowStatusMessage": str,
-        "sourceFlowConfig": SourceFlowConfigTypeDef,
-        "destinationFlowConfigList": List[DestinationFlowConfigTypeDef],
-        "lastRunExecutionDetails": ExecutionDetailsTypeDef,
-        "triggerConfig": TriggerConfigTypeDef,
-        "tasks": List[TaskTypeDef],
-        "createdAt": datetime,
-        "lastUpdatedAt": datetime,
-        "createdBy": str,
-        "lastUpdatedBy": str,
-        "tags": Dict[str, str],
-        "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
-        "lastRunMetadataCatalogDetails": List[MetadataCatalogDetailTypeDef],
-        "schemaVersion": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdateFlowRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFlowRequestRequestTypeDef",
     {
         "flowName": str,
         "triggerConfig": TriggerConfigTypeDef,
         "sourceFlowConfig": SourceFlowConfigTypeDef,
-        "destinationFlowConfigList": Sequence[DestinationFlowConfigTypeDef],
-        "tasks": Sequence[TaskTypeDef],
+        "destinationFlowConfigList": Sequence[DestinationFlowConfigUnionTypeDef],
+        "tasks": Sequence[TaskUnionTypeDef],
     },
 )
 _OptionalUpdateFlowRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateFlowRequestRequestTypeDef",
     {
         "description": str,
         "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateFlowRequestRequestTypeDef(
     _RequiredUpdateFlowRequestRequestTypeDef, _OptionalUpdateFlowRequestRequestTypeDef
 ):
     pass
```

### Comparing `types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow.egg-info/PKG-INFO` & `types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appflow
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Appflow 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Appflow 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore appflow type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore appflow type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-appflow"></a>
 
 # types-aiobotocore-appflow
 
 [![PyPI - types-aiobotocore-appflow](https://img.shields.io/pypi/v/types-aiobotocore-appflow.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appflow)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appflow.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appflow)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-appflow?color=blue)](https://pypistats.org/packages/types-aiobotocore-appflow)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appflow)](https://pepy.tech/project/types-aiobotocore-appflow)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Appflow 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
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
 [types-aiobotocore-appflow docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/).
 
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
@@ -323,31 +322,31 @@
 )
 
 
 def check_value(value: AggregationTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_appflow.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_appflow.type_defs import (
     AggregationConfigTypeDef,
     AmplitudeConnectorProfileCredentialsTypeDef,
     AmplitudeSourcePropertiesTypeDef,
     ApiKeyCredentialsTypeDef,
     AuthParameterTypeDef,
     BasicAuthCredentialsTypeDef,
     CancelFlowExecutionsRequestRequestTypeDef,
-    CancelFlowExecutionsResponseTypeDef,
+    ResponseMetadataTypeDef,
     ConnectorRuntimeSettingTypeDef,
     DataTransferApiTypeDef,
     ConnectorDetailTypeDef,
     DestinationFieldPropertiesTypeDef,
     SourceFieldPropertiesTypeDef,
     ConnectorEntityTypeDef,
     GoogleAnalyticsMetadataTypeDef,
@@ -377,18 +376,17 @@
     ServiceNowConnectorProfilePropertiesTypeDef,
     SlackConnectorProfilePropertiesTypeDef,
     SnowflakeConnectorProfilePropertiesTypeDef,
     VeevaConnectorProfilePropertiesTypeDef,
     ZendeskConnectorProfilePropertiesTypeDef,
     PrivateConnectionProvisioningStateTypeDef,
     LambdaConnectorProvisioningConfigTypeDef,
-    CreateConnectorProfileResponseTypeDef,
-    CreateFlowResponseTypeDef,
     CustomAuthCredentialsTypeDef,
     ErrorHandlingConfigTypeDef,
+    OAuth2PropertiesOutputTypeDef,
     OAuth2PropertiesTypeDef,
     CustomerProfilesDestinationPropertiesTypeDef,
     DatadogSourcePropertiesTypeDef,
     DeleteConnectorProfileRequestRequestTypeDef,
     DeleteFlowRequestRequestTypeDef,
     DescribeConnectorEntityRequestRequestTypeDef,
     DescribeConnectorProfilesRequestRequestTypeDef,
@@ -404,117 +402,146 @@
     GoogleAnalyticsSourcePropertiesTypeDef,
     IncrementalPullConfigTypeDef,
     InforNexusSourcePropertiesTypeDef,
     ListConnectorEntitiesRequestRequestTypeDef,
     ListConnectorsRequestRequestTypeDef,
     ListFlowsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     MarketoSourcePropertiesTypeDef,
     RegistrationOutputTypeDef,
     OAuth2CustomParameterTypeDef,
+    OAuthPropertiesOutputTypeDef,
     OAuthPropertiesTypeDef,
     PardotSourcePropertiesTypeDef,
+    PrefixConfigOutputTypeDef,
     PrefixConfigTypeDef,
-    RegisterConnectorResponseTypeDef,
     ResetConnectorMetadataCacheRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     S3InputFormatConfigTypeDef,
     SuccessResponseHandlingConfigTypeDef,
     SAPODataSourcePropertiesTypeDef,
     SalesforceSourcePropertiesTypeDef,
-    ScheduledTriggerPropertiesTypeDef,
+    ScheduledTriggerPropertiesOutputTypeDef,
+    TimestampTypeDef,
     ServiceNowSourcePropertiesTypeDef,
     SingularSourcePropertiesTypeDef,
     SlackSourcePropertiesTypeDef,
     TrendmicroSourcePropertiesTypeDef,
     VeevaSourcePropertiesTypeDef,
     ZendeskSourcePropertiesTypeDef,
     StartFlowRequestRequestTypeDef,
-    StartFlowResponseTypeDef,
     StopFlowRequestRequestTypeDef,
-    StopFlowResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UnregisterConnectorRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    CustomAuthConfigTypeDef,
+    CancelFlowExecutionsResponseTypeDef,
+    CreateConnectorProfileResponseTypeDef,
+    CreateFlowResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RegisterConnectorResponseTypeDef,
+    StartFlowResponseTypeDef,
+    StopFlowResponseTypeDef,
     UpdateConnectorProfileResponseTypeDef,
     UpdateConnectorRegistrationResponseTypeDef,
     UpdateFlowResponseTypeDef,
-    CustomAuthConfigTypeDef,
+    CustomConnectorSourcePropertiesOutputTypeDef,
     CustomConnectorSourcePropertiesTypeDef,
     ListConnectorsResponseTypeDef,
     ListConnectorEntitiesResponseTypeDef,
     ConnectorMetadataTypeDef,
     GoogleAnalyticsConnectorProfileCredentialsTypeDef,
     HoneycodeConnectorProfileCredentialsTypeDef,
     MarketoConnectorProfileCredentialsTypeDef,
     OAuth2CredentialsTypeDef,
     OAuthCredentialsTypeDef,
     PardotConnectorProfileCredentialsTypeDef,
     SalesforceConnectorProfileCredentialsTypeDef,
     SlackConnectorProfileCredentialsTypeDef,
     ZendeskConnectorProfileCredentialsTypeDef,
+    TaskOutputTypeDef,
     TaskTypeDef,
     ConnectorProvisioningConfigTypeDef,
+    CustomConnectorDestinationPropertiesOutputTypeDef,
     CustomConnectorDestinationPropertiesTypeDef,
     EventBridgeDestinationPropertiesTypeDef,
     HoneycodeDestinationPropertiesTypeDef,
     MarketoDestinationPropertiesTypeDef,
     RedshiftDestinationPropertiesTypeDef,
+    SalesforceDestinationPropertiesOutputTypeDef,
     SalesforceDestinationPropertiesTypeDef,
     SnowflakeDestinationPropertiesTypeDef,
+    ZendeskDestinationPropertiesOutputTypeDef,
     ZendeskDestinationPropertiesTypeDef,
+    CustomConnectorProfilePropertiesOutputTypeDef,
     CustomConnectorProfilePropertiesTypeDef,
     FlowDefinitionTypeDef,
     ExecutionResultTypeDef,
     FieldTypeDetailsTypeDef,
     MetadataCatalogConfigTypeDef,
     MetadataCatalogDetailTypeDef,
     OAuth2DefaultsTypeDef,
+    SAPODataConnectorProfilePropertiesOutputTypeDef,
     SAPODataConnectorProfilePropertiesTypeDef,
+    S3OutputFormatConfigOutputTypeDef,
+    UpsolverS3OutputFormatConfigOutputTypeDef,
     S3OutputFormatConfigTypeDef,
     UpsolverS3OutputFormatConfigTypeDef,
     S3SourcePropertiesTypeDef,
+    SAPODataDestinationPropertiesOutputTypeDef,
     SAPODataDestinationPropertiesTypeDef,
-    TriggerPropertiesTypeDef,
+    TriggerPropertiesOutputTypeDef,
+    ScheduledTriggerPropertiesTypeDef,
     CustomConnectorProfileCredentialsTypeDef,
     SAPODataConnectorProfileCredentialsTypeDef,
+    TaskUnionTypeDef,
     RegisterConnectorRequestRequestTypeDef,
     UpdateConnectorRegistrationRequestRequestTypeDef,
     ListFlowsResponseTypeDef,
     SupportedFieldTypeDetailsTypeDef,
     ExecutionRecordTypeDef,
     AuthenticationConfigTypeDef,
+    ConnectorProfilePropertiesOutputTypeDef,
     ConnectorProfilePropertiesTypeDef,
+    S3DestinationPropertiesOutputTypeDef,
+    UpsolverDestinationPropertiesOutputTypeDef,
     S3DestinationPropertiesTypeDef,
     UpsolverDestinationPropertiesTypeDef,
+    SourceConnectorPropertiesOutputTypeDef,
     SourceConnectorPropertiesTypeDef,
-    TriggerConfigTypeDef,
+    TriggerConfigOutputTypeDef,
+    TriggerPropertiesTypeDef,
     ConnectorProfileCredentialsTypeDef,
     ConnectorEntityFieldTypeDef,
     DescribeFlowExecutionRecordsResponseTypeDef,
     ConnectorConfigurationTypeDef,
     ConnectorProfileTypeDef,
+    DestinationConnectorPropertiesOutputTypeDef,
     DestinationConnectorPropertiesTypeDef,
+    SourceFlowConfigOutputTypeDef,
     SourceFlowConfigTypeDef,
+    TriggerConfigTypeDef,
     ConnectorProfileConfigTypeDef,
     DescribeConnectorEntityResponseTypeDef,
     DescribeConnectorResponseTypeDef,
     DescribeConnectorsResponseTypeDef,
     DescribeConnectorProfilesResponseTypeDef,
+    DestinationFlowConfigOutputTypeDef,
     DestinationFlowConfigTypeDef,
+    SourceFlowConfigUnionTypeDef,
+    TriggerConfigUnionTypeDef,
     CreateConnectorProfileRequestRequestTypeDef,
     UpdateConnectorProfileRequestRequestTypeDef,
-    CreateFlowRequestRequestTypeDef,
     DescribeFlowResponseTypeDef,
+    DestinationFlowConfigUnionTypeDef,
+    CreateFlowRequestRequestTypeDef,
     UpdateFlowRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AggregationConfigTypeDef:
+def get_value() -> AggregationConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-appflow-2.5.2/types_aiobotocore_appflow.egg-info/SOURCES.txt` & `types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*


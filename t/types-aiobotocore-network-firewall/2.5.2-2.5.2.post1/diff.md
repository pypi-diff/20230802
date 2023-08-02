# Comparing `tmp/types-aiobotocore-network-firewall-2.5.2.tar.gz` & `tmp/types-aiobotocore-network-firewall-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-network-firewall-2.5.2.tar", last modified: Sat Jul  8 01:44:02 2023, max compression
+gzip compressed data, was "types-aiobotocore-network-firewall-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:43 2023, max compression
```

## Comparing `types-aiobotocore-network-firewall-2.5.2.tar` & `types-aiobotocore-network-firewall-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:02.718602 types-aiobotocore-network-firewall-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:35:42.000000 types-aiobotocore-network-firewall-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19798 2023-07-08 01:44:02.718602 types-aiobotocore-network-firewall-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18198 2023-07-08 01:35:42.000000 types-aiobotocore-network-firewall-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:02.718602 types-aiobotocore-network-firewall-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-08 01:35:42.000000 types-aiobotocore-network-firewall-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:02.714602 types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall/
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-08 01:35:42.000000 types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-08 01:35:42.000000 types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-08 01:35:42.000000 types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34077 2023-07-08 01:35:42.000000 types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    34027 2023-07-08 01:35:42.000000 types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-07-08 01:35:42.000000 types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-07-08 01:35:42.000000 types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-07-08 01:35:42.000000 types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-07-08 01:35:42.000000 types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:35:42.000000 types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    47547 2023-07-08 01:35:43.000000 types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    47491 2023-07-08 01:35:43.000000 types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:35:42.000000 types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:02.718602 types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19798 2023-07-08 01:44:02.000000 types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-08 01:44:02.000000 types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:02.000000 types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:02.000000 types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:02.000000 types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-08 01:44:02.000000 types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.301512 types-aiobotocore-network-firewall-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:43:58.000000 types-aiobotocore-network-firewall-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20704 2023-08-02 14:52:43.301512 types-aiobotocore-network-firewall-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19151 2023-08-02 14:43:58.000000 types-aiobotocore-network-firewall-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:43.301512 types-aiobotocore-network-firewall-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-02 14:43:58.000000 types-aiobotocore-network-firewall-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.297512 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-08-02 14:43:58.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-08-02 14:43:58.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-02 14:43:58.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34132 2023-08-02 14:43:58.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34082 2023-08-02 14:43:58.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-08-02 14:43:59.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-08-02 14:43:58.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-08-02 14:43:58.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-08-02 14:43:58.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:43:58.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    55815 2023-08-02 14:44:02.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55749 2023-08-02 14:43:59.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:43:58.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.301512 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20704 2023-08-02 14:52:43.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-02 14:52:43.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:43.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:43.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:43.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 14:52:43.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-network-firewall-2.5.2/LICENSE` & `types-aiobotocore-network-firewall-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-network-firewall-2.5.2/PKG-INFO` & `types-aiobotocore-network-firewall-2.5.2.post1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-network-firewall
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.NetworkFirewall 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.NetworkFirewall 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore network-firewall type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore network-firewall type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-network-firewall"></a>
 
 # types-aiobotocore-network-firewall
 
 [![PyPI - types-aiobotocore-network-firewall](https://img.shields.io/pypi/v/types-aiobotocore-network-firewall.svg?color=blue)](https://pypi.org/project/types-aiobotocore-network-firewall)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-network-firewall.svg?color=blue)](https://pypi.org/project/types-aiobotocore-network-firewall)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-network-firewall?color=blue)](https://pypistats.org/packages/types-aiobotocore-network-firewall)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-network-firewall)](https://pepy.tech/project/types-aiobotocore-network-firewall)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.NetworkFirewall 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
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
 [types-aiobotocore-network-firewall docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/).
 
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
@@ -346,26 +345,26 @@
 )
 
 
 def check_value(value: AttachmentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_network_firewall.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_network_firewall.type_defs import (
     AddressTypeDef,
     AssociateFirewallPolicyRequestRequestTypeDef,
-    AssociateFirewallPolicyResponseTypeDef,
+    ResponseMetadataTypeDef,
     SubnetMappingTypeDef,
     AttachmentTypeDef,
     IPSetMetadataTypeDef,
     EncryptionConfigurationTypeDef,
     TagTypeDef,
     SourceMetadataTypeDef,
     DeleteFirewallPolicyRequestRequestTypeDef,
@@ -373,130 +372,158 @@
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRuleGroupRequestRequestTypeDef,
     DeleteTLSInspectionConfigurationRequestRequestTypeDef,
     DescribeFirewallPolicyRequestRequestTypeDef,
     DescribeFirewallRequestRequestTypeDef,
     DescribeLoggingConfigurationRequestRequestTypeDef,
     DescribeResourcePolicyRequestRequestTypeDef,
-    DescribeResourcePolicyResponseTypeDef,
     DescribeRuleGroupMetadataRequestRequestTypeDef,
     StatefulRuleOptionsTypeDef,
     DescribeRuleGroupRequestRequestTypeDef,
     DescribeTLSInspectionConfigurationRequestRequestTypeDef,
     DimensionTypeDef,
     DisassociateSubnetsRequestRequestTypeDef,
     FirewallMetadataTypeDef,
     FirewallPolicyMetadataTypeDef,
     StatefulEngineOptionsTypeDef,
     StatelessRuleGroupReferenceTypeDef,
     HeaderTypeDef,
+    IPSetOutputTypeDef,
     IPSetReferenceTypeDef,
     IPSetTypeDef,
-    ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListFirewallPoliciesRequestRequestTypeDef,
-    ListFirewallsRequestListFirewallsPaginateTypeDef,
     ListFirewallsRequestRequestTypeDef,
-    ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     RuleGroupMetadataTypeDef,
-    ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef,
     ListTLSInspectionConfigurationsRequestRequestTypeDef,
     TLSInspectionConfigurationMetadataTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    LogDestinationConfigOutputTypeDef,
     LogDestinationConfigTypeDef,
     PortRangeTypeDef,
+    TCPFlagFieldOutputTypeDef,
     TCPFlagFieldTypeDef,
-    PaginatorConfigTypeDef,
     PerObjectStatusTypeDef,
+    PortSetOutputTypeDef,
     PortSetTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    RuleOptionOutputTypeDef,
     RuleOptionTypeDef,
+    RulesSourceListOutputTypeDef,
     RulesSourceListTypeDef,
     ServerCertificateTypeDef,
     StatefulRuleGroupOverrideTypeDef,
     TlsCertificateDataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFirewallDeleteProtectionRequestRequestTypeDef,
-    UpdateFirewallDeleteProtectionResponseTypeDef,
     UpdateFirewallDescriptionRequestRequestTypeDef,
-    UpdateFirewallDescriptionResponseTypeDef,
     UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef,
-    UpdateFirewallPolicyChangeProtectionResponseTypeDef,
     UpdateSubnetChangeProtectionRequestRequestTypeDef,
+    AssociateFirewallPolicyResponseTypeDef,
+    DescribeResourcePolicyResponseTypeDef,
+    UpdateFirewallDeleteProtectionResponseTypeDef,
+    UpdateFirewallDescriptionResponseTypeDef,
+    UpdateFirewallPolicyChangeProtectionResponseTypeDef,
     UpdateSubnetChangeProtectionResponseTypeDef,
     AssociateSubnetsRequestRequestTypeDef,
     AssociateSubnetsResponseTypeDef,
     DisassociateSubnetsResponseTypeDef,
     CIDRSummaryTypeDef,
     UpdateFirewallEncryptionConfigurationRequestRequestTypeDef,
     UpdateFirewallEncryptionConfigurationResponseTypeDef,
     CreateFirewallRequestRequestTypeDef,
     FirewallPolicyResponseTypeDef,
     FirewallTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     RuleGroupResponseTypeDef,
     DescribeRuleGroupMetadataResponseTypeDef,
+    PublishMetricActionOutputTypeDef,
     PublishMetricActionTypeDef,
     ListFirewallsResponseTypeDef,
     ListFirewallPoliciesResponseTypeDef,
+    PolicyVariablesOutputTypeDef,
+    ReferenceSetsOutputTypeDef,
     ReferenceSetsTypeDef,
     PolicyVariablesTypeDef,
+    ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef,
+    ListFirewallsRequestListFirewallsPaginateTypeDef,
+    ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
+    ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListRuleGroupsResponseTypeDef,
     ListTLSInspectionConfigurationsResponseTypeDef,
+    LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
+    ServerCertificateScopeOutputTypeDef,
     ServerCertificateScopeTypeDef,
+    MatchAttributesOutputTypeDef,
     MatchAttributesTypeDef,
     SyncStateTypeDef,
+    RuleVariablesOutputTypeDef,
     RuleVariablesTypeDef,
+    StatefulRuleOutputTypeDef,
     StatefulRuleTypeDef,
     StatefulRuleGroupReferenceTypeDef,
     TLSInspectionConfigurationResponseTypeDef,
     CapacityUsageSummaryTypeDef,
     CreateFirewallPolicyResponseTypeDef,
     DeleteFirewallPolicyResponseTypeDef,
     UpdateFirewallPolicyResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     DeleteRuleGroupResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
+    ActionDefinitionOutputTypeDef,
     ActionDefinitionTypeDef,
     DescribeLoggingConfigurationResponseTypeDef,
-    UpdateLoggingConfigurationRequestRequestTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
+    LoggingConfigurationUnionTypeDef,
+    UpdateLoggingConfigurationRequestRequestTypeDef,
+    ServerCertificateConfigurationOutputTypeDef,
     ServerCertificateConfigurationTypeDef,
+    RuleDefinitionOutputTypeDef,
     RuleDefinitionTypeDef,
     CreateTLSInspectionConfigurationResponseTypeDef,
     DeleteTLSInspectionConfigurationResponseTypeDef,
     UpdateTLSInspectionConfigurationResponseTypeDef,
     FirewallStatusTypeDef,
+    CustomActionOutputTypeDef,
     CustomActionTypeDef,
+    TLSInspectionConfigurationOutputTypeDef,
     TLSInspectionConfigurationTypeDef,
+    StatelessRuleOutputTypeDef,
     StatelessRuleTypeDef,
     CreateFirewallResponseTypeDef,
     DeleteFirewallResponseTypeDef,
     DescribeFirewallResponseTypeDef,
+    FirewallPolicyOutputTypeDef,
     FirewallPolicyTypeDef,
-    CreateTLSInspectionConfigurationRequestRequestTypeDef,
     DescribeTLSInspectionConfigurationResponseTypeDef,
+    CreateTLSInspectionConfigurationRequestRequestTypeDef,
+    TLSInspectionConfigurationUnionTypeDef,
     UpdateTLSInspectionConfigurationRequestRequestTypeDef,
+    StatelessRulesAndCustomActionsOutputTypeDef,
     StatelessRulesAndCustomActionsTypeDef,
-    CreateFirewallPolicyRequestRequestTypeDef,
     DescribeFirewallPolicyResponseTypeDef,
+    CreateFirewallPolicyRequestRequestTypeDef,
+    FirewallPolicyUnionTypeDef,
     UpdateFirewallPolicyRequestRequestTypeDef,
+    RulesSourceOutputTypeDef,
     RulesSourceTypeDef,
+    RuleGroupOutputTypeDef,
     RuleGroupTypeDef,
-    CreateRuleGroupRequestRequestTypeDef,
     DescribeRuleGroupResponseTypeDef,
+    CreateRuleGroupRequestRequestTypeDef,
+    RuleGroupUnionTypeDef,
     UpdateRuleGroupRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddressTypeDef:
+def get_value() -> AddressTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-network-firewall-2.5.2/README.md` & `types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-network-firewall
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.NetworkFirewall 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore network-firewall type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-network-firewall"></a>
 
 # types-aiobotocore-network-firewall
 
 [![PyPI - types-aiobotocore-network-firewall](https://img.shields.io/pypi/v/types-aiobotocore-network-firewall.svg?color=blue)](https://pypi.org/project/types-aiobotocore-network-firewall)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-network-firewall.svg?color=blue)](https://pypi.org/project/types-aiobotocore-network-firewall)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-network-firewall?color=blue)](https://pypistats.org/packages/types-aiobotocore-network-firewall)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-network-firewall)](https://pepy.tech/project/types-aiobotocore-network-firewall)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.NetworkFirewall 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
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
 [types-aiobotocore-network-firewall docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/).
 
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
@@ -313,26 +345,26 @@
 )
 
 
 def check_value(value: AttachmentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_network_firewall.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_network_firewall.type_defs import (
     AddressTypeDef,
     AssociateFirewallPolicyRequestRequestTypeDef,
-    AssociateFirewallPolicyResponseTypeDef,
+    ResponseMetadataTypeDef,
     SubnetMappingTypeDef,
     AttachmentTypeDef,
     IPSetMetadataTypeDef,
     EncryptionConfigurationTypeDef,
     TagTypeDef,
     SourceMetadataTypeDef,
     DeleteFirewallPolicyRequestRequestTypeDef,
@@ -340,130 +372,158 @@
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRuleGroupRequestRequestTypeDef,
     DeleteTLSInspectionConfigurationRequestRequestTypeDef,
     DescribeFirewallPolicyRequestRequestTypeDef,
     DescribeFirewallRequestRequestTypeDef,
     DescribeLoggingConfigurationRequestRequestTypeDef,
     DescribeResourcePolicyRequestRequestTypeDef,
-    DescribeResourcePolicyResponseTypeDef,
     DescribeRuleGroupMetadataRequestRequestTypeDef,
     StatefulRuleOptionsTypeDef,
     DescribeRuleGroupRequestRequestTypeDef,
     DescribeTLSInspectionConfigurationRequestRequestTypeDef,
     DimensionTypeDef,
     DisassociateSubnetsRequestRequestTypeDef,
     FirewallMetadataTypeDef,
     FirewallPolicyMetadataTypeDef,
     StatefulEngineOptionsTypeDef,
     StatelessRuleGroupReferenceTypeDef,
     HeaderTypeDef,
+    IPSetOutputTypeDef,
     IPSetReferenceTypeDef,
     IPSetTypeDef,
-    ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListFirewallPoliciesRequestRequestTypeDef,
-    ListFirewallsRequestListFirewallsPaginateTypeDef,
     ListFirewallsRequestRequestTypeDef,
-    ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     RuleGroupMetadataTypeDef,
-    ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef,
     ListTLSInspectionConfigurationsRequestRequestTypeDef,
     TLSInspectionConfigurationMetadataTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    LogDestinationConfigOutputTypeDef,
     LogDestinationConfigTypeDef,
     PortRangeTypeDef,
+    TCPFlagFieldOutputTypeDef,
     TCPFlagFieldTypeDef,
-    PaginatorConfigTypeDef,
     PerObjectStatusTypeDef,
+    PortSetOutputTypeDef,
     PortSetTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    RuleOptionOutputTypeDef,
     RuleOptionTypeDef,
+    RulesSourceListOutputTypeDef,
     RulesSourceListTypeDef,
     ServerCertificateTypeDef,
     StatefulRuleGroupOverrideTypeDef,
     TlsCertificateDataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFirewallDeleteProtectionRequestRequestTypeDef,
-    UpdateFirewallDeleteProtectionResponseTypeDef,
     UpdateFirewallDescriptionRequestRequestTypeDef,
-    UpdateFirewallDescriptionResponseTypeDef,
     UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef,
-    UpdateFirewallPolicyChangeProtectionResponseTypeDef,
     UpdateSubnetChangeProtectionRequestRequestTypeDef,
+    AssociateFirewallPolicyResponseTypeDef,
+    DescribeResourcePolicyResponseTypeDef,
+    UpdateFirewallDeleteProtectionResponseTypeDef,
+    UpdateFirewallDescriptionResponseTypeDef,
+    UpdateFirewallPolicyChangeProtectionResponseTypeDef,
     UpdateSubnetChangeProtectionResponseTypeDef,
     AssociateSubnetsRequestRequestTypeDef,
     AssociateSubnetsResponseTypeDef,
     DisassociateSubnetsResponseTypeDef,
     CIDRSummaryTypeDef,
     UpdateFirewallEncryptionConfigurationRequestRequestTypeDef,
     UpdateFirewallEncryptionConfigurationResponseTypeDef,
     CreateFirewallRequestRequestTypeDef,
     FirewallPolicyResponseTypeDef,
     FirewallTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     RuleGroupResponseTypeDef,
     DescribeRuleGroupMetadataResponseTypeDef,
+    PublishMetricActionOutputTypeDef,
     PublishMetricActionTypeDef,
     ListFirewallsResponseTypeDef,
     ListFirewallPoliciesResponseTypeDef,
+    PolicyVariablesOutputTypeDef,
+    ReferenceSetsOutputTypeDef,
     ReferenceSetsTypeDef,
     PolicyVariablesTypeDef,
+    ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef,
+    ListFirewallsRequestListFirewallsPaginateTypeDef,
+    ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
+    ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListRuleGroupsResponseTypeDef,
     ListTLSInspectionConfigurationsResponseTypeDef,
+    LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
+    ServerCertificateScopeOutputTypeDef,
     ServerCertificateScopeTypeDef,
+    MatchAttributesOutputTypeDef,
     MatchAttributesTypeDef,
     SyncStateTypeDef,
+    RuleVariablesOutputTypeDef,
     RuleVariablesTypeDef,
+    StatefulRuleOutputTypeDef,
     StatefulRuleTypeDef,
     StatefulRuleGroupReferenceTypeDef,
     TLSInspectionConfigurationResponseTypeDef,
     CapacityUsageSummaryTypeDef,
     CreateFirewallPolicyResponseTypeDef,
     DeleteFirewallPolicyResponseTypeDef,
     UpdateFirewallPolicyResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     DeleteRuleGroupResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
+    ActionDefinitionOutputTypeDef,
     ActionDefinitionTypeDef,
     DescribeLoggingConfigurationResponseTypeDef,
-    UpdateLoggingConfigurationRequestRequestTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
+    LoggingConfigurationUnionTypeDef,
+    UpdateLoggingConfigurationRequestRequestTypeDef,
+    ServerCertificateConfigurationOutputTypeDef,
     ServerCertificateConfigurationTypeDef,
+    RuleDefinitionOutputTypeDef,
     RuleDefinitionTypeDef,
     CreateTLSInspectionConfigurationResponseTypeDef,
     DeleteTLSInspectionConfigurationResponseTypeDef,
     UpdateTLSInspectionConfigurationResponseTypeDef,
     FirewallStatusTypeDef,
+    CustomActionOutputTypeDef,
     CustomActionTypeDef,
+    TLSInspectionConfigurationOutputTypeDef,
     TLSInspectionConfigurationTypeDef,
+    StatelessRuleOutputTypeDef,
     StatelessRuleTypeDef,
     CreateFirewallResponseTypeDef,
     DeleteFirewallResponseTypeDef,
     DescribeFirewallResponseTypeDef,
+    FirewallPolicyOutputTypeDef,
     FirewallPolicyTypeDef,
-    CreateTLSInspectionConfigurationRequestRequestTypeDef,
     DescribeTLSInspectionConfigurationResponseTypeDef,
+    CreateTLSInspectionConfigurationRequestRequestTypeDef,
+    TLSInspectionConfigurationUnionTypeDef,
     UpdateTLSInspectionConfigurationRequestRequestTypeDef,
+    StatelessRulesAndCustomActionsOutputTypeDef,
     StatelessRulesAndCustomActionsTypeDef,
-    CreateFirewallPolicyRequestRequestTypeDef,
     DescribeFirewallPolicyResponseTypeDef,
+    CreateFirewallPolicyRequestRequestTypeDef,
+    FirewallPolicyUnionTypeDef,
     UpdateFirewallPolicyRequestRequestTypeDef,
+    RulesSourceOutputTypeDef,
     RulesSourceTypeDef,
+    RuleGroupOutputTypeDef,
     RuleGroupTypeDef,
-    CreateRuleGroupRequestRequestTypeDef,
     DescribeRuleGroupResponseTypeDef,
+    CreateRuleGroupRequestRequestTypeDef,
+    RuleGroupUnionTypeDef,
     UpdateRuleGroupRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddressTypeDef:
+def get_value() -> AddressTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-network-firewall-2.5.2/setup.py` & `types-aiobotocore-network-firewall-2.5.2.post1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-network-firewall",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_network_firewall"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.NetworkFirewall 2.5.2 service generated with"
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
-    keywords="aiobotocore network-firewall type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore network-firewall type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_network_firewall": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/"
```

### Comparing `types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall/__init__.py` & `types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall/__init__.pyi` & `types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall/__main__.py` & `types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.NetworkFirewall 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.NetworkFirewall 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall\nOther"
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

### Comparing `types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall/client.py` & `types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -44,26 +44,26 @@
     DescribeLoggingConfigurationResponseTypeDef,
     DescribeResourcePolicyResponseTypeDef,
     DescribeRuleGroupMetadataResponseTypeDef,
     DescribeRuleGroupResponseTypeDef,
     DescribeTLSInspectionConfigurationResponseTypeDef,
     DisassociateSubnetsResponseTypeDef,
     EncryptionConfigurationTypeDef,
-    FirewallPolicyTypeDef,
+    FirewallPolicyUnionTypeDef,
     ListFirewallPoliciesResponseTypeDef,
     ListFirewallsResponseTypeDef,
     ListRuleGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTLSInspectionConfigurationsResponseTypeDef,
-    LoggingConfigurationTypeDef,
-    RuleGroupTypeDef,
+    LoggingConfigurationUnionTypeDef,
+    RuleGroupUnionTypeDef,
     SourceMetadataTypeDef,
     SubnetMappingTypeDef,
     TagTypeDef,
-    TLSInspectionConfigurationTypeDef,
+    TLSInspectionConfigurationUnionTypeDef,
     UpdateFirewallDeleteProtectionResponseTypeDef,
     UpdateFirewallDescriptionResponseTypeDef,
     UpdateFirewallEncryptionConfigurationResponseTypeDef,
     UpdateFirewallPolicyChangeProtectionResponseTypeDef,
     UpdateFirewallPolicyResponseTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
@@ -72,26 +72,23 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("NetworkFirewallClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     InsufficientCapacityException: Type[BotocoreClientError]
     InternalServerError: Type[BotocoreClientError]
     InvalidOperationException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
     InvalidResourcePolicyException: Type[BotocoreClientError]
@@ -99,15 +96,14 @@
     LimitExceededException: Type[BotocoreClientError]
     LogDestinationPermissionException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ResourceOwnerCheckException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     UnsupportedOperationException: Type[BotocoreClientError]
 
-
 class NetworkFirewallClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/)
     """
 
     meta: ClientMeta
@@ -116,61 +112,56 @@
     def exceptions(self) -> Exceptions:
         """
         NetworkFirewallClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#exceptions)
         """
-
     async def associate_firewall_policy(
         self,
         *,
         FirewallPolicyArn: str,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...
     ) -> AssociateFirewallPolicyResponseTypeDef:
         """
         Associates a  FirewallPolicy to a  Firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.associate_firewall_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#associate_firewall_policy)
         """
-
     async def associate_subnets(
         self,
         *,
         SubnetMappings: Sequence[SubnetMappingTypeDef],
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...
     ) -> AssociateSubnetsResponseTypeDef:
         """
         Associates the specified subnets in the Amazon VPC to the firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.associate_subnets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#associate_subnets)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#can_paginate)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#close)
         """
-
     async def create_firewall(
         self,
         *,
         FirewallName: str,
         FirewallPolicyArn: str,
         VpcId: str,
         SubnetMappings: Sequence[SubnetMappingTypeDef],
@@ -184,238 +175,218 @@
         """
         Creates an Network Firewall  Firewall and accompanying  FirewallStatus for a
         VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.create_firewall)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#create_firewall)
         """
-
     async def create_firewall_policy(
         self,
         *,
         FirewallPolicyName: str,
-        FirewallPolicy: FirewallPolicyTypeDef,
+        FirewallPolicy: FirewallPolicyUnionTypeDef,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> CreateFirewallPolicyResponseTypeDef:
         """
         Creates the firewall policy for the firewall according to the specifications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.create_firewall_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#create_firewall_policy)
         """
-
     async def create_rule_group(
         self,
         *,
         RuleGroupName: str,
         Type: RuleGroupTypeType,
         Capacity: int,
-        RuleGroup: RuleGroupTypeDef = ...,
+        RuleGroup: RuleGroupUnionTypeDef = ...,
         Rules: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
         SourceMetadata: SourceMetadataTypeDef = ...
     ) -> CreateRuleGroupResponseTypeDef:
         """
         Creates the specified stateless or stateful rule group, which includes the rules
         for network traffic inspection, a capacity setting, and tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.create_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#create_rule_group)
         """
-
     async def create_tls_inspection_configuration(
         self,
         *,
         TLSInspectionConfigurationName: str,
-        TLSInspectionConfiguration: TLSInspectionConfigurationTypeDef,
+        TLSInspectionConfiguration: TLSInspectionConfigurationUnionTypeDef,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> CreateTLSInspectionConfigurationResponseTypeDef:
         """
         Creates an Network Firewall TLS inspection configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.create_tls_inspection_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#create_tls_inspection_configuration)
         """
-
     async def delete_firewall(
         self, *, FirewallName: str = ..., FirewallArn: str = ...
     ) -> DeleteFirewallResponseTypeDef:
         """
         Deletes the specified  Firewall and its  FirewallStatus.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.delete_firewall)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#delete_firewall)
         """
-
     async def delete_firewall_policy(
         self, *, FirewallPolicyName: str = ..., FirewallPolicyArn: str = ...
     ) -> DeleteFirewallPolicyResponseTypeDef:
         """
         Deletes the specified  FirewallPolicy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.delete_firewall_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#delete_firewall_policy)
         """
-
     async def delete_resource_policy(self, *, ResourceArn: str) -> Dict[str, Any]:
         """
         Deletes a resource policy that you created in a  PutResourcePolicy request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.delete_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#delete_resource_policy)
         """
-
     async def delete_rule_group(
         self, *, RuleGroupName: str = ..., RuleGroupArn: str = ..., Type: RuleGroupTypeType = ...
     ) -> DeleteRuleGroupResponseTypeDef:
         """
         Deletes the specified  RuleGroup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.delete_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#delete_rule_group)
         """
-
     async def delete_tls_inspection_configuration(
         self, *, TLSInspectionConfigurationArn: str = ..., TLSInspectionConfigurationName: str = ...
     ) -> DeleteTLSInspectionConfigurationResponseTypeDef:
         """
         Deletes the specified  TLSInspectionConfiguration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.delete_tls_inspection_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#delete_tls_inspection_configuration)
         """
-
     async def describe_firewall(
         self, *, FirewallName: str = ..., FirewallArn: str = ...
     ) -> DescribeFirewallResponseTypeDef:
         """
         Returns the data objects for the specified firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.describe_firewall)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#describe_firewall)
         """
-
     async def describe_firewall_policy(
         self, *, FirewallPolicyName: str = ..., FirewallPolicyArn: str = ...
     ) -> DescribeFirewallPolicyResponseTypeDef:
         """
         Returns the data objects for the specified firewall policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.describe_firewall_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#describe_firewall_policy)
         """
-
     async def describe_logging_configuration(
         self, *, FirewallArn: str = ..., FirewallName: str = ...
     ) -> DescribeLoggingConfigurationResponseTypeDef:
         """
         Returns the logging configuration for the specified firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.describe_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#describe_logging_configuration)
         """
-
     async def describe_resource_policy(
         self, *, ResourceArn: str
     ) -> DescribeResourcePolicyResponseTypeDef:
         """
         Retrieves a resource policy that you created in a  PutResourcePolicy request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.describe_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#describe_resource_policy)
         """
-
     async def describe_rule_group(
         self, *, RuleGroupName: str = ..., RuleGroupArn: str = ..., Type: RuleGroupTypeType = ...
     ) -> DescribeRuleGroupResponseTypeDef:
         """
         Returns the data objects for the specified rule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.describe_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#describe_rule_group)
         """
-
     async def describe_rule_group_metadata(
         self, *, RuleGroupName: str = ..., RuleGroupArn: str = ..., Type: RuleGroupTypeType = ...
     ) -> DescribeRuleGroupMetadataResponseTypeDef:
         """
         High-level information about a rule group, returned by operations like create
         and describe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.describe_rule_group_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#describe_rule_group_metadata)
         """
-
     async def describe_tls_inspection_configuration(
         self, *, TLSInspectionConfigurationArn: str = ..., TLSInspectionConfigurationName: str = ...
     ) -> DescribeTLSInspectionConfigurationResponseTypeDef:
         """
         Returns the data objects for the specified TLS inspection configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.describe_tls_inspection_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#describe_tls_inspection_configuration)
         """
-
     async def disassociate_subnets(
         self,
         *,
         SubnetIds: Sequence[str],
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...
     ) -> DisassociateSubnetsResponseTypeDef:
         """
         Removes the specified subnet associations from the firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.disassociate_subnets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#disassociate_subnets)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#generate_presigned_url)
         """
-
     async def list_firewall_policies(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListFirewallPoliciesResponseTypeDef:
         """
         Retrieves the metadata for the firewall policies that you have defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.list_firewall_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#list_firewall_policies)
         """
-
     async def list_firewalls(
         self, *, NextToken: str = ..., VpcIds: Sequence[str] = ..., MaxResults: int = ...
     ) -> ListFirewallsResponseTypeDef:
         """
         Retrieves the metadata for the firewalls that you have defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.list_firewalls)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#list_firewalls)
         """
-
     async def list_rule_groups(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Scope: ResourceManagedStatusType = ...,
         ManagedType: ResourceManagedTypeType = ...,
@@ -423,60 +394,54 @@
     ) -> ListRuleGroupsResponseTypeDef:
         """
         Retrieves the metadata for the rule groups that you have defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.list_rule_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#list_rule_groups)
         """
-
     async def list_tags_for_resource(
         self, *, ResourceArn: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Retrieves the tags associated with the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#list_tags_for_resource)
         """
-
     async def list_tls_inspection_configurations(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListTLSInspectionConfigurationsResponseTypeDef:
         """
         Retrieves the metadata for the TLS inspection configurations that you have
         defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.list_tls_inspection_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#list_tls_inspection_configurations)
         """
-
     async def put_resource_policy(self, *, ResourceArn: str, Policy: str) -> Dict[str, Any]:
         """
         Creates or updates an IAM policy for your rule group or firewall policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.put_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#put_resource_policy)
         """
-
     async def tag_resource(self, *, ResourceArn: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Adds the specified tags to the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#tag_resource)
         """
-
     async def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes the tags with the specified keys from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#untag_resource)
         """
-
     async def update_firewall_delete_protection(
         self,
         *,
         DeleteProtection: bool,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...
@@ -484,63 +449,59 @@
         """
         Modifies the flag, `DeleteProtection`, which indicates whether it is possible to
         delete the firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_delete_protection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_firewall_delete_protection)
         """
-
     async def update_firewall_description(
         self,
         *,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...,
         Description: str = ...
     ) -> UpdateFirewallDescriptionResponseTypeDef:
         """
         Modifies the description for the specified firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_description)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_firewall_description)
         """
-
     async def update_firewall_encryption_configuration(
         self,
         *,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> UpdateFirewallEncryptionConfigurationResponseTypeDef:
         """
         A complex type that contains settings for encryption of your firewall resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_encryption_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_firewall_encryption_configuration)
         """
-
     async def update_firewall_policy(
         self,
         *,
         UpdateToken: str,
-        FirewallPolicy: FirewallPolicyTypeDef,
+        FirewallPolicy: FirewallPolicyUnionTypeDef,
         FirewallPolicyArn: str = ...,
         FirewallPolicyName: str = ...,
         Description: str = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> UpdateFirewallPolicyResponseTypeDef:
         """
         Updates the properties of the specified firewall policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_firewall_policy)
         """
-
     async def update_firewall_policy_change_protection(
         self,
         *,
         FirewallPolicyChangeProtection: bool,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...
@@ -548,50 +509,47 @@
         """
         Modifies the flag, `ChangeProtection`, which indicates whether it is possible to
         change the firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_policy_change_protection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_firewall_policy_change_protection)
         """
-
     async def update_logging_configuration(
         self,
         *,
         FirewallArn: str = ...,
         FirewallName: str = ...,
-        LoggingConfiguration: LoggingConfigurationTypeDef = ...
+        LoggingConfiguration: LoggingConfigurationUnionTypeDef = ...
     ) -> UpdateLoggingConfigurationResponseTypeDef:
         """
         Sets the logging configuration for the specified firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_logging_configuration)
         """
-
     async def update_rule_group(
         self,
         *,
         UpdateToken: str,
         RuleGroupArn: str = ...,
         RuleGroupName: str = ...,
-        RuleGroup: RuleGroupTypeDef = ...,
+        RuleGroup: RuleGroupUnionTypeDef = ...,
         Rules: str = ...,
         Type: RuleGroupTypeType = ...,
         Description: str = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
         SourceMetadata: SourceMetadataTypeDef = ...
     ) -> UpdateRuleGroupResponseTypeDef:
         """
         Updates the rule settings for the specified rule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_rule_group)
         """
-
     async def update_subnet_change_protection(
         self,
         *,
         SubnetChangeProtection: bool,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...
@@ -600,78 +558,70 @@
         See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/network-
         firewall-2020-11-12/UpdateSubnetChangeProtection).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_subnet_change_protection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_subnet_change_protection)
         """
-
     async def update_tls_inspection_configuration(
         self,
         *,
-        TLSInspectionConfiguration: TLSInspectionConfigurationTypeDef,
+        TLSInspectionConfiguration: TLSInspectionConfigurationUnionTypeDef,
         UpdateToken: str,
         TLSInspectionConfigurationArn: str = ...,
         TLSInspectionConfigurationName: str = ...,
         Description: str = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> UpdateTLSInspectionConfigurationResponseTypeDef:
         """
         Updates the TLS inspection configuration settings for the specified TLS
         inspection configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_tls_inspection_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_tls_inspection_configuration)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_firewall_policies"]
     ) -> ListFirewallPoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_firewalls"]) -> ListFirewallsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_rule_groups"]) -> ListRuleGroupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_tls_inspection_configurations"]
     ) -> ListTLSInspectionConfigurationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_tags_for_resource"]
     ) -> ListTagsForResourcePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#get_paginator)
         """
-
     async def __aenter__(self) -> "NetworkFirewallClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/)
         """
```

### Comparing `types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall/client.pyi` & `types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,26 +44,26 @@
     DescribeLoggingConfigurationResponseTypeDef,
     DescribeResourcePolicyResponseTypeDef,
     DescribeRuleGroupMetadataResponseTypeDef,
     DescribeRuleGroupResponseTypeDef,
     DescribeTLSInspectionConfigurationResponseTypeDef,
     DisassociateSubnetsResponseTypeDef,
     EncryptionConfigurationTypeDef,
-    FirewallPolicyTypeDef,
+    FirewallPolicyUnionTypeDef,
     ListFirewallPoliciesResponseTypeDef,
     ListFirewallsResponseTypeDef,
     ListRuleGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTLSInspectionConfigurationsResponseTypeDef,
-    LoggingConfigurationTypeDef,
-    RuleGroupTypeDef,
+    LoggingConfigurationUnionTypeDef,
+    RuleGroupUnionTypeDef,
     SourceMetadataTypeDef,
     SubnetMappingTypeDef,
     TagTypeDef,
-    TLSInspectionConfigurationTypeDef,
+    TLSInspectionConfigurationUnionTypeDef,
     UpdateFirewallDeleteProtectionResponseTypeDef,
     UpdateFirewallDescriptionResponseTypeDef,
     UpdateFirewallEncryptionConfigurationResponseTypeDef,
     UpdateFirewallPolicyChangeProtectionResponseTypeDef,
     UpdateFirewallPolicyResponseTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
@@ -72,23 +72,26 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("NetworkFirewallClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     InsufficientCapacityException: Type[BotocoreClientError]
     InternalServerError: Type[BotocoreClientError]
     InvalidOperationException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
     InvalidResourcePolicyException: Type[BotocoreClientError]
@@ -96,14 +99,15 @@
     LimitExceededException: Type[BotocoreClientError]
     LogDestinationPermissionException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ResourceOwnerCheckException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     UnsupportedOperationException: Type[BotocoreClientError]
 
+
 class NetworkFirewallClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/)
     """
 
     meta: ClientMeta
@@ -112,56 +116,61 @@
     def exceptions(self) -> Exceptions:
         """
         NetworkFirewallClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#exceptions)
         """
+
     async def associate_firewall_policy(
         self,
         *,
         FirewallPolicyArn: str,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...
     ) -> AssociateFirewallPolicyResponseTypeDef:
         """
         Associates a  FirewallPolicy to a  Firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.associate_firewall_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#associate_firewall_policy)
         """
+
     async def associate_subnets(
         self,
         *,
         SubnetMappings: Sequence[SubnetMappingTypeDef],
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...
     ) -> AssociateSubnetsResponseTypeDef:
         """
         Associates the specified subnets in the Amazon VPC to the firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.associate_subnets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#associate_subnets)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#can_paginate)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#close)
         """
+
     async def create_firewall(
         self,
         *,
         FirewallName: str,
         FirewallPolicyArn: str,
         VpcId: str,
         SubnetMappings: Sequence[SubnetMappingTypeDef],
@@ -175,218 +184,238 @@
         """
         Creates an Network Firewall  Firewall and accompanying  FirewallStatus for a
         VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.create_firewall)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#create_firewall)
         """
+
     async def create_firewall_policy(
         self,
         *,
         FirewallPolicyName: str,
-        FirewallPolicy: FirewallPolicyTypeDef,
+        FirewallPolicy: FirewallPolicyUnionTypeDef,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> CreateFirewallPolicyResponseTypeDef:
         """
         Creates the firewall policy for the firewall according to the specifications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.create_firewall_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#create_firewall_policy)
         """
+
     async def create_rule_group(
         self,
         *,
         RuleGroupName: str,
         Type: RuleGroupTypeType,
         Capacity: int,
-        RuleGroup: RuleGroupTypeDef = ...,
+        RuleGroup: RuleGroupUnionTypeDef = ...,
         Rules: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
         SourceMetadata: SourceMetadataTypeDef = ...
     ) -> CreateRuleGroupResponseTypeDef:
         """
         Creates the specified stateless or stateful rule group, which includes the rules
         for network traffic inspection, a capacity setting, and tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.create_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#create_rule_group)
         """
+
     async def create_tls_inspection_configuration(
         self,
         *,
         TLSInspectionConfigurationName: str,
-        TLSInspectionConfiguration: TLSInspectionConfigurationTypeDef,
+        TLSInspectionConfiguration: TLSInspectionConfigurationUnionTypeDef,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> CreateTLSInspectionConfigurationResponseTypeDef:
         """
         Creates an Network Firewall TLS inspection configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.create_tls_inspection_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#create_tls_inspection_configuration)
         """
+
     async def delete_firewall(
         self, *, FirewallName: str = ..., FirewallArn: str = ...
     ) -> DeleteFirewallResponseTypeDef:
         """
         Deletes the specified  Firewall and its  FirewallStatus.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.delete_firewall)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#delete_firewall)
         """
+
     async def delete_firewall_policy(
         self, *, FirewallPolicyName: str = ..., FirewallPolicyArn: str = ...
     ) -> DeleteFirewallPolicyResponseTypeDef:
         """
         Deletes the specified  FirewallPolicy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.delete_firewall_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#delete_firewall_policy)
         """
+
     async def delete_resource_policy(self, *, ResourceArn: str) -> Dict[str, Any]:
         """
         Deletes a resource policy that you created in a  PutResourcePolicy request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.delete_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#delete_resource_policy)
         """
+
     async def delete_rule_group(
         self, *, RuleGroupName: str = ..., RuleGroupArn: str = ..., Type: RuleGroupTypeType = ...
     ) -> DeleteRuleGroupResponseTypeDef:
         """
         Deletes the specified  RuleGroup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.delete_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#delete_rule_group)
         """
+
     async def delete_tls_inspection_configuration(
         self, *, TLSInspectionConfigurationArn: str = ..., TLSInspectionConfigurationName: str = ...
     ) -> DeleteTLSInspectionConfigurationResponseTypeDef:
         """
         Deletes the specified  TLSInspectionConfiguration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.delete_tls_inspection_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#delete_tls_inspection_configuration)
         """
+
     async def describe_firewall(
         self, *, FirewallName: str = ..., FirewallArn: str = ...
     ) -> DescribeFirewallResponseTypeDef:
         """
         Returns the data objects for the specified firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.describe_firewall)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#describe_firewall)
         """
+
     async def describe_firewall_policy(
         self, *, FirewallPolicyName: str = ..., FirewallPolicyArn: str = ...
     ) -> DescribeFirewallPolicyResponseTypeDef:
         """
         Returns the data objects for the specified firewall policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.describe_firewall_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#describe_firewall_policy)
         """
+
     async def describe_logging_configuration(
         self, *, FirewallArn: str = ..., FirewallName: str = ...
     ) -> DescribeLoggingConfigurationResponseTypeDef:
         """
         Returns the logging configuration for the specified firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.describe_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#describe_logging_configuration)
         """
+
     async def describe_resource_policy(
         self, *, ResourceArn: str
     ) -> DescribeResourcePolicyResponseTypeDef:
         """
         Retrieves a resource policy that you created in a  PutResourcePolicy request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.describe_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#describe_resource_policy)
         """
+
     async def describe_rule_group(
         self, *, RuleGroupName: str = ..., RuleGroupArn: str = ..., Type: RuleGroupTypeType = ...
     ) -> DescribeRuleGroupResponseTypeDef:
         """
         Returns the data objects for the specified rule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.describe_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#describe_rule_group)
         """
+
     async def describe_rule_group_metadata(
         self, *, RuleGroupName: str = ..., RuleGroupArn: str = ..., Type: RuleGroupTypeType = ...
     ) -> DescribeRuleGroupMetadataResponseTypeDef:
         """
         High-level information about a rule group, returned by operations like create
         and describe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.describe_rule_group_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#describe_rule_group_metadata)
         """
+
     async def describe_tls_inspection_configuration(
         self, *, TLSInspectionConfigurationArn: str = ..., TLSInspectionConfigurationName: str = ...
     ) -> DescribeTLSInspectionConfigurationResponseTypeDef:
         """
         Returns the data objects for the specified TLS inspection configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.describe_tls_inspection_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#describe_tls_inspection_configuration)
         """
+
     async def disassociate_subnets(
         self,
         *,
         SubnetIds: Sequence[str],
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...
     ) -> DisassociateSubnetsResponseTypeDef:
         """
         Removes the specified subnet associations from the firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.disassociate_subnets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#disassociate_subnets)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#generate_presigned_url)
         """
+
     async def list_firewall_policies(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListFirewallPoliciesResponseTypeDef:
         """
         Retrieves the metadata for the firewall policies that you have defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.list_firewall_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#list_firewall_policies)
         """
+
     async def list_firewalls(
         self, *, NextToken: str = ..., VpcIds: Sequence[str] = ..., MaxResults: int = ...
     ) -> ListFirewallsResponseTypeDef:
         """
         Retrieves the metadata for the firewalls that you have defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.list_firewalls)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#list_firewalls)
         """
+
     async def list_rule_groups(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Scope: ResourceManagedStatusType = ...,
         ManagedType: ResourceManagedTypeType = ...,
@@ -394,54 +423,60 @@
     ) -> ListRuleGroupsResponseTypeDef:
         """
         Retrieves the metadata for the rule groups that you have defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.list_rule_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#list_rule_groups)
         """
+
     async def list_tags_for_resource(
         self, *, ResourceArn: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Retrieves the tags associated with the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#list_tags_for_resource)
         """
+
     async def list_tls_inspection_configurations(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListTLSInspectionConfigurationsResponseTypeDef:
         """
         Retrieves the metadata for the TLS inspection configurations that you have
         defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.list_tls_inspection_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#list_tls_inspection_configurations)
         """
+
     async def put_resource_policy(self, *, ResourceArn: str, Policy: str) -> Dict[str, Any]:
         """
         Creates or updates an IAM policy for your rule group or firewall policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.put_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#put_resource_policy)
         """
+
     async def tag_resource(self, *, ResourceArn: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Adds the specified tags to the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#tag_resource)
         """
+
     async def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes the tags with the specified keys from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#untag_resource)
         """
+
     async def update_firewall_delete_protection(
         self,
         *,
         DeleteProtection: bool,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...
@@ -449,59 +484,63 @@
         """
         Modifies the flag, `DeleteProtection`, which indicates whether it is possible to
         delete the firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_delete_protection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_firewall_delete_protection)
         """
+
     async def update_firewall_description(
         self,
         *,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...,
         Description: str = ...
     ) -> UpdateFirewallDescriptionResponseTypeDef:
         """
         Modifies the description for the specified firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_description)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_firewall_description)
         """
+
     async def update_firewall_encryption_configuration(
         self,
         *,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> UpdateFirewallEncryptionConfigurationResponseTypeDef:
         """
         A complex type that contains settings for encryption of your firewall resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_encryption_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_firewall_encryption_configuration)
         """
+
     async def update_firewall_policy(
         self,
         *,
         UpdateToken: str,
-        FirewallPolicy: FirewallPolicyTypeDef,
+        FirewallPolicy: FirewallPolicyUnionTypeDef,
         FirewallPolicyArn: str = ...,
         FirewallPolicyName: str = ...,
         Description: str = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> UpdateFirewallPolicyResponseTypeDef:
         """
         Updates the properties of the specified firewall policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_firewall_policy)
         """
+
     async def update_firewall_policy_change_protection(
         self,
         *,
         FirewallPolicyChangeProtection: bool,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...
@@ -509,47 +548,50 @@
         """
         Modifies the flag, `ChangeProtection`, which indicates whether it is possible to
         change the firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_policy_change_protection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_firewall_policy_change_protection)
         """
+
     async def update_logging_configuration(
         self,
         *,
         FirewallArn: str = ...,
         FirewallName: str = ...,
-        LoggingConfiguration: LoggingConfigurationTypeDef = ...
+        LoggingConfiguration: LoggingConfigurationUnionTypeDef = ...
     ) -> UpdateLoggingConfigurationResponseTypeDef:
         """
         Sets the logging configuration for the specified firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_logging_configuration)
         """
+
     async def update_rule_group(
         self,
         *,
         UpdateToken: str,
         RuleGroupArn: str = ...,
         RuleGroupName: str = ...,
-        RuleGroup: RuleGroupTypeDef = ...,
+        RuleGroup: RuleGroupUnionTypeDef = ...,
         Rules: str = ...,
         Type: RuleGroupTypeType = ...,
         Description: str = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
         SourceMetadata: SourceMetadataTypeDef = ...
     ) -> UpdateRuleGroupResponseTypeDef:
         """
         Updates the rule settings for the specified rule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_rule_group)
         """
+
     async def update_subnet_change_protection(
         self,
         *,
         SubnetChangeProtection: bool,
         UpdateToken: str = ...,
         FirewallArn: str = ...,
         FirewallName: str = ...
@@ -558,70 +600,78 @@
         See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/network-
         firewall-2020-11-12/UpdateSubnetChangeProtection).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_subnet_change_protection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_subnet_change_protection)
         """
+
     async def update_tls_inspection_configuration(
         self,
         *,
-        TLSInspectionConfiguration: TLSInspectionConfigurationTypeDef,
+        TLSInspectionConfiguration: TLSInspectionConfigurationUnionTypeDef,
         UpdateToken: str,
         TLSInspectionConfigurationArn: str = ...,
         TLSInspectionConfigurationName: str = ...,
         Description: str = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> UpdateTLSInspectionConfigurationResponseTypeDef:
         """
         Updates the TLS inspection configuration settings for the specified TLS
         inspection configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_tls_inspection_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_tls_inspection_configuration)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_firewall_policies"]
     ) -> ListFirewallPoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_firewalls"]) -> ListFirewallsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_rule_groups"]) -> ListRuleGroupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_tls_inspection_configurations"]
     ) -> ListTLSInspectionConfigurationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_tags_for_resource"]
     ) -> ListTagsForResourcePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#get_paginator)
         """
+
     async def __aenter__(self) -> "NetworkFirewallClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/)
         """
```

### Comparing `types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall/literals.py` & `types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall/literals.pyi` & `types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall/paginator.py` & `types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,30 +65,30 @@
 class ListFirewallPoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListFirewallPolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/paginators/#listfirewallpoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFirewallPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListFirewallPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/paginators/#listfirewallpoliciespaginator)
         """
 
 
 class ListFirewallsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListFirewalls)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/paginators/#listfirewallspaginator)
     """
 
     def paginate(
-        self, *, VpcIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, VpcIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFirewallsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListFirewalls.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/paginators/#listfirewallspaginator)
         """
 
 
@@ -100,43 +100,43 @@
 
     def paginate(
         self,
         *,
         Scope: ResourceManagedStatusType = ...,
         ManagedType: ResourceManagedTypeType = ...,
         Type: RuleGroupTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRuleGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListRuleGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/paginators/#listrulegroupspaginator)
         """
 
 
 class ListTLSInspectionConfigurationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListTLSInspectionConfigurations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/paginators/#listtlsinspectionconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTLSInspectionConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListTLSInspectionConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/paginators/#listtlsinspectionconfigurationspaginator)
         """
 
 
 class ListTagsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListTagsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListTagsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall/paginator.pyi` & `types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -62,29 +62,29 @@
 class ListFirewallPoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListFirewallPolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/paginators/#listfirewallpoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFirewallPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListFirewallPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/paginators/#listfirewallpoliciespaginator)
         """
 
 class ListFirewallsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListFirewalls)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/paginators/#listfirewallspaginator)
     """
 
     def paginate(
-        self, *, VpcIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, VpcIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFirewallsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListFirewalls.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/paginators/#listfirewallspaginator)
         """
 
 class ListRuleGroupsPaginator(AioPaginator):
@@ -95,41 +95,41 @@
 
     def paginate(
         self,
         *,
         Scope: ResourceManagedStatusType = ...,
         ManagedType: ResourceManagedTypeType = ...,
         Type: RuleGroupTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRuleGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListRuleGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/paginators/#listrulegroupspaginator)
         """
 
 class ListTLSInspectionConfigurationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListTLSInspectionConfigurations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/paginators/#listtlsinspectionconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTLSInspectionConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListTLSInspectionConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/paginators/#listtlsinspectionconfigurationspaginator)
         """
 
 class ListTagsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListTagsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListTagsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall/type_defs.py` & `types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_network_firewall.type_defs import AddressTypeDef
 
-    data: AddressTypeDef = {...}
+    data: AddressTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AttachmentStatusType,
     ConfigurationSyncStateType,
     EncryptionTypeType,
     FirewallStatusValueType,
     GeneratedRulesTypeType,
@@ -47,15 +47,15 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AddressTypeDef",
     "AssociateFirewallPolicyRequestRequestTypeDef",
-    "AssociateFirewallPolicyResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "SubnetMappingTypeDef",
     "AttachmentTypeDef",
     "IPSetMetadataTypeDef",
     "EncryptionConfigurationTypeDef",
     "TagTypeDef",
     "SourceMetadataTypeDef",
     "DeleteFirewallPolicyRequestRequestTypeDef",
@@ -63,125 +63,153 @@
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteRuleGroupRequestRequestTypeDef",
     "DeleteTLSInspectionConfigurationRequestRequestTypeDef",
     "DescribeFirewallPolicyRequestRequestTypeDef",
     "DescribeFirewallRequestRequestTypeDef",
     "DescribeLoggingConfigurationRequestRequestTypeDef",
     "DescribeResourcePolicyRequestRequestTypeDef",
-    "DescribeResourcePolicyResponseTypeDef",
     "DescribeRuleGroupMetadataRequestRequestTypeDef",
     "StatefulRuleOptionsTypeDef",
     "DescribeRuleGroupRequestRequestTypeDef",
     "DescribeTLSInspectionConfigurationRequestRequestTypeDef",
     "DimensionTypeDef",
     "DisassociateSubnetsRequestRequestTypeDef",
     "FirewallMetadataTypeDef",
     "FirewallPolicyMetadataTypeDef",
     "StatefulEngineOptionsTypeDef",
     "StatelessRuleGroupReferenceTypeDef",
     "HeaderTypeDef",
+    "IPSetOutputTypeDef",
     "IPSetReferenceTypeDef",
     "IPSetTypeDef",
-    "ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListFirewallPoliciesRequestRequestTypeDef",
-    "ListFirewallsRequestListFirewallsPaginateTypeDef",
     "ListFirewallsRequestRequestTypeDef",
-    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
     "ListRuleGroupsRequestRequestTypeDef",
     "RuleGroupMetadataTypeDef",
-    "ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef",
     "ListTLSInspectionConfigurationsRequestRequestTypeDef",
     "TLSInspectionConfigurationMetadataTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "LogDestinationConfigOutputTypeDef",
     "LogDestinationConfigTypeDef",
     "PortRangeTypeDef",
+    "TCPFlagFieldOutputTypeDef",
     "TCPFlagFieldTypeDef",
-    "PaginatorConfigTypeDef",
     "PerObjectStatusTypeDef",
+    "PortSetOutputTypeDef",
     "PortSetTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "RuleOptionOutputTypeDef",
     "RuleOptionTypeDef",
+    "RulesSourceListOutputTypeDef",
     "RulesSourceListTypeDef",
     "ServerCertificateTypeDef",
     "StatefulRuleGroupOverrideTypeDef",
     "TlsCertificateDataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFirewallDeleteProtectionRequestRequestTypeDef",
-    "UpdateFirewallDeleteProtectionResponseTypeDef",
     "UpdateFirewallDescriptionRequestRequestTypeDef",
-    "UpdateFirewallDescriptionResponseTypeDef",
     "UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef",
-    "UpdateFirewallPolicyChangeProtectionResponseTypeDef",
     "UpdateSubnetChangeProtectionRequestRequestTypeDef",
+    "AssociateFirewallPolicyResponseTypeDef",
+    "DescribeResourcePolicyResponseTypeDef",
+    "UpdateFirewallDeleteProtectionResponseTypeDef",
+    "UpdateFirewallDescriptionResponseTypeDef",
+    "UpdateFirewallPolicyChangeProtectionResponseTypeDef",
     "UpdateSubnetChangeProtectionResponseTypeDef",
     "AssociateSubnetsRequestRequestTypeDef",
     "AssociateSubnetsResponseTypeDef",
     "DisassociateSubnetsResponseTypeDef",
     "CIDRSummaryTypeDef",
     "UpdateFirewallEncryptionConfigurationRequestRequestTypeDef",
     "UpdateFirewallEncryptionConfigurationResponseTypeDef",
     "CreateFirewallRequestRequestTypeDef",
     "FirewallPolicyResponseTypeDef",
     "FirewallTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "RuleGroupResponseTypeDef",
     "DescribeRuleGroupMetadataResponseTypeDef",
+    "PublishMetricActionOutputTypeDef",
     "PublishMetricActionTypeDef",
     "ListFirewallsResponseTypeDef",
     "ListFirewallPoliciesResponseTypeDef",
+    "PolicyVariablesOutputTypeDef",
+    "ReferenceSetsOutputTypeDef",
     "ReferenceSetsTypeDef",
     "PolicyVariablesTypeDef",
+    "ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef",
+    "ListFirewallsRequestListFirewallsPaginateTypeDef",
+    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
+    "ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListRuleGroupsResponseTypeDef",
     "ListTLSInspectionConfigurationsResponseTypeDef",
+    "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
+    "ServerCertificateScopeOutputTypeDef",
     "ServerCertificateScopeTypeDef",
+    "MatchAttributesOutputTypeDef",
     "MatchAttributesTypeDef",
     "SyncStateTypeDef",
+    "RuleVariablesOutputTypeDef",
     "RuleVariablesTypeDef",
+    "StatefulRuleOutputTypeDef",
     "StatefulRuleTypeDef",
     "StatefulRuleGroupReferenceTypeDef",
     "TLSInspectionConfigurationResponseTypeDef",
     "CapacityUsageSummaryTypeDef",
     "CreateFirewallPolicyResponseTypeDef",
     "DeleteFirewallPolicyResponseTypeDef",
     "UpdateFirewallPolicyResponseTypeDef",
     "CreateRuleGroupResponseTypeDef",
     "DeleteRuleGroupResponseTypeDef",
     "UpdateRuleGroupResponseTypeDef",
+    "ActionDefinitionOutputTypeDef",
     "ActionDefinitionTypeDef",
     "DescribeLoggingConfigurationResponseTypeDef",
-    "UpdateLoggingConfigurationRequestRequestTypeDef",
     "UpdateLoggingConfigurationResponseTypeDef",
+    "LoggingConfigurationUnionTypeDef",
+    "UpdateLoggingConfigurationRequestRequestTypeDef",
+    "ServerCertificateConfigurationOutputTypeDef",
     "ServerCertificateConfigurationTypeDef",
+    "RuleDefinitionOutputTypeDef",
     "RuleDefinitionTypeDef",
     "CreateTLSInspectionConfigurationResponseTypeDef",
     "DeleteTLSInspectionConfigurationResponseTypeDef",
     "UpdateTLSInspectionConfigurationResponseTypeDef",
     "FirewallStatusTypeDef",
+    "CustomActionOutputTypeDef",
     "CustomActionTypeDef",
+    "TLSInspectionConfigurationOutputTypeDef",
     "TLSInspectionConfigurationTypeDef",
+    "StatelessRuleOutputTypeDef",
     "StatelessRuleTypeDef",
     "CreateFirewallResponseTypeDef",
     "DeleteFirewallResponseTypeDef",
     "DescribeFirewallResponseTypeDef",
+    "FirewallPolicyOutputTypeDef",
     "FirewallPolicyTypeDef",
-    "CreateTLSInspectionConfigurationRequestRequestTypeDef",
     "DescribeTLSInspectionConfigurationResponseTypeDef",
+    "CreateTLSInspectionConfigurationRequestRequestTypeDef",
+    "TLSInspectionConfigurationUnionTypeDef",
     "UpdateTLSInspectionConfigurationRequestRequestTypeDef",
+    "StatelessRulesAndCustomActionsOutputTypeDef",
     "StatelessRulesAndCustomActionsTypeDef",
-    "CreateFirewallPolicyRequestRequestTypeDef",
     "DescribeFirewallPolicyResponseTypeDef",
+    "CreateFirewallPolicyRequestRequestTypeDef",
+    "FirewallPolicyUnionTypeDef",
     "UpdateFirewallPolicyRequestRequestTypeDef",
+    "RulesSourceOutputTypeDef",
     "RulesSourceTypeDef",
+    "RuleGroupOutputTypeDef",
     "RuleGroupTypeDef",
-    "CreateRuleGroupRequestRequestTypeDef",
     "DescribeRuleGroupResponseTypeDef",
+    "CreateRuleGroupRequestRequestTypeDef",
+    "RuleGroupUnionTypeDef",
     "UpdateRuleGroupRequestRequestTypeDef",
 )
 
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
         "AddressDefinition": str,
@@ -208,22 +236,22 @@
 class AssociateFirewallPolicyRequestRequestTypeDef(
     _RequiredAssociateFirewallPolicyRequestRequestTypeDef,
     _OptionalAssociateFirewallPolicyRequestRequestTypeDef,
 ):
     pass
 
 
-AssociateFirewallPolicyResponseTypeDef = TypedDict(
-    "AssociateFirewallPolicyResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "FirewallArn": str,
-        "FirewallName": str,
-        "FirewallPolicyArn": str,
-        "UpdateToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredSubnetMappingTypeDef = TypedDict(
     "_RequiredSubnetMappingTypeDef",
     {
         "SubnetId": str,
@@ -373,22 +401,14 @@
 DescribeResourcePolicyRequestRequestTypeDef = TypedDict(
     "DescribeResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-DescribeResourcePolicyResponseTypeDef = TypedDict(
-    "DescribeResourcePolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeRuleGroupMetadataRequestRequestTypeDef = TypedDict(
     "DescribeRuleGroupMetadataRequestRequestTypeDef",
     {
         "RuleGroupName": str,
         "RuleGroupArn": str,
         "Type": RuleGroupTypeType,
     },
@@ -496,14 +516,21 @@
         "SourcePort": str,
         "Direction": StatefulRuleDirectionType,
         "Destination": str,
         "DestinationPort": str,
     },
 )
 
+IPSetOutputTypeDef = TypedDict(
+    "IPSetOutputTypeDef",
+    {
+        "Definition": List[str],
+    },
+)
+
 IPSetReferenceTypeDef = TypedDict(
     "IPSetReferenceTypeDef",
     {
         "ReferenceArn": str,
     },
     total=False,
 )
@@ -511,61 +538,43 @@
 IPSetTypeDef = TypedDict(
     "IPSetTypeDef",
     {
         "Definition": Sequence[str],
     },
 )
 
-ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef = TypedDict(
-    "ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef",
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
 
 ListFirewallPoliciesRequestRequestTypeDef = TypedDict(
     "ListFirewallPoliciesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListFirewallsRequestListFirewallsPaginateTypeDef = TypedDict(
-    "ListFirewallsRequestListFirewallsPaginateTypeDef",
-    {
-        "VpcIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFirewallsRequestRequestTypeDef = TypedDict(
     "ListFirewallsRequestRequestTypeDef",
     {
         "NextToken": str,
         "VpcIds": Sequence[str],
         "MaxResults": int,
     },
     total=False,
 )
 
-ListRuleGroupsRequestListRuleGroupsPaginateTypeDef = TypedDict(
-    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
-    {
-        "Scope": ResourceManagedStatusType,
-        "ManagedType": ResourceManagedTypeType,
-        "Type": RuleGroupTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRuleGroupsRequestRequestTypeDef = TypedDict(
     "ListRuleGroupsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Scope": ResourceManagedStatusType,
         "ManagedType": ResourceManagedTypeType,
@@ -579,22 +588,14 @@
     {
         "Name": str,
         "Arn": str,
     },
     total=False,
 )
 
-ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef = TypedDict(
-    "ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTLSInspectionConfigurationsRequestRequestTypeDef = TypedDict(
     "ListTLSInspectionConfigurationsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -605,36 +606,14 @@
     {
         "Name": str,
         "Arn": str,
     },
     total=False,
 )
 
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
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
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -650,31 +629,61 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
+LogDestinationConfigOutputTypeDef = TypedDict(
+    "LogDestinationConfigOutputTypeDef",
+    {
+        "LogType": LogTypeType,
+        "LogDestinationType": LogDestinationTypeType,
+        "LogDestination": Dict[str, str],
+    },
+)
+
 LogDestinationConfigTypeDef = TypedDict(
     "LogDestinationConfigTypeDef",
     {
         "LogType": LogTypeType,
         "LogDestinationType": LogDestinationTypeType,
-        "LogDestination": Dict[str, str],
+        "LogDestination": Mapping[str, str],
     },
 )
 
 PortRangeTypeDef = TypedDict(
     "PortRangeTypeDef",
     {
         "FromPort": int,
         "ToPort": int,
     },
 )
 
+_RequiredTCPFlagFieldOutputTypeDef = TypedDict(
+    "_RequiredTCPFlagFieldOutputTypeDef",
+    {
+        "Flags": List[TCPFlagType],
+    },
+)
+_OptionalTCPFlagFieldOutputTypeDef = TypedDict(
+    "_OptionalTCPFlagFieldOutputTypeDef",
+    {
+        "Masks": List[TCPFlagType],
+    },
+    total=False,
+)
+
+
+class TCPFlagFieldOutputTypeDef(
+    _RequiredTCPFlagFieldOutputTypeDef, _OptionalTCPFlagFieldOutputTypeDef
+):
+    pass
+
+
 _RequiredTCPFlagFieldTypeDef = TypedDict(
     "_RequiredTCPFlagFieldTypeDef",
     {
         "Flags": Sequence[TCPFlagType],
     },
 )
 _OptionalTCPFlagFieldTypeDef = TypedDict(
@@ -686,29 +695,27 @@
 )
 
 
 class TCPFlagFieldTypeDef(_RequiredTCPFlagFieldTypeDef, _OptionalTCPFlagFieldTypeDef):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+PerObjectStatusTypeDef = TypedDict(
+    "PerObjectStatusTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "SyncStatus": PerObjectSyncStatusType,
+        "UpdateToken": str,
     },
     total=False,
 )
 
-PerObjectStatusTypeDef = TypedDict(
-    "PerObjectStatusTypeDef",
+PortSetOutputTypeDef = TypedDict(
+    "PortSetOutputTypeDef",
     {
-        "SyncStatus": PerObjectSyncStatusType,
-        "UpdateToken": str,
+        "Definition": List[str],
     },
     total=False,
 )
 
 PortSetTypeDef = TypedDict(
     "PortSetTypeDef",
     {
@@ -721,25 +728,33 @@
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Policy": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_RequiredRuleOptionOutputTypeDef = TypedDict(
+    "_RequiredRuleOptionOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Keyword": str,
+    },
+)
+_OptionalRuleOptionOutputTypeDef = TypedDict(
+    "_OptionalRuleOptionOutputTypeDef",
+    {
+        "Settings": List[str],
     },
+    total=False,
 )
 
+
+class RuleOptionOutputTypeDef(_RequiredRuleOptionOutputTypeDef, _OptionalRuleOptionOutputTypeDef):
+    pass
+
+
 _RequiredRuleOptionTypeDef = TypedDict(
     "_RequiredRuleOptionTypeDef",
     {
         "Keyword": str,
     },
 )
 _OptionalRuleOptionTypeDef = TypedDict(
@@ -751,14 +766,23 @@
 )
 
 
 class RuleOptionTypeDef(_RequiredRuleOptionTypeDef, _OptionalRuleOptionTypeDef):
     pass
 
 
+RulesSourceListOutputTypeDef = TypedDict(
+    "RulesSourceListOutputTypeDef",
+    {
+        "Targets": List[str],
+        "TargetTypes": List[TargetTypeType],
+        "GeneratedRulesType": GeneratedRulesTypeType,
+    },
+)
+
 RulesSourceListTypeDef = TypedDict(
     "RulesSourceListTypeDef",
     {
         "Targets": Sequence[str],
         "TargetTypes": Sequence[TargetTypeType],
         "GeneratedRulesType": GeneratedRulesTypeType,
     },
@@ -819,47 +843,25 @@
 class UpdateFirewallDeleteProtectionRequestRequestTypeDef(
     _RequiredUpdateFirewallDeleteProtectionRequestRequestTypeDef,
     _OptionalUpdateFirewallDeleteProtectionRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateFirewallDeleteProtectionResponseTypeDef = TypedDict(
-    "UpdateFirewallDeleteProtectionResponseTypeDef",
-    {
-        "FirewallArn": str,
-        "FirewallName": str,
-        "DeleteProtection": bool,
-        "UpdateToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateFirewallDescriptionRequestRequestTypeDef = TypedDict(
     "UpdateFirewallDescriptionRequestRequestTypeDef",
     {
         "UpdateToken": str,
         "FirewallArn": str,
         "FirewallName": str,
         "Description": str,
     },
     total=False,
 )
 
-UpdateFirewallDescriptionResponseTypeDef = TypedDict(
-    "UpdateFirewallDescriptionResponseTypeDef",
-    {
-        "FirewallArn": str,
-        "FirewallName": str,
-        "Description": str,
-        "UpdateToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef",
     {
         "FirewallPolicyChangeProtection": bool,
     },
 )
 _OptionalUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef = TypedDict(
@@ -876,25 +878,14 @@
 class UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef(
     _RequiredUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef,
     _OptionalUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateFirewallPolicyChangeProtectionResponseTypeDef = TypedDict(
-    "UpdateFirewallPolicyChangeProtectionResponseTypeDef",
-    {
-        "UpdateToken": str,
-        "FirewallArn": str,
-        "FirewallName": str,
-        "FirewallPolicyChangeProtection": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateSubnetChangeProtectionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSubnetChangeProtectionRequestRequestTypeDef",
     {
         "SubnetChangeProtection": bool,
     },
 )
 _OptionalUpdateSubnetChangeProtectionRequestRequestTypeDef = TypedDict(
@@ -911,22 +902,74 @@
 class UpdateSubnetChangeProtectionRequestRequestTypeDef(
     _RequiredUpdateSubnetChangeProtectionRequestRequestTypeDef,
     _OptionalUpdateSubnetChangeProtectionRequestRequestTypeDef,
 ):
     pass
 
 
+AssociateFirewallPolicyResponseTypeDef = TypedDict(
+    "AssociateFirewallPolicyResponseTypeDef",
+    {
+        "FirewallArn": str,
+        "FirewallName": str,
+        "FirewallPolicyArn": str,
+        "UpdateToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeResourcePolicyResponseTypeDef = TypedDict(
+    "DescribeResourcePolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFirewallDeleteProtectionResponseTypeDef = TypedDict(
+    "UpdateFirewallDeleteProtectionResponseTypeDef",
+    {
+        "FirewallArn": str,
+        "FirewallName": str,
+        "DeleteProtection": bool,
+        "UpdateToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFirewallDescriptionResponseTypeDef = TypedDict(
+    "UpdateFirewallDescriptionResponseTypeDef",
+    {
+        "FirewallArn": str,
+        "FirewallName": str,
+        "Description": str,
+        "UpdateToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFirewallPolicyChangeProtectionResponseTypeDef = TypedDict(
+    "UpdateFirewallPolicyChangeProtectionResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "FirewallArn": str,
+        "FirewallName": str,
+        "FirewallPolicyChangeProtection": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateSubnetChangeProtectionResponseTypeDef = TypedDict(
     "UpdateSubnetChangeProtectionResponseTypeDef",
     {
         "UpdateToken": str,
         "FirewallArn": str,
         "FirewallName": str,
         "SubnetChangeProtection": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAssociateSubnetsRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateSubnetsRequestRequestTypeDef",
     {
         "SubnetMappings": Sequence[SubnetMappingTypeDef],
@@ -952,26 +995,26 @@
 AssociateSubnetsResponseTypeDef = TypedDict(
     "AssociateSubnetsResponseTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
         "SubnetMappings": List[SubnetMappingTypeDef],
         "UpdateToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateSubnetsResponseTypeDef = TypedDict(
     "DisassociateSubnetsResponseTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
         "SubnetMappings": List[SubnetMappingTypeDef],
         "UpdateToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CIDRSummaryTypeDef = TypedDict(
     "CIDRSummaryTypeDef",
     {
         "AvailableCIDRCount": int,
@@ -995,15 +1038,15 @@
 UpdateFirewallEncryptionConfigurationResponseTypeDef = TypedDict(
     "UpdateFirewallEncryptionConfigurationResponseTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
         "UpdateToken": str,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateFirewallRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFirewallRequestRequestTypeDef",
     {
         "FirewallName": str,
@@ -1092,15 +1135,15 @@
 
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "NextToken": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -1147,15 +1190,22 @@
         "RuleGroupArn": str,
         "RuleGroupName": str,
         "Description": str,
         "Type": RuleGroupTypeType,
         "Capacity": int,
         "StatefulRuleOptions": StatefulRuleOptionsTypeDef,
         "LastModifiedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PublishMetricActionOutputTypeDef = TypedDict(
+    "PublishMetricActionOutputTypeDef",
+    {
+        "Dimensions": List[DimensionTypeDef],
     },
 )
 
 PublishMetricActionTypeDef = TypedDict(
     "PublishMetricActionTypeDef",
     {
         "Dimensions": Sequence[DimensionTypeDef],
@@ -1163,25 +1213,41 @@
 )
 
 ListFirewallsResponseTypeDef = TypedDict(
     "ListFirewallsResponseTypeDef",
     {
         "NextToken": str,
         "Firewalls": List[FirewallMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFirewallPoliciesResponseTypeDef = TypedDict(
     "ListFirewallPoliciesResponseTypeDef",
     {
         "NextToken": str,
         "FirewallPolicies": List[FirewallPolicyMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PolicyVariablesOutputTypeDef = TypedDict(
+    "PolicyVariablesOutputTypeDef",
+    {
+        "RuleVariables": Dict[str, IPSetOutputTypeDef],
+    },
+    total=False,
+)
+
+ReferenceSetsOutputTypeDef = TypedDict(
+    "ReferenceSetsOutputTypeDef",
+    {
+        "IPSetReferences": Dict[str, IPSetReferenceTypeDef],
     },
+    total=False,
 )
 
 ReferenceSetsTypeDef = TypedDict(
     "ReferenceSetsTypeDef",
     {
         "IPSetReferences": Mapping[str, IPSetReferenceTypeDef],
     },
@@ -1192,51 +1258,141 @@
     "PolicyVariablesTypeDef",
     {
         "RuleVariables": Mapping[str, IPSetTypeDef],
     },
     total=False,
 )
 
+ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef = TypedDict(
+    "ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListFirewallsRequestListFirewallsPaginateTypeDef = TypedDict(
+    "ListFirewallsRequestListFirewallsPaginateTypeDef",
+    {
+        "VpcIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRuleGroupsRequestListRuleGroupsPaginateTypeDef = TypedDict(
+    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
+    {
+        "Scope": ResourceManagedStatusType,
+        "ManagedType": ResourceManagedTypeType,
+        "Type": RuleGroupTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef = TypedDict(
+    "ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
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
 ListRuleGroupsResponseTypeDef = TypedDict(
     "ListRuleGroupsResponseTypeDef",
     {
         "NextToken": str,
         "RuleGroups": List[RuleGroupMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTLSInspectionConfigurationsResponseTypeDef = TypedDict(
     "ListTLSInspectionConfigurationsResponseTypeDef",
     {
         "NextToken": str,
         "TLSInspectionConfigurations": List[TLSInspectionConfigurationMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LoggingConfigurationOutputTypeDef = TypedDict(
+    "LoggingConfigurationOutputTypeDef",
+    {
+        "LogDestinationConfigs": List[LogDestinationConfigOutputTypeDef],
     },
 )
 
 LoggingConfigurationTypeDef = TypedDict(
     "LoggingConfigurationTypeDef",
     {
-        "LogDestinationConfigs": List[LogDestinationConfigTypeDef],
+        "LogDestinationConfigs": Sequence[LogDestinationConfigTypeDef],
+    },
+)
+
+ServerCertificateScopeOutputTypeDef = TypedDict(
+    "ServerCertificateScopeOutputTypeDef",
+    {
+        "Sources": List[AddressTypeDef],
+        "Destinations": List[AddressTypeDef],
+        "SourcePorts": List[PortRangeTypeDef],
+        "DestinationPorts": List[PortRangeTypeDef],
+        "Protocols": List[int],
     },
+    total=False,
 )
 
 ServerCertificateScopeTypeDef = TypedDict(
     "ServerCertificateScopeTypeDef",
     {
         "Sources": Sequence[AddressTypeDef],
         "Destinations": Sequence[AddressTypeDef],
         "SourcePorts": Sequence[PortRangeTypeDef],
         "DestinationPorts": Sequence[PortRangeTypeDef],
         "Protocols": Sequence[int],
     },
     total=False,
 )
 
+MatchAttributesOutputTypeDef = TypedDict(
+    "MatchAttributesOutputTypeDef",
+    {
+        "Sources": List[AddressTypeDef],
+        "Destinations": List[AddressTypeDef],
+        "SourcePorts": List[PortRangeTypeDef],
+        "DestinationPorts": List[PortRangeTypeDef],
+        "Protocols": List[int],
+        "TCPFlags": List[TCPFlagFieldOutputTypeDef],
+    },
+    total=False,
+)
+
 MatchAttributesTypeDef = TypedDict(
     "MatchAttributesTypeDef",
     {
         "Sources": Sequence[AddressTypeDef],
         "Destinations": Sequence[AddressTypeDef],
         "SourcePorts": Sequence[PortRangeTypeDef],
         "DestinationPorts": Sequence[PortRangeTypeDef],
@@ -1251,23 +1407,41 @@
     {
         "Attachment": AttachmentTypeDef,
         "Config": Dict[str, PerObjectStatusTypeDef],
     },
     total=False,
 )
 
+RuleVariablesOutputTypeDef = TypedDict(
+    "RuleVariablesOutputTypeDef",
+    {
+        "IPSets": Dict[str, IPSetOutputTypeDef],
+        "PortSets": Dict[str, PortSetOutputTypeDef],
+    },
+    total=False,
+)
+
 RuleVariablesTypeDef = TypedDict(
     "RuleVariablesTypeDef",
     {
         "IPSets": Mapping[str, IPSetTypeDef],
         "PortSets": Mapping[str, PortSetTypeDef],
     },
     total=False,
 )
 
+StatefulRuleOutputTypeDef = TypedDict(
+    "StatefulRuleOutputTypeDef",
+    {
+        "Action": StatefulActionType,
+        "Header": HeaderTypeDef,
+        "RuleOptions": List[RuleOptionOutputTypeDef],
+    },
+)
+
 StatefulRuleTypeDef = TypedDict(
     "StatefulRuleTypeDef",
     {
         "Action": StatefulActionType,
         "Header": HeaderTypeDef,
         "RuleOptions": Sequence[RuleOptionTypeDef],
     },
@@ -1334,138 +1508,166 @@
 )
 
 CreateFirewallPolicyResponseTypeDef = TypedDict(
     "CreateFirewallPolicyResponseTypeDef",
     {
         "UpdateToken": str,
         "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteFirewallPolicyResponseTypeDef = TypedDict(
     "DeleteFirewallPolicyResponseTypeDef",
     {
         "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFirewallPolicyResponseTypeDef = TypedDict(
     "UpdateFirewallPolicyResponseTypeDef",
     {
         "UpdateToken": str,
         "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRuleGroupResponseTypeDef = TypedDict(
     "CreateRuleGroupResponseTypeDef",
     {
         "UpdateToken": str,
         "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRuleGroupResponseTypeDef = TypedDict(
     "DeleteRuleGroupResponseTypeDef",
     {
         "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRuleGroupResponseTypeDef = TypedDict(
     "UpdateRuleGroupResponseTypeDef",
     {
         "UpdateToken": str,
         "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ActionDefinitionOutputTypeDef = TypedDict(
+    "ActionDefinitionOutputTypeDef",
+    {
+        "PublishMetricAction": PublishMetricActionOutputTypeDef,
+    },
+    total=False,
+)
+
 ActionDefinitionTypeDef = TypedDict(
     "ActionDefinitionTypeDef",
     {
         "PublishMetricAction": PublishMetricActionTypeDef,
     },
     total=False,
 )
 
 DescribeLoggingConfigurationResponseTypeDef = TypedDict(
     "DescribeLoggingConfigurationResponseTypeDef",
     {
         "FirewallArn": str,
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateLoggingConfigurationResponseTypeDef = TypedDict(
+    "UpdateLoggingConfigurationResponseTypeDef",
+    {
+        "FirewallArn": str,
+        "FirewallName": str,
+        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LoggingConfigurationUnionTypeDef = Union[
+    LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
+]
 UpdateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateLoggingConfigurationRequestRequestTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
     },
     total=False,
 )
 
-UpdateLoggingConfigurationResponseTypeDef = TypedDict(
-    "UpdateLoggingConfigurationResponseTypeDef",
+ServerCertificateConfigurationOutputTypeDef = TypedDict(
+    "ServerCertificateConfigurationOutputTypeDef",
     {
-        "FirewallArn": str,
-        "FirewallName": str,
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ServerCertificates": List[ServerCertificateTypeDef],
+        "Scopes": List[ServerCertificateScopeOutputTypeDef],
     },
+    total=False,
 )
 
 ServerCertificateConfigurationTypeDef = TypedDict(
     "ServerCertificateConfigurationTypeDef",
     {
         "ServerCertificates": Sequence[ServerCertificateTypeDef],
         "Scopes": Sequence[ServerCertificateScopeTypeDef],
     },
     total=False,
 )
 
+RuleDefinitionOutputTypeDef = TypedDict(
+    "RuleDefinitionOutputTypeDef",
+    {
+        "MatchAttributes": MatchAttributesOutputTypeDef,
+        "Actions": List[str],
+    },
+)
+
 RuleDefinitionTypeDef = TypedDict(
     "RuleDefinitionTypeDef",
     {
         "MatchAttributes": MatchAttributesTypeDef,
         "Actions": Sequence[str],
     },
 )
 
 CreateTLSInspectionConfigurationResponseTypeDef = TypedDict(
     "CreateTLSInspectionConfigurationResponseTypeDef",
     {
         "UpdateToken": str,
         "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteTLSInspectionConfigurationResponseTypeDef = TypedDict(
     "DeleteTLSInspectionConfigurationResponseTypeDef",
     {
         "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTLSInspectionConfigurationResponseTypeDef = TypedDict(
     "UpdateTLSInspectionConfigurationResponseTypeDef",
     {
         "UpdateToken": str,
         "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFirewallStatusTypeDef = TypedDict(
     "_RequiredFirewallStatusTypeDef",
     {
         "Status": FirewallStatusValueType,
@@ -1482,65 +1684,117 @@
 )
 
 
 class FirewallStatusTypeDef(_RequiredFirewallStatusTypeDef, _OptionalFirewallStatusTypeDef):
     pass
 
 
+CustomActionOutputTypeDef = TypedDict(
+    "CustomActionOutputTypeDef",
+    {
+        "ActionName": str,
+        "ActionDefinition": ActionDefinitionOutputTypeDef,
+    },
+)
+
 CustomActionTypeDef = TypedDict(
     "CustomActionTypeDef",
     {
         "ActionName": str,
         "ActionDefinition": ActionDefinitionTypeDef,
     },
 )
 
+TLSInspectionConfigurationOutputTypeDef = TypedDict(
+    "TLSInspectionConfigurationOutputTypeDef",
+    {
+        "ServerCertificateConfigurations": List[ServerCertificateConfigurationOutputTypeDef],
+    },
+    total=False,
+)
+
 TLSInspectionConfigurationTypeDef = TypedDict(
     "TLSInspectionConfigurationTypeDef",
     {
         "ServerCertificateConfigurations": Sequence[ServerCertificateConfigurationTypeDef],
     },
     total=False,
 )
 
+StatelessRuleOutputTypeDef = TypedDict(
+    "StatelessRuleOutputTypeDef",
+    {
+        "RuleDefinition": RuleDefinitionOutputTypeDef,
+        "Priority": int,
+    },
+)
+
 StatelessRuleTypeDef = TypedDict(
     "StatelessRuleTypeDef",
     {
         "RuleDefinition": RuleDefinitionTypeDef,
         "Priority": int,
     },
 )
 
 CreateFirewallResponseTypeDef = TypedDict(
     "CreateFirewallResponseTypeDef",
     {
         "Firewall": FirewallTypeDef,
         "FirewallStatus": FirewallStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteFirewallResponseTypeDef = TypedDict(
     "DeleteFirewallResponseTypeDef",
     {
         "Firewall": FirewallTypeDef,
         "FirewallStatus": FirewallStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFirewallResponseTypeDef = TypedDict(
     "DescribeFirewallResponseTypeDef",
     {
         "UpdateToken": str,
         "Firewall": FirewallTypeDef,
         "FirewallStatus": FirewallStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredFirewallPolicyOutputTypeDef = TypedDict(
+    "_RequiredFirewallPolicyOutputTypeDef",
+    {
+        "StatelessDefaultActions": List[str],
+        "StatelessFragmentDefaultActions": List[str],
     },
 )
+_OptionalFirewallPolicyOutputTypeDef = TypedDict(
+    "_OptionalFirewallPolicyOutputTypeDef",
+    {
+        "StatelessRuleGroupReferences": List[StatelessRuleGroupReferenceTypeDef],
+        "StatelessCustomActions": List[CustomActionOutputTypeDef],
+        "StatefulRuleGroupReferences": List[StatefulRuleGroupReferenceTypeDef],
+        "StatefulDefaultActions": List[str],
+        "StatefulEngineOptions": StatefulEngineOptionsTypeDef,
+        "TLSInspectionConfigurationArn": str,
+        "PolicyVariables": PolicyVariablesOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class FirewallPolicyOutputTypeDef(
+    _RequiredFirewallPolicyOutputTypeDef, _OptionalFirewallPolicyOutputTypeDef
+):
+    pass
+
 
 _RequiredFirewallPolicyTypeDef = TypedDict(
     "_RequiredFirewallPolicyTypeDef",
     {
         "StatelessDefaultActions": Sequence[str],
         "StatelessFragmentDefaultActions": Sequence[str],
     },
@@ -1560,14 +1814,24 @@
 )
 
 
 class FirewallPolicyTypeDef(_RequiredFirewallPolicyTypeDef, _OptionalFirewallPolicyTypeDef):
     pass
 
 
+DescribeTLSInspectionConfigurationResponseTypeDef = TypedDict(
+    "DescribeTLSInspectionConfigurationResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "TLSInspectionConfiguration": TLSInspectionConfigurationOutputTypeDef,
+        "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateTLSInspectionConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTLSInspectionConfigurationRequestRequestTypeDef",
     {
         "TLSInspectionConfigurationName": str,
         "TLSInspectionConfiguration": TLSInspectionConfigurationTypeDef,
     },
 )
@@ -1585,24 +1849,17 @@
 class CreateTLSInspectionConfigurationRequestRequestTypeDef(
     _RequiredCreateTLSInspectionConfigurationRequestRequestTypeDef,
     _OptionalCreateTLSInspectionConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeTLSInspectionConfigurationResponseTypeDef = TypedDict(
-    "DescribeTLSInspectionConfigurationResponseTypeDef",
-    {
-        "UpdateToken": str,
-        "TLSInspectionConfiguration": TLSInspectionConfigurationTypeDef,
-        "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+TLSInspectionConfigurationUnionTypeDef = Union[
+    TLSInspectionConfigurationTypeDef, TLSInspectionConfigurationOutputTypeDef
+]
 _RequiredUpdateTLSInspectionConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTLSInspectionConfigurationRequestRequestTypeDef",
     {
         "TLSInspectionConfiguration": TLSInspectionConfigurationTypeDef,
         "UpdateToken": str,
     },
 )
@@ -1621,14 +1878,36 @@
 class UpdateTLSInspectionConfigurationRequestRequestTypeDef(
     _RequiredUpdateTLSInspectionConfigurationRequestRequestTypeDef,
     _OptionalUpdateTLSInspectionConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredStatelessRulesAndCustomActionsOutputTypeDef = TypedDict(
+    "_RequiredStatelessRulesAndCustomActionsOutputTypeDef",
+    {
+        "StatelessRules": List[StatelessRuleOutputTypeDef],
+    },
+)
+_OptionalStatelessRulesAndCustomActionsOutputTypeDef = TypedDict(
+    "_OptionalStatelessRulesAndCustomActionsOutputTypeDef",
+    {
+        "CustomActions": List[CustomActionOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class StatelessRulesAndCustomActionsOutputTypeDef(
+    _RequiredStatelessRulesAndCustomActionsOutputTypeDef,
+    _OptionalStatelessRulesAndCustomActionsOutputTypeDef,
+):
+    pass
+
+
 _RequiredStatelessRulesAndCustomActionsTypeDef = TypedDict(
     "_RequiredStatelessRulesAndCustomActionsTypeDef",
     {
         "StatelessRules": Sequence[StatelessRuleTypeDef],
     },
 )
 _OptionalStatelessRulesAndCustomActionsTypeDef = TypedDict(
@@ -1642,14 +1921,24 @@
 
 class StatelessRulesAndCustomActionsTypeDef(
     _RequiredStatelessRulesAndCustomActionsTypeDef, _OptionalStatelessRulesAndCustomActionsTypeDef
 ):
     pass
 
 
+DescribeFirewallPolicyResponseTypeDef = TypedDict(
+    "DescribeFirewallPolicyResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
+        "FirewallPolicy": FirewallPolicyOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateFirewallPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFirewallPolicyRequestRequestTypeDef",
     {
         "FirewallPolicyName": str,
         "FirewallPolicy": FirewallPolicyTypeDef,
     },
 )
@@ -1668,24 +1957,15 @@
 class CreateFirewallPolicyRequestRequestTypeDef(
     _RequiredCreateFirewallPolicyRequestRequestTypeDef,
     _OptionalCreateFirewallPolicyRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeFirewallPolicyResponseTypeDef = TypedDict(
-    "DescribeFirewallPolicyResponseTypeDef",
-    {
-        "UpdateToken": str,
-        "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
-        "FirewallPolicy": FirewallPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+FirewallPolicyUnionTypeDef = Union[FirewallPolicyTypeDef, FirewallPolicyOutputTypeDef]
 _RequiredUpdateFirewallPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFirewallPolicyRequestRequestTypeDef",
     {
         "UpdateToken": str,
         "FirewallPolicy": FirewallPolicyTypeDef,
     },
 )
@@ -1705,25 +1985,57 @@
 class UpdateFirewallPolicyRequestRequestTypeDef(
     _RequiredUpdateFirewallPolicyRequestRequestTypeDef,
     _OptionalUpdateFirewallPolicyRequestRequestTypeDef,
 ):
     pass
 
 
+RulesSourceOutputTypeDef = TypedDict(
+    "RulesSourceOutputTypeDef",
+    {
+        "RulesString": str,
+        "RulesSourceList": RulesSourceListOutputTypeDef,
+        "StatefulRules": List[StatefulRuleOutputTypeDef],
+        "StatelessRulesAndCustomActions": StatelessRulesAndCustomActionsOutputTypeDef,
+    },
+    total=False,
+)
+
 RulesSourceTypeDef = TypedDict(
     "RulesSourceTypeDef",
     {
         "RulesString": str,
         "RulesSourceList": RulesSourceListTypeDef,
         "StatefulRules": Sequence[StatefulRuleTypeDef],
         "StatelessRulesAndCustomActions": StatelessRulesAndCustomActionsTypeDef,
     },
     total=False,
 )
 
+_RequiredRuleGroupOutputTypeDef = TypedDict(
+    "_RequiredRuleGroupOutputTypeDef",
+    {
+        "RulesSource": RulesSourceOutputTypeDef,
+    },
+)
+_OptionalRuleGroupOutputTypeDef = TypedDict(
+    "_OptionalRuleGroupOutputTypeDef",
+    {
+        "RuleVariables": RuleVariablesOutputTypeDef,
+        "ReferenceSets": ReferenceSetsOutputTypeDef,
+        "StatefulRuleOptions": StatefulRuleOptionsTypeDef,
+    },
+    total=False,
+)
+
+
+class RuleGroupOutputTypeDef(_RequiredRuleGroupOutputTypeDef, _OptionalRuleGroupOutputTypeDef):
+    pass
+
+
 _RequiredRuleGroupTypeDef = TypedDict(
     "_RequiredRuleGroupTypeDef",
     {
         "RulesSource": RulesSourceTypeDef,
     },
 )
 _OptionalRuleGroupTypeDef = TypedDict(
@@ -1737,14 +2049,24 @@
 )
 
 
 class RuleGroupTypeDef(_RequiredRuleGroupTypeDef, _OptionalRuleGroupTypeDef):
     pass
 
 
+DescribeRuleGroupResponseTypeDef = TypedDict(
+    "DescribeRuleGroupResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "RuleGroup": RuleGroupOutputTypeDef,
+        "RuleGroupResponse": RuleGroupResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRuleGroupRequestRequestTypeDef",
     {
         "RuleGroupName": str,
         "Type": RuleGroupTypeType,
         "Capacity": int,
     },
@@ -1766,24 +2088,15 @@
 
 class CreateRuleGroupRequestRequestTypeDef(
     _RequiredCreateRuleGroupRequestRequestTypeDef, _OptionalCreateRuleGroupRequestRequestTypeDef
 ):
     pass
 
 
-DescribeRuleGroupResponseTypeDef = TypedDict(
-    "DescribeRuleGroupResponseTypeDef",
-    {
-        "UpdateToken": str,
-        "RuleGroup": RuleGroupTypeDef,
-        "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+RuleGroupUnionTypeDef = Union[RuleGroupTypeDef, RuleGroupOutputTypeDef]
 _RequiredUpdateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRuleGroupRequestRequestTypeDef",
     {
         "UpdateToken": str,
     },
 )
 _OptionalUpdateRuleGroupRequestRequestTypeDef = TypedDict(
```

### Comparing `types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall/type_defs.pyi` & `types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_network_firewall.type_defs import AddressTypeDef
 
-    data: AddressTypeDef = {...}
+    data: AddressTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AttachmentStatusType,
     ConfigurationSyncStateType,
     EncryptionTypeType,
     FirewallStatusValueType,
     GeneratedRulesTypeType,
@@ -46,15 +46,15 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddressTypeDef",
     "AssociateFirewallPolicyRequestRequestTypeDef",
-    "AssociateFirewallPolicyResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "SubnetMappingTypeDef",
     "AttachmentTypeDef",
     "IPSetMetadataTypeDef",
     "EncryptionConfigurationTypeDef",
     "TagTypeDef",
     "SourceMetadataTypeDef",
     "DeleteFirewallPolicyRequestRequestTypeDef",
@@ -62,125 +62,153 @@
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteRuleGroupRequestRequestTypeDef",
     "DeleteTLSInspectionConfigurationRequestRequestTypeDef",
     "DescribeFirewallPolicyRequestRequestTypeDef",
     "DescribeFirewallRequestRequestTypeDef",
     "DescribeLoggingConfigurationRequestRequestTypeDef",
     "DescribeResourcePolicyRequestRequestTypeDef",
-    "DescribeResourcePolicyResponseTypeDef",
     "DescribeRuleGroupMetadataRequestRequestTypeDef",
     "StatefulRuleOptionsTypeDef",
     "DescribeRuleGroupRequestRequestTypeDef",
     "DescribeTLSInspectionConfigurationRequestRequestTypeDef",
     "DimensionTypeDef",
     "DisassociateSubnetsRequestRequestTypeDef",
     "FirewallMetadataTypeDef",
     "FirewallPolicyMetadataTypeDef",
     "StatefulEngineOptionsTypeDef",
     "StatelessRuleGroupReferenceTypeDef",
     "HeaderTypeDef",
+    "IPSetOutputTypeDef",
     "IPSetReferenceTypeDef",
     "IPSetTypeDef",
-    "ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListFirewallPoliciesRequestRequestTypeDef",
-    "ListFirewallsRequestListFirewallsPaginateTypeDef",
     "ListFirewallsRequestRequestTypeDef",
-    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
     "ListRuleGroupsRequestRequestTypeDef",
     "RuleGroupMetadataTypeDef",
-    "ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef",
     "ListTLSInspectionConfigurationsRequestRequestTypeDef",
     "TLSInspectionConfigurationMetadataTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "LogDestinationConfigOutputTypeDef",
     "LogDestinationConfigTypeDef",
     "PortRangeTypeDef",
+    "TCPFlagFieldOutputTypeDef",
     "TCPFlagFieldTypeDef",
-    "PaginatorConfigTypeDef",
     "PerObjectStatusTypeDef",
+    "PortSetOutputTypeDef",
     "PortSetTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "RuleOptionOutputTypeDef",
     "RuleOptionTypeDef",
+    "RulesSourceListOutputTypeDef",
     "RulesSourceListTypeDef",
     "ServerCertificateTypeDef",
     "StatefulRuleGroupOverrideTypeDef",
     "TlsCertificateDataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFirewallDeleteProtectionRequestRequestTypeDef",
-    "UpdateFirewallDeleteProtectionResponseTypeDef",
     "UpdateFirewallDescriptionRequestRequestTypeDef",
-    "UpdateFirewallDescriptionResponseTypeDef",
     "UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef",
-    "UpdateFirewallPolicyChangeProtectionResponseTypeDef",
     "UpdateSubnetChangeProtectionRequestRequestTypeDef",
+    "AssociateFirewallPolicyResponseTypeDef",
+    "DescribeResourcePolicyResponseTypeDef",
+    "UpdateFirewallDeleteProtectionResponseTypeDef",
+    "UpdateFirewallDescriptionResponseTypeDef",
+    "UpdateFirewallPolicyChangeProtectionResponseTypeDef",
     "UpdateSubnetChangeProtectionResponseTypeDef",
     "AssociateSubnetsRequestRequestTypeDef",
     "AssociateSubnetsResponseTypeDef",
     "DisassociateSubnetsResponseTypeDef",
     "CIDRSummaryTypeDef",
     "UpdateFirewallEncryptionConfigurationRequestRequestTypeDef",
     "UpdateFirewallEncryptionConfigurationResponseTypeDef",
     "CreateFirewallRequestRequestTypeDef",
     "FirewallPolicyResponseTypeDef",
     "FirewallTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "RuleGroupResponseTypeDef",
     "DescribeRuleGroupMetadataResponseTypeDef",
+    "PublishMetricActionOutputTypeDef",
     "PublishMetricActionTypeDef",
     "ListFirewallsResponseTypeDef",
     "ListFirewallPoliciesResponseTypeDef",
+    "PolicyVariablesOutputTypeDef",
+    "ReferenceSetsOutputTypeDef",
     "ReferenceSetsTypeDef",
     "PolicyVariablesTypeDef",
+    "ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef",
+    "ListFirewallsRequestListFirewallsPaginateTypeDef",
+    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
+    "ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListRuleGroupsResponseTypeDef",
     "ListTLSInspectionConfigurationsResponseTypeDef",
+    "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
+    "ServerCertificateScopeOutputTypeDef",
     "ServerCertificateScopeTypeDef",
+    "MatchAttributesOutputTypeDef",
     "MatchAttributesTypeDef",
     "SyncStateTypeDef",
+    "RuleVariablesOutputTypeDef",
     "RuleVariablesTypeDef",
+    "StatefulRuleOutputTypeDef",
     "StatefulRuleTypeDef",
     "StatefulRuleGroupReferenceTypeDef",
     "TLSInspectionConfigurationResponseTypeDef",
     "CapacityUsageSummaryTypeDef",
     "CreateFirewallPolicyResponseTypeDef",
     "DeleteFirewallPolicyResponseTypeDef",
     "UpdateFirewallPolicyResponseTypeDef",
     "CreateRuleGroupResponseTypeDef",
     "DeleteRuleGroupResponseTypeDef",
     "UpdateRuleGroupResponseTypeDef",
+    "ActionDefinitionOutputTypeDef",
     "ActionDefinitionTypeDef",
     "DescribeLoggingConfigurationResponseTypeDef",
-    "UpdateLoggingConfigurationRequestRequestTypeDef",
     "UpdateLoggingConfigurationResponseTypeDef",
+    "LoggingConfigurationUnionTypeDef",
+    "UpdateLoggingConfigurationRequestRequestTypeDef",
+    "ServerCertificateConfigurationOutputTypeDef",
     "ServerCertificateConfigurationTypeDef",
+    "RuleDefinitionOutputTypeDef",
     "RuleDefinitionTypeDef",
     "CreateTLSInspectionConfigurationResponseTypeDef",
     "DeleteTLSInspectionConfigurationResponseTypeDef",
     "UpdateTLSInspectionConfigurationResponseTypeDef",
     "FirewallStatusTypeDef",
+    "CustomActionOutputTypeDef",
     "CustomActionTypeDef",
+    "TLSInspectionConfigurationOutputTypeDef",
     "TLSInspectionConfigurationTypeDef",
+    "StatelessRuleOutputTypeDef",
     "StatelessRuleTypeDef",
     "CreateFirewallResponseTypeDef",
     "DeleteFirewallResponseTypeDef",
     "DescribeFirewallResponseTypeDef",
+    "FirewallPolicyOutputTypeDef",
     "FirewallPolicyTypeDef",
-    "CreateTLSInspectionConfigurationRequestRequestTypeDef",
     "DescribeTLSInspectionConfigurationResponseTypeDef",
+    "CreateTLSInspectionConfigurationRequestRequestTypeDef",
+    "TLSInspectionConfigurationUnionTypeDef",
     "UpdateTLSInspectionConfigurationRequestRequestTypeDef",
+    "StatelessRulesAndCustomActionsOutputTypeDef",
     "StatelessRulesAndCustomActionsTypeDef",
-    "CreateFirewallPolicyRequestRequestTypeDef",
     "DescribeFirewallPolicyResponseTypeDef",
+    "CreateFirewallPolicyRequestRequestTypeDef",
+    "FirewallPolicyUnionTypeDef",
     "UpdateFirewallPolicyRequestRequestTypeDef",
+    "RulesSourceOutputTypeDef",
     "RulesSourceTypeDef",
+    "RuleGroupOutputTypeDef",
     "RuleGroupTypeDef",
-    "CreateRuleGroupRequestRequestTypeDef",
     "DescribeRuleGroupResponseTypeDef",
+    "CreateRuleGroupRequestRequestTypeDef",
+    "RuleGroupUnionTypeDef",
     "UpdateRuleGroupRequestRequestTypeDef",
 )
 
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
         "AddressDefinition": str,
@@ -205,22 +233,22 @@
 
 class AssociateFirewallPolicyRequestRequestTypeDef(
     _RequiredAssociateFirewallPolicyRequestRequestTypeDef,
     _OptionalAssociateFirewallPolicyRequestRequestTypeDef,
 ):
     pass
 
-AssociateFirewallPolicyResponseTypeDef = TypedDict(
-    "AssociateFirewallPolicyResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "FirewallArn": str,
-        "FirewallName": str,
-        "FirewallPolicyArn": str,
-        "UpdateToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredSubnetMappingTypeDef = TypedDict(
     "_RequiredSubnetMappingTypeDef",
     {
         "SubnetId": str,
@@ -366,22 +394,14 @@
 DescribeResourcePolicyRequestRequestTypeDef = TypedDict(
     "DescribeResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-DescribeResourcePolicyResponseTypeDef = TypedDict(
-    "DescribeResourcePolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeRuleGroupMetadataRequestRequestTypeDef = TypedDict(
     "DescribeRuleGroupMetadataRequestRequestTypeDef",
     {
         "RuleGroupName": str,
         "RuleGroupArn": str,
         "Type": RuleGroupTypeType,
     },
@@ -487,14 +507,21 @@
         "SourcePort": str,
         "Direction": StatefulRuleDirectionType,
         "Destination": str,
         "DestinationPort": str,
     },
 )
 
+IPSetOutputTypeDef = TypedDict(
+    "IPSetOutputTypeDef",
+    {
+        "Definition": List[str],
+    },
+)
+
 IPSetReferenceTypeDef = TypedDict(
     "IPSetReferenceTypeDef",
     {
         "ReferenceArn": str,
     },
     total=False,
 )
@@ -502,61 +529,43 @@
 IPSetTypeDef = TypedDict(
     "IPSetTypeDef",
     {
         "Definition": Sequence[str],
     },
 )
 
-ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef = TypedDict(
-    "ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef",
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
 
 ListFirewallPoliciesRequestRequestTypeDef = TypedDict(
     "ListFirewallPoliciesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListFirewallsRequestListFirewallsPaginateTypeDef = TypedDict(
-    "ListFirewallsRequestListFirewallsPaginateTypeDef",
-    {
-        "VpcIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFirewallsRequestRequestTypeDef = TypedDict(
     "ListFirewallsRequestRequestTypeDef",
     {
         "NextToken": str,
         "VpcIds": Sequence[str],
         "MaxResults": int,
     },
     total=False,
 )
 
-ListRuleGroupsRequestListRuleGroupsPaginateTypeDef = TypedDict(
-    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
-    {
-        "Scope": ResourceManagedStatusType,
-        "ManagedType": ResourceManagedTypeType,
-        "Type": RuleGroupTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRuleGroupsRequestRequestTypeDef = TypedDict(
     "ListRuleGroupsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Scope": ResourceManagedStatusType,
         "ManagedType": ResourceManagedTypeType,
@@ -570,22 +579,14 @@
     {
         "Name": str,
         "Arn": str,
     },
     total=False,
 )
 
-ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef = TypedDict(
-    "ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTLSInspectionConfigurationsRequestRequestTypeDef = TypedDict(
     "ListTLSInspectionConfigurationsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -596,34 +597,14 @@
     {
         "Name": str,
         "Arn": str,
     },
     total=False,
 )
 
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
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
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -637,31 +618,59 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
+LogDestinationConfigOutputTypeDef = TypedDict(
+    "LogDestinationConfigOutputTypeDef",
+    {
+        "LogType": LogTypeType,
+        "LogDestinationType": LogDestinationTypeType,
+        "LogDestination": Dict[str, str],
+    },
+)
+
 LogDestinationConfigTypeDef = TypedDict(
     "LogDestinationConfigTypeDef",
     {
         "LogType": LogTypeType,
         "LogDestinationType": LogDestinationTypeType,
-        "LogDestination": Dict[str, str],
+        "LogDestination": Mapping[str, str],
     },
 )
 
 PortRangeTypeDef = TypedDict(
     "PortRangeTypeDef",
     {
         "FromPort": int,
         "ToPort": int,
     },
 )
 
+_RequiredTCPFlagFieldOutputTypeDef = TypedDict(
+    "_RequiredTCPFlagFieldOutputTypeDef",
+    {
+        "Flags": List[TCPFlagType],
+    },
+)
+_OptionalTCPFlagFieldOutputTypeDef = TypedDict(
+    "_OptionalTCPFlagFieldOutputTypeDef",
+    {
+        "Masks": List[TCPFlagType],
+    },
+    total=False,
+)
+
+class TCPFlagFieldOutputTypeDef(
+    _RequiredTCPFlagFieldOutputTypeDef, _OptionalTCPFlagFieldOutputTypeDef
+):
+    pass
+
 _RequiredTCPFlagFieldTypeDef = TypedDict(
     "_RequiredTCPFlagFieldTypeDef",
     {
         "Flags": Sequence[TCPFlagType],
     },
 )
 _OptionalTCPFlagFieldTypeDef = TypedDict(
@@ -671,29 +680,27 @@
     },
     total=False,
 )
 
 class TCPFlagFieldTypeDef(_RequiredTCPFlagFieldTypeDef, _OptionalTCPFlagFieldTypeDef):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+PerObjectStatusTypeDef = TypedDict(
+    "PerObjectStatusTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "SyncStatus": PerObjectSyncStatusType,
+        "UpdateToken": str,
     },
     total=False,
 )
 
-PerObjectStatusTypeDef = TypedDict(
-    "PerObjectStatusTypeDef",
+PortSetOutputTypeDef = TypedDict(
+    "PortSetOutputTypeDef",
     {
-        "SyncStatus": PerObjectSyncStatusType,
-        "UpdateToken": str,
+        "Definition": List[str],
     },
     total=False,
 )
 
 PortSetTypeDef = TypedDict(
     "PortSetTypeDef",
     {
@@ -706,25 +713,31 @@
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Policy": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_RequiredRuleOptionOutputTypeDef = TypedDict(
+    "_RequiredRuleOptionOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Keyword": str,
+    },
+)
+_OptionalRuleOptionOutputTypeDef = TypedDict(
+    "_OptionalRuleOptionOutputTypeDef",
+    {
+        "Settings": List[str],
     },
+    total=False,
 )
 
+class RuleOptionOutputTypeDef(_RequiredRuleOptionOutputTypeDef, _OptionalRuleOptionOutputTypeDef):
+    pass
+
 _RequiredRuleOptionTypeDef = TypedDict(
     "_RequiredRuleOptionTypeDef",
     {
         "Keyword": str,
     },
 )
 _OptionalRuleOptionTypeDef = TypedDict(
@@ -734,14 +747,23 @@
     },
     total=False,
 )
 
 class RuleOptionTypeDef(_RequiredRuleOptionTypeDef, _OptionalRuleOptionTypeDef):
     pass
 
+RulesSourceListOutputTypeDef = TypedDict(
+    "RulesSourceListOutputTypeDef",
+    {
+        "Targets": List[str],
+        "TargetTypes": List[TargetTypeType],
+        "GeneratedRulesType": GeneratedRulesTypeType,
+    },
+)
+
 RulesSourceListTypeDef = TypedDict(
     "RulesSourceListTypeDef",
     {
         "Targets": Sequence[str],
         "TargetTypes": Sequence[TargetTypeType],
         "GeneratedRulesType": GeneratedRulesTypeType,
     },
@@ -800,47 +822,25 @@
 
 class UpdateFirewallDeleteProtectionRequestRequestTypeDef(
     _RequiredUpdateFirewallDeleteProtectionRequestRequestTypeDef,
     _OptionalUpdateFirewallDeleteProtectionRequestRequestTypeDef,
 ):
     pass
 
-UpdateFirewallDeleteProtectionResponseTypeDef = TypedDict(
-    "UpdateFirewallDeleteProtectionResponseTypeDef",
-    {
-        "FirewallArn": str,
-        "FirewallName": str,
-        "DeleteProtection": bool,
-        "UpdateToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateFirewallDescriptionRequestRequestTypeDef = TypedDict(
     "UpdateFirewallDescriptionRequestRequestTypeDef",
     {
         "UpdateToken": str,
         "FirewallArn": str,
         "FirewallName": str,
         "Description": str,
     },
     total=False,
 )
 
-UpdateFirewallDescriptionResponseTypeDef = TypedDict(
-    "UpdateFirewallDescriptionResponseTypeDef",
-    {
-        "FirewallArn": str,
-        "FirewallName": str,
-        "Description": str,
-        "UpdateToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef",
     {
         "FirewallPolicyChangeProtection": bool,
     },
 )
 _OptionalUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef = TypedDict(
@@ -855,25 +855,14 @@
 
 class UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef(
     _RequiredUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef,
     _OptionalUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef,
 ):
     pass
 
-UpdateFirewallPolicyChangeProtectionResponseTypeDef = TypedDict(
-    "UpdateFirewallPolicyChangeProtectionResponseTypeDef",
-    {
-        "UpdateToken": str,
-        "FirewallArn": str,
-        "FirewallName": str,
-        "FirewallPolicyChangeProtection": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateSubnetChangeProtectionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSubnetChangeProtectionRequestRequestTypeDef",
     {
         "SubnetChangeProtection": bool,
     },
 )
 _OptionalUpdateSubnetChangeProtectionRequestRequestTypeDef = TypedDict(
@@ -888,22 +877,74 @@
 
 class UpdateSubnetChangeProtectionRequestRequestTypeDef(
     _RequiredUpdateSubnetChangeProtectionRequestRequestTypeDef,
     _OptionalUpdateSubnetChangeProtectionRequestRequestTypeDef,
 ):
     pass
 
+AssociateFirewallPolicyResponseTypeDef = TypedDict(
+    "AssociateFirewallPolicyResponseTypeDef",
+    {
+        "FirewallArn": str,
+        "FirewallName": str,
+        "FirewallPolicyArn": str,
+        "UpdateToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeResourcePolicyResponseTypeDef = TypedDict(
+    "DescribeResourcePolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFirewallDeleteProtectionResponseTypeDef = TypedDict(
+    "UpdateFirewallDeleteProtectionResponseTypeDef",
+    {
+        "FirewallArn": str,
+        "FirewallName": str,
+        "DeleteProtection": bool,
+        "UpdateToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFirewallDescriptionResponseTypeDef = TypedDict(
+    "UpdateFirewallDescriptionResponseTypeDef",
+    {
+        "FirewallArn": str,
+        "FirewallName": str,
+        "Description": str,
+        "UpdateToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFirewallPolicyChangeProtectionResponseTypeDef = TypedDict(
+    "UpdateFirewallPolicyChangeProtectionResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "FirewallArn": str,
+        "FirewallName": str,
+        "FirewallPolicyChangeProtection": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateSubnetChangeProtectionResponseTypeDef = TypedDict(
     "UpdateSubnetChangeProtectionResponseTypeDef",
     {
         "UpdateToken": str,
         "FirewallArn": str,
         "FirewallName": str,
         "SubnetChangeProtection": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAssociateSubnetsRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateSubnetsRequestRequestTypeDef",
     {
         "SubnetMappings": Sequence[SubnetMappingTypeDef],
@@ -927,26 +968,26 @@
 AssociateSubnetsResponseTypeDef = TypedDict(
     "AssociateSubnetsResponseTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
         "SubnetMappings": List[SubnetMappingTypeDef],
         "UpdateToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateSubnetsResponseTypeDef = TypedDict(
     "DisassociateSubnetsResponseTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
         "SubnetMappings": List[SubnetMappingTypeDef],
         "UpdateToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CIDRSummaryTypeDef = TypedDict(
     "CIDRSummaryTypeDef",
     {
         "AvailableCIDRCount": int,
@@ -970,15 +1011,15 @@
 UpdateFirewallEncryptionConfigurationResponseTypeDef = TypedDict(
     "UpdateFirewallEncryptionConfigurationResponseTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
         "UpdateToken": str,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateFirewallRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFirewallRequestRequestTypeDef",
     {
         "FirewallName": str,
@@ -1061,15 +1102,15 @@
     pass
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "NextToken": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -1114,15 +1155,22 @@
         "RuleGroupArn": str,
         "RuleGroupName": str,
         "Description": str,
         "Type": RuleGroupTypeType,
         "Capacity": int,
         "StatefulRuleOptions": StatefulRuleOptionsTypeDef,
         "LastModifiedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PublishMetricActionOutputTypeDef = TypedDict(
+    "PublishMetricActionOutputTypeDef",
+    {
+        "Dimensions": List[DimensionTypeDef],
     },
 )
 
 PublishMetricActionTypeDef = TypedDict(
     "PublishMetricActionTypeDef",
     {
         "Dimensions": Sequence[DimensionTypeDef],
@@ -1130,27 +1178,43 @@
 )
 
 ListFirewallsResponseTypeDef = TypedDict(
     "ListFirewallsResponseTypeDef",
     {
         "NextToken": str,
         "Firewalls": List[FirewallMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFirewallPoliciesResponseTypeDef = TypedDict(
     "ListFirewallPoliciesResponseTypeDef",
     {
         "NextToken": str,
         "FirewallPolicies": List[FirewallPolicyMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PolicyVariablesOutputTypeDef = TypedDict(
+    "PolicyVariablesOutputTypeDef",
+    {
+        "RuleVariables": Dict[str, IPSetOutputTypeDef],
+    },
+    total=False,
+)
+
+ReferenceSetsOutputTypeDef = TypedDict(
+    "ReferenceSetsOutputTypeDef",
+    {
+        "IPSetReferences": Dict[str, IPSetReferenceTypeDef],
+    },
+    total=False,
+)
+
 ReferenceSetsTypeDef = TypedDict(
     "ReferenceSetsTypeDef",
     {
         "IPSetReferences": Mapping[str, IPSetReferenceTypeDef],
     },
     total=False,
 )
@@ -1159,51 +1223,139 @@
     "PolicyVariablesTypeDef",
     {
         "RuleVariables": Mapping[str, IPSetTypeDef],
     },
     total=False,
 )
 
+ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef = TypedDict(
+    "ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListFirewallsRequestListFirewallsPaginateTypeDef = TypedDict(
+    "ListFirewallsRequestListFirewallsPaginateTypeDef",
+    {
+        "VpcIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRuleGroupsRequestListRuleGroupsPaginateTypeDef = TypedDict(
+    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
+    {
+        "Scope": ResourceManagedStatusType,
+        "ManagedType": ResourceManagedTypeType,
+        "Type": RuleGroupTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef = TypedDict(
+    "ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
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
 ListRuleGroupsResponseTypeDef = TypedDict(
     "ListRuleGroupsResponseTypeDef",
     {
         "NextToken": str,
         "RuleGroups": List[RuleGroupMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTLSInspectionConfigurationsResponseTypeDef = TypedDict(
     "ListTLSInspectionConfigurationsResponseTypeDef",
     {
         "NextToken": str,
         "TLSInspectionConfigurations": List[TLSInspectionConfigurationMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LoggingConfigurationOutputTypeDef = TypedDict(
+    "LoggingConfigurationOutputTypeDef",
+    {
+        "LogDestinationConfigs": List[LogDestinationConfigOutputTypeDef],
     },
 )
 
 LoggingConfigurationTypeDef = TypedDict(
     "LoggingConfigurationTypeDef",
     {
-        "LogDestinationConfigs": List[LogDestinationConfigTypeDef],
+        "LogDestinationConfigs": Sequence[LogDestinationConfigTypeDef],
+    },
+)
+
+ServerCertificateScopeOutputTypeDef = TypedDict(
+    "ServerCertificateScopeOutputTypeDef",
+    {
+        "Sources": List[AddressTypeDef],
+        "Destinations": List[AddressTypeDef],
+        "SourcePorts": List[PortRangeTypeDef],
+        "DestinationPorts": List[PortRangeTypeDef],
+        "Protocols": List[int],
     },
+    total=False,
 )
 
 ServerCertificateScopeTypeDef = TypedDict(
     "ServerCertificateScopeTypeDef",
     {
         "Sources": Sequence[AddressTypeDef],
         "Destinations": Sequence[AddressTypeDef],
         "SourcePorts": Sequence[PortRangeTypeDef],
         "DestinationPorts": Sequence[PortRangeTypeDef],
         "Protocols": Sequence[int],
     },
     total=False,
 )
 
+MatchAttributesOutputTypeDef = TypedDict(
+    "MatchAttributesOutputTypeDef",
+    {
+        "Sources": List[AddressTypeDef],
+        "Destinations": List[AddressTypeDef],
+        "SourcePorts": List[PortRangeTypeDef],
+        "DestinationPorts": List[PortRangeTypeDef],
+        "Protocols": List[int],
+        "TCPFlags": List[TCPFlagFieldOutputTypeDef],
+    },
+    total=False,
+)
+
 MatchAttributesTypeDef = TypedDict(
     "MatchAttributesTypeDef",
     {
         "Sources": Sequence[AddressTypeDef],
         "Destinations": Sequence[AddressTypeDef],
         "SourcePorts": Sequence[PortRangeTypeDef],
         "DestinationPorts": Sequence[PortRangeTypeDef],
@@ -1218,23 +1370,41 @@
     {
         "Attachment": AttachmentTypeDef,
         "Config": Dict[str, PerObjectStatusTypeDef],
     },
     total=False,
 )
 
+RuleVariablesOutputTypeDef = TypedDict(
+    "RuleVariablesOutputTypeDef",
+    {
+        "IPSets": Dict[str, IPSetOutputTypeDef],
+        "PortSets": Dict[str, PortSetOutputTypeDef],
+    },
+    total=False,
+)
+
 RuleVariablesTypeDef = TypedDict(
     "RuleVariablesTypeDef",
     {
         "IPSets": Mapping[str, IPSetTypeDef],
         "PortSets": Mapping[str, PortSetTypeDef],
     },
     total=False,
 )
 
+StatefulRuleOutputTypeDef = TypedDict(
+    "StatefulRuleOutputTypeDef",
+    {
+        "Action": StatefulActionType,
+        "Header": HeaderTypeDef,
+        "RuleOptions": List[RuleOptionOutputTypeDef],
+    },
+)
+
 StatefulRuleTypeDef = TypedDict(
     "StatefulRuleTypeDef",
     {
         "Action": StatefulActionType,
         "Header": HeaderTypeDef,
         "RuleOptions": Sequence[RuleOptionTypeDef],
     },
@@ -1297,138 +1467,166 @@
 )
 
 CreateFirewallPolicyResponseTypeDef = TypedDict(
     "CreateFirewallPolicyResponseTypeDef",
     {
         "UpdateToken": str,
         "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteFirewallPolicyResponseTypeDef = TypedDict(
     "DeleteFirewallPolicyResponseTypeDef",
     {
         "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFirewallPolicyResponseTypeDef = TypedDict(
     "UpdateFirewallPolicyResponseTypeDef",
     {
         "UpdateToken": str,
         "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRuleGroupResponseTypeDef = TypedDict(
     "CreateRuleGroupResponseTypeDef",
     {
         "UpdateToken": str,
         "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRuleGroupResponseTypeDef = TypedDict(
     "DeleteRuleGroupResponseTypeDef",
     {
         "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRuleGroupResponseTypeDef = TypedDict(
     "UpdateRuleGroupResponseTypeDef",
     {
         "UpdateToken": str,
         "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ActionDefinitionOutputTypeDef = TypedDict(
+    "ActionDefinitionOutputTypeDef",
+    {
+        "PublishMetricAction": PublishMetricActionOutputTypeDef,
     },
+    total=False,
 )
 
 ActionDefinitionTypeDef = TypedDict(
     "ActionDefinitionTypeDef",
     {
         "PublishMetricAction": PublishMetricActionTypeDef,
     },
     total=False,
 )
 
 DescribeLoggingConfigurationResponseTypeDef = TypedDict(
     "DescribeLoggingConfigurationResponseTypeDef",
     {
         "FirewallArn": str,
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateLoggingConfigurationResponseTypeDef = TypedDict(
+    "UpdateLoggingConfigurationResponseTypeDef",
+    {
+        "FirewallArn": str,
+        "FirewallName": str,
+        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LoggingConfigurationUnionTypeDef = Union[
+    LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
+]
 UpdateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateLoggingConfigurationRequestRequestTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
     },
     total=False,
 )
 
-UpdateLoggingConfigurationResponseTypeDef = TypedDict(
-    "UpdateLoggingConfigurationResponseTypeDef",
+ServerCertificateConfigurationOutputTypeDef = TypedDict(
+    "ServerCertificateConfigurationOutputTypeDef",
     {
-        "FirewallArn": str,
-        "FirewallName": str,
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ServerCertificates": List[ServerCertificateTypeDef],
+        "Scopes": List[ServerCertificateScopeOutputTypeDef],
     },
+    total=False,
 )
 
 ServerCertificateConfigurationTypeDef = TypedDict(
     "ServerCertificateConfigurationTypeDef",
     {
         "ServerCertificates": Sequence[ServerCertificateTypeDef],
         "Scopes": Sequence[ServerCertificateScopeTypeDef],
     },
     total=False,
 )
 
+RuleDefinitionOutputTypeDef = TypedDict(
+    "RuleDefinitionOutputTypeDef",
+    {
+        "MatchAttributes": MatchAttributesOutputTypeDef,
+        "Actions": List[str],
+    },
+)
+
 RuleDefinitionTypeDef = TypedDict(
     "RuleDefinitionTypeDef",
     {
         "MatchAttributes": MatchAttributesTypeDef,
         "Actions": Sequence[str],
     },
 )
 
 CreateTLSInspectionConfigurationResponseTypeDef = TypedDict(
     "CreateTLSInspectionConfigurationResponseTypeDef",
     {
         "UpdateToken": str,
         "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteTLSInspectionConfigurationResponseTypeDef = TypedDict(
     "DeleteTLSInspectionConfigurationResponseTypeDef",
     {
         "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTLSInspectionConfigurationResponseTypeDef = TypedDict(
     "UpdateTLSInspectionConfigurationResponseTypeDef",
     {
         "UpdateToken": str,
         "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFirewallStatusTypeDef = TypedDict(
     "_RequiredFirewallStatusTypeDef",
     {
         "Status": FirewallStatusValueType,
@@ -1443,66 +1641,116 @@
     },
     total=False,
 )
 
 class FirewallStatusTypeDef(_RequiredFirewallStatusTypeDef, _OptionalFirewallStatusTypeDef):
     pass
 
+CustomActionOutputTypeDef = TypedDict(
+    "CustomActionOutputTypeDef",
+    {
+        "ActionName": str,
+        "ActionDefinition": ActionDefinitionOutputTypeDef,
+    },
+)
+
 CustomActionTypeDef = TypedDict(
     "CustomActionTypeDef",
     {
         "ActionName": str,
         "ActionDefinition": ActionDefinitionTypeDef,
     },
 )
 
+TLSInspectionConfigurationOutputTypeDef = TypedDict(
+    "TLSInspectionConfigurationOutputTypeDef",
+    {
+        "ServerCertificateConfigurations": List[ServerCertificateConfigurationOutputTypeDef],
+    },
+    total=False,
+)
+
 TLSInspectionConfigurationTypeDef = TypedDict(
     "TLSInspectionConfigurationTypeDef",
     {
         "ServerCertificateConfigurations": Sequence[ServerCertificateConfigurationTypeDef],
     },
     total=False,
 )
 
+StatelessRuleOutputTypeDef = TypedDict(
+    "StatelessRuleOutputTypeDef",
+    {
+        "RuleDefinition": RuleDefinitionOutputTypeDef,
+        "Priority": int,
+    },
+)
+
 StatelessRuleTypeDef = TypedDict(
     "StatelessRuleTypeDef",
     {
         "RuleDefinition": RuleDefinitionTypeDef,
         "Priority": int,
     },
 )
 
 CreateFirewallResponseTypeDef = TypedDict(
     "CreateFirewallResponseTypeDef",
     {
         "Firewall": FirewallTypeDef,
         "FirewallStatus": FirewallStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteFirewallResponseTypeDef = TypedDict(
     "DeleteFirewallResponseTypeDef",
     {
         "Firewall": FirewallTypeDef,
         "FirewallStatus": FirewallStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFirewallResponseTypeDef = TypedDict(
     "DescribeFirewallResponseTypeDef",
     {
         "UpdateToken": str,
         "Firewall": FirewallTypeDef,
         "FirewallStatus": FirewallStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredFirewallPolicyOutputTypeDef = TypedDict(
+    "_RequiredFirewallPolicyOutputTypeDef",
+    {
+        "StatelessDefaultActions": List[str],
+        "StatelessFragmentDefaultActions": List[str],
+    },
+)
+_OptionalFirewallPolicyOutputTypeDef = TypedDict(
+    "_OptionalFirewallPolicyOutputTypeDef",
+    {
+        "StatelessRuleGroupReferences": List[StatelessRuleGroupReferenceTypeDef],
+        "StatelessCustomActions": List[CustomActionOutputTypeDef],
+        "StatefulRuleGroupReferences": List[StatefulRuleGroupReferenceTypeDef],
+        "StatefulDefaultActions": List[str],
+        "StatefulEngineOptions": StatefulEngineOptionsTypeDef,
+        "TLSInspectionConfigurationArn": str,
+        "PolicyVariables": PolicyVariablesOutputTypeDef,
+    },
+    total=False,
+)
+
+class FirewallPolicyOutputTypeDef(
+    _RequiredFirewallPolicyOutputTypeDef, _OptionalFirewallPolicyOutputTypeDef
+):
+    pass
+
 _RequiredFirewallPolicyTypeDef = TypedDict(
     "_RequiredFirewallPolicyTypeDef",
     {
         "StatelessDefaultActions": Sequence[str],
         "StatelessFragmentDefaultActions": Sequence[str],
     },
 )
@@ -1519,14 +1767,24 @@
     },
     total=False,
 )
 
 class FirewallPolicyTypeDef(_RequiredFirewallPolicyTypeDef, _OptionalFirewallPolicyTypeDef):
     pass
 
+DescribeTLSInspectionConfigurationResponseTypeDef = TypedDict(
+    "DescribeTLSInspectionConfigurationResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "TLSInspectionConfiguration": TLSInspectionConfigurationOutputTypeDef,
+        "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateTLSInspectionConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTLSInspectionConfigurationRequestRequestTypeDef",
     {
         "TLSInspectionConfigurationName": str,
         "TLSInspectionConfiguration": TLSInspectionConfigurationTypeDef,
     },
 )
@@ -1542,24 +1800,17 @@
 
 class CreateTLSInspectionConfigurationRequestRequestTypeDef(
     _RequiredCreateTLSInspectionConfigurationRequestRequestTypeDef,
     _OptionalCreateTLSInspectionConfigurationRequestRequestTypeDef,
 ):
     pass
 
-DescribeTLSInspectionConfigurationResponseTypeDef = TypedDict(
-    "DescribeTLSInspectionConfigurationResponseTypeDef",
-    {
-        "UpdateToken": str,
-        "TLSInspectionConfiguration": TLSInspectionConfigurationTypeDef,
-        "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+TLSInspectionConfigurationUnionTypeDef = Union[
+    TLSInspectionConfigurationTypeDef, TLSInspectionConfigurationOutputTypeDef
+]
 _RequiredUpdateTLSInspectionConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTLSInspectionConfigurationRequestRequestTypeDef",
     {
         "TLSInspectionConfiguration": TLSInspectionConfigurationTypeDef,
         "UpdateToken": str,
     },
 )
@@ -1576,14 +1827,34 @@
 
 class UpdateTLSInspectionConfigurationRequestRequestTypeDef(
     _RequiredUpdateTLSInspectionConfigurationRequestRequestTypeDef,
     _OptionalUpdateTLSInspectionConfigurationRequestRequestTypeDef,
 ):
     pass
 
+_RequiredStatelessRulesAndCustomActionsOutputTypeDef = TypedDict(
+    "_RequiredStatelessRulesAndCustomActionsOutputTypeDef",
+    {
+        "StatelessRules": List[StatelessRuleOutputTypeDef],
+    },
+)
+_OptionalStatelessRulesAndCustomActionsOutputTypeDef = TypedDict(
+    "_OptionalStatelessRulesAndCustomActionsOutputTypeDef",
+    {
+        "CustomActions": List[CustomActionOutputTypeDef],
+    },
+    total=False,
+)
+
+class StatelessRulesAndCustomActionsOutputTypeDef(
+    _RequiredStatelessRulesAndCustomActionsOutputTypeDef,
+    _OptionalStatelessRulesAndCustomActionsOutputTypeDef,
+):
+    pass
+
 _RequiredStatelessRulesAndCustomActionsTypeDef = TypedDict(
     "_RequiredStatelessRulesAndCustomActionsTypeDef",
     {
         "StatelessRules": Sequence[StatelessRuleTypeDef],
     },
 )
 _OptionalStatelessRulesAndCustomActionsTypeDef = TypedDict(
@@ -1595,14 +1866,24 @@
 )
 
 class StatelessRulesAndCustomActionsTypeDef(
     _RequiredStatelessRulesAndCustomActionsTypeDef, _OptionalStatelessRulesAndCustomActionsTypeDef
 ):
     pass
 
+DescribeFirewallPolicyResponseTypeDef = TypedDict(
+    "DescribeFirewallPolicyResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
+        "FirewallPolicy": FirewallPolicyOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateFirewallPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFirewallPolicyRequestRequestTypeDef",
     {
         "FirewallPolicyName": str,
         "FirewallPolicy": FirewallPolicyTypeDef,
     },
 )
@@ -1619,24 +1900,15 @@
 
 class CreateFirewallPolicyRequestRequestTypeDef(
     _RequiredCreateFirewallPolicyRequestRequestTypeDef,
     _OptionalCreateFirewallPolicyRequestRequestTypeDef,
 ):
     pass
 
-DescribeFirewallPolicyResponseTypeDef = TypedDict(
-    "DescribeFirewallPolicyResponseTypeDef",
-    {
-        "UpdateToken": str,
-        "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
-        "FirewallPolicy": FirewallPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+FirewallPolicyUnionTypeDef = Union[FirewallPolicyTypeDef, FirewallPolicyOutputTypeDef]
 _RequiredUpdateFirewallPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFirewallPolicyRequestRequestTypeDef",
     {
         "UpdateToken": str,
         "FirewallPolicy": FirewallPolicyTypeDef,
     },
 )
@@ -1654,25 +1926,55 @@
 
 class UpdateFirewallPolicyRequestRequestTypeDef(
     _RequiredUpdateFirewallPolicyRequestRequestTypeDef,
     _OptionalUpdateFirewallPolicyRequestRequestTypeDef,
 ):
     pass
 
+RulesSourceOutputTypeDef = TypedDict(
+    "RulesSourceOutputTypeDef",
+    {
+        "RulesString": str,
+        "RulesSourceList": RulesSourceListOutputTypeDef,
+        "StatefulRules": List[StatefulRuleOutputTypeDef],
+        "StatelessRulesAndCustomActions": StatelessRulesAndCustomActionsOutputTypeDef,
+    },
+    total=False,
+)
+
 RulesSourceTypeDef = TypedDict(
     "RulesSourceTypeDef",
     {
         "RulesString": str,
         "RulesSourceList": RulesSourceListTypeDef,
         "StatefulRules": Sequence[StatefulRuleTypeDef],
         "StatelessRulesAndCustomActions": StatelessRulesAndCustomActionsTypeDef,
     },
     total=False,
 )
 
+_RequiredRuleGroupOutputTypeDef = TypedDict(
+    "_RequiredRuleGroupOutputTypeDef",
+    {
+        "RulesSource": RulesSourceOutputTypeDef,
+    },
+)
+_OptionalRuleGroupOutputTypeDef = TypedDict(
+    "_OptionalRuleGroupOutputTypeDef",
+    {
+        "RuleVariables": RuleVariablesOutputTypeDef,
+        "ReferenceSets": ReferenceSetsOutputTypeDef,
+        "StatefulRuleOptions": StatefulRuleOptionsTypeDef,
+    },
+    total=False,
+)
+
+class RuleGroupOutputTypeDef(_RequiredRuleGroupOutputTypeDef, _OptionalRuleGroupOutputTypeDef):
+    pass
+
 _RequiredRuleGroupTypeDef = TypedDict(
     "_RequiredRuleGroupTypeDef",
     {
         "RulesSource": RulesSourceTypeDef,
     },
 )
 _OptionalRuleGroupTypeDef = TypedDict(
@@ -1684,14 +1986,24 @@
     },
     total=False,
 )
 
 class RuleGroupTypeDef(_RequiredRuleGroupTypeDef, _OptionalRuleGroupTypeDef):
     pass
 
+DescribeRuleGroupResponseTypeDef = TypedDict(
+    "DescribeRuleGroupResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "RuleGroup": RuleGroupOutputTypeDef,
+        "RuleGroupResponse": RuleGroupResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRuleGroupRequestRequestTypeDef",
     {
         "RuleGroupName": str,
         "Type": RuleGroupTypeType,
         "Capacity": int,
     },
@@ -1711,24 +2023,15 @@
 )
 
 class CreateRuleGroupRequestRequestTypeDef(
     _RequiredCreateRuleGroupRequestRequestTypeDef, _OptionalCreateRuleGroupRequestRequestTypeDef
 ):
     pass
 
-DescribeRuleGroupResponseTypeDef = TypedDict(
-    "DescribeRuleGroupResponseTypeDef",
-    {
-        "UpdateToken": str,
-        "RuleGroup": RuleGroupTypeDef,
-        "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+RuleGroupUnionTypeDef = Union[RuleGroupTypeDef, RuleGroupOutputTypeDef]
 _RequiredUpdateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRuleGroupRequestRequestTypeDef",
     {
         "UpdateToken": str,
     },
 )
 _OptionalUpdateRuleGroupRequestRequestTypeDef = TypedDict(
```

### Comparing `types-aiobotocore-network-firewall-2.5.2/types_aiobotocore_network_firewall.egg-info/SOURCES.txt` & `types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall.egg-info/SOURCES.txt`

 * *Files identical despite different names*


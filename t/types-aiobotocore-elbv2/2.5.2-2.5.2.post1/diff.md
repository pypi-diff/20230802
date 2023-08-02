# Comparing `tmp/types-aiobotocore-elbv2-2.5.2.tar.gz` & `tmp/types-aiobotocore-elbv2-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-elbv2-2.5.2.tar", last modified: Sat Jul  8 01:43:36 2023, max compression
+gzip compressed data, was "types-aiobotocore-elbv2-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:16 2023, max compression
```

## Comparing `types-aiobotocore-elbv2-2.5.2.tar` & `types-aiobotocore-elbv2-2.5.2.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:36.674113 types-aiobotocore-elbv2-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:30:31.000000 types-aiobotocore-elbv2-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20402 2023-07-08 01:43:36.666113 types-aiobotocore-elbv2-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18828 2023-07-08 01:30:31.000000 types-aiobotocore-elbv2-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:36.674113 types-aiobotocore-elbv2-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-08 01:30:31.000000 types-aiobotocore-elbv2-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:36.666113 types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2/
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-08 01:30:31.000000 types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-08 01:30:31.000000 types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-08 01:30:31.000000 types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35950 2023-07-08 01:30:33.000000 types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    35895 2023-07-08 01:30:32.000000 types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11662 2023-07-08 01:30:33.000000 types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-07-08 01:30:33.000000 types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-07-08 01:30:33.000000 types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-07-08 01:30:33.000000 types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:30:31.000000 types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    38688 2023-07-08 01:30:34.000000 types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38647 2023-07-08 01:30:33.000000 types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:30:31.000000 types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-07-08 01:30:33.000000 types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-07-08 01:30:33.000000 types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:36.666113 types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20402 2023-07-08 01:43:36.000000 types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-08 01:43:36.000000 types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:36.000000 types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:36.000000 types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:36.000000 types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-08 01:43:36.000000 types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:16.649589 types-aiobotocore-elbv2-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:21.000000 types-aiobotocore-elbv2-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20862 2023-08-02 14:52:16.649589 types-aiobotocore-elbv2-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19335 2023-08-02 14:38:21.000000 types-aiobotocore-elbv2-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:16.649589 types-aiobotocore-elbv2-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-08-02 14:38:21.000000 types-aiobotocore-elbv2-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:16.649589 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-08-02 14:38:21.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-08-02 14:38:21.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-08-02 14:38:21.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35990 2023-08-02 14:38:21.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35935 2023-08-02 14:38:21.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11662 2023-08-02 14:38:22.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-08-02 14:38:22.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-08-02 14:38:21.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-08-02 14:38:21.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:21.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    43710 2023-08-02 14:38:22.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43664 2023-08-02 14:38:22.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:21.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-08-02 14:38:21.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-08-02 14:38:21.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:16.649589 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20862 2023-08-02 14:52:16.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-02 14:52:16.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:16.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:16.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:16.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 14:52:16.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-elbv2-2.5.2/LICENSE` & `types-aiobotocore-elbv2-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elbv2-2.5.2/PKG-INFO` & `types-aiobotocore-elbv2-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elbv2
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ElasticLoadBalancingv2 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ElasticLoadBalancingv2 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore elbv2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore elbv2 type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-elbv2"></a>
 
 # types-aiobotocore-elbv2
 
 [![PyPI - types-aiobotocore-elbv2](https://img.shields.io/pypi/v/types-aiobotocore-elbv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elbv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elbv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elbv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-elbv2?color=blue)](https://pypistats.org/packages/types-aiobotocore-elbv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elbv2)](https://pepy.tech/project/types-aiobotocore-elbv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ElasticLoadBalancingv2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
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
 [types-aiobotocore-elbv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/).
 
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
@@ -394,138 +393,151 @@
 )
 
 
 def check_value(value: ActionTypeEnumType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_elbv2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_elbv2.type_defs import (
-    AuthenticateCognitoActionConfigTypeDef,
-    AuthenticateOidcActionConfigTypeDef,
+    AuthenticateCognitoActionConfigOutputTypeDef,
+    AuthenticateOidcActionConfigOutputTypeDef,
     FixedResponseActionConfigTypeDef,
     RedirectActionConfigTypeDef,
+    AuthenticateCognitoActionConfigTypeDef,
+    AuthenticateOidcActionConfigTypeDef,
     CertificateTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     LoadBalancerAddressTypeDef,
     CipherTypeDef,
     SubnetMappingTypeDef,
     MatcherTypeDef,
     DeleteListenerInputRequestTypeDef,
     DeleteLoadBalancerInputRequestTypeDef,
     DeleteRuleInputRequestTypeDef,
     DeleteTargetGroupInputRequestTypeDef,
     TargetDescriptionTypeDef,
-    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     LimitTypeDef,
-    DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
     DescribeListenerCertificatesInputRequestTypeDef,
-    DescribeListenersInputDescribeListenersPaginateTypeDef,
     DescribeListenersInputRequestTypeDef,
     DescribeLoadBalancerAttributesInputRequestTypeDef,
     LoadBalancerAttributeTypeDef,
-    DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef,
     WaiterConfigTypeDef,
     DescribeLoadBalancersInputRequestTypeDef,
-    DescribeRulesInputDescribeRulesPaginateTypeDef,
     DescribeRulesInputRequestTypeDef,
-    DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef,
     DescribeSSLPoliciesInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
     DescribeTargetGroupAttributesInputRequestTypeDef,
     TargetGroupAttributeTypeDef,
-    DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef,
     DescribeTargetGroupsInputRequestTypeDef,
     TargetGroupStickinessConfigTypeDef,
     TargetGroupTupleTypeDef,
+    HostHeaderConditionConfigOutputTypeDef,
     HostHeaderConditionConfigTypeDef,
+    HttpHeaderConditionConfigOutputTypeDef,
     HttpHeaderConditionConfigTypeDef,
+    HttpRequestMethodConditionConfigOutputTypeDef,
     HttpRequestMethodConditionConfigTypeDef,
     LoadBalancerStateTypeDef,
-    PaginatorConfigTypeDef,
+    PathPatternConditionConfigOutputTypeDef,
     PathPatternConditionConfigTypeDef,
     QueryStringKeyValuePairTypeDef,
     RemoveTagsInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    SourceIpConditionConfigOutputTypeDef,
     SourceIpConditionConfigTypeDef,
     RulePriorityPairTypeDef,
     SetIpAddressTypeInputRequestTypeDef,
-    SetIpAddressTypeOutputTypeDef,
     SetSecurityGroupsInputRequestTypeDef,
-    SetSecurityGroupsOutputTypeDef,
     TargetHealthTypeDef,
     AddListenerCertificatesInputRequestTypeDef,
+    RemoveListenerCertificatesInputRequestTypeDef,
     AddListenerCertificatesOutputTypeDef,
     DescribeListenerCertificatesOutputTypeDef,
-    RemoveListenerCertificatesInputRequestTypeDef,
+    SetIpAddressTypeOutputTypeDef,
+    SetSecurityGroupsOutputTypeDef,
     AddTagsInputRequestTypeDef,
     TagDescriptionTypeDef,
     AvailabilityZoneTypeDef,
     SslPolicyTypeDef,
     CreateLoadBalancerInputRequestTypeDef,
     SetSubnetsInputRequestTypeDef,
     CreateTargetGroupInputRequestTypeDef,
     ModifyTargetGroupInputRequestTypeDef,
     TargetGroupTypeDef,
     DeregisterTargetsInputRequestTypeDef,
     DescribeTargetHealthInputRequestTypeDef,
     RegisterTargetsInputRequestTypeDef,
+    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
+    DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
+    DescribeListenersInputDescribeListenersPaginateTypeDef,
+    DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef,
+    DescribeRulesInputDescribeRulesPaginateTypeDef,
+    DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef,
+    DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef,
     DescribeAccountLimitsOutputTypeDef,
     DescribeLoadBalancerAttributesOutputTypeDef,
     ModifyLoadBalancerAttributesInputRequestTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
     DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef,
     DescribeLoadBalancersInputLoadBalancerExistsWaitTypeDef,
     DescribeLoadBalancersInputLoadBalancersDeletedWaitTypeDef,
     DescribeTargetHealthInputTargetDeregisteredWaitTypeDef,
     DescribeTargetHealthInputTargetInServiceWaitTypeDef,
     DescribeTargetGroupAttributesOutputTypeDef,
     ModifyTargetGroupAttributesInputRequestTypeDef,
     ModifyTargetGroupAttributesOutputTypeDef,
+    ForwardActionConfigOutputTypeDef,
     ForwardActionConfigTypeDef,
+    QueryStringConditionConfigOutputTypeDef,
     QueryStringConditionConfigTypeDef,
     SetRulePrioritiesInputRequestTypeDef,
     TargetHealthDescriptionTypeDef,
     DescribeTagsOutputTypeDef,
     LoadBalancerTypeDef,
     SetSubnetsOutputTypeDef,
     DescribeSSLPoliciesOutputTypeDef,
     CreateTargetGroupOutputTypeDef,
     DescribeTargetGroupsOutputTypeDef,
     ModifyTargetGroupOutputTypeDef,
+    ActionOutputTypeDef,
     ActionTypeDef,
+    RuleConditionOutputTypeDef,
     RuleConditionTypeDef,
     DescribeTargetHealthOutputTypeDef,
     CreateLoadBalancerOutputTypeDef,
     DescribeLoadBalancersOutputTypeDef,
-    CreateListenerInputRequestTypeDef,
     ListenerTypeDef,
-    ModifyListenerInputRequestTypeDef,
-    CreateRuleInputRequestTypeDef,
-    ModifyRuleInputRequestTypeDef,
+    ActionUnionTypeDef,
     RuleTypeDef,
+    RuleConditionUnionTypeDef,
     CreateListenerOutputTypeDef,
     DescribeListenersOutputTypeDef,
     ModifyListenerOutputTypeDef,
+    CreateListenerInputRequestTypeDef,
+    ModifyListenerInputRequestTypeDef,
     CreateRuleOutputTypeDef,
     DescribeRulesOutputTypeDef,
     ModifyRuleOutputTypeDef,
     SetRulePrioritiesOutputTypeDef,
+    CreateRuleInputRequestTypeDef,
+    ModifyRuleInputRequestTypeDef,
 )
 
 
-def get_structure() -> AuthenticateCognitoActionConfigTypeDef:
+def get_value() -> AuthenticateCognitoActionConfigOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-elbv2-2.5.2/README.md` & `types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-elbv2
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ElasticLoadBalancingv2 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore elbv2 type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-elbv2"></a>
 
 # types-aiobotocore-elbv2
 
 [![PyPI - types-aiobotocore-elbv2](https://img.shields.io/pypi/v/types-aiobotocore-elbv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elbv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elbv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elbv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-elbv2?color=blue)](https://pypistats.org/packages/types-aiobotocore-elbv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elbv2)](https://pepy.tech/project/types-aiobotocore-elbv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ElasticLoadBalancingv2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
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
 [types-aiobotocore-elbv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/).
 
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
@@ -361,138 +393,151 @@
 )
 
 
 def check_value(value: ActionTypeEnumType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_elbv2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_elbv2.type_defs import (
-    AuthenticateCognitoActionConfigTypeDef,
-    AuthenticateOidcActionConfigTypeDef,
+    AuthenticateCognitoActionConfigOutputTypeDef,
+    AuthenticateOidcActionConfigOutputTypeDef,
     FixedResponseActionConfigTypeDef,
     RedirectActionConfigTypeDef,
+    AuthenticateCognitoActionConfigTypeDef,
+    AuthenticateOidcActionConfigTypeDef,
     CertificateTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     LoadBalancerAddressTypeDef,
     CipherTypeDef,
     SubnetMappingTypeDef,
     MatcherTypeDef,
     DeleteListenerInputRequestTypeDef,
     DeleteLoadBalancerInputRequestTypeDef,
     DeleteRuleInputRequestTypeDef,
     DeleteTargetGroupInputRequestTypeDef,
     TargetDescriptionTypeDef,
-    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     LimitTypeDef,
-    DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
     DescribeListenerCertificatesInputRequestTypeDef,
-    DescribeListenersInputDescribeListenersPaginateTypeDef,
     DescribeListenersInputRequestTypeDef,
     DescribeLoadBalancerAttributesInputRequestTypeDef,
     LoadBalancerAttributeTypeDef,
-    DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef,
     WaiterConfigTypeDef,
     DescribeLoadBalancersInputRequestTypeDef,
-    DescribeRulesInputDescribeRulesPaginateTypeDef,
     DescribeRulesInputRequestTypeDef,
-    DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef,
     DescribeSSLPoliciesInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
     DescribeTargetGroupAttributesInputRequestTypeDef,
     TargetGroupAttributeTypeDef,
-    DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef,
     DescribeTargetGroupsInputRequestTypeDef,
     TargetGroupStickinessConfigTypeDef,
     TargetGroupTupleTypeDef,
+    HostHeaderConditionConfigOutputTypeDef,
     HostHeaderConditionConfigTypeDef,
+    HttpHeaderConditionConfigOutputTypeDef,
     HttpHeaderConditionConfigTypeDef,
+    HttpRequestMethodConditionConfigOutputTypeDef,
     HttpRequestMethodConditionConfigTypeDef,
     LoadBalancerStateTypeDef,
-    PaginatorConfigTypeDef,
+    PathPatternConditionConfigOutputTypeDef,
     PathPatternConditionConfigTypeDef,
     QueryStringKeyValuePairTypeDef,
     RemoveTagsInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    SourceIpConditionConfigOutputTypeDef,
     SourceIpConditionConfigTypeDef,
     RulePriorityPairTypeDef,
     SetIpAddressTypeInputRequestTypeDef,
-    SetIpAddressTypeOutputTypeDef,
     SetSecurityGroupsInputRequestTypeDef,
-    SetSecurityGroupsOutputTypeDef,
     TargetHealthTypeDef,
     AddListenerCertificatesInputRequestTypeDef,
+    RemoveListenerCertificatesInputRequestTypeDef,
     AddListenerCertificatesOutputTypeDef,
     DescribeListenerCertificatesOutputTypeDef,
-    RemoveListenerCertificatesInputRequestTypeDef,
+    SetIpAddressTypeOutputTypeDef,
+    SetSecurityGroupsOutputTypeDef,
     AddTagsInputRequestTypeDef,
     TagDescriptionTypeDef,
     AvailabilityZoneTypeDef,
     SslPolicyTypeDef,
     CreateLoadBalancerInputRequestTypeDef,
     SetSubnetsInputRequestTypeDef,
     CreateTargetGroupInputRequestTypeDef,
     ModifyTargetGroupInputRequestTypeDef,
     TargetGroupTypeDef,
     DeregisterTargetsInputRequestTypeDef,
     DescribeTargetHealthInputRequestTypeDef,
     RegisterTargetsInputRequestTypeDef,
+    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
+    DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
+    DescribeListenersInputDescribeListenersPaginateTypeDef,
+    DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef,
+    DescribeRulesInputDescribeRulesPaginateTypeDef,
+    DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef,
+    DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef,
     DescribeAccountLimitsOutputTypeDef,
     DescribeLoadBalancerAttributesOutputTypeDef,
     ModifyLoadBalancerAttributesInputRequestTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
     DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef,
     DescribeLoadBalancersInputLoadBalancerExistsWaitTypeDef,
     DescribeLoadBalancersInputLoadBalancersDeletedWaitTypeDef,
     DescribeTargetHealthInputTargetDeregisteredWaitTypeDef,
     DescribeTargetHealthInputTargetInServiceWaitTypeDef,
     DescribeTargetGroupAttributesOutputTypeDef,
     ModifyTargetGroupAttributesInputRequestTypeDef,
     ModifyTargetGroupAttributesOutputTypeDef,
+    ForwardActionConfigOutputTypeDef,
     ForwardActionConfigTypeDef,
+    QueryStringConditionConfigOutputTypeDef,
     QueryStringConditionConfigTypeDef,
     SetRulePrioritiesInputRequestTypeDef,
     TargetHealthDescriptionTypeDef,
     DescribeTagsOutputTypeDef,
     LoadBalancerTypeDef,
     SetSubnetsOutputTypeDef,
     DescribeSSLPoliciesOutputTypeDef,
     CreateTargetGroupOutputTypeDef,
     DescribeTargetGroupsOutputTypeDef,
     ModifyTargetGroupOutputTypeDef,
+    ActionOutputTypeDef,
     ActionTypeDef,
+    RuleConditionOutputTypeDef,
     RuleConditionTypeDef,
     DescribeTargetHealthOutputTypeDef,
     CreateLoadBalancerOutputTypeDef,
     DescribeLoadBalancersOutputTypeDef,
-    CreateListenerInputRequestTypeDef,
     ListenerTypeDef,
-    ModifyListenerInputRequestTypeDef,
-    CreateRuleInputRequestTypeDef,
-    ModifyRuleInputRequestTypeDef,
+    ActionUnionTypeDef,
     RuleTypeDef,
+    RuleConditionUnionTypeDef,
     CreateListenerOutputTypeDef,
     DescribeListenersOutputTypeDef,
     ModifyListenerOutputTypeDef,
+    CreateListenerInputRequestTypeDef,
+    ModifyListenerInputRequestTypeDef,
     CreateRuleOutputTypeDef,
     DescribeRulesOutputTypeDef,
     ModifyRuleOutputTypeDef,
     SetRulePrioritiesOutputTypeDef,
+    CreateRuleInputRequestTypeDef,
+    ModifyRuleInputRequestTypeDef,
 )
 
 
-def get_structure() -> AuthenticateCognitoActionConfigTypeDef:
+def get_value() -> AuthenticateCognitoActionConfigOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-elbv2-2.5.2/setup.py` & `types-aiobotocore-elbv2-2.5.2.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-elbv2",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_elbv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ElasticLoadBalancingv2 2.5.2 service generated with"
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
-    keywords="aiobotocore elbv2 type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore elbv2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_elbv2": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/"
```

### Comparing `types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2/__init__.py` & `types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2/__init__.pyi` & `types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2/__main__.py` & `types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ElasticLoadBalancingv2 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2\nOther"
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

### Comparing `types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2/client.py` & `types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     DescribeListenersPaginator,
     DescribeLoadBalancersPaginator,
     DescribeRulesPaginator,
     DescribeSSLPoliciesPaginator,
     DescribeTargetGroupsPaginator,
 )
 from .type_defs import (
-    ActionTypeDef,
+    ActionUnionTypeDef,
     AddListenerCertificatesOutputTypeDef,
     CertificateTypeDef,
     CreateListenerOutputTypeDef,
     CreateLoadBalancerOutputTypeDef,
     CreateRuleOutputTypeDef,
     CreateTargetGroupOutputTypeDef,
     DescribeAccountLimitsOutputTypeDef,
@@ -59,15 +59,15 @@
     LoadBalancerAttributeTypeDef,
     MatcherTypeDef,
     ModifyListenerOutputTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
     ModifyRuleOutputTypeDef,
     ModifyTargetGroupAttributesOutputTypeDef,
     ModifyTargetGroupOutputTypeDef,
-    RuleConditionTypeDef,
+    RuleConditionUnionTypeDef,
     RulePriorityPairTypeDef,
     SetIpAddressTypeOutputTypeDef,
     SetRulePrioritiesOutputTypeDef,
     SetSecurityGroupsOutputTypeDef,
     SetSubnetsOutputTypeDef,
     SubnetMappingTypeDef,
     TagTypeDef,
@@ -194,15 +194,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#close)
         """
 
     async def create_listener(
         self,
         *,
         LoadBalancerArn: str,
-        DefaultActions: Sequence[ActionTypeDef],
+        DefaultActions: Sequence[ActionUnionTypeDef],
         Protocol: ProtocolEnumType = ...,
         Port: int = ...,
         SslPolicy: str = ...,
         Certificates: Sequence[CertificateTypeDef] = ...,
         AlpnPolicy: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateListenerOutputTypeDef:
@@ -235,17 +235,17 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#create_load_balancer)
         """
 
     async def create_rule(
         self,
         *,
         ListenerArn: str,
-        Conditions: Sequence[RuleConditionTypeDef],
+        Conditions: Sequence[RuleConditionUnionTypeDef],
         Priority: int,
-        Actions: Sequence[ActionTypeDef],
+        Actions: Sequence[ActionUnionTypeDef],
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateRuleOutputTypeDef:
         """
         Creates a rule for the specified listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.create_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#create_rule)
@@ -478,15 +478,15 @@
         self,
         *,
         ListenerArn: str,
         Port: int = ...,
         Protocol: ProtocolEnumType = ...,
         SslPolicy: str = ...,
         Certificates: Sequence[CertificateTypeDef] = ...,
-        DefaultActions: Sequence[ActionTypeDef] = ...,
+        DefaultActions: Sequence[ActionUnionTypeDef] = ...,
         AlpnPolicy: Sequence[str] = ...
     ) -> ModifyListenerOutputTypeDef:
         """
         Replaces the specified properties of the specified listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.modify_listener)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#modify_listener)
@@ -503,16 +503,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#modify_load_balancer_attributes)
         """
 
     async def modify_rule(
         self,
         *,
         RuleArn: str,
-        Conditions: Sequence[RuleConditionTypeDef] = ...,
-        Actions: Sequence[ActionTypeDef] = ...
+        Conditions: Sequence[RuleConditionUnionTypeDef] = ...,
+        Actions: Sequence[ActionUnionTypeDef] = ...
     ) -> ModifyRuleOutputTypeDef:
         """
         Replaces the specified properties of the specified rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.modify_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#modify_rule)
         """
```

### Comparing `types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2/client.pyi` & `types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     DescribeListenersPaginator,
     DescribeLoadBalancersPaginator,
     DescribeRulesPaginator,
     DescribeSSLPoliciesPaginator,
     DescribeTargetGroupsPaginator,
 )
 from .type_defs import (
-    ActionTypeDef,
+    ActionUnionTypeDef,
     AddListenerCertificatesOutputTypeDef,
     CertificateTypeDef,
     CreateListenerOutputTypeDef,
     CreateLoadBalancerOutputTypeDef,
     CreateRuleOutputTypeDef,
     CreateTargetGroupOutputTypeDef,
     DescribeAccountLimitsOutputTypeDef,
@@ -59,15 +59,15 @@
     LoadBalancerAttributeTypeDef,
     MatcherTypeDef,
     ModifyListenerOutputTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
     ModifyRuleOutputTypeDef,
     ModifyTargetGroupAttributesOutputTypeDef,
     ModifyTargetGroupOutputTypeDef,
-    RuleConditionTypeDef,
+    RuleConditionUnionTypeDef,
     RulePriorityPairTypeDef,
     SetIpAddressTypeOutputTypeDef,
     SetRulePrioritiesOutputTypeDef,
     SetSecurityGroupsOutputTypeDef,
     SetSubnetsOutputTypeDef,
     SubnetMappingTypeDef,
     TagTypeDef,
@@ -185,15 +185,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#close)
         """
     async def create_listener(
         self,
         *,
         LoadBalancerArn: str,
-        DefaultActions: Sequence[ActionTypeDef],
+        DefaultActions: Sequence[ActionUnionTypeDef],
         Protocol: ProtocolEnumType = ...,
         Port: int = ...,
         SslPolicy: str = ...,
         Certificates: Sequence[CertificateTypeDef] = ...,
         AlpnPolicy: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateListenerOutputTypeDef:
@@ -224,17 +224,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.create_load_balancer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#create_load_balancer)
         """
     async def create_rule(
         self,
         *,
         ListenerArn: str,
-        Conditions: Sequence[RuleConditionTypeDef],
+        Conditions: Sequence[RuleConditionUnionTypeDef],
         Priority: int,
-        Actions: Sequence[ActionTypeDef],
+        Actions: Sequence[ActionUnionTypeDef],
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateRuleOutputTypeDef:
         """
         Creates a rule for the specified listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.create_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#create_rule)
@@ -448,15 +448,15 @@
         self,
         *,
         ListenerArn: str,
         Port: int = ...,
         Protocol: ProtocolEnumType = ...,
         SslPolicy: str = ...,
         Certificates: Sequence[CertificateTypeDef] = ...,
-        DefaultActions: Sequence[ActionTypeDef] = ...,
+        DefaultActions: Sequence[ActionUnionTypeDef] = ...,
         AlpnPolicy: Sequence[str] = ...
     ) -> ModifyListenerOutputTypeDef:
         """
         Replaces the specified properties of the specified listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.modify_listener)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#modify_listener)
@@ -471,16 +471,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.modify_load_balancer_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#modify_load_balancer_attributes)
         """
     async def modify_rule(
         self,
         *,
         RuleArn: str,
-        Conditions: Sequence[RuleConditionTypeDef] = ...,
-        Actions: Sequence[ActionTypeDef] = ...
+        Conditions: Sequence[RuleConditionUnionTypeDef] = ...,
+        Actions: Sequence[ActionUnionTypeDef] = ...
     ) -> ModifyRuleOutputTypeDef:
         """
         Replaces the specified properties of the specified rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.modify_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#modify_rule)
         """
```

### Comparing `types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2/literals.py` & `types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2/literals.pyi` & `types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2/paginator.py` & `types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -55,142 +55,133 @@
     "DescribeListenersPaginator",
     "DescribeLoadBalancersPaginator",
     "DescribeRulesPaginator",
     "DescribeSSLPoliciesPaginator",
     "DescribeTargetGroupsPaginator",
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
 class DescribeAccountLimitsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeAccountLimits)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describeaccountlimitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAccountLimitsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeAccountLimits.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describeaccountlimitspaginator)
         """
 
-
 class DescribeListenerCertificatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeListenerCertificates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describelistenercertificatespaginator)
     """
 
     def paginate(
-        self, *, ListenerArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ListenerArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeListenerCertificatesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeListenerCertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describelistenercertificatespaginator)
         """
 
-
 class DescribeListenersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeListeners)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describelistenerspaginator)
     """
 
     def paginate(
         self,
         *,
         LoadBalancerArn: str = ...,
         ListenerArns: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeListenersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeListeners.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describelistenerspaginator)
         """
 
-
 class DescribeLoadBalancersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeLoadBalancers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describeloadbalancerspaginator)
     """
 
     def paginate(
         self,
         *,
         LoadBalancerArns: Sequence[str] = ...,
         Names: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeLoadBalancersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeLoadBalancers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describeloadbalancerspaginator)
         """
 
-
 class DescribeRulesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeRules)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describerulespaginator)
     """
 
     def paginate(
         self,
         *,
         ListenerArn: str = ...,
         RuleArns: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeRulesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describerulespaginator)
         """
 
-
 class DescribeSSLPoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeSSLPolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describesslpoliciespaginator)
     """
 
     def paginate(
         self,
         *,
         Names: Sequence[str] = ...,
         LoadBalancerType: LoadBalancerTypeEnumType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeSSLPoliciesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeSSLPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describesslpoliciespaginator)
         """
 
-
 class DescribeTargetGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeTargetGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describetargetgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         LoadBalancerArn: str = ...,
         TargetGroupArns: Sequence[str] = ...,
         Names: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeTargetGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeTargetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describetargetgroupspaginator)
         """
```

### Comparing `types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2/paginator.pyi` & `types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,133 +55,142 @@
     "DescribeListenersPaginator",
     "DescribeLoadBalancersPaginator",
     "DescribeRulesPaginator",
     "DescribeSSLPoliciesPaginator",
     "DescribeTargetGroupsPaginator",
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
 class DescribeAccountLimitsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeAccountLimits)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describeaccountlimitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAccountLimitsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeAccountLimits.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describeaccountlimitspaginator)
         """
 
+
 class DescribeListenerCertificatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeListenerCertificates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describelistenercertificatespaginator)
     """
 
     def paginate(
-        self, *, ListenerArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ListenerArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeListenerCertificatesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeListenerCertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describelistenercertificatespaginator)
         """
 
+
 class DescribeListenersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeListeners)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describelistenerspaginator)
     """
 
     def paginate(
         self,
         *,
         LoadBalancerArn: str = ...,
         ListenerArns: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeListenersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeListeners.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describelistenerspaginator)
         """
 
+
 class DescribeLoadBalancersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeLoadBalancers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describeloadbalancerspaginator)
     """
 
     def paginate(
         self,
         *,
         LoadBalancerArns: Sequence[str] = ...,
         Names: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeLoadBalancersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeLoadBalancers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describeloadbalancerspaginator)
         """
 
+
 class DescribeRulesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeRules)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describerulespaginator)
     """
 
     def paginate(
         self,
         *,
         ListenerArn: str = ...,
         RuleArns: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeRulesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describerulespaginator)
         """
 
+
 class DescribeSSLPoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeSSLPolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describesslpoliciespaginator)
     """
 
     def paginate(
         self,
         *,
         Names: Sequence[str] = ...,
         LoadBalancerType: LoadBalancerTypeEnumType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeSSLPoliciesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeSSLPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describesslpoliciespaginator)
         """
 
+
 class DescribeTargetGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeTargetGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describetargetgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         LoadBalancerArn: str = ...,
         TargetGroupArns: Sequence[str] = ...,
         Names: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeTargetGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeTargetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/paginators/#describetargetgroupspaginator)
         """
```

### Comparing `types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2/type_defs.py` & `types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for elbv2 service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_elbv2.type_defs import AuthenticateCognitoActionConfigTypeDef
+    from types_aiobotocore_elbv2.type_defs import AuthenticateCognitoActionConfigOutputTypeDef
 
-    data: AuthenticateCognitoActionConfigTypeDef = {...}
+    data: AuthenticateCognitoActionConfigOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ActionTypeEnumType,
     AuthenticateCognitoActionConditionalBehaviorEnumType,
     AuthenticateOidcActionConditionalBehaviorEnumType,
     IpAddressTypeType,
     LoadBalancerSchemeEnumType,
@@ -34,181 +34,196 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AuthenticateCognitoActionConfigTypeDef",
-    "AuthenticateOidcActionConfigTypeDef",
+    "AuthenticateCognitoActionConfigOutputTypeDef",
+    "AuthenticateOidcActionConfigOutputTypeDef",
     "FixedResponseActionConfigTypeDef",
     "RedirectActionConfigTypeDef",
+    "AuthenticateCognitoActionConfigTypeDef",
+    "AuthenticateOidcActionConfigTypeDef",
     "CertificateTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "LoadBalancerAddressTypeDef",
     "CipherTypeDef",
     "SubnetMappingTypeDef",
     "MatcherTypeDef",
     "DeleteListenerInputRequestTypeDef",
     "DeleteLoadBalancerInputRequestTypeDef",
     "DeleteRuleInputRequestTypeDef",
     "DeleteTargetGroupInputRequestTypeDef",
     "TargetDescriptionTypeDef",
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAccountLimitsInputRequestTypeDef",
     "LimitTypeDef",
-    "DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
     "DescribeListenerCertificatesInputRequestTypeDef",
-    "DescribeListenersInputDescribeListenersPaginateTypeDef",
     "DescribeListenersInputRequestTypeDef",
     "DescribeLoadBalancerAttributesInputRequestTypeDef",
     "LoadBalancerAttributeTypeDef",
-    "DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef",
     "WaiterConfigTypeDef",
     "DescribeLoadBalancersInputRequestTypeDef",
-    "DescribeRulesInputDescribeRulesPaginateTypeDef",
     "DescribeRulesInputRequestTypeDef",
-    "DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef",
     "DescribeSSLPoliciesInputRequestTypeDef",
     "DescribeTagsInputRequestTypeDef",
     "DescribeTargetGroupAttributesInputRequestTypeDef",
     "TargetGroupAttributeTypeDef",
-    "DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef",
     "DescribeTargetGroupsInputRequestTypeDef",
     "TargetGroupStickinessConfigTypeDef",
     "TargetGroupTupleTypeDef",
+    "HostHeaderConditionConfigOutputTypeDef",
     "HostHeaderConditionConfigTypeDef",
+    "HttpHeaderConditionConfigOutputTypeDef",
     "HttpHeaderConditionConfigTypeDef",
+    "HttpRequestMethodConditionConfigOutputTypeDef",
     "HttpRequestMethodConditionConfigTypeDef",
     "LoadBalancerStateTypeDef",
-    "PaginatorConfigTypeDef",
+    "PathPatternConditionConfigOutputTypeDef",
     "PathPatternConditionConfigTypeDef",
     "QueryStringKeyValuePairTypeDef",
     "RemoveTagsInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "SourceIpConditionConfigOutputTypeDef",
     "SourceIpConditionConfigTypeDef",
     "RulePriorityPairTypeDef",
     "SetIpAddressTypeInputRequestTypeDef",
-    "SetIpAddressTypeOutputTypeDef",
     "SetSecurityGroupsInputRequestTypeDef",
-    "SetSecurityGroupsOutputTypeDef",
     "TargetHealthTypeDef",
     "AddListenerCertificatesInputRequestTypeDef",
+    "RemoveListenerCertificatesInputRequestTypeDef",
     "AddListenerCertificatesOutputTypeDef",
     "DescribeListenerCertificatesOutputTypeDef",
-    "RemoveListenerCertificatesInputRequestTypeDef",
+    "SetIpAddressTypeOutputTypeDef",
+    "SetSecurityGroupsOutputTypeDef",
     "AddTagsInputRequestTypeDef",
     "TagDescriptionTypeDef",
     "AvailabilityZoneTypeDef",
     "SslPolicyTypeDef",
     "CreateLoadBalancerInputRequestTypeDef",
     "SetSubnetsInputRequestTypeDef",
     "CreateTargetGroupInputRequestTypeDef",
     "ModifyTargetGroupInputRequestTypeDef",
     "TargetGroupTypeDef",
     "DeregisterTargetsInputRequestTypeDef",
     "DescribeTargetHealthInputRequestTypeDef",
     "RegisterTargetsInputRequestTypeDef",
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    "DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
+    "DescribeListenersInputDescribeListenersPaginateTypeDef",
+    "DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef",
+    "DescribeRulesInputDescribeRulesPaginateTypeDef",
+    "DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef",
+    "DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef",
     "DescribeAccountLimitsOutputTypeDef",
     "DescribeLoadBalancerAttributesOutputTypeDef",
     "ModifyLoadBalancerAttributesInputRequestTypeDef",
     "ModifyLoadBalancerAttributesOutputTypeDef",
     "DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef",
     "DescribeLoadBalancersInputLoadBalancerExistsWaitTypeDef",
     "DescribeLoadBalancersInputLoadBalancersDeletedWaitTypeDef",
     "DescribeTargetHealthInputTargetDeregisteredWaitTypeDef",
     "DescribeTargetHealthInputTargetInServiceWaitTypeDef",
     "DescribeTargetGroupAttributesOutputTypeDef",
     "ModifyTargetGroupAttributesInputRequestTypeDef",
     "ModifyTargetGroupAttributesOutputTypeDef",
+    "ForwardActionConfigOutputTypeDef",
     "ForwardActionConfigTypeDef",
+    "QueryStringConditionConfigOutputTypeDef",
     "QueryStringConditionConfigTypeDef",
     "SetRulePrioritiesInputRequestTypeDef",
     "TargetHealthDescriptionTypeDef",
     "DescribeTagsOutputTypeDef",
     "LoadBalancerTypeDef",
     "SetSubnetsOutputTypeDef",
     "DescribeSSLPoliciesOutputTypeDef",
     "CreateTargetGroupOutputTypeDef",
     "DescribeTargetGroupsOutputTypeDef",
     "ModifyTargetGroupOutputTypeDef",
+    "ActionOutputTypeDef",
     "ActionTypeDef",
+    "RuleConditionOutputTypeDef",
     "RuleConditionTypeDef",
     "DescribeTargetHealthOutputTypeDef",
     "CreateLoadBalancerOutputTypeDef",
     "DescribeLoadBalancersOutputTypeDef",
-    "CreateListenerInputRequestTypeDef",
     "ListenerTypeDef",
-    "ModifyListenerInputRequestTypeDef",
-    "CreateRuleInputRequestTypeDef",
-    "ModifyRuleInputRequestTypeDef",
+    "ActionUnionTypeDef",
     "RuleTypeDef",
+    "RuleConditionUnionTypeDef",
     "CreateListenerOutputTypeDef",
     "DescribeListenersOutputTypeDef",
     "ModifyListenerOutputTypeDef",
+    "CreateListenerInputRequestTypeDef",
+    "ModifyListenerInputRequestTypeDef",
     "CreateRuleOutputTypeDef",
     "DescribeRulesOutputTypeDef",
     "ModifyRuleOutputTypeDef",
     "SetRulePrioritiesOutputTypeDef",
+    "CreateRuleInputRequestTypeDef",
+    "ModifyRuleInputRequestTypeDef",
 )
 
-_RequiredAuthenticateCognitoActionConfigTypeDef = TypedDict(
-    "_RequiredAuthenticateCognitoActionConfigTypeDef",
+_RequiredAuthenticateCognitoActionConfigOutputTypeDef = TypedDict(
+    "_RequiredAuthenticateCognitoActionConfigOutputTypeDef",
     {
         "UserPoolArn": str,
         "UserPoolClientId": str,
         "UserPoolDomain": str,
     },
 )
-_OptionalAuthenticateCognitoActionConfigTypeDef = TypedDict(
-    "_OptionalAuthenticateCognitoActionConfigTypeDef",
+_OptionalAuthenticateCognitoActionConfigOutputTypeDef = TypedDict(
+    "_OptionalAuthenticateCognitoActionConfigOutputTypeDef",
     {
         "SessionCookieName": str,
         "Scope": str,
         "SessionTimeout": int,
-        "AuthenticationRequestExtraParams": Mapping[str, str],
+        "AuthenticationRequestExtraParams": Dict[str, str],
         "OnUnauthenticatedRequest": AuthenticateCognitoActionConditionalBehaviorEnumType,
     },
     total=False,
 )
 
 
-class AuthenticateCognitoActionConfigTypeDef(
-    _RequiredAuthenticateCognitoActionConfigTypeDef, _OptionalAuthenticateCognitoActionConfigTypeDef
+class AuthenticateCognitoActionConfigOutputTypeDef(
+    _RequiredAuthenticateCognitoActionConfigOutputTypeDef,
+    _OptionalAuthenticateCognitoActionConfigOutputTypeDef,
 ):
     pass
 
 
-_RequiredAuthenticateOidcActionConfigTypeDef = TypedDict(
-    "_RequiredAuthenticateOidcActionConfigTypeDef",
+_RequiredAuthenticateOidcActionConfigOutputTypeDef = TypedDict(
+    "_RequiredAuthenticateOidcActionConfigOutputTypeDef",
     {
         "Issuer": str,
         "AuthorizationEndpoint": str,
         "TokenEndpoint": str,
         "UserInfoEndpoint": str,
         "ClientId": str,
     },
 )
-_OptionalAuthenticateOidcActionConfigTypeDef = TypedDict(
-    "_OptionalAuthenticateOidcActionConfigTypeDef",
+_OptionalAuthenticateOidcActionConfigOutputTypeDef = TypedDict(
+    "_OptionalAuthenticateOidcActionConfigOutputTypeDef",
     {
         "ClientSecret": str,
         "SessionCookieName": str,
         "Scope": str,
         "SessionTimeout": int,
-        "AuthenticationRequestExtraParams": Mapping[str, str],
+        "AuthenticationRequestExtraParams": Dict[str, str],
         "OnUnauthenticatedRequest": AuthenticateOidcActionConditionalBehaviorEnumType,
         "UseExistingClientSecret": bool,
     },
     total=False,
 )
 
 
-class AuthenticateOidcActionConfigTypeDef(
-    _RequiredAuthenticateOidcActionConfigTypeDef, _OptionalAuthenticateOidcActionConfigTypeDef
+class AuthenticateOidcActionConfigOutputTypeDef(
+    _RequiredAuthenticateOidcActionConfigOutputTypeDef,
+    _OptionalAuthenticateOidcActionConfigOutputTypeDef,
 ):
     pass
 
 
 _RequiredFixedResponseActionConfigTypeDef = TypedDict(
     "_RequiredFixedResponseActionConfigTypeDef",
     {
@@ -252,23 +267,92 @@
 
 class RedirectActionConfigTypeDef(
     _RequiredRedirectActionConfigTypeDef, _OptionalRedirectActionConfigTypeDef
 ):
     pass
 
 
+_RequiredAuthenticateCognitoActionConfigTypeDef = TypedDict(
+    "_RequiredAuthenticateCognitoActionConfigTypeDef",
+    {
+        "UserPoolArn": str,
+        "UserPoolClientId": str,
+        "UserPoolDomain": str,
+    },
+)
+_OptionalAuthenticateCognitoActionConfigTypeDef = TypedDict(
+    "_OptionalAuthenticateCognitoActionConfigTypeDef",
+    {
+        "SessionCookieName": str,
+        "Scope": str,
+        "SessionTimeout": int,
+        "AuthenticationRequestExtraParams": Mapping[str, str],
+        "OnUnauthenticatedRequest": AuthenticateCognitoActionConditionalBehaviorEnumType,
+    },
+    total=False,
+)
+
+
+class AuthenticateCognitoActionConfigTypeDef(
+    _RequiredAuthenticateCognitoActionConfigTypeDef, _OptionalAuthenticateCognitoActionConfigTypeDef
+):
+    pass
+
+
+_RequiredAuthenticateOidcActionConfigTypeDef = TypedDict(
+    "_RequiredAuthenticateOidcActionConfigTypeDef",
+    {
+        "Issuer": str,
+        "AuthorizationEndpoint": str,
+        "TokenEndpoint": str,
+        "UserInfoEndpoint": str,
+        "ClientId": str,
+    },
+)
+_OptionalAuthenticateOidcActionConfigTypeDef = TypedDict(
+    "_OptionalAuthenticateOidcActionConfigTypeDef",
+    {
+        "ClientSecret": str,
+        "SessionCookieName": str,
+        "Scope": str,
+        "SessionTimeout": int,
+        "AuthenticationRequestExtraParams": Mapping[str, str],
+        "OnUnauthenticatedRequest": AuthenticateOidcActionConditionalBehaviorEnumType,
+        "UseExistingClientSecret": bool,
+    },
+    total=False,
+)
+
+
+class AuthenticateOidcActionConfigTypeDef(
+    _RequiredAuthenticateOidcActionConfigTypeDef, _OptionalAuthenticateOidcActionConfigTypeDef
+):
+    pass
+
+
 CertificateTypeDef = TypedDict(
     "CertificateTypeDef",
     {
         "CertificateArn": str,
         "IsDefault": bool,
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
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalTagTypeDef = TypedDict(
@@ -370,18 +454,20 @@
 
 class TargetDescriptionTypeDef(
     _RequiredTargetDescriptionTypeDef, _OptionalTargetDescriptionTypeDef
 ):
     pass
 
 
-DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
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
 
 DescribeAccountLimitsInputRequestTypeDef = TypedDict(
     "DescribeAccountLimitsInputRequestTypeDef",
     {
@@ -396,36 +482,14 @@
     {
         "Name": str,
         "Max": str,
     },
     total=False,
 )
 
-_RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
-    {
-        "ListenerArn": str,
-    },
-)
-_OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef(
-    _RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
-    _OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeListenerCertificatesInputRequestTypeDef = TypedDict(
     "_RequiredDescribeListenerCertificatesInputRequestTypeDef",
     {
         "ListenerArn": str,
     },
 )
 _OptionalDescribeListenerCertificatesInputRequestTypeDef = TypedDict(
@@ -441,24 +505,14 @@
 class DescribeListenerCertificatesInputRequestTypeDef(
     _RequiredDescribeListenerCertificatesInputRequestTypeDef,
     _OptionalDescribeListenerCertificatesInputRequestTypeDef,
 ):
     pass
 
 
-DescribeListenersInputDescribeListenersPaginateTypeDef = TypedDict(
-    "DescribeListenersInputDescribeListenersPaginateTypeDef",
-    {
-        "LoadBalancerArn": str,
-        "ListenerArns": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeListenersInputRequestTypeDef = TypedDict(
     "DescribeListenersInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
         "ListenerArns": Sequence[str],
         "Marker": str,
         "PageSize": int,
@@ -478,24 +532,14 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef = TypedDict(
-    "DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef",
-    {
-        "LoadBalancerArns": Sequence[str],
-        "Names": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -508,45 +552,25 @@
         "Names": Sequence[str],
         "Marker": str,
         "PageSize": int,
     },
     total=False,
 )
 
-DescribeRulesInputDescribeRulesPaginateTypeDef = TypedDict(
-    "DescribeRulesInputDescribeRulesPaginateTypeDef",
-    {
-        "ListenerArn": str,
-        "RuleArns": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeRulesInputRequestTypeDef = TypedDict(
     "DescribeRulesInputRequestTypeDef",
     {
         "ListenerArn": str,
         "RuleArns": Sequence[str],
         "Marker": str,
         "PageSize": int,
     },
     total=False,
 )
 
-DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef = TypedDict(
-    "DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef",
-    {
-        "Names": Sequence[str],
-        "LoadBalancerType": LoadBalancerTypeEnumType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeSSLPoliciesInputRequestTypeDef = TypedDict(
     "DescribeSSLPoliciesInputRequestTypeDef",
     {
         "Names": Sequence[str],
         "Marker": str,
         "PageSize": int,
         "LoadBalancerType": LoadBalancerTypeEnumType,
@@ -573,25 +597,14 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef = TypedDict(
-    "DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef",
-    {
-        "LoadBalancerArn": str,
-        "TargetGroupArns": Sequence[str],
-        "Names": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeTargetGroupsInputRequestTypeDef = TypedDict(
     "DescribeTargetGroupsInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
         "TargetGroupArns": Sequence[str],
         "Names": Sequence[str],
         "Marker": str,
@@ -614,31 +627,56 @@
     {
         "TargetGroupArn": str,
         "Weight": int,
     },
     total=False,
 )
 
+HostHeaderConditionConfigOutputTypeDef = TypedDict(
+    "HostHeaderConditionConfigOutputTypeDef",
+    {
+        "Values": List[str],
+    },
+    total=False,
+)
+
 HostHeaderConditionConfigTypeDef = TypedDict(
     "HostHeaderConditionConfigTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
 
+HttpHeaderConditionConfigOutputTypeDef = TypedDict(
+    "HttpHeaderConditionConfigOutputTypeDef",
+    {
+        "HttpHeaderName": str,
+        "Values": List[str],
+    },
+    total=False,
+)
+
 HttpHeaderConditionConfigTypeDef = TypedDict(
     "HttpHeaderConditionConfigTypeDef",
     {
         "HttpHeaderName": str,
         "Values": Sequence[str],
     },
     total=False,
 )
 
+HttpRequestMethodConditionConfigOutputTypeDef = TypedDict(
+    "HttpRequestMethodConditionConfigOutputTypeDef",
+    {
+        "Values": List[str],
+    },
+    total=False,
+)
+
 HttpRequestMethodConditionConfigTypeDef = TypedDict(
     "HttpRequestMethodConditionConfigTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
@@ -648,20 +686,18 @@
     {
         "Code": LoadBalancerStateEnumType,
         "Reason": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+PathPatternConditionConfigOutputTypeDef = TypedDict(
+    "PathPatternConditionConfigOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Values": List[str],
     },
     total=False,
 )
 
 PathPatternConditionConfigTypeDef = TypedDict(
     "PathPatternConditionConfigTypeDef",
     {
@@ -683,23 +719,20 @@
     "RemoveTagsInputRequestTypeDef",
     {
         "ResourceArns": Sequence[str],
         "TagKeys": Sequence[str],
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+SourceIpConditionConfigOutputTypeDef = TypedDict(
+    "SourceIpConditionConfigOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Values": List[str],
     },
+    total=False,
 )
 
 SourceIpConditionConfigTypeDef = TypedDict(
     "SourceIpConditionConfigTypeDef",
     {
         "Values": Sequence[str],
     },
@@ -719,38 +752,22 @@
     "SetIpAddressTypeInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
         "IpAddressType": IpAddressTypeType,
     },
 )
 
-SetIpAddressTypeOutputTypeDef = TypedDict(
-    "SetIpAddressTypeOutputTypeDef",
-    {
-        "IpAddressType": IpAddressTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetSecurityGroupsInputRequestTypeDef = TypedDict(
     "SetSecurityGroupsInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
         "SecurityGroups": Sequence[str],
     },
 )
 
-SetSecurityGroupsOutputTypeDef = TypedDict(
-    "SetSecurityGroupsOutputTypeDef",
-    {
-        "SecurityGroupIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TargetHealthTypeDef = TypedDict(
     "TargetHealthTypeDef",
     {
         "State": TargetHealthStateEnumType,
         "Reason": TargetHealthReasonEnumType,
         "Description": str,
     },
@@ -761,36 +778,52 @@
     "AddListenerCertificatesInputRequestTypeDef",
     {
         "ListenerArn": str,
         "Certificates": Sequence[CertificateTypeDef],
     },
 )
 
+RemoveListenerCertificatesInputRequestTypeDef = TypedDict(
+    "RemoveListenerCertificatesInputRequestTypeDef",
+    {
+        "ListenerArn": str,
+        "Certificates": Sequence[CertificateTypeDef],
+    },
+)
+
 AddListenerCertificatesOutputTypeDef = TypedDict(
     "AddListenerCertificatesOutputTypeDef",
     {
         "Certificates": List[CertificateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeListenerCertificatesOutputTypeDef = TypedDict(
     "DescribeListenerCertificatesOutputTypeDef",
     {
         "Certificates": List[CertificateTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RemoveListenerCertificatesInputRequestTypeDef = TypedDict(
-    "RemoveListenerCertificatesInputRequestTypeDef",
+SetIpAddressTypeOutputTypeDef = TypedDict(
+    "SetIpAddressTypeOutputTypeDef",
     {
-        "ListenerArn": str,
-        "Certificates": Sequence[CertificateTypeDef],
+        "IpAddressType": IpAddressTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetSecurityGroupsOutputTypeDef = TypedDict(
+    "SetSecurityGroupsOutputTypeDef",
+    {
+        "SecurityGroupIds": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddTagsInputRequestTypeDef = TypedDict(
     "AddTagsInputRequestTypeDef",
     {
         "ResourceArns": Sequence[str],
@@ -1004,28 +1037,109 @@
     "RegisterTargetsInputRequestTypeDef",
     {
         "TargetGroupArn": str,
         "Targets": Sequence[TargetDescriptionTypeDef],
     },
 )
 
+DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
+    {
+        "ListenerArn": str,
+    },
+)
+_OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef(
+    _RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
+    _OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
+):
+    pass
+
+
+DescribeListenersInputDescribeListenersPaginateTypeDef = TypedDict(
+    "DescribeListenersInputDescribeListenersPaginateTypeDef",
+    {
+        "LoadBalancerArn": str,
+        "ListenerArns": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef = TypedDict(
+    "DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef",
+    {
+        "LoadBalancerArns": Sequence[str],
+        "Names": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeRulesInputDescribeRulesPaginateTypeDef = TypedDict(
+    "DescribeRulesInputDescribeRulesPaginateTypeDef",
+    {
+        "ListenerArn": str,
+        "RuleArns": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef = TypedDict(
+    "DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef",
+    {
+        "Names": Sequence[str],
+        "LoadBalancerType": LoadBalancerTypeEnumType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef = TypedDict(
+    "DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef",
+    {
+        "LoadBalancerArn": str,
+        "TargetGroupArns": Sequence[str],
+        "Names": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeAccountLimitsOutputTypeDef = TypedDict(
     "DescribeAccountLimitsOutputTypeDef",
     {
         "Limits": List[LimitTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLoadBalancerAttributesOutputTypeDef = TypedDict(
     "DescribeLoadBalancerAttributesOutputTypeDef",
     {
         "Attributes": List[LoadBalancerAttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyLoadBalancerAttributesInputRequestTypeDef = TypedDict(
     "ModifyLoadBalancerAttributesInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
@@ -1033,15 +1147,15 @@
     },
 )
 
 ModifyLoadBalancerAttributesOutputTypeDef = TypedDict(
     "ModifyLoadBalancerAttributesOutputTypeDef",
     {
         "Attributes": List[LoadBalancerAttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef = TypedDict(
     "DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef",
     {
         "LoadBalancerArns": Sequence[str],
@@ -1123,15 +1237,15 @@
     pass
 
 
 DescribeTargetGroupAttributesOutputTypeDef = TypedDict(
     "DescribeTargetGroupAttributesOutputTypeDef",
     {
         "Attributes": List[TargetGroupAttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyTargetGroupAttributesInputRequestTypeDef = TypedDict(
     "ModifyTargetGroupAttributesInputRequestTypeDef",
     {
         "TargetGroupArn": str,
@@ -1139,27 +1253,44 @@
     },
 )
 
 ModifyTargetGroupAttributesOutputTypeDef = TypedDict(
     "ModifyTargetGroupAttributesOutputTypeDef",
     {
         "Attributes": List[TargetGroupAttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ForwardActionConfigOutputTypeDef = TypedDict(
+    "ForwardActionConfigOutputTypeDef",
+    {
+        "TargetGroups": List[TargetGroupTupleTypeDef],
+        "TargetGroupStickinessConfig": TargetGroupStickinessConfigTypeDef,
+    },
+    total=False,
+)
+
 ForwardActionConfigTypeDef = TypedDict(
     "ForwardActionConfigTypeDef",
     {
         "TargetGroups": Sequence[TargetGroupTupleTypeDef],
         "TargetGroupStickinessConfig": TargetGroupStickinessConfigTypeDef,
     },
     total=False,
 )
 
+QueryStringConditionConfigOutputTypeDef = TypedDict(
+    "QueryStringConditionConfigOutputTypeDef",
+    {
+        "Values": List[QueryStringKeyValuePairTypeDef],
+    },
+    total=False,
+)
+
 QueryStringConditionConfigTypeDef = TypedDict(
     "QueryStringConditionConfigTypeDef",
     {
         "Values": Sequence[QueryStringKeyValuePairTypeDef],
     },
     total=False,
 )
@@ -1181,15 +1312,15 @@
     total=False,
 )
 
 DescribeTagsOutputTypeDef = TypedDict(
     "DescribeTagsOutputTypeDef",
     {
         "TagDescriptions": List[TagDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LoadBalancerTypeDef = TypedDict(
     "LoadBalancerTypeDef",
     {
         "LoadBalancerArn": str,
@@ -1210,51 +1341,76 @@
 )
 
 SetSubnetsOutputTypeDef = TypedDict(
     "SetSubnetsOutputTypeDef",
     {
         "AvailabilityZones": List[AvailabilityZoneTypeDef],
         "IpAddressType": IpAddressTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSSLPoliciesOutputTypeDef = TypedDict(
     "DescribeSSLPoliciesOutputTypeDef",
     {
         "SslPolicies": List[SslPolicyTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTargetGroupOutputTypeDef = TypedDict(
     "CreateTargetGroupOutputTypeDef",
     {
         "TargetGroups": List[TargetGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTargetGroupsOutputTypeDef = TypedDict(
     "DescribeTargetGroupsOutputTypeDef",
     {
         "TargetGroups": List[TargetGroupTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyTargetGroupOutputTypeDef = TypedDict(
     "ModifyTargetGroupOutputTypeDef",
     {
         "TargetGroups": List[TargetGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredActionOutputTypeDef = TypedDict(
+    "_RequiredActionOutputTypeDef",
+    {
+        "Type": ActionTypeEnumType,
     },
 )
+_OptionalActionOutputTypeDef = TypedDict(
+    "_OptionalActionOutputTypeDef",
+    {
+        "TargetGroupArn": str,
+        "AuthenticateOidcConfig": AuthenticateOidcActionConfigOutputTypeDef,
+        "AuthenticateCognitoConfig": AuthenticateCognitoActionConfigOutputTypeDef,
+        "Order": int,
+        "RedirectConfig": RedirectActionConfigTypeDef,
+        "FixedResponseConfig": FixedResponseActionConfigTypeDef,
+        "ForwardConfig": ForwardActionConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class ActionOutputTypeDef(_RequiredActionOutputTypeDef, _OptionalActionOutputTypeDef):
+    pass
+
 
 _RequiredActionTypeDef = TypedDict(
     "_RequiredActionTypeDef",
     {
         "Type": ActionTypeEnumType,
     },
 )
@@ -1273,14 +1429,29 @@
 )
 
 
 class ActionTypeDef(_RequiredActionTypeDef, _OptionalActionTypeDef):
     pass
 
 
+RuleConditionOutputTypeDef = TypedDict(
+    "RuleConditionOutputTypeDef",
+    {
+        "Field": str,
+        "Values": List[str],
+        "HostHeaderConfig": HostHeaderConditionConfigOutputTypeDef,
+        "PathPatternConfig": PathPatternConditionConfigOutputTypeDef,
+        "HttpHeaderConfig": HttpHeaderConditionConfigOutputTypeDef,
+        "QueryStringConfig": QueryStringConditionConfigOutputTypeDef,
+        "HttpRequestMethodConfig": HttpRequestMethodConditionConfigOutputTypeDef,
+        "SourceIpConfig": SourceIpConditionConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 RuleConditionTypeDef = TypedDict(
     "RuleConditionTypeDef",
     {
         "Field": str,
         "Values": Sequence[str],
         "HostHeaderConfig": HostHeaderConditionConfigTypeDef,
         "PathPatternConfig": PathPatternConditionConfigTypeDef,
@@ -1292,40 +1463,94 @@
     total=False,
 )
 
 DescribeTargetHealthOutputTypeDef = TypedDict(
     "DescribeTargetHealthOutputTypeDef",
     {
         "TargetHealthDescriptions": List[TargetHealthDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateLoadBalancerOutputTypeDef = TypedDict(
     "CreateLoadBalancerOutputTypeDef",
     {
         "LoadBalancers": List[LoadBalancerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLoadBalancersOutputTypeDef = TypedDict(
     "DescribeLoadBalancersOutputTypeDef",
     {
         "LoadBalancers": List[LoadBalancerTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListenerTypeDef = TypedDict(
+    "ListenerTypeDef",
+    {
+        "ListenerArn": str,
+        "LoadBalancerArn": str,
+        "Port": int,
+        "Protocol": ProtocolEnumType,
+        "Certificates": List[CertificateTypeDef],
+        "SslPolicy": str,
+        "DefaultActions": List[ActionOutputTypeDef],
+        "AlpnPolicy": List[str],
+    },
+    total=False,
+)
+
+ActionUnionTypeDef = Union[ActionTypeDef, ActionOutputTypeDef]
+RuleTypeDef = TypedDict(
+    "RuleTypeDef",
+    {
+        "RuleArn": str,
+        "Priority": str,
+        "Conditions": List[RuleConditionOutputTypeDef],
+        "Actions": List[ActionOutputTypeDef],
+        "IsDefault": bool,
+    },
+    total=False,
+)
+
+RuleConditionUnionTypeDef = Union[RuleConditionTypeDef, RuleConditionOutputTypeDef]
+CreateListenerOutputTypeDef = TypedDict(
+    "CreateListenerOutputTypeDef",
+    {
+        "Listeners": List[ListenerTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeListenersOutputTypeDef = TypedDict(
+    "DescribeListenersOutputTypeDef",
+    {
+        "Listeners": List[ListenerTypeDef],
+        "NextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyListenerOutputTypeDef = TypedDict(
+    "ModifyListenerOutputTypeDef",
+    {
+        "Listeners": List[ListenerTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateListenerInputRequestTypeDef = TypedDict(
     "_RequiredCreateListenerInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
-        "DefaultActions": Sequence[ActionTypeDef],
+        "DefaultActions": Sequence[ActionUnionTypeDef],
     },
 )
 _OptionalCreateListenerInputRequestTypeDef = TypedDict(
     "_OptionalCreateListenerInputRequestTypeDef",
     {
         "Protocol": ProtocolEnumType,
         "Port": int,
@@ -1340,62 +1565,80 @@
 
 class CreateListenerInputRequestTypeDef(
     _RequiredCreateListenerInputRequestTypeDef, _OptionalCreateListenerInputRequestTypeDef
 ):
     pass
 
 
-ListenerTypeDef = TypedDict(
-    "ListenerTypeDef",
-    {
-        "ListenerArn": str,
-        "LoadBalancerArn": str,
-        "Port": int,
-        "Protocol": ProtocolEnumType,
-        "Certificates": List[CertificateTypeDef],
-        "SslPolicy": str,
-        "DefaultActions": List[ActionTypeDef],
-        "AlpnPolicy": List[str],
-    },
-    total=False,
-)
-
 _RequiredModifyListenerInputRequestTypeDef = TypedDict(
     "_RequiredModifyListenerInputRequestTypeDef",
     {
         "ListenerArn": str,
     },
 )
 _OptionalModifyListenerInputRequestTypeDef = TypedDict(
     "_OptionalModifyListenerInputRequestTypeDef",
     {
         "Port": int,
         "Protocol": ProtocolEnumType,
         "SslPolicy": str,
         "Certificates": Sequence[CertificateTypeDef],
-        "DefaultActions": Sequence[ActionTypeDef],
+        "DefaultActions": Sequence[ActionUnionTypeDef],
         "AlpnPolicy": Sequence[str],
     },
     total=False,
 )
 
 
 class ModifyListenerInputRequestTypeDef(
     _RequiredModifyListenerInputRequestTypeDef, _OptionalModifyListenerInputRequestTypeDef
 ):
     pass
 
 
+CreateRuleOutputTypeDef = TypedDict(
+    "CreateRuleOutputTypeDef",
+    {
+        "Rules": List[RuleTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeRulesOutputTypeDef = TypedDict(
+    "DescribeRulesOutputTypeDef",
+    {
+        "Rules": List[RuleTypeDef],
+        "NextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyRuleOutputTypeDef = TypedDict(
+    "ModifyRuleOutputTypeDef",
+    {
+        "Rules": List[RuleTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetRulePrioritiesOutputTypeDef = TypedDict(
+    "SetRulePrioritiesOutputTypeDef",
+    {
+        "Rules": List[RuleTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateRuleInputRequestTypeDef = TypedDict(
     "_RequiredCreateRuleInputRequestTypeDef",
     {
         "ListenerArn": str,
-        "Conditions": Sequence[RuleConditionTypeDef],
+        "Conditions": Sequence[RuleConditionUnionTypeDef],
         "Priority": int,
-        "Actions": Sequence[ActionTypeDef],
+        "Actions": Sequence[ActionUnionTypeDef],
     },
 )
 _OptionalCreateRuleInputRequestTypeDef = TypedDict(
     "_OptionalCreateRuleInputRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
@@ -1414,89 +1657,18 @@
     {
         "RuleArn": str,
     },
 )
 _OptionalModifyRuleInputRequestTypeDef = TypedDict(
     "_OptionalModifyRuleInputRequestTypeDef",
     {
-        "Conditions": Sequence[RuleConditionTypeDef],
-        "Actions": Sequence[ActionTypeDef],
+        "Conditions": Sequence[RuleConditionUnionTypeDef],
+        "Actions": Sequence[ActionUnionTypeDef],
     },
     total=False,
 )
 
 
 class ModifyRuleInputRequestTypeDef(
     _RequiredModifyRuleInputRequestTypeDef, _OptionalModifyRuleInputRequestTypeDef
 ):
     pass
-
-
-RuleTypeDef = TypedDict(
-    "RuleTypeDef",
-    {
-        "RuleArn": str,
-        "Priority": str,
-        "Conditions": List[RuleConditionTypeDef],
-        "Actions": List[ActionTypeDef],
-        "IsDefault": bool,
-    },
-    total=False,
-)
-
-CreateListenerOutputTypeDef = TypedDict(
-    "CreateListenerOutputTypeDef",
-    {
-        "Listeners": List[ListenerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeListenersOutputTypeDef = TypedDict(
-    "DescribeListenersOutputTypeDef",
-    {
-        "Listeners": List[ListenerTypeDef],
-        "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ModifyListenerOutputTypeDef = TypedDict(
-    "ModifyListenerOutputTypeDef",
-    {
-        "Listeners": List[ListenerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateRuleOutputTypeDef = TypedDict(
-    "CreateRuleOutputTypeDef",
-    {
-        "Rules": List[RuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeRulesOutputTypeDef = TypedDict(
-    "DescribeRulesOutputTypeDef",
-    {
-        "Rules": List[RuleTypeDef],
-        "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ModifyRuleOutputTypeDef = TypedDict(
-    "ModifyRuleOutputTypeDef",
-    {
-        "Rules": List[RuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SetRulePrioritiesOutputTypeDef = TypedDict(
-    "SetRulePrioritiesOutputTypeDef",
-    {
-        "Rules": List[RuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2/type_defs.pyi` & `types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for elbv2 service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_elbv2.type_defs import AuthenticateCognitoActionConfigTypeDef
+    from types_aiobotocore_elbv2.type_defs import AuthenticateCognitoActionConfigOutputTypeDef
 
-    data: AuthenticateCognitoActionConfigTypeDef = {...}
+    data: AuthenticateCognitoActionConfigOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ActionTypeEnumType,
     AuthenticateCognitoActionConditionalBehaviorEnumType,
     AuthenticateOidcActionConditionalBehaviorEnumType,
     IpAddressTypeType,
     LoadBalancerSchemeEnumType,
@@ -33,178 +33,193 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AuthenticateCognitoActionConfigTypeDef",
-    "AuthenticateOidcActionConfigTypeDef",
+    "AuthenticateCognitoActionConfigOutputTypeDef",
+    "AuthenticateOidcActionConfigOutputTypeDef",
     "FixedResponseActionConfigTypeDef",
     "RedirectActionConfigTypeDef",
+    "AuthenticateCognitoActionConfigTypeDef",
+    "AuthenticateOidcActionConfigTypeDef",
     "CertificateTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "LoadBalancerAddressTypeDef",
     "CipherTypeDef",
     "SubnetMappingTypeDef",
     "MatcherTypeDef",
     "DeleteListenerInputRequestTypeDef",
     "DeleteLoadBalancerInputRequestTypeDef",
     "DeleteRuleInputRequestTypeDef",
     "DeleteTargetGroupInputRequestTypeDef",
     "TargetDescriptionTypeDef",
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAccountLimitsInputRequestTypeDef",
     "LimitTypeDef",
-    "DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
     "DescribeListenerCertificatesInputRequestTypeDef",
-    "DescribeListenersInputDescribeListenersPaginateTypeDef",
     "DescribeListenersInputRequestTypeDef",
     "DescribeLoadBalancerAttributesInputRequestTypeDef",
     "LoadBalancerAttributeTypeDef",
-    "DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef",
     "WaiterConfigTypeDef",
     "DescribeLoadBalancersInputRequestTypeDef",
-    "DescribeRulesInputDescribeRulesPaginateTypeDef",
     "DescribeRulesInputRequestTypeDef",
-    "DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef",
     "DescribeSSLPoliciesInputRequestTypeDef",
     "DescribeTagsInputRequestTypeDef",
     "DescribeTargetGroupAttributesInputRequestTypeDef",
     "TargetGroupAttributeTypeDef",
-    "DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef",
     "DescribeTargetGroupsInputRequestTypeDef",
     "TargetGroupStickinessConfigTypeDef",
     "TargetGroupTupleTypeDef",
+    "HostHeaderConditionConfigOutputTypeDef",
     "HostHeaderConditionConfigTypeDef",
+    "HttpHeaderConditionConfigOutputTypeDef",
     "HttpHeaderConditionConfigTypeDef",
+    "HttpRequestMethodConditionConfigOutputTypeDef",
     "HttpRequestMethodConditionConfigTypeDef",
     "LoadBalancerStateTypeDef",
-    "PaginatorConfigTypeDef",
+    "PathPatternConditionConfigOutputTypeDef",
     "PathPatternConditionConfigTypeDef",
     "QueryStringKeyValuePairTypeDef",
     "RemoveTagsInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "SourceIpConditionConfigOutputTypeDef",
     "SourceIpConditionConfigTypeDef",
     "RulePriorityPairTypeDef",
     "SetIpAddressTypeInputRequestTypeDef",
-    "SetIpAddressTypeOutputTypeDef",
     "SetSecurityGroupsInputRequestTypeDef",
-    "SetSecurityGroupsOutputTypeDef",
     "TargetHealthTypeDef",
     "AddListenerCertificatesInputRequestTypeDef",
+    "RemoveListenerCertificatesInputRequestTypeDef",
     "AddListenerCertificatesOutputTypeDef",
     "DescribeListenerCertificatesOutputTypeDef",
-    "RemoveListenerCertificatesInputRequestTypeDef",
+    "SetIpAddressTypeOutputTypeDef",
+    "SetSecurityGroupsOutputTypeDef",
     "AddTagsInputRequestTypeDef",
     "TagDescriptionTypeDef",
     "AvailabilityZoneTypeDef",
     "SslPolicyTypeDef",
     "CreateLoadBalancerInputRequestTypeDef",
     "SetSubnetsInputRequestTypeDef",
     "CreateTargetGroupInputRequestTypeDef",
     "ModifyTargetGroupInputRequestTypeDef",
     "TargetGroupTypeDef",
     "DeregisterTargetsInputRequestTypeDef",
     "DescribeTargetHealthInputRequestTypeDef",
     "RegisterTargetsInputRequestTypeDef",
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    "DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
+    "DescribeListenersInputDescribeListenersPaginateTypeDef",
+    "DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef",
+    "DescribeRulesInputDescribeRulesPaginateTypeDef",
+    "DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef",
+    "DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef",
     "DescribeAccountLimitsOutputTypeDef",
     "DescribeLoadBalancerAttributesOutputTypeDef",
     "ModifyLoadBalancerAttributesInputRequestTypeDef",
     "ModifyLoadBalancerAttributesOutputTypeDef",
     "DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef",
     "DescribeLoadBalancersInputLoadBalancerExistsWaitTypeDef",
     "DescribeLoadBalancersInputLoadBalancersDeletedWaitTypeDef",
     "DescribeTargetHealthInputTargetDeregisteredWaitTypeDef",
     "DescribeTargetHealthInputTargetInServiceWaitTypeDef",
     "DescribeTargetGroupAttributesOutputTypeDef",
     "ModifyTargetGroupAttributesInputRequestTypeDef",
     "ModifyTargetGroupAttributesOutputTypeDef",
+    "ForwardActionConfigOutputTypeDef",
     "ForwardActionConfigTypeDef",
+    "QueryStringConditionConfigOutputTypeDef",
     "QueryStringConditionConfigTypeDef",
     "SetRulePrioritiesInputRequestTypeDef",
     "TargetHealthDescriptionTypeDef",
     "DescribeTagsOutputTypeDef",
     "LoadBalancerTypeDef",
     "SetSubnetsOutputTypeDef",
     "DescribeSSLPoliciesOutputTypeDef",
     "CreateTargetGroupOutputTypeDef",
     "DescribeTargetGroupsOutputTypeDef",
     "ModifyTargetGroupOutputTypeDef",
+    "ActionOutputTypeDef",
     "ActionTypeDef",
+    "RuleConditionOutputTypeDef",
     "RuleConditionTypeDef",
     "DescribeTargetHealthOutputTypeDef",
     "CreateLoadBalancerOutputTypeDef",
     "DescribeLoadBalancersOutputTypeDef",
-    "CreateListenerInputRequestTypeDef",
     "ListenerTypeDef",
-    "ModifyListenerInputRequestTypeDef",
-    "CreateRuleInputRequestTypeDef",
-    "ModifyRuleInputRequestTypeDef",
+    "ActionUnionTypeDef",
     "RuleTypeDef",
+    "RuleConditionUnionTypeDef",
     "CreateListenerOutputTypeDef",
     "DescribeListenersOutputTypeDef",
     "ModifyListenerOutputTypeDef",
+    "CreateListenerInputRequestTypeDef",
+    "ModifyListenerInputRequestTypeDef",
     "CreateRuleOutputTypeDef",
     "DescribeRulesOutputTypeDef",
     "ModifyRuleOutputTypeDef",
     "SetRulePrioritiesOutputTypeDef",
+    "CreateRuleInputRequestTypeDef",
+    "ModifyRuleInputRequestTypeDef",
 )
 
-_RequiredAuthenticateCognitoActionConfigTypeDef = TypedDict(
-    "_RequiredAuthenticateCognitoActionConfigTypeDef",
+_RequiredAuthenticateCognitoActionConfigOutputTypeDef = TypedDict(
+    "_RequiredAuthenticateCognitoActionConfigOutputTypeDef",
     {
         "UserPoolArn": str,
         "UserPoolClientId": str,
         "UserPoolDomain": str,
     },
 )
-_OptionalAuthenticateCognitoActionConfigTypeDef = TypedDict(
-    "_OptionalAuthenticateCognitoActionConfigTypeDef",
+_OptionalAuthenticateCognitoActionConfigOutputTypeDef = TypedDict(
+    "_OptionalAuthenticateCognitoActionConfigOutputTypeDef",
     {
         "SessionCookieName": str,
         "Scope": str,
         "SessionTimeout": int,
-        "AuthenticationRequestExtraParams": Mapping[str, str],
+        "AuthenticationRequestExtraParams": Dict[str, str],
         "OnUnauthenticatedRequest": AuthenticateCognitoActionConditionalBehaviorEnumType,
     },
     total=False,
 )
 
-class AuthenticateCognitoActionConfigTypeDef(
-    _RequiredAuthenticateCognitoActionConfigTypeDef, _OptionalAuthenticateCognitoActionConfigTypeDef
+class AuthenticateCognitoActionConfigOutputTypeDef(
+    _RequiredAuthenticateCognitoActionConfigOutputTypeDef,
+    _OptionalAuthenticateCognitoActionConfigOutputTypeDef,
 ):
     pass
 
-_RequiredAuthenticateOidcActionConfigTypeDef = TypedDict(
-    "_RequiredAuthenticateOidcActionConfigTypeDef",
+_RequiredAuthenticateOidcActionConfigOutputTypeDef = TypedDict(
+    "_RequiredAuthenticateOidcActionConfigOutputTypeDef",
     {
         "Issuer": str,
         "AuthorizationEndpoint": str,
         "TokenEndpoint": str,
         "UserInfoEndpoint": str,
         "ClientId": str,
     },
 )
-_OptionalAuthenticateOidcActionConfigTypeDef = TypedDict(
-    "_OptionalAuthenticateOidcActionConfigTypeDef",
+_OptionalAuthenticateOidcActionConfigOutputTypeDef = TypedDict(
+    "_OptionalAuthenticateOidcActionConfigOutputTypeDef",
     {
         "ClientSecret": str,
         "SessionCookieName": str,
         "Scope": str,
         "SessionTimeout": int,
-        "AuthenticationRequestExtraParams": Mapping[str, str],
+        "AuthenticationRequestExtraParams": Dict[str, str],
         "OnUnauthenticatedRequest": AuthenticateOidcActionConditionalBehaviorEnumType,
         "UseExistingClientSecret": bool,
     },
     total=False,
 )
 
-class AuthenticateOidcActionConfigTypeDef(
-    _RequiredAuthenticateOidcActionConfigTypeDef, _OptionalAuthenticateOidcActionConfigTypeDef
+class AuthenticateOidcActionConfigOutputTypeDef(
+    _RequiredAuthenticateOidcActionConfigOutputTypeDef,
+    _OptionalAuthenticateOidcActionConfigOutputTypeDef,
 ):
     pass
 
 _RequiredFixedResponseActionConfigTypeDef = TypedDict(
     "_RequiredFixedResponseActionConfigTypeDef",
     {
         "StatusCode": str,
@@ -243,23 +258,88 @@
 )
 
 class RedirectActionConfigTypeDef(
     _RequiredRedirectActionConfigTypeDef, _OptionalRedirectActionConfigTypeDef
 ):
     pass
 
+_RequiredAuthenticateCognitoActionConfigTypeDef = TypedDict(
+    "_RequiredAuthenticateCognitoActionConfigTypeDef",
+    {
+        "UserPoolArn": str,
+        "UserPoolClientId": str,
+        "UserPoolDomain": str,
+    },
+)
+_OptionalAuthenticateCognitoActionConfigTypeDef = TypedDict(
+    "_OptionalAuthenticateCognitoActionConfigTypeDef",
+    {
+        "SessionCookieName": str,
+        "Scope": str,
+        "SessionTimeout": int,
+        "AuthenticationRequestExtraParams": Mapping[str, str],
+        "OnUnauthenticatedRequest": AuthenticateCognitoActionConditionalBehaviorEnumType,
+    },
+    total=False,
+)
+
+class AuthenticateCognitoActionConfigTypeDef(
+    _RequiredAuthenticateCognitoActionConfigTypeDef, _OptionalAuthenticateCognitoActionConfigTypeDef
+):
+    pass
+
+_RequiredAuthenticateOidcActionConfigTypeDef = TypedDict(
+    "_RequiredAuthenticateOidcActionConfigTypeDef",
+    {
+        "Issuer": str,
+        "AuthorizationEndpoint": str,
+        "TokenEndpoint": str,
+        "UserInfoEndpoint": str,
+        "ClientId": str,
+    },
+)
+_OptionalAuthenticateOidcActionConfigTypeDef = TypedDict(
+    "_OptionalAuthenticateOidcActionConfigTypeDef",
+    {
+        "ClientSecret": str,
+        "SessionCookieName": str,
+        "Scope": str,
+        "SessionTimeout": int,
+        "AuthenticationRequestExtraParams": Mapping[str, str],
+        "OnUnauthenticatedRequest": AuthenticateOidcActionConditionalBehaviorEnumType,
+        "UseExistingClientSecret": bool,
+    },
+    total=False,
+)
+
+class AuthenticateOidcActionConfigTypeDef(
+    _RequiredAuthenticateOidcActionConfigTypeDef, _OptionalAuthenticateOidcActionConfigTypeDef
+):
+    pass
+
 CertificateTypeDef = TypedDict(
     "CertificateTypeDef",
     {
         "CertificateArn": str,
         "IsDefault": bool,
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
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalTagTypeDef = TypedDict(
@@ -357,18 +437,20 @@
 )
 
 class TargetDescriptionTypeDef(
     _RequiredTargetDescriptionTypeDef, _OptionalTargetDescriptionTypeDef
 ):
     pass
 
-DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
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
 
 DescribeAccountLimitsInputRequestTypeDef = TypedDict(
     "DescribeAccountLimitsInputRequestTypeDef",
     {
@@ -383,34 +465,14 @@
     {
         "Name": str,
         "Max": str,
     },
     total=False,
 )
 
-_RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
-    {
-        "ListenerArn": str,
-    },
-)
-_OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef(
-    _RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
-    _OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeListenerCertificatesInputRequestTypeDef = TypedDict(
     "_RequiredDescribeListenerCertificatesInputRequestTypeDef",
     {
         "ListenerArn": str,
     },
 )
 _OptionalDescribeListenerCertificatesInputRequestTypeDef = TypedDict(
@@ -424,24 +486,14 @@
 
 class DescribeListenerCertificatesInputRequestTypeDef(
     _RequiredDescribeListenerCertificatesInputRequestTypeDef,
     _OptionalDescribeListenerCertificatesInputRequestTypeDef,
 ):
     pass
 
-DescribeListenersInputDescribeListenersPaginateTypeDef = TypedDict(
-    "DescribeListenersInputDescribeListenersPaginateTypeDef",
-    {
-        "LoadBalancerArn": str,
-        "ListenerArns": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeListenersInputRequestTypeDef = TypedDict(
     "DescribeListenersInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
         "ListenerArns": Sequence[str],
         "Marker": str,
         "PageSize": int,
@@ -461,24 +513,14 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef = TypedDict(
-    "DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef",
-    {
-        "LoadBalancerArns": Sequence[str],
-        "Names": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -491,45 +533,25 @@
         "Names": Sequence[str],
         "Marker": str,
         "PageSize": int,
     },
     total=False,
 )
 
-DescribeRulesInputDescribeRulesPaginateTypeDef = TypedDict(
-    "DescribeRulesInputDescribeRulesPaginateTypeDef",
-    {
-        "ListenerArn": str,
-        "RuleArns": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeRulesInputRequestTypeDef = TypedDict(
     "DescribeRulesInputRequestTypeDef",
     {
         "ListenerArn": str,
         "RuleArns": Sequence[str],
         "Marker": str,
         "PageSize": int,
     },
     total=False,
 )
 
-DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef = TypedDict(
-    "DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef",
-    {
-        "Names": Sequence[str],
-        "LoadBalancerType": LoadBalancerTypeEnumType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeSSLPoliciesInputRequestTypeDef = TypedDict(
     "DescribeSSLPoliciesInputRequestTypeDef",
     {
         "Names": Sequence[str],
         "Marker": str,
         "PageSize": int,
         "LoadBalancerType": LoadBalancerTypeEnumType,
@@ -556,25 +578,14 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef = TypedDict(
-    "DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef",
-    {
-        "LoadBalancerArn": str,
-        "TargetGroupArns": Sequence[str],
-        "Names": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeTargetGroupsInputRequestTypeDef = TypedDict(
     "DescribeTargetGroupsInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
         "TargetGroupArns": Sequence[str],
         "Names": Sequence[str],
         "Marker": str,
@@ -597,31 +608,56 @@
     {
         "TargetGroupArn": str,
         "Weight": int,
     },
     total=False,
 )
 
+HostHeaderConditionConfigOutputTypeDef = TypedDict(
+    "HostHeaderConditionConfigOutputTypeDef",
+    {
+        "Values": List[str],
+    },
+    total=False,
+)
+
 HostHeaderConditionConfigTypeDef = TypedDict(
     "HostHeaderConditionConfigTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
 
+HttpHeaderConditionConfigOutputTypeDef = TypedDict(
+    "HttpHeaderConditionConfigOutputTypeDef",
+    {
+        "HttpHeaderName": str,
+        "Values": List[str],
+    },
+    total=False,
+)
+
 HttpHeaderConditionConfigTypeDef = TypedDict(
     "HttpHeaderConditionConfigTypeDef",
     {
         "HttpHeaderName": str,
         "Values": Sequence[str],
     },
     total=False,
 )
 
+HttpRequestMethodConditionConfigOutputTypeDef = TypedDict(
+    "HttpRequestMethodConditionConfigOutputTypeDef",
+    {
+        "Values": List[str],
+    },
+    total=False,
+)
+
 HttpRequestMethodConditionConfigTypeDef = TypedDict(
     "HttpRequestMethodConditionConfigTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
@@ -631,20 +667,18 @@
     {
         "Code": LoadBalancerStateEnumType,
         "Reason": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+PathPatternConditionConfigOutputTypeDef = TypedDict(
+    "PathPatternConditionConfigOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Values": List[str],
     },
     total=False,
 )
 
 PathPatternConditionConfigTypeDef = TypedDict(
     "PathPatternConditionConfigTypeDef",
     {
@@ -666,23 +700,20 @@
     "RemoveTagsInputRequestTypeDef",
     {
         "ResourceArns": Sequence[str],
         "TagKeys": Sequence[str],
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+SourceIpConditionConfigOutputTypeDef = TypedDict(
+    "SourceIpConditionConfigOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Values": List[str],
     },
+    total=False,
 )
 
 SourceIpConditionConfigTypeDef = TypedDict(
     "SourceIpConditionConfigTypeDef",
     {
         "Values": Sequence[str],
     },
@@ -702,38 +733,22 @@
     "SetIpAddressTypeInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
         "IpAddressType": IpAddressTypeType,
     },
 )
 
-SetIpAddressTypeOutputTypeDef = TypedDict(
-    "SetIpAddressTypeOutputTypeDef",
-    {
-        "IpAddressType": IpAddressTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetSecurityGroupsInputRequestTypeDef = TypedDict(
     "SetSecurityGroupsInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
         "SecurityGroups": Sequence[str],
     },
 )
 
-SetSecurityGroupsOutputTypeDef = TypedDict(
-    "SetSecurityGroupsOutputTypeDef",
-    {
-        "SecurityGroupIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TargetHealthTypeDef = TypedDict(
     "TargetHealthTypeDef",
     {
         "State": TargetHealthStateEnumType,
         "Reason": TargetHealthReasonEnumType,
         "Description": str,
     },
@@ -744,36 +759,52 @@
     "AddListenerCertificatesInputRequestTypeDef",
     {
         "ListenerArn": str,
         "Certificates": Sequence[CertificateTypeDef],
     },
 )
 
+RemoveListenerCertificatesInputRequestTypeDef = TypedDict(
+    "RemoveListenerCertificatesInputRequestTypeDef",
+    {
+        "ListenerArn": str,
+        "Certificates": Sequence[CertificateTypeDef],
+    },
+)
+
 AddListenerCertificatesOutputTypeDef = TypedDict(
     "AddListenerCertificatesOutputTypeDef",
     {
         "Certificates": List[CertificateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeListenerCertificatesOutputTypeDef = TypedDict(
     "DescribeListenerCertificatesOutputTypeDef",
     {
         "Certificates": List[CertificateTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RemoveListenerCertificatesInputRequestTypeDef = TypedDict(
-    "RemoveListenerCertificatesInputRequestTypeDef",
+SetIpAddressTypeOutputTypeDef = TypedDict(
+    "SetIpAddressTypeOutputTypeDef",
     {
-        "ListenerArn": str,
-        "Certificates": Sequence[CertificateTypeDef],
+        "IpAddressType": IpAddressTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetSecurityGroupsOutputTypeDef = TypedDict(
+    "SetSecurityGroupsOutputTypeDef",
+    {
+        "SecurityGroupIds": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddTagsInputRequestTypeDef = TypedDict(
     "AddTagsInputRequestTypeDef",
     {
         "ResourceArns": Sequence[str],
@@ -977,28 +1008,107 @@
     "RegisterTargetsInputRequestTypeDef",
     {
         "TargetGroupArn": str,
         "Targets": Sequence[TargetDescriptionTypeDef],
     },
 )
 
+DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
+    {
+        "ListenerArn": str,
+    },
+)
+_OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef(
+    _RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
+    _OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
+):
+    pass
+
+DescribeListenersInputDescribeListenersPaginateTypeDef = TypedDict(
+    "DescribeListenersInputDescribeListenersPaginateTypeDef",
+    {
+        "LoadBalancerArn": str,
+        "ListenerArns": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef = TypedDict(
+    "DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef",
+    {
+        "LoadBalancerArns": Sequence[str],
+        "Names": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeRulesInputDescribeRulesPaginateTypeDef = TypedDict(
+    "DescribeRulesInputDescribeRulesPaginateTypeDef",
+    {
+        "ListenerArn": str,
+        "RuleArns": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef = TypedDict(
+    "DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef",
+    {
+        "Names": Sequence[str],
+        "LoadBalancerType": LoadBalancerTypeEnumType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef = TypedDict(
+    "DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef",
+    {
+        "LoadBalancerArn": str,
+        "TargetGroupArns": Sequence[str],
+        "Names": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeAccountLimitsOutputTypeDef = TypedDict(
     "DescribeAccountLimitsOutputTypeDef",
     {
         "Limits": List[LimitTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLoadBalancerAttributesOutputTypeDef = TypedDict(
     "DescribeLoadBalancerAttributesOutputTypeDef",
     {
         "Attributes": List[LoadBalancerAttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyLoadBalancerAttributesInputRequestTypeDef = TypedDict(
     "ModifyLoadBalancerAttributesInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
@@ -1006,15 +1116,15 @@
     },
 )
 
 ModifyLoadBalancerAttributesOutputTypeDef = TypedDict(
     "ModifyLoadBalancerAttributesOutputTypeDef",
     {
         "Attributes": List[LoadBalancerAttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef = TypedDict(
     "DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef",
     {
         "LoadBalancerArns": Sequence[str],
@@ -1092,15 +1202,15 @@
 ):
     pass
 
 DescribeTargetGroupAttributesOutputTypeDef = TypedDict(
     "DescribeTargetGroupAttributesOutputTypeDef",
     {
         "Attributes": List[TargetGroupAttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyTargetGroupAttributesInputRequestTypeDef = TypedDict(
     "ModifyTargetGroupAttributesInputRequestTypeDef",
     {
         "TargetGroupArn": str,
@@ -1108,27 +1218,44 @@
     },
 )
 
 ModifyTargetGroupAttributesOutputTypeDef = TypedDict(
     "ModifyTargetGroupAttributesOutputTypeDef",
     {
         "Attributes": List[TargetGroupAttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ForwardActionConfigOutputTypeDef = TypedDict(
+    "ForwardActionConfigOutputTypeDef",
+    {
+        "TargetGroups": List[TargetGroupTupleTypeDef],
+        "TargetGroupStickinessConfig": TargetGroupStickinessConfigTypeDef,
     },
+    total=False,
 )
 
 ForwardActionConfigTypeDef = TypedDict(
     "ForwardActionConfigTypeDef",
     {
         "TargetGroups": Sequence[TargetGroupTupleTypeDef],
         "TargetGroupStickinessConfig": TargetGroupStickinessConfigTypeDef,
     },
     total=False,
 )
 
+QueryStringConditionConfigOutputTypeDef = TypedDict(
+    "QueryStringConditionConfigOutputTypeDef",
+    {
+        "Values": List[QueryStringKeyValuePairTypeDef],
+    },
+    total=False,
+)
+
 QueryStringConditionConfigTypeDef = TypedDict(
     "QueryStringConditionConfigTypeDef",
     {
         "Values": Sequence[QueryStringKeyValuePairTypeDef],
     },
     total=False,
 )
@@ -1150,15 +1277,15 @@
     total=False,
 )
 
 DescribeTagsOutputTypeDef = TypedDict(
     "DescribeTagsOutputTypeDef",
     {
         "TagDescriptions": List[TagDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LoadBalancerTypeDef = TypedDict(
     "LoadBalancerTypeDef",
     {
         "LoadBalancerArn": str,
@@ -1179,52 +1306,75 @@
 )
 
 SetSubnetsOutputTypeDef = TypedDict(
     "SetSubnetsOutputTypeDef",
     {
         "AvailabilityZones": List[AvailabilityZoneTypeDef],
         "IpAddressType": IpAddressTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSSLPoliciesOutputTypeDef = TypedDict(
     "DescribeSSLPoliciesOutputTypeDef",
     {
         "SslPolicies": List[SslPolicyTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTargetGroupOutputTypeDef = TypedDict(
     "CreateTargetGroupOutputTypeDef",
     {
         "TargetGroups": List[TargetGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTargetGroupsOutputTypeDef = TypedDict(
     "DescribeTargetGroupsOutputTypeDef",
     {
         "TargetGroups": List[TargetGroupTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyTargetGroupOutputTypeDef = TypedDict(
     "ModifyTargetGroupOutputTypeDef",
     {
         "TargetGroups": List[TargetGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredActionOutputTypeDef = TypedDict(
+    "_RequiredActionOutputTypeDef",
+    {
+        "Type": ActionTypeEnumType,
+    },
+)
+_OptionalActionOutputTypeDef = TypedDict(
+    "_OptionalActionOutputTypeDef",
+    {
+        "TargetGroupArn": str,
+        "AuthenticateOidcConfig": AuthenticateOidcActionConfigOutputTypeDef,
+        "AuthenticateCognitoConfig": AuthenticateCognitoActionConfigOutputTypeDef,
+        "Order": int,
+        "RedirectConfig": RedirectActionConfigTypeDef,
+        "FixedResponseConfig": FixedResponseActionConfigTypeDef,
+        "ForwardConfig": ForwardActionConfigOutputTypeDef,
     },
+    total=False,
 )
 
+class ActionOutputTypeDef(_RequiredActionOutputTypeDef, _OptionalActionOutputTypeDef):
+    pass
+
 _RequiredActionTypeDef = TypedDict(
     "_RequiredActionTypeDef",
     {
         "Type": ActionTypeEnumType,
     },
 )
 _OptionalActionTypeDef = TypedDict(
@@ -1240,14 +1390,29 @@
     },
     total=False,
 )
 
 class ActionTypeDef(_RequiredActionTypeDef, _OptionalActionTypeDef):
     pass
 
+RuleConditionOutputTypeDef = TypedDict(
+    "RuleConditionOutputTypeDef",
+    {
+        "Field": str,
+        "Values": List[str],
+        "HostHeaderConfig": HostHeaderConditionConfigOutputTypeDef,
+        "PathPatternConfig": PathPatternConditionConfigOutputTypeDef,
+        "HttpHeaderConfig": HttpHeaderConditionConfigOutputTypeDef,
+        "QueryStringConfig": QueryStringConditionConfigOutputTypeDef,
+        "HttpRequestMethodConfig": HttpRequestMethodConditionConfigOutputTypeDef,
+        "SourceIpConfig": SourceIpConditionConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 RuleConditionTypeDef = TypedDict(
     "RuleConditionTypeDef",
     {
         "Field": str,
         "Values": Sequence[str],
         "HostHeaderConfig": HostHeaderConditionConfigTypeDef,
         "PathPatternConfig": PathPatternConditionConfigTypeDef,
@@ -1259,40 +1424,94 @@
     total=False,
 )
 
 DescribeTargetHealthOutputTypeDef = TypedDict(
     "DescribeTargetHealthOutputTypeDef",
     {
         "TargetHealthDescriptions": List[TargetHealthDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateLoadBalancerOutputTypeDef = TypedDict(
     "CreateLoadBalancerOutputTypeDef",
     {
         "LoadBalancers": List[LoadBalancerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLoadBalancersOutputTypeDef = TypedDict(
     "DescribeLoadBalancersOutputTypeDef",
     {
         "LoadBalancers": List[LoadBalancerTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListenerTypeDef = TypedDict(
+    "ListenerTypeDef",
+    {
+        "ListenerArn": str,
+        "LoadBalancerArn": str,
+        "Port": int,
+        "Protocol": ProtocolEnumType,
+        "Certificates": List[CertificateTypeDef],
+        "SslPolicy": str,
+        "DefaultActions": List[ActionOutputTypeDef],
+        "AlpnPolicy": List[str],
+    },
+    total=False,
+)
+
+ActionUnionTypeDef = Union[ActionTypeDef, ActionOutputTypeDef]
+RuleTypeDef = TypedDict(
+    "RuleTypeDef",
+    {
+        "RuleArn": str,
+        "Priority": str,
+        "Conditions": List[RuleConditionOutputTypeDef],
+        "Actions": List[ActionOutputTypeDef],
+        "IsDefault": bool,
+    },
+    total=False,
+)
+
+RuleConditionUnionTypeDef = Union[RuleConditionTypeDef, RuleConditionOutputTypeDef]
+CreateListenerOutputTypeDef = TypedDict(
+    "CreateListenerOutputTypeDef",
+    {
+        "Listeners": List[ListenerTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeListenersOutputTypeDef = TypedDict(
+    "DescribeListenersOutputTypeDef",
+    {
+        "Listeners": List[ListenerTypeDef],
+        "NextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyListenerOutputTypeDef = TypedDict(
+    "ModifyListenerOutputTypeDef",
+    {
+        "Listeners": List[ListenerTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateListenerInputRequestTypeDef = TypedDict(
     "_RequiredCreateListenerInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
-        "DefaultActions": Sequence[ActionTypeDef],
+        "DefaultActions": Sequence[ActionUnionTypeDef],
     },
 )
 _OptionalCreateListenerInputRequestTypeDef = TypedDict(
     "_OptionalCreateListenerInputRequestTypeDef",
     {
         "Protocol": ProtocolEnumType,
         "Port": int,
@@ -1305,60 +1524,78 @@
 )
 
 class CreateListenerInputRequestTypeDef(
     _RequiredCreateListenerInputRequestTypeDef, _OptionalCreateListenerInputRequestTypeDef
 ):
     pass
 
-ListenerTypeDef = TypedDict(
-    "ListenerTypeDef",
-    {
-        "ListenerArn": str,
-        "LoadBalancerArn": str,
-        "Port": int,
-        "Protocol": ProtocolEnumType,
-        "Certificates": List[CertificateTypeDef],
-        "SslPolicy": str,
-        "DefaultActions": List[ActionTypeDef],
-        "AlpnPolicy": List[str],
-    },
-    total=False,
-)
-
 _RequiredModifyListenerInputRequestTypeDef = TypedDict(
     "_RequiredModifyListenerInputRequestTypeDef",
     {
         "ListenerArn": str,
     },
 )
 _OptionalModifyListenerInputRequestTypeDef = TypedDict(
     "_OptionalModifyListenerInputRequestTypeDef",
     {
         "Port": int,
         "Protocol": ProtocolEnumType,
         "SslPolicy": str,
         "Certificates": Sequence[CertificateTypeDef],
-        "DefaultActions": Sequence[ActionTypeDef],
+        "DefaultActions": Sequence[ActionUnionTypeDef],
         "AlpnPolicy": Sequence[str],
     },
     total=False,
 )
 
 class ModifyListenerInputRequestTypeDef(
     _RequiredModifyListenerInputRequestTypeDef, _OptionalModifyListenerInputRequestTypeDef
 ):
     pass
 
+CreateRuleOutputTypeDef = TypedDict(
+    "CreateRuleOutputTypeDef",
+    {
+        "Rules": List[RuleTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeRulesOutputTypeDef = TypedDict(
+    "DescribeRulesOutputTypeDef",
+    {
+        "Rules": List[RuleTypeDef],
+        "NextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyRuleOutputTypeDef = TypedDict(
+    "ModifyRuleOutputTypeDef",
+    {
+        "Rules": List[RuleTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetRulePrioritiesOutputTypeDef = TypedDict(
+    "SetRulePrioritiesOutputTypeDef",
+    {
+        "Rules": List[RuleTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateRuleInputRequestTypeDef = TypedDict(
     "_RequiredCreateRuleInputRequestTypeDef",
     {
         "ListenerArn": str,
-        "Conditions": Sequence[RuleConditionTypeDef],
+        "Conditions": Sequence[RuleConditionUnionTypeDef],
         "Priority": int,
-        "Actions": Sequence[ActionTypeDef],
+        "Actions": Sequence[ActionUnionTypeDef],
     },
 )
 _OptionalCreateRuleInputRequestTypeDef = TypedDict(
     "_OptionalCreateRuleInputRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
@@ -1375,87 +1612,17 @@
     {
         "RuleArn": str,
     },
 )
 _OptionalModifyRuleInputRequestTypeDef = TypedDict(
     "_OptionalModifyRuleInputRequestTypeDef",
     {
-        "Conditions": Sequence[RuleConditionTypeDef],
-        "Actions": Sequence[ActionTypeDef],
+        "Conditions": Sequence[RuleConditionUnionTypeDef],
+        "Actions": Sequence[ActionUnionTypeDef],
     },
     total=False,
 )
 
 class ModifyRuleInputRequestTypeDef(
     _RequiredModifyRuleInputRequestTypeDef, _OptionalModifyRuleInputRequestTypeDef
 ):
     pass
-
-RuleTypeDef = TypedDict(
-    "RuleTypeDef",
-    {
-        "RuleArn": str,
-        "Priority": str,
-        "Conditions": List[RuleConditionTypeDef],
-        "Actions": List[ActionTypeDef],
-        "IsDefault": bool,
-    },
-    total=False,
-)
-
-CreateListenerOutputTypeDef = TypedDict(
-    "CreateListenerOutputTypeDef",
-    {
-        "Listeners": List[ListenerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeListenersOutputTypeDef = TypedDict(
-    "DescribeListenersOutputTypeDef",
-    {
-        "Listeners": List[ListenerTypeDef],
-        "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ModifyListenerOutputTypeDef = TypedDict(
-    "ModifyListenerOutputTypeDef",
-    {
-        "Listeners": List[ListenerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateRuleOutputTypeDef = TypedDict(
-    "CreateRuleOutputTypeDef",
-    {
-        "Rules": List[RuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeRulesOutputTypeDef = TypedDict(
-    "DescribeRulesOutputTypeDef",
-    {
-        "Rules": List[RuleTypeDef],
-        "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ModifyRuleOutputTypeDef = TypedDict(
-    "ModifyRuleOutputTypeDef",
-    {
-        "Rules": List[RuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SetRulePrioritiesOutputTypeDef = TypedDict(
-    "SetRulePrioritiesOutputTypeDef",
-    {
-        "Rules": List[RuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2/waiter.py` & `types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2/waiter.pyi` & `types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2.egg-info/PKG-INFO` & `types-aiobotocore-elbv2-2.5.2.post1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,29 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-elbv2
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ElasticLoadBalancingv2 2.5.2 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore elbv2 type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="types-aiobotocore-elbv2"></a>
 
 # types-aiobotocore-elbv2
 
 [![PyPI - types-aiobotocore-elbv2](https://img.shields.io/pypi/v/types-aiobotocore-elbv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elbv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elbv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elbv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-elbv2?color=blue)](https://pypistats.org/packages/types-aiobotocore-elbv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elbv2)](https://pepy.tech/project/types-aiobotocore-elbv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ElasticLoadBalancingv2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
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
 [types-aiobotocore-elbv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/).
 
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
@@ -394,138 +361,151 @@
 )
 
 
 def check_value(value: ActionTypeEnumType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_elbv2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_elbv2.type_defs import (
-    AuthenticateCognitoActionConfigTypeDef,
-    AuthenticateOidcActionConfigTypeDef,
+    AuthenticateCognitoActionConfigOutputTypeDef,
+    AuthenticateOidcActionConfigOutputTypeDef,
     FixedResponseActionConfigTypeDef,
     RedirectActionConfigTypeDef,
+    AuthenticateCognitoActionConfigTypeDef,
+    AuthenticateOidcActionConfigTypeDef,
     CertificateTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     LoadBalancerAddressTypeDef,
     CipherTypeDef,
     SubnetMappingTypeDef,
     MatcherTypeDef,
     DeleteListenerInputRequestTypeDef,
     DeleteLoadBalancerInputRequestTypeDef,
     DeleteRuleInputRequestTypeDef,
     DeleteTargetGroupInputRequestTypeDef,
     TargetDescriptionTypeDef,
-    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     LimitTypeDef,
-    DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
     DescribeListenerCertificatesInputRequestTypeDef,
-    DescribeListenersInputDescribeListenersPaginateTypeDef,
     DescribeListenersInputRequestTypeDef,
     DescribeLoadBalancerAttributesInputRequestTypeDef,
     LoadBalancerAttributeTypeDef,
-    DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef,
     WaiterConfigTypeDef,
     DescribeLoadBalancersInputRequestTypeDef,
-    DescribeRulesInputDescribeRulesPaginateTypeDef,
     DescribeRulesInputRequestTypeDef,
-    DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef,
     DescribeSSLPoliciesInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
     DescribeTargetGroupAttributesInputRequestTypeDef,
     TargetGroupAttributeTypeDef,
-    DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef,
     DescribeTargetGroupsInputRequestTypeDef,
     TargetGroupStickinessConfigTypeDef,
     TargetGroupTupleTypeDef,
+    HostHeaderConditionConfigOutputTypeDef,
     HostHeaderConditionConfigTypeDef,
+    HttpHeaderConditionConfigOutputTypeDef,
     HttpHeaderConditionConfigTypeDef,
+    HttpRequestMethodConditionConfigOutputTypeDef,
     HttpRequestMethodConditionConfigTypeDef,
     LoadBalancerStateTypeDef,
-    PaginatorConfigTypeDef,
+    PathPatternConditionConfigOutputTypeDef,
     PathPatternConditionConfigTypeDef,
     QueryStringKeyValuePairTypeDef,
     RemoveTagsInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    SourceIpConditionConfigOutputTypeDef,
     SourceIpConditionConfigTypeDef,
     RulePriorityPairTypeDef,
     SetIpAddressTypeInputRequestTypeDef,
-    SetIpAddressTypeOutputTypeDef,
     SetSecurityGroupsInputRequestTypeDef,
-    SetSecurityGroupsOutputTypeDef,
     TargetHealthTypeDef,
     AddListenerCertificatesInputRequestTypeDef,
+    RemoveListenerCertificatesInputRequestTypeDef,
     AddListenerCertificatesOutputTypeDef,
     DescribeListenerCertificatesOutputTypeDef,
-    RemoveListenerCertificatesInputRequestTypeDef,
+    SetIpAddressTypeOutputTypeDef,
+    SetSecurityGroupsOutputTypeDef,
     AddTagsInputRequestTypeDef,
     TagDescriptionTypeDef,
     AvailabilityZoneTypeDef,
     SslPolicyTypeDef,
     CreateLoadBalancerInputRequestTypeDef,
     SetSubnetsInputRequestTypeDef,
     CreateTargetGroupInputRequestTypeDef,
     ModifyTargetGroupInputRequestTypeDef,
     TargetGroupTypeDef,
     DeregisterTargetsInputRequestTypeDef,
     DescribeTargetHealthInputRequestTypeDef,
     RegisterTargetsInputRequestTypeDef,
+    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
+    DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
+    DescribeListenersInputDescribeListenersPaginateTypeDef,
+    DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef,
+    DescribeRulesInputDescribeRulesPaginateTypeDef,
+    DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef,
+    DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef,
     DescribeAccountLimitsOutputTypeDef,
     DescribeLoadBalancerAttributesOutputTypeDef,
     ModifyLoadBalancerAttributesInputRequestTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
     DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef,
     DescribeLoadBalancersInputLoadBalancerExistsWaitTypeDef,
     DescribeLoadBalancersInputLoadBalancersDeletedWaitTypeDef,
     DescribeTargetHealthInputTargetDeregisteredWaitTypeDef,
     DescribeTargetHealthInputTargetInServiceWaitTypeDef,
     DescribeTargetGroupAttributesOutputTypeDef,
     ModifyTargetGroupAttributesInputRequestTypeDef,
     ModifyTargetGroupAttributesOutputTypeDef,
+    ForwardActionConfigOutputTypeDef,
     ForwardActionConfigTypeDef,
+    QueryStringConditionConfigOutputTypeDef,
     QueryStringConditionConfigTypeDef,
     SetRulePrioritiesInputRequestTypeDef,
     TargetHealthDescriptionTypeDef,
     DescribeTagsOutputTypeDef,
     LoadBalancerTypeDef,
     SetSubnetsOutputTypeDef,
     DescribeSSLPoliciesOutputTypeDef,
     CreateTargetGroupOutputTypeDef,
     DescribeTargetGroupsOutputTypeDef,
     ModifyTargetGroupOutputTypeDef,
+    ActionOutputTypeDef,
     ActionTypeDef,
+    RuleConditionOutputTypeDef,
     RuleConditionTypeDef,
     DescribeTargetHealthOutputTypeDef,
     CreateLoadBalancerOutputTypeDef,
     DescribeLoadBalancersOutputTypeDef,
-    CreateListenerInputRequestTypeDef,
     ListenerTypeDef,
-    ModifyListenerInputRequestTypeDef,
-    CreateRuleInputRequestTypeDef,
-    ModifyRuleInputRequestTypeDef,
+    ActionUnionTypeDef,
     RuleTypeDef,
+    RuleConditionUnionTypeDef,
     CreateListenerOutputTypeDef,
     DescribeListenersOutputTypeDef,
     ModifyListenerOutputTypeDef,
+    CreateListenerInputRequestTypeDef,
+    ModifyListenerInputRequestTypeDef,
     CreateRuleOutputTypeDef,
     DescribeRulesOutputTypeDef,
     ModifyRuleOutputTypeDef,
     SetRulePrioritiesOutputTypeDef,
+    CreateRuleInputRequestTypeDef,
+    ModifyRuleInputRequestTypeDef,
 )
 
 
-def get_structure() -> AuthenticateCognitoActionConfigTypeDef:
+def get_value() -> AuthenticateCognitoActionConfigOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-elbv2-2.5.2/types_aiobotocore_elbv2.egg-info/SOURCES.txt` & `types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*


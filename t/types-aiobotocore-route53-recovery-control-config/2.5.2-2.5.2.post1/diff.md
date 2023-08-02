# Comparing `tmp/types-aiobotocore-route53-recovery-control-config-2.5.2.tar.gz` & `tmp/types-aiobotocore-route53-recovery-control-config-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-route53-recovery-control-config-2.5.2.tar", last modified: Sat Jul  8 01:44:13 2023, max compression
+gzip compressed data, was "types-aiobotocore-route53-recovery-control-config-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:54 2023, max compression
```

## Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2.tar` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:13.638802 types-aiobotocore-route53-recovery-control-config-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:39:28.000000 types-aiobotocore-route53-recovery-control-config-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19529 2023-07-08 01:44:13.638802 types-aiobotocore-route53-recovery-control-config-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17871 2023-07-08 01:39:28.000000 types-aiobotocore-route53-recovery-control-config-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:13.638802 types-aiobotocore-route53-recovery-control-config-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-08 01:39:28.000000 types-aiobotocore-route53-recovery-control-config-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:13.638802 types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config/
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-08 01:39:28.000000 types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-08 01:39:28.000000 types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-08 01:39:28.000000 types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25723 2023-07-08 01:39:28.000000 types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25680 2023-07-08 01:39:28.000000 types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9366 2023-07-08 01:39:31.000000 types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-07-08 01:39:29.000000 types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-07-08 01:39:28.000000 types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-07-08 01:39:28.000000 types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:39:28.000000 types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23280 2023-07-08 01:39:31.000000 types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23249 2023-07-08 01:39:31.000000 types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:39:28.000000 types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-07-08 01:39:28.000000 types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-07-08 01:39:28.000000 types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:13.638802 types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19529 2023-07-08 01:44:13.000000 types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-08 01:44:13.000000 types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:13.000000 types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:13.000000 types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:13.000000 types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-08 01:44:13.000000 types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:54.789475 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19465 2023-08-02 14:52:54.789475 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17854 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:54.789475 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:54.789475 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25723 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25680 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9366 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23234 2023-08-02 14:48:07.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23203 2023-08-02 14:48:07.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:54.789475 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19465 2023-08-02 14:52:54.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-08-02 14:52:54.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:54.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:54.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:54.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-02 14:52:54.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2/LICENSE` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2/PKG-INFO` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-route53-recovery-control-config
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Route53RecoveryControlConfig 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Route53RecoveryControlConfig 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore route53-recovery-control-config type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore route53-recovery-control-config type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-route53-recovery-control-config"></a>
 
 # types-aiobotocore-route53-recovery-control-config
 
 [![PyPI - types-aiobotocore-route53-recovery-control-config](https://img.shields.io/pypi/v/types-aiobotocore-route53-recovery-control-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-control-config)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53-recovery-control-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-control-config)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-route53-recovery-control-config?color=blue)](https://pypistats.org/packages/types-aiobotocore-route53-recovery-control-config)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53-recovery-control-config)](https://pepy.tech/project/types-aiobotocore-route53-recovery-control-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Route53RecoveryControlConfig 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig)
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
 [types-aiobotocore-route53-recovery-control-config docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/).
 
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
@@ -384,94 +383,94 @@
 )
 
 
 def check_value(value: ClusterCreatedWaiterName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_route53_recovery_control_config.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from types_aiobotocore_route53_recovery_control_config.type_defs import (
     RuleConfigTypeDef,
     AssertionRuleUpdateTypeDef,
     ClusterEndpointTypeDef,
     ControlPanelTypeDef,
     CreateClusterRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     CreateControlPanelRequestRequestTypeDef,
     CreateRoutingControlRequestRequestTypeDef,
     RoutingControlTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteControlPanelRequestRequestTypeDef,
     DeleteRoutingControlRequestRequestTypeDef,
     DeleteSafetyRuleRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeControlPanelRequestRequestTypeDef,
     DescribeRoutingControlRequestRequestTypeDef,
     DescribeSafetyRuleRequestRequestTypeDef,
     GatingRuleUpdateTypeDef,
-    ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAssociatedRoute53HealthChecksRequestRequestTypeDef,
-    ListAssociatedRoute53HealthChecksResponseTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
-    ListControlPanelsRequestListControlPanelsPaginateTypeDef,
     ListControlPanelsRequestRequestTypeDef,
-    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
     ListRoutingControlsRequestRequestTypeDef,
-    ListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
     ListSafetyRulesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateControlPanelRequestRequestTypeDef,
     UpdateRoutingControlRequestRequestTypeDef,
     AssertionRuleTypeDef,
     GatingRuleTypeDef,
     NewAssertionRuleTypeDef,
     NewGatingRuleTypeDef,
     ClusterTypeDef,
     CreateControlPanelResponseTypeDef,
     DescribeControlPanelResponseTypeDef,
+    ListAssociatedRoute53HealthChecksResponseTypeDef,
     ListControlPanelsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     UpdateControlPanelResponseTypeDef,
     CreateRoutingControlResponseTypeDef,
     DescribeRoutingControlResponseTypeDef,
     ListRoutingControlsResponseTypeDef,
     UpdateRoutingControlResponseTypeDef,
     DescribeClusterRequestClusterCreatedWaitTypeDef,
     DescribeClusterRequestClusterDeletedWaitTypeDef,
     DescribeControlPanelRequestControlPanelCreatedWaitTypeDef,
     DescribeControlPanelRequestControlPanelDeletedWaitTypeDef,
     DescribeRoutingControlRequestRoutingControlCreatedWaitTypeDef,
     DescribeRoutingControlRequestRoutingControlDeletedWaitTypeDef,
     UpdateSafetyRuleRequestRequestTypeDef,
+    ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
+    ListControlPanelsRequestListControlPanelsPaginateTypeDef,
+    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
+    ListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
     CreateSafetyRuleResponseTypeDef,
     DescribeSafetyRuleResponseTypeDef,
     RuleTypeDef,
     UpdateSafetyRuleResponseTypeDef,
     CreateSafetyRuleRequestRequestTypeDef,
     CreateClusterResponseTypeDef,
     DescribeClusterResponseTypeDef,
     ListClustersResponseTypeDef,
     ListSafetyRulesResponseTypeDef,
 )
 
 
-def get_structure() -> RuleConfigTypeDef:
+def get_value() -> RuleConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2/README.md` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-route53-recovery-control-config"></a>
 
 # types-aiobotocore-route53-recovery-control-config
 
 [![PyPI - types-aiobotocore-route53-recovery-control-config](https://img.shields.io/pypi/v/types-aiobotocore-route53-recovery-control-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-control-config)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53-recovery-control-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-control-config)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-route53-recovery-control-config?color=blue)](https://pypistats.org/packages/types-aiobotocore-route53-recovery-control-config)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53-recovery-control-config)](https://pepy.tech/project/types-aiobotocore-route53-recovery-control-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Route53RecoveryControlConfig 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig)
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
 [types-aiobotocore-route53-recovery-control-config docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/).
 
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
@@ -351,94 +351,94 @@
 )
 
 
 def check_value(value: ClusterCreatedWaiterName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_route53_recovery_control_config.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from types_aiobotocore_route53_recovery_control_config.type_defs import (
     RuleConfigTypeDef,
     AssertionRuleUpdateTypeDef,
     ClusterEndpointTypeDef,
     ControlPanelTypeDef,
     CreateClusterRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     CreateControlPanelRequestRequestTypeDef,
     CreateRoutingControlRequestRequestTypeDef,
     RoutingControlTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteControlPanelRequestRequestTypeDef,
     DeleteRoutingControlRequestRequestTypeDef,
     DeleteSafetyRuleRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeControlPanelRequestRequestTypeDef,
     DescribeRoutingControlRequestRequestTypeDef,
     DescribeSafetyRuleRequestRequestTypeDef,
     GatingRuleUpdateTypeDef,
-    ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAssociatedRoute53HealthChecksRequestRequestTypeDef,
-    ListAssociatedRoute53HealthChecksResponseTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
-    ListControlPanelsRequestListControlPanelsPaginateTypeDef,
     ListControlPanelsRequestRequestTypeDef,
-    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
     ListRoutingControlsRequestRequestTypeDef,
-    ListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
     ListSafetyRulesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateControlPanelRequestRequestTypeDef,
     UpdateRoutingControlRequestRequestTypeDef,
     AssertionRuleTypeDef,
     GatingRuleTypeDef,
     NewAssertionRuleTypeDef,
     NewGatingRuleTypeDef,
     ClusterTypeDef,
     CreateControlPanelResponseTypeDef,
     DescribeControlPanelResponseTypeDef,
+    ListAssociatedRoute53HealthChecksResponseTypeDef,
     ListControlPanelsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     UpdateControlPanelResponseTypeDef,
     CreateRoutingControlResponseTypeDef,
     DescribeRoutingControlResponseTypeDef,
     ListRoutingControlsResponseTypeDef,
     UpdateRoutingControlResponseTypeDef,
     DescribeClusterRequestClusterCreatedWaitTypeDef,
     DescribeClusterRequestClusterDeletedWaitTypeDef,
     DescribeControlPanelRequestControlPanelCreatedWaitTypeDef,
     DescribeControlPanelRequestControlPanelDeletedWaitTypeDef,
     DescribeRoutingControlRequestRoutingControlCreatedWaitTypeDef,
     DescribeRoutingControlRequestRoutingControlDeletedWaitTypeDef,
     UpdateSafetyRuleRequestRequestTypeDef,
+    ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
+    ListControlPanelsRequestListControlPanelsPaginateTypeDef,
+    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
+    ListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
     CreateSafetyRuleResponseTypeDef,
     DescribeSafetyRuleResponseTypeDef,
     RuleTypeDef,
     UpdateSafetyRuleResponseTypeDef,
     CreateSafetyRuleRequestRequestTypeDef,
     CreateClusterResponseTypeDef,
     DescribeClusterResponseTypeDef,
     ListClustersResponseTypeDef,
     ListSafetyRulesResponseTypeDef,
 )
 
 
-def get_structure() -> RuleConfigTypeDef:
+def get_value() -> RuleConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2/setup.py` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,45 +6,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-route53-recovery-control-config",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_route53_recovery_control_config"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Route53RecoveryControlConfig 2.5.2 service generated with"
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
     keywords=(
-        "aiobotocore route53-recovery-control-config type-annotations boto3-stubs mypy typeshed"
+        "aiobotocore route53-recovery-control-config type-annotations botocore mypy typeshed"
         " autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_route53_recovery_control_config": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
```

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config/__init__.py` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config/__init__.pyi` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config/__main__.py` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.Route53RecoveryControlConfig 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig\nOther"
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

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config/client.py` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config/client.pyi` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config/literals.py` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config/literals.pyi` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config/paginator.py` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,73 +64,73 @@
 class ListAssociatedRoute53HealthChecksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListAssociatedRoute53HealthChecks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/paginators/#listassociatedroute53healthcheckspaginator)
     """
 
     def paginate(
-        self, *, RoutingControlArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RoutingControlArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAssociatedRoute53HealthChecksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListAssociatedRoute53HealthChecks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/paginators/#listassociatedroute53healthcheckspaginator)
         """
 
 
 class ListClustersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListClusters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/paginators/#listclusterspaginator)
         """
 
 
 class ListControlPanelsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListControlPanels)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/paginators/#listcontrolpanelspaginator)
     """
 
     def paginate(
-        self, *, ClusterArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ClusterArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListControlPanelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListControlPanels.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/paginators/#listcontrolpanelspaginator)
         """
 
 
 class ListRoutingControlsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListRoutingControls)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/paginators/#listroutingcontrolspaginator)
     """
 
     def paginate(
-        self, *, ControlPanelArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ControlPanelArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRoutingControlsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListRoutingControls.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/paginators/#listroutingcontrolspaginator)
         """
 
 
 class ListSafetyRulesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListSafetyRules)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/paginators/#listsafetyrulespaginator)
     """
 
     def paginate(
-        self, *, ControlPanelArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ControlPanelArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSafetyRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListSafetyRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/paginators/#listsafetyrulespaginator)
         """
```

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config/paginator.pyi` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -61,69 +61,69 @@
 class ListAssociatedRoute53HealthChecksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListAssociatedRoute53HealthChecks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/paginators/#listassociatedroute53healthcheckspaginator)
     """
 
     def paginate(
-        self, *, RoutingControlArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RoutingControlArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAssociatedRoute53HealthChecksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListAssociatedRoute53HealthChecks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/paginators/#listassociatedroute53healthcheckspaginator)
         """
 
 class ListClustersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListClusters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/paginators/#listclusterspaginator)
         """
 
 class ListControlPanelsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListControlPanels)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/paginators/#listcontrolpanelspaginator)
     """
 
     def paginate(
-        self, *, ClusterArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ClusterArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListControlPanelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListControlPanels.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/paginators/#listcontrolpanelspaginator)
         """
 
 class ListRoutingControlsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListRoutingControls)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/paginators/#listroutingcontrolspaginator)
     """
 
     def paginate(
-        self, *, ControlPanelArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ControlPanelArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRoutingControlsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListRoutingControls.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/paginators/#listroutingcontrolspaginator)
         """
 
 class ListSafetyRulesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListSafetyRules)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/paginators/#listsafetyrulespaginator)
     """
 
     def paginate(
-        self, *, ControlPanelArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ControlPanelArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSafetyRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListSafetyRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/paginators/#listsafetyrulespaginator)
         """
```

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config/type_defs.py` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_route53_recovery_control_config.type_defs import RuleConfigTypeDef
 
-    data: RuleConfigTypeDef = {...}
+    data: RuleConfigTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import RuleTypeType, StatusType
 
@@ -24,66 +24,66 @@
 
 __all__ = (
     "RuleConfigTypeDef",
     "AssertionRuleUpdateTypeDef",
     "ClusterEndpointTypeDef",
     "ControlPanelTypeDef",
     "CreateClusterRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateControlPanelRequestRequestTypeDef",
     "CreateRoutingControlRequestRequestTypeDef",
     "RoutingControlTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteControlPanelRequestRequestTypeDef",
     "DeleteRoutingControlRequestRequestTypeDef",
     "DeleteSafetyRuleRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeControlPanelRequestRequestTypeDef",
     "DescribeRoutingControlRequestRequestTypeDef",
     "DescribeSafetyRuleRequestRequestTypeDef",
     "GatingRuleUpdateTypeDef",
-    "ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAssociatedRoute53HealthChecksRequestRequestTypeDef",
-    "ListAssociatedRoute53HealthChecksResponseTypeDef",
-    "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
-    "ListControlPanelsRequestListControlPanelsPaginateTypeDef",
     "ListControlPanelsRequestRequestTypeDef",
-    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
     "ListRoutingControlsRequestRequestTypeDef",
-    "ListSafetyRulesRequestListSafetyRulesPaginateTypeDef",
     "ListSafetyRulesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateControlPanelRequestRequestTypeDef",
     "UpdateRoutingControlRequestRequestTypeDef",
     "AssertionRuleTypeDef",
     "GatingRuleTypeDef",
     "NewAssertionRuleTypeDef",
     "NewGatingRuleTypeDef",
     "ClusterTypeDef",
     "CreateControlPanelResponseTypeDef",
     "DescribeControlPanelResponseTypeDef",
+    "ListAssociatedRoute53HealthChecksResponseTypeDef",
     "ListControlPanelsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "UpdateControlPanelResponseTypeDef",
     "CreateRoutingControlResponseTypeDef",
     "DescribeRoutingControlResponseTypeDef",
     "ListRoutingControlsResponseTypeDef",
     "UpdateRoutingControlResponseTypeDef",
     "DescribeClusterRequestClusterCreatedWaitTypeDef",
     "DescribeClusterRequestClusterDeletedWaitTypeDef",
     "DescribeControlPanelRequestControlPanelCreatedWaitTypeDef",
     "DescribeControlPanelRequestControlPanelDeletedWaitTypeDef",
     "DescribeRoutingControlRequestRoutingControlCreatedWaitTypeDef",
     "DescribeRoutingControlRequestRoutingControlDeletedWaitTypeDef",
     "UpdateSafetyRuleRequestRequestTypeDef",
+    "ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef",
+    "ListClustersRequestListClustersPaginateTypeDef",
+    "ListControlPanelsRequestListControlPanelsPaginateTypeDef",
+    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
+    "ListSafetyRulesRequestListSafetyRulesPaginateTypeDef",
     "CreateSafetyRuleResponseTypeDef",
     "DescribeSafetyRuleResponseTypeDef",
     "RuleTypeDef",
     "UpdateSafetyRuleResponseTypeDef",
     "CreateSafetyRuleRequestRequestTypeDef",
     "CreateClusterResponseTypeDef",
     "DescribeClusterResponseTypeDef",
@@ -149,14 +149,25 @@
 
 class CreateClusterRequestRequestTypeDef(
     _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
 ):
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
 _RequiredCreateControlPanelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateControlPanelRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "ControlPanelName": str,
     },
 )
@@ -282,36 +293,24 @@
     {
         "Name": str,
         "SafetyRuleArn": str,
         "WaitPeriodMs": int,
     },
 )
 
-_RequiredListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef = TypedDict(
-    "_RequiredListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef",
-    {
-        "RoutingControlArn": str,
-    },
-)
-_OptionalListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef = TypedDict(
-    "_OptionalListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef",
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
-class ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef(
-    _RequiredListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
-    _OptionalListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAssociatedRoute53HealthChecksRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociatedRoute53HealthChecksRequestRequestTypeDef",
     {
         "RoutingControlArn": str,
     },
 )
 _OptionalListAssociatedRoute53HealthChecksRequestRequestTypeDef = TypedDict(
@@ -327,81 +326,33 @@
 class ListAssociatedRoute53HealthChecksRequestRequestTypeDef(
     _RequiredListAssociatedRoute53HealthChecksRequestRequestTypeDef,
     _OptionalListAssociatedRoute53HealthChecksRequestRequestTypeDef,
 ):
     pass
 
 
-ListAssociatedRoute53HealthChecksResponseTypeDef = TypedDict(
-    "ListAssociatedRoute53HealthChecksResponseTypeDef",
-    {
-        "HealthCheckIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListClustersRequestListClustersPaginateTypeDef = TypedDict(
-    "ListClustersRequestListClustersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListControlPanelsRequestListControlPanelsPaginateTypeDef = TypedDict(
-    "ListControlPanelsRequestListControlPanelsPaginateTypeDef",
-    {
-        "ClusterArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListControlPanelsRequestRequestTypeDef = TypedDict(
     "ListControlPanelsRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListRoutingControlsRequestListRoutingControlsPaginateTypeDef = TypedDict(
-    "_RequiredListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
-    {
-        "ControlPanelArn": str,
-    },
-)
-_OptionalListRoutingControlsRequestListRoutingControlsPaginateTypeDef = TypedDict(
-    "_OptionalListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRoutingControlsRequestListRoutingControlsPaginateTypeDef(
-    _RequiredListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
-    _OptionalListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRoutingControlsRequestRequestTypeDef = TypedDict(
     "_RequiredListRoutingControlsRequestRequestTypeDef",
     {
         "ControlPanelArn": str,
     },
 )
 _OptionalListRoutingControlsRequestRequestTypeDef = TypedDict(
@@ -417,36 +368,14 @@
 class ListRoutingControlsRequestRequestTypeDef(
     _RequiredListRoutingControlsRequestRequestTypeDef,
     _OptionalListRoutingControlsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListSafetyRulesRequestListSafetyRulesPaginateTypeDef = TypedDict(
-    "_RequiredListSafetyRulesRequestListSafetyRulesPaginateTypeDef",
-    {
-        "ControlPanelArn": str,
-    },
-)
-_OptionalListSafetyRulesRequestListSafetyRulesPaginateTypeDef = TypedDict(
-    "_OptionalListSafetyRulesRequestListSafetyRulesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSafetyRulesRequestListSafetyRulesPaginateTypeDef(
-    _RequiredListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
-    _OptionalListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSafetyRulesRequestRequestTypeDef = TypedDict(
     "_RequiredListSafetyRulesRequestRequestTypeDef",
     {
         "ControlPanelArn": str,
     },
 )
 _OptionalListSafetyRulesRequestRequestTypeDef = TypedDict(
@@ -468,43 +397,14 @@
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -594,73 +494,90 @@
     total=False,
 )
 
 CreateControlPanelResponseTypeDef = TypedDict(
     "CreateControlPanelResponseTypeDef",
     {
         "ControlPanel": ControlPanelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeControlPanelResponseTypeDef = TypedDict(
     "DescribeControlPanelResponseTypeDef",
     {
         "ControlPanel": ControlPanelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAssociatedRoute53HealthChecksResponseTypeDef = TypedDict(
+    "ListAssociatedRoute53HealthChecksResponseTypeDef",
+    {
+        "HealthCheckIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListControlPanelsResponseTypeDef = TypedDict(
     "ListControlPanelsResponseTypeDef",
     {
         "ControlPanels": List[ControlPanelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateControlPanelResponseTypeDef = TypedDict(
     "UpdateControlPanelResponseTypeDef",
     {
         "ControlPanel": ControlPanelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRoutingControlResponseTypeDef = TypedDict(
     "CreateRoutingControlResponseTypeDef",
     {
         "RoutingControl": RoutingControlTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRoutingControlResponseTypeDef = TypedDict(
     "DescribeRoutingControlResponseTypeDef",
     {
         "RoutingControl": RoutingControlTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRoutingControlsResponseTypeDef = TypedDict(
     "ListRoutingControlsResponseTypeDef",
     {
         "NextToken": str,
         "RoutingControls": List[RoutingControlTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRoutingControlResponseTypeDef = TypedDict(
     "UpdateRoutingControlResponseTypeDef",
     {
         "RoutingControl": RoutingControlTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeClusterRequestClusterCreatedWaitTypeDef = TypedDict(
     "_RequiredDescribeClusterRequestClusterCreatedWaitTypeDef",
     {
         "ClusterArn": str,
@@ -797,29 +714,112 @@
     {
         "AssertionRuleUpdate": AssertionRuleUpdateTypeDef,
         "GatingRuleUpdate": GatingRuleUpdateTypeDef,
     },
     total=False,
 )
 
+_RequiredListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef = TypedDict(
+    "_RequiredListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef",
+    {
+        "RoutingControlArn": str,
+    },
+)
+_OptionalListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef = TypedDict(
+    "_OptionalListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef(
+    _RequiredListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
+    _OptionalListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
+):
+    pass
+
+
+ListClustersRequestListClustersPaginateTypeDef = TypedDict(
+    "ListClustersRequestListClustersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListControlPanelsRequestListControlPanelsPaginateTypeDef = TypedDict(
+    "ListControlPanelsRequestListControlPanelsPaginateTypeDef",
+    {
+        "ClusterArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListRoutingControlsRequestListRoutingControlsPaginateTypeDef = TypedDict(
+    "_RequiredListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
+    {
+        "ControlPanelArn": str,
+    },
+)
+_OptionalListRoutingControlsRequestListRoutingControlsPaginateTypeDef = TypedDict(
+    "_OptionalListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRoutingControlsRequestListRoutingControlsPaginateTypeDef(
+    _RequiredListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
+    _OptionalListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListSafetyRulesRequestListSafetyRulesPaginateTypeDef = TypedDict(
+    "_RequiredListSafetyRulesRequestListSafetyRulesPaginateTypeDef",
+    {
+        "ControlPanelArn": str,
+    },
+)
+_OptionalListSafetyRulesRequestListSafetyRulesPaginateTypeDef = TypedDict(
+    "_OptionalListSafetyRulesRequestListSafetyRulesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListSafetyRulesRequestListSafetyRulesPaginateTypeDef(
+    _RequiredListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
+    _OptionalListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
+):
+    pass
+
+
 CreateSafetyRuleResponseTypeDef = TypedDict(
     "CreateSafetyRuleResponseTypeDef",
     {
         "AssertionRule": AssertionRuleTypeDef,
         "GatingRule": GatingRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSafetyRuleResponseTypeDef = TypedDict(
     "DescribeSafetyRuleResponseTypeDef",
     {
         "AssertionRule": AssertionRuleTypeDef,
         "GatingRule": GatingRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "ASSERTION": AssertionRuleTypeDef,
@@ -829,15 +829,15 @@
 )
 
 UpdateSafetyRuleResponseTypeDef = TypedDict(
     "UpdateSafetyRuleResponseTypeDef",
     {
         "AssertionRule": AssertionRuleTypeDef,
         "GatingRule": GatingRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSafetyRuleRequestRequestTypeDef = TypedDict(
     "CreateSafetyRuleRequestRequestTypeDef",
     {
         "AssertionRule": NewAssertionRuleTypeDef,
@@ -848,36 +848,36 @@
     total=False,
 )
 
 CreateClusterResponseTypeDef = TypedDict(
     "CreateClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeClusterResponseTypeDef = TypedDict(
     "DescribeClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListClustersResponseTypeDef = TypedDict(
     "ListClustersResponseTypeDef",
     {
         "Clusters": List[ClusterTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSafetyRulesResponseTypeDef = TypedDict(
     "ListSafetyRulesResponseTypeDef",
     {
         "NextToken": str,
         "SafetyRules": List[RuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config/type_defs.pyi` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_route53_recovery_control_config.type_defs import RuleConfigTypeDef
 
-    data: RuleConfigTypeDef = {...}
+    data: RuleConfigTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import RuleTypeType, StatusType
 
@@ -23,66 +23,66 @@
 
 __all__ = (
     "RuleConfigTypeDef",
     "AssertionRuleUpdateTypeDef",
     "ClusterEndpointTypeDef",
     "ControlPanelTypeDef",
     "CreateClusterRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateControlPanelRequestRequestTypeDef",
     "CreateRoutingControlRequestRequestTypeDef",
     "RoutingControlTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteControlPanelRequestRequestTypeDef",
     "DeleteRoutingControlRequestRequestTypeDef",
     "DeleteSafetyRuleRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeControlPanelRequestRequestTypeDef",
     "DescribeRoutingControlRequestRequestTypeDef",
     "DescribeSafetyRuleRequestRequestTypeDef",
     "GatingRuleUpdateTypeDef",
-    "ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAssociatedRoute53HealthChecksRequestRequestTypeDef",
-    "ListAssociatedRoute53HealthChecksResponseTypeDef",
-    "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
-    "ListControlPanelsRequestListControlPanelsPaginateTypeDef",
     "ListControlPanelsRequestRequestTypeDef",
-    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
     "ListRoutingControlsRequestRequestTypeDef",
-    "ListSafetyRulesRequestListSafetyRulesPaginateTypeDef",
     "ListSafetyRulesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateControlPanelRequestRequestTypeDef",
     "UpdateRoutingControlRequestRequestTypeDef",
     "AssertionRuleTypeDef",
     "GatingRuleTypeDef",
     "NewAssertionRuleTypeDef",
     "NewGatingRuleTypeDef",
     "ClusterTypeDef",
     "CreateControlPanelResponseTypeDef",
     "DescribeControlPanelResponseTypeDef",
+    "ListAssociatedRoute53HealthChecksResponseTypeDef",
     "ListControlPanelsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "UpdateControlPanelResponseTypeDef",
     "CreateRoutingControlResponseTypeDef",
     "DescribeRoutingControlResponseTypeDef",
     "ListRoutingControlsResponseTypeDef",
     "UpdateRoutingControlResponseTypeDef",
     "DescribeClusterRequestClusterCreatedWaitTypeDef",
     "DescribeClusterRequestClusterDeletedWaitTypeDef",
     "DescribeControlPanelRequestControlPanelCreatedWaitTypeDef",
     "DescribeControlPanelRequestControlPanelDeletedWaitTypeDef",
     "DescribeRoutingControlRequestRoutingControlCreatedWaitTypeDef",
     "DescribeRoutingControlRequestRoutingControlDeletedWaitTypeDef",
     "UpdateSafetyRuleRequestRequestTypeDef",
+    "ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef",
+    "ListClustersRequestListClustersPaginateTypeDef",
+    "ListControlPanelsRequestListControlPanelsPaginateTypeDef",
+    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
+    "ListSafetyRulesRequestListSafetyRulesPaginateTypeDef",
     "CreateSafetyRuleResponseTypeDef",
     "DescribeSafetyRuleResponseTypeDef",
     "RuleTypeDef",
     "UpdateSafetyRuleResponseTypeDef",
     "CreateSafetyRuleRequestRequestTypeDef",
     "CreateClusterResponseTypeDef",
     "DescribeClusterResponseTypeDef",
@@ -146,14 +146,25 @@
 )
 
 class CreateClusterRequestRequestTypeDef(
     _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
 ):
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
 _RequiredCreateControlPanelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateControlPanelRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "ControlPanelName": str,
     },
 )
@@ -275,34 +286,24 @@
     {
         "Name": str,
         "SafetyRuleArn": str,
         "WaitPeriodMs": int,
     },
 )
 
-_RequiredListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef = TypedDict(
-    "_RequiredListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef",
-    {
-        "RoutingControlArn": str,
-    },
-)
-_OptionalListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef = TypedDict(
-    "_OptionalListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef",
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
 
-class ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef(
-    _RequiredListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
-    _OptionalListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
-):
-    pass
-
 _RequiredListAssociatedRoute53HealthChecksRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociatedRoute53HealthChecksRequestRequestTypeDef",
     {
         "RoutingControlArn": str,
     },
 )
 _OptionalListAssociatedRoute53HealthChecksRequestRequestTypeDef = TypedDict(
@@ -316,79 +317,33 @@
 
 class ListAssociatedRoute53HealthChecksRequestRequestTypeDef(
     _RequiredListAssociatedRoute53HealthChecksRequestRequestTypeDef,
     _OptionalListAssociatedRoute53HealthChecksRequestRequestTypeDef,
 ):
     pass
 
-ListAssociatedRoute53HealthChecksResponseTypeDef = TypedDict(
-    "ListAssociatedRoute53HealthChecksResponseTypeDef",
-    {
-        "HealthCheckIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListClustersRequestListClustersPaginateTypeDef = TypedDict(
-    "ListClustersRequestListClustersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListControlPanelsRequestListControlPanelsPaginateTypeDef = TypedDict(
-    "ListControlPanelsRequestListControlPanelsPaginateTypeDef",
-    {
-        "ClusterArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListControlPanelsRequestRequestTypeDef = TypedDict(
     "ListControlPanelsRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListRoutingControlsRequestListRoutingControlsPaginateTypeDef = TypedDict(
-    "_RequiredListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
-    {
-        "ControlPanelArn": str,
-    },
-)
-_OptionalListRoutingControlsRequestListRoutingControlsPaginateTypeDef = TypedDict(
-    "_OptionalListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRoutingControlsRequestListRoutingControlsPaginateTypeDef(
-    _RequiredListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
-    _OptionalListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
-):
-    pass
-
 _RequiredListRoutingControlsRequestRequestTypeDef = TypedDict(
     "_RequiredListRoutingControlsRequestRequestTypeDef",
     {
         "ControlPanelArn": str,
     },
 )
 _OptionalListRoutingControlsRequestRequestTypeDef = TypedDict(
@@ -402,34 +357,14 @@
 
 class ListRoutingControlsRequestRequestTypeDef(
     _RequiredListRoutingControlsRequestRequestTypeDef,
     _OptionalListRoutingControlsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListSafetyRulesRequestListSafetyRulesPaginateTypeDef = TypedDict(
-    "_RequiredListSafetyRulesRequestListSafetyRulesPaginateTypeDef",
-    {
-        "ControlPanelArn": str,
-    },
-)
-_OptionalListSafetyRulesRequestListSafetyRulesPaginateTypeDef = TypedDict(
-    "_OptionalListSafetyRulesRequestListSafetyRulesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSafetyRulesRequestListSafetyRulesPaginateTypeDef(
-    _RequiredListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
-    _OptionalListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
-):
-    pass
-
 _RequiredListSafetyRulesRequestRequestTypeDef = TypedDict(
     "_RequiredListSafetyRulesRequestRequestTypeDef",
     {
         "ControlPanelArn": str,
     },
 )
 _OptionalListSafetyRulesRequestRequestTypeDef = TypedDict(
@@ -449,43 +384,14 @@
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -575,73 +481,90 @@
     total=False,
 )
 
 CreateControlPanelResponseTypeDef = TypedDict(
     "CreateControlPanelResponseTypeDef",
     {
         "ControlPanel": ControlPanelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeControlPanelResponseTypeDef = TypedDict(
     "DescribeControlPanelResponseTypeDef",
     {
         "ControlPanel": ControlPanelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAssociatedRoute53HealthChecksResponseTypeDef = TypedDict(
+    "ListAssociatedRoute53HealthChecksResponseTypeDef",
+    {
+        "HealthCheckIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListControlPanelsResponseTypeDef = TypedDict(
     "ListControlPanelsResponseTypeDef",
     {
         "ControlPanels": List[ControlPanelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateControlPanelResponseTypeDef = TypedDict(
     "UpdateControlPanelResponseTypeDef",
     {
         "ControlPanel": ControlPanelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRoutingControlResponseTypeDef = TypedDict(
     "CreateRoutingControlResponseTypeDef",
     {
         "RoutingControl": RoutingControlTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRoutingControlResponseTypeDef = TypedDict(
     "DescribeRoutingControlResponseTypeDef",
     {
         "RoutingControl": RoutingControlTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRoutingControlsResponseTypeDef = TypedDict(
     "ListRoutingControlsResponseTypeDef",
     {
         "NextToken": str,
         "RoutingControls": List[RoutingControlTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRoutingControlResponseTypeDef = TypedDict(
     "UpdateRoutingControlResponseTypeDef",
     {
         "RoutingControl": RoutingControlTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeClusterRequestClusterCreatedWaitTypeDef = TypedDict(
     "_RequiredDescribeClusterRequestClusterCreatedWaitTypeDef",
     {
         "ClusterArn": str,
@@ -766,29 +689,106 @@
     {
         "AssertionRuleUpdate": AssertionRuleUpdateTypeDef,
         "GatingRuleUpdate": GatingRuleUpdateTypeDef,
     },
     total=False,
 )
 
+_RequiredListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef = TypedDict(
+    "_RequiredListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef",
+    {
+        "RoutingControlArn": str,
+    },
+)
+_OptionalListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef = TypedDict(
+    "_OptionalListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef(
+    _RequiredListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
+    _OptionalListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
+):
+    pass
+
+ListClustersRequestListClustersPaginateTypeDef = TypedDict(
+    "ListClustersRequestListClustersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListControlPanelsRequestListControlPanelsPaginateTypeDef = TypedDict(
+    "ListControlPanelsRequestListControlPanelsPaginateTypeDef",
+    {
+        "ClusterArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListRoutingControlsRequestListRoutingControlsPaginateTypeDef = TypedDict(
+    "_RequiredListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
+    {
+        "ControlPanelArn": str,
+    },
+)
+_OptionalListRoutingControlsRequestListRoutingControlsPaginateTypeDef = TypedDict(
+    "_OptionalListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRoutingControlsRequestListRoutingControlsPaginateTypeDef(
+    _RequiredListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
+    _OptionalListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
+):
+    pass
+
+_RequiredListSafetyRulesRequestListSafetyRulesPaginateTypeDef = TypedDict(
+    "_RequiredListSafetyRulesRequestListSafetyRulesPaginateTypeDef",
+    {
+        "ControlPanelArn": str,
+    },
+)
+_OptionalListSafetyRulesRequestListSafetyRulesPaginateTypeDef = TypedDict(
+    "_OptionalListSafetyRulesRequestListSafetyRulesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListSafetyRulesRequestListSafetyRulesPaginateTypeDef(
+    _RequiredListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
+    _OptionalListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
+):
+    pass
+
 CreateSafetyRuleResponseTypeDef = TypedDict(
     "CreateSafetyRuleResponseTypeDef",
     {
         "AssertionRule": AssertionRuleTypeDef,
         "GatingRule": GatingRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSafetyRuleResponseTypeDef = TypedDict(
     "DescribeSafetyRuleResponseTypeDef",
     {
         "AssertionRule": AssertionRuleTypeDef,
         "GatingRule": GatingRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "ASSERTION": AssertionRuleTypeDef,
@@ -798,15 +798,15 @@
 )
 
 UpdateSafetyRuleResponseTypeDef = TypedDict(
     "UpdateSafetyRuleResponseTypeDef",
     {
         "AssertionRule": AssertionRuleTypeDef,
         "GatingRule": GatingRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSafetyRuleRequestRequestTypeDef = TypedDict(
     "CreateSafetyRuleRequestRequestTypeDef",
     {
         "AssertionRule": NewAssertionRuleTypeDef,
@@ -817,36 +817,36 @@
     total=False,
 )
 
 CreateClusterResponseTypeDef = TypedDict(
     "CreateClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeClusterResponseTypeDef = TypedDict(
     "DescribeClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListClustersResponseTypeDef = TypedDict(
     "ListClustersResponseTypeDef",
     {
         "Clusters": List[ClusterTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSafetyRulesResponseTypeDef = TypedDict(
     "ListSafetyRulesResponseTypeDef",
     {
         "NextToken": str,
         "SafetyRules": List[RuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config/waiter.py` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config/waiter.pyi` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config.egg-info/PKG-INFO` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-route53-recovery-control-config
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Route53RecoveryControlConfig 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Route53RecoveryControlConfig 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore route53-recovery-control-config type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore route53-recovery-control-config type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-route53-recovery-control-config"></a>
 
 # types-aiobotocore-route53-recovery-control-config
 
 [![PyPI - types-aiobotocore-route53-recovery-control-config](https://img.shields.io/pypi/v/types-aiobotocore-route53-recovery-control-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-control-config)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53-recovery-control-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-control-config)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-route53-recovery-control-config?color=blue)](https://pypistats.org/packages/types-aiobotocore-route53-recovery-control-config)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53-recovery-control-config)](https://pepy.tech/project/types-aiobotocore-route53-recovery-control-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Route53RecoveryControlConfig 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig)
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
 [types-aiobotocore-route53-recovery-control-config docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/).
 
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
@@ -384,94 +383,94 @@
 )
 
 
 def check_value(value: ClusterCreatedWaiterName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_route53_recovery_control_config.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from types_aiobotocore_route53_recovery_control_config.type_defs import (
     RuleConfigTypeDef,
     AssertionRuleUpdateTypeDef,
     ClusterEndpointTypeDef,
     ControlPanelTypeDef,
     CreateClusterRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     CreateControlPanelRequestRequestTypeDef,
     CreateRoutingControlRequestRequestTypeDef,
     RoutingControlTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteControlPanelRequestRequestTypeDef,
     DeleteRoutingControlRequestRequestTypeDef,
     DeleteSafetyRuleRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeControlPanelRequestRequestTypeDef,
     DescribeRoutingControlRequestRequestTypeDef,
     DescribeSafetyRuleRequestRequestTypeDef,
     GatingRuleUpdateTypeDef,
-    ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAssociatedRoute53HealthChecksRequestRequestTypeDef,
-    ListAssociatedRoute53HealthChecksResponseTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
-    ListControlPanelsRequestListControlPanelsPaginateTypeDef,
     ListControlPanelsRequestRequestTypeDef,
-    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
     ListRoutingControlsRequestRequestTypeDef,
-    ListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
     ListSafetyRulesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateControlPanelRequestRequestTypeDef,
     UpdateRoutingControlRequestRequestTypeDef,
     AssertionRuleTypeDef,
     GatingRuleTypeDef,
     NewAssertionRuleTypeDef,
     NewGatingRuleTypeDef,
     ClusterTypeDef,
     CreateControlPanelResponseTypeDef,
     DescribeControlPanelResponseTypeDef,
+    ListAssociatedRoute53HealthChecksResponseTypeDef,
     ListControlPanelsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     UpdateControlPanelResponseTypeDef,
     CreateRoutingControlResponseTypeDef,
     DescribeRoutingControlResponseTypeDef,
     ListRoutingControlsResponseTypeDef,
     UpdateRoutingControlResponseTypeDef,
     DescribeClusterRequestClusterCreatedWaitTypeDef,
     DescribeClusterRequestClusterDeletedWaitTypeDef,
     DescribeControlPanelRequestControlPanelCreatedWaitTypeDef,
     DescribeControlPanelRequestControlPanelDeletedWaitTypeDef,
     DescribeRoutingControlRequestRoutingControlCreatedWaitTypeDef,
     DescribeRoutingControlRequestRoutingControlDeletedWaitTypeDef,
     UpdateSafetyRuleRequestRequestTypeDef,
+    ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
+    ListControlPanelsRequestListControlPanelsPaginateTypeDef,
+    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
+    ListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
     CreateSafetyRuleResponseTypeDef,
     DescribeSafetyRuleResponseTypeDef,
     RuleTypeDef,
     UpdateSafetyRuleResponseTypeDef,
     CreateSafetyRuleRequestRequestTypeDef,
     CreateClusterResponseTypeDef,
     DescribeClusterResponseTypeDef,
     ListClustersResponseTypeDef,
     ListSafetyRulesResponseTypeDef,
 )
 
 
-def get_structure() -> RuleConfigTypeDef:
+def get_value() -> RuleConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2/types_aiobotocore_route53_recovery_control_config.egg-info/SOURCES.txt` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*


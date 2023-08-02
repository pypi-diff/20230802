# Comparing `tmp/types-aiobotocore-elb-2.5.2.tar.gz` & `tmp/types-aiobotocore-elb-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-elb-2.5.2.tar", last modified: Sat Jul  8 01:43:36 2023, max compression
+gzip compressed data, was "types-aiobotocore-elb-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:16 2023, max compression
```

## Comparing `types-aiobotocore-elb-2.5.2.tar` & `types-aiobotocore-elb-2.5.2.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:36.590112 types-aiobotocore-elb-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:30:30.000000 types-aiobotocore-elb-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17461 2023-07-08 01:43:36.590112 types-aiobotocore-elb-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15895 2023-07-08 01:30:30.000000 types-aiobotocore-elb-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:36.590112 types-aiobotocore-elb-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-08 01:30:30.000000 types-aiobotocore-elb-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:36.570111 types-aiobotocore-elb-2.5.2/types_aiobotocore_elb/
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-08 01:30:30.000000 types-aiobotocore-elb-2.5.2/types_aiobotocore_elb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-08 01:30:30.000000 types-aiobotocore-elb-2.5.2/types_aiobotocore_elb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-08 01:30:30.000000 types-aiobotocore-elb-2.5.2/types_aiobotocore_elb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26720 2023-07-08 01:30:30.000000 types-aiobotocore-elb-2.5.2/types_aiobotocore_elb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26677 2023-07-08 01:30:30.000000 types-aiobotocore-elb-2.5.2/types_aiobotocore_elb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-08 01:30:30.000000 types-aiobotocore-elb-2.5.2/types_aiobotocore_elb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-07-08 01:30:30.000000 types-aiobotocore-elb-2.5.2/types_aiobotocore_elb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-08 01:30:30.000000 types-aiobotocore-elb-2.5.2/types_aiobotocore_elb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-07-08 01:30:30.000000 types-aiobotocore-elb-2.5.2/types_aiobotocore_elb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:30:30.000000 types-aiobotocore-elb-2.5.2/types_aiobotocore_elb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24613 2023-07-08 01:30:31.000000 types-aiobotocore-elb-2.5.2/types_aiobotocore_elb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24590 2023-07-08 01:30:30.000000 types-aiobotocore-elb-2.5.2/types_aiobotocore_elb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:30:30.000000 types-aiobotocore-elb-2.5.2/types_aiobotocore_elb/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-07-08 01:30:30.000000 types-aiobotocore-elb-2.5.2/types_aiobotocore_elb/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-07-08 01:30:30.000000 types-aiobotocore-elb-2.5.2/types_aiobotocore_elb/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:36.590112 types-aiobotocore-elb-2.5.2/types_aiobotocore_elb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17461 2023-07-08 01:43:36.000000 types-aiobotocore-elb-2.5.2/types_aiobotocore_elb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-08 01:43:36.000000 types-aiobotocore-elb-2.5.2/types_aiobotocore_elb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:36.000000 types-aiobotocore-elb-2.5.2/types_aiobotocore_elb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:36.000000 types-aiobotocore-elb-2.5.2/types_aiobotocore_elb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:36.000000 types-aiobotocore-elb-2.5.2/types_aiobotocore_elb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:43:36.000000 types-aiobotocore-elb-2.5.2/types_aiobotocore_elb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:16.653589 types-aiobotocore-elb-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17478 2023-08-02 14:52:16.653589 types-aiobotocore-elb-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15959 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:16.653589 types-aiobotocore-elb-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:16.653589 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26730 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26687 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25207 2023-08-02 14:38:20.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25184 2023-08-02 14:38:20.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:16.653589 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17478 2023-08-02 14:52:16.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-02 14:52:16.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:16.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:16.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:16.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:16.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-elb-2.5.2/LICENSE` & `types-aiobotocore-elb-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elb-2.5.2/PKG-INFO` & `types-aiobotocore-elb-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elb
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ElasticLoadBalancing 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ElasticLoadBalancing 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore elb type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore elb type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-elb"></a>
 
 # types-aiobotocore-elb
 
 [![PyPI - types-aiobotocore-elb](https://img.shields.io/pypi/v/types-aiobotocore-elb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-elb?color=blue)](https://pypistats.org/packages/types-aiobotocore-elb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elb)](https://pepy.tech/project/types-aiobotocore-elb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ElasticLoadBalancing 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
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
 [types-aiobotocore-elb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/).
 
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
@@ -350,107 +349,109 @@
 )
 
 
 def check_value(value: AnyInstanceInServiceWaiterName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_elb.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_elb.type_defs import (
     AccessLogTypeDef,
     AddAvailabilityZonesInputRequestTypeDef,
-    AddAvailabilityZonesOutputTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     AdditionalAttributeTypeDef,
     AppCookieStickinessPolicyTypeDef,
     ApplySecurityGroupsToLoadBalancerInputRequestTypeDef,
-    ApplySecurityGroupsToLoadBalancerOutputTypeDef,
     AttachLoadBalancerToSubnetsInputRequestTypeDef,
-    AttachLoadBalancerToSubnetsOutputTypeDef,
     BackendServerDescriptionTypeDef,
     HealthCheckTypeDef,
     ConnectionDrainingTypeDef,
     ConnectionSettingsTypeDef,
     ListenerTypeDef,
-    CreateAccessPointOutputTypeDef,
     CreateAppCookieStickinessPolicyInputRequestTypeDef,
     CreateLBCookieStickinessPolicyInputRequestTypeDef,
     PolicyAttributeTypeDef,
     CrossZoneLoadBalancingTypeDef,
     DeleteAccessPointInputRequestTypeDef,
     DeleteLoadBalancerListenerInputRequestTypeDef,
     DeleteLoadBalancerPolicyInputRequestTypeDef,
     InstanceTypeDef,
-    DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAccessPointsInputRequestTypeDef,
-    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     LimitTypeDef,
     WaiterConfigTypeDef,
     InstanceStateTypeDef,
     DescribeLoadBalancerAttributesInputRequestTypeDef,
     DescribeLoadBalancerPoliciesInputRequestTypeDef,
     DescribeLoadBalancerPolicyTypesInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
     DetachLoadBalancerFromSubnetsInputRequestTypeDef,
-    DetachLoadBalancerFromSubnetsOutputTypeDef,
     LBCookieStickinessPolicyTypeDef,
     SourceSecurityGroupTypeDef,
-    PaginatorConfigTypeDef,
     PolicyAttributeDescriptionTypeDef,
     PolicyAttributeTypeDescriptionTypeDef,
     RemoveAvailabilityZonesInputRequestTypeDef,
-    RemoveAvailabilityZonesOutputTypeDef,
     TagKeyOnlyTypeDef,
-    ResponseMetadataTypeDef,
     SetLoadBalancerListenerSSLCertificateInputRequestTypeDef,
     SetLoadBalancerPoliciesForBackendServerInputRequestTypeDef,
     SetLoadBalancerPoliciesOfListenerInputRequestTypeDef,
+    AddAvailabilityZonesOutputTypeDef,
+    ApplySecurityGroupsToLoadBalancerOutputTypeDef,
+    AttachLoadBalancerToSubnetsOutputTypeDef,
+    CreateAccessPointOutputTypeDef,
+    DetachLoadBalancerFromSubnetsOutputTypeDef,
+    RemoveAvailabilityZonesOutputTypeDef,
     AddTagsInputRequestTypeDef,
     TagDescriptionTypeDef,
     ConfigureHealthCheckInputRequestTypeDef,
     ConfigureHealthCheckOutputTypeDef,
     CreateAccessPointInputRequestTypeDef,
     CreateLoadBalancerListenerInputRequestTypeDef,
     ListenerDescriptionTypeDef,
     CreateLoadBalancerPolicyInputRequestTypeDef,
+    LoadBalancerAttributesOutputTypeDef,
     LoadBalancerAttributesTypeDef,
     DeregisterEndPointsInputRequestTypeDef,
     DeregisterEndPointsOutputTypeDef,
     DescribeEndPointStateInputRequestTypeDef,
     RegisterEndPointsInputRequestTypeDef,
     RegisterEndPointsOutputTypeDef,
+    DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef,
+    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsOutputTypeDef,
     DescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef,
     DescribeEndPointStateInputInstanceDeregisteredWaitTypeDef,
     DescribeEndPointStateInputInstanceInServiceWaitTypeDef,
     DescribeEndPointStateOutputTypeDef,
     PoliciesTypeDef,
     PolicyDescriptionTypeDef,
     PolicyTypeDescriptionTypeDef,
     RemoveTagsInputRequestTypeDef,
     DescribeTagsOutputTypeDef,
     DescribeLoadBalancerAttributesOutputTypeDef,
-    ModifyLoadBalancerAttributesInputRequestTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
+    LoadBalancerAttributesUnionTypeDef,
+    ModifyLoadBalancerAttributesInputRequestTypeDef,
     LoadBalancerDescriptionTypeDef,
     DescribeLoadBalancerPoliciesOutputTypeDef,
     DescribeLoadBalancerPolicyTypesOutputTypeDef,
     DescribeAccessPointsOutputTypeDef,
 )
 
 
-def get_structure() -> AccessLogTypeDef:
+def get_value() -> AccessLogTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-elb-2.5.2/README.md` & `types-aiobotocore-elb-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-elb"></a>
 
 # types-aiobotocore-elb
 
 [![PyPI - types-aiobotocore-elb](https://img.shields.io/pypi/v/types-aiobotocore-elb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-elb?color=blue)](https://pypistats.org/packages/types-aiobotocore-elb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elb)](https://pepy.tech/project/types-aiobotocore-elb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ElasticLoadBalancing 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
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
 [types-aiobotocore-elb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/).
 
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
@@ -317,107 +317,109 @@
 )
 
 
 def check_value(value: AnyInstanceInServiceWaiterName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_elb.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_elb.type_defs import (
     AccessLogTypeDef,
     AddAvailabilityZonesInputRequestTypeDef,
-    AddAvailabilityZonesOutputTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     AdditionalAttributeTypeDef,
     AppCookieStickinessPolicyTypeDef,
     ApplySecurityGroupsToLoadBalancerInputRequestTypeDef,
-    ApplySecurityGroupsToLoadBalancerOutputTypeDef,
     AttachLoadBalancerToSubnetsInputRequestTypeDef,
-    AttachLoadBalancerToSubnetsOutputTypeDef,
     BackendServerDescriptionTypeDef,
     HealthCheckTypeDef,
     ConnectionDrainingTypeDef,
     ConnectionSettingsTypeDef,
     ListenerTypeDef,
-    CreateAccessPointOutputTypeDef,
     CreateAppCookieStickinessPolicyInputRequestTypeDef,
     CreateLBCookieStickinessPolicyInputRequestTypeDef,
     PolicyAttributeTypeDef,
     CrossZoneLoadBalancingTypeDef,
     DeleteAccessPointInputRequestTypeDef,
     DeleteLoadBalancerListenerInputRequestTypeDef,
     DeleteLoadBalancerPolicyInputRequestTypeDef,
     InstanceTypeDef,
-    DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAccessPointsInputRequestTypeDef,
-    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     LimitTypeDef,
     WaiterConfigTypeDef,
     InstanceStateTypeDef,
     DescribeLoadBalancerAttributesInputRequestTypeDef,
     DescribeLoadBalancerPoliciesInputRequestTypeDef,
     DescribeLoadBalancerPolicyTypesInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
     DetachLoadBalancerFromSubnetsInputRequestTypeDef,
-    DetachLoadBalancerFromSubnetsOutputTypeDef,
     LBCookieStickinessPolicyTypeDef,
     SourceSecurityGroupTypeDef,
-    PaginatorConfigTypeDef,
     PolicyAttributeDescriptionTypeDef,
     PolicyAttributeTypeDescriptionTypeDef,
     RemoveAvailabilityZonesInputRequestTypeDef,
-    RemoveAvailabilityZonesOutputTypeDef,
     TagKeyOnlyTypeDef,
-    ResponseMetadataTypeDef,
     SetLoadBalancerListenerSSLCertificateInputRequestTypeDef,
     SetLoadBalancerPoliciesForBackendServerInputRequestTypeDef,
     SetLoadBalancerPoliciesOfListenerInputRequestTypeDef,
+    AddAvailabilityZonesOutputTypeDef,
+    ApplySecurityGroupsToLoadBalancerOutputTypeDef,
+    AttachLoadBalancerToSubnetsOutputTypeDef,
+    CreateAccessPointOutputTypeDef,
+    DetachLoadBalancerFromSubnetsOutputTypeDef,
+    RemoveAvailabilityZonesOutputTypeDef,
     AddTagsInputRequestTypeDef,
     TagDescriptionTypeDef,
     ConfigureHealthCheckInputRequestTypeDef,
     ConfigureHealthCheckOutputTypeDef,
     CreateAccessPointInputRequestTypeDef,
     CreateLoadBalancerListenerInputRequestTypeDef,
     ListenerDescriptionTypeDef,
     CreateLoadBalancerPolicyInputRequestTypeDef,
+    LoadBalancerAttributesOutputTypeDef,
     LoadBalancerAttributesTypeDef,
     DeregisterEndPointsInputRequestTypeDef,
     DeregisterEndPointsOutputTypeDef,
     DescribeEndPointStateInputRequestTypeDef,
     RegisterEndPointsInputRequestTypeDef,
     RegisterEndPointsOutputTypeDef,
+    DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef,
+    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsOutputTypeDef,
     DescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef,
     DescribeEndPointStateInputInstanceDeregisteredWaitTypeDef,
     DescribeEndPointStateInputInstanceInServiceWaitTypeDef,
     DescribeEndPointStateOutputTypeDef,
     PoliciesTypeDef,
     PolicyDescriptionTypeDef,
     PolicyTypeDescriptionTypeDef,
     RemoveTagsInputRequestTypeDef,
     DescribeTagsOutputTypeDef,
     DescribeLoadBalancerAttributesOutputTypeDef,
-    ModifyLoadBalancerAttributesInputRequestTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
+    LoadBalancerAttributesUnionTypeDef,
+    ModifyLoadBalancerAttributesInputRequestTypeDef,
     LoadBalancerDescriptionTypeDef,
     DescribeLoadBalancerPoliciesOutputTypeDef,
     DescribeLoadBalancerPolicyTypesOutputTypeDef,
     DescribeAccessPointsOutputTypeDef,
 )
 
 
-def get_structure() -> AccessLogTypeDef:
+def get_value() -> AccessLogTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-elb-2.5.2/setup.py` & `types-aiobotocore-elb-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-elb",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_elb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ElasticLoadBalancing 2.5.2 service generated with"
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
-    keywords="aiobotocore elb type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore elb type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_elb": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-elb-2.5.2/types_aiobotocore_elb/__init__.py` & `types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elb-2.5.2/types_aiobotocore_elb/__init__.pyi` & `types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elb-2.5.2/types_aiobotocore_elb/__main__.py` & `types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ElasticLoadBalancing 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing\nOther"
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

### Comparing `types-aiobotocore-elb-2.5.2/types_aiobotocore_elb/client.py` & `types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     DescribeLoadBalancerPoliciesOutputTypeDef,
     DescribeLoadBalancerPolicyTypesOutputTypeDef,
     DescribeTagsOutputTypeDef,
     DetachLoadBalancerFromSubnetsOutputTypeDef,
     HealthCheckTypeDef,
     InstanceTypeDef,
     ListenerTypeDef,
-    LoadBalancerAttributesTypeDef,
+    LoadBalancerAttributesUnionTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
     PolicyAttributeTypeDef,
     RegisterEndPointsOutputTypeDef,
     RemoveAvailabilityZonesOutputTypeDef,
     TagKeyOnlyTypeDef,
     TagTypeDef,
 )
@@ -386,15 +386,15 @@
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/client/#generate_presigned_url)
         """
 
     async def modify_load_balancer_attributes(
-        self, *, LoadBalancerName: str, LoadBalancerAttributes: LoadBalancerAttributesTypeDef
+        self, *, LoadBalancerName: str, LoadBalancerAttributes: LoadBalancerAttributesUnionTypeDef
     ) -> ModifyLoadBalancerAttributesOutputTypeDef:
         """
         Modifies the attributes of the specified load balancer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Client.modify_load_balancer_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/client/#modify_load_balancer_attributes)
         """
```

### Comparing `types-aiobotocore-elb-2.5.2/types_aiobotocore_elb/client.pyi` & `types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     DescribeLoadBalancerPoliciesOutputTypeDef,
     DescribeLoadBalancerPolicyTypesOutputTypeDef,
     DescribeTagsOutputTypeDef,
     DetachLoadBalancerFromSubnetsOutputTypeDef,
     HealthCheckTypeDef,
     InstanceTypeDef,
     ListenerTypeDef,
-    LoadBalancerAttributesTypeDef,
+    LoadBalancerAttributesUnionTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
     PolicyAttributeTypeDef,
     RegisterEndPointsOutputTypeDef,
     RemoveAvailabilityZonesOutputTypeDef,
     TagKeyOnlyTypeDef,
     TagTypeDef,
 )
@@ -355,15 +355,15 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/client/#generate_presigned_url)
         """
     async def modify_load_balancer_attributes(
-        self, *, LoadBalancerName: str, LoadBalancerAttributes: LoadBalancerAttributesTypeDef
+        self, *, LoadBalancerName: str, LoadBalancerAttributes: LoadBalancerAttributesUnionTypeDef
     ) -> ModifyLoadBalancerAttributesOutputTypeDef:
         """
         Modifies the attributes of the specified load balancer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Client.modify_load_balancer_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/client/#modify_load_balancer_attributes)
         """
```

### Comparing `types-aiobotocore-elb-2.5.2/types_aiobotocore_elb/literals.py` & `types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elb-2.5.2/types_aiobotocore_elb/literals.pyi` & `types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elb-2.5.2/types_aiobotocore_elb/paginator.py` & `types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 class DescribeAccountLimitsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Paginator.DescribeAccountLimits)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/paginators/#describeaccountlimitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAccountLimitsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Paginator.DescribeAccountLimits.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/paginators/#describeaccountlimitspaginator)
         """
 
 
@@ -67,13 +67,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/paginators/#describeloadbalancerspaginator)
     """
 
     def paginate(
         self,
         *,
         LoadBalancerNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAccessPointsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Paginator.DescribeLoadBalancers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/paginators/#describeloadbalancerspaginator)
         """
```

### Comparing `types-aiobotocore-elb-2.5.2/types_aiobotocore_elb/paginator.pyi` & `types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/paginator.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 class DescribeAccountLimitsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Paginator.DescribeAccountLimits)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/paginators/#describeaccountlimitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAccountLimitsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Paginator.DescribeAccountLimits.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/paginators/#describeaccountlimitspaginator)
         """
 
 class DescribeLoadBalancersPaginator(AioPaginator):
@@ -63,13 +63,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/paginators/#describeloadbalancerspaginator)
     """
 
     def paginate(
         self,
         *,
         LoadBalancerNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAccessPointsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Paginator.DescribeLoadBalancers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/paginators/#describeloadbalancerspaginator)
         """
```

### Comparing `types-aiobotocore-elb-2.5.2/types_aiobotocore_elb/type_defs.py` & `types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,104 +4,105 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_elb.type_defs import AccessLogTypeDef
 
-    data: AccessLogTypeDef = {...}
+    data: AccessLogTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccessLogTypeDef",
     "AddAvailabilityZonesInputRequestTypeDef",
-    "AddAvailabilityZonesOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "AdditionalAttributeTypeDef",
     "AppCookieStickinessPolicyTypeDef",
     "ApplySecurityGroupsToLoadBalancerInputRequestTypeDef",
-    "ApplySecurityGroupsToLoadBalancerOutputTypeDef",
     "AttachLoadBalancerToSubnetsInputRequestTypeDef",
-    "AttachLoadBalancerToSubnetsOutputTypeDef",
     "BackendServerDescriptionTypeDef",
     "HealthCheckTypeDef",
     "ConnectionDrainingTypeDef",
     "ConnectionSettingsTypeDef",
     "ListenerTypeDef",
-    "CreateAccessPointOutputTypeDef",
     "CreateAppCookieStickinessPolicyInputRequestTypeDef",
     "CreateLBCookieStickinessPolicyInputRequestTypeDef",
     "PolicyAttributeTypeDef",
     "CrossZoneLoadBalancingTypeDef",
     "DeleteAccessPointInputRequestTypeDef",
     "DeleteLoadBalancerListenerInputRequestTypeDef",
     "DeleteLoadBalancerPolicyInputRequestTypeDef",
     "InstanceTypeDef",
-    "DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAccessPointsInputRequestTypeDef",
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
     "DescribeAccountLimitsInputRequestTypeDef",
     "LimitTypeDef",
     "WaiterConfigTypeDef",
     "InstanceStateTypeDef",
     "DescribeLoadBalancerAttributesInputRequestTypeDef",
     "DescribeLoadBalancerPoliciesInputRequestTypeDef",
     "DescribeLoadBalancerPolicyTypesInputRequestTypeDef",
     "DescribeTagsInputRequestTypeDef",
     "DetachLoadBalancerFromSubnetsInputRequestTypeDef",
-    "DetachLoadBalancerFromSubnetsOutputTypeDef",
     "LBCookieStickinessPolicyTypeDef",
     "SourceSecurityGroupTypeDef",
-    "PaginatorConfigTypeDef",
     "PolicyAttributeDescriptionTypeDef",
     "PolicyAttributeTypeDescriptionTypeDef",
     "RemoveAvailabilityZonesInputRequestTypeDef",
-    "RemoveAvailabilityZonesOutputTypeDef",
     "TagKeyOnlyTypeDef",
-    "ResponseMetadataTypeDef",
     "SetLoadBalancerListenerSSLCertificateInputRequestTypeDef",
     "SetLoadBalancerPoliciesForBackendServerInputRequestTypeDef",
     "SetLoadBalancerPoliciesOfListenerInputRequestTypeDef",
+    "AddAvailabilityZonesOutputTypeDef",
+    "ApplySecurityGroupsToLoadBalancerOutputTypeDef",
+    "AttachLoadBalancerToSubnetsOutputTypeDef",
+    "CreateAccessPointOutputTypeDef",
+    "DetachLoadBalancerFromSubnetsOutputTypeDef",
+    "RemoveAvailabilityZonesOutputTypeDef",
     "AddTagsInputRequestTypeDef",
     "TagDescriptionTypeDef",
     "ConfigureHealthCheckInputRequestTypeDef",
     "ConfigureHealthCheckOutputTypeDef",
     "CreateAccessPointInputRequestTypeDef",
     "CreateLoadBalancerListenerInputRequestTypeDef",
     "ListenerDescriptionTypeDef",
     "CreateLoadBalancerPolicyInputRequestTypeDef",
+    "LoadBalancerAttributesOutputTypeDef",
     "LoadBalancerAttributesTypeDef",
     "DeregisterEndPointsInputRequestTypeDef",
     "DeregisterEndPointsOutputTypeDef",
     "DescribeEndPointStateInputRequestTypeDef",
     "RegisterEndPointsInputRequestTypeDef",
     "RegisterEndPointsOutputTypeDef",
+    "DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef",
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
     "DescribeAccountLimitsOutputTypeDef",
     "DescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef",
     "DescribeEndPointStateInputInstanceDeregisteredWaitTypeDef",
     "DescribeEndPointStateInputInstanceInServiceWaitTypeDef",
     "DescribeEndPointStateOutputTypeDef",
     "PoliciesTypeDef",
     "PolicyDescriptionTypeDef",
     "PolicyTypeDescriptionTypeDef",
     "RemoveTagsInputRequestTypeDef",
     "DescribeTagsOutputTypeDef",
     "DescribeLoadBalancerAttributesOutputTypeDef",
-    "ModifyLoadBalancerAttributesInputRequestTypeDef",
     "ModifyLoadBalancerAttributesOutputTypeDef",
+    "LoadBalancerAttributesUnionTypeDef",
+    "ModifyLoadBalancerAttributesInputRequestTypeDef",
     "LoadBalancerDescriptionTypeDef",
     "DescribeLoadBalancerPoliciesOutputTypeDef",
     "DescribeLoadBalancerPolicyTypesOutputTypeDef",
     "DescribeAccessPointsOutputTypeDef",
 )
 
 _RequiredAccessLogTypeDef = TypedDict(
@@ -116,32 +117,33 @@
         "S3BucketName": str,
         "EmitInterval": int,
         "S3BucketPrefix": str,
     },
     total=False,
 )
 
-
 class AccessLogTypeDef(_RequiredAccessLogTypeDef, _OptionalAccessLogTypeDef):
     pass
 
-
 AddAvailabilityZonesInputRequestTypeDef = TypedDict(
     "AddAvailabilityZonesInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "AvailabilityZones": Sequence[str],
     },
 )
 
-AddAvailabilityZonesOutputTypeDef = TypedDict(
-    "AddAvailabilityZonesOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AvailabilityZones": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
@@ -151,19 +153,17 @@
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
-
 AdditionalAttributeTypeDef = TypedDict(
     "AdditionalAttributeTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -182,38 +182,22 @@
     "ApplySecurityGroupsToLoadBalancerInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "SecurityGroups": Sequence[str],
     },
 )
 
-ApplySecurityGroupsToLoadBalancerOutputTypeDef = TypedDict(
-    "ApplySecurityGroupsToLoadBalancerOutputTypeDef",
-    {
-        "SecurityGroups": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AttachLoadBalancerToSubnetsInputRequestTypeDef = TypedDict(
     "AttachLoadBalancerToSubnetsInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "Subnets": Sequence[str],
     },
 )
 
-AttachLoadBalancerToSubnetsOutputTypeDef = TypedDict(
-    "AttachLoadBalancerToSubnetsOutputTypeDef",
-    {
-        "Subnets": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BackendServerDescriptionTypeDef = TypedDict(
     "BackendServerDescriptionTypeDef",
     {
         "InstancePort": int,
         "PolicyNames": List[str],
     },
     total=False,
@@ -240,21 +224,19 @@
     "_OptionalConnectionDrainingTypeDef",
     {
         "Timeout": int,
     },
     total=False,
 )
 
-
 class ConnectionDrainingTypeDef(
     _RequiredConnectionDrainingTypeDef, _OptionalConnectionDrainingTypeDef
 ):
     pass
 
-
 ConnectionSettingsTypeDef = TypedDict(
     "ConnectionSettingsTypeDef",
     {
         "IdleTimeout": int,
     },
 )
 
@@ -271,27 +253,17 @@
     {
         "InstanceProtocol": str,
         "SSLCertificateId": str,
     },
     total=False,
 )
 
-
 class ListenerTypeDef(_RequiredListenerTypeDef, _OptionalListenerTypeDef):
     pass
 
-
-CreateAccessPointOutputTypeDef = TypedDict(
-    "CreateAccessPointOutputTypeDef",
-    {
-        "DNSName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateAppCookieStickinessPolicyInputRequestTypeDef = TypedDict(
     "CreateAppCookieStickinessPolicyInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "PolicyName": str,
         "CookieName": str,
     },
@@ -308,22 +280,20 @@
     "_OptionalCreateLBCookieStickinessPolicyInputRequestTypeDef",
     {
         "CookieExpirationPeriod": int,
     },
     total=False,
 )
 
-
 class CreateLBCookieStickinessPolicyInputRequestTypeDef(
     _RequiredCreateLBCookieStickinessPolicyInputRequestTypeDef,
     _OptionalCreateLBCookieStickinessPolicyInputRequestTypeDef,
 ):
     pass
 
-
 PolicyAttributeTypeDef = TypedDict(
     "PolicyAttributeTypeDef",
     {
         "AttributeName": str,
         "AttributeValue": str,
     },
     total=False,
@@ -363,41 +333,34 @@
     "InstanceTypeDef",
     {
         "InstanceId": str,
     },
     total=False,
 )
 
-DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef = TypedDict(
-    "DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "LoadBalancerNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeAccessPointsInputRequestTypeDef = TypedDict(
     "DescribeAccessPointsInputRequestTypeDef",
     {
         "LoadBalancerNames": Sequence[str],
         "Marker": str,
         "PageSize": int,
     },
     total=False,
 )
 
-DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeAccountLimitsInputRequestTypeDef = TypedDict(
     "DescribeAccountLimitsInputRequestTypeDef",
     {
         "Marker": str,
         "PageSize": int,
     },
     total=False,
@@ -467,22 +430,14 @@
     "DetachLoadBalancerFromSubnetsInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "Subnets": Sequence[str],
     },
 )
 
-DetachLoadBalancerFromSubnetsOutputTypeDef = TypedDict(
-    "DetachLoadBalancerFromSubnetsOutputTypeDef",
-    {
-        "Subnets": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LBCookieStickinessPolicyTypeDef = TypedDict(
     "LBCookieStickinessPolicyTypeDef",
     {
         "PolicyName": str,
         "CookieExpirationPeriod": int,
     },
     total=False,
@@ -493,24 +448,14 @@
     {
         "OwnerAlias": str,
         "GroupName": str,
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
 PolicyAttributeDescriptionTypeDef = TypedDict(
     "PolicyAttributeDescriptionTypeDef",
     {
         "AttributeName": str,
         "AttributeValue": str,
     },
     total=False,
@@ -532,41 +477,22 @@
     "RemoveAvailabilityZonesInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "AvailabilityZones": Sequence[str],
     },
 )
 
-RemoveAvailabilityZonesOutputTypeDef = TypedDict(
-    "RemoveAvailabilityZonesOutputTypeDef",
-    {
-        "AvailabilityZones": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagKeyOnlyTypeDef = TypedDict(
     "TagKeyOnlyTypeDef",
     {
         "Key": str,
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
 SetLoadBalancerListenerSSLCertificateInputRequestTypeDef = TypedDict(
     "SetLoadBalancerListenerSSLCertificateInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "LoadBalancerPort": int,
         "SSLCertificateId": str,
     },
@@ -586,14 +512,62 @@
     {
         "LoadBalancerName": str,
         "LoadBalancerPort": int,
         "PolicyNames": Sequence[str],
     },
 )
 
+AddAvailabilityZonesOutputTypeDef = TypedDict(
+    "AddAvailabilityZonesOutputTypeDef",
+    {
+        "AvailabilityZones": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ApplySecurityGroupsToLoadBalancerOutputTypeDef = TypedDict(
+    "ApplySecurityGroupsToLoadBalancerOutputTypeDef",
+    {
+        "SecurityGroups": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AttachLoadBalancerToSubnetsOutputTypeDef = TypedDict(
+    "AttachLoadBalancerToSubnetsOutputTypeDef",
+    {
+        "Subnets": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAccessPointOutputTypeDef = TypedDict(
+    "CreateAccessPointOutputTypeDef",
+    {
+        "DNSName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DetachLoadBalancerFromSubnetsOutputTypeDef = TypedDict(
+    "DetachLoadBalancerFromSubnetsOutputTypeDef",
+    {
+        "Subnets": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemoveAvailabilityZonesOutputTypeDef = TypedDict(
+    "RemoveAvailabilityZonesOutputTypeDef",
+    {
+        "AvailabilityZones": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AddTagsInputRequestTypeDef = TypedDict(
     "AddTagsInputRequestTypeDef",
     {
         "LoadBalancerNames": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -615,15 +589,15 @@
     },
 )
 
 ConfigureHealthCheckOutputTypeDef = TypedDict(
     "ConfigureHealthCheckOutputTypeDef",
     {
         "HealthCheck": HealthCheckTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateAccessPointInputRequestTypeDef = TypedDict(
     "_RequiredCreateAccessPointInputRequestTypeDef",
     {
         "LoadBalancerName": str,
@@ -638,21 +612,19 @@
         "SecurityGroups": Sequence[str],
         "Scheme": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateAccessPointInputRequestTypeDef(
     _RequiredCreateAccessPointInputRequestTypeDef, _OptionalCreateAccessPointInputRequestTypeDef
 ):
     pass
 
-
 CreateLoadBalancerListenerInputRequestTypeDef = TypedDict(
     "CreateLoadBalancerListenerInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "Listeners": Sequence[ListenerTypeDef],
     },
 )
@@ -678,30 +650,40 @@
     "_OptionalCreateLoadBalancerPolicyInputRequestTypeDef",
     {
         "PolicyAttributes": Sequence[PolicyAttributeTypeDef],
     },
     total=False,
 )
 
-
 class CreateLoadBalancerPolicyInputRequestTypeDef(
     _RequiredCreateLoadBalancerPolicyInputRequestTypeDef,
     _OptionalCreateLoadBalancerPolicyInputRequestTypeDef,
 ):
     pass
 
+LoadBalancerAttributesOutputTypeDef = TypedDict(
+    "LoadBalancerAttributesOutputTypeDef",
+    {
+        "CrossZoneLoadBalancing": CrossZoneLoadBalancingTypeDef,
+        "AccessLog": AccessLogTypeDef,
+        "ConnectionDraining": ConnectionDrainingTypeDef,
+        "ConnectionSettings": ConnectionSettingsTypeDef,
+        "AdditionalAttributes": List[AdditionalAttributeTypeDef],
+    },
+    total=False,
+)
 
 LoadBalancerAttributesTypeDef = TypedDict(
     "LoadBalancerAttributesTypeDef",
     {
         "CrossZoneLoadBalancing": CrossZoneLoadBalancingTypeDef,
         "AccessLog": AccessLogTypeDef,
         "ConnectionDraining": ConnectionDrainingTypeDef,
         "ConnectionSettings": ConnectionSettingsTypeDef,
-        "AdditionalAttributes": List[AdditionalAttributeTypeDef],
+        "AdditionalAttributes": Sequence[AdditionalAttributeTypeDef],
     },
     total=False,
 )
 
 DeregisterEndPointsInputRequestTypeDef = TypedDict(
     "DeregisterEndPointsInputRequestTypeDef",
     {
@@ -710,15 +692,15 @@
     },
 )
 
 DeregisterEndPointsOutputTypeDef = TypedDict(
     "DeregisterEndPointsOutputTypeDef",
     {
         "Instances": List[InstanceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeEndPointStateInputRequestTypeDef = TypedDict(
     "_RequiredDescribeEndPointStateInputRequestTypeDef",
     {
         "LoadBalancerName": str,
@@ -728,44 +710,59 @@
     "_OptionalDescribeEndPointStateInputRequestTypeDef",
     {
         "Instances": Sequence[InstanceTypeDef],
     },
     total=False,
 )
 
-
 class DescribeEndPointStateInputRequestTypeDef(
     _RequiredDescribeEndPointStateInputRequestTypeDef,
     _OptionalDescribeEndPointStateInputRequestTypeDef,
 ):
     pass
 
-
 RegisterEndPointsInputRequestTypeDef = TypedDict(
     "RegisterEndPointsInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "Instances": Sequence[InstanceTypeDef],
     },
 )
 
 RegisterEndPointsOutputTypeDef = TypedDict(
     "RegisterEndPointsOutputTypeDef",
     {
         "Instances": List[InstanceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef = TypedDict(
+    "DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef",
+    {
+        "LoadBalancerNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 DescribeAccountLimitsOutputTypeDef = TypedDict(
     "DescribeAccountLimitsOutputTypeDef",
     {
         "Limits": List[LimitTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef = TypedDict(
     "_RequiredDescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef",
     {
         "LoadBalancerName": str,
@@ -776,22 +773,20 @@
     {
         "Instances": Sequence[InstanceTypeDef],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef(
     _RequiredDescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef,
     _OptionalDescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeEndPointStateInputInstanceDeregisteredWaitTypeDef = TypedDict(
     "_RequiredDescribeEndPointStateInputInstanceDeregisteredWaitTypeDef",
     {
         "LoadBalancerName": str,
     },
 )
 _OptionalDescribeEndPointStateInputInstanceDeregisteredWaitTypeDef = TypedDict(
@@ -799,22 +794,20 @@
     {
         "Instances": Sequence[InstanceTypeDef],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeEndPointStateInputInstanceDeregisteredWaitTypeDef(
     _RequiredDescribeEndPointStateInputInstanceDeregisteredWaitTypeDef,
     _OptionalDescribeEndPointStateInputInstanceDeregisteredWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeEndPointStateInputInstanceInServiceWaitTypeDef = TypedDict(
     "_RequiredDescribeEndPointStateInputInstanceInServiceWaitTypeDef",
     {
         "LoadBalancerName": str,
     },
 )
 _OptionalDescribeEndPointStateInputInstanceInServiceWaitTypeDef = TypedDict(
@@ -822,27 +815,25 @@
     {
         "Instances": Sequence[InstanceTypeDef],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeEndPointStateInputInstanceInServiceWaitTypeDef(
     _RequiredDescribeEndPointStateInputInstanceInServiceWaitTypeDef,
     _OptionalDescribeEndPointStateInputInstanceInServiceWaitTypeDef,
 ):
     pass
 
-
 DescribeEndPointStateOutputTypeDef = TypedDict(
     "DescribeEndPointStateOutputTypeDef",
     {
         "InstanceStates": List[InstanceStateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PoliciesTypeDef = TypedDict(
     "PoliciesTypeDef",
     {
         "AppCookieStickinessPolicies": List[AppCookieStickinessPolicyTypeDef],
@@ -880,40 +871,43 @@
     },
 )
 
 DescribeTagsOutputTypeDef = TypedDict(
     "DescribeTagsOutputTypeDef",
     {
         "TagDescriptions": List[TagDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLoadBalancerAttributesOutputTypeDef = TypedDict(
     "DescribeLoadBalancerAttributesOutputTypeDef",
     {
-        "LoadBalancerAttributes": LoadBalancerAttributesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "LoadBalancerAttributes": LoadBalancerAttributesOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ModifyLoadBalancerAttributesInputRequestTypeDef = TypedDict(
-    "ModifyLoadBalancerAttributesInputRequestTypeDef",
+ModifyLoadBalancerAttributesOutputTypeDef = TypedDict(
+    "ModifyLoadBalancerAttributesOutputTypeDef",
     {
         "LoadBalancerName": str,
-        "LoadBalancerAttributes": LoadBalancerAttributesTypeDef,
+        "LoadBalancerAttributes": LoadBalancerAttributesOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ModifyLoadBalancerAttributesOutputTypeDef = TypedDict(
-    "ModifyLoadBalancerAttributesOutputTypeDef",
+LoadBalancerAttributesUnionTypeDef = Union[
+    LoadBalancerAttributesTypeDef, LoadBalancerAttributesOutputTypeDef
+]
+ModifyLoadBalancerAttributesInputRequestTypeDef = TypedDict(
+    "ModifyLoadBalancerAttributesInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "LoadBalancerAttributes": LoadBalancerAttributesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LoadBalancerDescriptionTypeDef = TypedDict(
     "LoadBalancerDescriptionTypeDef",
     {
         "LoadBalancerName": str,
@@ -936,27 +930,27 @@
     total=False,
 )
 
 DescribeLoadBalancerPoliciesOutputTypeDef = TypedDict(
     "DescribeLoadBalancerPoliciesOutputTypeDef",
     {
         "PolicyDescriptions": List[PolicyDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLoadBalancerPolicyTypesOutputTypeDef = TypedDict(
     "DescribeLoadBalancerPolicyTypesOutputTypeDef",
     {
         "PolicyTypeDescriptions": List[PolicyTypeDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAccessPointsOutputTypeDef = TypedDict(
     "DescribeAccessPointsOutputTypeDef",
     {
         "LoadBalancerDescriptions": List[LoadBalancerDescriptionTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-elb-2.5.2/types_aiobotocore_elb/type_defs.pyi` & `types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,103 +4,106 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_elb.type_defs import AccessLogTypeDef
 
-    data: AccessLogTypeDef = {...}
+    data: AccessLogTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AccessLogTypeDef",
     "AddAvailabilityZonesInputRequestTypeDef",
-    "AddAvailabilityZonesOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "AdditionalAttributeTypeDef",
     "AppCookieStickinessPolicyTypeDef",
     "ApplySecurityGroupsToLoadBalancerInputRequestTypeDef",
-    "ApplySecurityGroupsToLoadBalancerOutputTypeDef",
     "AttachLoadBalancerToSubnetsInputRequestTypeDef",
-    "AttachLoadBalancerToSubnetsOutputTypeDef",
     "BackendServerDescriptionTypeDef",
     "HealthCheckTypeDef",
     "ConnectionDrainingTypeDef",
     "ConnectionSettingsTypeDef",
     "ListenerTypeDef",
-    "CreateAccessPointOutputTypeDef",
     "CreateAppCookieStickinessPolicyInputRequestTypeDef",
     "CreateLBCookieStickinessPolicyInputRequestTypeDef",
     "PolicyAttributeTypeDef",
     "CrossZoneLoadBalancingTypeDef",
     "DeleteAccessPointInputRequestTypeDef",
     "DeleteLoadBalancerListenerInputRequestTypeDef",
     "DeleteLoadBalancerPolicyInputRequestTypeDef",
     "InstanceTypeDef",
-    "DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAccessPointsInputRequestTypeDef",
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
     "DescribeAccountLimitsInputRequestTypeDef",
     "LimitTypeDef",
     "WaiterConfigTypeDef",
     "InstanceStateTypeDef",
     "DescribeLoadBalancerAttributesInputRequestTypeDef",
     "DescribeLoadBalancerPoliciesInputRequestTypeDef",
     "DescribeLoadBalancerPolicyTypesInputRequestTypeDef",
     "DescribeTagsInputRequestTypeDef",
     "DetachLoadBalancerFromSubnetsInputRequestTypeDef",
-    "DetachLoadBalancerFromSubnetsOutputTypeDef",
     "LBCookieStickinessPolicyTypeDef",
     "SourceSecurityGroupTypeDef",
-    "PaginatorConfigTypeDef",
     "PolicyAttributeDescriptionTypeDef",
     "PolicyAttributeTypeDescriptionTypeDef",
     "RemoveAvailabilityZonesInputRequestTypeDef",
-    "RemoveAvailabilityZonesOutputTypeDef",
     "TagKeyOnlyTypeDef",
-    "ResponseMetadataTypeDef",
     "SetLoadBalancerListenerSSLCertificateInputRequestTypeDef",
     "SetLoadBalancerPoliciesForBackendServerInputRequestTypeDef",
     "SetLoadBalancerPoliciesOfListenerInputRequestTypeDef",
+    "AddAvailabilityZonesOutputTypeDef",
+    "ApplySecurityGroupsToLoadBalancerOutputTypeDef",
+    "AttachLoadBalancerToSubnetsOutputTypeDef",
+    "CreateAccessPointOutputTypeDef",
+    "DetachLoadBalancerFromSubnetsOutputTypeDef",
+    "RemoveAvailabilityZonesOutputTypeDef",
     "AddTagsInputRequestTypeDef",
     "TagDescriptionTypeDef",
     "ConfigureHealthCheckInputRequestTypeDef",
     "ConfigureHealthCheckOutputTypeDef",
     "CreateAccessPointInputRequestTypeDef",
     "CreateLoadBalancerListenerInputRequestTypeDef",
     "ListenerDescriptionTypeDef",
     "CreateLoadBalancerPolicyInputRequestTypeDef",
+    "LoadBalancerAttributesOutputTypeDef",
     "LoadBalancerAttributesTypeDef",
     "DeregisterEndPointsInputRequestTypeDef",
     "DeregisterEndPointsOutputTypeDef",
     "DescribeEndPointStateInputRequestTypeDef",
     "RegisterEndPointsInputRequestTypeDef",
     "RegisterEndPointsOutputTypeDef",
+    "DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef",
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
     "DescribeAccountLimitsOutputTypeDef",
     "DescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef",
     "DescribeEndPointStateInputInstanceDeregisteredWaitTypeDef",
     "DescribeEndPointStateInputInstanceInServiceWaitTypeDef",
     "DescribeEndPointStateOutputTypeDef",
     "PoliciesTypeDef",
     "PolicyDescriptionTypeDef",
     "PolicyTypeDescriptionTypeDef",
     "RemoveTagsInputRequestTypeDef",
     "DescribeTagsOutputTypeDef",
     "DescribeLoadBalancerAttributesOutputTypeDef",
-    "ModifyLoadBalancerAttributesInputRequestTypeDef",
     "ModifyLoadBalancerAttributesOutputTypeDef",
+    "LoadBalancerAttributesUnionTypeDef",
+    "ModifyLoadBalancerAttributesInputRequestTypeDef",
     "LoadBalancerDescriptionTypeDef",
     "DescribeLoadBalancerPoliciesOutputTypeDef",
     "DescribeLoadBalancerPolicyTypesOutputTypeDef",
     "DescribeAccessPointsOutputTypeDef",
 )
 
 _RequiredAccessLogTypeDef = TypedDict(
@@ -115,30 +118,35 @@
         "S3BucketName": str,
         "EmitInterval": int,
         "S3BucketPrefix": str,
     },
     total=False,
 )
 
+
 class AccessLogTypeDef(_RequiredAccessLogTypeDef, _OptionalAccessLogTypeDef):
     pass
 
+
 AddAvailabilityZonesInputRequestTypeDef = TypedDict(
     "AddAvailabilityZonesInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "AvailabilityZones": Sequence[str],
     },
 )
 
-AddAvailabilityZonesOutputTypeDef = TypedDict(
-    "AddAvailabilityZonesOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AvailabilityZones": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
@@ -148,17 +156,19 @@
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
+
 AdditionalAttributeTypeDef = TypedDict(
     "AdditionalAttributeTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -177,38 +187,22 @@
     "ApplySecurityGroupsToLoadBalancerInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "SecurityGroups": Sequence[str],
     },
 )
 
-ApplySecurityGroupsToLoadBalancerOutputTypeDef = TypedDict(
-    "ApplySecurityGroupsToLoadBalancerOutputTypeDef",
-    {
-        "SecurityGroups": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AttachLoadBalancerToSubnetsInputRequestTypeDef = TypedDict(
     "AttachLoadBalancerToSubnetsInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "Subnets": Sequence[str],
     },
 )
 
-AttachLoadBalancerToSubnetsOutputTypeDef = TypedDict(
-    "AttachLoadBalancerToSubnetsOutputTypeDef",
-    {
-        "Subnets": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BackendServerDescriptionTypeDef = TypedDict(
     "BackendServerDescriptionTypeDef",
     {
         "InstancePort": int,
         "PolicyNames": List[str],
     },
     total=False,
@@ -235,19 +229,21 @@
     "_OptionalConnectionDrainingTypeDef",
     {
         "Timeout": int,
     },
     total=False,
 )
 
+
 class ConnectionDrainingTypeDef(
     _RequiredConnectionDrainingTypeDef, _OptionalConnectionDrainingTypeDef
 ):
     pass
 
+
 ConnectionSettingsTypeDef = TypedDict(
     "ConnectionSettingsTypeDef",
     {
         "IdleTimeout": int,
     },
 )
 
@@ -264,24 +260,18 @@
     {
         "InstanceProtocol": str,
         "SSLCertificateId": str,
     },
     total=False,
 )
 
+
 class ListenerTypeDef(_RequiredListenerTypeDef, _OptionalListenerTypeDef):
     pass
 
-CreateAccessPointOutputTypeDef = TypedDict(
-    "CreateAccessPointOutputTypeDef",
-    {
-        "DNSName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 CreateAppCookieStickinessPolicyInputRequestTypeDef = TypedDict(
     "CreateAppCookieStickinessPolicyInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "PolicyName": str,
         "CookieName": str,
@@ -299,20 +289,22 @@
     "_OptionalCreateLBCookieStickinessPolicyInputRequestTypeDef",
     {
         "CookieExpirationPeriod": int,
     },
     total=False,
 )
 
+
 class CreateLBCookieStickinessPolicyInputRequestTypeDef(
     _RequiredCreateLBCookieStickinessPolicyInputRequestTypeDef,
     _OptionalCreateLBCookieStickinessPolicyInputRequestTypeDef,
 ):
     pass
 
+
 PolicyAttributeTypeDef = TypedDict(
     "PolicyAttributeTypeDef",
     {
         "AttributeName": str,
         "AttributeValue": str,
     },
     total=False,
@@ -352,41 +344,34 @@
     "InstanceTypeDef",
     {
         "InstanceId": str,
     },
     total=False,
 )
 
-DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef = TypedDict(
-    "DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "LoadBalancerNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeAccessPointsInputRequestTypeDef = TypedDict(
     "DescribeAccessPointsInputRequestTypeDef",
     {
         "LoadBalancerNames": Sequence[str],
         "Marker": str,
         "PageSize": int,
     },
     total=False,
 )
 
-DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeAccountLimitsInputRequestTypeDef = TypedDict(
     "DescribeAccountLimitsInputRequestTypeDef",
     {
         "Marker": str,
         "PageSize": int,
     },
     total=False,
@@ -456,22 +441,14 @@
     "DetachLoadBalancerFromSubnetsInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "Subnets": Sequence[str],
     },
 )
 
-DetachLoadBalancerFromSubnetsOutputTypeDef = TypedDict(
-    "DetachLoadBalancerFromSubnetsOutputTypeDef",
-    {
-        "Subnets": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LBCookieStickinessPolicyTypeDef = TypedDict(
     "LBCookieStickinessPolicyTypeDef",
     {
         "PolicyName": str,
         "CookieExpirationPeriod": int,
     },
     total=False,
@@ -482,24 +459,14 @@
     {
         "OwnerAlias": str,
         "GroupName": str,
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
 PolicyAttributeDescriptionTypeDef = TypedDict(
     "PolicyAttributeDescriptionTypeDef",
     {
         "AttributeName": str,
         "AttributeValue": str,
     },
     total=False,
@@ -521,41 +488,22 @@
     "RemoveAvailabilityZonesInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "AvailabilityZones": Sequence[str],
     },
 )
 
-RemoveAvailabilityZonesOutputTypeDef = TypedDict(
-    "RemoveAvailabilityZonesOutputTypeDef",
-    {
-        "AvailabilityZones": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagKeyOnlyTypeDef = TypedDict(
     "TagKeyOnlyTypeDef",
     {
         "Key": str,
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
 SetLoadBalancerListenerSSLCertificateInputRequestTypeDef = TypedDict(
     "SetLoadBalancerListenerSSLCertificateInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "LoadBalancerPort": int,
         "SSLCertificateId": str,
     },
@@ -575,14 +523,62 @@
     {
         "LoadBalancerName": str,
         "LoadBalancerPort": int,
         "PolicyNames": Sequence[str],
     },
 )
 
+AddAvailabilityZonesOutputTypeDef = TypedDict(
+    "AddAvailabilityZonesOutputTypeDef",
+    {
+        "AvailabilityZones": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ApplySecurityGroupsToLoadBalancerOutputTypeDef = TypedDict(
+    "ApplySecurityGroupsToLoadBalancerOutputTypeDef",
+    {
+        "SecurityGroups": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AttachLoadBalancerToSubnetsOutputTypeDef = TypedDict(
+    "AttachLoadBalancerToSubnetsOutputTypeDef",
+    {
+        "Subnets": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAccessPointOutputTypeDef = TypedDict(
+    "CreateAccessPointOutputTypeDef",
+    {
+        "DNSName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DetachLoadBalancerFromSubnetsOutputTypeDef = TypedDict(
+    "DetachLoadBalancerFromSubnetsOutputTypeDef",
+    {
+        "Subnets": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemoveAvailabilityZonesOutputTypeDef = TypedDict(
+    "RemoveAvailabilityZonesOutputTypeDef",
+    {
+        "AvailabilityZones": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AddTagsInputRequestTypeDef = TypedDict(
     "AddTagsInputRequestTypeDef",
     {
         "LoadBalancerNames": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -604,15 +600,15 @@
     },
 )
 
 ConfigureHealthCheckOutputTypeDef = TypedDict(
     "ConfigureHealthCheckOutputTypeDef",
     {
         "HealthCheck": HealthCheckTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateAccessPointInputRequestTypeDef = TypedDict(
     "_RequiredCreateAccessPointInputRequestTypeDef",
     {
         "LoadBalancerName": str,
@@ -627,19 +623,21 @@
         "SecurityGroups": Sequence[str],
         "Scheme": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateAccessPointInputRequestTypeDef(
     _RequiredCreateAccessPointInputRequestTypeDef, _OptionalCreateAccessPointInputRequestTypeDef
 ):
     pass
 
+
 CreateLoadBalancerListenerInputRequestTypeDef = TypedDict(
     "CreateLoadBalancerListenerInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "Listeners": Sequence[ListenerTypeDef],
     },
 )
@@ -665,28 +663,42 @@
     "_OptionalCreateLoadBalancerPolicyInputRequestTypeDef",
     {
         "PolicyAttributes": Sequence[PolicyAttributeTypeDef],
     },
     total=False,
 )
 
+
 class CreateLoadBalancerPolicyInputRequestTypeDef(
     _RequiredCreateLoadBalancerPolicyInputRequestTypeDef,
     _OptionalCreateLoadBalancerPolicyInputRequestTypeDef,
 ):
     pass
 
+
+LoadBalancerAttributesOutputTypeDef = TypedDict(
+    "LoadBalancerAttributesOutputTypeDef",
+    {
+        "CrossZoneLoadBalancing": CrossZoneLoadBalancingTypeDef,
+        "AccessLog": AccessLogTypeDef,
+        "ConnectionDraining": ConnectionDrainingTypeDef,
+        "ConnectionSettings": ConnectionSettingsTypeDef,
+        "AdditionalAttributes": List[AdditionalAttributeTypeDef],
+    },
+    total=False,
+)
+
 LoadBalancerAttributesTypeDef = TypedDict(
     "LoadBalancerAttributesTypeDef",
     {
         "CrossZoneLoadBalancing": CrossZoneLoadBalancingTypeDef,
         "AccessLog": AccessLogTypeDef,
         "ConnectionDraining": ConnectionDrainingTypeDef,
         "ConnectionSettings": ConnectionSettingsTypeDef,
-        "AdditionalAttributes": List[AdditionalAttributeTypeDef],
+        "AdditionalAttributes": Sequence[AdditionalAttributeTypeDef],
     },
     total=False,
 )
 
 DeregisterEndPointsInputRequestTypeDef = TypedDict(
     "DeregisterEndPointsInputRequestTypeDef",
     {
@@ -695,15 +707,15 @@
     },
 )
 
 DeregisterEndPointsOutputTypeDef = TypedDict(
     "DeregisterEndPointsOutputTypeDef",
     {
         "Instances": List[InstanceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeEndPointStateInputRequestTypeDef = TypedDict(
     "_RequiredDescribeEndPointStateInputRequestTypeDef",
     {
         "LoadBalancerName": str,
@@ -713,42 +725,61 @@
     "_OptionalDescribeEndPointStateInputRequestTypeDef",
     {
         "Instances": Sequence[InstanceTypeDef],
     },
     total=False,
 )
 
+
 class DescribeEndPointStateInputRequestTypeDef(
     _RequiredDescribeEndPointStateInputRequestTypeDef,
     _OptionalDescribeEndPointStateInputRequestTypeDef,
 ):
     pass
 
+
 RegisterEndPointsInputRequestTypeDef = TypedDict(
     "RegisterEndPointsInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "Instances": Sequence[InstanceTypeDef],
     },
 )
 
 RegisterEndPointsOutputTypeDef = TypedDict(
     "RegisterEndPointsOutputTypeDef",
     {
         "Instances": List[InstanceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef = TypedDict(
+    "DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef",
+    {
+        "LoadBalancerNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 DescribeAccountLimitsOutputTypeDef = TypedDict(
     "DescribeAccountLimitsOutputTypeDef",
     {
         "Limits": List[LimitTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef = TypedDict(
     "_RequiredDescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef",
     {
         "LoadBalancerName": str,
@@ -759,20 +790,22 @@
     {
         "Instances": Sequence[InstanceTypeDef],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef(
     _RequiredDescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef,
     _OptionalDescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeEndPointStateInputInstanceDeregisteredWaitTypeDef = TypedDict(
     "_RequiredDescribeEndPointStateInputInstanceDeregisteredWaitTypeDef",
     {
         "LoadBalancerName": str,
     },
 )
 _OptionalDescribeEndPointStateInputInstanceDeregisteredWaitTypeDef = TypedDict(
@@ -780,20 +813,22 @@
     {
         "Instances": Sequence[InstanceTypeDef],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeEndPointStateInputInstanceDeregisteredWaitTypeDef(
     _RequiredDescribeEndPointStateInputInstanceDeregisteredWaitTypeDef,
     _OptionalDescribeEndPointStateInputInstanceDeregisteredWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeEndPointStateInputInstanceInServiceWaitTypeDef = TypedDict(
     "_RequiredDescribeEndPointStateInputInstanceInServiceWaitTypeDef",
     {
         "LoadBalancerName": str,
     },
 )
 _OptionalDescribeEndPointStateInputInstanceInServiceWaitTypeDef = TypedDict(
@@ -801,25 +836,27 @@
     {
         "Instances": Sequence[InstanceTypeDef],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeEndPointStateInputInstanceInServiceWaitTypeDef(
     _RequiredDescribeEndPointStateInputInstanceInServiceWaitTypeDef,
     _OptionalDescribeEndPointStateInputInstanceInServiceWaitTypeDef,
 ):
     pass
 
+
 DescribeEndPointStateOutputTypeDef = TypedDict(
     "DescribeEndPointStateOutputTypeDef",
     {
         "InstanceStates": List[InstanceStateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PoliciesTypeDef = TypedDict(
     "PoliciesTypeDef",
     {
         "AppCookieStickinessPolicies": List[AppCookieStickinessPolicyTypeDef],
@@ -857,40 +894,43 @@
     },
 )
 
 DescribeTagsOutputTypeDef = TypedDict(
     "DescribeTagsOutputTypeDef",
     {
         "TagDescriptions": List[TagDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLoadBalancerAttributesOutputTypeDef = TypedDict(
     "DescribeLoadBalancerAttributesOutputTypeDef",
     {
-        "LoadBalancerAttributes": LoadBalancerAttributesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "LoadBalancerAttributes": LoadBalancerAttributesOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ModifyLoadBalancerAttributesInputRequestTypeDef = TypedDict(
-    "ModifyLoadBalancerAttributesInputRequestTypeDef",
+ModifyLoadBalancerAttributesOutputTypeDef = TypedDict(
+    "ModifyLoadBalancerAttributesOutputTypeDef",
     {
         "LoadBalancerName": str,
-        "LoadBalancerAttributes": LoadBalancerAttributesTypeDef,
+        "LoadBalancerAttributes": LoadBalancerAttributesOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ModifyLoadBalancerAttributesOutputTypeDef = TypedDict(
-    "ModifyLoadBalancerAttributesOutputTypeDef",
+LoadBalancerAttributesUnionTypeDef = Union[
+    LoadBalancerAttributesTypeDef, LoadBalancerAttributesOutputTypeDef
+]
+ModifyLoadBalancerAttributesInputRequestTypeDef = TypedDict(
+    "ModifyLoadBalancerAttributesInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "LoadBalancerAttributes": LoadBalancerAttributesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LoadBalancerDescriptionTypeDef = TypedDict(
     "LoadBalancerDescriptionTypeDef",
     {
         "LoadBalancerName": str,
@@ -913,27 +953,27 @@
     total=False,
 )
 
 DescribeLoadBalancerPoliciesOutputTypeDef = TypedDict(
     "DescribeLoadBalancerPoliciesOutputTypeDef",
     {
         "PolicyDescriptions": List[PolicyDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLoadBalancerPolicyTypesOutputTypeDef = TypedDict(
     "DescribeLoadBalancerPolicyTypesOutputTypeDef",
     {
         "PolicyTypeDescriptions": List[PolicyTypeDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAccessPointsOutputTypeDef = TypedDict(
     "DescribeAccessPointsOutputTypeDef",
     {
         "LoadBalancerDescriptions": List[LoadBalancerDescriptionTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-elb-2.5.2/types_aiobotocore_elb/waiter.py` & `types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elb-2.5.2/types_aiobotocore_elb/waiter.pyi` & `types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elb-2.5.2/types_aiobotocore_elb.egg-info/PKG-INFO` & `types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elb
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ElasticLoadBalancing 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ElasticLoadBalancing 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore elb type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore elb type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-elb"></a>
 
 # types-aiobotocore-elb
 
 [![PyPI - types-aiobotocore-elb](https://img.shields.io/pypi/v/types-aiobotocore-elb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-elb?color=blue)](https://pypistats.org/packages/types-aiobotocore-elb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elb)](https://pepy.tech/project/types-aiobotocore-elb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ElasticLoadBalancing 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
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
 [types-aiobotocore-elb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/).
 
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
@@ -350,107 +349,109 @@
 )
 
 
 def check_value(value: AnyInstanceInServiceWaiterName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_elb.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_elb.type_defs import (
     AccessLogTypeDef,
     AddAvailabilityZonesInputRequestTypeDef,
-    AddAvailabilityZonesOutputTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     AdditionalAttributeTypeDef,
     AppCookieStickinessPolicyTypeDef,
     ApplySecurityGroupsToLoadBalancerInputRequestTypeDef,
-    ApplySecurityGroupsToLoadBalancerOutputTypeDef,
     AttachLoadBalancerToSubnetsInputRequestTypeDef,
-    AttachLoadBalancerToSubnetsOutputTypeDef,
     BackendServerDescriptionTypeDef,
     HealthCheckTypeDef,
     ConnectionDrainingTypeDef,
     ConnectionSettingsTypeDef,
     ListenerTypeDef,
-    CreateAccessPointOutputTypeDef,
     CreateAppCookieStickinessPolicyInputRequestTypeDef,
     CreateLBCookieStickinessPolicyInputRequestTypeDef,
     PolicyAttributeTypeDef,
     CrossZoneLoadBalancingTypeDef,
     DeleteAccessPointInputRequestTypeDef,
     DeleteLoadBalancerListenerInputRequestTypeDef,
     DeleteLoadBalancerPolicyInputRequestTypeDef,
     InstanceTypeDef,
-    DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAccessPointsInputRequestTypeDef,
-    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     LimitTypeDef,
     WaiterConfigTypeDef,
     InstanceStateTypeDef,
     DescribeLoadBalancerAttributesInputRequestTypeDef,
     DescribeLoadBalancerPoliciesInputRequestTypeDef,
     DescribeLoadBalancerPolicyTypesInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
     DetachLoadBalancerFromSubnetsInputRequestTypeDef,
-    DetachLoadBalancerFromSubnetsOutputTypeDef,
     LBCookieStickinessPolicyTypeDef,
     SourceSecurityGroupTypeDef,
-    PaginatorConfigTypeDef,
     PolicyAttributeDescriptionTypeDef,
     PolicyAttributeTypeDescriptionTypeDef,
     RemoveAvailabilityZonesInputRequestTypeDef,
-    RemoveAvailabilityZonesOutputTypeDef,
     TagKeyOnlyTypeDef,
-    ResponseMetadataTypeDef,
     SetLoadBalancerListenerSSLCertificateInputRequestTypeDef,
     SetLoadBalancerPoliciesForBackendServerInputRequestTypeDef,
     SetLoadBalancerPoliciesOfListenerInputRequestTypeDef,
+    AddAvailabilityZonesOutputTypeDef,
+    ApplySecurityGroupsToLoadBalancerOutputTypeDef,
+    AttachLoadBalancerToSubnetsOutputTypeDef,
+    CreateAccessPointOutputTypeDef,
+    DetachLoadBalancerFromSubnetsOutputTypeDef,
+    RemoveAvailabilityZonesOutputTypeDef,
     AddTagsInputRequestTypeDef,
     TagDescriptionTypeDef,
     ConfigureHealthCheckInputRequestTypeDef,
     ConfigureHealthCheckOutputTypeDef,
     CreateAccessPointInputRequestTypeDef,
     CreateLoadBalancerListenerInputRequestTypeDef,
     ListenerDescriptionTypeDef,
     CreateLoadBalancerPolicyInputRequestTypeDef,
+    LoadBalancerAttributesOutputTypeDef,
     LoadBalancerAttributesTypeDef,
     DeregisterEndPointsInputRequestTypeDef,
     DeregisterEndPointsOutputTypeDef,
     DescribeEndPointStateInputRequestTypeDef,
     RegisterEndPointsInputRequestTypeDef,
     RegisterEndPointsOutputTypeDef,
+    DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef,
+    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsOutputTypeDef,
     DescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef,
     DescribeEndPointStateInputInstanceDeregisteredWaitTypeDef,
     DescribeEndPointStateInputInstanceInServiceWaitTypeDef,
     DescribeEndPointStateOutputTypeDef,
     PoliciesTypeDef,
     PolicyDescriptionTypeDef,
     PolicyTypeDescriptionTypeDef,
     RemoveTagsInputRequestTypeDef,
     DescribeTagsOutputTypeDef,
     DescribeLoadBalancerAttributesOutputTypeDef,
-    ModifyLoadBalancerAttributesInputRequestTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
+    LoadBalancerAttributesUnionTypeDef,
+    ModifyLoadBalancerAttributesInputRequestTypeDef,
     LoadBalancerDescriptionTypeDef,
     DescribeLoadBalancerPoliciesOutputTypeDef,
     DescribeLoadBalancerPolicyTypesOutputTypeDef,
     DescribeAccessPointsOutputTypeDef,
 )
 
 
-def get_structure() -> AccessLogTypeDef:
+def get_value() -> AccessLogTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-elb-2.5.2/types_aiobotocore_elb.egg-info/SOURCES.txt` & `types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb.egg-info/SOURCES.txt`

 * *Files identical despite different names*


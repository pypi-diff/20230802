# Comparing `tmp/types-aiobotocore-ecs-2.5.2.tar.gz` & `tmp/types-aiobotocore-ecs-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ecs-2.5.2.tar", last modified: Sat Jul  8 01:43:35 2023, max compression
+gzip compressed data, was "types-aiobotocore-ecs-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:14 2023, max compression
```

## Comparing `types-aiobotocore-ecs-2.5.2.tar` & `types-aiobotocore-ecs-2.5.2.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:35.146084 types-aiobotocore-ecs-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:30:10.000000 types-aiobotocore-ecs-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24924 2023-07-08 01:43:35.146084 types-aiobotocore-ecs-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23375 2023-07-08 01:30:10.000000 types-aiobotocore-ecs-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:35.146084 types-aiobotocore-ecs-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-08 01:30:10.000000 types-aiobotocore-ecs-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:35.142084 types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs/
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-08 01:30:10.000000 types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-08 01:30:10.000000 types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-08 01:30:10.000000 types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52556 2023-07-08 01:30:10.000000 types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    52478 2023-07-08 01:30:10.000000 types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15687 2023-07-08 01:30:11.000000 types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15685 2023-07-08 01:30:10.000000 types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12062 2023-07-08 01:30:10.000000 types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-07-08 01:30:10.000000 types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:30:10.000000 types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    85562 2023-07-08 01:30:13.000000 types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    85461 2023-07-08 01:30:12.000000 types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:30:10.000000 types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-07-08 01:30:10.000000 types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-07-08 01:30:10.000000 types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:35.146084 types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24924 2023-07-08 01:43:34.000000 types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-08 01:43:35.000000 types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:34.000000 types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:34.000000 types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:34.000000 types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:43:34.000000 types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.505594 types-aiobotocore-ecs-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:37:57.000000 types-aiobotocore-ecs-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25862 2023-08-02 14:52:14.505594 types-aiobotocore-ecs-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24360 2023-08-02 14:37:57.000000 types-aiobotocore-ecs-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:14.505594 types-aiobotocore-ecs-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:37:57.000000 types-aiobotocore-ecs-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.493594 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-08-02 14:37:57.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-08-02 14:37:57.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:37:57.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52644 2023-08-02 14:37:57.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52566 2023-08-02 14:37:57.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15687 2023-08-02 14:37:58.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15685 2023-08-02 14:37:58.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-08-02 14:37:57.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12032 2023-08-02 14:37:57.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:37:57.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    96682 2023-08-02 14:38:01.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96563 2023-08-02 14:37:59.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:37:57.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-08-02 14:37:57.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-08-02 14:37:57.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.505594 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25862 2023-08-02 14:52:14.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-02 14:52:14.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:14.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:14.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ecs-2.5.2/LICENSE` & `types-aiobotocore-ecs-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecs-2.5.2/PKG-INFO` & `types-aiobotocore-ecs-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ecs
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ECS 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ECS 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore ecs type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore ecs type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-ecs"></a>
 
 # types-aiobotocore-ecs
 
 [![PyPI - types-aiobotocore-ecs](https://img.shields.io/pypi/v/types-aiobotocore-ecs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ecs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ecs?color=blue)](https://pypistats.org/packages/types-aiobotocore-ecs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ecs)](https://pepy.tech/project/types-aiobotocore-ecs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ECS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
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
 [types-aiobotocore-ecs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/).
 
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
@@ -433,217 +432,245 @@
 )
 
 
 def check_value(value: AgentUpdateStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_ecs.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_ecs.type_defs import (
     AttachmentStateChangeTypeDef,
     KeyValuePairTypeDef,
     AttributeTypeDef,
     ManagedScalingTypeDef,
+    AwsVpcConfigurationOutputTypeDef,
     AwsVpcConfigurationTypeDef,
     CapacityProviderStrategyItemTypeDef,
     TagTypeDef,
     ClusterServiceConnectDefaultsRequestTypeDef,
     ClusterServiceConnectDefaultsTypeDef,
     ClusterSettingTypeDef,
     ContainerDependencyTypeDef,
     EnvironmentFileTypeDef,
-    FirelensConfigurationTypeDef,
-    HealthCheckTypeDef,
+    FirelensConfigurationOutputTypeDef,
+    HealthCheckOutputTypeDef,
     HostEntryTypeDef,
     MountPointTypeDef,
     PortMappingTypeDef,
     RepositoryCredentialsTypeDef,
     ResourceRequirementTypeDef,
     SecretTypeDef,
     SystemControlTypeDef,
     UlimitTypeDef,
     VolumeFromTypeDef,
+    FirelensConfigurationTypeDef,
+    HealthCheckTypeDef,
     InstanceHealthCheckResultTypeDef,
-    ResourceTypeDef,
+    ResourceOutputTypeDef,
     VersionInfoTypeDef,
     NetworkBindingTypeDef,
     ManagedAgentTypeDef,
     NetworkInterfaceTypeDef,
+    ResponseMetadataTypeDef,
     DeploymentControllerTypeDef,
     LoadBalancerTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     ServiceRegistryTypeDef,
     ScaleTypeDef,
     DeleteAccountSettingRequestRequestTypeDef,
     SettingTypeDef,
     DeleteCapacityProviderRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteServiceRequestRequestTypeDef,
     DeleteTaskDefinitionsRequestRequestTypeDef,
     FailureTypeDef,
     DeleteTaskSetRequestRequestTypeDef,
+    DeploymentAlarmsOutputTypeDef,
     DeploymentAlarmsTypeDef,
     DeploymentCircuitBreakerTypeDef,
     ServiceConnectServiceResourceTypeDef,
     DeregisterContainerInstanceRequestRequestTypeDef,
     DeregisterTaskDefinitionRequestRequestTypeDef,
     DescribeCapacityProvidersRequestRequestTypeDef,
     DescribeClustersRequestRequestTypeDef,
     DescribeContainerInstancesRequestRequestTypeDef,
     DescribeServicesRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTaskDefinitionRequestRequestTypeDef,
     DescribeTaskSetsRequestRequestTypeDef,
     DescribeTasksRequestRequestTypeDef,
+    DeviceOutputTypeDef,
     DeviceTypeDef,
     DiscoverPollEndpointRequestRequestTypeDef,
-    DiscoverPollEndpointResponseTypeDef,
+    DockerVolumeConfigurationOutputTypeDef,
     DockerVolumeConfigurationTypeDef,
     EFSAuthorizationConfigTypeDef,
     EphemeralStorageTypeDef,
     ExecuteCommandLogConfigurationTypeDef,
     ExecuteCommandRequestRequestTypeDef,
     SessionTypeDef,
     FSxWindowsFileServerAuthorizationConfigTypeDef,
     GetTaskProtectionRequestRequestTypeDef,
     ProtectedTaskTypeDef,
     HostVolumePropertiesTypeDef,
     InferenceAcceleratorOverrideTypeDef,
     InferenceAcceleratorTypeDef,
+    KernelCapabilitiesOutputTypeDef,
     KernelCapabilitiesTypeDef,
+    TmpfsOutputTypeDef,
     TmpfsTypeDef,
-    ListAccountSettingsRequestListAccountSettingsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccountSettingsRequestRequestTypeDef,
-    ListAttributesRequestListAttributesPaginateTypeDef,
     ListAttributesRequestRequestTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
-    ListClustersResponseTypeDef,
-    ListContainerInstancesRequestListContainerInstancesPaginateTypeDef,
     ListContainerInstancesRequestRequestTypeDef,
-    ListContainerInstancesResponseTypeDef,
-    ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
     ListServicesByNamespaceRequestRequestTypeDef,
-    ListServicesByNamespaceResponseTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
-    ListServicesResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef,
     ListTaskDefinitionFamiliesRequestRequestTypeDef,
-    ListTaskDefinitionFamiliesResponseTypeDef,
-    ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef,
     ListTaskDefinitionsRequestRequestTypeDef,
-    ListTaskDefinitionsResponseTypeDef,
-    ListTasksRequestListTasksPaginateTypeDef,
     ListTasksRequestRequestTypeDef,
-    ListTasksResponseTypeDef,
     ManagedAgentStateChangeTypeDef,
-    PaginatorConfigTypeDef,
     PlatformDeviceTypeDef,
     PutAccountSettingDefaultRequestRequestTypeDef,
     PutAccountSettingRequestRequestTypeDef,
     RuntimePlatformTypeDef,
     TaskDefinitionPlacementConstraintTypeDef,
-    ResponseMetadataTypeDef,
+    ResourceTypeDef,
     ServiceConnectClientAliasTypeDef,
     ServiceEventTypeDef,
     StopTaskRequestRequestTypeDef,
-    SubmitAttachmentStateChangesResponseTypeDef,
-    SubmitContainerStateChangeResponseTypeDef,
-    SubmitTaskStateChangeResponseTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateContainerAgentRequestRequestTypeDef,
     UpdateContainerInstancesStateRequestRequestTypeDef,
     UpdateServicePrimaryTaskSetRequestRequestTypeDef,
     UpdateTaskProtectionRequestRequestTypeDef,
     SubmitAttachmentStateChangesRequestRequestTypeDef,
     AttachmentTypeDef,
+    ProxyConfigurationOutputTypeDef,
     ProxyConfigurationTypeDef,
     DeleteAttributesRequestRequestTypeDef,
-    DeleteAttributesResponseTypeDef,
-    ListAttributesResponseTypeDef,
     PutAttributesRequestRequestTypeDef,
-    PutAttributesResponseTypeDef,
     AutoScalingGroupProviderTypeDef,
     AutoScalingGroupProviderUpdateTypeDef,
+    NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
     PutClusterCapacityProvidersRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UpdateClusterSettingsRequestRequestTypeDef,
+    ContainerOverrideOutputTypeDef,
     ContainerOverrideTypeDef,
+    LogConfigurationOutputTypeDef,
     LogConfigurationTypeDef,
     ContainerInstanceHealthStatusTypeDef,
     ContainerStateChangeTypeDef,
     SubmitContainerStateChangeRequestRequestTypeDef,
     ContainerTypeDef,
+    DeleteAttributesResponseTypeDef,
+    DiscoverPollEndpointResponseTypeDef,
+    ListAttributesResponseTypeDef,
+    ListClustersResponseTypeDef,
+    ListContainerInstancesResponseTypeDef,
+    ListServicesByNamespaceResponseTypeDef,
+    ListServicesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTaskDefinitionFamiliesResponseTypeDef,
+    ListTaskDefinitionsResponseTypeDef,
+    ListTasksResponseTypeDef,
+    PutAttributesResponseTypeDef,
+    SubmitAttachmentStateChangesResponseTypeDef,
+    SubmitContainerStateChangeResponseTypeDef,
+    SubmitTaskStateChangeResponseTypeDef,
     UpdateTaskSetRequestRequestTypeDef,
     DeleteAccountSettingResponseTypeDef,
     ListAccountSettingsResponseTypeDef,
     PutAccountSettingDefaultResponseTypeDef,
     PutAccountSettingResponseTypeDef,
+    DeploymentConfigurationOutputTypeDef,
     DeploymentConfigurationTypeDef,
     DescribeServicesRequestServicesInactiveWaitTypeDef,
     DescribeServicesRequestServicesStableWaitTypeDef,
     DescribeTasksRequestTasksRunningWaitTypeDef,
     DescribeTasksRequestTasksStoppedWaitTypeDef,
     EFSVolumeConfigurationTypeDef,
     ExecuteCommandConfigurationTypeDef,
     ExecuteCommandResponseTypeDef,
     FSxWindowsFileServerVolumeConfigurationTypeDef,
     GetTaskProtectionResponseTypeDef,
     UpdateTaskProtectionResponseTypeDef,
+    LinuxParametersOutputTypeDef,
     LinuxParametersTypeDef,
-    RegisterContainerInstanceRequestRequestTypeDef,
+    ListAccountSettingsRequestListAccountSettingsPaginateTypeDef,
+    ListAttributesRequestListAttributesPaginateTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
+    ListContainerInstancesRequestListContainerInstancesPaginateTypeDef,
+    ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
+    ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef,
+    ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef,
+    ListTasksRequestListTasksPaginateTypeDef,
+    ResourceUnionTypeDef,
+    ServiceConnectServiceOutputTypeDef,
     ServiceConnectServiceTypeDef,
+    ProxyConfigurationUnionTypeDef,
     CapacityProviderTypeDef,
     CreateCapacityProviderRequestRequestTypeDef,
     UpdateCapacityProviderRequestRequestTypeDef,
-    CreateTaskSetRequestRequestTypeDef,
     TaskSetTypeDef,
+    CreateTaskSetRequestRequestTypeDef,
+    NetworkConfigurationUnionTypeDef,
+    TaskOverrideOutputTypeDef,
     TaskOverrideTypeDef,
     ContainerInstanceTypeDef,
     SubmitTaskStateChangeRequestRequestTypeDef,
+    DeploymentConfigurationUnionTypeDef,
     ClusterConfigurationTypeDef,
+    VolumeOutputTypeDef,
     VolumeTypeDef,
+    ContainerDefinitionOutputTypeDef,
     ContainerDefinitionTypeDef,
+    RegisterContainerInstanceRequestRequestTypeDef,
+    ServiceConnectConfigurationOutputTypeDef,
     ServiceConnectConfigurationTypeDef,
     CreateCapacityProviderResponseTypeDef,
     DeleteCapacityProviderResponseTypeDef,
     DescribeCapacityProvidersResponseTypeDef,
     UpdateCapacityProviderResponseTypeDef,
     CreateTaskSetResponseTypeDef,
     DeleteTaskSetResponseTypeDef,
     DescribeTaskSetsResponseTypeDef,
     UpdateServicePrimaryTaskSetResponseTypeDef,
     UpdateTaskSetResponseTypeDef,
+    TaskTypeDef,
     RunTaskRequestRequestTypeDef,
     StartTaskRequestRequestTypeDef,
-    TaskTypeDef,
+    TaskOverrideUnionTypeDef,
     DeregisterContainerInstanceResponseTypeDef,
     DescribeContainerInstancesResponseTypeDef,
     RegisterContainerInstanceResponseTypeDef,
     UpdateContainerAgentResponseTypeDef,
     UpdateContainerInstancesStateResponseTypeDef,
     ClusterTypeDef,
     CreateClusterRequestRequestTypeDef,
     UpdateClusterRequestRequestTypeDef,
-    RegisterTaskDefinitionRequestRequestTypeDef,
+    VolumeUnionTypeDef,
     TaskDefinitionTypeDef,
-    CreateServiceRequestRequestTypeDef,
+    ContainerDefinitionUnionTypeDef,
     DeploymentTypeDef,
+    CreateServiceRequestRequestTypeDef,
+    ServiceConnectConfigurationUnionTypeDef,
     UpdateServiceRequestRequestTypeDef,
     DescribeTasksResponseTypeDef,
     RunTaskResponseTypeDef,
     StartTaskResponseTypeDef,
     StopTaskResponseTypeDef,
     CreateClusterResponseTypeDef,
     DeleteClusterResponseTypeDef,
@@ -651,23 +678,24 @@
     PutClusterCapacityProvidersResponseTypeDef,
     UpdateClusterResponseTypeDef,
     UpdateClusterSettingsResponseTypeDef,
     DeleteTaskDefinitionsResponseTypeDef,
     DeregisterTaskDefinitionResponseTypeDef,
     DescribeTaskDefinitionResponseTypeDef,
     RegisterTaskDefinitionResponseTypeDef,
+    RegisterTaskDefinitionRequestRequestTypeDef,
     ServiceTypeDef,
     CreateServiceResponseTypeDef,
     DeleteServiceResponseTypeDef,
     DescribeServicesResponseTypeDef,
     UpdateServiceResponseTypeDef,
 )
 
 
-def get_structure() -> AttachmentStateChangeTypeDef:
+def get_value() -> AttachmentStateChangeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-ecs-2.5.2/README.md` & `types-aiobotocore-ecs-2.5.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-ecs"></a>
 
 # types-aiobotocore-ecs
 
 [![PyPI - types-aiobotocore-ecs](https://img.shields.io/pypi/v/types-aiobotocore-ecs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ecs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ecs?color=blue)](https://pypistats.org/packages/types-aiobotocore-ecs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ecs)](https://pepy.tech/project/types-aiobotocore-ecs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ECS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
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
 [types-aiobotocore-ecs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/).
 
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
@@ -400,217 +400,245 @@
 )
 
 
 def check_value(value: AgentUpdateStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_ecs.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_ecs.type_defs import (
     AttachmentStateChangeTypeDef,
     KeyValuePairTypeDef,
     AttributeTypeDef,
     ManagedScalingTypeDef,
+    AwsVpcConfigurationOutputTypeDef,
     AwsVpcConfigurationTypeDef,
     CapacityProviderStrategyItemTypeDef,
     TagTypeDef,
     ClusterServiceConnectDefaultsRequestTypeDef,
     ClusterServiceConnectDefaultsTypeDef,
     ClusterSettingTypeDef,
     ContainerDependencyTypeDef,
     EnvironmentFileTypeDef,
-    FirelensConfigurationTypeDef,
-    HealthCheckTypeDef,
+    FirelensConfigurationOutputTypeDef,
+    HealthCheckOutputTypeDef,
     HostEntryTypeDef,
     MountPointTypeDef,
     PortMappingTypeDef,
     RepositoryCredentialsTypeDef,
     ResourceRequirementTypeDef,
     SecretTypeDef,
     SystemControlTypeDef,
     UlimitTypeDef,
     VolumeFromTypeDef,
+    FirelensConfigurationTypeDef,
+    HealthCheckTypeDef,
     InstanceHealthCheckResultTypeDef,
-    ResourceTypeDef,
+    ResourceOutputTypeDef,
     VersionInfoTypeDef,
     NetworkBindingTypeDef,
     ManagedAgentTypeDef,
     NetworkInterfaceTypeDef,
+    ResponseMetadataTypeDef,
     DeploymentControllerTypeDef,
     LoadBalancerTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     ServiceRegistryTypeDef,
     ScaleTypeDef,
     DeleteAccountSettingRequestRequestTypeDef,
     SettingTypeDef,
     DeleteCapacityProviderRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteServiceRequestRequestTypeDef,
     DeleteTaskDefinitionsRequestRequestTypeDef,
     FailureTypeDef,
     DeleteTaskSetRequestRequestTypeDef,
+    DeploymentAlarmsOutputTypeDef,
     DeploymentAlarmsTypeDef,
     DeploymentCircuitBreakerTypeDef,
     ServiceConnectServiceResourceTypeDef,
     DeregisterContainerInstanceRequestRequestTypeDef,
     DeregisterTaskDefinitionRequestRequestTypeDef,
     DescribeCapacityProvidersRequestRequestTypeDef,
     DescribeClustersRequestRequestTypeDef,
     DescribeContainerInstancesRequestRequestTypeDef,
     DescribeServicesRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTaskDefinitionRequestRequestTypeDef,
     DescribeTaskSetsRequestRequestTypeDef,
     DescribeTasksRequestRequestTypeDef,
+    DeviceOutputTypeDef,
     DeviceTypeDef,
     DiscoverPollEndpointRequestRequestTypeDef,
-    DiscoverPollEndpointResponseTypeDef,
+    DockerVolumeConfigurationOutputTypeDef,
     DockerVolumeConfigurationTypeDef,
     EFSAuthorizationConfigTypeDef,
     EphemeralStorageTypeDef,
     ExecuteCommandLogConfigurationTypeDef,
     ExecuteCommandRequestRequestTypeDef,
     SessionTypeDef,
     FSxWindowsFileServerAuthorizationConfigTypeDef,
     GetTaskProtectionRequestRequestTypeDef,
     ProtectedTaskTypeDef,
     HostVolumePropertiesTypeDef,
     InferenceAcceleratorOverrideTypeDef,
     InferenceAcceleratorTypeDef,
+    KernelCapabilitiesOutputTypeDef,
     KernelCapabilitiesTypeDef,
+    TmpfsOutputTypeDef,
     TmpfsTypeDef,
-    ListAccountSettingsRequestListAccountSettingsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccountSettingsRequestRequestTypeDef,
-    ListAttributesRequestListAttributesPaginateTypeDef,
     ListAttributesRequestRequestTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
-    ListClustersResponseTypeDef,
-    ListContainerInstancesRequestListContainerInstancesPaginateTypeDef,
     ListContainerInstancesRequestRequestTypeDef,
-    ListContainerInstancesResponseTypeDef,
-    ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
     ListServicesByNamespaceRequestRequestTypeDef,
-    ListServicesByNamespaceResponseTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
-    ListServicesResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef,
     ListTaskDefinitionFamiliesRequestRequestTypeDef,
-    ListTaskDefinitionFamiliesResponseTypeDef,
-    ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef,
     ListTaskDefinitionsRequestRequestTypeDef,
-    ListTaskDefinitionsResponseTypeDef,
-    ListTasksRequestListTasksPaginateTypeDef,
     ListTasksRequestRequestTypeDef,
-    ListTasksResponseTypeDef,
     ManagedAgentStateChangeTypeDef,
-    PaginatorConfigTypeDef,
     PlatformDeviceTypeDef,
     PutAccountSettingDefaultRequestRequestTypeDef,
     PutAccountSettingRequestRequestTypeDef,
     RuntimePlatformTypeDef,
     TaskDefinitionPlacementConstraintTypeDef,
-    ResponseMetadataTypeDef,
+    ResourceTypeDef,
     ServiceConnectClientAliasTypeDef,
     ServiceEventTypeDef,
     StopTaskRequestRequestTypeDef,
-    SubmitAttachmentStateChangesResponseTypeDef,
-    SubmitContainerStateChangeResponseTypeDef,
-    SubmitTaskStateChangeResponseTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateContainerAgentRequestRequestTypeDef,
     UpdateContainerInstancesStateRequestRequestTypeDef,
     UpdateServicePrimaryTaskSetRequestRequestTypeDef,
     UpdateTaskProtectionRequestRequestTypeDef,
     SubmitAttachmentStateChangesRequestRequestTypeDef,
     AttachmentTypeDef,
+    ProxyConfigurationOutputTypeDef,
     ProxyConfigurationTypeDef,
     DeleteAttributesRequestRequestTypeDef,
-    DeleteAttributesResponseTypeDef,
-    ListAttributesResponseTypeDef,
     PutAttributesRequestRequestTypeDef,
-    PutAttributesResponseTypeDef,
     AutoScalingGroupProviderTypeDef,
     AutoScalingGroupProviderUpdateTypeDef,
+    NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
     PutClusterCapacityProvidersRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UpdateClusterSettingsRequestRequestTypeDef,
+    ContainerOverrideOutputTypeDef,
     ContainerOverrideTypeDef,
+    LogConfigurationOutputTypeDef,
     LogConfigurationTypeDef,
     ContainerInstanceHealthStatusTypeDef,
     ContainerStateChangeTypeDef,
     SubmitContainerStateChangeRequestRequestTypeDef,
     ContainerTypeDef,
+    DeleteAttributesResponseTypeDef,
+    DiscoverPollEndpointResponseTypeDef,
+    ListAttributesResponseTypeDef,
+    ListClustersResponseTypeDef,
+    ListContainerInstancesResponseTypeDef,
+    ListServicesByNamespaceResponseTypeDef,
+    ListServicesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTaskDefinitionFamiliesResponseTypeDef,
+    ListTaskDefinitionsResponseTypeDef,
+    ListTasksResponseTypeDef,
+    PutAttributesResponseTypeDef,
+    SubmitAttachmentStateChangesResponseTypeDef,
+    SubmitContainerStateChangeResponseTypeDef,
+    SubmitTaskStateChangeResponseTypeDef,
     UpdateTaskSetRequestRequestTypeDef,
     DeleteAccountSettingResponseTypeDef,
     ListAccountSettingsResponseTypeDef,
     PutAccountSettingDefaultResponseTypeDef,
     PutAccountSettingResponseTypeDef,
+    DeploymentConfigurationOutputTypeDef,
     DeploymentConfigurationTypeDef,
     DescribeServicesRequestServicesInactiveWaitTypeDef,
     DescribeServicesRequestServicesStableWaitTypeDef,
     DescribeTasksRequestTasksRunningWaitTypeDef,
     DescribeTasksRequestTasksStoppedWaitTypeDef,
     EFSVolumeConfigurationTypeDef,
     ExecuteCommandConfigurationTypeDef,
     ExecuteCommandResponseTypeDef,
     FSxWindowsFileServerVolumeConfigurationTypeDef,
     GetTaskProtectionResponseTypeDef,
     UpdateTaskProtectionResponseTypeDef,
+    LinuxParametersOutputTypeDef,
     LinuxParametersTypeDef,
-    RegisterContainerInstanceRequestRequestTypeDef,
+    ListAccountSettingsRequestListAccountSettingsPaginateTypeDef,
+    ListAttributesRequestListAttributesPaginateTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
+    ListContainerInstancesRequestListContainerInstancesPaginateTypeDef,
+    ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
+    ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef,
+    ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef,
+    ListTasksRequestListTasksPaginateTypeDef,
+    ResourceUnionTypeDef,
+    ServiceConnectServiceOutputTypeDef,
     ServiceConnectServiceTypeDef,
+    ProxyConfigurationUnionTypeDef,
     CapacityProviderTypeDef,
     CreateCapacityProviderRequestRequestTypeDef,
     UpdateCapacityProviderRequestRequestTypeDef,
-    CreateTaskSetRequestRequestTypeDef,
     TaskSetTypeDef,
+    CreateTaskSetRequestRequestTypeDef,
+    NetworkConfigurationUnionTypeDef,
+    TaskOverrideOutputTypeDef,
     TaskOverrideTypeDef,
     ContainerInstanceTypeDef,
     SubmitTaskStateChangeRequestRequestTypeDef,
+    DeploymentConfigurationUnionTypeDef,
     ClusterConfigurationTypeDef,
+    VolumeOutputTypeDef,
     VolumeTypeDef,
+    ContainerDefinitionOutputTypeDef,
     ContainerDefinitionTypeDef,
+    RegisterContainerInstanceRequestRequestTypeDef,
+    ServiceConnectConfigurationOutputTypeDef,
     ServiceConnectConfigurationTypeDef,
     CreateCapacityProviderResponseTypeDef,
     DeleteCapacityProviderResponseTypeDef,
     DescribeCapacityProvidersResponseTypeDef,
     UpdateCapacityProviderResponseTypeDef,
     CreateTaskSetResponseTypeDef,
     DeleteTaskSetResponseTypeDef,
     DescribeTaskSetsResponseTypeDef,
     UpdateServicePrimaryTaskSetResponseTypeDef,
     UpdateTaskSetResponseTypeDef,
+    TaskTypeDef,
     RunTaskRequestRequestTypeDef,
     StartTaskRequestRequestTypeDef,
-    TaskTypeDef,
+    TaskOverrideUnionTypeDef,
     DeregisterContainerInstanceResponseTypeDef,
     DescribeContainerInstancesResponseTypeDef,
     RegisterContainerInstanceResponseTypeDef,
     UpdateContainerAgentResponseTypeDef,
     UpdateContainerInstancesStateResponseTypeDef,
     ClusterTypeDef,
     CreateClusterRequestRequestTypeDef,
     UpdateClusterRequestRequestTypeDef,
-    RegisterTaskDefinitionRequestRequestTypeDef,
+    VolumeUnionTypeDef,
     TaskDefinitionTypeDef,
-    CreateServiceRequestRequestTypeDef,
+    ContainerDefinitionUnionTypeDef,
     DeploymentTypeDef,
+    CreateServiceRequestRequestTypeDef,
+    ServiceConnectConfigurationUnionTypeDef,
     UpdateServiceRequestRequestTypeDef,
     DescribeTasksResponseTypeDef,
     RunTaskResponseTypeDef,
     StartTaskResponseTypeDef,
     StopTaskResponseTypeDef,
     CreateClusterResponseTypeDef,
     DeleteClusterResponseTypeDef,
@@ -618,23 +646,24 @@
     PutClusterCapacityProvidersResponseTypeDef,
     UpdateClusterResponseTypeDef,
     UpdateClusterSettingsResponseTypeDef,
     DeleteTaskDefinitionsResponseTypeDef,
     DeregisterTaskDefinitionResponseTypeDef,
     DescribeTaskDefinitionResponseTypeDef,
     RegisterTaskDefinitionResponseTypeDef,
+    RegisterTaskDefinitionRequestRequestTypeDef,
     ServiceTypeDef,
     CreateServiceResponseTypeDef,
     DeleteServiceResponseTypeDef,
     DescribeServicesResponseTypeDef,
     UpdateServiceResponseTypeDef,
 )
 
 
-def get_structure() -> AttachmentStateChangeTypeDef:
+def get_value() -> AttachmentStateChangeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-ecs-2.5.2/setup.py` & `types-aiobotocore-ecs-2.5.2.post1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ecs",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_ecs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ECS 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore ecs type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore ecs type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_ecs": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs/__init__.py` & `types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs/__init__.pyi` & `types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs/__main__.py` & `types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ECS 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.ECS 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS\nOther"
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

### Comparing `types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs/client.py` & `types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("ecs") as client:
         client: ECSClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     ClusterFieldType,
     CompatibilityType,
@@ -54,28 +53,28 @@
     AttributeTypeDef,
     AutoScalingGroupProviderTypeDef,
     AutoScalingGroupProviderUpdateTypeDef,
     CapacityProviderStrategyItemTypeDef,
     ClusterConfigurationTypeDef,
     ClusterServiceConnectDefaultsRequestTypeDef,
     ClusterSettingTypeDef,
-    ContainerDefinitionTypeDef,
+    ContainerDefinitionUnionTypeDef,
     ContainerStateChangeTypeDef,
     CreateCapacityProviderResponseTypeDef,
     CreateClusterResponseTypeDef,
     CreateServiceResponseTypeDef,
     CreateTaskSetResponseTypeDef,
     DeleteAccountSettingResponseTypeDef,
     DeleteAttributesResponseTypeDef,
     DeleteCapacityProviderResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DeleteServiceResponseTypeDef,
     DeleteTaskDefinitionsResponseTypeDef,
     DeleteTaskSetResponseTypeDef,
-    DeploymentConfigurationTypeDef,
+    DeploymentConfigurationUnionTypeDef,
     DeploymentControllerTypeDef,
     DeregisterContainerInstanceResponseTypeDef,
     DeregisterTaskDefinitionResponseTypeDef,
     DescribeCapacityProvidersResponseTypeDef,
     DescribeClustersResponseTypeDef,
     DescribeContainerInstancesResponseTypeDef,
     DescribeServicesResponseTypeDef,
@@ -96,50 +95,51 @@
     ListTagsForResourceResponseTypeDef,
     ListTaskDefinitionFamiliesResponseTypeDef,
     ListTaskDefinitionsResponseTypeDef,
     ListTasksResponseTypeDef,
     LoadBalancerTypeDef,
     ManagedAgentStateChangeTypeDef,
     NetworkBindingTypeDef,
-    NetworkConfigurationTypeDef,
+    NetworkConfigurationUnionTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     PlatformDeviceTypeDef,
-    ProxyConfigurationTypeDef,
+    ProxyConfigurationUnionTypeDef,
     PutAccountSettingDefaultResponseTypeDef,
     PutAccountSettingResponseTypeDef,
     PutAttributesResponseTypeDef,
     PutClusterCapacityProvidersResponseTypeDef,
     RegisterContainerInstanceResponseTypeDef,
     RegisterTaskDefinitionResponseTypeDef,
-    ResourceTypeDef,
+    ResourceUnionTypeDef,
     RunTaskResponseTypeDef,
     RuntimePlatformTypeDef,
     ScaleTypeDef,
-    ServiceConnectConfigurationTypeDef,
+    ServiceConnectConfigurationUnionTypeDef,
     ServiceRegistryTypeDef,
     StartTaskResponseTypeDef,
     StopTaskResponseTypeDef,
     SubmitAttachmentStateChangesResponseTypeDef,
     SubmitContainerStateChangeResponseTypeDef,
     SubmitTaskStateChangeResponseTypeDef,
     TagTypeDef,
     TaskDefinitionPlacementConstraintTypeDef,
-    TaskOverrideTypeDef,
+    TaskOverrideUnionTypeDef,
+    TimestampTypeDef,
     UpdateCapacityProviderResponseTypeDef,
     UpdateClusterResponseTypeDef,
     UpdateClusterSettingsResponseTypeDef,
     UpdateContainerAgentResponseTypeDef,
     UpdateContainerInstancesStateResponseTypeDef,
     UpdateServicePrimaryTaskSetResponseTypeDef,
     UpdateServiceResponseTypeDef,
     UpdateTaskProtectionResponseTypeDef,
     UpdateTaskSetResponseTypeDef,
     VersionInfoTypeDef,
-    VolumeTypeDef,
+    VolumeUnionTypeDef,
 )
 from .waiter import (
     ServicesInactiveWaiter,
     ServicesStableWaiter,
     TasksRunningWaiter,
     TasksStoppedWaiter,
 )
@@ -265,26 +265,26 @@
         serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,
         desiredCount: int = ...,
         clientToken: str = ...,
         launchType: LaunchTypeType = ...,
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
         platformVersion: str = ...,
         role: str = ...,
-        deploymentConfiguration: DeploymentConfigurationTypeDef = ...,
+        deploymentConfiguration: DeploymentConfigurationUnionTypeDef = ...,
         placementConstraints: Sequence[PlacementConstraintTypeDef] = ...,
         placementStrategy: Sequence[PlacementStrategyTypeDef] = ...,
-        networkConfiguration: NetworkConfigurationTypeDef = ...,
+        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
         healthCheckGracePeriodSeconds: int = ...,
         schedulingStrategy: SchedulingStrategyType = ...,
         deploymentController: DeploymentControllerTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         enableECSManagedTags: bool = ...,
         propagateTags: PropagateTagsType = ...,
         enableExecuteCommand: bool = ...,
-        serviceConnectConfiguration: ServiceConnectConfigurationTypeDef = ...
+        serviceConnectConfiguration: ServiceConnectConfigurationUnionTypeDef = ...
     ) -> CreateServiceResponseTypeDef:
         """
         Runs and maintains your desired number of tasks from a specified task
         definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.create_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#create_service)
@@ -293,15 +293,15 @@
     async def create_task_set(
         self,
         *,
         service: str,
         cluster: str,
         taskDefinition: str,
         externalId: str = ...,
-        networkConfiguration: NetworkConfigurationTypeDef = ...,
+        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
         loadBalancers: Sequence[LoadBalancerTypeDef] = ...,
         serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,
         launchType: LaunchTypeType = ...,
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
         platformVersion: str = ...,
         scale: ScaleTypeDef = ...,
         clientToken: str = ...,
@@ -738,15 +738,15 @@
 
     async def register_container_instance(
         self,
         *,
         cluster: str = ...,
         instanceIdentityDocument: str = ...,
         instanceIdentityDocumentSignature: str = ...,
-        totalResources: Sequence[ResourceTypeDef] = ...,
+        totalResources: Sequence[ResourceUnionTypeDef] = ...,
         versionInfo: VersionInfoTypeDef = ...,
         containerInstanceArn: str = ...,
         attributes: Sequence[AttributeTypeDef] = ...,
         platformDevices: Sequence[PlatformDeviceTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> RegisterContainerInstanceResponseTypeDef:
         """
@@ -756,27 +756,27 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#register_container_instance)
         """
 
     async def register_task_definition(
         self,
         *,
         family: str,
-        containerDefinitions: Sequence[ContainerDefinitionTypeDef],
+        containerDefinitions: Sequence[ContainerDefinitionUnionTypeDef],
         taskRoleArn: str = ...,
         executionRoleArn: str = ...,
         networkMode: NetworkModeType = ...,
-        volumes: Sequence[VolumeTypeDef] = ...,
+        volumes: Sequence[VolumeUnionTypeDef] = ...,
         placementConstraints: Sequence[TaskDefinitionPlacementConstraintTypeDef] = ...,
         requiresCompatibilities: Sequence[CompatibilityType] = ...,
         cpu: str = ...,
         memory: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         pidMode: PidModeType = ...,
         ipcMode: IpcModeType = ...,
-        proxyConfiguration: ProxyConfigurationTypeDef = ...,
+        proxyConfiguration: ProxyConfigurationUnionTypeDef = ...,
         inferenceAccelerators: Sequence[InferenceAcceleratorTypeDef] = ...,
         ephemeralStorage: EphemeralStorageTypeDef = ...,
         runtimePlatform: RuntimePlatformTypeDef = ...
     ) -> RegisterTaskDefinitionResponseTypeDef:
         """
         Registers a new task definition from the supplied `family` and
         `containerDefinitions`.
@@ -792,16 +792,16 @@
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
         cluster: str = ...,
         count: int = ...,
         enableECSManagedTags: bool = ...,
         enableExecuteCommand: bool = ...,
         group: str = ...,
         launchType: LaunchTypeType = ...,
-        networkConfiguration: NetworkConfigurationTypeDef = ...,
-        overrides: TaskOverrideTypeDef = ...,
+        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
+        overrides: TaskOverrideUnionTypeDef = ...,
         placementConstraints: Sequence[PlacementConstraintTypeDef] = ...,
         placementStrategy: Sequence[PlacementStrategyTypeDef] = ...,
         platformVersion: str = ...,
         propagateTags: PropagateTagsType = ...,
         referenceId: str = ...,
         startedBy: str = ...,
         tags: Sequence[TagTypeDef] = ...
@@ -818,16 +818,16 @@
         *,
         containerInstances: Sequence[str],
         taskDefinition: str,
         cluster: str = ...,
         enableECSManagedTags: bool = ...,
         enableExecuteCommand: bool = ...,
         group: str = ...,
-        networkConfiguration: NetworkConfigurationTypeDef = ...,
-        overrides: TaskOverrideTypeDef = ...,
+        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
+        overrides: TaskOverrideUnionTypeDef = ...,
         propagateTags: PropagateTagsType = ...,
         referenceId: str = ...,
         startedBy: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> StartTaskResponseTypeDef:
         """
         Starts a new task from the specified task definition on the specified container
@@ -882,17 +882,17 @@
         cluster: str = ...,
         task: str = ...,
         status: str = ...,
         reason: str = ...,
         containers: Sequence[ContainerStateChangeTypeDef] = ...,
         attachments: Sequence[AttachmentStateChangeTypeDef] = ...,
         managedAgents: Sequence[ManagedAgentStateChangeTypeDef] = ...,
-        pullStartedAt: Union[datetime, str] = ...,
-        pullStoppedAt: Union[datetime, str] = ...,
-        executionStoppedAt: Union[datetime, str] = ...
+        pullStartedAt: TimestampTypeDef = ...,
+        pullStoppedAt: TimestampTypeDef = ...,
+        executionStoppedAt: TimestampTypeDef = ...
     ) -> SubmitTaskStateChangeResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.submit_task_state_change)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#submit_task_state_change)
         """
@@ -976,27 +976,27 @@
         self,
         *,
         service: str,
         cluster: str = ...,
         desiredCount: int = ...,
         taskDefinition: str = ...,
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
-        deploymentConfiguration: DeploymentConfigurationTypeDef = ...,
-        networkConfiguration: NetworkConfigurationTypeDef = ...,
+        deploymentConfiguration: DeploymentConfigurationUnionTypeDef = ...,
+        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
         placementConstraints: Sequence[PlacementConstraintTypeDef] = ...,
         placementStrategy: Sequence[PlacementStrategyTypeDef] = ...,
         platformVersion: str = ...,
         forceNewDeployment: bool = ...,
         healthCheckGracePeriodSeconds: int = ...,
         enableExecuteCommand: bool = ...,
         enableECSManagedTags: bool = ...,
         loadBalancers: Sequence[LoadBalancerTypeDef] = ...,
         propagateTags: PropagateTagsType = ...,
         serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,
-        serviceConnectConfiguration: ServiceConnectConfigurationTypeDef = ...
+        serviceConnectConfiguration: ServiceConnectConfigurationUnionTypeDef = ...
     ) -> UpdateServiceResponseTypeDef:
         """
         Modifies the parameters of a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#update_service)
         """
```

### Comparing `types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs/client.pyi` & `types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("ecs") as client:
         client: ECSClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     ClusterFieldType,
     CompatibilityType,
@@ -54,28 +53,28 @@
     AttributeTypeDef,
     AutoScalingGroupProviderTypeDef,
     AutoScalingGroupProviderUpdateTypeDef,
     CapacityProviderStrategyItemTypeDef,
     ClusterConfigurationTypeDef,
     ClusterServiceConnectDefaultsRequestTypeDef,
     ClusterSettingTypeDef,
-    ContainerDefinitionTypeDef,
+    ContainerDefinitionUnionTypeDef,
     ContainerStateChangeTypeDef,
     CreateCapacityProviderResponseTypeDef,
     CreateClusterResponseTypeDef,
     CreateServiceResponseTypeDef,
     CreateTaskSetResponseTypeDef,
     DeleteAccountSettingResponseTypeDef,
     DeleteAttributesResponseTypeDef,
     DeleteCapacityProviderResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DeleteServiceResponseTypeDef,
     DeleteTaskDefinitionsResponseTypeDef,
     DeleteTaskSetResponseTypeDef,
-    DeploymentConfigurationTypeDef,
+    DeploymentConfigurationUnionTypeDef,
     DeploymentControllerTypeDef,
     DeregisterContainerInstanceResponseTypeDef,
     DeregisterTaskDefinitionResponseTypeDef,
     DescribeCapacityProvidersResponseTypeDef,
     DescribeClustersResponseTypeDef,
     DescribeContainerInstancesResponseTypeDef,
     DescribeServicesResponseTypeDef,
@@ -96,50 +95,51 @@
     ListTagsForResourceResponseTypeDef,
     ListTaskDefinitionFamiliesResponseTypeDef,
     ListTaskDefinitionsResponseTypeDef,
     ListTasksResponseTypeDef,
     LoadBalancerTypeDef,
     ManagedAgentStateChangeTypeDef,
     NetworkBindingTypeDef,
-    NetworkConfigurationTypeDef,
+    NetworkConfigurationUnionTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     PlatformDeviceTypeDef,
-    ProxyConfigurationTypeDef,
+    ProxyConfigurationUnionTypeDef,
     PutAccountSettingDefaultResponseTypeDef,
     PutAccountSettingResponseTypeDef,
     PutAttributesResponseTypeDef,
     PutClusterCapacityProvidersResponseTypeDef,
     RegisterContainerInstanceResponseTypeDef,
     RegisterTaskDefinitionResponseTypeDef,
-    ResourceTypeDef,
+    ResourceUnionTypeDef,
     RunTaskResponseTypeDef,
     RuntimePlatformTypeDef,
     ScaleTypeDef,
-    ServiceConnectConfigurationTypeDef,
+    ServiceConnectConfigurationUnionTypeDef,
     ServiceRegistryTypeDef,
     StartTaskResponseTypeDef,
     StopTaskResponseTypeDef,
     SubmitAttachmentStateChangesResponseTypeDef,
     SubmitContainerStateChangeResponseTypeDef,
     SubmitTaskStateChangeResponseTypeDef,
     TagTypeDef,
     TaskDefinitionPlacementConstraintTypeDef,
-    TaskOverrideTypeDef,
+    TaskOverrideUnionTypeDef,
+    TimestampTypeDef,
     UpdateCapacityProviderResponseTypeDef,
     UpdateClusterResponseTypeDef,
     UpdateClusterSettingsResponseTypeDef,
     UpdateContainerAgentResponseTypeDef,
     UpdateContainerInstancesStateResponseTypeDef,
     UpdateServicePrimaryTaskSetResponseTypeDef,
     UpdateServiceResponseTypeDef,
     UpdateTaskProtectionResponseTypeDef,
     UpdateTaskSetResponseTypeDef,
     VersionInfoTypeDef,
-    VolumeTypeDef,
+    VolumeUnionTypeDef,
 )
 from .waiter import (
     ServicesInactiveWaiter,
     ServicesStableWaiter,
     TasksRunningWaiter,
     TasksStoppedWaiter,
 )
@@ -256,26 +256,26 @@
         serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,
         desiredCount: int = ...,
         clientToken: str = ...,
         launchType: LaunchTypeType = ...,
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
         platformVersion: str = ...,
         role: str = ...,
-        deploymentConfiguration: DeploymentConfigurationTypeDef = ...,
+        deploymentConfiguration: DeploymentConfigurationUnionTypeDef = ...,
         placementConstraints: Sequence[PlacementConstraintTypeDef] = ...,
         placementStrategy: Sequence[PlacementStrategyTypeDef] = ...,
-        networkConfiguration: NetworkConfigurationTypeDef = ...,
+        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
         healthCheckGracePeriodSeconds: int = ...,
         schedulingStrategy: SchedulingStrategyType = ...,
         deploymentController: DeploymentControllerTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         enableECSManagedTags: bool = ...,
         propagateTags: PropagateTagsType = ...,
         enableExecuteCommand: bool = ...,
-        serviceConnectConfiguration: ServiceConnectConfigurationTypeDef = ...
+        serviceConnectConfiguration: ServiceConnectConfigurationUnionTypeDef = ...
     ) -> CreateServiceResponseTypeDef:
         """
         Runs and maintains your desired number of tasks from a specified task
         definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.create_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#create_service)
@@ -283,15 +283,15 @@
     async def create_task_set(
         self,
         *,
         service: str,
         cluster: str,
         taskDefinition: str,
         externalId: str = ...,
-        networkConfiguration: NetworkConfigurationTypeDef = ...,
+        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
         loadBalancers: Sequence[LoadBalancerTypeDef] = ...,
         serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,
         launchType: LaunchTypeType = ...,
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
         platformVersion: str = ...,
         scale: ScaleTypeDef = ...,
         clientToken: str = ...,
@@ -693,15 +693,15 @@
         """
     async def register_container_instance(
         self,
         *,
         cluster: str = ...,
         instanceIdentityDocument: str = ...,
         instanceIdentityDocumentSignature: str = ...,
-        totalResources: Sequence[ResourceTypeDef] = ...,
+        totalResources: Sequence[ResourceUnionTypeDef] = ...,
         versionInfo: VersionInfoTypeDef = ...,
         containerInstanceArn: str = ...,
         attributes: Sequence[AttributeTypeDef] = ...,
         platformDevices: Sequence[PlatformDeviceTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> RegisterContainerInstanceResponseTypeDef:
         """
@@ -710,27 +710,27 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.register_container_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#register_container_instance)
         """
     async def register_task_definition(
         self,
         *,
         family: str,
-        containerDefinitions: Sequence[ContainerDefinitionTypeDef],
+        containerDefinitions: Sequence[ContainerDefinitionUnionTypeDef],
         taskRoleArn: str = ...,
         executionRoleArn: str = ...,
         networkMode: NetworkModeType = ...,
-        volumes: Sequence[VolumeTypeDef] = ...,
+        volumes: Sequence[VolumeUnionTypeDef] = ...,
         placementConstraints: Sequence[TaskDefinitionPlacementConstraintTypeDef] = ...,
         requiresCompatibilities: Sequence[CompatibilityType] = ...,
         cpu: str = ...,
         memory: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         pidMode: PidModeType = ...,
         ipcMode: IpcModeType = ...,
-        proxyConfiguration: ProxyConfigurationTypeDef = ...,
+        proxyConfiguration: ProxyConfigurationUnionTypeDef = ...,
         inferenceAccelerators: Sequence[InferenceAcceleratorTypeDef] = ...,
         ephemeralStorage: EphemeralStorageTypeDef = ...,
         runtimePlatform: RuntimePlatformTypeDef = ...
     ) -> RegisterTaskDefinitionResponseTypeDef:
         """
         Registers a new task definition from the supplied `family` and
         `containerDefinitions`.
@@ -745,16 +745,16 @@
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
         cluster: str = ...,
         count: int = ...,
         enableECSManagedTags: bool = ...,
         enableExecuteCommand: bool = ...,
         group: str = ...,
         launchType: LaunchTypeType = ...,
-        networkConfiguration: NetworkConfigurationTypeDef = ...,
-        overrides: TaskOverrideTypeDef = ...,
+        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
+        overrides: TaskOverrideUnionTypeDef = ...,
         placementConstraints: Sequence[PlacementConstraintTypeDef] = ...,
         placementStrategy: Sequence[PlacementStrategyTypeDef] = ...,
         platformVersion: str = ...,
         propagateTags: PropagateTagsType = ...,
         referenceId: str = ...,
         startedBy: str = ...,
         tags: Sequence[TagTypeDef] = ...
@@ -770,16 +770,16 @@
         *,
         containerInstances: Sequence[str],
         taskDefinition: str,
         cluster: str = ...,
         enableECSManagedTags: bool = ...,
         enableExecuteCommand: bool = ...,
         group: str = ...,
-        networkConfiguration: NetworkConfigurationTypeDef = ...,
-        overrides: TaskOverrideTypeDef = ...,
+        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
+        overrides: TaskOverrideUnionTypeDef = ...,
         propagateTags: PropagateTagsType = ...,
         referenceId: str = ...,
         startedBy: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> StartTaskResponseTypeDef:
         """
         Starts a new task from the specified task definition on the specified container
@@ -830,17 +830,17 @@
         cluster: str = ...,
         task: str = ...,
         status: str = ...,
         reason: str = ...,
         containers: Sequence[ContainerStateChangeTypeDef] = ...,
         attachments: Sequence[AttachmentStateChangeTypeDef] = ...,
         managedAgents: Sequence[ManagedAgentStateChangeTypeDef] = ...,
-        pullStartedAt: Union[datetime, str] = ...,
-        pullStoppedAt: Union[datetime, str] = ...,
-        executionStoppedAt: Union[datetime, str] = ...
+        pullStartedAt: TimestampTypeDef = ...,
+        pullStoppedAt: TimestampTypeDef = ...,
+        executionStoppedAt: TimestampTypeDef = ...
     ) -> SubmitTaskStateChangeResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.submit_task_state_change)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#submit_task_state_change)
         """
@@ -916,27 +916,27 @@
         self,
         *,
         service: str,
         cluster: str = ...,
         desiredCount: int = ...,
         taskDefinition: str = ...,
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
-        deploymentConfiguration: DeploymentConfigurationTypeDef = ...,
-        networkConfiguration: NetworkConfigurationTypeDef = ...,
+        deploymentConfiguration: DeploymentConfigurationUnionTypeDef = ...,
+        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
         placementConstraints: Sequence[PlacementConstraintTypeDef] = ...,
         placementStrategy: Sequence[PlacementStrategyTypeDef] = ...,
         platformVersion: str = ...,
         forceNewDeployment: bool = ...,
         healthCheckGracePeriodSeconds: int = ...,
         enableExecuteCommand: bool = ...,
         enableECSManagedTags: bool = ...,
         loadBalancers: Sequence[LoadBalancerTypeDef] = ...,
         propagateTags: PropagateTagsType = ...,
         serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,
-        serviceConnectConfiguration: ServiceConnectConfigurationTypeDef = ...
+        serviceConnectConfiguration: ServiceConnectConfigurationUnionTypeDef = ...
     ) -> UpdateServiceResponseTypeDef:
         """
         Modifies the parameters of a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#update_service)
         """
```

### Comparing `types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs/literals.py` & `types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs/literals.pyi` & `types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs/paginator.py` & `types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -66,189 +66,177 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListAccountSettingsPaginator",
     "ListAttributesPaginator",
     "ListClustersPaginator",
     "ListContainerInstancesPaginator",
     "ListServicesPaginator",
     "ListServicesByNamespacePaginator",
     "ListTaskDefinitionFamiliesPaginator",
     "ListTaskDefinitionsPaginator",
     "ListTasksPaginator",
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
 class ListAccountSettingsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAccountSettings)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listaccountsettingspaginator)
     """
 
     def paginate(
         self,
         *,
         name: SettingNameType = ...,
         value: str = ...,
         principalArn: str = ...,
         effectiveSettings: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAccountSettingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAccountSettings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listaccountsettingspaginator)
         """
 
-
 class ListAttributesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAttributes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listattributespaginator)
     """
 
     def paginate(
         self,
         *,
         targetType: Literal["container-instance"],
         cluster: str = ...,
         attributeName: str = ...,
         attributeValue: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAttributes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listattributespaginator)
         """
 
-
 class ListClustersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListClusters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listclusterspaginator)
         """
 
-
 class ListContainerInstancesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListContainerInstances)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listcontainerinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         cluster: str = ...,
         filter: str = ...,
         status: ContainerInstanceStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListContainerInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListContainerInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listcontainerinstancespaginator)
         """
 
-
 class ListServicesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServices)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listservicespaginator)
     """
 
     def paginate(
         self,
         *,
         cluster: str = ...,
         launchType: LaunchTypeType = ...,
         schedulingStrategy: SchedulingStrategyType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listservicespaginator)
         """
 
-
 class ListServicesByNamespacePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServicesByNamespace)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listservicesbynamespacepaginator)
     """
 
     def paginate(
-        self, *, namespace: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, namespace: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServicesByNamespaceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServicesByNamespace.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listservicesbynamespacepaginator)
         """
 
-
 class ListTaskDefinitionFamiliesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitionFamilies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listtaskdefinitionfamiliespaginator)
     """
 
     def paginate(
         self,
         *,
         familyPrefix: str = ...,
         status: TaskDefinitionFamilyStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTaskDefinitionFamiliesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitionFamilies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listtaskdefinitionfamiliespaginator)
         """
 
-
 class ListTaskDefinitionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listtaskdefinitionspaginator)
     """
 
     def paginate(
         self,
         *,
         familyPrefix: str = ...,
         status: TaskDefinitionStatusType = ...,
         sort: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTaskDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listtaskdefinitionspaginator)
         """
 
-
 class ListTasksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTasks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listtaskspaginator)
     """
 
     def paginate(
@@ -257,13 +245,13 @@
         cluster: str = ...,
         containerInstance: str = ...,
         family: str = ...,
         startedBy: str = ...,
         serviceName: str = ...,
         desiredStatus: DesiredStatusType = ...,
         launchType: LaunchTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listtaskspaginator)
         """
```

### Comparing `types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs/paginator.pyi` & `types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/paginator.py`

 * *Files 7% similar despite different names*

```diff
@@ -66,177 +66,189 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ListAccountSettingsPaginator",
     "ListAttributesPaginator",
     "ListClustersPaginator",
     "ListContainerInstancesPaginator",
     "ListServicesPaginator",
     "ListServicesByNamespacePaginator",
     "ListTaskDefinitionFamiliesPaginator",
     "ListTaskDefinitionsPaginator",
     "ListTasksPaginator",
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
 class ListAccountSettingsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAccountSettings)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listaccountsettingspaginator)
     """
 
     def paginate(
         self,
         *,
         name: SettingNameType = ...,
         value: str = ...,
         principalArn: str = ...,
         effectiveSettings: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAccountSettingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAccountSettings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listaccountsettingspaginator)
         """
 
+
 class ListAttributesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAttributes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listattributespaginator)
     """
 
     def paginate(
         self,
         *,
         targetType: Literal["container-instance"],
         cluster: str = ...,
         attributeName: str = ...,
         attributeValue: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAttributes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listattributespaginator)
         """
 
+
 class ListClustersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListClusters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listclusterspaginator)
         """
 
+
 class ListContainerInstancesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListContainerInstances)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listcontainerinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         cluster: str = ...,
         filter: str = ...,
         status: ContainerInstanceStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListContainerInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListContainerInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listcontainerinstancespaginator)
         """
 
+
 class ListServicesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServices)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listservicespaginator)
     """
 
     def paginate(
         self,
         *,
         cluster: str = ...,
         launchType: LaunchTypeType = ...,
         schedulingStrategy: SchedulingStrategyType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listservicespaginator)
         """
 
+
 class ListServicesByNamespacePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServicesByNamespace)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listservicesbynamespacepaginator)
     """
 
     def paginate(
-        self, *, namespace: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, namespace: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServicesByNamespaceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServicesByNamespace.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listservicesbynamespacepaginator)
         """
 
+
 class ListTaskDefinitionFamiliesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitionFamilies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listtaskdefinitionfamiliespaginator)
     """
 
     def paginate(
         self,
         *,
         familyPrefix: str = ...,
         status: TaskDefinitionFamilyStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTaskDefinitionFamiliesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitionFamilies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listtaskdefinitionfamiliespaginator)
         """
 
+
 class ListTaskDefinitionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listtaskdefinitionspaginator)
     """
 
     def paginate(
         self,
         *,
         familyPrefix: str = ...,
         status: TaskDefinitionStatusType = ...,
         sort: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTaskDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listtaskdefinitionspaginator)
         """
 
+
 class ListTasksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTasks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listtaskspaginator)
     """
 
     def paginate(
@@ -245,13 +257,13 @@
         cluster: str = ...,
         containerInstance: str = ...,
         family: str = ...,
         startedBy: str = ...,
         serviceName: str = ...,
         desiredStatus: DesiredStatusType = ...,
         launchType: LaunchTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/paginators/#listtaskspaginator)
         """
```

### Comparing `types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs/type_defs.py` & `types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_ecs.type_defs import AttachmentStateChangeTypeDef
 
-    data: AttachmentStateChangeTypeDef = {...}
+    data: AttachmentStateChangeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -67,210 +67,237 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AttachmentStateChangeTypeDef",
     "KeyValuePairTypeDef",
     "AttributeTypeDef",
     "ManagedScalingTypeDef",
+    "AwsVpcConfigurationOutputTypeDef",
     "AwsVpcConfigurationTypeDef",
     "CapacityProviderStrategyItemTypeDef",
     "TagTypeDef",
     "ClusterServiceConnectDefaultsRequestTypeDef",
     "ClusterServiceConnectDefaultsTypeDef",
     "ClusterSettingTypeDef",
     "ContainerDependencyTypeDef",
     "EnvironmentFileTypeDef",
-    "FirelensConfigurationTypeDef",
-    "HealthCheckTypeDef",
+    "FirelensConfigurationOutputTypeDef",
+    "HealthCheckOutputTypeDef",
     "HostEntryTypeDef",
     "MountPointTypeDef",
     "PortMappingTypeDef",
     "RepositoryCredentialsTypeDef",
     "ResourceRequirementTypeDef",
     "SecretTypeDef",
     "SystemControlTypeDef",
     "UlimitTypeDef",
     "VolumeFromTypeDef",
+    "FirelensConfigurationTypeDef",
+    "HealthCheckTypeDef",
     "InstanceHealthCheckResultTypeDef",
-    "ResourceTypeDef",
+    "ResourceOutputTypeDef",
     "VersionInfoTypeDef",
     "NetworkBindingTypeDef",
     "ManagedAgentTypeDef",
     "NetworkInterfaceTypeDef",
+    "ResponseMetadataTypeDef",
     "DeploymentControllerTypeDef",
     "LoadBalancerTypeDef",
     "PlacementConstraintTypeDef",
     "PlacementStrategyTypeDef",
     "ServiceRegistryTypeDef",
     "ScaleTypeDef",
     "DeleteAccountSettingRequestRequestTypeDef",
     "SettingTypeDef",
     "DeleteCapacityProviderRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteServiceRequestRequestTypeDef",
     "DeleteTaskDefinitionsRequestRequestTypeDef",
     "FailureTypeDef",
     "DeleteTaskSetRequestRequestTypeDef",
+    "DeploymentAlarmsOutputTypeDef",
     "DeploymentAlarmsTypeDef",
     "DeploymentCircuitBreakerTypeDef",
     "ServiceConnectServiceResourceTypeDef",
     "DeregisterContainerInstanceRequestRequestTypeDef",
     "DeregisterTaskDefinitionRequestRequestTypeDef",
     "DescribeCapacityProvidersRequestRequestTypeDef",
     "DescribeClustersRequestRequestTypeDef",
     "DescribeContainerInstancesRequestRequestTypeDef",
     "DescribeServicesRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeTaskDefinitionRequestRequestTypeDef",
     "DescribeTaskSetsRequestRequestTypeDef",
     "DescribeTasksRequestRequestTypeDef",
+    "DeviceOutputTypeDef",
     "DeviceTypeDef",
     "DiscoverPollEndpointRequestRequestTypeDef",
-    "DiscoverPollEndpointResponseTypeDef",
+    "DockerVolumeConfigurationOutputTypeDef",
     "DockerVolumeConfigurationTypeDef",
     "EFSAuthorizationConfigTypeDef",
     "EphemeralStorageTypeDef",
     "ExecuteCommandLogConfigurationTypeDef",
     "ExecuteCommandRequestRequestTypeDef",
     "SessionTypeDef",
     "FSxWindowsFileServerAuthorizationConfigTypeDef",
     "GetTaskProtectionRequestRequestTypeDef",
     "ProtectedTaskTypeDef",
     "HostVolumePropertiesTypeDef",
     "InferenceAcceleratorOverrideTypeDef",
     "InferenceAcceleratorTypeDef",
+    "KernelCapabilitiesOutputTypeDef",
     "KernelCapabilitiesTypeDef",
+    "TmpfsOutputTypeDef",
     "TmpfsTypeDef",
-    "ListAccountSettingsRequestListAccountSettingsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccountSettingsRequestRequestTypeDef",
-    "ListAttributesRequestListAttributesPaginateTypeDef",
     "ListAttributesRequestRequestTypeDef",
-    "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
-    "ListClustersResponseTypeDef",
-    "ListContainerInstancesRequestListContainerInstancesPaginateTypeDef",
     "ListContainerInstancesRequestRequestTypeDef",
-    "ListContainerInstancesResponseTypeDef",
-    "ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
     "ListServicesByNamespaceRequestRequestTypeDef",
-    "ListServicesByNamespaceResponseTypeDef",
-    "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
-    "ListServicesResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef",
     "ListTaskDefinitionFamiliesRequestRequestTypeDef",
-    "ListTaskDefinitionFamiliesResponseTypeDef",
-    "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
     "ListTaskDefinitionsRequestRequestTypeDef",
-    "ListTaskDefinitionsResponseTypeDef",
-    "ListTasksRequestListTasksPaginateTypeDef",
     "ListTasksRequestRequestTypeDef",
-    "ListTasksResponseTypeDef",
     "ManagedAgentStateChangeTypeDef",
-    "PaginatorConfigTypeDef",
     "PlatformDeviceTypeDef",
     "PutAccountSettingDefaultRequestRequestTypeDef",
     "PutAccountSettingRequestRequestTypeDef",
     "RuntimePlatformTypeDef",
     "TaskDefinitionPlacementConstraintTypeDef",
-    "ResponseMetadataTypeDef",
+    "ResourceTypeDef",
     "ServiceConnectClientAliasTypeDef",
     "ServiceEventTypeDef",
     "StopTaskRequestRequestTypeDef",
-    "SubmitAttachmentStateChangesResponseTypeDef",
-    "SubmitContainerStateChangeResponseTypeDef",
-    "SubmitTaskStateChangeResponseTypeDef",
+    "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateContainerAgentRequestRequestTypeDef",
     "UpdateContainerInstancesStateRequestRequestTypeDef",
     "UpdateServicePrimaryTaskSetRequestRequestTypeDef",
     "UpdateTaskProtectionRequestRequestTypeDef",
     "SubmitAttachmentStateChangesRequestRequestTypeDef",
     "AttachmentTypeDef",
+    "ProxyConfigurationOutputTypeDef",
     "ProxyConfigurationTypeDef",
     "DeleteAttributesRequestRequestTypeDef",
-    "DeleteAttributesResponseTypeDef",
-    "ListAttributesResponseTypeDef",
     "PutAttributesRequestRequestTypeDef",
-    "PutAttributesResponseTypeDef",
     "AutoScalingGroupProviderTypeDef",
     "AutoScalingGroupProviderUpdateTypeDef",
+    "NetworkConfigurationOutputTypeDef",
     "NetworkConfigurationTypeDef",
     "PutClusterCapacityProvidersRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UpdateClusterSettingsRequestRequestTypeDef",
+    "ContainerOverrideOutputTypeDef",
     "ContainerOverrideTypeDef",
+    "LogConfigurationOutputTypeDef",
     "LogConfigurationTypeDef",
     "ContainerInstanceHealthStatusTypeDef",
     "ContainerStateChangeTypeDef",
     "SubmitContainerStateChangeRequestRequestTypeDef",
     "ContainerTypeDef",
+    "DeleteAttributesResponseTypeDef",
+    "DiscoverPollEndpointResponseTypeDef",
+    "ListAttributesResponseTypeDef",
+    "ListClustersResponseTypeDef",
+    "ListContainerInstancesResponseTypeDef",
+    "ListServicesByNamespaceResponseTypeDef",
+    "ListServicesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListTaskDefinitionFamiliesResponseTypeDef",
+    "ListTaskDefinitionsResponseTypeDef",
+    "ListTasksResponseTypeDef",
+    "PutAttributesResponseTypeDef",
+    "SubmitAttachmentStateChangesResponseTypeDef",
+    "SubmitContainerStateChangeResponseTypeDef",
+    "SubmitTaskStateChangeResponseTypeDef",
     "UpdateTaskSetRequestRequestTypeDef",
     "DeleteAccountSettingResponseTypeDef",
     "ListAccountSettingsResponseTypeDef",
     "PutAccountSettingDefaultResponseTypeDef",
     "PutAccountSettingResponseTypeDef",
+    "DeploymentConfigurationOutputTypeDef",
     "DeploymentConfigurationTypeDef",
     "DescribeServicesRequestServicesInactiveWaitTypeDef",
     "DescribeServicesRequestServicesStableWaitTypeDef",
     "DescribeTasksRequestTasksRunningWaitTypeDef",
     "DescribeTasksRequestTasksStoppedWaitTypeDef",
     "EFSVolumeConfigurationTypeDef",
     "ExecuteCommandConfigurationTypeDef",
     "ExecuteCommandResponseTypeDef",
     "FSxWindowsFileServerVolumeConfigurationTypeDef",
     "GetTaskProtectionResponseTypeDef",
     "UpdateTaskProtectionResponseTypeDef",
+    "LinuxParametersOutputTypeDef",
     "LinuxParametersTypeDef",
-    "RegisterContainerInstanceRequestRequestTypeDef",
+    "ListAccountSettingsRequestListAccountSettingsPaginateTypeDef",
+    "ListAttributesRequestListAttributesPaginateTypeDef",
+    "ListClustersRequestListClustersPaginateTypeDef",
+    "ListContainerInstancesRequestListContainerInstancesPaginateTypeDef",
+    "ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
+    "ListServicesRequestListServicesPaginateTypeDef",
+    "ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef",
+    "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
+    "ListTasksRequestListTasksPaginateTypeDef",
+    "ResourceUnionTypeDef",
+    "ServiceConnectServiceOutputTypeDef",
     "ServiceConnectServiceTypeDef",
+    "ProxyConfigurationUnionTypeDef",
     "CapacityProviderTypeDef",
     "CreateCapacityProviderRequestRequestTypeDef",
     "UpdateCapacityProviderRequestRequestTypeDef",
-    "CreateTaskSetRequestRequestTypeDef",
     "TaskSetTypeDef",
+    "CreateTaskSetRequestRequestTypeDef",
+    "NetworkConfigurationUnionTypeDef",
+    "TaskOverrideOutputTypeDef",
     "TaskOverrideTypeDef",
     "ContainerInstanceTypeDef",
     "SubmitTaskStateChangeRequestRequestTypeDef",
+    "DeploymentConfigurationUnionTypeDef",
     "ClusterConfigurationTypeDef",
+    "VolumeOutputTypeDef",
     "VolumeTypeDef",
+    "ContainerDefinitionOutputTypeDef",
     "ContainerDefinitionTypeDef",
+    "RegisterContainerInstanceRequestRequestTypeDef",
+    "ServiceConnectConfigurationOutputTypeDef",
     "ServiceConnectConfigurationTypeDef",
     "CreateCapacityProviderResponseTypeDef",
     "DeleteCapacityProviderResponseTypeDef",
     "DescribeCapacityProvidersResponseTypeDef",
     "UpdateCapacityProviderResponseTypeDef",
     "CreateTaskSetResponseTypeDef",
     "DeleteTaskSetResponseTypeDef",
     "DescribeTaskSetsResponseTypeDef",
     "UpdateServicePrimaryTaskSetResponseTypeDef",
     "UpdateTaskSetResponseTypeDef",
+    "TaskTypeDef",
     "RunTaskRequestRequestTypeDef",
     "StartTaskRequestRequestTypeDef",
-    "TaskTypeDef",
+    "TaskOverrideUnionTypeDef",
     "DeregisterContainerInstanceResponseTypeDef",
     "DescribeContainerInstancesResponseTypeDef",
     "RegisterContainerInstanceResponseTypeDef",
     "UpdateContainerAgentResponseTypeDef",
     "UpdateContainerInstancesStateResponseTypeDef",
     "ClusterTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "UpdateClusterRequestRequestTypeDef",
-    "RegisterTaskDefinitionRequestRequestTypeDef",
+    "VolumeUnionTypeDef",
     "TaskDefinitionTypeDef",
-    "CreateServiceRequestRequestTypeDef",
+    "ContainerDefinitionUnionTypeDef",
     "DeploymentTypeDef",
+    "CreateServiceRequestRequestTypeDef",
+    "ServiceConnectConfigurationUnionTypeDef",
     "UpdateServiceRequestRequestTypeDef",
     "DescribeTasksResponseTypeDef",
     "RunTaskResponseTypeDef",
     "StartTaskResponseTypeDef",
     "StopTaskResponseTypeDef",
     "CreateClusterResponseTypeDef",
     "DeleteClusterResponseTypeDef",
@@ -278,14 +305,15 @@
     "PutClusterCapacityProvidersResponseTypeDef",
     "UpdateClusterResponseTypeDef",
     "UpdateClusterSettingsResponseTypeDef",
     "DeleteTaskDefinitionsResponseTypeDef",
     "DeregisterTaskDefinitionResponseTypeDef",
     "DescribeTaskDefinitionResponseTypeDef",
     "RegisterTaskDefinitionResponseTypeDef",
+    "RegisterTaskDefinitionRequestRequestTypeDef",
     "ServiceTypeDef",
     "CreateServiceResponseTypeDef",
     "DeleteServiceResponseTypeDef",
     "DescribeServicesResponseTypeDef",
     "UpdateServiceResponseTypeDef",
 )
 
@@ -318,31 +346,49 @@
         "value": str,
         "targetType": Literal["container-instance"],
         "targetId": str,
     },
     total=False,
 )
 
-
 class AttributeTypeDef(_RequiredAttributeTypeDef, _OptionalAttributeTypeDef):
     pass
 
-
 ManagedScalingTypeDef = TypedDict(
     "ManagedScalingTypeDef",
     {
         "status": ManagedScalingStatusType,
         "targetCapacity": int,
         "minimumScalingStepSize": int,
         "maximumScalingStepSize": int,
         "instanceWarmupPeriod": int,
     },
     total=False,
 )
 
+_RequiredAwsVpcConfigurationOutputTypeDef = TypedDict(
+    "_RequiredAwsVpcConfigurationOutputTypeDef",
+    {
+        "subnets": List[str],
+    },
+)
+_OptionalAwsVpcConfigurationOutputTypeDef = TypedDict(
+    "_OptionalAwsVpcConfigurationOutputTypeDef",
+    {
+        "securityGroups": List[str],
+        "assignPublicIp": AssignPublicIpType,
+    },
+    total=False,
+)
+
+class AwsVpcConfigurationOutputTypeDef(
+    _RequiredAwsVpcConfigurationOutputTypeDef, _OptionalAwsVpcConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredAwsVpcConfigurationTypeDef = TypedDict(
     "_RequiredAwsVpcConfigurationTypeDef",
     {
         "subnets": Sequence[str],
     },
 )
 _OptionalAwsVpcConfigurationTypeDef = TypedDict(
@@ -350,21 +396,19 @@
     {
         "securityGroups": Sequence[str],
         "assignPublicIp": AssignPublicIpType,
     },
     total=False,
 )
 
-
 class AwsVpcConfigurationTypeDef(
     _RequiredAwsVpcConfigurationTypeDef, _OptionalAwsVpcConfigurationTypeDef
 ):
     pass
 
-
 _RequiredCapacityProviderStrategyItemTypeDef = TypedDict(
     "_RequiredCapacityProviderStrategyItemTypeDef",
     {
         "capacityProvider": str,
     },
 )
 _OptionalCapacityProviderStrategyItemTypeDef = TypedDict(
@@ -372,21 +416,19 @@
     {
         "weight": int,
         "base": int,
     },
     total=False,
 )
 
-
 class CapacityProviderStrategyItemTypeDef(
     _RequiredCapacityProviderStrategyItemTypeDef, _OptionalCapacityProviderStrategyItemTypeDef
 ):
     pass
 
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
@@ -428,57 +470,55 @@
     "EnvironmentFileTypeDef",
     {
         "value": str,
         "type": Literal["s3"],
     },
 )
 
-_RequiredFirelensConfigurationTypeDef = TypedDict(
-    "_RequiredFirelensConfigurationTypeDef",
+_RequiredFirelensConfigurationOutputTypeDef = TypedDict(
+    "_RequiredFirelensConfigurationOutputTypeDef",
     {
         "type": FirelensConfigurationTypeType,
     },
 )
-_OptionalFirelensConfigurationTypeDef = TypedDict(
-    "_OptionalFirelensConfigurationTypeDef",
+_OptionalFirelensConfigurationOutputTypeDef = TypedDict(
+    "_OptionalFirelensConfigurationOutputTypeDef",
     {
         "options": Dict[str, str],
     },
     total=False,
 )
 
-
-class FirelensConfigurationTypeDef(
-    _RequiredFirelensConfigurationTypeDef, _OptionalFirelensConfigurationTypeDef
+class FirelensConfigurationOutputTypeDef(
+    _RequiredFirelensConfigurationOutputTypeDef, _OptionalFirelensConfigurationOutputTypeDef
 ):
     pass
 
-
-_RequiredHealthCheckTypeDef = TypedDict(
-    "_RequiredHealthCheckTypeDef",
+_RequiredHealthCheckOutputTypeDef = TypedDict(
+    "_RequiredHealthCheckOutputTypeDef",
     {
         "command": List[str],
     },
 )
-_OptionalHealthCheckTypeDef = TypedDict(
-    "_OptionalHealthCheckTypeDef",
+_OptionalHealthCheckOutputTypeDef = TypedDict(
+    "_OptionalHealthCheckOutputTypeDef",
     {
         "interval": int,
         "timeout": int,
         "retries": int,
         "startPeriod": int,
     },
     total=False,
 )
 
-
-class HealthCheckTypeDef(_RequiredHealthCheckTypeDef, _OptionalHealthCheckTypeDef):
+class HealthCheckOutputTypeDef(
+    _RequiredHealthCheckOutputTypeDef, _OptionalHealthCheckOutputTypeDef
+):
     pass
 
-
 HostEntryTypeDef = TypedDict(
     "HostEntryTypeDef",
     {
         "hostname": str,
         "ipAddress": str,
     },
 )
@@ -552,27 +592,66 @@
     {
         "sourceContainer": str,
         "readOnly": bool,
     },
     total=False,
 )
 
+_RequiredFirelensConfigurationTypeDef = TypedDict(
+    "_RequiredFirelensConfigurationTypeDef",
+    {
+        "type": FirelensConfigurationTypeType,
+    },
+)
+_OptionalFirelensConfigurationTypeDef = TypedDict(
+    "_OptionalFirelensConfigurationTypeDef",
+    {
+        "options": Mapping[str, str],
+    },
+    total=False,
+)
+
+class FirelensConfigurationTypeDef(
+    _RequiredFirelensConfigurationTypeDef, _OptionalFirelensConfigurationTypeDef
+):
+    pass
+
+_RequiredHealthCheckTypeDef = TypedDict(
+    "_RequiredHealthCheckTypeDef",
+    {
+        "command": Sequence[str],
+    },
+)
+_OptionalHealthCheckTypeDef = TypedDict(
+    "_OptionalHealthCheckTypeDef",
+    {
+        "interval": int,
+        "timeout": int,
+        "retries": int,
+        "startPeriod": int,
+    },
+    total=False,
+)
+
+class HealthCheckTypeDef(_RequiredHealthCheckTypeDef, _OptionalHealthCheckTypeDef):
+    pass
+
 InstanceHealthCheckResultTypeDef = TypedDict(
     "InstanceHealthCheckResultTypeDef",
     {
         "type": Literal["CONTAINER_RUNTIME"],
         "status": InstanceHealthCheckStateType,
         "lastUpdated": datetime,
         "lastStatusChange": datetime,
     },
     total=False,
 )
 
-ResourceTypeDef = TypedDict(
-    "ResourceTypeDef",
+ResourceOutputTypeDef = TypedDict(
+    "ResourceOutputTypeDef",
     {
         "name": str,
         "type": str,
         "doubleValue": float,
         "longValue": int,
         "integerValue": int,
         "stringSetValue": List[str],
@@ -620,14 +699,25 @@
         "attachmentId": str,
         "privateIpv4Address": str,
         "ipv6Address": str,
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
 DeploymentControllerTypeDef = TypedDict(
     "DeploymentControllerTypeDef",
     {
         "type": DeploymentControllerTypeType,
     },
 )
 
@@ -690,22 +780,20 @@
     "_OptionalDeleteAccountSettingRequestRequestTypeDef",
     {
         "principalArn": str,
     },
     total=False,
 )
 
-
 class DeleteAccountSettingRequestRequestTypeDef(
     _RequiredDeleteAccountSettingRequestRequestTypeDef,
     _OptionalDeleteAccountSettingRequestRequestTypeDef,
 ):
     pass
 
-
 SettingTypeDef = TypedDict(
     "SettingTypeDef",
     {
         "name": SettingNameType,
         "value": str,
         "principalArn": str,
     },
@@ -737,21 +825,19 @@
     {
         "cluster": str,
         "force": bool,
     },
     total=False,
 )
 
-
 class DeleteServiceRequestRequestTypeDef(
     _RequiredDeleteServiceRequestRequestTypeDef, _OptionalDeleteServiceRequestRequestTypeDef
 ):
     pass
 
-
 DeleteTaskDefinitionsRequestRequestTypeDef = TypedDict(
     "DeleteTaskDefinitionsRequestRequestTypeDef",
     {
         "taskDefinitions": Sequence[str],
     },
 )
 
@@ -777,20 +863,27 @@
     "_OptionalDeleteTaskSetRequestRequestTypeDef",
     {
         "force": bool,
     },
     total=False,
 )
 
-
 class DeleteTaskSetRequestRequestTypeDef(
     _RequiredDeleteTaskSetRequestRequestTypeDef, _OptionalDeleteTaskSetRequestRequestTypeDef
 ):
     pass
 
+DeploymentAlarmsOutputTypeDef = TypedDict(
+    "DeploymentAlarmsOutputTypeDef",
+    {
+        "alarmNames": List[str],
+        "enable": bool,
+        "rollback": bool,
+    },
+)
 
 DeploymentAlarmsTypeDef = TypedDict(
     "DeploymentAlarmsTypeDef",
     {
         "alarmNames": Sequence[str],
         "enable": bool,
         "rollback": bool,
@@ -825,22 +918,20 @@
     {
         "cluster": str,
         "force": bool,
     },
     total=False,
 )
 
-
 class DeregisterContainerInstanceRequestRequestTypeDef(
     _RequiredDeregisterContainerInstanceRequestRequestTypeDef,
     _OptionalDeregisterContainerInstanceRequestRequestTypeDef,
 ):
     pass
 
-
 DeregisterTaskDefinitionRequestRequestTypeDef = TypedDict(
     "DeregisterTaskDefinitionRequestRequestTypeDef",
     {
         "taskDefinition": str,
     },
 )
 
@@ -875,22 +966,20 @@
     {
         "cluster": str,
         "include": Sequence[ContainerInstanceFieldType],
     },
     total=False,
 )
 
-
 class DescribeContainerInstancesRequestRequestTypeDef(
     _RequiredDescribeContainerInstancesRequestRequestTypeDef,
     _OptionalDescribeContainerInstancesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeServicesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeServicesRequestRequestTypeDef",
     {
         "services": Sequence[str],
     },
 )
 _OptionalDescribeServicesRequestRequestTypeDef = TypedDict(
@@ -898,21 +987,19 @@
     {
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
     },
     total=False,
 )
 
-
 class DescribeServicesRequestRequestTypeDef(
     _RequiredDescribeServicesRequestRequestTypeDef, _OptionalDescribeServicesRequestRequestTypeDef
 ):
     pass
 
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -928,22 +1015,20 @@
     "_OptionalDescribeTaskDefinitionRequestRequestTypeDef",
     {
         "include": Sequence[Literal["TAGS"]],
     },
     total=False,
 )
 
-
 class DescribeTaskDefinitionRequestRequestTypeDef(
     _RequiredDescribeTaskDefinitionRequestRequestTypeDef,
     _OptionalDescribeTaskDefinitionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeTaskSetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTaskSetsRequestRequestTypeDef",
     {
         "cluster": str,
         "service": str,
     },
 )
@@ -952,21 +1037,19 @@
     {
         "taskSets": Sequence[str],
         "include": Sequence[Literal["TAGS"]],
     },
     total=False,
 )
 
-
 class DescribeTaskSetsRequestRequestTypeDef(
     _RequiredDescribeTaskSetsRequestRequestTypeDef, _OptionalDescribeTaskSetsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDescribeTasksRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTasksRequestRequestTypeDef",
     {
         "tasks": Sequence[str],
     },
 )
 _OptionalDescribeTasksRequestRequestTypeDef = TypedDict(
@@ -974,68 +1057,84 @@
     {
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
     },
     total=False,
 )
 
-
 class DescribeTasksRequestRequestTypeDef(
     _RequiredDescribeTasksRequestRequestTypeDef, _OptionalDescribeTasksRequestRequestTypeDef
 ):
     pass
 
+_RequiredDeviceOutputTypeDef = TypedDict(
+    "_RequiredDeviceOutputTypeDef",
+    {
+        "hostPath": str,
+    },
+)
+_OptionalDeviceOutputTypeDef = TypedDict(
+    "_OptionalDeviceOutputTypeDef",
+    {
+        "containerPath": str,
+        "permissions": List[DeviceCgroupPermissionType],
+    },
+    total=False,
+)
+
+class DeviceOutputTypeDef(_RequiredDeviceOutputTypeDef, _OptionalDeviceOutputTypeDef):
+    pass
 
 _RequiredDeviceTypeDef = TypedDict(
     "_RequiredDeviceTypeDef",
     {
         "hostPath": str,
     },
 )
 _OptionalDeviceTypeDef = TypedDict(
     "_OptionalDeviceTypeDef",
     {
         "containerPath": str,
-        "permissions": List[DeviceCgroupPermissionType],
+        "permissions": Sequence[DeviceCgroupPermissionType],
     },
     total=False,
 )
 
-
 class DeviceTypeDef(_RequiredDeviceTypeDef, _OptionalDeviceTypeDef):
     pass
 
-
 DiscoverPollEndpointRequestRequestTypeDef = TypedDict(
     "DiscoverPollEndpointRequestRequestTypeDef",
     {
         "containerInstance": str,
         "cluster": str,
     },
     total=False,
 )
 
-DiscoverPollEndpointResponseTypeDef = TypedDict(
-    "DiscoverPollEndpointResponseTypeDef",
+DockerVolumeConfigurationOutputTypeDef = TypedDict(
+    "DockerVolumeConfigurationOutputTypeDef",
     {
-        "endpoint": str,
-        "telemetryEndpoint": str,
-        "serviceConnectEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "scope": ScopeType,
+        "autoprovision": bool,
+        "driver": str,
+        "driverOpts": Dict[str, str],
+        "labels": Dict[str, str],
     },
+    total=False,
 )
 
 DockerVolumeConfigurationTypeDef = TypedDict(
     "DockerVolumeConfigurationTypeDef",
     {
         "scope": ScopeType,
         "autoprovision": bool,
         "driver": str,
-        "driverOpts": Dict[str, str],
-        "labels": Dict[str, str],
+        "driverOpts": Mapping[str, str],
+        "labels": Mapping[str, str],
     },
     total=False,
 )
 
 EFSAuthorizationConfigTypeDef = TypedDict(
     "EFSAuthorizationConfigTypeDef",
     {
@@ -1077,21 +1176,19 @@
     {
         "cluster": str,
         "container": str,
     },
     total=False,
 )
 
-
 class ExecuteCommandRequestRequestTypeDef(
     _RequiredExecuteCommandRequestRequestTypeDef, _OptionalExecuteCommandRequestRequestTypeDef
 ):
     pass
 
-
 SessionTypeDef = TypedDict(
     "SessionTypeDef",
     {
         "sessionId": str,
         "streamUrl": str,
         "tokenValue": str,
     },
@@ -1116,21 +1213,19 @@
     "_OptionalGetTaskProtectionRequestRequestTypeDef",
     {
         "tasks": Sequence[str],
     },
     total=False,
 )
 
-
 class GetTaskProtectionRequestRequestTypeDef(
     _RequiredGetTaskProtectionRequestRequestTypeDef, _OptionalGetTaskProtectionRequestRequestTypeDef
 ):
     pass
 
-
 ProtectedTaskTypeDef = TypedDict(
     "ProtectedTaskTypeDef",
     {
         "taskArn": str,
         "protectionEnabled": bool,
         "expirationDate": datetime,
     },
@@ -1158,51 +1253,74 @@
     "InferenceAcceleratorTypeDef",
     {
         "deviceName": str,
         "deviceType": str,
     },
 )
 
-KernelCapabilitiesTypeDef = TypedDict(
-    "KernelCapabilitiesTypeDef",
+KernelCapabilitiesOutputTypeDef = TypedDict(
+    "KernelCapabilitiesOutputTypeDef",
     {
         "add": List[str],
         "drop": List[str],
     },
     total=False,
 )
 
+KernelCapabilitiesTypeDef = TypedDict(
+    "KernelCapabilitiesTypeDef",
+    {
+        "add": Sequence[str],
+        "drop": Sequence[str],
+    },
+    total=False,
+)
+
+_RequiredTmpfsOutputTypeDef = TypedDict(
+    "_RequiredTmpfsOutputTypeDef",
+    {
+        "containerPath": str,
+        "size": int,
+    },
+)
+_OptionalTmpfsOutputTypeDef = TypedDict(
+    "_OptionalTmpfsOutputTypeDef",
+    {
+        "mountOptions": List[str],
+    },
+    total=False,
+)
+
+class TmpfsOutputTypeDef(_RequiredTmpfsOutputTypeDef, _OptionalTmpfsOutputTypeDef):
+    pass
+
 _RequiredTmpfsTypeDef = TypedDict(
     "_RequiredTmpfsTypeDef",
     {
         "containerPath": str,
         "size": int,
     },
 )
 _OptionalTmpfsTypeDef = TypedDict(
     "_OptionalTmpfsTypeDef",
     {
-        "mountOptions": List[str],
+        "mountOptions": Sequence[str],
     },
     total=False,
 )
 
-
 class TmpfsTypeDef(_RequiredTmpfsTypeDef, _OptionalTmpfsTypeDef):
     pass
 
-
-ListAccountSettingsRequestListAccountSettingsPaginateTypeDef = TypedDict(
-    "ListAccountSettingsRequestListAccountSettingsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "name": SettingNameType,
-        "value": str,
-        "principalArn": str,
-        "effectiveSettings": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListAccountSettingsRequestRequestTypeDef = TypedDict(
     "ListAccountSettingsRequestRequestTypeDef",
     {
@@ -1212,39 +1330,14 @@
         "effectiveSettings": bool,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListAttributesRequestListAttributesPaginateTypeDef = TypedDict(
-    "_RequiredListAttributesRequestListAttributesPaginateTypeDef",
-    {
-        "targetType": Literal["container-instance"],
-    },
-)
-_OptionalListAttributesRequestListAttributesPaginateTypeDef = TypedDict(
-    "_OptionalListAttributesRequestListAttributesPaginateTypeDef",
-    {
-        "cluster": str,
-        "attributeName": str,
-        "attributeValue": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAttributesRequestListAttributesPaginateTypeDef(
-    _RequiredListAttributesRequestListAttributesPaginateTypeDef,
-    _OptionalListAttributesRequestListAttributesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredListAttributesRequestRequestTypeDef",
     {
         "targetType": Literal["container-instance"],
     },
 )
 _OptionalListAttributesRequestRequestTypeDef = TypedDict(
@@ -1255,101 +1348,40 @@
         "attributeValue": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListAttributesRequestRequestTypeDef(
     _RequiredListAttributesRequestRequestTypeDef, _OptionalListAttributesRequestRequestTypeDef
 ):
     pass
 
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
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListClustersResponseTypeDef = TypedDict(
-    "ListClustersResponseTypeDef",
-    {
-        "clusterArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListContainerInstancesRequestListContainerInstancesPaginateTypeDef = TypedDict(
-    "ListContainerInstancesRequestListContainerInstancesPaginateTypeDef",
-    {
-        "cluster": str,
-        "filter": str,
-        "status": ContainerInstanceStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListContainerInstancesRequestRequestTypeDef = TypedDict(
     "ListContainerInstancesRequestRequestTypeDef",
     {
         "cluster": str,
         "filter": str,
         "nextToken": str,
         "maxResults": int,
         "status": ContainerInstanceStatusType,
     },
     total=False,
 )
 
-ListContainerInstancesResponseTypeDef = TypedDict(
-    "ListContainerInstancesResponseTypeDef",
-    {
-        "containerInstanceArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef = TypedDict(
-    "_RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
-    {
-        "namespace": str,
-    },
-)
-_OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef = TypedDict(
-    "_OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef(
-    _RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
-    _OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListServicesByNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredListServicesByNamespaceRequestRequestTypeDef",
     {
         "namespace": str,
     },
 )
 _OptionalListServicesByNamespaceRequestRequestTypeDef = TypedDict(
@@ -1357,147 +1389,62 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListServicesByNamespaceRequestRequestTypeDef(
     _RequiredListServicesByNamespaceRequestRequestTypeDef,
     _OptionalListServicesByNamespaceRequestRequestTypeDef,
 ):
     pass
 
-
-ListServicesByNamespaceResponseTypeDef = TypedDict(
-    "ListServicesByNamespaceResponseTypeDef",
-    {
-        "serviceArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListServicesRequestListServicesPaginateTypeDef = TypedDict(
-    "ListServicesRequestListServicesPaginateTypeDef",
-    {
-        "cluster": str,
-        "launchType": LaunchTypeType,
-        "schedulingStrategy": SchedulingStrategyType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServicesRequestRequestTypeDef = TypedDict(
     "ListServicesRequestRequestTypeDef",
     {
         "cluster": str,
         "nextToken": str,
         "maxResults": int,
         "launchType": LaunchTypeType,
         "schedulingStrategy": SchedulingStrategyType,
     },
     total=False,
 )
 
-ListServicesResponseTypeDef = TypedDict(
-    "ListServicesResponseTypeDef",
-    {
-        "serviceArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef = TypedDict(
-    "ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef",
-    {
-        "familyPrefix": str,
-        "status": TaskDefinitionFamilyStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTaskDefinitionFamiliesRequestRequestTypeDef = TypedDict(
     "ListTaskDefinitionFamiliesRequestRequestTypeDef",
     {
         "familyPrefix": str,
         "status": TaskDefinitionFamilyStatusType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListTaskDefinitionFamiliesResponseTypeDef = TypedDict(
-    "ListTaskDefinitionFamiliesResponseTypeDef",
-    {
-        "families": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef = TypedDict(
-    "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
-    {
-        "familyPrefix": str,
-        "status": TaskDefinitionStatusType,
-        "sort": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTaskDefinitionsRequestRequestTypeDef = TypedDict(
     "ListTaskDefinitionsRequestRequestTypeDef",
     {
         "familyPrefix": str,
         "status": TaskDefinitionStatusType,
         "sort": SortOrderType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListTaskDefinitionsResponseTypeDef = TypedDict(
-    "ListTaskDefinitionsResponseTypeDef",
-    {
-        "taskDefinitionArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTasksRequestListTasksPaginateTypeDef = TypedDict(
-    "ListTasksRequestListTasksPaginateTypeDef",
-    {
-        "cluster": str,
-        "containerInstance": str,
-        "family": str,
-        "startedBy": str,
-        "serviceName": str,
-        "desiredStatus": DesiredStatusType,
-        "launchType": LaunchTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTasksRequestRequestTypeDef = TypedDict(
     "ListTasksRequestRequestTypeDef",
     {
         "cluster": str,
         "containerInstance": str,
         "family": str,
         "nextToken": str,
@@ -1506,23 +1453,14 @@
         "serviceName": str,
         "desiredStatus": DesiredStatusType,
         "launchType": LaunchTypeType,
     },
     total=False,
 )
 
-ListTasksResponseTypeDef = TypedDict(
-    "ListTasksResponseTypeDef",
-    {
-        "taskArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredManagedAgentStateChangeTypeDef = TypedDict(
     "_RequiredManagedAgentStateChangeTypeDef",
     {
         "containerName": str,
         "managedAgentName": Literal["ExecuteCommandAgent"],
         "status": str,
     },
@@ -1531,31 +1469,19 @@
     "_OptionalManagedAgentStateChangeTypeDef",
     {
         "reason": str,
     },
     total=False,
 )
 
-
 class ManagedAgentStateChangeTypeDef(
     _RequiredManagedAgentStateChangeTypeDef, _OptionalManagedAgentStateChangeTypeDef
 ):
     pass
 
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
 PlatformDeviceTypeDef = TypedDict(
     "PlatformDeviceTypeDef",
     {
         "id": str,
         "type": Literal["GPU"],
     },
 )
@@ -1579,21 +1505,19 @@
     "_OptionalPutAccountSettingRequestRequestTypeDef",
     {
         "principalArn": str,
     },
     total=False,
 )
 
-
 class PutAccountSettingRequestRequestTypeDef(
     _RequiredPutAccountSettingRequestRequestTypeDef, _OptionalPutAccountSettingRequestRequestTypeDef
 ):
     pass
 
-
 RuntimePlatformTypeDef = TypedDict(
     "RuntimePlatformTypeDef",
     {
         "cpuArchitecture": CPUArchitectureType,
         "operatingSystemFamily": OSFamilyType,
     },
     total=False,
@@ -1604,23 +1528,25 @@
     {
         "type": Literal["memberOf"],
         "expression": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ResourceTypeDef = TypedDict(
+    "ResourceTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "name": str,
+        "type": str,
+        "doubleValue": float,
+        "longValue": int,
+        "integerValue": int,
+        "stringSetValue": Sequence[str],
     },
+    total=False,
 )
 
 _RequiredServiceConnectClientAliasTypeDef = TypedDict(
     "_RequiredServiceConnectClientAliasTypeDef",
     {
         "port": int,
     },
@@ -1629,21 +1555,19 @@
     "_OptionalServiceConnectClientAliasTypeDef",
     {
         "dnsName": str,
     },
     total=False,
 )
 
-
 class ServiceConnectClientAliasTypeDef(
     _RequiredServiceConnectClientAliasTypeDef, _OptionalServiceConnectClientAliasTypeDef
 ):
     pass
 
-
 ServiceEventTypeDef = TypedDict(
     "ServiceEventTypeDef",
     {
         "id": str,
         "createdAt": datetime,
         "message": str,
     },
@@ -1661,45 +1585,20 @@
     {
         "cluster": str,
         "reason": str,
     },
     total=False,
 )
 
-
 class StopTaskRequestRequestTypeDef(
     _RequiredStopTaskRequestRequestTypeDef, _OptionalStopTaskRequestRequestTypeDef
 ):
     pass
 
-
-SubmitAttachmentStateChangesResponseTypeDef = TypedDict(
-    "SubmitAttachmentStateChangesResponseTypeDef",
-    {
-        "acknowledgment": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SubmitContainerStateChangeResponseTypeDef = TypedDict(
-    "SubmitContainerStateChangeResponseTypeDef",
-    {
-        "acknowledgment": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SubmitTaskStateChangeResponseTypeDef = TypedDict(
-    "SubmitTaskStateChangeResponseTypeDef",
-    {
-        "acknowledgment": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -1714,22 +1613,20 @@
     "_OptionalUpdateContainerAgentRequestRequestTypeDef",
     {
         "cluster": str,
     },
     total=False,
 )
 
-
 class UpdateContainerAgentRequestRequestTypeDef(
     _RequiredUpdateContainerAgentRequestRequestTypeDef,
     _OptionalUpdateContainerAgentRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateContainerInstancesStateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContainerInstancesStateRequestRequestTypeDef",
     {
         "containerInstances": Sequence[str],
         "status": ContainerInstanceStatusType,
     },
 )
@@ -1737,22 +1634,20 @@
     "_OptionalUpdateContainerInstancesStateRequestRequestTypeDef",
     {
         "cluster": str,
     },
     total=False,
 )
 
-
 class UpdateContainerInstancesStateRequestRequestTypeDef(
     _RequiredUpdateContainerInstancesStateRequestRequestTypeDef,
     _OptionalUpdateContainerInstancesStateRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateServicePrimaryTaskSetRequestRequestTypeDef = TypedDict(
     "UpdateServicePrimaryTaskSetRequestRequestTypeDef",
     {
         "cluster": str,
         "service": str,
         "primaryTaskSet": str,
     },
@@ -1770,144 +1665,129 @@
     "_OptionalUpdateTaskProtectionRequestRequestTypeDef",
     {
         "expiresInMinutes": int,
     },
     total=False,
 )
 
-
 class UpdateTaskProtectionRequestRequestTypeDef(
     _RequiredUpdateTaskProtectionRequestRequestTypeDef,
     _OptionalUpdateTaskProtectionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSubmitAttachmentStateChangesRequestRequestTypeDef = TypedDict(
     "_RequiredSubmitAttachmentStateChangesRequestRequestTypeDef",
     {
         "attachments": Sequence[AttachmentStateChangeTypeDef],
     },
 )
 _OptionalSubmitAttachmentStateChangesRequestRequestTypeDef = TypedDict(
     "_OptionalSubmitAttachmentStateChangesRequestRequestTypeDef",
     {
         "cluster": str,
     },
     total=False,
 )
 
-
 class SubmitAttachmentStateChangesRequestRequestTypeDef(
     _RequiredSubmitAttachmentStateChangesRequestRequestTypeDef,
     _OptionalSubmitAttachmentStateChangesRequestRequestTypeDef,
 ):
     pass
 
-
 AttachmentTypeDef = TypedDict(
     "AttachmentTypeDef",
     {
         "id": str,
         "type": str,
         "status": str,
         "details": List[KeyValuePairTypeDef],
     },
     total=False,
 )
 
+_RequiredProxyConfigurationOutputTypeDef = TypedDict(
+    "_RequiredProxyConfigurationOutputTypeDef",
+    {
+        "containerName": str,
+    },
+)
+_OptionalProxyConfigurationOutputTypeDef = TypedDict(
+    "_OptionalProxyConfigurationOutputTypeDef",
+    {
+        "type": Literal["APPMESH"],
+        "properties": List[KeyValuePairTypeDef],
+    },
+    total=False,
+)
+
+class ProxyConfigurationOutputTypeDef(
+    _RequiredProxyConfigurationOutputTypeDef, _OptionalProxyConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredProxyConfigurationTypeDef = TypedDict(
     "_RequiredProxyConfigurationTypeDef",
     {
         "containerName": str,
     },
 )
 _OptionalProxyConfigurationTypeDef = TypedDict(
     "_OptionalProxyConfigurationTypeDef",
     {
         "type": Literal["APPMESH"],
-        "properties": List[KeyValuePairTypeDef],
+        "properties": Sequence[KeyValuePairTypeDef],
     },
     total=False,
 )
 
-
 class ProxyConfigurationTypeDef(
     _RequiredProxyConfigurationTypeDef, _OptionalProxyConfigurationTypeDef
 ):
     pass
 
-
 _RequiredDeleteAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAttributesRequestRequestTypeDef",
     {
         "attributes": Sequence[AttributeTypeDef],
     },
 )
 _OptionalDeleteAttributesRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteAttributesRequestRequestTypeDef",
     {
         "cluster": str,
     },
     total=False,
 )
 
-
 class DeleteAttributesRequestRequestTypeDef(
     _RequiredDeleteAttributesRequestRequestTypeDef, _OptionalDeleteAttributesRequestRequestTypeDef
 ):
     pass
 
-
-DeleteAttributesResponseTypeDef = TypedDict(
-    "DeleteAttributesResponseTypeDef",
-    {
-        "attributes": List[AttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAttributesResponseTypeDef = TypedDict(
-    "ListAttributesResponseTypeDef",
-    {
-        "attributes": List[AttributeTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutAttributesRequestRequestTypeDef",
     {
         "attributes": Sequence[AttributeTypeDef],
     },
 )
 _OptionalPutAttributesRequestRequestTypeDef = TypedDict(
     "_OptionalPutAttributesRequestRequestTypeDef",
     {
         "cluster": str,
     },
     total=False,
 )
 
-
 class PutAttributesRequestRequestTypeDef(
     _RequiredPutAttributesRequestRequestTypeDef, _OptionalPutAttributesRequestRequestTypeDef
 ):
     pass
 
-
-PutAttributesResponseTypeDef = TypedDict(
-    "PutAttributesResponseTypeDef",
-    {
-        "attributes": List[AttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAutoScalingGroupProviderTypeDef = TypedDict(
     "_RequiredAutoScalingGroupProviderTypeDef",
     {
         "autoScalingGroupArn": str,
     },
 )
 _OptionalAutoScalingGroupProviderTypeDef = TypedDict(
@@ -1915,30 +1795,36 @@
     {
         "managedScaling": ManagedScalingTypeDef,
         "managedTerminationProtection": ManagedTerminationProtectionType,
     },
     total=False,
 )
 
-
 class AutoScalingGroupProviderTypeDef(
     _RequiredAutoScalingGroupProviderTypeDef, _OptionalAutoScalingGroupProviderTypeDef
 ):
     pass
 
-
 AutoScalingGroupProviderUpdateTypeDef = TypedDict(
     "AutoScalingGroupProviderUpdateTypeDef",
     {
         "managedScaling": ManagedScalingTypeDef,
         "managedTerminationProtection": ManagedTerminationProtectionType,
     },
     total=False,
 )
 
+NetworkConfigurationOutputTypeDef = TypedDict(
+    "NetworkConfigurationOutputTypeDef",
+    {
+        "awsvpcConfiguration": AwsVpcConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "awsvpcConfiguration": AwsVpcConfigurationTypeDef,
     },
     total=False,
 )
@@ -1948,22 +1834,14 @@
     {
         "cluster": str,
         "capacityProviders": Sequence[str],
         "defaultCapacityProviderStrategy": Sequence[CapacityProviderStrategyItemTypeDef],
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -1972,29 +1850,64 @@
     "UpdateClusterSettingsRequestRequestTypeDef",
     {
         "cluster": str,
         "settings": Sequence[ClusterSettingTypeDef],
     },
 )
 
-ContainerOverrideTypeDef = TypedDict(
-    "ContainerOverrideTypeDef",
+ContainerOverrideOutputTypeDef = TypedDict(
+    "ContainerOverrideOutputTypeDef",
     {
         "name": str,
         "command": List[str],
         "environment": List[KeyValuePairTypeDef],
         "environmentFiles": List[EnvironmentFileTypeDef],
         "cpu": int,
         "memory": int,
         "memoryReservation": int,
         "resourceRequirements": List[ResourceRequirementTypeDef],
     },
     total=False,
 )
 
+ContainerOverrideTypeDef = TypedDict(
+    "ContainerOverrideTypeDef",
+    {
+        "name": str,
+        "command": Sequence[str],
+        "environment": Sequence[KeyValuePairTypeDef],
+        "environmentFiles": Sequence[EnvironmentFileTypeDef],
+        "cpu": int,
+        "memory": int,
+        "memoryReservation": int,
+        "resourceRequirements": Sequence[ResourceRequirementTypeDef],
+    },
+    total=False,
+)
+
+_RequiredLogConfigurationOutputTypeDef = TypedDict(
+    "_RequiredLogConfigurationOutputTypeDef",
+    {
+        "logDriver": LogDriverType,
+    },
+)
+_OptionalLogConfigurationOutputTypeDef = TypedDict(
+    "_OptionalLogConfigurationOutputTypeDef",
+    {
+        "options": Dict[str, str],
+        "secretOptions": List[SecretTypeDef],
+    },
+    total=False,
+)
+
+class LogConfigurationOutputTypeDef(
+    _RequiredLogConfigurationOutputTypeDef, _OptionalLogConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredLogConfigurationTypeDef = TypedDict(
     "_RequiredLogConfigurationTypeDef",
     {
         "logDriver": LogDriverType,
     },
 )
 _OptionalLogConfigurationTypeDef = TypedDict(
@@ -2002,19 +1915,17 @@
     {
         "options": Mapping[str, str],
         "secretOptions": Sequence[SecretTypeDef],
     },
     total=False,
 )
 
-
 class LogConfigurationTypeDef(_RequiredLogConfigurationTypeDef, _OptionalLogConfigurationTypeDef):
     pass
 
-
 ContainerInstanceHealthStatusTypeDef = TypedDict(
     "ContainerInstanceHealthStatusTypeDef",
     {
         "overallStatus": InstanceHealthCheckStateType,
         "details": List[InstanceHealthCheckResultTypeDef],
     },
     total=False,
@@ -2069,57 +1980,198 @@
         "memory": str,
         "memoryReservation": str,
         "gpuIds": List[str],
     },
     total=False,
 )
 
+DeleteAttributesResponseTypeDef = TypedDict(
+    "DeleteAttributesResponseTypeDef",
+    {
+        "attributes": List[AttributeTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DiscoverPollEndpointResponseTypeDef = TypedDict(
+    "DiscoverPollEndpointResponseTypeDef",
+    {
+        "endpoint": str,
+        "telemetryEndpoint": str,
+        "serviceConnectEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAttributesResponseTypeDef = TypedDict(
+    "ListAttributesResponseTypeDef",
+    {
+        "attributes": List[AttributeTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListClustersResponseTypeDef = TypedDict(
+    "ListClustersResponseTypeDef",
+    {
+        "clusterArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListContainerInstancesResponseTypeDef = TypedDict(
+    "ListContainerInstancesResponseTypeDef",
+    {
+        "containerInstanceArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListServicesByNamespaceResponseTypeDef = TypedDict(
+    "ListServicesByNamespaceResponseTypeDef",
+    {
+        "serviceArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListServicesResponseTypeDef = TypedDict(
+    "ListServicesResponseTypeDef",
+    {
+        "serviceArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTaskDefinitionFamiliesResponseTypeDef = TypedDict(
+    "ListTaskDefinitionFamiliesResponseTypeDef",
+    {
+        "families": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTaskDefinitionsResponseTypeDef = TypedDict(
+    "ListTaskDefinitionsResponseTypeDef",
+    {
+        "taskDefinitionArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTasksResponseTypeDef = TypedDict(
+    "ListTasksResponseTypeDef",
+    {
+        "taskArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutAttributesResponseTypeDef = TypedDict(
+    "PutAttributesResponseTypeDef",
+    {
+        "attributes": List[AttributeTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SubmitAttachmentStateChangesResponseTypeDef = TypedDict(
+    "SubmitAttachmentStateChangesResponseTypeDef",
+    {
+        "acknowledgment": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SubmitContainerStateChangeResponseTypeDef = TypedDict(
+    "SubmitContainerStateChangeResponseTypeDef",
+    {
+        "acknowledgment": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SubmitTaskStateChangeResponseTypeDef = TypedDict(
+    "SubmitTaskStateChangeResponseTypeDef",
+    {
+        "acknowledgment": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateTaskSetRequestRequestTypeDef = TypedDict(
     "UpdateTaskSetRequestRequestTypeDef",
     {
         "cluster": str,
         "service": str,
         "taskSet": str,
         "scale": ScaleTypeDef,
     },
 )
 
 DeleteAccountSettingResponseTypeDef = TypedDict(
     "DeleteAccountSettingResponseTypeDef",
     {
         "setting": SettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAccountSettingsResponseTypeDef = TypedDict(
     "ListAccountSettingsResponseTypeDef",
     {
         "settings": List[SettingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAccountSettingDefaultResponseTypeDef = TypedDict(
     "PutAccountSettingDefaultResponseTypeDef",
     {
         "setting": SettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAccountSettingResponseTypeDef = TypedDict(
     "PutAccountSettingResponseTypeDef",
     {
         "setting": SettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DeploymentConfigurationOutputTypeDef = TypedDict(
+    "DeploymentConfigurationOutputTypeDef",
+    {
+        "deploymentCircuitBreaker": DeploymentCircuitBreakerTypeDef,
+        "maximumPercent": int,
+        "minimumHealthyPercent": int,
+        "alarms": DeploymentAlarmsOutputTypeDef,
+    },
+    total=False,
+)
+
 DeploymentConfigurationTypeDef = TypedDict(
     "DeploymentConfigurationTypeDef",
     {
         "deploymentCircuitBreaker": DeploymentCircuitBreakerTypeDef,
         "maximumPercent": int,
         "minimumHealthyPercent": int,
         "alarms": DeploymentAlarmsTypeDef,
@@ -2139,22 +2191,20 @@
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeServicesRequestServicesInactiveWaitTypeDef(
     _RequiredDescribeServicesRequestServicesInactiveWaitTypeDef,
     _OptionalDescribeServicesRequestServicesInactiveWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeServicesRequestServicesStableWaitTypeDef = TypedDict(
     "_RequiredDescribeServicesRequestServicesStableWaitTypeDef",
     {
         "services": Sequence[str],
     },
 )
 _OptionalDescribeServicesRequestServicesStableWaitTypeDef = TypedDict(
@@ -2163,22 +2213,20 @@
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeServicesRequestServicesStableWaitTypeDef(
     _RequiredDescribeServicesRequestServicesStableWaitTypeDef,
     _OptionalDescribeServicesRequestServicesStableWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeTasksRequestTasksRunningWaitTypeDef = TypedDict(
     "_RequiredDescribeTasksRequestTasksRunningWaitTypeDef",
     {
         "tasks": Sequence[str],
     },
 )
 _OptionalDescribeTasksRequestTasksRunningWaitTypeDef = TypedDict(
@@ -2187,22 +2235,20 @@
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeTasksRequestTasksRunningWaitTypeDef(
     _RequiredDescribeTasksRequestTasksRunningWaitTypeDef,
     _OptionalDescribeTasksRequestTasksRunningWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeTasksRequestTasksStoppedWaitTypeDef = TypedDict(
     "_RequiredDescribeTasksRequestTasksStoppedWaitTypeDef",
     {
         "tasks": Sequence[str],
     },
 )
 _OptionalDescribeTasksRequestTasksStoppedWaitTypeDef = TypedDict(
@@ -2211,22 +2257,20 @@
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeTasksRequestTasksStoppedWaitTypeDef(
     _RequiredDescribeTasksRequestTasksStoppedWaitTypeDef,
     _OptionalDescribeTasksRequestTasksStoppedWaitTypeDef,
 ):
     pass
 
-
 _RequiredEFSVolumeConfigurationTypeDef = TypedDict(
     "_RequiredEFSVolumeConfigurationTypeDef",
     {
         "fileSystemId": str,
     },
 )
 _OptionalEFSVolumeConfigurationTypeDef = TypedDict(
@@ -2236,21 +2280,19 @@
         "transitEncryption": EFSTransitEncryptionType,
         "transitEncryptionPort": int,
         "authorizationConfig": EFSAuthorizationConfigTypeDef,
     },
     total=False,
 )
 
-
 class EFSVolumeConfigurationTypeDef(
     _RequiredEFSVolumeConfigurationTypeDef, _OptionalEFSVolumeConfigurationTypeDef
 ):
     pass
 
-
 ExecuteCommandConfigurationTypeDef = TypedDict(
     "ExecuteCommandConfigurationTypeDef",
     {
         "kmsKeyId": str,
         "logging": ExecuteCommandLoggingType,
         "logConfiguration": ExecuteCommandLogConfigurationTypeDef,
     },
@@ -2262,15 +2304,15 @@
     {
         "clusterArn": str,
         "containerArn": str,
         "containerName": str,
         "interactive": bool,
         "session": SessionTypeDef,
         "taskArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FSxWindowsFileServerVolumeConfigurationTypeDef = TypedDict(
     "FSxWindowsFileServerVolumeConfigurationTypeDef",
     {
         "fileSystemId": str,
@@ -2280,57 +2322,198 @@
 )
 
 GetTaskProtectionResponseTypeDef = TypedDict(
     "GetTaskProtectionResponseTypeDef",
     {
         "protectedTasks": List[ProtectedTaskTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTaskProtectionResponseTypeDef = TypedDict(
     "UpdateTaskProtectionResponseTypeDef",
     {
         "protectedTasks": List[ProtectedTaskTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LinuxParametersOutputTypeDef = TypedDict(
+    "LinuxParametersOutputTypeDef",
+    {
+        "capabilities": KernelCapabilitiesOutputTypeDef,
+        "devices": List[DeviceOutputTypeDef],
+        "initProcessEnabled": bool,
+        "sharedMemorySize": int,
+        "tmpfs": List[TmpfsOutputTypeDef],
+        "maxSwap": int,
+        "swappiness": int,
     },
+    total=False,
 )
 
 LinuxParametersTypeDef = TypedDict(
     "LinuxParametersTypeDef",
     {
         "capabilities": KernelCapabilitiesTypeDef,
-        "devices": List[DeviceTypeDef],
+        "devices": Sequence[DeviceTypeDef],
         "initProcessEnabled": bool,
         "sharedMemorySize": int,
-        "tmpfs": List[TmpfsTypeDef],
+        "tmpfs": Sequence[TmpfsTypeDef],
         "maxSwap": int,
         "swappiness": int,
     },
     total=False,
 )
 
-RegisterContainerInstanceRequestRequestTypeDef = TypedDict(
-    "RegisterContainerInstanceRequestRequestTypeDef",
+ListAccountSettingsRequestListAccountSettingsPaginateTypeDef = TypedDict(
+    "ListAccountSettingsRequestListAccountSettingsPaginateTypeDef",
+    {
+        "name": SettingNameType,
+        "value": str,
+        "principalArn": str,
+        "effectiveSettings": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListAttributesRequestListAttributesPaginateTypeDef = TypedDict(
+    "_RequiredListAttributesRequestListAttributesPaginateTypeDef",
+    {
+        "targetType": Literal["container-instance"],
+    },
+)
+_OptionalListAttributesRequestListAttributesPaginateTypeDef = TypedDict(
+    "_OptionalListAttributesRequestListAttributesPaginateTypeDef",
     {
         "cluster": str,
-        "instanceIdentityDocument": str,
-        "instanceIdentityDocumentSignature": str,
-        "totalResources": Sequence[ResourceTypeDef],
-        "versionInfo": VersionInfoTypeDef,
-        "containerInstanceArn": str,
-        "attributes": Sequence[AttributeTypeDef],
-        "platformDevices": Sequence[PlatformDeviceTypeDef],
-        "tags": Sequence[TagTypeDef],
+        "attributeName": str,
+        "attributeValue": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+class ListAttributesRequestListAttributesPaginateTypeDef(
+    _RequiredListAttributesRequestListAttributesPaginateTypeDef,
+    _OptionalListAttributesRequestListAttributesPaginateTypeDef,
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
+ListContainerInstancesRequestListContainerInstancesPaginateTypeDef = TypedDict(
+    "ListContainerInstancesRequestListContainerInstancesPaginateTypeDef",
+    {
+        "cluster": str,
+        "filter": str,
+        "status": ContainerInstanceStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef = TypedDict(
+    "_RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
+    {
+        "namespace": str,
+    },
+)
+_OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef = TypedDict(
+    "_OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef(
+    _RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
+    _OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
+):
+    pass
+
+ListServicesRequestListServicesPaginateTypeDef = TypedDict(
+    "ListServicesRequestListServicesPaginateTypeDef",
+    {
+        "cluster": str,
+        "launchType": LaunchTypeType,
+        "schedulingStrategy": SchedulingStrategyType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef = TypedDict(
+    "ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef",
+    {
+        "familyPrefix": str,
+        "status": TaskDefinitionFamilyStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef = TypedDict(
+    "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
+    {
+        "familyPrefix": str,
+        "status": TaskDefinitionStatusType,
+        "sort": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTasksRequestListTasksPaginateTypeDef = TypedDict(
+    "ListTasksRequestListTasksPaginateTypeDef",
+    {
+        "cluster": str,
+        "containerInstance": str,
+        "family": str,
+        "startedBy": str,
+        "serviceName": str,
+        "desiredStatus": DesiredStatusType,
+        "launchType": LaunchTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ResourceUnionTypeDef = Union[ResourceTypeDef, ResourceOutputTypeDef]
+_RequiredServiceConnectServiceOutputTypeDef = TypedDict(
+    "_RequiredServiceConnectServiceOutputTypeDef",
+    {
+        "portName": str,
+    },
+)
+_OptionalServiceConnectServiceOutputTypeDef = TypedDict(
+    "_OptionalServiceConnectServiceOutputTypeDef",
+    {
+        "discoveryName": str,
+        "clientAliases": List[ServiceConnectClientAliasTypeDef],
+        "ingressPortOverride": int,
+    },
+    total=False,
+)
+
+class ServiceConnectServiceOutputTypeDef(
+    _RequiredServiceConnectServiceOutputTypeDef, _OptionalServiceConnectServiceOutputTypeDef
+):
+    pass
+
 _RequiredServiceConnectServiceTypeDef = TypedDict(
     "_RequiredServiceConnectServiceTypeDef",
     {
         "portName": str,
     },
 )
 _OptionalServiceConnectServiceTypeDef = TypedDict(
@@ -2339,21 +2522,20 @@
         "discoveryName": str,
         "clientAliases": Sequence[ServiceConnectClientAliasTypeDef],
         "ingressPortOverride": int,
     },
     total=False,
 )
 
-
 class ServiceConnectServiceTypeDef(
     _RequiredServiceConnectServiceTypeDef, _OptionalServiceConnectServiceTypeDef
 ):
     pass
 
-
+ProxyConfigurationUnionTypeDef = Union[ProxyConfigurationTypeDef, ProxyConfigurationOutputTypeDef]
 CapacityProviderTypeDef = TypedDict(
     "CapacityProviderTypeDef",
     {
         "capacityProviderArn": str,
         "name": str,
         "status": CapacityProviderStatusType,
         "autoScalingGroupProvider": AutoScalingGroupProviderTypeDef,
@@ -2375,30 +2557,59 @@
     "_OptionalCreateCapacityProviderRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateCapacityProviderRequestRequestTypeDef(
     _RequiredCreateCapacityProviderRequestRequestTypeDef,
     _OptionalCreateCapacityProviderRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateCapacityProviderRequestRequestTypeDef = TypedDict(
     "UpdateCapacityProviderRequestRequestTypeDef",
     {
         "name": str,
         "autoScalingGroupProvider": AutoScalingGroupProviderUpdateTypeDef,
     },
 )
 
+TaskSetTypeDef = TypedDict(
+    "TaskSetTypeDef",
+    {
+        "id": str,
+        "taskSetArn": str,
+        "serviceArn": str,
+        "clusterArn": str,
+        "startedBy": str,
+        "externalId": str,
+        "status": str,
+        "taskDefinition": str,
+        "computedDesiredCount": int,
+        "pendingCount": int,
+        "runningCount": int,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "launchType": LaunchTypeType,
+        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
+        "platformVersion": str,
+        "platformFamily": str,
+        "networkConfiguration": NetworkConfigurationOutputTypeDef,
+        "loadBalancers": List[LoadBalancerTypeDef],
+        "serviceRegistries": List[ServiceRegistryTypeDef],
+        "scale": ScaleTypeDef,
+        "stabilityStatus": StabilityStatusType,
+        "stabilityStatusAt": datetime,
+        "tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
 _RequiredCreateTaskSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTaskSetRequestRequestTypeDef",
     {
         "service": str,
         "cluster": str,
         "taskDefinition": str,
     },
@@ -2416,58 +2627,42 @@
         "scale": ScaleTypeDef,
         "clientToken": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateTaskSetRequestRequestTypeDef(
     _RequiredCreateTaskSetRequestRequestTypeDef, _OptionalCreateTaskSetRequestRequestTypeDef
 ):
     pass
 
-
-TaskSetTypeDef = TypedDict(
-    "TaskSetTypeDef",
+NetworkConfigurationUnionTypeDef = Union[
+    NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
+]
+TaskOverrideOutputTypeDef = TypedDict(
+    "TaskOverrideOutputTypeDef",
     {
-        "id": str,
-        "taskSetArn": str,
-        "serviceArn": str,
-        "clusterArn": str,
-        "startedBy": str,
-        "externalId": str,
-        "status": str,
-        "taskDefinition": str,
-        "computedDesiredCount": int,
-        "pendingCount": int,
-        "runningCount": int,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "launchType": LaunchTypeType,
-        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
-        "platformVersion": str,
-        "platformFamily": str,
-        "networkConfiguration": NetworkConfigurationTypeDef,
-        "loadBalancers": List[LoadBalancerTypeDef],
-        "serviceRegistries": List[ServiceRegistryTypeDef],
-        "scale": ScaleTypeDef,
-        "stabilityStatus": StabilityStatusType,
-        "stabilityStatusAt": datetime,
-        "tags": List[TagTypeDef],
+        "containerOverrides": List[ContainerOverrideOutputTypeDef],
+        "cpu": str,
+        "inferenceAcceleratorOverrides": List[InferenceAcceleratorOverrideTypeDef],
+        "executionRoleArn": str,
+        "memory": str,
+        "taskRoleArn": str,
+        "ephemeralStorage": EphemeralStorageTypeDef,
     },
     total=False,
 )
 
 TaskOverrideTypeDef = TypedDict(
     "TaskOverrideTypeDef",
     {
-        "containerOverrides": List[ContainerOverrideTypeDef],
+        "containerOverrides": Sequence[ContainerOverrideTypeDef],
         "cpu": str,
-        "inferenceAcceleratorOverrides": List[InferenceAcceleratorOverrideTypeDef],
+        "inferenceAcceleratorOverrides": Sequence[InferenceAcceleratorOverrideTypeDef],
         "executionRoleArn": str,
         "memory": str,
         "taskRoleArn": str,
         "ephemeralStorage": EphemeralStorageTypeDef,
     },
     total=False,
 )
@@ -2476,16 +2671,16 @@
     "ContainerInstanceTypeDef",
     {
         "containerInstanceArn": str,
         "ec2InstanceId": str,
         "capacityProviderName": str,
         "version": int,
         "versionInfo": VersionInfoTypeDef,
-        "remainingResources": List[ResourceTypeDef],
-        "registeredResources": List[ResourceTypeDef],
+        "remainingResources": List[ResourceOutputTypeDef],
+        "registeredResources": List[ResourceOutputTypeDef],
         "status": str,
         "statusReason": str,
         "agentConnected": bool,
         "runningTasksCount": int,
         "pendingTasksCount": int,
         "agentUpdateStatus": AgentUpdateStatusType,
         "attributes": List[AttributeTypeDef],
@@ -2503,43 +2698,58 @@
         "cluster": str,
         "task": str,
         "status": str,
         "reason": str,
         "containers": Sequence[ContainerStateChangeTypeDef],
         "attachments": Sequence[AttachmentStateChangeTypeDef],
         "managedAgents": Sequence[ManagedAgentStateChangeTypeDef],
-        "pullStartedAt": Union[datetime, str],
-        "pullStoppedAt": Union[datetime, str],
-        "executionStoppedAt": Union[datetime, str],
+        "pullStartedAt": TimestampTypeDef,
+        "pullStoppedAt": TimestampTypeDef,
+        "executionStoppedAt": TimestampTypeDef,
     },
     total=False,
 )
 
+DeploymentConfigurationUnionTypeDef = Union[
+    DeploymentConfigurationTypeDef, DeploymentConfigurationOutputTypeDef
+]
 ClusterConfigurationTypeDef = TypedDict(
     "ClusterConfigurationTypeDef",
     {
         "executeCommandConfiguration": ExecuteCommandConfigurationTypeDef,
     },
     total=False,
 )
 
+VolumeOutputTypeDef = TypedDict(
+    "VolumeOutputTypeDef",
+    {
+        "name": str,
+        "host": HostVolumePropertiesTypeDef,
+        "dockerVolumeConfiguration": DockerVolumeConfigurationOutputTypeDef,
+        "efsVolumeConfiguration": EFSVolumeConfigurationTypeDef,
+        "fsxWindowsFileServerVolumeConfiguration": FSxWindowsFileServerVolumeConfigurationTypeDef,
+    },
+    total=False,
+)
+
 VolumeTypeDef = TypedDict(
     "VolumeTypeDef",
     {
         "name": str,
         "host": HostVolumePropertiesTypeDef,
         "dockerVolumeConfiguration": DockerVolumeConfigurationTypeDef,
         "efsVolumeConfiguration": EFSVolumeConfigurationTypeDef,
         "fsxWindowsFileServerVolumeConfiguration": FSxWindowsFileServerVolumeConfigurationTypeDef,
     },
     total=False,
 )
 
-ContainerDefinitionTypeDef = TypedDict(
-    "ContainerDefinitionTypeDef",
+ContainerDefinitionOutputTypeDef = TypedDict(
+    "ContainerDefinitionOutputTypeDef",
     {
         "name": str,
         "image": str,
         "repositoryCredentials": RepositoryCredentialsTypeDef,
         "cpu": int,
         "memory": int,
         "memoryReservation": int,
@@ -2548,15 +2758,15 @@
         "essential": bool,
         "entryPoint": List[str],
         "command": List[str],
         "environment": List[KeyValuePairTypeDef],
         "environmentFiles": List[EnvironmentFileTypeDef],
         "mountPoints": List[MountPointTypeDef],
         "volumesFrom": List[VolumeFromTypeDef],
-        "linuxParameters": LinuxParametersTypeDef,
+        "linuxParameters": LinuxParametersOutputTypeDef,
         "secrets": List[SecretTypeDef],
         "dependsOn": List[ContainerDependencyTypeDef],
         "startTimeout": int,
         "stopTimeout": int,
         "hostname": str,
         "user": str,
         "workingDirectory": str,
@@ -2567,23 +2777,107 @@
         "dnsSearchDomains": List[str],
         "extraHosts": List[HostEntryTypeDef],
         "dockerSecurityOptions": List[str],
         "interactive": bool,
         "pseudoTerminal": bool,
         "dockerLabels": Dict[str, str],
         "ulimits": List[UlimitTypeDef],
-        "logConfiguration": LogConfigurationTypeDef,
-        "healthCheck": HealthCheckTypeDef,
+        "logConfiguration": LogConfigurationOutputTypeDef,
+        "healthCheck": HealthCheckOutputTypeDef,
         "systemControls": List[SystemControlTypeDef],
         "resourceRequirements": List[ResourceRequirementTypeDef],
+        "firelensConfiguration": FirelensConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+ContainerDefinitionTypeDef = TypedDict(
+    "ContainerDefinitionTypeDef",
+    {
+        "name": str,
+        "image": str,
+        "repositoryCredentials": RepositoryCredentialsTypeDef,
+        "cpu": int,
+        "memory": int,
+        "memoryReservation": int,
+        "links": Sequence[str],
+        "portMappings": Sequence[PortMappingTypeDef],
+        "essential": bool,
+        "entryPoint": Sequence[str],
+        "command": Sequence[str],
+        "environment": Sequence[KeyValuePairTypeDef],
+        "environmentFiles": Sequence[EnvironmentFileTypeDef],
+        "mountPoints": Sequence[MountPointTypeDef],
+        "volumesFrom": Sequence[VolumeFromTypeDef],
+        "linuxParameters": LinuxParametersTypeDef,
+        "secrets": Sequence[SecretTypeDef],
+        "dependsOn": Sequence[ContainerDependencyTypeDef],
+        "startTimeout": int,
+        "stopTimeout": int,
+        "hostname": str,
+        "user": str,
+        "workingDirectory": str,
+        "disableNetworking": bool,
+        "privileged": bool,
+        "readonlyRootFilesystem": bool,
+        "dnsServers": Sequence[str],
+        "dnsSearchDomains": Sequence[str],
+        "extraHosts": Sequence[HostEntryTypeDef],
+        "dockerSecurityOptions": Sequence[str],
+        "interactive": bool,
+        "pseudoTerminal": bool,
+        "dockerLabels": Mapping[str, str],
+        "ulimits": Sequence[UlimitTypeDef],
+        "logConfiguration": LogConfigurationTypeDef,
+        "healthCheck": HealthCheckTypeDef,
+        "systemControls": Sequence[SystemControlTypeDef],
+        "resourceRequirements": Sequence[ResourceRequirementTypeDef],
         "firelensConfiguration": FirelensConfigurationTypeDef,
     },
     total=False,
 )
 
+RegisterContainerInstanceRequestRequestTypeDef = TypedDict(
+    "RegisterContainerInstanceRequestRequestTypeDef",
+    {
+        "cluster": str,
+        "instanceIdentityDocument": str,
+        "instanceIdentityDocumentSignature": str,
+        "totalResources": Sequence[ResourceUnionTypeDef],
+        "versionInfo": VersionInfoTypeDef,
+        "containerInstanceArn": str,
+        "attributes": Sequence[AttributeTypeDef],
+        "platformDevices": Sequence[PlatformDeviceTypeDef],
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+_RequiredServiceConnectConfigurationOutputTypeDef = TypedDict(
+    "_RequiredServiceConnectConfigurationOutputTypeDef",
+    {
+        "enabled": bool,
+    },
+)
+_OptionalServiceConnectConfigurationOutputTypeDef = TypedDict(
+    "_OptionalServiceConnectConfigurationOutputTypeDef",
+    {
+        "namespace": str,
+        "services": List[ServiceConnectServiceOutputTypeDef],
+        "logConfiguration": LogConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+class ServiceConnectConfigurationOutputTypeDef(
+    _RequiredServiceConnectConfigurationOutputTypeDef,
+    _OptionalServiceConnectConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredServiceConnectConfigurationTypeDef = TypedDict(
     "_RequiredServiceConnectConfigurationTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalServiceConnectConfigurationTypeDef = TypedDict(
@@ -2592,94 +2886,135 @@
         "namespace": str,
         "services": Sequence[ServiceConnectServiceTypeDef],
         "logConfiguration": LogConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class ServiceConnectConfigurationTypeDef(
     _RequiredServiceConnectConfigurationTypeDef, _OptionalServiceConnectConfigurationTypeDef
 ):
     pass
 
-
 CreateCapacityProviderResponseTypeDef = TypedDict(
     "CreateCapacityProviderResponseTypeDef",
     {
         "capacityProvider": CapacityProviderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteCapacityProviderResponseTypeDef = TypedDict(
     "DeleteCapacityProviderResponseTypeDef",
     {
         "capacityProvider": CapacityProviderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCapacityProvidersResponseTypeDef = TypedDict(
     "DescribeCapacityProvidersResponseTypeDef",
     {
         "capacityProviders": List[CapacityProviderTypeDef],
         "failures": List[FailureTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCapacityProviderResponseTypeDef = TypedDict(
     "UpdateCapacityProviderResponseTypeDef",
     {
         "capacityProvider": CapacityProviderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTaskSetResponseTypeDef = TypedDict(
     "CreateTaskSetResponseTypeDef",
     {
         "taskSet": TaskSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteTaskSetResponseTypeDef = TypedDict(
     "DeleteTaskSetResponseTypeDef",
     {
         "taskSet": TaskSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTaskSetsResponseTypeDef = TypedDict(
     "DescribeTaskSetsResponseTypeDef",
     {
         "taskSets": List[TaskSetTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServicePrimaryTaskSetResponseTypeDef = TypedDict(
     "UpdateServicePrimaryTaskSetResponseTypeDef",
     {
         "taskSet": TaskSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTaskSetResponseTypeDef = TypedDict(
     "UpdateTaskSetResponseTypeDef",
     {
         "taskSet": TaskSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TaskTypeDef = TypedDict(
+    "TaskTypeDef",
+    {
+        "attachments": List[AttachmentTypeDef],
+        "attributes": List[AttributeTypeDef],
+        "availabilityZone": str,
+        "capacityProviderName": str,
+        "clusterArn": str,
+        "connectivity": ConnectivityType,
+        "connectivityAt": datetime,
+        "containerInstanceArn": str,
+        "containers": List[ContainerTypeDef],
+        "cpu": str,
+        "createdAt": datetime,
+        "desiredStatus": str,
+        "enableExecuteCommand": bool,
+        "executionStoppedAt": datetime,
+        "group": str,
+        "healthStatus": HealthStatusType,
+        "inferenceAccelerators": List[InferenceAcceleratorTypeDef],
+        "lastStatus": str,
+        "launchType": LaunchTypeType,
+        "memory": str,
+        "overrides": TaskOverrideOutputTypeDef,
+        "platformVersion": str,
+        "platformFamily": str,
+        "pullStartedAt": datetime,
+        "pullStoppedAt": datetime,
+        "startedAt": datetime,
+        "startedBy": str,
+        "stopCode": TaskStopCodeType,
+        "stoppedAt": datetime,
+        "stoppedReason": str,
+        "stoppingAt": datetime,
+        "tags": List[TagTypeDef],
+        "taskArn": str,
+        "taskDefinitionArn": str,
+        "version": int,
+        "ephemeralStorage": EphemeralStorageTypeDef,
     },
+    total=False,
 )
 
 _RequiredRunTaskRequestRequestTypeDef = TypedDict(
     "_RequiredRunTaskRequestRequestTypeDef",
     {
         "taskDefinition": str,
     },
@@ -2703,21 +3038,19 @@
         "referenceId": str,
         "startedBy": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class RunTaskRequestRequestTypeDef(
     _RequiredRunTaskRequestRequestTypeDef, _OptionalRunTaskRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredStartTaskRequestRequestTypeDef = TypedDict(
     "_RequiredStartTaskRequestRequestTypeDef",
     {
         "containerInstances": Sequence[str],
         "taskDefinition": str,
     },
 )
@@ -2734,103 +3067,59 @@
         "referenceId": str,
         "startedBy": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class StartTaskRequestRequestTypeDef(
     _RequiredStartTaskRequestRequestTypeDef, _OptionalStartTaskRequestRequestTypeDef
 ):
     pass
 
-
-TaskTypeDef = TypedDict(
-    "TaskTypeDef",
-    {
-        "attachments": List[AttachmentTypeDef],
-        "attributes": List[AttributeTypeDef],
-        "availabilityZone": str,
-        "capacityProviderName": str,
-        "clusterArn": str,
-        "connectivity": ConnectivityType,
-        "connectivityAt": datetime,
-        "containerInstanceArn": str,
-        "containers": List[ContainerTypeDef],
-        "cpu": str,
-        "createdAt": datetime,
-        "desiredStatus": str,
-        "enableExecuteCommand": bool,
-        "executionStoppedAt": datetime,
-        "group": str,
-        "healthStatus": HealthStatusType,
-        "inferenceAccelerators": List[InferenceAcceleratorTypeDef],
-        "lastStatus": str,
-        "launchType": LaunchTypeType,
-        "memory": str,
-        "overrides": TaskOverrideTypeDef,
-        "platformVersion": str,
-        "platformFamily": str,
-        "pullStartedAt": datetime,
-        "pullStoppedAt": datetime,
-        "startedAt": datetime,
-        "startedBy": str,
-        "stopCode": TaskStopCodeType,
-        "stoppedAt": datetime,
-        "stoppedReason": str,
-        "stoppingAt": datetime,
-        "tags": List[TagTypeDef],
-        "taskArn": str,
-        "taskDefinitionArn": str,
-        "version": int,
-        "ephemeralStorage": EphemeralStorageTypeDef,
-    },
-    total=False,
-)
-
+TaskOverrideUnionTypeDef = Union[TaskOverrideTypeDef, TaskOverrideOutputTypeDef]
 DeregisterContainerInstanceResponseTypeDef = TypedDict(
     "DeregisterContainerInstanceResponseTypeDef",
     {
         "containerInstance": ContainerInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeContainerInstancesResponseTypeDef = TypedDict(
     "DescribeContainerInstancesResponseTypeDef",
     {
         "containerInstances": List[ContainerInstanceTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegisterContainerInstanceResponseTypeDef = TypedDict(
     "RegisterContainerInstanceResponseTypeDef",
     {
         "containerInstance": ContainerInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateContainerAgentResponseTypeDef = TypedDict(
     "UpdateContainerAgentResponseTypeDef",
     {
         "containerInstance": ContainerInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateContainerInstancesStateResponseTypeDef = TypedDict(
     "UpdateContainerInstancesStateResponseTypeDef",
     {
         "containerInstances": List[ContainerInstanceTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterTypeDef = TypedDict(
     "ClusterTypeDef",
     {
         "clusterArn": str,
@@ -2879,89 +3168,79 @@
         "settings": Sequence[ClusterSettingTypeDef],
         "configuration": ClusterConfigurationTypeDef,
         "serviceConnectDefaults": ClusterServiceConnectDefaultsRequestTypeDef,
     },
     total=False,
 )
 
-
 class UpdateClusterRequestRequestTypeDef(
     _RequiredUpdateClusterRequestRequestTypeDef, _OptionalUpdateClusterRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredRegisterTaskDefinitionRequestRequestTypeDef",
-    {
-        "family": str,
-        "containerDefinitions": Sequence[ContainerDefinitionTypeDef],
-    },
-)
-_OptionalRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalRegisterTaskDefinitionRequestRequestTypeDef",
-    {
-        "taskRoleArn": str,
-        "executionRoleArn": str,
-        "networkMode": NetworkModeType,
-        "volumes": Sequence[VolumeTypeDef],
-        "placementConstraints": Sequence[TaskDefinitionPlacementConstraintTypeDef],
-        "requiresCompatibilities": Sequence[CompatibilityType],
-        "cpu": str,
-        "memory": str,
-        "tags": Sequence[TagTypeDef],
-        "pidMode": PidModeType,
-        "ipcMode": IpcModeType,
-        "proxyConfiguration": ProxyConfigurationTypeDef,
-        "inferenceAccelerators": Sequence[InferenceAcceleratorTypeDef],
-        "ephemeralStorage": EphemeralStorageTypeDef,
-        "runtimePlatform": RuntimePlatformTypeDef,
-    },
-    total=False,
-)
-
-
-class RegisterTaskDefinitionRequestRequestTypeDef(
-    _RequiredRegisterTaskDefinitionRequestRequestTypeDef,
-    _OptionalRegisterTaskDefinitionRequestRequestTypeDef,
-):
-    pass
-
-
+VolumeUnionTypeDef = Union[VolumeTypeDef, VolumeOutputTypeDef]
 TaskDefinitionTypeDef = TypedDict(
     "TaskDefinitionTypeDef",
     {
         "taskDefinitionArn": str,
-        "containerDefinitions": List[ContainerDefinitionTypeDef],
+        "containerDefinitions": List[ContainerDefinitionOutputTypeDef],
         "family": str,
         "taskRoleArn": str,
         "executionRoleArn": str,
         "networkMode": NetworkModeType,
         "revision": int,
-        "volumes": List[VolumeTypeDef],
+        "volumes": List[VolumeOutputTypeDef],
         "status": TaskDefinitionStatusType,
         "requiresAttributes": List[AttributeTypeDef],
         "placementConstraints": List[TaskDefinitionPlacementConstraintTypeDef],
         "compatibilities": List[CompatibilityType],
         "runtimePlatform": RuntimePlatformTypeDef,
         "requiresCompatibilities": List[CompatibilityType],
         "cpu": str,
         "memory": str,
         "inferenceAccelerators": List[InferenceAcceleratorTypeDef],
         "pidMode": PidModeType,
         "ipcMode": IpcModeType,
-        "proxyConfiguration": ProxyConfigurationTypeDef,
+        "proxyConfiguration": ProxyConfigurationOutputTypeDef,
         "registeredAt": datetime,
         "deregisteredAt": datetime,
         "registeredBy": str,
         "ephemeralStorage": EphemeralStorageTypeDef,
     },
     total=False,
 )
 
+ContainerDefinitionUnionTypeDef = Union[
+    ContainerDefinitionTypeDef, ContainerDefinitionOutputTypeDef
+]
+DeploymentTypeDef = TypedDict(
+    "DeploymentTypeDef",
+    {
+        "id": str,
+        "status": str,
+        "taskDefinition": str,
+        "desiredCount": int,
+        "pendingCount": int,
+        "runningCount": int,
+        "failedTasks": int,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
+        "launchType": LaunchTypeType,
+        "platformVersion": str,
+        "platformFamily": str,
+        "networkConfiguration": NetworkConfigurationOutputTypeDef,
+        "rolloutState": DeploymentRolloutStateType,
+        "rolloutStateReason": str,
+        "serviceConnectConfiguration": ServiceConnectConfigurationOutputTypeDef,
+        "serviceConnectResources": List[ServiceConnectServiceResourceTypeDef],
+    },
+    total=False,
+)
+
 _RequiredCreateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceRequestRequestTypeDef",
     {
         "serviceName": str,
     },
 )
 _OptionalCreateServiceRequestRequestTypeDef = TypedDict(
@@ -2989,46 +3268,22 @@
         "propagateTags": PropagateTagsType,
         "enableExecuteCommand": bool,
         "serviceConnectConfiguration": ServiceConnectConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateServiceRequestRequestTypeDef(
     _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
 ):
     pass
 
-
-DeploymentTypeDef = TypedDict(
-    "DeploymentTypeDef",
-    {
-        "id": str,
-        "status": str,
-        "taskDefinition": str,
-        "desiredCount": int,
-        "pendingCount": int,
-        "runningCount": int,
-        "failedTasks": int,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
-        "launchType": LaunchTypeType,
-        "platformVersion": str,
-        "platformFamily": str,
-        "networkConfiguration": NetworkConfigurationTypeDef,
-        "rolloutState": DeploymentRolloutStateType,
-        "rolloutStateReason": str,
-        "serviceConnectConfiguration": ServiceConnectConfigurationTypeDef,
-        "serviceConnectResources": List[ServiceConnectServiceResourceTypeDef],
-    },
-    total=False,
-)
-
+ServiceConnectConfigurationUnionTypeDef = Union[
+    ServiceConnectConfigurationTypeDef, ServiceConnectConfigurationOutputTypeDef
+]
 _RequiredUpdateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceRequestRequestTypeDef",
     {
         "service": str,
     },
 )
 _OptionalUpdateServiceRequestRequestTypeDef = TypedDict(
@@ -3051,140 +3306,173 @@
         "propagateTags": PropagateTagsType,
         "serviceRegistries": Sequence[ServiceRegistryTypeDef],
         "serviceConnectConfiguration": ServiceConnectConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateServiceRequestRequestTypeDef(
     _RequiredUpdateServiceRequestRequestTypeDef, _OptionalUpdateServiceRequestRequestTypeDef
 ):
     pass
 
-
 DescribeTasksResponseTypeDef = TypedDict(
     "DescribeTasksResponseTypeDef",
     {
         "tasks": List[TaskTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RunTaskResponseTypeDef = TypedDict(
     "RunTaskResponseTypeDef",
     {
         "tasks": List[TaskTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartTaskResponseTypeDef = TypedDict(
     "StartTaskResponseTypeDef",
     {
         "tasks": List[TaskTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopTaskResponseTypeDef = TypedDict(
     "StopTaskResponseTypeDef",
     {
         "task": TaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterResponseTypeDef = TypedDict(
     "CreateClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteClusterResponseTypeDef = TypedDict(
     "DeleteClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeClustersResponseTypeDef = TypedDict(
     "DescribeClustersResponseTypeDef",
     {
         "clusters": List[ClusterTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutClusterCapacityProvidersResponseTypeDef = TypedDict(
     "PutClusterCapacityProvidersResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateClusterResponseTypeDef = TypedDict(
     "UpdateClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateClusterSettingsResponseTypeDef = TypedDict(
     "UpdateClusterSettingsResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteTaskDefinitionsResponseTypeDef = TypedDict(
     "DeleteTaskDefinitionsResponseTypeDef",
     {
         "taskDefinitions": List[TaskDefinitionTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeregisterTaskDefinitionResponseTypeDef = TypedDict(
     "DeregisterTaskDefinitionResponseTypeDef",
     {
         "taskDefinition": TaskDefinitionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTaskDefinitionResponseTypeDef = TypedDict(
     "DescribeTaskDefinitionResponseTypeDef",
     {
         "taskDefinition": TaskDefinitionTypeDef,
         "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegisterTaskDefinitionResponseTypeDef = TypedDict(
     "RegisterTaskDefinitionResponseTypeDef",
     {
         "taskDefinition": TaskDefinitionTypeDef,
         "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredRegisterTaskDefinitionRequestRequestTypeDef",
+    {
+        "family": str,
+        "containerDefinitions": Sequence[ContainerDefinitionUnionTypeDef],
+    },
+)
+_OptionalRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalRegisterTaskDefinitionRequestRequestTypeDef",
+    {
+        "taskRoleArn": str,
+        "executionRoleArn": str,
+        "networkMode": NetworkModeType,
+        "volumes": Sequence[VolumeUnionTypeDef],
+        "placementConstraints": Sequence[TaskDefinitionPlacementConstraintTypeDef],
+        "requiresCompatibilities": Sequence[CompatibilityType],
+        "cpu": str,
+        "memory": str,
+        "tags": Sequence[TagTypeDef],
+        "pidMode": PidModeType,
+        "ipcMode": IpcModeType,
+        "proxyConfiguration": ProxyConfigurationTypeDef,
+        "inferenceAccelerators": Sequence[InferenceAcceleratorTypeDef],
+        "ephemeralStorage": EphemeralStorageTypeDef,
+        "runtimePlatform": RuntimePlatformTypeDef,
     },
+    total=False,
 )
 
+class RegisterTaskDefinitionRequestRequestTypeDef(
+    _RequiredRegisterTaskDefinitionRequestRequestTypeDef,
+    _OptionalRegisterTaskDefinitionRequestRequestTypeDef,
+):
+    pass
+
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "serviceArn": str,
         "serviceName": str,
         "clusterArn": str,
         "loadBalancers": List[LoadBalancerTypeDef],
@@ -3194,23 +3482,23 @@
         "runningCount": int,
         "pendingCount": int,
         "launchType": LaunchTypeType,
         "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
         "platformVersion": str,
         "platformFamily": str,
         "taskDefinition": str,
-        "deploymentConfiguration": DeploymentConfigurationTypeDef,
+        "deploymentConfiguration": DeploymentConfigurationOutputTypeDef,
         "taskSets": List[TaskSetTypeDef],
         "deployments": List[DeploymentTypeDef],
         "roleArn": str,
         "events": List[ServiceEventTypeDef],
         "createdAt": datetime,
         "placementConstraints": List[PlacementConstraintTypeDef],
         "placementStrategy": List[PlacementStrategyTypeDef],
-        "networkConfiguration": NetworkConfigurationTypeDef,
+        "networkConfiguration": NetworkConfigurationOutputTypeDef,
         "healthCheckGracePeriodSeconds": int,
         "schedulingStrategy": SchedulingStrategyType,
         "deploymentController": DeploymentControllerTypeDef,
         "tags": List[TagTypeDef],
         "createdBy": str,
         "enableECSManagedTags": bool,
         "propagateTags": PropagateTagsType,
@@ -3219,35 +3507,35 @@
     total=False,
 )
 
 CreateServiceResponseTypeDef = TypedDict(
     "CreateServiceResponseTypeDef",
     {
         "service": ServiceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteServiceResponseTypeDef = TypedDict(
     "DeleteServiceResponseTypeDef",
     {
         "service": ServiceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeServicesResponseTypeDef = TypedDict(
     "DescribeServicesResponseTypeDef",
     {
         "services": List[ServiceTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServiceResponseTypeDef = TypedDict(
     "UpdateServiceResponseTypeDef",
     {
         "service": ServiceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs/type_defs.pyi` & `types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_ecs.type_defs import AttachmentStateChangeTypeDef
 
-    data: AttachmentStateChangeTypeDef = {...}
+    data: AttachmentStateChangeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -67,209 +67,238 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AttachmentStateChangeTypeDef",
     "KeyValuePairTypeDef",
     "AttributeTypeDef",
     "ManagedScalingTypeDef",
+    "AwsVpcConfigurationOutputTypeDef",
     "AwsVpcConfigurationTypeDef",
     "CapacityProviderStrategyItemTypeDef",
     "TagTypeDef",
     "ClusterServiceConnectDefaultsRequestTypeDef",
     "ClusterServiceConnectDefaultsTypeDef",
     "ClusterSettingTypeDef",
     "ContainerDependencyTypeDef",
     "EnvironmentFileTypeDef",
-    "FirelensConfigurationTypeDef",
-    "HealthCheckTypeDef",
+    "FirelensConfigurationOutputTypeDef",
+    "HealthCheckOutputTypeDef",
     "HostEntryTypeDef",
     "MountPointTypeDef",
     "PortMappingTypeDef",
     "RepositoryCredentialsTypeDef",
     "ResourceRequirementTypeDef",
     "SecretTypeDef",
     "SystemControlTypeDef",
     "UlimitTypeDef",
     "VolumeFromTypeDef",
+    "FirelensConfigurationTypeDef",
+    "HealthCheckTypeDef",
     "InstanceHealthCheckResultTypeDef",
-    "ResourceTypeDef",
+    "ResourceOutputTypeDef",
     "VersionInfoTypeDef",
     "NetworkBindingTypeDef",
     "ManagedAgentTypeDef",
     "NetworkInterfaceTypeDef",
+    "ResponseMetadataTypeDef",
     "DeploymentControllerTypeDef",
     "LoadBalancerTypeDef",
     "PlacementConstraintTypeDef",
     "PlacementStrategyTypeDef",
     "ServiceRegistryTypeDef",
     "ScaleTypeDef",
     "DeleteAccountSettingRequestRequestTypeDef",
     "SettingTypeDef",
     "DeleteCapacityProviderRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteServiceRequestRequestTypeDef",
     "DeleteTaskDefinitionsRequestRequestTypeDef",
     "FailureTypeDef",
     "DeleteTaskSetRequestRequestTypeDef",
+    "DeploymentAlarmsOutputTypeDef",
     "DeploymentAlarmsTypeDef",
     "DeploymentCircuitBreakerTypeDef",
     "ServiceConnectServiceResourceTypeDef",
     "DeregisterContainerInstanceRequestRequestTypeDef",
     "DeregisterTaskDefinitionRequestRequestTypeDef",
     "DescribeCapacityProvidersRequestRequestTypeDef",
     "DescribeClustersRequestRequestTypeDef",
     "DescribeContainerInstancesRequestRequestTypeDef",
     "DescribeServicesRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeTaskDefinitionRequestRequestTypeDef",
     "DescribeTaskSetsRequestRequestTypeDef",
     "DescribeTasksRequestRequestTypeDef",
+    "DeviceOutputTypeDef",
     "DeviceTypeDef",
     "DiscoverPollEndpointRequestRequestTypeDef",
-    "DiscoverPollEndpointResponseTypeDef",
+    "DockerVolumeConfigurationOutputTypeDef",
     "DockerVolumeConfigurationTypeDef",
     "EFSAuthorizationConfigTypeDef",
     "EphemeralStorageTypeDef",
     "ExecuteCommandLogConfigurationTypeDef",
     "ExecuteCommandRequestRequestTypeDef",
     "SessionTypeDef",
     "FSxWindowsFileServerAuthorizationConfigTypeDef",
     "GetTaskProtectionRequestRequestTypeDef",
     "ProtectedTaskTypeDef",
     "HostVolumePropertiesTypeDef",
     "InferenceAcceleratorOverrideTypeDef",
     "InferenceAcceleratorTypeDef",
+    "KernelCapabilitiesOutputTypeDef",
     "KernelCapabilitiesTypeDef",
+    "TmpfsOutputTypeDef",
     "TmpfsTypeDef",
-    "ListAccountSettingsRequestListAccountSettingsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccountSettingsRequestRequestTypeDef",
-    "ListAttributesRequestListAttributesPaginateTypeDef",
     "ListAttributesRequestRequestTypeDef",
-    "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
-    "ListClustersResponseTypeDef",
-    "ListContainerInstancesRequestListContainerInstancesPaginateTypeDef",
     "ListContainerInstancesRequestRequestTypeDef",
-    "ListContainerInstancesResponseTypeDef",
-    "ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
     "ListServicesByNamespaceRequestRequestTypeDef",
-    "ListServicesByNamespaceResponseTypeDef",
-    "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
-    "ListServicesResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef",
     "ListTaskDefinitionFamiliesRequestRequestTypeDef",
-    "ListTaskDefinitionFamiliesResponseTypeDef",
-    "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
     "ListTaskDefinitionsRequestRequestTypeDef",
-    "ListTaskDefinitionsResponseTypeDef",
-    "ListTasksRequestListTasksPaginateTypeDef",
     "ListTasksRequestRequestTypeDef",
-    "ListTasksResponseTypeDef",
     "ManagedAgentStateChangeTypeDef",
-    "PaginatorConfigTypeDef",
     "PlatformDeviceTypeDef",
     "PutAccountSettingDefaultRequestRequestTypeDef",
     "PutAccountSettingRequestRequestTypeDef",
     "RuntimePlatformTypeDef",
     "TaskDefinitionPlacementConstraintTypeDef",
-    "ResponseMetadataTypeDef",
+    "ResourceTypeDef",
     "ServiceConnectClientAliasTypeDef",
     "ServiceEventTypeDef",
     "StopTaskRequestRequestTypeDef",
-    "SubmitAttachmentStateChangesResponseTypeDef",
-    "SubmitContainerStateChangeResponseTypeDef",
-    "SubmitTaskStateChangeResponseTypeDef",
+    "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateContainerAgentRequestRequestTypeDef",
     "UpdateContainerInstancesStateRequestRequestTypeDef",
     "UpdateServicePrimaryTaskSetRequestRequestTypeDef",
     "UpdateTaskProtectionRequestRequestTypeDef",
     "SubmitAttachmentStateChangesRequestRequestTypeDef",
     "AttachmentTypeDef",
+    "ProxyConfigurationOutputTypeDef",
     "ProxyConfigurationTypeDef",
     "DeleteAttributesRequestRequestTypeDef",
-    "DeleteAttributesResponseTypeDef",
-    "ListAttributesResponseTypeDef",
     "PutAttributesRequestRequestTypeDef",
-    "PutAttributesResponseTypeDef",
     "AutoScalingGroupProviderTypeDef",
     "AutoScalingGroupProviderUpdateTypeDef",
+    "NetworkConfigurationOutputTypeDef",
     "NetworkConfigurationTypeDef",
     "PutClusterCapacityProvidersRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UpdateClusterSettingsRequestRequestTypeDef",
+    "ContainerOverrideOutputTypeDef",
     "ContainerOverrideTypeDef",
+    "LogConfigurationOutputTypeDef",
     "LogConfigurationTypeDef",
     "ContainerInstanceHealthStatusTypeDef",
     "ContainerStateChangeTypeDef",
     "SubmitContainerStateChangeRequestRequestTypeDef",
     "ContainerTypeDef",
+    "DeleteAttributesResponseTypeDef",
+    "DiscoverPollEndpointResponseTypeDef",
+    "ListAttributesResponseTypeDef",
+    "ListClustersResponseTypeDef",
+    "ListContainerInstancesResponseTypeDef",
+    "ListServicesByNamespaceResponseTypeDef",
+    "ListServicesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListTaskDefinitionFamiliesResponseTypeDef",
+    "ListTaskDefinitionsResponseTypeDef",
+    "ListTasksResponseTypeDef",
+    "PutAttributesResponseTypeDef",
+    "SubmitAttachmentStateChangesResponseTypeDef",
+    "SubmitContainerStateChangeResponseTypeDef",
+    "SubmitTaskStateChangeResponseTypeDef",
     "UpdateTaskSetRequestRequestTypeDef",
     "DeleteAccountSettingResponseTypeDef",
     "ListAccountSettingsResponseTypeDef",
     "PutAccountSettingDefaultResponseTypeDef",
     "PutAccountSettingResponseTypeDef",
+    "DeploymentConfigurationOutputTypeDef",
     "DeploymentConfigurationTypeDef",
     "DescribeServicesRequestServicesInactiveWaitTypeDef",
     "DescribeServicesRequestServicesStableWaitTypeDef",
     "DescribeTasksRequestTasksRunningWaitTypeDef",
     "DescribeTasksRequestTasksStoppedWaitTypeDef",
     "EFSVolumeConfigurationTypeDef",
     "ExecuteCommandConfigurationTypeDef",
     "ExecuteCommandResponseTypeDef",
     "FSxWindowsFileServerVolumeConfigurationTypeDef",
     "GetTaskProtectionResponseTypeDef",
     "UpdateTaskProtectionResponseTypeDef",
+    "LinuxParametersOutputTypeDef",
     "LinuxParametersTypeDef",
-    "RegisterContainerInstanceRequestRequestTypeDef",
+    "ListAccountSettingsRequestListAccountSettingsPaginateTypeDef",
+    "ListAttributesRequestListAttributesPaginateTypeDef",
+    "ListClustersRequestListClustersPaginateTypeDef",
+    "ListContainerInstancesRequestListContainerInstancesPaginateTypeDef",
+    "ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
+    "ListServicesRequestListServicesPaginateTypeDef",
+    "ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef",
+    "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
+    "ListTasksRequestListTasksPaginateTypeDef",
+    "ResourceUnionTypeDef",
+    "ServiceConnectServiceOutputTypeDef",
     "ServiceConnectServiceTypeDef",
+    "ProxyConfigurationUnionTypeDef",
     "CapacityProviderTypeDef",
     "CreateCapacityProviderRequestRequestTypeDef",
     "UpdateCapacityProviderRequestRequestTypeDef",
-    "CreateTaskSetRequestRequestTypeDef",
     "TaskSetTypeDef",
+    "CreateTaskSetRequestRequestTypeDef",
+    "NetworkConfigurationUnionTypeDef",
+    "TaskOverrideOutputTypeDef",
     "TaskOverrideTypeDef",
     "ContainerInstanceTypeDef",
     "SubmitTaskStateChangeRequestRequestTypeDef",
+    "DeploymentConfigurationUnionTypeDef",
     "ClusterConfigurationTypeDef",
+    "VolumeOutputTypeDef",
     "VolumeTypeDef",
+    "ContainerDefinitionOutputTypeDef",
     "ContainerDefinitionTypeDef",
+    "RegisterContainerInstanceRequestRequestTypeDef",
+    "ServiceConnectConfigurationOutputTypeDef",
     "ServiceConnectConfigurationTypeDef",
     "CreateCapacityProviderResponseTypeDef",
     "DeleteCapacityProviderResponseTypeDef",
     "DescribeCapacityProvidersResponseTypeDef",
     "UpdateCapacityProviderResponseTypeDef",
     "CreateTaskSetResponseTypeDef",
     "DeleteTaskSetResponseTypeDef",
     "DescribeTaskSetsResponseTypeDef",
     "UpdateServicePrimaryTaskSetResponseTypeDef",
     "UpdateTaskSetResponseTypeDef",
+    "TaskTypeDef",
     "RunTaskRequestRequestTypeDef",
     "StartTaskRequestRequestTypeDef",
-    "TaskTypeDef",
+    "TaskOverrideUnionTypeDef",
     "DeregisterContainerInstanceResponseTypeDef",
     "DescribeContainerInstancesResponseTypeDef",
     "RegisterContainerInstanceResponseTypeDef",
     "UpdateContainerAgentResponseTypeDef",
     "UpdateContainerInstancesStateResponseTypeDef",
     "ClusterTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "UpdateClusterRequestRequestTypeDef",
-    "RegisterTaskDefinitionRequestRequestTypeDef",
+    "VolumeUnionTypeDef",
     "TaskDefinitionTypeDef",
-    "CreateServiceRequestRequestTypeDef",
+    "ContainerDefinitionUnionTypeDef",
     "DeploymentTypeDef",
+    "CreateServiceRequestRequestTypeDef",
+    "ServiceConnectConfigurationUnionTypeDef",
     "UpdateServiceRequestRequestTypeDef",
     "DescribeTasksResponseTypeDef",
     "RunTaskResponseTypeDef",
     "StartTaskResponseTypeDef",
     "StopTaskResponseTypeDef",
     "CreateClusterResponseTypeDef",
     "DeleteClusterResponseTypeDef",
@@ -277,14 +306,15 @@
     "PutClusterCapacityProvidersResponseTypeDef",
     "UpdateClusterResponseTypeDef",
     "UpdateClusterSettingsResponseTypeDef",
     "DeleteTaskDefinitionsResponseTypeDef",
     "DeregisterTaskDefinitionResponseTypeDef",
     "DescribeTaskDefinitionResponseTypeDef",
     "RegisterTaskDefinitionResponseTypeDef",
+    "RegisterTaskDefinitionRequestRequestTypeDef",
     "ServiceTypeDef",
     "CreateServiceResponseTypeDef",
     "DeleteServiceResponseTypeDef",
     "DescribeServicesResponseTypeDef",
     "UpdateServiceResponseTypeDef",
 )
 
@@ -317,29 +347,53 @@
         "value": str,
         "targetType": Literal["container-instance"],
         "targetId": str,
     },
     total=False,
 )
 
+
 class AttributeTypeDef(_RequiredAttributeTypeDef, _OptionalAttributeTypeDef):
     pass
 
+
 ManagedScalingTypeDef = TypedDict(
     "ManagedScalingTypeDef",
     {
         "status": ManagedScalingStatusType,
         "targetCapacity": int,
         "minimumScalingStepSize": int,
         "maximumScalingStepSize": int,
         "instanceWarmupPeriod": int,
     },
     total=False,
 )
 
+_RequiredAwsVpcConfigurationOutputTypeDef = TypedDict(
+    "_RequiredAwsVpcConfigurationOutputTypeDef",
+    {
+        "subnets": List[str],
+    },
+)
+_OptionalAwsVpcConfigurationOutputTypeDef = TypedDict(
+    "_OptionalAwsVpcConfigurationOutputTypeDef",
+    {
+        "securityGroups": List[str],
+        "assignPublicIp": AssignPublicIpType,
+    },
+    total=False,
+)
+
+
+class AwsVpcConfigurationOutputTypeDef(
+    _RequiredAwsVpcConfigurationOutputTypeDef, _OptionalAwsVpcConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredAwsVpcConfigurationTypeDef = TypedDict(
     "_RequiredAwsVpcConfigurationTypeDef",
     {
         "subnets": Sequence[str],
     },
 )
 _OptionalAwsVpcConfigurationTypeDef = TypedDict(
@@ -347,19 +401,21 @@
     {
         "securityGroups": Sequence[str],
         "assignPublicIp": AssignPublicIpType,
     },
     total=False,
 )
 
+
 class AwsVpcConfigurationTypeDef(
     _RequiredAwsVpcConfigurationTypeDef, _OptionalAwsVpcConfigurationTypeDef
 ):
     pass
 
+
 _RequiredCapacityProviderStrategyItemTypeDef = TypedDict(
     "_RequiredCapacityProviderStrategyItemTypeDef",
     {
         "capacityProvider": str,
     },
 )
 _OptionalCapacityProviderStrategyItemTypeDef = TypedDict(
@@ -367,19 +423,21 @@
     {
         "weight": int,
         "base": int,
     },
     total=False,
 )
 
+
 class CapacityProviderStrategyItemTypeDef(
     _RequiredCapacityProviderStrategyItemTypeDef, _OptionalCapacityProviderStrategyItemTypeDef
 ):
     pass
 
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
@@ -421,53 +479,59 @@
     "EnvironmentFileTypeDef",
     {
         "value": str,
         "type": Literal["s3"],
     },
 )
 
-_RequiredFirelensConfigurationTypeDef = TypedDict(
-    "_RequiredFirelensConfigurationTypeDef",
+_RequiredFirelensConfigurationOutputTypeDef = TypedDict(
+    "_RequiredFirelensConfigurationOutputTypeDef",
     {
         "type": FirelensConfigurationTypeType,
     },
 )
-_OptionalFirelensConfigurationTypeDef = TypedDict(
-    "_OptionalFirelensConfigurationTypeDef",
+_OptionalFirelensConfigurationOutputTypeDef = TypedDict(
+    "_OptionalFirelensConfigurationOutputTypeDef",
     {
         "options": Dict[str, str],
     },
     total=False,
 )
 
-class FirelensConfigurationTypeDef(
-    _RequiredFirelensConfigurationTypeDef, _OptionalFirelensConfigurationTypeDef
+
+class FirelensConfigurationOutputTypeDef(
+    _RequiredFirelensConfigurationOutputTypeDef, _OptionalFirelensConfigurationOutputTypeDef
 ):
     pass
 
-_RequiredHealthCheckTypeDef = TypedDict(
-    "_RequiredHealthCheckTypeDef",
+
+_RequiredHealthCheckOutputTypeDef = TypedDict(
+    "_RequiredHealthCheckOutputTypeDef",
     {
         "command": List[str],
     },
 )
-_OptionalHealthCheckTypeDef = TypedDict(
-    "_OptionalHealthCheckTypeDef",
+_OptionalHealthCheckOutputTypeDef = TypedDict(
+    "_OptionalHealthCheckOutputTypeDef",
     {
         "interval": int,
         "timeout": int,
         "retries": int,
         "startPeriod": int,
     },
     total=False,
 )
 
-class HealthCheckTypeDef(_RequiredHealthCheckTypeDef, _OptionalHealthCheckTypeDef):
+
+class HealthCheckOutputTypeDef(
+    _RequiredHealthCheckOutputTypeDef, _OptionalHealthCheckOutputTypeDef
+):
     pass
 
+
 HostEntryTypeDef = TypedDict(
     "HostEntryTypeDef",
     {
         "hostname": str,
         "ipAddress": str,
     },
 )
@@ -541,27 +605,70 @@
     {
         "sourceContainer": str,
         "readOnly": bool,
     },
     total=False,
 )
 
+_RequiredFirelensConfigurationTypeDef = TypedDict(
+    "_RequiredFirelensConfigurationTypeDef",
+    {
+        "type": FirelensConfigurationTypeType,
+    },
+)
+_OptionalFirelensConfigurationTypeDef = TypedDict(
+    "_OptionalFirelensConfigurationTypeDef",
+    {
+        "options": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class FirelensConfigurationTypeDef(
+    _RequiredFirelensConfigurationTypeDef, _OptionalFirelensConfigurationTypeDef
+):
+    pass
+
+
+_RequiredHealthCheckTypeDef = TypedDict(
+    "_RequiredHealthCheckTypeDef",
+    {
+        "command": Sequence[str],
+    },
+)
+_OptionalHealthCheckTypeDef = TypedDict(
+    "_OptionalHealthCheckTypeDef",
+    {
+        "interval": int,
+        "timeout": int,
+        "retries": int,
+        "startPeriod": int,
+    },
+    total=False,
+)
+
+
+class HealthCheckTypeDef(_RequiredHealthCheckTypeDef, _OptionalHealthCheckTypeDef):
+    pass
+
+
 InstanceHealthCheckResultTypeDef = TypedDict(
     "InstanceHealthCheckResultTypeDef",
     {
         "type": Literal["CONTAINER_RUNTIME"],
         "status": InstanceHealthCheckStateType,
         "lastUpdated": datetime,
         "lastStatusChange": datetime,
     },
     total=False,
 )
 
-ResourceTypeDef = TypedDict(
-    "ResourceTypeDef",
+ResourceOutputTypeDef = TypedDict(
+    "ResourceOutputTypeDef",
     {
         "name": str,
         "type": str,
         "doubleValue": float,
         "longValue": int,
         "integerValue": int,
         "stringSetValue": List[str],
@@ -609,14 +716,25 @@
         "attachmentId": str,
         "privateIpv4Address": str,
         "ipv6Address": str,
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
 DeploymentControllerTypeDef = TypedDict(
     "DeploymentControllerTypeDef",
     {
         "type": DeploymentControllerTypeType,
     },
 )
 
@@ -679,20 +797,22 @@
     "_OptionalDeleteAccountSettingRequestRequestTypeDef",
     {
         "principalArn": str,
     },
     total=False,
 )
 
+
 class DeleteAccountSettingRequestRequestTypeDef(
     _RequiredDeleteAccountSettingRequestRequestTypeDef,
     _OptionalDeleteAccountSettingRequestRequestTypeDef,
 ):
     pass
 
+
 SettingTypeDef = TypedDict(
     "SettingTypeDef",
     {
         "name": SettingNameType,
         "value": str,
         "principalArn": str,
     },
@@ -724,19 +844,21 @@
     {
         "cluster": str,
         "force": bool,
     },
     total=False,
 )
 
+
 class DeleteServiceRequestRequestTypeDef(
     _RequiredDeleteServiceRequestRequestTypeDef, _OptionalDeleteServiceRequestRequestTypeDef
 ):
     pass
 
+
 DeleteTaskDefinitionsRequestRequestTypeDef = TypedDict(
     "DeleteTaskDefinitionsRequestRequestTypeDef",
     {
         "taskDefinitions": Sequence[str],
     },
 )
 
@@ -762,19 +884,30 @@
     "_OptionalDeleteTaskSetRequestRequestTypeDef",
     {
         "force": bool,
     },
     total=False,
 )
 
+
 class DeleteTaskSetRequestRequestTypeDef(
     _RequiredDeleteTaskSetRequestRequestTypeDef, _OptionalDeleteTaskSetRequestRequestTypeDef
 ):
     pass
 
+
+DeploymentAlarmsOutputTypeDef = TypedDict(
+    "DeploymentAlarmsOutputTypeDef",
+    {
+        "alarmNames": List[str],
+        "enable": bool,
+        "rollback": bool,
+    },
+)
+
 DeploymentAlarmsTypeDef = TypedDict(
     "DeploymentAlarmsTypeDef",
     {
         "alarmNames": Sequence[str],
         "enable": bool,
         "rollback": bool,
     },
@@ -808,20 +941,22 @@
     {
         "cluster": str,
         "force": bool,
     },
     total=False,
 )
 
+
 class DeregisterContainerInstanceRequestRequestTypeDef(
     _RequiredDeregisterContainerInstanceRequestRequestTypeDef,
     _OptionalDeregisterContainerInstanceRequestRequestTypeDef,
 ):
     pass
 
+
 DeregisterTaskDefinitionRequestRequestTypeDef = TypedDict(
     "DeregisterTaskDefinitionRequestRequestTypeDef",
     {
         "taskDefinition": str,
     },
 )
 
@@ -856,20 +991,22 @@
     {
         "cluster": str,
         "include": Sequence[ContainerInstanceFieldType],
     },
     total=False,
 )
 
+
 class DescribeContainerInstancesRequestRequestTypeDef(
     _RequiredDescribeContainerInstancesRequestRequestTypeDef,
     _OptionalDescribeContainerInstancesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeServicesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeServicesRequestRequestTypeDef",
     {
         "services": Sequence[str],
     },
 )
 _OptionalDescribeServicesRequestRequestTypeDef = TypedDict(
@@ -877,19 +1014,21 @@
     {
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
     },
     total=False,
 )
 
+
 class DescribeServicesRequestRequestTypeDef(
     _RequiredDescribeServicesRequestRequestTypeDef, _OptionalDescribeServicesRequestRequestTypeDef
 ):
     pass
 
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -905,20 +1044,22 @@
     "_OptionalDescribeTaskDefinitionRequestRequestTypeDef",
     {
         "include": Sequence[Literal["TAGS"]],
     },
     total=False,
 )
 
+
 class DescribeTaskDefinitionRequestRequestTypeDef(
     _RequiredDescribeTaskDefinitionRequestRequestTypeDef,
     _OptionalDescribeTaskDefinitionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeTaskSetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTaskSetsRequestRequestTypeDef",
     {
         "cluster": str,
         "service": str,
     },
 )
@@ -927,19 +1068,21 @@
     {
         "taskSets": Sequence[str],
         "include": Sequence[Literal["TAGS"]],
     },
     total=False,
 )
 
+
 class DescribeTaskSetsRequestRequestTypeDef(
     _RequiredDescribeTaskSetsRequestRequestTypeDef, _OptionalDescribeTaskSetsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDescribeTasksRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTasksRequestRequestTypeDef",
     {
         "tasks": Sequence[str],
     },
 )
 _OptionalDescribeTasksRequestRequestTypeDef = TypedDict(
@@ -947,64 +1090,90 @@
     {
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
     },
     total=False,
 )
 
+
 class DescribeTasksRequestRequestTypeDef(
     _RequiredDescribeTasksRequestRequestTypeDef, _OptionalDescribeTasksRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredDeviceOutputTypeDef = TypedDict(
+    "_RequiredDeviceOutputTypeDef",
+    {
+        "hostPath": str,
+    },
+)
+_OptionalDeviceOutputTypeDef = TypedDict(
+    "_OptionalDeviceOutputTypeDef",
+    {
+        "containerPath": str,
+        "permissions": List[DeviceCgroupPermissionType],
+    },
+    total=False,
+)
+
+
+class DeviceOutputTypeDef(_RequiredDeviceOutputTypeDef, _OptionalDeviceOutputTypeDef):
+    pass
+
+
 _RequiredDeviceTypeDef = TypedDict(
     "_RequiredDeviceTypeDef",
     {
         "hostPath": str,
     },
 )
 _OptionalDeviceTypeDef = TypedDict(
     "_OptionalDeviceTypeDef",
     {
         "containerPath": str,
-        "permissions": List[DeviceCgroupPermissionType],
+        "permissions": Sequence[DeviceCgroupPermissionType],
     },
     total=False,
 )
 
+
 class DeviceTypeDef(_RequiredDeviceTypeDef, _OptionalDeviceTypeDef):
     pass
 
+
 DiscoverPollEndpointRequestRequestTypeDef = TypedDict(
     "DiscoverPollEndpointRequestRequestTypeDef",
     {
         "containerInstance": str,
         "cluster": str,
     },
     total=False,
 )
 
-DiscoverPollEndpointResponseTypeDef = TypedDict(
-    "DiscoverPollEndpointResponseTypeDef",
+DockerVolumeConfigurationOutputTypeDef = TypedDict(
+    "DockerVolumeConfigurationOutputTypeDef",
     {
-        "endpoint": str,
-        "telemetryEndpoint": str,
-        "serviceConnectEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "scope": ScopeType,
+        "autoprovision": bool,
+        "driver": str,
+        "driverOpts": Dict[str, str],
+        "labels": Dict[str, str],
     },
+    total=False,
 )
 
 DockerVolumeConfigurationTypeDef = TypedDict(
     "DockerVolumeConfigurationTypeDef",
     {
         "scope": ScopeType,
         "autoprovision": bool,
         "driver": str,
-        "driverOpts": Dict[str, str],
-        "labels": Dict[str, str],
+        "driverOpts": Mapping[str, str],
+        "labels": Mapping[str, str],
     },
     total=False,
 )
 
 EFSAuthorizationConfigTypeDef = TypedDict(
     "EFSAuthorizationConfigTypeDef",
     {
@@ -1046,19 +1215,21 @@
     {
         "cluster": str,
         "container": str,
     },
     total=False,
 )
 
+
 class ExecuteCommandRequestRequestTypeDef(
     _RequiredExecuteCommandRequestRequestTypeDef, _OptionalExecuteCommandRequestRequestTypeDef
 ):
     pass
 
+
 SessionTypeDef = TypedDict(
     "SessionTypeDef",
     {
         "sessionId": str,
         "streamUrl": str,
         "tokenValue": str,
     },
@@ -1083,19 +1254,21 @@
     "_OptionalGetTaskProtectionRequestRequestTypeDef",
     {
         "tasks": Sequence[str],
     },
     total=False,
 )
 
+
 class GetTaskProtectionRequestRequestTypeDef(
     _RequiredGetTaskProtectionRequestRequestTypeDef, _OptionalGetTaskProtectionRequestRequestTypeDef
 ):
     pass
 
+
 ProtectedTaskTypeDef = TypedDict(
     "ProtectedTaskTypeDef",
     {
         "taskArn": str,
         "protectionEnabled": bool,
         "expirationDate": datetime,
     },
@@ -1123,49 +1296,78 @@
     "InferenceAcceleratorTypeDef",
     {
         "deviceName": str,
         "deviceType": str,
     },
 )
 
-KernelCapabilitiesTypeDef = TypedDict(
-    "KernelCapabilitiesTypeDef",
+KernelCapabilitiesOutputTypeDef = TypedDict(
+    "KernelCapabilitiesOutputTypeDef",
     {
         "add": List[str],
         "drop": List[str],
     },
     total=False,
 )
 
+KernelCapabilitiesTypeDef = TypedDict(
+    "KernelCapabilitiesTypeDef",
+    {
+        "add": Sequence[str],
+        "drop": Sequence[str],
+    },
+    total=False,
+)
+
+_RequiredTmpfsOutputTypeDef = TypedDict(
+    "_RequiredTmpfsOutputTypeDef",
+    {
+        "containerPath": str,
+        "size": int,
+    },
+)
+_OptionalTmpfsOutputTypeDef = TypedDict(
+    "_OptionalTmpfsOutputTypeDef",
+    {
+        "mountOptions": List[str],
+    },
+    total=False,
+)
+
+
+class TmpfsOutputTypeDef(_RequiredTmpfsOutputTypeDef, _OptionalTmpfsOutputTypeDef):
+    pass
+
+
 _RequiredTmpfsTypeDef = TypedDict(
     "_RequiredTmpfsTypeDef",
     {
         "containerPath": str,
         "size": int,
     },
 )
 _OptionalTmpfsTypeDef = TypedDict(
     "_OptionalTmpfsTypeDef",
     {
-        "mountOptions": List[str],
+        "mountOptions": Sequence[str],
     },
     total=False,
 )
 
+
 class TmpfsTypeDef(_RequiredTmpfsTypeDef, _OptionalTmpfsTypeDef):
     pass
 
-ListAccountSettingsRequestListAccountSettingsPaginateTypeDef = TypedDict(
-    "ListAccountSettingsRequestListAccountSettingsPaginateTypeDef",
+
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "name": SettingNameType,
-        "value": str,
-        "principalArn": str,
-        "effectiveSettings": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListAccountSettingsRequestRequestTypeDef = TypedDict(
     "ListAccountSettingsRequestRequestTypeDef",
     {
@@ -1175,37 +1377,14 @@
         "effectiveSettings": bool,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListAttributesRequestListAttributesPaginateTypeDef = TypedDict(
-    "_RequiredListAttributesRequestListAttributesPaginateTypeDef",
-    {
-        "targetType": Literal["container-instance"],
-    },
-)
-_OptionalListAttributesRequestListAttributesPaginateTypeDef = TypedDict(
-    "_OptionalListAttributesRequestListAttributesPaginateTypeDef",
-    {
-        "cluster": str,
-        "attributeName": str,
-        "attributeValue": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAttributesRequestListAttributesPaginateTypeDef(
-    _RequiredListAttributesRequestListAttributesPaginateTypeDef,
-    _OptionalListAttributesRequestListAttributesPaginateTypeDef,
-):
-    pass
-
 _RequiredListAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredListAttributesRequestRequestTypeDef",
     {
         "targetType": Literal["container-instance"],
     },
 )
 _OptionalListAttributesRequestRequestTypeDef = TypedDict(
@@ -1216,97 +1395,42 @@
         "attributeValue": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListAttributesRequestRequestTypeDef(
     _RequiredListAttributesRequestRequestTypeDef, _OptionalListAttributesRequestRequestTypeDef
 ):
     pass
 
-ListClustersRequestListClustersPaginateTypeDef = TypedDict(
-    "ListClustersRequestListClustersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListClustersResponseTypeDef = TypedDict(
-    "ListClustersResponseTypeDef",
-    {
-        "clusterArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListContainerInstancesRequestListContainerInstancesPaginateTypeDef = TypedDict(
-    "ListContainerInstancesRequestListContainerInstancesPaginateTypeDef",
-    {
-        "cluster": str,
-        "filter": str,
-        "status": ContainerInstanceStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListContainerInstancesRequestRequestTypeDef = TypedDict(
     "ListContainerInstancesRequestRequestTypeDef",
     {
         "cluster": str,
         "filter": str,
         "nextToken": str,
         "maxResults": int,
         "status": ContainerInstanceStatusType,
     },
     total=False,
 )
 
-ListContainerInstancesResponseTypeDef = TypedDict(
-    "ListContainerInstancesResponseTypeDef",
-    {
-        "containerInstanceArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef = TypedDict(
-    "_RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
-    {
-        "namespace": str,
-    },
-)
-_OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef = TypedDict(
-    "_OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef(
-    _RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
-    _OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
-):
-    pass
-
 _RequiredListServicesByNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredListServicesByNamespaceRequestRequestTypeDef",
     {
         "namespace": str,
     },
 )
 _OptionalListServicesByNamespaceRequestRequestTypeDef = TypedDict(
@@ -1314,145 +1438,64 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListServicesByNamespaceRequestRequestTypeDef(
     _RequiredListServicesByNamespaceRequestRequestTypeDef,
     _OptionalListServicesByNamespaceRequestRequestTypeDef,
 ):
     pass
 
-ListServicesByNamespaceResponseTypeDef = TypedDict(
-    "ListServicesByNamespaceResponseTypeDef",
-    {
-        "serviceArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListServicesRequestListServicesPaginateTypeDef = TypedDict(
-    "ListServicesRequestListServicesPaginateTypeDef",
-    {
-        "cluster": str,
-        "launchType": LaunchTypeType,
-        "schedulingStrategy": SchedulingStrategyType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListServicesRequestRequestTypeDef = TypedDict(
     "ListServicesRequestRequestTypeDef",
     {
         "cluster": str,
         "nextToken": str,
         "maxResults": int,
         "launchType": LaunchTypeType,
         "schedulingStrategy": SchedulingStrategyType,
     },
     total=False,
 )
 
-ListServicesResponseTypeDef = TypedDict(
-    "ListServicesResponseTypeDef",
-    {
-        "serviceArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef = TypedDict(
-    "ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef",
-    {
-        "familyPrefix": str,
-        "status": TaskDefinitionFamilyStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTaskDefinitionFamiliesRequestRequestTypeDef = TypedDict(
     "ListTaskDefinitionFamiliesRequestRequestTypeDef",
     {
         "familyPrefix": str,
         "status": TaskDefinitionFamilyStatusType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListTaskDefinitionFamiliesResponseTypeDef = TypedDict(
-    "ListTaskDefinitionFamiliesResponseTypeDef",
-    {
-        "families": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef = TypedDict(
-    "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
-    {
-        "familyPrefix": str,
-        "status": TaskDefinitionStatusType,
-        "sort": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTaskDefinitionsRequestRequestTypeDef = TypedDict(
     "ListTaskDefinitionsRequestRequestTypeDef",
     {
         "familyPrefix": str,
         "status": TaskDefinitionStatusType,
         "sort": SortOrderType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListTaskDefinitionsResponseTypeDef = TypedDict(
-    "ListTaskDefinitionsResponseTypeDef",
-    {
-        "taskDefinitionArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTasksRequestListTasksPaginateTypeDef = TypedDict(
-    "ListTasksRequestListTasksPaginateTypeDef",
-    {
-        "cluster": str,
-        "containerInstance": str,
-        "family": str,
-        "startedBy": str,
-        "serviceName": str,
-        "desiredStatus": DesiredStatusType,
-        "launchType": LaunchTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTasksRequestRequestTypeDef = TypedDict(
     "ListTasksRequestRequestTypeDef",
     {
         "cluster": str,
         "containerInstance": str,
         "family": str,
         "nextToken": str,
@@ -1461,23 +1504,14 @@
         "serviceName": str,
         "desiredStatus": DesiredStatusType,
         "launchType": LaunchTypeType,
     },
     total=False,
 )
 
-ListTasksResponseTypeDef = TypedDict(
-    "ListTasksResponseTypeDef",
-    {
-        "taskArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredManagedAgentStateChangeTypeDef = TypedDict(
     "_RequiredManagedAgentStateChangeTypeDef",
     {
         "containerName": str,
         "managedAgentName": Literal["ExecuteCommandAgent"],
         "status": str,
     },
@@ -1486,28 +1520,20 @@
     "_OptionalManagedAgentStateChangeTypeDef",
     {
         "reason": str,
     },
     total=False,
 )
 
+
 class ManagedAgentStateChangeTypeDef(
     _RequiredManagedAgentStateChangeTypeDef, _OptionalManagedAgentStateChangeTypeDef
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
 
 PlatformDeviceTypeDef = TypedDict(
     "PlatformDeviceTypeDef",
     {
         "id": str,
         "type": Literal["GPU"],
     },
@@ -1532,19 +1558,21 @@
     "_OptionalPutAccountSettingRequestRequestTypeDef",
     {
         "principalArn": str,
     },
     total=False,
 )
 
+
 class PutAccountSettingRequestRequestTypeDef(
     _RequiredPutAccountSettingRequestRequestTypeDef, _OptionalPutAccountSettingRequestRequestTypeDef
 ):
     pass
 
+
 RuntimePlatformTypeDef = TypedDict(
     "RuntimePlatformTypeDef",
     {
         "cpuArchitecture": CPUArchitectureType,
         "operatingSystemFamily": OSFamilyType,
     },
     total=False,
@@ -1555,23 +1583,25 @@
     {
         "type": Literal["memberOf"],
         "expression": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ResourceTypeDef = TypedDict(
+    "ResourceTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "name": str,
+        "type": str,
+        "doubleValue": float,
+        "longValue": int,
+        "integerValue": int,
+        "stringSetValue": Sequence[str],
     },
+    total=False,
 )
 
 _RequiredServiceConnectClientAliasTypeDef = TypedDict(
     "_RequiredServiceConnectClientAliasTypeDef",
     {
         "port": int,
     },
@@ -1580,19 +1610,21 @@
     "_OptionalServiceConnectClientAliasTypeDef",
     {
         "dnsName": str,
     },
     total=False,
 )
 
+
 class ServiceConnectClientAliasTypeDef(
     _RequiredServiceConnectClientAliasTypeDef, _OptionalServiceConnectClientAliasTypeDef
 ):
     pass
 
+
 ServiceEventTypeDef = TypedDict(
     "ServiceEventTypeDef",
     {
         "id": str,
         "createdAt": datetime,
         "message": str,
     },
@@ -1610,43 +1642,22 @@
     {
         "cluster": str,
         "reason": str,
     },
     total=False,
 )
 
+
 class StopTaskRequestRequestTypeDef(
     _RequiredStopTaskRequestRequestTypeDef, _OptionalStopTaskRequestRequestTypeDef
 ):
     pass
 
-SubmitAttachmentStateChangesResponseTypeDef = TypedDict(
-    "SubmitAttachmentStateChangesResponseTypeDef",
-    {
-        "acknowledgment": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SubmitContainerStateChangeResponseTypeDef = TypedDict(
-    "SubmitContainerStateChangeResponseTypeDef",
-    {
-        "acknowledgment": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SubmitTaskStateChangeResponseTypeDef = TypedDict(
-    "SubmitTaskStateChangeResponseTypeDef",
-    {
-        "acknowledgment": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
+TimestampTypeDef = Union[datetime, str]
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -1661,20 +1672,22 @@
     "_OptionalUpdateContainerAgentRequestRequestTypeDef",
     {
         "cluster": str,
     },
     total=False,
 )
 
+
 class UpdateContainerAgentRequestRequestTypeDef(
     _RequiredUpdateContainerAgentRequestRequestTypeDef,
     _OptionalUpdateContainerAgentRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateContainerInstancesStateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContainerInstancesStateRequestRequestTypeDef",
     {
         "containerInstances": Sequence[str],
         "status": ContainerInstanceStatusType,
     },
 )
@@ -1682,20 +1695,22 @@
     "_OptionalUpdateContainerInstancesStateRequestRequestTypeDef",
     {
         "cluster": str,
     },
     total=False,
 )
 
+
 class UpdateContainerInstancesStateRequestRequestTypeDef(
     _RequiredUpdateContainerInstancesStateRequestRequestTypeDef,
     _OptionalUpdateContainerInstancesStateRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateServicePrimaryTaskSetRequestRequestTypeDef = TypedDict(
     "UpdateServicePrimaryTaskSetRequestRequestTypeDef",
     {
         "cluster": str,
         "service": str,
         "primaryTaskSet": str,
     },
@@ -1713,106 +1728,119 @@
     "_OptionalUpdateTaskProtectionRequestRequestTypeDef",
     {
         "expiresInMinutes": int,
     },
     total=False,
 )
 
+
 class UpdateTaskProtectionRequestRequestTypeDef(
     _RequiredUpdateTaskProtectionRequestRequestTypeDef,
     _OptionalUpdateTaskProtectionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSubmitAttachmentStateChangesRequestRequestTypeDef = TypedDict(
     "_RequiredSubmitAttachmentStateChangesRequestRequestTypeDef",
     {
         "attachments": Sequence[AttachmentStateChangeTypeDef],
     },
 )
 _OptionalSubmitAttachmentStateChangesRequestRequestTypeDef = TypedDict(
     "_OptionalSubmitAttachmentStateChangesRequestRequestTypeDef",
     {
         "cluster": str,
     },
     total=False,
 )
 
+
 class SubmitAttachmentStateChangesRequestRequestTypeDef(
     _RequiredSubmitAttachmentStateChangesRequestRequestTypeDef,
     _OptionalSubmitAttachmentStateChangesRequestRequestTypeDef,
 ):
     pass
 
+
 AttachmentTypeDef = TypedDict(
     "AttachmentTypeDef",
     {
         "id": str,
         "type": str,
         "status": str,
         "details": List[KeyValuePairTypeDef],
     },
     total=False,
 )
 
+_RequiredProxyConfigurationOutputTypeDef = TypedDict(
+    "_RequiredProxyConfigurationOutputTypeDef",
+    {
+        "containerName": str,
+    },
+)
+_OptionalProxyConfigurationOutputTypeDef = TypedDict(
+    "_OptionalProxyConfigurationOutputTypeDef",
+    {
+        "type": Literal["APPMESH"],
+        "properties": List[KeyValuePairTypeDef],
+    },
+    total=False,
+)
+
+
+class ProxyConfigurationOutputTypeDef(
+    _RequiredProxyConfigurationOutputTypeDef, _OptionalProxyConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredProxyConfigurationTypeDef = TypedDict(
     "_RequiredProxyConfigurationTypeDef",
     {
         "containerName": str,
     },
 )
 _OptionalProxyConfigurationTypeDef = TypedDict(
     "_OptionalProxyConfigurationTypeDef",
     {
         "type": Literal["APPMESH"],
-        "properties": List[KeyValuePairTypeDef],
+        "properties": Sequence[KeyValuePairTypeDef],
     },
     total=False,
 )
 
+
 class ProxyConfigurationTypeDef(
     _RequiredProxyConfigurationTypeDef, _OptionalProxyConfigurationTypeDef
 ):
     pass
 
+
 _RequiredDeleteAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAttributesRequestRequestTypeDef",
     {
         "attributes": Sequence[AttributeTypeDef],
     },
 )
 _OptionalDeleteAttributesRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteAttributesRequestRequestTypeDef",
     {
         "cluster": str,
     },
     total=False,
 )
 
+
 class DeleteAttributesRequestRequestTypeDef(
     _RequiredDeleteAttributesRequestRequestTypeDef, _OptionalDeleteAttributesRequestRequestTypeDef
 ):
     pass
 
-DeleteAttributesResponseTypeDef = TypedDict(
-    "DeleteAttributesResponseTypeDef",
-    {
-        "attributes": List[AttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAttributesResponseTypeDef = TypedDict(
-    "ListAttributesResponseTypeDef",
-    {
-        "attributes": List[AttributeTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredPutAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutAttributesRequestRequestTypeDef",
     {
         "attributes": Sequence[AttributeTypeDef],
     },
 )
@@ -1820,26 +1848,20 @@
     "_OptionalPutAttributesRequestRequestTypeDef",
     {
         "cluster": str,
     },
     total=False,
 )
 
+
 class PutAttributesRequestRequestTypeDef(
     _RequiredPutAttributesRequestRequestTypeDef, _OptionalPutAttributesRequestRequestTypeDef
 ):
     pass
 
-PutAttributesResponseTypeDef = TypedDict(
-    "PutAttributesResponseTypeDef",
-    {
-        "attributes": List[AttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredAutoScalingGroupProviderTypeDef = TypedDict(
     "_RequiredAutoScalingGroupProviderTypeDef",
     {
         "autoScalingGroupArn": str,
     },
 )
@@ -1848,28 +1870,38 @@
     {
         "managedScaling": ManagedScalingTypeDef,
         "managedTerminationProtection": ManagedTerminationProtectionType,
     },
     total=False,
 )
 
+
 class AutoScalingGroupProviderTypeDef(
     _RequiredAutoScalingGroupProviderTypeDef, _OptionalAutoScalingGroupProviderTypeDef
 ):
     pass
 
+
 AutoScalingGroupProviderUpdateTypeDef = TypedDict(
     "AutoScalingGroupProviderUpdateTypeDef",
     {
         "managedScaling": ManagedScalingTypeDef,
         "managedTerminationProtection": ManagedTerminationProtectionType,
     },
     total=False,
 )
 
+NetworkConfigurationOutputTypeDef = TypedDict(
+    "NetworkConfigurationOutputTypeDef",
+    {
+        "awsvpcConfiguration": AwsVpcConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "awsvpcConfiguration": AwsVpcConfigurationTypeDef,
     },
     total=False,
 )
@@ -1879,22 +1911,14 @@
     {
         "cluster": str,
         "capacityProviders": Sequence[str],
         "defaultCapacityProviderStrategy": Sequence[CapacityProviderStrategyItemTypeDef],
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -1903,29 +1927,66 @@
     "UpdateClusterSettingsRequestRequestTypeDef",
     {
         "cluster": str,
         "settings": Sequence[ClusterSettingTypeDef],
     },
 )
 
-ContainerOverrideTypeDef = TypedDict(
-    "ContainerOverrideTypeDef",
+ContainerOverrideOutputTypeDef = TypedDict(
+    "ContainerOverrideOutputTypeDef",
     {
         "name": str,
         "command": List[str],
         "environment": List[KeyValuePairTypeDef],
         "environmentFiles": List[EnvironmentFileTypeDef],
         "cpu": int,
         "memory": int,
         "memoryReservation": int,
         "resourceRequirements": List[ResourceRequirementTypeDef],
     },
     total=False,
 )
 
+ContainerOverrideTypeDef = TypedDict(
+    "ContainerOverrideTypeDef",
+    {
+        "name": str,
+        "command": Sequence[str],
+        "environment": Sequence[KeyValuePairTypeDef],
+        "environmentFiles": Sequence[EnvironmentFileTypeDef],
+        "cpu": int,
+        "memory": int,
+        "memoryReservation": int,
+        "resourceRequirements": Sequence[ResourceRequirementTypeDef],
+    },
+    total=False,
+)
+
+_RequiredLogConfigurationOutputTypeDef = TypedDict(
+    "_RequiredLogConfigurationOutputTypeDef",
+    {
+        "logDriver": LogDriverType,
+    },
+)
+_OptionalLogConfigurationOutputTypeDef = TypedDict(
+    "_OptionalLogConfigurationOutputTypeDef",
+    {
+        "options": Dict[str, str],
+        "secretOptions": List[SecretTypeDef],
+    },
+    total=False,
+)
+
+
+class LogConfigurationOutputTypeDef(
+    _RequiredLogConfigurationOutputTypeDef, _OptionalLogConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredLogConfigurationTypeDef = TypedDict(
     "_RequiredLogConfigurationTypeDef",
     {
         "logDriver": LogDriverType,
     },
 )
 _OptionalLogConfigurationTypeDef = TypedDict(
@@ -1933,17 +1994,19 @@
     {
         "options": Mapping[str, str],
         "secretOptions": Sequence[SecretTypeDef],
     },
     total=False,
 )
 
+
 class LogConfigurationTypeDef(_RequiredLogConfigurationTypeDef, _OptionalLogConfigurationTypeDef):
     pass
 
+
 ContainerInstanceHealthStatusTypeDef = TypedDict(
     "ContainerInstanceHealthStatusTypeDef",
     {
         "overallStatus": InstanceHealthCheckStateType,
         "details": List[InstanceHealthCheckResultTypeDef],
     },
     total=False,
@@ -1998,57 +2061,198 @@
         "memory": str,
         "memoryReservation": str,
         "gpuIds": List[str],
     },
     total=False,
 )
 
+DeleteAttributesResponseTypeDef = TypedDict(
+    "DeleteAttributesResponseTypeDef",
+    {
+        "attributes": List[AttributeTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DiscoverPollEndpointResponseTypeDef = TypedDict(
+    "DiscoverPollEndpointResponseTypeDef",
+    {
+        "endpoint": str,
+        "telemetryEndpoint": str,
+        "serviceConnectEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAttributesResponseTypeDef = TypedDict(
+    "ListAttributesResponseTypeDef",
+    {
+        "attributes": List[AttributeTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListClustersResponseTypeDef = TypedDict(
+    "ListClustersResponseTypeDef",
+    {
+        "clusterArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListContainerInstancesResponseTypeDef = TypedDict(
+    "ListContainerInstancesResponseTypeDef",
+    {
+        "containerInstanceArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListServicesByNamespaceResponseTypeDef = TypedDict(
+    "ListServicesByNamespaceResponseTypeDef",
+    {
+        "serviceArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListServicesResponseTypeDef = TypedDict(
+    "ListServicesResponseTypeDef",
+    {
+        "serviceArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTaskDefinitionFamiliesResponseTypeDef = TypedDict(
+    "ListTaskDefinitionFamiliesResponseTypeDef",
+    {
+        "families": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTaskDefinitionsResponseTypeDef = TypedDict(
+    "ListTaskDefinitionsResponseTypeDef",
+    {
+        "taskDefinitionArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTasksResponseTypeDef = TypedDict(
+    "ListTasksResponseTypeDef",
+    {
+        "taskArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutAttributesResponseTypeDef = TypedDict(
+    "PutAttributesResponseTypeDef",
+    {
+        "attributes": List[AttributeTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SubmitAttachmentStateChangesResponseTypeDef = TypedDict(
+    "SubmitAttachmentStateChangesResponseTypeDef",
+    {
+        "acknowledgment": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SubmitContainerStateChangeResponseTypeDef = TypedDict(
+    "SubmitContainerStateChangeResponseTypeDef",
+    {
+        "acknowledgment": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SubmitTaskStateChangeResponseTypeDef = TypedDict(
+    "SubmitTaskStateChangeResponseTypeDef",
+    {
+        "acknowledgment": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateTaskSetRequestRequestTypeDef = TypedDict(
     "UpdateTaskSetRequestRequestTypeDef",
     {
         "cluster": str,
         "service": str,
         "taskSet": str,
         "scale": ScaleTypeDef,
     },
 )
 
 DeleteAccountSettingResponseTypeDef = TypedDict(
     "DeleteAccountSettingResponseTypeDef",
     {
         "setting": SettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAccountSettingsResponseTypeDef = TypedDict(
     "ListAccountSettingsResponseTypeDef",
     {
         "settings": List[SettingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAccountSettingDefaultResponseTypeDef = TypedDict(
     "PutAccountSettingDefaultResponseTypeDef",
     {
         "setting": SettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAccountSettingResponseTypeDef = TypedDict(
     "PutAccountSettingResponseTypeDef",
     {
         "setting": SettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DeploymentConfigurationOutputTypeDef = TypedDict(
+    "DeploymentConfigurationOutputTypeDef",
+    {
+        "deploymentCircuitBreaker": DeploymentCircuitBreakerTypeDef,
+        "maximumPercent": int,
+        "minimumHealthyPercent": int,
+        "alarms": DeploymentAlarmsOutputTypeDef,
+    },
+    total=False,
+)
+
 DeploymentConfigurationTypeDef = TypedDict(
     "DeploymentConfigurationTypeDef",
     {
         "deploymentCircuitBreaker": DeploymentCircuitBreakerTypeDef,
         "maximumPercent": int,
         "minimumHealthyPercent": int,
         "alarms": DeploymentAlarmsTypeDef,
@@ -2068,20 +2272,22 @@
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeServicesRequestServicesInactiveWaitTypeDef(
     _RequiredDescribeServicesRequestServicesInactiveWaitTypeDef,
     _OptionalDescribeServicesRequestServicesInactiveWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeServicesRequestServicesStableWaitTypeDef = TypedDict(
     "_RequiredDescribeServicesRequestServicesStableWaitTypeDef",
     {
         "services": Sequence[str],
     },
 )
 _OptionalDescribeServicesRequestServicesStableWaitTypeDef = TypedDict(
@@ -2090,20 +2296,22 @@
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeServicesRequestServicesStableWaitTypeDef(
     _RequiredDescribeServicesRequestServicesStableWaitTypeDef,
     _OptionalDescribeServicesRequestServicesStableWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeTasksRequestTasksRunningWaitTypeDef = TypedDict(
     "_RequiredDescribeTasksRequestTasksRunningWaitTypeDef",
     {
         "tasks": Sequence[str],
     },
 )
 _OptionalDescribeTasksRequestTasksRunningWaitTypeDef = TypedDict(
@@ -2112,20 +2320,22 @@
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeTasksRequestTasksRunningWaitTypeDef(
     _RequiredDescribeTasksRequestTasksRunningWaitTypeDef,
     _OptionalDescribeTasksRequestTasksRunningWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeTasksRequestTasksStoppedWaitTypeDef = TypedDict(
     "_RequiredDescribeTasksRequestTasksStoppedWaitTypeDef",
     {
         "tasks": Sequence[str],
     },
 )
 _OptionalDescribeTasksRequestTasksStoppedWaitTypeDef = TypedDict(
@@ -2134,20 +2344,22 @@
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeTasksRequestTasksStoppedWaitTypeDef(
     _RequiredDescribeTasksRequestTasksStoppedWaitTypeDef,
     _OptionalDescribeTasksRequestTasksStoppedWaitTypeDef,
 ):
     pass
 
+
 _RequiredEFSVolumeConfigurationTypeDef = TypedDict(
     "_RequiredEFSVolumeConfigurationTypeDef",
     {
         "fileSystemId": str,
     },
 )
 _OptionalEFSVolumeConfigurationTypeDef = TypedDict(
@@ -2157,19 +2369,21 @@
         "transitEncryption": EFSTransitEncryptionType,
         "transitEncryptionPort": int,
         "authorizationConfig": EFSAuthorizationConfigTypeDef,
     },
     total=False,
 )
 
+
 class EFSVolumeConfigurationTypeDef(
     _RequiredEFSVolumeConfigurationTypeDef, _OptionalEFSVolumeConfigurationTypeDef
 ):
     pass
 
+
 ExecuteCommandConfigurationTypeDef = TypedDict(
     "ExecuteCommandConfigurationTypeDef",
     {
         "kmsKeyId": str,
         "logging": ExecuteCommandLoggingType,
         "logConfiguration": ExecuteCommandLogConfigurationTypeDef,
     },
@@ -2181,15 +2395,15 @@
     {
         "clusterArn": str,
         "containerArn": str,
         "containerName": str,
         "interactive": bool,
         "session": SessionTypeDef,
         "taskArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FSxWindowsFileServerVolumeConfigurationTypeDef = TypedDict(
     "FSxWindowsFileServerVolumeConfigurationTypeDef",
     {
         "fileSystemId": str,
@@ -2199,57 +2413,204 @@
 )
 
 GetTaskProtectionResponseTypeDef = TypedDict(
     "GetTaskProtectionResponseTypeDef",
     {
         "protectedTasks": List[ProtectedTaskTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTaskProtectionResponseTypeDef = TypedDict(
     "UpdateTaskProtectionResponseTypeDef",
     {
         "protectedTasks": List[ProtectedTaskTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LinuxParametersOutputTypeDef = TypedDict(
+    "LinuxParametersOutputTypeDef",
+    {
+        "capabilities": KernelCapabilitiesOutputTypeDef,
+        "devices": List[DeviceOutputTypeDef],
+        "initProcessEnabled": bool,
+        "sharedMemorySize": int,
+        "tmpfs": List[TmpfsOutputTypeDef],
+        "maxSwap": int,
+        "swappiness": int,
     },
+    total=False,
 )
 
 LinuxParametersTypeDef = TypedDict(
     "LinuxParametersTypeDef",
     {
         "capabilities": KernelCapabilitiesTypeDef,
-        "devices": List[DeviceTypeDef],
+        "devices": Sequence[DeviceTypeDef],
         "initProcessEnabled": bool,
         "sharedMemorySize": int,
-        "tmpfs": List[TmpfsTypeDef],
+        "tmpfs": Sequence[TmpfsTypeDef],
         "maxSwap": int,
         "swappiness": int,
     },
     total=False,
 )
 
-RegisterContainerInstanceRequestRequestTypeDef = TypedDict(
-    "RegisterContainerInstanceRequestRequestTypeDef",
+ListAccountSettingsRequestListAccountSettingsPaginateTypeDef = TypedDict(
+    "ListAccountSettingsRequestListAccountSettingsPaginateTypeDef",
+    {
+        "name": SettingNameType,
+        "value": str,
+        "principalArn": str,
+        "effectiveSettings": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListAttributesRequestListAttributesPaginateTypeDef = TypedDict(
+    "_RequiredListAttributesRequestListAttributesPaginateTypeDef",
+    {
+        "targetType": Literal["container-instance"],
+    },
+)
+_OptionalListAttributesRequestListAttributesPaginateTypeDef = TypedDict(
+    "_OptionalListAttributesRequestListAttributesPaginateTypeDef",
     {
         "cluster": str,
-        "instanceIdentityDocument": str,
-        "instanceIdentityDocumentSignature": str,
-        "totalResources": Sequence[ResourceTypeDef],
-        "versionInfo": VersionInfoTypeDef,
-        "containerInstanceArn": str,
-        "attributes": Sequence[AttributeTypeDef],
-        "platformDevices": Sequence[PlatformDeviceTypeDef],
-        "tags": Sequence[TagTypeDef],
+        "attributeName": str,
+        "attributeValue": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAttributesRequestListAttributesPaginateTypeDef(
+    _RequiredListAttributesRequestListAttributesPaginateTypeDef,
+    _OptionalListAttributesRequestListAttributesPaginateTypeDef,
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
+ListContainerInstancesRequestListContainerInstancesPaginateTypeDef = TypedDict(
+    "ListContainerInstancesRequestListContainerInstancesPaginateTypeDef",
+    {
+        "cluster": str,
+        "filter": str,
+        "status": ContainerInstanceStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef = TypedDict(
+    "_RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
+    {
+        "namespace": str,
+    },
+)
+_OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef = TypedDict(
+    "_OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef(
+    _RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
+    _OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
+):
+    pass
+
+
+ListServicesRequestListServicesPaginateTypeDef = TypedDict(
+    "ListServicesRequestListServicesPaginateTypeDef",
+    {
+        "cluster": str,
+        "launchType": LaunchTypeType,
+        "schedulingStrategy": SchedulingStrategyType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef = TypedDict(
+    "ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef",
+    {
+        "familyPrefix": str,
+        "status": TaskDefinitionFamilyStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef = TypedDict(
+    "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
+    {
+        "familyPrefix": str,
+        "status": TaskDefinitionStatusType,
+        "sort": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTasksRequestListTasksPaginateTypeDef = TypedDict(
+    "ListTasksRequestListTasksPaginateTypeDef",
+    {
+        "cluster": str,
+        "containerInstance": str,
+        "family": str,
+        "startedBy": str,
+        "serviceName": str,
+        "desiredStatus": DesiredStatusType,
+        "launchType": LaunchTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+ResourceUnionTypeDef = Union[ResourceTypeDef, ResourceOutputTypeDef]
+_RequiredServiceConnectServiceOutputTypeDef = TypedDict(
+    "_RequiredServiceConnectServiceOutputTypeDef",
+    {
+        "portName": str,
+    },
+)
+_OptionalServiceConnectServiceOutputTypeDef = TypedDict(
+    "_OptionalServiceConnectServiceOutputTypeDef",
+    {
+        "discoveryName": str,
+        "clientAliases": List[ServiceConnectClientAliasTypeDef],
+        "ingressPortOverride": int,
+    },
+    total=False,
+)
+
+
+class ServiceConnectServiceOutputTypeDef(
+    _RequiredServiceConnectServiceOutputTypeDef, _OptionalServiceConnectServiceOutputTypeDef
+):
+    pass
+
+
 _RequiredServiceConnectServiceTypeDef = TypedDict(
     "_RequiredServiceConnectServiceTypeDef",
     {
         "portName": str,
     },
 )
 _OptionalServiceConnectServiceTypeDef = TypedDict(
@@ -2258,19 +2619,22 @@
         "discoveryName": str,
         "clientAliases": Sequence[ServiceConnectClientAliasTypeDef],
         "ingressPortOverride": int,
     },
     total=False,
 )
 
+
 class ServiceConnectServiceTypeDef(
     _RequiredServiceConnectServiceTypeDef, _OptionalServiceConnectServiceTypeDef
 ):
     pass
 
+
+ProxyConfigurationUnionTypeDef = Union[ProxyConfigurationTypeDef, ProxyConfigurationOutputTypeDef]
 CapacityProviderTypeDef = TypedDict(
     "CapacityProviderTypeDef",
     {
         "capacityProviderArn": str,
         "name": str,
         "status": CapacityProviderStatusType,
         "autoScalingGroupProvider": AutoScalingGroupProviderTypeDef,
@@ -2292,28 +2656,61 @@
     "_OptionalCreateCapacityProviderRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateCapacityProviderRequestRequestTypeDef(
     _RequiredCreateCapacityProviderRequestRequestTypeDef,
     _OptionalCreateCapacityProviderRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateCapacityProviderRequestRequestTypeDef = TypedDict(
     "UpdateCapacityProviderRequestRequestTypeDef",
     {
         "name": str,
         "autoScalingGroupProvider": AutoScalingGroupProviderUpdateTypeDef,
     },
 )
 
+TaskSetTypeDef = TypedDict(
+    "TaskSetTypeDef",
+    {
+        "id": str,
+        "taskSetArn": str,
+        "serviceArn": str,
+        "clusterArn": str,
+        "startedBy": str,
+        "externalId": str,
+        "status": str,
+        "taskDefinition": str,
+        "computedDesiredCount": int,
+        "pendingCount": int,
+        "runningCount": int,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "launchType": LaunchTypeType,
+        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
+        "platformVersion": str,
+        "platformFamily": str,
+        "networkConfiguration": NetworkConfigurationOutputTypeDef,
+        "loadBalancers": List[LoadBalancerTypeDef],
+        "serviceRegistries": List[ServiceRegistryTypeDef],
+        "scale": ScaleTypeDef,
+        "stabilityStatus": StabilityStatusType,
+        "stabilityStatusAt": datetime,
+        "tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
 _RequiredCreateTaskSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTaskSetRequestRequestTypeDef",
     {
         "service": str,
         "cluster": str,
         "taskDefinition": str,
     },
@@ -2331,56 +2728,44 @@
         "scale": ScaleTypeDef,
         "clientToken": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateTaskSetRequestRequestTypeDef(
     _RequiredCreateTaskSetRequestRequestTypeDef, _OptionalCreateTaskSetRequestRequestTypeDef
 ):
     pass
 
-TaskSetTypeDef = TypedDict(
-    "TaskSetTypeDef",
+
+NetworkConfigurationUnionTypeDef = Union[
+    NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
+]
+TaskOverrideOutputTypeDef = TypedDict(
+    "TaskOverrideOutputTypeDef",
     {
-        "id": str,
-        "taskSetArn": str,
-        "serviceArn": str,
-        "clusterArn": str,
-        "startedBy": str,
-        "externalId": str,
-        "status": str,
-        "taskDefinition": str,
-        "computedDesiredCount": int,
-        "pendingCount": int,
-        "runningCount": int,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "launchType": LaunchTypeType,
-        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
-        "platformVersion": str,
-        "platformFamily": str,
-        "networkConfiguration": NetworkConfigurationTypeDef,
-        "loadBalancers": List[LoadBalancerTypeDef],
-        "serviceRegistries": List[ServiceRegistryTypeDef],
-        "scale": ScaleTypeDef,
-        "stabilityStatus": StabilityStatusType,
-        "stabilityStatusAt": datetime,
-        "tags": List[TagTypeDef],
+        "containerOverrides": List[ContainerOverrideOutputTypeDef],
+        "cpu": str,
+        "inferenceAcceleratorOverrides": List[InferenceAcceleratorOverrideTypeDef],
+        "executionRoleArn": str,
+        "memory": str,
+        "taskRoleArn": str,
+        "ephemeralStorage": EphemeralStorageTypeDef,
     },
     total=False,
 )
 
 TaskOverrideTypeDef = TypedDict(
     "TaskOverrideTypeDef",
     {
-        "containerOverrides": List[ContainerOverrideTypeDef],
+        "containerOverrides": Sequence[ContainerOverrideTypeDef],
         "cpu": str,
-        "inferenceAcceleratorOverrides": List[InferenceAcceleratorOverrideTypeDef],
+        "inferenceAcceleratorOverrides": Sequence[InferenceAcceleratorOverrideTypeDef],
         "executionRoleArn": str,
         "memory": str,
         "taskRoleArn": str,
         "ephemeralStorage": EphemeralStorageTypeDef,
     },
     total=False,
 )
@@ -2389,16 +2774,16 @@
     "ContainerInstanceTypeDef",
     {
         "containerInstanceArn": str,
         "ec2InstanceId": str,
         "capacityProviderName": str,
         "version": int,
         "versionInfo": VersionInfoTypeDef,
-        "remainingResources": List[ResourceTypeDef],
-        "registeredResources": List[ResourceTypeDef],
+        "remainingResources": List[ResourceOutputTypeDef],
+        "registeredResources": List[ResourceOutputTypeDef],
         "status": str,
         "statusReason": str,
         "agentConnected": bool,
         "runningTasksCount": int,
         "pendingTasksCount": int,
         "agentUpdateStatus": AgentUpdateStatusType,
         "attributes": List[AttributeTypeDef],
@@ -2416,43 +2801,58 @@
         "cluster": str,
         "task": str,
         "status": str,
         "reason": str,
         "containers": Sequence[ContainerStateChangeTypeDef],
         "attachments": Sequence[AttachmentStateChangeTypeDef],
         "managedAgents": Sequence[ManagedAgentStateChangeTypeDef],
-        "pullStartedAt": Union[datetime, str],
-        "pullStoppedAt": Union[datetime, str],
-        "executionStoppedAt": Union[datetime, str],
+        "pullStartedAt": TimestampTypeDef,
+        "pullStoppedAt": TimestampTypeDef,
+        "executionStoppedAt": TimestampTypeDef,
     },
     total=False,
 )
 
+DeploymentConfigurationUnionTypeDef = Union[
+    DeploymentConfigurationTypeDef, DeploymentConfigurationOutputTypeDef
+]
 ClusterConfigurationTypeDef = TypedDict(
     "ClusterConfigurationTypeDef",
     {
         "executeCommandConfiguration": ExecuteCommandConfigurationTypeDef,
     },
     total=False,
 )
 
+VolumeOutputTypeDef = TypedDict(
+    "VolumeOutputTypeDef",
+    {
+        "name": str,
+        "host": HostVolumePropertiesTypeDef,
+        "dockerVolumeConfiguration": DockerVolumeConfigurationOutputTypeDef,
+        "efsVolumeConfiguration": EFSVolumeConfigurationTypeDef,
+        "fsxWindowsFileServerVolumeConfiguration": FSxWindowsFileServerVolumeConfigurationTypeDef,
+    },
+    total=False,
+)
+
 VolumeTypeDef = TypedDict(
     "VolumeTypeDef",
     {
         "name": str,
         "host": HostVolumePropertiesTypeDef,
         "dockerVolumeConfiguration": DockerVolumeConfigurationTypeDef,
         "efsVolumeConfiguration": EFSVolumeConfigurationTypeDef,
         "fsxWindowsFileServerVolumeConfiguration": FSxWindowsFileServerVolumeConfigurationTypeDef,
     },
     total=False,
 )
 
-ContainerDefinitionTypeDef = TypedDict(
-    "ContainerDefinitionTypeDef",
+ContainerDefinitionOutputTypeDef = TypedDict(
+    "ContainerDefinitionOutputTypeDef",
     {
         "name": str,
         "image": str,
         "repositoryCredentials": RepositoryCredentialsTypeDef,
         "cpu": int,
         "memory": int,
         "memoryReservation": int,
@@ -2461,15 +2861,15 @@
         "essential": bool,
         "entryPoint": List[str],
         "command": List[str],
         "environment": List[KeyValuePairTypeDef],
         "environmentFiles": List[EnvironmentFileTypeDef],
         "mountPoints": List[MountPointTypeDef],
         "volumesFrom": List[VolumeFromTypeDef],
-        "linuxParameters": LinuxParametersTypeDef,
+        "linuxParameters": LinuxParametersOutputTypeDef,
         "secrets": List[SecretTypeDef],
         "dependsOn": List[ContainerDependencyTypeDef],
         "startTimeout": int,
         "stopTimeout": int,
         "hostname": str,
         "user": str,
         "workingDirectory": str,
@@ -2480,23 +2880,109 @@
         "dnsSearchDomains": List[str],
         "extraHosts": List[HostEntryTypeDef],
         "dockerSecurityOptions": List[str],
         "interactive": bool,
         "pseudoTerminal": bool,
         "dockerLabels": Dict[str, str],
         "ulimits": List[UlimitTypeDef],
-        "logConfiguration": LogConfigurationTypeDef,
-        "healthCheck": HealthCheckTypeDef,
+        "logConfiguration": LogConfigurationOutputTypeDef,
+        "healthCheck": HealthCheckOutputTypeDef,
         "systemControls": List[SystemControlTypeDef],
         "resourceRequirements": List[ResourceRequirementTypeDef],
+        "firelensConfiguration": FirelensConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+ContainerDefinitionTypeDef = TypedDict(
+    "ContainerDefinitionTypeDef",
+    {
+        "name": str,
+        "image": str,
+        "repositoryCredentials": RepositoryCredentialsTypeDef,
+        "cpu": int,
+        "memory": int,
+        "memoryReservation": int,
+        "links": Sequence[str],
+        "portMappings": Sequence[PortMappingTypeDef],
+        "essential": bool,
+        "entryPoint": Sequence[str],
+        "command": Sequence[str],
+        "environment": Sequence[KeyValuePairTypeDef],
+        "environmentFiles": Sequence[EnvironmentFileTypeDef],
+        "mountPoints": Sequence[MountPointTypeDef],
+        "volumesFrom": Sequence[VolumeFromTypeDef],
+        "linuxParameters": LinuxParametersTypeDef,
+        "secrets": Sequence[SecretTypeDef],
+        "dependsOn": Sequence[ContainerDependencyTypeDef],
+        "startTimeout": int,
+        "stopTimeout": int,
+        "hostname": str,
+        "user": str,
+        "workingDirectory": str,
+        "disableNetworking": bool,
+        "privileged": bool,
+        "readonlyRootFilesystem": bool,
+        "dnsServers": Sequence[str],
+        "dnsSearchDomains": Sequence[str],
+        "extraHosts": Sequence[HostEntryTypeDef],
+        "dockerSecurityOptions": Sequence[str],
+        "interactive": bool,
+        "pseudoTerminal": bool,
+        "dockerLabels": Mapping[str, str],
+        "ulimits": Sequence[UlimitTypeDef],
+        "logConfiguration": LogConfigurationTypeDef,
+        "healthCheck": HealthCheckTypeDef,
+        "systemControls": Sequence[SystemControlTypeDef],
+        "resourceRequirements": Sequence[ResourceRequirementTypeDef],
         "firelensConfiguration": FirelensConfigurationTypeDef,
     },
     total=False,
 )
 
+RegisterContainerInstanceRequestRequestTypeDef = TypedDict(
+    "RegisterContainerInstanceRequestRequestTypeDef",
+    {
+        "cluster": str,
+        "instanceIdentityDocument": str,
+        "instanceIdentityDocumentSignature": str,
+        "totalResources": Sequence[ResourceUnionTypeDef],
+        "versionInfo": VersionInfoTypeDef,
+        "containerInstanceArn": str,
+        "attributes": Sequence[AttributeTypeDef],
+        "platformDevices": Sequence[PlatformDeviceTypeDef],
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+_RequiredServiceConnectConfigurationOutputTypeDef = TypedDict(
+    "_RequiredServiceConnectConfigurationOutputTypeDef",
+    {
+        "enabled": bool,
+    },
+)
+_OptionalServiceConnectConfigurationOutputTypeDef = TypedDict(
+    "_OptionalServiceConnectConfigurationOutputTypeDef",
+    {
+        "namespace": str,
+        "services": List[ServiceConnectServiceOutputTypeDef],
+        "logConfiguration": LogConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class ServiceConnectConfigurationOutputTypeDef(
+    _RequiredServiceConnectConfigurationOutputTypeDef,
+    _OptionalServiceConnectConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredServiceConnectConfigurationTypeDef = TypedDict(
     "_RequiredServiceConnectConfigurationTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalServiceConnectConfigurationTypeDef = TypedDict(
@@ -2505,92 +2991,137 @@
         "namespace": str,
         "services": Sequence[ServiceConnectServiceTypeDef],
         "logConfiguration": LogConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class ServiceConnectConfigurationTypeDef(
     _RequiredServiceConnectConfigurationTypeDef, _OptionalServiceConnectConfigurationTypeDef
 ):
     pass
 
+
 CreateCapacityProviderResponseTypeDef = TypedDict(
     "CreateCapacityProviderResponseTypeDef",
     {
         "capacityProvider": CapacityProviderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteCapacityProviderResponseTypeDef = TypedDict(
     "DeleteCapacityProviderResponseTypeDef",
     {
         "capacityProvider": CapacityProviderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCapacityProvidersResponseTypeDef = TypedDict(
     "DescribeCapacityProvidersResponseTypeDef",
     {
         "capacityProviders": List[CapacityProviderTypeDef],
         "failures": List[FailureTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCapacityProviderResponseTypeDef = TypedDict(
     "UpdateCapacityProviderResponseTypeDef",
     {
         "capacityProvider": CapacityProviderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTaskSetResponseTypeDef = TypedDict(
     "CreateTaskSetResponseTypeDef",
     {
         "taskSet": TaskSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteTaskSetResponseTypeDef = TypedDict(
     "DeleteTaskSetResponseTypeDef",
     {
         "taskSet": TaskSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTaskSetsResponseTypeDef = TypedDict(
     "DescribeTaskSetsResponseTypeDef",
     {
         "taskSets": List[TaskSetTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServicePrimaryTaskSetResponseTypeDef = TypedDict(
     "UpdateServicePrimaryTaskSetResponseTypeDef",
     {
         "taskSet": TaskSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTaskSetResponseTypeDef = TypedDict(
     "UpdateTaskSetResponseTypeDef",
     {
         "taskSet": TaskSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TaskTypeDef = TypedDict(
+    "TaskTypeDef",
+    {
+        "attachments": List[AttachmentTypeDef],
+        "attributes": List[AttributeTypeDef],
+        "availabilityZone": str,
+        "capacityProviderName": str,
+        "clusterArn": str,
+        "connectivity": ConnectivityType,
+        "connectivityAt": datetime,
+        "containerInstanceArn": str,
+        "containers": List[ContainerTypeDef],
+        "cpu": str,
+        "createdAt": datetime,
+        "desiredStatus": str,
+        "enableExecuteCommand": bool,
+        "executionStoppedAt": datetime,
+        "group": str,
+        "healthStatus": HealthStatusType,
+        "inferenceAccelerators": List[InferenceAcceleratorTypeDef],
+        "lastStatus": str,
+        "launchType": LaunchTypeType,
+        "memory": str,
+        "overrides": TaskOverrideOutputTypeDef,
+        "platformVersion": str,
+        "platformFamily": str,
+        "pullStartedAt": datetime,
+        "pullStoppedAt": datetime,
+        "startedAt": datetime,
+        "startedBy": str,
+        "stopCode": TaskStopCodeType,
+        "stoppedAt": datetime,
+        "stoppedReason": str,
+        "stoppingAt": datetime,
+        "tags": List[TagTypeDef],
+        "taskArn": str,
+        "taskDefinitionArn": str,
+        "version": int,
+        "ephemeralStorage": EphemeralStorageTypeDef,
     },
+    total=False,
 )
 
 _RequiredRunTaskRequestRequestTypeDef = TypedDict(
     "_RequiredRunTaskRequestRequestTypeDef",
     {
         "taskDefinition": str,
     },
@@ -2614,19 +3145,21 @@
         "referenceId": str,
         "startedBy": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class RunTaskRequestRequestTypeDef(
     _RequiredRunTaskRequestRequestTypeDef, _OptionalRunTaskRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredStartTaskRequestRequestTypeDef = TypedDict(
     "_RequiredStartTaskRequestRequestTypeDef",
     {
         "containerInstances": Sequence[str],
         "taskDefinition": str,
     },
 )
@@ -2643,101 +3176,61 @@
         "referenceId": str,
         "startedBy": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class StartTaskRequestRequestTypeDef(
     _RequiredStartTaskRequestRequestTypeDef, _OptionalStartTaskRequestRequestTypeDef
 ):
     pass
 
-TaskTypeDef = TypedDict(
-    "TaskTypeDef",
-    {
-        "attachments": List[AttachmentTypeDef],
-        "attributes": List[AttributeTypeDef],
-        "availabilityZone": str,
-        "capacityProviderName": str,
-        "clusterArn": str,
-        "connectivity": ConnectivityType,
-        "connectivityAt": datetime,
-        "containerInstanceArn": str,
-        "containers": List[ContainerTypeDef],
-        "cpu": str,
-        "createdAt": datetime,
-        "desiredStatus": str,
-        "enableExecuteCommand": bool,
-        "executionStoppedAt": datetime,
-        "group": str,
-        "healthStatus": HealthStatusType,
-        "inferenceAccelerators": List[InferenceAcceleratorTypeDef],
-        "lastStatus": str,
-        "launchType": LaunchTypeType,
-        "memory": str,
-        "overrides": TaskOverrideTypeDef,
-        "platformVersion": str,
-        "platformFamily": str,
-        "pullStartedAt": datetime,
-        "pullStoppedAt": datetime,
-        "startedAt": datetime,
-        "startedBy": str,
-        "stopCode": TaskStopCodeType,
-        "stoppedAt": datetime,
-        "stoppedReason": str,
-        "stoppingAt": datetime,
-        "tags": List[TagTypeDef],
-        "taskArn": str,
-        "taskDefinitionArn": str,
-        "version": int,
-        "ephemeralStorage": EphemeralStorageTypeDef,
-    },
-    total=False,
-)
 
+TaskOverrideUnionTypeDef = Union[TaskOverrideTypeDef, TaskOverrideOutputTypeDef]
 DeregisterContainerInstanceResponseTypeDef = TypedDict(
     "DeregisterContainerInstanceResponseTypeDef",
     {
         "containerInstance": ContainerInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeContainerInstancesResponseTypeDef = TypedDict(
     "DescribeContainerInstancesResponseTypeDef",
     {
         "containerInstances": List[ContainerInstanceTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegisterContainerInstanceResponseTypeDef = TypedDict(
     "RegisterContainerInstanceResponseTypeDef",
     {
         "containerInstance": ContainerInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateContainerAgentResponseTypeDef = TypedDict(
     "UpdateContainerAgentResponseTypeDef",
     {
         "containerInstance": ContainerInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateContainerInstancesStateResponseTypeDef = TypedDict(
     "UpdateContainerInstancesStateResponseTypeDef",
     {
         "containerInstances": List[ContainerInstanceTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterTypeDef = TypedDict(
     "ClusterTypeDef",
     {
         "clusterArn": str,
@@ -2786,85 +3279,81 @@
         "settings": Sequence[ClusterSettingTypeDef],
         "configuration": ClusterConfigurationTypeDef,
         "serviceConnectDefaults": ClusterServiceConnectDefaultsRequestTypeDef,
     },
     total=False,
 )
 
+
 class UpdateClusterRequestRequestTypeDef(
     _RequiredUpdateClusterRequestRequestTypeDef, _OptionalUpdateClusterRequestRequestTypeDef
 ):
     pass
 
-_RequiredRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredRegisterTaskDefinitionRequestRequestTypeDef",
-    {
-        "family": str,
-        "containerDefinitions": Sequence[ContainerDefinitionTypeDef],
-    },
-)
-_OptionalRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalRegisterTaskDefinitionRequestRequestTypeDef",
-    {
-        "taskRoleArn": str,
-        "executionRoleArn": str,
-        "networkMode": NetworkModeType,
-        "volumes": Sequence[VolumeTypeDef],
-        "placementConstraints": Sequence[TaskDefinitionPlacementConstraintTypeDef],
-        "requiresCompatibilities": Sequence[CompatibilityType],
-        "cpu": str,
-        "memory": str,
-        "tags": Sequence[TagTypeDef],
-        "pidMode": PidModeType,
-        "ipcMode": IpcModeType,
-        "proxyConfiguration": ProxyConfigurationTypeDef,
-        "inferenceAccelerators": Sequence[InferenceAcceleratorTypeDef],
-        "ephemeralStorage": EphemeralStorageTypeDef,
-        "runtimePlatform": RuntimePlatformTypeDef,
-    },
-    total=False,
-)
-
-class RegisterTaskDefinitionRequestRequestTypeDef(
-    _RequiredRegisterTaskDefinitionRequestRequestTypeDef,
-    _OptionalRegisterTaskDefinitionRequestRequestTypeDef,
-):
-    pass
 
+VolumeUnionTypeDef = Union[VolumeTypeDef, VolumeOutputTypeDef]
 TaskDefinitionTypeDef = TypedDict(
     "TaskDefinitionTypeDef",
     {
         "taskDefinitionArn": str,
-        "containerDefinitions": List[ContainerDefinitionTypeDef],
+        "containerDefinitions": List[ContainerDefinitionOutputTypeDef],
         "family": str,
         "taskRoleArn": str,
         "executionRoleArn": str,
         "networkMode": NetworkModeType,
         "revision": int,
-        "volumes": List[VolumeTypeDef],
+        "volumes": List[VolumeOutputTypeDef],
         "status": TaskDefinitionStatusType,
         "requiresAttributes": List[AttributeTypeDef],
         "placementConstraints": List[TaskDefinitionPlacementConstraintTypeDef],
         "compatibilities": List[CompatibilityType],
         "runtimePlatform": RuntimePlatformTypeDef,
         "requiresCompatibilities": List[CompatibilityType],
         "cpu": str,
         "memory": str,
         "inferenceAccelerators": List[InferenceAcceleratorTypeDef],
         "pidMode": PidModeType,
         "ipcMode": IpcModeType,
-        "proxyConfiguration": ProxyConfigurationTypeDef,
+        "proxyConfiguration": ProxyConfigurationOutputTypeDef,
         "registeredAt": datetime,
         "deregisteredAt": datetime,
         "registeredBy": str,
         "ephemeralStorage": EphemeralStorageTypeDef,
     },
     total=False,
 )
 
+ContainerDefinitionUnionTypeDef = Union[
+    ContainerDefinitionTypeDef, ContainerDefinitionOutputTypeDef
+]
+DeploymentTypeDef = TypedDict(
+    "DeploymentTypeDef",
+    {
+        "id": str,
+        "status": str,
+        "taskDefinition": str,
+        "desiredCount": int,
+        "pendingCount": int,
+        "runningCount": int,
+        "failedTasks": int,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
+        "launchType": LaunchTypeType,
+        "platformVersion": str,
+        "platformFamily": str,
+        "networkConfiguration": NetworkConfigurationOutputTypeDef,
+        "rolloutState": DeploymentRolloutStateType,
+        "rolloutStateReason": str,
+        "serviceConnectConfiguration": ServiceConnectConfigurationOutputTypeDef,
+        "serviceConnectResources": List[ServiceConnectServiceResourceTypeDef],
+    },
+    total=False,
+)
+
 _RequiredCreateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceRequestRequestTypeDef",
     {
         "serviceName": str,
     },
 )
 _OptionalCreateServiceRequestRequestTypeDef = TypedDict(
@@ -2892,44 +3381,24 @@
         "propagateTags": PropagateTagsType,
         "enableExecuteCommand": bool,
         "serviceConnectConfiguration": ServiceConnectConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateServiceRequestRequestTypeDef(
     _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
 ):
     pass
 
-DeploymentTypeDef = TypedDict(
-    "DeploymentTypeDef",
-    {
-        "id": str,
-        "status": str,
-        "taskDefinition": str,
-        "desiredCount": int,
-        "pendingCount": int,
-        "runningCount": int,
-        "failedTasks": int,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
-        "launchType": LaunchTypeType,
-        "platformVersion": str,
-        "platformFamily": str,
-        "networkConfiguration": NetworkConfigurationTypeDef,
-        "rolloutState": DeploymentRolloutStateType,
-        "rolloutStateReason": str,
-        "serviceConnectConfiguration": ServiceConnectConfigurationTypeDef,
-        "serviceConnectResources": List[ServiceConnectServiceResourceTypeDef],
-    },
-    total=False,
-)
 
+ServiceConnectConfigurationUnionTypeDef = Union[
+    ServiceConnectConfigurationTypeDef, ServiceConnectConfigurationOutputTypeDef
+]
 _RequiredUpdateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceRequestRequestTypeDef",
     {
         "service": str,
     },
 )
 _OptionalUpdateServiceRequestRequestTypeDef = TypedDict(
@@ -2952,138 +3421,177 @@
         "propagateTags": PropagateTagsType,
         "serviceRegistries": Sequence[ServiceRegistryTypeDef],
         "serviceConnectConfiguration": ServiceConnectConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateServiceRequestRequestTypeDef(
     _RequiredUpdateServiceRequestRequestTypeDef, _OptionalUpdateServiceRequestRequestTypeDef
 ):
     pass
 
+
 DescribeTasksResponseTypeDef = TypedDict(
     "DescribeTasksResponseTypeDef",
     {
         "tasks": List[TaskTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RunTaskResponseTypeDef = TypedDict(
     "RunTaskResponseTypeDef",
     {
         "tasks": List[TaskTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartTaskResponseTypeDef = TypedDict(
     "StartTaskResponseTypeDef",
     {
         "tasks": List[TaskTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopTaskResponseTypeDef = TypedDict(
     "StopTaskResponseTypeDef",
     {
         "task": TaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterResponseTypeDef = TypedDict(
     "CreateClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteClusterResponseTypeDef = TypedDict(
     "DeleteClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeClustersResponseTypeDef = TypedDict(
     "DescribeClustersResponseTypeDef",
     {
         "clusters": List[ClusterTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutClusterCapacityProvidersResponseTypeDef = TypedDict(
     "PutClusterCapacityProvidersResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateClusterResponseTypeDef = TypedDict(
     "UpdateClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateClusterSettingsResponseTypeDef = TypedDict(
     "UpdateClusterSettingsResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteTaskDefinitionsResponseTypeDef = TypedDict(
     "DeleteTaskDefinitionsResponseTypeDef",
     {
         "taskDefinitions": List[TaskDefinitionTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeregisterTaskDefinitionResponseTypeDef = TypedDict(
     "DeregisterTaskDefinitionResponseTypeDef",
     {
         "taskDefinition": TaskDefinitionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTaskDefinitionResponseTypeDef = TypedDict(
     "DescribeTaskDefinitionResponseTypeDef",
     {
         "taskDefinition": TaskDefinitionTypeDef,
         "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegisterTaskDefinitionResponseTypeDef = TypedDict(
     "RegisterTaskDefinitionResponseTypeDef",
     {
         "taskDefinition": TaskDefinitionTypeDef,
         "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredRegisterTaskDefinitionRequestRequestTypeDef",
+    {
+        "family": str,
+        "containerDefinitions": Sequence[ContainerDefinitionUnionTypeDef],
+    },
+)
+_OptionalRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalRegisterTaskDefinitionRequestRequestTypeDef",
+    {
+        "taskRoleArn": str,
+        "executionRoleArn": str,
+        "networkMode": NetworkModeType,
+        "volumes": Sequence[VolumeUnionTypeDef],
+        "placementConstraints": Sequence[TaskDefinitionPlacementConstraintTypeDef],
+        "requiresCompatibilities": Sequence[CompatibilityType],
+        "cpu": str,
+        "memory": str,
+        "tags": Sequence[TagTypeDef],
+        "pidMode": PidModeType,
+        "ipcMode": IpcModeType,
+        "proxyConfiguration": ProxyConfigurationTypeDef,
+        "inferenceAccelerators": Sequence[InferenceAcceleratorTypeDef],
+        "ephemeralStorage": EphemeralStorageTypeDef,
+        "runtimePlatform": RuntimePlatformTypeDef,
+    },
+    total=False,
+)
+
+
+class RegisterTaskDefinitionRequestRequestTypeDef(
+    _RequiredRegisterTaskDefinitionRequestRequestTypeDef,
+    _OptionalRegisterTaskDefinitionRequestRequestTypeDef,
+):
+    pass
+
+
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "serviceArn": str,
         "serviceName": str,
         "clusterArn": str,
         "loadBalancers": List[LoadBalancerTypeDef],
@@ -3093,23 +3601,23 @@
         "runningCount": int,
         "pendingCount": int,
         "launchType": LaunchTypeType,
         "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
         "platformVersion": str,
         "platformFamily": str,
         "taskDefinition": str,
-        "deploymentConfiguration": DeploymentConfigurationTypeDef,
+        "deploymentConfiguration": DeploymentConfigurationOutputTypeDef,
         "taskSets": List[TaskSetTypeDef],
         "deployments": List[DeploymentTypeDef],
         "roleArn": str,
         "events": List[ServiceEventTypeDef],
         "createdAt": datetime,
         "placementConstraints": List[PlacementConstraintTypeDef],
         "placementStrategy": List[PlacementStrategyTypeDef],
-        "networkConfiguration": NetworkConfigurationTypeDef,
+        "networkConfiguration": NetworkConfigurationOutputTypeDef,
         "healthCheckGracePeriodSeconds": int,
         "schedulingStrategy": SchedulingStrategyType,
         "deploymentController": DeploymentControllerTypeDef,
         "tags": List[TagTypeDef],
         "createdBy": str,
         "enableECSManagedTags": bool,
         "propagateTags": PropagateTagsType,
@@ -3118,35 +3626,35 @@
     total=False,
 )
 
 CreateServiceResponseTypeDef = TypedDict(
     "CreateServiceResponseTypeDef",
     {
         "service": ServiceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteServiceResponseTypeDef = TypedDict(
     "DeleteServiceResponseTypeDef",
     {
         "service": ServiceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeServicesResponseTypeDef = TypedDict(
     "DescribeServicesResponseTypeDef",
     {
         "services": List[ServiceTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServiceResponseTypeDef = TypedDict(
     "UpdateServiceResponseTypeDef",
     {
         "service": ServiceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs/waiter.py` & `types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs/waiter.pyi` & `types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs.egg-info/PKG-INFO` & `types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ecs
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ECS 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ECS 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore ecs type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore ecs type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-ecs"></a>
 
 # types-aiobotocore-ecs
 
 [![PyPI - types-aiobotocore-ecs](https://img.shields.io/pypi/v/types-aiobotocore-ecs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ecs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ecs?color=blue)](https://pypistats.org/packages/types-aiobotocore-ecs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ecs)](https://pepy.tech/project/types-aiobotocore-ecs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ECS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
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
 [types-aiobotocore-ecs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/).
 
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
@@ -433,217 +432,245 @@
 )
 
 
 def check_value(value: AgentUpdateStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_ecs.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_ecs.type_defs import (
     AttachmentStateChangeTypeDef,
     KeyValuePairTypeDef,
     AttributeTypeDef,
     ManagedScalingTypeDef,
+    AwsVpcConfigurationOutputTypeDef,
     AwsVpcConfigurationTypeDef,
     CapacityProviderStrategyItemTypeDef,
     TagTypeDef,
     ClusterServiceConnectDefaultsRequestTypeDef,
     ClusterServiceConnectDefaultsTypeDef,
     ClusterSettingTypeDef,
     ContainerDependencyTypeDef,
     EnvironmentFileTypeDef,
-    FirelensConfigurationTypeDef,
-    HealthCheckTypeDef,
+    FirelensConfigurationOutputTypeDef,
+    HealthCheckOutputTypeDef,
     HostEntryTypeDef,
     MountPointTypeDef,
     PortMappingTypeDef,
     RepositoryCredentialsTypeDef,
     ResourceRequirementTypeDef,
     SecretTypeDef,
     SystemControlTypeDef,
     UlimitTypeDef,
     VolumeFromTypeDef,
+    FirelensConfigurationTypeDef,
+    HealthCheckTypeDef,
     InstanceHealthCheckResultTypeDef,
-    ResourceTypeDef,
+    ResourceOutputTypeDef,
     VersionInfoTypeDef,
     NetworkBindingTypeDef,
     ManagedAgentTypeDef,
     NetworkInterfaceTypeDef,
+    ResponseMetadataTypeDef,
     DeploymentControllerTypeDef,
     LoadBalancerTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     ServiceRegistryTypeDef,
     ScaleTypeDef,
     DeleteAccountSettingRequestRequestTypeDef,
     SettingTypeDef,
     DeleteCapacityProviderRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteServiceRequestRequestTypeDef,
     DeleteTaskDefinitionsRequestRequestTypeDef,
     FailureTypeDef,
     DeleteTaskSetRequestRequestTypeDef,
+    DeploymentAlarmsOutputTypeDef,
     DeploymentAlarmsTypeDef,
     DeploymentCircuitBreakerTypeDef,
     ServiceConnectServiceResourceTypeDef,
     DeregisterContainerInstanceRequestRequestTypeDef,
     DeregisterTaskDefinitionRequestRequestTypeDef,
     DescribeCapacityProvidersRequestRequestTypeDef,
     DescribeClustersRequestRequestTypeDef,
     DescribeContainerInstancesRequestRequestTypeDef,
     DescribeServicesRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTaskDefinitionRequestRequestTypeDef,
     DescribeTaskSetsRequestRequestTypeDef,
     DescribeTasksRequestRequestTypeDef,
+    DeviceOutputTypeDef,
     DeviceTypeDef,
     DiscoverPollEndpointRequestRequestTypeDef,
-    DiscoverPollEndpointResponseTypeDef,
+    DockerVolumeConfigurationOutputTypeDef,
     DockerVolumeConfigurationTypeDef,
     EFSAuthorizationConfigTypeDef,
     EphemeralStorageTypeDef,
     ExecuteCommandLogConfigurationTypeDef,
     ExecuteCommandRequestRequestTypeDef,
     SessionTypeDef,
     FSxWindowsFileServerAuthorizationConfigTypeDef,
     GetTaskProtectionRequestRequestTypeDef,
     ProtectedTaskTypeDef,
     HostVolumePropertiesTypeDef,
     InferenceAcceleratorOverrideTypeDef,
     InferenceAcceleratorTypeDef,
+    KernelCapabilitiesOutputTypeDef,
     KernelCapabilitiesTypeDef,
+    TmpfsOutputTypeDef,
     TmpfsTypeDef,
-    ListAccountSettingsRequestListAccountSettingsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccountSettingsRequestRequestTypeDef,
-    ListAttributesRequestListAttributesPaginateTypeDef,
     ListAttributesRequestRequestTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
-    ListClustersResponseTypeDef,
-    ListContainerInstancesRequestListContainerInstancesPaginateTypeDef,
     ListContainerInstancesRequestRequestTypeDef,
-    ListContainerInstancesResponseTypeDef,
-    ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
     ListServicesByNamespaceRequestRequestTypeDef,
-    ListServicesByNamespaceResponseTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
-    ListServicesResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef,
     ListTaskDefinitionFamiliesRequestRequestTypeDef,
-    ListTaskDefinitionFamiliesResponseTypeDef,
-    ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef,
     ListTaskDefinitionsRequestRequestTypeDef,
-    ListTaskDefinitionsResponseTypeDef,
-    ListTasksRequestListTasksPaginateTypeDef,
     ListTasksRequestRequestTypeDef,
-    ListTasksResponseTypeDef,
     ManagedAgentStateChangeTypeDef,
-    PaginatorConfigTypeDef,
     PlatformDeviceTypeDef,
     PutAccountSettingDefaultRequestRequestTypeDef,
     PutAccountSettingRequestRequestTypeDef,
     RuntimePlatformTypeDef,
     TaskDefinitionPlacementConstraintTypeDef,
-    ResponseMetadataTypeDef,
+    ResourceTypeDef,
     ServiceConnectClientAliasTypeDef,
     ServiceEventTypeDef,
     StopTaskRequestRequestTypeDef,
-    SubmitAttachmentStateChangesResponseTypeDef,
-    SubmitContainerStateChangeResponseTypeDef,
-    SubmitTaskStateChangeResponseTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateContainerAgentRequestRequestTypeDef,
     UpdateContainerInstancesStateRequestRequestTypeDef,
     UpdateServicePrimaryTaskSetRequestRequestTypeDef,
     UpdateTaskProtectionRequestRequestTypeDef,
     SubmitAttachmentStateChangesRequestRequestTypeDef,
     AttachmentTypeDef,
+    ProxyConfigurationOutputTypeDef,
     ProxyConfigurationTypeDef,
     DeleteAttributesRequestRequestTypeDef,
-    DeleteAttributesResponseTypeDef,
-    ListAttributesResponseTypeDef,
     PutAttributesRequestRequestTypeDef,
-    PutAttributesResponseTypeDef,
     AutoScalingGroupProviderTypeDef,
     AutoScalingGroupProviderUpdateTypeDef,
+    NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
     PutClusterCapacityProvidersRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UpdateClusterSettingsRequestRequestTypeDef,
+    ContainerOverrideOutputTypeDef,
     ContainerOverrideTypeDef,
+    LogConfigurationOutputTypeDef,
     LogConfigurationTypeDef,
     ContainerInstanceHealthStatusTypeDef,
     ContainerStateChangeTypeDef,
     SubmitContainerStateChangeRequestRequestTypeDef,
     ContainerTypeDef,
+    DeleteAttributesResponseTypeDef,
+    DiscoverPollEndpointResponseTypeDef,
+    ListAttributesResponseTypeDef,
+    ListClustersResponseTypeDef,
+    ListContainerInstancesResponseTypeDef,
+    ListServicesByNamespaceResponseTypeDef,
+    ListServicesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTaskDefinitionFamiliesResponseTypeDef,
+    ListTaskDefinitionsResponseTypeDef,
+    ListTasksResponseTypeDef,
+    PutAttributesResponseTypeDef,
+    SubmitAttachmentStateChangesResponseTypeDef,
+    SubmitContainerStateChangeResponseTypeDef,
+    SubmitTaskStateChangeResponseTypeDef,
     UpdateTaskSetRequestRequestTypeDef,
     DeleteAccountSettingResponseTypeDef,
     ListAccountSettingsResponseTypeDef,
     PutAccountSettingDefaultResponseTypeDef,
     PutAccountSettingResponseTypeDef,
+    DeploymentConfigurationOutputTypeDef,
     DeploymentConfigurationTypeDef,
     DescribeServicesRequestServicesInactiveWaitTypeDef,
     DescribeServicesRequestServicesStableWaitTypeDef,
     DescribeTasksRequestTasksRunningWaitTypeDef,
     DescribeTasksRequestTasksStoppedWaitTypeDef,
     EFSVolumeConfigurationTypeDef,
     ExecuteCommandConfigurationTypeDef,
     ExecuteCommandResponseTypeDef,
     FSxWindowsFileServerVolumeConfigurationTypeDef,
     GetTaskProtectionResponseTypeDef,
     UpdateTaskProtectionResponseTypeDef,
+    LinuxParametersOutputTypeDef,
     LinuxParametersTypeDef,
-    RegisterContainerInstanceRequestRequestTypeDef,
+    ListAccountSettingsRequestListAccountSettingsPaginateTypeDef,
+    ListAttributesRequestListAttributesPaginateTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
+    ListContainerInstancesRequestListContainerInstancesPaginateTypeDef,
+    ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
+    ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef,
+    ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef,
+    ListTasksRequestListTasksPaginateTypeDef,
+    ResourceUnionTypeDef,
+    ServiceConnectServiceOutputTypeDef,
     ServiceConnectServiceTypeDef,
+    ProxyConfigurationUnionTypeDef,
     CapacityProviderTypeDef,
     CreateCapacityProviderRequestRequestTypeDef,
     UpdateCapacityProviderRequestRequestTypeDef,
-    CreateTaskSetRequestRequestTypeDef,
     TaskSetTypeDef,
+    CreateTaskSetRequestRequestTypeDef,
+    NetworkConfigurationUnionTypeDef,
+    TaskOverrideOutputTypeDef,
     TaskOverrideTypeDef,
     ContainerInstanceTypeDef,
     SubmitTaskStateChangeRequestRequestTypeDef,
+    DeploymentConfigurationUnionTypeDef,
     ClusterConfigurationTypeDef,
+    VolumeOutputTypeDef,
     VolumeTypeDef,
+    ContainerDefinitionOutputTypeDef,
     ContainerDefinitionTypeDef,
+    RegisterContainerInstanceRequestRequestTypeDef,
+    ServiceConnectConfigurationOutputTypeDef,
     ServiceConnectConfigurationTypeDef,
     CreateCapacityProviderResponseTypeDef,
     DeleteCapacityProviderResponseTypeDef,
     DescribeCapacityProvidersResponseTypeDef,
     UpdateCapacityProviderResponseTypeDef,
     CreateTaskSetResponseTypeDef,
     DeleteTaskSetResponseTypeDef,
     DescribeTaskSetsResponseTypeDef,
     UpdateServicePrimaryTaskSetResponseTypeDef,
     UpdateTaskSetResponseTypeDef,
+    TaskTypeDef,
     RunTaskRequestRequestTypeDef,
     StartTaskRequestRequestTypeDef,
-    TaskTypeDef,
+    TaskOverrideUnionTypeDef,
     DeregisterContainerInstanceResponseTypeDef,
     DescribeContainerInstancesResponseTypeDef,
     RegisterContainerInstanceResponseTypeDef,
     UpdateContainerAgentResponseTypeDef,
     UpdateContainerInstancesStateResponseTypeDef,
     ClusterTypeDef,
     CreateClusterRequestRequestTypeDef,
     UpdateClusterRequestRequestTypeDef,
-    RegisterTaskDefinitionRequestRequestTypeDef,
+    VolumeUnionTypeDef,
     TaskDefinitionTypeDef,
-    CreateServiceRequestRequestTypeDef,
+    ContainerDefinitionUnionTypeDef,
     DeploymentTypeDef,
+    CreateServiceRequestRequestTypeDef,
+    ServiceConnectConfigurationUnionTypeDef,
     UpdateServiceRequestRequestTypeDef,
     DescribeTasksResponseTypeDef,
     RunTaskResponseTypeDef,
     StartTaskResponseTypeDef,
     StopTaskResponseTypeDef,
     CreateClusterResponseTypeDef,
     DeleteClusterResponseTypeDef,
@@ -651,23 +678,24 @@
     PutClusterCapacityProvidersResponseTypeDef,
     UpdateClusterResponseTypeDef,
     UpdateClusterSettingsResponseTypeDef,
     DeleteTaskDefinitionsResponseTypeDef,
     DeregisterTaskDefinitionResponseTypeDef,
     DescribeTaskDefinitionResponseTypeDef,
     RegisterTaskDefinitionResponseTypeDef,
+    RegisterTaskDefinitionRequestRequestTypeDef,
     ServiceTypeDef,
     CreateServiceResponseTypeDef,
     DeleteServiceResponseTypeDef,
     DescribeServicesResponseTypeDef,
     UpdateServiceResponseTypeDef,
 )
 
 
-def get_structure() -> AttachmentStateChangeTypeDef:
+def get_value() -> AttachmentStateChangeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-ecs-2.5.2/types_aiobotocore_ecs.egg-info/SOURCES.txt` & `types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs.egg-info/SOURCES.txt`

 * *Files identical despite different names*


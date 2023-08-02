# Comparing `tmp/types-aiobotocore-panorama-2.5.2.tar.gz` & `tmp/types-aiobotocore-panorama-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-panorama-2.5.2.tar", last modified: Sat Jul  8 01:44:05 2023, max compression
+gzip compressed data, was "types-aiobotocore-panorama-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:45 2023, max compression
```

## Comparing `types-aiobotocore-panorama-2.5.2.tar` & `types-aiobotocore-panorama-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:05.126647 types-aiobotocore-panorama-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:36:16.000000 types-aiobotocore-panorama-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16642 2023-07-08 01:44:05.126647 types-aiobotocore-panorama-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15073 2023-07-08 01:36:16.000000 types-aiobotocore-panorama-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:05.126647 types-aiobotocore-panorama-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-08 01:36:16.000000 types-aiobotocore-panorama-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:05.122647 types-aiobotocore-panorama-2.5.2/types_aiobotocore_panorama/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-08 01:36:16.000000 types-aiobotocore-panorama-2.5.2/types_aiobotocore_panorama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-08 01:36:16.000000 types-aiobotocore-panorama-2.5.2/types_aiobotocore_panorama/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-08 01:36:16.000000 types-aiobotocore-panorama-2.5.2/types_aiobotocore_panorama/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25607 2023-07-08 01:36:17.000000 types-aiobotocore-panorama-2.5.2/types_aiobotocore_panorama/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25564 2023-07-08 01:36:17.000000 types-aiobotocore-panorama-2.5.2/types_aiobotocore_panorama/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-07-08 01:36:17.000000 types-aiobotocore-panorama-2.5.2/types_aiobotocore_panorama/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-07-08 01:36:17.000000 types-aiobotocore-panorama-2.5.2/types_aiobotocore_panorama/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:36:16.000000 types-aiobotocore-panorama-2.5.2/types_aiobotocore_panorama/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37374 2023-07-08 01:36:18.000000 types-aiobotocore-panorama-2.5.2/types_aiobotocore_panorama/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    37333 2023-07-08 01:36:17.000000 types-aiobotocore-panorama-2.5.2/types_aiobotocore_panorama/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:36:16.000000 types-aiobotocore-panorama-2.5.2/types_aiobotocore_panorama/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:05.126647 types-aiobotocore-panorama-2.5.2/types_aiobotocore_panorama.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16642 2023-07-08 01:44:04.000000 types-aiobotocore-panorama-2.5.2/types_aiobotocore_panorama.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-08 01:44:04.000000 types-aiobotocore-panorama-2.5.2/types_aiobotocore_panorama.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:04.000000 types-aiobotocore-panorama-2.5.2/types_aiobotocore_panorama.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:04.000000 types-aiobotocore-panorama-2.5.2/types_aiobotocore_panorama.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:04.000000 types-aiobotocore-panorama-2.5.2/types_aiobotocore_panorama.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-08 01:44:04.000000 types-aiobotocore-panorama-2.5.2/types_aiobotocore_panorama.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:45.853503 types-aiobotocore-panorama-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:44:35.000000 types-aiobotocore-panorama-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-08-02 14:52:45.853503 types-aiobotocore-panorama-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-08-02 14:44:35.000000 types-aiobotocore-panorama-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:45.853503 types-aiobotocore-panorama-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:44:35.000000 types-aiobotocore-panorama-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:45.849503 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-02 14:44:35.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-02 14:44:35.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:44:35.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25632 2023-08-02 14:44:35.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25589 2023-08-02 14:44:35.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-08-02 14:44:35.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-08-02 14:44:35.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:44:35.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39025 2023-08-02 14:44:36.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38982 2023-08-02 14:44:36.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:44:35.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:45.853503 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-08-02 14:52:45.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-02 14:52:45.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:45.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:45.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:45.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:52:45.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-panorama-2.5.2/LICENSE` & `types-aiobotocore-panorama-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-panorama-2.5.2/PKG-INFO` & `types-aiobotocore-panorama-2.5.2.post1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-panorama
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Panorama 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Panorama 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore panorama type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore panorama type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-panorama"></a>
 
 # types-aiobotocore-panorama
 
 [![PyPI - types-aiobotocore-panorama](https://img.shields.io/pypi/v/types-aiobotocore-panorama.svg?color=blue)](https://pypi.org/project/types-aiobotocore-panorama)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-panorama.svg?color=blue)](https://pypi.org/project/types-aiobotocore-panorama)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-panorama?color=blue)](https://pypistats.org/packages/types-aiobotocore-panorama)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-panorama)](https://pepy.tech/project/types-aiobotocore-panorama)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Panorama 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
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
 [types-aiobotocore-panorama docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/).
 
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
@@ -304,54 +303,51 @@
 )
 
 
 def check_value(value: ApplicationInstanceHealthStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_panorama.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_panorama.type_defs import (
     AlternateSoftwareMetadataTypeDef,
     ReportedRuntimeContextStateTypeDef,
     ManifestOverridesPayloadTypeDef,
     ManifestPayloadTypeDef,
-    CreateApplicationInstanceResponseTypeDef,
+    ResponseMetadataTypeDef,
     JobTypeDef,
-    JobResourceTagsTypeDef,
-    CreateNodeFromTemplateJobResponseTypeDef,
-    CreatePackageImportJobResponseTypeDef,
     CreatePackageRequestRequestTypeDef,
     StorageLocationTypeDef,
     DeleteDeviceRequestRequestTypeDef,
-    DeleteDeviceResponseTypeDef,
     DeletePackageRequestRequestTypeDef,
     DeregisterPackageVersionRequestRequestTypeDef,
     DescribeApplicationInstanceDetailsRequestRequestTypeDef,
     DescribeApplicationInstanceRequestRequestTypeDef,
     DescribeDeviceJobRequestRequestTypeDef,
-    DescribeDeviceJobResponseTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     LatestDeviceJobTypeDef,
     DescribeNodeFromTemplateJobRequestRequestTypeDef,
+    JobResourceTagsOutputTypeDef,
     DescribeNodeRequestRequestTypeDef,
     DescribePackageImportJobRequestRequestTypeDef,
     DescribePackageRequestRequestTypeDef,
     DescribePackageVersionRequestRequestTypeDef,
-    DescribePackageVersionResponseTypeDef,
     OTAJobConfigTypeDef,
     DeviceJobTypeDef,
+    StaticIpConnectionInfoOutputTypeDef,
     StaticIpConnectionInfoTypeDef,
     EthernetStatusTypeDef,
+    JobResourceTagsTypeDef,
     ListApplicationInstanceDependenciesRequestRequestTypeDef,
     PackageObjectTypeDef,
     ListApplicationInstanceNodeInstancesRequestRequestTypeDef,
     NodeInstanceTypeDef,
     ListApplicationInstancesRequestRequestTypeDef,
     ListDevicesJobsRequestRequestTypeDef,
     ListDevicesRequestRequestTypeDef,
@@ -360,45 +356,52 @@
     ListNodesRequestRequestTypeDef,
     NodeTypeDef,
     ListPackageImportJobsRequestRequestTypeDef,
     PackageImportJobTypeDef,
     ListPackagesRequestRequestTypeDef,
     PackageListItemTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    NtpPayloadOutputTypeDef,
     NtpPayloadTypeDef,
     NtpStatusTypeDef,
     NodeInputPortTypeDef,
     NodeOutputPortTypeDef,
     NodeSignalTypeDef,
     OutPutS3LocationTypeDef,
     PackageVersionOutputConfigTypeDef,
     S3LocationTypeDef,
-    ProvisionDeviceResponseTypeDef,
     RegisterPackageVersionRequestRequestTypeDef,
     RemoveApplicationInstanceRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    SignalApplicationInstanceNodeInstancesResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceMetadataRequestRequestTypeDef,
-    UpdateDeviceMetadataResponseTypeDef,
     ApplicationInstanceTypeDef,
-    DescribeApplicationInstanceResponseTypeDef,
     CreateApplicationInstanceRequestRequestTypeDef,
+    CreateApplicationInstanceResponseTypeDef,
+    CreateNodeFromTemplateJobResponseTypeDef,
+    CreatePackageImportJobResponseTypeDef,
+    DeleteDeviceResponseTypeDef,
     DescribeApplicationInstanceDetailsResponseTypeDef,
+    DescribeApplicationInstanceResponseTypeDef,
+    DescribeDeviceJobResponseTypeDef,
+    DescribePackageVersionResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ProvisionDeviceResponseTypeDef,
+    SignalApplicationInstanceNodeInstancesResponseTypeDef,
+    UpdateDeviceMetadataResponseTypeDef,
     CreateJobForDevicesResponseTypeDef,
-    CreateNodeFromTemplateJobRequestRequestTypeDef,
-    DescribeNodeFromTemplateJobResponseTypeDef,
     CreatePackageResponseTypeDef,
     DescribePackageResponseTypeDef,
     DeviceTypeDef,
+    DescribeNodeFromTemplateJobResponseTypeDef,
     DeviceJobConfigTypeDef,
     ListDevicesJobsResponseTypeDef,
+    EthernetPayloadOutputTypeDef,
     EthernetPayloadTypeDef,
+    JobResourceTagsUnionTypeDef,
     ListApplicationInstanceDependenciesResponseTypeDef,
     ListApplicationInstanceNodeInstancesResponseTypeDef,
     ListNodeFromTemplateJobsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListPackageImportJobsResponseTypeDef,
     ListPackagesResponseTypeDef,
     NetworkStatusTypeDef,
@@ -406,25 +409,28 @@
     SignalApplicationInstanceNodeInstancesRequestRequestTypeDef,
     PackageImportJobOutputTypeDef,
     PackageImportJobOutputConfigTypeDef,
     PackageVersionInputConfigTypeDef,
     ListApplicationInstancesResponseTypeDef,
     ListDevicesResponseTypeDef,
     CreateJobForDevicesRequestRequestTypeDef,
+    NetworkPayloadOutputTypeDef,
     NetworkPayloadTypeDef,
+    CreateNodeFromTemplateJobRequestRequestTypeDef,
     DescribeNodeResponseTypeDef,
     PackageImportJobInputConfigTypeDef,
     DescribeDeviceResponseTypeDef,
+    NetworkPayloadUnionTypeDef,
     ProvisionDeviceRequestRequestTypeDef,
     CreatePackageImportJobRequestRequestTypeDef,
     DescribePackageImportJobResponseTypeDef,
 )
 
 
-def get_structure() -> AlternateSoftwareMetadataTypeDef:
+def get_value() -> AlternateSoftwareMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-panorama-2.5.2/README.md` & `types-aiobotocore-panorama-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-panorama"></a>
 
 # types-aiobotocore-panorama
 
 [![PyPI - types-aiobotocore-panorama](https://img.shields.io/pypi/v/types-aiobotocore-panorama.svg?color=blue)](https://pypi.org/project/types-aiobotocore-panorama)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-panorama.svg?color=blue)](https://pypi.org/project/types-aiobotocore-panorama)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-panorama?color=blue)](https://pypistats.org/packages/types-aiobotocore-panorama)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-panorama)](https://pepy.tech/project/types-aiobotocore-panorama)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Panorama 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
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
 [types-aiobotocore-panorama docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/).
 
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
@@ -271,54 +271,51 @@
 )
 
 
 def check_value(value: ApplicationInstanceHealthStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_panorama.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_panorama.type_defs import (
     AlternateSoftwareMetadataTypeDef,
     ReportedRuntimeContextStateTypeDef,
     ManifestOverridesPayloadTypeDef,
     ManifestPayloadTypeDef,
-    CreateApplicationInstanceResponseTypeDef,
+    ResponseMetadataTypeDef,
     JobTypeDef,
-    JobResourceTagsTypeDef,
-    CreateNodeFromTemplateJobResponseTypeDef,
-    CreatePackageImportJobResponseTypeDef,
     CreatePackageRequestRequestTypeDef,
     StorageLocationTypeDef,
     DeleteDeviceRequestRequestTypeDef,
-    DeleteDeviceResponseTypeDef,
     DeletePackageRequestRequestTypeDef,
     DeregisterPackageVersionRequestRequestTypeDef,
     DescribeApplicationInstanceDetailsRequestRequestTypeDef,
     DescribeApplicationInstanceRequestRequestTypeDef,
     DescribeDeviceJobRequestRequestTypeDef,
-    DescribeDeviceJobResponseTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     LatestDeviceJobTypeDef,
     DescribeNodeFromTemplateJobRequestRequestTypeDef,
+    JobResourceTagsOutputTypeDef,
     DescribeNodeRequestRequestTypeDef,
     DescribePackageImportJobRequestRequestTypeDef,
     DescribePackageRequestRequestTypeDef,
     DescribePackageVersionRequestRequestTypeDef,
-    DescribePackageVersionResponseTypeDef,
     OTAJobConfigTypeDef,
     DeviceJobTypeDef,
+    StaticIpConnectionInfoOutputTypeDef,
     StaticIpConnectionInfoTypeDef,
     EthernetStatusTypeDef,
+    JobResourceTagsTypeDef,
     ListApplicationInstanceDependenciesRequestRequestTypeDef,
     PackageObjectTypeDef,
     ListApplicationInstanceNodeInstancesRequestRequestTypeDef,
     NodeInstanceTypeDef,
     ListApplicationInstancesRequestRequestTypeDef,
     ListDevicesJobsRequestRequestTypeDef,
     ListDevicesRequestRequestTypeDef,
@@ -327,45 +324,52 @@
     ListNodesRequestRequestTypeDef,
     NodeTypeDef,
     ListPackageImportJobsRequestRequestTypeDef,
     PackageImportJobTypeDef,
     ListPackagesRequestRequestTypeDef,
     PackageListItemTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    NtpPayloadOutputTypeDef,
     NtpPayloadTypeDef,
     NtpStatusTypeDef,
     NodeInputPortTypeDef,
     NodeOutputPortTypeDef,
     NodeSignalTypeDef,
     OutPutS3LocationTypeDef,
     PackageVersionOutputConfigTypeDef,
     S3LocationTypeDef,
-    ProvisionDeviceResponseTypeDef,
     RegisterPackageVersionRequestRequestTypeDef,
     RemoveApplicationInstanceRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    SignalApplicationInstanceNodeInstancesResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceMetadataRequestRequestTypeDef,
-    UpdateDeviceMetadataResponseTypeDef,
     ApplicationInstanceTypeDef,
-    DescribeApplicationInstanceResponseTypeDef,
     CreateApplicationInstanceRequestRequestTypeDef,
+    CreateApplicationInstanceResponseTypeDef,
+    CreateNodeFromTemplateJobResponseTypeDef,
+    CreatePackageImportJobResponseTypeDef,
+    DeleteDeviceResponseTypeDef,
     DescribeApplicationInstanceDetailsResponseTypeDef,
+    DescribeApplicationInstanceResponseTypeDef,
+    DescribeDeviceJobResponseTypeDef,
+    DescribePackageVersionResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ProvisionDeviceResponseTypeDef,
+    SignalApplicationInstanceNodeInstancesResponseTypeDef,
+    UpdateDeviceMetadataResponseTypeDef,
     CreateJobForDevicesResponseTypeDef,
-    CreateNodeFromTemplateJobRequestRequestTypeDef,
-    DescribeNodeFromTemplateJobResponseTypeDef,
     CreatePackageResponseTypeDef,
     DescribePackageResponseTypeDef,
     DeviceTypeDef,
+    DescribeNodeFromTemplateJobResponseTypeDef,
     DeviceJobConfigTypeDef,
     ListDevicesJobsResponseTypeDef,
+    EthernetPayloadOutputTypeDef,
     EthernetPayloadTypeDef,
+    JobResourceTagsUnionTypeDef,
     ListApplicationInstanceDependenciesResponseTypeDef,
     ListApplicationInstanceNodeInstancesResponseTypeDef,
     ListNodeFromTemplateJobsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListPackageImportJobsResponseTypeDef,
     ListPackagesResponseTypeDef,
     NetworkStatusTypeDef,
@@ -373,25 +377,28 @@
     SignalApplicationInstanceNodeInstancesRequestRequestTypeDef,
     PackageImportJobOutputTypeDef,
     PackageImportJobOutputConfigTypeDef,
     PackageVersionInputConfigTypeDef,
     ListApplicationInstancesResponseTypeDef,
     ListDevicesResponseTypeDef,
     CreateJobForDevicesRequestRequestTypeDef,
+    NetworkPayloadOutputTypeDef,
     NetworkPayloadTypeDef,
+    CreateNodeFromTemplateJobRequestRequestTypeDef,
     DescribeNodeResponseTypeDef,
     PackageImportJobInputConfigTypeDef,
     DescribeDeviceResponseTypeDef,
+    NetworkPayloadUnionTypeDef,
     ProvisionDeviceRequestRequestTypeDef,
     CreatePackageImportJobRequestRequestTypeDef,
     DescribePackageImportJobResponseTypeDef,
 )
 
 
-def get_structure() -> AlternateSoftwareMetadataTypeDef:
+def get_value() -> AlternateSoftwareMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-panorama-2.5.2/setup.py` & `types-aiobotocore-panorama-2.5.2.post1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-panorama",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_panorama"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Panorama 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore panorama type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore panorama type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_panorama": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/"
```

### Comparing `types-aiobotocore-panorama-2.5.2/types_aiobotocore_panorama/__main__.py` & `types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Panorama 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Panorama 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama\nOther"
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

### Comparing `types-aiobotocore-panorama-2.5.2/types_aiobotocore_panorama/client.py` & `types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,28 +42,28 @@
     DescribeDeviceResponseTypeDef,
     DescribeNodeFromTemplateJobResponseTypeDef,
     DescribeNodeResponseTypeDef,
     DescribePackageImportJobResponseTypeDef,
     DescribePackageResponseTypeDef,
     DescribePackageVersionResponseTypeDef,
     DeviceJobConfigTypeDef,
-    JobResourceTagsTypeDef,
+    JobResourceTagsUnionTypeDef,
     ListApplicationInstanceDependenciesResponseTypeDef,
     ListApplicationInstanceNodeInstancesResponseTypeDef,
     ListApplicationInstancesResponseTypeDef,
     ListDevicesJobsResponseTypeDef,
     ListDevicesResponseTypeDef,
     ListNodeFromTemplateJobsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListPackageImportJobsResponseTypeDef,
     ListPackagesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ManifestOverridesPayloadTypeDef,
     ManifestPayloadTypeDef,
-    NetworkPayloadTypeDef,
+    NetworkPayloadUnionTypeDef,
     NodeSignalTypeDef,
     PackageImportJobInputConfigTypeDef,
     PackageImportJobOutputConfigTypeDef,
     ProvisionDeviceResponseTypeDef,
     SignalApplicationInstanceNodeInstancesResponseTypeDef,
     UpdateDeviceMetadataResponseTypeDef,
 )
@@ -165,15 +165,15 @@
         self,
         *,
         NodeName: str,
         OutputPackageName: str,
         OutputPackageVersion: str,
         TemplateParameters: Mapping[str, str],
         TemplateType: Literal["RTSP_CAMERA_STREAM"],
-        JobTags: Sequence[JobResourceTagsTypeDef] = ...,
+        JobTags: Sequence[JobResourceTagsUnionTypeDef] = ...,
         NodeDescription: str = ...
     ) -> CreateNodeFromTemplateJobResponseTypeDef:
         """
         Creates a camera stream node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_node_from_template_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#create_node_from_template_job)
@@ -192,15 +192,15 @@
     async def create_package_import_job(
         self,
         *,
         ClientToken: str,
         InputConfig: PackageImportJobInputConfigTypeDef,
         JobType: PackageImportJobTypeType,
         OutputConfig: PackageImportJobOutputConfigTypeDef,
-        JobTags: Sequence[JobResourceTagsTypeDef] = ...
+        JobTags: Sequence[JobResourceTagsUnionTypeDef] = ...
     ) -> CreatePackageImportJobResponseTypeDef:
         """
         Imports a node package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_package_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#create_package_import_job)
         """
@@ -461,15 +461,15 @@
         """
 
     async def provision_device(
         self,
         *,
         Name: str,
         Description: str = ...,
-        NetworkingConfiguration: NetworkPayloadTypeDef = ...,
+        NetworkingConfiguration: NetworkPayloadUnionTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> ProvisionDeviceResponseTypeDef:
         """
         Creates a device and returns a configuration archive.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.provision_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#provision_device)
```

### Comparing `types-aiobotocore-panorama-2.5.2/types_aiobotocore_panorama/client.pyi` & `types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -42,28 +42,28 @@
     DescribeDeviceResponseTypeDef,
     DescribeNodeFromTemplateJobResponseTypeDef,
     DescribeNodeResponseTypeDef,
     DescribePackageImportJobResponseTypeDef,
     DescribePackageResponseTypeDef,
     DescribePackageVersionResponseTypeDef,
     DeviceJobConfigTypeDef,
-    JobResourceTagsTypeDef,
+    JobResourceTagsUnionTypeDef,
     ListApplicationInstanceDependenciesResponseTypeDef,
     ListApplicationInstanceNodeInstancesResponseTypeDef,
     ListApplicationInstancesResponseTypeDef,
     ListDevicesJobsResponseTypeDef,
     ListDevicesResponseTypeDef,
     ListNodeFromTemplateJobsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListPackageImportJobsResponseTypeDef,
     ListPackagesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ManifestOverridesPayloadTypeDef,
     ManifestPayloadTypeDef,
-    NetworkPayloadTypeDef,
+    NetworkPayloadUnionTypeDef,
     NodeSignalTypeDef,
     PackageImportJobInputConfigTypeDef,
     PackageImportJobOutputConfigTypeDef,
     ProvisionDeviceResponseTypeDef,
     SignalApplicationInstanceNodeInstancesResponseTypeDef,
     UpdateDeviceMetadataResponseTypeDef,
 )
@@ -156,15 +156,15 @@
         self,
         *,
         NodeName: str,
         OutputPackageName: str,
         OutputPackageVersion: str,
         TemplateParameters: Mapping[str, str],
         TemplateType: Literal["RTSP_CAMERA_STREAM"],
-        JobTags: Sequence[JobResourceTagsTypeDef] = ...,
+        JobTags: Sequence[JobResourceTagsUnionTypeDef] = ...,
         NodeDescription: str = ...
     ) -> CreateNodeFromTemplateJobResponseTypeDef:
         """
         Creates a camera stream node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_node_from_template_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#create_node_from_template_job)
@@ -181,15 +181,15 @@
     async def create_package_import_job(
         self,
         *,
         ClientToken: str,
         InputConfig: PackageImportJobInputConfigTypeDef,
         JobType: PackageImportJobTypeType,
         OutputConfig: PackageImportJobOutputConfigTypeDef,
-        JobTags: Sequence[JobResourceTagsTypeDef] = ...
+        JobTags: Sequence[JobResourceTagsUnionTypeDef] = ...
     ) -> CreatePackageImportJobResponseTypeDef:
         """
         Imports a node package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_package_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#create_package_import_job)
         """
@@ -426,15 +426,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#list_tags_for_resource)
         """
     async def provision_device(
         self,
         *,
         Name: str,
         Description: str = ...,
-        NetworkingConfiguration: NetworkPayloadTypeDef = ...,
+        NetworkingConfiguration: NetworkPayloadUnionTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> ProvisionDeviceResponseTypeDef:
         """
         Creates a device and returns a configuration archive.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.provision_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#provision_device)
```

### Comparing `types-aiobotocore-panorama-2.5.2/types_aiobotocore_panorama/literals.py` & `types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-panorama-2.5.2/types_aiobotocore_panorama/literals.pyi` & `types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-panorama-2.5.2/types_aiobotocore_panorama/type_defs.py` & `types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_panorama.type_defs import AlternateSoftwareMetadataTypeDef
 
-    data: AlternateSoftwareMetadataTypeDef = {...}
+    data: AlternateSoftwareMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ApplicationInstanceHealthStatusType,
     ApplicationInstanceStatusType,
     ConnectionTypeType,
     DesiredStateType,
     DeviceAggregatedStatusType,
@@ -53,41 +53,38 @@
 
 
 __all__ = (
     "AlternateSoftwareMetadataTypeDef",
     "ReportedRuntimeContextStateTypeDef",
     "ManifestOverridesPayloadTypeDef",
     "ManifestPayloadTypeDef",
-    "CreateApplicationInstanceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "JobTypeDef",
-    "JobResourceTagsTypeDef",
-    "CreateNodeFromTemplateJobResponseTypeDef",
-    "CreatePackageImportJobResponseTypeDef",
     "CreatePackageRequestRequestTypeDef",
     "StorageLocationTypeDef",
     "DeleteDeviceRequestRequestTypeDef",
-    "DeleteDeviceResponseTypeDef",
     "DeletePackageRequestRequestTypeDef",
     "DeregisterPackageVersionRequestRequestTypeDef",
     "DescribeApplicationInstanceDetailsRequestRequestTypeDef",
     "DescribeApplicationInstanceRequestRequestTypeDef",
     "DescribeDeviceJobRequestRequestTypeDef",
-    "DescribeDeviceJobResponseTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
     "LatestDeviceJobTypeDef",
     "DescribeNodeFromTemplateJobRequestRequestTypeDef",
+    "JobResourceTagsOutputTypeDef",
     "DescribeNodeRequestRequestTypeDef",
     "DescribePackageImportJobRequestRequestTypeDef",
     "DescribePackageRequestRequestTypeDef",
     "DescribePackageVersionRequestRequestTypeDef",
-    "DescribePackageVersionResponseTypeDef",
     "OTAJobConfigTypeDef",
     "DeviceJobTypeDef",
+    "StaticIpConnectionInfoOutputTypeDef",
     "StaticIpConnectionInfoTypeDef",
     "EthernetStatusTypeDef",
+    "JobResourceTagsTypeDef",
     "ListApplicationInstanceDependenciesRequestRequestTypeDef",
     "PackageObjectTypeDef",
     "ListApplicationInstanceNodeInstancesRequestRequestTypeDef",
     "NodeInstanceTypeDef",
     "ListApplicationInstancesRequestRequestTypeDef",
     "ListDevicesJobsRequestRequestTypeDef",
     "ListDevicesRequestRequestTypeDef",
@@ -96,45 +93,52 @@
     "ListNodesRequestRequestTypeDef",
     "NodeTypeDef",
     "ListPackageImportJobsRequestRequestTypeDef",
     "PackageImportJobTypeDef",
     "ListPackagesRequestRequestTypeDef",
     "PackageListItemTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "NtpPayloadOutputTypeDef",
     "NtpPayloadTypeDef",
     "NtpStatusTypeDef",
     "NodeInputPortTypeDef",
     "NodeOutputPortTypeDef",
     "NodeSignalTypeDef",
     "OutPutS3LocationTypeDef",
     "PackageVersionOutputConfigTypeDef",
     "S3LocationTypeDef",
-    "ProvisionDeviceResponseTypeDef",
     "RegisterPackageVersionRequestRequestTypeDef",
     "RemoveApplicationInstanceRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "SignalApplicationInstanceNodeInstancesResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeviceMetadataRequestRequestTypeDef",
-    "UpdateDeviceMetadataResponseTypeDef",
     "ApplicationInstanceTypeDef",
-    "DescribeApplicationInstanceResponseTypeDef",
     "CreateApplicationInstanceRequestRequestTypeDef",
+    "CreateApplicationInstanceResponseTypeDef",
+    "CreateNodeFromTemplateJobResponseTypeDef",
+    "CreatePackageImportJobResponseTypeDef",
+    "DeleteDeviceResponseTypeDef",
     "DescribeApplicationInstanceDetailsResponseTypeDef",
+    "DescribeApplicationInstanceResponseTypeDef",
+    "DescribeDeviceJobResponseTypeDef",
+    "DescribePackageVersionResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ProvisionDeviceResponseTypeDef",
+    "SignalApplicationInstanceNodeInstancesResponseTypeDef",
+    "UpdateDeviceMetadataResponseTypeDef",
     "CreateJobForDevicesResponseTypeDef",
-    "CreateNodeFromTemplateJobRequestRequestTypeDef",
-    "DescribeNodeFromTemplateJobResponseTypeDef",
     "CreatePackageResponseTypeDef",
     "DescribePackageResponseTypeDef",
     "DeviceTypeDef",
+    "DescribeNodeFromTemplateJobResponseTypeDef",
     "DeviceJobConfigTypeDef",
     "ListDevicesJobsResponseTypeDef",
+    "EthernetPayloadOutputTypeDef",
     "EthernetPayloadTypeDef",
+    "JobResourceTagsUnionTypeDef",
     "ListApplicationInstanceDependenciesResponseTypeDef",
     "ListApplicationInstanceNodeInstancesResponseTypeDef",
     "ListNodeFromTemplateJobsResponseTypeDef",
     "ListNodesResponseTypeDef",
     "ListPackageImportJobsResponseTypeDef",
     "ListPackagesResponseTypeDef",
     "NetworkStatusTypeDef",
@@ -142,18 +146,21 @@
     "SignalApplicationInstanceNodeInstancesRequestRequestTypeDef",
     "PackageImportJobOutputTypeDef",
     "PackageImportJobOutputConfigTypeDef",
     "PackageVersionInputConfigTypeDef",
     "ListApplicationInstancesResponseTypeDef",
     "ListDevicesResponseTypeDef",
     "CreateJobForDevicesRequestRequestTypeDef",
+    "NetworkPayloadOutputTypeDef",
     "NetworkPayloadTypeDef",
+    "CreateNodeFromTemplateJobRequestRequestTypeDef",
     "DescribeNodeResponseTypeDef",
     "PackageImportJobInputConfigTypeDef",
     "DescribeDeviceResponseTypeDef",
+    "NetworkPayloadUnionTypeDef",
     "ProvisionDeviceRequestRequestTypeDef",
     "CreatePackageImportJobRequestRequestTypeDef",
     "DescribePackageImportJobResponseTypeDef",
 )
 
 AlternateSoftwareMetadataTypeDef = TypedDict(
     "AlternateSoftwareMetadataTypeDef",
@@ -185,55 +192,34 @@
     "ManifestPayloadTypeDef",
     {
         "PayloadData": str,
     },
     total=False,
 )
 
-CreateApplicationInstanceResponseTypeDef = TypedDict(
-    "CreateApplicationInstanceResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ApplicationInstanceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
         "DeviceId": str,
         "JobId": str,
     },
     total=False,
 )
 
-JobResourceTagsTypeDef = TypedDict(
-    "JobResourceTagsTypeDef",
-    {
-        "ResourceType": Literal["PACKAGE"],
-        "Tags": Mapping[str, str],
-    },
-)
-
-CreateNodeFromTemplateJobResponseTypeDef = TypedDict(
-    "CreateNodeFromTemplateJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePackageImportJobResponseTypeDef = TypedDict(
-    "CreatePackageImportJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePackageRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackageRequestRequestTypeDef",
     {
         "PackageName": str,
     },
 )
 _OptionalCreatePackageRequestRequestTypeDef = TypedDict(
@@ -265,22 +251,14 @@
 DeleteDeviceRequestRequestTypeDef = TypedDict(
     "DeleteDeviceRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 
-DeleteDeviceResponseTypeDef = TypedDict(
-    "DeleteDeviceResponseTypeDef",
-    {
-        "DeviceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeletePackageRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePackageRequestRequestTypeDef",
     {
         "PackageId": str,
     },
 )
 _OptionalDeletePackageRequestRequestTypeDef = TypedDict(
@@ -340,30 +318,14 @@
 DescribeDeviceJobRequestRequestTypeDef = TypedDict(
     "DescribeDeviceJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-DescribeDeviceJobResponseTypeDef = TypedDict(
-    "DescribeDeviceJobResponseTypeDef",
-    {
-        "CreatedTime": datetime,
-        "DeviceArn": str,
-        "DeviceId": str,
-        "DeviceName": str,
-        "DeviceType": DeviceTypeType,
-        "ImageVersion": str,
-        "JobId": str,
-        "JobType": JobTypeType,
-        "Status": UpdateProgressType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDeviceRequestRequestTypeDef = TypedDict(
     "DescribeDeviceRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 
@@ -380,14 +342,22 @@
 DescribeNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
     "DescribeNodeFromTemplateJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+JobResourceTagsOutputTypeDef = TypedDict(
+    "JobResourceTagsOutputTypeDef",
+    {
+        "ResourceType": Literal["PACKAGE"],
+        "Tags": Dict[str, str],
+    },
+)
+
 _RequiredDescribeNodeRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeNodeRequestRequestTypeDef",
     {
         "NodeId": str,
     },
 )
 _OptionalDescribeNodeRequestRequestTypeDef = TypedDict(
@@ -439,31 +409,14 @@
 class DescribePackageVersionRequestRequestTypeDef(
     _RequiredDescribePackageVersionRequestRequestTypeDef,
     _OptionalDescribePackageVersionRequestRequestTypeDef,
 ):
     pass
 
 
-DescribePackageVersionResponseTypeDef = TypedDict(
-    "DescribePackageVersionResponseTypeDef",
-    {
-        "IsLatestPatch": bool,
-        "OwnerAccount": str,
-        "PackageArn": str,
-        "PackageId": str,
-        "PackageName": str,
-        "PackageVersion": str,
-        "PatchVersion": str,
-        "RegisteredTime": datetime,
-        "Status": PackageVersionStatusType,
-        "StatusDescription": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredOTAJobConfigTypeDef = TypedDict(
     "_RequiredOTAJobConfigTypeDef",
     {
         "ImageVersion": str,
     },
 )
 _OptionalOTAJobConfigTypeDef = TypedDict(
@@ -487,19 +440,29 @@
         "DeviceName": str,
         "JobId": str,
         "JobType": JobTypeType,
     },
     total=False,
 )
 
+StaticIpConnectionInfoOutputTypeDef = TypedDict(
+    "StaticIpConnectionInfoOutputTypeDef",
+    {
+        "DefaultGateway": str,
+        "Dns": List[str],
+        "IpAddress": str,
+        "Mask": str,
+    },
+)
+
 StaticIpConnectionInfoTypeDef = TypedDict(
     "StaticIpConnectionInfoTypeDef",
     {
         "DefaultGateway": str,
-        "Dns": List[str],
+        "Dns": Sequence[str],
         "IpAddress": str,
         "Mask": str,
     },
 )
 
 EthernetStatusTypeDef = TypedDict(
     "EthernetStatusTypeDef",
@@ -507,14 +470,22 @@
         "ConnectionStatus": NetworkConnectionStatusType,
         "HwAddress": str,
         "IpAddress": str,
     },
     total=False,
 )
 
+JobResourceTagsTypeDef = TypedDict(
+    "JobResourceTagsTypeDef",
+    {
+        "ResourceType": Literal["PACKAGE"],
+        "Tags": Mapping[str, str],
+    },
+)
+
 _RequiredListApplicationInstanceDependenciesRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationInstanceDependenciesRequestRequestTypeDef",
     {
         "ApplicationInstanceId": str,
     },
 )
 _OptionalListApplicationInstanceDependenciesRequestRequestTypeDef = TypedDict(
@@ -734,26 +705,25 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+NtpPayloadOutputTypeDef = TypedDict(
+    "NtpPayloadOutputTypeDef",
     {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "NtpServers": List[str],
     },
 )
 
 NtpPayloadTypeDef = TypedDict(
     "NtpPayloadTypeDef",
     {
-        "NtpServers": List[str],
+        "NtpServers": Sequence[str],
     },
 )
 
 NtpStatusTypeDef = TypedDict(
     "NtpStatusTypeDef",
     {
         "ConnectionStatus": NetworkConnectionStatusType,
@@ -839,26 +809,14 @@
 )
 
 
 class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
 
-ProvisionDeviceResponseTypeDef = TypedDict(
-    "ProvisionDeviceResponseTypeDef",
-    {
-        "Arn": str,
-        "Certificates": bytes,
-        "DeviceId": str,
-        "IotThingName": str,
-        "Status": DeviceStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRegisterPackageVersionRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterPackageVersionRequestRequestTypeDef",
     {
         "PackageId": str,
         "PackageVersion": str,
         "PatchVersion": str,
     },
@@ -883,33 +841,14 @@
 RemoveApplicationInstanceRequestRequestTypeDef = TypedDict(
     "RemoveApplicationInstanceRequestRequestTypeDef",
     {
         "ApplicationInstanceId": str,
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
-SignalApplicationInstanceNodeInstancesResponseTypeDef = TypedDict(
-    "SignalApplicationInstanceNodeInstancesResponseTypeDef",
-    {
-        "ApplicationInstanceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -940,22 +879,14 @@
 class UpdateDeviceMetadataRequestRequestTypeDef(
     _RequiredUpdateDeviceMetadataRequestRequestTypeDef,
     _OptionalUpdateDeviceMetadataRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateDeviceMetadataResponseTypeDef = TypedDict(
-    "UpdateDeviceMetadataResponseTypeDef",
-    {
-        "DeviceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ApplicationInstanceTypeDef = TypedDict(
     "ApplicationInstanceTypeDef",
     {
         "ApplicationInstanceId": str,
         "Arn": str,
         "CreatedTime": datetime,
         "DefaultRuntimeContextDevice": str,
@@ -967,36 +898,14 @@
         "Status": ApplicationInstanceStatusType,
         "StatusDescription": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-DescribeApplicationInstanceResponseTypeDef = TypedDict(
-    "DescribeApplicationInstanceResponseTypeDef",
-    {
-        "ApplicationInstanceId": str,
-        "ApplicationInstanceIdToReplace": str,
-        "Arn": str,
-        "CreatedTime": datetime,
-        "DefaultRuntimeContextDevice": str,
-        "DefaultRuntimeContextDeviceName": str,
-        "Description": str,
-        "HealthStatus": ApplicationInstanceHealthStatusType,
-        "LastUpdatedTime": datetime,
-        "Name": str,
-        "RuntimeContextStates": List[ReportedRuntimeContextStateTypeDef],
-        "RuntimeRoleArn": str,
-        "Status": ApplicationInstanceStatusType,
-        "StatusDescription": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateApplicationInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationInstanceRequestRequestTypeDef",
     {
         "DefaultRuntimeContextDevice": str,
         "ManifestPayload": ManifestPayloadTypeDef,
     },
 )
@@ -1017,105 +926,182 @@
 class CreateApplicationInstanceRequestRequestTypeDef(
     _RequiredCreateApplicationInstanceRequestRequestTypeDef,
     _OptionalCreateApplicationInstanceRequestRequestTypeDef,
 ):
     pass
 
 
+CreateApplicationInstanceResponseTypeDef = TypedDict(
+    "CreateApplicationInstanceResponseTypeDef",
+    {
+        "ApplicationInstanceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateNodeFromTemplateJobResponseTypeDef = TypedDict(
+    "CreateNodeFromTemplateJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePackageImportJobResponseTypeDef = TypedDict(
+    "CreatePackageImportJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDeviceResponseTypeDef = TypedDict(
+    "DeleteDeviceResponseTypeDef",
+    {
+        "DeviceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeApplicationInstanceDetailsResponseTypeDef = TypedDict(
     "DescribeApplicationInstanceDetailsResponseTypeDef",
     {
         "ApplicationInstanceId": str,
         "ApplicationInstanceIdToReplace": str,
         "CreatedTime": datetime,
         "DefaultRuntimeContextDevice": str,
         "Description": str,
         "ManifestOverridesPayload": ManifestOverridesPayloadTypeDef,
         "ManifestPayload": ManifestPayloadTypeDef,
         "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateJobForDevicesResponseTypeDef = TypedDict(
-    "CreateJobForDevicesResponseTypeDef",
+DescribeApplicationInstanceResponseTypeDef = TypedDict(
+    "DescribeApplicationInstanceResponseTypeDef",
     {
-        "Jobs": List[JobTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ApplicationInstanceId": str,
+        "ApplicationInstanceIdToReplace": str,
+        "Arn": str,
+        "CreatedTime": datetime,
+        "DefaultRuntimeContextDevice": str,
+        "DefaultRuntimeContextDeviceName": str,
+        "Description": str,
+        "HealthStatus": ApplicationInstanceHealthStatusType,
+        "LastUpdatedTime": datetime,
+        "Name": str,
+        "RuntimeContextStates": List[ReportedRuntimeContextStateTypeDef],
+        "RuntimeRoleArn": str,
+        "Status": ApplicationInstanceStatusType,
+        "StatusDescription": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateNodeFromTemplateJobRequestRequestTypeDef",
+DescribeDeviceJobResponseTypeDef = TypedDict(
+    "DescribeDeviceJobResponseTypeDef",
     {
-        "NodeName": str,
-        "OutputPackageName": str,
-        "OutputPackageVersion": str,
-        "TemplateParameters": Mapping[str, str],
-        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
+        "CreatedTime": datetime,
+        "DeviceArn": str,
+        "DeviceId": str,
+        "DeviceName": str,
+        "DeviceType": DeviceTypeType,
+        "ImageVersion": str,
+        "JobId": str,
+        "JobType": JobTypeType,
+        "Status": UpdateProgressType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateNodeFromTemplateJobRequestRequestTypeDef",
+
+DescribePackageVersionResponseTypeDef = TypedDict(
+    "DescribePackageVersionResponseTypeDef",
     {
-        "JobTags": Sequence[JobResourceTagsTypeDef],
-        "NodeDescription": str,
+        "IsLatestPatch": bool,
+        "OwnerAccount": str,
+        "PackageArn": str,
+        "PackageId": str,
+        "PackageName": str,
+        "PackageVersion": str,
+        "PatchVersion": str,
+        "RegisteredTime": datetime,
+        "Status": PackageVersionStatusType,
+        "StatusDescription": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class CreateNodeFromTemplateJobRequestRequestTypeDef(
-    _RequiredCreateNodeFromTemplateJobRequestRequestTypeDef,
-    _OptionalCreateNodeFromTemplateJobRequestRequestTypeDef,
-):
-    pass
+ProvisionDeviceResponseTypeDef = TypedDict(
+    "ProvisionDeviceResponseTypeDef",
+    {
+        "Arn": str,
+        "Certificates": bytes,
+        "DeviceId": str,
+        "IotThingName": str,
+        "Status": DeviceStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+SignalApplicationInstanceNodeInstancesResponseTypeDef = TypedDict(
+    "SignalApplicationInstanceNodeInstancesResponseTypeDef",
+    {
+        "ApplicationInstanceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-DescribeNodeFromTemplateJobResponseTypeDef = TypedDict(
-    "DescribeNodeFromTemplateJobResponseTypeDef",
+UpdateDeviceMetadataResponseTypeDef = TypedDict(
+    "UpdateDeviceMetadataResponseTypeDef",
     {
-        "CreatedTime": datetime,
-        "JobId": str,
-        "JobTags": List[JobResourceTagsTypeDef],
-        "LastUpdatedTime": datetime,
-        "NodeDescription": str,
-        "NodeName": str,
-        "OutputPackageName": str,
-        "OutputPackageVersion": str,
-        "Status": NodeFromTemplateJobStatusType,
-        "StatusMessage": str,
-        "TemplateParameters": Dict[str, str],
-        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DeviceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateJobForDevicesResponseTypeDef = TypedDict(
+    "CreateJobForDevicesResponseTypeDef",
+    {
+        "Jobs": List[JobTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePackageResponseTypeDef = TypedDict(
     "CreatePackageResponseTypeDef",
     {
         "Arn": str,
         "PackageId": str,
         "StorageLocation": StorageLocationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePackageResponseTypeDef = TypedDict(
     "DescribePackageResponseTypeDef",
     {
         "Arn": str,
         "CreatedTime": datetime,
         "PackageId": str,
         "PackageName": str,
         "ReadAccessPrincipalArns": List[str],
         "StorageLocation": StorageLocationTypeDef,
         "Tags": Dict[str, str],
         "WriteAccessPrincipalArns": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeviceTypeDef = TypedDict(
     "DeviceTypeDef",
     {
         "Brand": DeviceBrandType,
@@ -1131,30 +1117,70 @@
         "ProvisioningStatus": DeviceStatusType,
         "Tags": Dict[str, str],
         "Type": DeviceTypeType,
     },
     total=False,
 )
 
+DescribeNodeFromTemplateJobResponseTypeDef = TypedDict(
+    "DescribeNodeFromTemplateJobResponseTypeDef",
+    {
+        "CreatedTime": datetime,
+        "JobId": str,
+        "JobTags": List[JobResourceTagsOutputTypeDef],
+        "LastUpdatedTime": datetime,
+        "NodeDescription": str,
+        "NodeName": str,
+        "OutputPackageName": str,
+        "OutputPackageVersion": str,
+        "Status": NodeFromTemplateJobStatusType,
+        "StatusMessage": str,
+        "TemplateParameters": Dict[str, str],
+        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DeviceJobConfigTypeDef = TypedDict(
     "DeviceJobConfigTypeDef",
     {
         "OTAJobConfig": OTAJobConfigTypeDef,
     },
     total=False,
 )
 
 ListDevicesJobsResponseTypeDef = TypedDict(
     "ListDevicesJobsResponseTypeDef",
     {
         "DeviceJobs": List[DeviceJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredEthernetPayloadOutputTypeDef = TypedDict(
+    "_RequiredEthernetPayloadOutputTypeDef",
+    {
+        "ConnectionType": ConnectionTypeType,
     },
 )
+_OptionalEthernetPayloadOutputTypeDef = TypedDict(
+    "_OptionalEthernetPayloadOutputTypeDef",
+    {
+        "StaticIpConnectionInfo": StaticIpConnectionInfoOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class EthernetPayloadOutputTypeDef(
+    _RequiredEthernetPayloadOutputTypeDef, _OptionalEthernetPayloadOutputTypeDef
+):
+    pass
+
 
 _RequiredEthernetPayloadTypeDef = TypedDict(
     "_RequiredEthernetPayloadTypeDef",
     {
         "ConnectionType": ConnectionTypeType,
     },
 )
@@ -1167,65 +1193,66 @@
 )
 
 
 class EthernetPayloadTypeDef(_RequiredEthernetPayloadTypeDef, _OptionalEthernetPayloadTypeDef):
     pass
 
 
+JobResourceTagsUnionTypeDef = Union[JobResourceTagsTypeDef, JobResourceTagsOutputTypeDef]
 ListApplicationInstanceDependenciesResponseTypeDef = TypedDict(
     "ListApplicationInstanceDependenciesResponseTypeDef",
     {
         "NextToken": str,
         "PackageObjects": List[PackageObjectTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationInstanceNodeInstancesResponseTypeDef = TypedDict(
     "ListApplicationInstanceNodeInstancesResponseTypeDef",
     {
         "NextToken": str,
         "NodeInstances": List[NodeInstanceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNodeFromTemplateJobsResponseTypeDef = TypedDict(
     "ListNodeFromTemplateJobsResponseTypeDef",
     {
         "NextToken": str,
         "NodeFromTemplateJobs": List[NodeFromTemplateJobTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNodesResponseTypeDef = TypedDict(
     "ListNodesResponseTypeDef",
     {
         "NextToken": str,
         "Nodes": List[NodeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPackageImportJobsResponseTypeDef = TypedDict(
     "ListPackageImportJobsResponseTypeDef",
     {
         "NextToken": str,
         "PackageImportJobs": List[PackageImportJobTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPackagesResponseTypeDef = TypedDict(
     "ListPackagesResponseTypeDef",
     {
         "NextToken": str,
         "Packages": List[PackageListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NetworkStatusTypeDef = TypedDict(
     "NetworkStatusTypeDef",
     {
         "Ethernet0Status": EthernetStatusTypeDef,
@@ -1278,24 +1305,24 @@
 )
 
 ListApplicationInstancesResponseTypeDef = TypedDict(
     "ListApplicationInstancesResponseTypeDef",
     {
         "ApplicationInstances": List[ApplicationInstanceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDevicesResponseTypeDef = TypedDict(
     "ListDevicesResponseTypeDef",
     {
         "Devices": List[DeviceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateJobForDevicesRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobForDevicesRequestRequestTypeDef",
     {
         "DeviceIds": Sequence[str],
@@ -1314,24 +1341,61 @@
 class CreateJobForDevicesRequestRequestTypeDef(
     _RequiredCreateJobForDevicesRequestRequestTypeDef,
     _OptionalCreateJobForDevicesRequestRequestTypeDef,
 ):
     pass
 
 
+NetworkPayloadOutputTypeDef = TypedDict(
+    "NetworkPayloadOutputTypeDef",
+    {
+        "Ethernet0": EthernetPayloadOutputTypeDef,
+        "Ethernet1": EthernetPayloadOutputTypeDef,
+        "Ntp": NtpPayloadOutputTypeDef,
+    },
+    total=False,
+)
+
 NetworkPayloadTypeDef = TypedDict(
     "NetworkPayloadTypeDef",
     {
         "Ethernet0": EthernetPayloadTypeDef,
         "Ethernet1": EthernetPayloadTypeDef,
         "Ntp": NtpPayloadTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateNodeFromTemplateJobRequestRequestTypeDef",
+    {
+        "NodeName": str,
+        "OutputPackageName": str,
+        "OutputPackageVersion": str,
+        "TemplateParameters": Mapping[str, str],
+        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
+    },
+)
+_OptionalCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateNodeFromTemplateJobRequestRequestTypeDef",
+    {
+        "JobTags": Sequence[JobResourceTagsUnionTypeDef],
+        "NodeDescription": str,
+    },
+    total=False,
+)
+
+
+class CreateNodeFromTemplateJobRequestRequestTypeDef(
+    _RequiredCreateNodeFromTemplateJobRequestRequestTypeDef,
+    _OptionalCreateNodeFromTemplateJobRequestRequestTypeDef,
+):
+    pass
+
+
 DescribeNodeResponseTypeDef = TypedDict(
     "DescribeNodeResponseTypeDef",
     {
         "AssetName": str,
         "Category": NodeCategoryType,
         "CreatedTime": datetime,
         "Description": str,
@@ -1341,15 +1405,15 @@
         "NodeInterface": NodeInterfaceTypeDef,
         "OwnerAccount": str,
         "PackageArn": str,
         "PackageId": str,
         "PackageName": str,
         "PackageVersion": str,
         "PatchVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PackageImportJobInputConfigTypeDef = TypedDict(
     "PackageImportJobInputConfigTypeDef",
     {
         "PackageVersionInputConfig": PackageVersionInputConfigTypeDef,
@@ -1371,23 +1435,24 @@
         "DeviceConnectionStatus": DeviceConnectionStatusType,
         "DeviceId": str,
         "LatestAlternateSoftware": str,
         "LatestDeviceJob": LatestDeviceJobTypeDef,
         "LatestSoftware": str,
         "LeaseExpirationTime": datetime,
         "Name": str,
-        "NetworkingConfiguration": NetworkPayloadTypeDef,
+        "NetworkingConfiguration": NetworkPayloadOutputTypeDef,
         "ProvisioningStatus": DeviceStatusType,
         "SerialNumber": str,
         "Tags": Dict[str, str],
         "Type": DeviceTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+NetworkPayloadUnionTypeDef = Union[NetworkPayloadTypeDef, NetworkPayloadOutputTypeDef]
 _RequiredProvisionDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredProvisionDeviceRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalProvisionDeviceRequestRequestTypeDef = TypedDict(
@@ -1415,15 +1480,15 @@
         "JobType": PackageImportJobTypeType,
         "OutputConfig": PackageImportJobOutputConfigTypeDef,
     },
 )
 _OptionalCreatePackageImportJobRequestRequestTypeDef = TypedDict(
     "_OptionalCreatePackageImportJobRequestRequestTypeDef",
     {
-        "JobTags": Sequence[JobResourceTagsTypeDef],
+        "JobTags": Sequence[JobResourceTagsUnionTypeDef],
     },
     total=False,
 )
 
 
 class CreatePackageImportJobRequestRequestTypeDef(
     _RequiredCreatePackageImportJobRequestRequestTypeDef,
@@ -1435,17 +1500,17 @@
 DescribePackageImportJobResponseTypeDef = TypedDict(
     "DescribePackageImportJobResponseTypeDef",
     {
         "ClientToken": str,
         "CreatedTime": datetime,
         "InputConfig": PackageImportJobInputConfigTypeDef,
         "JobId": str,
-        "JobTags": List[JobResourceTagsTypeDef],
+        "JobTags": List[JobResourceTagsOutputTypeDef],
         "JobType": PackageImportJobTypeType,
         "LastUpdatedTime": datetime,
         "Output": PackageImportJobOutputTypeDef,
         "OutputConfig": PackageImportJobOutputConfigTypeDef,
         "Status": PackageImportJobStatusType,
         "StatusMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-panorama-2.5.2/types_aiobotocore_panorama/type_defs.pyi` & `types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_panorama.type_defs import AlternateSoftwareMetadataTypeDef
 
-    data: AlternateSoftwareMetadataTypeDef = {...}
+    data: AlternateSoftwareMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ApplicationInstanceHealthStatusType,
     ApplicationInstanceStatusType,
     ConnectionTypeType,
     DesiredStateType,
     DeviceAggregatedStatusType,
@@ -52,41 +52,38 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AlternateSoftwareMetadataTypeDef",
     "ReportedRuntimeContextStateTypeDef",
     "ManifestOverridesPayloadTypeDef",
     "ManifestPayloadTypeDef",
-    "CreateApplicationInstanceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "JobTypeDef",
-    "JobResourceTagsTypeDef",
-    "CreateNodeFromTemplateJobResponseTypeDef",
-    "CreatePackageImportJobResponseTypeDef",
     "CreatePackageRequestRequestTypeDef",
     "StorageLocationTypeDef",
     "DeleteDeviceRequestRequestTypeDef",
-    "DeleteDeviceResponseTypeDef",
     "DeletePackageRequestRequestTypeDef",
     "DeregisterPackageVersionRequestRequestTypeDef",
     "DescribeApplicationInstanceDetailsRequestRequestTypeDef",
     "DescribeApplicationInstanceRequestRequestTypeDef",
     "DescribeDeviceJobRequestRequestTypeDef",
-    "DescribeDeviceJobResponseTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
     "LatestDeviceJobTypeDef",
     "DescribeNodeFromTemplateJobRequestRequestTypeDef",
+    "JobResourceTagsOutputTypeDef",
     "DescribeNodeRequestRequestTypeDef",
     "DescribePackageImportJobRequestRequestTypeDef",
     "DescribePackageRequestRequestTypeDef",
     "DescribePackageVersionRequestRequestTypeDef",
-    "DescribePackageVersionResponseTypeDef",
     "OTAJobConfigTypeDef",
     "DeviceJobTypeDef",
+    "StaticIpConnectionInfoOutputTypeDef",
     "StaticIpConnectionInfoTypeDef",
     "EthernetStatusTypeDef",
+    "JobResourceTagsTypeDef",
     "ListApplicationInstanceDependenciesRequestRequestTypeDef",
     "PackageObjectTypeDef",
     "ListApplicationInstanceNodeInstancesRequestRequestTypeDef",
     "NodeInstanceTypeDef",
     "ListApplicationInstancesRequestRequestTypeDef",
     "ListDevicesJobsRequestRequestTypeDef",
     "ListDevicesRequestRequestTypeDef",
@@ -95,45 +92,52 @@
     "ListNodesRequestRequestTypeDef",
     "NodeTypeDef",
     "ListPackageImportJobsRequestRequestTypeDef",
     "PackageImportJobTypeDef",
     "ListPackagesRequestRequestTypeDef",
     "PackageListItemTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "NtpPayloadOutputTypeDef",
     "NtpPayloadTypeDef",
     "NtpStatusTypeDef",
     "NodeInputPortTypeDef",
     "NodeOutputPortTypeDef",
     "NodeSignalTypeDef",
     "OutPutS3LocationTypeDef",
     "PackageVersionOutputConfigTypeDef",
     "S3LocationTypeDef",
-    "ProvisionDeviceResponseTypeDef",
     "RegisterPackageVersionRequestRequestTypeDef",
     "RemoveApplicationInstanceRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "SignalApplicationInstanceNodeInstancesResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeviceMetadataRequestRequestTypeDef",
-    "UpdateDeviceMetadataResponseTypeDef",
     "ApplicationInstanceTypeDef",
-    "DescribeApplicationInstanceResponseTypeDef",
     "CreateApplicationInstanceRequestRequestTypeDef",
+    "CreateApplicationInstanceResponseTypeDef",
+    "CreateNodeFromTemplateJobResponseTypeDef",
+    "CreatePackageImportJobResponseTypeDef",
+    "DeleteDeviceResponseTypeDef",
     "DescribeApplicationInstanceDetailsResponseTypeDef",
+    "DescribeApplicationInstanceResponseTypeDef",
+    "DescribeDeviceJobResponseTypeDef",
+    "DescribePackageVersionResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ProvisionDeviceResponseTypeDef",
+    "SignalApplicationInstanceNodeInstancesResponseTypeDef",
+    "UpdateDeviceMetadataResponseTypeDef",
     "CreateJobForDevicesResponseTypeDef",
-    "CreateNodeFromTemplateJobRequestRequestTypeDef",
-    "DescribeNodeFromTemplateJobResponseTypeDef",
     "CreatePackageResponseTypeDef",
     "DescribePackageResponseTypeDef",
     "DeviceTypeDef",
+    "DescribeNodeFromTemplateJobResponseTypeDef",
     "DeviceJobConfigTypeDef",
     "ListDevicesJobsResponseTypeDef",
+    "EthernetPayloadOutputTypeDef",
     "EthernetPayloadTypeDef",
+    "JobResourceTagsUnionTypeDef",
     "ListApplicationInstanceDependenciesResponseTypeDef",
     "ListApplicationInstanceNodeInstancesResponseTypeDef",
     "ListNodeFromTemplateJobsResponseTypeDef",
     "ListNodesResponseTypeDef",
     "ListPackageImportJobsResponseTypeDef",
     "ListPackagesResponseTypeDef",
     "NetworkStatusTypeDef",
@@ -141,18 +145,21 @@
     "SignalApplicationInstanceNodeInstancesRequestRequestTypeDef",
     "PackageImportJobOutputTypeDef",
     "PackageImportJobOutputConfigTypeDef",
     "PackageVersionInputConfigTypeDef",
     "ListApplicationInstancesResponseTypeDef",
     "ListDevicesResponseTypeDef",
     "CreateJobForDevicesRequestRequestTypeDef",
+    "NetworkPayloadOutputTypeDef",
     "NetworkPayloadTypeDef",
+    "CreateNodeFromTemplateJobRequestRequestTypeDef",
     "DescribeNodeResponseTypeDef",
     "PackageImportJobInputConfigTypeDef",
     "DescribeDeviceResponseTypeDef",
+    "NetworkPayloadUnionTypeDef",
     "ProvisionDeviceRequestRequestTypeDef",
     "CreatePackageImportJobRequestRequestTypeDef",
     "DescribePackageImportJobResponseTypeDef",
 )
 
 AlternateSoftwareMetadataTypeDef = TypedDict(
     "AlternateSoftwareMetadataTypeDef",
@@ -184,55 +191,34 @@
     "ManifestPayloadTypeDef",
     {
         "PayloadData": str,
     },
     total=False,
 )
 
-CreateApplicationInstanceResponseTypeDef = TypedDict(
-    "CreateApplicationInstanceResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ApplicationInstanceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
         "DeviceId": str,
         "JobId": str,
     },
     total=False,
 )
 
-JobResourceTagsTypeDef = TypedDict(
-    "JobResourceTagsTypeDef",
-    {
-        "ResourceType": Literal["PACKAGE"],
-        "Tags": Mapping[str, str],
-    },
-)
-
-CreateNodeFromTemplateJobResponseTypeDef = TypedDict(
-    "CreateNodeFromTemplateJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePackageImportJobResponseTypeDef = TypedDict(
-    "CreatePackageImportJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePackageRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackageRequestRequestTypeDef",
     {
         "PackageName": str,
     },
 )
 _OptionalCreatePackageRequestRequestTypeDef = TypedDict(
@@ -262,22 +248,14 @@
 DeleteDeviceRequestRequestTypeDef = TypedDict(
     "DeleteDeviceRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 
-DeleteDeviceResponseTypeDef = TypedDict(
-    "DeleteDeviceResponseTypeDef",
-    {
-        "DeviceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeletePackageRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePackageRequestRequestTypeDef",
     {
         "PackageId": str,
     },
 )
 _OptionalDeletePackageRequestRequestTypeDef = TypedDict(
@@ -333,30 +311,14 @@
 DescribeDeviceJobRequestRequestTypeDef = TypedDict(
     "DescribeDeviceJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-DescribeDeviceJobResponseTypeDef = TypedDict(
-    "DescribeDeviceJobResponseTypeDef",
-    {
-        "CreatedTime": datetime,
-        "DeviceArn": str,
-        "DeviceId": str,
-        "DeviceName": str,
-        "DeviceType": DeviceTypeType,
-        "ImageVersion": str,
-        "JobId": str,
-        "JobType": JobTypeType,
-        "Status": UpdateProgressType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDeviceRequestRequestTypeDef = TypedDict(
     "DescribeDeviceRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 
@@ -373,14 +335,22 @@
 DescribeNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
     "DescribeNodeFromTemplateJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+JobResourceTagsOutputTypeDef = TypedDict(
+    "JobResourceTagsOutputTypeDef",
+    {
+        "ResourceType": Literal["PACKAGE"],
+        "Tags": Dict[str, str],
+    },
+)
+
 _RequiredDescribeNodeRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeNodeRequestRequestTypeDef",
     {
         "NodeId": str,
     },
 )
 _OptionalDescribeNodeRequestRequestTypeDef = TypedDict(
@@ -428,31 +398,14 @@
 
 class DescribePackageVersionRequestRequestTypeDef(
     _RequiredDescribePackageVersionRequestRequestTypeDef,
     _OptionalDescribePackageVersionRequestRequestTypeDef,
 ):
     pass
 
-DescribePackageVersionResponseTypeDef = TypedDict(
-    "DescribePackageVersionResponseTypeDef",
-    {
-        "IsLatestPatch": bool,
-        "OwnerAccount": str,
-        "PackageArn": str,
-        "PackageId": str,
-        "PackageName": str,
-        "PackageVersion": str,
-        "PatchVersion": str,
-        "RegisteredTime": datetime,
-        "Status": PackageVersionStatusType,
-        "StatusDescription": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredOTAJobConfigTypeDef = TypedDict(
     "_RequiredOTAJobConfigTypeDef",
     {
         "ImageVersion": str,
     },
 )
 _OptionalOTAJobConfigTypeDef = TypedDict(
@@ -474,19 +427,29 @@
         "DeviceName": str,
         "JobId": str,
         "JobType": JobTypeType,
     },
     total=False,
 )
 
+StaticIpConnectionInfoOutputTypeDef = TypedDict(
+    "StaticIpConnectionInfoOutputTypeDef",
+    {
+        "DefaultGateway": str,
+        "Dns": List[str],
+        "IpAddress": str,
+        "Mask": str,
+    },
+)
+
 StaticIpConnectionInfoTypeDef = TypedDict(
     "StaticIpConnectionInfoTypeDef",
     {
         "DefaultGateway": str,
-        "Dns": List[str],
+        "Dns": Sequence[str],
         "IpAddress": str,
         "Mask": str,
     },
 )
 
 EthernetStatusTypeDef = TypedDict(
     "EthernetStatusTypeDef",
@@ -494,14 +457,22 @@
         "ConnectionStatus": NetworkConnectionStatusType,
         "HwAddress": str,
         "IpAddress": str,
     },
     total=False,
 )
 
+JobResourceTagsTypeDef = TypedDict(
+    "JobResourceTagsTypeDef",
+    {
+        "ResourceType": Literal["PACKAGE"],
+        "Tags": Mapping[str, str],
+    },
+)
+
 _RequiredListApplicationInstanceDependenciesRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationInstanceDependenciesRequestRequestTypeDef",
     {
         "ApplicationInstanceId": str,
     },
 )
 _OptionalListApplicationInstanceDependenciesRequestRequestTypeDef = TypedDict(
@@ -713,26 +684,25 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+NtpPayloadOutputTypeDef = TypedDict(
+    "NtpPayloadOutputTypeDef",
     {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "NtpServers": List[str],
     },
 )
 
 NtpPayloadTypeDef = TypedDict(
     "NtpPayloadTypeDef",
     {
-        "NtpServers": List[str],
+        "NtpServers": Sequence[str],
     },
 )
 
 NtpStatusTypeDef = TypedDict(
     "NtpStatusTypeDef",
     {
         "ConnectionStatus": NetworkConnectionStatusType,
@@ -814,26 +784,14 @@
     },
     total=False,
 )
 
 class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
-ProvisionDeviceResponseTypeDef = TypedDict(
-    "ProvisionDeviceResponseTypeDef",
-    {
-        "Arn": str,
-        "Certificates": bytes,
-        "DeviceId": str,
-        "IotThingName": str,
-        "Status": DeviceStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRegisterPackageVersionRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterPackageVersionRequestRequestTypeDef",
     {
         "PackageId": str,
         "PackageVersion": str,
         "PatchVersion": str,
     },
@@ -856,33 +814,14 @@
 RemoveApplicationInstanceRequestRequestTypeDef = TypedDict(
     "RemoveApplicationInstanceRequestRequestTypeDef",
     {
         "ApplicationInstanceId": str,
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
-SignalApplicationInstanceNodeInstancesResponseTypeDef = TypedDict(
-    "SignalApplicationInstanceNodeInstancesResponseTypeDef",
-    {
-        "ApplicationInstanceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -911,22 +850,14 @@
 
 class UpdateDeviceMetadataRequestRequestTypeDef(
     _RequiredUpdateDeviceMetadataRequestRequestTypeDef,
     _OptionalUpdateDeviceMetadataRequestRequestTypeDef,
 ):
     pass
 
-UpdateDeviceMetadataResponseTypeDef = TypedDict(
-    "UpdateDeviceMetadataResponseTypeDef",
-    {
-        "DeviceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ApplicationInstanceTypeDef = TypedDict(
     "ApplicationInstanceTypeDef",
     {
         "ApplicationInstanceId": str,
         "Arn": str,
         "CreatedTime": datetime,
         "DefaultRuntimeContextDevice": str,
@@ -938,36 +869,14 @@
         "Status": ApplicationInstanceStatusType,
         "StatusDescription": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-DescribeApplicationInstanceResponseTypeDef = TypedDict(
-    "DescribeApplicationInstanceResponseTypeDef",
-    {
-        "ApplicationInstanceId": str,
-        "ApplicationInstanceIdToReplace": str,
-        "Arn": str,
-        "CreatedTime": datetime,
-        "DefaultRuntimeContextDevice": str,
-        "DefaultRuntimeContextDeviceName": str,
-        "Description": str,
-        "HealthStatus": ApplicationInstanceHealthStatusType,
-        "LastUpdatedTime": datetime,
-        "Name": str,
-        "RuntimeContextStates": List[ReportedRuntimeContextStateTypeDef],
-        "RuntimeRoleArn": str,
-        "Status": ApplicationInstanceStatusType,
-        "StatusDescription": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateApplicationInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationInstanceRequestRequestTypeDef",
     {
         "DefaultRuntimeContextDevice": str,
         "ManifestPayload": ManifestPayloadTypeDef,
     },
 )
@@ -986,103 +895,182 @@
 
 class CreateApplicationInstanceRequestRequestTypeDef(
     _RequiredCreateApplicationInstanceRequestRequestTypeDef,
     _OptionalCreateApplicationInstanceRequestRequestTypeDef,
 ):
     pass
 
+CreateApplicationInstanceResponseTypeDef = TypedDict(
+    "CreateApplicationInstanceResponseTypeDef",
+    {
+        "ApplicationInstanceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateNodeFromTemplateJobResponseTypeDef = TypedDict(
+    "CreateNodeFromTemplateJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePackageImportJobResponseTypeDef = TypedDict(
+    "CreatePackageImportJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDeviceResponseTypeDef = TypedDict(
+    "DeleteDeviceResponseTypeDef",
+    {
+        "DeviceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeApplicationInstanceDetailsResponseTypeDef = TypedDict(
     "DescribeApplicationInstanceDetailsResponseTypeDef",
     {
         "ApplicationInstanceId": str,
         "ApplicationInstanceIdToReplace": str,
         "CreatedTime": datetime,
         "DefaultRuntimeContextDevice": str,
         "Description": str,
         "ManifestOverridesPayload": ManifestOverridesPayloadTypeDef,
         "ManifestPayload": ManifestPayloadTypeDef,
         "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateJobForDevicesResponseTypeDef = TypedDict(
-    "CreateJobForDevicesResponseTypeDef",
+DescribeApplicationInstanceResponseTypeDef = TypedDict(
+    "DescribeApplicationInstanceResponseTypeDef",
     {
-        "Jobs": List[JobTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ApplicationInstanceId": str,
+        "ApplicationInstanceIdToReplace": str,
+        "Arn": str,
+        "CreatedTime": datetime,
+        "DefaultRuntimeContextDevice": str,
+        "DefaultRuntimeContextDeviceName": str,
+        "Description": str,
+        "HealthStatus": ApplicationInstanceHealthStatusType,
+        "LastUpdatedTime": datetime,
+        "Name": str,
+        "RuntimeContextStates": List[ReportedRuntimeContextStateTypeDef],
+        "RuntimeRoleArn": str,
+        "Status": ApplicationInstanceStatusType,
+        "StatusDescription": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateNodeFromTemplateJobRequestRequestTypeDef",
+DescribeDeviceJobResponseTypeDef = TypedDict(
+    "DescribeDeviceJobResponseTypeDef",
     {
-        "NodeName": str,
-        "OutputPackageName": str,
-        "OutputPackageVersion": str,
-        "TemplateParameters": Mapping[str, str],
-        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
+        "CreatedTime": datetime,
+        "DeviceArn": str,
+        "DeviceId": str,
+        "DeviceName": str,
+        "DeviceType": DeviceTypeType,
+        "ImageVersion": str,
+        "JobId": str,
+        "JobType": JobTypeType,
+        "Status": UpdateProgressType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateNodeFromTemplateJobRequestRequestTypeDef",
+
+DescribePackageVersionResponseTypeDef = TypedDict(
+    "DescribePackageVersionResponseTypeDef",
     {
-        "JobTags": Sequence[JobResourceTagsTypeDef],
-        "NodeDescription": str,
+        "IsLatestPatch": bool,
+        "OwnerAccount": str,
+        "PackageArn": str,
+        "PackageId": str,
+        "PackageName": str,
+        "PackageVersion": str,
+        "PatchVersion": str,
+        "RegisteredTime": datetime,
+        "Status": PackageVersionStatusType,
+        "StatusDescription": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateNodeFromTemplateJobRequestRequestTypeDef(
-    _RequiredCreateNodeFromTemplateJobRequestRequestTypeDef,
-    _OptionalCreateNodeFromTemplateJobRequestRequestTypeDef,
-):
-    pass
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-DescribeNodeFromTemplateJobResponseTypeDef = TypedDict(
-    "DescribeNodeFromTemplateJobResponseTypeDef",
+ProvisionDeviceResponseTypeDef = TypedDict(
+    "ProvisionDeviceResponseTypeDef",
     {
-        "CreatedTime": datetime,
-        "JobId": str,
-        "JobTags": List[JobResourceTagsTypeDef],
-        "LastUpdatedTime": datetime,
-        "NodeDescription": str,
-        "NodeName": str,
-        "OutputPackageName": str,
-        "OutputPackageVersion": str,
-        "Status": NodeFromTemplateJobStatusType,
-        "StatusMessage": str,
-        "TemplateParameters": Dict[str, str],
-        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Arn": str,
+        "Certificates": bytes,
+        "DeviceId": str,
+        "IotThingName": str,
+        "Status": DeviceStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SignalApplicationInstanceNodeInstancesResponseTypeDef = TypedDict(
+    "SignalApplicationInstanceNodeInstancesResponseTypeDef",
+    {
+        "ApplicationInstanceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDeviceMetadataResponseTypeDef = TypedDict(
+    "UpdateDeviceMetadataResponseTypeDef",
+    {
+        "DeviceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateJobForDevicesResponseTypeDef = TypedDict(
+    "CreateJobForDevicesResponseTypeDef",
+    {
+        "Jobs": List[JobTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePackageResponseTypeDef = TypedDict(
     "CreatePackageResponseTypeDef",
     {
         "Arn": str,
         "PackageId": str,
         "StorageLocation": StorageLocationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePackageResponseTypeDef = TypedDict(
     "DescribePackageResponseTypeDef",
     {
         "Arn": str,
         "CreatedTime": datetime,
         "PackageId": str,
         "PackageName": str,
         "ReadAccessPrincipalArns": List[str],
         "StorageLocation": StorageLocationTypeDef,
         "Tags": Dict[str, str],
         "WriteAccessPrincipalArns": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeviceTypeDef = TypedDict(
     "DeviceTypeDef",
     {
         "Brand": DeviceBrandType,
@@ -1098,31 +1086,69 @@
         "ProvisioningStatus": DeviceStatusType,
         "Tags": Dict[str, str],
         "Type": DeviceTypeType,
     },
     total=False,
 )
 
+DescribeNodeFromTemplateJobResponseTypeDef = TypedDict(
+    "DescribeNodeFromTemplateJobResponseTypeDef",
+    {
+        "CreatedTime": datetime,
+        "JobId": str,
+        "JobTags": List[JobResourceTagsOutputTypeDef],
+        "LastUpdatedTime": datetime,
+        "NodeDescription": str,
+        "NodeName": str,
+        "OutputPackageName": str,
+        "OutputPackageVersion": str,
+        "Status": NodeFromTemplateJobStatusType,
+        "StatusMessage": str,
+        "TemplateParameters": Dict[str, str],
+        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DeviceJobConfigTypeDef = TypedDict(
     "DeviceJobConfigTypeDef",
     {
         "OTAJobConfig": OTAJobConfigTypeDef,
     },
     total=False,
 )
 
 ListDevicesJobsResponseTypeDef = TypedDict(
     "ListDevicesJobsResponseTypeDef",
     {
         "DeviceJobs": List[DeviceJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredEthernetPayloadOutputTypeDef = TypedDict(
+    "_RequiredEthernetPayloadOutputTypeDef",
+    {
+        "ConnectionType": ConnectionTypeType,
+    },
+)
+_OptionalEthernetPayloadOutputTypeDef = TypedDict(
+    "_OptionalEthernetPayloadOutputTypeDef",
+    {
+        "StaticIpConnectionInfo": StaticIpConnectionInfoOutputTypeDef,
     },
+    total=False,
 )
 
+class EthernetPayloadOutputTypeDef(
+    _RequiredEthernetPayloadOutputTypeDef, _OptionalEthernetPayloadOutputTypeDef
+):
+    pass
+
 _RequiredEthernetPayloadTypeDef = TypedDict(
     "_RequiredEthernetPayloadTypeDef",
     {
         "ConnectionType": ConnectionTypeType,
     },
 )
 _OptionalEthernetPayloadTypeDef = TypedDict(
@@ -1132,65 +1158,66 @@
     },
     total=False,
 )
 
 class EthernetPayloadTypeDef(_RequiredEthernetPayloadTypeDef, _OptionalEthernetPayloadTypeDef):
     pass
 
+JobResourceTagsUnionTypeDef = Union[JobResourceTagsTypeDef, JobResourceTagsOutputTypeDef]
 ListApplicationInstanceDependenciesResponseTypeDef = TypedDict(
     "ListApplicationInstanceDependenciesResponseTypeDef",
     {
         "NextToken": str,
         "PackageObjects": List[PackageObjectTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationInstanceNodeInstancesResponseTypeDef = TypedDict(
     "ListApplicationInstanceNodeInstancesResponseTypeDef",
     {
         "NextToken": str,
         "NodeInstances": List[NodeInstanceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNodeFromTemplateJobsResponseTypeDef = TypedDict(
     "ListNodeFromTemplateJobsResponseTypeDef",
     {
         "NextToken": str,
         "NodeFromTemplateJobs": List[NodeFromTemplateJobTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNodesResponseTypeDef = TypedDict(
     "ListNodesResponseTypeDef",
     {
         "NextToken": str,
         "Nodes": List[NodeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPackageImportJobsResponseTypeDef = TypedDict(
     "ListPackageImportJobsResponseTypeDef",
     {
         "NextToken": str,
         "PackageImportJobs": List[PackageImportJobTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPackagesResponseTypeDef = TypedDict(
     "ListPackagesResponseTypeDef",
     {
         "NextToken": str,
         "Packages": List[PackageListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NetworkStatusTypeDef = TypedDict(
     "NetworkStatusTypeDef",
     {
         "Ethernet0Status": EthernetStatusTypeDef,
@@ -1243,24 +1270,24 @@
 )
 
 ListApplicationInstancesResponseTypeDef = TypedDict(
     "ListApplicationInstancesResponseTypeDef",
     {
         "ApplicationInstances": List[ApplicationInstanceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDevicesResponseTypeDef = TypedDict(
     "ListDevicesResponseTypeDef",
     {
         "Devices": List[DeviceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateJobForDevicesRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobForDevicesRequestRequestTypeDef",
     {
         "DeviceIds": Sequence[str],
@@ -1277,24 +1304,59 @@
 
 class CreateJobForDevicesRequestRequestTypeDef(
     _RequiredCreateJobForDevicesRequestRequestTypeDef,
     _OptionalCreateJobForDevicesRequestRequestTypeDef,
 ):
     pass
 
+NetworkPayloadOutputTypeDef = TypedDict(
+    "NetworkPayloadOutputTypeDef",
+    {
+        "Ethernet0": EthernetPayloadOutputTypeDef,
+        "Ethernet1": EthernetPayloadOutputTypeDef,
+        "Ntp": NtpPayloadOutputTypeDef,
+    },
+    total=False,
+)
+
 NetworkPayloadTypeDef = TypedDict(
     "NetworkPayloadTypeDef",
     {
         "Ethernet0": EthernetPayloadTypeDef,
         "Ethernet1": EthernetPayloadTypeDef,
         "Ntp": NtpPayloadTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateNodeFromTemplateJobRequestRequestTypeDef",
+    {
+        "NodeName": str,
+        "OutputPackageName": str,
+        "OutputPackageVersion": str,
+        "TemplateParameters": Mapping[str, str],
+        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
+    },
+)
+_OptionalCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateNodeFromTemplateJobRequestRequestTypeDef",
+    {
+        "JobTags": Sequence[JobResourceTagsUnionTypeDef],
+        "NodeDescription": str,
+    },
+    total=False,
+)
+
+class CreateNodeFromTemplateJobRequestRequestTypeDef(
+    _RequiredCreateNodeFromTemplateJobRequestRequestTypeDef,
+    _OptionalCreateNodeFromTemplateJobRequestRequestTypeDef,
+):
+    pass
+
 DescribeNodeResponseTypeDef = TypedDict(
     "DescribeNodeResponseTypeDef",
     {
         "AssetName": str,
         "Category": NodeCategoryType,
         "CreatedTime": datetime,
         "Description": str,
@@ -1304,15 +1366,15 @@
         "NodeInterface": NodeInterfaceTypeDef,
         "OwnerAccount": str,
         "PackageArn": str,
         "PackageId": str,
         "PackageName": str,
         "PackageVersion": str,
         "PatchVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PackageImportJobInputConfigTypeDef = TypedDict(
     "PackageImportJobInputConfigTypeDef",
     {
         "PackageVersionInputConfig": PackageVersionInputConfigTypeDef,
@@ -1334,23 +1396,24 @@
         "DeviceConnectionStatus": DeviceConnectionStatusType,
         "DeviceId": str,
         "LatestAlternateSoftware": str,
         "LatestDeviceJob": LatestDeviceJobTypeDef,
         "LatestSoftware": str,
         "LeaseExpirationTime": datetime,
         "Name": str,
-        "NetworkingConfiguration": NetworkPayloadTypeDef,
+        "NetworkingConfiguration": NetworkPayloadOutputTypeDef,
         "ProvisioningStatus": DeviceStatusType,
         "SerialNumber": str,
         "Tags": Dict[str, str],
         "Type": DeviceTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+NetworkPayloadUnionTypeDef = Union[NetworkPayloadTypeDef, NetworkPayloadOutputTypeDef]
 _RequiredProvisionDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredProvisionDeviceRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalProvisionDeviceRequestRequestTypeDef = TypedDict(
@@ -1376,15 +1439,15 @@
         "JobType": PackageImportJobTypeType,
         "OutputConfig": PackageImportJobOutputConfigTypeDef,
     },
 )
 _OptionalCreatePackageImportJobRequestRequestTypeDef = TypedDict(
     "_OptionalCreatePackageImportJobRequestRequestTypeDef",
     {
-        "JobTags": Sequence[JobResourceTagsTypeDef],
+        "JobTags": Sequence[JobResourceTagsUnionTypeDef],
     },
     total=False,
 )
 
 class CreatePackageImportJobRequestRequestTypeDef(
     _RequiredCreatePackageImportJobRequestRequestTypeDef,
     _OptionalCreatePackageImportJobRequestRequestTypeDef,
@@ -1394,17 +1457,17 @@
 DescribePackageImportJobResponseTypeDef = TypedDict(
     "DescribePackageImportJobResponseTypeDef",
     {
         "ClientToken": str,
         "CreatedTime": datetime,
         "InputConfig": PackageImportJobInputConfigTypeDef,
         "JobId": str,
-        "JobTags": List[JobResourceTagsTypeDef],
+        "JobTags": List[JobResourceTagsOutputTypeDef],
         "JobType": PackageImportJobTypeType,
         "LastUpdatedTime": datetime,
         "Output": PackageImportJobOutputTypeDef,
         "OutputConfig": PackageImportJobOutputConfigTypeDef,
         "Status": PackageImportJobStatusType,
         "StatusMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-panorama-2.5.2/types_aiobotocore_panorama.egg-info/PKG-INFO` & `types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-panorama
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Panorama 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Panorama 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore panorama type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore panorama type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-panorama"></a>
 
 # types-aiobotocore-panorama
 
 [![PyPI - types-aiobotocore-panorama](https://img.shields.io/pypi/v/types-aiobotocore-panorama.svg?color=blue)](https://pypi.org/project/types-aiobotocore-panorama)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-panorama.svg?color=blue)](https://pypi.org/project/types-aiobotocore-panorama)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-panorama?color=blue)](https://pypistats.org/packages/types-aiobotocore-panorama)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-panorama)](https://pepy.tech/project/types-aiobotocore-panorama)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Panorama 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
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
 [types-aiobotocore-panorama docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/).
 
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
@@ -304,54 +303,51 @@
 )
 
 
 def check_value(value: ApplicationInstanceHealthStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_panorama.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_panorama.type_defs import (
     AlternateSoftwareMetadataTypeDef,
     ReportedRuntimeContextStateTypeDef,
     ManifestOverridesPayloadTypeDef,
     ManifestPayloadTypeDef,
-    CreateApplicationInstanceResponseTypeDef,
+    ResponseMetadataTypeDef,
     JobTypeDef,
-    JobResourceTagsTypeDef,
-    CreateNodeFromTemplateJobResponseTypeDef,
-    CreatePackageImportJobResponseTypeDef,
     CreatePackageRequestRequestTypeDef,
     StorageLocationTypeDef,
     DeleteDeviceRequestRequestTypeDef,
-    DeleteDeviceResponseTypeDef,
     DeletePackageRequestRequestTypeDef,
     DeregisterPackageVersionRequestRequestTypeDef,
     DescribeApplicationInstanceDetailsRequestRequestTypeDef,
     DescribeApplicationInstanceRequestRequestTypeDef,
     DescribeDeviceJobRequestRequestTypeDef,
-    DescribeDeviceJobResponseTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     LatestDeviceJobTypeDef,
     DescribeNodeFromTemplateJobRequestRequestTypeDef,
+    JobResourceTagsOutputTypeDef,
     DescribeNodeRequestRequestTypeDef,
     DescribePackageImportJobRequestRequestTypeDef,
     DescribePackageRequestRequestTypeDef,
     DescribePackageVersionRequestRequestTypeDef,
-    DescribePackageVersionResponseTypeDef,
     OTAJobConfigTypeDef,
     DeviceJobTypeDef,
+    StaticIpConnectionInfoOutputTypeDef,
     StaticIpConnectionInfoTypeDef,
     EthernetStatusTypeDef,
+    JobResourceTagsTypeDef,
     ListApplicationInstanceDependenciesRequestRequestTypeDef,
     PackageObjectTypeDef,
     ListApplicationInstanceNodeInstancesRequestRequestTypeDef,
     NodeInstanceTypeDef,
     ListApplicationInstancesRequestRequestTypeDef,
     ListDevicesJobsRequestRequestTypeDef,
     ListDevicesRequestRequestTypeDef,
@@ -360,45 +356,52 @@
     ListNodesRequestRequestTypeDef,
     NodeTypeDef,
     ListPackageImportJobsRequestRequestTypeDef,
     PackageImportJobTypeDef,
     ListPackagesRequestRequestTypeDef,
     PackageListItemTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    NtpPayloadOutputTypeDef,
     NtpPayloadTypeDef,
     NtpStatusTypeDef,
     NodeInputPortTypeDef,
     NodeOutputPortTypeDef,
     NodeSignalTypeDef,
     OutPutS3LocationTypeDef,
     PackageVersionOutputConfigTypeDef,
     S3LocationTypeDef,
-    ProvisionDeviceResponseTypeDef,
     RegisterPackageVersionRequestRequestTypeDef,
     RemoveApplicationInstanceRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    SignalApplicationInstanceNodeInstancesResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceMetadataRequestRequestTypeDef,
-    UpdateDeviceMetadataResponseTypeDef,
     ApplicationInstanceTypeDef,
-    DescribeApplicationInstanceResponseTypeDef,
     CreateApplicationInstanceRequestRequestTypeDef,
+    CreateApplicationInstanceResponseTypeDef,
+    CreateNodeFromTemplateJobResponseTypeDef,
+    CreatePackageImportJobResponseTypeDef,
+    DeleteDeviceResponseTypeDef,
     DescribeApplicationInstanceDetailsResponseTypeDef,
+    DescribeApplicationInstanceResponseTypeDef,
+    DescribeDeviceJobResponseTypeDef,
+    DescribePackageVersionResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ProvisionDeviceResponseTypeDef,
+    SignalApplicationInstanceNodeInstancesResponseTypeDef,
+    UpdateDeviceMetadataResponseTypeDef,
     CreateJobForDevicesResponseTypeDef,
-    CreateNodeFromTemplateJobRequestRequestTypeDef,
-    DescribeNodeFromTemplateJobResponseTypeDef,
     CreatePackageResponseTypeDef,
     DescribePackageResponseTypeDef,
     DeviceTypeDef,
+    DescribeNodeFromTemplateJobResponseTypeDef,
     DeviceJobConfigTypeDef,
     ListDevicesJobsResponseTypeDef,
+    EthernetPayloadOutputTypeDef,
     EthernetPayloadTypeDef,
+    JobResourceTagsUnionTypeDef,
     ListApplicationInstanceDependenciesResponseTypeDef,
     ListApplicationInstanceNodeInstancesResponseTypeDef,
     ListNodeFromTemplateJobsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListPackageImportJobsResponseTypeDef,
     ListPackagesResponseTypeDef,
     NetworkStatusTypeDef,
@@ -406,25 +409,28 @@
     SignalApplicationInstanceNodeInstancesRequestRequestTypeDef,
     PackageImportJobOutputTypeDef,
     PackageImportJobOutputConfigTypeDef,
     PackageVersionInputConfigTypeDef,
     ListApplicationInstancesResponseTypeDef,
     ListDevicesResponseTypeDef,
     CreateJobForDevicesRequestRequestTypeDef,
+    NetworkPayloadOutputTypeDef,
     NetworkPayloadTypeDef,
+    CreateNodeFromTemplateJobRequestRequestTypeDef,
     DescribeNodeResponseTypeDef,
     PackageImportJobInputConfigTypeDef,
     DescribeDeviceResponseTypeDef,
+    NetworkPayloadUnionTypeDef,
     ProvisionDeviceRequestRequestTypeDef,
     CreatePackageImportJobRequestRequestTypeDef,
     DescribePackageImportJobResponseTypeDef,
 )
 
 
-def get_structure() -> AlternateSoftwareMetadataTypeDef:
+def get_value() -> AlternateSoftwareMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-panorama-2.5.2/types_aiobotocore_panorama.egg-info/SOURCES.txt` & `types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama.egg-info/SOURCES.txt`

 * *Files identical despite different names*


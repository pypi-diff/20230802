# Comparing `tmp/types-aiobotocore-codestar-connections-2.5.2.tar.gz` & `tmp/types-aiobotocore-codestar-connections-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codestar-connections-2.5.2.tar", last modified: Sat Jul  8 01:43:25 2023, max compression
+gzip compressed data, was "types-aiobotocore-codestar-connections-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:04 2023, max compression
```

## Comparing `types-aiobotocore-codestar-connections-2.5.2.tar` & `types-aiobotocore-codestar-connections-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:25.705905 types-aiobotocore-codestar-connections-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:41.000000 types-aiobotocore-codestar-connections-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-07-08 01:43:25.701905 types-aiobotocore-codestar-connections-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-07-08 01:27:41.000000 types-aiobotocore-codestar-connections-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:25.705905 types-aiobotocore-codestar-connections-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-08 01:27:41.000000 types-aiobotocore-codestar-connections-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:25.701905 types-aiobotocore-codestar-connections-2.5.2/types_aiobotocore_codestar_connections/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-08 01:27:41.000000 types-aiobotocore-codestar-connections-2.5.2/types_aiobotocore_codestar_connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-08 01:27:41.000000 types-aiobotocore-codestar-connections-2.5.2/types_aiobotocore_codestar_connections/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-08 01:27:41.000000 types-aiobotocore-codestar-connections-2.5.2/types_aiobotocore_codestar_connections/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-07-08 01:27:41.000000 types-aiobotocore-codestar-connections-2.5.2/types_aiobotocore_codestar_connections/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11728 2023-07-08 01:27:41.000000 types-aiobotocore-codestar-connections-2.5.2/types_aiobotocore_codestar_connections/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-07-08 01:27:42.000000 types-aiobotocore-codestar-connections-2.5.2/types_aiobotocore_codestar_connections/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-07-08 01:27:41.000000 types-aiobotocore-codestar-connections-2.5.2/types_aiobotocore_codestar_connections/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:41.000000 types-aiobotocore-codestar-connections-2.5.2/types_aiobotocore_codestar_connections/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-07-08 01:27:42.000000 types-aiobotocore-codestar-connections-2.5.2/types_aiobotocore_codestar_connections/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-07-08 01:27:42.000000 types-aiobotocore-codestar-connections-2.5.2/types_aiobotocore_codestar_connections/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:41.000000 types-aiobotocore-codestar-connections-2.5.2/types_aiobotocore_codestar_connections/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:25.701905 types-aiobotocore-codestar-connections-2.5.2/types_aiobotocore_codestar_connections.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-07-08 01:43:25.000000 types-aiobotocore-codestar-connections-2.5.2/types_aiobotocore_codestar_connections.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-08 01:43:25.000000 types-aiobotocore-codestar-connections-2.5.2/types_aiobotocore_codestar_connections.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:25.000000 types-aiobotocore-codestar-connections-2.5.2/types_aiobotocore_codestar_connections.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:25.000000 types-aiobotocore-codestar-connections-2.5.2/types_aiobotocore_codestar_connections.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:25.000000 types-aiobotocore-codestar-connections-2.5.2/types_aiobotocore_codestar_connections.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-08 01:43:25.000000 types-aiobotocore-codestar-connections-2.5.2/types_aiobotocore_codestar_connections.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.745619 types-aiobotocore-codestar-connections-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-connections-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-08-02 14:52:04.745619 types-aiobotocore-codestar-connections-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11923 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-connections-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:04.745619 types-aiobotocore-codestar-connections-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-connections-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.733619 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11763 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.745619 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codestar-connections-2.5.2/LICENSE` & `types-aiobotocore-codestar-connections-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-connections-2.5.2/PKG-INFO` & `types-aiobotocore-codestar-connections-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codestar-connections
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CodeStarconnections 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CodeStarconnections 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore codestar-connections type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore codestar-connections type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-codestar-connections"></a>
 
 # types-aiobotocore-codestar-connections
 
 [![PyPI - types-aiobotocore-codestar-connections](https://img.shields.io/pypi/v/types-aiobotocore-codestar-connections.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-connections)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codestar-connections.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-connections)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codestar-connections?color=blue)](https://pypistats.org/packages/types-aiobotocore-codestar-connections)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codestar-connections)](https://pepy.tech/project/types-aiobotocore-codestar-connections)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeStarconnections 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
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
 [types-aiobotocore-codestar-connections docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/).
 
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
@@ -282,51 +281,54 @@
 )
 
 
 def check_value(value: ConnectionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codestar_connections.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from types_aiobotocore_codestar_connections.type_defs import (
     ConnectionTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     VpcConfigurationTypeDef,
     DeleteConnectionInputRequestTypeDef,
     DeleteHostInputRequestTypeDef,
     GetConnectionInputRequestTypeDef,
     GetHostInputRequestTypeDef,
+    VpcConfigurationOutputTypeDef,
     ListConnectionsInputRequestTypeDef,
     ListHostsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceInputRequestTypeDef,
-    GetConnectionOutputTypeDef,
-    ListConnectionsOutputTypeDef,
     CreateConnectionInputRequestTypeDef,
+    TagResourceInputRequestTypeDef,
     CreateConnectionOutputTypeDef,
     CreateHostOutputTypeDef,
+    GetConnectionOutputTypeDef,
+    ListConnectionsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    TagResourceInputRequestTypeDef,
     CreateHostInputRequestTypeDef,
+    UpdateHostInputRequestTypeDef,
     GetHostOutputTypeDef,
     HostTypeDef,
-    UpdateHostInputRequestTypeDef,
+    VpcConfigurationUnionTypeDef,
     ListHostsOutputTypeDef,
 )
 
 
-def get_structure() -> ConnectionTypeDef:
+def get_value() -> ConnectionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codestar-connections-2.5.2/README.md` & `types-aiobotocore-codestar-connections-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-codestar-connections"></a>
 
 # types-aiobotocore-codestar-connections
 
 [![PyPI - types-aiobotocore-codestar-connections](https://img.shields.io/pypi/v/types-aiobotocore-codestar-connections.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-connections)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codestar-connections.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-connections)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codestar-connections?color=blue)](https://pypistats.org/packages/types-aiobotocore-codestar-connections)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codestar-connections)](https://pepy.tech/project/types-aiobotocore-codestar-connections)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeStarconnections 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
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
 [types-aiobotocore-codestar-connections docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/).
 
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
@@ -249,51 +249,54 @@
 )
 
 
 def check_value(value: ConnectionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codestar_connections.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from types_aiobotocore_codestar_connections.type_defs import (
     ConnectionTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     VpcConfigurationTypeDef,
     DeleteConnectionInputRequestTypeDef,
     DeleteHostInputRequestTypeDef,
     GetConnectionInputRequestTypeDef,
     GetHostInputRequestTypeDef,
+    VpcConfigurationOutputTypeDef,
     ListConnectionsInputRequestTypeDef,
     ListHostsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceInputRequestTypeDef,
-    GetConnectionOutputTypeDef,
-    ListConnectionsOutputTypeDef,
     CreateConnectionInputRequestTypeDef,
+    TagResourceInputRequestTypeDef,
     CreateConnectionOutputTypeDef,
     CreateHostOutputTypeDef,
+    GetConnectionOutputTypeDef,
+    ListConnectionsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    TagResourceInputRequestTypeDef,
     CreateHostInputRequestTypeDef,
+    UpdateHostInputRequestTypeDef,
     GetHostOutputTypeDef,
     HostTypeDef,
-    UpdateHostInputRequestTypeDef,
+    VpcConfigurationUnionTypeDef,
     ListHostsOutputTypeDef,
 )
 
 
-def get_structure() -> ConnectionTypeDef:
+def get_value() -> ConnectionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codestar-connections-2.5.2/setup.py` & `types-aiobotocore-codestar-connections-2.5.2.post1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,45 +6,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codestar-connections",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_codestar_connections"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CodeStarconnections 2.5.2 service generated with"
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
-        "aiobotocore codestar-connections type-annotations boto3-stubs mypy typeshed autocomplete"
+        "aiobotocore codestar-connections type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_codestar_connections": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/",
```

### Comparing `types-aiobotocore-codestar-connections-2.5.2/types_aiobotocore_codestar_connections/__init__.py` & `types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-connections-2.5.2/types_aiobotocore_codestar_connections/__init__.pyi` & `types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-connections-2.5.2/types_aiobotocore_codestar_connections/__main__.py` & `types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.CodeStarconnections 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections\nOther"
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

### Comparing `types-aiobotocore-codestar-connections-2.5.2/types_aiobotocore_codestar_connections/client.py` & `types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     CreateHostOutputTypeDef,
     GetConnectionOutputTypeDef,
     GetHostOutputTypeDef,
     ListConnectionsOutputTypeDef,
     ListHostsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagTypeDef,
-    VpcConfigurationTypeDef,
+    VpcConfigurationUnionTypeDef,
 )
 
 __all__ = ("CodeStarconnectionsClient",)
 
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
@@ -103,15 +103,15 @@
 
     async def create_host(
         self,
         *,
         Name: str,
         ProviderType: ProviderTypeType,
         ProviderEndpoint: str,
-        VpcConfiguration: VpcConfigurationTypeDef = ...,
+        VpcConfiguration: VpcConfigurationUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateHostOutputTypeDef:
         """
         Creates a resource that represents the infrastructure where a third-party
         provider is installed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.create_host)
@@ -215,15 +215,15 @@
         """
 
     async def update_host(
         self,
         *,
         HostArn: str,
         ProviderEndpoint: str = ...,
-        VpcConfiguration: VpcConfigurationTypeDef = ...
+        VpcConfiguration: VpcConfigurationUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates a specified host with the provided configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.update_host)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#update_host)
         """
```

### Comparing `types-aiobotocore-codestar-connections-2.5.2/types_aiobotocore_codestar_connections/client.pyi` & `types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     CreateHostOutputTypeDef,
     GetConnectionOutputTypeDef,
     GetHostOutputTypeDef,
     ListConnectionsOutputTypeDef,
     ListHostsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagTypeDef,
-    VpcConfigurationTypeDef,
+    VpcConfigurationUnionTypeDef,
 )
 
 __all__ = ("CodeStarconnectionsClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
@@ -96,15 +96,15 @@
         """
     async def create_host(
         self,
         *,
         Name: str,
         ProviderType: ProviderTypeType,
         ProviderEndpoint: str,
-        VpcConfiguration: VpcConfigurationTypeDef = ...,
+        VpcConfiguration: VpcConfigurationUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateHostOutputTypeDef:
         """
         Creates a resource that represents the infrastructure where a third-party
         provider is installed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.create_host)
@@ -197,15 +197,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#untag_resource)
         """
     async def update_host(
         self,
         *,
         HostArn: str,
         ProviderEndpoint: str = ...,
-        VpcConfiguration: VpcConfigurationTypeDef = ...
+        VpcConfiguration: VpcConfigurationUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates a specified host with the provided configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.update_host)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#update_host)
         """
```

### Comparing `types-aiobotocore-codestar-connections-2.5.2/types_aiobotocore_codestar_connections/literals.py` & `types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-connections-2.5.2/types_aiobotocore_codestar_connections/literals.pyi` & `types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-connections-2.5.2/types_aiobotocore_codestar_connections/type_defs.py` & `types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/type_defs.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,52 +4,54 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_codestar_connections.type_defs import ConnectionTypeDef
 
-    data: ConnectionTypeDef = {...}
+    data: ConnectionTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import ConnectionStatusType, ProviderTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ConnectionTypeDef",
     "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "VpcConfigurationTypeDef",
     "DeleteConnectionInputRequestTypeDef",
     "DeleteHostInputRequestTypeDef",
     "GetConnectionInputRequestTypeDef",
     "GetHostInputRequestTypeDef",
+    "VpcConfigurationOutputTypeDef",
     "ListConnectionsInputRequestTypeDef",
     "ListHostsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "GetConnectionOutputTypeDef",
-    "ListConnectionsOutputTypeDef",
     "CreateConnectionInputRequestTypeDef",
+    "TagResourceInputRequestTypeDef",
     "CreateConnectionOutputTypeDef",
     "CreateHostOutputTypeDef",
+    "GetConnectionOutputTypeDef",
+    "ListConnectionsOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
-    "TagResourceInputRequestTypeDef",
     "CreateHostInputRequestTypeDef",
+    "UpdateHostInputRequestTypeDef",
     "GetHostOutputTypeDef",
     "HostTypeDef",
-    "UpdateHostInputRequestTypeDef",
+    "VpcConfigurationUnionTypeDef",
     "ListHostsOutputTypeDef",
 )
 
 ConnectionTypeDef = TypedDict(
     "ConnectionTypeDef",
     {
         "ConnectionName": str,
@@ -66,14 +68,25 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
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
 _RequiredVpcConfigurationTypeDef = TypedDict(
     "_RequiredVpcConfigurationTypeDef",
     {
         "VpcId": str,
         "SubnetIds": Sequence[str],
         "SecurityGroupIds": Sequence[str],
     },
@@ -115,14 +128,37 @@
 GetHostInputRequestTypeDef = TypedDict(
     "GetHostInputRequestTypeDef",
     {
         "HostArn": str,
     },
 )
 
+_RequiredVpcConfigurationOutputTypeDef = TypedDict(
+    "_RequiredVpcConfigurationOutputTypeDef",
+    {
+        "VpcId": str,
+        "SubnetIds": List[str],
+        "SecurityGroupIds": List[str],
+    },
+)
+_OptionalVpcConfigurationOutputTypeDef = TypedDict(
+    "_OptionalVpcConfigurationOutputTypeDef",
+    {
+        "TlsCertificate": str,
+    },
+    total=False,
+)
+
+
+class VpcConfigurationOutputTypeDef(
+    _RequiredVpcConfigurationOutputTypeDef, _OptionalVpcConfigurationOutputTypeDef
+):
+    pass
+
+
 ListConnectionsInputRequestTypeDef = TypedDict(
     "ListConnectionsInputRequestTypeDef",
     {
         "ProviderTypeFilter": ProviderTypeType,
         "HostArnFilter": str,
         "MaxResults": int,
         "NextToken": str,
@@ -142,50 +178,22 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
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
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-GetConnectionOutputTypeDef = TypedDict(
-    "GetConnectionOutputTypeDef",
-    {
-        "Connection": ConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListConnectionsOutputTypeDef = TypedDict(
-    "ListConnectionsOutputTypeDef",
-    {
-        "Connections": List[ConnectionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateConnectionInputRequestTypeDef = TypedDict(
     "_RequiredCreateConnectionInputRequestTypeDef",
     {
         "ConnectionName": str,
     },
 )
 _OptionalCreateConnectionInputRequestTypeDef = TypedDict(
@@ -201,45 +209,62 @@
 
 class CreateConnectionInputRequestTypeDef(
     _RequiredCreateConnectionInputRequestTypeDef, _OptionalCreateConnectionInputRequestTypeDef
 ):
     pass
 
 
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
 CreateConnectionOutputTypeDef = TypedDict(
     "CreateConnectionOutputTypeDef",
     {
         "ConnectionArn": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateHostOutputTypeDef = TypedDict(
     "CreateHostOutputTypeDef",
     {
         "HostArn": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
+GetConnectionOutputTypeDef = TypedDict(
+    "GetConnectionOutputTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Connection": ConnectionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceInputRequestTypeDef = TypedDict(
-    "TagResourceInputRequestTypeDef",
+ListConnectionsOutputTypeDef = TypedDict(
+    "ListConnectionsOutputTypeDef",
     {
-        "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
+        "Connections": List[ConnectionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateHostInputRequestTypeDef = TypedDict(
     "_RequiredCreateHostInputRequestTypeDef",
     {
         "Name": str,
@@ -259,63 +284,64 @@
 
 class CreateHostInputRequestTypeDef(
     _RequiredCreateHostInputRequestTypeDef, _OptionalCreateHostInputRequestTypeDef
 ):
     pass
 
 
+_RequiredUpdateHostInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateHostInputRequestTypeDef",
+    {
+        "HostArn": str,
+    },
+)
+_OptionalUpdateHostInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateHostInputRequestTypeDef",
+    {
+        "ProviderEndpoint": str,
+        "VpcConfiguration": VpcConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateHostInputRequestTypeDef(
+    _RequiredUpdateHostInputRequestTypeDef, _OptionalUpdateHostInputRequestTypeDef
+):
+    pass
+
+
 GetHostOutputTypeDef = TypedDict(
     "GetHostOutputTypeDef",
     {
         "Name": str,
         "Status": str,
         "ProviderType": ProviderTypeType,
         "ProviderEndpoint": str,
-        "VpcConfiguration": VpcConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VpcConfiguration": VpcConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HostTypeDef = TypedDict(
     "HostTypeDef",
     {
         "Name": str,
         "HostArn": str,
         "ProviderType": ProviderTypeType,
         "ProviderEndpoint": str,
-        "VpcConfiguration": VpcConfigurationTypeDef,
+        "VpcConfiguration": VpcConfigurationOutputTypeDef,
         "Status": str,
         "StatusMessage": str,
     },
     total=False,
 )
 
-_RequiredUpdateHostInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateHostInputRequestTypeDef",
-    {
-        "HostArn": str,
-    },
-)
-_OptionalUpdateHostInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateHostInputRequestTypeDef",
-    {
-        "ProviderEndpoint": str,
-        "VpcConfiguration": VpcConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class UpdateHostInputRequestTypeDef(
-    _RequiredUpdateHostInputRequestTypeDef, _OptionalUpdateHostInputRequestTypeDef
-):
-    pass
-
-
+VpcConfigurationUnionTypeDef = Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef]
 ListHostsOutputTypeDef = TypedDict(
     "ListHostsOutputTypeDef",
     {
         "Hosts": List[HostTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-codestar-connections-2.5.2/types_aiobotocore_codestar_connections/type_defs.pyi` & `types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/type_defs.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -4,51 +4,53 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_codestar_connections.type_defs import ConnectionTypeDef
 
-    data: ConnectionTypeDef = {...}
+    data: ConnectionTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import ConnectionStatusType, ProviderTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ConnectionTypeDef",
     "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "VpcConfigurationTypeDef",
     "DeleteConnectionInputRequestTypeDef",
     "DeleteHostInputRequestTypeDef",
     "GetConnectionInputRequestTypeDef",
     "GetHostInputRequestTypeDef",
+    "VpcConfigurationOutputTypeDef",
     "ListConnectionsInputRequestTypeDef",
     "ListHostsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "GetConnectionOutputTypeDef",
-    "ListConnectionsOutputTypeDef",
     "CreateConnectionInputRequestTypeDef",
+    "TagResourceInputRequestTypeDef",
     "CreateConnectionOutputTypeDef",
     "CreateHostOutputTypeDef",
+    "GetConnectionOutputTypeDef",
+    "ListConnectionsOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
-    "TagResourceInputRequestTypeDef",
     "CreateHostInputRequestTypeDef",
+    "UpdateHostInputRequestTypeDef",
     "GetHostOutputTypeDef",
     "HostTypeDef",
-    "UpdateHostInputRequestTypeDef",
+    "VpcConfigurationUnionTypeDef",
     "ListHostsOutputTypeDef",
 )
 
 ConnectionTypeDef = TypedDict(
     "ConnectionTypeDef",
     {
         "ConnectionName": str,
@@ -65,14 +67,25 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
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
 _RequiredVpcConfigurationTypeDef = TypedDict(
     "_RequiredVpcConfigurationTypeDef",
     {
         "VpcId": str,
         "SubnetIds": Sequence[str],
         "SecurityGroupIds": Sequence[str],
     },
@@ -112,14 +125,35 @@
 GetHostInputRequestTypeDef = TypedDict(
     "GetHostInputRequestTypeDef",
     {
         "HostArn": str,
     },
 )
 
+_RequiredVpcConfigurationOutputTypeDef = TypedDict(
+    "_RequiredVpcConfigurationOutputTypeDef",
+    {
+        "VpcId": str,
+        "SubnetIds": List[str],
+        "SecurityGroupIds": List[str],
+    },
+)
+_OptionalVpcConfigurationOutputTypeDef = TypedDict(
+    "_OptionalVpcConfigurationOutputTypeDef",
+    {
+        "TlsCertificate": str,
+    },
+    total=False,
+)
+
+class VpcConfigurationOutputTypeDef(
+    _RequiredVpcConfigurationOutputTypeDef, _OptionalVpcConfigurationOutputTypeDef
+):
+    pass
+
 ListConnectionsInputRequestTypeDef = TypedDict(
     "ListConnectionsInputRequestTypeDef",
     {
         "ProviderTypeFilter": ProviderTypeType,
         "HostArnFilter": str,
         "MaxResults": int,
         "NextToken": str,
@@ -139,50 +173,22 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
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
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-GetConnectionOutputTypeDef = TypedDict(
-    "GetConnectionOutputTypeDef",
-    {
-        "Connection": ConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListConnectionsOutputTypeDef = TypedDict(
-    "ListConnectionsOutputTypeDef",
-    {
-        "Connections": List[ConnectionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateConnectionInputRequestTypeDef = TypedDict(
     "_RequiredCreateConnectionInputRequestTypeDef",
     {
         "ConnectionName": str,
     },
 )
 _OptionalCreateConnectionInputRequestTypeDef = TypedDict(
@@ -196,45 +202,62 @@
 )
 
 class CreateConnectionInputRequestTypeDef(
     _RequiredCreateConnectionInputRequestTypeDef, _OptionalCreateConnectionInputRequestTypeDef
 ):
     pass
 
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
 CreateConnectionOutputTypeDef = TypedDict(
     "CreateConnectionOutputTypeDef",
     {
         "ConnectionArn": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateHostOutputTypeDef = TypedDict(
     "CreateHostOutputTypeDef",
     {
         "HostArn": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
+GetConnectionOutputTypeDef = TypedDict(
+    "GetConnectionOutputTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Connection": ConnectionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceInputRequestTypeDef = TypedDict(
-    "TagResourceInputRequestTypeDef",
+ListConnectionsOutputTypeDef = TypedDict(
+    "ListConnectionsOutputTypeDef",
     {
-        "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
+        "Connections": List[ConnectionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateHostInputRequestTypeDef = TypedDict(
     "_RequiredCreateHostInputRequestTypeDef",
     {
         "Name": str,
@@ -252,61 +275,62 @@
 )
 
 class CreateHostInputRequestTypeDef(
     _RequiredCreateHostInputRequestTypeDef, _OptionalCreateHostInputRequestTypeDef
 ):
     pass
 
+_RequiredUpdateHostInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateHostInputRequestTypeDef",
+    {
+        "HostArn": str,
+    },
+)
+_OptionalUpdateHostInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateHostInputRequestTypeDef",
+    {
+        "ProviderEndpoint": str,
+        "VpcConfiguration": VpcConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class UpdateHostInputRequestTypeDef(
+    _RequiredUpdateHostInputRequestTypeDef, _OptionalUpdateHostInputRequestTypeDef
+):
+    pass
+
 GetHostOutputTypeDef = TypedDict(
     "GetHostOutputTypeDef",
     {
         "Name": str,
         "Status": str,
         "ProviderType": ProviderTypeType,
         "ProviderEndpoint": str,
-        "VpcConfiguration": VpcConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VpcConfiguration": VpcConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HostTypeDef = TypedDict(
     "HostTypeDef",
     {
         "Name": str,
         "HostArn": str,
         "ProviderType": ProviderTypeType,
         "ProviderEndpoint": str,
-        "VpcConfiguration": VpcConfigurationTypeDef,
+        "VpcConfiguration": VpcConfigurationOutputTypeDef,
         "Status": str,
         "StatusMessage": str,
     },
     total=False,
 )
 
-_RequiredUpdateHostInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateHostInputRequestTypeDef",
-    {
-        "HostArn": str,
-    },
-)
-_OptionalUpdateHostInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateHostInputRequestTypeDef",
-    {
-        "ProviderEndpoint": str,
-        "VpcConfiguration": VpcConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class UpdateHostInputRequestTypeDef(
-    _RequiredUpdateHostInputRequestTypeDef, _OptionalUpdateHostInputRequestTypeDef
-):
-    pass
-
+VpcConfigurationUnionTypeDef = Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef]
 ListHostsOutputTypeDef = TypedDict(
     "ListHostsOutputTypeDef",
     {
         "Hosts": List[HostTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-codestar-connections-2.5.2/types_aiobotocore_codestar_connections.egg-info/PKG-INFO` & `types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codestar-connections
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CodeStarconnections 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CodeStarconnections 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore codestar-connections type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore codestar-connections type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-codestar-connections"></a>
 
 # types-aiobotocore-codestar-connections
 
 [![PyPI - types-aiobotocore-codestar-connections](https://img.shields.io/pypi/v/types-aiobotocore-codestar-connections.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-connections)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codestar-connections.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-connections)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codestar-connections?color=blue)](https://pypistats.org/packages/types-aiobotocore-codestar-connections)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codestar-connections)](https://pepy.tech/project/types-aiobotocore-codestar-connections)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeStarconnections 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
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
 [types-aiobotocore-codestar-connections docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/).
 
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
@@ -282,51 +281,54 @@
 )
 
 
 def check_value(value: ConnectionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codestar_connections.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from types_aiobotocore_codestar_connections.type_defs import (
     ConnectionTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     VpcConfigurationTypeDef,
     DeleteConnectionInputRequestTypeDef,
     DeleteHostInputRequestTypeDef,
     GetConnectionInputRequestTypeDef,
     GetHostInputRequestTypeDef,
+    VpcConfigurationOutputTypeDef,
     ListConnectionsInputRequestTypeDef,
     ListHostsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceInputRequestTypeDef,
-    GetConnectionOutputTypeDef,
-    ListConnectionsOutputTypeDef,
     CreateConnectionInputRequestTypeDef,
+    TagResourceInputRequestTypeDef,
     CreateConnectionOutputTypeDef,
     CreateHostOutputTypeDef,
+    GetConnectionOutputTypeDef,
+    ListConnectionsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    TagResourceInputRequestTypeDef,
     CreateHostInputRequestTypeDef,
+    UpdateHostInputRequestTypeDef,
     GetHostOutputTypeDef,
     HostTypeDef,
-    UpdateHostInputRequestTypeDef,
+    VpcConfigurationUnionTypeDef,
     ListHostsOutputTypeDef,
 )
 
 
-def get_structure() -> ConnectionTypeDef:
+def get_value() -> ConnectionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codestar-connections-2.5.2/types_aiobotocore_codestar_connections.egg-info/SOURCES.txt` & `types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-ec2-instance-connect-2.5.2.tar.gz` & `tmp/types-aiobotocore-ec2-instance-connect-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ec2-instance-connect-2.5.2.tar", last modified: Sat Jul  8 01:43:33 2023, max compression
+gzip compressed data, was "types-aiobotocore-ec2-instance-connect-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:12 2023, max compression
```

## Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.tar` & `types-aiobotocore-ec2-instance-connect-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:33.158047 types-aiobotocore-ec2-instance-connect-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:30:03.000000 types-aiobotocore-ec2-instance-connect-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12860 2023-07-08 01:43:33.158047 types-aiobotocore-ec2-instance-connect-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-07-08 01:30:03.000000 types-aiobotocore-ec2-instance-connect-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:33.158047 types-aiobotocore-ec2-instance-connect-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-08 01:30:03.000000 types-aiobotocore-ec2-instance-connect-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:33.158047 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-08 01:30:03.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-08 01:30:03.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-08 01:30:03.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-07-08 01:30:03.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-07-08 01:30:03.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-07-08 01:30:03.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-07-08 01:30:03.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:30:03.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-08 01:30:03.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-08 01:30:03.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:30:03.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:33.158047 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12860 2023-07-08 01:43:33.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-08 01:43:33.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:33.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:33.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:33.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-08 01:43:33.000000 types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.465600 types-aiobotocore-ec2-instance-connect-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:37:48.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12796 2023-08-02 14:52:12.465600 types-aiobotocore-ec2-instance-connect-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-08-02 14:37:48.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:12.465600 types-aiobotocore-ec2-instance-connect-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-08-02 14:37:48.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.457600 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-02 14:37:48.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-02 14:37:48.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-02 14:37:48.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-08-02 14:37:48.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-08-02 14:37:48.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-08-02 14:37:49.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-08-02 14:37:48.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:37:48.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-08-02 14:37:49.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-08-02 14:37:49.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:37:48.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.465600 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12796 2023-08-02 14:52:12.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:52:12.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:12.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:12.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:12.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-02 14:52:12.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2/LICENSE` & `types-aiobotocore-ec2-instance-connect-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2/PKG-INFO` & `types-aiobotocore-ec2-instance-connect-2.5.2.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ec2-instance-connect
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.EC2InstanceConnect 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.EC2InstanceConnect 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore ec2-instance-connect type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore ec2-instance-connect type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-ec2-instance-connect"></a>
 
 # types-aiobotocore-ec2-instance-connect
 
 [![PyPI - types-aiobotocore-ec2-instance-connect](https://img.shields.io/pypi/v/types-aiobotocore-ec2-instance-connect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ec2-instance-connect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ec2-instance-connect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ec2-instance-connect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ec2-instance-connect?color=blue)](https://pypistats.org/packages/types-aiobotocore-ec2-instance-connect)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ec2-instance-connect)](https://pepy.tech/project/types-aiobotocore-ec2-instance-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.EC2InstanceConnect 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
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
 [types-aiobotocore-ec2-instance-connect docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/).
 
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
@@ -279,32 +278,33 @@
 )
 
 
 def check_value(value: EC2InstanceConnectServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_ec2_instance_connect.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from types_aiobotocore_ec2_instance_connect.type_defs import (
     ResponseMetadataTypeDef,
     SendSSHPublicKeyRequestRequestTypeDef,
-    SendSSHPublicKeyResponseTypeDef,
     SendSerialConsoleSSHPublicKeyRequestRequestTypeDef,
+    SendSSHPublicKeyResponseTypeDef,
     SendSerialConsoleSSHPublicKeyResponseTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2/README.md` & `types-aiobotocore-ec2-instance-connect-2.5.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-ec2-instance-connect"></a>
 
 # types-aiobotocore-ec2-instance-connect
 
 [![PyPI - types-aiobotocore-ec2-instance-connect](https://img.shields.io/pypi/v/types-aiobotocore-ec2-instance-connect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ec2-instance-connect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ec2-instance-connect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ec2-instance-connect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ec2-instance-connect?color=blue)](https://pypistats.org/packages/types-aiobotocore-ec2-instance-connect)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ec2-instance-connect)](https://pepy.tech/project/types-aiobotocore-ec2-instance-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.EC2InstanceConnect 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
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
 [types-aiobotocore-ec2-instance-connect docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/).
 
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
@@ -246,32 +246,33 @@
 )
 
 
 def check_value(value: EC2InstanceConnectServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_ec2_instance_connect.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from types_aiobotocore_ec2_instance_connect.type_defs import (
     ResponseMetadataTypeDef,
     SendSSHPublicKeyRequestRequestTypeDef,
-    SendSSHPublicKeyResponseTypeDef,
     SendSerialConsoleSSHPublicKeyRequestRequestTypeDef,
+    SendSSHPublicKeyResponseTypeDef,
     SendSerialConsoleSSHPublicKeyResponseTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2/setup.py` & `types-aiobotocore-ec2-instance-connect-2.5.2.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,45 +6,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ec2-instance-connect",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_ec2_instance_connect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.EC2InstanceConnect 2.5.2 service generated with"
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
-        "aiobotocore ec2-instance-connect type-annotations boto3-stubs mypy typeshed autocomplete"
+        "aiobotocore ec2-instance-connect type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_ec2_instance_connect": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/",
```

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/__init__.py` & `types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/__init__.pyi` & `types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/__main__.py` & `types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EC2InstanceConnect 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.EC2InstanceConnect 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect\nOther"
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

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/client.py` & `types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/client.pyi` & `types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/literals.py` & `types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/literals.pyi` & `types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/type_defs.py` & `types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_ec2_instance_connect.type_defs import ResponseMetadataTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from typing import Dict
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ResponseMetadataTypeDef",
     "SendSSHPublicKeyRequestRequestTypeDef",
-    "SendSSHPublicKeyResponseTypeDef",
     "SendSerialConsoleSSHPublicKeyRequestRequestTypeDef",
+    "SendSSHPublicKeyResponseTypeDef",
     "SendSerialConsoleSSHPublicKeyResponseTypeDef",
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
@@ -58,23 +58,14 @@
 
 class SendSSHPublicKeyRequestRequestTypeDef(
     _RequiredSendSSHPublicKeyRequestRequestTypeDef, _OptionalSendSSHPublicKeyRequestRequestTypeDef
 ):
     pass
 
 
-SendSSHPublicKeyResponseTypeDef = TypedDict(
-    "SendSSHPublicKeyResponseTypeDef",
-    {
-        "RequestId": str,
-        "Success": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredSendSerialConsoleSSHPublicKeyRequestRequestTypeDef = TypedDict(
     "_RequiredSendSerialConsoleSSHPublicKeyRequestRequestTypeDef",
     {
         "InstanceId": str,
         "SSHPublicKey": str,
     },
 )
@@ -90,15 +81,24 @@
 class SendSerialConsoleSSHPublicKeyRequestRequestTypeDef(
     _RequiredSendSerialConsoleSSHPublicKeyRequestRequestTypeDef,
     _OptionalSendSerialConsoleSSHPublicKeyRequestRequestTypeDef,
 ):
     pass
 
 
+SendSSHPublicKeyResponseTypeDef = TypedDict(
+    "SendSSHPublicKeyResponseTypeDef",
+    {
+        "RequestId": str,
+        "Success": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 SendSerialConsoleSSHPublicKeyResponseTypeDef = TypedDict(
     "SendSerialConsoleSSHPublicKeyResponseTypeDef",
     {
         "RequestId": str,
         "Success": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect/type_defs.pyi` & `types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_ec2_instance_connect.type_defs import ResponseMetadataTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from typing import Dict
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ResponseMetadataTypeDef",
     "SendSSHPublicKeyRequestRequestTypeDef",
-    "SendSSHPublicKeyResponseTypeDef",
     "SendSerialConsoleSSHPublicKeyRequestRequestTypeDef",
+    "SendSSHPublicKeyResponseTypeDef",
     "SendSerialConsoleSSHPublicKeyResponseTypeDef",
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
@@ -55,23 +55,14 @@
 )
 
 class SendSSHPublicKeyRequestRequestTypeDef(
     _RequiredSendSSHPublicKeyRequestRequestTypeDef, _OptionalSendSSHPublicKeyRequestRequestTypeDef
 ):
     pass
 
-SendSSHPublicKeyResponseTypeDef = TypedDict(
-    "SendSSHPublicKeyResponseTypeDef",
-    {
-        "RequestId": str,
-        "Success": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredSendSerialConsoleSSHPublicKeyRequestRequestTypeDef = TypedDict(
     "_RequiredSendSerialConsoleSSHPublicKeyRequestRequestTypeDef",
     {
         "InstanceId": str,
         "SSHPublicKey": str,
     },
 )
@@ -85,15 +76,24 @@
 
 class SendSerialConsoleSSHPublicKeyRequestRequestTypeDef(
     _RequiredSendSerialConsoleSSHPublicKeyRequestRequestTypeDef,
     _OptionalSendSerialConsoleSSHPublicKeyRequestRequestTypeDef,
 ):
     pass
 
+SendSSHPublicKeyResponseTypeDef = TypedDict(
+    "SendSSHPublicKeyResponseTypeDef",
+    {
+        "RequestId": str,
+        "Success": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 SendSerialConsoleSSHPublicKeyResponseTypeDef = TypedDict(
     "SendSerialConsoleSSHPublicKeyResponseTypeDef",
     {
         "RequestId": str,
         "Success": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect.egg-info/PKG-INFO` & `types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ec2-instance-connect
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.EC2InstanceConnect 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.EC2InstanceConnect 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore ec2-instance-connect type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore ec2-instance-connect type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-ec2-instance-connect"></a>
 
 # types-aiobotocore-ec2-instance-connect
 
 [![PyPI - types-aiobotocore-ec2-instance-connect](https://img.shields.io/pypi/v/types-aiobotocore-ec2-instance-connect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ec2-instance-connect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ec2-instance-connect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ec2-instance-connect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ec2-instance-connect?color=blue)](https://pypistats.org/packages/types-aiobotocore-ec2-instance-connect)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ec2-instance-connect)](https://pepy.tech/project/types-aiobotocore-ec2-instance-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.EC2InstanceConnect 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
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
 [types-aiobotocore-ec2-instance-connect docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/).
 
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
@@ -279,32 +278,33 @@
 )
 
 
 def check_value(value: EC2InstanceConnectServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_ec2_instance_connect.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from types_aiobotocore_ec2_instance_connect.type_defs import (
     ResponseMetadataTypeDef,
     SendSSHPublicKeyRequestRequestTypeDef,
-    SendSSHPublicKeyResponseTypeDef,
     SendSerialConsoleSSHPublicKeyRequestRequestTypeDef,
+    SendSSHPublicKeyResponseTypeDef,
     SendSerialConsoleSSHPublicKeyResponseTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2/types_aiobotocore_ec2_instance_connect.egg-info/SOURCES.txt` & `types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*


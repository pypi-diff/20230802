# Comparing `tmp/types-aiobotocore-sts-2.5.2.tar.gz` & `tmp/types-aiobotocore-sts-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sts-2.5.2.tar", last modified: Sat Jul  8 01:44:23 2023, max compression
+gzip compressed data, was "types-aiobotocore-sts-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:05 2023, max compression
```

## Comparing `types-aiobotocore-sts-2.5.2.tar` & `types-aiobotocore-sts-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:23.938969 types-aiobotocore-sts-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:41:49.000000 types-aiobotocore-sts-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-07-08 01:44:23.938969 types-aiobotocore-sts-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-07-08 01:41:49.000000 types-aiobotocore-sts-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:23.938969 types-aiobotocore-sts-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-08 01:41:48.000000 types-aiobotocore-sts-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:23.934969 types-aiobotocore-sts-2.5.2/types_aiobotocore_sts/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-08 01:41:49.000000 types-aiobotocore-sts-2.5.2/types_aiobotocore_sts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-08 01:41:49.000000 types-aiobotocore-sts-2.5.2/types_aiobotocore_sts/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-08 01:41:49.000000 types-aiobotocore-sts-2.5.2/types_aiobotocore_sts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-07-08 01:41:49.000000 types-aiobotocore-sts-2.5.2/types_aiobotocore_sts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-07-08 01:41:49.000000 types-aiobotocore-sts-2.5.2/types_aiobotocore_sts/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-07-08 01:41:49.000000 types-aiobotocore-sts-2.5.2/types_aiobotocore_sts/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-07-08 01:41:49.000000 types-aiobotocore-sts-2.5.2/types_aiobotocore_sts/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:41:49.000000 types-aiobotocore-sts-2.5.2/types_aiobotocore_sts/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-07-08 01:41:49.000000 types-aiobotocore-sts-2.5.2/types_aiobotocore_sts/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-07-08 01:41:49.000000 types-aiobotocore-sts-2.5.2/types_aiobotocore_sts/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:41:49.000000 types-aiobotocore-sts-2.5.2/types_aiobotocore_sts/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:23.938969 types-aiobotocore-sts-2.5.2/types_aiobotocore_sts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-07-08 01:44:23.000000 types-aiobotocore-sts-2.5.2/types_aiobotocore_sts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-08 01:44:23.000000 types-aiobotocore-sts-2.5.2/types_aiobotocore_sts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:23.000000 types-aiobotocore-sts-2.5.2/types_aiobotocore_sts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:23.000000 types-aiobotocore-sts-2.5.2/types_aiobotocore_sts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:23.000000 types-aiobotocore-sts-2.5.2/types_aiobotocore_sts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:44:23.000000 types-aiobotocore-sts-2.5.2/types_aiobotocore_sts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:05.789443 types-aiobotocore-sts-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:24.000000 types-aiobotocore-sts-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12536 2023-08-02 14:53:05.781443 types-aiobotocore-sts-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11034 2023-08-02 14:50:24.000000 types-aiobotocore-sts-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:05.789443 types-aiobotocore-sts-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:50:24.000000 types-aiobotocore-sts-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:05.777443 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-02 14:50:24.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-02 14:50:24.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:50:24.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-08-02 14:50:24.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-08-02 14:50:24.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-08-02 14:50:24.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-08-02 14:50:24.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:24.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-08-02 14:50:24.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-08-02 14:50:24.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:24.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:05.781443 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12536 2023-08-02 14:53:05.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-02 14:53:05.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:05.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:05.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:05.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:53:05.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sts-2.5.2/LICENSE` & `types-aiobotocore-sts-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sts-2.5.2/PKG-INFO` & `types-aiobotocore-sts-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sts
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.STS 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.STS 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore sts type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore sts type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-sts"></a>
 
 # types-aiobotocore-sts
 
 [![PyPI - types-aiobotocore-sts](https://img.shields.io/pypi/v/types-aiobotocore-sts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sts)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sts?color=blue)](https://pypistats.org/packages/types-aiobotocore-sts)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sts)](https://pepy.tech/project/types-aiobotocore-sts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.STS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS)
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
 [types-aiobotocore-sts docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/).
 
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
@@ -278,48 +277,48 @@
 )
 
 
 def check_value(value: STSServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_sts.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_sts.type_defs import (
     PolicyDescriptorTypeTypeDef,
     TagTypeDef,
     AssumedRoleUserTypeDef,
     CredentialsTypeDef,
+    ResponseMetadataTypeDef,
     DecodeAuthorizationMessageRequestRequestTypeDef,
-    DecodeAuthorizationMessageResponseTypeDef,
     FederatedUserTypeDef,
     GetAccessKeyInfoRequestRequestTypeDef,
-    GetAccessKeyInfoResponseTypeDef,
-    GetCallerIdentityResponseTypeDef,
     GetSessionTokenRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     AssumeRoleWithSAMLRequestRequestTypeDef,
     AssumeRoleWithWebIdentityRequestRequestTypeDef,
     AssumeRoleRequestRequestTypeDef,
     GetFederationTokenRequestRequestTypeDef,
     AssumeRoleResponseTypeDef,
     AssumeRoleWithSAMLResponseTypeDef,
     AssumeRoleWithWebIdentityResponseTypeDef,
+    DecodeAuthorizationMessageResponseTypeDef,
+    GetAccessKeyInfoResponseTypeDef,
+    GetCallerIdentityResponseTypeDef,
     GetSessionTokenResponseTypeDef,
     GetFederationTokenResponseTypeDef,
 )
 
 
-def get_structure() -> PolicyDescriptorTypeTypeDef:
+def get_value() -> PolicyDescriptorTypeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-sts-2.5.2/README.md` & `types-aiobotocore-sts-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-sts"></a>
 
 # types-aiobotocore-sts
 
 [![PyPI - types-aiobotocore-sts](https://img.shields.io/pypi/v/types-aiobotocore-sts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sts)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sts?color=blue)](https://pypistats.org/packages/types-aiobotocore-sts)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sts)](https://pepy.tech/project/types-aiobotocore-sts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.STS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS)
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
 [types-aiobotocore-sts docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/).
 
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
@@ -245,48 +245,48 @@
 )
 
 
 def check_value(value: STSServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_sts.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_sts.type_defs import (
     PolicyDescriptorTypeTypeDef,
     TagTypeDef,
     AssumedRoleUserTypeDef,
     CredentialsTypeDef,
+    ResponseMetadataTypeDef,
     DecodeAuthorizationMessageRequestRequestTypeDef,
-    DecodeAuthorizationMessageResponseTypeDef,
     FederatedUserTypeDef,
     GetAccessKeyInfoRequestRequestTypeDef,
-    GetAccessKeyInfoResponseTypeDef,
-    GetCallerIdentityResponseTypeDef,
     GetSessionTokenRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     AssumeRoleWithSAMLRequestRequestTypeDef,
     AssumeRoleWithWebIdentityRequestRequestTypeDef,
     AssumeRoleRequestRequestTypeDef,
     GetFederationTokenRequestRequestTypeDef,
     AssumeRoleResponseTypeDef,
     AssumeRoleWithSAMLResponseTypeDef,
     AssumeRoleWithWebIdentityResponseTypeDef,
+    DecodeAuthorizationMessageResponseTypeDef,
+    GetAccessKeyInfoResponseTypeDef,
+    GetCallerIdentityResponseTypeDef,
     GetSessionTokenResponseTypeDef,
     GetFederationTokenResponseTypeDef,
 )
 
 
-def get_structure() -> PolicyDescriptorTypeTypeDef:
+def get_value() -> PolicyDescriptorTypeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-sts-2.5.2/setup.py` & `types-aiobotocore-sts-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sts",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_sts"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.STS 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore sts type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore sts type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_sts": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-sts-2.5.2/types_aiobotocore_sts/__main__.py` & `types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.STS 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.STS 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS\nOther"
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

### Comparing `types-aiobotocore-sts-2.5.2/types_aiobotocore_sts/client.py` & `types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sts-2.5.2/types_aiobotocore_sts/client.pyi` & `types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sts-2.5.2/types_aiobotocore_sts/literals.py` & `types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sts-2.5.2/types_aiobotocore_sts/literals.pyi` & `types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sts-2.5.2/types_aiobotocore_sts/type_defs.py` & `types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_sts.type_defs import PolicyDescriptorTypeTypeDef
 
-    data: PolicyDescriptorTypeTypeDef = {...}
+    data: PolicyDescriptorTypeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, Sequence
 
 if sys.version_info >= (3, 9):
@@ -22,29 +22,29 @@
 
 
 __all__ = (
     "PolicyDescriptorTypeTypeDef",
     "TagTypeDef",
     "AssumedRoleUserTypeDef",
     "CredentialsTypeDef",
+    "ResponseMetadataTypeDef",
     "DecodeAuthorizationMessageRequestRequestTypeDef",
-    "DecodeAuthorizationMessageResponseTypeDef",
     "FederatedUserTypeDef",
     "GetAccessKeyInfoRequestRequestTypeDef",
-    "GetAccessKeyInfoResponseTypeDef",
-    "GetCallerIdentityResponseTypeDef",
     "GetSessionTokenRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "AssumeRoleWithSAMLRequestRequestTypeDef",
     "AssumeRoleWithWebIdentityRequestRequestTypeDef",
     "AssumeRoleRequestRequestTypeDef",
     "GetFederationTokenRequestRequestTypeDef",
     "AssumeRoleResponseTypeDef",
     "AssumeRoleWithSAMLResponseTypeDef",
     "AssumeRoleWithWebIdentityResponseTypeDef",
+    "DecodeAuthorizationMessageResponseTypeDef",
+    "GetAccessKeyInfoResponseTypeDef",
+    "GetCallerIdentityResponseTypeDef",
     "GetSessionTokenResponseTypeDef",
     "GetFederationTokenResponseTypeDef",
 )
 
 PolicyDescriptorTypeTypeDef = TypedDict(
     "PolicyDescriptorTypeTypeDef",
     {
@@ -75,26 +75,29 @@
         "AccessKeyId": str,
         "SecretAccessKey": str,
         "SessionToken": str,
         "Expiration": datetime,
     },
 )
 
-DecodeAuthorizationMessageRequestRequestTypeDef = TypedDict(
-    "DecodeAuthorizationMessageRequestRequestTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "EncodedMessage": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-DecodeAuthorizationMessageResponseTypeDef = TypedDict(
-    "DecodeAuthorizationMessageResponseTypeDef",
+DecodeAuthorizationMessageRequestRequestTypeDef = TypedDict(
+    "DecodeAuthorizationMessageRequestRequestTypeDef",
     {
-        "DecodedMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "EncodedMessage": str,
     },
 )
 
 FederatedUserTypeDef = TypedDict(
     "FederatedUserTypeDef",
     {
         "FederatedUserId": str,
@@ -105,53 +108,24 @@
 GetAccessKeyInfoRequestRequestTypeDef = TypedDict(
     "GetAccessKeyInfoRequestRequestTypeDef",
     {
         "AccessKeyId": str,
     },
 )
 
-GetAccessKeyInfoResponseTypeDef = TypedDict(
-    "GetAccessKeyInfoResponseTypeDef",
-    {
-        "Account": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetCallerIdentityResponseTypeDef = TypedDict(
-    "GetCallerIdentityResponseTypeDef",
-    {
-        "UserId": str,
-        "Account": str,
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSessionTokenRequestRequestTypeDef = TypedDict(
     "GetSessionTokenRequestRequestTypeDef",
     {
         "DurationSeconds": int,
         "SerialNumber": str,
         "TokenCode": str,
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
 _RequiredAssumeRoleWithSAMLRequestRequestTypeDef = TypedDict(
     "_RequiredAssumeRoleWithSAMLRequestRequestTypeDef",
     {
         "RoleArn": str,
         "PrincipalArn": str,
         "SAMLAssertion": str,
     },
@@ -259,15 +233,15 @@
 AssumeRoleResponseTypeDef = TypedDict(
     "AssumeRoleResponseTypeDef",
     {
         "Credentials": CredentialsTypeDef,
         "AssumedRoleUser": AssumedRoleUserTypeDef,
         "PackedPolicySize": int,
         "SourceIdentity": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssumeRoleWithSAMLResponseTypeDef = TypedDict(
     "AssumeRoleWithSAMLResponseTypeDef",
     {
         "Credentials": CredentialsTypeDef,
@@ -275,42 +249,68 @@
         "PackedPolicySize": int,
         "Subject": str,
         "SubjectType": str,
         "Issuer": str,
         "Audience": str,
         "NameQualifier": str,
         "SourceIdentity": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssumeRoleWithWebIdentityResponseTypeDef = TypedDict(
     "AssumeRoleWithWebIdentityResponseTypeDef",
     {
         "Credentials": CredentialsTypeDef,
         "SubjectFromWebIdentityToken": str,
         "AssumedRoleUser": AssumedRoleUserTypeDef,
         "PackedPolicySize": int,
         "Provider": str,
         "Audience": str,
         "SourceIdentity": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DecodeAuthorizationMessageResponseTypeDef = TypedDict(
+    "DecodeAuthorizationMessageResponseTypeDef",
+    {
+        "DecodedMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccessKeyInfoResponseTypeDef = TypedDict(
+    "GetAccessKeyInfoResponseTypeDef",
+    {
+        "Account": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCallerIdentityResponseTypeDef = TypedDict(
+    "GetCallerIdentityResponseTypeDef",
+    {
+        "UserId": str,
+        "Account": str,
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSessionTokenResponseTypeDef = TypedDict(
     "GetSessionTokenResponseTypeDef",
     {
         "Credentials": CredentialsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFederationTokenResponseTypeDef = TypedDict(
     "GetFederationTokenResponseTypeDef",
     {
         "Credentials": CredentialsTypeDef,
         "FederatedUser": FederatedUserTypeDef,
         "PackedPolicySize": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-sts-2.5.2/types_aiobotocore_sts/type_defs.pyi` & `types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_sts.type_defs import PolicyDescriptorTypeTypeDef
 
-    data: PolicyDescriptorTypeTypeDef = {...}
+    data: PolicyDescriptorTypeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, Sequence
 
 if sys.version_info >= (3, 9):
@@ -21,29 +21,29 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "PolicyDescriptorTypeTypeDef",
     "TagTypeDef",
     "AssumedRoleUserTypeDef",
     "CredentialsTypeDef",
+    "ResponseMetadataTypeDef",
     "DecodeAuthorizationMessageRequestRequestTypeDef",
-    "DecodeAuthorizationMessageResponseTypeDef",
     "FederatedUserTypeDef",
     "GetAccessKeyInfoRequestRequestTypeDef",
-    "GetAccessKeyInfoResponseTypeDef",
-    "GetCallerIdentityResponseTypeDef",
     "GetSessionTokenRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "AssumeRoleWithSAMLRequestRequestTypeDef",
     "AssumeRoleWithWebIdentityRequestRequestTypeDef",
     "AssumeRoleRequestRequestTypeDef",
     "GetFederationTokenRequestRequestTypeDef",
     "AssumeRoleResponseTypeDef",
     "AssumeRoleWithSAMLResponseTypeDef",
     "AssumeRoleWithWebIdentityResponseTypeDef",
+    "DecodeAuthorizationMessageResponseTypeDef",
+    "GetAccessKeyInfoResponseTypeDef",
+    "GetCallerIdentityResponseTypeDef",
     "GetSessionTokenResponseTypeDef",
     "GetFederationTokenResponseTypeDef",
 )
 
 PolicyDescriptorTypeTypeDef = TypedDict(
     "PolicyDescriptorTypeTypeDef",
     {
@@ -74,26 +74,29 @@
         "AccessKeyId": str,
         "SecretAccessKey": str,
         "SessionToken": str,
         "Expiration": datetime,
     },
 )
 
-DecodeAuthorizationMessageRequestRequestTypeDef = TypedDict(
-    "DecodeAuthorizationMessageRequestRequestTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "EncodedMessage": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-DecodeAuthorizationMessageResponseTypeDef = TypedDict(
-    "DecodeAuthorizationMessageResponseTypeDef",
+DecodeAuthorizationMessageRequestRequestTypeDef = TypedDict(
+    "DecodeAuthorizationMessageRequestRequestTypeDef",
     {
-        "DecodedMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "EncodedMessage": str,
     },
 )
 
 FederatedUserTypeDef = TypedDict(
     "FederatedUserTypeDef",
     {
         "FederatedUserId": str,
@@ -104,53 +107,24 @@
 GetAccessKeyInfoRequestRequestTypeDef = TypedDict(
     "GetAccessKeyInfoRequestRequestTypeDef",
     {
         "AccessKeyId": str,
     },
 )
 
-GetAccessKeyInfoResponseTypeDef = TypedDict(
-    "GetAccessKeyInfoResponseTypeDef",
-    {
-        "Account": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetCallerIdentityResponseTypeDef = TypedDict(
-    "GetCallerIdentityResponseTypeDef",
-    {
-        "UserId": str,
-        "Account": str,
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSessionTokenRequestRequestTypeDef = TypedDict(
     "GetSessionTokenRequestRequestTypeDef",
     {
         "DurationSeconds": int,
         "SerialNumber": str,
         "TokenCode": str,
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
 _RequiredAssumeRoleWithSAMLRequestRequestTypeDef = TypedDict(
     "_RequiredAssumeRoleWithSAMLRequestRequestTypeDef",
     {
         "RoleArn": str,
         "PrincipalArn": str,
         "SAMLAssertion": str,
     },
@@ -250,15 +224,15 @@
 AssumeRoleResponseTypeDef = TypedDict(
     "AssumeRoleResponseTypeDef",
     {
         "Credentials": CredentialsTypeDef,
         "AssumedRoleUser": AssumedRoleUserTypeDef,
         "PackedPolicySize": int,
         "SourceIdentity": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssumeRoleWithSAMLResponseTypeDef = TypedDict(
     "AssumeRoleWithSAMLResponseTypeDef",
     {
         "Credentials": CredentialsTypeDef,
@@ -266,42 +240,68 @@
         "PackedPolicySize": int,
         "Subject": str,
         "SubjectType": str,
         "Issuer": str,
         "Audience": str,
         "NameQualifier": str,
         "SourceIdentity": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssumeRoleWithWebIdentityResponseTypeDef = TypedDict(
     "AssumeRoleWithWebIdentityResponseTypeDef",
     {
         "Credentials": CredentialsTypeDef,
         "SubjectFromWebIdentityToken": str,
         "AssumedRoleUser": AssumedRoleUserTypeDef,
         "PackedPolicySize": int,
         "Provider": str,
         "Audience": str,
         "SourceIdentity": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DecodeAuthorizationMessageResponseTypeDef = TypedDict(
+    "DecodeAuthorizationMessageResponseTypeDef",
+    {
+        "DecodedMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccessKeyInfoResponseTypeDef = TypedDict(
+    "GetAccessKeyInfoResponseTypeDef",
+    {
+        "Account": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCallerIdentityResponseTypeDef = TypedDict(
+    "GetCallerIdentityResponseTypeDef",
+    {
+        "UserId": str,
+        "Account": str,
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSessionTokenResponseTypeDef = TypedDict(
     "GetSessionTokenResponseTypeDef",
     {
         "Credentials": CredentialsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFederationTokenResponseTypeDef = TypedDict(
     "GetFederationTokenResponseTypeDef",
     {
         "Credentials": CredentialsTypeDef,
         "FederatedUser": FederatedUserTypeDef,
         "PackedPolicySize": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-sts-2.5.2/types_aiobotocore_sts.egg-info/PKG-INFO` & `types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sts
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.STS 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.STS 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore sts type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore sts type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-sts"></a>
 
 # types-aiobotocore-sts
 
 [![PyPI - types-aiobotocore-sts](https://img.shields.io/pypi/v/types-aiobotocore-sts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sts)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sts?color=blue)](https://pypistats.org/packages/types-aiobotocore-sts)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sts)](https://pepy.tech/project/types-aiobotocore-sts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.STS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS)
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
 [types-aiobotocore-sts docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/).
 
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
@@ -278,48 +277,48 @@
 )
 
 
 def check_value(value: STSServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_sts.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_sts.type_defs import (
     PolicyDescriptorTypeTypeDef,
     TagTypeDef,
     AssumedRoleUserTypeDef,
     CredentialsTypeDef,
+    ResponseMetadataTypeDef,
     DecodeAuthorizationMessageRequestRequestTypeDef,
-    DecodeAuthorizationMessageResponseTypeDef,
     FederatedUserTypeDef,
     GetAccessKeyInfoRequestRequestTypeDef,
-    GetAccessKeyInfoResponseTypeDef,
-    GetCallerIdentityResponseTypeDef,
     GetSessionTokenRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     AssumeRoleWithSAMLRequestRequestTypeDef,
     AssumeRoleWithWebIdentityRequestRequestTypeDef,
     AssumeRoleRequestRequestTypeDef,
     GetFederationTokenRequestRequestTypeDef,
     AssumeRoleResponseTypeDef,
     AssumeRoleWithSAMLResponseTypeDef,
     AssumeRoleWithWebIdentityResponseTypeDef,
+    DecodeAuthorizationMessageResponseTypeDef,
+    GetAccessKeyInfoResponseTypeDef,
+    GetCallerIdentityResponseTypeDef,
     GetSessionTokenResponseTypeDef,
     GetFederationTokenResponseTypeDef,
 )
 
 
-def get_structure() -> PolicyDescriptorTypeTypeDef:
+def get_value() -> PolicyDescriptorTypeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-sts-2.5.2/types_aiobotocore_sts.egg-info/SOURCES.txt` & `types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts.egg-info/SOURCES.txt`

 * *Files identical despite different names*


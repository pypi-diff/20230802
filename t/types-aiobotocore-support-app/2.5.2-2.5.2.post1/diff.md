# Comparing `tmp/types-aiobotocore-support-app-2.5.2.tar.gz` & `tmp/types-aiobotocore-support-app-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-support-app-2.5.2.tar", last modified: Sat Jul  8 01:44:24 2023, max compression
+gzip compressed data, was "types-aiobotocore-support-app-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:06 2023, max compression
```

## Comparing `types-aiobotocore-support-app-2.5.2.tar` & `types-aiobotocore-support-app-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:24.310976 types-aiobotocore-support-app-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:41:50.000000 types-aiobotocore-support-app-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13093 2023-07-08 01:44:24.310976 types-aiobotocore-support-app-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11513 2023-07-08 01:41:50.000000 types-aiobotocore-support-app-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:24.310976 types-aiobotocore-support-app-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-08 01:41:50.000000 types-aiobotocore-support-app-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:24.306976 types-aiobotocore-support-app-2.5.2/types_aiobotocore_support_app/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-08 01:41:50.000000 types-aiobotocore-support-app-2.5.2/types_aiobotocore_support_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-08 01:41:50.000000 types-aiobotocore-support-app-2.5.2/types_aiobotocore_support_app/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-08 01:41:50.000000 types-aiobotocore-support-app-2.5.2/types_aiobotocore_support_app/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10743 2023-07-08 01:41:50.000000 types-aiobotocore-support-app-2.5.2/types_aiobotocore_support_app/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-07-08 01:41:50.000000 types-aiobotocore-support-app-2.5.2/types_aiobotocore_support_app/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-07-08 01:41:51.000000 types-aiobotocore-support-app-2.5.2/types_aiobotocore_support_app/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-07-08 01:41:50.000000 types-aiobotocore-support-app-2.5.2/types_aiobotocore_support_app/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:41:50.000000 types-aiobotocore-support-app-2.5.2/types_aiobotocore_support_app/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-07-08 01:41:51.000000 types-aiobotocore-support-app-2.5.2/types_aiobotocore_support_app/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-07-08 01:41:51.000000 types-aiobotocore-support-app-2.5.2/types_aiobotocore_support_app/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:41:50.000000 types-aiobotocore-support-app-2.5.2/types_aiobotocore_support_app/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:24.310976 types-aiobotocore-support-app-2.5.2/types_aiobotocore_support_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13093 2023-07-08 01:44:24.000000 types-aiobotocore-support-app-2.5.2/types_aiobotocore_support_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-08 01:44:24.000000 types-aiobotocore-support-app-2.5.2/types_aiobotocore_support_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:24.000000 types-aiobotocore-support-app-2.5.2/types_aiobotocore_support_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:24.000000 types-aiobotocore-support-app-2.5.2/types_aiobotocore_support_app.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:24.000000 types-aiobotocore-support-app-2.5.2/types_aiobotocore_support_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-08 01:44:24.000000 types-aiobotocore-support-app-2.5.2/types_aiobotocore_support_app.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.273441 types-aiobotocore-support-app-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:25.000000 types-aiobotocore-support-app-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-08-02 14:53:06.273441 types-aiobotocore-support-app-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11496 2023-08-02 14:50:25.000000 types-aiobotocore-support-app-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:06.273441 types-aiobotocore-support-app-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-08-02 14:50:25.000000 types-aiobotocore-support-app-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.273441 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-02 14:50:25.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-02 14:50:25.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-02 14:50:25.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10743 2023-08-02 14:50:25.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-08-02 14:50:25.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-08-02 14:50:25.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-08-02 14:50:25.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:25.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7155 2023-08-02 14:50:26.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-08-02 14:50:26.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:25.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.273441 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-08-02 14:53:06.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-02 14:53:06.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:06.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:06.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:06.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 14:53:06.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-support-app-2.5.2/LICENSE` & `types-aiobotocore-support-app-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-app-2.5.2/PKG-INFO` & `types-aiobotocore-support-app-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-support-app
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SupportApp 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SupportApp 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore support-app type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore support-app type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-support-app"></a>
 
 # types-aiobotocore-support-app
 
 [![PyPI - types-aiobotocore-support-app](https://img.shields.io/pypi/v/types-aiobotocore-support-app.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support-app)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-support-app.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support-app)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-support-app?color=blue)](https://pypistats.org/packages/types-aiobotocore-support-app)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-support-app)](https://pepy.tech/project/types-aiobotocore-support-app)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SupportApp 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp)
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
 [types-aiobotocore-support-app docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/).
 
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
@@ -282,43 +281,43 @@
 )
 
 
 def check_value(value: AccountTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_support_app.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_support_app.type_defs import (
     CreateSlackChannelConfigurationRequestRequestTypeDef,
     DeleteSlackChannelConfigurationRequestRequestTypeDef,
     DeleteSlackWorkspaceConfigurationRequestRequestTypeDef,
-    GetAccountAliasResultTypeDef,
+    ResponseMetadataTypeDef,
     ListSlackChannelConfigurationsRequestRequestTypeDef,
     SlackChannelConfigurationTypeDef,
     ListSlackWorkspaceConfigurationsRequestRequestTypeDef,
     SlackWorkspaceConfigurationTypeDef,
     PutAccountAliasRequestRequestTypeDef,
     RegisterSlackWorkspaceForOrganizationRequestRequestTypeDef,
-    RegisterSlackWorkspaceForOrganizationResultTypeDef,
-    ResponseMetadataTypeDef,
     UpdateSlackChannelConfigurationRequestRequestTypeDef,
+    GetAccountAliasResultTypeDef,
+    RegisterSlackWorkspaceForOrganizationResultTypeDef,
     UpdateSlackChannelConfigurationResultTypeDef,
     ListSlackChannelConfigurationsResultTypeDef,
     ListSlackWorkspaceConfigurationsResultTypeDef,
 )
 
 
-def get_structure() -> CreateSlackChannelConfigurationRequestRequestTypeDef:
+def get_value() -> CreateSlackChannelConfigurationRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-support-app-2.5.2/README.md` & `types-aiobotocore-support-app-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-support-app"></a>
 
 # types-aiobotocore-support-app
 
 [![PyPI - types-aiobotocore-support-app](https://img.shields.io/pypi/v/types-aiobotocore-support-app.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support-app)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-support-app.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support-app)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-support-app?color=blue)](https://pypistats.org/packages/types-aiobotocore-support-app)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-support-app)](https://pepy.tech/project/types-aiobotocore-support-app)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SupportApp 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp)
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
 [types-aiobotocore-support-app docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/).
 
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
@@ -249,43 +249,43 @@
 )
 
 
 def check_value(value: AccountTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_support_app.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_support_app.type_defs import (
     CreateSlackChannelConfigurationRequestRequestTypeDef,
     DeleteSlackChannelConfigurationRequestRequestTypeDef,
     DeleteSlackWorkspaceConfigurationRequestRequestTypeDef,
-    GetAccountAliasResultTypeDef,
+    ResponseMetadataTypeDef,
     ListSlackChannelConfigurationsRequestRequestTypeDef,
     SlackChannelConfigurationTypeDef,
     ListSlackWorkspaceConfigurationsRequestRequestTypeDef,
     SlackWorkspaceConfigurationTypeDef,
     PutAccountAliasRequestRequestTypeDef,
     RegisterSlackWorkspaceForOrganizationRequestRequestTypeDef,
-    RegisterSlackWorkspaceForOrganizationResultTypeDef,
-    ResponseMetadataTypeDef,
     UpdateSlackChannelConfigurationRequestRequestTypeDef,
+    GetAccountAliasResultTypeDef,
+    RegisterSlackWorkspaceForOrganizationResultTypeDef,
     UpdateSlackChannelConfigurationResultTypeDef,
     ListSlackChannelConfigurationsResultTypeDef,
     ListSlackWorkspaceConfigurationsResultTypeDef,
 )
 
 
-def get_structure() -> CreateSlackChannelConfigurationRequestRequestTypeDef:
+def get_value() -> CreateSlackChannelConfigurationRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-support-app-2.5.2/setup.py` & `types-aiobotocore-support-app-2.5.2.post1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-support-app",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_support_app"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SupportApp 2.5.2 service generated with"
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
-    keywords="aiobotocore support-app type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore support-app type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_support_app": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/"
```

### Comparing `types-aiobotocore-support-app-2.5.2/types_aiobotocore_support_app/__main__.py` & `types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SupportApp 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.SupportApp 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp\nOther"
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

### Comparing `types-aiobotocore-support-app-2.5.2/types_aiobotocore_support_app/client.py` & `types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-app-2.5.2/types_aiobotocore_support_app/client.pyi` & `types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-app-2.5.2/types_aiobotocore_support_app/literals.py` & `types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-app-2.5.2/types_aiobotocore_support_app/literals.pyi` & `types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-app-2.5.2/types_aiobotocore_support_app/type_defs.py` & `types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,42 +4,41 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_support_app.type_defs import CreateSlackChannelConfigurationRequestRequestTypeDef
 
-    data: CreateSlackChannelConfigurationRequestRequestTypeDef = {...}
+    data: CreateSlackChannelConfigurationRequestRequestTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List
 
 from .literals import AccountTypeType, NotificationSeverityLevelType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CreateSlackChannelConfigurationRequestRequestTypeDef",
     "DeleteSlackChannelConfigurationRequestRequestTypeDef",
     "DeleteSlackWorkspaceConfigurationRequestRequestTypeDef",
-    "GetAccountAliasResultTypeDef",
+    "ResponseMetadataTypeDef",
     "ListSlackChannelConfigurationsRequestRequestTypeDef",
     "SlackChannelConfigurationTypeDef",
     "ListSlackWorkspaceConfigurationsRequestRequestTypeDef",
     "SlackWorkspaceConfigurationTypeDef",
     "PutAccountAliasRequestRequestTypeDef",
     "RegisterSlackWorkspaceForOrganizationRequestRequestTypeDef",
-    "RegisterSlackWorkspaceForOrganizationResultTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateSlackChannelConfigurationRequestRequestTypeDef",
+    "GetAccountAliasResultTypeDef",
+    "RegisterSlackWorkspaceForOrganizationResultTypeDef",
     "UpdateSlackChannelConfigurationResultTypeDef",
     "ListSlackChannelConfigurationsResultTypeDef",
     "ListSlackWorkspaceConfigurationsResultTypeDef",
 )
 
 _RequiredCreateSlackChannelConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSlackChannelConfigurationRequestRequestTypeDef",
@@ -57,22 +56,20 @@
         "notifyOnAddCorrespondenceToCase": bool,
         "notifyOnCreateOrReopenCase": bool,
         "notifyOnResolveCase": bool,
     },
     total=False,
 )
 
-
 class CreateSlackChannelConfigurationRequestRequestTypeDef(
     _RequiredCreateSlackChannelConfigurationRequestRequestTypeDef,
     _OptionalCreateSlackChannelConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteSlackChannelConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteSlackChannelConfigurationRequestRequestTypeDef",
     {
         "channelId": str,
         "teamId": str,
     },
 )
@@ -80,19 +77,22 @@
 DeleteSlackWorkspaceConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteSlackWorkspaceConfigurationRequestRequestTypeDef",
     {
         "teamId": str,
     },
 )
 
-GetAccountAliasResultTypeDef = TypedDict(
-    "GetAccountAliasResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "accountAlias": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ListSlackChannelConfigurationsRequestRequestTypeDef = TypedDict(
     "ListSlackChannelConfigurationsRequestRequestTypeDef",
     {
         "nextToken": str,
@@ -116,21 +116,19 @@
         "notifyOnCaseSeverity": NotificationSeverityLevelType,
         "notifyOnCreateOrReopenCase": bool,
         "notifyOnResolveCase": bool,
     },
     total=False,
 )
 
-
 class SlackChannelConfigurationTypeDef(
     _RequiredSlackChannelConfigurationTypeDef, _OptionalSlackChannelConfigurationTypeDef
 ):
     pass
 
-
 ListSlackWorkspaceConfigurationsRequestRequestTypeDef = TypedDict(
     "ListSlackWorkspaceConfigurationsRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
@@ -146,56 +144,33 @@
     {
         "allowOrganizationMemberAccount": bool,
         "teamName": str,
     },
     total=False,
 )
 
-
 class SlackWorkspaceConfigurationTypeDef(
     _RequiredSlackWorkspaceConfigurationTypeDef, _OptionalSlackWorkspaceConfigurationTypeDef
 ):
     pass
 
-
 PutAccountAliasRequestRequestTypeDef = TypedDict(
     "PutAccountAliasRequestRequestTypeDef",
     {
         "accountAlias": str,
     },
 )
 
 RegisterSlackWorkspaceForOrganizationRequestRequestTypeDef = TypedDict(
     "RegisterSlackWorkspaceForOrganizationRequestRequestTypeDef",
     {
         "teamId": str,
     },
 )
 
-RegisterSlackWorkspaceForOrganizationResultTypeDef = TypedDict(
-    "RegisterSlackWorkspaceForOrganizationResultTypeDef",
-    {
-        "accountType": AccountTypeType,
-        "teamId": str,
-        "teamName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
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
 _RequiredUpdateSlackChannelConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSlackChannelConfigurationRequestRequestTypeDef",
     {
         "channelId": str,
         "teamId": str,
     },
 )
@@ -208,47 +183,63 @@
         "notifyOnCaseSeverity": NotificationSeverityLevelType,
         "notifyOnCreateOrReopenCase": bool,
         "notifyOnResolveCase": bool,
     },
     total=False,
 )
 
-
 class UpdateSlackChannelConfigurationRequestRequestTypeDef(
     _RequiredUpdateSlackChannelConfigurationRequestRequestTypeDef,
     _OptionalUpdateSlackChannelConfigurationRequestRequestTypeDef,
 ):
     pass
 
+GetAccountAliasResultTypeDef = TypedDict(
+    "GetAccountAliasResultTypeDef",
+    {
+        "accountAlias": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterSlackWorkspaceForOrganizationResultTypeDef = TypedDict(
+    "RegisterSlackWorkspaceForOrganizationResultTypeDef",
+    {
+        "accountType": AccountTypeType,
+        "teamId": str,
+        "teamName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 UpdateSlackChannelConfigurationResultTypeDef = TypedDict(
     "UpdateSlackChannelConfigurationResultTypeDef",
     {
         "channelId": str,
         "channelName": str,
         "channelRoleArn": str,
         "notifyOnAddCorrespondenceToCase": bool,
         "notifyOnCaseSeverity": NotificationSeverityLevelType,
         "notifyOnCreateOrReopenCase": bool,
         "notifyOnResolveCase": bool,
         "teamId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSlackChannelConfigurationsResultTypeDef = TypedDict(
     "ListSlackChannelConfigurationsResultTypeDef",
     {
         "nextToken": str,
         "slackChannelConfigurations": List[SlackChannelConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSlackWorkspaceConfigurationsResultTypeDef = TypedDict(
     "ListSlackWorkspaceConfigurationsResultTypeDef",
     {
         "nextToken": str,
         "slackWorkspaceConfigurations": List[SlackWorkspaceConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-support-app-2.5.2/types_aiobotocore_support_app/type_defs.pyi` & `types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,41 +4,42 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_support_app.type_defs import CreateSlackChannelConfigurationRequestRequestTypeDef
 
-    data: CreateSlackChannelConfigurationRequestRequestTypeDef = {...}
+    data: CreateSlackChannelConfigurationRequestRequestTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List
 
 from .literals import AccountTypeType, NotificationSeverityLevelType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CreateSlackChannelConfigurationRequestRequestTypeDef",
     "DeleteSlackChannelConfigurationRequestRequestTypeDef",
     "DeleteSlackWorkspaceConfigurationRequestRequestTypeDef",
-    "GetAccountAliasResultTypeDef",
+    "ResponseMetadataTypeDef",
     "ListSlackChannelConfigurationsRequestRequestTypeDef",
     "SlackChannelConfigurationTypeDef",
     "ListSlackWorkspaceConfigurationsRequestRequestTypeDef",
     "SlackWorkspaceConfigurationTypeDef",
     "PutAccountAliasRequestRequestTypeDef",
     "RegisterSlackWorkspaceForOrganizationRequestRequestTypeDef",
-    "RegisterSlackWorkspaceForOrganizationResultTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateSlackChannelConfigurationRequestRequestTypeDef",
+    "GetAccountAliasResultTypeDef",
+    "RegisterSlackWorkspaceForOrganizationResultTypeDef",
     "UpdateSlackChannelConfigurationResultTypeDef",
     "ListSlackChannelConfigurationsResultTypeDef",
     "ListSlackWorkspaceConfigurationsResultTypeDef",
 )
 
 _RequiredCreateSlackChannelConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSlackChannelConfigurationRequestRequestTypeDef",
@@ -56,20 +57,22 @@
         "notifyOnAddCorrespondenceToCase": bool,
         "notifyOnCreateOrReopenCase": bool,
         "notifyOnResolveCase": bool,
     },
     total=False,
 )
 
+
 class CreateSlackChannelConfigurationRequestRequestTypeDef(
     _RequiredCreateSlackChannelConfigurationRequestRequestTypeDef,
     _OptionalCreateSlackChannelConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteSlackChannelConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteSlackChannelConfigurationRequestRequestTypeDef",
     {
         "channelId": str,
         "teamId": str,
     },
 )
@@ -77,19 +80,22 @@
 DeleteSlackWorkspaceConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteSlackWorkspaceConfigurationRequestRequestTypeDef",
     {
         "teamId": str,
     },
 )
 
-GetAccountAliasResultTypeDef = TypedDict(
-    "GetAccountAliasResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "accountAlias": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ListSlackChannelConfigurationsRequestRequestTypeDef = TypedDict(
     "ListSlackChannelConfigurationsRequestRequestTypeDef",
     {
         "nextToken": str,
@@ -113,19 +119,21 @@
         "notifyOnCaseSeverity": NotificationSeverityLevelType,
         "notifyOnCreateOrReopenCase": bool,
         "notifyOnResolveCase": bool,
     },
     total=False,
 )
 
+
 class SlackChannelConfigurationTypeDef(
     _RequiredSlackChannelConfigurationTypeDef, _OptionalSlackChannelConfigurationTypeDef
 ):
     pass
 
+
 ListSlackWorkspaceConfigurationsRequestRequestTypeDef = TypedDict(
     "ListSlackWorkspaceConfigurationsRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
@@ -141,54 +149,35 @@
     {
         "allowOrganizationMemberAccount": bool,
         "teamName": str,
     },
     total=False,
 )
 
+
 class SlackWorkspaceConfigurationTypeDef(
     _RequiredSlackWorkspaceConfigurationTypeDef, _OptionalSlackWorkspaceConfigurationTypeDef
 ):
     pass
 
+
 PutAccountAliasRequestRequestTypeDef = TypedDict(
     "PutAccountAliasRequestRequestTypeDef",
     {
         "accountAlias": str,
     },
 )
 
 RegisterSlackWorkspaceForOrganizationRequestRequestTypeDef = TypedDict(
     "RegisterSlackWorkspaceForOrganizationRequestRequestTypeDef",
     {
         "teamId": str,
     },
 )
 
-RegisterSlackWorkspaceForOrganizationResultTypeDef = TypedDict(
-    "RegisterSlackWorkspaceForOrganizationResultTypeDef",
-    {
-        "accountType": AccountTypeType,
-        "teamId": str,
-        "teamName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
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
 _RequiredUpdateSlackChannelConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSlackChannelConfigurationRequestRequestTypeDef",
     {
         "channelId": str,
         "teamId": str,
     },
 )
@@ -201,45 +190,65 @@
         "notifyOnCaseSeverity": NotificationSeverityLevelType,
         "notifyOnCreateOrReopenCase": bool,
         "notifyOnResolveCase": bool,
     },
     total=False,
 )
 
+
 class UpdateSlackChannelConfigurationRequestRequestTypeDef(
     _RequiredUpdateSlackChannelConfigurationRequestRequestTypeDef,
     _OptionalUpdateSlackChannelConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
+GetAccountAliasResultTypeDef = TypedDict(
+    "GetAccountAliasResultTypeDef",
+    {
+        "accountAlias": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterSlackWorkspaceForOrganizationResultTypeDef = TypedDict(
+    "RegisterSlackWorkspaceForOrganizationResultTypeDef",
+    {
+        "accountType": AccountTypeType,
+        "teamId": str,
+        "teamName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateSlackChannelConfigurationResultTypeDef = TypedDict(
     "UpdateSlackChannelConfigurationResultTypeDef",
     {
         "channelId": str,
         "channelName": str,
         "channelRoleArn": str,
         "notifyOnAddCorrespondenceToCase": bool,
         "notifyOnCaseSeverity": NotificationSeverityLevelType,
         "notifyOnCreateOrReopenCase": bool,
         "notifyOnResolveCase": bool,
         "teamId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSlackChannelConfigurationsResultTypeDef = TypedDict(
     "ListSlackChannelConfigurationsResultTypeDef",
     {
         "nextToken": str,
         "slackChannelConfigurations": List[SlackChannelConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSlackWorkspaceConfigurationsResultTypeDef = TypedDict(
     "ListSlackWorkspaceConfigurationsResultTypeDef",
     {
         "nextToken": str,
         "slackWorkspaceConfigurations": List[SlackWorkspaceConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-support-app-2.5.2/types_aiobotocore_support_app.egg-info/PKG-INFO` & `types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-support-app
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SupportApp 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SupportApp 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore support-app type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore support-app type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-support-app"></a>
 
 # types-aiobotocore-support-app
 
 [![PyPI - types-aiobotocore-support-app](https://img.shields.io/pypi/v/types-aiobotocore-support-app.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support-app)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-support-app.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support-app)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-support-app?color=blue)](https://pypistats.org/packages/types-aiobotocore-support-app)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-support-app)](https://pepy.tech/project/types-aiobotocore-support-app)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SupportApp 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp)
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
 [types-aiobotocore-support-app docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/).
 
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
@@ -282,43 +281,43 @@
 )
 
 
 def check_value(value: AccountTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_support_app.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_support_app.type_defs import (
     CreateSlackChannelConfigurationRequestRequestTypeDef,
     DeleteSlackChannelConfigurationRequestRequestTypeDef,
     DeleteSlackWorkspaceConfigurationRequestRequestTypeDef,
-    GetAccountAliasResultTypeDef,
+    ResponseMetadataTypeDef,
     ListSlackChannelConfigurationsRequestRequestTypeDef,
     SlackChannelConfigurationTypeDef,
     ListSlackWorkspaceConfigurationsRequestRequestTypeDef,
     SlackWorkspaceConfigurationTypeDef,
     PutAccountAliasRequestRequestTypeDef,
     RegisterSlackWorkspaceForOrganizationRequestRequestTypeDef,
-    RegisterSlackWorkspaceForOrganizationResultTypeDef,
-    ResponseMetadataTypeDef,
     UpdateSlackChannelConfigurationRequestRequestTypeDef,
+    GetAccountAliasResultTypeDef,
+    RegisterSlackWorkspaceForOrganizationResultTypeDef,
     UpdateSlackChannelConfigurationResultTypeDef,
     ListSlackChannelConfigurationsResultTypeDef,
     ListSlackWorkspaceConfigurationsResultTypeDef,
 )
 
 
-def get_structure() -> CreateSlackChannelConfigurationRequestRequestTypeDef:
+def get_value() -> CreateSlackChannelConfigurationRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-support-app-2.5.2/types_aiobotocore_support_app.egg-info/SOURCES.txt` & `types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*


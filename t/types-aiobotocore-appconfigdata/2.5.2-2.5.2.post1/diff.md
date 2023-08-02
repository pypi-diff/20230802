# Comparing `tmp/types-aiobotocore-appconfigdata-2.5.2.tar.gz` & `tmp/types-aiobotocore-appconfigdata-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-appconfigdata-2.5.2.tar", last modified: Sat Jul  8 01:43:12 2023, max compression
+gzip compressed data, was "types-aiobotocore-appconfigdata-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:50 2023, max compression
```

## Comparing `types-aiobotocore-appconfigdata-2.5.2.tar` & `types-aiobotocore-appconfigdata-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:12.433654 types-aiobotocore-appconfigdata-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:25:41.000000 types-aiobotocore-appconfigdata-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-07-08 01:43:12.433654 types-aiobotocore-appconfigdata-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-07-08 01:25:41.000000 types-aiobotocore-appconfigdata-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:12.433654 types-aiobotocore-appconfigdata-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-08 01:25:41.000000 types-aiobotocore-appconfigdata-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:12.425654 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-08 01:25:41.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-08 01:25:41.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-08 01:25:41.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-07-08 01:25:41.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-08 01:25:41.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-07-08 01:25:42.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-07-08 01:25:42.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:25:41.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-08 01:25:42.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-08 01:25:42.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:25:41.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:12.433654 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-07-08 01:43:12.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-08 01:43:12.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:12.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:12.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:12.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-08 01:43:12.000000 types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.541660 types-aiobotocore-appconfigdata-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:07.000000 types-aiobotocore-appconfigdata-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-08-02 14:51:50.541660 types-aiobotocore-appconfigdata-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-08-02 14:33:07.000000 types-aiobotocore-appconfigdata-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:50.541660 types-aiobotocore-appconfigdata-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-02 14:33:07.000000 types-aiobotocore-appconfigdata-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.541660 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 14:33:07.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-02 14:33:07.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-02 14:33:07.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-08-02 14:33:07.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-08-02 14:33:07.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-08-02 14:33:07.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-08-02 14:33:07.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:07.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-08-02 14:33:08.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-08-02 14:33:08.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:07.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.541660 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-08-02 14:51:50.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-02 14:51:50.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:50.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:50.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:50.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 14:51:50.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-appconfigdata-2.5.2/LICENSE` & `types-aiobotocore-appconfigdata-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfigdata-2.5.2/PKG-INFO` & `types-aiobotocore-appconfigdata-2.5.2.post1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appconfigdata
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.AppConfigData 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.AppConfigData 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore appconfigdata type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore appconfigdata type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-appconfigdata"></a>
 
 # types-aiobotocore-appconfigdata
 
 [![PyPI - types-aiobotocore-appconfigdata](https://img.shields.io/pypi/v/types-aiobotocore-appconfigdata.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appconfigdata)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appconfigdata.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appconfigdata)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-appconfigdata?color=blue)](https://pypistats.org/packages/types-aiobotocore-appconfigdata)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appconfigdata)](https://pepy.tech/project/types-aiobotocore-appconfigdata)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AppConfigData 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData)
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
 [types-aiobotocore-appconfigdata docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/).
 
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
@@ -280,32 +279,32 @@
 )
 
 
 def check_value(value: AppConfigDataServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_appconfigdata.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_appconfigdata.type_defs import (
     GetLatestConfigurationRequestRequestTypeDef,
-    GetLatestConfigurationResponseTypeDef,
     ResponseMetadataTypeDef,
     StartConfigurationSessionRequestRequestTypeDef,
+    GetLatestConfigurationResponseTypeDef,
     StartConfigurationSessionResponseTypeDef,
 )
 
 
-def get_structure() -> GetLatestConfigurationRequestRequestTypeDef:
+def get_value() -> GetLatestConfigurationRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-appconfigdata-2.5.2/README.md` & `types-aiobotocore-appconfigdata-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-appconfigdata"></a>
 
 # types-aiobotocore-appconfigdata
 
 [![PyPI - types-aiobotocore-appconfigdata](https://img.shields.io/pypi/v/types-aiobotocore-appconfigdata.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appconfigdata)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appconfigdata.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appconfigdata)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-appconfigdata?color=blue)](https://pypistats.org/packages/types-aiobotocore-appconfigdata)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appconfigdata)](https://pepy.tech/project/types-aiobotocore-appconfigdata)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AppConfigData 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData)
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
 [types-aiobotocore-appconfigdata docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/).
 
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
@@ -247,32 +247,32 @@
 )
 
 
 def check_value(value: AppConfigDataServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_appconfigdata.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_appconfigdata.type_defs import (
     GetLatestConfigurationRequestRequestTypeDef,
-    GetLatestConfigurationResponseTypeDef,
     ResponseMetadataTypeDef,
     StartConfigurationSessionRequestRequestTypeDef,
+    GetLatestConfigurationResponseTypeDef,
     StartConfigurationSessionResponseTypeDef,
 )
 
 
-def get_structure() -> GetLatestConfigurationRequestRequestTypeDef:
+def get_value() -> GetLatestConfigurationRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-appconfigdata-2.5.2/setup.py` & `types-aiobotocore-appconfigdata-2.5.2.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-appconfigdata",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_appconfigdata"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.AppConfigData 2.5.2 service generated with"
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
-    keywords="aiobotocore appconfigdata type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore appconfigdata type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_appconfigdata": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/"
```

### Comparing `types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/__main__.py` & `types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AppConfigData 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.AppConfigData 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData\nOther"
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

### Comparing `types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/client.py` & `types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/client.pyi` & `types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/literals.py` & `types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/literals.pyi` & `types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/type_defs.py` & `types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_appconfigdata.type_defs import GetLatestConfigurationRequestRequestTypeDef
 
-    data: GetLatestConfigurationRequestRequestTypeDef = {...}
+    data: GetLatestConfigurationRequestRequestTypeDef = ...
     ```
 """
 import sys
 from typing import Dict
 
 from aiobotocore.response import StreamingBody
 
@@ -20,39 +20,27 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "GetLatestConfigurationRequestRequestTypeDef",
-    "GetLatestConfigurationResponseTypeDef",
     "ResponseMetadataTypeDef",
     "StartConfigurationSessionRequestRequestTypeDef",
+    "GetLatestConfigurationResponseTypeDef",
     "StartConfigurationSessionResponseTypeDef",
 )
 
 GetLatestConfigurationRequestRequestTypeDef = TypedDict(
     "GetLatestConfigurationRequestRequestTypeDef",
     {
         "ConfigurationToken": str,
     },
 )
 
-GetLatestConfigurationResponseTypeDef = TypedDict(
-    "GetLatestConfigurationResponseTypeDef",
-    {
-        "NextPollConfigurationToken": str,
-        "NextPollIntervalInSeconds": int,
-        "ContentType": str,
-        "Configuration": StreamingBody,
-        "VersionLabel": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -80,14 +68,26 @@
 class StartConfigurationSessionRequestRequestTypeDef(
     _RequiredStartConfigurationSessionRequestRequestTypeDef,
     _OptionalStartConfigurationSessionRequestRequestTypeDef,
 ):
     pass
 
 
+GetLatestConfigurationResponseTypeDef = TypedDict(
+    "GetLatestConfigurationResponseTypeDef",
+    {
+        "NextPollConfigurationToken": str,
+        "NextPollIntervalInSeconds": int,
+        "ContentType": str,
+        "Configuration": StreamingBody,
+        "VersionLabel": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 StartConfigurationSessionResponseTypeDef = TypedDict(
     "StartConfigurationSessionResponseTypeDef",
     {
         "InitialConfigurationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata/type_defs.pyi` & `types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -4,54 +4,42 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_appconfigdata.type_defs import GetLatestConfigurationRequestRequestTypeDef
 
-    data: GetLatestConfigurationRequestRequestTypeDef = {...}
+    data: GetLatestConfigurationRequestRequestTypeDef = ...
     ```
 """
 import sys
 from typing import Dict
 
 from aiobotocore.response import StreamingBody
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "GetLatestConfigurationRequestRequestTypeDef",
-    "GetLatestConfigurationResponseTypeDef",
     "ResponseMetadataTypeDef",
     "StartConfigurationSessionRequestRequestTypeDef",
+    "GetLatestConfigurationResponseTypeDef",
     "StartConfigurationSessionResponseTypeDef",
 )
 
 GetLatestConfigurationRequestRequestTypeDef = TypedDict(
     "GetLatestConfigurationRequestRequestTypeDef",
     {
         "ConfigurationToken": str,
     },
 )
 
-GetLatestConfigurationResponseTypeDef = TypedDict(
-    "GetLatestConfigurationResponseTypeDef",
-    {
-        "NextPollConfigurationToken": str,
-        "NextPollIntervalInSeconds": int,
-        "ContentType": str,
-        "Configuration": StreamingBody,
-        "VersionLabel": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -77,14 +65,26 @@
 
 class StartConfigurationSessionRequestRequestTypeDef(
     _RequiredStartConfigurationSessionRequestRequestTypeDef,
     _OptionalStartConfigurationSessionRequestRequestTypeDef,
 ):
     pass
 
+GetLatestConfigurationResponseTypeDef = TypedDict(
+    "GetLatestConfigurationResponseTypeDef",
+    {
+        "NextPollConfigurationToken": str,
+        "NextPollIntervalInSeconds": int,
+        "ContentType": str,
+        "Configuration": StreamingBody,
+        "VersionLabel": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 StartConfigurationSessionResponseTypeDef = TypedDict(
     "StartConfigurationSessionResponseTypeDef",
     {
         "InitialConfigurationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata.egg-info/PKG-INFO` & `types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appconfigdata
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.AppConfigData 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.AppConfigData 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore appconfigdata type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore appconfigdata type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-appconfigdata"></a>
 
 # types-aiobotocore-appconfigdata
 
 [![PyPI - types-aiobotocore-appconfigdata](https://img.shields.io/pypi/v/types-aiobotocore-appconfigdata.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appconfigdata)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appconfigdata.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appconfigdata)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-appconfigdata?color=blue)](https://pypistats.org/packages/types-aiobotocore-appconfigdata)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appconfigdata)](https://pepy.tech/project/types-aiobotocore-appconfigdata)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AppConfigData 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData)
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
 [types-aiobotocore-appconfigdata docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/).
 
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
@@ -280,32 +279,32 @@
 )
 
 
 def check_value(value: AppConfigDataServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_appconfigdata.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_appconfigdata.type_defs import (
     GetLatestConfigurationRequestRequestTypeDef,
-    GetLatestConfigurationResponseTypeDef,
     ResponseMetadataTypeDef,
     StartConfigurationSessionRequestRequestTypeDef,
+    GetLatestConfigurationResponseTypeDef,
     StartConfigurationSessionResponseTypeDef,
 )
 
 
-def get_structure() -> GetLatestConfigurationRequestRequestTypeDef:
+def get_value() -> GetLatestConfigurationRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-appconfigdata-2.5.2/types_aiobotocore_appconfigdata.egg-info/SOURCES.txt` & `types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*


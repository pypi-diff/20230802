# Comparing `tmp/types-aiobotocore-cloudtrail-data-2.5.2.tar.gz` & `tmp/types-aiobotocore-cloudtrail-data-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudtrail-data-2.5.2.tar", last modified: Sat Jul  8 01:43:22 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudtrail-data-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:02 2023, max compression
```

## Comparing `types-aiobotocore-cloudtrail-data-2.5.2.tar` & `types-aiobotocore-cloudtrail-data-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:22.801849 types-aiobotocore-cloudtrail-data-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:15.000000 types-aiobotocore-cloudtrail-data-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12674 2023-07-08 01:43:22.801849 types-aiobotocore-cloudtrail-data-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11071 2023-07-08 01:27:15.000000 types-aiobotocore-cloudtrail-data-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:22.801849 types-aiobotocore-cloudtrail-data-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-08 01:27:15.000000 types-aiobotocore-cloudtrail-data-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:22.801849 types-aiobotocore-cloudtrail-data-2.5.2/types_aiobotocore_cloudtrail_data/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-08 01:27:15.000000 types-aiobotocore-cloudtrail-data-2.5.2/types_aiobotocore_cloudtrail_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-08 01:27:15.000000 types-aiobotocore-cloudtrail-data-2.5.2/types_aiobotocore_cloudtrail_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-08 01:27:15.000000 types-aiobotocore-cloudtrail-data-2.5.2/types_aiobotocore_cloudtrail_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-07-08 01:27:15.000000 types-aiobotocore-cloudtrail-data-2.5.2/types_aiobotocore_cloudtrail_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-07-08 01:27:15.000000 types-aiobotocore-cloudtrail-data-2.5.2/types_aiobotocore_cloudtrail_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-07-08 01:27:15.000000 types-aiobotocore-cloudtrail-data-2.5.2/types_aiobotocore_cloudtrail_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-07-08 01:27:15.000000 types-aiobotocore-cloudtrail-data-2.5.2/types_aiobotocore_cloudtrail_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:15.000000 types-aiobotocore-cloudtrail-data-2.5.2/types_aiobotocore_cloudtrail_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-07-08 01:27:15.000000 types-aiobotocore-cloudtrail-data-2.5.2/types_aiobotocore_cloudtrail_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-08 01:27:15.000000 types-aiobotocore-cloudtrail-data-2.5.2/types_aiobotocore_cloudtrail_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:15.000000 types-aiobotocore-cloudtrail-data-2.5.2/types_aiobotocore_cloudtrail_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:22.801849 types-aiobotocore-cloudtrail-data-2.5.2/types_aiobotocore_cloudtrail_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12674 2023-07-08 01:43:22.000000 types-aiobotocore-cloudtrail-data-2.5.2/types_aiobotocore_cloudtrail_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-08 01:43:22.000000 types-aiobotocore-cloudtrail-data-2.5.2/types_aiobotocore_cloudtrail_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:22.000000 types-aiobotocore-cloudtrail-data-2.5.2/types_aiobotocore_cloudtrail_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:22.000000 types-aiobotocore-cloudtrail-data-2.5.2/types_aiobotocore_cloudtrail_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:22.000000 types-aiobotocore-cloudtrail-data-2.5.2/types_aiobotocore_cloudtrail_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-08 01:43:22.000000 types-aiobotocore-cloudtrail-data-2.5.2/types_aiobotocore_cloudtrail_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.201627 types-aiobotocore-cloudtrail-data-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:46.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12610 2023-08-02 14:52:02.201627 types-aiobotocore-cloudtrail-data-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11054 2023-08-02 14:34:46.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:02.201627 types-aiobotocore-cloudtrail-data-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-02 14:34:46.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.201627 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-02 14:34:46.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-02 14:34:46.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-02 14:34:46.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-08-02 14:34:46.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-08-02 14:34:46.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-08-02 14:34:47.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-08-02 14:34:46.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:46.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-08-02 14:34:47.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-08-02 14:34:47.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:46.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.201627 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12610 2023-08-02 14:52:02.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:52:02.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:02.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 14:52:02.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudtrail-data-2.5.2/LICENSE` & `types-aiobotocore-cloudtrail-data-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-data-2.5.2/PKG-INFO` & `types-aiobotocore-cloudtrail-data-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudtrail-data
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CloudTrailDataService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CloudTrailDataService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore cloudtrail-data type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore cloudtrail-data type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cloudtrail-data"></a>
 
 # types-aiobotocore-cloudtrail-data
 
 [![PyPI - types-aiobotocore-cloudtrail-data](https://img.shields.io/pypi/v/types-aiobotocore-cloudtrail-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudtrail-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudtrail-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudtrail-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail_data/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudtrail-data?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudtrail-data)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudtrail-data)](https://pepy.tech/project/types-aiobotocore-cloudtrail-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudTrailDataService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail-data.html#CloudTrailDataService)
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
 [types-aiobotocore-cloudtrail-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail_data/).
 
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
@@ -280,33 +279,33 @@
 )
 
 
 def check_value(value: CloudTrailDataServiceServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloudtrail_data.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloudtrail_data.type_defs import (
     AuditEventResultEntryTypeDef,
     AuditEventTypeDef,
-    ResultErrorEntryTypeDef,
     ResponseMetadataTypeDef,
+    ResultErrorEntryTypeDef,
     PutAuditEventsRequestRequestTypeDef,
     PutAuditEventsResponseTypeDef,
 )
 
 
-def get_structure() -> AuditEventResultEntryTypeDef:
+def get_value() -> AuditEventResultEntryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloudtrail-data-2.5.2/README.md` & `types-aiobotocore-cloudtrail-data-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-cloudtrail-data"></a>
 
 # types-aiobotocore-cloudtrail-data
 
 [![PyPI - types-aiobotocore-cloudtrail-data](https://img.shields.io/pypi/v/types-aiobotocore-cloudtrail-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudtrail-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudtrail-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudtrail-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail_data/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudtrail-data?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudtrail-data)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudtrail-data)](https://pepy.tech/project/types-aiobotocore-cloudtrail-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudTrailDataService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail-data.html#CloudTrailDataService)
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
 [types-aiobotocore-cloudtrail-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail_data/).
 
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
@@ -247,33 +247,33 @@
 )
 
 
 def check_value(value: CloudTrailDataServiceServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloudtrail_data.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloudtrail_data.type_defs import (
     AuditEventResultEntryTypeDef,
     AuditEventTypeDef,
-    ResultErrorEntryTypeDef,
     ResponseMetadataTypeDef,
+    ResultErrorEntryTypeDef,
     PutAuditEventsRequestRequestTypeDef,
     PutAuditEventsResponseTypeDef,
 )
 
 
-def get_structure() -> AuditEventResultEntryTypeDef:
+def get_value() -> AuditEventResultEntryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloudtrail-data-2.5.2/setup.py` & `types-aiobotocore-cloudtrail-data-2.5.2.post1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudtrail-data",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_cloudtrail_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CloudTrailDataService 2.5.2 service generated with"
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
-    keywords="aiobotocore cloudtrail-data type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore cloudtrail-data type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_cloudtrail_data": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail_data/"
```

### Comparing `types-aiobotocore-cloudtrail-data-2.5.2/types_aiobotocore_cloudtrail_data/__init__.py` & `types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-data-2.5.2/types_aiobotocore_cloudtrail_data/__init__.pyi` & `types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-data-2.5.2/types_aiobotocore_cloudtrail_data/__main__.py` & `types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.CloudTrailDataService 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail_data//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail-data.html#CloudTrailDataService\nOther"
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

### Comparing `types-aiobotocore-cloudtrail-data-2.5.2/types_aiobotocore_cloudtrail_data/client.py` & `types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-data-2.5.2/types_aiobotocore_cloudtrail_data/client.pyi` & `types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-data-2.5.2/types_aiobotocore_cloudtrail_data/literals.py` & `types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-data-2.5.2/types_aiobotocore_cloudtrail_data/literals.pyi` & `types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-data-2.5.2/types_aiobotocore_cloudtrail_data/type_defs.py` & `types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail_data/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_cloudtrail_data.type_defs import AuditEventResultEntryTypeDef
 
-    data: AuditEventResultEntryTypeDef = {...}
+    data: AuditEventResultEntryTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AuditEventResultEntryTypeDef",
     "AuditEventTypeDef",
-    "ResultErrorEntryTypeDef",
     "ResponseMetadataTypeDef",
+    "ResultErrorEntryTypeDef",
     "PutAuditEventsRequestRequestTypeDef",
     "PutAuditEventsResponseTypeDef",
 )
 
 AuditEventResultEntryTypeDef = TypedDict(
     "AuditEventResultEntryTypeDef",
     {
@@ -53,34 +53,34 @@
 )
 
 
 class AuditEventTypeDef(_RequiredAuditEventTypeDef, _OptionalAuditEventTypeDef):
     pass
 
 
-ResultErrorEntryTypeDef = TypedDict(
-    "ResultErrorEntryTypeDef",
-    {
-        "errorCode": str,
-        "errorMessage": str,
-        "id": str,
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
         "RetryAttempts": int,
     },
 )
 
+ResultErrorEntryTypeDef = TypedDict(
+    "ResultErrorEntryTypeDef",
+    {
+        "errorCode": str,
+        "errorMessage": str,
+        "id": str,
+    },
+)
+
 _RequiredPutAuditEventsRequestRequestTypeDef = TypedDict(
     "_RequiredPutAuditEventsRequestRequestTypeDef",
     {
         "auditEvents": Sequence[AuditEventTypeDef],
         "channelArn": str,
     },
 )
@@ -100,10 +100,10 @@
 
 
 PutAuditEventsResponseTypeDef = TypedDict(
     "PutAuditEventsResponseTypeDef",
     {
         "failed": List[ResultErrorEntryTypeDef],
         "successful": List[AuditEventResultEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-cloudtrail-data-2.5.2/types_aiobotocore_cloudtrail_data/type_defs.pyi` & `types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail_data/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_cloudtrail_data.type_defs import AuditEventResultEntryTypeDef
 
-    data: AuditEventResultEntryTypeDef = {...}
+    data: AuditEventResultEntryTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AuditEventResultEntryTypeDef",
     "AuditEventTypeDef",
-    "ResultErrorEntryTypeDef",
     "ResponseMetadataTypeDef",
+    "ResultErrorEntryTypeDef",
     "PutAuditEventsRequestRequestTypeDef",
     "PutAuditEventsResponseTypeDef",
 )
 
 AuditEventResultEntryTypeDef = TypedDict(
     "AuditEventResultEntryTypeDef",
     {
@@ -50,34 +50,34 @@
     },
     total=False,
 )
 
 class AuditEventTypeDef(_RequiredAuditEventTypeDef, _OptionalAuditEventTypeDef):
     pass
 
-ResultErrorEntryTypeDef = TypedDict(
-    "ResultErrorEntryTypeDef",
-    {
-        "errorCode": str,
-        "errorMessage": str,
-        "id": str,
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
         "RetryAttempts": int,
     },
 )
 
+ResultErrorEntryTypeDef = TypedDict(
+    "ResultErrorEntryTypeDef",
+    {
+        "errorCode": str,
+        "errorMessage": str,
+        "id": str,
+    },
+)
+
 _RequiredPutAuditEventsRequestRequestTypeDef = TypedDict(
     "_RequiredPutAuditEventsRequestRequestTypeDef",
     {
         "auditEvents": Sequence[AuditEventTypeDef],
         "channelArn": str,
     },
 )
@@ -95,10 +95,10 @@
     pass
 
 PutAuditEventsResponseTypeDef = TypedDict(
     "PutAuditEventsResponseTypeDef",
     {
         "failed": List[ResultErrorEntryTypeDef],
         "successful": List[AuditEventResultEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-cloudtrail-data-2.5.2/types_aiobotocore_cloudtrail_data.egg-info/PKG-INFO` & `types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudtrail-data
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CloudTrailDataService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CloudTrailDataService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore cloudtrail-data type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore cloudtrail-data type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cloudtrail-data"></a>
 
 # types-aiobotocore-cloudtrail-data
 
 [![PyPI - types-aiobotocore-cloudtrail-data](https://img.shields.io/pypi/v/types-aiobotocore-cloudtrail-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudtrail-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudtrail-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudtrail-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail_data/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudtrail-data?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudtrail-data)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudtrail-data)](https://pepy.tech/project/types-aiobotocore-cloudtrail-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudTrailDataService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail-data.html#CloudTrailDataService)
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
 [types-aiobotocore-cloudtrail-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail_data/).
 
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
@@ -280,33 +279,33 @@
 )
 
 
 def check_value(value: CloudTrailDataServiceServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloudtrail_data.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloudtrail_data.type_defs import (
     AuditEventResultEntryTypeDef,
     AuditEventTypeDef,
-    ResultErrorEntryTypeDef,
     ResponseMetadataTypeDef,
+    ResultErrorEntryTypeDef,
     PutAuditEventsRequestRequestTypeDef,
     PutAuditEventsResponseTypeDef,
 )
 
 
-def get_structure() -> AuditEventResultEntryTypeDef:
+def get_value() -> AuditEventResultEntryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloudtrail-data-2.5.2/types_aiobotocore_cloudtrail_data.egg-info/SOURCES.txt` & `types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-sagemaker-geospatial-2.5.1.tar.gz` & `tmp/types-aiobotocore-sagemaker-geospatial-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sagemaker-geospatial-2.5.1.tar", last modified: Wed Jun 28 01:44:07 2023, max compression
+gzip compressed data, was "types-aiobotocore-sagemaker-geospatial-2.5.2.tar", last modified: Sat Jul  8 01:44:15 2023, max compression
```

## Comparing `types-aiobotocore-sagemaker-geospatial-2.5.1.tar` & `types-aiobotocore-sagemaker-geospatial-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:07.646208 types-aiobotocore-sagemaker-geospatial-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:40:18.000000 types-aiobotocore-sagemaker-geospatial-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18532 2023-06-28 01:44:07.646208 types-aiobotocore-sagemaker-geospatial-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16904 2023-06-28 01:40:18.000000 types-aiobotocore-sagemaker-geospatial-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:44:07.646208 types-aiobotocore-sagemaker-geospatial-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-06-28 01:40:18.000000 types-aiobotocore-sagemaker-geospatial-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:07.646208 types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-28 01:40:18.000000 types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-28 01:40:18.000000 types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-28 01:40:18.000000 types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20183 2023-06-28 01:40:18.000000 types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20152 2023-06-28 01:40:18.000000 types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11070 2023-06-28 01:40:18.000000 types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-06-28 01:40:18.000000 types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-06-28 01:40:18.000000 types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-06-28 01:40:18.000000 types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:40:18.000000 types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34454 2023-06-28 01:40:19.000000 types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34411 2023-06-28 01:40:19.000000 types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:40:18.000000 types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:07.646208 types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18532 2023-06-28 01:44:07.000000 types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-28 01:44:07.000000 types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:44:07.000000 types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:44:07.000000 types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:44:07.000000 types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-28 01:44:07.000000 types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:15.894842 types-aiobotocore-sagemaker-geospatial-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:40:23.000000 types-aiobotocore-sagemaker-geospatial-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18532 2023-07-08 01:44:15.894842 types-aiobotocore-sagemaker-geospatial-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16904 2023-07-08 01:40:23.000000 types-aiobotocore-sagemaker-geospatial-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:15.894842 types-aiobotocore-sagemaker-geospatial-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-08 01:40:23.000000 types-aiobotocore-sagemaker-geospatial-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:15.886842 types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-08 01:40:23.000000 types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-08 01:40:23.000000 types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-08 01:40:23.000000 types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20183 2023-07-08 01:40:24.000000 types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20152 2023-07-08 01:40:24.000000 types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11070 2023-07-08 01:40:24.000000 types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-07-08 01:40:24.000000 types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-08 01:40:24.000000 types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-07-08 01:40:24.000000 types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:40:23.000000 types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34454 2023-07-08 01:40:24.000000 types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34411 2023-07-08 01:40:24.000000 types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:40:23.000000 types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:15.894842 types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18532 2023-07-08 01:44:15.000000 types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-08 01:44:15.000000 types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:15.000000 types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:15.000000 types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:15.000000 types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-08 01:44:15.000000 types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sagemaker-geospatial-2.5.1/LICENSE` & `types-aiobotocore-sagemaker-geospatial-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-geospatial-2.5.1/PKG-INFO` & `types-aiobotocore-sagemaker-geospatial-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sagemaker-geospatial
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.SageMakergeospatialcapabilities 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.SageMakergeospatialcapabilities 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sagemaker-geospatial.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-geospatial)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sagemaker-geospatial?color=blue)](https://pypistats.org/packages/types-aiobotocore-sagemaker-geospatial)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SageMakergeospatialcapabilities 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
+[aiobotocore.SageMakergeospatialcapabilities 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-sagemaker-geospatial-2.5.1/README.md` & `types-aiobotocore-sagemaker-geospatial-2.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sagemaker-geospatial.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-geospatial)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sagemaker-geospatial?color=blue)](https://pypistats.org/packages/types-aiobotocore-sagemaker-geospatial)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SageMakergeospatialcapabilities 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
+[aiobotocore.SageMakergeospatialcapabilities 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-sagemaker-geospatial-2.5.1/setup.py` & `types-aiobotocore-sagemaker-geospatial-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sagemaker-geospatial",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_sagemaker_geospatial"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SageMakergeospatialcapabilities 2.5.1 service generated"
+        "Type annotations for aiobotocore.SageMakergeospatialcapabilities 2.5.2 service generated"
         " with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial/__init__.py` & `types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial/__init__.pyi` & `types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial/__main__.py` & `types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SageMakergeospatialcapabilities 2.5.1\nVersion:        "
-        " 2.5.1\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.SageMakergeospatialcapabilities 2.5.2\nVersion:        "
+        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.5.1")
+    print("2.5.2")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial/client.py` & `types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial/client.pyi` & `types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial/literals.py` & `types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial/literals.pyi` & `types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial/paginator.py` & `types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial/paginator.pyi` & `types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial/type_defs.py` & `types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial/type_defs.pyi` & `types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial.egg-info/PKG-INFO` & `types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sagemaker-geospatial
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.SageMakergeospatialcapabilities 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.SageMakergeospatialcapabilities 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sagemaker-geospatial.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-geospatial)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sagemaker-geospatial?color=blue)](https://pypistats.org/packages/types-aiobotocore-sagemaker-geospatial)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SageMakergeospatialcapabilities 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
+[aiobotocore.SageMakergeospatialcapabilities 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-sagemaker-geospatial-2.5.1/types_aiobotocore_sagemaker_geospatial.egg-info/SOURCES.txt` & `types-aiobotocore-sagemaker-geospatial-2.5.2/types_aiobotocore_sagemaker_geospatial.egg-info/SOURCES.txt`

 * *Files identical despite different names*


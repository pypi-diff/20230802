# Comparing `tmp/types-aiobotocore-rum-2.5.1.tar.gz` & `tmp/types-aiobotocore-rum-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-rum-2.5.1.tar", last modified: Wed Jun 28 01:44:05 2023, max compression
+gzip compressed data, was "types-aiobotocore-rum-2.5.2.tar", last modified: Sat Jul  8 01:44:14 2023, max compression
```

## Comparing `types-aiobotocore-rum-2.5.1.tar` & `types-aiobotocore-rum-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:05.706205 types-aiobotocore-rum-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:39:36.000000 types-aiobotocore-rum-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-06-28 01:44:05.698204 types-aiobotocore-rum-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-06-28 01:39:36.000000 types-aiobotocore-rum-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:44:05.706205 types-aiobotocore-rum-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-28 01:39:36.000000 types-aiobotocore-rum-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:05.694204 types-aiobotocore-rum-2.5.1/types_aiobotocore_rum/
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-28 01:39:36.000000 types-aiobotocore-rum-2.5.1/types_aiobotocore_rum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-28 01:39:36.000000 types-aiobotocore-rum-2.5.1/types_aiobotocore_rum/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-28 01:39:36.000000 types-aiobotocore-rum-2.5.1/types_aiobotocore_rum/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18059 2023-06-28 01:39:36.000000 types-aiobotocore-rum-2.5.1/types_aiobotocore_rum/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18029 2023-06-28 01:39:36.000000 types-aiobotocore-rum-2.5.1/types_aiobotocore_rum/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-06-28 01:39:36.000000 types-aiobotocore-rum-2.5.1/types_aiobotocore_rum/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-06-28 01:39:36.000000 types-aiobotocore-rum-2.5.1/types_aiobotocore_rum/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-06-28 01:39:36.000000 types-aiobotocore-rum-2.5.1/types_aiobotocore_rum/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-06-28 01:39:36.000000 types-aiobotocore-rum-2.5.1/types_aiobotocore_rum/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:39:36.000000 types-aiobotocore-rum-2.5.1/types_aiobotocore_rum/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20152 2023-06-28 01:39:37.000000 types-aiobotocore-rum-2.5.1/types_aiobotocore_rum/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20117 2023-06-28 01:39:36.000000 types-aiobotocore-rum-2.5.1/types_aiobotocore_rum/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:39:36.000000 types-aiobotocore-rum-2.5.1/types_aiobotocore_rum/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:05.698204 types-aiobotocore-rum-2.5.1/types_aiobotocore_rum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-06-28 01:44:05.000000 types-aiobotocore-rum-2.5.1/types_aiobotocore_rum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-28 01:44:05.000000 types-aiobotocore-rum-2.5.1/types_aiobotocore_rum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:44:05.000000 types-aiobotocore-rum-2.5.1/types_aiobotocore_rum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:44:05.000000 types-aiobotocore-rum-2.5.1/types_aiobotocore_rum.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:44:05.000000 types-aiobotocore-rum-2.5.1/types_aiobotocore_rum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-28 01:44:05.000000 types-aiobotocore-rum-2.5.1/types_aiobotocore_rum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:14.122811 types-aiobotocore-rum-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:39:38.000000 types-aiobotocore-rum-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-07-08 01:44:14.118811 types-aiobotocore-rum-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-07-08 01:39:38.000000 types-aiobotocore-rum-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:14.122811 types-aiobotocore-rum-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-08 01:39:37.000000 types-aiobotocore-rum-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:14.106811 types-aiobotocore-rum-2.5.2/types_aiobotocore_rum/
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-08 01:39:38.000000 types-aiobotocore-rum-2.5.2/types_aiobotocore_rum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-08 01:39:38.000000 types-aiobotocore-rum-2.5.2/types_aiobotocore_rum/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-08 01:39:38.000000 types-aiobotocore-rum-2.5.2/types_aiobotocore_rum/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18059 2023-07-08 01:39:38.000000 types-aiobotocore-rum-2.5.2/types_aiobotocore_rum/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18029 2023-07-08 01:39:38.000000 types-aiobotocore-rum-2.5.2/types_aiobotocore_rum/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-07-08 01:39:38.000000 types-aiobotocore-rum-2.5.2/types_aiobotocore_rum/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-07-08 01:39:38.000000 types-aiobotocore-rum-2.5.2/types_aiobotocore_rum/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-07-08 01:39:38.000000 types-aiobotocore-rum-2.5.2/types_aiobotocore_rum/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-07-08 01:39:38.000000 types-aiobotocore-rum-2.5.2/types_aiobotocore_rum/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:39:38.000000 types-aiobotocore-rum-2.5.2/types_aiobotocore_rum/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20152 2023-07-08 01:39:38.000000 types-aiobotocore-rum-2.5.2/types_aiobotocore_rum/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20117 2023-07-08 01:39:38.000000 types-aiobotocore-rum-2.5.2/types_aiobotocore_rum/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:39:38.000000 types-aiobotocore-rum-2.5.2/types_aiobotocore_rum/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:14.118811 types-aiobotocore-rum-2.5.2/types_aiobotocore_rum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-07-08 01:44:13.000000 types-aiobotocore-rum-2.5.2/types_aiobotocore_rum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-08 01:44:13.000000 types-aiobotocore-rum-2.5.2/types_aiobotocore_rum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:13.000000 types-aiobotocore-rum-2.5.2/types_aiobotocore_rum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:13.000000 types-aiobotocore-rum-2.5.2/types_aiobotocore_rum.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:13.000000 types-aiobotocore-rum-2.5.2/types_aiobotocore_rum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:44:13.000000 types-aiobotocore-rum-2.5.2/types_aiobotocore_rum.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-rum-2.5.1/LICENSE` & `types-aiobotocore-rum-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rum-2.5.1/PKG-INFO` & `types-aiobotocore-rum-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rum
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.CloudWatchRUM 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.CloudWatchRUM 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rum.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rum)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-rum?color=blue)](https://pypistats.org/packages/types-aiobotocore-rum)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchRUM 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
+[aiobotocore.CloudWatchRUM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-rum-2.5.1/README.md` & `types-aiobotocore-rum-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rum.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rum)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-rum?color=blue)](https://pypistats.org/packages/types-aiobotocore-rum)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchRUM 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
+[aiobotocore.CloudWatchRUM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-rum-2.5.1/setup.py` & `types-aiobotocore-rum-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-rum",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_rum"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudWatchRUM 2.5.1 service generated with"
+        "Type annotations for aiobotocore.CloudWatchRUM 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-rum-2.5.1/types_aiobotocore_rum/__init__.py` & `types-aiobotocore-rum-2.5.2/types_aiobotocore_rum/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rum-2.5.1/types_aiobotocore_rum/__init__.pyi` & `types-aiobotocore-rum-2.5.2/types_aiobotocore_rum/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rum-2.5.1/types_aiobotocore_rum/__main__.py` & `types-aiobotocore-rum-2.5.2/types_aiobotocore_rum/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudWatchRUM 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.CloudWatchRUM 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM\nOther"
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

### Comparing `types-aiobotocore-rum-2.5.1/types_aiobotocore_rum/client.py` & `types-aiobotocore-rum-2.5.2/types_aiobotocore_rum/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rum-2.5.1/types_aiobotocore_rum/client.pyi` & `types-aiobotocore-rum-2.5.2/types_aiobotocore_rum/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rum-2.5.1/types_aiobotocore_rum/literals.py` & `types-aiobotocore-rum-2.5.2/types_aiobotocore_rum/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rum-2.5.1/types_aiobotocore_rum/literals.pyi` & `types-aiobotocore-rum-2.5.2/types_aiobotocore_rum/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rum-2.5.1/types_aiobotocore_rum/paginator.py` & `types-aiobotocore-rum-2.5.2/types_aiobotocore_rum/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rum-2.5.1/types_aiobotocore_rum/paginator.pyi` & `types-aiobotocore-rum-2.5.2/types_aiobotocore_rum/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rum-2.5.1/types_aiobotocore_rum/type_defs.py` & `types-aiobotocore-rum-2.5.2/types_aiobotocore_rum/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rum-2.5.1/types_aiobotocore_rum/type_defs.pyi` & `types-aiobotocore-rum-2.5.2/types_aiobotocore_rum/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rum-2.5.1/types_aiobotocore_rum.egg-info/PKG-INFO` & `types-aiobotocore-rum-2.5.2/types_aiobotocore_rum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rum
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.CloudWatchRUM 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.CloudWatchRUM 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rum.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rum)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-rum?color=blue)](https://pypistats.org/packages/types-aiobotocore-rum)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchRUM 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
+[aiobotocore.CloudWatchRUM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-rum-2.5.1/types_aiobotocore_rum.egg-info/SOURCES.txt` & `types-aiobotocore-rum-2.5.2/types_aiobotocore_rum.egg-info/SOURCES.txt`

 * *Files identical despite different names*


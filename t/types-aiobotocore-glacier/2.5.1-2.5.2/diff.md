# Comparing `tmp/types-aiobotocore-glacier-2.5.1.tar.gz` & `tmp/types-aiobotocore-glacier-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-glacier-2.5.1.tar", last modified: Wed Jun 28 01:43:31 2023, max compression
+gzip compressed data, was "types-aiobotocore-glacier-2.5.2.tar", last modified: Sat Jul  8 01:43:40 2023, max compression
```

## Comparing `types-aiobotocore-glacier-2.5.1.tar` & `types-aiobotocore-glacier-2.5.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:31.954141 types-aiobotocore-glacier-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:31:37.000000 types-aiobotocore-glacier-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20509 2023-06-28 01:43:31.946141 types-aiobotocore-glacier-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18944 2023-06-28 01:31:37.000000 types-aiobotocore-glacier-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:31.954141 types-aiobotocore-glacier-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-28 01:31:37.000000 types-aiobotocore-glacier-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:31.946141 types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-28 01:31:37.000000 types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-28 01:31:37.000000 types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-28 01:31:37.000000 types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28540 2023-06-28 01:31:38.000000 types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28492 2023-06-28 01:31:38.000000 types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-06-28 01:31:38.000000 types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9645 2023-06-28 01:31:38.000000 types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-06-28 01:31:38.000000 types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-06-28 01:31:38.000000 types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:31:37.000000 types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    42972 2023-06-28 01:31:38.000000 types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    42854 2023-06-28 01:31:38.000000 types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    38693 2023-06-28 01:31:40.000000 types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38621 2023-06-28 01:31:40.000000 types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:31:37.000000 types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-28 01:31:38.000000 types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-28 01:31:38.000000 types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:31.946141 types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20509 2023-06-28 01:43:31.000000 types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-28 01:43:31.000000 types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:31.000000 types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:31.000000 types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:31.000000 types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-28 01:43:31.000000 types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:40.146179 types-aiobotocore-glacier-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:31:22.000000 types-aiobotocore-glacier-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20509 2023-07-08 01:43:40.146179 types-aiobotocore-glacier-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18944 2023-07-08 01:31:22.000000 types-aiobotocore-glacier-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:40.146179 types-aiobotocore-glacier-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-08 01:31:21.000000 types-aiobotocore-glacier-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:40.138179 types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-08 01:31:22.000000 types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-08 01:31:22.000000 types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-08 01:31:22.000000 types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28540 2023-07-08 01:31:22.000000 types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28492 2023-07-08 01:31:22.000000 types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-07-08 01:31:22.000000 types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9645 2023-07-08 01:31:22.000000 types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-07-08 01:31:22.000000 types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-07-08 01:31:22.000000 types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:31:22.000000 types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    42972 2023-07-08 01:31:22.000000 types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42854 2023-07-08 01:31:22.000000 types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    38693 2023-07-08 01:31:23.000000 types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38621 2023-07-08 01:31:23.000000 types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:31:22.000000 types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-08 01:31:22.000000 types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-08 01:31:22.000000 types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:40.146179 types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20509 2023-07-08 01:43:39.000000 types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-08 01:43:40.000000 types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:39.000000 types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:39.000000 types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:39.000000 types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-08 01:43:39.000000 types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-glacier-2.5.1/LICENSE` & `types-aiobotocore-glacier-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.1/PKG-INFO` & `types-aiobotocore-glacier-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-glacier
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.Glacier 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.Glacier 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-glacier.svg?color=blue)](https://pypi.org/project/types-aiobotocore-glacier)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-glacier?color=blue)](https://pypistats.org/packages/types-aiobotocore-glacier)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Glacier 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
+[aiobotocore.Glacier 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-glacier-2.5.1/README.md` & `types-aiobotocore-glacier-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-glacier.svg?color=blue)](https://pypi.org/project/types-aiobotocore-glacier)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-glacier?color=blue)](https://pypistats.org/packages/types-aiobotocore-glacier)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Glacier 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
+[aiobotocore.Glacier 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-glacier-2.5.1/setup.py` & `types-aiobotocore-glacier-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-glacier",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_glacier"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Glacier 2.5.1 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Glacier 2.5.2 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/__init__.py` & `types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/__init__.pyi` & `types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/__main__.py` & `types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Glacier 2.5.1\nVersion:         2.5.1\nBuilder version:"
+        "Type annotations for aiobotocore.Glacier 2.5.2\nVersion:         2.5.2\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier\nOther"
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

### Comparing `types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/client.py` & `types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/client.pyi` & `types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/literals.py` & `types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/literals.pyi` & `types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/paginator.py` & `types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/paginator.pyi` & `types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/service_resource.py` & `types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/service_resource.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/service_resource.pyi` & `types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/type_defs.py` & `types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/type_defs.pyi` & `types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/waiter.py` & `types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier/waiter.pyi` & `types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier.egg-info/PKG-INFO` & `types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-glacier
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.Glacier 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.Glacier 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-glacier.svg?color=blue)](https://pypi.org/project/types-aiobotocore-glacier)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-glacier?color=blue)](https://pypistats.org/packages/types-aiobotocore-glacier)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Glacier 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
+[aiobotocore.Glacier 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-glacier-2.5.1/types_aiobotocore_glacier.egg-info/SOURCES.txt` & `types-aiobotocore-glacier-2.5.2/types_aiobotocore_glacier.egg-info/SOURCES.txt`

 * *Files identical despite different names*


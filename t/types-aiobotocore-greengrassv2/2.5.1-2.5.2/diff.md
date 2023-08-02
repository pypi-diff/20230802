# Comparing `tmp/types-aiobotocore-greengrassv2-2.5.1.tar.gz` & `tmp/types-aiobotocore-greengrassv2-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-greengrassv2-2.5.1.tar", last modified: Wed Jun 28 01:43:33 2023, max compression
+gzip compressed data, was "types-aiobotocore-greengrassv2-2.5.2.tar", last modified: Sat Jul  8 01:43:42 2023, max compression
```

## Comparing `types-aiobotocore-greengrassv2-2.5.1.tar` & `types-aiobotocore-greengrassv2-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:33.746144 types-aiobotocore-greengrassv2-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:32:01.000000 types-aiobotocore-greengrassv2-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19476 2023-06-28 01:43:33.746144 types-aiobotocore-greengrassv2-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17891 2023-06-28 01:32:01.000000 types-aiobotocore-greengrassv2-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:33.746144 types-aiobotocore-greengrassv2-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-28 01:32:01.000000 types-aiobotocore-greengrassv2-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:33.746144 types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2/
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-28 01:32:01.000000 types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-28 01:32:01.000000 types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-28 01:32:01.000000 types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27509 2023-06-28 01:32:01.000000 types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27464 2023-06-28 01:32:01.000000 types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-06-28 01:32:02.000000 types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-06-28 01:32:02.000000 types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9925 2023-06-28 01:32:02.000000 types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-06-28 01:32:02.000000 types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:32:01.000000 types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37233 2023-06-28 01:32:03.000000 types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    37200 2023-06-28 01:32:03.000000 types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:32:01.000000 types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:33.746144 types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19476 2023-06-28 01:43:33.000000 types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-28 01:43:33.000000 types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:33.000000 types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:33.000000 types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:33.000000 types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-28 01:43:33.000000 types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:42.042215 types-aiobotocore-greengrassv2-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:31:46.000000 types-aiobotocore-greengrassv2-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19476 2023-07-08 01:43:42.038215 types-aiobotocore-greengrassv2-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17891 2023-07-08 01:31:46.000000 types-aiobotocore-greengrassv2-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:42.042215 types-aiobotocore-greengrassv2-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-08 01:31:46.000000 types-aiobotocore-greengrassv2-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:42.030214 types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-08 01:31:46.000000 types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-08 01:31:46.000000 types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-08 01:31:46.000000 types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27509 2023-07-08 01:31:46.000000 types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27464 2023-07-08 01:31:46.000000 types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-07-08 01:31:46.000000 types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-07-08 01:31:46.000000 types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9925 2023-07-08 01:31:46.000000 types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-07-08 01:31:46.000000 types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:31:46.000000 types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37233 2023-07-08 01:31:47.000000 types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37200 2023-07-08 01:31:47.000000 types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:31:46.000000 types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:42.038215 types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19476 2023-07-08 01:43:41.000000 types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-08 01:43:41.000000 types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:41.000000 types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:41.000000 types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:41.000000 types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-08 01:43:41.000000 types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-greengrassv2-2.5.1/LICENSE` & `types-aiobotocore-greengrassv2-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrassv2-2.5.1/PKG-INFO` & `types-aiobotocore-greengrassv2-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-greengrassv2
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.GreengrassV2 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.GreengrassV2 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-greengrassv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-greengrassv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-greengrassv2?color=blue)](https://pypistats.org/packages/types-aiobotocore-greengrassv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GreengrassV2 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
+[aiobotocore.GreengrassV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-greengrassv2-2.5.1/README.md` & `types-aiobotocore-greengrassv2-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-greengrassv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-greengrassv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-greengrassv2?color=blue)](https://pypistats.org/packages/types-aiobotocore-greengrassv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GreengrassV2 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
+[aiobotocore.GreengrassV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-greengrassv2-2.5.1/setup.py` & `types-aiobotocore-greengrassv2-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-greengrassv2",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_greengrassv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.GreengrassV2 2.5.1 service generated with"
+        "Type annotations for aiobotocore.GreengrassV2 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2/__init__.py` & `types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2/__init__.pyi` & `types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2/__main__.py` & `types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.GreengrassV2 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.GreengrassV2 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2\nOther"
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

### Comparing `types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2/client.py` & `types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2/client.pyi` & `types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2/literals.py` & `types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2/literals.pyi` & `types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2/paginator.py` & `types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2/paginator.pyi` & `types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2/type_defs.py` & `types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2/type_defs.pyi` & `types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2.egg-info/PKG-INFO` & `types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-greengrassv2
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.GreengrassV2 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.GreengrassV2 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-greengrassv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-greengrassv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-greengrassv2?color=blue)](https://pypistats.org/packages/types-aiobotocore-greengrassv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GreengrassV2 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
+[aiobotocore.GreengrassV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-greengrassv2-2.5.1/types_aiobotocore_greengrassv2.egg-info/SOURCES.txt` & `types-aiobotocore-greengrassv2-2.5.2/types_aiobotocore_greengrassv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*


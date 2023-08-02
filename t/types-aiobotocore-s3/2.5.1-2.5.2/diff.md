# Comparing `tmp/types-aiobotocore-s3-2.5.1.tar.gz` & `tmp/types-aiobotocore-s3-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-s3-2.5.1.tar", last modified: Wed Jun 28 01:44:05 2023, max compression
+gzip compressed data, was "types-aiobotocore-s3-2.5.2.tar", last modified: Sat Jul  8 01:44:14 2023, max compression
```

## Comparing `types-aiobotocore-s3-2.5.1.tar` & `types-aiobotocore-s3-2.5.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:05.714204 types-aiobotocore-s3-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:39:38.000000 types-aiobotocore-s3-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    34160 2023-06-28 01:44:05.710204 types-aiobotocore-s3-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    32615 2023-06-28 01:39:38.000000 types-aiobotocore-s3-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:44:05.714204 types-aiobotocore-s3-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-28 01:39:38.000000 types-aiobotocore-s3-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:05.702204 types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-28 01:39:38.000000 types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-28 01:39:38.000000 types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-28 01:39:38.000000 types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    87383 2023-06-28 01:39:39.000000 types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    87262 2023-06-28 01:39:39.000000 types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16429 2023-06-28 01:39:40.000000 types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-06-28 01:39:40.000000 types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-06-28 01:39:40.000000 types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-06-28 01:39:40.000000 types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:39:38.000000 types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   124738 2023-06-28 01:39:40.000000 types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)   124517 2023-06-28 01:39:40.000000 types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   184232 2023-06-28 01:39:46.000000 types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   183920 2023-06-28 01:39:44.000000 types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:39:38.000000 types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-06-28 01:39:40.000000 types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-06-28 01:39:40.000000 types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:05.710204 types-aiobotocore-s3-2.5.1/types_aiobotocore_s3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    34160 2023-06-28 01:44:05.000000 types-aiobotocore-s3-2.5.1/types_aiobotocore_s3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-28 01:44:05.000000 types-aiobotocore-s3-2.5.1/types_aiobotocore_s3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:44:05.000000 types-aiobotocore-s3-2.5.1/types_aiobotocore_s3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:44:05.000000 types-aiobotocore-s3-2.5.1/types_aiobotocore_s3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:44:05.000000 types-aiobotocore-s3-2.5.1/types_aiobotocore_s3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-28 01:44:05.000000 types-aiobotocore-s3-2.5.1/types_aiobotocore_s3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:14.174812 types-aiobotocore-s3-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:39:42.000000 types-aiobotocore-s3-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    34160 2023-07-08 01:44:14.166812 types-aiobotocore-s3-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    32615 2023-07-08 01:39:42.000000 types-aiobotocore-s3-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:14.174812 types-aiobotocore-s3-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-08 01:39:42.000000 types-aiobotocore-s3-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:14.166812 types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-08 01:39:42.000000 types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-08 01:39:42.000000 types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-08 01:39:42.000000 types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87383 2023-07-08 01:39:43.000000 types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87262 2023-07-08 01:39:43.000000 types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16429 2023-07-08 01:39:45.000000 types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-07-08 01:39:44.000000 types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-07-08 01:39:44.000000 types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-07-08 01:39:44.000000 types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:39:42.000000 types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   124738 2023-07-08 01:39:44.000000 types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124517 2023-07-08 01:39:44.000000 types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   184232 2023-07-08 01:39:51.000000 types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   183920 2023-07-08 01:39:49.000000 types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:39:42.000000 types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-07-08 01:39:44.000000 types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-08 01:39:44.000000 types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:14.166812 types-aiobotocore-s3-2.5.2/types_aiobotocore_s3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    34160 2023-07-08 01:44:13.000000 types-aiobotocore-s3-2.5.2/types_aiobotocore_s3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-08 01:44:14.000000 types-aiobotocore-s3-2.5.2/types_aiobotocore_s3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:14.000000 types-aiobotocore-s3-2.5.2/types_aiobotocore_s3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:13.000000 types-aiobotocore-s3-2.5.2/types_aiobotocore_s3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:14.000000 types-aiobotocore-s3-2.5.2/types_aiobotocore_s3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-08 01:44:14.000000 types-aiobotocore-s3-2.5.2/types_aiobotocore_s3.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-s3-2.5.1/LICENSE` & `types-aiobotocore-s3-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.1/PKG-INFO` & `types-aiobotocore-s3-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-s3
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.S3 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.S3 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-s3.svg?color=blue)](https://pypi.org/project/types-aiobotocore-s3)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-s3?color=blue)](https://pypistats.org/packages/types-aiobotocore-s3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.S3 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
+[aiobotocore.S3 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-s3-2.5.1/README.md` & `types-aiobotocore-s3-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-s3.svg?color=blue)](https://pypi.org/project/types-aiobotocore-s3)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-s3?color=blue)](https://pypistats.org/packages/types-aiobotocore-s3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.S3 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
+[aiobotocore.S3 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-s3-2.5.1/setup.py` & `types-aiobotocore-s3-2.5.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-s3",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_s3"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.S3 2.5.1 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for aiobotocore.S3 2.5.2 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/__init__.py` & `types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/__init__.pyi` & `types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/__main__.py` & `types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.S3 2.5.1\nVersion:         2.5.1\nBuilder version:"
+        "Type annotations for aiobotocore.S3 2.5.2\nVersion:         2.5.2\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3\nOther"
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

### Comparing `types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/client.py` & `types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/client.pyi` & `types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/literals.py` & `types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/literals.pyi` & `types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/paginator.py` & `types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/paginator.pyi` & `types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/service_resource.py` & `types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/service_resource.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/service_resource.pyi` & `types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/type_defs.py` & `types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/type_defs.pyi` & `types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/waiter.py` & `types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.1/types_aiobotocore_s3/waiter.pyi` & `types-aiobotocore-s3-2.5.2/types_aiobotocore_s3/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.1/types_aiobotocore_s3.egg-info/PKG-INFO` & `types-aiobotocore-s3-2.5.2/types_aiobotocore_s3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-s3
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.S3 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.S3 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-s3.svg?color=blue)](https://pypi.org/project/types-aiobotocore-s3)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-s3?color=blue)](https://pypistats.org/packages/types-aiobotocore-s3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.S3 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
+[aiobotocore.S3 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-s3-2.5.1/types_aiobotocore_s3.egg-info/SOURCES.txt` & `types-aiobotocore-s3-2.5.2/types_aiobotocore_s3.egg-info/SOURCES.txt`

 * *Files identical despite different names*


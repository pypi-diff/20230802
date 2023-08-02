# Comparing `tmp/types-aiobotocore-amp-2.5.1.tar.gz` & `tmp/types-aiobotocore-amp-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-amp-2.5.1.tar", last modified: Wed Jun 28 01:43:01 2023, max compression
+gzip compressed data, was "types-aiobotocore-amp-2.5.2.tar", last modified: Sat Jul  8 01:43:09 2023, max compression
```

## Comparing `types-aiobotocore-amp-2.5.1.tar` & `types-aiobotocore-amp-2.5.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:01.678085 types-aiobotocore-amp-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:25:48.000000 types-aiobotocore-amp-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-06-28 01:43:01.678085 types-aiobotocore-amp-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-06-28 01:25:48.000000 types-aiobotocore-amp-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:01.678085 types-aiobotocore-amp-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-28 01:25:48.000000 types-aiobotocore-amp-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:01.678085 types-aiobotocore-amp-2.5.1/types_aiobotocore_amp/
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-28 01:25:48.000000 types-aiobotocore-amp-2.5.1/types_aiobotocore_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-28 01:25:48.000000 types-aiobotocore-amp-2.5.1/types_aiobotocore_amp/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-28 01:25:48.000000 types-aiobotocore-amp-2.5.1/types_aiobotocore_amp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18652 2023-06-28 01:25:48.000000 types-aiobotocore-amp-2.5.1/types_aiobotocore_amp/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18618 2023-06-28 01:25:48.000000 types-aiobotocore-amp-2.5.1/types_aiobotocore_amp/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-06-28 01:25:48.000000 types-aiobotocore-amp-2.5.1/types_aiobotocore_amp/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-06-28 01:25:48.000000 types-aiobotocore-amp-2.5.1/types_aiobotocore_amp/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-28 01:25:48.000000 types-aiobotocore-amp-2.5.1/types_aiobotocore_amp/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-06-28 01:25:48.000000 types-aiobotocore-amp-2.5.1/types_aiobotocore_amp/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:25:48.000000 types-aiobotocore-amp-2.5.1/types_aiobotocore_amp/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22736 2023-06-28 01:25:48.000000 types-aiobotocore-amp-2.5.1/types_aiobotocore_amp/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22691 2023-06-28 01:25:48.000000 types-aiobotocore-amp-2.5.1/types_aiobotocore_amp/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:25:48.000000 types-aiobotocore-amp-2.5.1/types_aiobotocore_amp/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-28 01:25:48.000000 types-aiobotocore-amp-2.5.1/types_aiobotocore_amp/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-06-28 01:25:48.000000 types-aiobotocore-amp-2.5.1/types_aiobotocore_amp/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:01.678085 types-aiobotocore-amp-2.5.1/types_aiobotocore_amp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-06-28 01:43:01.000000 types-aiobotocore-amp-2.5.1/types_aiobotocore_amp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-28 01:43:01.000000 types-aiobotocore-amp-2.5.1/types_aiobotocore_amp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:01.000000 types-aiobotocore-amp-2.5.1/types_aiobotocore_amp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:01.000000 types-aiobotocore-amp-2.5.1/types_aiobotocore_amp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:01.000000 types-aiobotocore-amp-2.5.1/types_aiobotocore_amp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-28 01:43:01.000000 types-aiobotocore-amp-2.5.1/types_aiobotocore_amp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:09.837605 types-aiobotocore-amp-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:25:21.000000 types-aiobotocore-amp-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-07-08 01:43:09.837605 types-aiobotocore-amp-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-07-08 01:25:21.000000 types-aiobotocore-amp-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:09.837605 types-aiobotocore-amp-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-08 01:25:21.000000 types-aiobotocore-amp-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:09.829605 types-aiobotocore-amp-2.5.2/types_aiobotocore_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-08 01:25:21.000000 types-aiobotocore-amp-2.5.2/types_aiobotocore_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-08 01:25:21.000000 types-aiobotocore-amp-2.5.2/types_aiobotocore_amp/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-08 01:25:21.000000 types-aiobotocore-amp-2.5.2/types_aiobotocore_amp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18652 2023-07-08 01:25:22.000000 types-aiobotocore-amp-2.5.2/types_aiobotocore_amp/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18618 2023-07-08 01:25:22.000000 types-aiobotocore-amp-2.5.2/types_aiobotocore_amp/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-07-08 01:25:22.000000 types-aiobotocore-amp-2.5.2/types_aiobotocore_amp/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-07-08 01:25:22.000000 types-aiobotocore-amp-2.5.2/types_aiobotocore_amp/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-08 01:25:22.000000 types-aiobotocore-amp-2.5.2/types_aiobotocore_amp/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-07-08 01:25:22.000000 types-aiobotocore-amp-2.5.2/types_aiobotocore_amp/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:25:21.000000 types-aiobotocore-amp-2.5.2/types_aiobotocore_amp/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22736 2023-07-08 01:25:22.000000 types-aiobotocore-amp-2.5.2/types_aiobotocore_amp/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22691 2023-07-08 01:25:22.000000 types-aiobotocore-amp-2.5.2/types_aiobotocore_amp/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:25:21.000000 types-aiobotocore-amp-2.5.2/types_aiobotocore_amp/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-08 01:25:22.000000 types-aiobotocore-amp-2.5.2/types_aiobotocore_amp/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-08 01:25:22.000000 types-aiobotocore-amp-2.5.2/types_aiobotocore_amp/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:09.837605 types-aiobotocore-amp-2.5.2/types_aiobotocore_amp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-07-08 01:43:09.000000 types-aiobotocore-amp-2.5.2/types_aiobotocore_amp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-08 01:43:09.000000 types-aiobotocore-amp-2.5.2/types_aiobotocore_amp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:09.000000 types-aiobotocore-amp-2.5.2/types_aiobotocore_amp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:09.000000 types-aiobotocore-amp-2.5.2/types_aiobotocore_amp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:09.000000 types-aiobotocore-amp-2.5.2/types_aiobotocore_amp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:43:09.000000 types-aiobotocore-amp-2.5.2/types_aiobotocore_amp.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-amp-2.5.1/LICENSE` & `types-aiobotocore-amp-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.1/PKG-INFO` & `types-aiobotocore-amp-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-amp
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.PrometheusService 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.PrometheusService 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-amp.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amp)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-amp?color=blue)](https://pypistats.org/packages/types-aiobotocore-amp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PrometheusService 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
+[aiobotocore.PrometheusService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-amp-2.5.1/README.md` & `types-aiobotocore-amp-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-amp.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amp)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-amp?color=blue)](https://pypistats.org/packages/types-aiobotocore-amp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PrometheusService 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
+[aiobotocore.PrometheusService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-amp-2.5.1/setup.py` & `types-aiobotocore-amp-2.5.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-amp",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_amp"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.PrometheusService 2.5.1 service generated with"
+        "Type annotations for aiobotocore.PrometheusService 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-amp-2.5.1/types_aiobotocore_amp/__init__.py` & `types-aiobotocore-amp-2.5.2/types_aiobotocore_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.1/types_aiobotocore_amp/__init__.pyi` & `types-aiobotocore-amp-2.5.2/types_aiobotocore_amp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.1/types_aiobotocore_amp/__main__.py` & `types-aiobotocore-amp-2.5.2/types_aiobotocore_amp/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.PrometheusService 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.PrometheusService 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService\nOther"
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

### Comparing `types-aiobotocore-amp-2.5.1/types_aiobotocore_amp/client.py` & `types-aiobotocore-amp-2.5.2/types_aiobotocore_amp/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.1/types_aiobotocore_amp/client.pyi` & `types-aiobotocore-amp-2.5.2/types_aiobotocore_amp/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.1/types_aiobotocore_amp/literals.py` & `types-aiobotocore-amp-2.5.2/types_aiobotocore_amp/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.1/types_aiobotocore_amp/literals.pyi` & `types-aiobotocore-amp-2.5.2/types_aiobotocore_amp/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.1/types_aiobotocore_amp/paginator.py` & `types-aiobotocore-amp-2.5.2/types_aiobotocore_amp/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.1/types_aiobotocore_amp/paginator.pyi` & `types-aiobotocore-amp-2.5.2/types_aiobotocore_amp/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.1/types_aiobotocore_amp/type_defs.py` & `types-aiobotocore-amp-2.5.2/types_aiobotocore_amp/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.1/types_aiobotocore_amp/type_defs.pyi` & `types-aiobotocore-amp-2.5.2/types_aiobotocore_amp/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.1/types_aiobotocore_amp/waiter.py` & `types-aiobotocore-amp-2.5.2/types_aiobotocore_amp/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.1/types_aiobotocore_amp/waiter.pyi` & `types-aiobotocore-amp-2.5.2/types_aiobotocore_amp/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.1/types_aiobotocore_amp.egg-info/PKG-INFO` & `types-aiobotocore-amp-2.5.2/types_aiobotocore_amp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-amp
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.PrometheusService 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.PrometheusService 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-amp.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amp)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-amp?color=blue)](https://pypistats.org/packages/types-aiobotocore-amp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PrometheusService 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
+[aiobotocore.PrometheusService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-amp-2.5.1/types_aiobotocore_amp.egg-info/SOURCES.txt` & `types-aiobotocore-amp-2.5.2/types_aiobotocore_amp.egg-info/SOURCES.txt`

 * *Files identical despite different names*


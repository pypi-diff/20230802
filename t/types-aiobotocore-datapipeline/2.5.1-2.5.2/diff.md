# Comparing `tmp/types-aiobotocore-datapipeline-2.5.1.tar.gz` & `tmp/types-aiobotocore-datapipeline-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-datapipeline-2.5.1.tar", last modified: Wed Jun 28 01:43:22 2023, max compression
+gzip compressed data, was "types-aiobotocore-datapipeline-2.5.2.tar", last modified: Sat Jul  8 01:43:30 2023, max compression
```

## Comparing `types-aiobotocore-datapipeline-2.5.1.tar` & `types-aiobotocore-datapipeline-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:22.038123 types-aiobotocore-datapipeline-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:28:51.000000 types-aiobotocore-datapipeline-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15263 2023-06-28 01:43:22.038123 types-aiobotocore-datapipeline-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13678 2023-06-28 01:28:51.000000 types-aiobotocore-datapipeline-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:22.038123 types-aiobotocore-datapipeline-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-28 01:28:51.000000 types-aiobotocore-datapipeline-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:22.030122 types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-28 01:28:51.000000 types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-28 01:28:51.000000 types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-28 01:28:51.000000 types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18109 2023-06-28 01:28:51.000000 types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18078 2023-06-28 01:28:51.000000 types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-06-28 01:28:52.000000 types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-06-28 01:28:51.000000 types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-06-28 01:28:51.000000 types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-06-28 01:28:51.000000 types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:28:51.000000 types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17925 2023-06-28 01:28:52.000000 types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17893 2023-06-28 01:28:52.000000 types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:28:51.000000 types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:22.038123 types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15263 2023-06-28 01:43:21.000000 types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-28 01:43:21.000000 types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:21.000000 types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:21.000000 types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:21.000000 types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-28 01:43:21.000000 types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:30.057988 types-aiobotocore-datapipeline-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:28:29.000000 types-aiobotocore-datapipeline-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15263 2023-07-08 01:43:30.053988 types-aiobotocore-datapipeline-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13678 2023-07-08 01:28:29.000000 types-aiobotocore-datapipeline-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:30.057988 types-aiobotocore-datapipeline-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-08 01:28:29.000000 types-aiobotocore-datapipeline-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:30.049988 types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-08 01:28:29.000000 types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-08 01:28:29.000000 types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-08 01:28:29.000000 types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18109 2023-07-08 01:28:29.000000 types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18078 2023-07-08 01:28:29.000000 types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-07-08 01:28:29.000000 types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-07-08 01:28:29.000000 types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-08 01:28:29.000000 types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-08 01:28:29.000000 types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:28:29.000000 types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17925 2023-07-08 01:28:30.000000 types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17893 2023-07-08 01:28:30.000000 types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:28:29.000000 types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:30.053988 types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15263 2023-07-08 01:43:29.000000 types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-08 01:43:29.000000 types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:29.000000 types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:29.000000 types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:29.000000 types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-08 01:43:29.000000 types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-datapipeline-2.5.1/LICENSE` & `types-aiobotocore-datapipeline-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datapipeline-2.5.1/PKG-INFO` & `types-aiobotocore-datapipeline-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-datapipeline
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.DataPipeline 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.DataPipeline 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-datapipeline.svg?color=blue)](https://pypi.org/project/types-aiobotocore-datapipeline)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-datapipeline?color=blue)](https://pypistats.org/packages/types-aiobotocore-datapipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DataPipeline 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
+[aiobotocore.DataPipeline 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-datapipeline-2.5.1/README.md` & `types-aiobotocore-datapipeline-2.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-datapipeline.svg?color=blue)](https://pypi.org/project/types-aiobotocore-datapipeline)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-datapipeline?color=blue)](https://pypistats.org/packages/types-aiobotocore-datapipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DataPipeline 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
+[aiobotocore.DataPipeline 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-datapipeline-2.5.1/setup.py` & `types-aiobotocore-datapipeline-2.5.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-datapipeline",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_datapipeline"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DataPipeline 2.5.1 service generated with"
+        "Type annotations for aiobotocore.DataPipeline 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline/__init__.py` & `types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline/__init__.pyi` & `types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline/__main__.py` & `types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DataPipeline 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.DataPipeline 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline\nOther"
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

### Comparing `types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline/client.py` & `types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline/client.pyi` & `types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline/literals.py` & `types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline/literals.pyi` & `types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline/paginator.py` & `types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline/paginator.pyi` & `types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline/type_defs.py` & `types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline/type_defs.pyi` & `types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline.egg-info/PKG-INFO` & `types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-datapipeline
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.DataPipeline 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.DataPipeline 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-datapipeline.svg?color=blue)](https://pypi.org/project/types-aiobotocore-datapipeline)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-datapipeline?color=blue)](https://pypistats.org/packages/types-aiobotocore-datapipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DataPipeline 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
+[aiobotocore.DataPipeline 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-datapipeline-2.5.1/types_aiobotocore_datapipeline.egg-info/SOURCES.txt` & `types-aiobotocore-datapipeline-2.5.2/types_aiobotocore_datapipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*


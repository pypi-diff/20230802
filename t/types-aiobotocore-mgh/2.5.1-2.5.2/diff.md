# Comparing `tmp/types-aiobotocore-mgh-2.5.1.tar.gz` & `tmp/types-aiobotocore-mgh-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mgh-2.5.1.tar", last modified: Wed Jun 28 01:43:52 2023, max compression
+gzip compressed data, was "types-aiobotocore-mgh-2.5.2.tar", last modified: Sat Jul  8 01:44:00 2023, max compression
```

## Comparing `types-aiobotocore-mgh-2.5.1.tar` & `types-aiobotocore-mgh-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:52.038179 types-aiobotocore-mgh-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:35:27.000000 types-aiobotocore-mgh-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-06-28 01:43:52.038179 types-aiobotocore-mgh-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-06-28 01:35:27.000000 types-aiobotocore-mgh-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:52.038179 types-aiobotocore-mgh-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-28 01:35:27.000000 types-aiobotocore-mgh-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:52.038179 types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh/
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-28 01:35:27.000000 types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-28 01:35:27.000000 types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-28 01:35:27.000000 types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18657 2023-06-28 01:35:28.000000 types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18626 2023-06-28 01:35:28.000000 types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8952 2023-06-28 01:35:28.000000 types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-06-28 01:35:28.000000 types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-06-28 01:35:28.000000 types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-06-28 01:35:28.000000 types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:35:27.000000 types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17708 2023-06-28 01:35:28.000000 types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17673 2023-06-28 01:35:28.000000 types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:35:27.000000 types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:52.038179 types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-06-28 01:43:51.000000 types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-28 01:43:51.000000 types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:51.000000 types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:51.000000 types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:51.000000 types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-28 01:43:51.000000 types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:00.398559 types-aiobotocore-mgh-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:35:18.000000 types-aiobotocore-mgh-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-07-08 01:44:00.394559 types-aiobotocore-mgh-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-07-08 01:35:18.000000 types-aiobotocore-mgh-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:00.398559 types-aiobotocore-mgh-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-08 01:35:18.000000 types-aiobotocore-mgh-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:00.394559 types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-08 01:35:18.000000 types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-08 01:35:18.000000 types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-08 01:35:18.000000 types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18657 2023-07-08 01:35:18.000000 types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18626 2023-07-08 01:35:18.000000 types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8952 2023-07-08 01:35:18.000000 types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-07-08 01:35:18.000000 types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-07-08 01:35:18.000000 types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-07-08 01:35:18.000000 types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:35:18.000000 types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17708 2023-07-08 01:35:18.000000 types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17673 2023-07-08 01:35:18.000000 types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:35:18.000000 types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:00.394559 types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-07-08 01:44:00.000000 types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-08 01:44:00.000000 types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:00.000000 types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:00.000000 types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:00.000000 types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:44:00.000000 types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mgh-2.5.1/LICENSE` & `types-aiobotocore-mgh-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.5.1/PKG-INFO` & `types-aiobotocore-mgh-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mgh
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.MigrationHub 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.MigrationHub 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mgh.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mgh)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-mgh?color=blue)](https://pypistats.org/packages/types-aiobotocore-mgh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MigrationHub 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
+[aiobotocore.MigrationHub 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-mgh-2.5.1/README.md` & `types-aiobotocore-mgh-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mgh.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mgh)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-mgh?color=blue)](https://pypistats.org/packages/types-aiobotocore-mgh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MigrationHub 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
+[aiobotocore.MigrationHub 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-mgh-2.5.1/setup.py` & `types-aiobotocore-mgh-2.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mgh",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_mgh"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MigrationHub 2.5.1 service generated with"
+        "Type annotations for aiobotocore.MigrationHub 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh/__init__.py` & `types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh/__init__.pyi` & `types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh/__main__.py` & `types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MigrationHub 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.MigrationHub 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub\nOther"
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

### Comparing `types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh/client.py` & `types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh/client.pyi` & `types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh/literals.py` & `types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh/literals.pyi` & `types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh/paginator.py` & `types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh/paginator.pyi` & `types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh/type_defs.py` & `types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh/type_defs.pyi` & `types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh.egg-info/PKG-INFO` & `types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mgh
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.MigrationHub 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.MigrationHub 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mgh.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mgh)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-mgh?color=blue)](https://pypistats.org/packages/types-aiobotocore-mgh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MigrationHub 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
+[aiobotocore.MigrationHub 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-mgh-2.5.1/types_aiobotocore_mgh.egg-info/SOURCES.txt` & `types-aiobotocore-mgh-2.5.2/types_aiobotocore_mgh.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-rds-data-2.5.1.tar.gz` & `tmp/types-aiobotocore-rds-data-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-rds-data-2.5.1.tar", last modified: Wed Jun 28 01:44:01 2023, max compression
+gzip compressed data, was "types-aiobotocore-rds-data-2.5.2.tar", last modified: Sat Jul  8 01:44:09 2023, max compression
```

## Comparing `types-aiobotocore-rds-data-2.5.1.tar` & `types-aiobotocore-rds-data-2.5.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:01.322196 types-aiobotocore-rds-data-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:38:53.000000 types-aiobotocore-rds-data-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13015 2023-06-28 01:44:01.322196 types-aiobotocore-rds-data-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-06-28 01:38:53.000000 types-aiobotocore-rds-data-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:44:01.322196 types-aiobotocore-rds-data-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-28 01:38:52.000000 types-aiobotocore-rds-data-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:01.318196 types-aiobotocore-rds-data-2.5.1/types_aiobotocore_rds_data/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-28 01:38:53.000000 types-aiobotocore-rds-data-2.5.1/types_aiobotocore_rds_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-28 01:38:53.000000 types-aiobotocore-rds-data-2.5.1/types_aiobotocore_rds_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-28 01:38:53.000000 types-aiobotocore-rds-data-2.5.1/types_aiobotocore_rds_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-06-28 01:38:53.000000 types-aiobotocore-rds-data-2.5.1/types_aiobotocore_rds_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-06-28 01:38:53.000000 types-aiobotocore-rds-data-2.5.1/types_aiobotocore_rds_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-06-28 01:38:53.000000 types-aiobotocore-rds-data-2.5.1/types_aiobotocore_rds_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-06-28 01:38:53.000000 types-aiobotocore-rds-data-2.5.1/types_aiobotocore_rds_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:38:53.000000 types-aiobotocore-rds-data-2.5.1/types_aiobotocore_rds_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-06-28 01:38:53.000000 types-aiobotocore-rds-data-2.5.1/types_aiobotocore_rds_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-06-28 01:38:53.000000 types-aiobotocore-rds-data-2.5.1/types_aiobotocore_rds_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:38:53.000000 types-aiobotocore-rds-data-2.5.1/types_aiobotocore_rds_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:01.322196 types-aiobotocore-rds-data-2.5.1/types_aiobotocore_rds_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13015 2023-06-28 01:44:01.000000 types-aiobotocore-rds-data-2.5.1/types_aiobotocore_rds_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-28 01:44:01.000000 types-aiobotocore-rds-data-2.5.1/types_aiobotocore_rds_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:44:01.000000 types-aiobotocore-rds-data-2.5.1/types_aiobotocore_rds_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:44:01.000000 types-aiobotocore-rds-data-2.5.1/types_aiobotocore_rds_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:44:01.000000 types-aiobotocore-rds-data-2.5.1/types_aiobotocore_rds_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-28 01:44:01.000000 types-aiobotocore-rds-data-2.5.1/types_aiobotocore_rds_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:09.738733 types-aiobotocore-rds-data-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:38:53.000000 types-aiobotocore-rds-data-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13015 2023-07-08 01:44:09.734732 types-aiobotocore-rds-data-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-07-08 01:38:53.000000 types-aiobotocore-rds-data-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:09.738733 types-aiobotocore-rds-data-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-08 01:38:53.000000 types-aiobotocore-rds-data-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:09.730733 types-aiobotocore-rds-data-2.5.2/types_aiobotocore_rds_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-08 01:38:53.000000 types-aiobotocore-rds-data-2.5.2/types_aiobotocore_rds_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-08 01:38:53.000000 types-aiobotocore-rds-data-2.5.2/types_aiobotocore_rds_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-08 01:38:53.000000 types-aiobotocore-rds-data-2.5.2/types_aiobotocore_rds_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-07-08 01:38:54.000000 types-aiobotocore-rds-data-2.5.2/types_aiobotocore_rds_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-07-08 01:38:53.000000 types-aiobotocore-rds-data-2.5.2/types_aiobotocore_rds_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-07-08 01:38:56.000000 types-aiobotocore-rds-data-2.5.2/types_aiobotocore_rds_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-07-08 01:38:56.000000 types-aiobotocore-rds-data-2.5.2/types_aiobotocore_rds_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:38:53.000000 types-aiobotocore-rds-data-2.5.2/types_aiobotocore_rds_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-07-08 01:38:56.000000 types-aiobotocore-rds-data-2.5.2/types_aiobotocore_rds_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-07-08 01:38:56.000000 types-aiobotocore-rds-data-2.5.2/types_aiobotocore_rds_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:38:53.000000 types-aiobotocore-rds-data-2.5.2/types_aiobotocore_rds_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:09.734732 types-aiobotocore-rds-data-2.5.2/types_aiobotocore_rds_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13015 2023-07-08 01:44:09.000000 types-aiobotocore-rds-data-2.5.2/types_aiobotocore_rds_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-08 01:44:09.000000 types-aiobotocore-rds-data-2.5.2/types_aiobotocore_rds_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:09.000000 types-aiobotocore-rds-data-2.5.2/types_aiobotocore_rds_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:09.000000 types-aiobotocore-rds-data-2.5.2/types_aiobotocore_rds_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:09.000000 types-aiobotocore-rds-data-2.5.2/types_aiobotocore_rds_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-08 01:44:09.000000 types-aiobotocore-rds-data-2.5.2/types_aiobotocore_rds_data.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-rds-data-2.5.1/LICENSE` & `types-aiobotocore-rds-data-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rds-data-2.5.1/PKG-INFO` & `types-aiobotocore-rds-data-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rds-data
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.RDSDataService 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.RDSDataService 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rds-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rds-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-rds-data?color=blue)](https://pypistats.org/packages/types-aiobotocore-rds-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RDSDataService 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService)
+[aiobotocore.RDSDataService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-rds-data-2.5.1/README.md` & `types-aiobotocore-rds-data-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rds-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rds-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-rds-data?color=blue)](https://pypistats.org/packages/types-aiobotocore-rds-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RDSDataService 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService)
+[aiobotocore.RDSDataService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-rds-data-2.5.1/setup.py` & `types-aiobotocore-rds-data-2.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-rds-data",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_rds_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.RDSDataService 2.5.1 service generated with"
+        "Type annotations for aiobotocore.RDSDataService 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-rds-data-2.5.1/types_aiobotocore_rds_data/__main__.py` & `types-aiobotocore-rds-data-2.5.2/types_aiobotocore_rds_data/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.RDSDataService 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.RDSDataService 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService\nOther"
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

### Comparing `types-aiobotocore-rds-data-2.5.1/types_aiobotocore_rds_data/client.py` & `types-aiobotocore-rds-data-2.5.2/types_aiobotocore_rds_data/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rds-data-2.5.1/types_aiobotocore_rds_data/client.pyi` & `types-aiobotocore-rds-data-2.5.2/types_aiobotocore_rds_data/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rds-data-2.5.1/types_aiobotocore_rds_data/literals.py` & `types-aiobotocore-rds-data-2.5.2/types_aiobotocore_rds_data/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rds-data-2.5.1/types_aiobotocore_rds_data/literals.pyi` & `types-aiobotocore-rds-data-2.5.2/types_aiobotocore_rds_data/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rds-data-2.5.1/types_aiobotocore_rds_data/type_defs.py` & `types-aiobotocore-rds-data-2.5.2/types_aiobotocore_rds_data/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rds-data-2.5.1/types_aiobotocore_rds_data/type_defs.pyi` & `types-aiobotocore-rds-data-2.5.2/types_aiobotocore_rds_data/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rds-data-2.5.1/types_aiobotocore_rds_data.egg-info/PKG-INFO` & `types-aiobotocore-rds-data-2.5.2/types_aiobotocore_rds_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rds-data
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.RDSDataService 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.RDSDataService 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rds-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rds-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-rds-data?color=blue)](https://pypistats.org/packages/types-aiobotocore-rds-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RDSDataService 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService)
+[aiobotocore.RDSDataService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-rds-data-2.5.1/types_aiobotocore_rds_data.egg-info/SOURCES.txt` & `types-aiobotocore-rds-data-2.5.2/types_aiobotocore_rds_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*


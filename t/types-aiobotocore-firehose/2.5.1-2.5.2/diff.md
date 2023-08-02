# Comparing `tmp/types-aiobotocore-firehose-2.5.1.tar.gz` & `tmp/types-aiobotocore-firehose-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-firehose-2.5.1.tar", last modified: Wed Jun 28 01:43:30 2023, max compression
+gzip compressed data, was "types-aiobotocore-firehose-2.5.2.tar", last modified: Sat Jul  8 01:43:38 2023, max compression
```

## Comparing `types-aiobotocore-firehose-2.5.1.tar` & `types-aiobotocore-firehose-2.5.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:30.590139 types-aiobotocore-firehose-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:31:12.000000 types-aiobotocore-firehose-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-06-28 01:43:30.590139 types-aiobotocore-firehose-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14871 2023-06-28 01:31:12.000000 types-aiobotocore-firehose-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:30.590139 types-aiobotocore-firehose-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-28 01:31:12.000000 types-aiobotocore-firehose-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:30.590139 types-aiobotocore-firehose-2.5.1/types_aiobotocore_firehose/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-28 01:31:12.000000 types-aiobotocore-firehose-2.5.1/types_aiobotocore_firehose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-28 01:31:12.000000 types-aiobotocore-firehose-2.5.1/types_aiobotocore_firehose/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-28 01:31:12.000000 types-aiobotocore-firehose-2.5.1/types_aiobotocore_firehose/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14113 2023-06-28 01:31:12.000000 types-aiobotocore-firehose-2.5.1/types_aiobotocore_firehose/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14093 2023-06-28 01:31:12.000000 types-aiobotocore-firehose-2.5.1/types_aiobotocore_firehose/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-06-28 01:31:12.000000 types-aiobotocore-firehose-2.5.1/types_aiobotocore_firehose/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-06-28 01:31:12.000000 types-aiobotocore-firehose-2.5.1/types_aiobotocore_firehose/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:31:12.000000 types-aiobotocore-firehose-2.5.1/types_aiobotocore_firehose/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    45031 2023-06-28 01:31:13.000000 types-aiobotocore-firehose-2.5.1/types_aiobotocore_firehose/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    44982 2023-06-28 01:31:12.000000 types-aiobotocore-firehose-2.5.1/types_aiobotocore_firehose/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:31:12.000000 types-aiobotocore-firehose-2.5.1/types_aiobotocore_firehose/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:30.590139 types-aiobotocore-firehose-2.5.1/types_aiobotocore_firehose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-06-28 01:43:30.000000 types-aiobotocore-firehose-2.5.1/types_aiobotocore_firehose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-28 01:43:30.000000 types-aiobotocore-firehose-2.5.1/types_aiobotocore_firehose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:30.000000 types-aiobotocore-firehose-2.5.1/types_aiobotocore_firehose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:30.000000 types-aiobotocore-firehose-2.5.1/types_aiobotocore_firehose.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:30.000000 types-aiobotocore-firehose-2.5.1/types_aiobotocore_firehose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-28 01:43:30.000000 types-aiobotocore-firehose-2.5.1/types_aiobotocore_firehose.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:38.842154 types-aiobotocore-firehose-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:30:55.000000 types-aiobotocore-firehose-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-07-08 01:43:38.842154 types-aiobotocore-firehose-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14871 2023-07-08 01:30:55.000000 types-aiobotocore-firehose-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:38.842154 types-aiobotocore-firehose-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-08 01:30:55.000000 types-aiobotocore-firehose-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:38.838154 types-aiobotocore-firehose-2.5.2/types_aiobotocore_firehose/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-08 01:30:55.000000 types-aiobotocore-firehose-2.5.2/types_aiobotocore_firehose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-08 01:30:55.000000 types-aiobotocore-firehose-2.5.2/types_aiobotocore_firehose/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-08 01:30:55.000000 types-aiobotocore-firehose-2.5.2/types_aiobotocore_firehose/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14113 2023-07-08 01:30:55.000000 types-aiobotocore-firehose-2.5.2/types_aiobotocore_firehose/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14093 2023-07-08 01:30:55.000000 types-aiobotocore-firehose-2.5.2/types_aiobotocore_firehose/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-07-08 01:30:55.000000 types-aiobotocore-firehose-2.5.2/types_aiobotocore_firehose/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-07-08 01:30:55.000000 types-aiobotocore-firehose-2.5.2/types_aiobotocore_firehose/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:30:55.000000 types-aiobotocore-firehose-2.5.2/types_aiobotocore_firehose/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    45031 2023-07-08 01:30:56.000000 types-aiobotocore-firehose-2.5.2/types_aiobotocore_firehose/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44982 2023-07-08 01:30:56.000000 types-aiobotocore-firehose-2.5.2/types_aiobotocore_firehose/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:30:55.000000 types-aiobotocore-firehose-2.5.2/types_aiobotocore_firehose/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:38.842154 types-aiobotocore-firehose-2.5.2/types_aiobotocore_firehose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-07-08 01:43:38.000000 types-aiobotocore-firehose-2.5.2/types_aiobotocore_firehose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-08 01:43:38.000000 types-aiobotocore-firehose-2.5.2/types_aiobotocore_firehose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:38.000000 types-aiobotocore-firehose-2.5.2/types_aiobotocore_firehose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:38.000000 types-aiobotocore-firehose-2.5.2/types_aiobotocore_firehose.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:38.000000 types-aiobotocore-firehose-2.5.2/types_aiobotocore_firehose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-08 01:43:38.000000 types-aiobotocore-firehose-2.5.2/types_aiobotocore_firehose.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-firehose-2.5.1/LICENSE` & `types-aiobotocore-firehose-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-firehose-2.5.1/PKG-INFO` & `types-aiobotocore-firehose-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-firehose
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.Firehose 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.Firehose 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-firehose.svg?color=blue)](https://pypi.org/project/types-aiobotocore-firehose)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-firehose?color=blue)](https://pypistats.org/packages/types-aiobotocore-firehose)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Firehose 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
+[aiobotocore.Firehose 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-firehose-2.5.1/README.md` & `types-aiobotocore-firehose-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-firehose.svg?color=blue)](https://pypi.org/project/types-aiobotocore-firehose)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-firehose?color=blue)](https://pypistats.org/packages/types-aiobotocore-firehose)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Firehose 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
+[aiobotocore.Firehose 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-firehose-2.5.1/setup.py` & `types-aiobotocore-firehose-2.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-firehose",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_firehose"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Firehose 2.5.1 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Firehose 2.5.2 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-firehose-2.5.1/types_aiobotocore_firehose/__main__.py` & `types-aiobotocore-firehose-2.5.2/types_aiobotocore_firehose/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Firehose 2.5.1\nVersion:         2.5.1\nBuilder version:"
+        "Type annotations for aiobotocore.Firehose 2.5.2\nVersion:         2.5.2\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose\nOther"
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

### Comparing `types-aiobotocore-firehose-2.5.1/types_aiobotocore_firehose/client.py` & `types-aiobotocore-firehose-2.5.2/types_aiobotocore_firehose/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-firehose-2.5.1/types_aiobotocore_firehose/client.pyi` & `types-aiobotocore-firehose-2.5.2/types_aiobotocore_firehose/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-firehose-2.5.1/types_aiobotocore_firehose/literals.py` & `types-aiobotocore-firehose-2.5.2/types_aiobotocore_firehose/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-firehose-2.5.1/types_aiobotocore_firehose/literals.pyi` & `types-aiobotocore-firehose-2.5.2/types_aiobotocore_firehose/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-firehose-2.5.1/types_aiobotocore_firehose/type_defs.py` & `types-aiobotocore-firehose-2.5.2/types_aiobotocore_firehose/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-firehose-2.5.1/types_aiobotocore_firehose/type_defs.pyi` & `types-aiobotocore-firehose-2.5.2/types_aiobotocore_firehose/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-firehose-2.5.1/types_aiobotocore_firehose.egg-info/PKG-INFO` & `types-aiobotocore-firehose-2.5.2/types_aiobotocore_firehose.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-firehose
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.Firehose 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.Firehose 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-firehose.svg?color=blue)](https://pypi.org/project/types-aiobotocore-firehose)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-firehose?color=blue)](https://pypistats.org/packages/types-aiobotocore-firehose)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Firehose 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
+[aiobotocore.Firehose 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-firehose-2.5.1/types_aiobotocore_firehose.egg-info/SOURCES.txt` & `types-aiobotocore-firehose-2.5.2/types_aiobotocore_firehose.egg-info/SOURCES.txt`

 * *Files identical despite different names*


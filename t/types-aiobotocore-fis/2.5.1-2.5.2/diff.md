# Comparing `tmp/types-aiobotocore-fis-2.5.1.tar.gz` & `tmp/types-aiobotocore-fis-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-fis-2.5.1.tar", last modified: Wed Jun 28 01:43:30 2023, max compression
+gzip compressed data, was "types-aiobotocore-fis-2.5.2.tar", last modified: Sat Jul  8 01:43:39 2023, max compression
```

## Comparing `types-aiobotocore-fis-2.5.1.tar` & `types-aiobotocore-fis-2.5.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:30.878139 types-aiobotocore-fis-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:31:14.000000 types-aiobotocore-fis-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14715 2023-06-28 01:43:30.878139 types-aiobotocore-fis-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-06-28 01:31:14.000000 types-aiobotocore-fis-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:30.878139 types-aiobotocore-fis-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-28 01:31:14.000000 types-aiobotocore-fis-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:30.878139 types-aiobotocore-fis-2.5.1/types_aiobotocore_fis/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-28 01:31:14.000000 types-aiobotocore-fis-2.5.1/types_aiobotocore_fis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-28 01:31:14.000000 types-aiobotocore-fis-2.5.1/types_aiobotocore_fis/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-28 01:31:14.000000 types-aiobotocore-fis-2.5.1/types_aiobotocore_fis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-06-28 01:31:14.000000 types-aiobotocore-fis-2.5.1/types_aiobotocore_fis/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13590 2023-06-28 01:31:14.000000 types-aiobotocore-fis-2.5.1/types_aiobotocore_fis/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-06-28 01:31:14.000000 types-aiobotocore-fis-2.5.1/types_aiobotocore_fis/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-06-28 01:31:14.000000 types-aiobotocore-fis-2.5.1/types_aiobotocore_fis/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:31:14.000000 types-aiobotocore-fis-2.5.1/types_aiobotocore_fis/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23919 2023-06-28 01:31:15.000000 types-aiobotocore-fis-2.5.1/types_aiobotocore_fis/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23896 2023-06-28 01:31:15.000000 types-aiobotocore-fis-2.5.1/types_aiobotocore_fis/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:31:14.000000 types-aiobotocore-fis-2.5.1/types_aiobotocore_fis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:30.878139 types-aiobotocore-fis-2.5.1/types_aiobotocore_fis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14715 2023-06-28 01:43:30.000000 types-aiobotocore-fis-2.5.1/types_aiobotocore_fis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-28 01:43:30.000000 types-aiobotocore-fis-2.5.1/types_aiobotocore_fis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:30.000000 types-aiobotocore-fis-2.5.1/types_aiobotocore_fis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:30.000000 types-aiobotocore-fis-2.5.1/types_aiobotocore_fis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:30.000000 types-aiobotocore-fis-2.5.1/types_aiobotocore_fis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-28 01:43:30.000000 types-aiobotocore-fis-2.5.1/types_aiobotocore_fis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:38.994157 types-aiobotocore-fis-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:30:56.000000 types-aiobotocore-fis-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14715 2023-07-08 01:43:38.994157 types-aiobotocore-fis-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-07-08 01:30:56.000000 types-aiobotocore-fis-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:38.994157 types-aiobotocore-fis-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-08 01:30:56.000000 types-aiobotocore-fis-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:38.990157 types-aiobotocore-fis-2.5.2/types_aiobotocore_fis/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-08 01:30:56.000000 types-aiobotocore-fis-2.5.2/types_aiobotocore_fis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-08 01:30:56.000000 types-aiobotocore-fis-2.5.2/types_aiobotocore_fis/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-08 01:30:56.000000 types-aiobotocore-fis-2.5.2/types_aiobotocore_fis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-07-08 01:30:57.000000 types-aiobotocore-fis-2.5.2/types_aiobotocore_fis/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13590 2023-07-08 01:30:56.000000 types-aiobotocore-fis-2.5.2/types_aiobotocore_fis/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-07-08 01:30:57.000000 types-aiobotocore-fis-2.5.2/types_aiobotocore_fis/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-07-08 01:30:57.000000 types-aiobotocore-fis-2.5.2/types_aiobotocore_fis/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:30:56.000000 types-aiobotocore-fis-2.5.2/types_aiobotocore_fis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23919 2023-07-08 01:30:57.000000 types-aiobotocore-fis-2.5.2/types_aiobotocore_fis/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23896 2023-07-08 01:30:57.000000 types-aiobotocore-fis-2.5.2/types_aiobotocore_fis/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:30:56.000000 types-aiobotocore-fis-2.5.2/types_aiobotocore_fis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:38.994157 types-aiobotocore-fis-2.5.2/types_aiobotocore_fis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14715 2023-07-08 01:43:38.000000 types-aiobotocore-fis-2.5.2/types_aiobotocore_fis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-08 01:43:38.000000 types-aiobotocore-fis-2.5.2/types_aiobotocore_fis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:38.000000 types-aiobotocore-fis-2.5.2/types_aiobotocore_fis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:38.000000 types-aiobotocore-fis-2.5.2/types_aiobotocore_fis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:38.000000 types-aiobotocore-fis-2.5.2/types_aiobotocore_fis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:43:38.000000 types-aiobotocore-fis-2.5.2/types_aiobotocore_fis.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-fis-2.5.1/LICENSE` & `types-aiobotocore-fis-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fis-2.5.1/PKG-INFO` & `types-aiobotocore-fis-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-fis
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.FIS 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.FIS 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-fis.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fis)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-fis?color=blue)](https://pypistats.org/packages/types-aiobotocore-fis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FIS 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
+[aiobotocore.FIS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-fis-2.5.1/README.md` & `types-aiobotocore-fis-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-fis.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fis)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-fis?color=blue)](https://pypistats.org/packages/types-aiobotocore-fis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FIS 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
+[aiobotocore.FIS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-fis-2.5.1/setup.py` & `types-aiobotocore-fis-2.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-fis",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_fis"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.FIS 2.5.1 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.FIS 2.5.2 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-fis-2.5.1/types_aiobotocore_fis/__main__.py` & `types-aiobotocore-fis-2.5.2/types_aiobotocore_fis/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.FIS 2.5.1\nVersion:         2.5.1\nBuilder version:"
+        "Type annotations for aiobotocore.FIS 2.5.2\nVersion:         2.5.2\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS\nOther"
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

### Comparing `types-aiobotocore-fis-2.5.1/types_aiobotocore_fis/client.py` & `types-aiobotocore-fis-2.5.2/types_aiobotocore_fis/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fis-2.5.1/types_aiobotocore_fis/client.pyi` & `types-aiobotocore-fis-2.5.2/types_aiobotocore_fis/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fis-2.5.1/types_aiobotocore_fis/literals.py` & `types-aiobotocore-fis-2.5.2/types_aiobotocore_fis/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fis-2.5.1/types_aiobotocore_fis/literals.pyi` & `types-aiobotocore-fis-2.5.2/types_aiobotocore_fis/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fis-2.5.1/types_aiobotocore_fis/type_defs.py` & `types-aiobotocore-fis-2.5.2/types_aiobotocore_fis/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fis-2.5.1/types_aiobotocore_fis/type_defs.pyi` & `types-aiobotocore-fis-2.5.2/types_aiobotocore_fis/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fis-2.5.1/types_aiobotocore_fis.egg-info/PKG-INFO` & `types-aiobotocore-fis-2.5.2/types_aiobotocore_fis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-fis
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.FIS 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.FIS 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-fis.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fis)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-fis?color=blue)](https://pypistats.org/packages/types-aiobotocore-fis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FIS 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
+[aiobotocore.FIS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-fis-2.5.1/types_aiobotocore_fis.egg-info/SOURCES.txt` & `types-aiobotocore-fis-2.5.2/types_aiobotocore_fis.egg-info/SOURCES.txt`

 * *Files identical despite different names*


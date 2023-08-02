# Comparing `tmp/types-aiobotocore-dax-2.5.1.tar.gz` & `tmp/types-aiobotocore-dax-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-dax-2.5.1.tar", last modified: Wed Jun 28 01:43:22 2023, max compression
+gzip compressed data, was "types-aiobotocore-dax-2.5.2.tar", last modified: Sat Jul  8 01:43:30 2023, max compression
```

## Comparing `types-aiobotocore-dax-2.5.1.tar` & `types-aiobotocore-dax-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:22.406123 types-aiobotocore-dax-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:28:56.000000 types-aiobotocore-dax-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16492 2023-06-28 01:43:22.402123 types-aiobotocore-dax-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-06-28 01:28:56.000000 types-aiobotocore-dax-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:22.406123 types-aiobotocore-dax-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-28 01:28:56.000000 types-aiobotocore-dax-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:22.402123 types-aiobotocore-dax-2.5.1/types_aiobotocore_dax/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-28 01:28:56.000000 types-aiobotocore-dax-2.5.1/types_aiobotocore_dax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-28 01:28:56.000000 types-aiobotocore-dax-2.5.1/types_aiobotocore_dax/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-28 01:28:56.000000 types-aiobotocore-dax-2.5.1/types_aiobotocore_dax/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22015 2023-06-28 01:28:56.000000 types-aiobotocore-dax-2.5.1/types_aiobotocore_dax/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21978 2023-06-28 01:28:56.000000 types-aiobotocore-dax-2.5.1/types_aiobotocore_dax/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9269 2023-06-28 01:28:56.000000 types-aiobotocore-dax-2.5.1/types_aiobotocore_dax/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9267 2023-06-28 01:28:56.000000 types-aiobotocore-dax-2.5.1/types_aiobotocore_dax/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9035 2023-06-28 01:28:56.000000 types-aiobotocore-dax-2.5.1/types_aiobotocore_dax/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9026 2023-06-28 01:28:56.000000 types-aiobotocore-dax-2.5.1/types_aiobotocore_dax/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:28:56.000000 types-aiobotocore-dax-2.5.1/types_aiobotocore_dax/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22407 2023-06-28 01:28:57.000000 types-aiobotocore-dax-2.5.1/types_aiobotocore_dax/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22384 2023-06-28 01:28:57.000000 types-aiobotocore-dax-2.5.1/types_aiobotocore_dax/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:28:56.000000 types-aiobotocore-dax-2.5.1/types_aiobotocore_dax/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:22.402123 types-aiobotocore-dax-2.5.1/types_aiobotocore_dax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16492 2023-06-28 01:43:22.000000 types-aiobotocore-dax-2.5.1/types_aiobotocore_dax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-28 01:43:22.000000 types-aiobotocore-dax-2.5.1/types_aiobotocore_dax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:22.000000 types-aiobotocore-dax-2.5.1/types_aiobotocore_dax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:22.000000 types-aiobotocore-dax-2.5.1/types_aiobotocore_dax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:22.000000 types-aiobotocore-dax-2.5.1/types_aiobotocore_dax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-28 01:43:22.000000 types-aiobotocore-dax-2.5.1/types_aiobotocore_dax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:30.641999 types-aiobotocore-dax-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:28:33.000000 types-aiobotocore-dax-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16492 2023-07-08 01:43:30.641999 types-aiobotocore-dax-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-07-08 01:28:33.000000 types-aiobotocore-dax-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:30.641999 types-aiobotocore-dax-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-08 01:28:33.000000 types-aiobotocore-dax-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:30.633999 types-aiobotocore-dax-2.5.2/types_aiobotocore_dax/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-08 01:28:34.000000 types-aiobotocore-dax-2.5.2/types_aiobotocore_dax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-08 01:28:34.000000 types-aiobotocore-dax-2.5.2/types_aiobotocore_dax/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-08 01:28:34.000000 types-aiobotocore-dax-2.5.2/types_aiobotocore_dax/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22015 2023-07-08 01:28:34.000000 types-aiobotocore-dax-2.5.2/types_aiobotocore_dax/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21978 2023-07-08 01:28:34.000000 types-aiobotocore-dax-2.5.2/types_aiobotocore_dax/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9269 2023-07-08 01:28:35.000000 types-aiobotocore-dax-2.5.2/types_aiobotocore_dax/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9267 2023-07-08 01:28:35.000000 types-aiobotocore-dax-2.5.2/types_aiobotocore_dax/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9035 2023-07-08 01:28:34.000000 types-aiobotocore-dax-2.5.2/types_aiobotocore_dax/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9026 2023-07-08 01:28:34.000000 types-aiobotocore-dax-2.5.2/types_aiobotocore_dax/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:28:34.000000 types-aiobotocore-dax-2.5.2/types_aiobotocore_dax/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22407 2023-07-08 01:28:35.000000 types-aiobotocore-dax-2.5.2/types_aiobotocore_dax/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22384 2023-07-08 01:28:35.000000 types-aiobotocore-dax-2.5.2/types_aiobotocore_dax/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:28:33.000000 types-aiobotocore-dax-2.5.2/types_aiobotocore_dax/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:30.641999 types-aiobotocore-dax-2.5.2/types_aiobotocore_dax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16492 2023-07-08 01:43:30.000000 types-aiobotocore-dax-2.5.2/types_aiobotocore_dax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-08 01:43:30.000000 types-aiobotocore-dax-2.5.2/types_aiobotocore_dax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:30.000000 types-aiobotocore-dax-2.5.2/types_aiobotocore_dax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:30.000000 types-aiobotocore-dax-2.5.2/types_aiobotocore_dax.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:30.000000 types-aiobotocore-dax-2.5.2/types_aiobotocore_dax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:43:30.000000 types-aiobotocore-dax-2.5.2/types_aiobotocore_dax.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-dax-2.5.1/LICENSE` & `types-aiobotocore-dax-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dax-2.5.1/PKG-INFO` & `types-aiobotocore-dax-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dax
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.DAX 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.DAX 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dax.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dax)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-dax?color=blue)](https://pypistats.org/packages/types-aiobotocore-dax)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DAX 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
+[aiobotocore.DAX 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-dax-2.5.1/README.md` & `types-aiobotocore-dax-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dax.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dax)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-dax?color=blue)](https://pypistats.org/packages/types-aiobotocore-dax)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DAX 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
+[aiobotocore.DAX 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-dax-2.5.1/setup.py` & `types-aiobotocore-dax-2.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-dax",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_dax"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DAX 2.5.1 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.DAX 2.5.2 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-dax-2.5.1/types_aiobotocore_dax/__init__.py` & `types-aiobotocore-dax-2.5.2/types_aiobotocore_dax/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dax-2.5.1/types_aiobotocore_dax/__init__.pyi` & `types-aiobotocore-dax-2.5.2/types_aiobotocore_dax/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dax-2.5.1/types_aiobotocore_dax/__main__.py` & `types-aiobotocore-dax-2.5.2/types_aiobotocore_dax/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DAX 2.5.1\nVersion:         2.5.1\nBuilder version:"
+        "Type annotations for aiobotocore.DAX 2.5.2\nVersion:         2.5.2\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX\nOther"
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

### Comparing `types-aiobotocore-dax-2.5.1/types_aiobotocore_dax/client.py` & `types-aiobotocore-dax-2.5.2/types_aiobotocore_dax/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dax-2.5.1/types_aiobotocore_dax/client.pyi` & `types-aiobotocore-dax-2.5.2/types_aiobotocore_dax/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dax-2.5.1/types_aiobotocore_dax/literals.py` & `types-aiobotocore-dax-2.5.2/types_aiobotocore_dax/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dax-2.5.1/types_aiobotocore_dax/literals.pyi` & `types-aiobotocore-dax-2.5.2/types_aiobotocore_dax/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dax-2.5.1/types_aiobotocore_dax/paginator.py` & `types-aiobotocore-dax-2.5.2/types_aiobotocore_dax/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dax-2.5.1/types_aiobotocore_dax/paginator.pyi` & `types-aiobotocore-dax-2.5.2/types_aiobotocore_dax/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dax-2.5.1/types_aiobotocore_dax/type_defs.py` & `types-aiobotocore-dax-2.5.2/types_aiobotocore_dax/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dax-2.5.1/types_aiobotocore_dax/type_defs.pyi` & `types-aiobotocore-dax-2.5.2/types_aiobotocore_dax/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dax-2.5.1/types_aiobotocore_dax.egg-info/PKG-INFO` & `types-aiobotocore-dax-2.5.2/types_aiobotocore_dax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dax
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.DAX 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.DAX 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dax.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dax)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-dax?color=blue)](https://pypistats.org/packages/types-aiobotocore-dax)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DAX 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
+[aiobotocore.DAX 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-dax-2.5.1/types_aiobotocore_dax.egg-info/SOURCES.txt` & `types-aiobotocore-dax-2.5.2/types_aiobotocore_dax.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-lightsail-2.5.1.tar.gz` & `tmp/types-aiobotocore-lightsail-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lightsail-2.5.1.tar", last modified: Wed Jun 28 01:43:46 2023, max compression
+gzip compressed data, was "types-aiobotocore-lightsail-2.5.2.tar", last modified: Sat Jul  8 01:43:54 2023, max compression
```

## Comparing `types-aiobotocore-lightsail-2.5.1.tar` & `types-aiobotocore-lightsail-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:46.506168 types-aiobotocore-lightsail-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:34:19.000000 types-aiobotocore-lightsail-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    37006 2023-06-28 01:43:46.502169 types-aiobotocore-lightsail-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35433 2023-06-28 01:34:19.000000 types-aiobotocore-lightsail-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:46.506168 types-aiobotocore-lightsail-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-28 01:34:19.000000 types-aiobotocore-lightsail-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:46.502169 types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail/
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-06-28 01:34:19.000000 types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-06-28 01:34:19.000000 types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-28 01:34:19.000000 types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   119354 2023-06-28 01:34:21.000000 types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   119166 2023-06-28 01:34:19.000000 types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25240 2023-06-28 01:34:21.000000 types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    25238 2023-06-28 01:34:21.000000 types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    24021 2023-06-28 01:34:21.000000 types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    23998 2023-06-28 01:34:21.000000 types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:34:19.000000 types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   146658 2023-06-28 01:34:24.000000 types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   146559 2023-06-28 01:34:23.000000 types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:34:19.000000 types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:46.502169 types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    37006 2023-06-28 01:43:46.000000 types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-28 01:43:46.000000 types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:46.000000 types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:46.000000 types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:46.000000 types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-28 01:43:46.000000 types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:54.778454 types-aiobotocore-lightsail-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:34:08.000000 types-aiobotocore-lightsail-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    37006 2023-07-08 01:43:54.770454 types-aiobotocore-lightsail-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35433 2023-07-08 01:34:08.000000 types-aiobotocore-lightsail-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:54.778454 types-aiobotocore-lightsail-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-08 01:34:08.000000 types-aiobotocore-lightsail-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:54.770454 types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail/
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-07-08 01:34:08.000000 types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-07-08 01:34:08.000000 types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-08 01:34:08.000000 types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119354 2023-07-08 01:34:09.000000 types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119166 2023-07-08 01:34:08.000000 types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25240 2023-07-08 01:34:09.000000 types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25238 2023-07-08 01:34:09.000000 types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    24021 2023-07-08 01:34:09.000000 types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23998 2023-07-08 01:34:09.000000 types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:34:08.000000 types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   146658 2023-07-08 01:34:14.000000 types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146559 2023-07-08 01:34:12.000000 types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:34:08.000000 types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:54.770454 types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    37006 2023-07-08 01:43:54.000000 types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-08 01:43:54.000000 types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:54.000000 types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:54.000000 types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:54.000000 types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-08 01:43:54.000000 types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lightsail-2.5.1/LICENSE` & `types-aiobotocore-lightsail-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lightsail-2.5.1/PKG-INFO` & `types-aiobotocore-lightsail-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lightsail
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.Lightsail 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.Lightsail 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lightsail.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lightsail)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-lightsail?color=blue)](https://pypistats.org/packages/types-aiobotocore-lightsail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Lightsail 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
+[aiobotocore.Lightsail 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-lightsail-2.5.1/README.md` & `types-aiobotocore-lightsail-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lightsail.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lightsail)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-lightsail?color=blue)](https://pypistats.org/packages/types-aiobotocore-lightsail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Lightsail 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
+[aiobotocore.Lightsail 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-lightsail-2.5.1/setup.py` & `types-aiobotocore-lightsail-2.5.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lightsail",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_lightsail"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Lightsail 2.5.1 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Lightsail 2.5.2 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail/__init__.py` & `types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail/__init__.pyi` & `types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail/__main__.py` & `types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Lightsail 2.5.1\nVersion:         2.5.1\nBuilder version:"
+        "Type annotations for aiobotocore.Lightsail 2.5.2\nVersion:         2.5.2\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail\nOther"
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

### Comparing `types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail/client.py` & `types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail/client.pyi` & `types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail/literals.py` & `types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail/literals.pyi` & `types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail/paginator.py` & `types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail/paginator.pyi` & `types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail/type_defs.py` & `types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail/type_defs.pyi` & `types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail.egg-info/PKG-INFO` & `types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lightsail
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.Lightsail 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.Lightsail 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lightsail.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lightsail)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-lightsail?color=blue)](https://pypistats.org/packages/types-aiobotocore-lightsail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Lightsail 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
+[aiobotocore.Lightsail 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-lightsail-2.5.1/types_aiobotocore_lightsail.egg-info/SOURCES.txt` & `types-aiobotocore-lightsail-2.5.2/types_aiobotocore_lightsail.egg-info/SOURCES.txt`

 * *Files identical despite different names*


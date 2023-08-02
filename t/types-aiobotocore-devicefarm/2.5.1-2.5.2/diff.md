# Comparing `tmp/types-aiobotocore-devicefarm-2.5.1.tar.gz` & `tmp/types-aiobotocore-devicefarm-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-devicefarm-2.5.1.tar", last modified: Wed Jun 28 01:43:22 2023, max compression
+gzip compressed data, was "types-aiobotocore-devicefarm-2.5.2.tar", last modified: Sat Jul  8 01:43:30 2023, max compression
```

## Comparing `types-aiobotocore-devicefarm-2.5.1.tar` & `types-aiobotocore-devicefarm-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:22.518123 types-aiobotocore-devicefarm-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:28:59.000000 types-aiobotocore-devicefarm-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25182 2023-06-28 01:43:22.514123 types-aiobotocore-devicefarm-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23605 2023-06-28 01:28:59.000000 types-aiobotocore-devicefarm-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:22.518123 types-aiobotocore-devicefarm-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-28 01:28:58.000000 types-aiobotocore-devicefarm-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:22.514123 types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm/
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-06-28 01:28:59.000000 types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-06-28 01:28:59.000000 types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-28 01:28:59.000000 types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60984 2023-06-28 01:29:00.000000 types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    60878 2023-06-28 01:29:00.000000 types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-06-28 01:29:00.000000 types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-06-28 01:29:00.000000 types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23406 2023-06-28 01:29:00.000000 types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    23384 2023-06-28 01:29:00.000000 types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:28:59.000000 types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    73270 2023-06-28 01:29:02.000000 types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    73179 2023-06-28 01:29:01.000000 types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:28:59.000000 types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:22.514123 types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25182 2023-06-28 01:43:22.000000 types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-28 01:43:22.000000 types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:22.000000 types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:22.000000 types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:22.000000 types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-28 01:43:22.000000 types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:30.722001 types-aiobotocore-devicefarm-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:28:37.000000 types-aiobotocore-devicefarm-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25182 2023-07-08 01:43:30.722001 types-aiobotocore-devicefarm-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23605 2023-07-08 01:28:37.000000 types-aiobotocore-devicefarm-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:30.722001 types-aiobotocore-devicefarm-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-08 01:28:37.000000 types-aiobotocore-devicefarm-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:30.722001 types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm/
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-07-08 01:28:37.000000 types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-07-08 01:28:37.000000 types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-08 01:28:37.000000 types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60984 2023-07-08 01:28:38.000000 types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60878 2023-07-08 01:28:37.000000 types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-07-08 01:28:39.000000 types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-07-08 01:28:39.000000 types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23406 2023-07-08 01:28:38.000000 types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23384 2023-07-08 01:28:38.000000 types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:28:37.000000 types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    73270 2023-07-08 01:28:40.000000 types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73179 2023-07-08 01:28:39.000000 types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:28:37.000000 types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:30.722001 types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25182 2023-07-08 01:43:30.000000 types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-08 01:43:30.000000 types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:30.000000 types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:30.000000 types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:30.000000 types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-08 01:43:30.000000 types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-devicefarm-2.5.1/LICENSE` & `types-aiobotocore-devicefarm-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devicefarm-2.5.1/PKG-INFO` & `types-aiobotocore-devicefarm-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-devicefarm
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.DeviceFarm 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.DeviceFarm 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-devicefarm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-devicefarm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-devicefarm?color=blue)](https://pypistats.org/packages/types-aiobotocore-devicefarm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DeviceFarm 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
+[aiobotocore.DeviceFarm 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-devicefarm-2.5.1/README.md` & `types-aiobotocore-devicefarm-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-devicefarm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-devicefarm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-devicefarm?color=blue)](https://pypistats.org/packages/types-aiobotocore-devicefarm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DeviceFarm 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
+[aiobotocore.DeviceFarm 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-devicefarm-2.5.1/setup.py` & `types-aiobotocore-devicefarm-2.5.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-devicefarm",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_devicefarm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DeviceFarm 2.5.1 service generated with"
+        "Type annotations for aiobotocore.DeviceFarm 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm/__init__.py` & `types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm/__init__.pyi` & `types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm/__main__.py` & `types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DeviceFarm 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.DeviceFarm 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm\nOther"
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

### Comparing `types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm/client.py` & `types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm/client.pyi` & `types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm/literals.py` & `types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm/literals.pyi` & `types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm/paginator.py` & `types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm/paginator.pyi` & `types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm/type_defs.py` & `types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm/type_defs.pyi` & `types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm.egg-info/PKG-INFO` & `types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-devicefarm
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.DeviceFarm 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.DeviceFarm 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-devicefarm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-devicefarm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-devicefarm?color=blue)](https://pypistats.org/packages/types-aiobotocore-devicefarm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DeviceFarm 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
+[aiobotocore.DeviceFarm 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-devicefarm-2.5.1/types_aiobotocore_devicefarm.egg-info/SOURCES.txt` & `types-aiobotocore-devicefarm-2.5.2/types_aiobotocore_devicefarm.egg-info/SOURCES.txt`

 * *Files identical despite different names*


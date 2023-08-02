# Comparing `tmp/types-aiobotocore-groundstation-2.5.1.tar.gz` & `tmp/types-aiobotocore-groundstation-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-groundstation-2.5.1.tar", last modified: Wed Jun 28 01:43:33 2023, max compression
+gzip compressed data, was "types-aiobotocore-groundstation-2.5.2.tar", last modified: Sat Jul  8 01:43:42 2023, max compression
```

## Comparing `types-aiobotocore-groundstation-2.5.1.tar` & `types-aiobotocore-groundstation-2.5.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:33.826145 types-aiobotocore-groundstation-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:32:04.000000 types-aiobotocore-groundstation-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19730 2023-06-28 01:43:33.826145 types-aiobotocore-groundstation-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18141 2023-06-28 01:32:04.000000 types-aiobotocore-groundstation-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:33.826145 types-aiobotocore-groundstation-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-28 01:32:03.000000 types-aiobotocore-groundstation-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:33.826145 types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation/
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-28 01:32:04.000000 types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-28 01:32:04.000000 types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-28 01:32:04.000000 types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28856 2023-06-28 01:32:04.000000 types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28806 2023-06-28 01:32:04.000000 types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10902 2023-06-28 01:32:04.000000 types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10900 2023-06-28 01:32:04.000000 types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-06-28 01:32:04.000000 types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-06-28 01:32:04.000000 types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:32:04.000000 types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    40205 2023-06-28 01:32:05.000000 types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40156 2023-06-28 01:32:04.000000 types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:32:04.000000 types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-28 01:32:04.000000 types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-28 01:32:04.000000 types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:33.826145 types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19730 2023-06-28 01:43:33.000000 types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-28 01:43:33.000000 types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:33.000000 types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:33.000000 types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:33.000000 types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-28 01:43:33.000000 types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:42.150217 types-aiobotocore-groundstation-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:31:48.000000 types-aiobotocore-groundstation-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19730 2023-07-08 01:43:42.150217 types-aiobotocore-groundstation-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18141 2023-07-08 01:31:48.000000 types-aiobotocore-groundstation-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:42.150217 types-aiobotocore-groundstation-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-08 01:31:48.000000 types-aiobotocore-groundstation-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:42.142217 types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-08 01:31:48.000000 types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-08 01:31:48.000000 types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-08 01:31:48.000000 types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28856 2023-07-08 01:31:48.000000 types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28806 2023-07-08 01:31:48.000000 types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10902 2023-07-08 01:31:49.000000 types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10900 2023-07-08 01:31:49.000000 types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-07-08 01:31:49.000000 types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-07-08 01:31:49.000000 types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:31:48.000000 types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    40205 2023-07-08 01:31:50.000000 types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40156 2023-07-08 01:31:50.000000 types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:31:48.000000 types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-08 01:31:49.000000 types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-08 01:31:49.000000 types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:42.150217 types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19730 2023-07-08 01:43:41.000000 types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-08 01:43:42.000000 types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:41.000000 types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:41.000000 types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:41.000000 types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-08 01:43:41.000000 types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-groundstation-2.5.1/LICENSE` & `types-aiobotocore-groundstation-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.1/PKG-INFO` & `types-aiobotocore-groundstation-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-groundstation
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.GroundStation 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.GroundStation 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-groundstation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-groundstation)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-groundstation?color=blue)](https://pypistats.org/packages/types-aiobotocore-groundstation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GroundStation 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
+[aiobotocore.GroundStation 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-groundstation-2.5.1/README.md` & `types-aiobotocore-groundstation-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-groundstation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-groundstation)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-groundstation?color=blue)](https://pypistats.org/packages/types-aiobotocore-groundstation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GroundStation 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
+[aiobotocore.GroundStation 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-groundstation-2.5.1/setup.py` & `types-aiobotocore-groundstation-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-groundstation",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_groundstation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.GroundStation 2.5.1 service generated with"
+        "Type annotations for aiobotocore.GroundStation 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation/__init__.py` & `types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation/__init__.pyi` & `types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation/__main__.py` & `types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.GroundStation 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.GroundStation 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation\nOther"
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

### Comparing `types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation/client.py` & `types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation/client.pyi` & `types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation/literals.py` & `types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation/literals.pyi` & `types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation/paginator.py` & `types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation/paginator.pyi` & `types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation/type_defs.py` & `types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation/type_defs.pyi` & `types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation/waiter.py` & `types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation/waiter.pyi` & `types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation.egg-info/PKG-INFO` & `types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-groundstation
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.GroundStation 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.GroundStation 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-groundstation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-groundstation)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-groundstation?color=blue)](https://pypistats.org/packages/types-aiobotocore-groundstation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GroundStation 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
+[aiobotocore.GroundStation 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-groundstation-2.5.1/types_aiobotocore_groundstation.egg-info/SOURCES.txt` & `types-aiobotocore-groundstation-2.5.2/types_aiobotocore_groundstation.egg-info/SOURCES.txt`

 * *Files identical despite different names*


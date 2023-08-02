# Comparing `tmp/types-aiobotocore-glue-2.5.1.tar.gz` & `tmp/types-aiobotocore-glue-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-glue-2.5.1.tar", last modified: Wed Jun 28 01:43:33 2023, max compression
+gzip compressed data, was "types-aiobotocore-glue-2.5.2.tar", last modified: Sat Jul  8 01:43:41 2023, max compression
```

## Comparing `types-aiobotocore-glue-2.5.1.tar` & `types-aiobotocore-glue-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:33.046143 types-aiobotocore-glue-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:31:46.000000 types-aiobotocore-glue-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    42491 2023-06-28 01:43:33.042143 types-aiobotocore-glue-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    40938 2023-06-28 01:31:46.000000 types-aiobotocore-glue-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:33.046143 types-aiobotocore-glue-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-28 01:31:46.000000 types-aiobotocore-glue-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:33.042143 types-aiobotocore-glue-2.5.1/types_aiobotocore_glue/
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-28 01:31:46.000000 types-aiobotocore-glue-2.5.1/types_aiobotocore_glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-06-28 01:31:46.000000 types-aiobotocore-glue-2.5.1/types_aiobotocore_glue/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-28 01:31:46.000000 types-aiobotocore-glue-2.5.1/types_aiobotocore_glue/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   143750 2023-06-28 01:31:47.000000 types-aiobotocore-glue-2.5.1/types_aiobotocore_glue/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   143520 2023-06-28 01:31:47.000000 types-aiobotocore-glue-2.5.1/types_aiobotocore_glue/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20771 2023-06-28 01:31:49.000000 types-aiobotocore-glue-2.5.1/types_aiobotocore_glue/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-06-28 01:31:49.000000 types-aiobotocore-glue-2.5.1/types_aiobotocore_glue/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22272 2023-06-28 01:31:48.000000 types-aiobotocore-glue-2.5.1/types_aiobotocore_glue/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22251 2023-06-28 01:31:48.000000 types-aiobotocore-glue-2.5.1/types_aiobotocore_glue/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:31:46.000000 types-aiobotocore-glue-2.5.1/types_aiobotocore_glue/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   253451 2023-06-28 01:31:55.000000 types-aiobotocore-glue-2.5.1/types_aiobotocore_glue/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   253076 2023-06-28 01:31:52.000000 types-aiobotocore-glue-2.5.1/types_aiobotocore_glue/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:31:46.000000 types-aiobotocore-glue-2.5.1/types_aiobotocore_glue/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:33.042143 types-aiobotocore-glue-2.5.1/types_aiobotocore_glue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42491 2023-06-28 01:43:32.000000 types-aiobotocore-glue-2.5.1/types_aiobotocore_glue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-28 01:43:32.000000 types-aiobotocore-glue-2.5.1/types_aiobotocore_glue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:32.000000 types-aiobotocore-glue-2.5.1/types_aiobotocore_glue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:32.000000 types-aiobotocore-glue-2.5.1/types_aiobotocore_glue.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:32.000000 types-aiobotocore-glue-2.5.1/types_aiobotocore_glue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-28 01:43:32.000000 types-aiobotocore-glue-2.5.1/types_aiobotocore_glue.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:41.198199 types-aiobotocore-glue-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:31:31.000000 types-aiobotocore-glue-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42491 2023-07-08 01:43:41.194199 types-aiobotocore-glue-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    40938 2023-07-08 01:31:31.000000 types-aiobotocore-glue-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:41.198199 types-aiobotocore-glue-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-08 01:31:31.000000 types-aiobotocore-glue-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:41.186199 types-aiobotocore-glue-2.5.2/types_aiobotocore_glue/
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-08 01:31:31.000000 types-aiobotocore-glue-2.5.2/types_aiobotocore_glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-07-08 01:31:31.000000 types-aiobotocore-glue-2.5.2/types_aiobotocore_glue/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-08 01:31:31.000000 types-aiobotocore-glue-2.5.2/types_aiobotocore_glue/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   143750 2023-07-08 01:31:32.000000 types-aiobotocore-glue-2.5.2/types_aiobotocore_glue/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   143520 2023-07-08 01:31:32.000000 types-aiobotocore-glue-2.5.2/types_aiobotocore_glue/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20771 2023-07-08 01:31:33.000000 types-aiobotocore-glue-2.5.2/types_aiobotocore_glue/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-07-08 01:31:32.000000 types-aiobotocore-glue-2.5.2/types_aiobotocore_glue/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22272 2023-07-08 01:31:32.000000 types-aiobotocore-glue-2.5.2/types_aiobotocore_glue/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22251 2023-07-08 01:31:32.000000 types-aiobotocore-glue-2.5.2/types_aiobotocore_glue/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:31:31.000000 types-aiobotocore-glue-2.5.2/types_aiobotocore_glue/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   253451 2023-07-08 01:31:40.000000 types-aiobotocore-glue-2.5.2/types_aiobotocore_glue/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   253076 2023-07-08 01:31:36.000000 types-aiobotocore-glue-2.5.2/types_aiobotocore_glue/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:31:31.000000 types-aiobotocore-glue-2.5.2/types_aiobotocore_glue/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:41.194199 types-aiobotocore-glue-2.5.2/types_aiobotocore_glue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42491 2023-07-08 01:43:41.000000 types-aiobotocore-glue-2.5.2/types_aiobotocore_glue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-08 01:43:41.000000 types-aiobotocore-glue-2.5.2/types_aiobotocore_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:41.000000 types-aiobotocore-glue-2.5.2/types_aiobotocore_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:41.000000 types-aiobotocore-glue-2.5.2/types_aiobotocore_glue.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:41.000000 types-aiobotocore-glue-2.5.2/types_aiobotocore_glue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-08 01:43:41.000000 types-aiobotocore-glue-2.5.2/types_aiobotocore_glue.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-glue-2.5.1/LICENSE` & `types-aiobotocore-glue-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glue-2.5.1/PKG-INFO` & `types-aiobotocore-glue-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-glue
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.Glue 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.Glue 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-glue.svg?color=blue)](https://pypi.org/project/types-aiobotocore-glue)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-glue?color=blue)](https://pypistats.org/packages/types-aiobotocore-glue)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Glue 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
+[aiobotocore.Glue 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-glue-2.5.1/README.md` & `types-aiobotocore-glue-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-glue.svg?color=blue)](https://pypi.org/project/types-aiobotocore-glue)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-glue?color=blue)](https://pypistats.org/packages/types-aiobotocore-glue)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Glue 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
+[aiobotocore.Glue 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-glue-2.5.1/setup.py` & `types-aiobotocore-glue-2.5.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-glue",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_glue"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Glue 2.5.1 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Glue 2.5.2 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-glue-2.5.1/types_aiobotocore_glue/__init__.py` & `types-aiobotocore-glue-2.5.2/types_aiobotocore_glue/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glue-2.5.1/types_aiobotocore_glue/__init__.pyi` & `types-aiobotocore-glue-2.5.2/types_aiobotocore_glue/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glue-2.5.1/types_aiobotocore_glue/__main__.py` & `types-aiobotocore-glue-2.5.2/types_aiobotocore_glue/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Glue 2.5.1\nVersion:         2.5.1\nBuilder version:"
+        "Type annotations for aiobotocore.Glue 2.5.2\nVersion:         2.5.2\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue\nOther"
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

### Comparing `types-aiobotocore-glue-2.5.1/types_aiobotocore_glue/client.py` & `types-aiobotocore-glue-2.5.2/types_aiobotocore_glue/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glue-2.5.1/types_aiobotocore_glue/client.pyi` & `types-aiobotocore-glue-2.5.2/types_aiobotocore_glue/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glue-2.5.1/types_aiobotocore_glue/literals.py` & `types-aiobotocore-glue-2.5.2/types_aiobotocore_glue/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glue-2.5.1/types_aiobotocore_glue/literals.pyi` & `types-aiobotocore-glue-2.5.2/types_aiobotocore_glue/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glue-2.5.1/types_aiobotocore_glue/paginator.py` & `types-aiobotocore-glue-2.5.2/types_aiobotocore_glue/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glue-2.5.1/types_aiobotocore_glue/paginator.pyi` & `types-aiobotocore-glue-2.5.2/types_aiobotocore_glue/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glue-2.5.1/types_aiobotocore_glue/type_defs.py` & `types-aiobotocore-glue-2.5.2/types_aiobotocore_glue/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glue-2.5.1/types_aiobotocore_glue/type_defs.pyi` & `types-aiobotocore-glue-2.5.2/types_aiobotocore_glue/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glue-2.5.1/types_aiobotocore_glue.egg-info/PKG-INFO` & `types-aiobotocore-glue-2.5.2/types_aiobotocore_glue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-glue
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.Glue 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.Glue 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-glue.svg?color=blue)](https://pypi.org/project/types-aiobotocore-glue)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-glue?color=blue)](https://pypistats.org/packages/types-aiobotocore-glue)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Glue 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
+[aiobotocore.Glue 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-glue-2.5.1/types_aiobotocore_glue.egg-info/SOURCES.txt` & `types-aiobotocore-glue-2.5.2/types_aiobotocore_glue.egg-info/SOURCES.txt`

 * *Files identical despite different names*


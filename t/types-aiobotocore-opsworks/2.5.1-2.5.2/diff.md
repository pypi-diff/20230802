# Comparing `tmp/types-aiobotocore-opsworks-2.5.1.tar.gz` & `tmp/types-aiobotocore-opsworks-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-opsworks-2.5.1.tar", last modified: Wed Jun 28 01:43:56 2023, max compression
+gzip compressed data, was "types-aiobotocore-opsworks-2.5.2.tar", last modified: Sat Jul  8 01:44:04 2023, max compression
```

## Comparing `types-aiobotocore-opsworks-2.5.1.tar` & `types-aiobotocore-opsworks-2.5.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:56.194187 types-aiobotocore-opsworks-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:36:12.000000 types-aiobotocore-opsworks-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23594 2023-06-28 01:43:56.194187 types-aiobotocore-opsworks-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22025 2023-06-28 01:36:12.000000 types-aiobotocore-opsworks-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:56.194187 types-aiobotocore-opsworks-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-28 01:36:12.000000 types-aiobotocore-opsworks-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:56.194187 types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-28 01:36:12.000000 types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-28 01:36:12.000000 types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-28 01:36:12.000000 types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54754 2023-06-28 01:36:14.000000 types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    54664 2023-06-28 01:36:12.000000 types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12440 2023-06-28 01:36:14.000000 types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12438 2023-06-28 01:36:14.000000 types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-28 01:36:14.000000 types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-28 01:36:14.000000 types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:36:12.000000 types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21853 2023-06-28 01:36:14.000000 types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    21815 2023-06-28 01:36:14.000000 types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    64317 2023-06-28 01:36:16.000000 types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    64250 2023-06-28 01:36:15.000000 types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:36:12.000000 types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-06-28 01:36:14.000000 types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-06-28 01:36:14.000000 types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:56.194187 types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23594 2023-06-28 01:43:56.000000 types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-28 01:43:56.000000 types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:56.000000 types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:56.000000 types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:56.000000 types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-28 01:43:56.000000 types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:04.514636 types-aiobotocore-opsworks-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:36:05.000000 types-aiobotocore-opsworks-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23594 2023-07-08 01:44:04.514636 types-aiobotocore-opsworks-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22025 2023-07-08 01:36:05.000000 types-aiobotocore-opsworks-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:04.514636 types-aiobotocore-opsworks-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-08 01:36:05.000000 types-aiobotocore-opsworks-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:04.502635 types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-08 01:36:05.000000 types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-08 01:36:05.000000 types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-08 01:36:05.000000 types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54754 2023-07-08 01:36:06.000000 types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54664 2023-07-08 01:36:05.000000 types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12440 2023-07-08 01:36:06.000000 types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12438 2023-07-08 01:36:06.000000 types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-08 01:36:06.000000 types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-08 01:36:06.000000 types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:36:05.000000 types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21853 2023-07-08 01:36:06.000000 types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21815 2023-07-08 01:36:06.000000 types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    64317 2023-07-08 01:36:07.000000 types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64250 2023-07-08 01:36:07.000000 types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:36:05.000000 types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-07-08 01:36:06.000000 types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-08 01:36:06.000000 types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:04.514636 types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23594 2023-07-08 01:44:04.000000 types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-08 01:44:04.000000 types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:04.000000 types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:04.000000 types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:04.000000 types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-08 01:44:04.000000 types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-opsworks-2.5.1/LICENSE` & `types-aiobotocore-opsworks-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworks-2.5.1/PKG-INFO` & `types-aiobotocore-opsworks-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-opsworks
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.OpsWorks 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.OpsWorks 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-opsworks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opsworks)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-opsworks?color=blue)](https://pypistats.org/packages/types-aiobotocore-opsworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.OpsWorks 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
+[aiobotocore.OpsWorks 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-opsworks-2.5.1/README.md` & `types-aiobotocore-opsworks-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-opsworks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opsworks)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-opsworks?color=blue)](https://pypistats.org/packages/types-aiobotocore-opsworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.OpsWorks 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
+[aiobotocore.OpsWorks 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-opsworks-2.5.1/setup.py` & `types-aiobotocore-opsworks-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-opsworks",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_opsworks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.OpsWorks 2.5.1 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.OpsWorks 2.5.2 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/__init__.py` & `types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/__init__.pyi` & `types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/__main__.py` & `types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.OpsWorks 2.5.1\nVersion:         2.5.1\nBuilder version:"
+        "Type annotations for aiobotocore.OpsWorks 2.5.2\nVersion:         2.5.2\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks\nOther"
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

### Comparing `types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/client.py` & `types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/client.pyi` & `types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/literals.py` & `types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/literals.pyi` & `types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/paginator.py` & `types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/paginator.pyi` & `types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/service_resource.py` & `types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/service_resource.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/service_resource.pyi` & `types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/type_defs.py` & `types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/type_defs.pyi` & `types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/waiter.py` & `types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks/waiter.pyi` & `types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks.egg-info/PKG-INFO` & `types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-opsworks
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.OpsWorks 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.OpsWorks 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-opsworks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opsworks)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-opsworks?color=blue)](https://pypistats.org/packages/types-aiobotocore-opsworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.OpsWorks 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
+[aiobotocore.OpsWorks 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-opsworks-2.5.1/types_aiobotocore_opsworks.egg-info/SOURCES.txt` & `types-aiobotocore-opsworks-2.5.2/types_aiobotocore_opsworks.egg-info/SOURCES.txt`

 * *Files identical despite different names*


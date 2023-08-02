# Comparing `tmp/types-aiobotocore-emr-containers-2.5.1.tar.gz` & `tmp/types-aiobotocore-emr-containers-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-emr-containers-2.5.1.tar", last modified: Wed Jun 28 01:43:29 2023, max compression
+gzip compressed data, was "types-aiobotocore-emr-containers-2.5.2.tar", last modified: Sat Jul  8 01:43:37 2023, max compression
```

## Comparing `types-aiobotocore-emr-containers-2.5.1.tar` & `types-aiobotocore-emr-containers-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:29.150136 types-aiobotocore-emr-containers-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:30:55.000000 types-aiobotocore-emr-containers-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16733 2023-06-28 01:43:29.150136 types-aiobotocore-emr-containers-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15141 2023-06-28 01:30:55.000000 types-aiobotocore-emr-containers-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:29.150136 types-aiobotocore-emr-containers-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-28 01:30:55.000000 types-aiobotocore-emr-containers-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:29.130136 types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers/
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-28 01:30:55.000000 types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-28 01:30:55.000000 types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-28 01:30:55.000000 types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19976 2023-06-28 01:30:56.000000 types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19943 2023-06-28 01:30:56.000000 types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-06-28 01:30:56.000000 types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-06-28 01:30:56.000000 types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-06-28 01:30:56.000000 types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-06-28 01:30:56.000000 types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:30:55.000000 types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    26001 2023-06-28 01:30:56.000000 types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25970 2023-06-28 01:30:56.000000 types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:30:55.000000 types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:29.150136 types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16733 2023-06-28 01:43:28.000000 types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-28 01:43:28.000000 types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:28.000000 types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:28.000000 types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:28.000000 types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-28 01:43:28.000000 types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:37.370127 types-aiobotocore-emr-containers-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:30:38.000000 types-aiobotocore-emr-containers-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16733 2023-07-08 01:43:37.370127 types-aiobotocore-emr-containers-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15141 2023-07-08 01:30:38.000000 types-aiobotocore-emr-containers-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:37.370127 types-aiobotocore-emr-containers-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-08 01:30:38.000000 types-aiobotocore-emr-containers-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:37.370127 types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-08 01:30:38.000000 types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-08 01:30:38.000000 types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-08 01:30:38.000000 types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19976 2023-07-08 01:30:38.000000 types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19943 2023-07-08 01:30:38.000000 types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-07-08 01:30:39.000000 types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-07-08 01:30:38.000000 types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-07-08 01:30:38.000000 types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-07-08 01:30:38.000000 types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:30:38.000000 types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26001 2023-07-08 01:30:39.000000 types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25970 2023-07-08 01:30:39.000000 types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:30:38.000000 types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:37.370127 types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16733 2023-07-08 01:43:37.000000 types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-08 01:43:37.000000 types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:37.000000 types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:37.000000 types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:37.000000 types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-08 01:43:37.000000 types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-emr-containers-2.5.1/LICENSE` & `types-aiobotocore-emr-containers-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-containers-2.5.1/PKG-INFO` & `types-aiobotocore-emr-containers-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-emr-containers
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.EMRContainers 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.EMRContainers 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-emr-containers.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr-containers)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-emr-containers?color=blue)](https://pypistats.org/packages/types-aiobotocore-emr-containers)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EMRContainers 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
+[aiobotocore.EMRContainers 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-emr-containers-2.5.1/README.md` & `types-aiobotocore-emr-containers-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-emr-containers.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr-containers)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-emr-containers?color=blue)](https://pypistats.org/packages/types-aiobotocore-emr-containers)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EMRContainers 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
+[aiobotocore.EMRContainers 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-emr-containers-2.5.1/setup.py` & `types-aiobotocore-emr-containers-2.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-emr-containers",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_emr_containers"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.EMRContainers 2.5.1 service generated with"
+        "Type annotations for aiobotocore.EMRContainers 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers/__init__.py` & `types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers/__init__.pyi` & `types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers/__main__.py` & `types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EMRContainers 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.EMRContainers 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers\nOther"
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

### Comparing `types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers/client.py` & `types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers/client.pyi` & `types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers/literals.py` & `types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers/literals.pyi` & `types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers/paginator.py` & `types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers/paginator.pyi` & `types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers/type_defs.py` & `types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers/type_defs.pyi` & `types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers.egg-info/PKG-INFO` & `types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-emr-containers
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.EMRContainers 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.EMRContainers 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-emr-containers.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr-containers)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-emr-containers?color=blue)](https://pypistats.org/packages/types-aiobotocore-emr-containers)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EMRContainers 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
+[aiobotocore.EMRContainers 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-emr-containers-2.5.1/types_aiobotocore_emr_containers.egg-info/SOURCES.txt` & `types-aiobotocore-emr-containers-2.5.2/types_aiobotocore_emr_containers.egg-info/SOURCES.txt`

 * *Files identical despite different names*


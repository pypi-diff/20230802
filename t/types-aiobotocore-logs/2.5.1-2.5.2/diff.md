# Comparing `tmp/types-aiobotocore-logs-2.5.1.tar.gz` & `tmp/types-aiobotocore-logs-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-logs-2.5.1.tar", last modified: Wed Jun 28 01:43:47 2023, max compression
+gzip compressed data, was "types-aiobotocore-logs-2.5.2.tar", last modified: Sat Jul  8 01:43:55 2023, max compression
```

## Comparing `types-aiobotocore-logs-2.5.1.tar` & `types-aiobotocore-logs-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:47.198170 types-aiobotocore-logs-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:34:29.000000 types-aiobotocore-logs-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19255 2023-06-28 01:43:47.198170 types-aiobotocore-logs-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17692 2023-06-28 01:34:29.000000 types-aiobotocore-logs-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:47.198170 types-aiobotocore-logs-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-28 01:34:28.000000 types-aiobotocore-logs-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:47.190170 types-aiobotocore-logs-2.5.1/types_aiobotocore_logs/
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-06-28 01:34:29.000000 types-aiobotocore-logs-2.5.1/types_aiobotocore_logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-28 01:34:29.000000 types-aiobotocore-logs-2.5.1/types_aiobotocore_logs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-28 01:34:29.000000 types-aiobotocore-logs-2.5.1/types_aiobotocore_logs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40488 2023-06-28 01:34:29.000000 types-aiobotocore-logs-2.5.1/types_aiobotocore_logs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40419 2023-06-28 01:34:29.000000 types-aiobotocore-logs-2.5.1/types_aiobotocore_logs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10697 2023-06-28 01:34:29.000000 types-aiobotocore-logs-2.5.1/types_aiobotocore_logs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-06-28 01:34:29.000000 types-aiobotocore-logs-2.5.1/types_aiobotocore_logs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12357 2023-06-28 01:34:29.000000 types-aiobotocore-logs-2.5.1/types_aiobotocore_logs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-06-28 01:34:29.000000 types-aiobotocore-logs-2.5.1/types_aiobotocore_logs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:34:29.000000 types-aiobotocore-logs-2.5.1/types_aiobotocore_logs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    36739 2023-06-28 01:34:30.000000 types-aiobotocore-logs-2.5.1/types_aiobotocore_logs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    36708 2023-06-28 01:34:29.000000 types-aiobotocore-logs-2.5.1/types_aiobotocore_logs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:34:29.000000 types-aiobotocore-logs-2.5.1/types_aiobotocore_logs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:47.198170 types-aiobotocore-logs-2.5.1/types_aiobotocore_logs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19255 2023-06-28 01:43:47.000000 types-aiobotocore-logs-2.5.1/types_aiobotocore_logs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-28 01:43:47.000000 types-aiobotocore-logs-2.5.1/types_aiobotocore_logs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:47.000000 types-aiobotocore-logs-2.5.1/types_aiobotocore_logs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:47.000000 types-aiobotocore-logs-2.5.1/types_aiobotocore_logs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:47.000000 types-aiobotocore-logs-2.5.1/types_aiobotocore_logs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-28 01:43:47.000000 types-aiobotocore-logs-2.5.1/types_aiobotocore_logs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:55.454467 types-aiobotocore-logs-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:34:18.000000 types-aiobotocore-logs-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19255 2023-07-08 01:43:55.454467 types-aiobotocore-logs-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17692 2023-07-08 01:34:18.000000 types-aiobotocore-logs-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:55.454467 types-aiobotocore-logs-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-08 01:34:18.000000 types-aiobotocore-logs-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:55.442467 types-aiobotocore-logs-2.5.2/types_aiobotocore_logs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-07-08 01:34:18.000000 types-aiobotocore-logs-2.5.2/types_aiobotocore_logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-08 01:34:18.000000 types-aiobotocore-logs-2.5.2/types_aiobotocore_logs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-08 01:34:18.000000 types-aiobotocore-logs-2.5.2/types_aiobotocore_logs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40488 2023-07-08 01:34:18.000000 types-aiobotocore-logs-2.5.2/types_aiobotocore_logs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40419 2023-07-08 01:34:18.000000 types-aiobotocore-logs-2.5.2/types_aiobotocore_logs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10697 2023-07-08 01:34:19.000000 types-aiobotocore-logs-2.5.2/types_aiobotocore_logs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-07-08 01:34:18.000000 types-aiobotocore-logs-2.5.2/types_aiobotocore_logs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12357 2023-07-08 01:34:18.000000 types-aiobotocore-logs-2.5.2/types_aiobotocore_logs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-07-08 01:34:18.000000 types-aiobotocore-logs-2.5.2/types_aiobotocore_logs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:34:18.000000 types-aiobotocore-logs-2.5.2/types_aiobotocore_logs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    36739 2023-07-08 01:34:19.000000 types-aiobotocore-logs-2.5.2/types_aiobotocore_logs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36708 2023-07-08 01:34:19.000000 types-aiobotocore-logs-2.5.2/types_aiobotocore_logs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:34:18.000000 types-aiobotocore-logs-2.5.2/types_aiobotocore_logs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:55.454467 types-aiobotocore-logs-2.5.2/types_aiobotocore_logs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19255 2023-07-08 01:43:55.000000 types-aiobotocore-logs-2.5.2/types_aiobotocore_logs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-08 01:43:55.000000 types-aiobotocore-logs-2.5.2/types_aiobotocore_logs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:55.000000 types-aiobotocore-logs-2.5.2/types_aiobotocore_logs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:55.000000 types-aiobotocore-logs-2.5.2/types_aiobotocore_logs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:55.000000 types-aiobotocore-logs-2.5.2/types_aiobotocore_logs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-08 01:43:55.000000 types-aiobotocore-logs-2.5.2/types_aiobotocore_logs.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-logs-2.5.1/LICENSE` & `types-aiobotocore-logs-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-logs-2.5.1/PKG-INFO` & `types-aiobotocore-logs-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-logs
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.CloudWatchLogs 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.CloudWatchLogs 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-logs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-logs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-logs?color=blue)](https://pypistats.org/packages/types-aiobotocore-logs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchLogs 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
+[aiobotocore.CloudWatchLogs 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-logs-2.5.1/README.md` & `types-aiobotocore-logs-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-logs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-logs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-logs?color=blue)](https://pypistats.org/packages/types-aiobotocore-logs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchLogs 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
+[aiobotocore.CloudWatchLogs 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-logs-2.5.1/setup.py` & `types-aiobotocore-logs-2.5.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-logs",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_logs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudWatchLogs 2.5.1 service generated with"
+        "Type annotations for aiobotocore.CloudWatchLogs 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-logs-2.5.1/types_aiobotocore_logs/__init__.py` & `types-aiobotocore-logs-2.5.2/types_aiobotocore_logs/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-logs-2.5.1/types_aiobotocore_logs/__init__.pyi` & `types-aiobotocore-logs-2.5.2/types_aiobotocore_logs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-logs-2.5.1/types_aiobotocore_logs/__main__.py` & `types-aiobotocore-logs-2.5.2/types_aiobotocore_logs/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudWatchLogs 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.CloudWatchLogs 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs\nOther"
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

### Comparing `types-aiobotocore-logs-2.5.1/types_aiobotocore_logs/client.py` & `types-aiobotocore-logs-2.5.2/types_aiobotocore_logs/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-logs-2.5.1/types_aiobotocore_logs/client.pyi` & `types-aiobotocore-logs-2.5.2/types_aiobotocore_logs/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-logs-2.5.1/types_aiobotocore_logs/literals.py` & `types-aiobotocore-logs-2.5.2/types_aiobotocore_logs/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-logs-2.5.1/types_aiobotocore_logs/literals.pyi` & `types-aiobotocore-logs-2.5.2/types_aiobotocore_logs/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-logs-2.5.1/types_aiobotocore_logs/paginator.py` & `types-aiobotocore-logs-2.5.2/types_aiobotocore_logs/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-logs-2.5.1/types_aiobotocore_logs/paginator.pyi` & `types-aiobotocore-logs-2.5.2/types_aiobotocore_logs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-logs-2.5.1/types_aiobotocore_logs/type_defs.py` & `types-aiobotocore-logs-2.5.2/types_aiobotocore_logs/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-logs-2.5.1/types_aiobotocore_logs/type_defs.pyi` & `types-aiobotocore-logs-2.5.2/types_aiobotocore_logs/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-logs-2.5.1/types_aiobotocore_logs.egg-info/PKG-INFO` & `types-aiobotocore-logs-2.5.2/types_aiobotocore_logs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-logs
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.CloudWatchLogs 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.CloudWatchLogs 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-logs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-logs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-logs?color=blue)](https://pypistats.org/packages/types-aiobotocore-logs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchLogs 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
+[aiobotocore.CloudWatchLogs 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-logs-2.5.1/types_aiobotocore_logs.egg-info/SOURCES.txt` & `types-aiobotocore-logs-2.5.2/types_aiobotocore_logs.egg-info/SOURCES.txt`

 * *Files identical despite different names*


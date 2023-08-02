# Comparing `tmp/types-aiobotocore-scheduler-2.5.1.tar.gz` & `tmp/types-aiobotocore-scheduler-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-scheduler-2.5.1.tar", last modified: Wed Jun 28 01:44:08 2023, max compression
+gzip compressed data, was "types-aiobotocore-scheduler-2.5.2.tar", last modified: Sat Jul  8 01:44:16 2023, max compression
```

## Comparing `types-aiobotocore-scheduler-2.5.1.tar` & `types-aiobotocore-scheduler-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:08.486210 types-aiobotocore-scheduler-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:40:21.000000 types-aiobotocore-scheduler-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14914 2023-06-28 01:44:08.478210 types-aiobotocore-scheduler-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-06-28 01:40:21.000000 types-aiobotocore-scheduler-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:44:08.486210 types-aiobotocore-scheduler-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-28 01:40:21.000000 types-aiobotocore-scheduler-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:08.478210 types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-28 01:40:21.000000 types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-28 01:40:21.000000 types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-28 01:40:21.000000 types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13131 2023-06-28 01:40:22.000000 types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-06-28 01:40:21.000000 types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-06-28 01:40:22.000000 types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9072 2023-06-28 01:40:22.000000 types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-06-28 01:40:22.000000 types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-06-28 01:40:22.000000 types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:40:21.000000 types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15566 2023-06-28 01:40:22.000000 types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15544 2023-06-28 01:40:22.000000 types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:40:21.000000 types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:08.478210 types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14914 2023-06-28 01:44:08.000000 types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-28 01:44:08.000000 types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:44:08.000000 types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:44:08.000000 types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:44:08.000000 types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-28 01:44:08.000000 types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:16.918861 types-aiobotocore-scheduler-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:40:27.000000 types-aiobotocore-scheduler-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14914 2023-07-08 01:44:16.914860 types-aiobotocore-scheduler-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-07-08 01:40:27.000000 types-aiobotocore-scheduler-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:16.918861 types-aiobotocore-scheduler-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-08 01:40:27.000000 types-aiobotocore-scheduler-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:16.910860 types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-08 01:40:27.000000 types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-08 01:40:27.000000 types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-08 01:40:27.000000 types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13131 2023-07-08 01:40:27.000000 types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-07-08 01:40:27.000000 types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-07-08 01:40:27.000000 types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9072 2023-07-08 01:40:27.000000 types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-08 01:40:27.000000 types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-07-08 01:40:27.000000 types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:40:27.000000 types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15566 2023-07-08 01:40:27.000000 types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15544 2023-07-08 01:40:27.000000 types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:40:27.000000 types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:16.914860 types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14914 2023-07-08 01:44:16.000000 types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-08 01:44:16.000000 types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:16.000000 types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:16.000000 types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:16.000000 types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-08 01:44:16.000000 types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-scheduler-2.5.1/LICENSE` & `types-aiobotocore-scheduler-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-scheduler-2.5.1/PKG-INFO` & `types-aiobotocore-scheduler-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-scheduler
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.EventBridgeScheduler 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.EventBridgeScheduler 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-scheduler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-scheduler)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-scheduler?color=blue)](https://pypistats.org/packages/types-aiobotocore-scheduler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EventBridgeScheduler 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
+[aiobotocore.EventBridgeScheduler 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-scheduler-2.5.1/README.md` & `types-aiobotocore-scheduler-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-scheduler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-scheduler)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-scheduler?color=blue)](https://pypistats.org/packages/types-aiobotocore-scheduler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EventBridgeScheduler 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
+[aiobotocore.EventBridgeScheduler 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-scheduler-2.5.1/setup.py` & `types-aiobotocore-scheduler-2.5.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-scheduler",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_scheduler"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.EventBridgeScheduler 2.5.1 service generated with"
+        "Type annotations for aiobotocore.EventBridgeScheduler 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler/__init__.py` & `types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler/__init__.pyi` & `types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler/__main__.py` & `types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EventBridgeScheduler 2.5.1\nVersion:        "
-        " 2.5.1\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.EventBridgeScheduler 2.5.2\nVersion:        "
+        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler\nOther"
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

### Comparing `types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler/client.py` & `types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler/client.pyi` & `types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler/literals.py` & `types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler/literals.pyi` & `types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler/paginator.py` & `types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler/paginator.pyi` & `types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler/type_defs.py` & `types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler/type_defs.pyi` & `types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler.egg-info/PKG-INFO` & `types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-scheduler
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.EventBridgeScheduler 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.EventBridgeScheduler 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-scheduler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-scheduler)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-scheduler?color=blue)](https://pypistats.org/packages/types-aiobotocore-scheduler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EventBridgeScheduler 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
+[aiobotocore.EventBridgeScheduler 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-scheduler-2.5.1/types_aiobotocore_scheduler.egg-info/SOURCES.txt` & `types-aiobotocore-scheduler-2.5.2/types_aiobotocore_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*


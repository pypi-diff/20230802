# Comparing `tmp/types-aiobotocore-medialive-2.5.1.tar.gz` & `tmp/types-aiobotocore-medialive-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-medialive-2.5.1.tar", last modified: Wed Jun 28 01:43:49 2023, max compression
+gzip compressed data, was "types-aiobotocore-medialive-2.5.2.tar", last modified: Sat Jul  8 01:43:58 2023, max compression
```

## Comparing `types-aiobotocore-medialive-2.5.1.tar` & `types-aiobotocore-medialive-2.5.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:49.722175 types-aiobotocore-medialive-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:35:07.000000 types-aiobotocore-medialive-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    37675 2023-06-28 01:43:49.722175 types-aiobotocore-medialive-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    36102 2023-06-28 01:35:07.000000 types-aiobotocore-medialive-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:49.722175 types-aiobotocore-medialive-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-28 01:35:07.000000 types-aiobotocore-medialive-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:49.722175 types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive/
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-06-28 01:35:07.000000 types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-28 01:35:07.000000 types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-28 01:35:07.000000 types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53844 2023-06-28 01:35:08.000000 types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    53755 2023-06-28 01:35:08.000000 types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    39348 2023-06-28 01:35:10.000000 types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    39346 2023-06-28 01:35:10.000000 types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-06-28 01:35:08.000000 types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-06-28 01:35:08.000000 types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:35:07.000000 types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   147116 2023-06-28 01:35:13.000000 types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   146967 2023-06-28 01:35:11.000000 types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:35:07.000000 types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-06-28 01:35:08.000000 types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11072 2023-06-28 01:35:08.000000 types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:49.722175 types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    37675 2023-06-28 01:43:49.000000 types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-28 01:43:49.000000 types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:49.000000 types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:49.000000 types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:49.000000 types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-28 01:43:49.000000 types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:58.042515 types-aiobotocore-medialive-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:34:58.000000 types-aiobotocore-medialive-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    37675 2023-07-08 01:43:58.038515 types-aiobotocore-medialive-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    36102 2023-07-08 01:34:58.000000 types-aiobotocore-medialive-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:58.042515 types-aiobotocore-medialive-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-08 01:34:58.000000 types-aiobotocore-medialive-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:58.038515 types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive/
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-07-08 01:34:58.000000 types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-07-08 01:34:58.000000 types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-08 01:34:58.000000 types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53844 2023-07-08 01:34:59.000000 types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53755 2023-07-08 01:34:59.000000 types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    39348 2023-07-08 01:35:00.000000 types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39346 2023-07-08 01:34:59.000000 types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-07-08 01:34:59.000000 types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-07-08 01:34:59.000000 types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:34:58.000000 types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   147116 2023-07-08 01:35:04.000000 types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146967 2023-07-08 01:35:03.000000 types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:34:58.000000 types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-07-08 01:34:59.000000 types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11072 2023-07-08 01:34:59.000000 types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:58.038515 types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    37675 2023-07-08 01:43:57.000000 types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-08 01:43:57.000000 types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:57.000000 types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:57.000000 types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:57.000000 types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-08 01:43:57.000000 types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-medialive-2.5.1/LICENSE` & `types-aiobotocore-medialive-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medialive-2.5.1/PKG-INFO` & `types-aiobotocore-medialive-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-medialive
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.MediaLive 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.MediaLive 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-medialive.svg?color=blue)](https://pypi.org/project/types-aiobotocore-medialive)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-medialive?color=blue)](https://pypistats.org/packages/types-aiobotocore-medialive)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaLive 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
+[aiobotocore.MediaLive 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-medialive-2.5.1/README.md` & `types-aiobotocore-medialive-2.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-medialive.svg?color=blue)](https://pypi.org/project/types-aiobotocore-medialive)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-medialive?color=blue)](https://pypistats.org/packages/types-aiobotocore-medialive)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaLive 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
+[aiobotocore.MediaLive 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-medialive-2.5.1/setup.py` & `types-aiobotocore-medialive-2.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-medialive",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_medialive"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MediaLive 2.5.1 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.MediaLive 2.5.2 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive/__init__.py` & `types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive/__init__.pyi` & `types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive/__main__.py` & `types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MediaLive 2.5.1\nVersion:         2.5.1\nBuilder version:"
+        "Type annotations for aiobotocore.MediaLive 2.5.2\nVersion:         2.5.2\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive\nOther"
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

### Comparing `types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive/client.py` & `types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive/client.pyi` & `types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive/literals.py` & `types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive/literals.pyi` & `types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive/paginator.py` & `types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive/paginator.pyi` & `types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive/type_defs.py` & `types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive/type_defs.pyi` & `types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive/waiter.py` & `types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive/waiter.pyi` & `types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive.egg-info/PKG-INFO` & `types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-medialive
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.MediaLive 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.MediaLive 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-medialive.svg?color=blue)](https://pypi.org/project/types-aiobotocore-medialive)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-medialive?color=blue)](https://pypistats.org/packages/types-aiobotocore-medialive)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaLive 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
+[aiobotocore.MediaLive 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-medialive-2.5.1/types_aiobotocore_medialive.egg-info/SOURCES.txt` & `types-aiobotocore-medialive-2.5.2/types_aiobotocore_medialive.egg-info/SOURCES.txt`

 * *Files identical despite different names*


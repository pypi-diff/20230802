# Comparing `tmp/types-aiobotocore-workmail-2.5.1.tar.gz` & `tmp/types-aiobotocore-workmail-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-workmail-2.5.1.tar", last modified: Wed Jun 28 01:44:20 2023, max compression
+gzip compressed data, was "types-aiobotocore-workmail-2.5.2.tar", last modified: Sat Jul  8 01:44:28 2023, max compression
```

## Comparing `types-aiobotocore-workmail-2.5.1.tar` & `types-aiobotocore-workmail-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:20.470232 types-aiobotocore-workmail-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:42:35.000000 types-aiobotocore-workmail-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21562 2023-06-28 01:44:20.470232 types-aiobotocore-workmail-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19993 2023-06-28 01:42:35.000000 types-aiobotocore-workmail-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:44:20.470232 types-aiobotocore-workmail-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-28 01:42:34.000000 types-aiobotocore-workmail-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:20.466232 types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail/
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-28 01:42:35.000000 types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-28 01:42:35.000000 types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-28 01:42:35.000000 types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60366 2023-06-28 01:42:35.000000 types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    60268 2023-06-28 01:42:35.000000 types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-06-28 01:42:35.000000 types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10082 2023-06-28 01:42:35.000000 types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11150 2023-06-28 01:42:35.000000 types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11139 2023-06-28 01:42:35.000000 types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:42:35.000000 types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    59811 2023-06-28 01:42:39.000000 types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    59732 2023-06-28 01:42:38.000000 types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:42:35.000000 types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:20.470232 types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21562 2023-06-28 01:44:20.000000 types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-28 01:44:20.000000 types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:44:20.000000 types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:44:20.000000 types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:44:20.000000 types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-28 01:44:20.000000 types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:28.895059 types-aiobotocore-workmail-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:42:42.000000 types-aiobotocore-workmail-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21562 2023-07-08 01:44:28.895059 types-aiobotocore-workmail-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19993 2023-07-08 01:42:42.000000 types-aiobotocore-workmail-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:28.895059 types-aiobotocore-workmail-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-08 01:42:41.000000 types-aiobotocore-workmail-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:28.895059 types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail/
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-08 01:42:42.000000 types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-08 01:42:42.000000 types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-08 01:42:42.000000 types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60366 2023-07-08 01:42:42.000000 types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60268 2023-07-08 01:42:42.000000 types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-07-08 01:42:42.000000 types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10082 2023-07-08 01:42:42.000000 types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11150 2023-07-08 01:42:42.000000 types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11139 2023-07-08 01:42:42.000000 types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:42.000000 types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    59811 2023-07-08 01:42:46.000000 types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59732 2023-07-08 01:42:43.000000 types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:42:42.000000 types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:28.895059 types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21562 2023-07-08 01:44:28.000000 types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-08 01:44:28.000000 types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:28.000000 types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:28.000000 types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:28.000000 types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-08 01:44:28.000000 types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-workmail-2.5.1/LICENSE` & `types-aiobotocore-workmail-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workmail-2.5.1/PKG-INFO` & `types-aiobotocore-workmail-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-workmail
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.WorkMail 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.WorkMail 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-workmail.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workmail)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-workmail?color=blue)](https://pypistats.org/packages/types-aiobotocore-workmail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WorkMail 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
+[aiobotocore.WorkMail 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-workmail-2.5.1/README.md` & `types-aiobotocore-workmail-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-workmail.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workmail)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-workmail?color=blue)](https://pypistats.org/packages/types-aiobotocore-workmail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WorkMail 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
+[aiobotocore.WorkMail 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-workmail-2.5.1/setup.py` & `types-aiobotocore-workmail-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-workmail",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_workmail"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.WorkMail 2.5.1 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.WorkMail 2.5.2 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail/__init__.py` & `types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail/__init__.pyi` & `types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail/__main__.py` & `types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.WorkMail 2.5.1\nVersion:         2.5.1\nBuilder version:"
+        "Type annotations for aiobotocore.WorkMail 2.5.2\nVersion:         2.5.2\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail\nOther"
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

### Comparing `types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail/client.py` & `types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail/client.pyi` & `types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail/literals.py` & `types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail/literals.pyi` & `types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail/paginator.py` & `types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail/paginator.pyi` & `types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail/type_defs.py` & `types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail/type_defs.pyi` & `types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail.egg-info/PKG-INFO` & `types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-workmail
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.WorkMail 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.WorkMail 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-workmail.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workmail)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-workmail?color=blue)](https://pypistats.org/packages/types-aiobotocore-workmail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WorkMail 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
+[aiobotocore.WorkMail 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-workmail-2.5.1/types_aiobotocore_workmail.egg-info/SOURCES.txt` & `types-aiobotocore-workmail-2.5.2/types_aiobotocore_workmail.egg-info/SOURCES.txt`

 * *Files identical despite different names*


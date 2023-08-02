# Comparing `tmp/mypy-boto3-budgets-1.28.16.tar.gz` & `tmp/mypy-boto3-budgets-1.28.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-budgets-1.28.16.tar", last modified: Tue Aug  1 11:36:18 2023, max compression
+gzip compressed data, was "mypy-boto3-budgets-1.28.18.tar", last modified: Wed Aug  2 19:47:54 2023, max compression
```

## Comparing `mypy-boto3-budgets-1.28.16.tar` & `mypy-boto3-budgets-1.28.18.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:18.728939 mypy-boto3-budgets-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:11:42.000000 mypy-boto3-budgets-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17986 2023-08-01 11:36:18.724939 mypy-boto3-budgets-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16502 2023-08-01 11:11:42.000000 mypy-boto3-budgets-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:18.720939 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-08-01 11:11:42.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-08-01 11:11:42.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-01 11:11:42.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22010 2023-08-01 11:11:43.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21972 2023-08-01 11:11:43.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-08-01 11:11:44.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-08-01 11:11:44.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-08-01 11:11:43.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10988 2023-08-01 11:11:43.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:11:42.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34538 2023-08-01 11:11:45.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34483 2023-08-01 11:11:44.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:11:42.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:18.724939 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17986 2023-08-01 11:36:18.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-01 11:36:18.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:18.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:18.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:18.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 11:36:18.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:18.728939 mypy-boto3-budgets-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-08-01 11:11:42.000000 mypy-boto3-budgets-1.28.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:47:54.568429 mypy-boto3-budgets-1.28.18/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 19:46:48.000000 mypy-boto3-budgets-1.28.18/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17986 2023-08-02 19:47:54.568429 mypy-boto3-budgets-1.28.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16502 2023-08-02 19:46:48.000000 mypy-boto3-budgets-1.28.18/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:47:54.548427 mypy-boto3-budgets-1.28.18/mypy_boto3_budgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-08-02 19:46:49.000000 mypy-boto3-budgets-1.28.18/mypy_boto3_budgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-08-02 19:46:48.000000 mypy-boto3-budgets-1.28.18/mypy_boto3_budgets/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-02 19:46:49.000000 mypy-boto3-budgets-1.28.18/mypy_boto3_budgets/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22010 2023-08-02 19:46:49.000000 mypy-boto3-budgets-1.28.18/mypy_boto3_budgets/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21972 2023-08-02 19:46:49.000000 mypy-boto3-budgets-1.28.18/mypy_boto3_budgets/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-08-02 19:46:49.000000 mypy-boto3-budgets-1.28.18/mypy_boto3_budgets/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-08-02 19:46:49.000000 mypy-boto3-budgets-1.28.18/mypy_boto3_budgets/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-08-02 19:46:49.000000 mypy-boto3-budgets-1.28.18/mypy_boto3_budgets/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10988 2023-08-02 19:46:49.000000 mypy-boto3-budgets-1.28.18/mypy_boto3_budgets/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:46:49.000000 mypy-boto3-budgets-1.28.18/mypy_boto3_budgets/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34538 2023-08-02 19:46:51.000000 mypy-boto3-budgets-1.28.18/mypy_boto3_budgets/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34483 2023-08-02 19:46:49.000000 mypy-boto3-budgets-1.28.18/mypy_boto3_budgets/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-02 19:46:48.000000 mypy-boto3-budgets-1.28.18/mypy_boto3_budgets/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:47:54.568429 mypy-boto3-budgets-1.28.18/mypy_boto3_budgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17986 2023-08-02 19:47:54.000000 mypy-boto3-budgets-1.28.18/mypy_boto3_budgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-02 19:47:54.000000 mypy-boto3-budgets-1.28.18/mypy_boto3_budgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:47:54.000000 mypy-boto3-budgets-1.28.18/mypy_boto3_budgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:47:54.000000 mypy-boto3-budgets-1.28.18/mypy_boto3_budgets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 19:47:54.000000 mypy-boto3-budgets-1.28.18/mypy_boto3_budgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-02 19:47:54.000000 mypy-boto3-budgets-1.28.18/mypy_boto3_budgets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 19:47:54.568429 mypy-boto3-budgets-1.28.18/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-08-02 19:46:48.000000 mypy-boto3-budgets-1.28.18/setup.py
```

### Comparing `mypy-boto3-budgets-1.28.16/LICENSE` & `mypy-boto3-budgets-1.28.18/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.16/PKG-INFO` & `mypy-boto3-budgets-1.28.18/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-budgets
-Version: 1.28.16
-Summary: Type annotations for boto3.Budgets 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.18
+Summary: Type annotations for boto3.Budgets 1.28.18 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-budgets.svg?color=blue)](https://pypi.org/project/mypy-boto3-budgets)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-budgets)](https://pepy.tech/project/mypy-boto3-budgets)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Budgets 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
+[boto3.Budgets 1.28.18](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-budgets-1.28.16/README.md` & `mypy-boto3-budgets-1.28.18/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-budgets.svg?color=blue)](https://pypi.org/project/mypy-boto3-budgets)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-budgets)](https://pepy.tech/project/mypy-boto3-budgets)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Budgets 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
+[boto3.Budgets 1.28.18](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/__init__.py` & `mypy-boto3-budgets-1.28.18/mypy_boto3_budgets/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/__init__.pyi` & `mypy-boto3-budgets-1.28.18/mypy_boto3_budgets/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/__main__.py` & `mypy-boto3-budgets-1.28.18/mypy_boto3_budgets/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Budgets 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        "Type annotations for boto3.Budgets 1.28.18\nVersion:         1.28.18\nBuilder version:"
         " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.16")
+    print("1.28.18")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/client.py` & `mypy-boto3-budgets-1.28.18/mypy_boto3_budgets/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/client.pyi` & `mypy-boto3-budgets-1.28.18/mypy_boto3_budgets/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/literals.py` & `mypy-boto3-budgets-1.28.18/mypy_boto3_budgets/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/literals.pyi` & `mypy-boto3-budgets-1.28.18/mypy_boto3_budgets/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/paginator.py` & `mypy-boto3-budgets-1.28.18/mypy_boto3_budgets/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/paginator.pyi` & `mypy-boto3-budgets-1.28.18/mypy_boto3_budgets/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/type_defs.py` & `mypy-boto3-budgets-1.28.18/mypy_boto3_budgets/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/type_defs.pyi` & `mypy-boto3-budgets-1.28.18/mypy_boto3_budgets/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.16/mypy_boto3_budgets.egg-info/PKG-INFO` & `mypy-boto3-budgets-1.28.18/mypy_boto3_budgets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-budgets
-Version: 1.28.16
-Summary: Type annotations for boto3.Budgets 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.18
+Summary: Type annotations for boto3.Budgets 1.28.18 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-budgets.svg?color=blue)](https://pypi.org/project/mypy-boto3-budgets)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-budgets)](https://pepy.tech/project/mypy-boto3-budgets)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Budgets 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
+[boto3.Budgets 1.28.18](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-budgets-1.28.16/mypy_boto3_budgets.egg-info/SOURCES.txt` & `mypy-boto3-budgets-1.28.18/mypy_boto3_budgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.16/setup.py` & `mypy-boto3-budgets-1.28.18/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-budgets",
-    version="1.28.16",
+    version="1.28.18",
     packages=["mypy_boto3_budgets"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Budgets 1.28.16 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.Budgets 1.28.18 service generated with mypy-boto3-builder"
         " 7.17.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```


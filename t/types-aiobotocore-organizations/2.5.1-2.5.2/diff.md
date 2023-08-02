# Comparing `tmp/types-aiobotocore-organizations-2.5.1.tar.gz` & `tmp/types-aiobotocore-organizations-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-organizations-2.5.1.tar", last modified: Wed Jun 28 01:43:56 2023, max compression
+gzip compressed data, was "types-aiobotocore-organizations-2.5.2.tar", last modified: Sat Jul  8 01:44:05 2023, max compression
```

## Comparing `types-aiobotocore-organizations-2.5.1.tar` & `types-aiobotocore-organizations-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:56.602187 types-aiobotocore-organizations-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:36:17.000000 types-aiobotocore-organizations-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22364 2023-06-28 01:43:56.602187 types-aiobotocore-organizations-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20775 2023-06-28 01:36:17.000000 types-aiobotocore-organizations-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:56.602187 types-aiobotocore-organizations-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-28 01:36:17.000000 types-aiobotocore-organizations-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:56.594187 types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations/
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-06-28 01:36:17.000000 types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-06-28 01:36:17.000000 types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-28 01:36:17.000000 types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49679 2023-06-28 01:36:18.000000 types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49599 2023-06-28 01:36:18.000000 types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-06-28 01:36:18.000000 types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12259 2023-06-28 01:36:18.000000 types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20535 2023-06-28 01:36:18.000000 types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    20517 2023-06-28 01:36:18.000000 types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:36:17.000000 types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    44414 2023-06-28 01:36:20.000000 types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    44359 2023-06-28 01:36:18.000000 types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:36:17.000000 types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:56.602187 types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22364 2023-06-28 01:43:56.000000 types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-28 01:43:56.000000 types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:56.000000 types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:56.000000 types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:56.000000 types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-28 01:43:56.000000 types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:05.002645 types-aiobotocore-organizations-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:36:11.000000 types-aiobotocore-organizations-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22364 2023-07-08 01:44:05.002645 types-aiobotocore-organizations-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20775 2023-07-08 01:36:11.000000 types-aiobotocore-organizations-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:05.002645 types-aiobotocore-organizations-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-08 01:36:11.000000 types-aiobotocore-organizations-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:04.994644 types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-07-08 01:36:11.000000 types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-07-08 01:36:11.000000 types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-08 01:36:11.000000 types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49679 2023-07-08 01:36:11.000000 types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49599 2023-07-08 01:36:11.000000 types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-07-08 01:36:11.000000 types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12259 2023-07-08 01:36:11.000000 types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20535 2023-07-08 01:36:11.000000 types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20517 2023-07-08 01:36:11.000000 types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:36:11.000000 types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    44414 2023-07-08 01:36:12.000000 types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44359 2023-07-08 01:36:12.000000 types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:36:11.000000 types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:05.002645 types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22364 2023-07-08 01:44:04.000000 types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-08 01:44:04.000000 types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:04.000000 types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:04.000000 types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:04.000000 types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-08 01:44:04.000000 types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-organizations-2.5.1/LICENSE` & `types-aiobotocore-organizations-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.5.1/PKG-INFO` & `types-aiobotocore-organizations-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-organizations
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.Organizations 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.Organizations 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-organizations.svg?color=blue)](https://pypi.org/project/types-aiobotocore-organizations)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-organizations?color=blue)](https://pypistats.org/packages/types-aiobotocore-organizations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Organizations 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations)
+[aiobotocore.Organizations 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-organizations-2.5.1/README.md` & `types-aiobotocore-organizations-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-organizations.svg?color=blue)](https://pypi.org/project/types-aiobotocore-organizations)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-organizations?color=blue)](https://pypistats.org/packages/types-aiobotocore-organizations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Organizations 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations)
+[aiobotocore.Organizations 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-organizations-2.5.1/setup.py` & `types-aiobotocore-organizations-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-organizations",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_organizations"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Organizations 2.5.1 service generated with"
+        "Type annotations for aiobotocore.Organizations 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations/__init__.py` & `types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations/__init__.pyi` & `types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations/__main__.py` & `types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Organizations 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.Organizations 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations\nOther"
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

### Comparing `types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations/client.py` & `types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations/client.pyi` & `types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations/literals.py` & `types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations/literals.pyi` & `types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations/paginator.py` & `types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations/paginator.pyi` & `types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations/type_defs.py` & `types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations/type_defs.pyi` & `types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations.egg-info/PKG-INFO` & `types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-organizations
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.Organizations 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.Organizations 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-organizations.svg?color=blue)](https://pypi.org/project/types-aiobotocore-organizations)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-organizations?color=blue)](https://pypistats.org/packages/types-aiobotocore-organizations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Organizations 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations)
+[aiobotocore.Organizations 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-organizations-2.5.1/types_aiobotocore_organizations.egg-info/SOURCES.txt` & `types-aiobotocore-organizations-2.5.2/types_aiobotocore_organizations.egg-info/SOURCES.txt`

 * *Files identical despite different names*


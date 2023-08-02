# Comparing `tmp/types-aiobotocore-customer-profiles-2.5.1.tar.gz` & `tmp/types-aiobotocore-customer-profiles-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-customer-profiles-2.5.1.tar", last modified: Wed Jun 28 01:43:20 2023, max compression
+gzip compressed data, was "types-aiobotocore-customer-profiles-2.5.2.tar", last modified: Sat Jul  8 01:43:28 2023, max compression
```

## Comparing `types-aiobotocore-customer-profiles-2.5.1.tar` & `types-aiobotocore-customer-profiles-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:20.414120 types-aiobotocore-customer-profiles-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:28:43.000000 types-aiobotocore-customer-profiles-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20088 2023-06-28 01:43:20.414120 types-aiobotocore-customer-profiles-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18484 2023-06-28 01:28:43.000000 types-aiobotocore-customer-profiles-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:20.414120 types-aiobotocore-customer-profiles-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-28 01:28:43.000000 types-aiobotocore-customer-profiles-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:20.410120 types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-28 01:28:43.000000 types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-28 01:28:43.000000 types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-28 01:28:43.000000 types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41040 2023-06-28 01:28:43.000000 types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40981 2023-06-28 01:28:43.000000 types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-06-28 01:28:44.000000 types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12677 2023-06-28 01:28:43.000000 types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-28 01:28:43.000000 types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-28 01:28:43.000000 types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:28:43.000000 types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    63039 2023-06-28 01:28:46.000000 types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    62951 2023-06-28 01:28:45.000000 types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:28:43.000000 types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:20.414120 types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20088 2023-06-28 01:43:20.000000 types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-28 01:43:20.000000 types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:20.000000 types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:20.000000 types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:20.000000 types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-28 01:43:20.000000 types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:28.597960 types-aiobotocore-customer-profiles-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:28:21.000000 types-aiobotocore-customer-profiles-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20088 2023-07-08 01:43:28.597960 types-aiobotocore-customer-profiles-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18484 2023-07-08 01:28:21.000000 types-aiobotocore-customer-profiles-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:28.597960 types-aiobotocore-customer-profiles-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-08 01:28:21.000000 types-aiobotocore-customer-profiles-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:28.581960 types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-08 01:28:21.000000 types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-08 01:28:21.000000 types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-08 01:28:21.000000 types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41040 2023-07-08 01:28:21.000000 types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40981 2023-07-08 01:28:21.000000 types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-07-08 01:28:22.000000 types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12677 2023-07-08 01:28:22.000000 types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-08 01:28:21.000000 types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-08 01:28:21.000000 types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:28:21.000000 types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    63039 2023-07-08 01:28:24.000000 types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62951 2023-07-08 01:28:22.000000 types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:28:21.000000 types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:28.597960 types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20088 2023-07-08 01:43:28.000000 types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-08 01:43:28.000000 types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:28.000000 types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:28.000000 types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:28.000000 types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-08 01:43:28.000000 types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-customer-profiles-2.5.1/LICENSE` & `types-aiobotocore-customer-profiles-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.1/PKG-INFO` & `types-aiobotocore-customer-profiles-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-customer-profiles
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.CustomerProfiles 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.CustomerProfiles 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-customer-profiles.svg?color=blue)](https://pypi.org/project/types-aiobotocore-customer-profiles)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-customer-profiles?color=blue)](https://pypistats.org/packages/types-aiobotocore-customer-profiles)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CustomerProfiles 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
+[aiobotocore.CustomerProfiles 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-customer-profiles-2.5.1/README.md` & `types-aiobotocore-customer-profiles-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-customer-profiles.svg?color=blue)](https://pypi.org/project/types-aiobotocore-customer-profiles)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-customer-profiles?color=blue)](https://pypistats.org/packages/types-aiobotocore-customer-profiles)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CustomerProfiles 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
+[aiobotocore.CustomerProfiles 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-customer-profiles-2.5.1/setup.py` & `types-aiobotocore-customer-profiles-2.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-customer-profiles",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_customer_profiles"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CustomerProfiles 2.5.1 service generated with"
+        "Type annotations for aiobotocore.CustomerProfiles 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles/__init__.py` & `types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles/__init__.pyi` & `types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles/__main__.py` & `types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CustomerProfiles 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.CustomerProfiles 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles\nOther"
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

### Comparing `types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles/client.py` & `types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles/client.pyi` & `types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles/literals.py` & `types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles/literals.pyi` & `types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles/paginator.py` & `types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles/paginator.pyi` & `types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles/type_defs.py` & `types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles/type_defs.pyi` & `types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles.egg-info/PKG-INFO` & `types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-customer-profiles
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.CustomerProfiles 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.CustomerProfiles 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-customer-profiles.svg?color=blue)](https://pypi.org/project/types-aiobotocore-customer-profiles)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-customer-profiles?color=blue)](https://pypistats.org/packages/types-aiobotocore-customer-profiles)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CustomerProfiles 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
+[aiobotocore.CustomerProfiles 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-customer-profiles-2.5.1/types_aiobotocore_customer_profiles.egg-info/SOURCES.txt` & `types-aiobotocore-customer-profiles-2.5.2/types_aiobotocore_customer_profiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-pinpoint-email-2.5.1.tar.gz` & `tmp/types-aiobotocore-pinpoint-email-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-pinpoint-email-2.5.1.tar", last modified: Wed Jun 28 01:43:58 2023, max compression
+gzip compressed data, was "types-aiobotocore-pinpoint-email-2.5.2.tar", last modified: Sat Jul  8 01:44:07 2023, max compression
```

## Comparing `types-aiobotocore-pinpoint-email-2.5.1.tar` & `types-aiobotocore-pinpoint-email-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:58.766191 types-aiobotocore-pinpoint-email-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:36:43.000000 types-aiobotocore-pinpoint-email-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18746 2023-06-28 01:43:58.758191 types-aiobotocore-pinpoint-email-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17154 2023-06-28 01:36:43.000000 types-aiobotocore-pinpoint-email-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:58.766191 types-aiobotocore-pinpoint-email-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-28 01:36:43.000000 types-aiobotocore-pinpoint-email-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:58.754191 types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email/
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-28 01:36:43.000000 types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-28 01:36:43.000000 types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-28 01:36:43.000000 types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35123 2023-06-28 01:36:44.000000 types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    35067 2023-06-28 01:36:44.000000 types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-06-28 01:36:44.000000 types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9863 2023-06-28 01:36:44.000000 types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-06-28 01:36:44.000000 types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-06-28 01:36:44.000000 types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:36:43.000000 types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    35008 2023-06-28 01:36:45.000000 types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34974 2023-06-28 01:36:44.000000 types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:36:43.000000 types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:58.758191 types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18746 2023-06-28 01:43:58.000000 types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-28 01:43:58.000000 types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:58.000000 types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:58.000000 types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:58.000000 types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-28 01:43:58.000000 types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:07.202685 types-aiobotocore-pinpoint-email-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:36:36.000000 types-aiobotocore-pinpoint-email-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18746 2023-07-08 01:44:07.198686 types-aiobotocore-pinpoint-email-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17154 2023-07-08 01:36:36.000000 types-aiobotocore-pinpoint-email-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:07.202685 types-aiobotocore-pinpoint-email-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-08 01:36:36.000000 types-aiobotocore-pinpoint-email-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:07.198686 types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email/
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-08 01:36:36.000000 types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-08 01:36:36.000000 types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-08 01:36:36.000000 types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35123 2023-07-08 01:36:36.000000 types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35067 2023-07-08 01:36:36.000000 types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-07-08 01:36:36.000000 types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9863 2023-07-08 01:36:36.000000 types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-07-08 01:36:36.000000 types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-07-08 01:36:36.000000 types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:36:36.000000 types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    35008 2023-07-08 01:36:39.000000 types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34974 2023-07-08 01:36:38.000000 types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:36:36.000000 types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:07.198686 types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18746 2023-07-08 01:44:07.000000 types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-08 01:44:07.000000 types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:07.000000 types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:07.000000 types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:07.000000 types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-08 01:44:07.000000 types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-pinpoint-email-2.5.1/LICENSE` & `types-aiobotocore-pinpoint-email-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-email-2.5.1/PKG-INFO` & `types-aiobotocore-pinpoint-email-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-pinpoint-email
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.PinpointEmail 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.PinpointEmail 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pinpoint-email.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pinpoint-email)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-pinpoint-email?color=blue)](https://pypistats.org/packages/types-aiobotocore-pinpoint-email)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PinpointEmail 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
+[aiobotocore.PinpointEmail 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-pinpoint-email-2.5.1/README.md` & `types-aiobotocore-pinpoint-email-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pinpoint-email.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pinpoint-email)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-pinpoint-email?color=blue)](https://pypistats.org/packages/types-aiobotocore-pinpoint-email)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PinpointEmail 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
+[aiobotocore.PinpointEmail 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-pinpoint-email-2.5.1/setup.py` & `types-aiobotocore-pinpoint-email-2.5.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-pinpoint-email",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_pinpoint_email"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.PinpointEmail 2.5.1 service generated with"
+        "Type annotations for aiobotocore.PinpointEmail 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email/__init__.py` & `types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email/__init__.pyi` & `types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email/__main__.py` & `types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.PinpointEmail 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.PinpointEmail 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail\nOther"
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

### Comparing `types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email/client.py` & `types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email/client.pyi` & `types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email/literals.py` & `types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email/literals.pyi` & `types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email/paginator.py` & `types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email/paginator.pyi` & `types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email/type_defs.py` & `types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email/type_defs.pyi` & `types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email.egg-info/PKG-INFO` & `types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-pinpoint-email
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.PinpointEmail 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.PinpointEmail 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pinpoint-email.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pinpoint-email)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-pinpoint-email?color=blue)](https://pypistats.org/packages/types-aiobotocore-pinpoint-email)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PinpointEmail 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
+[aiobotocore.PinpointEmail 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-pinpoint-email-2.5.1/types_aiobotocore_pinpoint_email.egg-info/SOURCES.txt` & `types-aiobotocore-pinpoint-email-2.5.2/types_aiobotocore_pinpoint_email.egg-info/SOURCES.txt`

 * *Files identical despite different names*


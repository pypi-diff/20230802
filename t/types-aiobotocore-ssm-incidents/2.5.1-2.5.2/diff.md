# Comparing `tmp/types-aiobotocore-ssm-incidents-2.5.1.tar.gz` & `tmp/types-aiobotocore-ssm-incidents-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ssm-incidents-2.5.1.tar", last modified: Wed Jun 28 01:44:13 2023, max compression
+gzip compressed data, was "types-aiobotocore-ssm-incidents-2.5.2.tar", last modified: Sat Jul  8 01:44:22 2023, max compression
```

## Comparing `types-aiobotocore-ssm-incidents-2.5.1.tar` & `types-aiobotocore-ssm-incidents-2.5.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:13.926220 types-aiobotocore-ssm-incidents-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:41:27.000000 types-aiobotocore-ssm-incidents-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18801 2023-06-28 01:44:13.922220 types-aiobotocore-ssm-incidents-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17213 2023-06-28 01:41:27.000000 types-aiobotocore-ssm-incidents-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:44:13.926220 types-aiobotocore-ssm-incidents-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-28 01:41:27.000000 types-aiobotocore-ssm-incidents-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:13.918220 types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-28 01:41:27.000000 types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-28 01:41:27.000000 types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-28 01:41:27.000000 types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27564 2023-06-28 01:41:30.000000 types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27518 2023-06-28 01:41:27.000000 types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-06-28 01:41:30.000000 types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-06-28 01:41:30.000000 types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-06-28 01:41:30.000000 types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-06-28 01:41:30.000000 types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:41:27.000000 types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33955 2023-06-28 01:41:31.000000 types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    33891 2023-06-28 01:41:30.000000 types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:41:27.000000 types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-06-28 01:41:30.000000 types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-28 01:41:30.000000 types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:13.922220 types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18801 2023-06-28 01:44:13.000000 types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-28 01:44:13.000000 types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:44:13.000000 types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:44:13.000000 types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:44:13.000000 types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-28 01:44:13.000000 types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:22.302939 types-aiobotocore-ssm-incidents-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:41:33.000000 types-aiobotocore-ssm-incidents-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18801 2023-07-08 01:44:22.294939 types-aiobotocore-ssm-incidents-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17213 2023-07-08 01:41:33.000000 types-aiobotocore-ssm-incidents-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:22.302939 types-aiobotocore-ssm-incidents-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-08 01:41:33.000000 types-aiobotocore-ssm-incidents-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:22.294939 types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-08 01:41:33.000000 types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-08 01:41:33.000000 types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-08 01:41:33.000000 types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27564 2023-07-08 01:41:33.000000 types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27518 2023-07-08 01:41:33.000000 types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-07-08 01:41:34.000000 types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-07-08 01:41:34.000000 types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-07-08 01:41:33.000000 types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-07-08 01:41:33.000000 types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:41:33.000000 types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33955 2023-07-08 01:41:37.000000 types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33891 2023-07-08 01:41:37.000000 types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:41:33.000000 types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-08 01:41:33.000000 types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-08 01:41:33.000000 types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:22.294939 types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18801 2023-07-08 01:44:22.000000 types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-08 01:44:22.000000 types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:22.000000 types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:22.000000 types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:22.000000 types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-08 01:44:22.000000 types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ssm-incidents-2.5.1/LICENSE` & `types-aiobotocore-ssm-incidents-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.1/PKG-INFO` & `types-aiobotocore-ssm-incidents-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ssm-incidents
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.SSMIncidents 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.SSMIncidents 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm-incidents.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-incidents)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ssm-incidents?color=blue)](https://pypistats.org/packages/types-aiobotocore-ssm-incidents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SSMIncidents 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
+[aiobotocore.SSMIncidents 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ssm-incidents-2.5.1/README.md` & `types-aiobotocore-ssm-incidents-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm-incidents.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-incidents)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ssm-incidents?color=blue)](https://pypistats.org/packages/types-aiobotocore-ssm-incidents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SSMIncidents 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
+[aiobotocore.SSMIncidents 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ssm-incidents-2.5.1/setup.py` & `types-aiobotocore-ssm-incidents-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ssm-incidents",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_ssm_incidents"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SSMIncidents 2.5.1 service generated with"
+        "Type annotations for aiobotocore.SSMIncidents 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents/__init__.py` & `types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents/__init__.pyi` & `types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents/__main__.py` & `types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SSMIncidents 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.SSMIncidents 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents\nOther"
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

### Comparing `types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents/client.py` & `types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents/client.pyi` & `types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents/literals.py` & `types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents/literals.pyi` & `types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents/paginator.py` & `types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents/paginator.pyi` & `types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents/type_defs.py` & `types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents/type_defs.pyi` & `types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents/waiter.py` & `types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents/waiter.pyi` & `types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents.egg-info/PKG-INFO` & `types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ssm-incidents
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.SSMIncidents 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.SSMIncidents 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm-incidents.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-incidents)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ssm-incidents?color=blue)](https://pypistats.org/packages/types-aiobotocore-ssm-incidents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SSMIncidents 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
+[aiobotocore.SSMIncidents 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ssm-incidents-2.5.1/types_aiobotocore_ssm_incidents.egg-info/SOURCES.txt` & `types-aiobotocore-ssm-incidents-2.5.2/types_aiobotocore_ssm_incidents.egg-info/SOURCES.txt`

 * *Files identical despite different names*


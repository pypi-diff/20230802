# Comparing `tmp/types-aiobotocore-ssm-sap-2.5.1.tar.gz` & `tmp/types-aiobotocore-ssm-sap-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ssm-sap-2.5.1.tar", last modified: Wed Jun 28 01:44:14 2023, max compression
+gzip compressed data, was "types-aiobotocore-ssm-sap-2.5.2.tar", last modified: Sat Jul  8 01:44:22 2023, max compression
```

## Comparing `types-aiobotocore-ssm-sap-2.5.1.tar` & `types-aiobotocore-ssm-sap-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:14.398221 types-aiobotocore-ssm-sap-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:41:31.000000 types-aiobotocore-ssm-sap-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15285 2023-06-28 01:44:14.398221 types-aiobotocore-ssm-sap-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13721 2023-06-28 01:41:31.000000 types-aiobotocore-ssm-sap-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:44:14.398221 types-aiobotocore-ssm-sap-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-28 01:41:31.000000 types-aiobotocore-ssm-sap-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:14.398221 types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-28 01:41:31.000000 types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-28 01:41:31.000000 types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-28 01:41:31.000000 types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16516 2023-06-28 01:41:31.000000 types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16486 2023-06-28 01:41:31.000000 types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-06-28 01:41:31.000000 types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-06-28 01:41:31.000000 types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-28 01:41:31.000000 types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-06-28 01:41:31.000000 types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:41:31.000000 types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15328 2023-06-28 01:41:32.000000 types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15315 2023-06-28 01:41:32.000000 types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:41:31.000000 types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:14.398221 types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15285 2023-06-28 01:44:14.000000 types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-28 01:44:14.000000 types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:44:14.000000 types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:44:14.000000 types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:44:14.000000 types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-28 01:44:14.000000 types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:22.742947 types-aiobotocore-ssm-sap-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:41:37.000000 types-aiobotocore-ssm-sap-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15285 2023-07-08 01:44:22.742947 types-aiobotocore-ssm-sap-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13721 2023-07-08 01:41:37.000000 types-aiobotocore-ssm-sap-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:22.742947 types-aiobotocore-ssm-sap-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-08 01:41:37.000000 types-aiobotocore-ssm-sap-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:22.734947 types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-08 01:41:37.000000 types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-08 01:41:37.000000 types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-08 01:41:37.000000 types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16516 2023-07-08 01:41:37.000000 types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16486 2023-07-08 01:41:37.000000 types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-07-08 01:41:38.000000 types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-07-08 01:41:37.000000 types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-07-08 01:41:37.000000 types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-08 01:41:37.000000 types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:41:37.000000 types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15328 2023-07-08 01:41:38.000000 types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15315 2023-07-08 01:41:38.000000 types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:41:37.000000 types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:22.742947 types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15285 2023-07-08 01:44:22.000000 types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-08 01:44:22.000000 types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:22.000000 types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:22.000000 types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:22.000000 types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-08 01:44:22.000000 types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ssm-sap-2.5.1/LICENSE` & `types-aiobotocore-ssm-sap-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-sap-2.5.1/PKG-INFO` & `types-aiobotocore-ssm-sap-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ssm-sap
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.SsmSap 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.SsmSap 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm-sap.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-sap)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ssm-sap?color=blue)](https://pypistats.org/packages/types-aiobotocore-ssm-sap)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SsmSap 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
+[aiobotocore.SsmSap 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ssm-sap-2.5.1/README.md` & `types-aiobotocore-ssm-sap-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm-sap.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-sap)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ssm-sap?color=blue)](https://pypistats.org/packages/types-aiobotocore-ssm-sap)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SsmSap 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
+[aiobotocore.SsmSap 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ssm-sap-2.5.1/setup.py` & `types-aiobotocore-ssm-sap-2.5.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ssm-sap",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_ssm_sap"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SsmSap 2.5.1 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.SsmSap 2.5.2 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap/__init__.py` & `types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap/__init__.pyi` & `types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap/__main__.py` & `types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SsmSap 2.5.1\nVersion:         2.5.1\nBuilder version:"
+        "Type annotations for aiobotocore.SsmSap 2.5.2\nVersion:         2.5.2\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap\nOther"
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

### Comparing `types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap/client.py` & `types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap/client.pyi` & `types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap/literals.py` & `types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap/literals.pyi` & `types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap/paginator.py` & `types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap/paginator.pyi` & `types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap/type_defs.py` & `types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap/type_defs.pyi` & `types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap.egg-info/PKG-INFO` & `types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ssm-sap
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.SsmSap 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.SsmSap 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm-sap.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-sap)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ssm-sap?color=blue)](https://pypistats.org/packages/types-aiobotocore-ssm-sap)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SsmSap 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
+[aiobotocore.SsmSap 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ssm-sap-2.5.1/types_aiobotocore_ssm_sap.egg-info/SOURCES.txt` & `types-aiobotocore-ssm-sap-2.5.2/types_aiobotocore_ssm_sap.egg-info/SOURCES.txt`

 * *Files identical despite different names*


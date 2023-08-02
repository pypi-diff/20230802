# Comparing `tmp/types-aiobotocore-payment-cryptography-2.5.1.tar.gz` & `tmp/types-aiobotocore-payment-cryptography-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-payment-cryptography-2.5.1.tar", last modified: Wed Jun 28 01:43:58 2023, max compression
+gzip compressed data, was "types-aiobotocore-payment-cryptography-2.5.2.tar", last modified: Sat Jul  8 01:44:06 2023, max compression
```

## Comparing `types-aiobotocore-payment-cryptography-2.5.1.tar` & `types-aiobotocore-payment-cryptography-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:57.994190 types-aiobotocore-payment-cryptography-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:36:25.000000 types-aiobotocore-payment-cryptography-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-06-28 01:43:57.994190 types-aiobotocore-payment-cryptography-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14401 2023-06-28 01:36:25.000000 types-aiobotocore-payment-cryptography-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:57.994190 types-aiobotocore-payment-cryptography-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-06-28 01:36:24.000000 types-aiobotocore-payment-cryptography-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:57.994190 types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-28 01:36:25.000000 types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-28 01:36:25.000000 types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-28 01:36:25.000000 types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19845 2023-06-28 01:36:25.000000 types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19813 2023-06-28 01:36:25.000000 types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9827 2023-06-28 01:36:25.000000 types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-06-28 01:36:25.000000 types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-28 01:36:25.000000 types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-06-28 01:36:25.000000 types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:36:25.000000 types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17707 2023-06-28 01:36:25.000000 types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17683 2023-06-28 01:36:25.000000 types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:36:25.000000 types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:57.994190 types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-06-28 01:43:57.000000 types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-28 01:43:57.000000 types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:57.000000 types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:57.000000 types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:57.000000 types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-28 01:43:57.000000 types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:06.190667 types-aiobotocore-payment-cryptography-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:36:18.000000 types-aiobotocore-payment-cryptography-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-07-08 01:44:06.186667 types-aiobotocore-payment-cryptography-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14401 2023-07-08 01:36:18.000000 types-aiobotocore-payment-cryptography-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:06.190667 types-aiobotocore-payment-cryptography-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-08 01:36:18.000000 types-aiobotocore-payment-cryptography-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:06.182667 types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-08 01:36:18.000000 types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-08 01:36:18.000000 types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-08 01:36:18.000000 types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19845 2023-07-08 01:36:18.000000 types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19813 2023-07-08 01:36:18.000000 types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9827 2023-07-08 01:36:18.000000 types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-07-08 01:36:18.000000 types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-08 01:36:18.000000 types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-07-08 01:36:18.000000 types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:36:18.000000 types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17707 2023-07-08 01:36:19.000000 types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17683 2023-07-08 01:36:19.000000 types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:36:18.000000 types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:06.186667 types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-07-08 01:44:06.000000 types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-08 01:44:06.000000 types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:06.000000 types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:06.000000 types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:06.000000 types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-08 01:44:06.000000 types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-payment-cryptography-2.5.1/LICENSE` & `types-aiobotocore-payment-cryptography-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.5.1/PKG-INFO` & `types-aiobotocore-payment-cryptography-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-payment-cryptography
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.PaymentCryptographyControlPlane 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.PaymentCryptographyControlPlane 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-payment-cryptography.svg?color=blue)](https://pypi.org/project/types-aiobotocore-payment-cryptography)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-payment-cryptography?color=blue)](https://pypistats.org/packages/types-aiobotocore-payment-cryptography)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PaymentCryptographyControlPlane 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
+[aiobotocore.PaymentCryptographyControlPlane 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-payment-cryptography-2.5.1/README.md` & `types-aiobotocore-payment-cryptography-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-payment-cryptography.svg?color=blue)](https://pypi.org/project/types-aiobotocore-payment-cryptography)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-payment-cryptography?color=blue)](https://pypistats.org/packages/types-aiobotocore-payment-cryptography)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PaymentCryptographyControlPlane 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
+[aiobotocore.PaymentCryptographyControlPlane 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-payment-cryptography-2.5.1/setup.py` & `types-aiobotocore-payment-cryptography-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-payment-cryptography",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_payment_cryptography"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.PaymentCryptographyControlPlane 2.5.1 service generated"
+        "Type annotations for aiobotocore.PaymentCryptographyControlPlane 2.5.2 service generated"
         " with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography/__init__.py` & `types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography/__init__.pyi` & `types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography/__main__.py` & `types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.PaymentCryptographyControlPlane 2.5.1\nVersion:        "
-        " 2.5.1\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.PaymentCryptographyControlPlane 2.5.2\nVersion:        "
+        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane\nOther"
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

### Comparing `types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography/client.py` & `types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography/client.pyi` & `types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography/literals.py` & `types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography/literals.pyi` & `types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography/paginator.py` & `types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography/paginator.pyi` & `types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography/type_defs.py` & `types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography/type_defs.pyi` & `types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography.egg-info/PKG-INFO` & `types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-payment-cryptography
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.PaymentCryptographyControlPlane 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.PaymentCryptographyControlPlane 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-payment-cryptography.svg?color=blue)](https://pypi.org/project/types-aiobotocore-payment-cryptography)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-payment-cryptography?color=blue)](https://pypistats.org/packages/types-aiobotocore-payment-cryptography)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PaymentCryptographyControlPlane 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
+[aiobotocore.PaymentCryptographyControlPlane 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-payment-cryptography-2.5.1/types_aiobotocore_payment_cryptography.egg-info/SOURCES.txt` & `types-aiobotocore-payment-cryptography-2.5.2/types_aiobotocore_payment_cryptography.egg-info/SOURCES.txt`

 * *Files identical despite different names*


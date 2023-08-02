# Comparing `tmp/types-aiobotocore-route53-recovery-readiness-2.5.1.tar.gz` & `tmp/types-aiobotocore-route53-recovery-readiness-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-route53-recovery-readiness-2.5.1.tar", last modified: Wed Jun 28 01:44:05 2023, max compression
+gzip compressed data, was "types-aiobotocore-route53-recovery-readiness-2.5.2.tar", last modified: Sat Jul  8 01:44:13 2023, max compression
```

## Comparing `types-aiobotocore-route53-recovery-readiness-2.5.1.tar` & `types-aiobotocore-route53-recovery-readiness-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:05.426204 types-aiobotocore-route53-recovery-readiness-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:39:28.000000 types-aiobotocore-route53-recovery-readiness-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19440 2023-06-28 01:44:05.422204 types-aiobotocore-route53-recovery-readiness-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17801 2023-06-28 01:39:28.000000 types-aiobotocore-route53-recovery-readiness-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:44:05.426204 types-aiobotocore-route53-recovery-readiness-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-28 01:39:28.000000 types-aiobotocore-route53-recovery-readiness-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:05.422204 types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness/
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-28 01:39:28.000000 types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-28 01:39:28.000000 types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-28 01:39:28.000000 types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30666 2023-06-28 01:39:28.000000 types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30615 2023-06-28 01:39:28.000000 types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-06-28 01:39:28.000000 types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-06-28 01:39:28.000000 types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-06-28 01:39:28.000000 types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-06-28 01:39:28.000000 types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:39:28.000000 types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29847 2023-06-28 01:39:29.000000 types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29810 2023-06-28 01:39:29.000000 types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:39:28.000000 types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:05.422204 types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19440 2023-06-28 01:44:05.000000 types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-28 01:44:05.000000 types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:44:05.000000 types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:44:05.000000 types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:44:05.000000 types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-28 01:44:05.000000 types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:13.662803 types-aiobotocore-route53-recovery-readiness-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:39:32.000000 types-aiobotocore-route53-recovery-readiness-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19440 2023-07-08 01:44:13.662803 types-aiobotocore-route53-recovery-readiness-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17801 2023-07-08 01:39:32.000000 types-aiobotocore-route53-recovery-readiness-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:13.662803 types-aiobotocore-route53-recovery-readiness-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-08 01:39:32.000000 types-aiobotocore-route53-recovery-readiness-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:13.650803 types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness/
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-08 01:39:32.000000 types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-08 01:39:32.000000 types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-08 01:39:32.000000 types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30666 2023-07-08 01:39:32.000000 types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30615 2023-07-08 01:39:32.000000 types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-07-08 01:39:32.000000 types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-07-08 01:39:32.000000 types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-07-08 01:39:32.000000 types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-07-08 01:39:32.000000 types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:39:32.000000 types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29847 2023-07-08 01:39:33.000000 types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29810 2023-07-08 01:39:33.000000 types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:39:32.000000 types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:13.662803 types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19440 2023-07-08 01:44:13.000000 types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-08 01:44:13.000000 types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:13.000000 types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:13.000000 types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:13.000000 types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-08 01:44:13.000000 types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.1/LICENSE` & `types-aiobotocore-route53-recovery-readiness-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.1/PKG-INFO` & `types-aiobotocore-route53-recovery-readiness-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-route53-recovery-readiness
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.Route53RecoveryReadiness 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.Route53RecoveryReadiness 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53-recovery-readiness.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-readiness)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-route53-recovery-readiness?color=blue)](https://pypistats.org/packages/types-aiobotocore-route53-recovery-readiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Route53RecoveryReadiness 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
+[aiobotocore.Route53RecoveryReadiness 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.1/README.md` & `types-aiobotocore-route53-recovery-readiness-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53-recovery-readiness.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-readiness)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-route53-recovery-readiness?color=blue)](https://pypistats.org/packages/types-aiobotocore-route53-recovery-readiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Route53RecoveryReadiness 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
+[aiobotocore.Route53RecoveryReadiness 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.1/setup.py` & `types-aiobotocore-route53-recovery-readiness-2.5.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-route53-recovery-readiness",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_route53_recovery_readiness"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Route53RecoveryReadiness 2.5.1 service generated with"
+        "Type annotations for aiobotocore.Route53RecoveryReadiness 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness/__init__.py` & `types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness/__init__.pyi` & `types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness/__main__.py` & `types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Route53RecoveryReadiness 2.5.1\nVersion:        "
-        " 2.5.1\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Route53RecoveryReadiness 2.5.2\nVersion:        "
+        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness\nOther"
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

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness/client.py` & `types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness/client.pyi` & `types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness/literals.py` & `types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness/literals.pyi` & `types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness/paginator.py` & `types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness/paginator.pyi` & `types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness/type_defs.py` & `types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness/type_defs.pyi` & `types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness.egg-info/PKG-INFO` & `types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-route53-recovery-readiness
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.Route53RecoveryReadiness 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.Route53RecoveryReadiness 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53-recovery-readiness.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-readiness)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-route53-recovery-readiness?color=blue)](https://pypistats.org/packages/types-aiobotocore-route53-recovery-readiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Route53RecoveryReadiness 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
+[aiobotocore.Route53RecoveryReadiness 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.1/types_aiobotocore_route53_recovery_readiness.egg-info/SOURCES.txt` & `types-aiobotocore-route53-recovery-readiness-2.5.2/types_aiobotocore_route53_recovery_readiness.egg-info/SOURCES.txt`

 * *Files identical despite different names*


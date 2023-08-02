# Comparing `tmp/types-aiobotocore-route53resolver-2.5.1.tar.gz` & `tmp/types-aiobotocore-route53resolver-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-route53resolver-2.5.1.tar", last modified: Wed Jun 28 01:44:05 2023, max compression
+gzip compressed data, was "types-aiobotocore-route53resolver-2.5.2.tar", last modified: Sat Jul  8 01:44:14 2023, max compression
```

## Comparing `types-aiobotocore-route53resolver-2.5.1.tar` & `types-aiobotocore-route53resolver-2.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:05.666204 types-aiobotocore-route53resolver-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:39:31.000000 types-aiobotocore-route53resolver-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25105 2023-06-28 01:44:05.666204 types-aiobotocore-route53resolver-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23508 2023-06-28 01:39:31.000000 types-aiobotocore-route53resolver-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:44:05.666204 types-aiobotocore-route53resolver-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-28 01:39:31.000000 types-aiobotocore-route53resolver-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:05.662204 types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver/
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-06-28 01:39:31.000000 types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-06-28 01:39:31.000000 types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-28 01:39:31.000000 types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58137 2023-06-28 01:39:32.000000 types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    58050 2023-06-28 01:39:32.000000 types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13933 2023-06-28 01:39:32.000000 types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-06-28 01:39:32.000000 types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20441 2023-06-28 01:39:32.000000 types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-06-28 01:39:32.000000 types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:39:31.000000 types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    57085 2023-06-28 01:39:35.000000 types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    57044 2023-06-28 01:39:33.000000 types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:39:31.000000 types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:05.666204 types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25105 2023-06-28 01:44:05.000000 types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-28 01:44:05.000000 types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:44:05.000000 types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:44:05.000000 types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:44:05.000000 types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-28 01:44:05.000000 types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:14.118811 types-aiobotocore-route53resolver-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:39:35.000000 types-aiobotocore-route53resolver-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25105 2023-07-08 01:44:14.118811 types-aiobotocore-route53resolver-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23508 2023-07-08 01:39:35.000000 types-aiobotocore-route53resolver-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:14.118811 types-aiobotocore-route53resolver-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-08 01:39:35.000000 types-aiobotocore-route53resolver-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:14.118811 types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-08 01:39:35.000000 types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-07-08 01:39:35.000000 types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-08 01:39:35.000000 types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58137 2023-07-08 01:39:36.000000 types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58050 2023-07-08 01:39:36.000000 types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13933 2023-07-08 01:39:36.000000 types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-07-08 01:39:36.000000 types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20441 2023-07-08 01:39:36.000000 types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-07-08 01:39:36.000000 types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:39:35.000000 types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    57085 2023-07-08 01:39:37.000000 types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57044 2023-07-08 01:39:37.000000 types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:39:35.000000 types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:14.118811 types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25105 2023-07-08 01:44:13.000000 types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-08 01:44:13.000000 types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:13.000000 types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:13.000000 types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:13.000000 types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-08 01:44:13.000000 types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-route53resolver-2.5.1/LICENSE` & `types-aiobotocore-route53resolver-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53resolver-2.5.1/PKG-INFO` & `types-aiobotocore-route53resolver-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-route53resolver
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.Route53Resolver 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.Route53Resolver 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53resolver.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53resolver)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-route53resolver?color=blue)](https://pypistats.org/packages/types-aiobotocore-route53resolver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Route53Resolver 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
+[aiobotocore.Route53Resolver 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-route53resolver-2.5.1/README.md` & `types-aiobotocore-route53resolver-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53resolver.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53resolver)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-route53resolver?color=blue)](https://pypistats.org/packages/types-aiobotocore-route53resolver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Route53Resolver 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
+[aiobotocore.Route53Resolver 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-route53resolver-2.5.1/setup.py` & `types-aiobotocore-route53resolver-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-route53resolver",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_route53resolver"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Route53Resolver 2.5.1 service generated with"
+        "Type annotations for aiobotocore.Route53Resolver 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver/__init__.py` & `types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver/__init__.pyi` & `types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver/__main__.py` & `types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Route53Resolver 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.Route53Resolver 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver\nOther"
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

### Comparing `types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver/client.py` & `types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver/client.pyi` & `types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver/literals.py` & `types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver/literals.pyi` & `types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver/paginator.py` & `types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver/paginator.pyi` & `types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver/type_defs.py` & `types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver/type_defs.pyi` & `types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver.egg-info/PKG-INFO` & `types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-route53resolver
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.Route53Resolver 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.Route53Resolver 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53resolver.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53resolver)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-route53resolver?color=blue)](https://pypistats.org/packages/types-aiobotocore-route53resolver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Route53Resolver 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
+[aiobotocore.Route53Resolver 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-route53resolver-2.5.1/types_aiobotocore_route53resolver.egg-info/SOURCES.txt` & `types-aiobotocore-route53resolver-2.5.2/types_aiobotocore_route53resolver.egg-info/SOURCES.txt`

 * *Files identical despite different names*


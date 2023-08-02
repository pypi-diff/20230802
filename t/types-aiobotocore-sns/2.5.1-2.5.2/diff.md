# Comparing `tmp/types-aiobotocore-sns-2.5.1.tar.gz` & `tmp/types-aiobotocore-sns-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sns-2.5.1.tar", last modified: Wed Jun 28 01:44:13 2023, max compression
+gzip compressed data, was "types-aiobotocore-sns-2.5.2.tar", last modified: Sat Jul  8 01:44:21 2023, max compression
```

## Comparing `types-aiobotocore-sns-2.5.1.tar` & `types-aiobotocore-sns-2.5.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:13.314219 types-aiobotocore-sns-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:41:10.000000 types-aiobotocore-sns-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21434 2023-06-28 01:44:13.310219 types-aiobotocore-sns-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19885 2023-06-28 01:41:10.000000 types-aiobotocore-sns-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:44:13.314219 types-aiobotocore-sns-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-28 01:41:10.000000 types-aiobotocore-sns-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:13.306219 types-aiobotocore-sns-2.5.1/types_aiobotocore_sns/
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-28 01:41:10.000000 types-aiobotocore-sns-2.5.1/types_aiobotocore_sns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-28 01:41:10.000000 types-aiobotocore-sns-2.5.1/types_aiobotocore_sns/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-28 01:41:10.000000 types-aiobotocore-sns-2.5.1/types_aiobotocore_sns/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35353 2023-06-28 01:41:13.000000 types-aiobotocore-sns-2.5.1/types_aiobotocore_sns/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    35294 2023-06-28 01:41:12.000000 types-aiobotocore-sns-2.5.1/types_aiobotocore_sns/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-06-28 01:41:13.000000 types-aiobotocore-sns-2.5.1/types_aiobotocore_sns/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-06-28 01:41:13.000000 types-aiobotocore-sns-2.5.1/types_aiobotocore_sns/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-06-28 01:41:13.000000 types-aiobotocore-sns-2.5.1/types_aiobotocore_sns/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-06-28 01:41:13.000000 types-aiobotocore-sns-2.5.1/types_aiobotocore_sns/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:41:10.000000 types-aiobotocore-sns-2.5.1/types_aiobotocore_sns/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37388 2023-06-28 01:41:13.000000 types-aiobotocore-sns-2.5.1/types_aiobotocore_sns/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    37313 2023-06-28 01:41:13.000000 types-aiobotocore-sns-2.5.1/types_aiobotocore_sns/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    34633 2023-06-28 01:41:14.000000 types-aiobotocore-sns-2.5.1/types_aiobotocore_sns/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34586 2023-06-28 01:41:13.000000 types-aiobotocore-sns-2.5.1/types_aiobotocore_sns/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:41:10.000000 types-aiobotocore-sns-2.5.1/types_aiobotocore_sns/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:44:13.310219 types-aiobotocore-sns-2.5.1/types_aiobotocore_sns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21434 2023-06-28 01:44:13.000000 types-aiobotocore-sns-2.5.1/types_aiobotocore_sns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-28 01:44:13.000000 types-aiobotocore-sns-2.5.1/types_aiobotocore_sns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:44:13.000000 types-aiobotocore-sns-2.5.1/types_aiobotocore_sns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:44:13.000000 types-aiobotocore-sns-2.5.1/types_aiobotocore_sns.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:44:13.000000 types-aiobotocore-sns-2.5.1/types_aiobotocore_sns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-28 01:44:13.000000 types-aiobotocore-sns-2.5.1/types_aiobotocore_sns.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:21.586926 types-aiobotocore-sns-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:41:16.000000 types-aiobotocore-sns-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21434 2023-07-08 01:44:21.582926 types-aiobotocore-sns-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19885 2023-07-08 01:41:16.000000 types-aiobotocore-sns-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:21.586926 types-aiobotocore-sns-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-08 01:41:16.000000 types-aiobotocore-sns-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:21.578925 types-aiobotocore-sns-2.5.2/types_aiobotocore_sns/
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-08 01:41:16.000000 types-aiobotocore-sns-2.5.2/types_aiobotocore_sns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-08 01:41:16.000000 types-aiobotocore-sns-2.5.2/types_aiobotocore_sns/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-08 01:41:16.000000 types-aiobotocore-sns-2.5.2/types_aiobotocore_sns/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35353 2023-07-08 01:41:16.000000 types-aiobotocore-sns-2.5.2/types_aiobotocore_sns/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35294 2023-07-08 01:41:16.000000 types-aiobotocore-sns-2.5.2/types_aiobotocore_sns/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-07-08 01:41:19.000000 types-aiobotocore-sns-2.5.2/types_aiobotocore_sns/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-07-08 01:41:19.000000 types-aiobotocore-sns-2.5.2/types_aiobotocore_sns/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-07-08 01:41:19.000000 types-aiobotocore-sns-2.5.2/types_aiobotocore_sns/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-07-08 01:41:19.000000 types-aiobotocore-sns-2.5.2/types_aiobotocore_sns/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:41:16.000000 types-aiobotocore-sns-2.5.2/types_aiobotocore_sns/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37388 2023-07-08 01:41:19.000000 types-aiobotocore-sns-2.5.2/types_aiobotocore_sns/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37313 2023-07-08 01:41:19.000000 types-aiobotocore-sns-2.5.2/types_aiobotocore_sns/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    34633 2023-07-08 01:41:19.000000 types-aiobotocore-sns-2.5.2/types_aiobotocore_sns/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34586 2023-07-08 01:41:19.000000 types-aiobotocore-sns-2.5.2/types_aiobotocore_sns/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:41:16.000000 types-aiobotocore-sns-2.5.2/types_aiobotocore_sns/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:21.582926 types-aiobotocore-sns-2.5.2/types_aiobotocore_sns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21434 2023-07-08 01:44:21.000000 types-aiobotocore-sns-2.5.2/types_aiobotocore_sns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-08 01:44:21.000000 types-aiobotocore-sns-2.5.2/types_aiobotocore_sns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:21.000000 types-aiobotocore-sns-2.5.2/types_aiobotocore_sns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:21.000000 types-aiobotocore-sns-2.5.2/types_aiobotocore_sns.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:21.000000 types-aiobotocore-sns-2.5.2/types_aiobotocore_sns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:44:21.000000 types-aiobotocore-sns-2.5.2/types_aiobotocore_sns.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sns-2.5.1/LICENSE` & `types-aiobotocore-sns-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.1/PKG-INFO` & `types-aiobotocore-sns-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sns
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.SNS 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.SNS 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sns.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sns)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sns?color=blue)](https://pypistats.org/packages/types-aiobotocore-sns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SNS 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
+[aiobotocore.SNS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-sns-2.5.1/README.md` & `types-aiobotocore-sns-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sns.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sns)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sns?color=blue)](https://pypistats.org/packages/types-aiobotocore-sns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SNS 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
+[aiobotocore.SNS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-sns-2.5.1/setup.py` & `types-aiobotocore-sns-2.5.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sns",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_sns"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SNS 2.5.1 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.SNS 2.5.2 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-sns-2.5.1/types_aiobotocore_sns/__init__.py` & `types-aiobotocore-sns-2.5.2/types_aiobotocore_sns/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.1/types_aiobotocore_sns/__init__.pyi` & `types-aiobotocore-sns-2.5.2/types_aiobotocore_sns/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.1/types_aiobotocore_sns/__main__.py` & `types-aiobotocore-sns-2.5.2/types_aiobotocore_sns/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SNS 2.5.1\nVersion:         2.5.1\nBuilder version:"
+        "Type annotations for aiobotocore.SNS 2.5.2\nVersion:         2.5.2\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS\nOther"
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

### Comparing `types-aiobotocore-sns-2.5.1/types_aiobotocore_sns/client.py` & `types-aiobotocore-sns-2.5.2/types_aiobotocore_sns/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.1/types_aiobotocore_sns/client.pyi` & `types-aiobotocore-sns-2.5.2/types_aiobotocore_sns/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.1/types_aiobotocore_sns/literals.py` & `types-aiobotocore-sns-2.5.2/types_aiobotocore_sns/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.1/types_aiobotocore_sns/literals.pyi` & `types-aiobotocore-sns-2.5.2/types_aiobotocore_sns/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.1/types_aiobotocore_sns/paginator.py` & `types-aiobotocore-sns-2.5.2/types_aiobotocore_sns/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.1/types_aiobotocore_sns/paginator.pyi` & `types-aiobotocore-sns-2.5.2/types_aiobotocore_sns/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.1/types_aiobotocore_sns/service_resource.py` & `types-aiobotocore-sns-2.5.2/types_aiobotocore_sns/service_resource.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.1/types_aiobotocore_sns/service_resource.pyi` & `types-aiobotocore-sns-2.5.2/types_aiobotocore_sns/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.1/types_aiobotocore_sns/type_defs.py` & `types-aiobotocore-sns-2.5.2/types_aiobotocore_sns/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.1/types_aiobotocore_sns/type_defs.pyi` & `types-aiobotocore-sns-2.5.2/types_aiobotocore_sns/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.1/types_aiobotocore_sns.egg-info/PKG-INFO` & `types-aiobotocore-sns-2.5.2/types_aiobotocore_sns.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sns
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.SNS 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.SNS 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sns.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sns)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sns?color=blue)](https://pypistats.org/packages/types-aiobotocore-sns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SNS 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
+[aiobotocore.SNS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-sns-2.5.1/types_aiobotocore_sns.egg-info/SOURCES.txt` & `types-aiobotocore-sns-2.5.2/types_aiobotocore_sns.egg-info/SOURCES.txt`

 * *Files identical despite different names*


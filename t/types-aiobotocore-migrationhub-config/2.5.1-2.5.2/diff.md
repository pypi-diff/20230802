# Comparing `tmp/types-aiobotocore-migrationhub-config-2.5.1.tar.gz` & `tmp/types-aiobotocore-migrationhub-config-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-migrationhub-config-2.5.1.tar", last modified: Wed Jun 28 01:43:52 2023, max compression
+gzip compressed data, was "types-aiobotocore-migrationhub-config-2.5.2.tar", last modified: Sat Jul  8 01:44:00 2023, max compression
```

## Comparing `types-aiobotocore-migrationhub-config-2.5.1.tar` & `types-aiobotocore-migrationhub-config-2.5.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:52.186179 types-aiobotocore-migrationhub-config-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:35:34.000000 types-aiobotocore-migrationhub-config-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-06-28 01:43:52.186179 types-aiobotocore-migrationhub-config-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11286 2023-06-28 01:35:34.000000 types-aiobotocore-migrationhub-config-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:52.186179 types-aiobotocore-migrationhub-config-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-28 01:35:34.000000 types-aiobotocore-migrationhub-config-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:52.182179 types-aiobotocore-migrationhub-config-2.5.1/types_aiobotocore_migrationhub_config/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-28 01:35:34.000000 types-aiobotocore-migrationhub-config-2.5.1/types_aiobotocore_migrationhub_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-28 01:35:34.000000 types-aiobotocore-migrationhub-config-2.5.1/types_aiobotocore_migrationhub_config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-28 01:35:34.000000 types-aiobotocore-migrationhub-config-2.5.1/types_aiobotocore_migrationhub_config/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-06-28 01:35:34.000000 types-aiobotocore-migrationhub-config-2.5.1/types_aiobotocore_migrationhub_config/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-06-28 01:35:34.000000 types-aiobotocore-migrationhub-config-2.5.1/types_aiobotocore_migrationhub_config/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-06-28 01:35:34.000000 types-aiobotocore-migrationhub-config-2.5.1/types_aiobotocore_migrationhub_config/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-06-28 01:35:34.000000 types-aiobotocore-migrationhub-config-2.5.1/types_aiobotocore_migrationhub_config/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:35:34.000000 types-aiobotocore-migrationhub-config-2.5.1/types_aiobotocore_migrationhub_config/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-06-28 01:35:34.000000 types-aiobotocore-migrationhub-config-2.5.1/types_aiobotocore_migrationhub_config/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-06-28 01:35:34.000000 types-aiobotocore-migrationhub-config-2.5.1/types_aiobotocore_migrationhub_config/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:35:34.000000 types-aiobotocore-migrationhub-config-2.5.1/types_aiobotocore_migrationhub_config/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:52.186179 types-aiobotocore-migrationhub-config-2.5.1/types_aiobotocore_migrationhub_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-06-28 01:43:52.000000 types-aiobotocore-migrationhub-config-2.5.1/types_aiobotocore_migrationhub_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-28 01:43:52.000000 types-aiobotocore-migrationhub-config-2.5.1/types_aiobotocore_migrationhub_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:52.000000 types-aiobotocore-migrationhub-config-2.5.1/types_aiobotocore_migrationhub_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:52.000000 types-aiobotocore-migrationhub-config-2.5.1/types_aiobotocore_migrationhub_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:52.000000 types-aiobotocore-migrationhub-config-2.5.1/types_aiobotocore_migrationhub_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:52.000000 types-aiobotocore-migrationhub-config-2.5.1/types_aiobotocore_migrationhub_config.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:00.554562 types-aiobotocore-migrationhub-config-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:35:25.000000 types-aiobotocore-migrationhub-config-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-07-08 01:44:00.554562 types-aiobotocore-migrationhub-config-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11286 2023-07-08 01:35:25.000000 types-aiobotocore-migrationhub-config-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:00.554562 types-aiobotocore-migrationhub-config-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-08 01:35:24.000000 types-aiobotocore-migrationhub-config-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:00.554562 types-aiobotocore-migrationhub-config-2.5.2/types_aiobotocore_migrationhub_config/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-08 01:35:25.000000 types-aiobotocore-migrationhub-config-2.5.2/types_aiobotocore_migrationhub_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-08 01:35:25.000000 types-aiobotocore-migrationhub-config-2.5.2/types_aiobotocore_migrationhub_config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-08 01:35:25.000000 types-aiobotocore-migrationhub-config-2.5.2/types_aiobotocore_migrationhub_config/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-07-08 01:35:25.000000 types-aiobotocore-migrationhub-config-2.5.2/types_aiobotocore_migrationhub_config/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-07-08 01:35:25.000000 types-aiobotocore-migrationhub-config-2.5.2/types_aiobotocore_migrationhub_config/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-07-08 01:35:25.000000 types-aiobotocore-migrationhub-config-2.5.2/types_aiobotocore_migrationhub_config/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-07-08 01:35:25.000000 types-aiobotocore-migrationhub-config-2.5.2/types_aiobotocore_migrationhub_config/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:35:25.000000 types-aiobotocore-migrationhub-config-2.5.2/types_aiobotocore_migrationhub_config/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-08 01:35:25.000000 types-aiobotocore-migrationhub-config-2.5.2/types_aiobotocore_migrationhub_config/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-08 01:35:25.000000 types-aiobotocore-migrationhub-config-2.5.2/types_aiobotocore_migrationhub_config/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:35:25.000000 types-aiobotocore-migrationhub-config-2.5.2/types_aiobotocore_migrationhub_config/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:00.554562 types-aiobotocore-migrationhub-config-2.5.2/types_aiobotocore_migrationhub_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-07-08 01:44:00.000000 types-aiobotocore-migrationhub-config-2.5.2/types_aiobotocore_migrationhub_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-08 01:44:00.000000 types-aiobotocore-migrationhub-config-2.5.2/types_aiobotocore_migrationhub_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:00.000000 types-aiobotocore-migrationhub-config-2.5.2/types_aiobotocore_migrationhub_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:00.000000 types-aiobotocore-migrationhub-config-2.5.2/types_aiobotocore_migrationhub_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:00.000000 types-aiobotocore-migrationhub-config-2.5.2/types_aiobotocore_migrationhub_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:00.000000 types-aiobotocore-migrationhub-config-2.5.2/types_aiobotocore_migrationhub_config.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-migrationhub-config-2.5.1/LICENSE` & `types-aiobotocore-migrationhub-config-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhub-config-2.5.1/PKG-INFO` & `types-aiobotocore-migrationhub-config-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-migrationhub-config
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.MigrationHubConfig 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.MigrationHubConfig 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhub_config/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-migrationhub-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-migrationhub-config)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhub_config/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-migrationhub-config?color=blue)](https://pypistats.org/packages/types-aiobotocore-migrationhub-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MigrationHubConfig 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
+[aiobotocore.MigrationHubConfig 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-migrationhub-config-2.5.1/README.md` & `types-aiobotocore-migrationhub-config-2.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-migrationhub-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-migrationhub-config)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhub_config/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-migrationhub-config?color=blue)](https://pypistats.org/packages/types-aiobotocore-migrationhub-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MigrationHubConfig 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
+[aiobotocore.MigrationHubConfig 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-migrationhub-config-2.5.1/setup.py` & `types-aiobotocore-migrationhub-config-2.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-migrationhub-config",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_migrationhub_config"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MigrationHubConfig 2.5.1 service generated with"
+        "Type annotations for aiobotocore.MigrationHubConfig 2.5.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-migrationhub-config-2.5.1/types_aiobotocore_migrationhub_config/__init__.py` & `types-aiobotocore-migrationhub-config-2.5.2/types_aiobotocore_migrationhub_config/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhub-config-2.5.1/types_aiobotocore_migrationhub_config/__init__.pyi` & `types-aiobotocore-migrationhub-config-2.5.2/types_aiobotocore_migrationhub_config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhub-config-2.5.1/types_aiobotocore_migrationhub_config/__main__.py` & `types-aiobotocore-migrationhub-config-2.5.2/types_aiobotocore_migrationhub_config/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MigrationHubConfig 2.5.1\nVersion:         2.5.1\nBuilder"
+        "Type annotations for aiobotocore.MigrationHubConfig 2.5.2\nVersion:         2.5.2\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhub_config//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig\nOther"
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

### Comparing `types-aiobotocore-migrationhub-config-2.5.1/types_aiobotocore_migrationhub_config/client.py` & `types-aiobotocore-migrationhub-config-2.5.2/types_aiobotocore_migrationhub_config/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhub-config-2.5.1/types_aiobotocore_migrationhub_config/client.pyi` & `types-aiobotocore-migrationhub-config-2.5.2/types_aiobotocore_migrationhub_config/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhub-config-2.5.1/types_aiobotocore_migrationhub_config/literals.py` & `types-aiobotocore-migrationhub-config-2.5.2/types_aiobotocore_migrationhub_config/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhub-config-2.5.1/types_aiobotocore_migrationhub_config/literals.pyi` & `types-aiobotocore-migrationhub-config-2.5.2/types_aiobotocore_migrationhub_config/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhub-config-2.5.1/types_aiobotocore_migrationhub_config/type_defs.py` & `types-aiobotocore-migrationhub-config-2.5.2/types_aiobotocore_migrationhub_config/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhub-config-2.5.1/types_aiobotocore_migrationhub_config/type_defs.pyi` & `types-aiobotocore-migrationhub-config-2.5.2/types_aiobotocore_migrationhub_config/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhub-config-2.5.1/types_aiobotocore_migrationhub_config.egg-info/PKG-INFO` & `types-aiobotocore-migrationhub-config-2.5.2/types_aiobotocore_migrationhub_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-migrationhub-config
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.MigrationHubConfig 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.MigrationHubConfig 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhub_config/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-migrationhub-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-migrationhub-config)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhub_config/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-migrationhub-config?color=blue)](https://pypistats.org/packages/types-aiobotocore-migrationhub-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MigrationHubConfig 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
+[aiobotocore.MigrationHubConfig 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-migrationhub-config-2.5.1/types_aiobotocore_migrationhub_config.egg-info/SOURCES.txt` & `types-aiobotocore-migrationhub-config-2.5.2/types_aiobotocore_migrationhub_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*


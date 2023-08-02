# Comparing `tmp/poetry_git_version_plugin-1.0.2.tar.gz` & `tmp/poetry_git_version_plugin-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_git_version_plugin-1.0.2.tar", max compression
+gzip compressed data, was "poetry_git_version_plugin-1.0.3.tar", max compression
```

## Comparing `poetry_git_version_plugin-1.0.2.tar` & `poetry_git_version_plugin-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1056 2023-06-01 21:41:56.857940 poetry_git_version_plugin-1.0.2/LICENSE
--rw-r--r--   0        0        0        0 2023-06-01 21:43:55.917358 poetry_git_version_plugin-1.0.2/poetry_git_version_plugin/__init__.py
--rw-r--r--   0        0        0      330 2023-06-01 21:41:56.857940 poetry_git_version_plugin-1.0.2/poetry_git_version_plugin/commands.py
--rw-r--r--   0        0        0     2264 2023-06-01 21:41:56.857940 poetry_git_version_plugin-1.0.2/poetry_git_version_plugin/config.py
--rw-r--r--   0        0        0      837 2023-06-01 21:41:56.857940 poetry_git_version_plugin-1.0.2/poetry_git_version_plugin/exceptions.py
--rw-r--r--   0        0        0     1114 2023-06-01 21:41:56.857940 poetry_git_version_plugin-1.0.2/poetry_git_version_plugin/plugins.py
--rw-r--r--   0        0        0     5882 2023-06-01 21:41:56.857940 poetry_git_version_plugin-1.0.2/poetry_git_version_plugin/services.py
--rw-r--r--   0        0        0      420 2023-06-01 21:41:56.857940 poetry_git_version_plugin-1.0.2/poetry_git_version_plugin/utils.py
--rw-r--r--   0        0        0     2776 2023-06-01 21:41:56.861940 poetry_git_version_plugin-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     4823 2023-06-01 21:41:56.861940 poetry_git_version_plugin-1.0.2/readme.md
--rw-r--r--   0        0        0     6375 1970-01-01 00:00:00.000000 poetry_git_version_plugin-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-08-02 07:32:58.551387 poetry_git_version_plugin-1.0.3/LICENSE
+-rw-r--r--   0        0        0        0 2023-08-02 07:32:58.655387 poetry_git_version_plugin-1.0.3/poetry_git_version_plugin/__init__.py
+-rw-r--r--   0        0        0      330 2023-08-02 07:32:58.555387 poetry_git_version_plugin-1.0.3/poetry_git_version_plugin/commands.py
+-rw-r--r--   0        0        0     2264 2023-08-02 07:32:58.555387 poetry_git_version_plugin-1.0.3/poetry_git_version_plugin/config.py
+-rw-r--r--   0        0        0      837 2023-08-02 07:32:58.555387 poetry_git_version_plugin-1.0.3/poetry_git_version_plugin/exceptions.py
+-rw-r--r--   0        0        0     1114 2023-08-02 07:32:58.555387 poetry_git_version_plugin-1.0.3/poetry_git_version_plugin/plugins.py
+-rw-r--r--   0        0        0     5882 2023-08-02 07:32:58.555387 poetry_git_version_plugin-1.0.3/poetry_git_version_plugin/services.py
+-rw-r--r--   0        0        0      420 2023-08-02 07:32:58.555387 poetry_git_version_plugin-1.0.3/poetry_git_version_plugin/utils.py
+-rw-r--r--   0        0        0     2776 2023-08-02 07:32:58.555387 poetry_git_version_plugin-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4823 2023-08-02 07:32:58.555387 poetry_git_version_plugin-1.0.3/readme.md
+-rw-r--r--   0        0        0     6375 1970-01-01 00:00:00.000000 poetry_git_version_plugin-1.0.3/PKG-INFO
```

### Comparing `poetry_git_version_plugin-1.0.2/LICENSE` & `poetry_git_version_plugin-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-1.0.2/poetry_git_version_plugin/config.py` & `poetry_git_version_plugin-1.0.3/poetry_git_version_plugin/config.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-1.0.2/poetry_git_version_plugin/exceptions.py` & `poetry_git_version_plugin-1.0.3/poetry_git_version_plugin/exceptions.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-1.0.2/poetry_git_version_plugin/plugins.py` & `poetry_git_version_plugin-1.0.3/poetry_git_version_plugin/plugins.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-1.0.2/poetry_git_version_plugin/services.py` & `poetry_git_version_plugin-1.0.3/poetry_git_version_plugin/services.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-1.0.2/pyproject.toml` & `poetry_git_version_plugin-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-1.0.2/readme.md` & `poetry_git_version_plugin-1.0.3/readme.md`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-1.0.2/PKG-INFO` & `poetry_git_version_plugin-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-git-version-plugin
-Version: 1.0.2
+Version: 1.0.3
 Summary: Poetry plugin to get package version from git
 Home-page: https://gitlab.com/rocshers/python/poetry-git-version-plugin
 License: MIT
 Author: irocshers
 Author-email: develop.iam@rocshers.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```


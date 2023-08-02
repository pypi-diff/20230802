# Comparing `tmp/polywrap_test_cases-0.1.0b2.tar.gz` & `tmp/polywrap_test_cases-0.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_test_cases-0.1.0b2.tar", max compression
+gzip compressed data, was "polywrap_test_cases-0.1.0b3.tar", max compression
```

## Comparing `polywrap_test_cases-0.1.0b2.tar` & `polywrap_test_cases-0.1.0b3.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0       96 2023-06-19 11:17:54.183708 polywrap_test_cases-0.1.0b2/README.md
--rw-r--r--   0        0        0     1257 2023-06-15 11:56:46.981710 polywrap_test_cases-0.1.0b2/polywrap_test_cases/__init__.py
--rw-r--r--   0        0        0      142 2023-06-15 11:56:46.977872 polywrap_test_cases-0.1.0b2/polywrap_test_cases/__main__.py
--rw-r--r--   0        0        0        0 2023-06-15 11:56:46.977757 polywrap_test_cases-0.1.0b2/polywrap_test_cases/py.typed
--rw-r--r--   0        0        0      941 2023-08-02 15:37:23.007110 polywrap_test_cases-0.1.0b2/pyproject.toml
--rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 polywrap_test_cases-0.1.0b2/setup.py
--rw-r--r--   0        0        0      452 1970-01-01 00:00:00.000000 polywrap_test_cases-0.1.0b2/PKG-INFO
+-rw-r--r--   0        0        0       96 2023-08-02 16:06:36.163338 polywrap_test_cases-0.1.0b3/README.md
+-rw-r--r--   0        0        0     1257 2023-08-02 16:06:36.163338 polywrap_test_cases-0.1.0b3/polywrap_test_cases/__init__.py
+-rw-r--r--   0        0        0      142 2023-08-02 16:06:36.163338 polywrap_test_cases-0.1.0b3/polywrap_test_cases/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-02 16:06:36.163338 polywrap_test_cases-0.1.0b3/polywrap_test_cases/py.typed
+-rw-r--r--   0        0        0      941 2023-08-02 16:09:26.414070 polywrap_test_cases-0.1.0b3/pyproject.toml
+-rw-r--r--   0        0        0      452 1970-01-01 00:00:00.000000 polywrap_test_cases-0.1.0b3/PKG-INFO
```

### Comparing `polywrap_test_cases-0.1.0b2/polywrap_test_cases/__init__.py` & `polywrap_test_cases-0.1.0b3/polywrap_test_cases/__init__.py`

 * *Files identical despite different names*

### Comparing `polywrap_test_cases-0.1.0b2/pyproject.toml` & `polywrap_test_cases-0.1.0b3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-test-cases"
-version = "0.1.0b2"
+version = "0.1.0b3"
 description = "Plugin package"
 authors = ["Cesar <cesar@polywrap.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```


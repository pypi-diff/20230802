# Comparing `tmp/textual_dev-1.1.0.tar.gz` & `tmp/textual_dev-1.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textual_dev-1.1.0.tar", max compression
+gzip compressed data, was "textual_dev-1.1.0a1.tar", max compression
```

## Comparing `textual_dev-1.1.0.tar` & `textual_dev-1.1.0a1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1067 2022-10-25 13:47:18.602610 textual_dev-1.1.0/LICENSE
--rw-r--r--   0        0        0      352 2023-08-01 15:24:52.501454 textual_dev-1.1.0/README.md
--rw-r--r--   0        0        0     1719 2023-08-01 16:02:19.684148 textual_dev-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       71 2023-06-27 12:09:27.878115 textual_dev-1.1.0/src/textual_dev/__init__.py
--rw-r--r--   0        0        0       59 2023-06-27 12:09:27.878216 textual_dev-1.1.0/src/textual_dev/__main__.py
--rw-r--r--   0        0        0     6124 2023-06-27 12:09:27.878759 textual_dev-1.1.0/src/textual_dev/cli.py
--rw-r--r--   0        0        0     9776 2023-06-27 12:09:27.878909 textual_dev-1.1.0/src/textual_dev/client.py
--rw-r--r--   0        0        0      246 2023-06-27 12:09:27.879032 textual_dev-1.1.0/src/textual_dev/previews/__init__.py
--rw-r--r--   0        0        0     1815 2023-08-01 15:24:52.502754 textual_dev-1.1.0/src/textual_dev/previews/borders.py
--rw-r--r--   0        0        0     5961 2023-08-01 15:24:52.503029 textual_dev-1.1.0/src/textual_dev/previews/colors.css
--rw-r--r--   0        0        0     2937 2023-08-01 15:24:52.503208 textual_dev-1.1.0/src/textual_dev/previews/colors.py
--rw-r--r--   0        0        0      748 2023-06-27 12:09:27.879871 textual_dev-1.1.0/src/textual_dev/previews/easing.css
--rw-r--r--   0        0        0     3691 2023-06-27 12:09:27.879984 textual_dev-1.1.0/src/textual_dev/previews/easing.py
--rw-r--r--   0        0        0     1861 2023-08-01 15:27:36.609856 textual_dev-1.1.0/src/textual_dev/previews/keys.py
--rw-r--r--   0        0        0        0 2023-06-27 12:09:27.880084 textual_dev-1.1.0/src/textual_dev/py.typed
--rw-r--r--   0        0        0     4278 2023-06-27 12:09:27.880682 textual_dev-1.1.0/src/textual_dev/redirect_output.py
--rw-r--r--   0        0        0     4237 2023-06-27 12:09:27.881448 textual_dev-1.1.0/src/textual_dev/renderables.py
--rw-r--r--   0        0        0     2278 2023-06-27 12:09:27.881594 textual_dev-1.1.0/src/textual_dev/server.py
--rw-r--r--   0        0        0    11068 2023-08-01 15:24:52.503410 textual_dev-1.1.0/src/textual_dev/service.py
--rw-r--r--   0        0        0     4514 2023-06-27 12:09:27.881905 textual_dev-1.1.0/src/textual_dev/tools/diagnose.py
--rw-r--r--   0        0        0     3901 2023-06-27 12:09:27.881987 textual_dev-1.1.0/src/textual_dev/tools/run.py
--rw-r--r--   0        0        0      627 2023-06-27 12:09:27.882134 textual_dev-1.1.0/tests/devtools/__init__.py
--rw-r--r--   0        0        0      776 2023-08-01 15:24:52.503597 textual_dev-1.1.0/tests/devtools/conftest.py
--rw-r--r--   0        0        0     2884 2023-08-01 15:24:52.503778 textual_dev-1.1.0/tests/devtools/test_devtools.py
--rw-r--r--   0        0        0     3723 2023-08-01 15:24:52.503936 textual_dev-1.1.0/tests/devtools/test_devtools_client.py
--rw-r--r--   0        0        0     3721 2023-08-01 15:24:52.504254 textual_dev-1.1.0/tests/devtools/test_redirect_output.py
--rw-r--r--   0        0        0      253 2023-08-01 15:24:52.504413 textual_dev-1.1.0/tests/test_cli.py
--rw-r--r--   0        0        0       46 2023-06-27 12:09:27.882573 textual_dev-1.1.0/tests/utilities/__init__.py
--rw-r--r--   0        0        0     1123 2023-08-01 15:24:52.504707 textual_dev-1.1.0/tests/utilities/wait_for_predicate.py
--rw-r--r--   0        0        0     1802 1970-01-01 00:00:00.000000 textual_dev-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-10-25 13:47:18.602610 textual_dev-1.1.0a1/LICENSE
+-rw-r--r--   0        0        0      352 2023-08-01 15:24:52.501454 textual_dev-1.1.0a1/README.md
+-rw-r--r--   0        0        0     1721 2023-08-01 15:27:36.609518 textual_dev-1.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0       71 2023-06-27 12:09:27.878115 textual_dev-1.1.0a1/src/textual_dev/__init__.py
+-rw-r--r--   0        0        0       59 2023-06-27 12:09:27.878216 textual_dev-1.1.0a1/src/textual_dev/__main__.py
+-rw-r--r--   0        0        0     6124 2023-06-27 12:09:27.878759 textual_dev-1.1.0a1/src/textual_dev/cli.py
+-rw-r--r--   0        0        0     9776 2023-06-27 12:09:27.878909 textual_dev-1.1.0a1/src/textual_dev/client.py
+-rw-r--r--   0        0        0      246 2023-06-27 12:09:27.879032 textual_dev-1.1.0a1/src/textual_dev/previews/__init__.py
+-rw-r--r--   0        0        0     1815 2023-08-01 15:24:52.502754 textual_dev-1.1.0a1/src/textual_dev/previews/borders.py
+-rw-r--r--   0        0        0     5961 2023-08-01 15:24:52.503029 textual_dev-1.1.0a1/src/textual_dev/previews/colors.css
+-rw-r--r--   0        0        0     2937 2023-08-01 15:24:52.503208 textual_dev-1.1.0a1/src/textual_dev/previews/colors.py
+-rw-r--r--   0        0        0      748 2023-06-27 12:09:27.879871 textual_dev-1.1.0a1/src/textual_dev/previews/easing.css
+-rw-r--r--   0        0        0     3691 2023-06-27 12:09:27.879984 textual_dev-1.1.0a1/src/textual_dev/previews/easing.py
+-rw-r--r--   0        0        0     1861 2023-08-01 15:27:36.609856 textual_dev-1.1.0a1/src/textual_dev/previews/keys.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:09:27.880084 textual_dev-1.1.0a1/src/textual_dev/py.typed
+-rw-r--r--   0        0        0     4278 2023-06-27 12:09:27.880682 textual_dev-1.1.0a1/src/textual_dev/redirect_output.py
+-rw-r--r--   0        0        0     4237 2023-06-27 12:09:27.881448 textual_dev-1.1.0a1/src/textual_dev/renderables.py
+-rw-r--r--   0        0        0     2278 2023-06-27 12:09:27.881594 textual_dev-1.1.0a1/src/textual_dev/server.py
+-rw-r--r--   0        0        0    11068 2023-08-01 15:24:52.503410 textual_dev-1.1.0a1/src/textual_dev/service.py
+-rw-r--r--   0        0        0     4514 2023-06-27 12:09:27.881905 textual_dev-1.1.0a1/src/textual_dev/tools/diagnose.py
+-rw-r--r--   0        0        0     3901 2023-06-27 12:09:27.881987 textual_dev-1.1.0a1/src/textual_dev/tools/run.py
+-rw-r--r--   0        0        0      627 2023-06-27 12:09:27.882134 textual_dev-1.1.0a1/tests/devtools/__init__.py
+-rw-r--r--   0        0        0      776 2023-08-01 15:24:52.503597 textual_dev-1.1.0a1/tests/devtools/conftest.py
+-rw-r--r--   0        0        0     2884 2023-08-01 15:24:52.503778 textual_dev-1.1.0a1/tests/devtools/test_devtools.py
+-rw-r--r--   0        0        0     3723 2023-08-01 15:24:52.503936 textual_dev-1.1.0a1/tests/devtools/test_devtools_client.py
+-rw-r--r--   0        0        0     3721 2023-08-01 15:24:52.504254 textual_dev-1.1.0a1/tests/devtools/test_redirect_output.py
+-rw-r--r--   0        0        0      253 2023-08-01 15:24:52.504413 textual_dev-1.1.0a1/tests/test_cli.py
+-rw-r--r--   0        0        0       46 2023-06-27 12:09:27.882573 textual_dev-1.1.0a1/tests/utilities/__init__.py
+-rw-r--r--   0        0        0     1123 2023-08-01 15:24:52.504707 textual_dev-1.1.0a1/tests/utilities/wait_for_predicate.py
+-rw-r--r--   0        0        0     1804 1970-01-01 00:00:00.000000 textual_dev-1.1.0a1/PKG-INFO
```

### Comparing `textual_dev-1.1.0/LICENSE` & `textual_dev-1.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `textual_dev-1.1.0/pyproject.toml` & `textual_dev-1.1.0a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "textual-dev"
-version = "1.1.0"
+version = "1.1.0a1"
 homepage = "https://github.com/Textualize/textual-dev"
 description = "Development tools for working with Textual"
 authors = ["Will McGugan <will@textualize.io>", "Dave Pearson <dave@textualize.io>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `textual_dev-1.1.0/src/textual_dev/cli.py` & `textual_dev-1.1.0a1/src/textual_dev/cli.py`

 * *Files identical despite different names*

### Comparing `textual_dev-1.1.0/src/textual_dev/client.py` & `textual_dev-1.1.0a1/src/textual_dev/client.py`

 * *Files identical despite different names*

### Comparing `textual_dev-1.1.0/src/textual_dev/previews/borders.py` & `textual_dev-1.1.0a1/src/textual_dev/previews/borders.py`

 * *Files identical despite different names*

### Comparing `textual_dev-1.1.0/src/textual_dev/previews/colors.css` & `textual_dev-1.1.0a1/src/textual_dev/previews/colors.css`

 * *Files identical despite different names*

### Comparing `textual_dev-1.1.0/src/textual_dev/previews/colors.py` & `textual_dev-1.1.0a1/src/textual_dev/previews/colors.py`

 * *Files identical despite different names*

### Comparing `textual_dev-1.1.0/src/textual_dev/previews/easing.css` & `textual_dev-1.1.0a1/src/textual_dev/previews/easing.css`

 * *Files identical despite different names*

### Comparing `textual_dev-1.1.0/src/textual_dev/previews/easing.py` & `textual_dev-1.1.0a1/src/textual_dev/previews/easing.py`

 * *Files identical despite different names*

### Comparing `textual_dev-1.1.0/src/textual_dev/previews/keys.py` & `textual_dev-1.1.0a1/src/textual_dev/previews/keys.py`

 * *Files identical despite different names*

### Comparing `textual_dev-1.1.0/src/textual_dev/redirect_output.py` & `textual_dev-1.1.0a1/src/textual_dev/redirect_output.py`

 * *Files identical despite different names*

### Comparing `textual_dev-1.1.0/src/textual_dev/renderables.py` & `textual_dev-1.1.0a1/src/textual_dev/renderables.py`

 * *Files identical despite different names*

### Comparing `textual_dev-1.1.0/src/textual_dev/server.py` & `textual_dev-1.1.0a1/src/textual_dev/server.py`

 * *Files identical despite different names*

### Comparing `textual_dev-1.1.0/src/textual_dev/service.py` & `textual_dev-1.1.0a1/src/textual_dev/service.py`

 * *Files identical despite different names*

### Comparing `textual_dev-1.1.0/src/textual_dev/tools/diagnose.py` & `textual_dev-1.1.0a1/src/textual_dev/tools/diagnose.py`

 * *Files identical despite different names*

### Comparing `textual_dev-1.1.0/src/textual_dev/tools/run.py` & `textual_dev-1.1.0a1/src/textual_dev/tools/run.py`

 * *Files identical despite different names*

### Comparing `textual_dev-1.1.0/tests/devtools/__init__.py` & `textual_dev-1.1.0a1/tests/devtools/__init__.py`

 * *Files identical despite different names*

### Comparing `textual_dev-1.1.0/tests/devtools/conftest.py` & `textual_dev-1.1.0a1/tests/devtools/conftest.py`

 * *Files identical despite different names*

### Comparing `textual_dev-1.1.0/tests/devtools/test_devtools.py` & `textual_dev-1.1.0a1/tests/devtools/test_devtools.py`

 * *Files identical despite different names*

### Comparing `textual_dev-1.1.0/tests/devtools/test_devtools_client.py` & `textual_dev-1.1.0a1/tests/devtools/test_devtools_client.py`

 * *Files identical despite different names*

### Comparing `textual_dev-1.1.0/tests/devtools/test_redirect_output.py` & `textual_dev-1.1.0a1/tests/devtools/test_redirect_output.py`

 * *Files identical despite different names*

### Comparing `textual_dev-1.1.0/tests/utilities/wait_for_predicate.py` & `textual_dev-1.1.0a1/tests/utilities/wait_for_predicate.py`

 * *Files identical despite different names*

### Comparing `textual_dev-1.1.0/PKG-INFO` & `textual_dev-1.1.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-dev
-Version: 1.1.0
+Version: 1.1.0a1
 Summary: Development tools for working with Textual
 Home-page: https://github.com/Textualize/textual-dev
 License: MIT
 Author: Will McGugan
 Author-email: will@textualize.io
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```


# Comparing `tmp/prettynumbers-0.3.6.tar.gz` & `tmp/prettynumbers-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prettynumbers-0.3.6.tar", max compression
+gzip compressed data, was "prettynumbers-0.3.7.tar", max compression
```

## Comparing `prettynumbers-0.3.6.tar` & `prettynumbers-0.3.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    14849 2023-07-26 10:44:02.217744 prettynumbers-0.3.6/LICENSE.txt
--rw-r--r--   0        0        0     1138 2023-07-26 10:44:02.217744 prettynumbers-0.3.6/README.md
--rw-r--r--   0        0        0      138 2023-07-26 10:44:02.217744 prettynumbers-0.3.6/pretty_numbers/__init__.py
--rwxr-xr-x   0        0        0     2405 2023-07-26 10:44:02.221744 prettynumbers-0.3.6/pretty_numbers/pretty_numbers.py
--rw-r--r--   0        0        0        0 2023-07-26 10:44:02.221744 prettynumbers-0.3.6/pretty_numbers/py.typed
--rw-r--r--   0        0        0      807 2023-07-26 10:44:02.221744 prettynumbers-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 prettynumbers-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0    14849 2023-08-02 08:37:00.714126 prettynumbers-0.3.7/LICENSE.txt
+-rw-r--r--   0        0        0     1138 2023-08-02 08:37:00.714126 prettynumbers-0.3.7/README.md
+-rw-r--r--   0        0        0      138 2023-08-02 08:37:00.714126 prettynumbers-0.3.7/pretty_numbers/__init__.py
+-rwxr-xr-x   0        0        0     2405 2023-08-02 08:37:00.714126 prettynumbers-0.3.7/pretty_numbers/pretty_numbers.py
+-rw-r--r--   0        0        0        0 2023-08-02 08:37:00.714126 prettynumbers-0.3.7/pretty_numbers/py.typed
+-rw-r--r--   0        0        0      790 2023-08-02 08:37:00.714126 prettynumbers-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 prettynumbers-0.3.7/PKG-INFO
```

### Comparing `prettynumbers-0.3.6/LICENSE.txt` & `prettynumbers-0.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.3.6/README.md` & `prettynumbers-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.3.6/pretty_numbers/pretty_numbers.py` & `prettynumbers-0.3.7/pretty_numbers/pretty_numbers.py`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.3.6/pyproject.toml` & `prettynumbers-0.3.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prettynumbers"
-version = "0.3.6"
+version = "0.3.7"
 authors = ["gerardk <gerardk@gmail.com>"]
 description="Display a range of numbers in a human readable way"
 license="GNU GENERAL PUBLIC LICENSE"
 packages = [{include = "pretty_numbers"}]
 readme = "README.md"
 repository = "https://github.com/vfxGer/pretty-numbers"
 
@@ -14,15 +14,14 @@
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.17.3"
 isort = "^5.12.0"
 nose = "^1.3.7"
 codecov = "^2.1.12"
 black = "^22.3.0"
 mypy = "^0.910"
-twine = "^3.6.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 82
```

### Comparing `prettynumbers-0.3.6/PKG-INFO` & `prettynumbers-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prettynumbers
-Version: 0.3.6
+Version: 0.3.7
 Summary: Display a range of numbers in a human readable way
 Home-page: https://github.com/vfxGer/pretty-numbers
 License: GNU GENERAL PUBLIC LICENSE
 Author: gerardk
 Author-email: gerardk@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: Other/Proprietary License
```


# Comparing `tmp/pyaddlicense-0.2.3.tar.gz` & `tmp/pyaddlicense-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaddlicense-0.2.3.tar", max compression
+gzip compressed data, was "pyaddlicense-0.3.0.tar", max compression
```

## Comparing `pyaddlicense-0.2.3.tar` & `pyaddlicense-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1066 2023-03-20 17:54:08.972910 pyaddlicense-0.2.3/LICENSE
--rw-r--r--   0        0        0     3158 2023-03-20 17:54:08.973383 pyaddlicense-0.2.3/README.md
--rw-r--r--   0        0        0      609 2023-08-02 06:37:04.486557 pyaddlicense-0.2.3/pyproject.toml
--rw-r--r--   0        0        0       22 2023-03-21 13:04:23.986634 pyaddlicense-0.2.3/src/pyaddlicense/__init__.py
--rw-r--r--   0        0        0    22342 2023-08-01 20:44:12.791541 pyaddlicense-0.2.3/src/pyaddlicense/main.py
--rw-r--r--   0        0        0     3715 1970-01-01 00:00:00.000000 pyaddlicense-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-03-20 17:54:08.972910 pyaddlicense-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3158 2023-03-20 17:54:08.973383 pyaddlicense-0.3.0/README.md
+-rw-r--r--   0        0        0      609 2023-08-01 20:44:47.721490 pyaddlicense-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-03-21 13:04:23.986634 pyaddlicense-0.3.0/src/pyaddlicense/__init__.py
+-rw-r--r--   0        0        0    22342 2023-08-01 20:44:12.791541 pyaddlicense-0.3.0/src/pyaddlicense/main.py
+-rw-r--r--   0        0        0     3715 1970-01-01 00:00:00.000000 pyaddlicense-0.3.0/PKG-INFO
```

### Comparing `pyaddlicense-0.2.3/LICENSE` & `pyaddlicense-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaddlicense-0.2.3/README.md` & `pyaddlicense-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyaddlicense-0.2.3/pyproject.toml` & `pyaddlicense-0.3.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pyaddlicense"
-version = "0.2.3"
+version = "0.3.0"
 description = ""
 authors = ["Mikey Coward <pyaddlicense@kixa.me>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pathspec = ">=0.9.0"
```

### Comparing `pyaddlicense-0.2.3/src/pyaddlicense/main.py` & `pyaddlicense-0.3.0/src/pyaddlicense/main.py`

 * *Files identical despite different names*

### Comparing `pyaddlicense-0.2.3/PKG-INFO` & `pyaddlicense-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaddlicense
-Version: 0.2.3
+Version: 0.3.0
 Summary: 
 Author: Mikey Coward
 Author-email: pyaddlicense@kixa.me
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```


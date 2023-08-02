# Comparing `tmp/python_simple_logger-1.0.5.tar.gz` & `tmp/python_simple_logger-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_simple_logger-1.0.5.tar", max compression
+gzip compressed data, was "python_simple_logger-1.0.6.tar", max compression
```

## Comparing `python_simple_logger-1.0.5.tar` & `python_simple_logger-1.0.6.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-03-30 14:39:49.339828 python_simple_logger-1.0.5/LICENSE
--rw-r--r--   0        0        0      638 2023-03-30 14:39:49.340828 python_simple_logger-1.0.5/README.md
--rw-r--r--   0        0        0      727 2023-03-30 14:39:51.291844 python_simple_logger-1.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-30 14:39:49.341828 python_simple_logger-1.0.5/simple_logger/__init__.py
--rw-r--r--   0        0        0     2805 2023-03-30 14:39:49.341828 python_simple_logger-1.0.5/simple_logger/logger.py
--rw-r--r--   0        0        0     1219 1970-01-01 00:00:00.000000 python_simple_logger-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-02 20:32:58.401713 python_simple_logger-1.0.6/LICENSE
+-rw-r--r--   0        0        0      638 2023-08-02 20:32:58.401713 python_simple_logger-1.0.6/README.md
+-rw-r--r--   0        0        0      656 2023-08-02 20:33:00.339734 python_simple_logger-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-02 20:32:58.402713 python_simple_logger-1.0.6/simple_logger/__init__.py
+-rw-r--r--   0        0        0     2805 2023-08-02 20:32:58.402713 python_simple_logger-1.0.6/simple_logger/logger.py
+-rw-r--r--   0        0        0        0 2023-08-02 20:32:58.403713 python_simple_logger-1.0.6/simple_logger/tests/__init__.py
+-rw-r--r--   0        0        0      539 2023-08-02 20:32:58.403713 python_simple_logger-1.0.6/simple_logger/tests/test_logger.py
+-rw-r--r--   0        0        0     1151 1970-01-01 00:00:00.000000 python_simple_logger-1.0.6/PKG-INFO
```

### Comparing `python_simple_logger-1.0.5/LICENSE` & `python_simple_logger-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python_simple_logger-1.0.5/README.md` & `python_simple_logger-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `python_simple_logger-1.0.5/pyproject.toml` & `python_simple_logger-1.0.6/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 [tool.poetry]
 name = "python-simple-logger"
-version = "1.0.5"
+version = "1.0.6"
 description = "A simple logger for python"
 authors = ["Meni Yakove <myakove@gmail.com>"]
 readme = "README.md"
 packages = [{include = "simple_logger"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 colorlog = "^6.7.0"
-poetry-dynamic-versioning = {extras = ["plugin"], version = "^0.21.4"}
 
 [tool.poetry.group.dev.dependencies]
 ipdb = "^0.13.13"
 ipython = "^8.12.0"
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `python_simple_logger-1.0.5/simple_logger/logger.py` & `python_simple_logger-1.0.6/simple_logger/logger.py`

 * *Files identical despite different names*

### Comparing `python_simple_logger-1.0.5/PKG-INFO` & `python_simple_logger-1.0.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: python-simple-logger
-Version: 1.0.5
+Version: 1.0.6
 Summary: A simple logger for python
 Author: Meni Yakove
 Author-email: myakove@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
-Requires-Dist: poetry-dynamic-versioning[plugin] (>=0.21.4,<0.22.0)
 Description-Content-Type: text/markdown
 
 # Simple Python logger
 
 A simple logger for console/file logging with duplicate logs filter support
 
 ## Release new version
```


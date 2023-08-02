# Comparing `tmp/hypymedia-0.1.3.tar.gz` & `tmp/hypymedia-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypymedia-0.1.3.tar", max compression
+gzip compressed data, was "hypymedia-0.1.4.tar", max compression
```

## Comparing `hypymedia-0.1.3.tar` & `hypymedia-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1065 2023-08-02 02:59:53.232320 hypymedia-0.1.3/LICENSE
--rw-r--r--   0        0        0       11 2023-08-02 02:59:53.232449 hypymedia-0.1.3/README.md
--rw-r--r--   0        0        0       19 2023-08-02 05:38:26.464065 hypymedia-0.1.3/hypymedia/__init__.py
--rw-r--r--   0        0        0     4241 2023-08-02 05:02:07.381365 hypymedia-0.1.3/hypymedia/main.py
--rw-r--r--   0        0        0      565 2023-08-02 05:38:36.053443 hypymedia-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 hypymedia-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-02 02:59:53.232320 hypymedia-0.1.4/LICENSE
+-rw-r--r--   0        0        0       11 2023-08-02 02:59:53.232449 hypymedia-0.1.4/README.md
+-rw-r--r--   0        0        0       20 2023-08-02 05:44:42.287465 hypymedia-0.1.4/hypymedia/__init__.py
+-rw-r--r--   0        0        0     4241 2023-08-02 05:02:07.381365 hypymedia-0.1.4/hypymedia/main.py
+-rw-r--r--   0        0        0      565 2023-08-02 05:44:55.835673 hypymedia-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 hypymedia-0.1.4/PKG-INFO
```

### Comparing `hypymedia-0.1.3/LICENSE` & `hypymedia-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hypymedia-0.1.3/hypymedia/main.py` & `hypymedia-0.1.4/hypymedia/main.py`

 * *Files identical despite different names*

### Comparing `hypymedia-0.1.3/pyproject.toml` & `hypymedia-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hypymedia"
-version = "0.1.3"
+version = "0.1.4"
 description = "HTML creation via Python for HATEOAS applications. #hypermediaFTW"
 authors = ["Tel Stupple <telstupple@gmail.com>"]
 packages = [{ include = "hypymedia" }]
 readme = "README.md"
 
 [tool.poetry.urls]
 "Homepage" = "https://github.com/telboyWA/hypymedia"
```


# Comparing `tmp/hypymedia-0.1.4.tar.gz` & `tmp/hypymedia-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypymedia-0.1.4.tar", max compression
+gzip compressed data, was "hypymedia-0.1.5.tar", max compression
```

## Comparing `hypymedia-0.1.4.tar` & `hypymedia-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1065 2023-08-02 02:59:53.232320 hypymedia-0.1.4/LICENSE
--rw-r--r--   0        0        0       11 2023-08-02 02:59:53.232449 hypymedia-0.1.4/README.md
--rw-r--r--   0        0        0       20 2023-08-02 05:44:42.287465 hypymedia-0.1.4/hypymedia/__init__.py
--rw-r--r--   0        0        0     4241 2023-08-02 05:02:07.381365 hypymedia-0.1.4/hypymedia/main.py
--rw-r--r--   0        0        0      565 2023-08-02 05:44:55.835673 hypymedia-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 hypymedia-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-02 02:59:53.232320 hypymedia-0.1.5/LICENSE
+-rw-r--r--   0        0        0       11 2023-08-02 02:59:53.232449 hypymedia-0.1.5/README.md
+-rw-r--r--   0        0        0       20 2023-08-02 05:44:42.287465 hypymedia-0.1.5/hypymedia/__init__.py
+-rw-r--r--   0        0        0     3353 2023-08-02 05:58:02.089621 hypymedia-0.1.5/hypymedia/main.py
+-rw-r--r--   0        0        0      565 2023-08-02 05:58:10.270369 hypymedia-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 hypymedia-0.1.5/PKG-INFO
```

### Comparing `hypymedia-0.1.4/LICENSE` & `hypymedia-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hypymedia-0.1.4/pyproject.toml` & `hypymedia-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hypymedia"
-version = "0.1.4"
+version = "0.1.5"
 description = "HTML creation via Python for HATEOAS applications. #hypermediaFTW"
 authors = ["Tel Stupple <telstupple@gmail.com>"]
 packages = [{ include = "hypymedia" }]
 readme = "README.md"
 
 [tool.poetry.urls]
 "Homepage" = "https://github.com/telboyWA/hypymedia"
```


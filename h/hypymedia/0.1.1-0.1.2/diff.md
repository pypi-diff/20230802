# Comparing `tmp/hypymedia-0.1.1.tar.gz` & `tmp/hypymedia-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypymedia-0.1.1.tar", max compression
+gzip compressed data, was "hypymedia-0.1.2.tar", max compression
```

## Comparing `hypymedia-0.1.1.tar` & `hypymedia-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1065 2023-08-02 02:59:53.232320 hypymedia-0.1.1/LICENSE
--rw-r--r--   0        0        0       11 2023-08-02 02:59:53.232449 hypymedia-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-08-02 04:05:41.638431 hypymedia-0.1.1/hypymedia/__init__.py
--rw-r--r--   0        0        0     4241 2023-08-02 05:02:07.381365 hypymedia-0.1.1/hypymedia/main.py
--rw-r--r--   0        0        0      618 2023-08-02 05:14:08.208322 hypymedia-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      574 1970-01-01 00:00:00.000000 hypymedia-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-02 02:59:53.232320 hypymedia-0.1.2/LICENSE
+-rw-r--r--   0        0        0       11 2023-08-02 02:59:53.232449 hypymedia-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-08-02 04:05:41.638431 hypymedia-0.1.2/hypymedia/__init__.py
+-rw-r--r--   0        0        0     4241 2023-08-02 05:02:07.381365 hypymedia-0.1.2/hypymedia/main.py
+-rw-r--r--   0        0        0      565 2023-08-02 05:31:43.407120 hypymedia-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 hypymedia-0.1.2/PKG-INFO
```

### Comparing `hypymedia-0.1.1/LICENSE` & `hypymedia-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hypymedia-0.1.1/hypymedia/main.py` & `hypymedia-0.1.2/hypymedia/main.py`

 * *Files identical despite different names*


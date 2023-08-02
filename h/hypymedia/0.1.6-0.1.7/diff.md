# Comparing `tmp/hypymedia-0.1.6.tar.gz` & `tmp/hypymedia-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypymedia-0.1.6.tar", max compression
+gzip compressed data, was "hypymedia-0.1.7.tar", max compression
```

## Comparing `hypymedia-0.1.6.tar` & `hypymedia-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-08-02 02:59:53.232320 hypymedia-0.1.6/LICENSE
--rw-r--r--   0        0        0       11 2023-08-02 02:59:53.232449 hypymedia-0.1.6/README.md
--rw-r--r--   0        0        0     1158 2023-08-02 06:05:47.537815 hypymedia-0.1.6/hypymedia/__init__.py
--rw-r--r--   0        0        0     3353 2023-08-02 05:58:02.089621 hypymedia-0.1.6/hypymedia/main.py
--rw-r--r--   0        0        0      565 2023-08-02 06:06:38.491430 hypymedia-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 hypymedia-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-02 02:59:53.232320 hypymedia-0.1.7/LICENSE
+-rw-r--r--   0        0        0       11 2023-08-02 02:59:53.232449 hypymedia-0.1.7/README.md
+-rw-r--r--   0        0        0     1158 2023-08-02 06:20:00.228959 hypymedia-0.1.7/hypymedia/__init__.py
+-rw-r--r--   0        0        0     1698 2023-08-02 06:19:54.715505 hypymedia-0.1.7/hypymedia/html_list.py
+-rw-r--r--   0        0        0     1159 2023-08-02 06:17:41.396821 hypymedia-0.1.7/hypymedia/main.py
+-rw-r--r--   0        0        0      509 2023-08-02 06:20:54.719314 hypymedia-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 hypymedia-0.1.7/PKG-INFO
```

### Comparing `hypymedia-0.1.6/LICENSE` & `hypymedia-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hypymedia-0.1.6/hypymedia/__init__.py` & `hypymedia-0.1.7/hypymedia/__init__.py`

 * *Files identical despite different names*


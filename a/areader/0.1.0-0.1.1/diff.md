# Comparing `tmp/areader-0.1.0.tar.gz` & `tmp/areader-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "areader-0.1.0.tar", last modified: Wed Aug  2 14:57:50 2023, max compression
+gzip compressed data, was "areader-0.1.1.tar", last modified: Wed Aug  2 15:08:39 2023, max compression
```

## Comparing `areader-0.1.0.tar` & `areader-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      674 2023-08-02 14:57:36.992567 areader-0.1.0/README.md
--rw-r--r--   0        0        0      744 2023-08-02 14:57:50.609775 areader-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-02 14:57:36.992567 areader-0.1.0/src/archive_reader/__init__.py
--rw-r--r--   0        0        0       61 2023-08-02 14:57:36.992567 areader-0.1.0/src/archive_reader/__main__.py
--rw-r--r--   0        0        0     7537 2023-08-02 14:57:36.992567 areader-0.1.0/src/archive_reader/app.py
--rw-r--r--   0        0        0     1165 2023-08-02 14:57:36.992567 areader-0.1.0/src/archive_reader/archiver.css
--rw-r--r--   0        0        0     4469 2023-08-02 14:57:36.996568 areader-0.1.0/src/archive_reader/core.py
--rw-r--r--   0        0        0     1833 2023-08-02 14:57:36.996568 areader-0.1.0/src/archive_reader/hyperkitty.py
--rw-r--r--   0        0        0     4210 2023-08-02 14:57:36.996568 areader-0.1.0/src/archive_reader/models.py
--rw-r--r--   0        0        0     1880 2023-08-02 14:57:36.996568 areader-0.1.0/src/archive_reader/schemas.py
--rw-r--r--   0        0        0     6469 2023-08-02 14:57:36.996568 areader-0.1.0/src/archive_reader/screens.py
--rw-r--r--   0        0        0     6806 2023-08-02 14:57:36.996568 areader-0.1.0/src/archive_reader/widgets.py
--rw-r--r--   0        0        0        0 2023-08-02 14:57:36.996568 areader-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 areader-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1051 2023-08-02 15:08:29.004163 areader-0.1.1/README.md
+-rw-r--r--   0        0        0      744 2023-08-02 15:08:39.920211 areader-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-02 15:08:29.008163 areader-0.1.1/src/archive_reader/__init__.py
+-rw-r--r--   0        0        0       61 2023-08-02 15:08:29.008163 areader-0.1.1/src/archive_reader/__main__.py
+-rw-r--r--   0        0        0     7537 2023-08-02 15:08:29.008163 areader-0.1.1/src/archive_reader/app.py
+-rw-r--r--   0        0        0     1165 2023-08-02 15:08:29.008163 areader-0.1.1/src/archive_reader/archiver.css
+-rw-r--r--   0        0        0     4469 2023-08-02 15:08:29.008163 areader-0.1.1/src/archive_reader/core.py
+-rw-r--r--   0        0        0     1833 2023-08-02 15:08:29.008163 areader-0.1.1/src/archive_reader/hyperkitty.py
+-rw-r--r--   0        0        0     4210 2023-08-02 15:08:29.008163 areader-0.1.1/src/archive_reader/models.py
+-rw-r--r--   0        0        0     1880 2023-08-02 15:08:29.008163 areader-0.1.1/src/archive_reader/schemas.py
+-rw-r--r--   0        0        0     6469 2023-08-02 15:08:29.008163 areader-0.1.1/src/archive_reader/screens.py
+-rw-r--r--   0        0        0     6806 2023-08-02 15:08:29.008163 areader-0.1.1/src/archive_reader/widgets.py
+-rw-r--r--   0        0        0        0 2023-08-02 15:08:29.008163 areader-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     1486 1970-01-01 00:00:00.000000 areader-0.1.1/PKG-INFO
```

### Comparing `areader-0.1.0/pyproject.toml` & `areader-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "areader"
-version = "0.1.0"
+version = "0.1.1"
 description = "Terminal based archives reader for Hyperkitty, GNU Mailman's archiver"
 authors = [
     { name = "Abhilash Raj", email = "raj.abhilash1@gmail.com" },
 ]
 dependencies = [
     "textual>=0.30.0",
     "httpx",
```

### Comparing `areader-0.1.0/src/archive_reader/app.py` & `areader-0.1.1/src/archive_reader/app.py`

 * *Files identical despite different names*

### Comparing `areader-0.1.0/src/archive_reader/archiver.css` & `areader-0.1.1/src/archive_reader/archiver.css`

 * *Files identical despite different names*

### Comparing `areader-0.1.0/src/archive_reader/core.py` & `areader-0.1.1/src/archive_reader/core.py`

 * *Files identical despite different names*

### Comparing `areader-0.1.0/src/archive_reader/hyperkitty.py` & `areader-0.1.1/src/archive_reader/hyperkitty.py`

 * *Files identical despite different names*

### Comparing `areader-0.1.0/src/archive_reader/models.py` & `areader-0.1.1/src/archive_reader/models.py`

 * *Files identical despite different names*

### Comparing `areader-0.1.0/src/archive_reader/schemas.py` & `areader-0.1.1/src/archive_reader/schemas.py`

 * *Files identical despite different names*

### Comparing `areader-0.1.0/src/archive_reader/screens.py` & `areader-0.1.1/src/archive_reader/screens.py`

 * *Files identical despite different names*

### Comparing `areader-0.1.0/src/archive_reader/widgets.py` & `areader-0.1.1/src/archive_reader/widgets.py`

 * *Files identical despite different names*


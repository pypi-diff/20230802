# Comparing `tmp/retakesearch-0.1.22.tar.gz` & `tmp/retakesearch-0.1.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retakesearch-0.1.22.tar", max compression
+gzip compressed data, was "retakesearch-0.1.23.tar", max compression
```

## Comparing `retakesearch-0.1.22.tar` & `retakesearch-0.1.23.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-08-01 23:55:39.956163 retakesearch-0.1.22/README.md
--rw-r--r--   0        0        0      429 2023-08-01 23:55:58.472211 retakesearch-0.1.22/pyproject.toml
--rw-r--r--   0        0        0      174 2023-08-01 23:55:39.956163 retakesearch-0.1.22/retakesearch/__init__.py
--rw-r--r--   0        0        0     1818 2023-08-01 23:55:39.956163 retakesearch-0.1.22/retakesearch/client.py
--rw-r--r--   0        0        0     3687 2023-08-01 23:55:39.956163 retakesearch-0.1.22/retakesearch/index.py
--rw-r--r--   0        0        0      159 2023-08-01 23:55:39.956163 retakesearch-0.1.22/retakesearch/search.py
--rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 retakesearch-0.1.22/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-02 00:18:15.720691 retakesearch-0.1.23/README.md
+-rw-r--r--   0        0        0      429 2023-08-02 00:18:37.364581 retakesearch-0.1.23/pyproject.toml
+-rw-r--r--   0        0        0      174 2023-08-02 00:18:15.720691 retakesearch-0.1.23/retakesearch/__init__.py
+-rw-r--r--   0        0        0     1818 2023-08-02 00:18:15.720691 retakesearch-0.1.23/retakesearch/client.py
+-rw-r--r--   0        0        0     3687 2023-08-02 00:18:15.720691 retakesearch-0.1.23/retakesearch/index.py
+-rw-r--r--   0        0        0      159 2023-08-02 00:18:15.720691 retakesearch-0.1.23/retakesearch/search.py
+-rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 retakesearch-0.1.23/PKG-INFO
```

### Comparing `retakesearch-0.1.22/retakesearch/client.py` & `retakesearch-0.1.23/retakesearch/client.py`

 * *Files identical despite different names*

### Comparing `retakesearch-0.1.22/retakesearch/index.py` & `retakesearch-0.1.23/retakesearch/index.py`

 * *Files identical despite different names*

### Comparing `retakesearch-0.1.22/PKG-INFO` & `retakesearch-0.1.23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retakesearch
-Version: 0.1.22
+Version: 0.1.23
 Summary: Python client for Retake: universal search infra for developers
 Author: Ming Ying
 Author-email: ming.ying.nyc@gmail.com
 Requires-Python: >=3.6,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```


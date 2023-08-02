# Comparing `tmp/piazza-api-0.8.0.tar.gz` & `tmp/piazza-api-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\piazza-api-0.8.0.tar", last modified: Fri Dec 28 04:38:56 2018, max compression
+gzip compressed data, was "dist\piazza-api-0.9.0.tar", last modified: Fri Dec 28 04:43:55 2018, max compression
```

## Comparing `piazza-api-0.8.0.tar` & `piazza-api-0.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2018-12-28 04:38:56.000000 piazza-api-0.8.0/
--rw-rw-rw-   0        0        0       45 2018-12-28 04:34:30.000000 piazza-api-0.8.0/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2018-12-28 04:38:56.000000 piazza-api-0.8.0/piazza_api/
--rw-rw-rw-   0        0        0      288 2018-12-28 04:34:30.000000 piazza-api-0.8.0/piazza_api/exceptions.py
--rw-rw-rw-   0        0        0    11836 2018-12-28 04:34:30.000000 piazza-api-0.8.0/piazza_api/network.py
--rw-rw-rw-   0        0        0     1559 2018-12-28 04:34:30.000000 piazza-api-0.8.0/piazza_api/nonce.py
--rw-rw-rw-   0        0        0     3236 2018-12-28 04:34:30.000000 piazza-api-0.8.0/piazza_api/piazza.py
--rw-rw-rw-   0        0        0    16364 2018-12-28 04:34:30.000000 piazza-api-0.8.0/piazza_api/rpc.py
--rw-rw-rw-   0        0        0       63 2018-12-28 04:34:30.000000 piazza-api-0.8.0/piazza_api/__init__.py
-drwxrwxrwx   0        0        0        0 2018-12-28 04:38:56.000000 piazza-api-0.8.0/piazza_api.egg-info/
--rw-rw-rw-   0        0        0        1 2018-12-28 04:38:55.000000 piazza-api-0.8.0/piazza_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     3997 2018-12-28 04:38:55.000000 piazza-api-0.8.0/piazza_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       13 2018-12-28 04:38:55.000000 piazza-api-0.8.0/piazza_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0      345 2018-12-28 04:38:56.000000 piazza-api-0.8.0/piazza_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       11 2018-12-28 04:38:55.000000 piazza-api-0.8.0/piazza_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3997 2018-12-28 04:38:56.000000 piazza-api-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     2422 2018-12-28 04:34:30.000000 piazza-api-0.8.0/README.md
--rw-rw-rw-   0        0        0       15 2018-12-28 04:34:30.000000 piazza-api-0.8.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2018-12-28 04:38:56.000000 piazza-api-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1548 2018-12-28 04:34:30.000000 piazza-api-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2018-12-28 04:43:55.000000 piazza-api-0.9.0/
+-rw-rw-rw-   0        0        0       45 2018-12-28 04:34:30.000000 piazza-api-0.9.0/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2018-12-28 04:43:55.000000 piazza-api-0.9.0/piazza_api/
+-rw-rw-rw-   0        0        0      288 2018-12-28 04:34:30.000000 piazza-api-0.9.0/piazza_api/exceptions.py
+-rw-rw-rw-   0        0        0    11836 2018-12-28 04:34:30.000000 piazza-api-0.9.0/piazza_api/network.py
+-rw-rw-rw-   0        0        0     1559 2018-12-28 04:34:30.000000 piazza-api-0.9.0/piazza_api/nonce.py
+-rw-rw-rw-   0        0        0     3236 2018-12-28 04:34:30.000000 piazza-api-0.9.0/piazza_api/piazza.py
+-rw-rw-rw-   0        0        0    16364 2018-12-28 04:34:30.000000 piazza-api-0.9.0/piazza_api/rpc.py
+-rw-rw-rw-   0        0        0       63 2018-12-28 04:41:22.000000 piazza-api-0.9.0/piazza_api/__init__.py
+drwxrwxrwx   0        0        0        0 2018-12-28 04:43:55.000000 piazza-api-0.9.0/piazza_api.egg-info/
+-rw-rw-rw-   0        0        0        1 2018-12-28 04:43:54.000000 piazza-api-0.9.0/piazza_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     3997 2018-12-28 04:43:54.000000 piazza-api-0.9.0/piazza_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2018-12-28 04:43:54.000000 piazza-api-0.9.0/piazza_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      345 2018-12-28 04:43:55.000000 piazza-api-0.9.0/piazza_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       11 2018-12-28 04:43:54.000000 piazza-api-0.9.0/piazza_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3997 2018-12-28 04:43:55.000000 piazza-api-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2422 2018-12-28 04:34:30.000000 piazza-api-0.9.0/README.md
+-rw-rw-rw-   0        0        0       15 2018-12-28 04:34:30.000000 piazza-api-0.9.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2018-12-28 04:43:55.000000 piazza-api-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1548 2018-12-28 04:34:30.000000 piazza-api-0.9.0/setup.py
```

### Comparing `piazza-api-0.8.0/piazza_api/network.py` & `piazza-api-0.9.0/piazza_api/network.py`

 * *Files identical despite different names*

### Comparing `piazza-api-0.8.0/piazza_api/nonce.py` & `piazza-api-0.9.0/piazza_api/nonce.py`

 * *Files identical despite different names*

### Comparing `piazza-api-0.8.0/piazza_api/piazza.py` & `piazza-api-0.9.0/piazza_api/piazza.py`

 * *Files identical despite different names*

### Comparing `piazza-api-0.8.0/piazza_api/rpc.py` & `piazza-api-0.9.0/piazza_api/rpc.py`

 * *Files identical despite different names*

### Comparing `piazza-api-0.8.0/piazza_api.egg-info/PKG-INFO` & `piazza-api-0.9.0/piazza_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: piazza-api
-Version: 0.8.0
+Version: 0.9.0
 Summary: Unofficial Client for Piazza's Internal API
 Home-page: http://github.com/hfaran/piazza-api/
 Author: Hamza Faran
 Author-email: UNKNOWN
 License: MIT License
 Description: # piazza-api
```

### Comparing `piazza-api-0.8.0/PKG-INFO` & `piazza-api-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: piazza-api
-Version: 0.8.0
+Version: 0.9.0
 Summary: Unofficial Client for Piazza's Internal API
 Home-page: http://github.com/hfaran/piazza-api/
 Author: Hamza Faran
 Author-email: UNKNOWN
 License: MIT License
 Description: # piazza-api
```

### Comparing `piazza-api-0.8.0/README.md` & `piazza-api-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `piazza-api-0.8.0/setup.py` & `piazza-api-0.9.0/setup.py`

 * *Files identical despite different names*


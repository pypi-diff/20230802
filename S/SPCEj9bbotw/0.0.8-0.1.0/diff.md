# Comparing `tmp/SPCEj9bbotw-0.0.8.tar.gz` & `tmp/SPCEj9bbotw-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPCEj9bbotw-0.0.8.tar", last modified: Wed Aug  2 17:08:42 2023, max compression
+gzip compressed data, was "SPCEj9bbotw-0.1.0.tar", last modified: Wed Aug  2 17:26:39 2023, max compression
```

## Comparing `SPCEj9bbotw-0.0.8.tar` & `SPCEj9bbotw-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 17:08:42.755973 SPCEj9bbotw-0.0.8/
--rw-rw-rw-   0        0        0       58 2023-08-02 17:08:42.754973 SPCEj9bbotw-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-02 17:08:42.737970 SPCEj9bbotw-0.0.8/SPCEj9bbotw.egg-info/
--rw-rw-rw-   0        0        0       58 2023-08-02 17:08:42.000000 SPCEj9bbotw-0.0.8/SPCEj9bbotw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      472 2023-08-02 17:08:42.000000 SPCEj9bbotw-0.0.8/SPCEj9bbotw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 17:08:42.000000 SPCEj9bbotw-0.0.8/SPCEj9bbotw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-08-02 17:08:42.000000 SPCEj9bbotw-0.0.8/SPCEj9bbotw.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-02 17:08:42.743971 SPCEj9bbotw-0.0.8/SPCEj9bbotw_/
--rw-rw-rw-   0        0        0       25 2023-08-02 16:59:55.000000 SPCEj9bbotw-0.0.8/SPCEj9bbotw_/__init__.py
--rw-rw-rw-   0        0        0     2048 2023-08-02 17:07:17.000000 SPCEj9bbotw-0.0.8/SPCEj9bbotw_/_main.py
-drwxrwxrwx   0        0        0        0 2023-08-02 17:08:42.748972 SPCEj9bbotw-0.0.8/SPCEj9bbotw_/functions/
--rw-rw-rw-   0        0        0     3024 2023-08-02 08:32:13.000000 SPCEj9bbotw-0.0.8/SPCEj9bbotw_/functions/_.py
--rw-rw-rw-   0        0        0        0 2023-08-02 17:03:01.000000 SPCEj9bbotw-0.0.8/SPCEj9bbotw_/functions/__init__.py
--rw-rw-rw-   0        0        0     3025 2023-08-02 08:30:42.000000 SPCEj9bbotw-0.0.8/SPCEj9bbotw_/functions/_matrix.py
--rw-rw-rw-   0        0        0     2917 2023-08-02 16:51:39.000000 SPCEj9bbotw-0.0.8/SPCEj9bbotw_/functions/_plot.py
-drwxrwxrwx   0        0        0        0 2023-08-02 17:08:42.753974 SPCEj9bbotw-0.0.8/SPCEj9bbotw_/optimizer/
--rw-rw-rw-   0        0        0       75 2023-08-02 17:06:27.000000 SPCEj9bbotw-0.0.8/SPCEj9bbotw_/optimizer/__init__.py
--rw-rw-rw-   0        0        0     9055 2023-08-02 16:34:50.000000 SPCEj9bbotw-0.0.8/SPCEj9bbotw_/optimizer/kernels.py
--rw-rw-rw-   0        0        0     6764 2023-08-02 10:18:20.000000 SPCEj9bbotw-0.0.8/SPCEj9bbotw_/optimizer/optimizer.py
--rw-rw-rw-   0        0        0     6989 2023-08-02 17:02:05.000000 SPCEj9bbotw-0.0.8/SPCEj9bbotw_/optimizer/optimizer_matrix.py
--rw-rw-rw-   0        0        0       42 2023-08-02 17:08:42.755973 SPCEj9bbotw-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      134 2023-08-02 16:59:18.000000 SPCEj9bbotw-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 17:26:39.996445 SPCEj9bbotw-0.1.0/
+-rw-rw-rw-   0        0        0       58 2023-08-02 17:26:39.995446 SPCEj9bbotw-0.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-02 17:26:39.979442 SPCEj9bbotw-0.1.0/SPCEj9bbotw/
+-rw-rw-rw-   0        0        0       25 2023-08-02 17:23:26.000000 SPCEj9bbotw-0.1.0/SPCEj9bbotw/__init__.py
+-rw-rw-rw-   0        0        0     2048 2023-08-02 17:07:17.000000 SPCEj9bbotw-0.1.0/SPCEj9bbotw/_main.py
+drwxrwxrwx   0        0        0        0 2023-08-02 17:26:39.989444 SPCEj9bbotw-0.1.0/SPCEj9bbotw/functions/
+-rw-rw-rw-   0        0        0     3024 2023-08-02 08:32:13.000000 SPCEj9bbotw-0.1.0/SPCEj9bbotw/functions/_.py
+-rw-rw-rw-   0        0        0        0 2023-08-02 17:03:01.000000 SPCEj9bbotw-0.1.0/SPCEj9bbotw/functions/__init__.py
+-rw-rw-rw-   0        0        0     3025 2023-08-02 08:30:42.000000 SPCEj9bbotw-0.1.0/SPCEj9bbotw/functions/_matrix.py
+-rw-rw-rw-   0        0        0     2917 2023-08-02 16:51:39.000000 SPCEj9bbotw-0.1.0/SPCEj9bbotw/functions/_plot.py
+drwxrwxrwx   0        0        0        0 2023-08-02 17:26:39.994445 SPCEj9bbotw-0.1.0/SPCEj9bbotw/optimizer/
+-rw-rw-rw-   0        0        0       75 2023-08-02 17:06:27.000000 SPCEj9bbotw-0.1.0/SPCEj9bbotw/optimizer/__init__.py
+-rw-rw-rw-   0        0        0     9055 2023-08-02 16:34:50.000000 SPCEj9bbotw-0.1.0/SPCEj9bbotw/optimizer/kernels.py
+-rw-rw-rw-   0        0        0     6764 2023-08-02 10:18:20.000000 SPCEj9bbotw-0.1.0/SPCEj9bbotw/optimizer/optimizer.py
+-rw-rw-rw-   0        0        0     6989 2023-08-02 17:02:05.000000 SPCEj9bbotw-0.1.0/SPCEj9bbotw/optimizer/optimizer_matrix.py
+drwxrwxrwx   0        0        0        0 2023-08-02 17:26:39.985443 SPCEj9bbotw-0.1.0/SPCEj9bbotw.egg-info/
+-rw-rw-rw-   0        0        0       58 2023-08-02 17:26:39.000000 SPCEj9bbotw-0.1.0/SPCEj9bbotw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      462 2023-08-02 17:26:39.000000 SPCEj9bbotw-0.1.0/SPCEj9bbotw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 17:26:39.000000 SPCEj9bbotw-0.1.0/SPCEj9bbotw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-08-02 17:26:39.000000 SPCEj9bbotw-0.1.0/SPCEj9bbotw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 17:26:39.996445 SPCEj9bbotw-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      169 2023-08-02 17:23:19.000000 SPCEj9bbotw-0.1.0/setup.py
```

### Comparing `SPCEj9bbotw-0.0.8/SPCEj9bbotw_/_main.py` & `SPCEj9bbotw-0.1.0/SPCEj9bbotw/_main.py`

 * *Files identical despite different names*

### Comparing `SPCEj9bbotw-0.0.8/SPCEj9bbotw_/functions/_.py` & `SPCEj9bbotw-0.1.0/SPCEj9bbotw/functions/_.py`

 * *Files identical despite different names*

### Comparing `SPCEj9bbotw-0.0.8/SPCEj9bbotw_/functions/_matrix.py` & `SPCEj9bbotw-0.1.0/SPCEj9bbotw/functions/_matrix.py`

 * *Files identical despite different names*

### Comparing `SPCEj9bbotw-0.0.8/SPCEj9bbotw_/functions/_plot.py` & `SPCEj9bbotw-0.1.0/SPCEj9bbotw/functions/_plot.py`

 * *Files identical despite different names*

### Comparing `SPCEj9bbotw-0.0.8/SPCEj9bbotw_/optimizer/kernels.py` & `SPCEj9bbotw-0.1.0/SPCEj9bbotw/optimizer/kernels.py`

 * *Files identical despite different names*

### Comparing `SPCEj9bbotw-0.0.8/SPCEj9bbotw_/optimizer/optimizer.py` & `SPCEj9bbotw-0.1.0/SPCEj9bbotw/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `SPCEj9bbotw-0.0.8/SPCEj9bbotw_/optimizer/optimizer_matrix.py` & `SPCEj9bbotw-0.1.0/SPCEj9bbotw/optimizer/optimizer_matrix.py`

 * *Files identical despite different names*


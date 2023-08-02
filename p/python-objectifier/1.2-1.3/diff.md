# Comparing `tmp/python-objectifier-1.2.tar.gz` & `tmp/python-objectifier-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-objectifier-1.2.tar", last modified: Wed Aug  2 13:01:57 2023, max compression
+gzip compressed data, was "python-objectifier-1.3.tar", last modified: Wed Aug  2 13:15:11 2023, max compression
```

## Comparing `python-objectifier-1.2.tar` & `python-objectifier-1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 13:01:57.682433 python-objectifier-1.2/
--rw-rw-rw-   0        0        0       38 2023-03-02 18:38:58.000000 python-objectifier-1.2/.gitignore
--rw-rw-rw-   0        0        0     2272 2023-08-02 13:01:57.682433 python-objectifier-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1994 2023-03-11 18:35:14.000000 python-objectifier-1.2/README.md
--rw-rw-rw-   0        0        0      285 2023-03-30 16:24:49.000000 python-objectifier-1.2/file.json
-drwxrwxrwx   0        0        0        0 2023-08-02 13:01:57.678437 python-objectifier-1.2/objectifier/
--rw-rw-rw-   0        0        0     1185 2023-08-02 13:01:45.000000 python-objectifier-1.2/objectifier/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 13:01:57.681434 python-objectifier-1.2/python_objectifier.egg-info/
--rw-rw-rw-   0        0        0     2272 2023-08-02 13:01:57.000000 python-objectifier-1.2/python_objectifier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-08-02 13:01:57.000000 python-objectifier-1.2/python_objectifier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 13:01:57.000000 python-objectifier-1.2/python_objectifier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-08-02 13:01:57.000000 python-objectifier-1.2/python_objectifier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-08-02 13:01:57.683433 python-objectifier-1.2/setup.cfg
--rw-rw-rw-   0        0        0      414 2023-08-02 13:01:49.000000 python-objectifier-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 13:15:11.131642 python-objectifier-1.3/
+-rw-rw-rw-   0        0        0       38 2023-03-02 18:38:58.000000 python-objectifier-1.3/.gitignore
+-rw-rw-rw-   0        0        0     2272 2023-08-02 13:15:11.131642 python-objectifier-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1994 2023-03-11 18:35:14.000000 python-objectifier-1.3/README.md
+-rw-rw-rw-   0        0        0      285 2023-03-30 16:24:49.000000 python-objectifier-1.3/file.json
+drwxrwxrwx   0        0        0        0 2023-08-02 13:15:11.127645 python-objectifier-1.3/objectifier/
+-rw-rw-rw-   0        0        0     1185 2023-08-02 13:01:45.000000 python-objectifier-1.3/objectifier/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 13:15:11.130643 python-objectifier-1.3/python_objectifier.egg-info/
+-rw-rw-rw-   0        0        0     2272 2023-08-02 13:15:10.000000 python-objectifier-1.3/python_objectifier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-08-02 13:15:11.000000 python-objectifier-1.3/python_objectifier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 13:15:10.000000 python-objectifier-1.3/python_objectifier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-08-02 13:15:10.000000 python-objectifier-1.3/python_objectifier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-08-02 13:15:11.132641 python-objectifier-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      414 2023-08-02 13:15:08.000000 python-objectifier-1.3/setup.py
```

### Comparing `python-objectifier-1.2/PKG-INFO` & `python-objectifier-1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-objectifier
-Version: 1.2
+Version: 1.3
 Summary: objectifier
 Home-page: https://github.com/xjxckk/python-objectifier/
 Download-URL: https://github.com/xjxckk/python-objectifier/archive/refs/tags/v0.1.tar.gz
 Description-Content-Type: text/markdown
 
 ### objectifier
```

### Comparing `python-objectifier-1.2/README.md` & `python-objectifier-1.3/README.md`

 * *Files identical despite different names*

### Comparing `python-objectifier-1.2/objectifier/__init__.py` & `python-objectifier-1.3/objectifier/__init__.py`

 * *Files identical despite different names*

### Comparing `python-objectifier-1.2/python_objectifier.egg-info/PKG-INFO` & `python-objectifier-1.3/python_objectifier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-objectifier
-Version: 1.2
+Version: 1.3
 Summary: objectifier
 Home-page: https://github.com/xjxckk/python-objectifier/
 Download-URL: https://github.com/xjxckk/python-objectifier/archive/refs/tags/v0.1.tar.gz
 Description-Content-Type: text/markdown
 
 ### objectifier
```


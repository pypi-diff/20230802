# Comparing `tmp/newspaper3k_haystack-0.1.0.tar.gz` & `tmp/newspaper3k_haystack-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newspaper3k_haystack-0.1.0.tar", last modified: Wed Aug  2 17:48:13 2023, max compression
+gzip compressed data, was "newspaper3k_haystack-0.1.1.tar", last modified: Wed Aug  2 18:16:13 2023, max compression
```

## Comparing `newspaper3k_haystack-0.1.0.tar` & `newspaper3k_haystack-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 josepsmachine   (501) staff       (20)        0 2023-08-02 17:48:13.569150 newspaper3k_haystack-0.1.0/
--rw-r--r--   0 josepsmachine   (501) staff       (20)     1074 2023-07-09 18:25:20.000000 newspaper3k_haystack-0.1.0/LICENSE.txt
--rw-r--r--   0 josepsmachine   (501) staff       (20)     9149 2023-08-02 17:48:13.569291 newspaper3k_haystack-0.1.0/PKG-INFO
--rw-r--r--   0 josepsmachine   (501) staff       (20)     8530 2023-07-09 19:09:58.000000 newspaper3k_haystack-0.1.0/README.md
--rw-r--r--   0 josepsmachine   (501) staff       (20)      103 2023-07-09 18:12:13.000000 newspaper3k_haystack-0.1.0/pyproject.toml
--rw-r--r--   0 josepsmachine   (501) staff       (20)      756 2023-08-02 17:48:13.569617 newspaper3k_haystack-0.1.0/setup.cfg
-drwxr-xr-x   0 josepsmachine   (501) staff       (20)        0 2023-08-02 17:48:13.566398 newspaper3k_haystack-0.1.0/src/
-drwxr-xr-x   0 josepsmachine   (501) staff       (20)        0 2023-08-02 17:48:13.568014 newspaper3k_haystack-0.1.0/src/newspaper3k_haystack/
--rw-r--r--   0 josepsmachine   (501) staff       (20)       74 2023-07-09 20:12:23.000000 newspaper3k_haystack-0.1.0/src/newspaper3k_haystack/__init__.py
--rw-r--r--   0 josepsmachine   (501) staff       (20)    10602 2023-08-02 16:56:52.000000 newspaper3k_haystack-0.1.0/src/newspaper3k_haystack/newspaper3k_haystack.py
-drwxr-xr-x   0 josepsmachine   (501) staff       (20)        0 2023-08-02 17:48:13.569039 newspaper3k_haystack-0.1.0/src/newspaper3k_haystack.egg-info/
--rw-r--r--   0 josepsmachine   (501) staff       (20)     9149 2023-08-02 17:48:13.000000 newspaper3k_haystack-0.1.0/src/newspaper3k_haystack.egg-info/PKG-INFO
--rw-r--r--   0 josepsmachine   (501) staff       (20)      371 2023-08-02 17:48:13.000000 newspaper3k_haystack-0.1.0/src/newspaper3k_haystack.egg-info/SOURCES.txt
--rw-r--r--   0 josepsmachine   (501) staff       (20)        1 2023-08-02 17:48:13.000000 newspaper3k_haystack-0.1.0/src/newspaper3k_haystack.egg-info/dependency_links.txt
--rw-r--r--   0 josepsmachine   (501) staff       (20)       46 2023-08-02 17:48:13.000000 newspaper3k_haystack-0.1.0/src/newspaper3k_haystack.egg-info/requires.txt
--rw-r--r--   0 josepsmachine   (501) staff       (20)       21 2023-08-02 17:48:13.000000 newspaper3k_haystack-0.1.0/src/newspaper3k_haystack.egg-info/top_level.txt
+drwxr-xr-x   0 josepsmachine   (501) staff       (20)        0 2023-08-02 18:16:13.522856 newspaper3k_haystack-0.1.1/
+-rw-r--r--   0 josepsmachine   (501) staff       (20)     1074 2023-07-09 18:25:20.000000 newspaper3k_haystack-0.1.1/LICENSE.txt
+-rw-r--r--   0 josepsmachine   (501) staff       (20)     9149 2023-08-02 18:16:13.522941 newspaper3k_haystack-0.1.1/PKG-INFO
+-rw-r--r--   0 josepsmachine   (501) staff       (20)     8530 2023-07-09 19:09:58.000000 newspaper3k_haystack-0.1.1/README.md
+-rw-r--r--   0 josepsmachine   (501) staff       (20)      103 2023-07-09 18:12:13.000000 newspaper3k_haystack-0.1.1/pyproject.toml
+-rw-r--r--   0 josepsmachine   (501) staff       (20)      756 2023-08-02 18:16:13.523286 newspaper3k_haystack-0.1.1/setup.cfg
+drwxr-xr-x   0 josepsmachine   (501) staff       (20)        0 2023-08-02 18:16:13.520357 newspaper3k_haystack-0.1.1/src/
+drwxr-xr-x   0 josepsmachine   (501) staff       (20)        0 2023-08-02 18:16:13.521636 newspaper3k_haystack-0.1.1/src/newspaper3k_haystack/
+-rw-r--r--   0 josepsmachine   (501) staff       (20)       74 2023-07-09 20:12:23.000000 newspaper3k_haystack-0.1.1/src/newspaper3k_haystack/__init__.py
+-rw-r--r--   0 josepsmachine   (501) staff       (20)    21410 2023-08-02 18:12:59.000000 newspaper3k_haystack-0.1.1/src/newspaper3k_haystack/newspaper3k_haystack.py
+drwxr-xr-x   0 josepsmachine   (501) staff       (20)        0 2023-08-02 18:16:13.522742 newspaper3k_haystack-0.1.1/src/newspaper3k_haystack.egg-info/
+-rw-r--r--   0 josepsmachine   (501) staff       (20)     9149 2023-08-02 18:16:13.000000 newspaper3k_haystack-0.1.1/src/newspaper3k_haystack.egg-info/PKG-INFO
+-rw-r--r--   0 josepsmachine   (501) staff       (20)      371 2023-08-02 18:16:13.000000 newspaper3k_haystack-0.1.1/src/newspaper3k_haystack.egg-info/SOURCES.txt
+-rw-r--r--   0 josepsmachine   (501) staff       (20)        1 2023-08-02 18:16:13.000000 newspaper3k_haystack-0.1.1/src/newspaper3k_haystack.egg-info/dependency_links.txt
+-rw-r--r--   0 josepsmachine   (501) staff       (20)       46 2023-08-02 18:16:13.000000 newspaper3k_haystack-0.1.1/src/newspaper3k_haystack.egg-info/requires.txt
+-rw-r--r--   0 josepsmachine   (501) staff       (20)       21 2023-08-02 18:16:13.000000 newspaper3k_haystack-0.1.1/src/newspaper3k_haystack.egg-info/top_level.txt
```

### Comparing `newspaper3k_haystack-0.1.0/LICENSE.txt` & `newspaper3k_haystack-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `newspaper3k_haystack-0.1.0/PKG-INFO` & `newspaper3k_haystack-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newspaper3k_haystack
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple newspaper3k haystack node wrapper. A node for scraping articles given a link and a crawler.
 Home-page: https://github.com/Haradai/newspaper3k_haystack
 Author: Josep Maria Rocafort
 Author-email: josem.rocafortf@gmail.com
 Project-URL: Bug Tracker, https://github.com/Haradai/newspaper3k_haystack/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `newspaper3k_haystack-0.1.0/README.md` & `newspaper3k_haystack-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `newspaper3k_haystack-0.1.0/setup.cfg` & `newspaper3k_haystack-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = newspaper3k_haystack
-version = 0.1.0
+version = 0.1.1
 author = Josep Maria Rocafort
 author_email = josem.rocafortf@gmail.com
 description = A simple newspaper3k haystack node wrapper. A node for scraping articles given a link and a crawler.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Haradai/newspaper3k_haystack
 project_urls =
```

### Comparing `newspaper3k_haystack-0.1.0/src/newspaper3k_haystack.egg-info/PKG-INFO` & `newspaper3k_haystack-0.1.1/src/newspaper3k_haystack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newspaper3k-haystack
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple newspaper3k haystack node wrapper. A node for scraping articles given a link and a crawler.
 Home-page: https://github.com/Haradai/newspaper3k_haystack
 Author: Josep Maria Rocafort
 Author-email: josem.rocafortf@gmail.com
 Project-URL: Bug Tracker, https://github.com/Haradai/newspaper3k_haystack/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```


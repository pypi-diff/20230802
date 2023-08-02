# Comparing `tmp/resotometrics-3.6.4.tar.gz` & `tmp/resotometrics-3.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotometrics-3.6.4.tar", last modified: Mon Jul 24 18:35:04 2023, max compression
+gzip compressed data, was "resotometrics-3.6.5.tar", last modified: Wed Aug  2 19:21:13 2023, max compression
```

## Comparing `resotometrics-3.6.4.tar` & `resotometrics-3.6.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:04.532129 resotometrics-3.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-24 18:31:03.000000 resotometrics-3.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-07-24 18:35:04.532129 resotometrics-3.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-07-24 18:31:03.000000 resotometrics-3.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-24 18:31:03.000000 resotometrics-3.6.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:04.528129 resotometrics-3.6.4/resotometrics/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-24 18:31:03.000000 resotometrics-3.6.4/resotometrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-07-24 18:31:03.000000 resotometrics-3.6.4/resotometrics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-24 18:31:03.000000 resotometrics-3.6.4/resotometrics/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-07-24 18:31:03.000000 resotometrics-3.6.4/resotometrics/default_metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-24 18:31:03.000000 resotometrics-3.6.4/resotometrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-24 18:31:03.000000 resotometrics-3.6.4/resotometrics/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:04.532129 resotometrics-3.6.4/resotometrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-07-24 18:35:04.000000 resotometrics-3.6.4/resotometrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-24 18:35:04.000000 resotometrics-3.6.4/resotometrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:35:04.000000 resotometrics-3.6.4/resotometrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-24 18:35:04.000000 resotometrics-3.6.4/resotometrics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:32:38.000000 resotometrics-3.6.4/resotometrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-24 18:35:04.000000 resotometrics-3.6.4/resotometrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-24 18:35:04.000000 resotometrics-3.6.4/resotometrics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 18:35:04.536130 resotometrics-3.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:04.532129 resotometrics-3.6.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-24 18:31:03.000000 resotometrics-3.6.4/test/test_args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:21:13.256527 resotometrics-3.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-02 19:17:24.000000 resotometrics-3.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-08-02 19:21:13.256527 resotometrics-3.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-08-02 19:17:24.000000 resotometrics-3.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-08-02 19:17:24.000000 resotometrics-3.6.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:21:13.256527 resotometrics-3.6.5/resotometrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-02 19:17:24.000000 resotometrics-3.6.5/resotometrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-08-02 19:17:24.000000 resotometrics-3.6.5/resotometrics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-08-02 19:17:24.000000 resotometrics-3.6.5/resotometrics/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-08-02 19:17:24.000000 resotometrics-3.6.5/resotometrics/default_metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-02 19:17:24.000000 resotometrics-3.6.5/resotometrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-02 19:17:24.000000 resotometrics-3.6.5/resotometrics/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:21:13.256527 resotometrics-3.6.5/resotometrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-08-02 19:21:13.000000 resotometrics-3.6.5/resotometrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-02 19:21:13.000000 resotometrics-3.6.5/resotometrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:21:13.000000 resotometrics-3.6.5/resotometrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-02 19:21:13.000000 resotometrics-3.6.5/resotometrics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:18:53.000000 resotometrics-3.6.5/resotometrics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-02 19:21:13.000000 resotometrics-3.6.5/resotometrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-02 19:21:13.000000 resotometrics-3.6.5/resotometrics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-02 19:21:13.256527 resotometrics-3.6.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:21:13.256527 resotometrics-3.6.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-02 19:17:24.000000 resotometrics-3.6.5/test/test_args.py
```

### Comparing `resotometrics-3.6.4/PKG-INFO` & `resotometrics-3.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotometrics
-Version: 3.6.4
+Version: 3.6.5
 Summary: Exports Resoto metrics in Prometheus format.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotometrics
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resotometrics-3.6.4/README.md` & `resotometrics-3.6.5/README.md`

 * *Files identical despite different names*

### Comparing `resotometrics-3.6.4/pyproject.toml` & `resotometrics-3.6.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resotometrics"
-version = "3.6.4"
+version = "3.6.5"
 authors = [{name="Some Engineering Inc."}]
 description = "Exports Resoto metrics in Prometheus format."
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
@@ -23,15 +23,15 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.6.4"
+    "resotolib==3.6.5"
 ]
 
 [pyproject.optional-dependencies]
 test = ["pytest"]
 
 [project.scripts]
 resotometrics = "resotometrics.__main__:main"
```

### Comparing `resotometrics-3.6.4/resotometrics/__main__.py` & `resotometrics-3.6.5/resotometrics/__main__.py`

 * *Files identical despite different names*

### Comparing `resotometrics-3.6.4/resotometrics/config.py` & `resotometrics-3.6.5/resotometrics/config.py`

 * *Files identical despite different names*

### Comparing `resotometrics-3.6.4/resotometrics/default_metrics.yaml` & `resotometrics-3.6.5/resotometrics/default_metrics.yaml`

 * *Files identical despite different names*

### Comparing `resotometrics-3.6.4/resotometrics/metrics.py` & `resotometrics-3.6.5/resotometrics/metrics.py`

 * *Files identical despite different names*

### Comparing `resotometrics-3.6.4/resotometrics/search.py` & `resotometrics-3.6.5/resotometrics/search.py`

 * *Files identical despite different names*

### Comparing `resotometrics-3.6.4/resotometrics.egg-info/PKG-INFO` & `resotometrics-3.6.5/resotometrics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotometrics
-Version: 3.6.4
+Version: 3.6.5
 Summary: Exports Resoto metrics in Prometheus format.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotometrics
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resotometrics-3.6.4/test/test_args.py` & `resotometrics-3.6.5/test/test_args.py`

 * *Files identical despite different names*


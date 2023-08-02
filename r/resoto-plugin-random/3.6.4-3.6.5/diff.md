# Comparing `tmp/resoto-plugin-random-3.6.4.tar.gz` & `tmp/resoto-plugin-random-3.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-random-3.6.4.tar", last modified: Mon Jul 24 18:28:29 2023, max compression
+gzip compressed data, was "resoto-plugin-random-3.6.5.tar", last modified: Wed Aug  2 19:22:46 2023, max compression
```

## Comparing `resoto-plugin-random-3.6.4.tar` & `resoto-plugin-random-3.6.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:28:29.774829 resoto-plugin-random-3.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 18:23:51.000000 resoto-plugin-random-3.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-24 18:28:29.774829 resoto-plugin-random-3.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-24 18:23:51.000000 resoto-plugin-random-3.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-24 18:23:51.000000 resoto-plugin-random-3.6.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:28:29.774829 resoto-plugin-random-3.6.4/resoto_plugin_random/
--rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-07-24 18:23:51.000000 resoto-plugin-random-3.6.4/resoto_plugin_random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-24 18:23:51.000000 resoto-plugin-random-3.6.4/resoto_plugin_random/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-07-24 18:23:51.000000 resoto-plugin-random-3.6.4/resoto_plugin_random/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:28:29.774829 resoto-plugin-random-3.6.4/resoto_plugin_random.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-24 18:28:29.000000 resoto-plugin-random-3.6.4/resoto_plugin_random.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-24 18:28:29.000000 resoto-plugin-random-3.6.4/resoto_plugin_random.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:28:29.000000 resoto-plugin-random-3.6.4/resoto_plugin_random.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-24 18:28:29.000000 resoto-plugin-random-3.6.4/resoto_plugin_random.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:25:40.000000 resoto-plugin-random-3.6.4/resoto_plugin_random.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-24 18:28:29.000000 resoto-plugin-random-3.6.4/resoto_plugin_random.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-24 18:28:29.000000 resoto-plugin-random-3.6.4/resoto_plugin_random.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 18:28:29.778830 resoto-plugin-random-3.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:28:29.774829 resoto-plugin-random-3.6.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-24 18:23:51.000000 resoto-plugin-random-3.6.4/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:46.403368 resoto-plugin-random-3.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 19:17:25.000000 resoto-plugin-random-3.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-08-02 19:22:46.403368 resoto-plugin-random-3.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-02 19:17:25.000000 resoto-plugin-random-3.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-08-02 19:17:25.000000 resoto-plugin-random-3.6.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:46.403368 resoto-plugin-random-3.6.5/resoto_plugin_random/
+-rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-08-02 19:17:25.000000 resoto-plugin-random-3.6.5/resoto_plugin_random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-02 19:17:25.000000 resoto-plugin-random-3.6.5/resoto_plugin_random/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-08-02 19:17:25.000000 resoto-plugin-random-3.6.5/resoto_plugin_random/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:46.403368 resoto-plugin-random-3.6.5/resoto_plugin_random.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-08-02 19:22:46.000000 resoto-plugin-random-3.6.5/resoto_plugin_random.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-08-02 19:22:46.000000 resoto-plugin-random-3.6.5/resoto_plugin_random.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:22:46.000000 resoto-plugin-random-3.6.5/resoto_plugin_random.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-02 19:22:46.000000 resoto-plugin-random-3.6.5/resoto_plugin_random.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:19:26.000000 resoto-plugin-random-3.6.5/resoto_plugin_random.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-02 19:22:46.000000 resoto-plugin-random-3.6.5/resoto_plugin_random.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 19:22:46.000000 resoto-plugin-random-3.6.5/resoto_plugin_random.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-02 19:22:46.403368 resoto-plugin-random-3.6.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:46.403368 resoto-plugin-random-3.6.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-02 19:17:25.000000 resoto-plugin-random-3.6.5/test/test_config.py
```

### Comparing `resoto-plugin-random-3.6.4/PKG-INFO` & `resoto-plugin-random-3.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-random
-Version: 3.6.4
+Version: 3.6.5
 Summary: Resoto Random Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/random
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-random-3.6.4/README.md` & `resoto-plugin-random-3.6.5/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-random-3.6.4/pyproject.toml` & `resoto-plugin-random-3.6.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-random"
 description = "Resoto Random Collector Plugin"
-version = "3.6.4"
+version = "3.6.5"
 authors = [{name="Some Engineering Inc."}]
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
     # Audience
@@ -23,15 +23,15 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.6.4",
+    "resotolib==3.6.5",
 ]
 
 [project.entry-points."resoto.plugins"]
 random = "resoto_plugin_random:RandomCollectorPlugin"
 
 [project.urls]
 Documentation = "https://resoto.com"
```

### Comparing `resoto-plugin-random-3.6.4/resoto_plugin_random/__init__.py` & `resoto-plugin-random-3.6.5/resoto_plugin_random/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-random-3.6.4/resoto_plugin_random/resources.py` & `resoto-plugin-random-3.6.5/resoto_plugin_random/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-random-3.6.4/resoto_plugin_random.egg-info/PKG-INFO` & `resoto-plugin-random-3.6.5/resoto_plugin_random.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-random
-Version: 3.6.4
+Version: 3.6.5
 Summary: Resoto Random Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/random
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```


# Comparing `tmp/resoto-plugin-dockerhub-3.6.4.tar.gz` & `tmp/resoto-plugin-dockerhub-3.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-dockerhub-3.6.4.tar", last modified: Mon Jul 24 18:34:41 2023, max compression
+gzip compressed data, was "resoto-plugin-dockerhub-3.6.5.tar", last modified: Wed Aug  2 19:26:35 2023, max compression
```

## Comparing `resoto-plugin-dockerhub-3.6.4.tar` & `resoto-plugin-dockerhub-3.6.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:34:41.204315 resoto-plugin-dockerhub-3.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 18:29:56.000000 resoto-plugin-dockerhub-3.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-24 18:34:41.204315 resoto-plugin-dockerhub-3.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-24 18:29:56.000000 resoto-plugin-dockerhub-3.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-24 18:29:56.000000 resoto-plugin-dockerhub-3.6.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:34:41.204315 resoto-plugin-dockerhub-3.6.4/resoto_plugin_dockerhub/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-24 18:29:56.000000 resoto-plugin-dockerhub-3.6.4/resoto_plugin_dockerhub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-24 18:29:56.000000 resoto-plugin-dockerhub-3.6.4/resoto_plugin_dockerhub/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-24 18:29:56.000000 resoto-plugin-dockerhub-3.6.4/resoto_plugin_dockerhub/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:34:41.204315 resoto-plugin-dockerhub-3.6.4/resoto_plugin_dockerhub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-24 18:34:41.000000 resoto-plugin-dockerhub-3.6.4/resoto_plugin_dockerhub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-24 18:34:41.000000 resoto-plugin-dockerhub-3.6.4/resoto_plugin_dockerhub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:34:41.000000 resoto-plugin-dockerhub-3.6.4/resoto_plugin_dockerhub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-24 18:34:41.000000 resoto-plugin-dockerhub-3.6.4/resoto_plugin_dockerhub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:31:45.000000 resoto-plugin-dockerhub-3.6.4/resoto_plugin_dockerhub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 18:34:41.000000 resoto-plugin-dockerhub-3.6.4/resoto_plugin_dockerhub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 18:34:41.000000 resoto-plugin-dockerhub-3.6.4/resoto_plugin_dockerhub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 18:34:41.204315 resoto-plugin-dockerhub-3.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:34:41.204315 resoto-plugin-dockerhub-3.6.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 18:29:56.000000 resoto-plugin-dockerhub-3.6.4/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:26:35.379704 resoto-plugin-dockerhub-3.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 19:22:29.000000 resoto-plugin-dockerhub-3.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-08-02 19:26:35.379704 resoto-plugin-dockerhub-3.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-08-02 19:22:29.000000 resoto-plugin-dockerhub-3.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-08-02 19:22:29.000000 resoto-plugin-dockerhub-3.6.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:26:35.379704 resoto-plugin-dockerhub-3.6.5/resoto_plugin_dockerhub/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-08-02 19:22:29.000000 resoto-plugin-dockerhub-3.6.5/resoto_plugin_dockerhub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-08-02 19:22:29.000000 resoto-plugin-dockerhub-3.6.5/resoto_plugin_dockerhub/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-08-02 19:22:29.000000 resoto-plugin-dockerhub-3.6.5/resoto_plugin_dockerhub/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:26:35.379704 resoto-plugin-dockerhub-3.6.5/resoto_plugin_dockerhub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-08-02 19:26:35.000000 resoto-plugin-dockerhub-3.6.5/resoto_plugin_dockerhub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-02 19:26:35.000000 resoto-plugin-dockerhub-3.6.5/resoto_plugin_dockerhub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:26:35.000000 resoto-plugin-dockerhub-3.6.5/resoto_plugin_dockerhub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-02 19:26:35.000000 resoto-plugin-dockerhub-3.6.5/resoto_plugin_dockerhub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:24:03.000000 resoto-plugin-dockerhub-3.6.5/resoto_plugin_dockerhub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 19:26:35.000000 resoto-plugin-dockerhub-3.6.5/resoto_plugin_dockerhub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 19:26:35.000000 resoto-plugin-dockerhub-3.6.5/resoto_plugin_dockerhub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-02 19:26:35.379704 resoto-plugin-dockerhub-3.6.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:26:35.379704 resoto-plugin-dockerhub-3.6.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-08-02 19:22:29.000000 resoto-plugin-dockerhub-3.6.5/test/test_config.py
```

### Comparing `resoto-plugin-dockerhub-3.6.4/PKG-INFO` & `resoto-plugin-dockerhub-3.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-dockerhub
-Version: 3.6.4
+Version: 3.6.5
 Summary: Resoto Docker Hub Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/dockerhub
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-dockerhub-3.6.4/README.md` & `resoto-plugin-dockerhub-3.6.5/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-dockerhub-3.6.4/pyproject.toml` & `resoto-plugin-dockerhub-3.6.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-dockerhub"
 description = "Resoto Docker Hub Collector Plugin"
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
     "requests",
 
 ]
 
 [project.entry-points."resoto.plugins"]
 dockerhub = "resoto_plugin_dockerhub:DockerHubCollectorPlugin"
```

### Comparing `resoto-plugin-dockerhub-3.6.4/resoto_plugin_dockerhub/__init__.py` & `resoto-plugin-dockerhub-3.6.5/resoto_plugin_dockerhub/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-dockerhub-3.6.4/resoto_plugin_dockerhub/resources.py` & `resoto-plugin-dockerhub-3.6.5/resoto_plugin_dockerhub/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-dockerhub-3.6.4/resoto_plugin_dockerhub.egg-info/PKG-INFO` & `resoto-plugin-dockerhub-3.6.5/resoto_plugin_dockerhub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-dockerhub
-Version: 3.6.4
+Version: 3.6.5
 Summary: Resoto Docker Hub Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/dockerhub
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```


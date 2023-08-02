# Comparing `tmp/resoto-plugin-cleanup-untagged-3.6.4.tar.gz` & `tmp/resoto-plugin-cleanup-untagged-3.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-cleanup-untagged-3.6.4.tar", last modified: Mon Jul 24 18:34:05 2023, max compression
+gzip compressed data, was "resoto-plugin-cleanup-untagged-3.6.5.tar", last modified: Wed Aug  2 19:21:34 2023, max compression
```

## Comparing `resoto-plugin-cleanup-untagged-3.6.4.tar` & `resoto-plugin-cleanup-untagged-3.6.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:34:05.879588 resoto-plugin-cleanup-untagged-3.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 18:29:08.000000 resoto-plugin-cleanup-untagged-3.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-24 18:34:05.879588 resoto-plugin-cleanup-untagged-3.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-24 18:29:08.000000 resoto-plugin-cleanup-untagged-3.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-24 18:29:08.000000 resoto-plugin-cleanup-untagged-3.6.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:34:05.879588 resoto-plugin-cleanup-untagged-3.6.4/resoto_plugin_cleanup_untagged/
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-24 18:29:08.000000 resoto-plugin-cleanup-untagged-3.6.4/resoto_plugin_cleanup_untagged/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-24 18:29:08.000000 resoto-plugin-cleanup-untagged-3.6.4/resoto_plugin_cleanup_untagged/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:34:05.879588 resoto-plugin-cleanup-untagged-3.6.4/resoto_plugin_cleanup_untagged.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-24 18:34:05.000000 resoto-plugin-cleanup-untagged-3.6.4/resoto_plugin_cleanup_untagged.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-24 18:34:05.000000 resoto-plugin-cleanup-untagged-3.6.4/resoto_plugin_cleanup_untagged.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:34:05.000000 resoto-plugin-cleanup-untagged-3.6.4/resoto_plugin_cleanup_untagged.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-24 18:34:05.000000 resoto-plugin-cleanup-untagged-3.6.4/resoto_plugin_cleanup_untagged.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:30:39.000000 resoto-plugin-cleanup-untagged-3.6.4/resoto_plugin_cleanup_untagged.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-24 18:34:05.000000 resoto-plugin-cleanup-untagged-3.6.4/resoto_plugin_cleanup_untagged.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 18:34:05.000000 resoto-plugin-cleanup-untagged-3.6.4/resoto_plugin_cleanup_untagged.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 18:34:05.879588 resoto-plugin-cleanup-untagged-3.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:34:05.879588 resoto-plugin-cleanup-untagged-3.6.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-24 18:29:08.000000 resoto-plugin-cleanup-untagged-3.6.4/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:21:34.840492 resoto-plugin-cleanup-untagged-3.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 19:17:00.000000 resoto-plugin-cleanup-untagged-3.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-08-02 19:21:34.840492 resoto-plugin-cleanup-untagged-3.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-02 19:17:00.000000 resoto-plugin-cleanup-untagged-3.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-02 19:17:00.000000 resoto-plugin-cleanup-untagged-3.6.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:21:34.840492 resoto-plugin-cleanup-untagged-3.6.5/resoto_plugin_cleanup_untagged/
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-08-02 19:17:00.000000 resoto-plugin-cleanup-untagged-3.6.5/resoto_plugin_cleanup_untagged/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-08-02 19:17:00.000000 resoto-plugin-cleanup-untagged-3.6.5/resoto_plugin_cleanup_untagged/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:21:34.840492 resoto-plugin-cleanup-untagged-3.6.5/resoto_plugin_cleanup_untagged.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-08-02 19:21:34.000000 resoto-plugin-cleanup-untagged-3.6.5/resoto_plugin_cleanup_untagged.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-08-02 19:21:34.000000 resoto-plugin-cleanup-untagged-3.6.5/resoto_plugin_cleanup_untagged.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:21:34.000000 resoto-plugin-cleanup-untagged-3.6.5/resoto_plugin_cleanup_untagged.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-02 19:21:34.000000 resoto-plugin-cleanup-untagged-3.6.5/resoto_plugin_cleanup_untagged.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:18:21.000000 resoto-plugin-cleanup-untagged-3.6.5/resoto_plugin_cleanup_untagged.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-02 19:21:34.000000 resoto-plugin-cleanup-untagged-3.6.5/resoto_plugin_cleanup_untagged.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 19:21:34.000000 resoto-plugin-cleanup-untagged-3.6.5/resoto_plugin_cleanup_untagged.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-02 19:21:34.840492 resoto-plugin-cleanup-untagged-3.6.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:21:34.840492 resoto-plugin-cleanup-untagged-3.6.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-08-02 19:17:00.000000 resoto-plugin-cleanup-untagged-3.6.5/test/test_config.py
```

### Comparing `resoto-plugin-cleanup-untagged-3.6.4/PKG-INFO` & `resoto-plugin-cleanup-untagged-3.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-untagged
-Version: 3.6.4
+Version: 3.6.5
 Summary: Resoto Cleanup Untagged Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_untagged
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-untagged-3.6.4/README.md` & `resoto-plugin-cleanup-untagged-3.6.5/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-untagged-3.6.4/pyproject.toml` & `resoto-plugin-cleanup-untagged-3.6.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-cleanup-untagged"
 description = "Resoto Cleanup Untagged Plugin"
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
 cleanup_untagged = "resoto_plugin_cleanup_untagged:CleanupUntaggedPlugin"
 
 [project.urls]
 Documentation = "https://resoto.com"
```

### Comparing `resoto-plugin-cleanup-untagged-3.6.4/resoto_plugin_cleanup_untagged/__init__.py` & `resoto-plugin-cleanup-untagged-3.6.5/resoto_plugin_cleanup_untagged/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-untagged-3.6.4/resoto_plugin_cleanup_untagged/config.py` & `resoto-plugin-cleanup-untagged-3.6.5/resoto_plugin_cleanup_untagged/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-untagged-3.6.4/resoto_plugin_cleanup_untagged.egg-info/PKG-INFO` & `resoto-plugin-cleanup-untagged-3.6.5/resoto_plugin_cleanup_untagged.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-untagged
-Version: 3.6.4
+Version: 3.6.5
 Summary: Resoto Cleanup Untagged Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_untagged
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-untagged-3.6.4/resoto_plugin_cleanup_untagged.egg-info/SOURCES.txt` & `resoto-plugin-cleanup-untagged-3.6.5/resoto_plugin_cleanup_untagged.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-untagged-3.6.4/test/test_config.py` & `resoto-plugin-cleanup-untagged-3.6.5/test/test_config.py`

 * *Files identical despite different names*


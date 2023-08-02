# Comparing `tmp/resoto-plugin-protector-3.6.4.tar.gz` & `tmp/resoto-plugin-protector-3.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-protector-3.6.4.tar", last modified: Mon Jul 24 18:31:46 2023, max compression
+gzip compressed data, was "resoto-plugin-protector-3.6.5.tar", last modified: Wed Aug  2 19:20:59 2023, max compression
```

## Comparing `resoto-plugin-protector-3.6.4.tar` & `resoto-plugin-protector-3.6.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:31:46.384057 resoto-plugin-protector-3.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 18:26:40.000000 resoto-plugin-protector-3.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-24 18:31:46.384057 resoto-plugin-protector-3.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-24 18:26:40.000000 resoto-plugin-protector-3.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-24 18:26:40.000000 resoto-plugin-protector-3.6.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:31:46.384057 resoto-plugin-protector-3.6.4/resoto_plugin_protector/
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-24 18:26:40.000000 resoto-plugin-protector-3.6.4/resoto_plugin_protector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-07-24 18:26:40.000000 resoto-plugin-protector-3.6.4/resoto_plugin_protector/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:31:46.384057 resoto-plugin-protector-3.6.4/resoto_plugin_protector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-24 18:31:46.000000 resoto-plugin-protector-3.6.4/resoto_plugin_protector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-24 18:31:46.000000 resoto-plugin-protector-3.6.4/resoto_plugin_protector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:31:46.000000 resoto-plugin-protector-3.6.4/resoto_plugin_protector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-24 18:31:46.000000 resoto-plugin-protector-3.6.4/resoto_plugin_protector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:28:38.000000 resoto-plugin-protector-3.6.4/resoto_plugin_protector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-24 18:31:46.000000 resoto-plugin-protector-3.6.4/resoto_plugin_protector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 18:31:46.000000 resoto-plugin-protector-3.6.4/resoto_plugin_protector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 18:31:46.384057 resoto-plugin-protector-3.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:31:46.384057 resoto-plugin-protector-3.6.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-24 18:26:40.000000 resoto-plugin-protector-3.6.4/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:20:59.215693 resoto-plugin-protector-3.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 19:17:16.000000 resoto-plugin-protector-3.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-08-02 19:20:59.215693 resoto-plugin-protector-3.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-08-02 19:17:16.000000 resoto-plugin-protector-3.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-08-02 19:17:16.000000 resoto-plugin-protector-3.6.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:20:59.215693 resoto-plugin-protector-3.6.5/resoto_plugin_protector/
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-08-02 19:17:16.000000 resoto-plugin-protector-3.6.5/resoto_plugin_protector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-08-02 19:17:16.000000 resoto-plugin-protector-3.6.5/resoto_plugin_protector/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:20:59.215693 resoto-plugin-protector-3.6.5/resoto_plugin_protector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-08-02 19:20:59.000000 resoto-plugin-protector-3.6.5/resoto_plugin_protector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-02 19:20:59.000000 resoto-plugin-protector-3.6.5/resoto_plugin_protector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:20:59.000000 resoto-plugin-protector-3.6.5/resoto_plugin_protector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-02 19:20:59.000000 resoto-plugin-protector-3.6.5/resoto_plugin_protector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:18:42.000000 resoto-plugin-protector-3.6.5/resoto_plugin_protector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-02 19:20:59.000000 resoto-plugin-protector-3.6.5/resoto_plugin_protector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 19:20:59.000000 resoto-plugin-protector-3.6.5/resoto_plugin_protector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-02 19:20:59.219694 resoto-plugin-protector-3.6.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:20:59.215693 resoto-plugin-protector-3.6.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-08-02 19:17:16.000000 resoto-plugin-protector-3.6.5/test/test_config.py
```

### Comparing `resoto-plugin-protector-3.6.4/PKG-INFO` & `resoto-plugin-protector-3.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-protector
-Version: 3.6.4
+Version: 3.6.5
 Summary: Resoto Protector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/protector
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-protector-3.6.4/README.md` & `resoto-plugin-protector-3.6.5/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-protector-3.6.4/pyproject.toml` & `resoto-plugin-protector-3.6.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-protector"
 description = "Resoto Protector Plugin"
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
 protector = "resoto_plugin_protector:ProtectorPlugin"
 
 [project.urls]
 Documentation = "https://resoto.com"
```

### Comparing `resoto-plugin-protector-3.6.4/resoto_plugin_protector/__init__.py` & `resoto-plugin-protector-3.6.5/resoto_plugin_protector/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-protector-3.6.4/resoto_plugin_protector/config.py` & `resoto-plugin-protector-3.6.5/resoto_plugin_protector/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-protector-3.6.4/resoto_plugin_protector.egg-info/PKG-INFO` & `resoto-plugin-protector-3.6.5/resoto_plugin_protector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-protector
-Version: 3.6.4
+Version: 3.6.5
 Summary: Resoto Protector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/protector
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```


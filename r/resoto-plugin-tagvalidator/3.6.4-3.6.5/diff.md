# Comparing `tmp/resoto-plugin-tagvalidator-3.6.4.tar.gz` & `tmp/resoto-plugin-tagvalidator-3.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-tagvalidator-3.6.4.tar", last modified: Mon Jul 24 18:35:20 2023, max compression
+gzip compressed data, was "resoto-plugin-tagvalidator-3.6.5.tar", last modified: Wed Aug  2 19:23:18 2023, max compression
```

## Comparing `resoto-plugin-tagvalidator-3.6.4.tar` & `resoto-plugin-tagvalidator-3.6.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:20.510604 resoto-plugin-tagvalidator-3.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 18:29:33.000000 resoto-plugin-tagvalidator-3.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-07-24 18:35:20.510604 resoto-plugin-tagvalidator-3.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-24 18:29:33.000000 resoto-plugin-tagvalidator-3.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-24 18:29:33.000000 resoto-plugin-tagvalidator-3.6.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:20.510604 resoto-plugin-tagvalidator-3.6.4/resoto_plugin_tagvalidator/
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-07-24 18:29:33.000000 resoto-plugin-tagvalidator-3.6.4/resoto_plugin_tagvalidator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-24 18:29:33.000000 resoto-plugin-tagvalidator-3.6.4/resoto_plugin_tagvalidator/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:20.510604 resoto-plugin-tagvalidator-3.6.4/resoto_plugin_tagvalidator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-07-24 18:35:20.000000 resoto-plugin-tagvalidator-3.6.4/resoto_plugin_tagvalidator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-24 18:35:20.000000 resoto-plugin-tagvalidator-3.6.4/resoto_plugin_tagvalidator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:35:20.000000 resoto-plugin-tagvalidator-3.6.4/resoto_plugin_tagvalidator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-24 18:35:20.000000 resoto-plugin-tagvalidator-3.6.4/resoto_plugin_tagvalidator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:31:21.000000 resoto-plugin-tagvalidator-3.6.4/resoto_plugin_tagvalidator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-24 18:35:20.000000 resoto-plugin-tagvalidator-3.6.4/resoto_plugin_tagvalidator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-24 18:35:20.000000 resoto-plugin-tagvalidator-3.6.4/resoto_plugin_tagvalidator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 18:35:20.510604 resoto-plugin-tagvalidator-3.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:35:20.510604 resoto-plugin-tagvalidator-3.6.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-24 18:29:33.000000 resoto-plugin-tagvalidator-3.6.4/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:23:18.065852 resoto-plugin-tagvalidator-3.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 19:17:19.000000 resoto-plugin-tagvalidator-3.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-08-02 19:23:18.065852 resoto-plugin-tagvalidator-3.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-08-02 19:17:19.000000 resoto-plugin-tagvalidator-3.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-08-02 19:17:19.000000 resoto-plugin-tagvalidator-3.6.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:23:18.061852 resoto-plugin-tagvalidator-3.6.5/resoto_plugin_tagvalidator/
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-08-02 19:17:19.000000 resoto-plugin-tagvalidator-3.6.5/resoto_plugin_tagvalidator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-08-02 19:17:19.000000 resoto-plugin-tagvalidator-3.6.5/resoto_plugin_tagvalidator/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:23:18.065852 resoto-plugin-tagvalidator-3.6.5/resoto_plugin_tagvalidator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-08-02 19:23:18.000000 resoto-plugin-tagvalidator-3.6.5/resoto_plugin_tagvalidator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-02 19:23:18.000000 resoto-plugin-tagvalidator-3.6.5/resoto_plugin_tagvalidator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:23:18.000000 resoto-plugin-tagvalidator-3.6.5/resoto_plugin_tagvalidator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-02 19:23:18.000000 resoto-plugin-tagvalidator-3.6.5/resoto_plugin_tagvalidator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:19:05.000000 resoto-plugin-tagvalidator-3.6.5/resoto_plugin_tagvalidator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-02 19:23:18.000000 resoto-plugin-tagvalidator-3.6.5/resoto_plugin_tagvalidator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 19:23:18.000000 resoto-plugin-tagvalidator-3.6.5/resoto_plugin_tagvalidator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-02 19:23:18.065852 resoto-plugin-tagvalidator-3.6.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:23:18.065852 resoto-plugin-tagvalidator-3.6.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-08-02 19:17:19.000000 resoto-plugin-tagvalidator-3.6.5/test/test_config.py
```

### Comparing `resoto-plugin-tagvalidator-3.6.4/PKG-INFO` & `resoto-plugin-tagvalidator-3.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-tagvalidator
-Version: 3.6.4
+Version: 3.6.5
 Summary: Resoto Tag Validator Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/tagvalidator
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-tagvalidator-3.6.4/README.md` & `resoto-plugin-tagvalidator-3.6.5/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-tagvalidator-3.6.4/pyproject.toml` & `resoto-plugin-tagvalidator-3.6.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-tagvalidator"
 description = "Resoto Tag Validator Plugin"
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
 tagvalidator = "resoto_plugin_tagvalidator:TagValidatorPlugin"
 
 [project.urls]
 Documentation = "https://resoto.com"
```

### Comparing `resoto-plugin-tagvalidator-3.6.4/resoto_plugin_tagvalidator/__init__.py` & `resoto-plugin-tagvalidator-3.6.5/resoto_plugin_tagvalidator/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-tagvalidator-3.6.4/resoto_plugin_tagvalidator/config.py` & `resoto-plugin-tagvalidator-3.6.5/resoto_plugin_tagvalidator/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-tagvalidator-3.6.4/resoto_plugin_tagvalidator.egg-info/PKG-INFO` & `resoto-plugin-tagvalidator-3.6.5/resoto_plugin_tagvalidator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-tagvalidator
-Version: 3.6.4
+Version: 3.6.5
 Summary: Resoto Tag Validator Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/tagvalidator
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-tagvalidator-3.6.4/test/test_config.py` & `resoto-plugin-tagvalidator-3.6.5/test/test_config.py`

 * *Files identical despite different names*


# Comparing `tmp/resoto-plugin-scarf-3.6.4.tar.gz` & `tmp/resoto-plugin-scarf-3.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-scarf-3.6.4.tar", last modified: Mon Jul 24 18:36:14 2023, max compression
+gzip compressed data, was "resoto-plugin-scarf-3.6.5.tar", last modified: Wed Aug  2 19:26:48 2023, max compression
```

## Comparing `resoto-plugin-scarf-3.6.4.tar` & `resoto-plugin-scarf-3.6.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:36:14.358401 resoto-plugin-scarf-3.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 18:31:34.000000 resoto-plugin-scarf-3.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-24 18:36:14.358401 resoto-plugin-scarf-3.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-24 18:31:34.000000 resoto-plugin-scarf-3.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-24 18:31:34.000000 resoto-plugin-scarf-3.6.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:36:14.358401 resoto-plugin-scarf-3.6.4/resoto_plugin_scarf/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-24 18:31:34.000000 resoto-plugin-scarf-3.6.4/resoto_plugin_scarf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-24 18:31:34.000000 resoto-plugin-scarf-3.6.4/resoto_plugin_scarf/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-24 18:31:34.000000 resoto-plugin-scarf-3.6.4/resoto_plugin_scarf/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-07-24 18:31:34.000000 resoto-plugin-scarf-3.6.4/resoto_plugin_scarf/scarf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:36:14.358401 resoto-plugin-scarf-3.6.4/resoto_plugin_scarf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-24 18:36:14.000000 resoto-plugin-scarf-3.6.4/resoto_plugin_scarf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-24 18:36:14.000000 resoto-plugin-scarf-3.6.4/resoto_plugin_scarf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:36:14.000000 resoto-plugin-scarf-3.6.4/resoto_plugin_scarf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-24 18:36:14.000000 resoto-plugin-scarf-3.6.4/resoto_plugin_scarf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:33:22.000000 resoto-plugin-scarf-3.6.4/resoto_plugin_scarf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 18:36:14.000000 resoto-plugin-scarf-3.6.4/resoto_plugin_scarf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-24 18:36:14.000000 resoto-plugin-scarf-3.6.4/resoto_plugin_scarf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 18:36:14.358401 resoto-plugin-scarf-3.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:36:14.358401 resoto-plugin-scarf-3.6.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-24 18:31:34.000000 resoto-plugin-scarf-3.6.4/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:26:48.612383 resoto-plugin-scarf-3.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 19:22:35.000000 resoto-plugin-scarf-3.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-08-02 19:26:48.612383 resoto-plugin-scarf-3.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-02 19:22:35.000000 resoto-plugin-scarf-3.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-08-02 19:22:35.000000 resoto-plugin-scarf-3.6.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:26:48.612383 resoto-plugin-scarf-3.6.5/resoto_plugin_scarf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-08-02 19:22:35.000000 resoto-plugin-scarf-3.6.5/resoto_plugin_scarf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-02 19:22:35.000000 resoto-plugin-scarf-3.6.5/resoto_plugin_scarf/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-08-02 19:22:35.000000 resoto-plugin-scarf-3.6.5/resoto_plugin_scarf/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-08-02 19:22:35.000000 resoto-plugin-scarf-3.6.5/resoto_plugin_scarf/scarf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:26:48.612383 resoto-plugin-scarf-3.6.5/resoto_plugin_scarf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-08-02 19:26:48.000000 resoto-plugin-scarf-3.6.5/resoto_plugin_scarf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-02 19:26:48.000000 resoto-plugin-scarf-3.6.5/resoto_plugin_scarf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:26:48.000000 resoto-plugin-scarf-3.6.5/resoto_plugin_scarf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-02 19:26:48.000000 resoto-plugin-scarf-3.6.5/resoto_plugin_scarf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:24:15.000000 resoto-plugin-scarf-3.6.5/resoto_plugin_scarf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 19:26:48.000000 resoto-plugin-scarf-3.6.5/resoto_plugin_scarf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-02 19:26:48.000000 resoto-plugin-scarf-3.6.5/resoto_plugin_scarf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-02 19:26:48.612383 resoto-plugin-scarf-3.6.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:26:48.612383 resoto-plugin-scarf-3.6.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-02 19:22:35.000000 resoto-plugin-scarf-3.6.5/test/test_config.py
```

### Comparing `resoto-plugin-scarf-3.6.4/PKG-INFO` & `resoto-plugin-scarf-3.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-scarf
-Version: 3.6.4
+Version: 3.6.5
 Summary: Resoto Scarf Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/scarf
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-scarf-3.6.4/README.md` & `resoto-plugin-scarf-3.6.5/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-scarf-3.6.4/pyproject.toml` & `resoto-plugin-scarf-3.6.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-scarf"
 description = "Resoto Scarf Collector Plugin"
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
 scarf = "resoto_plugin_scarf:ScarfCollectorPlugin"
 
 [project.urls]
```

### Comparing `resoto-plugin-scarf-3.6.4/resoto_plugin_scarf/__init__.py` & `resoto-plugin-scarf-3.6.5/resoto_plugin_scarf/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-scarf-3.6.4/resoto_plugin_scarf/resources.py` & `resoto-plugin-scarf-3.6.5/resoto_plugin_scarf/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-scarf-3.6.4/resoto_plugin_scarf/scarf.py` & `resoto-plugin-scarf-3.6.5/resoto_plugin_scarf/scarf.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-scarf-3.6.4/resoto_plugin_scarf.egg-info/PKG-INFO` & `resoto-plugin-scarf-3.6.5/resoto_plugin_scarf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-scarf
-Version: 3.6.4
+Version: 3.6.5
 Summary: Resoto Scarf Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/scarf
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```


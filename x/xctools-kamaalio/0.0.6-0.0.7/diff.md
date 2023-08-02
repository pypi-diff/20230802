# Comparing `tmp/xctools_kamaalio-0.0.6.tar.gz` & `tmp/xctools_kamaalio-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xctools_kamaalio-0.0.6.tar", last modified: Sun Jul 30 19:04:52 2023, max compression
+gzip compressed data, was "xctools_kamaalio-0.0.7.tar", last modified: Wed Aug  2 17:29:36 2023, max compression
```

## Comparing `xctools_kamaalio-0.0.6.tar` & `xctools_kamaalio-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-30 19:04:52.379246 xctools_kamaalio-0.0.6/
--rw-r--r--   0 kamaal     (503) staff       (20)     1077 2023-07-30 19:02:46.000000 xctools_kamaalio-0.0.6/LICENSE
--rw-r--r--   0 kamaal     (503) staff       (20)      532 2023-07-30 19:04:52.379135 xctools_kamaalio-0.0.6/PKG-INFO
--rw-r--r--   0 kamaal     (503) staff       (20)       10 2023-07-30 19:02:46.000000 xctools_kamaalio-0.0.6/README.md
--rw-r--r--   0 kamaal     (503) staff       (20)      688 2023-07-30 19:04:14.000000 xctools_kamaalio-0.0.6/pyproject.toml
--rw-r--r--   0 kamaal     (503) staff       (20)       38 2023-07-30 19:04:52.379292 xctools_kamaalio-0.0.6/setup.cfg
-drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-30 19:04:52.376607 xctools_kamaalio-0.0.6/src/
-drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-30 19:04:52.377619 xctools_kamaalio-0.0.6/src/xctools_kamaalio/
--rw-r--r--   0 kamaal     (503) staff       (20)        0 2023-07-30 19:02:46.000000 xctools_kamaalio-0.0.6/src/xctools_kamaalio/__init__.py
-drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-30 19:04:52.378970 xctools_kamaalio-0.0.6/src/xctools_kamaalio/actions/
--rw-r--r--   0 kamaal     (503) staff       (20)      875 2023-07-30 19:02:46.000000 xctools_kamaalio-0.0.6/src/xctools_kamaalio/actions/archive.py
--rw-r--r--   0 kamaal     (503) staff       (20)      340 2023-07-30 19:02:46.000000 xctools_kamaalio-0.0.6/src/xctools_kamaalio/actions/bump_version.py
--rw-r--r--   0 kamaal     (503) staff       (20)      358 2023-07-30 19:02:46.000000 xctools_kamaalio-0.0.6/src/xctools_kamaalio/actions/export_archive.py
--rw-r--r--   0 kamaal     (503) staff       (20)      496 2023-07-30 19:02:46.000000 xctools_kamaalio-0.0.6/src/xctools_kamaalio/actions/upload.py
--rw-r--r--   0 kamaal     (503) staff       (20)      943 2023-07-30 19:02:46.000000 xctools_kamaalio-0.0.6/src/xctools_kamaalio/cli.py
--rw-r--r--   0 kamaal     (503) staff       (20)      528 2023-07-30 19:02:46.000000 xctools_kamaalio-0.0.6/src/xctools_kamaalio/list_utils.py
--rw-r--r--   0 kamaal     (503) staff       (20)     3470 2023-07-30 19:02:46.000000 xctools_kamaalio-0.0.6/src/xctools_kamaalio/version_bumper.py
--rw-r--r--   0 kamaal     (503) staff       (20)     2239 2023-07-30 19:02:46.000000 xctools_kamaalio-0.0.6/src/xctools_kamaalio/xctools.py
-drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-30 19:04:52.378428 xctools_kamaalio-0.0.6/src/xctools_kamaalio.egg-info/
--rw-r--r--   0 kamaal     (503) staff       (20)      532 2023-07-30 19:04:52.000000 xctools_kamaalio-0.0.6/src/xctools_kamaalio.egg-info/PKG-INFO
--rw-r--r--   0 kamaal     (503) staff       (20)      636 2023-07-30 19:04:52.000000 xctools_kamaalio-0.0.6/src/xctools_kamaalio.egg-info/SOURCES.txt
--rw-r--r--   0 kamaal     (503) staff       (20)        1 2023-07-30 19:04:52.000000 xctools_kamaalio-0.0.6/src/xctools_kamaalio.egg-info/dependency_links.txt
--rw-r--r--   0 kamaal     (503) staff       (20)       53 2023-07-30 19:04:52.000000 xctools_kamaalio-0.0.6/src/xctools_kamaalio.egg-info/entry_points.txt
--rw-r--r--   0 kamaal     (503) staff       (20)       13 2023-07-30 19:04:52.000000 xctools_kamaalio-0.0.6/src/xctools_kamaalio.egg-info/requires.txt
--rw-r--r--   0 kamaal     (503) staff       (20)       17 2023-07-30 19:04:52.000000 xctools_kamaalio-0.0.6/src/xctools_kamaalio.egg-info/top_level.txt
+drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-08-02 17:29:36.150616 xctools_kamaalio-0.0.7/
+-rw-r--r--   0 kamaal     (503) staff       (20)     1077 2023-07-31 19:24:54.000000 xctools_kamaalio-0.0.7/LICENSE
+-rw-r--r--   0 kamaal     (503) staff       (20)      532 2023-08-02 17:29:36.150482 xctools_kamaalio-0.0.7/PKG-INFO
+-rw-r--r--   0 kamaal     (503) staff       (20)       10 2023-07-31 19:24:54.000000 xctools_kamaalio-0.0.7/README.md
+-rw-r--r--   0 kamaal     (503) staff       (20)      688 2023-08-02 17:28:16.000000 xctools_kamaalio-0.0.7/pyproject.toml
+-rw-r--r--   0 kamaal     (503) staff       (20)       38 2023-08-02 17:29:36.150673 xctools_kamaalio-0.0.7/setup.cfg
+drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-08-02 17:29:36.146605 xctools_kamaalio-0.0.7/src/
+drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-08-02 17:29:36.148366 xctools_kamaalio-0.0.7/src/xctools_kamaalio/
+-rw-r--r--   0 kamaal     (503) staff       (20)        0 2023-07-31 19:24:54.000000 xctools_kamaalio-0.0.7/src/xctools_kamaalio/__init__.py
+drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-08-02 17:29:36.150259 xctools_kamaalio-0.0.7/src/xctools_kamaalio/actions/
+-rw-r--r--   0 kamaal     (503) staff       (20)      875 2023-07-31 19:24:54.000000 xctools_kamaalio-0.0.7/src/xctools_kamaalio/actions/archive.py
+-rw-r--r--   0 kamaal     (503) staff       (20)      635 2023-08-02 17:16:13.000000 xctools_kamaalio-0.0.7/src/xctools_kamaalio/actions/build.py
+-rw-r--r--   0 kamaal     (503) staff       (20)      340 2023-07-31 19:24:54.000000 xctools_kamaalio-0.0.7/src/xctools_kamaalio/actions/bump_version.py
+-rw-r--r--   0 kamaal     (503) staff       (20)      358 2023-07-31 19:24:54.000000 xctools_kamaalio-0.0.7/src/xctools_kamaalio/actions/export_archive.py
+-rw-r--r--   0 kamaal     (503) staff       (20)      633 2023-08-02 16:44:45.000000 xctools_kamaalio-0.0.7/src/xctools_kamaalio/actions/test.py
+-rw-r--r--   0 kamaal     (503) staff       (20)      269 2023-08-01 19:35:55.000000 xctools_kamaalio-0.0.7/src/xctools_kamaalio/actions/trust_swift_plugins.py
+-rw-r--r--   0 kamaal     (503) staff       (20)      496 2023-07-31 19:24:54.000000 xctools_kamaalio-0.0.7/src/xctools_kamaalio/actions/upload.py
+-rw-r--r--   0 kamaal     (503) staff       (20)     1338 2023-08-02 17:14:30.000000 xctools_kamaalio-0.0.7/src/xctools_kamaalio/cli.py
+-rw-r--r--   0 kamaal     (503) staff       (20)      528 2023-07-31 19:24:54.000000 xctools_kamaalio-0.0.7/src/xctools_kamaalio/list_utils.py
+-rw-r--r--   0 kamaal     (503) staff       (20)     2268 2023-08-01 20:20:52.000000 xctools_kamaalio-0.0.7/src/xctools_kamaalio/project_updater.py
+-rw-r--r--   0 kamaal     (503) staff       (20)     5398 2023-08-02 17:17:22.000000 xctools_kamaalio-0.0.7/src/xctools_kamaalio/xctools.py
+drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-08-02 17:29:36.149265 xctools_kamaalio-0.0.7/src/xctools_kamaalio.egg-info/
+-rw-r--r--   0 kamaal     (503) staff       (20)      532 2023-08-02 17:29:36.000000 xctools_kamaalio-0.0.7/src/xctools_kamaalio.egg-info/PKG-INFO
+-rw-r--r--   0 kamaal     (503) staff       (20)      764 2023-08-02 17:29:36.000000 xctools_kamaalio-0.0.7/src/xctools_kamaalio.egg-info/SOURCES.txt
+-rw-r--r--   0 kamaal     (503) staff       (20)        1 2023-08-02 17:29:36.000000 xctools_kamaalio-0.0.7/src/xctools_kamaalio.egg-info/dependency_links.txt
+-rw-r--r--   0 kamaal     (503) staff       (20)       53 2023-08-02 17:29:36.000000 xctools_kamaalio-0.0.7/src/xctools_kamaalio.egg-info/entry_points.txt
+-rw-r--r--   0 kamaal     (503) staff       (20)       13 2023-08-02 17:29:36.000000 xctools_kamaalio-0.0.7/src/xctools_kamaalio.egg-info/requires.txt
+-rw-r--r--   0 kamaal     (503) staff       (20)       17 2023-08-02 17:29:36.000000 xctools_kamaalio-0.0.7/src/xctools_kamaalio.egg-info/top_level.txt
```

### Comparing `xctools_kamaalio-0.0.6/LICENSE` & `xctools_kamaalio-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xctools_kamaalio-0.0.6/PKG-INFO` & `xctools_kamaalio-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xctools_kamaalio
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package to help deal with Xcode projects.
 Author-email: Kamaal Farah <kamaal.f1@gmail.com>
 Project-URL: Homepage, https://github.com/Kamaalio/XcTools
 Project-URL: Bug Tracker, https://github.com/Kamaalio/XcTools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xctools_kamaalio-0.0.6/pyproject.toml` & `xctools_kamaalio-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [project.scripts]
 xctools = "xctools_kamaalio:cli.cli"
 
 
 [project]
 name = "xctools_kamaalio"
-version = "0.0.6"
+version = "0.0.7"
 authors = [{ name = "Kamaal Farah", email = "kamaal.f1@gmail.com" }]
 description = "A package to help deal with Xcode projects."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `xctools_kamaalio-0.0.6/src/xctools_kamaalio/actions/archive.py` & `xctools_kamaalio-0.0.7/src/xctools_kamaalio/actions/archive.py`

 * *Files identical despite different names*

### Comparing `xctools_kamaalio-0.0.6/src/xctools_kamaalio/cli.py` & `xctools_kamaalio-0.0.7/src/xctools_kamaalio/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 import sys
 
-
 from xctools_kamaalio.list_utils import removed, find_index
 from xctools_kamaalio.actions.upload import upload
 from xctools_kamaalio.actions.archive import archive
 from xctools_kamaalio.actions.bump_version import bump_version
 from xctools_kamaalio.actions.export_archive import export_archive
+from xctools_kamaalio.actions.trust_swift_plugins import trust_swift_plugins
+from xctools_kamaalio.actions.test import test
+from xctools_kamaalio.actions.build import build
 
 
-ACTIONS = ["archive", "upload", "bump-version", "export-archive"]
+ACTIONS = [
+    "archive",
+    "upload",
+    "bump-version",
+    "export-archive",
+    "trust-swift-plugins",
+    "test",
+    "build",
+]
 
 
 def cli():
     action_index = find_index(sys.argv, lambda arg: arg in ACTIONS)
     if action_index is None:
         raise CLIException("Invalid action provided")
 
@@ -23,12 +33,18 @@
         archive()
     if action == "upload":
         upload()
     if action == "bump-version":
         bump_version()
     if action == "export-archive":
         export_archive()
+    if action == "trust-swift-plugins":
+        trust_swift_plugins()
+    if action == "test":
+        test()
+    if action == "build":
+        build()
 
 
 class CLIException(Exception):
     def __init__(self, message: str) -> None:
         super().__init__(message)
```

### Comparing `xctools_kamaalio-0.0.6/src/xctools_kamaalio/list_utils.py` & `xctools_kamaalio-0.0.7/src/xctools_kamaalio/list_utils.py`

 * *Files identical despite different names*

### Comparing `xctools_kamaalio-0.0.6/src/xctools_kamaalio.egg-info/PKG-INFO` & `xctools_kamaalio-0.0.7/src/xctools_kamaalio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xctools-kamaalio
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package to help deal with Xcode projects.
 Author-email: Kamaal Farah <kamaal.f1@gmail.com>
 Project-URL: Homepage, https://github.com/Kamaalio/XcTools
 Project-URL: Bug Tracker, https://github.com/Kamaalio/XcTools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xctools_kamaalio-0.0.6/src/xctools_kamaalio.egg-info/SOURCES.txt` & `xctools_kamaalio-0.0.7/src/xctools_kamaalio.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 LICENSE
 README.md
 pyproject.toml
 src/xctools_kamaalio/__init__.py
 src/xctools_kamaalio/cli.py
 src/xctools_kamaalio/list_utils.py
-src/xctools_kamaalio/version_bumper.py
+src/xctools_kamaalio/project_updater.py
 src/xctools_kamaalio/xctools.py
 src/xctools_kamaalio.egg-info/PKG-INFO
 src/xctools_kamaalio.egg-info/SOURCES.txt
 src/xctools_kamaalio.egg-info/dependency_links.txt
 src/xctools_kamaalio.egg-info/entry_points.txt
 src/xctools_kamaalio.egg-info/requires.txt
 src/xctools_kamaalio.egg-info/top_level.txt
 src/xctools_kamaalio/actions/archive.py
+src/xctools_kamaalio/actions/build.py
 src/xctools_kamaalio/actions/bump_version.py
 src/xctools_kamaalio/actions/export_archive.py
+src/xctools_kamaalio/actions/test.py
+src/xctools_kamaalio/actions/trust_swift_plugins.py
 src/xctools_kamaalio/actions/upload.py
```


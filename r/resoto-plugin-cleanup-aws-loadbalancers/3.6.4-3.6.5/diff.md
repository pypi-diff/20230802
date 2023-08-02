# Comparing `tmp/resoto-plugin-cleanup-aws-loadbalancers-3.6.4.tar.gz` & `tmp/resoto-plugin-cleanup-aws-loadbalancers-3.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-cleanup-aws-loadbalancers-3.6.4.tar", last modified: Mon Jul 24 18:28:54 2023, max compression
+gzip compressed data, was "resoto-plugin-cleanup-aws-loadbalancers-3.6.5.tar", last modified: Wed Aug  2 19:27:40 2023, max compression
```

## Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.6.4.tar` & `resoto-plugin-cleanup-aws-loadbalancers-3.6.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:28:54.356675 resoto-plugin-cleanup-aws-loadbalancers-3.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 18:23:40.000000 resoto-plugin-cleanup-aws-loadbalancers-3.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-24 18:28:54.356675 resoto-plugin-cleanup-aws-loadbalancers-3.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-24 18:23:40.000000 resoto-plugin-cleanup-aws-loadbalancers-3.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-24 18:23:40.000000 resoto-plugin-cleanup-aws-loadbalancers-3.6.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:28:54.356675 resoto-plugin-cleanup-aws-loadbalancers-3.6.4/resoto_plugin_cleanup_aws_loadbalancers/
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-07-24 18:23:40.000000 resoto-plugin-cleanup-aws-loadbalancers-3.6.4/resoto_plugin_cleanup_aws_loadbalancers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-24 18:23:40.000000 resoto-plugin-cleanup-aws-loadbalancers-3.6.4/resoto_plugin_cleanup_aws_loadbalancers/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:28:54.356675 resoto-plugin-cleanup-aws-loadbalancers-3.6.4/resoto_plugin_cleanup_aws_loadbalancers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-24 18:28:54.000000 resoto-plugin-cleanup-aws-loadbalancers-3.6.4/resoto_plugin_cleanup_aws_loadbalancers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-24 18:28:54.000000 resoto-plugin-cleanup-aws-loadbalancers-3.6.4/resoto_plugin_cleanup_aws_loadbalancers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:28:54.000000 resoto-plugin-cleanup-aws-loadbalancers-3.6.4/resoto_plugin_cleanup_aws_loadbalancers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-24 18:28:54.000000 resoto-plugin-cleanup-aws-loadbalancers-3.6.4/resoto_plugin_cleanup_aws_loadbalancers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:25:46.000000 resoto-plugin-cleanup-aws-loadbalancers-3.6.4/resoto_plugin_cleanup_aws_loadbalancers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-24 18:28:54.000000 resoto-plugin-cleanup-aws-loadbalancers-3.6.4/resoto_plugin_cleanup_aws_loadbalancers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-24 18:28:54.000000 resoto-plugin-cleanup-aws-loadbalancers-3.6.4/resoto_plugin_cleanup_aws_loadbalancers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 18:28:54.356675 resoto-plugin-cleanup-aws-loadbalancers-3.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:28:54.356675 resoto-plugin-cleanup-aws-loadbalancers-3.6.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-24 18:23:40.000000 resoto-plugin-cleanup-aws-loadbalancers-3.6.4/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:40.281483 resoto-plugin-cleanup-aws-loadbalancers-3.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 19:23:33.000000 resoto-plugin-cleanup-aws-loadbalancers-3.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-08-02 19:27:40.281483 resoto-plugin-cleanup-aws-loadbalancers-3.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-08-02 19:23:33.000000 resoto-plugin-cleanup-aws-loadbalancers-3.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-08-02 19:23:33.000000 resoto-plugin-cleanup-aws-loadbalancers-3.6.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:40.281483 resoto-plugin-cleanup-aws-loadbalancers-3.6.5/resoto_plugin_cleanup_aws_loadbalancers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-08-02 19:23:33.000000 resoto-plugin-cleanup-aws-loadbalancers-3.6.5/resoto_plugin_cleanup_aws_loadbalancers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-02 19:23:33.000000 resoto-plugin-cleanup-aws-loadbalancers-3.6.5/resoto_plugin_cleanup_aws_loadbalancers/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:40.281483 resoto-plugin-cleanup-aws-loadbalancers-3.6.5/resoto_plugin_cleanup_aws_loadbalancers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-08-02 19:27:40.000000 resoto-plugin-cleanup-aws-loadbalancers-3.6.5/resoto_plugin_cleanup_aws_loadbalancers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-02 19:27:40.000000 resoto-plugin-cleanup-aws-loadbalancers-3.6.5/resoto_plugin_cleanup_aws_loadbalancers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:27:40.000000 resoto-plugin-cleanup-aws-loadbalancers-3.6.5/resoto_plugin_cleanup_aws_loadbalancers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-02 19:27:40.000000 resoto-plugin-cleanup-aws-loadbalancers-3.6.5/resoto_plugin_cleanup_aws_loadbalancers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:25:13.000000 resoto-plugin-cleanup-aws-loadbalancers-3.6.5/resoto_plugin_cleanup_aws_loadbalancers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-02 19:27:40.000000 resoto-plugin-cleanup-aws-loadbalancers-3.6.5/resoto_plugin_cleanup_aws_loadbalancers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-02 19:27:40.000000 resoto-plugin-cleanup-aws-loadbalancers-3.6.5/resoto_plugin_cleanup_aws_loadbalancers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-02 19:27:40.281483 resoto-plugin-cleanup-aws-loadbalancers-3.6.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:40.281483 resoto-plugin-cleanup-aws-loadbalancers-3.6.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-08-02 19:23:33.000000 resoto-plugin-cleanup-aws-loadbalancers-3.6.5/test/test_config.py
```

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.6.4/PKG-INFO` & `resoto-plugin-cleanup-aws-loadbalancers-3.6.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-aws-loadbalancers
-Version: 3.6.4
+Version: 3.6.5
 Summary: AWS Loadbalancers Cleaner Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_loadbalancers
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.6.4/README.md` & `resoto-plugin-cleanup-aws-loadbalancers-3.6.5/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.6.4/pyproject.toml` & `resoto-plugin-cleanup-aws-loadbalancers-3.6.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resoto-plugin-cleanup-aws-loadbalancers"
-version = "3.6.4"
+version = "3.6.5"
 authors = [{name="Some Engineering Inc."}]
 description = "AWS Loadbalancers Cleaner Plugin"
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
@@ -23,16 +23,16 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.6.4",
-    "resoto-plugin-aws==3.6.4"
+    "resotolib==3.6.5",
+    "resoto-plugin-aws==3.6.5"
 ]
 
 [project.entry-points."resoto.plugins"]
 cleanup_aws_loadbalancers = "resoto_plugin_cleanup_aws_loadbalancers:CleanupAWSLoadbalancersPlugin"
 
 [project.urls]
 Documentation = "https://resoto.com"
```

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.6.4/resoto_plugin_cleanup_aws_loadbalancers/__init__.py` & `resoto-plugin-cleanup-aws-loadbalancers-3.6.5/resoto_plugin_cleanup_aws_loadbalancers/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.6.4/resoto_plugin_cleanup_aws_loadbalancers/config.py` & `resoto-plugin-cleanup-aws-loadbalancers-3.6.5/resoto_plugin_cleanup_aws_loadbalancers/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.6.4/resoto_plugin_cleanup_aws_loadbalancers.egg-info/PKG-INFO` & `resoto-plugin-cleanup-aws-loadbalancers-3.6.5/resoto_plugin_cleanup_aws_loadbalancers.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-aws-loadbalancers
-Version: 3.6.4
+Version: 3.6.5
 Summary: AWS Loadbalancers Cleaner Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_loadbalancers
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.6.4/resoto_plugin_cleanup_aws_loadbalancers.egg-info/SOURCES.txt` & `resoto-plugin-cleanup-aws-loadbalancers-3.6.5/resoto_plugin_cleanup_aws_loadbalancers.egg-info/SOURCES.txt`

 * *Files identical despite different names*


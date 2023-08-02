# Comparing `tmp/resoto-plugin-cleanup-aws-vpcs-3.6.4.tar.gz` & `tmp/resoto-plugin-cleanup-aws-vpcs-3.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-cleanup-aws-vpcs-3.6.4.tar", last modified: Mon Jul 24 18:31:05 2023, max compression
+gzip compressed data, was "resoto-plugin-cleanup-aws-vpcs-3.6.5.tar", last modified: Wed Aug  2 19:27:13 2023, max compression
```

## Comparing `resoto-plugin-cleanup-aws-vpcs-3.6.4.tar` & `resoto-plugin-cleanup-aws-vpcs-3.6.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:31:05.515128 resoto-plugin-cleanup-aws-vpcs-3.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 18:25:34.000000 resoto-plugin-cleanup-aws-vpcs-3.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-24 18:31:05.515128 resoto-plugin-cleanup-aws-vpcs-3.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-24 18:25:34.000000 resoto-plugin-cleanup-aws-vpcs-3.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-24 18:25:34.000000 resoto-plugin-cleanup-aws-vpcs-3.6.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:31:05.511128 resoto-plugin-cleanup-aws-vpcs-3.6.4/resoto_plugin_cleanup_aws_vpcs/
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-07-24 18:25:34.000000 resoto-plugin-cleanup-aws-vpcs-3.6.4/resoto_plugin_cleanup_aws_vpcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-24 18:25:34.000000 resoto-plugin-cleanup-aws-vpcs-3.6.4/resoto_plugin_cleanup_aws_vpcs/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:31:05.511128 resoto-plugin-cleanup-aws-vpcs-3.6.4/resoto_plugin_cleanup_aws_vpcs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-24 18:31:05.000000 resoto-plugin-cleanup-aws-vpcs-3.6.4/resoto_plugin_cleanup_aws_vpcs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-24 18:31:05.000000 resoto-plugin-cleanup-aws-vpcs-3.6.4/resoto_plugin_cleanup_aws_vpcs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:31:05.000000 resoto-plugin-cleanup-aws-vpcs-3.6.4/resoto_plugin_cleanup_aws_vpcs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-24 18:31:05.000000 resoto-plugin-cleanup-aws-vpcs-3.6.4/resoto_plugin_cleanup_aws_vpcs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:27:46.000000 resoto-plugin-cleanup-aws-vpcs-3.6.4/resoto_plugin_cleanup_aws_vpcs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-24 18:31:05.000000 resoto-plugin-cleanup-aws-vpcs-3.6.4/resoto_plugin_cleanup_aws_vpcs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 18:31:05.000000 resoto-plugin-cleanup-aws-vpcs-3.6.4/resoto_plugin_cleanup_aws_vpcs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 18:31:05.515128 resoto-plugin-cleanup-aws-vpcs-3.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:31:05.515128 resoto-plugin-cleanup-aws-vpcs-3.6.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-24 18:25:34.000000 resoto-plugin-cleanup-aws-vpcs-3.6.4/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:13.218498 resoto-plugin-cleanup-aws-vpcs-3.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 19:22:03.000000 resoto-plugin-cleanup-aws-vpcs-3.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-08-02 19:27:13.218498 resoto-plugin-cleanup-aws-vpcs-3.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-08-02 19:22:03.000000 resoto-plugin-cleanup-aws-vpcs-3.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-08-02 19:22:03.000000 resoto-plugin-cleanup-aws-vpcs-3.6.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:13.214498 resoto-plugin-cleanup-aws-vpcs-3.6.5/resoto_plugin_cleanup_aws_vpcs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-08-02 19:22:03.000000 resoto-plugin-cleanup-aws-vpcs-3.6.5/resoto_plugin_cleanup_aws_vpcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-08-02 19:22:03.000000 resoto-plugin-cleanup-aws-vpcs-3.6.5/resoto_plugin_cleanup_aws_vpcs/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:13.218498 resoto-plugin-cleanup-aws-vpcs-3.6.5/resoto_plugin_cleanup_aws_vpcs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-08-02 19:27:13.000000 resoto-plugin-cleanup-aws-vpcs-3.6.5/resoto_plugin_cleanup_aws_vpcs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-08-02 19:27:13.000000 resoto-plugin-cleanup-aws-vpcs-3.6.5/resoto_plugin_cleanup_aws_vpcs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:27:13.000000 resoto-plugin-cleanup-aws-vpcs-3.6.5/resoto_plugin_cleanup_aws_vpcs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-02 19:27:13.000000 resoto-plugin-cleanup-aws-vpcs-3.6.5/resoto_plugin_cleanup_aws_vpcs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:24:07.000000 resoto-plugin-cleanup-aws-vpcs-3.6.5/resoto_plugin_cleanup_aws_vpcs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-02 19:27:13.000000 resoto-plugin-cleanup-aws-vpcs-3.6.5/resoto_plugin_cleanup_aws_vpcs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 19:27:13.000000 resoto-plugin-cleanup-aws-vpcs-3.6.5/resoto_plugin_cleanup_aws_vpcs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-02 19:27:13.218498 resoto-plugin-cleanup-aws-vpcs-3.6.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:13.218498 resoto-plugin-cleanup-aws-vpcs-3.6.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-08-02 19:22:03.000000 resoto-plugin-cleanup-aws-vpcs-3.6.5/test/test_config.py
```

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.6.4/PKG-INFO` & `resoto-plugin-cleanup-aws-vpcs-3.6.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-aws-vpcs
-Version: 3.6.4
+Version: 3.6.5
 Summary: AWS VPC Cleaner Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_vpcs
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.6.4/README.md` & `resoto-plugin-cleanup-aws-vpcs-3.6.5/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.6.4/pyproject.toml` & `resoto-plugin-cleanup-aws-vpcs-3.6.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-cleanup-aws-vpcs"
 description = "AWS VPC Cleaner Plugin"
-version = "3.6.4"
+version = "3.6.5"
 authors = [{name="Some Engineering Inc."}]
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
     # Audience
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
 cleanup_aws_vpcs = "resoto_plugin_cleanup_aws_vpcs:CleanupAWSVPCsPlugin"
 
 [project.urls]
 Documentation = "https://resoto.com"
```

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.6.4/resoto_plugin_cleanup_aws_vpcs/__init__.py` & `resoto-plugin-cleanup-aws-vpcs-3.6.5/resoto_plugin_cleanup_aws_vpcs/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.6.4/resoto_plugin_cleanup_aws_vpcs/config.py` & `resoto-plugin-cleanup-aws-vpcs-3.6.5/resoto_plugin_cleanup_aws_vpcs/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.6.4/resoto_plugin_cleanup_aws_vpcs.egg-info/PKG-INFO` & `resoto-plugin-cleanup-aws-vpcs-3.6.5/resoto_plugin_cleanup_aws_vpcs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-aws-vpcs
-Version: 3.6.4
+Version: 3.6.5
 Summary: AWS VPC Cleaner Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_vpcs
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.6.4/resoto_plugin_cleanup_aws_vpcs.egg-info/SOURCES.txt` & `resoto-plugin-cleanup-aws-vpcs-3.6.5/resoto_plugin_cleanup_aws_vpcs.egg-info/SOURCES.txt`

 * *Files identical despite different names*


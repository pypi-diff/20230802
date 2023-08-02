# Comparing `tmp/resoto-plugin-azure-3.6.4.tar.gz` & `tmp/resoto-plugin-azure-3.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-azure-3.6.4.tar", last modified: Mon Jul 24 18:29:47 2023, max compression
+gzip compressed data, was "resoto-plugin-azure-3.6.5.tar", last modified: Wed Aug  2 19:25:08 2023, max compression
```

## Comparing `resoto-plugin-azure-3.6.4.tar` & `resoto-plugin-azure-3.6.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:29:47.905970 resoto-plugin-azure-3.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-24 18:29:47.905970 resoto-plugin-azure-3.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-24 18:23:18.000000 resoto-plugin-azure-3.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-24 18:23:18.000000 resoto-plugin-azure-3.6.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:29:47.901970 resoto-plugin-azure-3.6.4/resoto_plugin_azure/
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-24 18:23:18.000000 resoto-plugin-azure-3.6.4/resoto_plugin_azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-07-24 18:23:18.000000 resoto-plugin-azure-3.6.4/resoto_plugin_azure/azure_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-24 18:23:18.000000 resoto-plugin-azure-3.6.4/resoto_plugin_azure/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-24 18:23:18.000000 resoto-plugin-azure-3.6.4/resoto_plugin_azure/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:29:47.901970 resoto-plugin-azure-3.6.4/resoto_plugin_azure/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:23:18.000000 resoto-plugin-azure-3.6.4/resoto_plugin_azure/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20818 2023-07-24 18:23:18.000000 resoto-plugin-azure-3.6.4/resoto_plugin_azure/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   274222 2023-07-24 18:23:18.000000 resoto-plugin-azure-3.6.4/resoto_plugin_azure/resource/compute.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:29:47.901970 resoto-plugin-azure-3.6.4/resoto_plugin_azure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-24 18:29:47.000000 resoto-plugin-azure-3.6.4/resoto_plugin_azure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-24 18:29:47.000000 resoto-plugin-azure-3.6.4/resoto_plugin_azure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:29:47.000000 resoto-plugin-azure-3.6.4/resoto_plugin_azure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-24 18:29:47.000000 resoto-plugin-azure-3.6.4/resoto_plugin_azure.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:24:56.000000 resoto-plugin-azure-3.6.4/resoto_plugin_azure.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-24 18:29:47.000000 resoto-plugin-azure-3.6.4/resoto_plugin_azure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-24 18:29:47.000000 resoto-plugin-azure-3.6.4/resoto_plugin_azure.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-24 18:29:47.905970 resoto-plugin-azure-3.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:25:08.169901 resoto-plugin-azure-3.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-08-02 19:25:08.169901 resoto-plugin-azure-3.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-02 19:17:24.000000 resoto-plugin-azure-3.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-08-02 19:17:24.000000 resoto-plugin-azure-3.6.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:25:08.169901 resoto-plugin-azure-3.6.5/resoto_plugin_azure/
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-08-02 19:17:24.000000 resoto-plugin-azure-3.6.5/resoto_plugin_azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-08-02 19:17:24.000000 resoto-plugin-azure-3.6.5/resoto_plugin_azure/azure_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-08-02 19:17:24.000000 resoto-plugin-azure-3.6.5/resoto_plugin_azure/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-08-02 19:17:24.000000 resoto-plugin-azure-3.6.5/resoto_plugin_azure/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:25:08.169901 resoto-plugin-azure-3.6.5/resoto_plugin_azure/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:17:24.000000 resoto-plugin-azure-3.6.5/resoto_plugin_azure/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20818 2023-08-02 19:17:24.000000 resoto-plugin-azure-3.6.5/resoto_plugin_azure/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   274222 2023-08-02 19:17:24.000000 resoto-plugin-azure-3.6.5/resoto_plugin_azure/resource/compute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:25:08.169901 resoto-plugin-azure-3.6.5/resoto_plugin_azure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-08-02 19:25:08.000000 resoto-plugin-azure-3.6.5/resoto_plugin_azure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-02 19:25:08.000000 resoto-plugin-azure-3.6.5/resoto_plugin_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:25:08.000000 resoto-plugin-azure-3.6.5/resoto_plugin_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-02 19:25:08.000000 resoto-plugin-azure-3.6.5/resoto_plugin_azure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:19:17.000000 resoto-plugin-azure-3.6.5/resoto_plugin_azure.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-02 19:25:08.000000 resoto-plugin-azure-3.6.5/resoto_plugin_azure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-02 19:25:08.000000 resoto-plugin-azure-3.6.5/resoto_plugin_azure.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-02 19:25:08.173902 resoto-plugin-azure-3.6.5/setup.cfg
```

### Comparing `resoto-plugin-azure-3.6.4/PKG-INFO` & `resoto-plugin-azure-3.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-azure
-Version: 3.6.4
+Version: 3.6.5
 Summary: Runs collector plugins and sends the result to resotocore.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/azure
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-azure-3.6.4/pyproject.toml` & `resoto-plugin-azure-3.6.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resoto-plugin-azure"
-version = "3.6.4"
+version = "3.6.5"
 authors = [{name="Some Engineering Inc."}]
 description = "Runs collector plugins and sends the result to resotocore."
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
-    "resotolib==3.6.4",
+    "resotolib==3.6.5",
     "retrying",
     "azure-identity",
     "azure-mgmt-resource"
 ]
 
 [project.entry-points."resoto.plugins"]
 azure = "resoto_plugin_azure:AzureCollectorPlugin"
```

### Comparing `resoto-plugin-azure-3.6.4/resoto_plugin_azure/__init__.py` & `resoto-plugin-azure-3.6.5/resoto_plugin_azure/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-azure-3.6.4/resoto_plugin_azure/azure_client.py` & `resoto-plugin-azure-3.6.5/resoto_plugin_azure/azure_client.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-azure-3.6.4/resoto_plugin_azure/collector.py` & `resoto-plugin-azure-3.6.5/resoto_plugin_azure/collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-azure-3.6.4/resoto_plugin_azure/config.py` & `resoto-plugin-azure-3.6.5/resoto_plugin_azure/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-azure-3.6.4/resoto_plugin_azure/resource/base.py` & `resoto-plugin-azure-3.6.5/resoto_plugin_azure/resource/base.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-azure-3.6.4/resoto_plugin_azure/resource/compute.py` & `resoto-plugin-azure-3.6.5/resoto_plugin_azure/resource/compute.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-azure-3.6.4/resoto_plugin_azure.egg-info/PKG-INFO` & `resoto-plugin-azure-3.6.5/resoto_plugin_azure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-azure
-Version: 3.6.4
+Version: 3.6.5
 Summary: Runs collector plugins and sends the result to resotocore.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/azure
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-azure-3.6.4/resoto_plugin_azure.egg-info/SOURCES.txt` & `resoto-plugin-azure-3.6.5/resoto_plugin_azure.egg-info/SOURCES.txt`

 * *Files identical despite different names*


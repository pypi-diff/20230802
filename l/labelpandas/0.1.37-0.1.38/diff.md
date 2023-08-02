# Comparing `tmp/labelpandas-0.1.37.tar.gz` & `tmp/labelpandas-0.1.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelpandas-0.1.37.tar", last modified: Tue Aug  1 21:27:20 2023, max compression
+gzip compressed data, was "labelpandas-0.1.38.tar", last modified: Wed Aug  2 18:46:51 2023, max compression
```

## Comparing `labelpandas-0.1.37.tar` & `labelpandas-0.1.38.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:27:20.431673 labelpandas-0.1.37/
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-08-01 21:27:20.431673 labelpandas-0.1.37/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-08-01 21:27:06.000000 labelpandas-0.1.37/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:27:20.431673 labelpandas-0.1.37/labelpandas/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-01 21:27:09.000000 labelpandas-0.1.37/labelpandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-08-01 21:27:09.000000 labelpandas-0.1.37/labelpandas/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-08-01 21:27:09.000000 labelpandas-0.1.37/labelpandas/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-08-01 21:27:09.000000 labelpandas-0.1.37/labelpandas/load_local_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    17044 2023-08-01 21:27:09.000000 labelpandas-0.1.37/labelpandas/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:27:20.431673 labelpandas-0.1.37/labelpandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-08-01 21:27:20.000000 labelpandas-0.1.37/labelpandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-01 21:27:20.000000 labelpandas-0.1.37/labelpandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 21:27:20.000000 labelpandas-0.1.37/labelpandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 21:27:20.000000 labelpandas-0.1.37/labelpandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 21:27:20.000000 labelpandas-0.1.37/labelpandas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 21:27:20.431673 labelpandas-0.1.37/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-01 21:27:09.000000 labelpandas-0.1.37/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:46:51.693026 labelpandas-0.1.38/
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-08-02 18:46:51.693026 labelpandas-0.1.38/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-08-02 18:46:39.000000 labelpandas-0.1.38/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:46:51.689026 labelpandas-0.1.38/labelpandas/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-02 18:46:42.000000 labelpandas-0.1.38/labelpandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24268 2023-08-02 18:46:42.000000 labelpandas-0.1.38/labelpandas/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-08-02 18:46:42.000000 labelpandas-0.1.38/labelpandas/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-08-02 18:46:42.000000 labelpandas-0.1.38/labelpandas/load_local_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17044 2023-08-02 18:46:42.000000 labelpandas-0.1.38/labelpandas/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:46:51.693026 labelpandas-0.1.38/labelpandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-08-02 18:46:51.000000 labelpandas-0.1.38/labelpandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-02 18:46:51.000000 labelpandas-0.1.38/labelpandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 18:46:51.000000 labelpandas-0.1.38/labelpandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 18:46:51.000000 labelpandas-0.1.38/labelpandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-02 18:46:51.000000 labelpandas-0.1.38/labelpandas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 18:46:51.693026 labelpandas-0.1.38/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-02 18:46:42.000000 labelpandas-0.1.38/setup.py
```

### Comparing `labelpandas-0.1.37/PKG-INFO` & `labelpandas-0.1.38/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelpandas
-Version: 0.1.37
+Version: 0.1.38
 Summary: Labelbox Connector for Pandas
 Home-page: https://github.com/Labelbox/labelpandas
 Author: Labelbox
 Author-email: raphael@labelbox.com
 Description-Content-Type: text/markdown
 
 # The Official Open-Source Labelbox <> Pandas Python Integration
```

### Comparing `labelpandas-0.1.37/README.md` & `labelpandas-0.1.38/README.md`

 * *Files identical despite different names*

### Comparing `labelpandas-0.1.37/labelpandas/client.py` & `labelpandas-0.1.38/labelpandas/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
                 client=self.lb_client, upload_dict=upload_dict, 
                 priority=priority, verbose=verbose
             )                
         else:
             batch_to_project_results = []
             
         # If performing actions that require data row IDs, we pull them here using labelbase.uploader.create_global_key_to_data_row_id_dict
-        if actions["annotate"] or actions["prediction"]:
+        if actions["annotate"] or actions["predictions"]:
             global_key_to_data_row_id = create_global_key_to_data_row_id_dict(
                 client=self.lb_client, global_keys=list(upload_dict.keys())
             )            
         
         # Annotation upload attempt using labelbase.uploader.batch_upload_annotations
         if actions["annotate"]:
             annotation_upload_results = batch_upload_annotations(
```

### Comparing `labelpandas-0.1.37/labelpandas/connector.py` & `labelpandas-0.1.38/labelpandas/connector.py`

 * *Files identical despite different names*

### Comparing `labelpandas-0.1.37/labelpandas/load_local_files.py` & `labelpandas-0.1.38/labelpandas/load_local_files.py`

 * *Files identical despite different names*

### Comparing `labelpandas-0.1.37/labelpandas/uploader.py` & `labelpandas-0.1.38/labelpandas/uploader.py`

 * *Files identical despite different names*

### Comparing `labelpandas-0.1.37/labelpandas.egg-info/PKG-INFO` & `labelpandas-0.1.38/labelpandas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelpandas
-Version: 0.1.37
+Version: 0.1.38
 Summary: Labelbox Connector for Pandas
 Home-page: https://github.com/Labelbox/labelpandas
 Author: Labelbox
 Author-email: raphael@labelbox.com
 Description-Content-Type: text/markdown
 
 # The Official Open-Source Labelbox <> Pandas Python Integration
```

### Comparing `labelpandas-0.1.37/setup.py` & `labelpandas-0.1.38/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='labelpandas',
-    version='0.1.37',
+    version='0.1.38',
     author='Labelbox',
     author_email="raphael@labelbox.com",
     description='Labelbox Connector for Pandas',
     long_description=long_description,
     long_description_content_type="text/markdown",    
     url='https://github.com/Labelbox/labelpandas',    
     packages=find_packages(),
```


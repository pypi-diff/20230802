# Comparing `tmp/labelbase-0.1.3.tar.gz` & `tmp/labelbase-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelbase-0.1.3.tar", last modified: Fri Jul 21 16:59:54 2023, max compression
+gzip compressed data, was "labelbase-0.1.4.tar", last modified: Wed Aug  2 17:25:55 2023, max compression
```

## Comparing `labelbase-0.1.3.tar` & `labelbase-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:59:54.831920 labelbase-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-21 16:59:43.000000 labelbase-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-21 16:59:54.831920 labelbase-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-21 16:59:43.000000 labelbase-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:59:54.831920 labelbase-0.1.3/labelbase/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-21 16:59:43.000000 labelbase-0.1.3/labelbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26651 2023-07-21 16:59:43.000000 labelbase-0.1.3/labelbase/annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-07-21 16:59:43.000000 labelbase-0.1.3/labelbase/connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:59:54.831920 labelbase-0.1.3/labelbase/converters/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-21 16:59:43.000000 labelbase-0.1.3/labelbase/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-07-21 16:59:43.000000 labelbase-0.1.3/labelbase/converters/coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-21 16:59:43.000000 labelbase-0.1.3/labelbase/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-07-21 16:59:43.000000 labelbase-0.1.3/labelbase/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-21 16:59:43.000000 labelbase-0.1.3/labelbase/masks.py
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-07-21 16:59:43.000000 labelbase-0.1.3/labelbase/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-21 16:59:43.000000 labelbase-0.1.3/labelbase/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-07-21 16:59:43.000000 labelbase-0.1.3/labelbase/ontology.py
--rw-r--r--   0 runner    (1001) docker     (123)    25499 2023-07-21 16:59:43.000000 labelbase-0.1.3/labelbase/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:59:54.831920 labelbase-0.1.3/labelbase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-21 16:59:54.000000 labelbase-0.1.3/labelbase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-21 16:59:54.000000 labelbase-0.1.3/labelbase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 16:59:54.000000 labelbase-0.1.3/labelbase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-21 16:59:54.000000 labelbase-0.1.3/labelbase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 16:59:54.000000 labelbase-0.1.3/labelbase.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 16:59:54.831920 labelbase-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-21 16:59:43.000000 labelbase-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:25:55.370760 labelbase-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-02 17:25:44.000000 labelbase-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-02 17:25:55.366760 labelbase-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-08-02 17:25:44.000000 labelbase-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:25:55.362760 labelbase-0.1.4/labelbase/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-02 17:25:44.000000 labelbase-0.1.4/labelbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26651 2023-08-02 17:25:44.000000 labelbase-0.1.4/labelbase/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-08-02 17:25:44.000000 labelbase-0.1.4/labelbase/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:25:55.366760 labelbase-0.1.4/labelbase/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 17:25:44.000000 labelbase-0.1.4/labelbase/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-08-02 17:25:44.000000 labelbase-0.1.4/labelbase/converters/coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-08-02 17:25:44.000000 labelbase-0.1.4/labelbase/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-08-02 17:25:44.000000 labelbase-0.1.4/labelbase/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-08-02 17:25:44.000000 labelbase-0.1.4/labelbase/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-08-02 17:25:44.000000 labelbase-0.1.4/labelbase/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-08-02 17:25:44.000000 labelbase-0.1.4/labelbase/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-08-02 17:25:44.000000 labelbase-0.1.4/labelbase/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25499 2023-08-02 17:25:44.000000 labelbase-0.1.4/labelbase/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:25:55.366760 labelbase-0.1.4/labelbase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-02 17:25:55.000000 labelbase-0.1.4/labelbase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-02 17:25:55.000000 labelbase-0.1.4/labelbase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:25:55.000000 labelbase-0.1.4/labelbase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-02 17:25:55.000000 labelbase-0.1.4/labelbase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-02 17:25:55.000000 labelbase-0.1.4/labelbase.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 17:25:55.370760 labelbase-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-02 17:25:44.000000 labelbase-0.1.4/setup.py
```

### Comparing `labelbase-0.1.3/LICENSE` & `labelbase-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `labelbase-0.1.3/PKG-INFO` & `labelbase-0.1.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelbase
-Version: 0.1.3
+Version: 0.1.4
 Summary: Labelbox Helper Library
 Home-page: https://labelbox.com
 Author: Labelbox
 Author-email: raphael@labelbox.com
 Keywords: labelbox,labelbase
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `labelbase-0.1.3/labelbase/annotate.py` & `labelbase-0.1.4/labelbase/annotate.py`

 * *Files identical despite different names*

### Comparing `labelbase-0.1.3/labelbase/connector.py` & `labelbase-0.1.4/labelbase/connector.py`

 * *Files identical despite different names*

### Comparing `labelbase-0.1.3/labelbase/converters/coco.py` & `labelbase-0.1.4/labelbase/converters/coco.py`

 * *Files identical despite different names*

### Comparing `labelbase-0.1.3/labelbase/dataset.py` & `labelbase-0.1.4/labelbase/dataset.py`

 * *Files identical despite different names*

### Comparing `labelbase-0.1.3/labelbase/downloader.py` & `labelbase-0.1.4/labelbase/downloader.py`

 * *Files identical despite different names*

### Comparing `labelbase-0.1.3/labelbase/masks.py` & `labelbase-0.1.4/labelbase/masks.py`

 * *Files identical despite different names*

### Comparing `labelbase-0.1.3/labelbase/metadata.py` & `labelbase-0.1.4/labelbase/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,17 +126,17 @@
     # By metadata type
     if metadata_type == "enum": # For enums, it must be a schema ID - if we can't match it, we have to skip it
         name_key = f"{parent_name}{divider}{str(metadata_value)}"
         if name_key in metadata_name_key_to_schema.keys():
             return_value = str(metadata_name_key_to_schema[name_key])
         else:
             return_value = None                  
-    elif metadata_type == "number": # For numbers, it's ints as strings
+    elif metadata_type == "number": # For numbers, it's floats as strings
         try:
-            return_value = str(int(metadata_value))
+            return_value = str(float(metadata_value))
         except:
             return_value = None                  
     elif metadata_type == "string": 
         return_value = str(metadata_value)
     else: # For datetime, it's an isoformat string
         if type(metadata_value) == str:
             metadata_value = parser.parse(metadata_value)
```

### Comparing `labelbase-0.1.3/labelbase/models.py` & `labelbase-0.1.4/labelbase/models.py`

 * *Files identical despite different names*

### Comparing `labelbase-0.1.3/labelbase/ontology.py` & `labelbase-0.1.4/labelbase/ontology.py`

 * *Files identical despite different names*

### Comparing `labelbase-0.1.3/labelbase/uploader.py` & `labelbase-0.1.4/labelbase/uploader.py`

 * *Files identical despite different names*

### Comparing `labelbase-0.1.3/labelbase.egg-info/PKG-INFO` & `labelbase-0.1.4/labelbase.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelbase
-Version: 0.1.3
+Version: 0.1.4
 Summary: Labelbox Helper Library
 Home-page: https://labelbox.com
 Author: Labelbox
 Author-email: raphael@labelbox.com
 Keywords: labelbox,labelbase
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `labelbase-0.1.3/setup.py` & `labelbase-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
       name='labelbase',
-      version='0.1.03',
+      version='0.1.04',
       author='Labelbox',
       author_email='raphael@labelbox.com',
       description='Labelbox Helper Library',      
       packages=setuptools.find_packages(),
       url="https://labelbox.com",
       long_description=long_description,
       long_description_content_type="text/markdown",
```


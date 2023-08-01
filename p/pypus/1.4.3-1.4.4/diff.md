# Comparing `tmp/pypus-1.4.3.tar.gz` & `tmp/pypus-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypus-1.4.3.tar", max compression
+gzip compressed data, was "pypus-1.4.4.tar", max compression
```

## Comparing `pypus-1.4.3.tar` & `pypus-1.4.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2021-05-28 19:35:21.744187 pypus-1.4.3/LICENSE
--rw-r--r--   0        0        0      104 2023-08-01 16:02:31.723883 pypus-1.4.3/README.md
--rw-r--r--   0        0        0      629 2023-08-01 16:14:46.780146 pypus-1.4.3/pyproject.toml
--rw-r--r--   0        0        0      937 2023-07-31 18:46:58.056574 pypus-1.4.3/src/pypus/Octo.py
--rw-r--r--   0        0        0        0 2021-05-11 19:37:09.641525 pypus-1.4.3/src/pypus/__init__.py
--rw-r--r--   0        0        0    33323 2023-08-01 16:13:54.300487 pypus-1.4.3/src/pypus/cli.py
--rw-r--r--   0        0        0      601 2023-07-31 21:09:19.484807 pypus-1.4.3/src/pypus/shelf.py
--rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 pypus-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2021-05-28 19:35:21.000000 pypus-1.4.4/LICENSE
+-rw-r--r--   0        0        0      104 2023-08-01 16:02:31.000000 pypus-1.4.4/README.md
+-rw-r--r--   0        0        0      721 2023-08-01 22:36:30.322671 pypus-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0      937 2023-07-31 18:46:58.000000 pypus-1.4.4/src/pypus/Octo.py
+-rw-r--r--   0        0        0        0 2021-05-11 19:37:09.000000 pypus-1.4.4/src/pypus/__init__.py
+-rw-r--r--   0        0        0    33379 2023-08-01 21:23:28.000000 pypus-1.4.4/src/pypus/cli.py
+-rw-r--r--   0        0        0      601 2023-07-31 21:09:19.000000 pypus-1.4.4/src/pypus/shelf.py
+-rw-r--r--   0        0        0      846 1970-01-01 00:00:00.000000 pypus-1.4.4/PKG-INFO
```

### Comparing `pypus-1.4.3/LICENSE` & `pypus-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypus-1.4.3/pyproject.toml` & `pypus-1.4.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 [tool.poetry]
 name = "pypus"
-version = "1.4.3"
+version = "1.4.4"
 description = "Octopus cli toolkit"
-authors = ["Michael MacKenna <mmackenna@unitedfiregroup.com>"]
+authors = ["Michael MacKenna <mpmackenna@gmail.com>"]
 license = "MIT"
 readme = "README.md"
+homepage = "https://mpmackenna.github.io/pypus"
+documentation = "https://mpmackenna.github.io/pypus"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.25.1"
 click = "^8.0.0"
 termcolor = "^1.1.0"
 pyyaml = "^6.0.1"
```

### Comparing `pypus-1.4.3/src/pypus/Octo.py` & `pypus-1.4.4/src/pypus/Octo.py`

 * *Files identical despite different names*

### Comparing `pypus-1.4.3/src/pypus/cli.py` & `pypus-1.4.4/src/pypus/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -690,18 +690,20 @@
 @click.argument('yaml-map-file', type=click.Path(exists=True))
 @click.argument('new-shelf')
 def transpose_from_shelf(shelf_name, key_name, yaml_map_file, new_shelf):
     """ Takes variables from a shelf and transposes Scope Values
     based on a provided map from a yaml file. New values are written
     to a new shelf file.
 
+    Example: yaml-map-file image in documentation
+
     Arguments:
         shelf-name: The current shelf that holds the variables
         key-name: The key that holds the variables to transpose
-        yaml-map: The yaml file with the mapped values
+        yaml-map-file: The yaml file with the mapped values
         new-shelf: The new shelf created with the transposed values
 
     """
     object_list = []
     var_dicts = []
     contents = shelf.get_shelf_item(shelf_name, key_name)
     with open(yaml_map_file, 'r') as stream:
```

### Comparing `pypus-1.4.3/src/pypus/shelf.py` & `pypus-1.4.4/src/pypus/shelf.py`

 * *Files identical despite different names*

### Comparing `pypus-1.4.3/PKG-INFO` & `pypus-1.4.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: pypus
-Version: 1.4.3
+Version: 1.4.4
 Summary: Octopus cli toolkit
+Home-page: https://mpmackenna.github.io/pypus
 License: MIT
 Author: Michael MacKenna
-Author-email: mmackenna@unitedfiregroup.com
+Author-email: mpmackenna@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.0.0,<9.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
+Project-URL: Documentation, https://mpmackenna.github.io/pypus
 Description-Content-Type: text/markdown
 
 # Pypus
 
 Pypus is a cli tool for Octopus Deploy API tasks.
 
 ## Install
```


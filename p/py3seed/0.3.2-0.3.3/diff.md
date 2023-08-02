# Comparing `tmp/py3seed-0.3.2.tar.gz` & `tmp/py3seed-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3seed-0.3.2.tar", last modified: Wed Aug  2 05:16:59 2023, max compression
+gzip compressed data, was "py3seed-0.3.3.tar", last modified: Wed Aug  2 06:17:03 2023, max compression
```

## Comparing `py3seed-0.3.2.tar` & `py3seed-0.3.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-02 05:16:59.890281 py3seed-0.3.2/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.3.2/LICENSE
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-08-02 05:16:59.890515 py3seed-0.3.2/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.3.2/README.md
--rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.3.2/pyproject.toml
--rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-08-02 05:16:59.892087 py3seed-0.3.2/setup.cfg
--rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.3.2/setup.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-02 05:16:59.860612 py3seed-0.3.2/src/
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-02 05:16:59.876571 py3seed-0.3.2/src/py3seed/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.3.2/src/py3seed/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.3.2/src/py3seed/__main__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.3.2/src/py3seed/admin.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     7571 2023-07-21 09:02:47.000000 py3seed-0.3.2/src/py3seed/cachesupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-02 05:16:59.884091 py3seed-0.3.2/src/py3seed/commands/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.3.2/src/py3seed/commands/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    22680 2023-08-02 04:10:01.000000 py3seed-0.3.2/src/py3seed/commands/gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.3.2/src/py3seed/error.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.3.2/src/py3seed/inflection.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.3.2/src/py3seed/log.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.3.2/src/py3seed/merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    57700 2023-07-31 04:55:20.000000 py3seed-0.3.2/src/py3seed/model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.3.2/src/py3seed/mongosupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14654 2023-08-02 02:06:33.000000 py3seed-0.3.2/src/py3seed/utils.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.3.2/src/py3seed/websupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-02 05:16:59.880406 py3seed-0.3.2/src/py3seed.egg-info/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-08-02 05:16:59.000000 py3seed-0.3.2/src/py3seed.egg-info/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-08-02 05:16:59.000000 py3seed-0.3.2/src/py3seed.egg-info/SOURCES.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-08-02 05:16:59.000000 py3seed-0.3.2/src/py3seed.egg-info/dependency_links.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-08-02 05:16:59.000000 py3seed-0.3.2/src/py3seed.egg-info/entry_points.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-08-02 05:16:59.000000 py3seed-0.3.2/src/py3seed.egg-info/requires.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-08-02 05:16:59.000000 py3seed-0.3.2/src/py3seed.egg-info/top_level.txt
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-02 05:16:59.889500 py3seed-0.3.2/tests/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     4032 2023-07-21 09:03:11.000000 py3seed-0.3.2/tests/test_cachesupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     6832 2023-07-31 12:50:18.000000 py3seed-0.3.2/tests/test_gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.3.2/tests/test_merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.3.2/tests/test_model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.3.2/tests/test_mongosupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-02 06:17:03.068670 py3seed-0.3.3/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.3.3/LICENSE
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-08-02 06:17:03.068834 py3seed-0.3.3/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.3.3/README.md
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.3.3/pyproject.toml
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-08-02 06:17:03.069778 py3seed-0.3.3/setup.cfg
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.3.3/setup.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-02 06:17:03.037302 py3seed-0.3.3/src/
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-02 06:17:03.060013 py3seed-0.3.3/src/py3seed/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.3.3/src/py3seed/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.3.3/src/py3seed/__main__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.3.3/src/py3seed/admin.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7571 2023-07-21 09:02:47.000000 py3seed-0.3.3/src/py3seed/cachesupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-02 06:17:03.064123 py3seed-0.3.3/src/py3seed/commands/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.3.3/src/py3seed/commands/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    22791 2023-08-02 06:16:01.000000 py3seed-0.3.3/src/py3seed/commands/gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.3.3/src/py3seed/error.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.3.3/src/py3seed/inflection.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.3.3/src/py3seed/log.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.3.3/src/py3seed/merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    57700 2023-07-31 04:55:20.000000 py3seed-0.3.3/src/py3seed/model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.3.3/src/py3seed/mongosupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14654 2023-08-02 02:06:33.000000 py3seed-0.3.3/src/py3seed/utils.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.3.3/src/py3seed/websupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-02 06:17:03.063123 py3seed-0.3.3/src/py3seed.egg-info/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-08-02 06:17:03.000000 py3seed-0.3.3/src/py3seed.egg-info/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-08-02 06:17:03.000000 py3seed-0.3.3/src/py3seed.egg-info/SOURCES.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-08-02 06:17:03.000000 py3seed-0.3.3/src/py3seed.egg-info/dependency_links.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-08-02 06:17:03.000000 py3seed-0.3.3/src/py3seed.egg-info/entry_points.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-08-02 06:17:03.000000 py3seed-0.3.3/src/py3seed.egg-info/requires.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-08-02 06:17:03.000000 py3seed-0.3.3/src/py3seed.egg-info/top_level.txt
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-02 06:17:03.067810 py3seed-0.3.3/tests/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     4032 2023-07-21 09:03:11.000000 py3seed-0.3.3/tests/test_cachesupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     6832 2023-07-31 12:50:18.000000 py3seed-0.3.3/tests/test_gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.3.3/tests/test_merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.3.3/tests/test_model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.3.3/tests/test_mongosupport.py
```

### Comparing `py3seed-0.3.2/LICENSE` & `py3seed-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.2/PKG-INFO` & `py3seed-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.3.2
+Version: 0.3.3
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.3.2/setup.cfg` & `py3seed-0.3.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py3seed
-version = 0.3.2
+version = 0.3.3
 author = Samuel Feng
 author_email = okosioc@gmail.com
 description = A package that bootstraps your project by simple data models definition and auto api and user interface generation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/okosioc/pyseed
 project_urls =
```

### Comparing `py3seed-0.3.2/src/py3seed/__init__.py` & `py3seed-0.3.3/src/py3seed/__init__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.2/src/py3seed/__main__.py` & `py3seed-0.3.3/src/py3seed/__main__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.2/src/py3seed/admin.py` & `py3seed-0.3.3/src/py3seed/admin.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.2/src/py3seed/cachesupport.py` & `py3seed-0.3.3/src/py3seed/cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.2/src/py3seed/commands/gen.py` & `py3seed-0.3.3/src/py3seed/commands/gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,21 +32,22 @@
 
 def _prepare_jinja2_env():
     """ Prepare env for rendering jinja2 templates. """
     #
     # For more env setting, please refer to https://jinja.palletsprojects.com/en/3.0.x/api/#jinja2.Environment
     # - trim_blocks=True, the first newline after a block is removed (block, not variable tag!)
     # - lstrip_blocks=True, leading spaces and tabs are stripped from the start of a line to a block
+    # - keep_trailing_newline=True, Preserve the trailing newline when rendering templates
     #
     # trim_blocks=True and lstrip_blocks=True -> make sure lines of {% ... %} and {# ... #} will be removed completely in render result
     #
-    # For extension loopcontrols, please refer to https://jinja.palletsprojects.com/en/3.0.x/extensions/#loopcontrols-extension
-    # -> you can use break, continue in for loop
+    # For extension, plrease refer to https://jinja.palletsprojects.com/en/3.0.x/extensions/
+    # - jinja2.ext.loopcontrols, add break and continue support in for loop
     #
-    env = Environment(trim_blocks=True, lstrip_blocks=True, extensions=['jinja2.ext.loopcontrols'])
+    env = Environment(trim_blocks=True, lstrip_blocks=True, keep_trailing_newline=True, extensions=['jinja2.ext.loopcontrols'])
 
     def update_query(**new_values):
         """ Update query. """
         args = request.args.copy()
         for key, value in new_values.items():
             args[key] = value
         return url_encode(args)
```

### Comparing `py3seed-0.3.2/src/py3seed/error.py` & `py3seed-0.3.3/src/py3seed/error.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.2/src/py3seed/inflection.py` & `py3seed-0.3.3/src/py3seed/inflection.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.2/src/py3seed/log.py` & `py3seed-0.3.3/src/py3seed/log.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.2/src/py3seed/merge3.py` & `py3seed-0.3.3/src/py3seed/merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.2/src/py3seed/model.py` & `py3seed-0.3.3/src/py3seed/model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.2/src/py3seed/mongosupport.py` & `py3seed-0.3.3/src/py3seed/mongosupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.2/src/py3seed/utils.py` & `py3seed-0.3.3/src/py3seed/utils.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.2/src/py3seed/websupport.py` & `py3seed-0.3.3/src/py3seed/websupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.2/src/py3seed.egg-info/PKG-INFO` & `py3seed-0.3.3/src/py3seed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.3.2
+Version: 0.3.3
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.3.2/src/py3seed.egg-info/SOURCES.txt` & `py3seed-0.3.3/src/py3seed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.2/tests/test_cachesupport.py` & `py3seed-0.3.3/tests/test_cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.2/tests/test_gen.py` & `py3seed-0.3.3/tests/test_gen.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.2/tests/test_merge3.py` & `py3seed-0.3.3/tests/test_merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.2/tests/test_model.py` & `py3seed-0.3.3/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.2/tests/test_mongosupport.py` & `py3seed-0.3.3/tests/test_mongosupport.py`

 * *Files identical despite different names*


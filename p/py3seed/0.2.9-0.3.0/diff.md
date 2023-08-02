# Comparing `tmp/py3seed-0.2.9.tar.gz` & `tmp/py3seed-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3seed-0.2.9.tar", last modified: Tue Aug  1 08:50:26 2023, max compression
+gzip compressed data, was "py3seed-0.3.0.tar", last modified: Wed Aug  2 02:28:35 2023, max compression
```

## Comparing `py3seed-0.2.9.tar` & `py3seed-0.3.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-01 08:50:26.741783 py3seed-0.2.9/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.2.9/LICENSE
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-08-01 08:50:26.741918 py3seed-0.2.9/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.2.9/README.md
--rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.2.9/pyproject.toml
--rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-08-01 08:50:26.742534 py3seed-0.2.9/setup.cfg
--rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.2.9/setup.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-01 08:50:26.715424 py3seed-0.2.9/src/
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-01 08:50:26.730803 py3seed-0.2.9/src/py3seed/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.2.9/src/py3seed/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.2.9/src/py3seed/__main__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.2.9/src/py3seed/admin.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     7571 2023-07-21 09:02:47.000000 py3seed-0.2.9/src/py3seed/cachesupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-01 08:50:26.734623 py3seed-0.2.9/src/py3seed/commands/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.2.9/src/py3seed/commands/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    22949 2023-08-01 08:49:28.000000 py3seed-0.2.9/src/py3seed/commands/gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.2.9/src/py3seed/error.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.2.9/src/py3seed/inflection.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.2.9/src/py3seed/log.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.2.9/src/py3seed/merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    57700 2023-07-31 04:55:20.000000 py3seed-0.2.9/src/py3seed/model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.2.9/src/py3seed/mongosupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14651 2023-07-27 13:10:29.000000 py3seed-0.2.9/src/py3seed/utils.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.2.9/src/py3seed/websupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-01 08:50:26.733484 py3seed-0.2.9/src/py3seed.egg-info/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-08-01 08:50:26.000000 py3seed-0.2.9/src/py3seed.egg-info/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-08-01 08:50:26.000000 py3seed-0.2.9/src/py3seed.egg-info/SOURCES.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-08-01 08:50:26.000000 py3seed-0.2.9/src/py3seed.egg-info/dependency_links.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-08-01 08:50:26.000000 py3seed-0.2.9/src/py3seed.egg-info/entry_points.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-08-01 08:50:26.000000 py3seed-0.2.9/src/py3seed.egg-info/requires.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-08-01 08:50:26.000000 py3seed-0.2.9/src/py3seed.egg-info/top_level.txt
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-01 08:50:26.741102 py3seed-0.2.9/tests/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     4032 2023-07-21 09:03:11.000000 py3seed-0.2.9/tests/test_cachesupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     6832 2023-07-31 12:50:18.000000 py3seed-0.2.9/tests/test_gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.2.9/tests/test_merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.2.9/tests/test_model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.2.9/tests/test_mongosupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-02 02:28:34.997338 py3seed-0.3.0/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.3.0/LICENSE
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-08-02 02:28:34.997504 py3seed-0.3.0/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.3.0/README.md
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.3.0/pyproject.toml
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-08-02 02:28:34.998232 py3seed-0.3.0/setup.cfg
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.3.0/setup.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-02 02:28:34.973247 py3seed-0.3.0/src/
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-02 02:28:34.988107 py3seed-0.3.0/src/py3seed/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.3.0/src/py3seed/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.3.0/src/py3seed/__main__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.3.0/src/py3seed/admin.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7571 2023-07-21 09:02:47.000000 py3seed-0.3.0/src/py3seed/cachesupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-02 02:28:34.992387 py3seed-0.3.0/src/py3seed/commands/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.3.0/src/py3seed/commands/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    22847 2023-08-02 02:26:16.000000 py3seed-0.3.0/src/py3seed/commands/gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.3.0/src/py3seed/error.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.3.0/src/py3seed/inflection.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.3.0/src/py3seed/log.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.3.0/src/py3seed/merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    57700 2023-07-31 04:55:20.000000 py3seed-0.3.0/src/py3seed/model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.3.0/src/py3seed/mongosupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14654 2023-08-02 02:06:33.000000 py3seed-0.3.0/src/py3seed/utils.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.3.0/src/py3seed/websupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-02 02:28:34.991214 py3seed-0.3.0/src/py3seed.egg-info/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-08-02 02:28:34.000000 py3seed-0.3.0/src/py3seed.egg-info/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-08-02 02:28:34.000000 py3seed-0.3.0/src/py3seed.egg-info/SOURCES.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-08-02 02:28:34.000000 py3seed-0.3.0/src/py3seed.egg-info/dependency_links.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-08-02 02:28:34.000000 py3seed-0.3.0/src/py3seed.egg-info/entry_points.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-08-02 02:28:34.000000 py3seed-0.3.0/src/py3seed.egg-info/requires.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-08-02 02:28:34.000000 py3seed-0.3.0/src/py3seed.egg-info/top_level.txt
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-02 02:28:34.996766 py3seed-0.3.0/tests/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     4032 2023-07-21 09:03:11.000000 py3seed-0.3.0/tests/test_cachesupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     6832 2023-07-31 12:50:18.000000 py3seed-0.3.0/tests/test_gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.3.0/tests/test_merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.3.0/tests/test_model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.3.0/tests/test_mongosupport.py
```

### Comparing `py3seed-0.2.9/LICENSE` & `py3seed-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.9/PKG-INFO` & `py3seed-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.2.9
+Version: 0.3.0
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.2.9/setup.cfg` & `py3seed-0.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py3seed
-version = 0.2.9
+version = 0.3.0
 author = Samuel Feng
 author_email = okosioc@gmail.com
 description = A package that bootstraps your project by simple data models definition and auto api and user interface generation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/okosioc/pyseed
 project_urls =
```

### Comparing `py3seed-0.2.9/src/py3seed/__init__.py` & `py3seed-0.3.0/src/py3seed/__init__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.9/src/py3seed/__main__.py` & `py3seed-0.3.0/src/py3seed/__main__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.9/src/py3seed/admin.py` & `py3seed-0.3.0/src/py3seed/admin.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.9/src/py3seed/cachesupport.py` & `py3seed-0.3.0/src/py3seed/cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.9/src/py3seed/commands/gen.py` & `py3seed-0.3.0/src/py3seed/commands/gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,17 +240,14 @@
                     'domains': domains,
                     'action': l['action'],
                     'params': l['params'],
                     'rows': l['rows'],
                     'layout': layout,  # NOTE: layout stores the original layout string, parsed layout is stored in rows
                     **generate_names(name)
                 })
-            # Views may be empty if no views match
-            if not views:
-                continue
             #
             model_setting['views'] = views
             model_settings[model_name] = model_setting
     #
     if not model_settings:
         logger.error('Can not find any models to gen')
         return False
```

### Comparing `py3seed-0.2.9/src/py3seed/error.py` & `py3seed-0.3.0/src/py3seed/error.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.9/src/py3seed/inflection.py` & `py3seed-0.3.0/src/py3seed/inflection.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.9/src/py3seed/log.py` & `py3seed-0.3.0/src/py3seed/log.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.9/src/py3seed/merge3.py` & `py3seed-0.3.0/src/py3seed/merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.9/src/py3seed/model.py` & `py3seed-0.3.0/src/py3seed/model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.9/src/py3seed/mongosupport.py` & `py3seed-0.3.0/src/py3seed/mongosupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.9/src/py3seed/utils.py` & `py3seed-0.3.0/src/py3seed/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,15 +236,15 @@
                         inner_schema = column_schema
                     elif column_type == 'array':
                         inner_schema = column_schema['items'] if column_schema['items']['type'] == 'object' else None
                     #
                     if inner_schema:
                         # Inner layout is optional for inner object
                         if col_lines:
-                            column['rows'] = _parse_lines(level + 1, col_lines, inner_schema)  # Schema passing recursively should always be object
+                            column['rows'] = _parse_lines(level + 1, col_lines, inner_schema)  # Schema passing recursively should always be an object
                     else:
                         if col_lines:
                             raise LayoutError(f'{column_type.capitalize()} field {col_name} can not have inner layout')
                     #
                     column.pop('lines', None)
             #
             _rows.append(columns)
```

### Comparing `py3seed-0.2.9/src/py3seed/websupport.py` & `py3seed-0.3.0/src/py3seed/websupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.9/src/py3seed.egg-info/PKG-INFO` & `py3seed-0.3.0/src/py3seed.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.2.9
+Version: 0.3.0
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.2.9/src/py3seed.egg-info/SOURCES.txt` & `py3seed-0.3.0/src/py3seed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.9/tests/test_cachesupport.py` & `py3seed-0.3.0/tests/test_cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.9/tests/test_gen.py` & `py3seed-0.3.0/tests/test_gen.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.9/tests/test_merge3.py` & `py3seed-0.3.0/tests/test_merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.9/tests/test_model.py` & `py3seed-0.3.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.9/tests/test_mongosupport.py` & `py3seed-0.3.0/tests/test_mongosupport.py`

 * *Files identical despite different names*


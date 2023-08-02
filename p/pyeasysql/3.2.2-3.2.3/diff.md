# Comparing `tmp/pyeasysql-3.2.2.tar.gz` & `tmp/pyeasysql-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeasysql-3.2.2.tar", last modified: Thu Jul 27 19:16:07 2023, max compression
+gzip compressed data, was "pyeasysql-3.2.3.tar", last modified: Wed Aug  2 08:37:27 2023, max compression
```

## Comparing `pyeasysql-3.2.2.tar` & `pyeasysql-3.2.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 19:16:07.844412 pyeasysql-3.2.2/
-drwxrwxrwx   0        0        0        0 2023-07-27 19:16:07.811077 pyeasysql-3.2.2/EasySQL/
--rw-rw-rw-   0        0        0     3662 2023-07-24 11:39:55.000000 pyeasysql-3.2.2/EasySQL/ABC.py
--rw-rw-rw-   0        0        0     2887 2021-06-27 12:24:21.000000 pyeasysql-3.2.2/EasySQL/Characters.py
--rw-rw-rw-   0        0        0    15280 2023-07-27 18:17:08.000000 pyeasysql-3.2.2/EasySQL/Classes.py
--rw-rw-rw-   0        0        0     6202 2023-07-25 17:49:13.000000 pyeasysql-3.2.2/EasySQL/Commands.py
--rw-rw-rw-   0        0        0      945 2023-07-25 08:49:05.000000 pyeasysql-3.2.2/EasySQL/Constraints.py
--rw-rw-rw-   0        0        0      305 2023-07-11 12:44:34.000000 pyeasysql-3.2.2/EasySQL/Decorators.py
--rw-rw-rw-   0        0        0     2097 2023-07-09 09:35:55.000000 pyeasysql-3.2.2/EasySQL/EasyInstances.py
--rw-rw-rw-   0        0        0      757 2023-06-08 19:41:42.000000 pyeasysql-3.2.2/EasySQL/Exceptions.py
--rw-rw-rw-   0        0        0      457 2021-04-04 16:17:30.000000 pyeasysql-3.2.2/EasySQL/Logging.py
--rw-rw-rw-   0        0        0     3079 2023-07-23 11:44:26.000000 pyeasysql-3.2.2/EasySQL/Types.py
--rw-rw-rw-   0        0        0     2496 2022-04-15 06:15:51.000000 pyeasysql-3.2.2/EasySQL/Where.py
--rw-rw-rw-   0        0        0      298 2023-07-24 15:21:11.000000 pyeasysql-3.2.2/EasySQL/__init__.py
--rw-rw-rw-   0        0        0     1085 2023-07-23 15:33:54.000000 pyeasysql-3.2.2/LICENSE.md
--rw-rw-rw-   0        0        0     6084 2023-07-27 19:16:07.838993 pyeasysql-3.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     5412 2023-07-24 15:30:12.000000 pyeasysql-3.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 19:16:07.836451 pyeasysql-3.2.2/pyeasysql.egg-info/
--rw-rw-rw-   0        0        0     6084 2023-07-27 19:16:07.000000 pyeasysql-3.2.2/pyeasysql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2023-07-27 19:16:07.000000 pyeasysql-3.2.2/pyeasysql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 19:16:07.000000 pyeasysql-3.2.2/pyeasysql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-27 19:16:07.000000 pyeasysql-3.2.2/pyeasysql.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-27 19:16:07.000000 pyeasysql-3.2.2/pyeasysql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      717 2023-07-27 16:55:01.000000 pyeasysql-3.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-27 19:16:07.844412 pyeasysql-3.2.2/setup.cfg
--rw-rw-rw-   0        0        0      831 2023-07-24 16:25:04.000000 pyeasysql-3.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:37:27.732017 pyeasysql-3.2.3/
+drwxrwxrwx   0        0        0        0 2023-08-02 08:37:27.717087 pyeasysql-3.2.3/EasySQL/
+-rw-rw-rw-   0        0        0     3662 2023-07-24 11:39:55.000000 pyeasysql-3.2.3/EasySQL/ABC.py
+-rw-rw-rw-   0        0        0     2887 2021-06-27 12:24:21.000000 pyeasysql-3.2.3/EasySQL/Characters.py
+-rw-rw-rw-   0        0        0    15360 2023-07-28 07:59:44.000000 pyeasysql-3.2.3/EasySQL/Classes.py
+-rw-rw-rw-   0        0        0     6202 2023-07-25 17:49:13.000000 pyeasysql-3.2.3/EasySQL/Commands.py
+-rw-rw-rw-   0        0        0      945 2023-07-25 08:49:05.000000 pyeasysql-3.2.3/EasySQL/Constraints.py
+-rw-rw-rw-   0        0        0      305 2023-07-11 12:44:34.000000 pyeasysql-3.2.3/EasySQL/Decorators.py
+-rw-rw-rw-   0        0        0     2097 2023-07-09 09:35:55.000000 pyeasysql-3.2.3/EasySQL/EasyInstances.py
+-rw-rw-rw-   0        0        0      757 2023-06-08 19:41:42.000000 pyeasysql-3.2.3/EasySQL/Exceptions.py
+-rw-rw-rw-   0        0        0      457 2021-04-04 16:17:30.000000 pyeasysql-3.2.3/EasySQL/Logging.py
+-rw-rw-rw-   0        0        0     3079 2023-07-23 11:44:26.000000 pyeasysql-3.2.3/EasySQL/Types.py
+-rw-rw-rw-   0        0        0     2496 2022-04-15 06:15:51.000000 pyeasysql-3.2.3/EasySQL/Where.py
+-rw-rw-rw-   0        0        0      298 2023-07-24 15:21:11.000000 pyeasysql-3.2.3/EasySQL/__init__.py
+-rw-rw-rw-   0        0        0     1085 2023-07-23 15:33:54.000000 pyeasysql-3.2.3/LICENSE.md
+-rw-rw-rw-   0        0        0     6084 2023-08-02 08:37:27.731048 pyeasysql-3.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5412 2023-07-24 15:30:12.000000 pyeasysql-3.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 08:37:27.729028 pyeasysql-3.2.3/pyeasysql.egg-info/
+-rw-rw-rw-   0        0        0     6084 2023-08-02 08:37:27.000000 pyeasysql-3.2.3/pyeasysql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      449 2023-08-02 08:37:27.000000 pyeasysql-3.2.3/pyeasysql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 08:37:27.000000 pyeasysql-3.2.3/pyeasysql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-08-02 08:37:27.000000 pyeasysql-3.2.3/pyeasysql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-02 08:37:27.000000 pyeasysql-3.2.3/pyeasysql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      717 2023-07-28 07:59:44.000000 pyeasysql-3.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-02 08:37:27.732017 pyeasysql-3.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      831 2023-07-24 16:25:04.000000 pyeasysql-3.2.3/setup.py
```

### Comparing `pyeasysql-3.2.2/EasySQL/ABC.py` & `pyeasysql-3.2.3/EasySQL/ABC.py`

 * *Files identical despite different names*

### Comparing `pyeasysql-3.2.2/EasySQL/Characters.py` & `pyeasysql-3.2.3/EasySQL/Characters.py`

 * *Files identical despite different names*

### Comparing `pyeasysql-3.2.2/EasySQL/Classes.py` & `pyeasysql-3.2.3/EasySQL/Classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,16 +259,16 @@
     PRIMARY: List[EasyColumn] = None
     UNIQUES: List[Unique] = None
 
     def __init_subclass__(cls, **kwargs):
         for key in ('database', 'name'):
             setattr(cls, f'_{key}', _safe_pop(kwargs, key) or getattr(cls, f'_{key}'))
 
-        cls.PRIMARY = []
-        cls.UNIQUES = []
+        cls.PRIMARY = [] if cls.PRIMARY is None else cls.PRIMARY
+        cls.UNIQUES = [] if cls.UNIQUES is None else cls.UNIQUES
 
         columns: List[EasyColumn] = [value for value in cls.__dict__.values() if isinstance(value, EasyColumn)]
         for column in columns:
             if UNIQUE in column.tags:
                 cls.UNIQUES.append(Unique(column))
             if PRIMARY in column.tags:
                 cls.PRIMARY.append(column)
```

### Comparing `pyeasysql-3.2.2/EasySQL/Commands.py` & `pyeasysql-3.2.3/EasySQL/Commands.py`

 * *Files identical despite different names*

### Comparing `pyeasysql-3.2.2/EasySQL/Constraints.py` & `pyeasysql-3.2.3/EasySQL/Constraints.py`

 * *Files identical despite different names*

### Comparing `pyeasysql-3.2.2/EasySQL/EasyInstances.py` & `pyeasysql-3.2.3/EasySQL/EasyInstances.py`

 * *Files identical despite different names*

### Comparing `pyeasysql-3.2.2/EasySQL/Exceptions.py` & `pyeasysql-3.2.3/EasySQL/Exceptions.py`

 * *Files identical despite different names*

### Comparing `pyeasysql-3.2.2/EasySQL/Types.py` & `pyeasysql-3.2.3/EasySQL/Types.py`

 * *Files identical despite different names*

### Comparing `pyeasysql-3.2.2/EasySQL/Where.py` & `pyeasysql-3.2.3/EasySQL/Where.py`

 * *Files identical despite different names*

### Comparing `pyeasysql-3.2.2/LICENSE.md` & `pyeasysql-3.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyeasysql-3.2.2/PKG-INFO` & `pyeasysql-3.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyeasysql
-Version: 3.2.2
+Version: 3.2.3
 Summary: SQL Database management without even a SQL line
 Home-page: https://github.com/AGM-Studio/easysql
 Author: Ashenguard
 Author-email: Ashenguard <ashenguard@agmstudio.xyz>
 Project-URL: Homepage, https://github.com/agm-studio/easysql
 Project-URL: Bug Tracker, https://github.com/agm-studio/easysql/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyeasysql-3.2.2/README.md` & `pyeasysql-3.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pyeasysql-3.2.2/pyeasysql.egg-info/PKG-INFO` & `pyeasysql-3.2.3/pyeasysql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyeasysql
-Version: 3.2.2
+Version: 3.2.3
 Summary: SQL Database management without even a SQL line
 Home-page: https://github.com/AGM-Studio/easysql
 Author: Ashenguard
 Author-email: Ashenguard <ashenguard@agmstudio.xyz>
 Project-URL: Homepage, https://github.com/agm-studio/easysql
 Project-URL: Bug Tracker, https://github.com/agm-studio/easysql/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyeasysql-3.2.2/pyproject.toml` & `pyeasysql-3.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyeasysql"
-version = "3.2.2"
+version = "3.2.3"
 authors = [
   { name="Ashenguard", email="ashenguard@agmstudio.xyz" },
 ]
 description = "SQL Database management without even a SQL line"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `pyeasysql-3.2.2/setup.py` & `pyeasysql-3.2.3/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/session-repository-0.3.6.tar.gz` & `tmp/session-repository-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "session-repository-0.3.6.tar", last modified: Tue Aug  1 22:08:52 2023, max compression
+gzip compressed data, was "session-repository-0.3.7.tar", last modified: Wed Aug  2 10:06:07 2023, max compression
```

## Comparing `session-repository-0.3.6.tar` & `session-repository-0.3.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 22:08:52.369881 session-repository-0.3.6/
--rw-rw-rw-   0        0        0      599 2023-08-01 22:08:52.367879 session-repository-0.3.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 22:08:52.316866 session-repository-0.3.6/session_repository/
--rw-rw-rw-   0        0        0      191 2023-07-18 08:45:38.000000 session-repository-0.3.6/session_repository/__init__.py
--rw-rw-rw-   0        0        0      583 2023-07-13 16:45:09.000000 session-repository-0.3.6/session_repository/enum.py
-drwxrwxrwx   0        0        0        0 2023-08-01 22:08:52.362271 session-repository-0.3.6/session_repository/models/
--rw-rw-rw-   0        0        0     9840 2023-08-01 22:07:29.000000 session-repository-0.3.6/session_repository/models/repository.py
--rw-rw-rw-   0        0        0      496 2023-07-18 09:04:38.000000 session-repository-0.3.6/session_repository/models/service.py
--rw-rw-rw-   0        0        0     9582 2023-07-24 19:16:34.000000 session-repository-0.3.6/session_repository/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-01 22:08:52.348051 session-repository-0.3.6/session_repository.egg-info/
--rw-rw-rw-   0        0        0      599 2023-08-01 22:08:52.000000 session-repository-0.3.6/session_repository.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      380 2023-08-01 22:08:52.000000 session-repository-0.3.6/session_repository.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 22:08:52.000000 session-repository-0.3.6/session_repository.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-08-01 22:08:52.000000 session-repository-0.3.6/session_repository.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-08-01 22:08:52.000000 session-repository-0.3.6/session_repository.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 22:08:52.370878 session-repository-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0      877 2023-08-01 22:00:13.000000 session-repository-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:06:07.413810 session-repository-0.3.7/
+-rw-rw-rw-   0        0        0      599 2023-08-02 10:06:07.410912 session-repository-0.3.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-02 10:06:07.371794 session-repository-0.3.7/session_repository/
+-rw-rw-rw-   0        0        0      191 2023-07-18 08:45:38.000000 session-repository-0.3.7/session_repository/__init__.py
+-rw-rw-rw-   0        0        0      583 2023-07-13 16:45:09.000000 session-repository-0.3.7/session_repository/enum.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:06:07.407913 session-repository-0.3.7/session_repository/models/
+-rw-rw-rw-   0        0        0     9840 2023-08-01 22:07:29.000000 session-repository-0.3.7/session_repository/models/repository.py
+-rw-rw-rw-   0        0        0      496 2023-07-18 09:04:38.000000 session-repository-0.3.7/session_repository/models/service.py
+-rw-rw-rw-   0        0        0    10978 2023-08-02 10:05:18.000000 session-repository-0.3.7/session_repository/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:06:07.395781 session-repository-0.3.7/session_repository.egg-info/
+-rw-rw-rw-   0        0        0      599 2023-08-02 10:06:07.000000 session-repository-0.3.7/session_repository.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-08-02 10:06:07.000000 session-repository-0.3.7/session_repository.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 10:06:07.000000 session-repository-0.3.7/session_repository.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-08-02 10:06:07.000000 session-repository-0.3.7/session_repository.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-08-02 10:06:07.000000 session-repository-0.3.7/session_repository.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 10:06:07.415033 session-repository-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      877 2023-08-02 10:05:31.000000 session-repository-0.3.7/setup.py
```

### Comparing `session-repository-0.3.6/PKG-INFO` & `session-repository-0.3.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.3.6
+Version: 0.3.7
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.3.6.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.3.7.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.3.6/session_repository/enum.py` & `session-repository-0.3.7/session_repository/enum.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.3.6/session_repository/models/repository.py` & `session-repository-0.3.7/session_repository/models/repository.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.3.6/session_repository/utils.py` & `session-repository-0.3.7/session_repository/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     Iterable,
     List,
     Tuple,
     Union,
 )
 
 # SQLALCHEMY
-from sqlalchemy import and_, asc, desc, tuple_, func
+from sqlalchemy import and_, asc, desc, tuple_, func, null
 from sqlalchemy.orm import (
     Query,
     InstrumentedAttribute,
     noload,
 )
 from sqlalchemy.sql.elements import Null
 
@@ -149,19 +149,25 @@
                 if with_optional and v is None:
                     continue
 
                 match k:
                     case Operators.EQUAL:
                         conditions.append(key == v)
                     case Operators.IEQUAL:
-                        conditions.append(func.lower(key) == func.lower(v))
+                        if not isinstance(v, Null):
+                            conditions.append(func.lower(key) == func.lower(v))
+                        else:
+                            conditions.append(key == v)
                     case Operators.DIFFERENT:
                         conditions.append(key != v)
                     case Operators.IDIFFERENT:
-                        conditions.append(func.lower(key) != func.lower(v))
+                        if not isinstance(v, Null):
+                            conditions.append(func.lower(key) != func.lower(v))
+                        else:
+                            conditions.append(key != v)
                     case Operators.LIKE:
                         if not isinstance(v, Null):
                             conditions.append(key.like(v))
                         else:
                             conditions.append(key == v)
                     case Operators.NOT_LIKE:
                         if not isinstance(v, Null):
@@ -207,39 +213,63 @@
                         else:
                             conditions.append(key.in_(v))
                     case Operators.IIN:
                         v = v if isinstance(v, Iterable) else [v]
                         if isinstance(key, tuple):
                             conditions.append(
                                 tuple_([func.lower(key_) for key_ in key]).in_(
-                                    [func.lower(v_) for v_ in v]
+                                    [
+                                        func.lower(v_)
+                                        if not isinstance(v_, Null)
+                                        else v_
+                                        for v_ in v
+                                    ]
                                 )
                             )
                         else:
                             conditions.append(
-                                func.lower(key).in_([func.lower(v_) for v_ in v])
+                                func.lower(key).in_(
+                                    [
+                                        func.lower(v_)
+                                        if not isinstance(v_, Null)
+                                        else v_
+                                        for v_ in v
+                                    ]
+                                )
                             )
                     case Operators.NOT_IN:
                         v = v if isinstance(v, Iterable) else [v]
                         if isinstance(key, tuple):
                             conditions.append(tuple_(*key).notin_(v))
                         else:
                             conditions.append(key.notin_(v))
 
                     case Operators.NOT_IIN:
                         v = v if isinstance(v, Iterable) else [v]
                         if isinstance(key, tuple):
                             conditions.append(
                                 tuple_([func.lower(key_) for key_ in key]).notin_(
-                                    [func.lower(v_) for v_ in v]
+                                    [
+                                        func.lower(v_)
+                                        if not isinstance(v_, Null)
+                                        else v_
+                                        for v_ in v
+                                    ]
                                 )
                             )
                         else:
                             conditions.append(
-                                func.lower(key).notin_([func.lower(v_) for v_ in v])
+                                func.lower(key).notin_(
+                                    [
+                                        func.lower(v_)
+                                        if not isinstance(v_, Null)
+                                        else v_
+                                        for v_ in v
+                                    ]
+                                )
                             )
                     case Operators.HAS:
                         v = get_filters(
                             v,
                             with_optional=with_optional,
                         )
                         for condition in v:
```

### Comparing `session-repository-0.3.6/session_repository.egg-info/PKG-INFO` & `session-repository-0.3.7/session_repository.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.3.6
+Version: 0.3.7
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.3.6.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.3.7.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.3.6/setup.py` & `session-repository-0.3.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.3.6"
+version = "0.3.7"
 
 setup(
     name="session-repository",
     version=version,
     packages=[
         "session_repository",
         "session_repository.models",
```


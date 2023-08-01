# Comparing `tmp/session-repository-0.3.5.tar.gz` & `tmp/session-repository-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "session-repository-0.3.5.tar", last modified: Mon Jul 31 17:32:10 2023, max compression
+gzip compressed data, was "session-repository-0.3.6.tar", last modified: Tue Aug  1 22:08:52 2023, max compression
```

## Comparing `session-repository-0.3.5.tar` & `session-repository-0.3.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 17:32:10.596607 session-repository-0.3.5/
--rw-rw-rw-   0        0        0      599 2023-07-31 17:32:10.595024 session-repository-0.3.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-31 17:32:10.564366 session-repository-0.3.5/session_repository/
--rw-rw-rw-   0        0        0      191 2023-07-18 08:45:38.000000 session-repository-0.3.5/session_repository/__init__.py
--rw-rw-rw-   0        0        0      583 2023-07-13 16:45:09.000000 session-repository-0.3.5/session_repository/enum.py
-drwxrwxrwx   0        0        0        0 2023-07-31 17:32:10.591837 session-repository-0.3.5/session_repository/models/
--rw-rw-rw-   0        0        0     9769 2023-07-31 17:30:42.000000 session-repository-0.3.5/session_repository/models/repository.py
--rw-rw-rw-   0        0        0      496 2023-07-18 09:04:38.000000 session-repository-0.3.5/session_repository/models/service.py
--rw-rw-rw-   0        0        0     9582 2023-07-24 19:16:34.000000 session-repository-0.3.5/session_repository/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-31 17:32:10.584137 session-repository-0.3.5/session_repository.egg-info/
--rw-rw-rw-   0        0        0      599 2023-07-31 17:32:10.000000 session-repository-0.3.5/session_repository.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      380 2023-07-31 17:32:10.000000 session-repository-0.3.5/session_repository.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 17:32:10.000000 session-repository-0.3.5/session_repository.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-31 17:32:10.000000 session-repository-0.3.5/session_repository.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-31 17:32:10.000000 session-repository-0.3.5/session_repository.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 17:32:10.598672 session-repository-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0      877 2023-07-31 17:31:55.000000 session-repository-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:08:52.369881 session-repository-0.3.6/
+-rw-rw-rw-   0        0        0      599 2023-08-01 22:08:52.367879 session-repository-0.3.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 22:08:52.316866 session-repository-0.3.6/session_repository/
+-rw-rw-rw-   0        0        0      191 2023-07-18 08:45:38.000000 session-repository-0.3.6/session_repository/__init__.py
+-rw-rw-rw-   0        0        0      583 2023-07-13 16:45:09.000000 session-repository-0.3.6/session_repository/enum.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:08:52.362271 session-repository-0.3.6/session_repository/models/
+-rw-rw-rw-   0        0        0     9840 2023-08-01 22:07:29.000000 session-repository-0.3.6/session_repository/models/repository.py
+-rw-rw-rw-   0        0        0      496 2023-07-18 09:04:38.000000 session-repository-0.3.6/session_repository/models/service.py
+-rw-rw-rw-   0        0        0     9582 2023-07-24 19:16:34.000000 session-repository-0.3.6/session_repository/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:08:52.348051 session-repository-0.3.6/session_repository.egg-info/
+-rw-rw-rw-   0        0        0      599 2023-08-01 22:08:52.000000 session-repository-0.3.6/session_repository.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-08-01 22:08:52.000000 session-repository-0.3.6/session_repository.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 22:08:52.000000 session-repository-0.3.6/session_repository.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-08-01 22:08:52.000000 session-repository-0.3.6/session_repository.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-08-01 22:08:52.000000 session-repository-0.3.6/session_repository.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 22:08:52.370878 session-repository-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      877 2023-08-01 22:00:13.000000 session-repository-0.3.6/setup.py
```

### Comparing `session-repository-0.3.5/PKG-INFO` & `session-repository-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.3.5
+Version: 0.3.6
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.3.5.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.3.6.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.3.5/session_repository/enum.py` & `session-repository-0.3.6/session_repository/enum.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.3.5/session_repository/models/repository.py` & `session-repository-0.3.6/session_repository/models/repository.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # MODULES
 from typing import Any, Callable, Dict, List, Optional, Tuple, Type, TypeVar, Union
-from logging import Logger
 
 # CONNTEXTLIB
 from contextlib import AbstractContextManager
 
 # SQLALCHEMY
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import Session, InstrumentedAttribute, Query
@@ -36,37 +35,16 @@
 T = TypeVar("T", bound=declarative_base())
 
 
 class SessionRepository:
     def __init__(
         self,
         session_factory: Callable[..., AbstractContextManager[Session]],
-        logger: Logger,
-        literal_binds: bool = True,
     ) -> None:
         self._session_factory = session_factory
-        self._logger = logger
-        self._literal_binds = literal_binds
-
-    @classmethod
-    def _log_sql_query(
-        cls,
-        query: Query,
-        logger: Logger,
-        literal_binds: bool = False,
-    ):
-        if logger is None:
-            return
-
-        query_compiled = query.statement.compile(
-            compile_kwargs={
-                "literal_binds": literal_binds,
-            }
-        )
-        logger.info(query_compiled.string)
 
     def session_manager(self):
         return self._session_factory()
 
     @with_session
     def _select(
         self,
@@ -103,20 +81,14 @@
         query = apply_filters(
             query=query,
             filter_dict=optional_filters,
             with_optional=True,
         )
         result = query.first()
 
-        self._log_sql_query(
-            query=query,
-            logger=self._logger,
-            literal_binds=self._literal_binds,
-        )
-
         return result
 
     @with_session
     def _select_all(
         self,
         model: Type[T],
         filters: Optional[_FilterType] = None,
@@ -173,20 +145,14 @@
         query = apply_limit(
             query=query,
             limit=limit,
         )
 
         results = query.all()
 
-        self._log_sql_query(
-            query=query,
-            logger=self._logger,
-            literal_binds=self._literal_binds,
-        )
-
         return results
 
     @with_session
     def _select_paginate(
         self,
         model: Type[T],
         page: int,
@@ -254,24 +220,18 @@
             query=query,
             page=page,
             per_page=per_page,
         )
 
         results = query.all()
 
-        self._log_sql_query(
-            query=query,
-            logger=self._logger,
-            literal_binds=self._literal_binds,
-        )
-
         return results, pagination
 
     @with_session
-    def _update(
+    def _update_all(
         self,
         model: Type[T],
         values: Dict,
         filters: Optional[_FilterType] = None,
         flush: bool = False,
         commit: bool = False,
         current_session: Optional[Session] = None,
@@ -295,24 +255,72 @@
             current_session.commit()
 
         [current_session.refresh(row) for row in rows]
 
         return rows
 
     @with_session
+    def _update(
+        self,
+        model: Type[T],
+        values: Dict,
+        filters: Optional[_FilterType] = None,
+        flush: bool = False,
+        commit: bool = False,
+        current_session: Optional[Session] = None,
+    ) -> T:
+        row = self._select(
+            model=model,
+            filters=filters,
+            current_session=current_session,
+        )
+
+        if row is None:
+            return
+
+        for key, value in values.items():
+            setattr(row, key, value)
+
+        if flush:
+            current_session.flush()
+        if commit:
+            current_session.commit()
+
+        current_session.refresh(row)
+
+        return row
+
+    @with_session
+    def _add_all(
+        self,
+        data: List[T],
+        flush: bool = False,
+        commit: bool = False,
+        current_session: Optional[Session] = None,
+    ) -> List[T]:
+        current_session.add_all(data)
+        if flush:
+            current_session.flush()
+        if commit:
+            current_session.commit()
+
+        if flush or commit:
+            [current_session.refresh(item) for item in data]
+
+        return data
+
+    @with_session
     def _add(
         self,
-        data: Union[List[T], T],
+        data: T,
         flush: bool = False,
         commit: bool = False,
         current_session: Optional[Session] = None,
-    ) -> Union[List[T], T]:
-        current_session.add_all(data) if isinstance(
-            data, list
-        ) else current_session.add(data)
+    ) -> T:
+        current_session.add(data)
         if flush:
             current_session.flush()
         if commit:
             current_session.commit()
 
         if flush or commit:
             current_session.refresh(data)
```

### Comparing `session-repository-0.3.5/session_repository/utils.py` & `session-repository-0.3.6/session_repository/utils.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.3.5/session_repository.egg-info/PKG-INFO` & `session-repository-0.3.6/session_repository.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.3.5
+Version: 0.3.6
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.3.5.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.3.6.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.3.5/setup.py` & `session-repository-0.3.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.3.5"
+version = "0.3.6"
 
 setup(
     name="session-repository",
     version=version,
     packages=[
         "session_repository",
         "session_repository.models",
```


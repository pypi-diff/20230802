# Comparing `tmp/lost_cat-0.1.6.tar.gz` & `tmp/lost_cat-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lost_cat-0.1.6.tar", last modified: Tue Jan 24 16:22:45 2023, max compression
+gzip compressed data, was "lost_cat-0.1.8.tar", last modified: Wed Aug  2 21:50:30 2023, max compression
```

## Comparing `lost_cat-0.1.6.tar` & `lost_cat-0.1.8.tar`

### file list

```diff
@@ -1,42 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-01-24 16:22:45.011569 lost_cat-0.1.6/
--rw-rw-rw-   0        0        0     1093 2022-10-31 17:45:04.000000 lost_cat-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     2115 2023-01-24 16:22:45.009567 lost_cat-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      136 2022-10-31 17:45:04.000000 lost_cat-0.1.6/README.md
--rw-rw-rw-   0        0        0      978 2023-01-24 16:21:09.000000 lost_cat-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-24 16:22:45.012564 lost_cat-0.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-01-24 16:22:44.900035 lost_cat-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-01-24 16:22:44.915046 lost_cat-0.1.6/src/lost_cat/
--rw-rw-rw-   0        0        0        0 2022-10-31 17:45:04.000000 lost_cat-0.1.6/src/lost_cat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-24 16:22:44.936561 lost_cat-0.1.6/src/lost_cat/actions/
--rw-rw-rw-   0        0        0        0 2022-11-04 17:24:28.000000 lost_cat-0.1.6/src/lost_cat/actions/__init__.py
--rw-rw-rw-   0        0        0      957 2022-11-04 17:24:28.000000 lost_cat-0.1.6/src/lost_cat/actions/base_actions.py
-drwxrwxrwx   0        0        0        0 2023-01-24 16:22:44.946555 lost_cat-0.1.6/src/lost_cat/database/
--rw-rw-rw-   0        0        0        0 2022-11-04 17:24:28.000000 lost_cat-0.1.6/src/lost_cat/database/__init__.py
--rw-rw-rw-   0        0        0     1939 2022-11-04 17:24:28.000000 lost_cat-0.1.6/src/lost_cat/database/db_utils.py
--rw-rw-rw-   0        0        0     5278 2022-12-04 00:43:56.000000 lost_cat-0.1.6/src/lost_cat/database/schema.py
--rw-rw-rw-   0        0        0    45387 2023-01-17 22:47:12.000000 lost_cat-0.1.6/src/lost_cat/lost_cat.py
-drwxrwxrwx   0        0        0        0 2023-01-24 16:22:44.956555 lost_cat-0.1.6/src/lost_cat/parsers/
--rw-rw-rw-   0        0        0        0 2022-11-04 17:24:28.000000 lost_cat-0.1.6/src/lost_cat/parsers/__init__.py
--rw-rw-rw-   0        0        0     2863 2022-11-04 17:24:28.000000 lost_cat-0.1.6/src/lost_cat/parsers/base_parser.py
--rw-rw-rw-   0        0        0     3369 2022-11-08 17:10:12.000000 lost_cat-0.1.6/src/lost_cat/parsers/zip_parser.py
-drwxrwxrwx   0        0        0        0 2023-01-24 16:22:44.967558 lost_cat-0.1.6/src/lost_cat/processors/
--rw-rw-rw-   0        0        0        0 2022-11-04 17:24:28.000000 lost_cat-0.1.6/src/lost_cat/processors/__init__.py
--rw-rw-rw-   0        0        0     5873 2022-11-04 17:24:28.000000 lost_cat-0.1.6/src/lost_cat/processors/base_processor.py
--rw-rw-rw-   0        0        0     8708 2022-11-04 17:24:28.000000 lost_cat-0.1.6/src/lost_cat/processors/filesystem_scanner.py
-drwxrwxrwx   0        0        0        0 2023-01-24 16:22:44.971557 lost_cat-0.1.6/src/lost_cat/ui/
--rw-rw-rw-   0        0        0        0 2022-11-04 17:24:28.000000 lost_cat-0.1.6/src/lost_cat/ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-24 16:22:45.005566 lost_cat-0.1.6/src/lost_cat/utils/
--rw-rw-rw-   0        0        0        0 2022-10-31 17:45:04.000000 lost_cat-0.1.6/src/lost_cat/utils/__init__.py
--rw-rw-rw-   0        0        0     3134 2022-11-04 17:24:28.000000 lost_cat-0.1.6/src/lost_cat/utils/module_utils.py
--rw-rw-rw-   0        0        0    15759 2022-11-04 17:24:28.000000 lost_cat-0.1.6/src/lost_cat/utils/path_utils.py
--rw-rw-rw-   0        0        0     5039 2022-12-04 16:47:15.000000 lost_cat-0.1.6/src/lost_cat/utils/phrase_utils.py
--rw-rw-rw-   0        0        0     9357 2023-01-24 16:21:09.000000 lost_cat-0.1.6/src/lost_cat/utils/rules_utils.py
--rw-rw-rw-   0        0        0     5861 2022-11-04 17:24:28.000000 lost_cat-0.1.6/src/lost_cat/utils/tag_anon.py
--rw-rw-rw-   0        0        0     4367 2022-11-04 17:24:28.000000 lost_cat-0.1.6/src/lost_cat/utils/text_utils.py
--rw-rw-rw-   0        0        0     5034 2022-11-04 17:24:28.000000 lost_cat-0.1.6/src/lost_cat/utils/trie_utils.py
-drwxrwxrwx   0        0        0        0 2023-01-24 16:22:44.931555 lost_cat-0.1.6/src/lost_cat.egg-info/
--rw-rw-rw-   0        0        0     2115 2023-01-24 16:22:44.000000 lost_cat-0.1.6/src/lost_cat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      952 2023-01-24 16:22:44.000000 lost_cat-0.1.6/src/lost_cat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-24 16:22:44.000000 lost_cat-0.1.6/src/lost_cat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-01-24 16:22:44.000000 lost_cat-0.1.6/src/lost_cat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-01-24 16:22:44.000000 lost_cat-0.1.6/src/lost_cat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 21:50:30.492903 lost_cat-0.1.8/
+-rw-rw-rw-   0        0        0     1093 2022-10-31 17:45:04.000000 lost_cat-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     2115 2023-08-02 21:50:30.490389 lost_cat-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      136 2022-10-31 17:45:04.000000 lost_cat-0.1.8/README.md
+-rw-rw-rw-   0        0        0      978 2023-08-02 21:48:33.000000 lost_cat-0.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-02 21:50:30.492903 lost_cat-0.1.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-02 21:50:30.260908 lost_cat-0.1.8/src/
+drwxrwxrwx   0        0        0        0 2023-08-02 21:50:30.279438 lost_cat-0.1.8/src/lost_cat/
+-rw-rw-rw-   0        0        0        0 2022-10-31 17:45:04.000000 lost_cat-0.1.8/src/lost_cat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 21:50:30.304008 lost_cat-0.1.8/src/lost_cat/actions/
+-rw-rw-rw-   0        0        0        0 2022-11-04 17:24:28.000000 lost_cat-0.1.8/src/lost_cat/actions/__init__.py
+-rw-rw-rw-   0        0        0      957 2022-11-04 17:24:28.000000 lost_cat-0.1.8/src/lost_cat/actions/base_actions.py
+drwxrwxrwx   0        0        0        0 2023-08-02 21:50:30.316528 lost_cat-0.1.8/src/lost_cat/database/
+-rw-rw-rw-   0        0        0        0 2022-11-04 17:24:28.000000 lost_cat-0.1.8/src/lost_cat/database/__init__.py
+-rw-rw-rw-   0        0        0     2043 2023-08-02 21:48:33.000000 lost_cat-0.1.8/src/lost_cat/database/db_utils.py
+-rw-rw-rw-   0        0        0     5278 2022-12-04 00:43:56.000000 lost_cat-0.1.8/src/lost_cat/database/schema.py
+-rw-rw-rw-   0        0        0    45426 2023-08-02 21:48:33.000000 lost_cat-0.1.8/src/lost_cat/lost_cat.py
+drwxrwxrwx   0        0        0        0 2023-08-02 21:50:30.331064 lost_cat-0.1.8/src/lost_cat/parsers/
+-rw-rw-rw-   0        0        0        0 2022-11-04 17:24:28.000000 lost_cat-0.1.8/src/lost_cat/parsers/__init__.py
+-rw-rw-rw-   0        0        0     2863 2022-11-04 17:24:28.000000 lost_cat-0.1.8/src/lost_cat/parsers/base_parser.py
+-rw-rw-rw-   0        0        0     3369 2022-11-08 17:10:12.000000 lost_cat-0.1.8/src/lost_cat/parsers/zip_parser.py
+drwxrwxrwx   0        0        0        0 2023-08-02 21:50:30.346591 lost_cat-0.1.8/src/lost_cat/processors/
+-rw-rw-rw-   0        0        0        0 2022-11-04 17:24:28.000000 lost_cat-0.1.8/src/lost_cat/processors/__init__.py
+-rw-rw-rw-   0        0        0     5873 2022-11-04 17:24:28.000000 lost_cat-0.1.8/src/lost_cat/processors/base_processor.py
+-rw-rw-rw-   0        0        0     8708 2022-11-04 17:24:28.000000 lost_cat-0.1.8/src/lost_cat/processors/filesystem_scanner.py
+drwxrwxrwx   0        0        0        0 2023-08-02 21:50:30.350589 lost_cat-0.1.8/src/lost_cat/ui/
+-rw-rw-rw-   0        0        0        0 2022-11-04 17:24:28.000000 lost_cat-0.1.8/src/lost_cat/ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 21:50:30.430768 lost_cat-0.1.8/src/lost_cat/utils/
+-rw-rw-rw-   0        0        0        0 2022-10-31 17:45:04.000000 lost_cat-0.1.8/src/lost_cat/utils/__init__.py
+-rw-rw-rw-   0        0        0     3134 2022-11-04 17:24:28.000000 lost_cat-0.1.8/src/lost_cat/utils/module_utils.py
+-rw-rw-rw-   0        0        0    15759 2022-11-04 17:24:28.000000 lost_cat-0.1.8/src/lost_cat/utils/path_utils.py
+-rw-rw-rw-   0        0        0     5039 2022-12-04 16:47:15.000000 lost_cat-0.1.8/src/lost_cat/utils/phrase_utils.py
+-rw-rw-rw-   0        0        0     9785 2023-08-02 21:48:33.000000 lost_cat-0.1.8/src/lost_cat/utils/rules_utils.py
+-rw-rw-rw-   0        0        0     5861 2022-11-04 17:24:28.000000 lost_cat-0.1.8/src/lost_cat/utils/tag_anon.py
+-rw-rw-rw-   0        0        0     4367 2022-11-04 17:24:28.000000 lost_cat-0.1.8/src/lost_cat/utils/text_utils.py
+-rw-rw-rw-   0        0        0     5034 2022-11-04 17:24:28.000000 lost_cat-0.1.8/src/lost_cat/utils/trie_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-02 21:50:30.297991 lost_cat-0.1.8/src/lost_cat.egg-info/
+-rw-rw-rw-   0        0        0     2115 2023-08-02 21:50:30.000000 lost_cat-0.1.8/src/lost_cat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1123 2023-08-02 21:50:30.000000 lost_cat-0.1.8/src/lost_cat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 21:50:30.000000 lost_cat-0.1.8/src/lost_cat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-08-02 21:50:30.000000 lost_cat-0.1.8/src/lost_cat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-02 21:50:30.000000 lost_cat-0.1.8/src/lost_cat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 21:50:30.485389 lost_cat-0.1.8/tests/
+-rw-rw-rw-   0        0        0     4517 2022-11-04 17:24:28.000000 lost_cat-0.1.8/tests/test_lostcat_core.py
+-rw-rw-rw-   0        0        0     1887 2022-11-04 17:24:28.000000 lost_cat-0.1.8/tests/test_module_utils.py
+-rw-rw-rw-   0        0        0     2242 2022-11-04 17:24:28.000000 lost_cat-0.1.8/tests/test_path_utils.py
+-rw-rw-rw-   0        0        0     1733 2022-12-04 16:46:55.000000 lost_cat-0.1.8/tests/test_phrasetool.py
+-rw-rw-rw-   0        0        0     2696 2023-01-23 15:12:00.000000 lost_cat-0.1.8/tests/test_rules.py
+-rw-rw-rw-   0        0        0     1928 2022-11-04 17:24:28.000000 lost_cat-0.1.8/tests/test_taganon.py
+-rw-rw-rw-   0        0        0     3716 2022-11-04 17:24:28.000000 lost_cat-0.1.8/tests/test_utils_trie.py
```

### Comparing `lost_cat-0.1.6/LICENSE` & `lost_cat-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lost_cat-0.1.6/PKG-INFO` & `lost_cat-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lost_cat
-Version: 0.1.6
+Version: 0.1.8
 Summary: Lost cat is a package to scan a variety of locations and report back the files, metadata, and summary contents as needed.
 Author-email: Dreffed aka David Gloyn-Cox <dreffed@gmail.com>, Thoughtswin Systems Inc <david.gloyn-cox@thoughtswinsystems.com>
 License: MIT License
         
         Copyright (c) 2022 David Gloyn-Cox
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `lost_cat-0.1.6/pyproject.toml` & `lost_cat-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lost_cat"
-version = "0.1.6"
+version = "0.1.8"
 authors = [
   { name="Dreffed aka David Gloyn-Cox", email="dreffed@gmail.com" },
   { name="Thoughtswin Systems Inc", email="david.gloyn-cox@thoughtswinsystems.com" },
 ]
 description = "Lost cat is a package to scan a variety of locations and report back the files, metadata, and summary contents as needed."
 readme = "README.md"
 license = { file="LICENSE" }
```

### Comparing `lost_cat-0.1.6/src/lost_cat/actions/base_actions.py` & `lost_cat-0.1.8/src/lost_cat/actions/base_actions.py`

 * *Files identical despite different names*

### Comparing `lost_cat-0.1.6/src/lost_cat/database/db_utils.py` & `lost_cat-0.1.8/src/lost_cat/database/db_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """A module to wrap the database functions and allow the syst4em to wru"""
 import logging
 
 from lost_cat.database.schema import Base
 from sqlalchemy import create_engine, MetaData, Table
 from sqlalchemy.orm import sessionmaker, session as sqlsession
+from sqlalchemy.sql import text
 
 logger = logging.getLogger(__name__)
 
 class DBEngine():
     """"""
     def __init__(self, connString: str = "sqlite:///lost-cat.db") -> None:
         """"""
@@ -31,28 +32,31 @@
         """"""
         return Table(tablename, self.metadata, autoload=True, autoload_with=self.engine)
 
     def tables_list(self) -> dict:
         """"""
         conn = self.engine.connect()
         _data = []
-        _res = conn.execute("SELECT name FROM sqlite_master WHERE type='table';")
+        _res = conn.execute(text("SELECT name FROM sqlite_master WHERE type='table';"))
         _keys = _res.keys()
         for _row in list(_res):
             _rout = {}
             for _rid, _rc in enumerate(_keys):
                 _rout[_rc] = _row[_rid]
             _data.append(_rout)
 
         return _data
 
     def sql(self, sql: str) -> list:
         """Returns a dictionary of objects"""
         _data = []
         _db_sess = self.session()
+        if isinstance(sql, str):
+            sql = text(sql)
+
         _res = _db_sess.execute(sql)
         _keys = _res.keys()
         logger.debug("COLUMNS: %s", _keys)
         for _row in list(_res.fetchall()):
             _rout = {}
             for _rid, _rc in enumerate(_keys):
                 _rout[_rc] = _row[_rid]
```

### Comparing `lost_cat-0.1.6/src/lost_cat/database/schema.py` & `lost_cat-0.1.8/src/lost_cat/database/schema.py`

 * *Files identical despite different names*

### Comparing `lost_cat-0.1.6/src/lost_cat/lost_cat.py` & `lost_cat-0.1.8/src/lost_cat/lost_cat.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import shelve
 import time
 
 from datetime import datetime
 from queue import Empty
 from sqlite3 import IntegrityError
 from sqlalchemy import func
+from sqlalchemy.sql import text
 
 from lost_cat.database.db_utils import DBEngine
 from lost_cat.database.schema import URIMD, Domains, DomainMD, ProcessorMD, \
                 ProcessorURIs, Processors, URIs, VersionMD, Versions
 from lost_cat.utils.module_utils import load_module, load_modulefile
 from lost_cat.utils.path_utils import SourceNotValid
 from lost_cat.utils.tag_anon import TagAnon
@@ -526,15 +527,15 @@
         # load in the tables from the source system...
         """type
                 processors []
                 uris
                     uri
         """
         self._sources = {}
-        sql = """SELECT
+        sql = text("""SELECT
                     uris.id AS uriid,
                     uris.uri AS uri,
                     uris.uri_type AS uritype,
                     uris.root AS uriroot,
                     uris.added AS uriadded,
                     uris.deleted AS urideleted,
                     processors.id AS processorid,
@@ -543,15 +544,15 @@
                 FROM processoruris
                 JOIN uris
                     ON uris.id = processoruris.uriid
                 JOIN processors
                     ON processors.id = processoruris.processorid
                 WHERE uris.root = 1
                     AND uris.deleted IS NULL
-                ORDER BY uris.uri_type"""
+                ORDER BY uris.uri_type""")
 
         for row in self._db.sql(sql=sql):
             # add to the sources dict'
             logger.debug(row)
             _uri_type = row.get("uritype")
             _processor = row.get("processorname")
             _uri = row.get("uri")
```

### Comparing `lost_cat-0.1.6/src/lost_cat/parsers/base_parser.py` & `lost_cat-0.1.8/src/lost_cat/parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `lost_cat-0.1.6/src/lost_cat/parsers/zip_parser.py` & `lost_cat-0.1.8/src/lost_cat/parsers/zip_parser.py`

 * *Files identical despite different names*

### Comparing `lost_cat-0.1.6/src/lost_cat/processors/base_processor.py` & `lost_cat-0.1.8/src/lost_cat/processors/base_processor.py`

 * *Files identical despite different names*

### Comparing `lost_cat-0.1.6/src/lost_cat/processors/filesystem_scanner.py` & `lost_cat-0.1.8/src/lost_cat/processors/filesystem_scanner.py`

 * *Files identical despite different names*

### Comparing `lost_cat-0.1.6/src/lost_cat/utils/module_utils.py` & `lost_cat-0.1.8/src/lost_cat/utils/module_utils.py`

 * *Files identical despite different names*

### Comparing `lost_cat-0.1.6/src/lost_cat/utils/path_utils.py` & `lost_cat-0.1.8/src/lost_cat/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `lost_cat-0.1.6/src/lost_cat/utils/phrase_utils.py` & `lost_cat-0.1.8/src/lost_cat/utils/phrase_utils.py`

 * *Files identical despite different names*

### Comparing `lost_cat-0.1.6/src/lost_cat/utils/rules_utils.py` & `lost_cat-0.1.8/src/lost_cat/utils/rules_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,30 +43,34 @@
             state: RuleState = RuleState.SINGLE,
             options: dict = None
         ):
         """Creates the rule """
         self.name = name
         self.idx = idx
         self.engine = engine
+        self.options = options
         if self.engine == RuleEngine.REGEX:
             if isinstance(expr, str):
-                self.expr = re.compile(expr)
+                igcase = self.options.get("ignorecase", True) if self.options is not None else True
+                if igcase is True:
+                    self.expr = re.compile(expr, re.IGNORECASE)
+                else:
+                    self.expr = re.compile(expr)
             elif isinstance(expr, re.Pattern):
                 self.expr = expr
             else:
                 # bad state...
                 # raise error
                 pass
         else:
             self.expr = expr
 
         self.stop = stop
         self.tags = tags if tags is not None else {}
         self.state = state
-        self.options = options
 
         # save out defaults
         self.ignorecase = self.options.get("ignorecase", True) if self.options is not None else True
         self.flags = self.options.get("flags") if self.options is not None else None
 
         if logger.level == logging.DEBUG:
             logger.info("Rule:")
@@ -97,45 +101,50 @@
             return data
 
         # check what type of rule to use
         if self.engine == RuleEngine.REGEX:
             flags = {
                 "flags": self.flags
             } if self.flags is not None else {}
+            findall = self.options.get("findall", False) if self.options is not None else False
 
-            if self.options.get("findall", False) is True:
+            if findall is True:
                 # use the find all to recover alll matchin
                 # <TODO: add finall code here>
-                if m_findall := self.expr.finditer(phrase, re.IGNORECASE) :#findall(phrase, re.IGNORECASE):#, **flags):
+                if m_findall := self.expr.finditer(phrase):
                     for m in m_findall:
                         for tagvalue in self.tags:
                             tagkey = tagvalue.get("key")
                             if grpkey := tagvalue.get("group"):
                                 # use the regex group
                                 resvalue = m.group(grpkey)
+                            elif grpkey := tagvalue.get("match"):
+                                resvalue = phrase
                             else:
                                 resvalue = tagvalue.get("value") if "value" in tagvalue else "<missing>"
 
                             if tagkey in data.get("tags",{}):
                                 # make a list
                                 if isinstance(data.get("tags",{}).get(tagkey), set):
                                     data["tags"][tagkey].add(resvalue)
                                 else:
                                     data["tags"][tagkey] = {data.get("tags",{}).get(tagkey), resvalue}
                             else:
                                 data["tags"][tagkey] = resvalue
 
-            elif m := self.expr.match(phrase, re.IGNORECASE): #**flags):
+            elif m := self.expr.match(phrase): #**flags):
                 data["passed"] = True
                 # populate the values if any
                 for tagvalue in self.tags:
                     tagkey = tagvalue.get("key")
                     if grpkey := tagvalue.get("group"):
                         # use the regex group
                         resvalue = m.group(grpkey)
+                    elif grpkey := tagvalue.get("match"):
+                        resvalue = phrase
                     else:
                         resvalue = tagvalue.get("value") if "value" in tagvalue else "<missing>"
 
                     if tagkey in data.get("tags",{}):
                         # make a list
                         if isinstance(data.get("tags",{}).get(tagkey), set):
                             data["tags"][tagkey].add(resvalue)
@@ -220,15 +229,15 @@
         """process the rules against each line and
         return the result"""
         results = []
         for phrase in phrases:
             for rule in self.rules:
                 result = rule.run(phrase=phrase)
                 passed = result.get("passed", False)
-                stop = result.get("stop", False)
+                stop = rule.stop
 
                 if passed is True:
                     results.append({
                         "rule": rule,
                         "phrase": phrase,
                         "result": {
                             "passed": passed,
```

### Comparing `lost_cat-0.1.6/src/lost_cat/utils/tag_anon.py` & `lost_cat-0.1.8/src/lost_cat/utils/tag_anon.py`

 * *Files identical despite different names*

### Comparing `lost_cat-0.1.6/src/lost_cat/utils/text_utils.py` & `lost_cat-0.1.8/src/lost_cat/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `lost_cat-0.1.6/src/lost_cat/utils/trie_utils.py` & `lost_cat-0.1.8/src/lost_cat/utils/trie_utils.py`

 * *Files identical despite different names*

### Comparing `lost_cat-0.1.6/src/lost_cat.egg-info/PKG-INFO` & `lost_cat-0.1.8/src/lost_cat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lost-cat
-Version: 0.1.6
+Version: 0.1.8
 Summary: Lost cat is a package to scan a variety of locations and report back the files, metadata, and summary contents as needed.
 Author-email: Dreffed aka David Gloyn-Cox <dreffed@gmail.com>, Thoughtswin Systems Inc <david.gloyn-cox@thoughtswinsystems.com>
 License: MIT License
         
         Copyright (c) 2022 David Gloyn-Cox
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `lost_cat-0.1.6/src/lost_cat.egg-info/SOURCES.txt` & `lost_cat-0.1.8/src/lost_cat.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -23,8 +23,15 @@
 src/lost_cat/utils/__init__.py
 src/lost_cat/utils/module_utils.py
 src/lost_cat/utils/path_utils.py
 src/lost_cat/utils/phrase_utils.py
 src/lost_cat/utils/rules_utils.py
 src/lost_cat/utils/tag_anon.py
 src/lost_cat/utils/text_utils.py
-src/lost_cat/utils/trie_utils.py
+src/lost_cat/utils/trie_utils.py
+tests/test_lostcat_core.py
+tests/test_module_utils.py
+tests/test_path_utils.py
+tests/test_phrasetool.py
+tests/test_rules.py
+tests/test_taganon.py
+tests/test_utils_trie.py
```


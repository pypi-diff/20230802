# Comparing `tmp/misery-0.6.0.tar.gz` & `tmp/misery-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misery-0.6.0.tar", max compression
+gzip compressed data, was "misery-0.6.1.tar", max compression
```

## Comparing `misery-0.6.0.tar` & `misery-0.6.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2022-04-18 18:05:07.195113 misery-0.6.0/LICENSE
--rw-r--r--   0        0        0     1100 2022-06-22 10:01:22.272337 misery-0.6.0/README.md
--rw-r--r--   0        0        0      190 2022-06-22 10:01:22.279012 misery-0.6.0/misery/__init__.py
--rw-r--r--   0        0        0    11655 2022-11-03 12:40:27.289158 misery-0.6.0/misery/clickhouse.py
--rw-r--r--   0        0        0    13424 2022-11-03 13:01:49.425500 misery-0.6.0/misery/core.py
--rw-r--r--   0        0        0     7419 2022-11-03 12:49:59.620667 misery-0.6.0/misery/dictionary.py
--rw-r--r--   0        0        0    13202 2022-11-03 12:44:19.965812 misery-0.6.0/misery/postgres.py
--rw-r--r--   0        0        0      767 2022-11-03 13:04:43.069643 misery-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1969 2022-11-03 13:28:02.544399 misery-0.6.0/setup.py
--rw-r--r--   0        0        0     1826 2022-11-03 13:28:02.544824 misery-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-08-02 07:20:28.078988 misery-0.6.1/LICENSE
+-rw-r--r--   0        0        0     1100 2023-08-02 07:20:28.079155 misery-0.6.1/README.md
+-rw-r--r--   0        0        0      190 2023-08-02 07:20:28.082026 misery-0.6.1/misery/__init__.py
+-rw-r--r--   0        0        0    11666 2023-08-02 07:20:49.380236 misery-0.6.1/misery/clickhouse.py
+-rw-r--r--   0        0        0    13415 2023-08-02 07:20:49.380601 misery-0.6.1/misery/core.py
+-rw-r--r--   0        0        0     7419 2023-08-02 07:20:28.082783 misery-0.6.1/misery/dictionary.py
+-rw-r--r--   0        0        0    13213 2023-08-02 07:20:49.380922 misery-0.6.1/misery/postgres.py
+-rw-r--r--   0        0        0      767 2023-08-02 07:20:49.381195 misery-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1969 2023-08-02 07:28:09.525332 misery-0.6.1/setup.py
+-rw-r--r--   0        0        0     1826 2023-08-02 07:28:09.525790 misery-0.6.1/PKG-INFO
```

### Comparing `misery-0.6.0/LICENSE` & `misery-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `misery-0.6.0/README.md` & `misery-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `misery-0.6.0/misery/clickhouse.py` & `misery-0.6.1/misery/clickhouse.py`

 * *Files 4% similar despite different names*

```diff
@@ -218,23 +218,22 @@
         for f in filters:
             criterion = self._filter_to_criterion(f)
             query = query.where(criterion)
 
         return query
 
     def _filter_to_criterion(self, f: F) -> Criterion:
-        if f.type == FilterType.OR:
-            return Criterion.any([self._filter_to_criterion(ff) for ff in f.value])
-        elif f.type == FilterType.AND:
-            return Criterion.all([self._filter_to_criterion(ff) for ff in f.value])
-
         column = self.table[f.field]
         criterion: Any = None
 
-        if f.type == FilterType.EQ:
+        if f.type == FilterType.OR:
+            criterion = Criterion.any([self._filter_to_criterion(ff) for ff in f.value])
+        elif f.type == FilterType.AND:
+            criterion = Criterion.all([self._filter_to_criterion(ff) for ff in f.value])
+        elif f.type == FilterType.EQ:
             if f.value is None:
                 criterion = _is_null(column)
             else:
                 criterion = column == f.value
         elif f.type == FilterType.NEQ:
             if f.value is None:
                 criterion = _is_not_null(column)
```

### Comparing `misery-0.6.0/misery/core.py` & `misery-0.6.1/misery/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -428,16 +428,15 @@
         the repository.
 
         :param kwargs: Lookup parameters as field-value pairs.
         """
         ...
 
     async def count_filtered(self, filter_: F) -> int:
-        """Count entities that match a given filter.
-        """
+        """Count entities that match a given filter."""
         ...
 
 
 class NotFound(Exception):
     """Error to raise when an entity cannot be found
     in the repository."""
```

### Comparing `misery-0.6.0/misery/dictionary.py` & `misery-0.6.1/misery/dictionary.py`

 * *Files identical despite different names*

### Comparing `misery-0.6.0/misery/postgres.py` & `misery-0.6.1/misery/postgres.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,23 +250,22 @@
         for f in filters:
             criterion = self._filter_to_criterion(f)
             query = query.where(criterion)
 
         return await self.fetch_many(query)
 
     def _filter_to_criterion(self, f: F) -> Criterion:
-        if f.type == FilterType.OR:
-            return Criterion.any([self._filter_to_criterion(ff) for ff in f.value])
-        elif f.type == FilterType.AND:
-            return Criterion.all([self._filter_to_criterion(ff) for ff in f.value])
-
         column = self.table[f.field]
         criterion: Any = None
 
-        if f.type == FilterType.EQ:
+        if f.type == FilterType.OR:
+            criterion = Criterion.any([self._filter_to_criterion(ff) for ff in f.value])
+        elif f.type == FilterType.AND:
+            criterion = Criterion.all([self._filter_to_criterion(ff) for ff in f.value])
+        elif f.type == FilterType.EQ:
             if f.value is None:
                 criterion = column.isnull()
             else:
                 criterion = column == f.value
         elif f.type == FilterType.NEQ:
             if f.value is None:
                 criterion = column.notnull()
```

### Comparing `misery-0.6.0/pyproject.toml` & `misery-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "misery"
-version = "0.6.0"
+version = "0.6.1"
 authors = ["Anton Evdokimov <meowmeowcode@gmail.com>"]
 description = "asyncio-friendly database toolkit"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 PyPika = { version = "^0.48.9", optional = true }
```

### Comparing `misery-0.6.0/setup.py` & `misery-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 extras_require = \
 {'clickhouse': ['PyPika>=0.48.9,<0.49.0', 'aiohttp>=3.8.1,<4.0.0'],
  'postgres': ['PyPika>=0.48.9,<0.49.0', 'asyncpg>=0.25.0,<0.26.0']}
 
 setup_kwargs = {
     'name': 'misery',
-    'version': '0.6.0',
+    'version': '0.6.1',
     'description': 'asyncio-friendly database toolkit',
     'long_description': '<p align="center">\n    <img src="https://github.com/meowmeowcode/misery/blob/clickhouse/docs/source/_static/misery.png" width="200" alt="misery" />\n</p>\n\n\n# Misery\n\nAn **asyncio**-friendly database toolkit that works well with **MyPy**.\n\n## Supported database systems\n\nAt the moment, PostgreSQL and ClickHouse are supported.\n\n## Documentation\n\nThe latest documentation: https://misery.readthedocs.io\n\n## Usage example\n\n```python\nfrom dataclasses import dataclass\nfrom uuid import UUID, uuid4\n\nimport asyncpg\nfrom pypika import Table\nfrom misery.postgres import PostgresRepo\n\n\nconn = await asyncpg.connect("postgresql://postgres:password@localhost/postgres")\n\nawait conn.execute(\n    """\n        CREATE TABLE users (\n            id uuid PRIMARY KEY,\n            name text NOT NULL UNIQUE\n        );\n    """\n)\n\n\n@dataclass\nclass User:\n    id: UUID\n    name: str\n\n\nclass UsersRepo(PostgresRepo[User]):\n    table = Table("users")\n\n\nusers_repo = UsersRepo(conn)\n\nuser_id = uuid4()\nbob = User(id=user_id, name="Bob")\nawait users_repo.add(bob)\n\nuser = await users_repo.get(id=user_id)\nassert user == bob\n```',
     'author': 'Anton Evdokimov',
     'author_email': 'meowmeowcode@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `misery-0.6.0/PKG-INFO` & `misery-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misery
-Version: 0.6.0
+Version: 0.6.1
 Summary: asyncio-friendly database toolkit
 Author: Anton Evdokimov
 Author-email: meowmeowcode@gmail.com
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
```


# Comparing `tmp/edwh_migrate-0.4.3.tar.gz` & `tmp/edwh_migrate-0.4.4.tar.gz`

## Comparing `edwh_migrate-0.4.3.tar` & `edwh_migrate-0.4.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/CHANGELOG.md
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/migrations.py
--rw-r--r--   0        0        0     6261 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/requirements.txt
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/src/edwh_migrate/__about__.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/src/edwh_migrate/__init__.py
--rw-r--r--   0        0        0    19223 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/src/edwh_migrate/migrate.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/tests/__init__.py
--rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/tests/test_basics.py
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/tests/sqlite_empty/empty_sqlite.db
--rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/tests/sqlite_empty/just_implemented_features.db
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/tests/sqlite_empty/just_implemented_features.sql
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/LICENSE.txt
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/README.md
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 edwh_migrate-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/CHANGELOG.md
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/migrations.py
+-rw-r--r--   0        0        0     6261 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/requirements.txt
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/src/edwh_migrate/__about__.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/src/edwh_migrate/__init__.py
+-rw-r--r--   0        0        0    19327 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/src/edwh_migrate/migrate.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/tests/__init__.py
+-rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/tests/test_basics.py
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/tests/sqlite_empty/empty_sqlite.db
+-rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/tests/sqlite_empty/just_implemented_features.db
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/tests/sqlite_empty/just_implemented_features.sql
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/LICENSE.txt
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/README.md
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/PKG-INFO
```

### Comparing `edwh_migrate-0.4.3/CHANGELOG.md` & `edwh_migrate-0.4.4/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.4.4 (2023-08-02)
+### Fix
+* Fixing an issue with long_running, and rollback the transaction after an error on a non-existing table. ([`accfbe4`](https://github.com/educationwarehouse/migrate/commit/accfbe4fd3ee0c9ea6b9933025a33166a16d9105))
+
 ## v0.4.3 (2023-05-15)
 ### Fix
 * BaseExceptionGroup does not exist in 3.10 yet ([`3433a4f`](https://github.com/educationwarehouse/migrate/commit/3433a4fda0d6ebfb2a551d9f5c3feb4f51e6afc0))
 
 ## v0.4.2 (2023-05-04)
 ### Documentation
 * **migrate:** Changed package name from '-' to edwh-migrate and added extra's dev dependencies ([`ae3eef6`](https://github.com/educationwarehouse/migrate/commit/ae3eef6a1e2db47d03fcd60a57d768d79b7f4a32))
```

### Comparing `edwh_migrate-0.4.3/migrations.py` & `edwh_migrate-0.4.4/migrations.py`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.3/requirements.txt` & `edwh_migrate-0.4.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.3/src/edwh_migrate/__init__.py` & `edwh_migrate-0.4.4/src/edwh_migrate/__init__.py`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.3/src/edwh_migrate/migrate.py` & `edwh_migrate-0.4.4/src/edwh_migrate/migrate.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,34 +108,37 @@
     db = dal_class(
         uri,
         migrate=migrate,
         migrate_enabled=migrate_enabled,
         driver_args=driver_args,
         pool_size=1,
     )
-    if is_postgres and not long_running:
+    if is_postgres and long_running:
         # https://www.pgpool.net/docs/latest/en/html/sql-pgpool-set.html
         # make this connection able to live longer, because the functions can take over 30s
         # to perform the job.
         # db.executesql("PGPOOL SET client_idle_limit = 3600;")
         with contextlib.suppress(Exception):
+            print('Setting up for long running connection')
             db.executesql(f"PGPOOL SET client_idle_limit = {long_running if str(long_running).isdigit() else 3600};")
-
+            db.rollback()
     db.define_table(
         "ewh_implemented_features",
         Field("name", unique=True),
         Field("installed", "boolean", default=False),
         Field("last_update_dttm", "datetime", default=datetime.datetime.now()),
     )
     try:
         db(db.ewh_implemented_features).count()
     except (psycopg2.errors.UndefinedTable, sqlite3.OperationalError) as e:
+        db.rollback()
         raise DatabaseNotYetInitialized(
             "ewh_implemented_features is missing.", db
         ) from e
+
     return db
 
 
 def migration(func: callable = None, requires: list[callable] | typing.Callable | None = None):
     """
     Decorator to register a function as a migration function.
```

### Comparing `edwh_migrate-0.4.3/tests/test_basics.py` & `edwh_migrate-0.4.4/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.3/tests/sqlite_empty/empty_sqlite.db` & `edwh_migrate-0.4.4/tests/sqlite_empty/empty_sqlite.db`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.3/tests/sqlite_empty/just_implemented_features.db` & `edwh_migrate-0.4.4/tests/sqlite_empty/just_implemented_features.db`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.3/.gitignore` & `edwh_migrate-0.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.3/LICENSE.txt` & `edwh_migrate-0.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.3/README.md` & `edwh_migrate-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.3/pyproject.toml` & `edwh_migrate-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.3/PKG-INFO` & `edwh_migrate-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-migrate
-Version: 0.4.3
+Version: 0.4.4
 Summary: Helps migrating database schema changes using pydal. 
 Project-URL: Documentation, https://github.com/educationwarehouse/migrate#readme
 Project-URL: Issues, https://github.com/educationwarehouse/migrate/issues
 Project-URL: Source, https://github.com/educationwarehouse/migrate
 Author-email: Remco <remco@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```


# Comparing `tmp/edwh_migrate-0.4.4.tar.gz` & `tmp/edwh_migrate-0.5.0.tar.gz`

## Comparing `edwh_migrate-0.4.4.tar` & `edwh_migrate-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/CHANGELOG.md
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/migrations.py
--rw-r--r--   0        0        0     6261 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/requirements.txt
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/src/edwh_migrate/__about__.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/src/edwh_migrate/__init__.py
--rw-r--r--   0        0        0    19327 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/src/edwh_migrate/migrate.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/tests/__init__.py
--rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/tests/test_basics.py
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/tests/sqlite_empty/empty_sqlite.db
--rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/tests/sqlite_empty/just_implemented_features.db
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/tests/sqlite_empty/just_implemented_features.sql
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/LICENSE.txt
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/README.md
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 edwh_migrate-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 edwh_migrate-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 edwh_migrate-0.5.0/migrations.py
+-rw-r--r--   0        0        0     6261 2020-02-02 00:00:00.000000 edwh_migrate-0.5.0/requirements.txt
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 edwh_migrate-0.5.0/src/edwh_migrate/__about__.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 edwh_migrate-0.5.0/src/edwh_migrate/__init__.py
+-rw-r--r--   0        0        0    18474 2020-02-02 00:00:00.000000 edwh_migrate-0.5.0/src/edwh_migrate/migrate.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 edwh_migrate-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 edwh_migrate-0.5.0/tests/test_basics.py
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 edwh_migrate-0.5.0/tests/sqlite_empty/empty_sqlite.db
+-rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 edwh_migrate-0.5.0/tests/sqlite_empty/just_implemented_features.db
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 edwh_migrate-0.5.0/tests/sqlite_empty/just_implemented_features.sql
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 edwh_migrate-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 edwh_migrate-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 edwh_migrate-0.5.0/README.md
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 edwh_migrate-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 edwh_migrate-0.5.0/PKG-INFO
```

### Comparing `edwh_migrate-0.4.4/CHANGELOG.md` & `edwh_migrate-0.5.0/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.5.0 (2023-08-02)
+### Feature
+* Supports passwords in database uri's using uri scheme instead of -U -p arguments etc. psql is compatible with the `postgres://` uri scheme, so why bother? ([`80f09ce`](https://github.com/educationwarehouse/migrate/commit/80f09ce15369ee6756afedc2a4d44e176a1c95fb))
+
 ## v0.4.4 (2023-08-02)
 ### Fix
 * Fixing an issue with long_running, and rollback the transaction after an error on a non-existing table. ([`accfbe4`](https://github.com/educationwarehouse/migrate/commit/accfbe4fd3ee0c9ea6b9933025a33166a16d9105))
 
 ## v0.4.3 (2023-05-15)
 ### Fix
 * BaseExceptionGroup does not exist in 3.10 yet ([`3433a4f`](https://github.com/educationwarehouse/migrate/commit/3433a4fda0d6ebfb2a551d9f5c3feb4f51e6afc0))
```

### Comparing `edwh_migrate-0.4.4/migrations.py` & `edwh_migrate-0.5.0/migrations.py`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.4/requirements.txt` & `edwh_migrate-0.5.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.4/src/edwh_migrate/__init__.py` & `edwh_migrate-0.5.0/src/edwh_migrate/__init__.py`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.4/src/edwh_migrate/migrate.py` & `edwh_migrate-0.5.0/src/edwh_migrate/migrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,57 +243,31 @@
 
     # unpack is now the command to cat the sql to stdout
     # which is piped to psql to perform the recovery
 
     # parse the db uri to find hostname and port and such to
     # feed to pqsl as commandline arguments
     uri = urllib.parse.urlparse(os.environ["MIGRATE_URI"])
-    is_postgres = uri.scheme.startswith("postgres")
-    database = str(uri.path).lstrip("/")
-    netloc = str(uri.netloc)
-    if "@" in netloc:
-        username_password, hostname_port = netloc.split("@")
-    else:
-        username_password = "postgres"
-        hostname_port = netloc
-    if ":" in username_password:
-        username, password = username_password.split(":")
-    else:
-        username = username_password
-        password = None
-    if ":" in hostname_port:
-        hostname, port = hostname_port.split(":")
-    else:
-        hostname = hostname_port
-        port = "5432"
 
-    if is_postgres:
+    if  uri.scheme.startswith("postgres"):
         # prepare the psql command
-        psql = plumbum.local["psql"]["-h", hostname, "-U", username, "-d", database]
-        if password:
-            raise InvalidConfigException(
-                "Postgresql Password NOT SUPPORTED for automatic migrations... "
-            )
-        if port:
-            psql = psql["-p", port]
+        psql = plumbum.local["psql"][uri]
         sql_consumer = psql
     else:
         sqlite_database_path = pathlib.Path(uri.netloc) / pathlib.Path(uri.path.strip('/'))
         sql_consumer = plumbum.local["sqlite3"][sqlite_database_path]
     # combine both
     cmd = unpack | sql_consumer
 
     print("UNPACKING AND INSTALLING DATABASE:", cmd)
     # noinspection PyStatementEffect
     # is plumbum syntax
     cmd() > "/dev/null"
     print("Done unpacking and feeding to", cmd)
 
-    # os.unlink(local_backup)
-
 
 def activate_migrations():
     """Start the migration process, don't wait for a lock"""
     started = time.time()
     while time.time() - started < 600:
         try:
             db = setup_db()
```

### Comparing `edwh_migrate-0.4.4/tests/test_basics.py` & `edwh_migrate-0.5.0/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.4/tests/sqlite_empty/empty_sqlite.db` & `edwh_migrate-0.5.0/tests/sqlite_empty/empty_sqlite.db`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.4/tests/sqlite_empty/just_implemented_features.db` & `edwh_migrate-0.5.0/tests/sqlite_empty/just_implemented_features.db`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.4/.gitignore` & `edwh_migrate-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.4/LICENSE.txt` & `edwh_migrate-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.4/README.md` & `edwh_migrate-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.4/pyproject.toml` & `edwh_migrate-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_migrate-0.4.4/PKG-INFO` & `edwh_migrate-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-migrate
-Version: 0.4.4
+Version: 0.5.0
 Summary: Helps migrating database schema changes using pydal. 
 Project-URL: Documentation, https://github.com/educationwarehouse/migrate#readme
 Project-URL: Issues, https://github.com/educationwarehouse/migrate/issues
 Project-URL: Source, https://github.com/educationwarehouse/migrate
 Author-email: Remco <remco@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```


# Comparing `tmp/arrow_odbc-1.2.0.tar.gz` & `tmp/arrow_odbc-1.2.1.tar.gz`

## Comparing `arrow_odbc-1.2.0.tar` & `arrow_odbc-1.2.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      788 1970-01-01 00:00:00.000000 arrow_odbc-1.2.0/Cargo.toml
--rw-r--r--   0      501       20      136 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/.gitattributes
--rw-r--r--   0      501       20      131 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/.github/dependabot.yml
--rw-r--r--   0      501       20     1522 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/.github/workflows/test.yml
--rw-r--r--   0      501       20     1807 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/.github/workflows/wheel.yml
--rw-r--r--   0      501       20      286 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/.gitignore
--rw-r--r--   0      501       20      841 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/.readthedocs.yaml
--rw-r--r--   0      501       20     5239 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/Changelog.md
--rw-r--r--   0      501       20     1954 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/Contributing.md
--rw-r--r--   0      501       20     1069 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/LICENSE
--rw-r--r--   0      501       20     7729 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/README.md
--rw-r--r--   0      501       20       14 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/cbindgen.toml
--rw-r--r--   0      501       20      639 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/conftest.py
--rw-r--r--   0      501       20      638 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/doc/Makefile
--rw-r--r--   0      501       20      804 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/doc/make.bat
--rw-r--r--   0      501       20       16 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/doc/requirements.txt
--rw-r--r--   0      501       20      155 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/doc/source/arrow_odbc.rst
--rw-r--r--   0      501       20     1965 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/doc/source/conf.py
--rw-r--r--   0      501       20      458 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/doc/source/index.rst
--rw-r--r--   0      501       20       67 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/doc/source/modules.rst
--rw-r--r--   0      501       20      348 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/docker-compose.yml
--rw-r--r--   0      501       20      564 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/manylinux/Dockerfile
--rw-r--r--   0      501       20      121 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/manylinux/Readme.md
--rw-r--r--   0      501       20      148 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/manylinux/WHEEL
--rw-r--r--   0      501       20     1256 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/manylinux/build_wheel.sh
--rw-r--r--   0      501       20      649 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/pyproject.toml
--rw-r--r--   0      501       20      445 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/python/arrow_odbc/__init__.py
--rw-r--r--   0      501       20     1645 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/python/arrow_odbc/connect.py
--rw-r--r--   0      501       20      672 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/python/arrow_odbc/error.py
--rw-r--r--   0      501       20      801 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/python/arrow_odbc/log.py
--rw-r--r--   0      501       20      579 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/python/arrow_odbc/pool.py
--rw-r--r--   0      501       20    15067 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/python/arrow_odbc/reader.py
--rw-r--r--   0      501       20     9164 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/python/arrow_odbc/writer.py
--rw-r--r--   0      501       20     2322 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/src/error.rs
--rw-r--r--   0      501       20     2907 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/src/lib.rs
--rw-r--r--   0      501       20      655 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/src/logging.rs
--rw-r--r--   0      501       20     1239 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/src/parameter.rs
--rw-r--r--   0      501       20      421 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/src/pool.rs
--rw-r--r--   0      501       20     2921 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/src/reader/arrow_odbc_reader.rs
--rw-r--r--   0      501       20     6502 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/src/reader.rs
--rw-r--r--   0      501       20     3545 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/src/writer.rs
--rw-r--r--   0      501       20        0 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/tests/__init__.py
--rw-r--r--   0      501       20     4115 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/tests/iris.csv
--rw-r--r--   0      501       20     2413 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/tests/iris.parquet
--rw-r--r--   0      501       20    19559 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/tests/test_arrow_odbc.py
--rw-r--r--   0      501       20    35078 2023-07-23 15:13:10.000000 arrow_odbc-1.2.0/Cargo.lock
--rw-r--r--   0        0        0     8261 1970-01-01 00:00:00.000000 arrow_odbc-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      788 1970-01-01 00:00:00.000000 arrow_odbc-1.2.1/Cargo.toml
+-rw-r--r--   0      501       20      136 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/.gitattributes
+-rw-r--r--   0      501       20      131 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/.github/dependabot.yml
+-rw-r--r--   0      501       20     1522 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/.github/workflows/test.yml
+-rw-r--r--   0      501       20     1807 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/.github/workflows/wheel.yml
+-rw-r--r--   0      501       20      286 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/.gitignore
+-rw-r--r--   0      501       20      841 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/.readthedocs.yaml
+-rw-r--r--   0      501       20     5451 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/Changelog.md
+-rw-r--r--   0      501       20     1954 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/Contributing.md
+-rw-r--r--   0      501       20     1069 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/LICENSE
+-rw-r--r--   0      501       20     7729 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/README.md
+-rw-r--r--   0      501       20       14 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/cbindgen.toml
+-rw-r--r--   0      501       20      639 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/conftest.py
+-rw-r--r--   0      501       20      638 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/doc/Makefile
+-rw-r--r--   0      501       20      804 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/doc/make.bat
+-rw-r--r--   0      501       20       16 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/doc/requirements.txt
+-rw-r--r--   0      501       20      155 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/doc/source/arrow_odbc.rst
+-rw-r--r--   0      501       20     1965 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/doc/source/conf.py
+-rw-r--r--   0      501       20      458 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/doc/source/index.rst
+-rw-r--r--   0      501       20       67 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/doc/source/modules.rst
+-rw-r--r--   0      501       20      348 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/docker-compose.yml
+-rw-r--r--   0      501       20      564 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/manylinux/Dockerfile
+-rw-r--r--   0      501       20      121 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/manylinux/Readme.md
+-rw-r--r--   0      501       20      148 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/manylinux/WHEEL
+-rw-r--r--   0      501       20     1256 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/manylinux/build_wheel.sh
+-rw-r--r--   0      501       20      649 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/pyproject.toml
+-rw-r--r--   0      501       20      445 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/python/arrow_odbc/__init__.py
+-rw-r--r--   0      501       20     1645 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/python/arrow_odbc/connect.py
+-rw-r--r--   0      501       20      672 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/python/arrow_odbc/error.py
+-rw-r--r--   0      501       20      801 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/python/arrow_odbc/log.py
+-rw-r--r--   0      501       20      579 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/python/arrow_odbc/pool.py
+-rw-r--r--   0      501       20    15067 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/python/arrow_odbc/reader.py
+-rw-r--r--   0      501       20     9164 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/python/arrow_odbc/writer.py
+-rw-r--r--   0      501       20     2322 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/src/error.rs
+-rw-r--r--   0      501       20     2907 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/src/lib.rs
+-rw-r--r--   0      501       20      655 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/src/logging.rs
+-rw-r--r--   0      501       20     1239 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/src/parameter.rs
+-rw-r--r--   0      501       20      421 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/src/pool.rs
+-rw-r--r--   0      501       20     2921 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/src/reader/arrow_odbc_reader.rs
+-rw-r--r--   0      501       20     6502 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/src/reader.rs
+-rw-r--r--   0      501       20     3545 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/src/writer.rs
+-rw-r--r--   0      501       20        0 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/tests/__init__.py
+-rw-r--r--   0      501       20     4115 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/tests/iris.csv
+-rw-r--r--   0      501       20     2413 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/tests/iris.parquet
+-rw-r--r--   0      501       20    20417 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/tests/test_arrow_odbc.py
+-rw-r--r--   0      501       20    35087 2023-08-02 06:07:32.000000 arrow_odbc-1.2.1/Cargo.lock
+-rw-r--r--   0        0        0     8261 1970-01-01 00:00:00.000000 arrow_odbc-1.2.1/PKG-INFO
```

### Comparing `arrow_odbc-1.2.0/Cargo.toml` & `arrow_odbc-1.2.1/Cargo.toml`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.2.0/.github/workflows/test.yml` & `arrow_odbc-1.2.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.2.0/.github/workflows/wheel.yml` & `arrow_odbc-1.2.1/.github/workflows/wheel.yml`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.2.0/.readthedocs.yaml` & `arrow_odbc-1.2.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.2.0/Changelog.md` & `arrow_odbc-1.2.1/Changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## 1.2.1
+
+- Update Rust dependencies. Includes update to arrow-odbc 0.28.9 which forwards the original error message from the ODBC driver in situtations there it has been previously hidden by error translation.
+
 ## 1.2.0
 
 - Introduce `enable_odbc_connection_pooling` to allow for reducing overhead then creating "new" connections.
 
 ## 1.1.3
 
 - Update Rust dependencies
```

### Comparing `arrow_odbc-1.2.0/Contributing.md` & `arrow_odbc-1.2.1/Contributing.md`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.2.0/LICENSE` & `arrow_odbc-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.2.0/README.md` & `arrow_odbc-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.2.0/conftest.py` & `arrow_odbc-1.2.1/conftest.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.2.0/doc/Makefile` & `arrow_odbc-1.2.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.2.0/doc/make.bat` & `arrow_odbc-1.2.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.2.0/doc/source/conf.py` & `arrow_odbc-1.2.1/doc/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "arrow-odbc"
 copyright = "2021, Markus Klein"
 author = "Markus Klein"
 
 # The full version, including alpha/beta/rc tags
-release = "1.2.0"
+release = "1.2.1"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `arrow_odbc-1.2.0/manylinux/Dockerfile` & `arrow_odbc-1.2.1/manylinux/Dockerfile`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.2.0/manylinux/build_wheel.sh` & `arrow_odbc-1.2.1/manylinux/build_wheel.sh`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.2.0/pyproject.toml` & `arrow_odbc-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "maturin"
 
 [project]
 name = "arrow-odbc"
 authors = [{name = "Markus Klein"}]
 description="Read the data of an ODBC data source as sequence of Apache Arrow record batches."
 readme = "README.md"
-version = "1.2.0"
+version = "1.2.1"
 dependencies = ["cffi", "pyarrow >= 8.0.0"]
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 test = ["pytest < 8.0.0"]
```

### Comparing `arrow_odbc-1.2.0/python/arrow_odbc/connect.py` & `arrow_odbc-1.2.1/python/arrow_odbc/connect.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.2.0/python/arrow_odbc/error.py` & `arrow_odbc-1.2.1/python/arrow_odbc/error.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.2.0/python/arrow_odbc/log.py` & `arrow_odbc-1.2.1/python/arrow_odbc/log.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.2.0/python/arrow_odbc/pool.py` & `arrow_odbc-1.2.1/python/arrow_odbc/pool.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.2.0/python/arrow_odbc/reader.py` & `arrow_odbc-1.2.1/python/arrow_odbc/reader.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.2.0/python/arrow_odbc/writer.py` & `arrow_odbc-1.2.1/python/arrow_odbc/writer.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.2.0/src/error.rs` & `arrow_odbc-1.2.1/src/error.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.2.0/src/lib.rs` & `arrow_odbc-1.2.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.2.0/src/logging.rs` & `arrow_odbc-1.2.1/src/logging.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.2.0/src/parameter.rs` & `arrow_odbc-1.2.1/src/parameter.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.2.0/src/reader/arrow_odbc_reader.rs` & `arrow_odbc-1.2.1/src/reader/arrow_odbc_reader.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.2.0/src/reader.rs` & `arrow_odbc-1.2.1/src/reader.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.2.0/src/writer.rs` & `arrow_odbc-1.2.1/src/writer.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.2.0/tests/iris.csv` & `arrow_odbc-1.2.1/tests/iris.csv`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.2.0/tests/iris.parquet` & `arrow_odbc-1.2.1/tests/iris.parquet`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.2.0/tests/test_arrow_odbc.py` & `arrow_odbc-1.2.1/tests/test_arrow_odbc.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,31 +203,56 @@
     table = "OneRow"
     os.system(f'odbcsv fetch -c "{MSSQL}" -q "DROP TABLE IF EXISTS {table};"')
     os.system(f'odbcsv fetch -c "{MSSQL}" -q "CREATE TABLE {table} (a DATETIME2(6));"')
     rows = "a\n2014-04-14 21:25:42.074841"
     run(["odbcsv", "insert", "-c", MSSQL, table], input=rows, encoding="ascii")
 
     query = f"SELECT * FROM {table}"
-
     reader = read_arrow_batches_from_odbc(
         query=query, batch_size=100, connection_string=MSSQL
     )
     it = iter(reader)
-
     actual = next(it)
 
     schema = pa.schema([("a", pa.timestamp("us"))])
     expected = pa.RecordBatch.from_pydict({"a": [1397510742074841]}, schema)
     print(expected[0])
     print(actual[0])
     assert expected == actual
 
     with raises(StopIteration):
         next(it)
 
+
+def test_timestamp_ns():
+    """
+    Query a table with one row. Should return one batch
+    """
+    table = "OneRow"
+    os.system(f'odbcsv fetch -c "{MSSQL}" -q "DROP TABLE IF EXISTS {table};"')
+    os.system(f'odbcsv fetch -c "{MSSQL}" -q "CREATE TABLE {table} (a DATETIME2(7));"')
+    rows = "a\n2014-04-14 21:25:42.0748412"
+    run(["odbcsv", "insert", "-c", MSSQL, table], input=rows, encoding="ascii")
+
+    query = f"SELECT * FROM {table}"
+    reader = read_arrow_batches_from_odbc(
+        query=query, batch_size=100, connection_string=MSSQL
+    )
+    it = iter(reader)
+    actual = next(it)
+
+    schema = pa.schema([("a", pa.timestamp("ns"))])
+    expected = pa.RecordBatch.from_pydict({"a": [1397510742074841200]}, schema)
+    print(expected[0])
+    print(actual[0])
+    assert expected == actual
+
+    with raises(StopIteration):
+        next(it)
+
 
 def test_specify_user_and_password_separatly():
     """
     Query a table with one row. Should return one batch
     """
 
     query = f"SELECT 42 as a;"
```

### Comparing `arrow_odbc-1.2.0/Cargo.lock` & `arrow_odbc-1.2.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "android-activity"
-version = "0.4.2"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "40bc1575e653f158cbdc6ebcd917b9564e66321c5325c232c3591269c257be69"
+checksum = "64529721f27c2314ced0890ce45e469574a73e5e6fdd6e9da1860eb29285f5e0"
 dependencies = [
  "android-properties",
  "bitflags 1.3.2",
  "cc",
  "jni-sys",
  "libc",
  "log",
@@ -151,17 +151,17 @@
  "arrow-schema",
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-odbc"
-version = "0.28.8"
+version = "0.28.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e3b64304ea22d71207a6ba3a87385c9161109ad34902cac7044a9c76c9b7dac5"
+checksum = "f4bc8f162ee94750954fd496573e263fc779adcbc74a4ff1590f278d7878c8fa"
 dependencies = [
  "arrow",
  "atoi",
  "chrono",
  "odbc-api",
  "thiserror",
 ]
@@ -306,19 +306,20 @@
 name = "bumpalo"
 version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
 
 [[package]]
 name = "cc"
-version = "1.0.79"
+version = "1.0.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
+checksum = "51f1226cd9da55587234753d1245dd5b132343ea240f26b6a9003d68706141ba"
 dependencies = [
  "jobserver",
+ "libc",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
@@ -786,15 +787,15 @@
 version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "96667db765a921f7b295ffee8b60472b686a51d4f21c2ee4ffdb94c7013b65a6"
 dependencies = [
  "proc-macro-crate",
  "proc-macro2",
  "quote",
- "syn 2.0.27",
+ "syn 2.0.28",
 ]
 
 [[package]]
 name = "objc-sys"
 version = "0.2.0-beta.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "df3b9834c1e95694a05a828b59f55fa2afec6288359cda67146126b3f90a55d7"
@@ -877,17 +878,17 @@
 checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.31"
+version = "1.0.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5fe8a65d69dd0808184ebb5f836ab526bb259db23c657efa38711b1072ee47f0"
+checksum = "50f3b39ccfb720540debaa0164757101c08ecb8d326b15358ce76a62c7e85965"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "raw-window-handle"
 version = "0.5.2"
@@ -913,17 +914,17 @@
  "memchr",
  "regex-automata",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
-version = "0.3.3"
+version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39354c10dd07468c2e73926b23bb9c2caca74c5501e38a35da70406f1d923310"
+checksum = "b7b6d6190b7594385f61bd3911cd1be99dfddcfc365a4160cc2ab5bff4aed294"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
@@ -960,17 +961,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.27"
+version = "2.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b60f673f44a8255b9c8c657daf66a596d435f2da81a555b06dc644d080ba45e0"
+checksum = "04361975b3f5e348b2189d8dc55bc942f278b2d482a6a0365de5bdd62d351567"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -995,15 +996,15 @@
 name = "thiserror-impl"
 version = "1.0.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "090198534930841fab3a5d1bb637cde49e339654e606195f8d9c76eeb081dc96"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.27",
+ "syn 2.0.28",
 ]
 
 [[package]]
 name = "thread_local"
 version = "1.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdd6f064ccff2d6567adcb3873ca630700f00b5ad3f060c25b5dcfd9a4ce152"
@@ -1090,15 +1091,15 @@
 checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.27",
+ "syn 2.0.28",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1112,15 +1113,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.27",
+ "syn 2.0.28",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.87"
@@ -1342,17 +1343,17 @@
  "wayland-scanner",
  "web-sys",
  "windows-sys",
 ]
 
 [[package]]
 name = "winnow"
-version = "0.5.0"
+version = "0.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "81fac9742fd1ad1bd9643b991319f72dd031016d44b77039a26977eb667141e7"
+checksum = "f46aab759304e4d7b2075a9aecba26228bb073ee8c50db796b2c72c676b5d807"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "xml-rs"
 version = "0.8.16"
```

### Comparing `arrow_odbc-1.2.0/PKG-INFO` & `arrow_odbc-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrow-odbc
-Version: 1.2.0
+Version: 1.2.1
 Requires-Dist: cffi
 Requires-Dist: pyarrow >=8.0.0
 Requires-Dist: pytest <8.0.0 ; extra == 'test'
 Provides-Extra: test
 License-File: LICENSE
 Summary: Read the data of an ODBC data source as sequence of Apache Arrow record batches.
 Author: Markus Klein
```


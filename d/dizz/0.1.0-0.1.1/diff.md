# Comparing `tmp/dizz-0.1.0.tar.gz` & `tmp/dizz-0.1.1.tar.gz`

## Comparing `dizz-0.1.0.tar` & `dizz-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 dizz-0.1.0/Cargo.toml
--rw-r--r--   0      501       20     2807 2023-08-02 04:55:56.000000 dizz-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0      501       20      685 2023-08-02 04:55:56.000000 dizz-0.1.0/.gitignore
--rw-r--r--   0      501       20      591 2023-08-02 17:21:21.000000 dizz-0.1.0/README.md
--rw-r--r--   0      501       20      364 2023-08-02 17:21:21.000000 dizz-0.1.0/pyproject.toml
--rw-r--r--   0      501       20       14 2023-08-02 16:37:54.000000 dizz-0.1.0/requirements.txt
--rw-r--r--   0      501       20      505 2023-08-02 17:21:22.000000 dizz-0.1.0/src/lib.rs
--rw-r--r--   0      501       20     8932 2023-08-02 17:21:21.000000 dizz-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 dizz-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 dizz-0.1.1/Cargo.toml
+-rw-r--r--   0      501       20     2807 2023-08-02 04:55:56.000000 dizz-0.1.1/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      685 2023-08-02 04:55:56.000000 dizz-0.1.1/.gitignore
+-rw-r--r--   0      501       20      591 2023-08-02 17:21:21.000000 dizz-0.1.1/README.md
+-rw-r--r--   0      501       20      364 2023-08-02 17:37:51.000000 dizz-0.1.1/pyproject.toml
+-rw-r--r--   0      501       20       14 2023-08-02 16:37:54.000000 dizz-0.1.1/requirements.txt
+-rw-r--r--   0      501       20      505 2023-08-02 17:36:12.000000 dizz-0.1.1/src/lib.rs
+-rw-r--r--   0      501       20     8932 2023-08-02 17:49:33.000000 dizz-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 dizz-0.1.1/PKG-INFO
```

### Comparing `dizz-0.1.0/.github/workflows/CI.yml` & `dizz-0.1.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `dizz-0.1.0/.gitignore` & `dizz-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dizz-0.1.0/README.md` & `dizz-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dizz-0.1.0/Cargo.lock` & `dizz-0.1.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "dizz"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "pyo3",
  "sqlformat",
 ]
 
 [[package]]
 name = "either"
```

### Comparing `dizz-0.1.0/PKG-INFO` & `dizz-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dizz
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # dizz
```


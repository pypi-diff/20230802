# Comparing `tmp/umka-0.1.0.tar.gz` & `tmp/umka-0.1.1.tar.gz`

## Comparing `umka-0.1.0.tar` & `umka-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 umka-0.1.0/Cargo.toml
--rw-r--r--   0     1001      123      455 2023-08-01 21:33:52.000000 umka-0.1.0/pyproject.toml
--rw-r--r--   0     1001      123     4110 2023-08-01 21:33:52.000000 umka-0.1.0/src/fuzzywuzzy.rs
--rw-r--r--   0     1001      123     3043 2023-08-01 21:33:52.000000 umka-0.1.0/src/lib.rs
--rw-r--r--   0     1001      123       38 2023-08-01 21:33:52.000000 umka-0.1.0/umka/__init__.py
--rw-r--r--   0     1001      123        0 2023-08-01 21:33:52.000000 umka-0.1.0/umka/fuzz/__init__.py
--rw-r--r--   0     1001      123     1106 2023-08-01 21:33:52.000000 umka-0.1.0/umka/fuzz/fuzz.py
--rw-r--r--   0     1001      123        0 2023-08-01 21:33:52.000000 umka-0.1.0/umka/test/__init__.py
--rw-r--r--   0     1001      123        0 2023-08-01 21:33:52.000000 umka-0.1.0/umka/test/fuzz/__init__.py
--rw-r--r--   0     1001      123     1214 2023-08-01 21:33:52.000000 umka-0.1.0/umka/test/fuzz/test_fuzz.py
--rw-r--r--   0     1001      123    47392 2023-08-01 21:33:52.000000 umka-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      223 1970-01-01 00:00:00.000000 umka-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      670 1970-01-01 00:00:00.000000 umka-0.1.1/Cargo.toml
+-rw-r--r--   0     1001      123      455 2023-08-02 10:12:21.000000 umka-0.1.1/pyproject.toml
+-rw-r--r--   0     1001      123     4110 2023-08-02 10:12:21.000000 umka-0.1.1/src/fuzzywuzzy.rs
+-rw-r--r--   0     1001      123     3043 2023-08-02 10:12:21.000000 umka-0.1.1/src/lib.rs
+-rw-r--r--   0     1001      123       38 2023-08-02 10:12:21.000000 umka-0.1.1/umka/__init__.py
+-rw-r--r--   0     1001      123        0 2023-08-02 10:12:21.000000 umka-0.1.1/umka/fuzz/__init__.py
+-rw-r--r--   0     1001      123     1106 2023-08-02 10:12:21.000000 umka-0.1.1/umka/fuzz/fuzz.py
+-rw-r--r--   0     1001      123        0 2023-08-02 10:12:21.000000 umka-0.1.1/umka/test/__init__.py
+-rw-r--r--   0     1001      123        0 2023-08-02 10:12:21.000000 umka-0.1.1/umka/test/fuzz/__init__.py
+-rw-r--r--   0     1001      123     1214 2023-08-02 10:12:21.000000 umka-0.1.1/umka/test/fuzz/test_fuzz.py
+-rw-r--r--   0     1001      123    48299 2023-08-02 10:12:21.000000 umka-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0      223 1970-01-01 00:00:00.000000 umka-0.1.1/PKG-INFO
```

### Comparing `umka-0.1.0/Cargo.toml` & `umka-0.1.1/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "umka"
 crate-type = ["cdylib"]
 
 [dependencies]
-fuzzywuzzy = "0.0.2"
+fuzzywuzzy = { git = "https://github.com/logannc/fuzzywuzzy-rs", branch = "master" }
 polars = "0.31.1"
 polars-core = "0.31.1"
 polars-lazy = "0.31.1"
 pyo3 = "0.19.1"
 pyo3-polars = "0.5.0"
 rayon = "1.7.0"
```

### Comparing `umka-0.1.0/src/fuzzywuzzy.rs` & `umka-0.1.1/src/fuzzywuzzy.rs`

 * *Files identical despite different names*

### Comparing `umka-0.1.0/src/lib.rs` & `umka-0.1.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `umka-0.1.0/umka/fuzz/fuzz.py` & `umka-0.1.1/umka/fuzz/fuzz.py`

 * *Files identical despite different names*

### Comparing `umka-0.1.0/umka/test/fuzz/test_fuzz.py` & `umka-0.1.1/umka/test/fuzz/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `umka-0.1.0/Cargo.lock` & `umka-0.1.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -441,16 +441,19 @@
  "pin-utils",
  "slab",
 ]
 
 [[package]]
 name = "fuzzywuzzy"
 version = "0.0.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c075dcf102b63d18ebeb6ee0e8680ca8ab06da01e73e45ff187f15ef18d50350"
+source = "git+https://github.com/logannc/fuzzywuzzy-rs?branch=master#a50731b735424bd651d97a0a580da387345f59ef"
+dependencies = [
+ "unicode-normalization",
+ "unicode-segmentation",
+]
 
 [[package]]
 name = "getrandom"
 version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
 dependencies = [
@@ -1613,14 +1616,29 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.28",
 ]
 
 [[package]]
+name = "tinyvec"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
+dependencies = [
+ "tinyvec_macros",
+]
+
+[[package]]
+name = "tinyvec_macros"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
+
+[[package]]
 name = "tokio"
 version = "1.29.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "532826ff75199d5833b9d2c5fe410f29235e25704ee5f0ef599fb51c21f4a4da"
 dependencies = [
  "autocfg",
  "backtrace",
@@ -1647,14 +1665,29 @@
 [[package]]
 name = "unicode-ident"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "301abaae475aa91687eb82514b328ab47a211a533026cb25fc3e519b86adfc3c"
 
 [[package]]
+name = "unicode-normalization"
+version = "0.1.22"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
+dependencies = [
+ "tinyvec",
+]
+
+[[package]]
+name = "unicode-segmentation"
+version = "1.10.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1dd624098567895118886609431a7c3b8f516e41d30e0643f03d94592a147e36"
+
+[[package]]
 name = "unicode-width"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c0edd1e5b14653f783770bce4a4dabb4a5108a5370a5f5d8cfe8710c361f6c8b"
 
 [[package]]
 name = "unindent"
```


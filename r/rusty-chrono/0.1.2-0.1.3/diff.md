# Comparing `tmp/rusty_chrono-0.1.2.tar.gz` & `tmp/rusty_chrono-0.1.3.tar.gz`

## Comparing `rusty_chrono-0.1.2.tar` & `rusty_chrono-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0      266 1970-01-01 00:00:00.000000 rusty_chrono-0.1.2/Cargo.toml
--rw-rw-rw-   0        0        0     5297 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/.gitignore
--rw-rw-rw-   0        0        0     1448 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/.gitlab-ci.yml
--rw-rw-rw-   0        0        0      886 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/Dockerfile
--rw-rw-rw-   0        0        0     1067 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       22 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/README.md
--rw-rw-rw-   0        0        0     1751 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/publish_script.py
--rw-rw-rw-   0        0        0      335 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0     1386 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/src/dateutil/date_errors.rs
--rw-rw-rw-   0        0        0     1122 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/src/dateutil/date_functions.rs
--rw-rw-rw-   0        0        0     1649 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/src/dateutil/date_parsing.rs
--rw-rw-rw-   0        0        0     5731 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/src/dateutil/dateutil_tests/date_functions_tests.rs
--rw-rw-rw-   0        0        0     3068 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/src/dateutil/dateutil_tests/date_parsing_tests.rs
--rw-rw-rw-   0        0        0       75 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/src/dateutil/dateutil_tests/mod.rs
--rw-rw-rw-   0        0        0      124 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/src/dateutil/mod.rs
--rw-rw-rw-   0        0        0      550 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/src/dateutil/time_fractions.rs
--rw-rw-rw-   0        0        0     2849 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/src/lib.rs
--rw-rw-rw-   0        0        0      661 2023-07-30 21:53:52.000000 rusty_chrono-0.1.2/test.py
--rw-r--r--   0        0        0    14585 2023-07-30 21:54:42.000000 rusty_chrono-0.1.2/Cargo.lock
--rw-r--r--   0        0        0      324 1970-01-01 00:00:00.000000 rusty_chrono-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      316 1970-01-01 00:00:00.000000 rusty_chrono-0.1.3/Cargo.toml
+-rw-r--r--   0     1001      123     2793 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/.github/workflows/maturin_build.yml
+-rw-r--r--   0     1001      123     5297 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/.gitignore
+-rw-r--r--   0     1001      123     1890 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/.gitlab-ci.yml.old
+-rw-r--r--   0     1001      123      886 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/Dockerfile
+-rw-r--r--   0     1001      123     1067 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/LICENSE
+-rw-r--r--   0     1001      123       22 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/README.md
+-rw-r--r--   0     1001      123       70 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/build.rs
+-rw-r--r--   0     1001      123     1751 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/publish_script.py
+-rw-r--r--   0     1001      123      335 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/pyproject.toml
+-rw-r--r--   0     1001      123     1386 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/src/dateutil/date_errors.rs
+-rw-r--r--   0     1001      123     1122 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/src/dateutil/date_functions.rs
+-rw-r--r--   0     1001      123     1649 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/src/dateutil/date_parsing.rs
+-rw-r--r--   0     1001      123     5731 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/src/dateutil/dateutil_tests/date_functions_tests.rs
+-rw-r--r--   0     1001      123     3068 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/src/dateutil/dateutil_tests/date_parsing_tests.rs
+-rw-r--r--   0     1001      123       75 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/src/dateutil/dateutil_tests/mod.rs
+-rw-r--r--   0     1001      123      124 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/src/dateutil/mod.rs
+-rw-r--r--   0     1001      123      550 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/src/dateutil/time_fractions.rs
+-rw-r--r--   0     1001      123     2849 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/src/lib.rs
+-rw-r--r--   0     1001      123      661 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/test.py
+-rw-r--r--   0     1001      123    14607 2023-08-01 23:44:38.000000 rusty_chrono-0.1.3/Cargo.lock
+-rw-r--r--   0        0        0      324 1970-01-01 00:00:00.000000 rusty_chrono-0.1.3/PKG-INFO
```

### Comparing `rusty_chrono-0.1.2/.gitignore` & `rusty_chrono-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.2/.gitlab-ci.yml` & `rusty_chrono-0.1.3/.gitlab-ci.yml.old`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 image: docker:20.10.16
 variables:
   DOCKER_TLS_CERTDIR: "/certs"
+  RUST_VERSION: stable
   TAG: "latest"
 
 services:
   - docker:20.10.16-dind 
 
 stages:
-#   - image
-#   - test
+  # - image
+  # - test
   - build
-  - publish
+  # - publish
 
 
 # build_Rust_Python_image:
 #   stage: image
 #   before_script:
 #     - docker info
 #   script:
 #     - docker build -t "$DOCKER_HUB_REGISTRY/rust_python:$TAG" .
 #     - docker login --username "$DOCKER_HUB_USERNAME" --password "$DOCKER_HUB_TOKEN"
 #     - docker push "$DOCKER_HUB_REGISTRY/rust_python:$TAG"
 
-
 # rust_tests:
 #   stage: test
 #   image: "$DOCKER_HUB_REGISTRY/rust_python:$TAG"
 #   script:
 #     - cargo clean
 #     - cargo test --verbose
 
@@ -39,31 +39,46 @@
   artifacts:
     untracked: false
     when: on_success
     expire_in: "60 min"
     paths:
       - ./Cargo.toml
 
-build_project:
+# build_project_manylinux:
+#   stage: build
+#   script:
+#     - docker run --rm -v $(pwd):/io ghcr.io/pyo3/maturin build --release --sdist
+#   artifacts:
+#     untracked: true
+#     when: on_success
+#     expire_in: "60 min"
+#     paths:
+#       - target/wheels/*
+#   needs:
+#     - update_project_version
+#   dependencies:
+#     - update_project_version
+
+build_project_macos:
   stage: build
+  image: python:alpine
   script:
-    - docker run --rm -v $(pwd):/io ghcr.io/pyo3/maturin build --release --sdist
+    - apk add --no-cache gcc musl-dev libffi-dev openssl-dev cargo
+    - pip install maturin patchelf
+    - maturin build --release --interpreter python --verbose
   artifacts:
-    untracked: true
-    when: on_success
-    expire_in: "60 min"
     paths:
-      - target/wheels/*
+      - target/wheels
   needs:
     - update_project_version
   dependencies:
     - update_project_version
 
-publish_package:
-  stage: publish
-  image: python:alpine
-  script:
-    - pip install twine
-    - ls target/wheels/
-    - twine upload --verbose --username "$DOCKER_HUB_USERNAME" --password "$PYPI_PASSWORD" target/wheels/*
-  dependencies:
-    - build_project
+# publish_package:
+#   stage: publish
+#   image: python:alpine
+#   script:
+#     - pip install twine
+#     - ls target/wheels/
+#     - twine upload --verbose --username "$DOCKER_HUB_USERNAME" --password "$PYPI_PASSWORD" target/wheels/*
+#   dependencies:
+#     - build_project
```

### Comparing `rusty_chrono-0.1.2/Dockerfile` & `rusty_chrono-0.1.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.2/LICENSE` & `rusty_chrono-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.2/publish_script.py` & `rusty_chrono-0.1.3/publish_script.py`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.2/src/dateutil/date_errors.rs` & `rusty_chrono-0.1.3/src/dateutil/date_errors.rs`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.2/src/dateutil/date_functions.rs` & `rusty_chrono-0.1.3/src/dateutil/date_functions.rs`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.2/src/dateutil/date_parsing.rs` & `rusty_chrono-0.1.3/src/dateutil/date_parsing.rs`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.2/src/dateutil/dateutil_tests/date_functions_tests.rs` & `rusty_chrono-0.1.3/src/dateutil/dateutil_tests/date_functions_tests.rs`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.2/src/dateutil/dateutil_tests/date_parsing_tests.rs` & `rusty_chrono-0.1.3/src/dateutil/dateutil_tests/date_parsing_tests.rs`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.2/src/dateutil/time_fractions.rs` & `rusty_chrono-0.1.3/src/dateutil/time_fractions.rs`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.2/src/lib.rs` & `rusty_chrono-0.1.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.2/test.py` & `rusty_chrono-0.1.3/test.py`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.2/Cargo.lock` & `rusty_chrono-0.1.3/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -206,66 +206,66 @@
 checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.19.1"
+version = "0.19.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffb88ae05f306b4bfcde40ac4a51dc0b05936a9207a4b75b798c7729c4258a59"
+checksum = "e681a6cfdc4adcc93b4d3cf993749a4552018ee0a9b65fc0ccfad74352c72a38"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.19.1"
+version = "0.19.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "554db24f0b3c180a9c0b1268f91287ab3f17c162e15b54caaae5a6b3773396b0"
+checksum = "076c73d0bc438f7a4ef6fdd0c3bb4732149136abd952b110ac93e4edb13a6ba5"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.19.1"
+version = "0.19.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "922ede8759e8600ad4da3195ae41259654b9c55da4f7eec84a0ccc7d067a70a4"
+checksum = "e53cee42e77ebe256066ba8aa77eff722b3bb91f3419177cf4cd0f304d3284d9"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.19.1"
+version = "0.19.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a5caec6a1dd355964a841fcbeeb1b89fe4146c87295573f94228911af3cc5a2"
+checksum = "dfeb4c99597e136528c6dd7d5e3de5434d1ceaf487436a3f03b2d56b6fc9efd1"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.19.1"
+version = "0.19.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0b78ccbb160db1556cdb6fd96c50334c5d4ec44dc5e0a968d0a1208fa0efa8b"
+checksum = "947dc12175c254889edc0c02e399476c2f652b4b9ebd123aa655c224de259536"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
@@ -284,18 +284,19 @@
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rusty_chrono"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "chrono",
  "pyo3",
+ "pyo3-build-config",
  "test-case",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -316,28 +317,28 @@
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
 name = "target-lexicon"
-version = "0.12.10"
+version = "0.12.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d2faeef5759ab89935255b1a4cd98e0baf99d1085e37d36599c625dac49ae8e"
+checksum = "9d0e916b1148c8e263850e1ebcbd046f333e0683c724876bb0da63ea4373dc8a"
 
 [[package]]
 name = "test-case"
 version = "3.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2a1d6e7bde536b0412f20765b76e921028059adfd1b90d8974d33fd3c91b25df"
 dependencies = [
@@ -422,15 +423,15 @@
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
@@ -444,15 +445,15 @@
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
```


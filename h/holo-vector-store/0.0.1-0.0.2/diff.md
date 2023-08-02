# Comparing `tmp/holo_vector_store-0.0.1.tar.gz` & `tmp/holo_vector_store-0.0.2.tar.gz`

## Comparing `holo_vector_store-0.0.1.tar` & `holo_vector_store-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,13 @@
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 holo_vector_store-0.0.1/src/holo_vector_store/__about__.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 holo_vector_store-0.0.1/src/holo_vector_store/__init__.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 holo_vector_store-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 holo_vector_store-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 holo_vector_store-0.0.1/README.md
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 holo_vector_store-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 holo_vector_store-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 holo_vector_store-0.0.2/Develop.md
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 holo_vector_store-0.0.2/env.sh
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 holo_vector_store-0.0.2/src/holo_vector_store/__about__.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 holo_vector_store-0.0.2/src/holo_vector_store/__init__.py
+-rw-r--r--   0        0        0     5742 2020-02-02 00:00:00.000000 holo_vector_store-0.0.2/src/holo_vector_store/holo_vector_store.py
+-rw-r--r--   0        0        0     6934 2020-02-02 00:00:00.000000 holo_vector_store-0.0.2/src/holo_vector_store/hologres_wrapper.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 holo_vector_store-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 holo_vector_store-0.0.2/tests/test_holo_vector_store.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 holo_vector_store-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 holo_vector_store-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 holo_vector_store-0.0.2/README.md
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 holo_vector_store-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 holo_vector_store-0.0.2/PKG-INFO
```

### Comparing `holo_vector_store-0.0.1/README.md` & `holo_vector_store-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `holo_vector_store-0.0.1/pyproject.toml` & `holo_vector_store-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -20,31 +20,36 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
-dependencies = []
+dependencies = [
+  "psycopg2-binary",
+  "typing",
+  "uuid",
+]
 
 [project.urls]
 Documentation = "https://github.com/unknown/holo-vector-store#readme"
 Issues = "https://github.com/unknown/holo-vector-store/issues"
 Source = "https://github.com/unknown/holo-vector-store"
 
 [tool.hatch.version]
 path = "src/holo_vector_store/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
+  "pytest-xdist",
 ]
 [tool.hatch.envs.default.scripts]
-test = "pytest {args:tests}"
+test = "pytest -n 8 -v {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
   "coverage report",
 ]
 cov = [
   "test-cov",
@@ -109,27 +114,33 @@
   "T",
   "TID",
   "UP",
   "W",
   "YTT",
 ]
 ignore = [
+  # shadowing a Python builtin
+  "A002",
   # Allow non-abstract empty methods in abstract base classes
   "B027",
   # Allow boolean positional values in function calls, like `dict.get(... True)`
+  "FBT001",
+  "FBT002",
   "FBT003",
   # Ignore checks for possible passwords
   "S105", "S106", "S107",
   # Ignore complexity
   "C901", "PLR0911", "PLR0912", "PLR0913", "PLR0915",
-]
-unfixable = [
+  # Ignore SQL injection
+  "S608",
   # Don't touch unused imports
   "F401",
 ]
+unfixable = [
+]
 
 [tool.ruff.isort]
 known-first-party = ["holo_vector_store"]
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
 
@@ -151,7 +162,16 @@
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
+
+[tool.hatch.build.targets.sdist]
+exclude = [
+  "/.github",
+  "/docs",
+]
+
+[tool.hatch.build.targets.wheel]
+packages = ["src/holo_vector_store"]
```

### Comparing `holo_vector_store-0.0.1/PKG-INFO` & `holo_vector_store-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holo-vector-store
-Version: 0.0.1
+Version: 0.0.2
 Project-URL: Documentation, https://github.com/unknown/holo-vector-store#readme
 Project-URL: Issues, https://github.com/unknown/holo-vector-store/issues
 Project-URL: Source, https://github.com/unknown/holo-vector-store
 Author-email: Changgeng Zhao <zhaochanggeng.zcg@alibaba-inc.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -13,14 +13,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
+Requires-Dist: psycopg2-binary
+Requires-Dist: typing
+Requires-Dist: uuid
 Description-Content-Type: text/markdown
 
 # holo-vector-store
 
 [![PyPI - Version](https://img.shields.io/pypi/v/holo-vector-store.svg)](https://pypi.org/project/holo-vector-store)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/holo-vector-store.svg)](https://pypi.org/project/holo-vector-store)
```


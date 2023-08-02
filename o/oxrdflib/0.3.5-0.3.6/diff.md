# Comparing `tmp/oxrdflib-0.3.5.tar.gz` & `tmp/oxrdflib-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oxrdflib-0.3.5.tar", last modified: Wed Jun 21 19:54:38 2023, max compression
+gzip compressed data, was "oxrdflib-0.3.6.tar", last modified: Wed Aug  2 16:35:20 2023, max compression
```

## Comparing `oxrdflib-0.3.5.tar` & `oxrdflib-0.3.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:54:38.870157 oxrdflib-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:54:38.866157 oxrdflib-0.3.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:54:38.866157 oxrdflib-0.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-06-21 19:54:38.870157 oxrdflib-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:54:38.866157 oxrdflib-0.3.5/oxrdflib/
--rw-r--r--   0 runner    (1001) docker     (123)    10349 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/oxrdflib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/oxrdflib/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:54:38.870157 oxrdflib-0.3.5/oxrdflib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-06-21 19:54:38.000000 oxrdflib-0.3.5/oxrdflib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-21 19:54:38.000000 oxrdflib-0.3.5/oxrdflib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:54:38.000000 oxrdflib-0.3.5/oxrdflib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-21 19:54:38.000000 oxrdflib-0.3.5/oxrdflib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-21 19:54:38.000000 oxrdflib-0.3.5/oxrdflib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 19:54:38.000000 oxrdflib-0.3.5/oxrdflib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 19:54:38.870157 oxrdflib-0.3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:54:38.870157 oxrdflib-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    14015 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/tests/test_graph_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/tests/test_sparql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/tests/test_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:35:20.764510 oxrdflib-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-02 16:35:11.000000 oxrdflib-0.3.6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:35:20.764510 oxrdflib-0.3.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-08-02 16:35:11.000000 oxrdflib-0.3.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:35:20.764510 oxrdflib-0.3.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-08-02 16:35:11.000000 oxrdflib-0.3.6/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-02 16:35:11.000000 oxrdflib-0.3.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-02 16:35:11.000000 oxrdflib-0.3.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-08-02 16:35:11.000000 oxrdflib-0.3.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-08-02 16:35:11.000000 oxrdflib-0.3.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-08-02 16:35:20.764510 oxrdflib-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-08-02 16:35:11.000000 oxrdflib-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:35:20.764510 oxrdflib-0.3.6/oxrdflib/
+-rw-r--r--   0 runner    (1001) docker     (123)    10349 2023-08-02 16:35:11.000000 oxrdflib-0.3.6/oxrdflib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:35:11.000000 oxrdflib-0.3.6/oxrdflib/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:35:20.764510 oxrdflib-0.3.6/oxrdflib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-08-02 16:35:20.000000 oxrdflib-0.3.6/oxrdflib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-02 16:35:20.000000 oxrdflib-0.3.6/oxrdflib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:35:20.000000 oxrdflib-0.3.6/oxrdflib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-02 16:35:20.000000 oxrdflib-0.3.6/oxrdflib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 16:35:20.000000 oxrdflib-0.3.6/oxrdflib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 16:35:20.000000 oxrdflib-0.3.6/oxrdflib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-08-02 16:35:11.000000 oxrdflib-0.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 16:35:11.000000 oxrdflib-0.3.6/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 16:35:20.764510 oxrdflib-0.3.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:35:20.764510 oxrdflib-0.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-08-02 16:35:11.000000 oxrdflib-0.3.6/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-08-02 16:35:11.000000 oxrdflib-0.3.6/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14015 2023-08-02 16:35:11.000000 oxrdflib-0.3.6/tests/test_graph_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-08-02 16:35:11.000000 oxrdflib-0.3.6/tests/test_sparql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-08-02 16:35:11.000000 oxrdflib-0.3.6/tests/test_store.py
```

### Comparing `oxrdflib-0.3.5/.github/workflows/build.yml` & `oxrdflib-0.3.6/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `oxrdflib-0.3.5/.pre-commit-config.yaml` & `oxrdflib-0.3.6/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -20,19 +20,19 @@
       - id: detect-private-key
       - id: end-of-file-fixer
       - id: fix-byte-order-marker
       - id: mixed-line-ending
       - id: requirements-txt-fixer
       - id: trailing-whitespace
   - repo: https://github.com/ambv/black
-    rev: 23.3.0
+    rev: 23.7.0
     hooks:
       - id: black
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.272
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.0.282
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.3.0
+    rev: v1.4.1
     hooks:
       - id: mypy
```

### Comparing `oxrdflib-0.3.5/CHANGELOG.md` & `oxrdflib-0.3.6/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## [0.3.6] - 2023-08-02
+
+### Added
+- Compatibility with rdflib 7.0
+
+
 ## [0.3.5] - 2023-06-21
 
 ### Changed
 - Fixes `Store.triples` and `Store.context` return types.
 
 
 ## [0.3.4] - 2023-04-22
```

### Comparing `oxrdflib-0.3.5/LICENSE.md` & `oxrdflib-0.3.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `oxrdflib-0.3.5/PKG-INFO` & `oxrdflib-0.3.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxrdflib
-Version: 0.3.5
+Version: 0.3.6
 Summary: rdflib stores based on pyoxigraph
 Author-email: Tpt <thomas@pellissier-tanon.fr>
 License: BSD-3-Clause
 Project-URL: Changelog, https://github.com/oxigraph/oxrdflib/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://github.com/oxigraph/oxrdflib/blob/main/README.md
 Project-URL: Homepage, https://github.com/oxigraph/oxrdflib
 Project-URL: Source, https://github.com/oxigraph/oxrdflib
@@ -79,15 +79,15 @@
 instead of the usual
 ```python
 rdflib.Dataset()
 ```
 
 If you want to get the store data persisted on disk, use the `open` method on the `Graph` object (or `ConjunctiveGraph` or `Dataset`) with the directory where data should be persisted. For example:
 ```python
-graph = rdflib.Graph(store="Oxigraph")
+graph = rdflib.Graph(store="Oxigraph", identifier="http://example.com") # without identifier, some blank node will be used
 graph.open("test_dir")
 ```
 The store is closed with the `close()` method or automatically when Python garbage collector collects the store object.
 
 If the `open` method is not called Oxigraph will automatically use a ramdisk on Linux and a temporary file in the other operating systems.
 
 To do anything else, use the usual rdflib python API.
```

### Comparing `oxrdflib-0.3.5/README.md` & `oxrdflib-0.3.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 instead of the usual
 ```python
 rdflib.Dataset()
 ```
 
 If you want to get the store data persisted on disk, use the `open` method on the `Graph` object (or `ConjunctiveGraph` or `Dataset`) with the directory where data should be persisted. For example:
 ```python
-graph = rdflib.Graph(store="Oxigraph")
+graph = rdflib.Graph(store="Oxigraph", identifier="http://example.com") # without identifier, some blank node will be used
 graph.open("test_dir")
 ```
 The store is closed with the `close()` method or automatically when Python garbage collector collects the store object.
 
 If the `open` method is not called Oxigraph will automatically use a ramdisk on Linux and a temporary file in the other operating systems.
 
 To do anything else, use the usual rdflib python API.
```

### Comparing `oxrdflib-0.3.5/oxrdflib/__init__.py` & `oxrdflib-0.3.6/oxrdflib/__init__.py`

 * *Files identical despite different names*

### Comparing `oxrdflib-0.3.5/oxrdflib.egg-info/PKG-INFO` & `oxrdflib-0.3.6/oxrdflib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxrdflib
-Version: 0.3.5
+Version: 0.3.6
 Summary: rdflib stores based on pyoxigraph
 Author-email: Tpt <thomas@pellissier-tanon.fr>
 License: BSD-3-Clause
 Project-URL: Changelog, https://github.com/oxigraph/oxrdflib/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://github.com/oxigraph/oxrdflib/blob/main/README.md
 Project-URL: Homepage, https://github.com/oxigraph/oxrdflib
 Project-URL: Source, https://github.com/oxigraph/oxrdflib
@@ -79,15 +79,15 @@
 instead of the usual
 ```python
 rdflib.Dataset()
 ```
 
 If you want to get the store data persisted on disk, use the `open` method on the `Graph` object (or `ConjunctiveGraph` or `Dataset`) with the directory where data should be persisted. For example:
 ```python
-graph = rdflib.Graph(store="Oxigraph")
+graph = rdflib.Graph(store="Oxigraph", identifier="http://example.com") # without identifier, some blank node will be used
 graph.open("test_dir")
 ```
 The store is closed with the `close()` method or automatically when Python garbage collector collects the store object.
 
 If the `open` method is not called Oxigraph will automatically use a ramdisk on Linux and a temporary file in the other operating systems.
 
 To do anything else, use the usual rdflib python API.
```

### Comparing `oxrdflib-0.3.5/pyproject.toml` & `oxrdflib-0.3.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: BSD License",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Database :: Database Engines/Servers"
 ]
 dependencies = [
     "pyoxigraph~=0.3.14",
-    "rdflib~=6.3"
+    "rdflib>=6.3,<8.0"
 ]
 dynamic = ["version"]
 license = { text = "BSD-3-Clause" }
 name = "oxrdflib"
 readme = "README.md"
 requires-python = ">=3.7"
 
@@ -52,18 +52,20 @@
 select = [
     "ARG",
     "B",
     "C40",
     "C901",
     "E",
     "F",
+    "FLY",
     "I",
     "ICN",
     "ISC",
     "N",
+    "PERF",
     "PIE",
     "PTH",
     "RET",
     "RUF",
     "SIM",
     "T10",
     "TCH",
```

### Comparing `oxrdflib-0.3.5/tests/test_dataset.py` & `oxrdflib-0.3.6/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `oxrdflib-0.3.5/tests/test_graph.py` & `oxrdflib-0.3.6/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `oxrdflib-0.3.5/tests/test_graph_context.py` & `oxrdflib-0.3.6/tests/test_graph_context.py`

 * *Files identical despite different names*

### Comparing `oxrdflib-0.3.5/tests/test_sparql.py` & `oxrdflib-0.3.6/tests/test_sparql.py`

 * *Files identical despite different names*

### Comparing `oxrdflib-0.3.5/tests/test_store.py` & `oxrdflib-0.3.6/tests/test_store.py`

 * *Files identical despite different names*


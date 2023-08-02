# Comparing `tmp/polywrap_manifest-0.1.0b2.tar.gz` & `tmp/polywrap_manifest-0.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_manifest-0.1.0b2.tar", max compression
+gzip compressed data, was "polywrap_manifest-0.1.0b3.tar", max compression
```

## Comparing `polywrap_manifest-0.1.0b2.tar` & `polywrap_manifest-0.1.0b3.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0      422 2023-04-10 13:52:54.309380 polywrap_manifest-0.1.0b2/README.md
--rw-r--r--   0        0        0      162 2023-04-10 13:52:54.307059 polywrap_manifest-0.1.0b2/polywrap_manifest/__init__.py
--rw-r--r--   0        0        0     2177 2023-06-15 11:56:46.969345 polywrap_manifest-0.1.0b2/polywrap_manifest/deserialize.py
--rw-r--r--   0        0        0      328 2023-06-15 11:56:46.969741 polywrap_manifest-0.1.0b2/polywrap_manifest/errors.py
--rw-r--r--   0        0        0     2056 2023-06-15 11:56:46.969967 polywrap_manifest-0.1.0b2/polywrap_manifest/manifest.py
--rw-r--r--   0        0        0        0 2023-04-10 13:52:54.307367 polywrap_manifest-0.1.0b2/polywrap_manifest/py.typed
--rw-r--r--   0        0        0     8911 2023-04-10 13:52:54.309172 polywrap_manifest-0.1.0b2/polywrap_manifest/wrap_0_1.py
--rw-r--r--   0        0        0     1201 2023-08-02 11:15:13.495551 polywrap_manifest-0.1.0b2/pyproject.toml
--rw-r--r--   0        0        0     1092 1970-01-01 00:00:00.000000 polywrap_manifest-0.1.0b2/setup.py
--rw-r--r--   0        0        0      868 1970-01-01 00:00:00.000000 polywrap_manifest-0.1.0b2/PKG-INFO
+-rw-r--r--   0        0        0      422 2023-08-02 16:06:36.159338 polywrap_manifest-0.1.0b3/README.md
+-rw-r--r--   0        0        0      162 2023-08-02 16:06:36.159338 polywrap_manifest-0.1.0b3/polywrap_manifest/__init__.py
+-rw-r--r--   0        0        0     2177 2023-08-02 16:06:36.159338 polywrap_manifest-0.1.0b3/polywrap_manifest/deserialize.py
+-rw-r--r--   0        0        0      328 2023-08-02 16:06:36.159338 polywrap_manifest-0.1.0b3/polywrap_manifest/errors.py
+-rw-r--r--   0        0        0     2056 2023-08-02 16:06:36.159338 polywrap_manifest-0.1.0b3/polywrap_manifest/manifest.py
+-rw-r--r--   0        0        0        0 2023-08-02 16:06:36.159338 polywrap_manifest-0.1.0b3/polywrap_manifest/py.typed
+-rw-r--r--   0        0        0     8911 2023-08-02 16:06:36.159338 polywrap_manifest-0.1.0b3/polywrap_manifest/wrap_0_1.py
+-rw-r--r--   0        0        0     1201 2023-08-02 16:08:09.161454 polywrap_manifest-0.1.0b3/pyproject.toml
+-rw-r--r--   0        0        0      868 1970-01-01 00:00:00.000000 polywrap_manifest-0.1.0b3/PKG-INFO
```

### Comparing `polywrap_manifest-0.1.0b2/polywrap_manifest/deserialize.py` & `polywrap_manifest-0.1.0b3/polywrap_manifest/deserialize.py`

 * *Files identical despite different names*

### Comparing `polywrap_manifest-0.1.0b2/polywrap_manifest/manifest.py` & `polywrap_manifest-0.1.0b3/polywrap_manifest/manifest.py`

 * *Files identical despite different names*

### Comparing `polywrap_manifest-0.1.0b2/polywrap_manifest/wrap_0_1.py` & `polywrap_manifest-0.1.0b3/polywrap_manifest/wrap_0_1.py`

 * *Files identical despite different names*

### Comparing `polywrap_manifest-0.1.0b2/pyproject.toml` & `polywrap_manifest-0.1.0b3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-manifest"
-version = "0.1.0b2"
+version = "0.1.0b3"
 description = "WRAP manifest"
 authors = ["Niraj <niraj@polywrap.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "^1.10.2"
-polywrap-msgpack = "^0.1.0b2"
+polywrap-msgpack = "^0.1.0b3"
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pylint = "^2.15.4"
 black = "^22.10.0"
 bandit = { version = "^1.7.4", extras = ["toml"]}
 tox = "^3.26.0"
 tox-poetry = "^0.4.1"
```

### Comparing `polywrap_manifest-0.1.0b2/PKG-INFO` & `polywrap_manifest-0.1.0b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: polywrap-manifest
-Version: 0.1.0b2
+Version: 0.1.0b3
 Summary: WRAP manifest
 Author: Niraj
 Author-email: niraj@polywrap.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: polywrap-msgpack (>=0.1.0b2,<0.2.0)
+Requires-Dist: polywrap-msgpack (>=0.1.0b3,<0.2.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 # polywrap-manifest
 
 Python implementation of the WRAP manifest schema at https://github.com/polywrap/wrap
```


# Comparing `tmp/tum_esm_em27_metadata-2.0.0rc4.tar.gz` & `tmp/tum_esm_em27_metadata-2.0.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tum_esm_em27_metadata-2.0.0rc4.tar", max compression
+gzip compressed data, was "tum_esm_em27_metadata-2.0.0rc5.tar", max compression
```

## Comparing `tum_esm_em27_metadata-2.0.0rc4.tar` & `tum_esm_em27_metadata-2.0.0rc5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3990 2023-08-02 12:33:06.624704 tum_esm_em27_metadata-2.0.0rc4/README.md
--rw-r--r--   0        0        0     1137 2023-08-02 12:25:22.653875 tum_esm_em27_metadata-2.0.0rc4/pyproject.toml
--rw-r--r--   0        0        0      126 2023-04-23 10:28:10.736200 tum_esm_em27_metadata-2.0.0rc4/tum_esm_em27_metadata/__init__.py
--rw-r--r--   0        0        0    13975 2023-08-02 12:25:22.654638 tum_esm_em27_metadata-2.0.0rc4/tum_esm_em27_metadata/interfaces.py
--rw-r--r--   0        0        0     2112 2023-04-23 11:12:48.008464 tum_esm_em27_metadata-2.0.0rc4/tum_esm_em27_metadata/loader.py
--rw-r--r--   0        0        0        0 2023-04-19 09:38:48.570525 tum_esm_em27_metadata-2.0.0rc4/tum_esm_em27_metadata/py.typed
--rw-r--r--   0        0        0     5517 2023-08-02 12:25:22.654845 tum_esm_em27_metadata-2.0.0rc4/tum_esm_em27_metadata/types.py
--rw-r--r--   0        0        0     4704 1970-01-01 00:00:00.000000 tum_esm_em27_metadata-2.0.0rc4/PKG-INFO
+-rw-r--r--   0        0        0     3990 2023-08-02 12:33:06.624704 tum_esm_em27_metadata-2.0.0rc5/README.md
+-rw-r--r--   0        0        0     1146 2023-08-02 14:39:56.395118 tum_esm_em27_metadata-2.0.0rc5/pyproject.toml
+-rw-r--r--   0        0        0      126 2023-04-23 10:28:10.736200 tum_esm_em27_metadata-2.0.0rc5/tum_esm_em27_metadata/__init__.py
+-rw-r--r--   0        0        0    13975 2023-08-02 12:25:22.654638 tum_esm_em27_metadata-2.0.0rc5/tum_esm_em27_metadata/interfaces.py
+-rw-r--r--   0        0        0     2112 2023-04-23 11:12:48.008464 tum_esm_em27_metadata-2.0.0rc5/tum_esm_em27_metadata/loader.py
+-rw-r--r--   0        0        0        0 2023-04-19 09:38:48.570525 tum_esm_em27_metadata-2.0.0rc5/tum_esm_em27_metadata/py.typed
+-rw-r--r--   0        0        0     5517 2023-08-02 12:25:22.654845 tum_esm_em27_metadata-2.0.0rc5/tum_esm_em27_metadata/types.py
+-rw-r--r--   0        0        0     4704 1970-01-01 00:00:00.000000 tum_esm_em27_metadata-2.0.0rc5/PKG-INFO
```

### Comparing `tum_esm_em27_metadata-2.0.0rc4/README.md` & `tum_esm_em27_metadata-2.0.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `tum_esm_em27_metadata-2.0.0rc4/pyproject.toml` & `tum_esm_em27_metadata-2.0.0rc5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "tum_esm_em27_metadata"
-version = "2.0.0-rc.4"
+version = "2.0.0-rc.5"
 description = "Single source of truth for ESM's EM27 measurement logistics"
 readme = "README.md"
 authors = [
     "Moritz Makowski <moritz.makowski@tum.de>",
-    "Marlon Mueller <marlon.mueller@tum.de>"
+    "Marlon Mueller <marlon.mueller@tum.de>",
 ]
 packages = [
-    {include = "tum_esm_em27_metadata"},
-    {include = "tum_esm_em27_metadata/py.typed"},
+    { include = "tum_esm_em27_metadata" },
+    { include = "tum_esm_em27_metadata/py.typed" },
 ]
 repository = "https://github.com/tum-esm/em27-metadata"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 tum-esm-utils = "^1.4.0"
 pendulum = "^2.1.2"
@@ -28,15 +28,15 @@
 mypy = "^1.2.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
-line-length=100
+line-length = 100
 
 [tool.mypy]
 strict = true
 implicit_reexport = true
 no_warn_unused_ignores = true
 plugins = ["pydantic.mypy"]
 
@@ -45,9 +45,9 @@
 module = ["pendulum"]
 ignore_missing_imports = true
 
 [tool.pytest.ini_options]
 markers = [
     "ci: run in GitHub CI",
     "action: run when using this repo as a GitHub Action",
-    "local: run locally"
-]
+    "local: run locally",
+]
```

### Comparing `tum_esm_em27_metadata-2.0.0rc4/tum_esm_em27_metadata/interfaces.py` & `tum_esm_em27_metadata-2.0.0rc5/tum_esm_em27_metadata/interfaces.py`

 * *Files identical despite different names*

### Comparing `tum_esm_em27_metadata-2.0.0rc4/tum_esm_em27_metadata/loader.py` & `tum_esm_em27_metadata-2.0.0rc5/tum_esm_em27_metadata/loader.py`

 * *Files identical despite different names*

### Comparing `tum_esm_em27_metadata-2.0.0rc4/tum_esm_em27_metadata/types.py` & `tum_esm_em27_metadata-2.0.0rc5/tum_esm_em27_metadata/types.py`

 * *Files identical despite different names*

### Comparing `tum_esm_em27_metadata-2.0.0rc4/PKG-INFO` & `tum_esm_em27_metadata-2.0.0rc5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tum-esm-em27-metadata
-Version: 2.0.0rc4
+Version: 2.0.0rc5
 Summary: Single source of truth for ESM's EM27 measurement logistics
 Home-page: https://github.com/tum-esm/em27-metadata
 Author: Moritz Makowski
 Author-email: moritz.makowski@tum.de
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```


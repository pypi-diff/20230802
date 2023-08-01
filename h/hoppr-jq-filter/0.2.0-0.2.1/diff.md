# Comparing `tmp/hoppr_jq_filter-0.2.0.tar.gz` & `tmp/hoppr_jq_filter-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoppr_jq_filter-0.2.0.tar", max compression
+gzip compressed data, was "hoppr_jq_filter-0.2.1.tar", max compression
```

## Comparing `hoppr_jq_filter-0.2.0.tar` & `hoppr_jq_filter-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1084 2023-07-27 14:35:48.000000 hoppr_jq_filter-0.2.0/LICENSE
--rw-r--r--   0        0        0     1764 2023-07-27 14:35:48.000000 hoppr_jq_filter-0.2.0/README.md
--rw-r--r--   0        0        0       77 2023-07-27 14:35:48.000000 hoppr_jq_filter-0.2.0/hoppr_jq_filter/__init__.py
--rw-r--r--   0        0        0     5356 2023-07-27 14:35:48.000000 hoppr_jq_filter-0.2.0/hoppr_jq_filter/plugin.py
--rw-r--r--   0        0        0        0 2023-07-27 14:35:48.000000 hoppr_jq_filter-0.2.0/hoppr_jq_filter/py.typed
--rw-r--r--   0        0        0     1087 2023-07-27 14:35:48.000000 hoppr_jq_filter-0.2.0/hoppr_jq_filter/renovate.json
--rw-r--r--   0        0        0     2592 2023-07-27 14:35:48.000000 hoppr_jq_filter-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3000 1970-01-01 00:00:00.000000 hoppr_jq_filter-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-08-01 22:04:57.000000 hoppr_jq_filter-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1764 2023-08-01 22:04:57.000000 hoppr_jq_filter-0.2.1/README.md
+-rw-r--r--   0        0        0       77 2023-08-01 22:04:57.000000 hoppr_jq_filter-0.2.1/hoppr_jq_filter/__init__.py
+-rw-r--r--   0        0        0     5356 2023-08-01 22:04:57.000000 hoppr_jq_filter-0.2.1/hoppr_jq_filter/plugin.py
+-rw-r--r--   0        0        0        0 2023-08-01 22:04:57.000000 hoppr_jq_filter-0.2.1/hoppr_jq_filter/py.typed
+-rw-r--r--   0        0        0     1087 2023-08-01 22:04:57.000000 hoppr_jq_filter-0.2.1/hoppr_jq_filter/renovate.json
+-rw-r--r--   0        0        0     2592 2023-08-01 22:04:57.000000 hoppr_jq_filter-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3000 1970-01-01 00:00:00.000000 hoppr_jq_filter-0.2.1/PKG-INFO
```

### Comparing `hoppr_jq_filter-0.2.0/LICENSE` & `hoppr_jq_filter-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hoppr_jq_filter-0.2.0/README.md` & `hoppr_jq_filter-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `hoppr_jq_filter-0.2.0/hoppr_jq_filter/plugin.py` & `hoppr_jq_filter-0.2.1/hoppr_jq_filter/plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr_jq_filter-0.2.0/hoppr_jq_filter/renovate.json` & `hoppr_jq_filter-0.2.1/hoppr_jq_filter/renovate.json`

 * *Files identical despite different names*

### Comparing `hoppr_jq_filter-0.2.0/pyproject.toml` & `hoppr_jq_filter-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hoppr_jq_filter"
-version = "0.2.0"
+version = "0.2.1"
 description = "Starter Plug-in for Hoppr"
 authors = ["LMCO Open Source <open.source@lmco.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://hoppr.dev/"
 
 keywords = [
```

### Comparing `hoppr_jq_filter-0.2.0/PKG-INFO` & `hoppr_jq_filter-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoppr-jq-filter
-Version: 0.2.0
+Version: 0.2.1
 Summary: Starter Plug-in for Hoppr
 Home-page: https://hoppr.dev/
 License: MIT
 Keywords: hoppr,plugin,packaging,reports,build dependencies,software bill of materials
 Author: LMCO Open Source
 Author-email: open.source@lmco.com
 Requires-Python: >=3.10,<4.0
```


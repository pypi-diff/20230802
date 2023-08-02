# Comparing `tmp/fmsfdata2-0.1.0.tar.gz` & `tmp/fmsfdata2-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmsfdata2-0.1.0.tar", max compression
+gzip compressed data, was "fmsfdata2-1.0.0.tar", max compression
```

## Comparing `fmsfdata2-0.1.0.tar` & `fmsfdata2-1.0.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     2200 2023-07-26 16:25:20.011374 fmsfdata2-0.1.0/README.md
--rw-r--r--   0        0        0       61 2023-08-02 09:04:23.701820 fmsfdata2-0.1.0/fmsfdata2/__init__.py
--rw-r--r--   0        0        0     1278 2023-08-02 13:17:51.725930 fmsfdata2-0.1.0/fmsfdata2/converter.py
--rw-r--r--   0        0        0      216 2023-07-31 11:10:27.203006 fmsfdata2-0.1.0/fmsfdata2/datastore/__init__.py
--rw-r--r--   0        0        0     1726 2023-07-31 12:01:41.140145 fmsfdata2-0.1.0/fmsfdata2/datastore/_store.py
--rw-r--r--   0        0        0     1775 2023-07-31 11:10:27.204118 fmsfdata2-0.1.0/fmsfdata2/datastore/_table.py
--rw-r--r--   0        0        0      480 2023-07-31 11:10:27.204508 fmsfdata2-0.1.0/fmsfdata2/datastore/_table_key.py
--rw-r--r--   0        0        0     2116 2023-07-31 11:10:27.204876 fmsfdata2-0.1.0/fmsfdata2/datastore/_table_row.py
--rw-r--r--   0        0        0     2805 2023-08-02 13:17:51.725964 fmsfdata2-0.1.0/fmsfdata2/exporter.py
--rw-r--r--   0        0        0     2061 2023-08-02 13:17:51.725831 fmsfdata2-0.1.0/fmsfdata2/identifier.py
--rw-r--r--   0        0        0     2909 2023-08-02 13:17:51.725881 fmsfdata2-0.1.0/fmsfdata2/normaliser.py
--rw-r--r--   0        0        0       51 2023-07-31 11:10:27.206997 fmsfdata2-0.1.0/fmsfdata2/schema/__init__.py
--rw-r--r--   0        0        0    13068 2023-08-02 12:56:48.724000 fmsfdata2-0.1.0/fmsfdata2/schema/_data.py
--rw-r--r--   0        0        0     9679 2023-07-31 11:10:27.208128 fmsfdata2-0.1.0/fmsfdata2/schema/_proxy.py
--rw-r--r--   0        0        0      164 2023-07-31 11:10:27.208691 fmsfdata2-0.1.0/fmsfdata2/schema/_types.py
--rw-r--r--   0        0        0     1224 2023-08-02 13:17:51.725794 fmsfdata2-0.1.0/fmsfdata2/schema/erd/__init__.py
--rw-r--r--   0        0        0      957 2023-07-31 11:10:27.209771 fmsfdata2-0.1.0/fmsfdata2/schema/erd/templates/erd.dot
--rw-r--r--   0        0        0      703 2023-08-02 13:17:51.725340 fmsfdata2-0.1.0/fmsfdata2/schema/parser/__init__.py
--rw-r--r--   0        0        0     1304 2023-08-02 12:56:48.724555 fmsfdata2-0.1.0/fmsfdata2/settings.py
--rw-r--r--   0        0        0     1555 2023-08-02 13:17:51.725733 fmsfdata2-0.1.0/fmsfdata2/standardiser.py
--rw-r--r--   0        0        0       22 2023-07-26 13:36:28.982395 fmsfdata2-0.1.0/fmsfdata2/stream_parser/__init__.py
--rw-r--r--   0        0        0     1636 2023-08-02 13:17:51.725245 fmsfdata2-0.1.0/fmsfdata2/stream_parser/checks.py
--rw-r--r--   0        0        0     7178 2023-08-02 13:17:51.725316 fmsfdata2-0.1.0/fmsfdata2/stream_parser/collectors.py
--rw-r--r--   0        0        0     1790 2023-08-02 13:09:34.836657 fmsfdata2-0.1.0/fmsfdata2/stream_parser/events.py
--rw-r--r--   0        0        0        0 2023-07-26 13:36:28.983244 fmsfdata2-0.1.0/fmsfdata2/stream_parser/filters/__init__.py
--rw-r--r--   0        0        0     2178 2023-08-02 13:17:51.725183 fmsfdata2-0.1.0/fmsfdata2/stream_parser/filters/column_headers.py
--rw-r--r--   0        0        0     1798 2023-08-02 13:17:51.726235 fmsfdata2-0.1.0/fmsfdata2/stream_parser/filters/context.py
--rw-r--r--   0        0        0     6114 2023-08-02 13:17:51.725141 fmsfdata2-0.1.0/fmsfdata2/stream_parser/filters/generic.py
--rw-r--r--   0        0        0     2433 2023-08-02 13:17:51.686261 fmsfdata2-0.1.0/fmsfdata2/stream_parser/filters/types.py
--rw-r--r--   0        0        0     2056 2023-08-02 13:17:51.725293 fmsfdata2-0.1.0/fmsfdata2/stream_parser/function_helpers.py
--rw-r--r--   0        0        0      429 2023-08-02 13:17:51.725262 fmsfdata2-0.1.0/fmsfdata2/stream_parser/functions.py
--rw-r--r--   0        0        0        0 2023-07-26 13:36:28.984861 fmsfdata2-0.1.0/fmsfdata2/stream_parser/parser/__init__.py
--rw-r--r--   0        0        0      528 2023-08-02 13:17:51.665185 fmsfdata2-0.1.0/fmsfdata2/stream_parser/parser/csv.py
--rw-r--r--   0        0        0     1876 2023-08-02 13:17:51.664927 fmsfdata2-0.1.0/fmsfdata2/stream_parser/parser/openpyxl.py
--rw-r--r--   0        0        0     1138 2023-08-02 13:17:51.664759 fmsfdata2-0.1.0/fmsfdata2/stream_parser/parser/xml.py
--rw-r--r--   0        0        0      485 2023-08-02 13:17:51.725212 fmsfdata2-0.1.0/fmsfdata2/stream_parser/stream.py
--rw-r--r--   0        0        0      296 2023-08-02 13:17:51.726120 fmsfdata2-0.1.0/fmsfdata2/stream_parser/types.py
--rw-r--r--   0        0        0      619 2023-08-02 13:18:19.187872 fmsfdata2-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2953 1970-01-01 00:00:00.000000 fmsfdata2-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2200 2023-07-26 16:25:20.011374 fmsfdata2-1.0.0/README.md
+-rw-r--r--   0        0        0       61 2023-08-02 09:04:23.701820 fmsfdata2-1.0.0/fmsfdata2/__init__.py
+-rw-r--r--   0        0        0     1278 2023-08-02 13:17:51.725930 fmsfdata2-1.0.0/fmsfdata2/converter.py
+-rw-r--r--   0        0        0      216 2023-07-31 11:10:27.203006 fmsfdata2-1.0.0/fmsfdata2/datastore/__init__.py
+-rw-r--r--   0        0        0     1726 2023-07-31 12:01:41.140145 fmsfdata2-1.0.0/fmsfdata2/datastore/_store.py
+-rw-r--r--   0        0        0     1775 2023-07-31 11:10:27.204118 fmsfdata2-1.0.0/fmsfdata2/datastore/_table.py
+-rw-r--r--   0        0        0      480 2023-07-31 11:10:27.204508 fmsfdata2-1.0.0/fmsfdata2/datastore/_table_key.py
+-rw-r--r--   0        0        0     2116 2023-07-31 11:10:27.204876 fmsfdata2-1.0.0/fmsfdata2/datastore/_table_row.py
+-rw-r--r--   0        0        0     2805 2023-08-02 13:17:51.725964 fmsfdata2-1.0.0/fmsfdata2/exporter.py
+-rw-r--r--   0        0        0     2061 2023-08-02 13:17:51.725831 fmsfdata2-1.0.0/fmsfdata2/identifier.py
+-rw-r--r--   0        0        0     2909 2023-08-02 13:17:51.725881 fmsfdata2-1.0.0/fmsfdata2/normaliser.py
+-rw-r--r--   0        0        0       51 2023-07-31 11:10:27.206997 fmsfdata2-1.0.0/fmsfdata2/schema/__init__.py
+-rw-r--r--   0        0        0    13068 2023-08-02 12:56:48.724000 fmsfdata2-1.0.0/fmsfdata2/schema/_data.py
+-rw-r--r--   0        0        0     9679 2023-07-31 11:10:27.208128 fmsfdata2-1.0.0/fmsfdata2/schema/_proxy.py
+-rw-r--r--   0        0        0      164 2023-07-31 11:10:27.208691 fmsfdata2-1.0.0/fmsfdata2/schema/_types.py
+-rw-r--r--   0        0        0     1224 2023-08-02 13:17:51.725794 fmsfdata2-1.0.0/fmsfdata2/schema/erd/__init__.py
+-rw-r--r--   0        0        0      957 2023-07-31 11:10:27.209771 fmsfdata2-1.0.0/fmsfdata2/schema/erd/templates/erd.dot
+-rw-r--r--   0        0        0      693 2023-08-02 13:28:58.826419 fmsfdata2-1.0.0/fmsfdata2/schema/parser/__init__.py
+-rw-r--r--   0        0        0     1304 2023-08-02 12:56:48.724555 fmsfdata2-1.0.0/fmsfdata2/settings.py
+-rw-r--r--   0        0        0     1555 2023-08-02 13:17:51.725733 fmsfdata2-1.0.0/fmsfdata2/standardiser.py
+-rw-r--r--   0        0        0       22 2023-07-26 13:36:28.982395 fmsfdata2-1.0.0/fmsfdata2/stream_parser/__init__.py
+-rw-r--r--   0        0        0     1636 2023-08-02 13:17:51.725245 fmsfdata2-1.0.0/fmsfdata2/stream_parser/checks.py
+-rw-r--r--   0        0        0     7178 2023-08-02 13:17:51.725316 fmsfdata2-1.0.0/fmsfdata2/stream_parser/collectors.py
+-rw-r--r--   0        0        0     1790 2023-08-02 13:09:34.836657 fmsfdata2-1.0.0/fmsfdata2/stream_parser/events.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:36:28.983244 fmsfdata2-1.0.0/fmsfdata2/stream_parser/filters/__init__.py
+-rw-r--r--   0        0        0     2178 2023-08-02 13:17:51.725183 fmsfdata2-1.0.0/fmsfdata2/stream_parser/filters/column_headers.py
+-rw-r--r--   0        0        0     1798 2023-08-02 13:17:51.726235 fmsfdata2-1.0.0/fmsfdata2/stream_parser/filters/context.py
+-rw-r--r--   0        0        0     6114 2023-08-02 13:17:51.725141 fmsfdata2-1.0.0/fmsfdata2/stream_parser/filters/generic.py
+-rw-r--r--   0        0        0     2433 2023-08-02 13:17:51.686261 fmsfdata2-1.0.0/fmsfdata2/stream_parser/filters/types.py
+-rw-r--r--   0        0        0     2056 2023-08-02 13:17:51.725293 fmsfdata2-1.0.0/fmsfdata2/stream_parser/function_helpers.py
+-rw-r--r--   0        0        0      429 2023-08-02 13:17:51.725262 fmsfdata2-1.0.0/fmsfdata2/stream_parser/functions.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:36:28.984861 fmsfdata2-1.0.0/fmsfdata2/stream_parser/parser/__init__.py
+-rw-r--r--   0        0        0      528 2023-08-02 13:17:51.665185 fmsfdata2-1.0.0/fmsfdata2/stream_parser/parser/csv.py
+-rw-r--r--   0        0        0     1876 2023-08-02 13:17:51.664927 fmsfdata2-1.0.0/fmsfdata2/stream_parser/parser/openpyxl.py
+-rw-r--r--   0        0        0     1138 2023-08-02 13:17:51.664759 fmsfdata2-1.0.0/fmsfdata2/stream_parser/parser/xml.py
+-rw-r--r--   0        0        0      485 2023-08-02 13:17:51.725212 fmsfdata2-1.0.0/fmsfdata2/stream_parser/stream.py
+-rw-r--r--   0        0        0      296 2023-08-02 13:17:51.726120 fmsfdata2-1.0.0/fmsfdata2/stream_parser/types.py
+-rw-r--r--   0        0        0      598 2023-08-02 13:29:13.568321 fmsfdata2-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2911 1970-01-01 00:00:00.000000 fmsfdata2-1.0.0/PKG-INFO
```

### Comparing `fmsfdata2-0.1.0/README.md` & `fmsfdata2-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `fmsfdata2-0.1.0/fmsfdata2/converter.py` & `fmsfdata2-1.0.0/fmsfdata2/converter.py`

 * *Files identical despite different names*

### Comparing `fmsfdata2-0.1.0/fmsfdata2/datastore/_store.py` & `fmsfdata2-1.0.0/fmsfdata2/datastore/_store.py`

 * *Files identical despite different names*

### Comparing `fmsfdata2-0.1.0/fmsfdata2/datastore/_table.py` & `fmsfdata2-1.0.0/fmsfdata2/datastore/_table.py`

 * *Files identical despite different names*

### Comparing `fmsfdata2-0.1.0/fmsfdata2/datastore/_table_row.py` & `fmsfdata2-1.0.0/fmsfdata2/datastore/_table_row.py`

 * *Files identical despite different names*

### Comparing `fmsfdata2-0.1.0/fmsfdata2/exporter.py` & `fmsfdata2-1.0.0/fmsfdata2/exporter.py`

 * *Files identical despite different names*

### Comparing `fmsfdata2-0.1.0/fmsfdata2/identifier.py` & `fmsfdata2-1.0.0/fmsfdata2/identifier.py`

 * *Files identical despite different names*

### Comparing `fmsfdata2-0.1.0/fmsfdata2/normaliser.py` & `fmsfdata2-1.0.0/fmsfdata2/normaliser.py`

 * *Files identical despite different names*

### Comparing `fmsfdata2-0.1.0/fmsfdata2/schema/_data.py` & `fmsfdata2-1.0.0/fmsfdata2/schema/_data.py`

 * *Files identical despite different names*

### Comparing `fmsfdata2-0.1.0/fmsfdata2/schema/_proxy.py` & `fmsfdata2-1.0.0/fmsfdata2/schema/_proxy.py`

 * *Files identical despite different names*

### Comparing `fmsfdata2-0.1.0/fmsfdata2/schema/erd/__init__.py` & `fmsfdata2-1.0.0/fmsfdata2/schema/erd/__init__.py`

 * *Files identical despite different names*

### Comparing `fmsfdata2-0.1.0/fmsfdata2/schema/erd/templates/erd.dot` & `fmsfdata2-1.0.0/fmsfdata2/schema/erd/templates/erd.dot`

 * *Files identical despite different names*

### Comparing `fmsfdata2-0.1.0/fmsfdata2/schema/parser/__init__.py` & `fmsfdata2-1.0.0/fmsfdata2/schema/parser/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 from typing import Any, Dict
 
-import jstyleson
+import json
 import yaml
 
 from fmsfdata2.schema import Field, Record, Schema
 
 
 def parse_schema(schema) -> Schema:
     if isinstance(schema, dict):
@@ -20,11 +20,11 @@
     path = Path(path)
     with path.open("rt") as f:
         return _parse_string(f.read())
 
 
 def _parse_string(content) -> Schema:
     if content.startswith("{"):
-        content = jstyleson.loads(content)
+        content = json.loads(content)
     else:
         content = yaml.safe_load(content)
     return Schema.from_value(content)
```

### Comparing `fmsfdata2-0.1.0/fmsfdata2/settings.py` & `fmsfdata2-1.0.0/fmsfdata2/settings.py`

 * *Files identical despite different names*

### Comparing `fmsfdata2-0.1.0/fmsfdata2/standardiser.py` & `fmsfdata2-1.0.0/fmsfdata2/standardiser.py`

 * *Files identical despite different names*

### Comparing `fmsfdata2-0.1.0/fmsfdata2/stream_parser/checks.py` & `fmsfdata2-1.0.0/fmsfdata2/stream_parser/checks.py`

 * *Files identical despite different names*

### Comparing `fmsfdata2-0.1.0/fmsfdata2/stream_parser/collectors.py` & `fmsfdata2-1.0.0/fmsfdata2/stream_parser/collectors.py`

 * *Files identical despite different names*

### Comparing `fmsfdata2-0.1.0/fmsfdata2/stream_parser/events.py` & `fmsfdata2-1.0.0/fmsfdata2/stream_parser/events.py`

 * *Files identical despite different names*

### Comparing `fmsfdata2-0.1.0/fmsfdata2/stream_parser/filters/column_headers.py` & `fmsfdata2-1.0.0/fmsfdata2/stream_parser/filters/column_headers.py`

 * *Files identical despite different names*

### Comparing `fmsfdata2-0.1.0/fmsfdata2/stream_parser/filters/context.py` & `fmsfdata2-1.0.0/fmsfdata2/stream_parser/filters/context.py`

 * *Files identical despite different names*

### Comparing `fmsfdata2-0.1.0/fmsfdata2/stream_parser/filters/generic.py` & `fmsfdata2-1.0.0/fmsfdata2/stream_parser/filters/generic.py`

 * *Files identical despite different names*

### Comparing `fmsfdata2-0.1.0/fmsfdata2/stream_parser/filters/types.py` & `fmsfdata2-1.0.0/fmsfdata2/stream_parser/filters/types.py`

 * *Files identical despite different names*

### Comparing `fmsfdata2-0.1.0/fmsfdata2/stream_parser/function_helpers.py` & `fmsfdata2-1.0.0/fmsfdata2/stream_parser/function_helpers.py`

 * *Files identical despite different names*

### Comparing `fmsfdata2-0.1.0/fmsfdata2/stream_parser/parser/csv.py` & `fmsfdata2-1.0.0/fmsfdata2/stream_parser/parser/csv.py`

 * *Files identical despite different names*

### Comparing `fmsfdata2-0.1.0/fmsfdata2/stream_parser/parser/openpyxl.py` & `fmsfdata2-1.0.0/fmsfdata2/stream_parser/parser/openpyxl.py`

 * *Files identical despite different names*

### Comparing `fmsfdata2-0.1.0/fmsfdata2/stream_parser/parser/xml.py` & `fmsfdata2-1.0.0/fmsfdata2/stream_parser/parser/xml.py`

 * *Files identical despite different names*

### Comparing `fmsfdata2-0.1.0/pyproject.toml` & `fmsfdata2-1.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 [tool.poetry]
 name = "fmsfdata2"
-version = "0.1.0"
+version = "1.0.0"
 description = ""
 authors = ["franciscobmacedo <franciscovcbm@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 xsdata = "^23.7"
-jstyleson = "^0.0.2"
 pyyaml = "^6.0.1"
 tablib = "^3.5.0"
 lxml = "^4.9.3"
 pandas = {version="^2.0.3", optional = true}
 more-itertools = "^10.0.0"
 openpyxl = "^3.1.2"
 pyhumps = "^3.8.0"
```

### Comparing `fmsfdata2-0.1.0/PKG-INFO` & `fmsfdata2-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: fmsfdata2
-Version: 0.1.0
+Version: 1.0.0
 Summary: 
 Author: franciscobmacedo
 Author-email: franciscovcbm@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: pandas
-Requires-Dist: jstyleson (>=0.0.2,<0.0.3)
 Requires-Dist: lxml (>=4.9.3,<5.0.0)
 Requires-Dist: more-itertools (>=10.0.0,<11.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0) ; extra == "pandas"
 Requires-Dist: pyhumps (>=3.8.0,<4.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: tablib (>=3.5.0,<4.0.0)
```


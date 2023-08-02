# Comparing `tmp/fmsfdata-3.0.0.tar.gz` & `tmp/fmsfdata-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmsfdata-3.0.0.tar", max compression
+gzip compressed data, was "fmsfdata-3.1.0.tar", max compression
```

## Comparing `fmsfdata-3.0.0.tar` & `fmsfdata-3.1.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     2200 2023-07-26 16:25:20.011374 fmsfdata-3.0.0/README.md
--rw-r--r--   0        0        0       61 2023-08-02 13:31:32.158029 fmsfdata-3.0.0/fmsfdata/__init__.py
--rw-r--r--   0        0        0     1276 2023-08-02 13:50:57.882830 fmsfdata-3.0.0/fmsfdata/converter.py
--rw-r--r--   0        0        0      216 2023-08-02 13:31:32.159333 fmsfdata-3.0.0/fmsfdata/datastore/__init__.py
--rw-r--r--   0        0        0     1726 2023-08-02 13:31:32.159904 fmsfdata-3.0.0/fmsfdata/datastore/_store.py
--rw-r--r--   0        0        0     1775 2023-08-02 13:31:32.160451 fmsfdata-3.0.0/fmsfdata/datastore/_table.py
--rw-r--r--   0        0        0      480 2023-08-02 13:31:32.160856 fmsfdata-3.0.0/fmsfdata/datastore/_table_key.py
--rw-r--r--   0        0        0     2116 2023-08-02 13:31:32.161238 fmsfdata-3.0.0/fmsfdata/datastore/_table_row.py
--rw-r--r--   0        0        0     2801 2023-08-02 13:50:57.882949 fmsfdata-3.0.0/fmsfdata/exporter.py
--rw-r--r--   0        0        0     2059 2023-08-02 13:50:57.883578 fmsfdata-3.0.0/fmsfdata/identifier.py
--rw-r--r--   0        0        0     2906 2023-08-02 13:50:57.863833 fmsfdata-3.0.0/fmsfdata/normaliser.py
--rw-r--r--   0        0        0       51 2023-08-02 13:31:32.163445 fmsfdata-3.0.0/fmsfdata/schema/__init__.py
--rw-r--r--   0        0        0    13068 2023-08-02 13:38:38.200740 fmsfdata-3.0.0/fmsfdata/schema/_data.py
--rw-r--r--   0        0        0     9679 2023-08-02 13:31:32.164719 fmsfdata-3.0.0/fmsfdata/schema/_proxy.py
--rw-r--r--   0        0        0      164 2023-08-02 13:31:32.165362 fmsfdata-3.0.0/fmsfdata/schema/_types.py
--rw-r--r--   0        0        0     1223 2023-08-02 13:50:57.863763 fmsfdata-3.0.0/fmsfdata/schema/erd/__init__.py
--rw-r--r--   0        0        0      957 2023-08-02 13:31:32.166261 fmsfdata-3.0.0/fmsfdata/schema/erd/templates/erd.dot
--rw-r--r--   0        0        0      692 2023-08-02 13:50:57.762214 fmsfdata-3.0.0/fmsfdata/schema/parser/__init__.py
--rw-r--r--   0        0        0     1304 2023-08-02 13:38:38.201518 fmsfdata-3.0.0/fmsfdata/settings.py
--rw-r--r--   0        0        0     1546 2023-08-02 13:50:57.863795 fmsfdata-3.0.0/fmsfdata/standardiser.py
--rw-r--r--   0        0        0       22 2023-08-02 13:31:32.168580 fmsfdata-3.0.0/fmsfdata/stream_parser/__init__.py
--rw-r--r--   0        0        0     1635 2023-08-02 13:50:57.863701 fmsfdata-3.0.0/fmsfdata/stream_parser/checks.py
--rw-r--r--   0        0        0     7172 2023-08-02 13:50:57.923863 fmsfdata-3.0.0/fmsfdata/stream_parser/collectors.py
--rw-r--r--   0        0        0     1790 2023-08-02 13:38:38.203045 fmsfdata-3.0.0/fmsfdata/stream_parser/events.py
--rw-r--r--   0        0        0        0 2023-08-02 13:31:32.170271 fmsfdata-3.0.0/fmsfdata/stream_parser/filters/__init__.py
--rw-r--r--   0        0        0     2173 2023-08-02 13:50:57.762806 fmsfdata-3.0.0/fmsfdata/stream_parser/filters/column_headers.py
--rw-r--r--   0        0        0     1802 2023-08-02 13:50:57.805318 fmsfdata-3.0.0/fmsfdata/stream_parser/filters/context.py
--rw-r--r--   0        0        0     6108 2023-08-02 13:50:57.805406 fmsfdata-3.0.0/fmsfdata/stream_parser/filters/generic.py
--rw-r--r--   0        0        0     2431 2023-08-02 13:50:57.762268 fmsfdata-3.0.0/fmsfdata/stream_parser/filters/types.py
--rw-r--r--   0        0        0     2053 2023-08-02 13:50:57.863643 fmsfdata-3.0.0/fmsfdata/stream_parser/function_helpers.py
--rw-r--r--   0        0        0      427 2023-08-02 13:50:57.863582 fmsfdata-3.0.0/fmsfdata/stream_parser/functions.py
--rw-r--r--   0        0        0        0 2023-08-02 13:31:32.175124 fmsfdata-3.0.0/fmsfdata/stream_parser/parser/__init__.py
--rw-r--r--   0        0        0      527 2023-08-02 13:50:57.762344 fmsfdata-3.0.0/fmsfdata/stream_parser/parser/csv.py
--rw-r--r--   0        0        0     1875 2023-08-02 13:50:57.762246 fmsfdata-3.0.0/fmsfdata/stream_parser/parser/openpyxl.py
--rw-r--r--   0        0        0     1137 2023-08-02 13:50:57.762309 fmsfdata-3.0.0/fmsfdata/stream_parser/parser/xml.py
--rw-r--r--   0        0        0      484 2023-08-02 13:50:57.805578 fmsfdata-3.0.0/fmsfdata/stream_parser/stream.py
--rw-r--r--   0        0        0      295 2023-08-02 13:50:57.805458 fmsfdata-3.0.0/fmsfdata/stream_parser/types.py
--rw-r--r--   0        0        0      600 2023-08-02 13:52:12.278175 fmsfdata-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     2910 1970-01-01 00:00:00.000000 fmsfdata-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2200 2023-07-26 16:25:20.011374 fmsfdata-3.1.0/README.md
+-rw-r--r--   0        0        0       61 2023-08-02 13:31:32.158029 fmsfdata-3.1.0/fmsfdata/__init__.py
+-rw-r--r--   0        0        0     1276 2023-08-02 13:50:57.882830 fmsfdata-3.1.0/fmsfdata/converter.py
+-rw-r--r--   0        0        0      216 2023-08-02 13:31:32.159333 fmsfdata-3.1.0/fmsfdata/datastore/__init__.py
+-rw-r--r--   0        0        0     1726 2023-08-02 13:31:32.159904 fmsfdata-3.1.0/fmsfdata/datastore/_store.py
+-rw-r--r--   0        0        0     1775 2023-08-02 13:31:32.160451 fmsfdata-3.1.0/fmsfdata/datastore/_table.py
+-rw-r--r--   0        0        0      480 2023-08-02 13:31:32.160856 fmsfdata-3.1.0/fmsfdata/datastore/_table_key.py
+-rw-r--r--   0        0        0     2116 2023-08-02 13:31:32.161238 fmsfdata-3.1.0/fmsfdata/datastore/_table_row.py
+-rw-r--r--   0        0        0     2801 2023-08-02 13:50:57.882949 fmsfdata-3.1.0/fmsfdata/exporter.py
+-rw-r--r--   0        0        0     2059 2023-08-02 13:50:57.883578 fmsfdata-3.1.0/fmsfdata/identifier.py
+-rw-r--r--   0        0        0     2906 2023-08-02 13:50:57.863833 fmsfdata-3.1.0/fmsfdata/normaliser.py
+-rw-r--r--   0        0        0       51 2023-08-02 13:31:32.163445 fmsfdata-3.1.0/fmsfdata/schema/__init__.py
+-rw-r--r--   0        0        0    13068 2023-08-02 13:38:38.200740 fmsfdata-3.1.0/fmsfdata/schema/_data.py
+-rw-r--r--   0        0        0     9679 2023-08-02 13:31:32.164719 fmsfdata-3.1.0/fmsfdata/schema/_proxy.py
+-rw-r--r--   0        0        0      164 2023-08-02 13:31:32.165362 fmsfdata-3.1.0/fmsfdata/schema/_types.py
+-rw-r--r--   0        0        0     1223 2023-08-02 13:50:57.863763 fmsfdata-3.1.0/fmsfdata/schema/erd/__init__.py
+-rw-r--r--   0        0        0      957 2023-08-02 13:31:32.166261 fmsfdata-3.1.0/fmsfdata/schema/erd/templates/erd.dot
+-rw-r--r--   0        0        0      692 2023-08-02 13:50:57.762214 fmsfdata-3.1.0/fmsfdata/schema/parser/__init__.py
+-rw-r--r--   0        0        0     1304 2023-08-02 13:38:38.201518 fmsfdata-3.1.0/fmsfdata/settings.py
+-rw-r--r--   0        0        0     1546 2023-08-02 13:50:57.863795 fmsfdata-3.1.0/fmsfdata/standardiser.py
+-rw-r--r--   0        0        0       22 2023-08-02 13:31:32.168580 fmsfdata-3.1.0/fmsfdata/stream_parser/__init__.py
+-rw-r--r--   0        0        0     1635 2023-08-02 13:50:57.863701 fmsfdata-3.1.0/fmsfdata/stream_parser/checks.py
+-rw-r--r--   0        0        0     7172 2023-08-02 13:50:57.923863 fmsfdata-3.1.0/fmsfdata/stream_parser/collectors.py
+-rw-r--r--   0        0        0     1790 2023-08-02 13:38:38.203045 fmsfdata-3.1.0/fmsfdata/stream_parser/events.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:31:32.170271 fmsfdata-3.1.0/fmsfdata/stream_parser/filters/__init__.py
+-rw-r--r--   0        0        0     2173 2023-08-02 13:50:57.762806 fmsfdata-3.1.0/fmsfdata/stream_parser/filters/column_headers.py
+-rw-r--r--   0        0        0     1802 2023-08-02 13:50:57.805318 fmsfdata-3.1.0/fmsfdata/stream_parser/filters/context.py
+-rw-r--r--   0        0        0     6108 2023-08-02 13:50:57.805406 fmsfdata-3.1.0/fmsfdata/stream_parser/filters/generic.py
+-rw-r--r--   0        0        0     2431 2023-08-02 13:50:57.762268 fmsfdata-3.1.0/fmsfdata/stream_parser/filters/types.py
+-rw-r--r--   0        0        0     2053 2023-08-02 13:50:57.863643 fmsfdata-3.1.0/fmsfdata/stream_parser/function_helpers.py
+-rw-r--r--   0        0        0      427 2023-08-02 13:50:57.863582 fmsfdata-3.1.0/fmsfdata/stream_parser/functions.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:31:32.175124 fmsfdata-3.1.0/fmsfdata/stream_parser/parser/__init__.py
+-rw-r--r--   0        0        0      527 2023-08-02 13:50:57.762344 fmsfdata-3.1.0/fmsfdata/stream_parser/parser/csv.py
+-rw-r--r--   0        0        0     1875 2023-08-02 13:50:57.762246 fmsfdata-3.1.0/fmsfdata/stream_parser/parser/openpyxl.py
+-rw-r--r--   0        0        0     1137 2023-08-02 13:50:57.762309 fmsfdata-3.1.0/fmsfdata/stream_parser/parser/xml.py
+-rw-r--r--   0        0        0      484 2023-08-02 13:50:57.805578 fmsfdata-3.1.0/fmsfdata/stream_parser/stream.py
+-rw-r--r--   0        0        0      295 2023-08-02 13:50:57.805458 fmsfdata-3.1.0/fmsfdata/stream_parser/types.py
+-rw-r--r--   0        0        0      600 2023-08-02 14:05:21.663059 fmsfdata-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2910 1970-01-01 00:00:00.000000 fmsfdata-3.1.0/PKG-INFO
```

### Comparing `fmsfdata-3.0.0/README.md` & `fmsfdata-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `fmsfdata-3.0.0/fmsfdata/converter.py` & `fmsfdata-3.1.0/fmsfdata/converter.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-3.0.0/fmsfdata/datastore/_store.py` & `fmsfdata-3.1.0/fmsfdata/datastore/_store.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-3.0.0/fmsfdata/datastore/_table.py` & `fmsfdata-3.1.0/fmsfdata/datastore/_table.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-3.0.0/fmsfdata/datastore/_table_row.py` & `fmsfdata-3.1.0/fmsfdata/datastore/_table_row.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-3.0.0/fmsfdata/exporter.py` & `fmsfdata-3.1.0/fmsfdata/exporter.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-3.0.0/fmsfdata/identifier.py` & `fmsfdata-3.1.0/fmsfdata/identifier.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-3.0.0/fmsfdata/normaliser.py` & `fmsfdata-3.1.0/fmsfdata/normaliser.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-3.0.0/fmsfdata/schema/_data.py` & `fmsfdata-3.1.0/fmsfdata/schema/_data.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-3.0.0/fmsfdata/schema/_proxy.py` & `fmsfdata-3.1.0/fmsfdata/schema/_proxy.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-3.0.0/fmsfdata/schema/erd/__init__.py` & `fmsfdata-3.1.0/fmsfdata/schema/erd/__init__.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-3.0.0/fmsfdata/schema/erd/templates/erd.dot` & `fmsfdata-3.1.0/fmsfdata/schema/erd/templates/erd.dot`

 * *Files identical despite different names*

### Comparing `fmsfdata-3.0.0/fmsfdata/schema/parser/__init__.py` & `fmsfdata-3.1.0/fmsfdata/schema/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-3.0.0/fmsfdata/settings.py` & `fmsfdata-3.1.0/fmsfdata/settings.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-3.0.0/fmsfdata/standardiser.py` & `fmsfdata-3.1.0/fmsfdata/standardiser.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-3.0.0/fmsfdata/stream_parser/checks.py` & `fmsfdata-3.1.0/fmsfdata/stream_parser/checks.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-3.0.0/fmsfdata/stream_parser/collectors.py` & `fmsfdata-3.1.0/fmsfdata/stream_parser/collectors.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-3.0.0/fmsfdata/stream_parser/events.py` & `fmsfdata-3.1.0/fmsfdata/stream_parser/events.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-3.0.0/fmsfdata/stream_parser/filters/column_headers.py` & `fmsfdata-3.1.0/fmsfdata/stream_parser/filters/column_headers.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-3.0.0/fmsfdata/stream_parser/filters/context.py` & `fmsfdata-3.1.0/fmsfdata/stream_parser/filters/context.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-3.0.0/fmsfdata/stream_parser/filters/generic.py` & `fmsfdata-3.1.0/fmsfdata/stream_parser/filters/generic.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-3.0.0/fmsfdata/stream_parser/filters/types.py` & `fmsfdata-3.1.0/fmsfdata/stream_parser/filters/types.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-3.0.0/fmsfdata/stream_parser/function_helpers.py` & `fmsfdata-3.1.0/fmsfdata/stream_parser/function_helpers.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-3.0.0/fmsfdata/stream_parser/parser/csv.py` & `fmsfdata-3.1.0/fmsfdata/stream_parser/parser/csv.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-3.0.0/fmsfdata/stream_parser/parser/openpyxl.py` & `fmsfdata-3.1.0/fmsfdata/stream_parser/parser/openpyxl.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-3.0.0/fmsfdata/stream_parser/parser/xml.py` & `fmsfdata-3.1.0/fmsfdata/stream_parser/parser/xml.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-3.0.0/pyproject.toml` & `fmsfdata-3.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "fmsfdata"
-version = "3.0.0"
+version = "3.1.0"
 description = ""
 authors = ["franciscobmacedo <franciscovcbm@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 xsdata = "^23.7"
 pyyaml = "^6.0.1"
 tablib = "^3.5.0"
-lxml = "^4.9.3"
+lxml = "^4.0.0"
 pandas = { version = "^2.0.3", optional = true }
 more-itertools = "^10.0.0"
 openpyxl = "^3.1.2"
 pyhumps = "^3.8.0"
 
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `fmsfdata-3.0.0/PKG-INFO` & `fmsfdata-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: fmsfdata
-Version: 3.0.0
+Version: 3.1.0
 Summary: 
 Author: franciscobmacedo
 Author-email: franciscovcbm@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: pandas
-Requires-Dist: lxml (>=4.9.3,<5.0.0)
+Requires-Dist: lxml (>=4.0.0,<5.0.0)
 Requires-Dist: more-itertools (>=10.0.0,<11.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0) ; extra == "pandas"
 Requires-Dist: pyhumps (>=3.8.0,<4.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: tablib (>=3.5.0,<4.0.0)
 Requires-Dist: xsdata (>=23.7,<24.0)
```


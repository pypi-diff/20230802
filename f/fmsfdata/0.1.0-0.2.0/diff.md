# Comparing `tmp/fmsfdata-0.1.0.tar.gz` & `tmp/fmsfdata-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmsfdata-0.1.0.tar", max compression
+gzip compressed data, was "fmsfdata-0.2.0.tar", max compression
```

## Comparing `fmsfdata-0.1.0.tar` & `fmsfdata-0.2.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     2200 2023-07-26 16:25:20.011374 fmsfdata-0.1.0/README.md
--rw-r--r--   0        0        0       61 2023-08-02 09:04:23.701820 fmsfdata-0.1.0/fmsfdata/__init__.py
--rw-r--r--   0        0        0     1276 2023-08-02 13:09:27.158267 fmsfdata-0.1.0/fmsfdata/converter.py
--rw-r--r--   0        0        0      216 2023-07-31 11:10:27.203006 fmsfdata-0.1.0/fmsfdata/datastore/__init__.py
--rw-r--r--   0        0        0     1726 2023-07-31 12:01:41.140145 fmsfdata-0.1.0/fmsfdata/datastore/_store.py
--rw-r--r--   0        0        0     1775 2023-07-31 11:10:27.204118 fmsfdata-0.1.0/fmsfdata/datastore/_table.py
--rw-r--r--   0        0        0      480 2023-07-31 11:10:27.204508 fmsfdata-0.1.0/fmsfdata/datastore/_table_key.py
--rw-r--r--   0        0        0     2116 2023-07-31 11:10:27.204876 fmsfdata-0.1.0/fmsfdata/datastore/_table_row.py
--rw-r--r--   0        0        0     2801 2023-08-02 13:09:26.462035 fmsfdata-0.1.0/fmsfdata/exporter.py
--rw-r--r--   0        0        0     2059 2023-08-02 13:09:25.473165 fmsfdata-0.1.0/fmsfdata/identifier.py
--rw-r--r--   0        0        0     2906 2023-08-02 13:09:23.961598 fmsfdata-0.1.0/fmsfdata/normaliser.py
--rw-r--r--   0        0        0       51 2023-07-31 11:10:27.206997 fmsfdata-0.1.0/fmsfdata/schema/__init__.py
--rw-r--r--   0        0        0    13068 2023-08-02 12:56:48.724000 fmsfdata-0.1.0/fmsfdata/schema/_data.py
--rw-r--r--   0        0        0     9679 2023-07-31 11:10:27.208128 fmsfdata-0.1.0/fmsfdata/schema/_proxy.py
--rw-r--r--   0        0        0      164 2023-07-31 11:10:27.208691 fmsfdata-0.1.0/fmsfdata/schema/_types.py
--rw-r--r--   0        0        0     1223 2023-08-02 13:09:15.033061 fmsfdata-0.1.0/fmsfdata/schema/erd/__init__.py
--rw-r--r--   0        0        0      957 2023-07-31 11:10:27.209771 fmsfdata-0.1.0/fmsfdata/schema/erd/templates/erd.dot
--rw-r--r--   0        0        0      702 2023-08-02 13:09:14.390173 fmsfdata-0.1.0/fmsfdata/schema/parser/__init__.py
--rw-r--r--   0        0        0     1304 2023-08-02 12:56:48.724555 fmsfdata-0.1.0/fmsfdata/settings.py
--rw-r--r--   0        0        0     1546 2023-08-02 13:09:29.256586 fmsfdata-0.1.0/fmsfdata/standardiser.py
--rw-r--r--   0        0        0       22 2023-07-26 13:36:28.982395 fmsfdata-0.1.0/fmsfdata/stream_parser/__init__.py
--rw-r--r--   0        0        0     1635 2023-08-02 13:09:13.893661 fmsfdata-0.1.0/fmsfdata/stream_parser/checks.py
--rw-r--r--   0        0        0     7172 2023-08-02 13:09:13.199264 fmsfdata-0.1.0/fmsfdata/stream_parser/collectors.py
--rw-r--r--   0        0        0     1790 2023-08-02 13:09:34.836657 fmsfdata-0.1.0/fmsfdata/stream_parser/events.py
--rw-r--r--   0        0        0        0 2023-07-26 13:36:28.983244 fmsfdata-0.1.0/fmsfdata/stream_parser/filters/__init__.py
--rw-r--r--   0        0        0     2173 2023-08-02 13:09:33.837804 fmsfdata-0.1.0/fmsfdata/stream_parser/filters/column_headers.py
--rw-r--r--   0        0        0     1796 2023-08-02 13:09:09.235365 fmsfdata-0.1.0/fmsfdata/stream_parser/filters/context.py
--rw-r--r--   0        0        0     6108 2023-08-02 13:09:32.875175 fmsfdata-0.1.0/fmsfdata/stream_parser/filters/generic.py
--rw-r--r--   0        0        0     2431 2023-08-02 13:09:31.080819 fmsfdata-0.1.0/fmsfdata/stream_parser/filters/types.py
--rw-r--r--   0        0        0     2053 2023-08-02 13:09:12.315854 fmsfdata-0.1.0/fmsfdata/stream_parser/function_helpers.py
--rw-r--r--   0        0        0      427 2023-08-02 13:09:11.533201 fmsfdata-0.1.0/fmsfdata/stream_parser/functions.py
--rw-r--r--   0        0        0        0 2023-07-26 13:36:28.984861 fmsfdata-0.1.0/fmsfdata/stream_parser/parser/__init__.py
--rw-r--r--   0        0        0      527 2023-08-02 13:09:29.964717 fmsfdata-0.1.0/fmsfdata/stream_parser/parser/csv.py
--rw-r--r--   0        0        0     1875 2023-08-02 13:09:08.368312 fmsfdata-0.1.0/fmsfdata/stream_parser/parser/openpyxl.py
--rw-r--r--   0        0        0     1137 2023-08-02 13:09:27.996847 fmsfdata-0.1.0/fmsfdata/stream_parser/parser/xml.py
--rw-r--r--   0        0        0      484 2023-08-02 13:09:10.799160 fmsfdata-0.1.0/fmsfdata/stream_parser/stream.py
--rw-r--r--   0        0        0      295 2023-08-02 13:09:10.078028 fmsfdata-0.1.0/fmsfdata/stream_parser/types.py
--rw-r--r--   0        0        0      638 2023-08-02 13:08:57.784288 fmsfdata-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2993 1970-01-01 00:00:00.000000 fmsfdata-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2200 2023-07-26 16:25:20.011374 fmsfdata-0.2.0/README.md
+-rw-r--r--   0        0        0       61 2023-08-02 09:04:23.701820 fmsfdata-0.2.0/fmsfdata/__init__.py
+-rw-r--r--   0        0        0     1276 2023-08-02 13:09:27.158267 fmsfdata-0.2.0/fmsfdata/converter.py
+-rw-r--r--   0        0        0      216 2023-07-31 11:10:27.203006 fmsfdata-0.2.0/fmsfdata/datastore/__init__.py
+-rw-r--r--   0        0        0     1726 2023-07-31 12:01:41.140145 fmsfdata-0.2.0/fmsfdata/datastore/_store.py
+-rw-r--r--   0        0        0     1775 2023-07-31 11:10:27.204118 fmsfdata-0.2.0/fmsfdata/datastore/_table.py
+-rw-r--r--   0        0        0      480 2023-07-31 11:10:27.204508 fmsfdata-0.2.0/fmsfdata/datastore/_table_key.py
+-rw-r--r--   0        0        0     2116 2023-07-31 11:10:27.204876 fmsfdata-0.2.0/fmsfdata/datastore/_table_row.py
+-rw-r--r--   0        0        0     2801 2023-08-02 13:09:26.462035 fmsfdata-0.2.0/fmsfdata/exporter.py
+-rw-r--r--   0        0        0     2059 2023-08-02 13:09:25.473165 fmsfdata-0.2.0/fmsfdata/identifier.py
+-rw-r--r--   0        0        0     2906 2023-08-02 13:09:23.961598 fmsfdata-0.2.0/fmsfdata/normaliser.py
+-rw-r--r--   0        0        0       51 2023-07-31 11:10:27.206997 fmsfdata-0.2.0/fmsfdata/schema/__init__.py
+-rw-r--r--   0        0        0    13068 2023-08-02 12:56:48.724000 fmsfdata-0.2.0/fmsfdata/schema/_data.py
+-rw-r--r--   0        0        0     9679 2023-07-31 11:10:27.208128 fmsfdata-0.2.0/fmsfdata/schema/_proxy.py
+-rw-r--r--   0        0        0      164 2023-07-31 11:10:27.208691 fmsfdata-0.2.0/fmsfdata/schema/_types.py
+-rw-r--r--   0        0        0     1223 2023-08-02 13:09:15.033061 fmsfdata-0.2.0/fmsfdata/schema/erd/__init__.py
+-rw-r--r--   0        0        0      957 2023-07-31 11:10:27.209771 fmsfdata-0.2.0/fmsfdata/schema/erd/templates/erd.dot
+-rw-r--r--   0        0        0      702 2023-08-02 13:09:14.390173 fmsfdata-0.2.0/fmsfdata/schema/parser/__init__.py
+-rw-r--r--   0        0        0     1304 2023-08-02 12:56:48.724555 fmsfdata-0.2.0/fmsfdata/settings.py
+-rw-r--r--   0        0        0     1546 2023-08-02 13:09:29.256586 fmsfdata-0.2.0/fmsfdata/standardiser.py
+-rw-r--r--   0        0        0       22 2023-07-26 13:36:28.982395 fmsfdata-0.2.0/fmsfdata/stream_parser/__init__.py
+-rw-r--r--   0        0        0     1635 2023-08-02 13:09:13.893661 fmsfdata-0.2.0/fmsfdata/stream_parser/checks.py
+-rw-r--r--   0        0        0     7172 2023-08-02 13:09:13.199264 fmsfdata-0.2.0/fmsfdata/stream_parser/collectors.py
+-rw-r--r--   0        0        0     1790 2023-08-02 13:09:34.836657 fmsfdata-0.2.0/fmsfdata/stream_parser/events.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:36:28.983244 fmsfdata-0.2.0/fmsfdata/stream_parser/filters/__init__.py
+-rw-r--r--   0        0        0     2173 2023-08-02 13:09:33.837804 fmsfdata-0.2.0/fmsfdata/stream_parser/filters/column_headers.py
+-rw-r--r--   0        0        0     1796 2023-08-02 13:09:09.235365 fmsfdata-0.2.0/fmsfdata/stream_parser/filters/context.py
+-rw-r--r--   0        0        0     6108 2023-08-02 13:09:32.875175 fmsfdata-0.2.0/fmsfdata/stream_parser/filters/generic.py
+-rw-r--r--   0        0        0     2431 2023-08-02 13:09:31.080819 fmsfdata-0.2.0/fmsfdata/stream_parser/filters/types.py
+-rw-r--r--   0        0        0     2053 2023-08-02 13:09:12.315854 fmsfdata-0.2.0/fmsfdata/stream_parser/function_helpers.py
+-rw-r--r--   0        0        0      427 2023-08-02 13:09:11.533201 fmsfdata-0.2.0/fmsfdata/stream_parser/functions.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:36:28.984861 fmsfdata-0.2.0/fmsfdata/stream_parser/parser/__init__.py
+-rw-r--r--   0        0        0      527 2023-08-02 13:09:29.964717 fmsfdata-0.2.0/fmsfdata/stream_parser/parser/csv.py
+-rw-r--r--   0        0        0     1875 2023-08-02 13:09:08.368312 fmsfdata-0.2.0/fmsfdata/stream_parser/parser/openpyxl.py
+-rw-r--r--   0        0        0     1137 2023-08-02 13:09:27.996847 fmsfdata-0.2.0/fmsfdata/stream_parser/parser/xml.py
+-rw-r--r--   0        0        0      484 2023-08-02 13:09:10.799160 fmsfdata-0.2.0/fmsfdata/stream_parser/stream.py
+-rw-r--r--   0        0        0      295 2023-08-02 13:09:10.078028 fmsfdata-0.2.0/fmsfdata/stream_parser/types.py
+-rw-r--r--   0        0        0      618 2023-08-02 13:12:43.926468 fmsfdata-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2952 1970-01-01 00:00:00.000000 fmsfdata-0.2.0/PKG-INFO
```

### Comparing `fmsfdata-0.1.0/README.md` & `fmsfdata-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `fmsfdata-0.1.0/fmsfdata/converter.py` & `fmsfdata-0.2.0/fmsfdata/converter.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-0.1.0/fmsfdata/datastore/_store.py` & `fmsfdata-0.2.0/fmsfdata/datastore/_store.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-0.1.0/fmsfdata/datastore/_table.py` & `fmsfdata-0.2.0/fmsfdata/datastore/_table.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-0.1.0/fmsfdata/datastore/_table_row.py` & `fmsfdata-0.2.0/fmsfdata/datastore/_table_row.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-0.1.0/fmsfdata/exporter.py` & `fmsfdata-0.2.0/fmsfdata/exporter.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-0.1.0/fmsfdata/identifier.py` & `fmsfdata-0.2.0/fmsfdata/identifier.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-0.1.0/fmsfdata/normaliser.py` & `fmsfdata-0.2.0/fmsfdata/normaliser.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-0.1.0/fmsfdata/schema/_data.py` & `fmsfdata-0.2.0/fmsfdata/schema/_data.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-0.1.0/fmsfdata/schema/_proxy.py` & `fmsfdata-0.2.0/fmsfdata/schema/_proxy.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-0.1.0/fmsfdata/schema/erd/__init__.py` & `fmsfdata-0.2.0/fmsfdata/schema/erd/__init__.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-0.1.0/fmsfdata/schema/erd/templates/erd.dot` & `fmsfdata-0.2.0/fmsfdata/schema/erd/templates/erd.dot`

 * *Files identical despite different names*

### Comparing `fmsfdata-0.1.0/fmsfdata/schema/parser/__init__.py` & `fmsfdata-0.2.0/fmsfdata/schema/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-0.1.0/fmsfdata/settings.py` & `fmsfdata-0.2.0/fmsfdata/settings.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-0.1.0/fmsfdata/standardiser.py` & `fmsfdata-0.2.0/fmsfdata/standardiser.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-0.1.0/fmsfdata/stream_parser/checks.py` & `fmsfdata-0.2.0/fmsfdata/stream_parser/checks.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-0.1.0/fmsfdata/stream_parser/collectors.py` & `fmsfdata-0.2.0/fmsfdata/stream_parser/collectors.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-0.1.0/fmsfdata/stream_parser/events.py` & `fmsfdata-0.2.0/fmsfdata/stream_parser/events.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-0.1.0/fmsfdata/stream_parser/filters/column_headers.py` & `fmsfdata-0.2.0/fmsfdata/stream_parser/filters/column_headers.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-0.1.0/fmsfdata/stream_parser/filters/context.py` & `fmsfdata-0.2.0/fmsfdata/stream_parser/filters/context.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-0.1.0/fmsfdata/stream_parser/filters/generic.py` & `fmsfdata-0.2.0/fmsfdata/stream_parser/filters/generic.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-0.1.0/fmsfdata/stream_parser/filters/types.py` & `fmsfdata-0.2.0/fmsfdata/stream_parser/filters/types.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-0.1.0/fmsfdata/stream_parser/function_helpers.py` & `fmsfdata-0.2.0/fmsfdata/stream_parser/function_helpers.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-0.1.0/fmsfdata/stream_parser/parser/csv.py` & `fmsfdata-0.2.0/fmsfdata/stream_parser/parser/csv.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-0.1.0/fmsfdata/stream_parser/parser/openpyxl.py` & `fmsfdata-0.2.0/fmsfdata/stream_parser/parser/openpyxl.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-0.1.0/fmsfdata/stream_parser/parser/xml.py` & `fmsfdata-0.2.0/fmsfdata/stream_parser/parser/xml.py`

 * *Files identical despite different names*

### Comparing `fmsfdata-0.1.0/pyproject.toml` & `fmsfdata-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 [tool.poetry]
 name = "fmsfdata"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["franciscobmacedo <franciscovcbm@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 xsdata = "^23.7"
 jstyleson = "^0.0.2"
-pydantic = "^2.1.1"
 pyyaml = "^6.0.1"
 tablib = "^3.5.0"
 lxml = "^4.9.3"
 pandas = {version="^2.0.3", optional = true}
 more-itertools = "^10.0.0"
 openpyxl = "^3.1.2"
 pyhumps = "^3.8.0"
```

### Comparing `fmsfdata-0.1.0/PKG-INFO` & `fmsfdata-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: fmsfdata
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: franciscobmacedo
 Author-email: franciscovcbm@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: pandas
 Requires-Dist: jstyleson (>=0.0.2,<0.0.3)
 Requires-Dist: lxml (>=4.9.3,<5.0.0)
 Requires-Dist: more-itertools (>=10.0.0,<11.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0) ; extra == "pandas"
-Requires-Dist: pydantic (>=2.1.1,<3.0.0)
 Requires-Dist: pyhumps (>=3.8.0,<4.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: tablib (>=3.5.0,<4.0.0)
 Requires-Dist: xsdata (>=23.7,<24.0)
 Description-Content-Type: text/markdown
 
 # Social Finance Data Pipeline
```


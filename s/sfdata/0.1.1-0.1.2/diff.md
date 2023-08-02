# Comparing `tmp/sfdata-0.1.1.tar.gz` & `tmp/sfdata-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sfdata-0.1.1.tar", max compression
+gzip compressed data, was "sfdata-0.1.2.tar", max compression
```

## Comparing `sfdata-0.1.1.tar` & `sfdata-0.1.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     2200 2023-07-26 16:25:20.011374 sfdata-0.1.1/README.md
--rw-r--r--   0        0        0      564 2023-08-02 12:57:34.848697 sfdata-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       61 2023-08-02 09:04:23.701820 sfdata-0.1.1/sfdata/__init__.py
--rw-r--r--   0        0        0     1272 2023-07-31 13:26:53.452217 sfdata-0.1.1/sfdata/converter.py
--rw-r--r--   0        0        0      216 2023-07-31 11:10:27.203006 sfdata-0.1.1/sfdata/datastore/__init__.py
--rw-r--r--   0        0        0     1726 2023-07-31 12:01:41.140145 sfdata-0.1.1/sfdata/datastore/_store.py
--rw-r--r--   0        0        0     1775 2023-07-31 11:10:27.204118 sfdata-0.1.1/sfdata/datastore/_table.py
--rw-r--r--   0        0        0      480 2023-07-31 11:10:27.204508 sfdata-0.1.1/sfdata/datastore/_table_key.py
--rw-r--r--   0        0        0     2116 2023-07-31 11:10:27.204876 sfdata-0.1.1/sfdata/datastore/_table_row.py
--rw-r--r--   0        0        0     2793 2023-07-31 15:09:13.317115 sfdata-0.1.1/sfdata/exporter.py
--rw-r--r--   0        0        0     2055 2023-07-31 15:09:01.831911 sfdata-0.1.1/sfdata/identifier.py
--rw-r--r--   0        0        0     2900 2023-07-31 15:09:09.055005 sfdata-0.1.1/sfdata/normaliser.py
--rw-r--r--   0        0        0       51 2023-07-31 11:10:27.206997 sfdata-0.1.1/sfdata/schema/__init__.py
--rw-r--r--   0        0        0    13068 2023-08-02 12:56:48.724000 sfdata-0.1.1/sfdata/schema/_data.py
--rw-r--r--   0        0        0     9679 2023-07-31 11:10:27.208128 sfdata-0.1.1/sfdata/schema/_proxy.py
--rw-r--r--   0        0        0      164 2023-07-31 11:10:27.208691 sfdata-0.1.1/sfdata/schema/_types.py
--rw-r--r--   0        0        0     1221 2023-07-31 11:10:27.209231 sfdata-0.1.1/sfdata/schema/erd/__init__.py
--rw-r--r--   0        0        0      957 2023-07-31 11:10:27.209771 sfdata-0.1.1/sfdata/schema/erd/templates/erd.dot
--rw-r--r--   0        0        0      700 2023-07-31 11:10:27.210196 sfdata-0.1.1/sfdata/schema/parser/__init__.py
--rw-r--r--   0        0        0     1304 2023-08-02 12:56:48.724555 sfdata-0.1.1/sfdata/settings.py
--rw-r--r--   0        0        0     1528 2023-08-02 12:56:48.725089 sfdata-0.1.1/sfdata/standardiser.py
--rw-r--r--   0        0        0       22 2023-07-26 13:36:28.982395 sfdata-0.1.1/sfdata/stream_parser/__init__.py
--rw-r--r--   0        0        0     1633 2023-07-26 13:52:12.920476 sfdata-0.1.1/sfdata/stream_parser/checks.py
--rw-r--r--   0        0        0     7160 2023-07-31 12:53:10.728103 sfdata-0.1.1/sfdata/stream_parser/collectors.py
--rw-r--r--   0        0        0     1790 2023-08-02 12:56:48.725657 sfdata-0.1.1/sfdata/stream_parser/events.py
--rw-r--r--   0        0        0        0 2023-07-26 13:36:28.983244 sfdata-0.1.1/sfdata/stream_parser/filters/__init__.py
--rw-r--r--   0        0        0     2163 2023-08-02 12:56:48.726195 sfdata-0.1.1/sfdata/stream_parser/filters/column_headers.py
--rw-r--r--   0        0        0     1792 2023-07-31 11:10:27.211858 sfdata-0.1.1/sfdata/stream_parser/filters/context.py
--rw-r--r--   0        0        0     6096 2023-08-02 12:56:48.726757 sfdata-0.1.1/sfdata/stream_parser/filters/generic.py
--rw-r--r--   0        0        0     2427 2023-08-02 12:56:48.727276 sfdata-0.1.1/sfdata/stream_parser/filters/types.py
--rw-r--r--   0        0        0     2047 2023-07-26 13:52:18.473790 sfdata-0.1.1/sfdata/stream_parser/function_helpers.py
--rw-r--r--   0        0        0      423 2023-07-26 13:52:21.590448 sfdata-0.1.1/sfdata/stream_parser/functions.py
--rw-r--r--   0        0        0        0 2023-07-26 13:36:28.984861 sfdata-0.1.1/sfdata/stream_parser/parser/__init__.py
--rw-r--r--   0        0        0      525 2023-08-02 12:56:48.727815 sfdata-0.1.1/sfdata/stream_parser/parser/csv.py
--rw-r--r--   0        0        0     1873 2023-08-02 12:56:48.728271 sfdata-0.1.1/sfdata/stream_parser/parser/openpyxl.py
--rw-r--r--   0        0        0     1135 2023-08-02 12:56:48.728780 sfdata-0.1.1/sfdata/stream_parser/parser/xml.py
--rw-r--r--   0        0        0      482 2023-07-26 13:52:23.956423 sfdata-0.1.1/sfdata/stream_parser/stream.py
--rw-r--r--   0        0        0      293 2023-07-26 13:52:25.810886 sfdata-0.1.1/sfdata/stream_parser/types.py
--rw-r--r--   0        0        0     2948 1970-01-01 00:00:00.000000 sfdata-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2200 2023-07-26 16:25:20.011374 sfdata-0.1.2/README.md
+-rw-r--r--   0        0        0      564 2023-08-02 13:01:00.384438 sfdata-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       61 2023-08-02 09:04:23.701820 sfdata-0.1.2/sfdata/__init__.py
+-rw-r--r--   0        0        0     1272 2023-07-31 13:26:53.452217 sfdata-0.1.2/sfdata/converter.py
+-rw-r--r--   0        0        0      216 2023-07-31 11:10:27.203006 sfdata-0.1.2/sfdata/datastore/__init__.py
+-rw-r--r--   0        0        0     1726 2023-07-31 12:01:41.140145 sfdata-0.1.2/sfdata/datastore/_store.py
+-rw-r--r--   0        0        0     1775 2023-07-31 11:10:27.204118 sfdata-0.1.2/sfdata/datastore/_table.py
+-rw-r--r--   0        0        0      480 2023-07-31 11:10:27.204508 sfdata-0.1.2/sfdata/datastore/_table_key.py
+-rw-r--r--   0        0        0     2116 2023-07-31 11:10:27.204876 sfdata-0.1.2/sfdata/datastore/_table_row.py
+-rw-r--r--   0        0        0     2793 2023-07-31 15:09:13.317115 sfdata-0.1.2/sfdata/exporter.py
+-rw-r--r--   0        0        0     2055 2023-07-31 15:09:01.831911 sfdata-0.1.2/sfdata/identifier.py
+-rw-r--r--   0        0        0     2900 2023-07-31 15:09:09.055005 sfdata-0.1.2/sfdata/normaliser.py
+-rw-r--r--   0        0        0       51 2023-07-31 11:10:27.206997 sfdata-0.1.2/sfdata/schema/__init__.py
+-rw-r--r--   0        0        0    13068 2023-08-02 12:56:48.724000 sfdata-0.1.2/sfdata/schema/_data.py
+-rw-r--r--   0        0        0     9679 2023-07-31 11:10:27.208128 sfdata-0.1.2/sfdata/schema/_proxy.py
+-rw-r--r--   0        0        0      164 2023-07-31 11:10:27.208691 sfdata-0.1.2/sfdata/schema/_types.py
+-rw-r--r--   0        0        0     1221 2023-07-31 11:10:27.209231 sfdata-0.1.2/sfdata/schema/erd/__init__.py
+-rw-r--r--   0        0        0      957 2023-07-31 11:10:27.209771 sfdata-0.1.2/sfdata/schema/erd/templates/erd.dot
+-rw-r--r--   0        0        0      700 2023-07-31 11:10:27.210196 sfdata-0.1.2/sfdata/schema/parser/__init__.py
+-rw-r--r--   0        0        0     1304 2023-08-02 12:56:48.724555 sfdata-0.1.2/sfdata/settings.py
+-rw-r--r--   0        0        0     1528 2023-08-02 12:56:48.725089 sfdata-0.1.2/sfdata/standardiser.py
+-rw-r--r--   0        0        0       22 2023-07-26 13:36:28.982395 sfdata-0.1.2/sfdata/stream_parser/__init__.py
+-rw-r--r--   0        0        0     1633 2023-07-26 13:52:12.920476 sfdata-0.1.2/sfdata/stream_parser/checks.py
+-rw-r--r--   0        0        0     7160 2023-07-31 12:53:10.728103 sfdata-0.1.2/sfdata/stream_parser/collectors.py
+-rw-r--r--   0        0        0     1790 2023-08-02 12:56:48.725657 sfdata-0.1.2/sfdata/stream_parser/events.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:36:28.983244 sfdata-0.1.2/sfdata/stream_parser/filters/__init__.py
+-rw-r--r--   0        0        0     2163 2023-08-02 12:56:48.726195 sfdata-0.1.2/sfdata/stream_parser/filters/column_headers.py
+-rw-r--r--   0        0        0     1792 2023-07-31 11:10:27.211858 sfdata-0.1.2/sfdata/stream_parser/filters/context.py
+-rw-r--r--   0        0        0     6096 2023-08-02 12:56:48.726757 sfdata-0.1.2/sfdata/stream_parser/filters/generic.py
+-rw-r--r--   0        0        0     2427 2023-08-02 12:56:48.727276 sfdata-0.1.2/sfdata/stream_parser/filters/types.py
+-rw-r--r--   0        0        0     2047 2023-07-26 13:52:18.473790 sfdata-0.1.2/sfdata/stream_parser/function_helpers.py
+-rw-r--r--   0        0        0      423 2023-07-26 13:52:21.590448 sfdata-0.1.2/sfdata/stream_parser/functions.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:36:28.984861 sfdata-0.1.2/sfdata/stream_parser/parser/__init__.py
+-rw-r--r--   0        0        0      525 2023-08-02 12:56:48.727815 sfdata-0.1.2/sfdata/stream_parser/parser/csv.py
+-rw-r--r--   0        0        0     1873 2023-08-02 12:56:48.728271 sfdata-0.1.2/sfdata/stream_parser/parser/openpyxl.py
+-rw-r--r--   0        0        0     1135 2023-08-02 12:56:48.728780 sfdata-0.1.2/sfdata/stream_parser/parser/xml.py
+-rw-r--r--   0        0        0      482 2023-07-26 13:52:23.956423 sfdata-0.1.2/sfdata/stream_parser/stream.py
+-rw-r--r--   0        0        0      293 2023-07-26 13:52:25.810886 sfdata-0.1.2/sfdata/stream_parser/types.py
+-rw-r--r--   0        0        0     2948 1970-01-01 00:00:00.000000 sfdata-0.1.2/PKG-INFO
```

### Comparing `sfdata-0.1.1/README.md` & `sfdata-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sfdata-0.1.1/pyproject.toml` & `sfdata-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "sfdata"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["franciscobmacedo <franciscovcbm@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 xsdata = "^23.7"
 jstyleson = "^0.0.2"
 pydantic = "^2.1.1"
 pyyaml = "^6.0.1"
 tablib = "^3.5.0"
 lxml = "^4.9.3"
-pandas = "^2.0.3"
+pandas = "^1.5.2"
 more-itertools = "^10.0.0"
 openpyxl = "^3.1.2"
 pyhumps = "^3.8.0"
 
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.25.0"
```

### Comparing `sfdata-0.1.1/sfdata/converter.py` & `sfdata-0.1.2/sfdata/converter.py`

 * *Files identical despite different names*

### Comparing `sfdata-0.1.1/sfdata/datastore/_store.py` & `sfdata-0.1.2/sfdata/datastore/_store.py`

 * *Files identical despite different names*

### Comparing `sfdata-0.1.1/sfdata/datastore/_table.py` & `sfdata-0.1.2/sfdata/datastore/_table.py`

 * *Files identical despite different names*

### Comparing `sfdata-0.1.1/sfdata/datastore/_table_row.py` & `sfdata-0.1.2/sfdata/datastore/_table_row.py`

 * *Files identical despite different names*

### Comparing `sfdata-0.1.1/sfdata/exporter.py` & `sfdata-0.1.2/sfdata/exporter.py`

 * *Files identical despite different names*

### Comparing `sfdata-0.1.1/sfdata/identifier.py` & `sfdata-0.1.2/sfdata/identifier.py`

 * *Files identical despite different names*

### Comparing `sfdata-0.1.1/sfdata/normaliser.py` & `sfdata-0.1.2/sfdata/normaliser.py`

 * *Files identical despite different names*

### Comparing `sfdata-0.1.1/sfdata/schema/_data.py` & `sfdata-0.1.2/sfdata/schema/_data.py`

 * *Files identical despite different names*

### Comparing `sfdata-0.1.1/sfdata/schema/_proxy.py` & `sfdata-0.1.2/sfdata/schema/_proxy.py`

 * *Files identical despite different names*

### Comparing `sfdata-0.1.1/sfdata/schema/erd/__init__.py` & `sfdata-0.1.2/sfdata/schema/erd/__init__.py`

 * *Files identical despite different names*

### Comparing `sfdata-0.1.1/sfdata/schema/erd/templates/erd.dot` & `sfdata-0.1.2/sfdata/schema/erd/templates/erd.dot`

 * *Files identical despite different names*

### Comparing `sfdata-0.1.1/sfdata/schema/parser/__init__.py` & `sfdata-0.1.2/sfdata/schema/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `sfdata-0.1.1/sfdata/settings.py` & `sfdata-0.1.2/sfdata/settings.py`

 * *Files identical despite different names*

### Comparing `sfdata-0.1.1/sfdata/standardiser.py` & `sfdata-0.1.2/sfdata/standardiser.py`

 * *Files identical despite different names*

### Comparing `sfdata-0.1.1/sfdata/stream_parser/checks.py` & `sfdata-0.1.2/sfdata/stream_parser/checks.py`

 * *Files identical despite different names*

### Comparing `sfdata-0.1.1/sfdata/stream_parser/collectors.py` & `sfdata-0.1.2/sfdata/stream_parser/collectors.py`

 * *Files identical despite different names*

### Comparing `sfdata-0.1.1/sfdata/stream_parser/events.py` & `sfdata-0.1.2/sfdata/stream_parser/events.py`

 * *Files identical despite different names*

### Comparing `sfdata-0.1.1/sfdata/stream_parser/filters/column_headers.py` & `sfdata-0.1.2/sfdata/stream_parser/filters/column_headers.py`

 * *Files identical despite different names*

### Comparing `sfdata-0.1.1/sfdata/stream_parser/filters/context.py` & `sfdata-0.1.2/sfdata/stream_parser/filters/context.py`

 * *Files identical despite different names*

### Comparing `sfdata-0.1.1/sfdata/stream_parser/filters/generic.py` & `sfdata-0.1.2/sfdata/stream_parser/filters/generic.py`

 * *Files identical despite different names*

### Comparing `sfdata-0.1.1/sfdata/stream_parser/filters/types.py` & `sfdata-0.1.2/sfdata/stream_parser/filters/types.py`

 * *Files identical despite different names*

### Comparing `sfdata-0.1.1/sfdata/stream_parser/function_helpers.py` & `sfdata-0.1.2/sfdata/stream_parser/function_helpers.py`

 * *Files identical despite different names*

### Comparing `sfdata-0.1.1/sfdata/stream_parser/parser/csv.py` & `sfdata-0.1.2/sfdata/stream_parser/parser/csv.py`

 * *Files identical despite different names*

### Comparing `sfdata-0.1.1/sfdata/stream_parser/parser/openpyxl.py` & `sfdata-0.1.2/sfdata/stream_parser/parser/openpyxl.py`

 * *Files identical despite different names*

### Comparing `sfdata-0.1.1/sfdata/stream_parser/parser/xml.py` & `sfdata-0.1.2/sfdata/stream_parser/parser/xml.py`

 * *Files identical despite different names*

### Comparing `sfdata-0.1.1/PKG-INFO` & `sfdata-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: sfdata
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: franciscobmacedo
 Author-email: franciscovcbm@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jstyleson (>=0.0.2,<0.0.3)
 Requires-Dist: lxml (>=4.9.3,<5.0.0)
 Requires-Dist: more-itertools (>=10.0.0,<11.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
-Requires-Dist: pandas (>=2.0.3,<3.0.0)
+Requires-Dist: pandas (>=1.5.2,<2.0.0)
 Requires-Dist: pydantic (>=2.1.1,<3.0.0)
 Requires-Dist: pyhumps (>=3.8.0,<4.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: tablib (>=3.5.0,<4.0.0)
 Requires-Dist: xsdata (>=23.7,<24.0)
 Description-Content-Type: text/markdown
```


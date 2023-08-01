# Comparing `tmp/tflstatuscli-0.1.2.tar.gz` & `tmp/tflstatuscli-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tflstatuscli-0.1.2.tar", max compression
+gzip compressed data, was "tflstatuscli-0.1.4.tar", max compression
```

## Comparing `tflstatuscli-0.1.2.tar` & `tflstatuscli-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      821 2023-08-01 18:43:56.625056 tflstatuscli-0.1.2/README.md
--rw-r--r--   0        0        0      461 2023-08-01 20:21:40.777857 tflstatuscli-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-26 22:24:52.823601 tflstatuscli-0.1.2/tflstatuscli/__init__.py
--rwxr-xr-x   0        0        0     2363 2023-08-01 18:02:56.312839 tflstatuscli-0.1.2/tflstatuscli/tflstatuscli.py
--rw-r--r--   0        0        0     1356 1970-01-01 00:00:00.000000 tflstatuscli-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1126 2023-08-01 23:01:03.979023 tflstatuscli-0.1.4/README.md
+-rw-r--r--   0        0        0      486 2023-08-01 22:37:46.805945 tflstatuscli-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-26 22:24:52.823601 tflstatuscli-0.1.4/tflstatuscli/__init__.py
+-rwxr-xr-x   0        0        0     3959 2023-08-01 23:03:04.132392 tflstatuscli-0.1.4/tflstatuscli/tflstatuscli.py
+-rw-r--r--   0        0        0     1661 1970-01-01 00:00:00.000000 tflstatuscli-0.1.4/PKG-INFO
```

### Comparing `tflstatuscli-0.1.2/PKG-INFO` & `tflstatuscli-0.1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tflstatuscli
-Version: 0.1.2
+Version: 0.1.4
 Summary: Query TFL tube line status
 Author: stevenb92
 Author-email: stevenb92@icloud.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -46,7 +46,27 @@
 - Waterloo & City
 
 ### Show all disruptions on TFL tube lines
 ```bash
 tflcli disruptions
 ```
 
+## Poetry Usage
+Run these commands within project root dir with python poetry installed.
+
+### Install package and dependancies locally
+```bash
+poetry install
+```
+
+### Run tests 
+```bash
+poetry run pytest -v
+``` 
+
+### Build wheel 
+```
+poetry build
+```
+NOTE: Wheel located under /dist in project root dir
+
+
```


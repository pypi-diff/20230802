# Comparing `tmp/tflstatuscli-0.1.4.tar.gz` & `tmp/tflstatuscli-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tflstatuscli-0.1.4.tar", max compression
+gzip compressed data, was "tflstatuscli-0.1.5.tar", max compression
```

## Comparing `tflstatuscli-0.1.4.tar` & `tflstatuscli-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1126 2023-08-01 23:01:03.979023 tflstatuscli-0.1.4/README.md
--rw-r--r--   0        0        0      486 2023-08-01 22:37:46.805945 tflstatuscli-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-26 22:24:52.823601 tflstatuscli-0.1.4/tflstatuscli/__init__.py
--rwxr-xr-x   0        0        0     3959 2023-08-01 23:03:04.132392 tflstatuscli-0.1.4/tflstatuscli/tflstatuscli.py
--rw-r--r--   0        0        0     1661 1970-01-01 00:00:00.000000 tflstatuscli-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1680 2023-08-01 23:05:38.529443 tflstatuscli-0.1.5/README.md
+-rw-r--r--   0        0        0      486 2023-08-01 23:06:06.896569 tflstatuscli-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-26 22:24:52.823601 tflstatuscli-0.1.5/tflstatuscli/__init__.py
+-rwxr-xr-x   0        0        0     3959 2023-08-01 23:03:04.132392 tflstatuscli-0.1.5/tflstatuscli/tflstatuscli.py
+-rw-r--r--   0        0        0     2215 1970-01-01 00:00:00.000000 tflstatuscli-0.1.5/PKG-INFO
```

### Comparing `tflstatuscli-0.1.4/README.md` & `tflstatuscli-0.1.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,32 @@
 - Jubilee            
 - Metropolitan                                         
 - Northern           
 - Piccadilly         
 - Victoria           
 - Waterloo & City
 
+### Show future disruptions of particular tube line
+```bash
+tflcli status --line <line_name> --startdate YYYY-MM-DD --enddate YYYY-MM-DD
+```
+NOTE: When searching a particular tube line, validity is checked against the TFL APIs list of tube lines which at the time of writing this includes;
+- Bakerloo 
+- Central            
+- Circle             
+- District           
+- Hammersmith & City 
+- Jubilee            
+- Metropolitan                                         
+- Northern           
+- Piccadilly         
+- Victoria           
+- Waterloo & City
+
+
 ### Show all disruptions on TFL tube lines
 ```bash
 tflcli disruptions
 ```
 
 ## Poetry Usage
 Run these commands within project root dir with python poetry installed.
```

### Comparing `tflstatuscli-0.1.4/tflstatuscli/tflstatuscli.py` & `tflstatuscli-0.1.5/tflstatuscli/tflstatuscli.py`

 * *Files identical despite different names*

### Comparing `tflstatuscli-0.1.4/PKG-INFO` & `tflstatuscli-0.1.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tflstatuscli
-Version: 0.1.4
+Version: 0.1.5
 Summary: Query TFL tube line status
 Author: stevenb92
 Author-email: stevenb92@icloud.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -41,14 +41,32 @@
 - Jubilee            
 - Metropolitan                                         
 - Northern           
 - Piccadilly         
 - Victoria           
 - Waterloo & City
 
+### Show future disruptions of particular tube line
+```bash
+tflcli status --line <line_name> --startdate YYYY-MM-DD --enddate YYYY-MM-DD
+```
+NOTE: When searching a particular tube line, validity is checked against the TFL APIs list of tube lines which at the time of writing this includes;
+- Bakerloo 
+- Central            
+- Circle             
+- District           
+- Hammersmith & City 
+- Jubilee            
+- Metropolitan                                         
+- Northern           
+- Piccadilly         
+- Victoria           
+- Waterloo & City
+
+
 ### Show all disruptions on TFL tube lines
 ```bash
 tflcli disruptions
 ```
 
 ## Poetry Usage
 Run these commands within project root dir with python poetry installed.
```


# Comparing `tmp/umpyutl-2.0.1.tar.gz` & `tmp/umpyutl-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umpyutl-2.0.1.tar", last modified: Mon Jan  2 17:05:42 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `umpyutl-2.0.1.tar` & `umpyutl-2.1.0.tar`

### file list

```diff
@@ -1,18 +1,12 @@
-drwxr-xr-x   0 arwhyte    (501) staff       (20)        0 2023-01-02 17:05:42.029981 umpyutl-2.0.1/
--rw-r--r--   0 arwhyte    (501) staff       (20)     1521 2022-10-10 03:13:21.000000 umpyutl-2.0.1/LICENSE
--rw-r--r--   0 arwhyte    (501) staff       (20)      567 2023-01-02 17:05:42.029865 umpyutl-2.0.1/PKG-INFO
--rw-r--r--   0 arwhyte    (501) staff       (20)      100 2022-12-17 20:31:15.000000 umpyutl-2.0.1/README.md
--rw-r--r--   0 arwhyte    (501) staff       (20)       38 2023-01-02 17:05:42.030023 umpyutl-2.0.1/setup.cfg
--rw-r--r--   0 arwhyte    (501) staff       (20)      901 2023-01-02 16:55:46.000000 umpyutl-2.0.1/setup.py
-drwxr-xr-x   0 arwhyte    (501) staff       (20)        0 2023-01-02 17:05:42.029004 umpyutl-2.0.1/umpyutl/
--rw-r--r--   0 arwhyte    (501) staff       (20)      128 2023-01-02 16:54:01.000000 umpyutl-2.0.1/umpyutl/__init__.py
--rw-r--r--   0 arwhyte    (501) staff       (20)     2304 2023-01-02 16:54:01.000000 umpyutl-2.0.1/umpyutl/convert.py
--rw-r--r--   0 arwhyte    (501) staff       (20)     1108 2023-01-02 16:54:01.000000 umpyutl-2.0.1/umpyutl/http.py
--rw-r--r--   0 arwhyte    (501) staff       (20)     8396 2023-01-02 16:54:01.000000 umpyutl-2.0.1/umpyutl/read.py
--rw-r--r--   0 arwhyte    (501) staff       (20)    10838 2023-01-02 16:54:01.000000 umpyutl-2.0.1/umpyutl/write.py
-drwxr-xr-x   0 arwhyte    (501) staff       (20)        0 2023-01-02 17:05:42.029705 umpyutl-2.0.1/umpyutl.egg-info/
--rw-r--r--   0 arwhyte    (501) staff       (20)      567 2023-01-02 17:05:42.000000 umpyutl-2.0.1/umpyutl.egg-info/PKG-INFO
--rw-r--r--   0 arwhyte    (501) staff       (20)      268 2023-01-02 17:05:42.000000 umpyutl-2.0.1/umpyutl.egg-info/SOURCES.txt
--rw-r--r--   0 arwhyte    (501) staff       (20)        1 2023-01-02 17:05:42.000000 umpyutl-2.0.1/umpyutl.egg-info/dependency_links.txt
--rw-r--r--   0 arwhyte    (501) staff       (20)       16 2023-01-02 17:05:42.000000 umpyutl-2.0.1/umpyutl.egg-info/requires.txt
--rw-r--r--   0 arwhyte    (501) staff       (20)        8 2023-01-02 17:05:42.000000 umpyutl-2.0.1/umpyutl.egg-info/top_level.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 umpyutl-2.1.0/src/umpyutl/__about__.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 umpyutl-2.1.0/src/umpyutl/__init__.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 umpyutl-2.1.0/src/umpyutl/convert.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 umpyutl-2.1.0/src/umpyutl/http.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 umpyutl-2.1.0/src/umpyutl/py.typed
+-rw-r--r--   0        0        0     8387 2020-02-02 00:00:00.000000 umpyutl-2.1.0/src/umpyutl/read.py
+-rw-r--r--   0        0        0    10838 2020-02-02 00:00:00.000000 umpyutl-2.1.0/src/umpyutl/write.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 umpyutl-2.1.0/.gitignore
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 umpyutl-2.1.0/LICENSE
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 umpyutl-2.1.0/README.md
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 umpyutl-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 umpyutl-2.1.0/PKG-INFO
```

### Comparing `umpyutl-2.0.1/LICENSE` & `umpyutl-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `umpyutl-2.0.1/PKG-INFO` & `umpyutl-2.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: umpyutl
-Version: 2.0.1
+Version: 2.1.0
 Summary: Utility classes and functions.
-Home-page: https://github.com/umsi-arwhyte/umpyutl
-Author: Anthony Whyte
-Author-email: anthwhyte@gmail.com
-Keywords: arwhyte,utilities,umpyutl
-Classifier: Programming Language :: Python :: 3
+Project-URL: Homepage, https://github.com/umsi-arwhyte/umpyutl
+Author-email: Anthony Whyte <anthwhyte@gmail.com>
+License: BSD-3-Clause
+License-File: LICENSE
+Keywords: arwhyte,umpyutl,utilities
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
+Requires-Dist: pyyaml
+Requires-Dist: requests
 Description-Content-Type: text/markdown
-License-File: LICENSE
+
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # umpyutl
 
 A collection of utility classes and functions.
 
-
 # mypy
 
 ```commandline
 mypy umpyutl
 ```
```

### Comparing `umpyutl-2.0.1/umpyutl/convert.py` & `umpyutl-2.1.0/src/umpyutl/convert.py`

 * *Files identical despite different names*

### Comparing `umpyutl-2.0.1/umpyutl/http.py` & `umpyutl-2.1.0/src/umpyutl/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import requests as req
 from typing import Optional
 
 
-def get_resource(
-    url: str, params: Optional[dict] = None, timeout: int = 10
-) -> req.Response:
+def get_resource(url: str, params: Optional[dict] = None, timeout: int = 10) -> req.Response:
     """Returns a response object.
 
     Parameters:
         url (str): a url that specifies the resource.
         params (dict): optional dictionary of querystring arguments.
         timeout (int): timeout value in seconds
 
@@ -18,17 +16,15 @@
 
     if params:
         return req.get(url, params, timeout=timeout)
     else:
         return req.get(url, timeout=timeout)
 
 
-def get_resource_json(
-    url: str, params: Optional[dict] = None, timeout: int = 10
-) -> dict | list:
+def get_resource_json(url: str, params: Optional[dict] = None, timeout: int = 10) -> dict | list:
     """Returns a response object decoded into a dictionary or list.
 
     Parameters:
         url (str): a url that specifies the resource.
         params (dict): optional dictionary of querystring arguments.
         timeout (int): timeout value in seconds
```

### Comparing `umpyutl-2.0.1/umpyutl/read.py` & `umpyutl-2.1.0/src/umpyutl/read.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,16 +29,15 @@
         delimiter (str): delimiter that separates the row values
 
     Returns:
         list: a list of nested "row" lists
     """
 
     with open(filepath, "r", encoding=encoding, newline=newline) as file_obj:
-        reader = csv.reader(file_obj, delimiter=delimiter)
-        return [row for row in reader]
+        return [row for row in csv.reader(file_obj, delimiter=delimiter)]
 
 
 def from_csv_to_dicts(
     filepath: str,
     encoding: str = "utf-8",
     newline: str = "",
     delimiter: str = ",",
@@ -57,19 +56,18 @@
         ordered (bool): return either list of OrderedDict objects or dict objects
 
     Returns:
         list: nested dictionaries representing the file contents
     """
 
     with open(filepath, "r", newline=newline, encoding=encoding) as file_obj:
-        reader = csv.DictReader(file_obj, delimiter=delimiter)
         if ordered:
-            return [row for row in reader]
+            return [row for row in csv.DictReader(file_obj, delimiter=delimiter)]
         else:
-            return [dict(row) for row in reader]
+            return [dict(row) for row in csv.DictReader(file_obj, delimiter=delimiter)]
 
 
 def from_json(filepath: str, encoding: str = "utf-8") -> dict | list:
     """Reads a JSON document, decodes the file content, and returns a list or dictionary if
     provided with a valid filepath.
 
     Parameters:
```

### Comparing `umpyutl-2.0.1/umpyutl/write.py` & `umpyutl-2.1.0/src/umpyutl/write.py`

 * *Files identical despite different names*


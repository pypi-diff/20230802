# Comparing `tmp/tlv-1.4.1.tar.gz` & `tmp/tlv-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tlv-1.4.1.tar", last modified: Mon Jul 24 10:28:24 2023, max compression
+gzip compressed data, was "tlv-1.4.2.tar", last modified: Wed Aug  2 09:47:16 2023, max compression
```

## Comparing `tlv-1.4.1.tar` & `tlv-1.4.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:28:24.680145 tlv-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-24 10:28:08.000000 tlv-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-24 10:28:08.000000 tlv-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11688 2023-07-24 10:28:24.680145 tlv-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-07-24 10:28:08.000000 tlv-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-24 10:28:08.000000 tlv-1.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-24 10:28:24.680145 tlv-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-24 10:28:24.000000 tlv-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:28:24.676145 tlv-1.4.1/tlv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:28:08.000000 tlv-1.4.1/tlv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-24 10:28:08.000000 tlv-1.4.1/tlv/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-24 10:28:08.000000 tlv-1.4.1/tlv/arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-07-24 10:28:08.000000 tlv-1.4.1/tlv/cls_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-24 10:28:08.000000 tlv-1.4.1/tlv/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-07-24 10:28:08.000000 tlv-1.4.1/tlv/lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-24 10:28:08.000000 tlv-1.4.1/tlv/src_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-24 10:28:08.000000 tlv-1.4.1/tlv/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:28:24.680145 tlv-1.4.1/tlv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11688 2023-07-24 10:28:24.000000 tlv-1.4.1/tlv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-24 10:28:24.000000 tlv-1.4.1/tlv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 10:28:24.000000 tlv-1.4.1/tlv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-24 10:28:24.000000 tlv-1.4.1/tlv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-24 10:28:24.000000 tlv-1.4.1/tlv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-24 10:28:24.000000 tlv-1.4.1/tlv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:47:16.759681 tlv-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-08-02 09:46:58.000000 tlv-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-02 09:46:58.000000 tlv-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11688 2023-08-02 09:47:16.763681 tlv-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-08-02 09:46:58.000000 tlv-1.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-02 09:46:58.000000 tlv-1.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-02 09:47:16.763681 tlv-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-08-02 09:47:16.000000 tlv-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:47:16.759681 tlv-1.4.2/tlv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 09:46:58.000000 tlv-1.4.2/tlv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-02 09:46:58.000000 tlv-1.4.2/tlv/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-08-02 09:46:58.000000 tlv-1.4.2/tlv/arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-08-02 09:46:58.000000 tlv-1.4.2/tlv/cls_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-02 09:46:58.000000 tlv-1.4.2/tlv/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-08-02 09:46:58.000000 tlv-1.4.2/tlv/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-08-02 09:46:58.000000 tlv-1.4.2/tlv/src_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-08-02 09:46:58.000000 tlv-1.4.2/tlv/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:47:16.759681 tlv-1.4.2/tlv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11688 2023-08-02 09:47:16.000000 tlv-1.4.2/tlv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-02 09:47:16.000000 tlv-1.4.2/tlv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 09:47:16.000000 tlv-1.4.2/tlv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-02 09:47:16.000000 tlv-1.4.2/tlv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-02 09:47:16.000000 tlv-1.4.2/tlv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-02 09:47:16.000000 tlv-1.4.2/tlv.egg-info/top_level.txt
```

### Comparing `tlv-1.4.1/LICENSE` & `tlv-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tlv-1.4.1/PKG-INFO` & `tlv-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tlv
-Version: 1.4.1
+Version: 1.4.2
 Summary: -- Too less variation -- Find duplicates in source code for various languages
 Home-page: https://github.com/priv-kweihmann/tlv
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tlv-1.4.1/README.md` & `tlv-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `tlv-1.4.1/setup.py` & `tlv-1.4.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 requirements = []
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="tlv",
-    version="1.4.1",
+    version="1.4.2",
     author="Konrad Weihmann",
     author_email="kweihmann@outlook.com",
     description="-- Too less variation -- Find duplicates in source code for various languages",
     long_description=_long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/priv-kweihmann/tlv",
     packages=setuptools.find_packages(),
```

### Comparing `tlv-1.4.1/tlv/arg_parser.py` & `tlv-1.4.2/tlv/arg_parser.py`

 * *Files identical despite different names*

### Comparing `tlv-1.4.1/tlv/cls_ast.py` & `tlv-1.4.2/tlv/cls_ast.py`

 * *Files identical despite different names*

### Comparing `tlv-1.4.1/tlv/lexer.py` & `tlv-1.4.2/tlv/lexer.py`

 * *Files identical despite different names*

### Comparing `tlv-1.4.1/tlv/src_parser.py` & `tlv-1.4.2/tlv/src_parser.py`

 * *Files identical despite different names*

### Comparing `tlv-1.4.1/tlv/tokens.py` & `tlv-1.4.2/tlv/tokens.py`

 * *Files identical despite different names*

### Comparing `tlv-1.4.1/tlv.egg-info/PKG-INFO` & `tlv-1.4.2/tlv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tlv
-Version: 1.4.1
+Version: 1.4.2
 Summary: -- Too less variation -- Find duplicates in source code for various languages
 Home-page: https://github.com/priv-kweihmann/tlv
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```


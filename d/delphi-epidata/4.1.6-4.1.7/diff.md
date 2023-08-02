# Comparing `tmp/delphi_epidata-4.1.6.tar.gz` & `tmp/delphi_epidata-4.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delphi_epidata-4.1.6.tar", last modified: Thu Jul 13 12:51:32 2023, max compression
+gzip compressed data, was "delphi_epidata-4.1.7.tar", last modified: Wed Aug  2 16:53:24 2023, max compression
```

## Comparing `delphi_epidata-4.1.6.tar` & `delphi_epidata-4.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:51:32.549520 delphi_epidata-4.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-13 12:51:20.000000 delphi_epidata-4.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-13 12:51:32.549520 delphi_epidata-4.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-13 12:51:20.000000 delphi_epidata-4.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:51:32.549520 delphi_epidata-4.1.6/delphi_epidata/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-13 12:51:20.000000 delphi_epidata-4.1.6/delphi_epidata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26740 2023-07-13 12:51:31.000000 delphi_epidata-4.1.6/delphi_epidata/delphi_epidata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:51:32.549520 delphi_epidata-4.1.6/delphi_epidata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-13 12:51:32.000000 delphi_epidata-4.1.6/delphi_epidata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-13 12:51:32.000000 delphi_epidata-4.1.6/delphi_epidata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 12:51:32.000000 delphi_epidata-4.1.6/delphi_epidata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-13 12:51:32.000000 delphi_epidata-4.1.6/delphi_epidata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 12:51:32.000000 delphi_epidata-4.1.6/delphi_epidata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 12:51:32.549520 delphi_epidata-4.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-13 12:51:20.000000 delphi_epidata-4.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:53:24.376552 delphi_epidata-4.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-08-02 16:53:10.000000 delphi_epidata-4.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 16:53:24.376552 delphi_epidata-4.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-02 16:53:10.000000 delphi_epidata-4.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:53:24.376552 delphi_epidata-4.1.7/delphi_epidata/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-02 16:53:10.000000 delphi_epidata-4.1.7/delphi_epidata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26740 2023-08-02 16:53:23.000000 delphi_epidata-4.1.7/delphi_epidata/delphi_epidata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:53:24.376552 delphi_epidata-4.1.7/delphi_epidata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 16:53:24.000000 delphi_epidata-4.1.7/delphi_epidata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-08-02 16:53:24.000000 delphi_epidata-4.1.7/delphi_epidata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:53:24.000000 delphi_epidata-4.1.7/delphi_epidata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 16:53:24.000000 delphi_epidata-4.1.7/delphi_epidata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-02 16:53:24.000000 delphi_epidata-4.1.7/delphi_epidata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 16:53:24.376552 delphi_epidata-4.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-02 16:53:10.000000 delphi_epidata-4.1.7/setup.py
```

### Comparing `delphi_epidata-4.1.6/LICENSE` & `delphi_epidata-4.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `delphi_epidata-4.1.6/PKG-INFO` & `delphi_epidata-4.1.7/delphi_epidata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: delphi_epidata
-Version: 4.1.6
+Name: delphi-epidata
+Version: 4.1.7
 Summary: A programmatic interface to Delphi's Epidata API.
 Home-page: https://github.com/cmu-delphi/delphi-epidata
 Author: David Farrow
 Author-email: dfarrow0@gmail.com
 License: UNKNOWN
 Description: # Delphi Epidata API Client
```

### Comparing `delphi_epidata-4.1.6/delphi_epidata/delphi_epidata.py` & `delphi_epidata-4.1.7/delphi_epidata/delphi_epidata.py`

 * *Files identical despite different names*

### Comparing `delphi_epidata-4.1.6/setup.py` & `delphi_epidata-4.1.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="delphi_epidata",
-    version="4.1.6",
+    version="4.1.7",
     author="David Farrow",
     author_email="dfarrow0@gmail.com",
     description="A programmatic interface to Delphi's Epidata API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cmu-delphi/delphi-epidata",
     packages=setuptools.find_packages(),
```


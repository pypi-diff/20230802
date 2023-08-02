# Comparing `tmp/dcf-tools-2.4.1.tar.gz` & `tmp/dcf-tools-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcf-tools-2.4.1.tar", last modified: Thu Jan 26 14:31:09 2023, max compression
+gzip compressed data, was "dcf-tools-2.4.2.tar", last modified: Wed Aug  2 12:12:33 2023, max compression
```

## Comparing `dcf-tools-2.4.1.tar` & `dcf-tools-2.4.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 uy        (1000) uy        (1000)        0 2023-01-26 14:31:09.490274 dcf-tools-2.4.1/
--rw-rw-r--   0 uy        (1000) uy        (1000)      295 2023-01-26 14:31:09.490274 dcf-tools-2.4.1/PKG-INFO
-drwxrwxr-x   0 uy        (1000) uy        (1000)        0 2023-01-26 14:31:09.490274 dcf-tools-2.4.1/dcf/
--rw-rw-r--   0 uy        (1000) uy        (1000)      813 2023-01-26 13:02:12.000000 dcf-tools-2.4.1/dcf/__init__.py
--rw-rw-r--   0 uy        (1000) uy        (1000)      927 2023-01-26 13:02:12.000000 dcf-tools-2.4.1/dcf/cli.py
--rw-rw-r--   0 uy        (1000) uy        (1000)    21931 2023-01-26 13:02:12.000000 dcf-tools-2.4.1/dcf/device.py
--rw-rw-r--   0 uy        (1000) uy        (1000)    25126 2023-01-26 13:02:12.000000 dcf-tools-2.4.1/dcf/lint.py
--rw-rw-r--   0 uy        (1000) uy        (1000)     9500 2023-01-26 13:02:12.000000 dcf-tools-2.4.1/dcf/parse.py
--rw-rw-r--   0 uy        (1000) uy        (1000)     2435 2023-01-26 13:02:12.000000 dcf-tools-2.4.1/dcf/print.py
-drwxrwxr-x   0 uy        (1000) uy        (1000)        0 2023-01-26 14:31:09.490274 dcf-tools-2.4.1/dcf2dev/
--rw-rw-r--   0 uy        (1000) uy        (1000)       72 2023-01-26 13:02:12.000000 dcf-tools-2.4.1/dcf2dev/__init__.py
--rw-rw-r--   0 uy        (1000) uy        (1000)     9439 2023-01-26 13:02:12.000000 dcf-tools-2.4.1/dcf2dev/cdevice.py
--rw-rw-r--   0 uy        (1000) uy        (1000)     2268 2023-01-26 13:02:12.000000 dcf-tools-2.4.1/dcf2dev/cli.py
-drwxrwxr-x   0 uy        (1000) uy        (1000)        0 2023-01-26 14:31:09.490274 dcf-tools-2.4.1/dcf2dev/data/
--rw-rw-r--   0 uy        (1000) uy        (1000)     3240 2023-01-26 13:02:12.000000 dcf-tools-2.4.1/dcf2dev/data/dev.c.em
--rw-rw-r--   0 uy        (1000) uy        (1000)      365 2023-01-26 13:02:12.000000 dcf-tools-2.4.1/dcf2dev/data/dev.h.em
-drwxrwxr-x   0 uy        (1000) uy        (1000)        0 2023-01-26 14:31:09.490274 dcf-tools-2.4.1/dcf_tools.egg-info/
--rw-rw-r--   0 uy        (1000) uy        (1000)      295 2023-01-26 14:31:09.000000 dcf-tools-2.4.1/dcf_tools.egg-info/PKG-INFO
--rw-rw-r--   0 uy        (1000) uy        (1000)      450 2023-01-26 14:31:09.000000 dcf-tools-2.4.1/dcf_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 uy        (1000) uy        (1000)        1 2023-01-26 14:31:09.000000 dcf-tools-2.4.1/dcf_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 uy        (1000) uy        (1000)       92 2023-01-26 14:31:09.000000 dcf-tools-2.4.1/dcf_tools.egg-info/entry_points.txt
--rw-rw-r--   0 uy        (1000) uy        (1000)       25 2023-01-26 14:31:09.000000 dcf-tools-2.4.1/dcf_tools.egg-info/requires.txt
--rw-rw-r--   0 uy        (1000) uy        (1000)       19 2023-01-26 14:31:09.000000 dcf-tools-2.4.1/dcf_tools.egg-info/top_level.txt
-drwxrwxr-x   0 uy        (1000) uy        (1000)        0 2023-01-26 14:31:09.490274 dcf-tools-2.4.1/dcfgen/
--rw-rw-r--   0 uy        (1000) uy        (1000)        0 2023-01-26 13:02:12.000000 dcf-tools-2.4.1/dcfgen/__init__.py
--rw-rw-r--   0 uy        (1000) uy        (1000)    25174 2023-01-26 13:02:12.000000 dcf-tools-2.4.1/dcfgen/cli.py
-drwxrwxr-x   0 uy        (1000) uy        (1000)        0 2023-01-26 14:31:09.490274 dcf-tools-2.4.1/dcfgen/data/
--rw-rw-r--   0 uy        (1000) uy        (1000)    17372 2023-01-26 13:02:12.000000 dcf-tools-2.4.1/dcfgen/data/master.dcf.em
--rw-r--r--   0 uy        (1000) uy        (1000)      688 2023-01-26 13:10:29.000000 dcf-tools-2.4.1/pyproject.toml
--rw-rw-r--   0 uy        (1000) uy        (1000)       38 2023-01-26 14:31:09.490274 dcf-tools-2.4.1/setup.cfg
+drwxrwxr-x   0 uy        (1000) uy        (1000)        0 2023-08-02 12:12:33.585452 dcf-tools-2.4.2/
+-rw-rw-r--   0 uy        (1000) uy        (1000)      295 2023-08-02 12:12:33.585452 dcf-tools-2.4.2/PKG-INFO
+drwxrwxr-x   0 uy        (1000) uy        (1000)        0 2023-08-02 12:12:33.585452 dcf-tools-2.4.2/dcf/
+-rw-rw-r--   0 uy        (1000) uy        (1000)      813 2023-01-26 13:02:12.000000 dcf-tools-2.4.2/dcf/__init__.py
+-rw-rw-r--   0 uy        (1000) uy        (1000)      927 2023-01-26 13:02:12.000000 dcf-tools-2.4.2/dcf/cli.py
+-rw-rw-r--   0 uy        (1000) uy        (1000)    21931 2023-01-26 13:02:12.000000 dcf-tools-2.4.2/dcf/device.py
+-rw-rw-r--   0 uy        (1000) uy        (1000)    25126 2023-01-26 13:02:12.000000 dcf-tools-2.4.2/dcf/lint.py
+-rw-rw-r--   0 uy        (1000) uy        (1000)     9500 2023-01-26 13:02:12.000000 dcf-tools-2.4.2/dcf/parse.py
+-rw-rw-r--   0 uy        (1000) uy        (1000)     2435 2023-01-26 13:02:12.000000 dcf-tools-2.4.2/dcf/print.py
+drwxrwxr-x   0 uy        (1000) uy        (1000)        0 2023-08-02 12:12:33.585452 dcf-tools-2.4.2/dcf2dev/
+-rw-rw-r--   0 uy        (1000) uy        (1000)       72 2023-01-26 13:02:12.000000 dcf-tools-2.4.2/dcf2dev/__init__.py
+-rw-rw-r--   0 uy        (1000) uy        (1000)     9439 2023-01-26 13:02:12.000000 dcf-tools-2.4.2/dcf2dev/cdevice.py
+-rw-rw-r--   0 uy        (1000) uy        (1000)     2268 2023-01-26 13:02:12.000000 dcf-tools-2.4.2/dcf2dev/cli.py
+drwxrwxr-x   0 uy        (1000) uy        (1000)        0 2023-08-02 12:12:33.585452 dcf-tools-2.4.2/dcf2dev/data/
+-rw-rw-r--   0 uy        (1000) uy        (1000)     3240 2023-01-26 13:02:12.000000 dcf-tools-2.4.2/dcf2dev/data/dev.c.em
+-rw-rw-r--   0 uy        (1000) uy        (1000)      365 2023-01-26 13:02:12.000000 dcf-tools-2.4.2/dcf2dev/data/dev.h.em
+drwxrwxr-x   0 uy        (1000) uy        (1000)        0 2023-08-02 12:12:33.585452 dcf-tools-2.4.2/dcf_tools.egg-info/
+-rw-rw-r--   0 uy        (1000) uy        (1000)      295 2023-08-02 12:12:33.000000 dcf-tools-2.4.2/dcf_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 uy        (1000) uy        (1000)      450 2023-08-02 12:12:33.000000 dcf-tools-2.4.2/dcf_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 uy        (1000) uy        (1000)        1 2023-08-02 12:12:33.000000 dcf-tools-2.4.2/dcf_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 uy        (1000) uy        (1000)       92 2023-08-02 12:12:33.000000 dcf-tools-2.4.2/dcf_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 uy        (1000) uy        (1000)       25 2023-08-02 12:12:33.000000 dcf-tools-2.4.2/dcf_tools.egg-info/requires.txt
+-rw-rw-r--   0 uy        (1000) uy        (1000)       19 2023-08-02 12:12:33.000000 dcf-tools-2.4.2/dcf_tools.egg-info/top_level.txt
+drwxrwxr-x   0 uy        (1000) uy        (1000)        0 2023-08-02 12:12:33.585452 dcf-tools-2.4.2/dcfgen/
+-rw-rw-r--   0 uy        (1000) uy        (1000)        0 2023-01-26 13:02:12.000000 dcf-tools-2.4.2/dcfgen/__init__.py
+-rw-rw-r--   0 uy        (1000) uy        (1000)    25201 2023-08-02 11:58:44.000000 dcf-tools-2.4.2/dcfgen/cli.py
+drwxrwxr-x   0 uy        (1000) uy        (1000)        0 2023-08-02 12:12:33.585452 dcf-tools-2.4.2/dcfgen/data/
+-rw-rw-r--   0 uy        (1000) uy        (1000)    17372 2023-01-26 13:02:12.000000 dcf-tools-2.4.2/dcfgen/data/master.dcf.em
+-rw-rw-r--   0 uy        (1000) uy        (1000)      688 2023-08-02 12:06:39.000000 dcf-tools-2.4.2/pyproject.toml
+-rw-rw-r--   0 uy        (1000) uy        (1000)       38 2023-08-02 12:12:33.585452 dcf-tools-2.4.2/setup.cfg
```

### Comparing `dcf-tools-2.4.1/dcf/__init__.py` & `dcf-tools-2.4.2/dcf/__init__.py`

 * *Files identical despite different names*

### Comparing `dcf-tools-2.4.1/dcf/cli.py` & `dcf-tools-2.4.2/dcf/cli.py`

 * *Files identical despite different names*

### Comparing `dcf-tools-2.4.1/dcf/device.py` & `dcf-tools-2.4.2/dcf/device.py`

 * *Files identical despite different names*

### Comparing `dcf-tools-2.4.1/dcf/lint.py` & `dcf-tools-2.4.2/dcf/lint.py`

 * *Files identical despite different names*

### Comparing `dcf-tools-2.4.1/dcf/parse.py` & `dcf-tools-2.4.2/dcf/parse.py`

 * *Files identical despite different names*

### Comparing `dcf-tools-2.4.1/dcf/print.py` & `dcf-tools-2.4.2/dcf/print.py`

 * *Files identical despite different names*

### Comparing `dcf-tools-2.4.1/dcf2dev/cdevice.py` & `dcf-tools-2.4.2/dcf2dev/cdevice.py`

 * *Files identical despite different names*

### Comparing `dcf-tools-2.4.1/dcf2dev/cli.py` & `dcf-tools-2.4.2/dcf2dev/cli.py`

 * *Files identical despite different names*

### Comparing `dcf-tools-2.4.1/dcf2dev/data/dev.c.em` & `dcf-tools-2.4.2/dcf2dev/data/dev.c.em`

 * *Files identical despite different names*

### Comparing `dcf-tools-2.4.1/dcfgen/cli.py` & `dcf-tools-2.4.2/dcfgen/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
                 if sync_start != pdo.sync_start_value:
                     pdo.sync_start_value = sync_start
                     if is_tpdo:
                         sdo.append(self.concise_value(comm_idx, 6, sync_start))
 
             map_idx = comm_idx + 0x200
             if "mapping" in cfg:
-                if pdo.n > 0:
+                if pdo.n > 0 or len(cfg["mapping"]) > 0:
                     pdo.n = 0
                     pdo.mapping = {}
                     sdo.append(self.concise_value(map_idx, 0, 0))
 
                 size = 0
                 n = 0
                 for pdo_mapping in cfg["mapping"]:
```

### Comparing `dcf-tools-2.4.1/dcfgen/data/master.dcf.em` & `dcf-tools-2.4.2/dcfgen/data/master.dcf.em`

 * *Files identical despite different names*

### Comparing `dcf-tools-2.4.1/pyproject.toml` & `dcf-tools-2.4.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dcf-tools"
-version = "2.4.1"
+version = "2.4.2"
 dependencies = ["PyYAML>=3.08", "empy>=3.3.2"]
 authors = [
   {name = "J. S. Seldenthuis", email = "jseldenthuis@lely.com"}
 ]
 description = "Tools to generate and manipulate DCF files"
 classifiers=["License :: OSI Approved :: Apache Software License"]
```


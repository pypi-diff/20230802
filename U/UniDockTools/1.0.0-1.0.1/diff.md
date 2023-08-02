# Comparing `tmp/UniDockTools-1.0.0.tar.gz` & `tmp/UniDockTools-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UniDockTools-1.0.0.tar", last modified: Wed Aug  2 03:18:17 2023, max compression
+gzip compressed data, was "UniDockTools-1.0.1.tar", last modified: Wed Aug  2 03:22:25 2023, max compression
```

## Comparing `UniDockTools-1.0.0.tar` & `UniDockTools-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 4294967294 4294967294        0 2023-08-02 03:18:17.680096 UniDockTools-1.0.0/
--rw-r--r--   0 4294967294 4294967294     1063 2023-08-02 02:58:30.000000 UniDockTools-1.0.0/LICENSE
--rw-r--r--   0 4294967294 4294967294      332 2023-08-02 03:18:17.672003 UniDockTools-1.0.0/PKG-INFO
--rw-r--r--   0 4294967294 4294967294      880 2023-08-02 02:58:30.000000 UniDockTools-1.0.0/README.md
-drwxr-xr-x   0 4294967294 4294967294        0 2023-08-02 03:18:17.339855 UniDockTools-1.0.0/UniDockTools/
--rw-r--r--   0 4294967294 4294967294       28 2023-08-02 02:58:31.000000 UniDockTools-1.0.0/UniDockTools/__init__.py
-drwxr-xr-x   0 4294967294 4294967294        0 2023-08-02 03:18:17.631291 UniDockTools-1.0.0/UniDockTools/ligandPrepare/
--rw-r--r--   0 4294967294 4294967294       92 2023-08-02 02:58:31.000000 UniDockTools-1.0.0/UniDockTools/ligandPrepare/__init__.py
--rw-r--r--   0 4294967294 4294967294     2951 2023-08-02 02:58:31.000000 UniDockTools-1.0.0/UniDockTools/ligandPrepare/atom_type.py
--rw-r--r--   0 4294967294 4294967294      924 2023-08-02 02:58:31.000000 UniDockTools-1.0.0/UniDockTools/ligandPrepare/rotatable_bond.py
--rw-r--r--   0 4294967294 4294967294    19674 2023-08-02 02:58:31.000000 UniDockTools-1.0.0/UniDockTools/ligandPrepare/topology_builder.py
--rw-r--r--   0 4294967294 4294967294     4987 2023-08-02 02:58:31.000000 UniDockTools-1.0.0/UniDockTools/ligandPrepare/utils.py
--rw-r--r--   0 4294967294 4294967294    13477 2023-08-02 03:16:24.000000 UniDockTools-1.0.0/UniDockTools/unidock.py
-drwxr-xr-x   0 4294967294 4294967294        0 2023-08-02 03:18:17.486543 UniDockTools-1.0.0/UniDockTools.egg-info/
--rw-r--r--   0 4294967294 4294967294      332 2023-08-02 03:18:16.000000 UniDockTools-1.0.0/UniDockTools.egg-info/PKG-INFO
--rw-r--r--   0 4294967294 4294967294      500 2023-08-02 03:18:17.000000 UniDockTools-1.0.0/UniDockTools.egg-info/SOURCES.txt
--rw-r--r--   0 4294967294 4294967294        1 2023-08-02 03:18:16.000000 UniDockTools-1.0.0/UniDockTools.egg-info/dependency_links.txt
--rw-r--r--   0 4294967294 4294967294       54 2023-08-02 03:18:16.000000 UniDockTools-1.0.0/UniDockTools.egg-info/entry_points.txt
--rw-r--r--   0 4294967294 4294967294       15 2023-08-02 03:18:16.000000 UniDockTools-1.0.0/UniDockTools.egg-info/requires.txt
--rw-r--r--   0 4294967294 4294967294       13 2023-08-02 03:18:16.000000 UniDockTools-1.0.0/UniDockTools.egg-info/top_level.txt
--rw-r--r--   0 4294967294 4294967294      644 2023-08-02 02:58:30.000000 UniDockTools-1.0.0/setpu.py
--rw-r--r--   0 4294967294 4294967294       38 2023-08-02 03:18:17.691581 UniDockTools-1.0.0/setup.cfg
+drwxr-xr-x   0 4294967294 4294967294        0 2023-08-02 03:22:25.036104 UniDockTools-1.0.1/
+-rw-r--r--   0 4294967294 4294967294     1063 2023-08-02 02:58:30.000000 UniDockTools-1.0.1/LICENSE
+-rw-r--r--   0 4294967294 4294967294      253 2023-08-02 03:22:25.028379 UniDockTools-1.0.1/PKG-INFO
+-rw-r--r--   0 4294967294 4294967294      880 2023-08-02 02:58:30.000000 UniDockTools-1.0.1/README.md
+drwxr-xr-x   0 4294967294 4294967294        0 2023-08-02 03:22:24.775335 UniDockTools-1.0.1/UniDockTools/
+-rw-r--r--   0 4294967294 4294967294       28 2023-08-02 02:58:31.000000 UniDockTools-1.0.1/UniDockTools/__init__.py
+drwxr-xr-x   0 4294967294 4294967294        0 2023-08-02 03:22:25.003373 UniDockTools-1.0.1/UniDockTools/ligandPrepare/
+-rw-r--r--   0 4294967294 4294967294       92 2023-08-02 02:58:31.000000 UniDockTools-1.0.1/UniDockTools/ligandPrepare/__init__.py
+-rw-r--r--   0 4294967294 4294967294     2951 2023-08-02 02:58:31.000000 UniDockTools-1.0.1/UniDockTools/ligandPrepare/atom_type.py
+-rw-r--r--   0 4294967294 4294967294      924 2023-08-02 02:58:31.000000 UniDockTools-1.0.1/UniDockTools/ligandPrepare/rotatable_bond.py
+-rw-r--r--   0 4294967294 4294967294    19674 2023-08-02 02:58:31.000000 UniDockTools-1.0.1/UniDockTools/ligandPrepare/topology_builder.py
+-rw-r--r--   0 4294967294 4294967294     4987 2023-08-02 02:58:31.000000 UniDockTools-1.0.1/UniDockTools/ligandPrepare/utils.py
+-rw-r--r--   0 4294967294 4294967294    13477 2023-08-02 03:16:24.000000 UniDockTools-1.0.1/UniDockTools/unidock.py
+drwxr-xr-x   0 4294967294 4294967294        0 2023-08-02 03:22:24.900167 UniDockTools-1.0.1/UniDockTools.egg-info/
+-rw-r--r--   0 4294967294 4294967294      253 2023-08-02 03:22:23.000000 UniDockTools-1.0.1/UniDockTools.egg-info/PKG-INFO
+-rw-r--r--   0 4294967294 4294967294      500 2023-08-02 03:22:24.000000 UniDockTools-1.0.1/UniDockTools.egg-info/SOURCES.txt
+-rw-r--r--   0 4294967294 4294967294        1 2023-08-02 03:22:24.000000 UniDockTools-1.0.1/UniDockTools.egg-info/dependency_links.txt
+-rw-r--r--   0 4294967294 4294967294       54 2023-08-02 03:22:24.000000 UniDockTools-1.0.1/UniDockTools.egg-info/entry_points.txt
+-rw-r--r--   0 4294967294 4294967294       15 2023-08-02 03:22:24.000000 UniDockTools-1.0.1/UniDockTools.egg-info/requires.txt
+-rw-r--r--   0 4294967294 4294967294       13 2023-08-02 03:22:24.000000 UniDockTools-1.0.1/UniDockTools.egg-info/top_level.txt
+-rw-r--r--   0 4294967294 4294967294      565 2023-08-02 03:22:21.000000 UniDockTools-1.0.1/setpu.py
+-rw-r--r--   0 4294967294 4294967294       38 2023-08-02 03:22:25.040091 UniDockTools-1.0.1/setup.cfg
```

### Comparing `UniDockTools-1.0.0/LICENSE` & `UniDockTools-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `UniDockTools-1.0.0/README.md` & `UniDockTools-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `UniDockTools-1.0.0/UniDockTools/ligandPrepare/atom_type.py` & `UniDockTools-1.0.1/UniDockTools/ligandPrepare/atom_type.py`

 * *Files identical despite different names*

### Comparing `UniDockTools-1.0.0/UniDockTools/ligandPrepare/rotatable_bond.py` & `UniDockTools-1.0.1/UniDockTools/ligandPrepare/rotatable_bond.py`

 * *Files identical despite different names*

### Comparing `UniDockTools-1.0.0/UniDockTools/ligandPrepare/topology_builder.py` & `UniDockTools-1.0.1/UniDockTools/ligandPrepare/topology_builder.py`

 * *Files identical despite different names*

### Comparing `UniDockTools-1.0.0/UniDockTools/ligandPrepare/utils.py` & `UniDockTools-1.0.1/UniDockTools/ligandPrepare/utils.py`

 * *Files identical despite different names*

### Comparing `UniDockTools-1.0.0/UniDockTools/unidock.py` & `UniDockTools-1.0.1/UniDockTools/unidock.py`

 * *Files identical despite different names*

### Comparing `UniDockTools-1.0.0/setpu.py` & `UniDockTools-1.0.1/setpu.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 install_requires = ['rdkit', 'networkx']
 
 setup(
     name='UniDockTools',
-    version='1.0.0',
+    version='1.0.1',
     author='DP BayMax',
     url='https://github.com/UR-Free/UniDockTools',
-    description="A tools used for preprossing and postprocessing of UniDock, a GPU-accelerated molecular docking program developed by DP Technology",
+    description="A data processing tool for UniDock input and output",
     packages=find_packages(),
     install_requires=install_requires,
     include_package_data=True,
     
     package_data={
         "UniDock": ["data"],
     },
```


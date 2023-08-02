# Comparing `tmp/UniDockTools-1.0.2.tar.gz` & `tmp/UniDockTools-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UniDockTools-1.0.2.tar", last modified: Wed Aug  2 07:39:54 2023, max compression
+gzip compressed data, was "UniDockTools-1.0.3.tar", last modified: Wed Aug  2 07:56:50 2023, max compression
```

## Comparing `UniDockTools-1.0.2.tar` & `UniDockTools-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:39:54.244777 UniDockTools-1.0.2/
--rw-r--r--   0 root         (0) root         (0)     1063 2023-08-02 07:12:43.000000 UniDockTools-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      230 2023-08-02 07:39:54.240777 UniDockTools-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      880 2023-08-02 07:12:43.000000 UniDockTools-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:39:54.240777 UniDockTools-1.0.2/UniDock/
--rw-r--r--   0 root         (0) root         (0)       28 2023-08-02 07:12:43.000000 UniDockTools-1.0.2/UniDock/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:39:54.240777 UniDockTools-1.0.2/UniDock/ligandPrepare/
--rw-r--r--   0 root         (0) root         (0)       92 2023-08-02 07:12:43.000000 UniDockTools-1.0.2/UniDock/ligandPrepare/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2951 2023-08-02 07:12:43.000000 UniDockTools-1.0.2/UniDock/ligandPrepare/atom_type.py
--rw-r--r--   0 root         (0) root         (0)      924 2023-08-02 07:12:43.000000 UniDockTools-1.0.2/UniDock/ligandPrepare/rotatable_bond.py
--rw-r--r--   0 root         (0) root         (0)    19659 2023-08-02 07:12:43.000000 UniDockTools-1.0.2/UniDock/ligandPrepare/topology_builder.py
--rw-r--r--   0 root         (0) root         (0)     4987 2023-08-02 07:12:43.000000 UniDockTools-1.0.2/UniDock/ligandPrepare/utils.py
--rw-r--r--   0 root         (0) root         (0)    13395 2023-08-02 07:12:43.000000 UniDockTools-1.0.2/UniDock/unidock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:39:54.240777 UniDockTools-1.0.2/UniDockTools.egg-info/
--rw-r--r--   0 root         (0) root         (0)      230 2023-08-02 07:39:53.000000 UniDockTools-1.0.2/UniDockTools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      465 2023-08-02 07:39:54.000000 UniDockTools-1.0.2/UniDockTools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 07:39:53.000000 UniDockTools-1.0.2/UniDockTools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-08-02 07:39:53.000000 UniDockTools-1.0.2/UniDockTools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-08-02 07:39:53.000000 UniDockTools-1.0.2/UniDockTools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-08-02 07:39:54.000000 UniDockTools-1.0.2/UniDockTools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      570 2023-08-02 07:38:46.000000 UniDockTools-1.0.2/setpu.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-02 07:39:54.244777 UniDockTools-1.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:56:50.149735 UniDockTools-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-08-02 07:12:43.000000 UniDockTools-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      230 2023-08-02 07:56:50.149735 UniDockTools-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      880 2023-08-02 07:12:43.000000 UniDockTools-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:56:50.145735 UniDockTools-1.0.3/UniDock/
+-rw-r--r--   0 root         (0) root         (0)       28 2023-08-02 07:12:43.000000 UniDockTools-1.0.3/UniDock/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:56:50.145735 UniDockTools-1.0.3/UniDock/ligandPrepare/
+-rw-r--r--   0 root         (0) root         (0)       92 2023-08-02 07:12:43.000000 UniDockTools-1.0.3/UniDock/ligandPrepare/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2951 2023-08-02 07:12:43.000000 UniDockTools-1.0.3/UniDock/ligandPrepare/atom_type.py
+-rw-r--r--   0 root         (0) root         (0)      924 2023-08-02 07:12:43.000000 UniDockTools-1.0.3/UniDock/ligandPrepare/rotatable_bond.py
+-rw-r--r--   0 root         (0) root         (0)    19659 2023-08-02 07:12:43.000000 UniDockTools-1.0.3/UniDock/ligandPrepare/topology_builder.py
+-rw-r--r--   0 root         (0) root         (0)     4987 2023-08-02 07:12:43.000000 UniDockTools-1.0.3/UniDock/ligandPrepare/utils.py
+-rw-r--r--   0 root         (0) root         (0)    13395 2023-08-02 07:12:43.000000 UniDockTools-1.0.3/UniDock/unidock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:56:50.145735 UniDockTools-1.0.3/UniDockTools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      230 2023-08-02 07:56:49.000000 UniDockTools-1.0.3/UniDockTools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      465 2023-08-02 07:56:50.000000 UniDockTools-1.0.3/UniDockTools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 07:56:49.000000 UniDockTools-1.0.3/UniDockTools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-08-02 07:56:49.000000 UniDockTools-1.0.3/UniDockTools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-08-02 07:56:49.000000 UniDockTools-1.0.3/UniDockTools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-02 07:56:49.000000 UniDockTools-1.0.3/UniDockTools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-02 07:56:50.149735 UniDockTools-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      570 2023-08-02 07:56:12.000000 UniDockTools-1.0.3/setup.py
```

### Comparing `UniDockTools-1.0.2/LICENSE` & `UniDockTools-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `UniDockTools-1.0.2/README.md` & `UniDockTools-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `UniDockTools-1.0.2/UniDock/ligandPrepare/atom_type.py` & `UniDockTools-1.0.3/UniDock/ligandPrepare/atom_type.py`

 * *Files identical despite different names*

### Comparing `UniDockTools-1.0.2/UniDock/ligandPrepare/rotatable_bond.py` & `UniDockTools-1.0.3/UniDock/ligandPrepare/rotatable_bond.py`

 * *Files identical despite different names*

### Comparing `UniDockTools-1.0.2/UniDock/ligandPrepare/topology_builder.py` & `UniDockTools-1.0.3/UniDock/ligandPrepare/topology_builder.py`

 * *Files identical despite different names*

### Comparing `UniDockTools-1.0.2/UniDock/ligandPrepare/utils.py` & `UniDockTools-1.0.3/UniDock/ligandPrepare/utils.py`

 * *Files identical despite different names*

### Comparing `UniDockTools-1.0.2/UniDock/unidock.py` & `UniDockTools-1.0.3/UniDock/unidock.py`

 * *Files identical despite different names*

### Comparing `UniDockTools-1.0.2/setpu.py` & `UniDockTools-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 install_requires = ['rdkit', 'networkx']
 
 setup(
     name='UniDockTools',
-    version='1.0.2',
+    version='1.0.3',
     author='DP BayMax',
     description="UniDock, a GPU-accelerated molecular docking program developed by DP Technology",
     packages=find_packages(),
     install_requires=install_requires,
     include_package_data=True,
     #scripts=['UniDock/bin/unidock'],
     package_data={
```


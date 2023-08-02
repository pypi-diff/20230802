# Comparing `tmp/scibd-1.1.0.tar.gz` & `tmp/scibd-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scibd-1.1.0.tar", last modified: Wed Aug  2 03:25:32 2023, max compression
+gzip compressed data, was "scibd-1.2.0.tar", last modified: Wed Aug  2 06:04:38 2023, max compression
```

## Comparing `scibd-1.1.0.tar` & `scibd-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 yingwang  (1000) yingwang  (1000)        0 2023-08-02 03:25:32.000000 scibd-1.1.0/
--rw-r--r--   0 yingwang  (1000) yingwang  (1000)     1060 2023-01-18 09:22:20.000000 scibd-1.1.0/LICENSE
--rw-r--r--   0 yingwang  (1000) yingwang  (1000)       26 2023-01-18 09:22:20.000000 scibd-1.1.0/MANIFEST.in
--rw-r--r--   0 yingwang  (1000) yingwang  (1000)     2228 2023-08-02 03:25:32.000000 scibd-1.1.0/PKG-INFO
--rw-r--r--   0 yingwang  (1000) yingwang  (1000)     1537 2023-01-28 15:11:37.000000 scibd-1.1.0/README.md
--rw-r--r--   0 yingwang  (1000) yingwang  (1000)      238 2023-01-18 08:54:31.000000 scibd-1.1.0/README.rst
-drwxr-xr-x   0 yingwang  (1000) yingwang  (1000)        0 2023-08-02 03:25:32.000000 scibd-1.1.0/scibd/
--rw-r--r--   0 yingwang  (1000) yingwang  (1000)       21 2023-01-18 09:34:52.000000 scibd-1.1.0/scibd/__init__.py
--rw-r--r--   0 yingwang  (1000) yingwang  (1000)      352 2023-01-18 09:33:16.000000 scibd-1.1.0/scibd/__version__.py
--rw-r--r--   0 yingwang  (1000) yingwang  (1000)    30376 2023-08-02 03:24:20.000000 scibd-1.1.0/scibd/scibd.py
-drwxr-xr-x   0 yingwang  (1000) yingwang  (1000)        0 2023-08-02 03:25:32.000000 scibd-1.1.0/scibd.egg-info/
--rw-r--r--   0 yingwang  (1000) yingwang  (1000)     2228 2023-08-02 03:25:32.000000 scibd-1.1.0/scibd.egg-info/PKG-INFO
--rw-r--r--   0 yingwang  (1000) yingwang  (1000)      219 2023-08-02 03:25:32.000000 scibd-1.1.0/scibd.egg-info/SOURCES.txt
--rw-r--r--   0 yingwang  (1000) yingwang  (1000)        1 2023-08-02 03:25:32.000000 scibd-1.1.0/scibd.egg-info/dependency_links.txt
--rw-r--r--   0 yingwang  (1000) yingwang  (1000)        6 2023-08-02 03:25:32.000000 scibd-1.1.0/scibd.egg-info/top_level.txt
--rw-r--r--   0 yingwang  (1000) yingwang  (1000)       38 2023-08-02 03:25:32.000000 scibd-1.1.0/setup.cfg
--rw-r--r--   0 yingwang  (1000) yingwang  (1000)     5217 2023-08-02 03:25:12.000000 scibd-1.1.0/setup.py
+drwxr-xr-x   0 yingwang  (1000) yingwang  (1000)        0 2023-08-02 06:04:38.610694 scibd-1.2.0/
+-rw-r--r--   0 yingwang  (1000) yingwang  (1000)     1060 2023-01-18 09:22:20.000000 scibd-1.2.0/LICENSE
+-rw-r--r--   0 yingwang  (1000) yingwang  (1000)       26 2023-01-18 09:22:20.000000 scibd-1.2.0/MANIFEST.in
+-rw-r--r--   0 yingwang  (1000) yingwang  (1000)     2208 2023-08-02 06:04:38.610694 scibd-1.2.0/PKG-INFO
+-rw-r--r--   0 yingwang  (1000) yingwang  (1000)     1537 2023-01-28 15:11:37.000000 scibd-1.2.0/README.md
+-rw-r--r--   0 yingwang  (1000) yingwang  (1000)      238 2023-01-18 08:54:31.000000 scibd-1.2.0/README.rst
+drwxr-xr-x   0 yingwang  (1000) yingwang  (1000)        0 2023-08-02 06:04:38.610694 scibd-1.2.0/scibd/
+-rw-r--r--   0 yingwang  (1000) yingwang  (1000)       21 2023-01-18 09:34:52.000000 scibd-1.2.0/scibd/__init__.py
+-rw-r--r--   0 yingwang  (1000) yingwang  (1000)      352 2023-01-18 09:33:16.000000 scibd-1.2.0/scibd/__version__.py
+-rw-r--r--   0 yingwang  (1000) yingwang  (1000)    30380 2023-08-02 06:03:09.000000 scibd-1.2.0/scibd/scibd.py
+drwxr-xr-x   0 yingwang  (1000) yingwang  (1000)        0 2023-08-02 06:04:38.610694 scibd-1.2.0/scibd.egg-info/
+-rw-r--r--   0 yingwang  (1000) yingwang  (1000)     2208 2023-08-02 06:04:38.000000 scibd-1.2.0/scibd.egg-info/PKG-INFO
+-rw-r--r--   0 yingwang  (1000) yingwang  (1000)      219 2023-08-02 06:04:38.000000 scibd-1.2.0/scibd.egg-info/SOURCES.txt
+-rw-r--r--   0 yingwang  (1000) yingwang  (1000)        1 2023-08-02 06:04:38.000000 scibd-1.2.0/scibd.egg-info/dependency_links.txt
+-rw-r--r--   0 yingwang  (1000) yingwang  (1000)        6 2023-08-02 06:04:38.000000 scibd-1.2.0/scibd.egg-info/top_level.txt
+-rw-r--r--   0 yingwang  (1000) yingwang  (1000)       38 2023-08-02 06:04:38.610694 scibd-1.2.0/setup.cfg
+-rw-r--r--   0 yingwang  (1000) yingwang  (1000)     5217 2023-08-02 06:04:28.000000 scibd-1.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `scibd-1.1.0/LICENSE` & `scibd-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scibd-1.1.0/PKG-INFO` & `scibd-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: scibd
-Version: 1.1.0
+Version: 1.2.0
 Summary: A doublet detetion tool for scCAS data. https://github.com/Ying-Lab/scIBD
 Home-page: https://github.com/Ying-Lab/scIBD/
 Author: Wenhao Zhang
 Author-email: zscotty@stu.xmu.edu.cn
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8.0
@@ -70,9 +69,7 @@
 
 n_tree: The number of trees in KNN constrcution, default is 30.
 
 
 
 
 
-
-
```

### Comparing `scibd-1.1.0/README.md` & `scibd-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `scibd-1.1.0/scibd/scibd.py` & `scibd-1.2.0/scibd/scibd.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,16 +239,16 @@
 
 
 #     sim_set = GetSparseUnion(single1set,single2set)
     sim_set = (single1set + single2set).astype(np.uint8)
 
 #     sim_set = scipy.sparse.csr_matrix(single1set|single2set)
 #     simulatelabel = np.array(simulatelabel)
-    print(simulate_size,'Doublets Construction Done!')
-    print(sim_set.shape)
+#     print(simulate_size,'Doublets Construction Done!')
+#     print(sim_set.shape)
     return sim_set
 
 
 
 
 def Splitmat(matsize,ncore):
     idx_set =[]
```

### Comparing `scibd-1.1.0/scibd.egg-info/PKG-INFO` & `scibd-1.2.0/scibd.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: scibd
-Version: 1.1.0
+Version: 1.2.0
 Summary: A doublet detetion tool for scCAS data. https://github.com/Ying-Lab/scIBD
 Home-page: https://github.com/Ying-Lab/scIBD/
 Author: Wenhao Zhang
 Author-email: zscotty@stu.xmu.edu.cn
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8.0
@@ -70,9 +69,7 @@
 
 n_tree: The number of trees in KNN constrcution, default is 30.
 
 
 
 
 
-
-
```

### Comparing `scibd-1.1.0/setup.py` & `scibd-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 # Package meta-data.
 NAME = 'scibd'
 DESCRIPTION = 'A doublet detetion tool for scCAS data. https://github.com/Ying-Lab/scIBD'
 URL = 'https://github.com/Ying-Lab/scIBD/'
 EMAIL = 'zscotty@stu.xmu.edu.cn'
 AUTHOR = 'Wenhao Zhang'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '1.1.0'
+VERSION = '1.2.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```


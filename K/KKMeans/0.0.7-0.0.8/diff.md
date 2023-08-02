# Comparing `tmp/KKMeans-0.0.7.tar.gz` & `tmp/KKMeans-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KKMeans-0.0.7.tar", last modified: Wed Aug  2 10:33:07 2023, max compression
+gzip compressed data, was "KKMeans-0.0.8.tar", last modified: Wed Aug  2 10:58:41 2023, max compression
```

## Comparing `KKMeans-0.0.7.tar` & `KKMeans-0.0.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 10:33:07.037694 KKMeans-0.0.7/
-drwxrwxrwx   0        0        0        0 2023-08-02 10:33:07.001921 KKMeans-0.0.7/KKMeans.egg-info/
--rw-rw-rw-   0        0        0     1171 2023-08-02 10:33:06.000000 KKMeans-0.0.7/KKMeans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      639 2023-08-02 10:33:06.000000 KKMeans-0.0.7/KKMeans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 10:33:06.000000 KKMeans-0.0.7/KKMeans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-08-02 10:33:06.000000 KKMeans-0.0.7/KKMeans.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-08-02 10:33:06.000000 KKMeans-0.0.7/KKMeans.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1171 2023-08-02 10:33:07.037180 KKMeans-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      778 2023-08-01 21:43:50.000000 KKMeans-0.0.7/README.md
--rw-rw-rw-   0        0        0     1086 2023-07-31 11:30:04.000000 KKMeans-0.0.7/license.txt
--rw-rw-rw-   0        0        0      521 2023-08-02 10:30:04.000000 KKMeans-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-02 10:33:07.037694 KKMeans-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1663 2023-07-31 12:13:21.000000 KKMeans-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 10:33:06.977872 KKMeans-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-08-02 10:33:07.029512 KKMeans-0.0.7/src/KKMeans/
--rw-rw-rw-   0        0        0   875796 2023-08-02 10:32:14.000000 KKMeans-0.0.7/src/KKMeans/KKMeans.c
--rw-rw-rw-   0        0        0    27233 2023-08-01 21:49:50.000000 KKMeans-0.0.7/src/KKMeans/KKMeans.py
--rw-rw-rw-   0        0        0      122 2023-08-01 18:06:49.000000 KKMeans-0.0.7/src/KKMeans/__init__.py
--rw-rw-rw-   0        0        0  1171323 2023-08-02 10:33:04.000000 KKMeans-0.0.7/src/KKMeans/elkan.c
--rw-rw-rw-   0        0        0    10024 2023-08-02 10:32:48.000000 KKMeans-0.0.7/src/KKMeans/elkan.pyx
--rw-rw-rw-   0        0        0  1182482 2023-08-02 10:33:05.000000 KKMeans-0.0.7/src/KKMeans/kernels.c
--rw-rw-rw-   0        0        0     6892 2023-08-01 21:47:36.000000 KKMeans-0.0.7/src/KKMeans/kernels.pyx
--rw-rw-rw-   0        0        0  1022804 2023-08-02 10:33:05.000000 KKMeans-0.0.7/src/KKMeans/lloyd.c
--rw-rw-rw-   0        0        0     3427 2023-08-01 21:47:44.000000 KKMeans-0.0.7/src/KKMeans/lloyd.pyx
--rw-rw-rw-   0        0        0  1004899 2023-07-31 11:50:00.000000 KKMeans-0.0.7/src/KKMeans/quality.c
--rw-rw-rw-   0        0        0     1966 2023-07-31 11:38:16.000000 KKMeans-0.0.7/src/KKMeans/quality.pyx
--rw-rw-rw-   0        0        0  1091357 2023-08-02 10:33:06.000000 KKMeans-0.0.7/src/KKMeans/utils.c
--rw-rw-rw-   0        0        0     5309 2023-08-01 18:03:59.000000 KKMeans-0.0.7/src/KKMeans/utils.pyx
-drwxrwxrwx   0        0        0        0 2023-08-02 10:33:07.035641 KKMeans-0.0.7/tests/
--rw-rw-rw-   0        0        0     1504 2023-08-01 21:50:30.000000 KKMeans-0.0.7/tests/test_pytest_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:58:41.751382 KKMeans-0.0.8/
+drwxrwxrwx   0        0        0        0 2023-08-02 10:58:41.723112 KKMeans-0.0.8/KKMeans.egg-info/
+-rw-rw-rw-   0        0        0     1106 2023-08-02 10:58:41.000000 KKMeans-0.0.8/KKMeans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      639 2023-08-02 10:58:41.000000 KKMeans-0.0.8/KKMeans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 10:58:41.000000 KKMeans-0.0.8/KKMeans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-08-02 10:58:41.000000 KKMeans-0.0.8/KKMeans.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-02 10:58:41.000000 KKMeans-0.0.8/KKMeans.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1106 2023-08-02 10:58:41.750873 KKMeans-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      713 2023-08-02 10:58:04.000000 KKMeans-0.0.8/README.md
+-rw-rw-rw-   0        0        0     1086 2023-07-31 11:30:04.000000 KKMeans-0.0.8/license.txt
+-rw-rw-rw-   0        0        0      521 2023-08-02 10:58:12.000000 KKMeans-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-02 10:58:41.751382 KKMeans-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1663 2023-07-31 12:13:21.000000 KKMeans-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:58:41.705163 KKMeans-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-08-02 10:58:41.748838 KKMeans-0.0.8/src/KKMeans/
+-rw-rw-rw-   0        0        0   875796 2023-08-02 10:32:14.000000 KKMeans-0.0.8/src/KKMeans/KKMeans.c
+-rw-rw-rw-   0        0        0    27233 2023-08-01 21:49:50.000000 KKMeans-0.0.8/src/KKMeans/KKMeans.py
+-rw-rw-rw-   0        0        0      122 2023-08-01 18:06:49.000000 KKMeans-0.0.8/src/KKMeans/__init__.py
+-rw-rw-rw-   0        0        0  1171323 2023-08-02 10:58:40.000000 KKMeans-0.0.8/src/KKMeans/elkan.c
+-rw-rw-rw-   0        0        0    10024 2023-08-02 10:32:48.000000 KKMeans-0.0.8/src/KKMeans/elkan.pyx
+-rw-rw-rw-   0        0        0  1182482 2023-08-02 10:58:40.000000 KKMeans-0.0.8/src/KKMeans/kernels.c
+-rw-rw-rw-   0        0        0     6892 2023-08-01 21:47:36.000000 KKMeans-0.0.8/src/KKMeans/kernels.pyx
+-rw-rw-rw-   0        0        0  1022804 2023-08-02 10:33:05.000000 KKMeans-0.0.8/src/KKMeans/lloyd.c
+-rw-rw-rw-   0        0        0     3427 2023-08-01 21:47:44.000000 KKMeans-0.0.8/src/KKMeans/lloyd.pyx
+-rw-rw-rw-   0        0        0  1004899 2023-07-31 11:50:00.000000 KKMeans-0.0.8/src/KKMeans/quality.c
+-rw-rw-rw-   0        0        0     1966 2023-07-31 11:38:16.000000 KKMeans-0.0.8/src/KKMeans/quality.pyx
+-rw-rw-rw-   0        0        0  1091357 2023-08-02 10:33:06.000000 KKMeans-0.0.8/src/KKMeans/utils.c
+-rw-rw-rw-   0        0        0     5309 2023-08-01 18:03:59.000000 KKMeans-0.0.8/src/KKMeans/utils.pyx
+drwxrwxrwx   0        0        0        0 2023-08-02 10:58:41.749855 KKMeans-0.0.8/tests/
+-rw-rw-rw-   0        0        0     1504 2023-08-01 21:50:30.000000 KKMeans-0.0.8/tests/test_pytest_utils.py
```

### Comparing `KKMeans-0.0.7/KKMeans.egg-info/PKG-INFO` & `KKMeans-0.0.8/KKMeans.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: KKMeans
-Version: 0.0.7
+Version: 0.0.8
 Summary: https://github.com/bauxn/kernel-kmeans. openMP is not enabled when installing via PiPy
 Author-email: Paul Theis <keymailt7@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: license.txt
 
-This is the github repository for my bachelor thesis.<br>
-<br>
 simple installation via "pip install KKMeans" <br>
 <br>
 To enable openMP, clone the project and open setup.py, you will find a list compile_args. The dcython argument prevents cython from transpling the assertions to c (-> do not remove).
 Add whatever arguments your compiler needs to compile with openMP (and all other args you like). <br>
 There are default arguments for msvc and gcc listed. <br>
 <br>
 When finished editing setup.py (or being content without openMP), install with "pip install ." in the root directory (the same where setup.py resides) <br>
```

### Comparing `KKMeans-0.0.7/KKMeans.egg-info/SOURCES.txt` & `KKMeans-0.0.8/KKMeans.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.7/PKG-INFO` & `KKMeans-0.0.8/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: KKMeans
-Version: 0.0.7
+Version: 0.0.8
 Summary: https://github.com/bauxn/kernel-kmeans. openMP is not enabled when installing via PiPy
 Author-email: Paul Theis <keymailt7@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: license.txt
 
-This is the github repository for my bachelor thesis.<br>
-<br>
 simple installation via "pip install KKMeans" <br>
 <br>
 To enable openMP, clone the project and open setup.py, you will find a list compile_args. The dcython argument prevents cython from transpling the assertions to c (-> do not remove).
 Add whatever arguments your compiler needs to compile with openMP (and all other args you like). <br>
 There are default arguments for msvc and gcc listed. <br>
 <br>
 When finished editing setup.py (or being content without openMP), install with "pip install ." in the root directory (the same where setup.py resides) <br>
```

### Comparing `KKMeans-0.0.7/README.md` & `KKMeans-0.0.8/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-This is the github repository for my bachelor thesis.<br>
-<br>
 simple installation via "pip install KKMeans" <br>
 <br>
 To enable openMP, clone the project and open setup.py, you will find a list compile_args. The dcython argument prevents cython from transpling the assertions to c (-> do not remove).
 Add whatever arguments your compiler needs to compile with openMP (and all other args you like). <br>
 There are default arguments for msvc and gcc listed. <br>
 <br>
 When finished editing setup.py (or being content without openMP), install with "pip install ." in the root directory (the same where setup.py resides) <br>
```

### Comparing `KKMeans-0.0.7/license.txt` & `KKMeans-0.0.8/license.txt`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.7/pyproject.toml` & `KKMeans-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=63", "wheel", "Cython"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "KKMeans"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Paul Theis", email="keymailt7@gmail.com" },
 ]
 dependencies = ["numpy>=1.25"]
 description = "https://github.com/bauxn/kernel-kmeans. openMP is not enabled when installing via PiPy"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `KKMeans-0.0.7/setup.py` & `KKMeans-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.7/src/KKMeans/KKMeans.c` & `KKMeans-0.0.8/src/KKMeans/KKMeans.c`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.7/src/KKMeans/KKMeans.py` & `KKMeans-0.0.8/src/KKMeans/KKMeans.py`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.7/src/KKMeans/elkan.c` & `KKMeans-0.0.8/src/KKMeans/elkan.c`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.7/src/KKMeans/elkan.pyx` & `KKMeans-0.0.8/src/KKMeans/elkan.pyx`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.7/src/KKMeans/kernels.c` & `KKMeans-0.0.8/src/KKMeans/kernels.c`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.7/src/KKMeans/kernels.pyx` & `KKMeans-0.0.8/src/KKMeans/kernels.pyx`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.7/src/KKMeans/lloyd.c` & `KKMeans-0.0.8/src/KKMeans/lloyd.c`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.7/src/KKMeans/lloyd.pyx` & `KKMeans-0.0.8/src/KKMeans/lloyd.pyx`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.7/src/KKMeans/quality.c` & `KKMeans-0.0.8/src/KKMeans/quality.c`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.7/src/KKMeans/quality.pyx` & `KKMeans-0.0.8/src/KKMeans/quality.pyx`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.7/src/KKMeans/utils.c` & `KKMeans-0.0.8/src/KKMeans/utils.c`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.7/src/KKMeans/utils.pyx` & `KKMeans-0.0.8/src/KKMeans/utils.pyx`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.7/tests/test_pytest_utils.py` & `KKMeans-0.0.8/tests/test_pytest_utils.py`

 * *Files identical despite different names*


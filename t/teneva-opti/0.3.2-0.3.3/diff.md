# Comparing `tmp/teneva_opti-0.3.2.tar.gz` & `tmp/teneva_opti-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teneva_opti-0.3.2.tar", last modified: Wed Aug  2 19:04:18 2023, max compression
+gzip compressed data, was "teneva_opti-0.3.3.tar", last modified: Wed Aug  2 19:32:13 2023, max compression
```

## Comparing `teneva_opti-0.3.2.tar` & `teneva_opti-0.3.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-02 19:04:18.102633 teneva_opti-0.3.2/
--rw-r--r--   0 andrei     (501) staff       (20)     1090 2023-02-25 19:48:03.000000 teneva_opti-0.3.2/LICENSE.txt
--rw-r--r--   0 andrei     (501) staff       (20)       79 2023-07-27 15:33:45.000000 teneva_opti-0.3.2/MANIFEST.in
--rw-r--r--   0 andrei     (501) staff       (20)     3198 2023-08-02 19:04:18.102891 teneva_opti-0.3.2/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)     1923 2023-08-02 19:04:05.000000 teneva_opti-0.3.2/README.md
--rw-r--r--   0 andrei     (501) staff       (20)     1244 2023-08-02 16:02:49.000000 teneva_opti-0.3.2/demo.py
--rw-r--r--   0 andrei     (501) staff       (20)       95 2023-08-02 12:48:02.000000 teneva_opti-0.3.2/requirements.txt
--rw-r--r--   0 andrei     (501) staff       (20)      107 2023-08-02 19:04:18.103697 teneva_opti-0.3.2/setup.cfg
--rw-r--r--   0 andrei     (501) staff       (20)     2538 2023-08-02 09:28:28.000000 teneva_opti-0.3.2/setup.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-02 19:04:18.091316 teneva_opti-0.3.2/teneva_opti/
--rw-r--r--   0 andrei     (501) staff       (20)      191 2023-08-02 19:04:01.000000 teneva_opti-0.3.2/teneva_opti/__init__.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-02 19:04:18.094697 teneva_opti-0.3.2/teneva_opti/func/
--rw-r--r--   0 andrei     (501) staff       (20)        0 2023-07-31 13:03:34.000000 teneva_opti-0.3.2/teneva_opti/func/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     6295 2023-08-02 16:22:44.000000 teneva_opti-0.3.2/teneva_opti/opti.py
--rw-r--r--   0 andrei     (501) staff       (20)      113 2023-07-31 13:44:41.000000 teneva_opti-0.3.2/teneva_opti/opti_func.py
--rw-r--r--   0 andrei     (501) staff       (20)     2442 2023-08-02 19:03:37.000000 teneva_opti-0.3.2/teneva_opti/opti_manager.py
--rw-r--r--   0 andrei     (501) staff       (20)     1043 2023-08-02 15:52:07.000000 teneva_opti-0.3.2/teneva_opti/opti_tens.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-02 19:04:18.101884 teneva_opti-0.3.2/teneva_opti/tens/
--rw-r--r--   0 andrei     (501) staff       (20)      344 2023-08-01 16:02:13.000000 teneva_opti-0.3.2/teneva_opti/tens/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)      391 2023-08-01 15:57:41.000000 teneva_opti-0.3.2/teneva_opti/tens/opti_tens_nb.py
--rw-r--r--   0 andrei     (501) staff       (20)      391 2023-08-01 15:57:39.000000 teneva_opti-0.3.2/teneva_opti/tens/opti_tens_opo.py
--rw-r--r--   0 andrei     (501) staff       (20)     1129 2023-08-02 14:22:34.000000 teneva_opti-0.3.2/teneva_opti/tens/opti_tens_optimatt.py
--rw-r--r--   0 andrei     (501) staff       (20)      401 2023-08-01 15:57:37.000000 teneva_opti-0.3.2/teneva_opti/tens/opti_tens_portfolio.py
--rw-r--r--   0 andrei     (501) staff       (20)     2090 2023-08-02 14:22:10.000000 teneva_opti-0.3.2/teneva_opti/tens/opti_tens_protes.py
--rw-r--r--   0 andrei     (501) staff       (20)      377 2023-08-01 15:57:35.000000 teneva_opti-0.3.2/teneva_opti/tens/opti_tens_pso.py
--rw-r--r--   0 andrei     (501) staff       (20)      381 2023-08-01 15:57:33.000000 teneva_opti-0.3.2/teneva_opti/tens/opti_tens_spsa.py
--rw-r--r--   0 andrei     (501) staff       (20)     1289 2023-08-02 14:22:01.000000 teneva_opti-0.3.2/teneva_opti/tens/opti_tens_ttopt.py
--rw-r--r--   0 andrei     (501) staff       (20)     2367 2023-08-02 13:40:17.000000 teneva_opti-0.3.2/teneva_opti/utils.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-02 19:04:18.094132 teneva_opti-0.3.2/teneva_opti.egg-info/
--rw-r--r--   0 andrei     (501) staff       (20)     3198 2023-08-02 19:04:17.000000 teneva_opti-0.3.2/teneva_opti.egg-info/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)      740 2023-08-02 19:04:18.000000 teneva_opti-0.3.2/teneva_opti.egg-info/SOURCES.txt
--rw-r--r--   0 andrei     (501) staff       (20)        1 2023-08-02 19:04:17.000000 teneva_opti-0.3.2/teneva_opti.egg-info/dependency_links.txt
--rw-r--r--   0 andrei     (501) staff       (20)       95 2023-08-02 19:04:17.000000 teneva_opti-0.3.2/teneva_opti.egg-info/requires.txt
--rw-r--r--   0 andrei     (501) staff       (20)       12 2023-08-02 19:04:17.000000 teneva_opti-0.3.2/teneva_opti.egg-info/top_level.txt
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-02 19:32:13.059709 teneva_opti-0.3.3/
+-rw-r--r--   0 andrei     (501) staff       (20)     1090 2023-02-25 19:48:03.000000 teneva_opti-0.3.3/LICENSE.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       79 2023-07-27 15:33:45.000000 teneva_opti-0.3.3/MANIFEST.in
+-rw-r--r--   0 andrei     (501) staff       (20)     3198 2023-08-02 19:32:13.059913 teneva_opti-0.3.3/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)     1923 2023-08-02 19:32:03.000000 teneva_opti-0.3.3/README.md
+-rw-r--r--   0 andrei     (501) staff       (20)     1244 2023-08-02 16:02:49.000000 teneva_opti-0.3.3/demo.py
+-rw-r--r--   0 andrei     (501) staff       (20)      137 2023-08-02 19:19:40.000000 teneva_opti-0.3.3/requirements.txt
+-rw-r--r--   0 andrei     (501) staff       (20)      107 2023-08-02 19:32:13.060403 teneva_opti-0.3.3/setup.cfg
+-rw-r--r--   0 andrei     (501) staff       (20)     2538 2023-08-02 09:28:28.000000 teneva_opti-0.3.3/setup.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-02 19:32:13.051117 teneva_opti-0.3.3/teneva_opti/
+-rw-r--r--   0 andrei     (501) staff       (20)      191 2023-08-02 19:31:58.000000 teneva_opti-0.3.3/teneva_opti/__init__.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-02 19:32:13.053841 teneva_opti-0.3.3/teneva_opti/func/
+-rw-r--r--   0 andrei     (501) staff       (20)        0 2023-07-31 13:03:34.000000 teneva_opti-0.3.3/teneva_opti/func/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     6277 2023-08-02 19:31:20.000000 teneva_opti-0.3.3/teneva_opti/opti.py
+-rw-r--r--   0 andrei     (501) staff       (20)      113 2023-07-31 13:44:41.000000 teneva_opti-0.3.3/teneva_opti/opti_func.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2442 2023-08-02 19:03:37.000000 teneva_opti-0.3.3/teneva_opti/opti_manager.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1043 2023-08-02 15:52:07.000000 teneva_opti-0.3.3/teneva_opti/opti_tens.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-02 19:32:13.059063 teneva_opti-0.3.3/teneva_opti/tens/
+-rw-r--r--   0 andrei     (501) staff       (20)      344 2023-08-01 16:02:13.000000 teneva_opti-0.3.3/teneva_opti/tens/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)      391 2023-08-01 15:57:41.000000 teneva_opti-0.3.3/teneva_opti/tens/opti_tens_nb.py
+-rw-r--r--   0 andrei     (501) staff       (20)      391 2023-08-01 15:57:39.000000 teneva_opti-0.3.3/teneva_opti/tens/opti_tens_opo.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1129 2023-08-02 14:22:34.000000 teneva_opti-0.3.3/teneva_opti/tens/opti_tens_optimatt.py
+-rw-r--r--   0 andrei     (501) staff       (20)      401 2023-08-01 15:57:37.000000 teneva_opti-0.3.3/teneva_opti/tens/opti_tens_portfolio.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2090 2023-08-02 14:22:10.000000 teneva_opti-0.3.3/teneva_opti/tens/opti_tens_protes.py
+-rw-r--r--   0 andrei     (501) staff       (20)      377 2023-08-01 15:57:35.000000 teneva_opti-0.3.3/teneva_opti/tens/opti_tens_pso.py
+-rw-r--r--   0 andrei     (501) staff       (20)      381 2023-08-01 15:57:33.000000 teneva_opti-0.3.3/teneva_opti/tens/opti_tens_spsa.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1289 2023-08-02 14:22:01.000000 teneva_opti-0.3.3/teneva_opti/tens/opti_tens_ttopt.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2367 2023-08-02 13:40:17.000000 teneva_opti-0.3.3/teneva_opti/utils.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-02 19:32:13.053425 teneva_opti-0.3.3/teneva_opti.egg-info/
+-rw-r--r--   0 andrei     (501) staff       (20)     3198 2023-08-02 19:32:12.000000 teneva_opti-0.3.3/teneva_opti.egg-info/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)      740 2023-08-02 19:32:12.000000 teneva_opti-0.3.3/teneva_opti.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        1 2023-08-02 19:32:12.000000 teneva_opti-0.3.3/teneva_opti.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei     (501) staff       (20)      137 2023-08-02 19:32:12.000000 teneva_opti-0.3.3/teneva_opti.egg-info/requires.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       12 2023-08-02 19:32:12.000000 teneva_opti-0.3.3/teneva_opti.egg-info/top_level.txt
```

### Comparing `teneva_opti-0.3.2/LICENSE.txt` & `teneva_opti-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.3.2/PKG-INFO` & `teneva_opti-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teneva_opti
-Version: 0.3.2
+Version: 0.3.3
 Summary: Collection of various optimization methods, including tensor based, for multivariate functions and multidimensional data arrays
 Home-page: https://github.com/AndreiChertkov/teneva_opti
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AndreiChertkov/teneva_opti
 Keywords: optimization method multidimensional array multivariate function tensor train nevergrad cma ttopt protes genetic algorithm evolutionary strategy
@@ -30,15 +30,15 @@
 ## Description
 
 Collection of various optimization methods (search for the global minimum and/or maximum) for multivariate functions and multidimensional data arrays (tensors). This library is based on a software product [teneva](https://github.com/AndreiChertkov/teneva). See also related benchmarks library [teneva_bm](https://github.com/AndreiChertkov/teneva_bm).
 
 
 ## Installation
 
-> Current version "0.3.2".
+> Current version "0.3.3".
 
 The package can be installed via pip: `pip install teneva_opti` (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9). It can be also downloaded from the repository [teneva_opti](https://github.com/AndreiChertkov/teneva_opti) and installed by `python setup.py install` command from the root folder of the project.
 
 We test optimizers with benchmarks from [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) library. For installation of additional dependencies (`gym` and `mujoco`) for `agent` collection , please, do the following (for existing conda environment `teneva_opti`; if you are using a different environment name, then please make the appropriate substitution in the script):
 ```bash
 wget https://raw.githubusercontent.com/AndreiChertkov/teneva_bm/main/install_mujoco.py && python install_mujoco.py --env teneva_opti && rm install_mujoco.py
 ```
```

### Comparing `teneva_opti-0.3.2/README.md` & `teneva_opti-0.3.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ## Description
 
 Collection of various optimization methods (search for the global minimum and/or maximum) for multivariate functions and multidimensional data arrays (tensors). This library is based on a software product [teneva](https://github.com/AndreiChertkov/teneva). See also related benchmarks library [teneva_bm](https://github.com/AndreiChertkov/teneva_bm).
 
 
 ## Installation
 
-> Current version "0.3.2".
+> Current version "0.3.3".
 
 The package can be installed via pip: `pip install teneva_opti` (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9). It can be also downloaded from the repository [teneva_opti](https://github.com/AndreiChertkov/teneva_opti) and installed by `python setup.py install` command from the root folder of the project.
 
 We test optimizers with benchmarks from [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) library. For installation of additional dependencies (`gym` and `mujoco`) for `agent` collection , please, do the following (for existing conda environment `teneva_opti`; if you are using a different environment name, then please make the appropriate substitution in the script):
 ```bash
 wget https://raw.githubusercontent.com/AndreiChertkov/teneva_bm/main/install_mujoco.py && python install_mujoco.py --env teneva_opti && rm install_mujoco.py
 ```
```

### Comparing `teneva_opti-0.3.2/demo.py` & `teneva_opti-0.3.3/demo.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.3.2/setup.py` & `teneva_opti-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.3.2/teneva_opti/opti.py` & `teneva_opti-0.3.3/teneva_opti/opti.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                 raise ValueError('Invalid BM configuration ("with_cache")')
         else:
             self.bm.set_cache(with_cache)
             self.bm.set_budget(m, m_cache=m)
             self.bm.prep()
 
         self.log = Log(self.fpath('log') if log_file else None, log, log_info)
-        self.bm.set_log(self.log if log else False, prefix=self.name,
+        self.bm.set_log(self.log, prefix=self.name,
             cond=('max' if self.is_max else 'min'),
             with_max=self.is_max, with_min=not self.is_max)
 
         self.is_fail = False
 
         self.set_opts()
```

### Comparing `teneva_opti-0.3.2/teneva_opti/opti_manager.py` & `teneva_opti-0.3.3/teneva_opti/opti_manager.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.3.2/teneva_opti/opti_tens.py` & `teneva_opti-0.3.3/teneva_opti/opti_tens.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.3.2/teneva_opti/tens/opti_tens_optimatt.py` & `teneva_opti-0.3.3/teneva_opti/tens/opti_tens_optimatt.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.3.2/teneva_opti/tens/opti_tens_protes.py` & `teneva_opti-0.3.3/teneva_opti/tens/opti_tens_protes.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.3.2/teneva_opti/tens/opti_tens_ttopt.py` & `teneva_opti-0.3.3/teneva_opti/tens/opti_tens_ttopt.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.3.2/teneva_opti/utils.py` & `teneva_opti-0.3.3/teneva_opti/utils.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.3.2/teneva_opti.egg-info/PKG-INFO` & `teneva_opti-0.3.3/teneva_opti.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teneva-opti
-Version: 0.3.2
+Version: 0.3.3
 Summary: Collection of various optimization methods, including tensor based, for multivariate functions and multidimensional data arrays
 Home-page: https://github.com/AndreiChertkov/teneva_opti
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AndreiChertkov/teneva_opti
 Keywords: optimization method multidimensional array multivariate function tensor train nevergrad cma ttopt protes genetic algorithm evolutionary strategy
@@ -30,15 +30,15 @@
 ## Description
 
 Collection of various optimization methods (search for the global minimum and/or maximum) for multivariate functions and multidimensional data arrays (tensors). This library is based on a software product [teneva](https://github.com/AndreiChertkov/teneva). See also related benchmarks library [teneva_bm](https://github.com/AndreiChertkov/teneva_bm).
 
 
 ## Installation
 
-> Current version "0.3.2".
+> Current version "0.3.3".
 
 The package can be installed via pip: `pip install teneva_opti` (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9). It can be also downloaded from the repository [teneva_opti](https://github.com/AndreiChertkov/teneva_opti) and installed by `python setup.py install` command from the root folder of the project.
 
 We test optimizers with benchmarks from [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) library. For installation of additional dependencies (`gym` and `mujoco`) for `agent` collection , please, do the following (for existing conda environment `teneva_opti`; if you are using a different environment name, then please make the appropriate substitution in the script):
 ```bash
 wget https://raw.githubusercontent.com/AndreiChertkov/teneva_bm/main/install_mujoco.py && python install_mujoco.py --env teneva_opti && rm install_mujoco.py
 ```
```

### Comparing `teneva_opti-0.3.2/teneva_opti.egg-info/SOURCES.txt` & `teneva_opti-0.3.3/teneva_opti.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/teneva_opti-0.2.0.tar.gz` & `tmp/teneva_opti-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teneva_opti-0.2.0.tar", last modified: Tue Aug  1 16:21:12 2023, max compression
+gzip compressed data, was "teneva_opti-0.3.0.tar", last modified: Wed Aug  2 16:25:30 2023, max compression
```

## Comparing `teneva_opti-0.2.0.tar` & `teneva_opti-0.3.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-01 16:21:12.516451 teneva_opti-0.2.0/
--rw-r--r--   0 andrei     (501) staff       (20)     1090 2023-02-25 19:48:03.000000 teneva_opti-0.2.0/LICENSE.txt
--rw-r--r--   0 andrei     (501) staff       (20)       79 2023-07-27 15:33:45.000000 teneva_opti-0.2.0/MANIFEST.in
--rw-r--r--   0 andrei     (501) staff       (20)     2873 2023-08-01 16:21:12.516583 teneva_opti-0.2.0/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)     1638 2023-08-01 16:19:15.000000 teneva_opti-0.2.0/README.md
--rw-r--r--   0 andrei     (501) staff       (20)      962 2023-08-01 14:40:29.000000 teneva_opti-0.2.0/demo.py
--rw-r--r--   0 andrei     (501) staff       (20)       95 2023-07-31 14:35:39.000000 teneva_opti-0.2.0/requirements.txt
--rw-r--r--   0 andrei     (501) staff       (20)      107 2023-08-01 16:21:12.517076 teneva_opti-0.2.0/setup.cfg
--rw-r--r--   0 andrei     (501) staff       (20)     2498 2023-07-27 15:35:28.000000 teneva_opti-0.2.0/setup.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-01 16:21:12.510992 teneva_opti-0.2.0/teneva_opti/
--rw-r--r--   0 andrei     (501) staff       (20)      191 2023-08-01 16:19:11.000000 teneva_opti-0.2.0/teneva_opti/__init__.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-01 16:21:12.512942 teneva_opti-0.2.0/teneva_opti/func/
--rw-r--r--   0 andrei     (501) staff       (20)        0 2023-07-31 13:03:34.000000 teneva_opti-0.2.0/teneva_opti/func/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     6401 2023-08-01 16:14:10.000000 teneva_opti-0.2.0/teneva_opti/opti.py
--rw-r--r--   0 andrei     (501) staff       (20)      113 2023-07-31 13:44:41.000000 teneva_opti-0.2.0/teneva_opti/opti_func.py
--rw-r--r--   0 andrei     (501) staff       (20)     1589 2023-08-01 16:14:38.000000 teneva_opti-0.2.0/teneva_opti/opti_manager.py
--rw-r--r--   0 andrei     (501) staff       (20)      722 2023-08-01 14:26:22.000000 teneva_opti-0.2.0/teneva_opti/opti_tens.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-01 16:21:12.516173 teneva_opti-0.2.0/teneva_opti/tens/
--rw-r--r--   0 andrei     (501) staff       (20)      344 2023-08-01 16:02:13.000000 teneva_opti-0.2.0/teneva_opti/tens/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)      391 2023-08-01 15:57:41.000000 teneva_opti-0.2.0/teneva_opti/tens/opti_tens_nb.py
--rw-r--r--   0 andrei     (501) staff       (20)      391 2023-08-01 15:57:39.000000 teneva_opti-0.2.0/teneva_opti/tens/opti_tens_opo.py
--rw-r--r--   0 andrei     (501) staff       (20)     1130 2023-08-01 16:01:42.000000 teneva_opti-0.2.0/teneva_opti/tens/opti_tens_optimatt.py
--rw-r--r--   0 andrei     (501) staff       (20)      401 2023-08-01 15:57:37.000000 teneva_opti-0.2.0/teneva_opti/tens/opti_tens_portfolio.py
--rw-r--r--   0 andrei     (501) staff       (20)     2116 2023-08-01 14:22:58.000000 teneva_opti-0.2.0/teneva_opti/tens/opti_tens_protes.py
--rw-r--r--   0 andrei     (501) staff       (20)      377 2023-08-01 15:57:35.000000 teneva_opti-0.2.0/teneva_opti/tens/opti_tens_pso.py
--rw-r--r--   0 andrei     (501) staff       (20)      381 2023-08-01 15:57:33.000000 teneva_opti-0.2.0/teneva_opti/tens/opti_tens_spsa.py
--rw-r--r--   0 andrei     (501) staff       (20)     1295 2023-08-01 15:54:43.000000 teneva_opti-0.2.0/teneva_opti/tens/opti_tens_ttopt.py
--rw-r--r--   0 andrei     (501) staff       (20)     1215 2023-08-01 15:12:42.000000 teneva_opti-0.2.0/teneva_opti/utils.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-01 16:21:12.512621 teneva_opti-0.2.0/teneva_opti.egg-info/
--rw-r--r--   0 andrei     (501) staff       (20)     2873 2023-08-01 16:21:12.000000 teneva_opti-0.2.0/teneva_opti.egg-info/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)      740 2023-08-01 16:21:12.000000 teneva_opti-0.2.0/teneva_opti.egg-info/SOURCES.txt
--rw-r--r--   0 andrei     (501) staff       (20)        1 2023-08-01 16:21:12.000000 teneva_opti-0.2.0/teneva_opti.egg-info/dependency_links.txt
--rw-r--r--   0 andrei     (501) staff       (20)       95 2023-08-01 16:21:12.000000 teneva_opti-0.2.0/teneva_opti.egg-info/requires.txt
--rw-r--r--   0 andrei     (501) staff       (20)       12 2023-08-01 16:21:12.000000 teneva_opti-0.2.0/teneva_opti.egg-info/top_level.txt
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-02 16:25:30.239149 teneva_opti-0.3.0/
+-rw-r--r--   0 andrei     (501) staff       (20)     1090 2023-02-25 19:48:03.000000 teneva_opti-0.3.0/LICENSE.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       79 2023-07-27 15:33:45.000000 teneva_opti-0.3.0/MANIFEST.in
+-rw-r--r--   0 andrei     (501) staff       (20)     3198 2023-08-02 16:25:30.239300 teneva_opti-0.3.0/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)     1923 2023-08-02 16:06:51.000000 teneva_opti-0.3.0/README.md
+-rw-r--r--   0 andrei     (501) staff       (20)     1244 2023-08-02 16:02:49.000000 teneva_opti-0.3.0/demo.py
+-rw-r--r--   0 andrei     (501) staff       (20)       95 2023-08-02 12:48:02.000000 teneva_opti-0.3.0/requirements.txt
+-rw-r--r--   0 andrei     (501) staff       (20)      107 2023-08-02 16:25:30.239805 teneva_opti-0.3.0/setup.cfg
+-rw-r--r--   0 andrei     (501) staff       (20)     2538 2023-08-02 09:28:28.000000 teneva_opti-0.3.0/setup.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-02 16:25:30.232010 teneva_opti-0.3.0/teneva_opti/
+-rw-r--r--   0 andrei     (501) staff       (20)      191 2023-08-02 16:06:55.000000 teneva_opti-0.3.0/teneva_opti/__init__.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-02 16:25:30.234291 teneva_opti-0.3.0/teneva_opti/func/
+-rw-r--r--   0 andrei     (501) staff       (20)        0 2023-07-31 13:03:34.000000 teneva_opti-0.3.0/teneva_opti/func/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     6295 2023-08-02 16:22:44.000000 teneva_opti-0.3.0/teneva_opti/opti.py
+-rw-r--r--   0 andrei     (501) staff       (20)      113 2023-07-31 13:44:41.000000 teneva_opti-0.3.0/teneva_opti/opti_func.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2274 2023-08-02 16:11:38.000000 teneva_opti-0.3.0/teneva_opti/opti_manager.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1043 2023-08-02 15:52:07.000000 teneva_opti-0.3.0/teneva_opti/opti_tens.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-02 16:25:30.238612 teneva_opti-0.3.0/teneva_opti/tens/
+-rw-r--r--   0 andrei     (501) staff       (20)      344 2023-08-01 16:02:13.000000 teneva_opti-0.3.0/teneva_opti/tens/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)      391 2023-08-01 15:57:41.000000 teneva_opti-0.3.0/teneva_opti/tens/opti_tens_nb.py
+-rw-r--r--   0 andrei     (501) staff       (20)      391 2023-08-01 15:57:39.000000 teneva_opti-0.3.0/teneva_opti/tens/opti_tens_opo.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1129 2023-08-02 14:22:34.000000 teneva_opti-0.3.0/teneva_opti/tens/opti_tens_optimatt.py
+-rw-r--r--   0 andrei     (501) staff       (20)      401 2023-08-01 15:57:37.000000 teneva_opti-0.3.0/teneva_opti/tens/opti_tens_portfolio.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2090 2023-08-02 14:22:10.000000 teneva_opti-0.3.0/teneva_opti/tens/opti_tens_protes.py
+-rw-r--r--   0 andrei     (501) staff       (20)      377 2023-08-01 15:57:35.000000 teneva_opti-0.3.0/teneva_opti/tens/opti_tens_pso.py
+-rw-r--r--   0 andrei     (501) staff       (20)      381 2023-08-01 15:57:33.000000 teneva_opti-0.3.0/teneva_opti/tens/opti_tens_spsa.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1289 2023-08-02 14:22:01.000000 teneva_opti-0.3.0/teneva_opti/tens/opti_tens_ttopt.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2367 2023-08-02 13:40:17.000000 teneva_opti-0.3.0/teneva_opti/utils.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-02 16:25:30.233974 teneva_opti-0.3.0/teneva_opti.egg-info/
+-rw-r--r--   0 andrei     (501) staff       (20)     3198 2023-08-02 16:25:30.000000 teneva_opti-0.3.0/teneva_opti.egg-info/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)      740 2023-08-02 16:25:30.000000 teneva_opti-0.3.0/teneva_opti.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        1 2023-08-02 16:25:30.000000 teneva_opti-0.3.0/teneva_opti.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       95 2023-08-02 16:25:30.000000 teneva_opti-0.3.0/teneva_opti.egg-info/requires.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       12 2023-08-02 16:25:30.000000 teneva_opti-0.3.0/teneva_opti.egg-info/top_level.txt
```

### Comparing `teneva_opti-0.2.0/LICENSE.txt` & `teneva_opti-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.2.0/PKG-INFO` & `teneva_opti-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: teneva_opti
-Version: 0.2.0
+Version: 0.3.0
 Summary: Collection of various optimization methods, including tensor based, for multivariate functions and multidimensional data arrays
 Home-page: https://github.com/AndreiChertkov/teneva_opti
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AndreiChertkov/teneva_opti
-Keywords: optimization method multidimensional array multivariate function tensor train nevergrad cma ttopt protes
+Keywords: optimization method multidimensional array multivariate function tensor train nevergrad cma ttopt protes genetic algorithm evolutionary strategy
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Intended Audience :: Science/Research
@@ -30,23 +30,25 @@
 ## Description
 
 Collection of various optimization methods (search for the global minimum and/or maximum) for multivariate functions and multidimensional data arrays (tensors). This library is based on a software product [teneva](https://github.com/AndreiChertkov/teneva). See also related benchmarks library [teneva_bm](https://github.com/AndreiChertkov/teneva_bm).
 
 
 ## Installation
 
-> Current version "0.2.0".
+> Current version "0.3.0".
 
 The package can be installed via pip: `pip install teneva_opti` (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9). It can be also downloaded from the repository [teneva_opti](https://github.com/AndreiChertkov/teneva_opti) and installed by `python setup.py install` command from the root folder of the project.
 
-We test optimizers with benchmarks from [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) library. For installation of additional dependencies (`gym` and `mujoco`) for `agent` collection , please, do the following (for existing environment `teneva_opti`):
+We test optimizers with benchmarks from [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) library. For installation of additional dependencies (`gym` and `mujoco`) for `agent` collection , please, do the following (for existing conda environment `teneva_opti`; if you are using a different environment name, then please make the appropriate substitution in the script):
 ```bash
 wget https://raw.githubusercontent.com/AndreiChertkov/teneva_bm/main/install_mujoco.py && python install_mujoco.py --env teneva_opti && rm install_mujoco.py
 ```
 
+> In the case of problems with `scikit-learn`, uninstall it `pip uninstall scikit-learn` and then install it from the anaconda: `conda install -c anaconda scikit-learn`.
+
 
 ## Documentation and examples (TODO)
 
 Please, run the demo script:
 ```bash
 clear && python demo.py
 ```
```

### Comparing `teneva_opti-0.2.0/README.md` & `teneva_opti-0.3.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 ## Description
 
 Collection of various optimization methods (search for the global minimum and/or maximum) for multivariate functions and multidimensional data arrays (tensors). This library is based on a software product [teneva](https://github.com/AndreiChertkov/teneva). See also related benchmarks library [teneva_bm](https://github.com/AndreiChertkov/teneva_bm).
 
 
 ## Installation
 
-> Current version "0.2.0".
+> Current version "0.3.0".
 
 The package can be installed via pip: `pip install teneva_opti` (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9). It can be also downloaded from the repository [teneva_opti](https://github.com/AndreiChertkov/teneva_opti) and installed by `python setup.py install` command from the root folder of the project.
 
-We test optimizers with benchmarks from [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) library. For installation of additional dependencies (`gym` and `mujoco`) for `agent` collection , please, do the following (for existing environment `teneva_opti`):
+We test optimizers with benchmarks from [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) library. For installation of additional dependencies (`gym` and `mujoco`) for `agent` collection , please, do the following (for existing conda environment `teneva_opti`; if you are using a different environment name, then please make the appropriate substitution in the script):
 ```bash
 wget https://raw.githubusercontent.com/AndreiChertkov/teneva_bm/main/install_mujoco.py && python install_mujoco.py --env teneva_opti && rm install_mujoco.py
 ```
 
+> In the case of problems with `scikit-learn`, uninstall it `pip uninstall scikit-learn` and then install it from the anaconda: `conda install -c anaconda scikit-learn`.
+
 
 ## Documentation and examples (TODO)
 
 Please, run the demo script:
 ```bash
 clear && python demo.py
 ```
```

### Comparing `teneva_opti-0.2.0/setup.py` & `teneva_opti-0.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         'Intended Audience :: Science/Research',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
-    keywords='optimization method multidimensional array multivariate function tensor train nevergrad cma ttopt protes',
+    keywords='optimization method multidimensional array multivariate function tensor train nevergrad cma ttopt protes genetic algorithm evolutionary strategy',
     packages=find_packages('teneva_opti', './teneva_opti/'),
     python_requires='>=3.8',
     project_urls={
         'Source': 'https://github.com/AndreiChertkov/teneva_opti',
     },
     license='MIT',
     license_files = ('LICENSE.txt',),
```

### Comparing `teneva_opti-0.2.0/teneva_opti/opti.py` & `teneva_opti-0.3.0/teneva_opti/opti.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import numpy as np
 import os
 
 
 from .utils import Log
+from .utils import get_identity_str
 from .utils import path
 from teneva_opti import __version__
 
 
 class Opti:
-    def __init__(self, name, desc, bm, m, seed=0, fold='result',
-                 with_cache=True, log=True, log_info=False, log_file=False):
+    def __init__(self, name, desc, bm, m=1.E+4, seed=0, fold='result_demo',
+                 with_cache=True, log=True, log_info=False, log_file=False,
+                 machine=''):
+        self.machine = machine
         self.name = name
         self.desc = desc
         self.seed = seed
         self.fold = fold
+        self.m = int(m)
 
         self.bm = bm
 
         if self.bm.is_prep:
             if self.bm.budget_m != m:
                 raise ValueError('Invalid BM configuration ("m")')
             if self.bm.budget_m_cache != m:
@@ -25,55 +29,34 @@
             if self.bm.with_cache != with_cache:
                 raise ValueError('Invalid BM configuration ("with_cache")')
         else:
             self.bm.set_cache(with_cache)
             self.bm.set_budget(m, m_cache=m)
             self.bm.prep()
 
-        self.log = Log(self.fpath() if log_file else None, log, log_info)
-        self.bm.set_log(self.log, prefix=self.name,
+        self.log = Log(self.fpath('log') if log_file else None, log, log_info)
+        self.bm.set_log(self.log if log else False, prefix=self.name,
             cond=('max' if self.is_max else 'min'),
             with_max=self.is_max, with_min=not self.is_max)
 
-        self.opts()
+        self.is_fail = False
+
+        self.set_opts()
 
     @property
     def d(self):
         return self.bm.d
 
     @property
     def i_opt(self):
         return self.bm.i_max if self.is_max else self.bm.i_min
 
     @property
     def identity(self):
-        dir = []
-
-        for id in self.bm.identity:
-            v = getattr(self.bm, id)
-
-            if isinstance(v, (list, np.ndarray)):
-                if isinstance(v[0], float):
-                    self.log.err('Float bm identity is not supported')
-                v = self.bm.list_convert(v, 'int')
-
-            if isinstance(v, (list, np.ndarray)):
-                self.log.err('List-like bm identity is not supported')
-
-            if isinstance(v, float):
-                self.log.err('Float bm identity is not supported')
-
-            if isinstance(v, bool):
-                if not v:
-                    continue
-                dir.append(f'{id}')
-            else:
-                dir.append(f'{id}-{v}')
-
-        return dir
+        return ['seed', 'm']
 
     @property
     def is_max(self):
         return self.bm.is_opti_max
 
     @property
     def is_n_equal(self):
@@ -95,32 +78,36 @@
     def x_opt(self):
         return self.bm.x_max if self.is_max else self.bm.x_min
 
     @property
     def y_opt(self):
         return self.bm.y_max if self.is_max else self.bm.y_min
 
-    def fpath(self, kind='log'):
-        fpath = [self.fold, self.bm.name, kind, *self.identity, self.name]
-        return os.path.join(*fpath)
+    def fpath(self, kind):
+        id = get_identity_str(self)
+        id_bm = get_identity_str(self.bm)
+        return os.path.join(self.fold, self.bm.name, kind, id_bm, id, self.name)
 
     def get_config(self):
         """Return a dict with configuration of the optimizer and benchmark."""
         conf = {}
         conf['d'] = self.d
-        conf['n'] = self.bm.list_convert(self.n, 'int'),
+        conf['n'] = self.bm.list_convert(self.n, 'int')
+        conf['m'] = self.m
         conf['seed'] = self.seed
         conf['name'] = self.name
+        conf['machine'] = self.machine
         conf['opti'] = self.__class__.__name__
         conf['bm'] = self.bm.get_config()
         return conf
 
     def get_history(self):
         """Return a dict with optimization results."""
         hist = {}
+        hist['err'] = 'Fail' if self.is_fail else ''
         hist['bm'] = self.bm.get_history()
         return hist
 
     def info(self, footer=''):
         """Returns a detailed description of the optimizer as text."""
         text = '*' * 78 + '\n' + 'OPTI: '
         text += self.name + ' ' * max(0, 34-len(self.name)) +  ' | '
@@ -146,14 +133,23 @@
         v = __version__
         text += f'{v}\n'
 
         text += 'Random seed                              : '
         v = self.seed
         text += f'{v}\n'
 
+        if self.machine:
+            text += 'Used machine                             : '
+            v = self.machine
+            text += f'{v}\n'
+
+        text += 'Computation budget                       : '
+        v = self.m
+        text += f'{v}\n'
+
         text += 'Optimizer                                : '
         v = self.__class__.__name__
         text += f'{v}\n'
 
         if footer:
             text += '-' * 41 + '|             '
             text += '>               Options'
@@ -165,51 +161,48 @@
 
     def load(self, fpath=None):
         """Load configuration and optimization result from npz file."""
         fpath = path(fpath or self.fpath('data'), 'npz')
         data = np.load(fpath, allow_pickle=True).get('data').item()
         return data
 
-    def run(self, with_raise=True):
+    def run(self, with_err=True):
         self.bm.init()
         self.log.info(self.info() + '\n' + self.bm.info())
 
         self.is_fail = False
 
         try:
             self._optimize()
         except Exception as e:
             self.is_fail = True
-            msg = f'Optimization with "{self.name}" failed [{e}]'
-            if with_raise:
-                raise ValueError(msg)
-            else:
-                self.log.wrn(msg)
+            msg = f'Optimization with "{self.name}" is failed [{e}]'
+            self.log.err(msg) if with_err else self.log.wrn(msg)
 
         self.log.info(self.bm.info_history())
 
-    def opts(self):
-        return
-
-    def render(self, fpath=None):
+    def render(self, fpath=None, with_wrn=True):
         if self.bm.with_render:
             return self.bm.render(fpath or self.fpath('render'))
-        else:
+        elif with_wrn:
             self.log.wrn(f'Render is not supported for BM "{self.bm.name}"')
 
     def save(self, fpath=None):
         """Save configuration and optimization result to npz file."""
         data = {'config': self.get_config(), 'history': self.get_history()}
         fpath = path(fpath or self.fpath('data'), 'npz')
         np.savez_compressed(fpath, data=data)
 
-    def show(self, fpath=None):
+    def set_opts(self):
+        return
+
+    def show(self, fpath=None, with_wrn=True):
         if self.bm.with_show:
             return self.bm.show(fpath or self.fpath('show'))
-        else:
+        elif with_wrn:
             self.log.wrn(f'Show is not supported for BM "{self.bm.name}"')
 
     def target(self, inp):
         raise NotImplementedError
 
     def target_func(self, x):
         return self.bm.get_poi(x)
```

### Comparing `teneva_opti-0.2.0/teneva_opti/tens/opti_tens_optimatt.py` & `teneva_opti-0.3.0/teneva_opti/tens/opti_tens_optimatt.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,31 +14,31 @@
 
 class OptiTensOptimatt(OptiTens):
     def __init__(self, *args, **kwargs):
         super().__init__('optimatt', DESC, *args, **kwargs)
 
     def get_config(self):
         conf = super().get_config()
-        conf['_dr_max'] = self._dr_max
+        conf['dr_max'] = self.dr_max
         return conf
 
     def info(self, footer=''):
         text = ''
 
-        text += '_dr_max (max rank increment)             : '
-        v = self._dr_max
+        text += 'dr_max (max rank increment)              : '
+        v = self.dr_max
         text += f'{v}\n'
 
         return super().info(text + footer)
 
-    def opts(self, dr_max=2):
-        self._dr_max = dr_max
+    def set_opts(self, dr_max=2):
+        self.dr_max = dr_max
 
     def _optimize(self):
         Y = teneva.rand(self.n, r=1)
         Y = teneva.cross(self.target, Y, e=1.E-16, m=self.bm.budget_m-2,
-            dr_max=self._dr_max)
+            dr_max=self.dr_max)
         Y = teneva.truncate(Y, e=1.E-16)
 
         i_min, y_min, i_max, y_max = teneva.optima_tt(Y)
         self.target(i_min)
         self.target(i_max)
```

### Comparing `teneva_opti-0.2.0/teneva_opti/tens/opti_tens_protes.py` & `teneva_opti-0.3.0/teneva_opti/tens/opti_tens_protes.py`

 * *Files 23% similar despite different names*

```diff
@@ -21,55 +21,55 @@
 
 class OptiTensProtes(OptiTens):
     def __init__(self, *args, **kwargs):
         super().__init__('protes', DESC, *args, **kwargs)
 
     def get_config(self):
         conf = super().get_config()
-        conf['_k'] = self._k
-        conf['_k_top'] = self._k_top
-        conf['_k_gd'] = self._k_gd
-        conf['_lr'] = self._lr
-        conf['_r'] = self._r
+        conf['k'] = self.k
+        conf['k_top'] = self.k_top
+        conf['k_gd'] = self.k_gd
+        conf['lr'] = self.lr
+        conf['r'] = self.r
         return conf
 
     def info(self, footer=''):
         text = ''
 
-        text += '_k (batch size)                          : '
-        v = self._k
+        text += 'k (batch size)                           : '
+        v = self.k
         text += f'{v}\n'
 
-        text += '_k_top (number of selected candidates)   : '
-        v = self._k_top
+        text += 'k_top (number of selected candidates)    : '
+        v = self.k_top
         text += f'{v}\n'
 
-        text += '_k_gd (number of gradient lifting iters) : '
-        v = self._k_gd
+        text += 'k_gd (number of gradient lifting iters)  : '
+        v = self.k_gd
         text += f'{v}\n'
 
-        text += '_lr (learning rate for gradient lifting) : '
-        v = self._lr
+        text += 'lr (learning rate for gradient lifting)  : '
+        v = self.lr
         text += f'{v}\n'
 
-        text += '_r (TT-rank of the inner prob tensor)    : '
-        v = self._r
+        text += 'r (TT-rank of the inner prob tensor)     : '
+        v = self.r
         text += f'{v}\n'
 
         return super().info(text + footer)
 
-    def opts(self, k=100, k_top=10, k_gd=1, lr=5.E-2, r=5):
-        self._k = k
-        self._k_top = k_top
-        self._k_gd = k_gd
-        self._lr = lr
-        self._r = r
+    def set_opts(self, k=100, k_top=10, k_gd=1, lr=5.E-2, r=5):
+        self.k = k
+        self.k_top = k_top
+        self.k_gd = k_gd
+        self.lr = lr
+        self.r = r
 
     def _optimize(self):
         if self.is_n_equal:
             protes(self.target, self.d, self.n0, 1.E+99,
-                k=self._k, k_top=self._k_top, k_gd=self._k_gd, lr=self._lr,
-                r=self._r, seed=self.seed, is_max=self.is_max)
+                k=self.k, k_top=self.k_top, k_gd=self.k_gd, lr=self.lr,
+                r=self.r, seed=self.seed, is_max=self.is_max)
         else:
             protes_general(self.target, self.n, 1.E+99,
-                k=self._k, k_top=self._k_top, k_gd=self._k_gd, lr=self._lr,
-                r=self._r, seed=self.seed, is_max=self.is_max)
+                k=self.k, k_top=self.k_top, k_gd=self.k_gd, lr=self.lr,
+                r=self.r, seed=self.seed, is_max=self.is_max)
```

### Comparing `teneva_opti-0.2.0/teneva_opti/tens/opti_tens_ttopt.py` & `teneva_opti-0.3.0/teneva_opti/tens/opti_tens_ttopt.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,33 +15,33 @@
 
 class OptiTensTtopt(OptiTens):
     def __init__(self, *args, **kwargs):
         super().__init__('ttopt', DESC, *args, **kwargs)
 
     def get_config(self):
         conf = super().get_config()
-        conf['_rank'] = self._rank
-        conf['_fs_opt'] = self._fs_opt
+        conf['rank'] = self.rank
+        conf['fs_opt'] = self.fs_opt
         return conf
 
     def info(self, footer=''):
         text = ''
 
-        text += '_rank (TT-rank)                          : '
-        v = self._rank
+        text += 'rank (TT-rank)                           : '
+        v = self.rank
         text += f'{v}\n'
 
-        text += '_fs_opt (transformation option)          : '
-        v = self._fs_opt
+        text += 'fs_opt (transformation option)           : '
+        v = self.fs_opt
         text += f'{v}\n'
 
         return super().info(text + footer)
 
-    def opts(self, rank=4, fs_opt=1.):
-        self._rank = rank
-        self._fs_opt = fs_opt
+    def set_opts(self, rank=4, fs_opt=1.):
+        self.rank = rank
+        self.fs_opt = fs_opt
 
     def _optimize(self):
         tto = TTOpt(f=self.target, d=self.d, n=self.n,
             evals=1.E+99, is_func=False, is_vect=True)
-        tto.optimize(rank=self._rank, seed=self.seed,
-            fs_opt=self._fs_opt, is_max=self.is_max)
+        tto.optimize(rank=self.rank, seed=self.seed,
+            fs_opt=self.fs_opt, is_max=self.is_max)
```

### Comparing `teneva_opti-0.2.0/teneva_opti.egg-info/PKG-INFO` & `teneva_opti-0.3.0/teneva_opti.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: teneva-opti
-Version: 0.2.0
+Version: 0.3.0
 Summary: Collection of various optimization methods, including tensor based, for multivariate functions and multidimensional data arrays
 Home-page: https://github.com/AndreiChertkov/teneva_opti
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AndreiChertkov/teneva_opti
-Keywords: optimization method multidimensional array multivariate function tensor train nevergrad cma ttopt protes
+Keywords: optimization method multidimensional array multivariate function tensor train nevergrad cma ttopt protes genetic algorithm evolutionary strategy
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Intended Audience :: Science/Research
@@ -30,23 +30,25 @@
 ## Description
 
 Collection of various optimization methods (search for the global minimum and/or maximum) for multivariate functions and multidimensional data arrays (tensors). This library is based on a software product [teneva](https://github.com/AndreiChertkov/teneva). See also related benchmarks library [teneva_bm](https://github.com/AndreiChertkov/teneva_bm).
 
 
 ## Installation
 
-> Current version "0.2.0".
+> Current version "0.3.0".
 
 The package can be installed via pip: `pip install teneva_opti` (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9). It can be also downloaded from the repository [teneva_opti](https://github.com/AndreiChertkov/teneva_opti) and installed by `python setup.py install` command from the root folder of the project.
 
-We test optimizers with benchmarks from [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) library. For installation of additional dependencies (`gym` and `mujoco`) for `agent` collection , please, do the following (for existing environment `teneva_opti`):
+We test optimizers with benchmarks from [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) library. For installation of additional dependencies (`gym` and `mujoco`) for `agent` collection , please, do the following (for existing conda environment `teneva_opti`; if you are using a different environment name, then please make the appropriate substitution in the script):
 ```bash
 wget https://raw.githubusercontent.com/AndreiChertkov/teneva_bm/main/install_mujoco.py && python install_mujoco.py --env teneva_opti && rm install_mujoco.py
 ```
 
+> In the case of problems with `scikit-learn`, uninstall it `pip uninstall scikit-learn` and then install it from the anaconda: `conda install -c anaconda scikit-learn`.
+
 
 ## Documentation and examples (TODO)
 
 Please, run the demo script:
 ```bash
 clear && python demo.py
 ```
```

### Comparing `teneva_opti-0.2.0/teneva_opti.egg-info/SOURCES.txt` & `teneva_opti-0.3.0/teneva_opti.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/fake_data_for_learning-0.4.1.tar.gz` & `tmp/fake_data_for_learning-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fake_data_for_learning-0.4.1.tar", last modified: Fri Jun 16 07:44:30 2023, max compression
+gzip compressed data, was "fake_data_for_learning-0.4.2.tar", last modified: Wed Aug  2 09:59:03 2023, max compression
```

## Comparing `fake_data_for_learning-0.4.1.tar` & `fake_data_for_learning-0.4.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 paullarsen   (501) staff       (20)        0 2023-06-16 07:44:30.870174 fake_data_for_learning-0.4.1/
--rw-r--r--   0 paullarsen   (501) staff       (20)     1074 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.1/LICENSE
--rw-r--r--   0 paullarsen   (501) staff       (20)     1711 2023-06-16 07:44:30.870234 fake_data_for_learning-0.4.1/PKG-INFO
--rw-r--r--   0 paullarsen   (501) staff       (20)     6455 2023-06-16 06:42:55.000000 fake_data_for_learning-0.4.1/README.md
-drwxr-xr-x   0 paullarsen   (501) staff       (20)        0 2023-06-16 07:44:30.867721 fake_data_for_learning-0.4.1/fake_data_for_learning/
--rw-r--r--   0 paullarsen   (501) staff       (20)        0 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.1/fake_data_for_learning/__init__.py
--rw-r--r--   0 paullarsen   (501) staff       (20)     2339 2023-06-15 12:49:41.000000 fake_data_for_learning-0.4.1/fake_data_for_learning/contingency_tables.py
--rw-r--r--   0 paullarsen   (501) staff       (20)    15082 2023-06-15 12:48:16.000000 fake_data_for_learning-0.4.1/fake_data_for_learning/fake_data_for_learning.py
--rw-r--r--   0 paullarsen   (501) staff       (20)    13482 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.1/fake_data_for_learning/probability_polytopes.py
--rw-r--r--   0 paullarsen   (501) staff       (20)      895 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.1/fake_data_for_learning/utils.py
-drwxr-xr-x   0 paullarsen   (501) staff       (20)        0 2023-06-16 07:44:30.868849 fake_data_for_learning-0.4.1/fake_data_for_learning.egg-info/
--rw-r--r--   0 paullarsen   (501) staff       (20)     1711 2023-06-16 07:44:30.000000 fake_data_for_learning-0.4.1/fake_data_for_learning.egg-info/PKG-INFO
--rw-r--r--   0 paullarsen   (501) staff       (20)      695 2023-06-16 07:44:30.000000 fake_data_for_learning-0.4.1/fake_data_for_learning.egg-info/SOURCES.txt
--rw-r--r--   0 paullarsen   (501) staff       (20)        1 2023-06-16 07:44:30.000000 fake_data_for_learning-0.4.1/fake_data_for_learning.egg-info/dependency_links.txt
--rw-r--r--   0 paullarsen   (501) staff       (20)        1 2023-06-15 12:43:35.000000 fake_data_for_learning-0.4.1/fake_data_for_learning.egg-info/not-zip-safe
--rw-r--r--   0 paullarsen   (501) staff       (20)       80 2023-06-16 07:44:30.000000 fake_data_for_learning-0.4.1/fake_data_for_learning.egg-info/requires.txt
--rw-r--r--   0 paullarsen   (501) staff       (20)       23 2023-06-16 07:44:30.000000 fake_data_for_learning-0.4.1/fake_data_for_learning.egg-info/top_level.txt
--rw-r--r--   0 paullarsen   (501) staff       (20)      302 2023-06-16 07:44:30.870450 fake_data_for_learning-0.4.1/setup.cfg
--rw-r--r--   0 paullarsen   (501) staff       (20)     2293 2023-06-15 15:14:49.000000 fake_data_for_learning-0.4.1/setup.py
-drwxr-xr-x   0 paullarsen   (501) staff       (20)        0 2023-06-16 07:44:30.870012 fake_data_for_learning-0.4.1/tests/
--rw-r--r--   0 paullarsen   (501) staff       (20)     5218 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.1/tests/test_bayesian_node_rv.py
--rw-r--r--   0 paullarsen   (501) staff       (20)     5353 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.1/tests/test_contingency_tables.py
--rw-r--r--   0 paullarsen   (501) staff       (20)     1281 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.1/tests/test_demo_notebooks.py
--rw-r--r--   0 paullarsen   (501) staff       (20)     8721 2023-06-16 06:45:18.000000 fake_data_for_learning-0.4.1/tests/test_fake_data_bn.py
--rw-r--r--   0 paullarsen   (501) staff       (20)    10959 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.1/tests/test_probability_polytopes.py
--rw-r--r--   0 paullarsen   (501) staff       (20)      577 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.1/tests/test_utils.py
+drwxr-xr-x   0 paullarsen   (501) staff       (20)        0 2023-08-02 09:59:03.267045 fake_data_for_learning-0.4.2/
+-rw-r--r--   0 paullarsen   (501) staff       (20)     1074 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.2/LICENSE
+-rw-r--r--   0 paullarsen   (501) staff       (20)     1711 2023-08-02 09:59:03.267103 fake_data_for_learning-0.4.2/PKG-INFO
+-rw-r--r--   0 paullarsen   (501) staff       (20)     6508 2023-08-02 09:45:17.000000 fake_data_for_learning-0.4.2/README.md
+drwxr-xr-x   0 paullarsen   (501) staff       (20)        0 2023-08-02 09:59:03.264309 fake_data_for_learning-0.4.2/fake_data_for_learning/
+-rw-r--r--   0 paullarsen   (501) staff       (20)        0 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.2/fake_data_for_learning/__init__.py
+-rw-r--r--   0 paullarsen   (501) staff       (20)     2339 2023-06-15 12:49:41.000000 fake_data_for_learning-0.4.2/fake_data_for_learning/contingency_tables.py
+-rw-r--r--   0 paullarsen   (501) staff       (20)    15082 2023-06-15 12:48:16.000000 fake_data_for_learning-0.4.2/fake_data_for_learning/fake_data_for_learning.py
+-rw-r--r--   0 paullarsen   (501) staff       (20)    13482 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.2/fake_data_for_learning/probability_polytopes.py
+-rw-r--r--   0 paullarsen   (501) staff       (20)      895 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.2/fake_data_for_learning/utils.py
+drwxr-xr-x   0 paullarsen   (501) staff       (20)        0 2023-08-02 09:59:03.265512 fake_data_for_learning-0.4.2/fake_data_for_learning.egg-info/
+-rw-r--r--   0 paullarsen   (501) staff       (20)     1711 2023-08-02 09:59:03.000000 fake_data_for_learning-0.4.2/fake_data_for_learning.egg-info/PKG-INFO
+-rw-r--r--   0 paullarsen   (501) staff       (20)      695 2023-08-02 09:59:03.000000 fake_data_for_learning-0.4.2/fake_data_for_learning.egg-info/SOURCES.txt
+-rw-r--r--   0 paullarsen   (501) staff       (20)        1 2023-08-02 09:59:03.000000 fake_data_for_learning-0.4.2/fake_data_for_learning.egg-info/dependency_links.txt
+-rw-r--r--   0 paullarsen   (501) staff       (20)        1 2023-06-15 12:43:35.000000 fake_data_for_learning-0.4.2/fake_data_for_learning.egg-info/not-zip-safe
+-rw-r--r--   0 paullarsen   (501) staff       (20)       80 2023-08-02 09:59:03.000000 fake_data_for_learning-0.4.2/fake_data_for_learning.egg-info/requires.txt
+-rw-r--r--   0 paullarsen   (501) staff       (20)       23 2023-08-02 09:59:03.000000 fake_data_for_learning-0.4.2/fake_data_for_learning.egg-info/top_level.txt
+-rw-r--r--   0 paullarsen   (501) staff       (20)      302 2023-08-02 09:59:03.267345 fake_data_for_learning-0.4.2/setup.cfg
+-rw-r--r--   0 paullarsen   (501) staff       (20)     2293 2023-08-02 09:45:45.000000 fake_data_for_learning-0.4.2/setup.py
+drwxr-xr-x   0 paullarsen   (501) staff       (20)        0 2023-08-02 09:59:03.266860 fake_data_for_learning-0.4.2/tests/
+-rw-r--r--   0 paullarsen   (501) staff       (20)     5218 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.2/tests/test_bayesian_node_rv.py
+-rw-r--r--   0 paullarsen   (501) staff       (20)     5353 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.2/tests/test_contingency_tables.py
+-rw-r--r--   0 paullarsen   (501) staff       (20)     1281 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.2/tests/test_demo_notebooks.py
+-rw-r--r--   0 paullarsen   (501) staff       (20)     8721 2023-06-16 08:13:57.000000 fake_data_for_learning-0.4.2/tests/test_fake_data_bn.py
+-rw-r--r--   0 paullarsen   (501) staff       (20)    10959 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.2/tests/test_probability_polytopes.py
+-rw-r--r--   0 paullarsen   (501) staff       (20)      577 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.2/tests/test_utils.py
```

### Comparing `fake_data_for_learning-0.4.1/LICENSE` & `fake_data_for_learning-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fake_data_for_learning-0.4.1/PKG-INFO` & `fake_data_for_learning-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fake_data_for_learning
-Version: 0.4.1
+Version: 0.4.2
 Author: Paul Larsen
 Author-email: munichpavel@gmail.com
 License: MIT license
 Project-URL: Homepage, https://munichpavel.github.io/fake-data-for-learning/
 Project-URL: Bug Tracker, https://github.com/munichpavel/fake-data-for-learning/issues
 Project-URL: Documentation, https://munichpavel.github.io/fake-data-docs/html/index.html
 Project-URL: Source Code, https://github.com/munichpavel/fake-data-for-learning/
```

### Comparing `fake_data_for_learning-0.4.1/README.md` & `fake_data_for_learning-0.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,18 @@
 
 * [pyagrum](https://pyagrum.readthedocs.io) is a Python wrapper around the C++ library [aGrUM](http://agrum.org/), and has similar funcionality with a larger scope. Unlike `pgmpy`, `pyagrum` has a similar API for specifying conditional probability tables to the one used here.
 
 * [causalgraphicalmodels](https://github.com/ijmbarr/causalgraphicalmodels)'s class `StructuralCausalModel` allows sampling from Bayesian network where the variables are related as functions of one another, rather than via the conditional probability tables used here.
 
 ## Change log
 
+### v0.4.2
+
+Fix mac os x dependency install issue.
+
 ### v0.4.1
 
-Fix dependencies' API changes
+Fix dependencies' API changes.
 
 ### v0.4.0
 
 This release adds a method for generating categorical data whose (multidimensional) contingency table equals a given one. The motivation is to generate fake data exhibiting [Simpson's paradox](https://en.wikipedia.org/wiki/Simpson%27s_paradox).
```

### Comparing `fake_data_for_learning-0.4.1/fake_data_for_learning/contingency_tables.py` & `fake_data_for_learning-0.4.2/fake_data_for_learning/contingency_tables.py`

 * *Files identical despite different names*

### Comparing `fake_data_for_learning-0.4.1/fake_data_for_learning/fake_data_for_learning.py` & `fake_data_for_learning-0.4.2/fake_data_for_learning/fake_data_for_learning.py`

 * *Files identical despite different names*

### Comparing `fake_data_for_learning-0.4.1/fake_data_for_learning/probability_polytopes.py` & `fake_data_for_learning-0.4.2/fake_data_for_learning/probability_polytopes.py`

 * *Files identical despite different names*

### Comparing `fake_data_for_learning-0.4.1/fake_data_for_learning/utils.py` & `fake_data_for_learning-0.4.2/fake_data_for_learning/utils.py`

 * *Files identical despite different names*

### Comparing `fake_data_for_learning-0.4.1/fake_data_for_learning.egg-info/PKG-INFO` & `fake_data_for_learning-0.4.2/fake_data_for_learning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fake-data-for-learning
-Version: 0.4.1
+Version: 0.4.2
 Author: Paul Larsen
 Author-email: munichpavel@gmail.com
 License: MIT license
 Project-URL: Homepage, https://munichpavel.github.io/fake-data-for-learning/
 Project-URL: Bug Tracker, https://github.com/munichpavel/fake-data-for-learning/issues
 Project-URL: Documentation, https://munichpavel.github.io/fake-data-docs/html/index.html
 Project-URL: Source Code, https://github.com/munichpavel/fake-data-for-learning/
```

### Comparing `fake_data_for_learning-0.4.1/fake_data_for_learning.egg-info/SOURCES.txt` & `fake_data_for_learning-0.4.2/fake_data_for_learning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fake_data_for_learning-0.4.1/setup.py` & `fake_data_for_learning-0.4.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     'xarray',
     'pypoman'
 ]
 
 
 setup(
     name='fake_data_for_learning',
-    version='0.4.1',
+    version='0.4.2',
     long_description=description,
     long_description_content_type='text/markdown',
     project_urls={
         "Homepage": "https://munichpavel.github.io/fake-data-for-learning/",
         "Bug Tracker": "https://github.com/munichpavel/fake-data-for-learning/issues",
         "Documentation": "https://munichpavel.github.io/fake-data-docs/html/index.html",
         "Source Code": "https://github.com/munichpavel/fake-data-for-learning/",
```

### Comparing `fake_data_for_learning-0.4.1/tests/test_bayesian_node_rv.py` & `fake_data_for_learning-0.4.2/tests/test_bayesian_node_rv.py`

 * *Files identical despite different names*

### Comparing `fake_data_for_learning-0.4.1/tests/test_contingency_tables.py` & `fake_data_for_learning-0.4.2/tests/test_contingency_tables.py`

 * *Files identical despite different names*

### Comparing `fake_data_for_learning-0.4.1/tests/test_demo_notebooks.py` & `fake_data_for_learning-0.4.2/tests/test_demo_notebooks.py`

 * *Files identical despite different names*

### Comparing `fake_data_for_learning-0.4.1/tests/test_fake_data_bn.py` & `fake_data_for_learning-0.4.2/tests/test_fake_data_bn.py`

 * *Files identical despite different names*

### Comparing `fake_data_for_learning-0.4.1/tests/test_probability_polytopes.py` & `fake_data_for_learning-0.4.2/tests/test_probability_polytopes.py`

 * *Files identical despite different names*

### Comparing `fake_data_for_learning-0.4.1/tests/test_utils.py` & `fake_data_for_learning-0.4.2/tests/test_utils.py`

 * *Files identical despite different names*


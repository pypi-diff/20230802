# Comparing `tmp/fake_data_for_learning-0.4.2.tar.gz` & `tmp/fake_data_for_learning-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fake_data_for_learning-0.4.2.tar", last modified: Wed Aug  2 09:59:03 2023, max compression
+gzip compressed data, was "fake_data_for_learning-0.4.3.tar", last modified: Wed Aug  2 10:23:57 2023, max compression
```

## Comparing `fake_data_for_learning-0.4.2.tar` & `fake_data_for_learning-0.4.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 paullarsen   (501) staff       (20)        0 2023-08-02 09:59:03.267045 fake_data_for_learning-0.4.2/
--rw-r--r--   0 paullarsen   (501) staff       (20)     1074 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.2/LICENSE
--rw-r--r--   0 paullarsen   (501) staff       (20)     1711 2023-08-02 09:59:03.267103 fake_data_for_learning-0.4.2/PKG-INFO
--rw-r--r--   0 paullarsen   (501) staff       (20)     6508 2023-08-02 09:45:17.000000 fake_data_for_learning-0.4.2/README.md
-drwxr-xr-x   0 paullarsen   (501) staff       (20)        0 2023-08-02 09:59:03.264309 fake_data_for_learning-0.4.2/fake_data_for_learning/
--rw-r--r--   0 paullarsen   (501) staff       (20)        0 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.2/fake_data_for_learning/__init__.py
--rw-r--r--   0 paullarsen   (501) staff       (20)     2339 2023-06-15 12:49:41.000000 fake_data_for_learning-0.4.2/fake_data_for_learning/contingency_tables.py
--rw-r--r--   0 paullarsen   (501) staff       (20)    15082 2023-06-15 12:48:16.000000 fake_data_for_learning-0.4.2/fake_data_for_learning/fake_data_for_learning.py
--rw-r--r--   0 paullarsen   (501) staff       (20)    13482 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.2/fake_data_for_learning/probability_polytopes.py
--rw-r--r--   0 paullarsen   (501) staff       (20)      895 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.2/fake_data_for_learning/utils.py
-drwxr-xr-x   0 paullarsen   (501) staff       (20)        0 2023-08-02 09:59:03.265512 fake_data_for_learning-0.4.2/fake_data_for_learning.egg-info/
--rw-r--r--   0 paullarsen   (501) staff       (20)     1711 2023-08-02 09:59:03.000000 fake_data_for_learning-0.4.2/fake_data_for_learning.egg-info/PKG-INFO
--rw-r--r--   0 paullarsen   (501) staff       (20)      695 2023-08-02 09:59:03.000000 fake_data_for_learning-0.4.2/fake_data_for_learning.egg-info/SOURCES.txt
--rw-r--r--   0 paullarsen   (501) staff       (20)        1 2023-08-02 09:59:03.000000 fake_data_for_learning-0.4.2/fake_data_for_learning.egg-info/dependency_links.txt
--rw-r--r--   0 paullarsen   (501) staff       (20)        1 2023-06-15 12:43:35.000000 fake_data_for_learning-0.4.2/fake_data_for_learning.egg-info/not-zip-safe
--rw-r--r--   0 paullarsen   (501) staff       (20)       80 2023-08-02 09:59:03.000000 fake_data_for_learning-0.4.2/fake_data_for_learning.egg-info/requires.txt
--rw-r--r--   0 paullarsen   (501) staff       (20)       23 2023-08-02 09:59:03.000000 fake_data_for_learning-0.4.2/fake_data_for_learning.egg-info/top_level.txt
--rw-r--r--   0 paullarsen   (501) staff       (20)      302 2023-08-02 09:59:03.267345 fake_data_for_learning-0.4.2/setup.cfg
--rw-r--r--   0 paullarsen   (501) staff       (20)     2293 2023-08-02 09:45:45.000000 fake_data_for_learning-0.4.2/setup.py
-drwxr-xr-x   0 paullarsen   (501) staff       (20)        0 2023-08-02 09:59:03.266860 fake_data_for_learning-0.4.2/tests/
--rw-r--r--   0 paullarsen   (501) staff       (20)     5218 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.2/tests/test_bayesian_node_rv.py
--rw-r--r--   0 paullarsen   (501) staff       (20)     5353 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.2/tests/test_contingency_tables.py
--rw-r--r--   0 paullarsen   (501) staff       (20)     1281 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.2/tests/test_demo_notebooks.py
--rw-r--r--   0 paullarsen   (501) staff       (20)     8721 2023-06-16 08:13:57.000000 fake_data_for_learning-0.4.2/tests/test_fake_data_bn.py
--rw-r--r--   0 paullarsen   (501) staff       (20)    10959 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.2/tests/test_probability_polytopes.py
--rw-r--r--   0 paullarsen   (501) staff       (20)      577 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.2/tests/test_utils.py
+drwxr-xr-x   0 paullarsen   (501) staff       (20)        0 2023-08-02 10:23:57.151759 fake_data_for_learning-0.4.3/
+-rw-r--r--   0 paullarsen   (501) staff       (20)     1074 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.3/LICENSE
+-rw-r--r--   0 paullarsen   (501) staff       (20)     1711 2023-08-02 10:23:57.151808 fake_data_for_learning-0.4.3/PKG-INFO
+-rw-r--r--   0 paullarsen   (501) staff       (20)     6890 2023-08-02 10:22:09.000000 fake_data_for_learning-0.4.3/README.md
+drwxr-xr-x   0 paullarsen   (501) staff       (20)        0 2023-08-02 10:23:57.149566 fake_data_for_learning-0.4.3/fake_data_for_learning/
+-rw-r--r--   0 paullarsen   (501) staff       (20)        0 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.3/fake_data_for_learning/__init__.py
+-rw-r--r--   0 paullarsen   (501) staff       (20)     2339 2023-06-15 12:49:41.000000 fake_data_for_learning-0.4.3/fake_data_for_learning/contingency_tables.py
+-rw-r--r--   0 paullarsen   (501) staff       (20)    15082 2023-06-15 12:48:16.000000 fake_data_for_learning-0.4.3/fake_data_for_learning/fake_data_for_learning.py
+-rw-r--r--   0 paullarsen   (501) staff       (20)    13482 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.3/fake_data_for_learning/probability_polytopes.py
+-rw-r--r--   0 paullarsen   (501) staff       (20)      895 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.3/fake_data_for_learning/utils.py
+drwxr-xr-x   0 paullarsen   (501) staff       (20)        0 2023-08-02 10:23:57.150636 fake_data_for_learning-0.4.3/fake_data_for_learning.egg-info/
+-rw-r--r--   0 paullarsen   (501) staff       (20)     1711 2023-08-02 10:23:57.000000 fake_data_for_learning-0.4.3/fake_data_for_learning.egg-info/PKG-INFO
+-rw-r--r--   0 paullarsen   (501) staff       (20)      695 2023-08-02 10:23:57.000000 fake_data_for_learning-0.4.3/fake_data_for_learning.egg-info/SOURCES.txt
+-rw-r--r--   0 paullarsen   (501) staff       (20)        1 2023-08-02 10:23:57.000000 fake_data_for_learning-0.4.3/fake_data_for_learning.egg-info/dependency_links.txt
+-rw-r--r--   0 paullarsen   (501) staff       (20)        1 2023-06-15 12:43:35.000000 fake_data_for_learning-0.4.3/fake_data_for_learning.egg-info/not-zip-safe
+-rw-r--r--   0 paullarsen   (501) staff       (20)       72 2023-08-02 10:23:57.000000 fake_data_for_learning-0.4.3/fake_data_for_learning.egg-info/requires.txt
+-rw-r--r--   0 paullarsen   (501) staff       (20)       23 2023-08-02 10:23:57.000000 fake_data_for_learning-0.4.3/fake_data_for_learning.egg-info/top_level.txt
+-rw-r--r--   0 paullarsen   (501) staff       (20)      302 2023-08-02 10:23:57.152041 fake_data_for_learning-0.4.3/setup.cfg
+-rw-r--r--   0 paullarsen   (501) staff       (20)     2350 2023-08-02 10:22:30.000000 fake_data_for_learning-0.4.3/setup.py
+drwxr-xr-x   0 paullarsen   (501) staff       (20)        0 2023-08-02 10:23:57.151615 fake_data_for_learning-0.4.3/tests/
+-rw-r--r--   0 paullarsen   (501) staff       (20)     5218 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.3/tests/test_bayesian_node_rv.py
+-rw-r--r--   0 paullarsen   (501) staff       (20)     5353 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.3/tests/test_contingency_tables.py
+-rw-r--r--   0 paullarsen   (501) staff       (20)     1281 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.3/tests/test_demo_notebooks.py
+-rw-r--r--   0 paullarsen   (501) staff       (20)     8721 2023-06-16 08:13:57.000000 fake_data_for_learning-0.4.3/tests/test_fake_data_bn.py
+-rw-r--r--   0 paullarsen   (501) staff       (20)    10959 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.3/tests/test_probability_polytopes.py
+-rw-r--r--   0 paullarsen   (501) staff       (20)      577 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.3/tests/test_utils.py
```

### Comparing `fake_data_for_learning-0.4.2/LICENSE` & `fake_data_for_learning-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fake_data_for_learning-0.4.2/PKG-INFO` & `fake_data_for_learning-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fake_data_for_learning
-Version: 0.4.2
+Version: 0.4.3
 Author: Paul Larsen
 Author-email: munichpavel@gmail.com
 License: MIT license
 Project-URL: Homepage, https://munichpavel.github.io/fake-data-for-learning/
 Project-URL: Bug Tracker, https://github.com/munichpavel/fake-data-for-learning/issues
 Project-URL: Documentation, https://munichpavel.github.io/fake-data-docs/html/index.html
 Project-URL: Source Code, https://github.com/munichpavel/fake-data-for-learning/
```

### Comparing `fake_data_for_learning-0.4.2/README.md` & `fake_data_for_learning-0.4.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -60,21 +60,25 @@
 
 ![docs/graphics/graph.png](docs/graphics/graph.png)
 
 See the demo notebook [notebooks/bayesian-network.ipynb](notebooks/bayesian-network.ipynb) for feature examples.
 
 To avoid having to enter all each value of a conditional probability array, there are also two methods to generate random conditional probability tables.
 
-The method `fake_data_for_learning.utils.RandomCpt()` gives a random conditional probability table, but if you want to constrain the entries to satisfy constraints on expectation values, this is done in the class `fake_data_for_learning.utils.ProbabilityPolytope`; see the example notebook [notebooks/conditional-probability-tables-with-constraints.ipynb](notebooks/conditional-probability-tables-with-constraints.ipynb).
+The method `fake_data_for_learning.utils.RandomCpt()` gives a random conditional probability table, but if you want to constrain the entries to satisfy constraints on expectation values, this is done in the class `fake_data_for_learning.utils.ProbabilityPolytope`; see the example notebook [notebooks/conditional-probability-tables-with-constraints.ipynb](notebooks/conditional-probability-tables-with-constraints.ipynb). See also [Optional Dependencies](#optional-dependencies) below.
 
 ## Installation
 
 Install from [pypi](https://pypi.org/project/fake-data-for-learning/): `pip install fake-data-for-learning`
 
-Note that the methods of `utils.ProbabilityPolytope` that use polytope calculatations to generate conditional probability tables subject to constraints on expectation value uses the non-pure-python library [pypoman](https://github.com/stephane-caron/pypoman). See the [installation instructions](https://github.com/stephane-caron/pypoman#installation) for external dependencies.
+### Optional dependencies
+
+Note that the methods of `utils.ProbabilityPolytope` that use polytope calculatations to generate conditional probability tables subject to constraints on expectation value use the non-pure-python library [pypoman](https://github.com/stephane-caron/pypoman). See the [installation instructions](https://github.com/stephane-caron/pypoman#installation) for external dependency instructions.
+
+By default the dependencies for `utils.ProbabilityPolytope` are not installed; to do so, run from your virtual environment `pip install 'fake-data-for-learning[probability_polytope]'`
 
 ### Local development
 
 * ``git clone`` the repository and ``cd`` into the project directory
 * Create a virtual environment from the included ``requirements.txt`` file
 
 ## Documentation
@@ -93,14 +97,18 @@
 
 * [pyagrum](https://pyagrum.readthedocs.io) is a Python wrapper around the C++ library [aGrUM](http://agrum.org/), and has similar funcionality with a larger scope. Unlike `pgmpy`, `pyagrum` has a similar API for specifying conditional probability tables to the one used here.
 
 * [causalgraphicalmodels](https://github.com/ijmbarr/causalgraphicalmodels)'s class `StructuralCausalModel` allows sampling from Bayesian network where the variables are related as functions of one another, rather than via the conditional probability tables used here.
 
 ## Change log
 
+### v0.4.3
+
+Make non-python-dependencies from `utils.ProbabilityPolytope` an optional install.
+
 ### v0.4.2
 
 Fix mac os x dependency install issue.
 
 ### v0.4.1
 
 Fix dependencies' API changes.
```

### Comparing `fake_data_for_learning-0.4.2/fake_data_for_learning/contingency_tables.py` & `fake_data_for_learning-0.4.3/fake_data_for_learning/contingency_tables.py`

 * *Files identical despite different names*

### Comparing `fake_data_for_learning-0.4.2/fake_data_for_learning/fake_data_for_learning.py` & `fake_data_for_learning-0.4.3/fake_data_for_learning/fake_data_for_learning.py`

 * *Files identical despite different names*

### Comparing `fake_data_for_learning-0.4.2/fake_data_for_learning/probability_polytopes.py` & `fake_data_for_learning-0.4.3/fake_data_for_learning/probability_polytopes.py`

 * *Files identical despite different names*

### Comparing `fake_data_for_learning-0.4.2/fake_data_for_learning/utils.py` & `fake_data_for_learning-0.4.3/fake_data_for_learning/utils.py`

 * *Files identical despite different names*

### Comparing `fake_data_for_learning-0.4.2/fake_data_for_learning.egg-info/PKG-INFO` & `fake_data_for_learning-0.4.3/fake_data_for_learning.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fake-data-for-learning
-Version: 0.4.2
+Version: 0.4.3
 Author: Paul Larsen
 Author-email: munichpavel@gmail.com
 License: MIT license
 Project-URL: Homepage, https://munichpavel.github.io/fake-data-for-learning/
 Project-URL: Bug Tracker, https://github.com/munichpavel/fake-data-for-learning/issues
 Project-URL: Documentation, https://munichpavel.github.io/fake-data-docs/html/index.html
 Project-URL: Source Code, https://github.com/munichpavel/fake-data-for-learning/
```

### Comparing `fake_data_for_learning-0.4.2/fake_data_for_learning.egg-info/SOURCES.txt` & `fake_data_for_learning-0.4.3/fake_data_for_learning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fake_data_for_learning-0.4.2/setup.py` & `fake_data_for_learning-0.4.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,21 +29,24 @@
 install_requirements = [
     'networkx>=2.4',
     'pandas>=0.25',
     'numpy',
     'scikit-learn>=0.21.3',
     'scipy>=1.3',
     'xarray',
-    'pypoman'
 ]
 
+extras_require = {
+        'probability_polytope':  ["pypoman"]
+    }
+
 
 setup(
     name='fake_data_for_learning',
-    version='0.4.2',
+    version='0.4.3',
     long_description=description,
     long_description_content_type='text/markdown',
     project_urls={
         "Homepage": "https://munichpavel.github.io/fake-data-for-learning/",
         "Bug Tracker": "https://github.com/munichpavel/fake-data-for-learning/issues",
         "Documentation": "https://munichpavel.github.io/fake-data-docs/html/index.html",
         "Source Code": "https://github.com/munichpavel/fake-data-for-learning/",
```

### Comparing `fake_data_for_learning-0.4.2/tests/test_bayesian_node_rv.py` & `fake_data_for_learning-0.4.3/tests/test_bayesian_node_rv.py`

 * *Files identical despite different names*

### Comparing `fake_data_for_learning-0.4.2/tests/test_contingency_tables.py` & `fake_data_for_learning-0.4.3/tests/test_contingency_tables.py`

 * *Files identical despite different names*

### Comparing `fake_data_for_learning-0.4.2/tests/test_demo_notebooks.py` & `fake_data_for_learning-0.4.3/tests/test_demo_notebooks.py`

 * *Files identical despite different names*

### Comparing `fake_data_for_learning-0.4.2/tests/test_fake_data_bn.py` & `fake_data_for_learning-0.4.3/tests/test_fake_data_bn.py`

 * *Files identical despite different names*

### Comparing `fake_data_for_learning-0.4.2/tests/test_probability_polytopes.py` & `fake_data_for_learning-0.4.3/tests/test_probability_polytopes.py`

 * *Files identical despite different names*

### Comparing `fake_data_for_learning-0.4.2/tests/test_utils.py` & `fake_data_for_learning-0.4.3/tests/test_utils.py`

 * *Files identical despite different names*


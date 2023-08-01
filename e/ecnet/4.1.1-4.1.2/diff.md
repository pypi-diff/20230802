# Comparing `tmp/ecnet-4.1.1.tar.gz` & `tmp/ecnet-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecnet-4.1.1.tar", last modified: Fri Apr  7 21:11:10 2023, max compression
+gzip compressed data, was "ecnet-4.1.2.tar", last modified: Tue Aug  1 22:27:09 2023, max compression
```

## Comparing `ecnet-4.1.1.tar` & `ecnet-4.1.2.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 21:11:10.290615 ecnet-4.1.1/
--rw-rw-rw-   0        0        0     1092 2023-04-07 20:45:50.000000 ecnet-4.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0      263 2023-04-07 21:11:10.290615 ecnet-4.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2797 2023-04-07 21:09:42.000000 ecnet-4.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 21:11:10.153180 ecnet-4.1.1/ecnet/
--rw-rw-rw-   0        0        0       47 2023-04-07 21:09:44.000000 ecnet-4.1.1/ecnet/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 21:11:10.178637 ecnet-4.1.1/ecnet/blends/
--rw-rw-rw-   0        0        0      189 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/blends/__init__.py
--rw-rw-rw-   0        0        0     3690 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/blends/equations.py
--rw-rw-rw-   0        0        0     3596 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/blends/predict.py
--rw-rw-rw-   0        0        0     5232 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/callbacks.py
-drwxrwxrwx   0        0        0        0 2023-04-07 21:11:10.182637 ecnet-4.1.1/ecnet/datasets/
--rw-rw-rw-   0        0        0      198 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 21:11:10.286615 ecnet-4.1.1/ecnet/datasets/data/
--rw-rw-rw-   0        0        0     2873 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/bp.smiles
--rw-rw-rw-   0        0        0      985 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/bp.target
--rw-rw-rw-   0        0        0     8824 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/cn.smiles
--rw-rw-rw-   0        0        0     1712 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/cn.target
--rw-rw-rw-   0        0        0     1399 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/cp.smiles
--rw-rw-rw-   0        0        0      173 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/cp.target
--rw-rw-rw-   0        0        0     2686 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/kv.smiles
--rw-rw-rw-   0        0        0     1465 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/kv.target
--rw-rw-rw-   0        0        0     4615 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/lhv.smiles
--rw-rw-rw-   0        0        0     1163 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/lhv.target
--rw-rw-rw-   0        0        0     4018 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/mon.smiles
--rw-rw-rw-   0        0        0     1466 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/mon.target
--rw-rw-rw-   0        0        0     2229 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/mp.smiles
--rw-rw-rw-   0        0        0      866 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/mp.target
--rw-rw-rw-   0        0        0     2075 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/pp.smiles
--rw-rw-rw-   0        0        0      159 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/pp.target
--rw-rw-rw-   0        0        0     4018 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/ron.smiles
--rw-rw-rw-   0        0        0     1543 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/ron.target
--rw-rw-rw-   0        0        0     8191 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/ysi.smiles
--rw-rw-rw-   0        0        0     2851 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/ysi.target
--rw-rw-rw-   0        0        0     9443 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/load_data.py
--rw-rw-rw-   0        0        0     7120 2023-04-07 21:09:44.000000 ecnet-4.1.1/ecnet/datasets/structs.py
--rw-rw-rw-   0        0        0     2261 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/utils.py
--rw-rw-rw-   0        0        0    10478 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/model.py
-drwxrwxrwx   0        0        0        0 2023-04-07 21:11:10.289615 ecnet-4.1.1/ecnet/tasks/
--rw-rw-rw-   0        0        0      161 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/tasks/__init__.py
--rw-rw-rw-   0        0        0     1425 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/tasks/feature_selection.py
--rw-rw-rw-   0        0        0    10850 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/tasks/parameter_tuning.py
-drwxrwxrwx   0        0        0        0 2023-04-07 21:11:10.175635 ecnet-4.1.1/ecnet.egg-info/
--rw-rw-rw-   0        0        0      263 2023-04-07 21:11:10.000000 ecnet-4.1.1/ecnet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1131 2023-04-07 21:11:10.000000 ecnet-4.1.1/ecnet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 21:11:10.000000 ecnet-4.1.1/ecnet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-07 21:11:10.000000 ecnet-4.1.1/ecnet.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       80 2023-04-07 21:11:10.000000 ecnet-4.1.1/ecnet.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-07 21:11:10.000000 ecnet-4.1.1/ecnet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-07 21:11:10.290615 ecnet-4.1.1/setup.cfg
--rw-rw-rw-   0        0        0      598 2023-04-07 21:09:44.000000 ecnet-4.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:27:09.390822 ecnet-4.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-01 22:26:59.000000 ecnet-4.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-08-01 22:27:09.390822 ecnet-4.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-08-01 22:26:59.000000 ecnet-4.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:27:09.386822 ecnet-4.1.2/ecnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:27:09.386822 ecnet-4.1.2/ecnet/blends/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/blends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/blends/equations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/blends/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:27:09.386822 ecnet-4.1.2/ecnet/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:27:09.390822 ecnet-4.1.2/ecnet/datasets/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/datasets/data/bp.smiles
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/datasets/data/bp.target
+-rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/datasets/data/cn.smiles
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/datasets/data/cn.target
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/datasets/data/cp.smiles
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/datasets/data/cp.target
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/datasets/data/kv.smiles
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/datasets/data/kv.target
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/datasets/data/lhv.smiles
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/datasets/data/lhv.target
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/datasets/data/mon.smiles
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/datasets/data/mon.target
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/datasets/data/mp.smiles
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/datasets/data/mp.target
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/datasets/data/pp.smiles
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/datasets/data/pp.target
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/datasets/data/ron.smiles
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/datasets/data/ron.target
+-rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/datasets/data/ysi.smiles
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/datasets/data/ysi.target
+-rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/datasets/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/datasets/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10478 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:27:09.390822 ecnet-4.1.2/ecnet/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/tasks/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10850 2023-08-01 22:26:59.000000 ecnet-4.1.2/ecnet/tasks/parameter_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:27:09.386822 ecnet-4.1.2/ecnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-08-01 22:27:09.000000 ecnet-4.1.2/ecnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-08-01 22:27:09.000000 ecnet-4.1.2/ecnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 22:27:09.000000 ecnet-4.1.2/ecnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-01 22:27:09.000000 ecnet-4.1.2/ecnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-01 22:27:09.000000 ecnet-4.1.2/ecnet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-01 22:26:59.000000 ecnet-4.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 22:27:09.390822 ecnet-4.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:27:09.390822 ecnet-4.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8088 2023-08-01 22:26:59.000000 ecnet-4.1.2/tests/test_all.py
```

### Comparing `ecnet-4.1.1/LICENSE.txt` & `ecnet-4.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.1/README.md` & `ecnet-4.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # ECNet: machine learning models for fuel property prediction
 
 [![GitHub version](https://badge.fury.io/gh/ecrl%2FECNet.svg)](https://badge.fury.io/gh/ecrl%2FECNet)
 [![PyPI version](https://badge.fury.io/py/ecnet.svg)](https://badge.fury.io/py/ecnet)
 [![status](http://joss.theoj.org/papers/f556afbc97e18e1c1294d98e0f7ff99f/status.svg)](http://joss.theoj.org/papers/f556afbc97e18e1c1294d98e0f7ff99f)
 [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/ECRL/ECNet/master/LICENSE.txt)
 [![Documentation Status](https://readthedocs.org/projects/ecnet/badge/?version=latest)](https://ecnet.readthedocs.io/en/latest/?badge=latest)
-[![Build Status](https://dev.azure.com/uml-ecrl/package-management/_apis/build/status/ECRL.ECNet?branchName=master)](https://dev.azure.com/uml-ecrl/package-management/_build/latest?definitionId=1&branchName=master)
 	
 **ECNet** is an open source Python package for creating machine learning models to predict fuel properties. ECNet comes bundled with a variety of fuel property datasets, including cetane number, yield sooting index, and research/motor octane number. ECNet was built using the [PyTorch](https://pytorch.org/) library, allowing easy implementation of our models in your existing ML pipelines.
 
 ECNet leverages [QSPR descriptors](https://en.wikipedia.org/wiki/Quantitative_structure%E2%80%93activity_relationship) for use as input variables, specifically [PaDEL-Descriptor](http://www.yapcwsoft.com/dd/padeldescriptor/) and [alvaDesc](https://www.alvascience.com/alvadesc/). Using alvaDesc requires a valid license.
 
 Future plans for ECNet include:
 - Implementating RDKit to train using molecular fingerprints
```

### Comparing `ecnet-4.1.1/ecnet/blends/equations.py` & `ecnet-4.1.2/ecnet/blends/equations.py`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.1/ecnet/blends/predict.py` & `ecnet-4.1.2/ecnet/blends/predict.py`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.1/ecnet/callbacks.py` & `ecnet-4.1.2/ecnet/callbacks.py`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.1/ecnet/datasets/data/bp.smiles` & `ecnet-4.1.2/ecnet/datasets/data/bp.smiles`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.1/ecnet/datasets/data/bp.target` & `ecnet-4.1.2/ecnet/datasets/data/bp.target`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.1/ecnet/datasets/data/cn.smiles` & `ecnet-4.1.2/ecnet/datasets/data/cn.smiles`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.1/ecnet/datasets/data/cn.target` & `ecnet-4.1.2/ecnet/datasets/data/cn.target`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.1/ecnet/datasets/data/kv.smiles` & `ecnet-4.1.2/ecnet/datasets/data/kv.smiles`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.1/ecnet/datasets/data/kv.target` & `ecnet-4.1.2/ecnet/datasets/data/kv.target`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.1/ecnet/datasets/data/lhv.smiles` & `ecnet-4.1.2/ecnet/datasets/data/lhv.smiles`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.1/ecnet/datasets/data/lhv.target` & `ecnet-4.1.2/ecnet/datasets/data/lhv.target`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.1/ecnet/datasets/data/mon.smiles` & `ecnet-4.1.2/ecnet/datasets/data/mon.smiles`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.1/ecnet/datasets/data/mon.target` & `ecnet-4.1.2/ecnet/datasets/data/mon.target`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.1/ecnet/datasets/data/mp.smiles` & `ecnet-4.1.2/ecnet/datasets/data/mp.smiles`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.1/ecnet/datasets/data/mp.target` & `ecnet-4.1.2/ecnet/datasets/data/mp.target`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.1/ecnet/datasets/data/pp.smiles` & `ecnet-4.1.2/ecnet/datasets/data/pp.smiles`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.1/ecnet/datasets/data/ron.smiles` & `ecnet-4.1.2/ecnet/datasets/data/ron.smiles`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.1/ecnet/datasets/data/ron.target` & `ecnet-4.1.2/ecnet/datasets/data/ron.target`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.1/ecnet/datasets/data/ysi.smiles` & `ecnet-4.1.2/ecnet/datasets/data/ysi.smiles`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.1/ecnet/datasets/data/ysi.target` & `ecnet-4.1.2/ecnet/datasets/data/ysi.target`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.1/ecnet/datasets/load_data.py` & `ecnet-4.1.2/ecnet/datasets/load_data.py`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.1/ecnet/datasets/structs.py` & `ecnet-4.1.2/ecnet/datasets/structs.py`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.1/ecnet/datasets/utils.py` & `ecnet-4.1.2/ecnet/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.1/ecnet/model.py` & `ecnet-4.1.2/ecnet/model.py`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.1/ecnet/tasks/feature_selection.py` & `ecnet-4.1.2/ecnet/tasks/feature_selection.py`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.1/ecnet/tasks/parameter_tuning.py` & `ecnet-4.1.2/ecnet/tasks/parameter_tuning.py`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.1/ecnet.egg-info/SOURCES.txt` & `ecnet-4.1.2/ecnet.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 LICENSE.txt
 README.md
-setup.py
+pyproject.toml
 ecnet/__init__.py
 ecnet/callbacks.py
 ecnet/model.py
 ecnet.egg-info/PKG-INFO
 ecnet.egg-info/SOURCES.txt
 ecnet.egg-info/dependency_links.txt
-ecnet.egg-info/not-zip-safe
 ecnet.egg-info/requires.txt
 ecnet.egg-info/top_level.txt
 ecnet/blends/__init__.py
 ecnet/blends/equations.py
 ecnet/blends/predict.py
 ecnet/datasets/__init__.py
 ecnet/datasets/load_data.py
@@ -35,8 +34,9 @@
 ecnet/datasets/data/pp.target
 ecnet/datasets/data/ron.smiles
 ecnet/datasets/data/ron.target
 ecnet/datasets/data/ysi.smiles
 ecnet/datasets/data/ysi.target
 ecnet/tasks/__init__.py
 ecnet/tasks/feature_selection.py
-ecnet/tasks/parameter_tuning.py
+ecnet/tasks/parameter_tuning.py
+tests/test_all.py
```


# Comparing `tmp/manic-xai-1.0.6.tar.gz` & `tmp/manic-xai-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manic-xai-1.0.6.tar", last modified: Wed Aug  2 20:29:01 2023, max compression
+gzip compressed data, was "manic-xai-1.0.7.tar", last modified: Wed Aug  2 20:38:33 2023, max compression
```

## Comparing `manic-xai-1.0.6.tar` & `manic-xai-1.0.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-08-02 20:29:01.782702 manic-xai-1.0.6/
--rw-r--r--   0 craigpirie   (501) staff       (20)     1064 2023-07-26 15:54:10.000000 manic-xai-1.0.6/LICENSE
--rw-r--r--   0 craigpirie   (501) staff       (20)     3261 2023-08-02 20:29:01.782392 manic-xai-1.0.6/PKG-INFO
--rw-r--r--   0 craigpirie   (501) staff       (20)     2721 2023-07-26 17:17:12.000000 manic-xai-1.0.6/README.md
-drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-08-02 20:29:01.775084 manic-xai-1.0.6/manic/
--rw-r--r--   0 craigpirie   (501) staff       (20)     2845 2023-08-01 23:21:50.000000 manic-xai-1.0.6/manic/Baseline.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     6369 2023-08-02 20:20:39.000000 manic-xai-1.0.6/manic/Crossover.py
--rw-r--r--   0 craigpirie   (501) staff       (20)    10944 2023-08-02 17:39:33.000000 manic-xai-1.0.6/manic/Disagreement.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     6987 2023-08-01 23:28:50.000000 manic-xai-1.0.6/manic/Evaluation.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     6644 2023-08-02 20:15:27.000000 manic-xai-1.0.6/manic/GeneticAlgorithm.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     7534 2023-08-02 20:15:40.000000 manic-xai-1.0.6/manic/Manic.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     5614 2023-08-01 23:32:04.000000 manic-xai-1.0.6/manic/Mutation.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     1563 2023-08-02 17:56:19.000000 manic-xai-1.0.6/manic/Replacement.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     7213 2023-08-02 17:44:55.000000 manic-xai-1.0.6/manic/Selection.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     1824 2023-08-01 22:52:00.000000 manic-xai-1.0.6/manic/Termination.py
--rw-r--r--   0 craigpirie   (501) staff       (20)    10672 2023-08-02 20:09:42.000000 manic-xai-1.0.6/manic/Utility.py
--rw-r--r--   0 craigpirie   (501) staff       (20)      471 2023-08-02 20:25:11.000000 manic-xai-1.0.6/manic/__init__.py
-drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-08-02 20:29:01.780364 manic-xai-1.0.6/manic/__tests__/
--rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-27 23:28:48.000000 manic-xai-1.0.6/manic/__tests__/__init__.py
--rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:45:16.000000 manic-xai-1.0.6/manic/__tests__/test_baseline.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     1905 2023-07-28 17:41:26.000000 manic-xai-1.0.6/manic/__tests__/test_crossover.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     5034 2023-07-28 16:53:03.000000 manic-xai-1.0.6/manic/__tests__/test_disagreement.py
--rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:45:35.000000 manic-xai-1.0.6/manic/__tests__/test_evaluation.py
--rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-31 01:59:12.000000 manic-xai-1.0.6/manic/__tests__/test_genetic_algorithm.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     1269 2023-07-26 17:02:40.000000 manic-xai-1.0.6/manic/__tests__/test_manic.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     4387 2023-07-28 14:27:49.000000 manic-xai-1.0.6/manic/__tests__/test_mutation.py
--rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-08-01 22:24:47.000000 manic-xai-1.0.6/manic/__tests__/test_replacement.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     9470 2023-07-28 15:04:45.000000 manic-xai-1.0.6/manic/__tests__/test_selection.py
--rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:45:43.000000 manic-xai-1.0.6/manic/__tests__/test_termination.py
--rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:46:05.000000 manic-xai-1.0.6/manic/__tests__/test_utility.py
-drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-08-02 20:29:01.781886 manic-xai-1.0.6/manic_xai.egg-info/
--rw-r--r--   0 craigpirie   (501) staff       (20)     3261 2023-08-02 20:29:01.000000 manic-xai-1.0.6/manic_xai.egg-info/PKG-INFO
--rw-r--r--   0 craigpirie   (501) staff       (20)      834 2023-08-02 20:29:01.000000 manic-xai-1.0.6/manic_xai.egg-info/SOURCES.txt
--rw-r--r--   0 craigpirie   (501) staff       (20)        1 2023-08-02 20:29:01.000000 manic-xai-1.0.6/manic_xai.egg-info/dependency_links.txt
--rw-r--r--   0 craigpirie   (501) staff       (20)       69 2023-08-02 20:29:01.000000 manic-xai-1.0.6/manic_xai.egg-info/requires.txt
--rw-r--r--   0 craigpirie   (501) staff       (20)        6 2023-08-02 20:29:01.000000 manic-xai-1.0.6/manic_xai.egg-info/top_level.txt
--rw-r--r--   0 craigpirie   (501) staff       (20)       38 2023-08-02 20:29:01.782819 manic-xai-1.0.6/setup.cfg
--rw-r--r--   0 craigpirie   (501) staff       (20)     1041 2023-08-02 20:28:46.000000 manic-xai-1.0.6/setup.py
+drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-08-02 20:38:33.127847 manic-xai-1.0.7/
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1064 2023-07-26 15:54:10.000000 manic-xai-1.0.7/LICENSE
+-rw-r--r--   0 craigpirie   (501) staff       (20)     3261 2023-08-02 20:38:33.127448 manic-xai-1.0.7/PKG-INFO
+-rw-r--r--   0 craigpirie   (501) staff       (20)     2721 2023-07-26 17:17:12.000000 manic-xai-1.0.7/README.md
+drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-08-02 20:38:33.114943 manic-xai-1.0.7/manic/
+-rw-r--r--   0 craigpirie   (501) staff       (20)     2845 2023-08-01 23:21:50.000000 manic-xai-1.0.7/manic/Baseline.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     6369 2023-08-02 20:20:39.000000 manic-xai-1.0.7/manic/Crossover.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)    10944 2023-08-02 17:39:33.000000 manic-xai-1.0.7/manic/Disagreement.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     6987 2023-08-01 23:28:50.000000 manic-xai-1.0.7/manic/Evaluation.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     6644 2023-08-02 20:15:27.000000 manic-xai-1.0.7/manic/GeneticAlgorithm.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     7248 2023-08-02 20:37:56.000000 manic-xai-1.0.7/manic/Manic.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     5614 2023-08-01 23:32:04.000000 manic-xai-1.0.7/manic/Mutation.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1563 2023-08-02 17:56:19.000000 manic-xai-1.0.7/manic/Replacement.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     7213 2023-08-02 17:44:55.000000 manic-xai-1.0.7/manic/Selection.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1824 2023-08-01 22:52:00.000000 manic-xai-1.0.7/manic/Termination.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)    10672 2023-08-02 20:09:42.000000 manic-xai-1.0.7/manic/Utility.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)      471 2023-08-02 20:25:11.000000 manic-xai-1.0.7/manic/__init__.py
+drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-08-02 20:38:33.123523 manic-xai-1.0.7/manic/__tests__/
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-27 23:28:48.000000 manic-xai-1.0.7/manic/__tests__/__init__.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:45:16.000000 manic-xai-1.0.7/manic/__tests__/test_baseline.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1905 2023-07-28 17:41:26.000000 manic-xai-1.0.7/manic/__tests__/test_crossover.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     5034 2023-07-28 16:53:03.000000 manic-xai-1.0.7/manic/__tests__/test_disagreement.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:45:35.000000 manic-xai-1.0.7/manic/__tests__/test_evaluation.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-31 01:59:12.000000 manic-xai-1.0.7/manic/__tests__/test_genetic_algorithm.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1269 2023-07-26 17:02:40.000000 manic-xai-1.0.7/manic/__tests__/test_manic.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     4387 2023-07-28 14:27:49.000000 manic-xai-1.0.7/manic/__tests__/test_mutation.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-08-01 22:24:47.000000 manic-xai-1.0.7/manic/__tests__/test_replacement.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     9470 2023-07-28 15:04:45.000000 manic-xai-1.0.7/manic/__tests__/test_selection.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:45:43.000000 manic-xai-1.0.7/manic/__tests__/test_termination.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:46:05.000000 manic-xai-1.0.7/manic/__tests__/test_utility.py
+drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-08-02 20:38:33.126803 manic-xai-1.0.7/manic_xai.egg-info/
+-rw-r--r--   0 craigpirie   (501) staff       (20)     3261 2023-08-02 20:38:33.000000 manic-xai-1.0.7/manic_xai.egg-info/PKG-INFO
+-rw-r--r--   0 craigpirie   (501) staff       (20)      834 2023-08-02 20:38:33.000000 manic-xai-1.0.7/manic_xai.egg-info/SOURCES.txt
+-rw-r--r--   0 craigpirie   (501) staff       (20)        1 2023-08-02 20:38:33.000000 manic-xai-1.0.7/manic_xai.egg-info/dependency_links.txt
+-rw-r--r--   0 craigpirie   (501) staff       (20)       69 2023-08-02 20:38:33.000000 manic-xai-1.0.7/manic_xai.egg-info/requires.txt
+-rw-r--r--   0 craigpirie   (501) staff       (20)        6 2023-08-02 20:38:33.000000 manic-xai-1.0.7/manic_xai.egg-info/top_level.txt
+-rw-r--r--   0 craigpirie   (501) staff       (20)       38 2023-08-02 20:38:33.127990 manic-xai-1.0.7/setup.cfg
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1041 2023-08-02 20:38:19.000000 manic-xai-1.0.7/setup.py
```

### Comparing `manic-xai-1.0.6/LICENSE` & `manic-xai-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.6/PKG-INFO` & `manic-xai-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manic-xai
-Version: 1.0.6
+Version: 1.0.7
 Summary: Genetic Algorithm for Generating Metacounterfactual Explanations
 Home-page: https://github.com/craigybaeb/MANIC
 Author: Craig Pirie
 Author-email: c.pirie11@rgu.ac.uk
 Keywords: manic,metacounterfactual,counterfactual,xai,explanation,aggregation,disagreement,agreement
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `manic-xai-1.0.6/README.md` & `manic-xai-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.6/manic/Baseline.py` & `manic-xai-1.0.7/manic/Baseline.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.6/manic/Crossover.py` & `manic-xai-1.0.7/manic/Crossover.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.6/manic/Disagreement.py` & `manic-xai-1.0.7/manic/Disagreement.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.6/manic/Evaluation.py` & `manic-xai-1.0.7/manic/Evaluation.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.6/manic/GeneticAlgorithm.py` & `manic-xai-1.0.7/manic/GeneticAlgorithm.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.6/manic/Manic.py` & `manic-xai-1.0.7/manic/Manic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,12 @@
 import heapq
 import random 
 import numpy as np
 
-from Baseline import Baseline
-from Crossover import Crossover
-from Disagreement import Disagreement
-from Evaluation import Evaluation
-from GeneticAlgorithm import GeneticAlgorithm
-from Mutation import Mutation
-from Replacement import Replacement
-from Selection import Selection
-from Utility import Utility
+from manic import *
 
 class Manic:
     def __init__(self, data_instance, base_counterfactuals, categorical_features, immutable_features, feature_ranges, data, predict_fn, predict_proba_fn, class_labels, population_size=100, num_generations=50, alpha=0.5, beta=0.5, crossover_method="uniform", mutation_method="random_resetting", perturbation_fraction=0.1, num_parents=2, seed=42, verbose=1, early_stopping=None, max_time=None, disagreement_method="euclidean_distance", theta=0.3, parallel=False, labels=[]):
         self.immutable_features_set = set(immutable_features)
         self.data = data
         self.data_instance = data_instance
         self.categorical_features = categorical_features
```

### Comparing `manic-xai-1.0.6/manic/Mutation.py` & `manic-xai-1.0.7/manic/Mutation.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.6/manic/Replacement.py` & `manic-xai-1.0.7/manic/Replacement.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.6/manic/Selection.py` & `manic-xai-1.0.7/manic/Selection.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.6/manic/Termination.py` & `manic-xai-1.0.7/manic/Termination.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.6/manic/Utility.py` & `manic-xai-1.0.7/manic/Utility.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.6/manic/__tests__/test_crossover.py` & `manic-xai-1.0.7/manic/__tests__/test_crossover.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.6/manic/__tests__/test_disagreement.py` & `manic-xai-1.0.7/manic/__tests__/test_disagreement.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.6/manic/__tests__/test_manic.py` & `manic-xai-1.0.7/manic/__tests__/test_manic.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.6/manic/__tests__/test_mutation.py` & `manic-xai-1.0.7/manic/__tests__/test_mutation.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.6/manic/__tests__/test_selection.py` & `manic-xai-1.0.7/manic/__tests__/test_selection.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.6/manic_xai.egg-info/PKG-INFO` & `manic-xai-1.0.7/manic_xai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manic-xai
-Version: 1.0.6
+Version: 1.0.7
 Summary: Genetic Algorithm for Generating Metacounterfactual Explanations
 Home-page: https://github.com/craigybaeb/MANIC
 Author: Craig Pirie
 Author-email: c.pirie11@rgu.ac.uk
 Keywords: manic,metacounterfactual,counterfactual,xai,explanation,aggregation,disagreement,agreement
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `manic-xai-1.0.6/manic_xai.egg-info/SOURCES.txt` & `manic-xai-1.0.7/manic_xai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.6/setup.py` & `manic-xai-1.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="manic-xai",
-    version='1.0.6',
+    version='1.0.7',
     author="Craig Pirie",
     author_email="c.pirie11@rgu.ac.uk",
     description="Genetic Algorithm for Generating Metacounterfactual Explanations",
     url = "https://github.com/craigybaeb/MANIC",
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
```


# Comparing `tmp/manic-xai-1.0.5.tar.gz` & `tmp/manic-xai-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manic-xai-1.0.5.tar", last modified: Wed Aug  2 20:20:45 2023, max compression
+gzip compressed data, was "manic-xai-1.0.6.tar", last modified: Wed Aug  2 20:29:01 2023, max compression
```

## Comparing `manic-xai-1.0.5.tar` & `manic-xai-1.0.6.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-08-02 20:20:45.387708 manic-xai-1.0.5/
--rw-r--r--   0 craigpirie   (501) staff       (20)     1064 2023-07-26 15:54:10.000000 manic-xai-1.0.5/LICENSE
--rw-r--r--   0 craigpirie   (501) staff       (20)     3261 2023-08-02 20:20:45.387464 manic-xai-1.0.5/PKG-INFO
--rw-r--r--   0 craigpirie   (501) staff       (20)     2721 2023-07-26 17:17:12.000000 manic-xai-1.0.5/README.md
-drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-08-02 20:20:45.379816 manic-xai-1.0.5/manic/
--rw-r--r--   0 craigpirie   (501) staff       (20)     2845 2023-08-01 23:21:50.000000 manic-xai-1.0.5/manic/Baseline.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     6369 2023-08-02 20:20:39.000000 manic-xai-1.0.5/manic/Crossover.py
--rw-r--r--   0 craigpirie   (501) staff       (20)    10944 2023-08-02 17:39:33.000000 manic-xai-1.0.5/manic/Disagreement.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     6987 2023-08-01 23:28:50.000000 manic-xai-1.0.5/manic/Evaluation.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     6644 2023-08-02 20:15:27.000000 manic-xai-1.0.5/manic/GeneticAlgorithm.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     5509 2023-07-31 00:24:07.000000 manic-xai-1.0.5/manic/Initialise.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     7534 2023-08-02 20:15:40.000000 manic-xai-1.0.5/manic/Manic.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     5614 2023-08-01 23:32:04.000000 manic-xai-1.0.5/manic/Mutation.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     1563 2023-08-02 17:56:19.000000 manic-xai-1.0.5/manic/Replacement.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     7213 2023-08-02 17:44:55.000000 manic-xai-1.0.5/manic/Selection.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     1824 2023-08-01 22:52:00.000000 manic-xai-1.0.5/manic/Termination.py
--rw-r--r--   0 craigpirie   (501) staff       (20)    10672 2023-08-02 20:09:42.000000 manic-xai-1.0.5/manic/Utility.py
--rw-r--r--   0 craigpirie   (501) staff       (20)      520 2023-08-01 22:24:38.000000 manic-xai-1.0.5/manic/__init__.py
-drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-08-02 20:20:45.385636 manic-xai-1.0.5/manic/__tests__/
--rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-27 23:28:48.000000 manic-xai-1.0.5/manic/__tests__/__init__.py
--rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:45:16.000000 manic-xai-1.0.5/manic/__tests__/test_baseline.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     1905 2023-07-28 17:41:26.000000 manic-xai-1.0.5/manic/__tests__/test_crossover.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     5034 2023-07-28 16:53:03.000000 manic-xai-1.0.5/manic/__tests__/test_disagreement.py
--rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:45:35.000000 manic-xai-1.0.5/manic/__tests__/test_evaluation.py
--rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-31 01:59:12.000000 manic-xai-1.0.5/manic/__tests__/test_genetic_algorithm.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     1269 2023-07-26 17:02:40.000000 manic-xai-1.0.5/manic/__tests__/test_manic.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     4387 2023-07-28 14:27:49.000000 manic-xai-1.0.5/manic/__tests__/test_mutation.py
--rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-08-01 22:24:47.000000 manic-xai-1.0.5/manic/__tests__/test_replacement.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     9470 2023-07-28 15:04:45.000000 manic-xai-1.0.5/manic/__tests__/test_selection.py
--rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:45:43.000000 manic-xai-1.0.5/manic/__tests__/test_termination.py
--rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:46:05.000000 manic-xai-1.0.5/manic/__tests__/test_utility.py
-drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-08-02 20:20:45.387100 manic-xai-1.0.5/manic_xai.egg-info/
--rw-r--r--   0 craigpirie   (501) staff       (20)     3261 2023-08-02 20:20:45.000000 manic-xai-1.0.5/manic_xai.egg-info/PKG-INFO
--rw-r--r--   0 craigpirie   (501) staff       (20)      854 2023-08-02 20:20:45.000000 manic-xai-1.0.5/manic_xai.egg-info/SOURCES.txt
--rw-r--r--   0 craigpirie   (501) staff       (20)        1 2023-08-02 20:20:45.000000 manic-xai-1.0.5/manic_xai.egg-info/dependency_links.txt
--rw-r--r--   0 craigpirie   (501) staff       (20)       69 2023-08-02 20:20:45.000000 manic-xai-1.0.5/manic_xai.egg-info/requires.txt
--rw-r--r--   0 craigpirie   (501) staff       (20)        6 2023-08-02 20:20:45.000000 manic-xai-1.0.5/manic_xai.egg-info/top_level.txt
--rw-r--r--   0 craigpirie   (501) staff       (20)       38 2023-08-02 20:20:45.387781 manic-xai-1.0.5/setup.cfg
--rw-r--r--   0 craigpirie   (501) staff       (20)     1041 2023-08-02 20:20:39.000000 manic-xai-1.0.5/setup.py
+drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-08-02 20:29:01.782702 manic-xai-1.0.6/
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1064 2023-07-26 15:54:10.000000 manic-xai-1.0.6/LICENSE
+-rw-r--r--   0 craigpirie   (501) staff       (20)     3261 2023-08-02 20:29:01.782392 manic-xai-1.0.6/PKG-INFO
+-rw-r--r--   0 craigpirie   (501) staff       (20)     2721 2023-07-26 17:17:12.000000 manic-xai-1.0.6/README.md
+drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-08-02 20:29:01.775084 manic-xai-1.0.6/manic/
+-rw-r--r--   0 craigpirie   (501) staff       (20)     2845 2023-08-01 23:21:50.000000 manic-xai-1.0.6/manic/Baseline.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     6369 2023-08-02 20:20:39.000000 manic-xai-1.0.6/manic/Crossover.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)    10944 2023-08-02 17:39:33.000000 manic-xai-1.0.6/manic/Disagreement.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     6987 2023-08-01 23:28:50.000000 manic-xai-1.0.6/manic/Evaluation.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     6644 2023-08-02 20:15:27.000000 manic-xai-1.0.6/manic/GeneticAlgorithm.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     7534 2023-08-02 20:15:40.000000 manic-xai-1.0.6/manic/Manic.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     5614 2023-08-01 23:32:04.000000 manic-xai-1.0.6/manic/Mutation.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1563 2023-08-02 17:56:19.000000 manic-xai-1.0.6/manic/Replacement.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     7213 2023-08-02 17:44:55.000000 manic-xai-1.0.6/manic/Selection.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1824 2023-08-01 22:52:00.000000 manic-xai-1.0.6/manic/Termination.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)    10672 2023-08-02 20:09:42.000000 manic-xai-1.0.6/manic/Utility.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)      471 2023-08-02 20:25:11.000000 manic-xai-1.0.6/manic/__init__.py
+drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-08-02 20:29:01.780364 manic-xai-1.0.6/manic/__tests__/
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-27 23:28:48.000000 manic-xai-1.0.6/manic/__tests__/__init__.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:45:16.000000 manic-xai-1.0.6/manic/__tests__/test_baseline.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1905 2023-07-28 17:41:26.000000 manic-xai-1.0.6/manic/__tests__/test_crossover.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     5034 2023-07-28 16:53:03.000000 manic-xai-1.0.6/manic/__tests__/test_disagreement.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:45:35.000000 manic-xai-1.0.6/manic/__tests__/test_evaluation.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-31 01:59:12.000000 manic-xai-1.0.6/manic/__tests__/test_genetic_algorithm.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1269 2023-07-26 17:02:40.000000 manic-xai-1.0.6/manic/__tests__/test_manic.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     4387 2023-07-28 14:27:49.000000 manic-xai-1.0.6/manic/__tests__/test_mutation.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-08-01 22:24:47.000000 manic-xai-1.0.6/manic/__tests__/test_replacement.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     9470 2023-07-28 15:04:45.000000 manic-xai-1.0.6/manic/__tests__/test_selection.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:45:43.000000 manic-xai-1.0.6/manic/__tests__/test_termination.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:46:05.000000 manic-xai-1.0.6/manic/__tests__/test_utility.py
+drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-08-02 20:29:01.781886 manic-xai-1.0.6/manic_xai.egg-info/
+-rw-r--r--   0 craigpirie   (501) staff       (20)     3261 2023-08-02 20:29:01.000000 manic-xai-1.0.6/manic_xai.egg-info/PKG-INFO
+-rw-r--r--   0 craigpirie   (501) staff       (20)      834 2023-08-02 20:29:01.000000 manic-xai-1.0.6/manic_xai.egg-info/SOURCES.txt
+-rw-r--r--   0 craigpirie   (501) staff       (20)        1 2023-08-02 20:29:01.000000 manic-xai-1.0.6/manic_xai.egg-info/dependency_links.txt
+-rw-r--r--   0 craigpirie   (501) staff       (20)       69 2023-08-02 20:29:01.000000 manic-xai-1.0.6/manic_xai.egg-info/requires.txt
+-rw-r--r--   0 craigpirie   (501) staff       (20)        6 2023-08-02 20:29:01.000000 manic-xai-1.0.6/manic_xai.egg-info/top_level.txt
+-rw-r--r--   0 craigpirie   (501) staff       (20)       38 2023-08-02 20:29:01.782819 manic-xai-1.0.6/setup.cfg
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1041 2023-08-02 20:28:46.000000 manic-xai-1.0.6/setup.py
```

### Comparing `manic-xai-1.0.5/LICENSE` & `manic-xai-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.5/PKG-INFO` & `manic-xai-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manic-xai
-Version: 1.0.5
+Version: 1.0.6
 Summary: Genetic Algorithm for Generating Metacounterfactual Explanations
 Home-page: https://github.com/craigybaeb/MANIC
 Author: Craig Pirie
 Author-email: c.pirie11@rgu.ac.uk
 Keywords: manic,metacounterfactual,counterfactual,xai,explanation,aggregation,disagreement,agreement
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `manic-xai-1.0.5/README.md` & `manic-xai-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.5/manic/Baseline.py` & `manic-xai-1.0.6/manic/Baseline.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.5/manic/Crossover.py` & `manic-xai-1.0.6/manic/Crossover.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.5/manic/Disagreement.py` & `manic-xai-1.0.6/manic/Disagreement.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.5/manic/Evaluation.py` & `manic-xai-1.0.6/manic/Evaluation.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.5/manic/GeneticAlgorithm.py` & `manic-xai-1.0.6/manic/GeneticAlgorithm.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.5/manic/Initialise.py` & `manic-xai-1.0.6/manic/Manic.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,72 @@
-import random
 import heapq
+import random 
 import numpy as np
 
 from Baseline import Baseline
+from Crossover import Crossover
 from Disagreement import Disagreement
 from Evaluation import Evaluation
+from GeneticAlgorithm import GeneticAlgorithm
+from Mutation import Mutation
+from Replacement import Replacement
 from Selection import Selection
 from Utility import Utility
 
-class Initialise:
-    def __init__(self, disagreement_method, data_instance, base_counterfactuals, predict_fn, predict_proba_fn, seed, population_size, categorical_features, feature_ranges, immutable_features, data, class_labels, theta, alpha, beta, num_parents, verbose, labels, parallel):
-        self.seed = seed
-        self.population_size = population_size
-        self.base_counterfactuals = base_counterfactuals
+class Manic:
+    def __init__(self, data_instance, base_counterfactuals, categorical_features, immutable_features, feature_ranges, data, predict_fn, predict_proba_fn, class_labels, population_size=100, num_generations=50, alpha=0.5, beta=0.5, crossover_method="uniform", mutation_method="random_resetting", perturbation_fraction=0.1, num_parents=2, seed=42, verbose=1, early_stopping=None, max_time=None, disagreement_method="euclidean_distance", theta=0.3, parallel=False, labels=[]):
+        self.immutable_features_set = set(immutable_features)
         self.data = data
-        self.class_labels = class_labels
-        self.categorical_features = categorical_features
         self.data_instance = data_instance
-        self.parallel = parallel
-        self.immutable_features_set = set(immutable_features)
+        self.categorical_features = categorical_features
+        self.base_counterfactuals = base_counterfactuals
+        self.population_size = population_size
+        self.labels = labels if labels else list(range(1, len(base_counterfactuals) + 1))
+        self.class_labels = class_labels
+        self.num_generations = num_generations
+        self.alpha = alpha
+        self.beta = beta
+        self.seed = seed
+        self.theta = theta
+        self.target_class = 1 - predict_fn(data_instance) #TODO don't assume binary classification
         self.categories = self.get_categories(categorical_features)
         self.feature_ranges = self.get_feature_ranges(feature_ranges)
-        self.target_class = 1 - predict_fn(data_instance) #TODO don't assume binary classification
         self.disagreement = Disagreement(disagreement_method, data_instance, base_counterfactuals, categorical_features, feature_ranges, predict_fn, predict_proba_fn, self.target_class, self.feature_ranges)
+        self.population = self.initialise_population()
+        self.categorical_features = categorical_features
+        self.immutable_features = immutable_features
+        self.crossover = Crossover(crossover_method, num_parents, population_size, parallel).crossover
+        self.mutate = Mutation(mutation_method, perturbation_fraction, self.feature_ranges).mutate
+        self.selection = Selection(num_parents, self.target_class, population_size, predict_fn, parallel)
         self.instance_probability = predict_proba_fn(data_instance)
         self.evaluation = Evaluation(alpha, beta, predict_proba_fn, self.instance_probability, base_counterfactuals, self.disagreement, data_instance, theta, parallel)
-        self.selection = Selection(num_parents, self.target_class, population_size, predict_fn, parallel)
-        self.utils = Utility(data_instance, self.categories, immutable_features, self.target_class, verbose, predict_fn, self.disagreement, base_counterfactuals, self.evaluation, labels)
-        self.population = self.initialise_population()
+        self.replacement = Replacement(self.crossover, self.mutate, self.evaluation, self.selection)
         self.baseline = Baseline(self.disagreement, base_counterfactuals, data_instance)
+        self.utils = Utility(data_instance, self.categories, immutable_features, self.target_class, verbose, predict_fn, self.disagreement, base_counterfactuals, self.labels)
+        self.is_counterfactual_valid = self.utils.is_counterfactual_valid
+        self.print_results = self.utils.print_results
+        self.generate_counterfactuals = GeneticAlgorithm(num_generations, early_stopping, predict_fn, self.evaluation, self.selection, self.crossover, self.mutate, verbose, self.target_class, max_time, self.utils, self.replacement, self.population, base_counterfactuals, data_instance).generate_counterfactuals
+
+    def __str__(self):
+        attributes_str = [
+            f"categorical_features: {self.categorical_features}",
+            f"immutable_features: {self.immutable_features}",
+            f"population_size: {self.population_size}",
+            f"num_generations: {self.num_generations}",
+            f"target_class: {self.target_class}",
+            f"continuous_feature_ranges: {self.continuous_feature_ranges}",
+            f"categories: {self.categories}",
+            f"feature_ranges: {self.feature_ranges}",
+            f"verbose: {self.verbose}"
+        ]
+        return "\n".join(attributes_str)
 
+    def to_string(self):
+        return str(self)
+    
     def weighted_random_choice(self, options, weights):
         return random.choices(options, weights, k=1)[0]
 
     def initialise_population(self):
         random.seed(self.seed)
         population = []
         options = [self.generate_random_instance, self.nearest_unlike_neighbors, self.randomly_sample_counterfactual]
```

### Comparing `manic-xai-1.0.5/manic/Mutation.py` & `manic-xai-1.0.6/manic/Mutation.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.5/manic/Replacement.py` & `manic-xai-1.0.6/manic/Replacement.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.5/manic/Selection.py` & `manic-xai-1.0.6/manic/Selection.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.5/manic/Termination.py` & `manic-xai-1.0.6/manic/Termination.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.5/manic/Utility.py` & `manic-xai-1.0.6/manic/Utility.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.5/manic/__tests__/test_crossover.py` & `manic-xai-1.0.6/manic/__tests__/test_crossover.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.5/manic/__tests__/test_disagreement.py` & `manic-xai-1.0.6/manic/__tests__/test_disagreement.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.5/manic/__tests__/test_manic.py` & `manic-xai-1.0.6/manic/__tests__/test_manic.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.5/manic/__tests__/test_mutation.py` & `manic-xai-1.0.6/manic/__tests__/test_mutation.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.5/manic/__tests__/test_selection.py` & `manic-xai-1.0.6/manic/__tests__/test_selection.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.5/manic_xai.egg-info/PKG-INFO` & `manic-xai-1.0.6/manic_xai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manic-xai
-Version: 1.0.5
+Version: 1.0.6
 Summary: Genetic Algorithm for Generating Metacounterfactual Explanations
 Home-page: https://github.com/craigybaeb/MANIC
 Author: Craig Pirie
 Author-email: c.pirie11@rgu.ac.uk
 Keywords: manic,metacounterfactual,counterfactual,xai,explanation,aggregation,disagreement,agreement
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `manic-xai-1.0.5/manic_xai.egg-info/SOURCES.txt` & `manic-xai-1.0.6/manic_xai.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 README.md
 setup.py
 manic/Baseline.py
 manic/Crossover.py
 manic/Disagreement.py
 manic/Evaluation.py
 manic/GeneticAlgorithm.py
-manic/Initialise.py
 manic/Manic.py
 manic/Mutation.py
 manic/Replacement.py
 manic/Selection.py
 manic/Termination.py
 manic/Utility.py
 manic/__init__.py
```

### Comparing `manic-xai-1.0.5/setup.py` & `manic-xai-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="manic-xai",
-    version='1.0.5',
+    version='1.0.6',
     author="Craig Pirie",
     author_email="c.pirie11@rgu.ac.uk",
     description="Genetic Algorithm for Generating Metacounterfactual Explanations",
     url = "https://github.com/craigybaeb/MANIC",
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
```


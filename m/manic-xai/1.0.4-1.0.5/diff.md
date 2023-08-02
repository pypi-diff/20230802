# Comparing `tmp/manic-xai-1.0.4.tar.gz` & `tmp/manic-xai-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manic-xai-1.0.4.tar", last modified: Sun Jul 30 17:33:33 2023, max compression
+gzip compressed data, was "manic-xai-1.0.5.tar", last modified: Wed Aug  2 20:20:45 2023, max compression
```

## Comparing `manic-xai-1.0.4.tar` & `manic-xai-1.0.5.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-07-30 17:33:33.237064 manic-xai-1.0.4/
--rw-r--r--   0 craigpirie   (501) staff       (20)     1064 2023-07-26 15:54:10.000000 manic-xai-1.0.4/LICENSE
--rw-r--r--   0 craigpirie   (501) staff       (20)     3261 2023-07-30 17:33:33.236779 manic-xai-1.0.4/PKG-INFO
--rw-r--r--   0 craigpirie   (501) staff       (20)     2721 2023-07-26 17:17:12.000000 manic-xai-1.0.4/README.md
-drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-07-30 17:33:33.226090 manic-xai-1.0.4/manic/
--rw-r--r--   0 craigpirie   (501) staff       (20)     1305 2023-07-27 14:07:07.000000 manic-xai-1.0.4/manic/Baseline.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     3057 2023-07-28 17:08:55.000000 manic-xai-1.0.4/manic/Crossover.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     4913 2023-07-28 16:49:09.000000 manic-xai-1.0.4/manic/Disagreement.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     3076 2023-07-28 15:13:20.000000 manic-xai-1.0.4/manic/Evaluation.py
--rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-27 10:52:56.000000 manic-xai-1.0.4/manic/Fitness.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     5468 2023-07-29 20:37:26.000000 manic-xai-1.0.4/manic/Initialise.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     8533 2023-07-28 18:00:44.000000 manic-xai-1.0.4/manic/Manic.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     2754 2023-07-28 12:57:57.000000 manic-xai-1.0.4/manic/Mutation.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     3470 2023-07-28 12:05:18.000000 manic-xai-1.0.4/manic/Selection.py
--rw-r--r--   0 craigpirie   (501) staff       (20)      379 2023-07-27 13:22:11.000000 manic-xai-1.0.4/manic/Termination.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     5693 2023-07-28 17:55:48.000000 manic-xai-1.0.4/manic/Utility.py
--rw-r--r--   0 craigpirie   (501) staff       (20)      400 2023-07-27 23:27:35.000000 manic-xai-1.0.4/manic/__init__.py
-drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-07-30 17:33:33.234849 manic-xai-1.0.4/manic/__tests__/
--rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-27 23:28:48.000000 manic-xai-1.0.4/manic/__tests__/__init__.py
--rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:45:16.000000 manic-xai-1.0.4/manic/__tests__/test_baseline.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     1905 2023-07-28 17:41:26.000000 manic-xai-1.0.4/manic/__tests__/test_crossover.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     5034 2023-07-28 16:53:03.000000 manic-xai-1.0.4/manic/__tests__/test_disagreement.py
--rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:45:35.000000 manic-xai-1.0.4/manic/__tests__/test_evaluation.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     3400 2023-07-26 16:45:04.000000 manic-xai-1.0.4/manic/__tests__/test_initialise.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     5512 2023-07-26 16:39:06.000000 manic-xai-1.0.4/manic/__tests__/test_initialise_population.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     1269 2023-07-26 17:02:40.000000 manic-xai-1.0.4/manic/__tests__/test_manic.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     4387 2023-07-28 14:27:49.000000 manic-xai-1.0.4/manic/__tests__/test_mutation.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     9470 2023-07-28 15:04:45.000000 manic-xai-1.0.4/manic/__tests__/test_selection.py
--rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:45:43.000000 manic-xai-1.0.4/manic/__tests__/test_termination.py
--rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:46:05.000000 manic-xai-1.0.4/manic/__tests__/test_utility.py
-drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-07-30 17:33:33.236288 manic-xai-1.0.4/manic_xai.egg-info/
--rw-r--r--   0 craigpirie   (501) staff       (20)     3261 2023-07-30 17:33:33.000000 manic-xai-1.0.4/manic_xai.egg-info/PKG-INFO
--rw-r--r--   0 craigpirie   (501) staff       (20)      827 2023-07-30 17:33:33.000000 manic-xai-1.0.4/manic_xai.egg-info/SOURCES.txt
--rw-r--r--   0 craigpirie   (501) staff       (20)        1 2023-07-30 17:33:33.000000 manic-xai-1.0.4/manic_xai.egg-info/dependency_links.txt
--rw-r--r--   0 craigpirie   (501) staff       (20)       69 2023-07-30 17:33:33.000000 manic-xai-1.0.4/manic_xai.egg-info/requires.txt
--rw-r--r--   0 craigpirie   (501) staff       (20)        6 2023-07-30 17:33:33.000000 manic-xai-1.0.4/manic_xai.egg-info/top_level.txt
--rw-r--r--   0 craigpirie   (501) staff       (20)       38 2023-07-30 17:33:33.237141 manic-xai-1.0.4/setup.cfg
--rw-r--r--   0 craigpirie   (501) staff       (20)     1041 2023-07-30 17:33:29.000000 manic-xai-1.0.4/setup.py
+drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-08-02 20:20:45.387708 manic-xai-1.0.5/
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1064 2023-07-26 15:54:10.000000 manic-xai-1.0.5/LICENSE
+-rw-r--r--   0 craigpirie   (501) staff       (20)     3261 2023-08-02 20:20:45.387464 manic-xai-1.0.5/PKG-INFO
+-rw-r--r--   0 craigpirie   (501) staff       (20)     2721 2023-07-26 17:17:12.000000 manic-xai-1.0.5/README.md
+drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-08-02 20:20:45.379816 manic-xai-1.0.5/manic/
+-rw-r--r--   0 craigpirie   (501) staff       (20)     2845 2023-08-01 23:21:50.000000 manic-xai-1.0.5/manic/Baseline.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     6369 2023-08-02 20:20:39.000000 manic-xai-1.0.5/manic/Crossover.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)    10944 2023-08-02 17:39:33.000000 manic-xai-1.0.5/manic/Disagreement.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     6987 2023-08-01 23:28:50.000000 manic-xai-1.0.5/manic/Evaluation.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     6644 2023-08-02 20:15:27.000000 manic-xai-1.0.5/manic/GeneticAlgorithm.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     5509 2023-07-31 00:24:07.000000 manic-xai-1.0.5/manic/Initialise.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     7534 2023-08-02 20:15:40.000000 manic-xai-1.0.5/manic/Manic.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     5614 2023-08-01 23:32:04.000000 manic-xai-1.0.5/manic/Mutation.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1563 2023-08-02 17:56:19.000000 manic-xai-1.0.5/manic/Replacement.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     7213 2023-08-02 17:44:55.000000 manic-xai-1.0.5/manic/Selection.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1824 2023-08-01 22:52:00.000000 manic-xai-1.0.5/manic/Termination.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)    10672 2023-08-02 20:09:42.000000 manic-xai-1.0.5/manic/Utility.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)      520 2023-08-01 22:24:38.000000 manic-xai-1.0.5/manic/__init__.py
+drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-08-02 20:20:45.385636 manic-xai-1.0.5/manic/__tests__/
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-27 23:28:48.000000 manic-xai-1.0.5/manic/__tests__/__init__.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:45:16.000000 manic-xai-1.0.5/manic/__tests__/test_baseline.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1905 2023-07-28 17:41:26.000000 manic-xai-1.0.5/manic/__tests__/test_crossover.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     5034 2023-07-28 16:53:03.000000 manic-xai-1.0.5/manic/__tests__/test_disagreement.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:45:35.000000 manic-xai-1.0.5/manic/__tests__/test_evaluation.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-31 01:59:12.000000 manic-xai-1.0.5/manic/__tests__/test_genetic_algorithm.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1269 2023-07-26 17:02:40.000000 manic-xai-1.0.5/manic/__tests__/test_manic.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     4387 2023-07-28 14:27:49.000000 manic-xai-1.0.5/manic/__tests__/test_mutation.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-08-01 22:24:47.000000 manic-xai-1.0.5/manic/__tests__/test_replacement.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     9470 2023-07-28 15:04:45.000000 manic-xai-1.0.5/manic/__tests__/test_selection.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:45:43.000000 manic-xai-1.0.5/manic/__tests__/test_termination.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:46:05.000000 manic-xai-1.0.5/manic/__tests__/test_utility.py
+drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-08-02 20:20:45.387100 manic-xai-1.0.5/manic_xai.egg-info/
+-rw-r--r--   0 craigpirie   (501) staff       (20)     3261 2023-08-02 20:20:45.000000 manic-xai-1.0.5/manic_xai.egg-info/PKG-INFO
+-rw-r--r--   0 craigpirie   (501) staff       (20)      854 2023-08-02 20:20:45.000000 manic-xai-1.0.5/manic_xai.egg-info/SOURCES.txt
+-rw-r--r--   0 craigpirie   (501) staff       (20)        1 2023-08-02 20:20:45.000000 manic-xai-1.0.5/manic_xai.egg-info/dependency_links.txt
+-rw-r--r--   0 craigpirie   (501) staff       (20)       69 2023-08-02 20:20:45.000000 manic-xai-1.0.5/manic_xai.egg-info/requires.txt
+-rw-r--r--   0 craigpirie   (501) staff       (20)        6 2023-08-02 20:20:45.000000 manic-xai-1.0.5/manic_xai.egg-info/top_level.txt
+-rw-r--r--   0 craigpirie   (501) staff       (20)       38 2023-08-02 20:20:45.387781 manic-xai-1.0.5/setup.cfg
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1041 2023-08-02 20:20:39.000000 manic-xai-1.0.5/setup.py
```

### Comparing `manic-xai-1.0.4/LICENSE` & `manic-xai-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.4/PKG-INFO` & `manic-xai-1.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manic-xai
-Version: 1.0.4
+Version: 1.0.5
 Summary: Genetic Algorithm for Generating Metacounterfactual Explanations
 Home-page: https://github.com/craigybaeb/MANIC
 Author: Craig Pirie
 Author-email: c.pirie11@rgu.ac.uk
 Keywords: manic,metacounterfactual,counterfactual,xai,explanation,aggregation,disagreement,agreement
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `manic-xai-1.0.4/README.md` & `manic-xai-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.4/manic/Initialise.py` & `manic-xai-1.0.5/manic/Initialise.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,30 +5,31 @@
 from Baseline import Baseline
 from Disagreement import Disagreement
 from Evaluation import Evaluation
 from Selection import Selection
 from Utility import Utility
 
 class Initialise:
-    def __init__(self, disagreement_method, data_instance, base_counterfactuals, predict_fn, predict_proba_fn, seed, population_size, categorical_features, feature_ranges, immutable_features, data, class_labels, theta, alpha, beta, num_parents, verbose, labels):
+    def __init__(self, disagreement_method, data_instance, base_counterfactuals, predict_fn, predict_proba_fn, seed, population_size, categorical_features, feature_ranges, immutable_features, data, class_labels, theta, alpha, beta, num_parents, verbose, labels, parallel):
         self.seed = seed
         self.population_size = population_size
         self.base_counterfactuals = base_counterfactuals
         self.data = data
         self.class_labels = class_labels
         self.categorical_features = categorical_features
         self.data_instance = data_instance
+        self.parallel = parallel
         self.immutable_features_set = set(immutable_features)
-        self.categories = self.get_categories(categorical_features) #TODO infer from data
+        self.categories = self.get_categories(categorical_features)
         self.feature_ranges = self.get_feature_ranges(feature_ranges)
         self.target_class = 1 - predict_fn(data_instance) #TODO don't assume binary classification
         self.disagreement = Disagreement(disagreement_method, data_instance, base_counterfactuals, categorical_features, feature_ranges, predict_fn, predict_proba_fn, self.target_class, self.feature_ranges)
         self.instance_probability = predict_proba_fn(data_instance)
-        self.evaluation = Evaluation(alpha, beta, predict_proba_fn, self.instance_probability, base_counterfactuals, self.disagreement, data_instance, theta)
-        self.selection = Selection(num_parents, self.target_class, population_size, predict_fn)
+        self.evaluation = Evaluation(alpha, beta, predict_proba_fn, self.instance_probability, base_counterfactuals, self.disagreement, data_instance, theta, parallel)
+        self.selection = Selection(num_parents, self.target_class, population_size, predict_fn, parallel)
         self.utils = Utility(data_instance, self.categories, immutable_features, self.target_class, verbose, predict_fn, self.disagreement, base_counterfactuals, self.evaluation, labels)
         self.population = self.initialise_population()
         self.baseline = Baseline(self.disagreement, base_counterfactuals, data_instance)
 
     def weighted_random_choice(self, options, weights):
         return random.choices(options, weights, k=1)[0]
```

### Comparing `manic-xai-1.0.4/manic/Manic.py` & `manic-xai-1.0.5/manic/GeneticAlgorithm.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,72 +1,32 @@
-import time
 import os
+import time
 
-from Crossover import Crossover
-from Initialise import Initialise
-from Mutation import Mutation
-
-class Manic:
-    def __init__(self, data_instance, base_counterfactuals, categorical_features, immutable_features, feature_ranges, data, predict_fn, predict_proba_fn, class_labels, population_size=100, num_generations=50, alpha=0.5, beta=0.5, crossover_method="uniform", mutation_method="random_resetting", perturbation_fraction=0.1, num_parents=2, seed=42, verbose=1, early_stopping=None, max_time=None, disagreement_method="euclidean_distance", theta=0.3, labels=[]):
-        self.initialise = Initialise(disagreement_method, data_instance, base_counterfactuals, predict_fn, predict_proba_fn, seed, population_size, categorical_features, feature_ranges, immutable_features, data, class_labels, theta, alpha, beta, num_parents, verbose, labels)
-        self.immutable_features_set = self.initialise.immutable_features_set
-        self.target_class = self.initialise.target_class
-        self.instance_probability = self.initialise.instance_probability
-        self.categories = self.initialise.categories
-        self.feature_ranges = self.initialise.feature_ranges
-        self.disagreement = self.initialise.disagreement
-        self.evaluation = self.initialise.evaluation
-        self.selection = self.initialise.selection
-        self.utils = self.initialise.utils
-        self.is_counterfactual_valid = self.utils.is_counterfactual_valid
-        self.print_results = self.utils.print_results
-        self.population = self.initialise.population
-        self.baseline = self.initialise.baseline
-
-        self.data_instance = data_instance
-        self.base_counterfactuals = base_counterfactuals
-        self.categorical_features = categorical_features
-        self.immutable_features = immutable_features
-        self.data = data
-        self.predict_fn = predict_fn
-        self.predict_proba_fn = predict_proba_fn
-        self.population_size = population_size
+class GeneticAlgorithm:
+    def __init__(self, num_generations, early_stopping, predict_fn, evaluation, selection, crossover, mutate, verbose, target_class, max_time, utils, replacement, population, base_counterfactuals, data_instance):
         self.num_generations = num_generations
-        self.crossover = Crossover(crossover_method, num_parents, population_size).crossover
-        self.continuous_feature_ranges = feature_ranges
-        self.verbose = verbose
         self.early_stopping = early_stopping
-        self.consecutive_generations_without_improvement = 0
-        self.max_time = max_time
-        self.mutate = Mutation(mutation_method, perturbation_fraction, self.feature_ranges).mutate
+        self.predict_fn = predict_fn
+        self.evaluation = evaluation
+        self.selection = selection
+        self.crossover = crossover
+        self.mutate = mutate
+        self.verbose = verbose
+        self.target_class = target_class
         self.best_counterfactual = None
         self.best_fitness = float('inf')
         self.generation_found = float('inf')
         self.time_found = float('inf')
+        self.max_time = max_time
+        self.utils = utils
+        self.replacement = replacement
+        self.population = population
+        self.base_counterfactuals = base_counterfactuals
+        self.data_instance
 
-    def __str__(self):
-        attributes_str = [
-            f"data_instance: {self.data_instance}",
-            f"base_counterfactuals: {self.base_counterfactuals}",
-            f"categorical_features: {self.categorical_features}",
-            f"immutable_features: {self.immutable_features}",
-            f"data: {self.data}",
-            f"population_size: {self.population_size}",
-            f"num_generations: {self.num_generations}",
-            f"target_class: {self.target_class}",
-            f"continuous_feature_ranges: {self.continuous_feature_ranges}",
-            f"categories: {self.categories}",
-            f"feature_ranges: {self.feature_ranges}",
-            f"verbose: {self.verbose}"
-        ]
-
-        return "\n".join(attributes_str)
-
-    def to_string(self):
-        return str(self)
 
     def should_stop(self, generations, time_elapsed):
       if('found' in list(self.early_stopping.keys()) and self.early_stopping['found'] == True):
         if('patience_generations' in list(self.early_stopping.keys())):
           if(self.early_stopping['patience_generations'] <= generations):
             print(f"Early stopping at generation {generations}. No improvement for {self.early_stopping['patience_generations']} consecutive generations.")
             return True
@@ -89,92 +49,100 @@
       return cpu_cycles
 
     def generate_counterfactuals(self):
         start_time = time.time()
         cpu_start_time = self.get_cpu_time()
 
         for generation in range(self.num_generations):
+            # Shows the current generation
             if self.verbose == 1:
                 print(f"Generation {generation + 1}")
-
-            fitness_scores = self.evaluation.evaluate_population(self.population)
-
-            #Maybe remove normalisation, not sure if ti works with our method
-            unnormalised_fitness_scores = fitness_scores
             
-            normalise=False
-            if(normalise):
-              min_score = min(fitness_scores)
-              max_score = max(fitness_scores)
-
-              if min_score == max_score:
-                  # Handle the case when all scores are the same
-                  fitness_scores = [1.0] * len(fitness_scores)
-              else:
-                  fitness_scores = [(score - min_score) / (max_score - min_score) for score in fitness_scores]
-            
-            parents = self.selection.select_parents(self.population, fitness_scores)
-            offspring = self.crossover(parents)
-            offspring = self.mutate(offspring)
-            
-            # Combine elites and offspring
-            elites = self.selection.select_elites(self.population, fitness_scores)
-            self.population = elites + offspring
-
-            best_idx = fitness_scores.index(min(fitness_scores))
-            generation_best_counterfactual = self.population[best_idx]
-            generation_best_fitness = fitness_scores[best_idx]
+            # Runs selection, crossover and mutation to get the new population
+            self.population, generation_best_counterfactual, generation_best_fitness = self.replacement.update_population(self.population)
 
+            # Check if a more optimal solution has been found
             if generation_best_fitness < self.best_fitness:
+                #Format the counterfactual so it is realistic
+                formatted_counterfactual = self.utils.format_counterfactual(generation_best_counterfactual) 
+                
                 # Check if the candidate counterfactual produces the target class
-                formatted_counterfactual = self.utils.format_counterfactual(generation_best_counterfactual)
                 prediction = self.predict_fn(formatted_counterfactual)
+                
                 if prediction == self.target_class:
                     self.best_fitness = generation_best_fitness
+
+                    # Check that the solution is an improvement
                     if(formatted_counterfactual != self.best_counterfactual):
                         self.best_counterfactual = formatted_counterfactual
                         self.generation_found = generation
                         self.time_found = time.time() - start_time
 
                     self.consecutive_generations_without_improvement = 0
-                else:
-                    self.consecutive_generations_without_improvement += 1
             else:
                 self.consecutive_generations_without_improvement += 1
 
+            # Show the progress of the generation
+            self.show_progress(generation, self.verbose)
+
+            # Check if the termination criteria has been met
             if self.early_stopping is not None:
                 time_elapsed = time.time() - start_time
                 if(self.should_stop(generation, time_elapsed)):
                     if self.verbose > 0:
                       break
 
-            if self.verbose == 2:
-                print(f"Generation {generation+1}: Best Counterfactual = {self.best_counterfactual}, Fitness = {self.best_fitness}")
-
-            if self.verbose == 3:
-                print(f"Generation {generation+1}:")
-                for idx, child in enumerate(offspring):
-                    print(f"Child {idx+1}: {child}")
-
             # Check if the specified maximum time is exceeded
             if self.max_time is not None and (time.time() - start_time) > (self.max_time * 60):
                 if self.verbose > 0:
                     print(f"Stopping search after {self.max_time} minutes.")
                 break
 
-        end_time = time.time()
+        # Calculate elapsed CPU time in seconds and convert to CPU cycles
         cpu_end_time = self.get_cpu_time()
-
-                # Calculate elapsed CPU time in seconds
         elapsed_cpu_time_seconds = cpu_end_time - cpu_start_time
-
         cpu_cycles = self.get_cpu_cycles(elapsed_cpu_time_seconds)
 
-        print(end_time - start_time)
+        # Calculate total time taken
+        end_time = time.time()
+        time_taken = end_time - start_time
 
+        proximity_score = self.disagreement.calculate_proximity(self.data_instance, self.best_counterfactual, True)
+        sparsity_score, number_of_changes = self.disagreement.calculate_sparsity(self.best_counterfactual)
+        base_cf_scores = []
+        for base_cf in self.base_counterfactuals:
+            base_cf_scores.append(self.evaluation.calculate_base_cf_scores([self.best_counterfactual], base_cf))
 
-        time_taken = end_time - start_time
+        disagreement_score = sum(score for score in base_cf_scores) / len(base_cf_scores)
 
+        # Show results
         if self.verbose > 0:
-            self.print_results(self.best_counterfactual, self.best_fitness, generation + 1, self.generation_found, time_taken, self.time_found, cpu_cycles)
+            self.utils.print_results(self.best_counterfactual, self.best_fitness, generation + 1, self.generation_found, time_taken, self.time_found, cpu_cycles, proximity_score, sparsity_score, number_of_changes, disagreement_score)
+
+        
+
+        # Store results in a dictionary
+        results = {
+          'best_counterfactual': self.best_counterfactual,
+          'best_counterfactual_fitness': self.best_fitness,
+          'generation_found': self.generation_found,
+          'time_found': self.time_found,
+          'cpu_cycles_found': cpu_cycles,
+          'proximity_score': proximity_score,
+          'sparsity_score': sparsity_score,
+          'number_of_changes': number_of_changes,
+          'disagreement_score': disagreement_score
+        }
+
+        return results
+
+    # Function to show the progress on each generation
+    def show_progress(self, generation, verbose):
+        if verbose == 2:
+            print(f"Generation {generation+1}: Best Counterfactual = {self.best_counterfactual}, Fitness = {self.best_fitness}")
+
+        if verbose == 3:
+            print(f"Generation {generation+1}:")
+            for idx, child in enumerate(self.population):
+                print(f"Child {idx+1}: {child}")
 
         return self.best_counterfactual
```

### Comparing `manic-xai-1.0.4/manic/Mutation.py` & `manic-xai-1.0.5/manic/__tests__/test_mutation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,92 @@
-
+import unittest
 import random
+from Mutation import Mutation
 
-class Mutation:
-    def __init__(self, mutation_method, perturbation_fraction, feature_ranges):
-        self.mutation_method = mutation_method
-        self.mutate = self.set_mutation(mutation_method)
-        self.perturbation_fraction = perturbation_fraction
-        self.feature_ranges = feature_ranges
-
-        self.validate_self()
-    
-    def set_mutation(self, mutation_method):
-            if(mutation_method == "random_resetting"):
-                return self.random_resetting_mutation
-            elif(mutation_method == "swap_mutation"):
-                return self.swap_mutation
-            else:
-                return self.random_resetting_mutation
-        
-    def random_resetting_mutation(self, offspring):
-        new_offspring = []  # Store the mutated offspring
-        for i in range(len(offspring)):
-            mutated_instance = offspring[i].copy()  # Create a copy of the instance
-            for j in range(len(offspring[i])):
-                if random.random() < self.perturbation_fraction:
-                    lower_bound, upper_bound = self.feature_ranges[j]
-                    mutation_value = random.uniform(lower_bound, upper_bound)
-                    mutated_instance[j] = max(lower_bound, min(upper_bound, mutation_value))
-            new_offspring.append(mutated_instance)
-        return new_offspring
-    
-    #Needs constraining for valid ranges if using.
-    def swap_mutation(self, offspring):
-        for i in range(len(offspring)):
-            # Randomly select two different feature indices
-            feature_indices = random.sample(range(len(offspring[i])), 2)
-
-            # Swap the values of the selected features
-            offspring[i][feature_indices[0]], offspring[i][feature_indices[1]] = \
-                offspring[i][feature_indices[1]], offspring[i][feature_indices[0]]
+class TestMutation(unittest.TestCase):
+    def setUp(self):
+        # Sample feature_ranges for testing
+        self.feature_ranges = [(0, 1), (-1, 1), (5, 10)]
 
+    def generate_random_offspring(self, length=100):
+        # Generate random offspring for testing
+        offspring = []
+        for _ in range(length):
+            instance = [random.uniform(lower, upper) for lower, upper in self.feature_ranges]
+            offspring.append(instance)
         return offspring
-    
-    def validate_self(self):
-        if(self.mutation_method not in ["random_resetting", "swap_mutation"]):
-            raise Warning("Invalid mutation method given, it must be random_resetting or swap_mutation. Defaulting to random_resetting.")
-        
-        if(self.mutate not in [self.random_resetting_mutation, self.swap_mutation]):
-            raise ValueError("Error initialising mutation method, no valid method was set.")
-        
-        if(self.perturbation_fraction == None):
-            raise ValueError("Perturbation fraction cannot be None.")
-        
-        if(self.perturbation_fraction < 0 or self.perturbation_fraction > 1):
-            raise ValueError("Perturbation fraction must be between 0 and 1.")
-        
-        if(self.feature_ranges == None or len(self.feature_ranges) == 0):
-            raise ValueError("Feature ranges must be given.")
-        
+
+    def test_random_resetting_mutation(self):
+        # Initialize Mutation with "random_resetting" method
+        mutation_method = "random_resetting"
+        perturbation_fraction = 0.5
+        mutation = Mutation(mutation_method, perturbation_fraction, self.feature_ranges)
+
+        # Test case 1: Random mutation for all features
+        offspring = self.generate_random_offspring()
+        with self.subTest(msg="Test mutation occurred"):
+            mutated_offspring = mutation.random_resetting_mutation(offspring)
+            self.assertNotEqual(mutated_offspring, offspring)
+
+        # Test case 2: No mutation if perturbation_fraction is 0
+        perturbation_fraction = 0.0
+        mutation = Mutation(mutation_method, perturbation_fraction, self.feature_ranges)
+        with self.subTest(msg="Test case no mutation"):
+            mutated_offspring = mutation.random_resetting_mutation(offspring)
+            self.assertEqual(mutated_offspring, offspring)
+
+        # Test case 3: All features should be within the given ranges
+        perturbation_fraction = 1.0
+        mutation = Mutation(mutation_method, perturbation_fraction, self.feature_ranges)
+        with self.subTest(msg="Test valid ranges"):
+            mutated_offspring = mutation.random_resetting_mutation(offspring)
+            for i in range(len(mutated_offspring)):
+                for j in range(len(mutated_offspring[i])):
+                    lower_bound, upper_bound = self.feature_ranges[j]
+                    self.assertTrue(lower_bound <= mutated_offspring[i][j] <= upper_bound)
+
+        # Test case 4: Offspring with invalid features should be clipped to the valid range
+        perturbation_fraction = 1.0
+        mutation = Mutation(mutation_method, perturbation_fraction, self.feature_ranges)
+        bad_offspring = offspring
+        bad_offspring[0] = [66, 300, -100]
+        bad_offspring[1] = [100, -400, -1400]
+        bad_offspring[2] = [1300, 0, 5]
+        with self.subTest(msg="Test clipping"):
+            mutated_offspring = mutation.random_resetting_mutation(bad_offspring)
+            for i in range(len(mutated_offspring)):
+                for j in range(len(mutated_offspring[i])):
+                    lower_bound, upper_bound = self.feature_ranges[j]
+                    self.assertTrue(lower_bound <= mutated_offspring[i][j] <= upper_bound)
+
+    def test_validate_self(self):
+        # Test case for invalid mutation_method
+        mutation_method = "invalid_method"
+        perturbation_fraction = 0.5
+        feature_ranges = [(0, 1), (-1, 1), (5, 10)]
+
+        with self.subTest("Invalid mutation_method"):
+            with self.assertRaises(Warning) as cm:
+                Mutation(mutation_method, perturbation_fraction, feature_ranges)
+            self.assertEqual(str(cm.exception), "Invalid mutation method given, it must be random_resetting or swap_mutation. Defaulting to random_resetting.")
+
+        # Test case for invalid perturbation_fraction
+        mutation_method = "random_resetting"
+        perturbation_fraction = 1.5  # Invalid value
+
+        with self.subTest("Invalid perturbation_fraction"):
+            with self.assertRaises(ValueError) as cm:
+                Mutation(mutation_method, perturbation_fraction, feature_ranges)
+            self.assertEqual(str(cm.exception), "Perturbation fraction must be between 0 and 1.")
+
+        # Test case for invalid feature_ranges
+        mutation_method = "random_resetting"
+        perturbation_fraction = 0.5
+        feature_ranges = []  # Invalid value
+
+        with self.subTest("Invalid feature_ranges"):
+            with self.assertRaises(ValueError) as cm:
+                Mutation(mutation_method, perturbation_fraction, feature_ranges)
+            self.assertEqual(str(cm.exception), "Feature ranges must be given.")
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `manic-xai-1.0.4/manic/__tests__/test_crossover.py` & `manic-xai-1.0.5/manic/__tests__/test_crossover.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.4/manic/__tests__/test_disagreement.py` & `manic-xai-1.0.5/manic/__tests__/test_disagreement.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.4/manic/__tests__/test_manic.py` & `manic-xai-1.0.5/manic/__tests__/test_manic.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.4/manic/__tests__/test_selection.py` & `manic-xai-1.0.5/manic/__tests__/test_selection.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.4/manic_xai.egg-info/PKG-INFO` & `manic-xai-1.0.5/manic_xai.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manic-xai
-Version: 1.0.4
+Version: 1.0.5
 Summary: Genetic Algorithm for Generating Metacounterfactual Explanations
 Home-page: https://github.com/craigybaeb/MANIC
 Author: Craig Pirie
 Author-email: c.pirie11@rgu.ac.uk
 Keywords: manic,metacounterfactual,counterfactual,xai,explanation,aggregation,disagreement,agreement
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `manic-xai-1.0.4/manic_xai.egg-info/SOURCES.txt` & `manic-xai-1.0.5/manic_xai.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 LICENSE
 README.md
 setup.py
 manic/Baseline.py
 manic/Crossover.py
 manic/Disagreement.py
 manic/Evaluation.py
-manic/Fitness.py
+manic/GeneticAlgorithm.py
 manic/Initialise.py
 manic/Manic.py
 manic/Mutation.py
+manic/Replacement.py
 manic/Selection.py
 manic/Termination.py
 manic/Utility.py
 manic/__init__.py
 manic/__tests__/__init__.py
 manic/__tests__/test_baseline.py
 manic/__tests__/test_crossover.py
 manic/__tests__/test_disagreement.py
 manic/__tests__/test_evaluation.py
-manic/__tests__/test_initialise.py
-manic/__tests__/test_initialise_population.py
+manic/__tests__/test_genetic_algorithm.py
 manic/__tests__/test_manic.py
 manic/__tests__/test_mutation.py
+manic/__tests__/test_replacement.py
 manic/__tests__/test_selection.py
 manic/__tests__/test_termination.py
 manic/__tests__/test_utility.py
 manic_xai.egg-info/PKG-INFO
 manic_xai.egg-info/SOURCES.txt
 manic_xai.egg-info/dependency_links.txt
 manic_xai.egg-info/requires.txt
```

### Comparing `manic-xai-1.0.4/setup.py` & `manic-xai-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="manic-xai",
-    version='1.0.4',
+    version='1.0.5',
     author="Craig Pirie",
     author_email="c.pirie11@rgu.ac.uk",
     description="Genetic Algorithm for Generating Metacounterfactual Explanations",
     url = "https://github.com/craigybaeb/MANIC",
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
```


# Comparing `tmp/sail-0.6.4.tar.gz` & `tmp/sail-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sail-0.6.4.tar", last modified: Thu Jul 13 21:26:49 2023, max compression
+gzip compressed data, was "sail-0.6.6.tar", last modified: Wed Aug  2 15:24:33 2023, max compression
```

## Comparing `sail-0.6.4.tar` & `sail-0.6.6.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.327736 sail-0.6.4/
--rw-r--r--   0 dhaval     (501) staff       (20)     1088 2023-07-12 19:00:43.000000 sail-0.6.4/LICENSE
--rw-r--r--   0 dhaval     (501) staff       (20)     4825 2023-07-13 21:26:49.327831 sail-0.6.4/PKG-INFO
--rw-r--r--   0 dhaval     (501) staff       (20)     3721 2023-07-12 19:01:03.000000 sail-0.6.4/README.md
--rw-r--r--   0 dhaval     (501) staff       (20)     1202 2023-07-12 19:00:43.000000 sail-0.6.4/pyproject.toml
--rw-r--r--   0 dhaval     (501) staff       (20)      794 2023-07-13 21:26:49.328193 sail-0.6.4/setup.cfg
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.310467 sail-0.6.4/src/
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.313265 sail-0.6.4/src/sail/
--rw-r--r--   0 dhaval     (501) staff       (20)      226 2023-07-12 19:01:03.000000 sail-0.6.4/src/sail/__init__.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.314779 sail-0.6.4/src/sail/drift_detection/
--rw-r--r--   0 dhaval     (501) staff       (20)     3336 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/drift_detection/drift_detector.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.315681 sail-0.6.4/src/sail/model_selector/
--rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/model_selector/__init__.py
--rw-r--r--   0 dhaval     (501) staff       (20)     4781 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/model_selector/base.py
--rw-r--r--   0 dhaval     (501) staff       (20)     2082 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/model_selector/holdout_best_model.py
--rw-r--r--   0 dhaval     (501) staff       (20)     2283 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/model_selector/prequential_best_model.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.316086 sail-0.6.4/src/sail/models/
--rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/__init__.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.317408 sail-0.6.4/src/sail/models/auto_ml/
--rw-r--r--   0 dhaval     (501) staff       (20)       44 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/auto_ml/__init__.py
--rw-r--r--   0 dhaval     (501) staff       (20)    13943 2023-07-12 19:01:03.000000 sail-0.6.4/src/sail/models/auto_ml/auto_pipeline.py
--rw-r--r--   0 dhaval     (501) staff       (20)     7896 2023-07-12 19:01:03.000000 sail-0.6.4/src/sail/models/auto_ml/base_strategy.py
--rw-r--r--   0 dhaval     (501) staff       (20)     7033 2023-07-12 19:01:03.000000 sail-0.6.4/src/sail/models/auto_ml/pipeline_strategy.py
--rw-r--r--   0 dhaval     (501) staff       (20)     2709 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/auto_ml/searcher.py
--rw-r--r--   0 dhaval     (501) staff       (20)    20259 2023-07-12 19:01:03.000000 sail-0.6.4/src/sail/models/auto_ml/tune.py
--rw-r--r--   0 dhaval     (501) staff       (20)     1346 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/base.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.318491 sail-0.6.4/src/sail/models/ensemble/
--rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/ensemble/__init__.py
--rw-r--r--   0 dhaval     (501) staff       (20)     9275 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/ensemble/base.py
--rw-r--r--   0 dhaval     (501) staff       (20)     4153 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/ensemble/distAggregateClassifier.py
--rw-r--r--   0 dhaval     (501) staff       (20)     3648 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/ensemble/distAggregateRegressor.py
--rw-r--r--   0 dhaval     (501) staff       (20)     3907 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/ensemble/distEWARegressor.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.319111 sail-0.6.4/src/sail/models/keras/
--rw-r--r--   0 dhaval     (501) staff       (20)       52 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/keras/__init__.py
--rw-r--r--   0 dhaval     (501) staff       (20)     2525 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/keras/base.py
--rw-r--r--   0 dhaval     (501) staff       (20)     8953 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/keras/oselm.py
--rw-r--r--   0 dhaval     (501) staff       (20)    13781 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/keras/wglstm.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.320187 sail-0.6.4/src/sail/models/native/
--rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/native/__init__.py
--rw-r--r--   0 dhaval     (501) staff       (20)    23089 2023-07-12 19:01:03.000000 sail-0.6.4/src/sail/models/native/base.py
--rw-r--r--   0 dhaval     (501) staff       (20)     4277 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/native/ielm.py
--rw-r--r--   0 dhaval     (501) staff       (20)     2162 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/native/isvm.py
--rw-r--r--   0 dhaval     (501) staff       (20)    14132 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/native/lasvm.py
--rw-r--r--   0 dhaval     (501) staff       (20)    12455 2023-07-12 19:01:03.000000 sail-0.6.4/src/sail/models/native/learn_pp.py
--rw-r--r--   0 dhaval     (501) staff       (20)     2901 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/native/robust_iml.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.321442 sail-0.6.4/src/sail/models/river/
--rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/river/__init__.py
--rw-r--r--   0 dhaval     (501) staff       (20)       75 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/river/anomaly.py
--rw-r--r--   0 dhaval     (501) staff       (20)     1073 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/river/base.py
--rw-r--r--   0 dhaval     (501) staff       (20)     3020 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/river/ensemble.py
--rw-r--r--   0 dhaval     (501) staff       (20)     4351 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/river/forest.py
--rw-r--r--   0 dhaval     (501) staff       (20)     3340 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/river/linear_model.py
--rw-r--r--   0 dhaval     (501) staff       (20)      930 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/river/naive_bayes.py
--rw-r--r--   0 dhaval     (501) staff       (20)     1574 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/river/neighbors.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.322392 sail-0.6.4/src/sail/models/sklearn/
--rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/sklearn/__init__.py
--rw-r--r--   0 dhaval     (501) staff       (20)      888 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/sklearn/base.py
--rw-r--r--   0 dhaval     (501) staff       (20)       80 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/sklearn/cluster.py
--rw-r--r--   0 dhaval     (501) staff       (20)      399 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/sklearn/linear_model.py
--rw-r--r--   0 dhaval     (501) staff       (20)      143 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/sklearn/naive_bayes.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.324989 sail-0.6.4/src/sail/models/torch/
--rw-r--r--   0 dhaval     (501) staff       (20)       90 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/__init__.py
--rw-r--r--   0 dhaval     (501) staff       (20)     1324 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/base.py
--rw-r--r--   0 dhaval     (501) staff       (20)     1807 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/data.py
--rw-r--r--   0 dhaval     (501) staff       (20)     2020 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/fcn.py
--rw-r--r--   0 dhaval     (501) staff       (20)     2107 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/fcn_classification.py
--rw-r--r--   0 dhaval     (501) staff       (20)     8676 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/inceptiontime.py
--rw-r--r--   0 dhaval     (501) staff       (20)     1499 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/layers.py
--rw-r--r--   0 dhaval     (501) staff       (20)      985 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/light_lstm.py
--rw-r--r--   0 dhaval     (501) staff       (20)     1813 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/lstm.py
--rw-r--r--   0 dhaval     (501) staff       (20)     2430 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/lstm_fcn.py
--rw-r--r--   0 dhaval     (501) staff       (20)     1146 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/nn.py
--rw-r--r--   0 dhaval     (501) staff       (20)    12028 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/onn_hbp.py
--rw-r--r--   0 dhaval     (501) staff       (20)     8576 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/os_cnn.py
--rw-r--r--   0 dhaval     (501) staff       (20)     4170 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/rnn.py
--rw-r--r--   0 dhaval     (501) staff       (20)     3159 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/rocket.py
--rw-r--r--   0 dhaval     (501) staff       (20)     7826 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/tcn.py
--rw-r--r--   0 dhaval     (501) staff       (20)     2018 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/models/torch/utils.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.325273 sail-0.6.4/src/sail/pipeline/
--rw-r--r--   0 dhaval     (501) staff       (20)       34 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/pipeline/__init__.py
--rw-r--r--   0 dhaval     (501) staff       (20)    11789 2023-07-12 19:01:03.000000 sail-0.6.4/src/sail/pipeline/pipeline.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.325529 sail-0.6.4/src/sail/transfomers/
--rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/transfomers/__init__.py
--rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/transfomers/base.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.326045 sail-0.6.4/src/sail/transfomers/river/
--rw-r--r--   0 dhaval     (501) staff       (20)      265 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/transfomers/river/base.py
--rw-r--r--   0 dhaval     (501) staff       (20)     2908 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/transfomers/river/feature_extraction.py
--rw-r--r--   0 dhaval     (501) staff       (20)      961 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/transfomers/river/feature_selection.py
--rw-r--r--   0 dhaval     (501) staff       (20)     3697 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/transfomers/river/preprocessing.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.326182 sail-0.6.4/src/sail/transfomers/sklearn/
--rw-r--r--   0 dhaval     (501) staff       (20)     2105 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/transfomers/sklearn/preprocessing.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.327339 sail-0.6.4/src/sail/utils/
--rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/utils/__init__.py
--rw-r--r--   0 dhaval     (501) staff       (20)     1034 2023-07-12 19:01:03.000000 sail-0.6.4/src/sail/utils/logging.py
--rw-r--r--   0 dhaval     (501) staff       (20)     2024 2023-07-12 19:01:03.000000 sail-0.6.4/src/sail/utils/progress_bar.py
--rw-r--r--   0 dhaval     (501) staff       (20)     2053 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/utils/ray_utils.py
--rw-r--r--   0 dhaval     (501) staff       (20)     4863 2023-07-12 19:01:03.000000 sail-0.6.4/src/sail/utils/scorer.py
--rw-r--r--   0 dhaval     (501) staff       (20)     1478 2023-07-12 19:01:03.000000 sail-0.6.4/src/sail/utils/serialization.py
--rw-r--r--   0 dhaval     (501) staff       (20)      241 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/utils/stats.py
--rw-r--r--   0 dhaval     (501) staff       (20)      794 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/utils/ts_utils.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.327579 sail-0.6.4/src/sail/visualisation/
--rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/visualisation/__init__.py
--rw-r--r--   0 dhaval     (501) staff       (20)     2453 2023-07-12 19:00:43.000000 sail-0.6.4/src/sail/visualisation/ts_plot.py
-drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-07-13 21:26:49.314441 sail-0.6.4/src/sail.egg-info/
--rw-r--r--   0 dhaval     (501) staff       (20)     4825 2023-07-13 21:26:49.000000 sail-0.6.4/src/sail.egg-info/PKG-INFO
--rw-r--r--   0 dhaval     (501) staff       (20)     2960 2023-07-13 21:26:49.000000 sail-0.6.4/src/sail.egg-info/SOURCES.txt
--rw-r--r--   0 dhaval     (501) staff       (20)        1 2023-07-13 21:26:49.000000 sail-0.6.4/src/sail.egg-info/dependency_links.txt
--rw-r--r--   0 dhaval     (501) staff       (20)        1 2023-07-13 21:26:49.000000 sail-0.6.4/src/sail.egg-info/not-zip-safe
--rw-r--r--   0 dhaval     (501) staff       (20)      653 2023-07-13 21:26:49.000000 sail-0.6.4/src/sail.egg-info/requires.txt
--rw-r--r--   0 dhaval     (501) staff       (20)        5 2023-07-13 21:26:49.000000 sail-0.6.4/src/sail.egg-info/top_level.txt
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-08-02 15:24:33.703982 sail-0.6.6/
+-rw-r--r--   0 dhaval     (501) staff       (20)     1088 2023-07-12 19:00:43.000000 sail-0.6.6/LICENSE
+-rw-r--r--   0 dhaval     (501) staff       (20)     4826 2023-08-02 15:24:33.704078 sail-0.6.6/PKG-INFO
+-rw-r--r--   0 dhaval     (501) staff       (20)     3721 2023-07-14 00:32:44.000000 sail-0.6.6/README.md
+-rw-r--r--   0 dhaval     (501) staff       (20)     1203 2023-08-02 15:22:49.000000 sail-0.6.6/pyproject.toml
+-rw-r--r--   0 dhaval     (501) staff       (20)      790 2023-08-02 15:24:33.704413 sail-0.6.6/setup.cfg
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-08-02 15:24:33.688309 sail-0.6.6/src/
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-08-02 15:24:33.690614 sail-0.6.6/src/sail/
+-rw-r--r--   0 dhaval     (501) staff       (20)      226 2023-08-02 14:42:33.000000 sail-0.6.6/src/sail/__init__.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-08-02 15:24:33.692081 sail-0.6.6/src/sail/drift_detection/
+-rw-r--r--   0 dhaval     (501) staff       (20)     3482 2023-08-02 15:04:32.000000 sail-0.6.6/src/sail/drift_detection/drift_detector.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-08-02 15:24:33.692745 sail-0.6.6/src/sail/model_selector/
+-rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/model_selector/__init__.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     4781 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/model_selector/base.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     2082 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/model_selector/holdout_best_model.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     2283 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/model_selector/prequential_best_model.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-08-02 15:24:33.693102 sail-0.6.6/src/sail/models/
+-rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/__init__.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-08-02 15:24:33.693953 sail-0.6.6/src/sail/models/auto_ml/
+-rw-r--r--   0 dhaval     (501) staff       (20)       44 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/auto_ml/__init__.py
+-rw-r--r--   0 dhaval     (501) staff       (20)    13772 2023-08-02 15:05:14.000000 sail-0.6.6/src/sail/models/auto_ml/auto_pipeline.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     8037 2023-08-02 11:47:17.000000 sail-0.6.6/src/sail/models/auto_ml/base_strategy.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     7033 2023-07-14 00:32:44.000000 sail-0.6.6/src/sail/models/auto_ml/pipeline_strategy.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     2709 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/auto_ml/searcher.py
+-rw-r--r--   0 dhaval     (501) staff       (20)    20484 2023-08-02 11:47:17.000000 sail-0.6.6/src/sail/models/auto_ml/tune.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     1346 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/base.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-08-02 15:24:33.694644 sail-0.6.6/src/sail/models/ensemble/
+-rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/ensemble/__init__.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     9275 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/ensemble/base.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     4153 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/ensemble/distAggregateClassifier.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     3648 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/ensemble/distAggregateRegressor.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     3907 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/ensemble/distEWARegressor.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-08-02 15:24:33.695200 sail-0.6.6/src/sail/models/keras/
+-rw-r--r--   0 dhaval     (501) staff       (20)       52 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/keras/__init__.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     2525 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/keras/base.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     8953 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/keras/oselm.py
+-rw-r--r--   0 dhaval     (501) staff       (20)    13262 2023-08-02 14:46:29.000000 sail-0.6.6/src/sail/models/keras/wglstm.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-08-02 15:24:33.696200 sail-0.6.6/src/sail/models/native/
+-rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/native/__init__.py
+-rw-r--r--   0 dhaval     (501) staff       (20)    23089 2023-07-14 00:32:44.000000 sail-0.6.6/src/sail/models/native/base.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     4277 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/native/ielm.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     2162 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/native/isvm.py
+-rw-r--r--   0 dhaval     (501) staff       (20)    14132 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/native/lasvm.py
+-rw-r--r--   0 dhaval     (501) staff       (20)    12455 2023-07-14 00:32:44.000000 sail-0.6.6/src/sail/models/native/learn_pp.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     2901 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/native/robust_iml.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-08-02 15:24:33.697338 sail-0.6.6/src/sail/models/river/
+-rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/river/__init__.py
+-rw-r--r--   0 dhaval     (501) staff       (20)       75 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/river/anomaly.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     1073 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/river/base.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     3020 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/river/ensemble.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     4397 2023-08-02 14:28:29.000000 sail-0.6.6/src/sail/models/river/forest.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     3340 2023-08-02 14:27:45.000000 sail-0.6.6/src/sail/models/river/linear_model.py
+-rw-r--r--   0 dhaval     (501) staff       (20)      930 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/river/naive_bayes.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     1574 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/river/neighbors.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-08-02 15:24:33.698123 sail-0.6.6/src/sail/models/sklearn/
+-rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/sklearn/__init__.py
+-rw-r--r--   0 dhaval     (501) staff       (20)      888 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/sklearn/base.py
+-rw-r--r--   0 dhaval     (501) staff       (20)       80 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/sklearn/cluster.py
+-rw-r--r--   0 dhaval     (501) staff       (20)      399 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/sklearn/linear_model.py
+-rw-r--r--   0 dhaval     (501) staff       (20)      143 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/sklearn/naive_bayes.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-08-02 15:24:33.700893 sail-0.6.6/src/sail/models/torch/
+-rw-r--r--   0 dhaval     (501) staff       (20)       90 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/torch/__init__.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     1324 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/torch/base.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     1807 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/torch/data.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     2020 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/torch/fcn.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     2107 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/torch/fcn_classification.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     8676 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/torch/inceptiontime.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     1499 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/torch/layers.py
+-rw-r--r--   0 dhaval     (501) staff       (20)      985 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/torch/light_lstm.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     1813 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/torch/lstm.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     2430 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/torch/lstm_fcn.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     1146 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/torch/nn.py
+-rw-r--r--   0 dhaval     (501) staff       (20)    12028 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/torch/onn_hbp.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     8576 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/torch/os_cnn.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     4170 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/torch/rnn.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     3159 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/torch/rocket.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     7826 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/torch/tcn.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     2018 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/models/torch/utils.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-08-02 15:24:33.701269 sail-0.6.6/src/sail/pipeline/
+-rw-r--r--   0 dhaval     (501) staff       (20)       34 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/pipeline/__init__.py
+-rw-r--r--   0 dhaval     (501) staff       (20)    11790 2023-07-21 20:35:29.000000 sail-0.6.6/src/sail/pipeline/pipeline.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-08-02 15:24:33.701549 sail-0.6.6/src/sail/transfomers/
+-rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/transfomers/__init__.py
+-rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/transfomers/base.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-08-02 15:24:33.702317 sail-0.6.6/src/sail/transfomers/river/
+-rw-r--r--   0 dhaval     (501) staff       (20)      265 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/transfomers/river/base.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     2908 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/transfomers/river/feature_extraction.py
+-rw-r--r--   0 dhaval     (501) staff       (20)      961 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/transfomers/river/feature_selection.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     3697 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/transfomers/river/preprocessing.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-08-02 15:24:33.702460 sail-0.6.6/src/sail/transfomers/sklearn/
+-rw-r--r--   0 dhaval     (501) staff       (20)     2105 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/transfomers/sklearn/preprocessing.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-08-02 15:24:33.703569 sail-0.6.6/src/sail/utils/
+-rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/utils/__init__.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     1034 2023-07-14 00:32:44.000000 sail-0.6.6/src/sail/utils/logging.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     2024 2023-07-14 00:32:44.000000 sail-0.6.6/src/sail/utils/progress_bar.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     2053 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/utils/ray_utils.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     4838 2023-07-14 00:32:44.000000 sail-0.6.6/src/sail/utils/scorer.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     1478 2023-07-14 00:32:44.000000 sail-0.6.6/src/sail/utils/serialization.py
+-rw-r--r--   0 dhaval     (501) staff       (20)      241 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/utils/stats.py
+-rw-r--r--   0 dhaval     (501) staff       (20)      794 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/utils/ts_utils.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-08-02 15:24:33.703851 sail-0.6.6/src/sail/visualisation/
+-rw-r--r--   0 dhaval     (501) staff       (20)        0 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/visualisation/__init__.py
+-rw-r--r--   0 dhaval     (501) staff       (20)     2453 2023-07-12 19:00:43.000000 sail-0.6.6/src/sail/visualisation/ts_plot.py
+drwxr-xr-x   0 dhaval     (501) staff       (20)        0 2023-08-02 15:24:33.691858 sail-0.6.6/src/sail.egg-info/
+-rw-r--r--   0 dhaval     (501) staff       (20)     4826 2023-08-02 15:24:33.000000 sail-0.6.6/src/sail.egg-info/PKG-INFO
+-rw-r--r--   0 dhaval     (501) staff       (20)     2960 2023-08-02 15:24:33.000000 sail-0.6.6/src/sail.egg-info/SOURCES.txt
+-rw-r--r--   0 dhaval     (501) staff       (20)        1 2023-08-02 15:24:33.000000 sail-0.6.6/src/sail.egg-info/dependency_links.txt
+-rw-r--r--   0 dhaval     (501) staff       (20)        1 2023-07-13 21:26:49.000000 sail-0.6.6/src/sail.egg-info/not-zip-safe
+-rw-r--r--   0 dhaval     (501) staff       (20)      649 2023-08-02 15:24:33.000000 sail-0.6.6/src/sail.egg-info/requires.txt
+-rw-r--r--   0 dhaval     (501) staff       (20)        5 2023-08-02 15:24:33.000000 sail-0.6.6/src/sail.egg-info/top_level.txt
```

### Comparing `sail-0.6.4/LICENSE` & `sail-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/PKG-INFO` & `sail-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: sail
-Version: 0.6.4
+Version: 0.6.6
 Summary: Python package for streaming data and incremental learning
 Author-email: Dhaval Salwala <dhaval.vinodbhai.salwala@ibm.com>, Seshu Tirupathi <seshutir@ie.ibm.com>
 License: MIT
 Project-URL: repository, https://github.com/IBM/sail
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: tensorflow
 Provides-Extra: tfarm64
 Provides-Extra: pytorch
 Provides-Extra: river
 Provides-Extra: ray
 Provides-Extra: dev
```

### Comparing `sail-0.6.4/README.md` & `sail-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/pyproject.toml` & `sail-0.6.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "version",
     "readme",
 ]
 authors = [
     { name = "Dhaval Salwala", email = "dhaval.vinodbhai.salwala@ibm.com" },
     { name = "Seshu Tirupathi", email = "seshutir@ie.ibm.com" },
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 license = { text = "MIT" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: MIT License",
```

### Comparing `sail-0.6.4/setup.cfg` & `sail-0.6.6/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 	scipy>=1.10
 	pandas>=2.0
 	matplotlib>=3.5.2
 	scikit-learn>=1.2
 
 [options.extras_require]
 tensorflow = 
-	tensorflow>=2.7,<=2.10
+	tensorflow>=2.7,<=2.13
 	scikeras
 	tensorflow-addons
 tfarm64 = 
-	tensorflow-macos>=2.7,<2.10
+	tensorflow-macos>=2.7,<=2.13
 	scikeras
 	tensorflow-addons
 pytorch = 
 	torch>=2.0
 	skorch
 river = 
-	river==0.14.*
+	river==0.18.*
 ray = 
-	ray>=2.0,<2.5
+	ray>=2.5
 	hyperopt
 	tune_sklearn
 dev = 
 	black
 	pylint
 tests = 
 	pytest
```

### Comparing `sail-0.6.4/src/sail/drift_detection/drift_detector.py` & `sail-0.6.6/src/sail/drift_detection/drift_detector.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import importlib
 from typing import Union, Literal
 import river
-from river.base import DriftDetector
-from river.drift import EDDM, PageHinkley
-
+from river.base import DriftDetector, BinaryDriftDetector
+from river.drift.binary import EDDM
+from river.drift.page_hinkley import PageHinkley
 from sail.utils.logging import configure_logger
 from sail.utils.progress_bar import SAILProgressBar
 
 LOGGER = configure_logger()
 
 
 class SAILDriftDetector:
@@ -16,15 +16,17 @@
         model: Union[str, DriftDetector] = EDDM(),
         drift_param: Literal["score", "difference"] = "score",
     ) -> None:
         self._drift_detector = self._resolve_drift_detector(model)
         self.drift_param = drift_param
 
     def _resolve_drift_detector(self, drift_detector) -> DriftDetector:
-        if isinstance(drift_detector, DriftDetector):
+        if isinstance(drift_detector, DriftDetector) or isinstance(
+            drift_detector, BinaryDriftDetector
+        ):
             return drift_detector
         elif isinstance(drift_detector, str):
             if drift_detector == "auto":
                 _drift_detector_class = PageHinkley
             elif isinstance(drift_detector, str):
                 module = importlib.import_module("river.drift")
                 try:
@@ -32,15 +34,15 @@
                 except AttributeError:
                     raise Exception(
                         f"Drift Detector '{drift_detector}' is not available in River. Available drift detectors: {river.drift.__all__}"
                     )
         else:
             raise TypeError(
                 " SAIL Drift Detector `model` must be an instance or str from "
-                f"{river.drift.__all__} from river.drift module. Got {drift_detector.__module__}.{drift_detector.__qualname__}. Set `auto` to use the default."
+                f"{river.drift.__all__} from river.drift module. Got {drift_detector.__module__}.{drift_detector.__class__.__qualname__}. Set `auto` to use the default."
             )
         return _drift_detector_class()
 
     def detect_drift(self, *args):
         if self.drift_param == "difference":
             return self._detect_drift_with_difference(args[1], args[2])
         elif self.drift_param == "score":
```

### Comparing `sail-0.6.4/src/sail/model_selector/base.py` & `sail-0.6.6/src/sail/model_selector/base.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/model_selector/holdout_best_model.py` & `sail-0.6.6/src/sail/model_selector/holdout_best_model.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/model_selector/prequential_best_model.py` & `sail-0.6.6/src/sail/model_selector/prequential_best_model.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/auto_ml/auto_pipeline.py` & `sail-0.6.6/src/sail/models/auto_ml/auto_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import importlib
-import inspect
 import os
 import shutil
 from typing import Type, Union
 
 import numpy as np
 from sklearn.base import BaseEstimator
 from sklearn.utils import check_array
@@ -27,26 +26,24 @@
         pipeline_params_grid: dict,
         search_method: Union[None, str] = None,
         search_method_params: dict = None,
         search_data_size: int = 1000,
         incremental_training: bool = False,
         drift_detector: Union[None, SAILDriftDetector] = None,
         pipeline_strategy: Union[None, str] = None,
-        cluster_address: str = None,
     ) -> None:
         self.pipeline = pipeline
         self.pipeline_params_grid = pipeline_params_grid
         self.search_method_params = search_method_params
         self.search_data_size = search_data_size
         self.incremental_training = incremental_training
         self.drift_detector = drift_detector
-        self.cluster_address = cluster_address
 
         self.search_method = self._resolve_search_method(
-            search_method, search_method_params, cluster_address
+            search_method, search_method_params
         )
         self.pipeline_strategy = self._resolve_pipeline_strategy(
             pipeline_strategy, incremental_training
         )
 
     @property
     def best_pipeline(self) -> SAILPipeline:
@@ -104,17 +101,15 @@
                 y = check_array(
                     np.array(y, ndmin=1),
                     ensure_2d=False,
                 )
 
         return X, y
 
-    def _resolve_search_method(
-        self, search_method, search_method_params, cluster_address
-    ):
+    def _resolve_search_method(self, search_method, search_method_params):
         if search_method is None:
             _search_class = SAILTuneGridSearchCV
         elif Type[search_method] in [
             Type[SAILTuneGridSearchCV],
             Type[SAILTuneSearchCV],
         ]:
             _search_class = search_method
@@ -125,30 +120,29 @@
             except AttributeError:
                 raise Exception(
                     f"Method '{search_method}' is not available. search_method must be from [SAILTuneGridSearchCV, SAILTuneSearchCV] from the module sail.models.auto_ml.tune. Set `None` to use the default."
                 )
         else:
             raise TypeError(
                 "`search_method` must be None or an instance or str from "
-                f"[SAILTuneGridSearchCV, SAILTuneSearchCV] from sail.models.auto_ml.tune. Got {search_method.__module__}.{search_method.__qualname__}. Set `None` to use the default."
+                f"[SAILTuneGridSearchCV, SAILTuneSearchCV] from sail.models.auto_ml.tune. Got {search_method.__module__}.{search_method.__class__.__qualname__}. Set `None` to use the default."
             )
 
         if search_method_params is None:
             search_method_params = _search_class.default_search_params
         else:
             # update params from the default ones if missing any.
             search_method_params = {
                 **_search_class.default_search_params,
                 **search_method_params,
             }
 
         return _search_class(
             estimator=self.pipeline,
             param_grid=self.pipeline_params_grid,
-            cluster_address=cluster_address,
             **search_method_params,
         )
 
     def _resolve_pipeline_strategy(self, pipeline_strategy, incremental_training):
         pipeline_strategy_class = None
         if pipeline_strategy is None:
             pipeline_strategy_class = DetectAndIncrement
@@ -164,15 +158,15 @@
                     "Please select from the list of available strategies: {}".format(
                         pipeline_strategy, PipelineStrategy.defined_stategies
                     )
                 )
         else:
             raise TypeError(
                 "`pipeline_strategy` must be a None, str, "
-                f"or an instance of PipelineStrategy. Got {pipeline_strategy.__module__}.{pipeline_strategy.__qualname__}. Set `None` to use the default."
+                f"or an instance of PipelineStrategy. Got {pipeline_strategy.__module__}.{pipeline_strategy.__class__.__qualname__}. Set `None` to use the default."
             )
 
         return pipeline_strategy_class(
             search_method=self.search_method,
             search_data_size=self.search_data_size,
             drift_detector=self.drift_detector,
             incremental_training=incremental_training,
@@ -210,15 +204,15 @@
                 f"{save_location} already exists, specify overwrite=True to replace contents"
             )
         else:
             # delete old folder to avoid unwanted file overlaps
             if os.path.exists(save_location) and os.path.isdir(save_location):
                 shutil.rmtree(save_location)
 
-            LOGGER.info(f"making directory tree {save_location}")
+            LOGGER.debug(f"making directory tree {save_location}")
             os.makedirs(save_location, exist_ok=True)
             if not os.path.exists(save_location):
                 raise Exception(f"target directory {save_location} can not be created!")
 
         # -------------------------------------------
         # Get all params
         # -------------------------------------------
```

### Comparing `sail-0.6.4/src/sail/models/auto_ml/base_strategy.py` & `sail-0.6.6/src/sail/models/auto_ml/base_strategy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from enum import Enum, auto
 
 import numpy as np
 import ray
-
+import sail
 from sail.drift_detection.drift_detector import SAILDriftDetector
 from sail.utils.logging import configure_logger
 
 LOGGER = configure_logger()
 
 
 class PipelineActionType(Enum):
@@ -171,28 +171,32 @@
     def _find_best_pipeline(self, tune_params={}, warm_start=False, **fit_params):
         class_name = (
             self.search_method.__class__.__module__
             + "."
             + self.search_method.__class__.__qualname__
         )
         LOGGER.info(f"Starting Pipeline tuning with {class_name}")
-        ray.init(address=self.search_method.cluster_address)
+        ray.init(
+            address=self.search_method.cluster_address,
+            namespace=self.search_method.namespace,
+            runtime_env=self.search_method.runtime_env,
+        )
         LOGGER.info(
             f"Cluster resources: Nodes: {len(ray.nodes())}, Cluster CPU: {ray.cluster_resources()['CPU']}, Cluster Memory: {str(format(ray.cluster_resources()['memory'] / (1024 * 1024 * 1024), '.2f')) + ' GB'}"
         )
         try:
             fit_result = self.search_method.fit(
                 X=self._input_X,
                 y=self._input_y,
                 warm_start=warm_start,
                 tune_params=tune_params,
                 **fit_params,
             )
         except Exception as e:
-            LOGGER.debug(e)
+            LOGGER.info(e)
             LOGGER.info("Pipeline tuning failed. Disconnecting Ray cluster...")
         finally:
             ray.shutdown()
         LOGGER.info("Pipeline tuning completed. Disconnecting Ray cluster...")
 
         # set best estimator and fit results
         self._best_pipeline = fit_result.best_estimator_
```

### Comparing `sail-0.6.4/src/sail/models/auto_ml/pipeline_strategy.py` & `sail-0.6.6/src/sail/models/auto_ml/pipeline_strategy.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/auto_ml/searcher.py` & `sail-0.6.6/src/sail/models/auto_ml/searcher.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/auto_ml/tune.py` & `sail-0.6.6/src/sail/models/auto_ml/tune.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 import importlib
-import json
 import os
 import random
 import time
 import warnings
 from operator import *
-from typing import Dict, List
 
 import numpy as np
 from ray import tune
-from ray.tune.experiment import Trial
-from ray.tune.logger import LoggerCallback
 from ray.tune.search import BasicVariantGenerator, ConcurrencyLimiter, Searcher
 from ray.tune.search.bohb import TuneBOHB
 from ray.tune.search.hyperopt import HyperOptSearch
 from ray.tune.search.optuna import OptunaSearch
 from ray.tune.search.skopt import SkOptSearch
 from ray.tune.sklearn import TuneGridSearchCV, TuneSearchCV
 from ray.tune.stopper import CombinedStopper
@@ -74,21 +70,27 @@
 
     def __init__(
         self,
         num_cpus_per_trial=1,
         num_gpus_per_trial=0,
         keep_best_configurations=1,
         cluster_address=None,
+        storage_path=None,
+        namespace=None,
+        runtime_env=None,
         **kwargs,
     ):
         super(SAILTuneGridSearchCV, self).__init__(**kwargs)
-        self.keep_best_configurations = keep_best_configurations
-        self.cluster_address = cluster_address
         self.num_cpus_per_trial = num_cpus_per_trial
         self.num_gpus_per_trial = num_gpus_per_trial
+        self.keep_best_configurations = keep_best_configurations
+        self.cluster_address = cluster_address
+        self.storage_path = storage_path
+        self.namespace = namespace
+        self.runtime_env = runtime_env
 
     def fit(
         self, X, y=None, warm_start=False, groups=None, tune_params=None, **fit_params
     ):
         self.warm_start = warm_start
         return super().fit(X, y, groups, tune_params, **fit_params)
 
@@ -168,14 +170,15 @@
         run_args = dict(
             scheduler=self.early_stopping_,
             reuse_actors=True,
             verbose=self.verbose,
             stop=stopper,
             config=config,
             fail_fast="raise",
+            storage_path=self.storage_path,
             resources_per_trial={
                 "cpu": self.num_cpus_per_trial,
                 "gpu": self.num_gpus_per_trial,
             },
             trial_dirname_creator=lambda trial: f"Trail_{trial.trial_id}",
             name="SAILAutoML_Experiment" + "_" + time.strftime("%d-%m-%Y_%H:%M:%S"),
             callbacks=resolve_logger_callbacks(self.loggers, self.defined_loggers),
@@ -257,21 +260,23 @@
 
     def __init__(
         self,
         num_cpus_per_trial=1,
         num_gpus_per_trial=0,
         keep_best_configurations=1,
         cluster_address=None,
+        storage_path=None,
         **kwargs,
     ):
         super(SAILTuneSearchCV, self).__init__(**kwargs)
-        self.keep_best_configurations = keep_best_configurations
-        self.cluster_address = cluster_address
         self.num_cpus_per_trial = num_cpus_per_trial
         self.num_gpus_per_trial = num_gpus_per_trial
+        self.keep_best_configurations = keep_best_configurations
+        self.cluster_address = cluster_address
+        self.storage_path = storage_path
 
     def fit(
         self, X, y=None, warm_start=False, groups=None, tune_params=None, **fit_params
     ):
         self.warm_start = warm_start
         return super().fit(X, y, groups, tune_params, **fit_params)
 
@@ -335,14 +340,15 @@
             scheduler=self.early_stopping_,
             reuse_actors=True,
             verbose=self.verbose,
             stop=stopper,
             num_samples=self.n_trials,
             config=config,
             fail_fast="raise",
+            storage_path=self.storage_path,
             resources_per_trial={
                 "cpu": self.num_cpus_per_trial,
                 "gpu": self.num_gpus_per_trial,
             },
             local_dir=self.local_dir,
             name="SAILAutoML_Experiment" + "_" + time.strftime("%d-%m-%Y_%H:%M:%S"),
             callbacks=resolve_logger_callbacks(self.loggers, self.defined_loggers),
```

### Comparing `sail-0.6.4/src/sail/models/base.py` & `sail-0.6.6/src/sail/models/base.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/ensemble/base.py` & `sail-0.6.6/src/sail/models/ensemble/base.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/ensemble/distAggregateClassifier.py` & `sail-0.6.6/src/sail/models/ensemble/distAggregateClassifier.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/ensemble/distAggregateRegressor.py` & `sail-0.6.6/src/sail/models/ensemble/distAggregateRegressor.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/ensemble/distEWARegressor.py` & `sail-0.6.6/src/sail/models/ensemble/distEWARegressor.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/keras/base.py` & `sail-0.6.6/src/sail/models/keras/base.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/keras/oselm.py` & `sail-0.6.6/src/sail/models/keras/oselm.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/keras/wglstm.py` & `sail-0.6.6/src/sail/models/keras/wglstm.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,17 +31,15 @@
         self.window_size = window_size
         self.add(
             tf.keras.layers.LSTM(
                 hidden_layer_neurons,
                 return_sequences=True,
                 stateful=True,
                 batch_input_shape=(1, timesteps, num_of_features),
-                kernel_regularizer=tf.keras.regularizers.l2(
-                    regularization_factor
-                ),
+                kernel_regularizer=tf.keras.regularizers.l2(regularization_factor),
             )
         )
         self.add(
             tf.keras.layers.TimeDistributed(
                 tf.keras.layers.Dense(units=num_of_features)
             )
         )
@@ -108,18 +106,15 @@
 
                 testval = point_diff * 1.0 / (sum(norm_diff) / len(norm_diff))
                 curmean = resi_mean
                 curvar = resi_var
                 tmp_zval = (tmpresi - curmean) * 1.0 / sqrt(curvar)
                 tmp_pro_conve = st.norm.cdf(tmp_zval)
 
-                if (
-                    tmp_pro_conve > (1 - conf_level)
-                    or tmp_pro_conve < conf_level
-                ):
+                if tmp_pro_conve > (1 - conf_level) or tmp_pro_conve < conf_level:
                     sus_point_bool = True
                     pre_susp_bool = True
                     weight = tmpw
                     win_susp.append(1)
                     win_susp.pop(0)
 
                     if outlier_flag[i + 1] == 1:
@@ -171,17 +166,17 @@
                 self.train_on_batch(tmp_cur_trnx, tmp_cur_trny * (weight))
 
             cur_pred = self.predict_on_batch(tmp_cur_trnx)[0][0][0]
             tmpresi = weight * (tmp_cur_trny[0][0][0] - cur_pred)
             resi_mean = resi_mean * seg_cnt * 1.0 / (seg_cnt + 1) + tmpresi / (
                 seg_cnt + 1
             )
-            resi_sqr = resi_sqr * seg_cnt * 1.0 / (
+            resi_sqr = resi_sqr * seg_cnt * 1.0 / (seg_cnt + 1) + tmpresi * tmpresi / (
                 seg_cnt + 1
-            ) + tmpresi * tmpresi / (seg_cnt + 1)
+            )
             resi_var = resi_sqr - resi_mean * resi_mean
             seg_cnt = seg_cnt + 1
 
             # ----------------prediction-------------------------- #
             if sus_point_bool is True:
                 vali_testx = copy.deepcopy(x[:, i : i + 1, :])
                 vali_testx[0][0][0] = cur_pred_ini
@@ -198,17 +193,15 @@
         # plot_series(
         #     y_orig,
         #     y_pred,
         #     plot_title="Online Prediction by WGSLTM on Bike rental",
         #     save_path="plot_wglstm.png",
         # )
 
-        return SimpleNamespace(
-            history={m.name: m.result() for m in self.metrics}
-        )
+        return SimpleNamespace(history={m.name: m.result() for m in self.metrics})
 
     def sliding_window_features(self, cur_pos, dataX, dataY, susp_list):
         winsize = self.window_size
         resi_list = []
         for i in range(cur_pos - winsize, cur_pos):
             cur_trnx = dataX[:, i : i + 1, :]
             cur_trny = dataY[:, i : i + 1, :]
@@ -227,51 +220,40 @@
             cur_val = dataX[:, i : i + 1, :][0][0][0]
             if susp_list[i - (cur_pos - winsize)] == 0:
                 if lnormal == -1:
                     lnormal = i
                     tmpdiff.append(0.0)
                 else:
                     tmpdiff.append(
-                        abs(
-                            cur_val
-                            - dataX[:, lnormal : lnormal + 1, :][0][0][0]
-                        )
+                        abs(cur_val - dataX[:, lnormal : lnormal + 1, :][0][0][0])
                     )
                     lnormal = i
             else:
                 rsus = i
                 if i >= (cur_pos - winsize):
-                    tmpdiff.append(
-                        abs(cur_val - dataX[:, i - 1 : i, :][0][0][0])
-                    )
+                    tmpdiff.append(abs(cur_val - dataX[:, i - 1 : i, :][0][0][0]))
                 else:
                     tmpdiff.append(abs(0.0))
 
         for i in range(cur_pos - winsize, cur_pos):
             tmp_dta = cur_pos - (i - (cur_pos - winsize)) - 1
             cur_val = dataX[:, tmp_dta : tmp_dta + 1, :][0][0][0]
             tmp_win = tmp_dta - (cur_pos - winsize)
             if susp_list[tmp_win] == 0:
                 if rnormal == -1:
                     rnormal = tmp_dta
                 else:
                     tmpdiff[tmp_win] = tmpdiff[tmp_win] + (
-                        abs(
-                            cur_val
-                            - dataX[:, rnormal : rnormal + 1, :][0][0][0]
-                        )
+                        abs(cur_val - dataX[:, rnormal : rnormal + 1, :][0][0][0])
                     )
                     rnormal = tmp_dta
             else:
                 if tmp_dta <= (cur_pos - 1):
                     tmpdiff[tmp_win] = tmpdiff[tmp_win] + (
-                        abs(
-                            cur_val
-                            - dataX[:, tmp_dta + 1 : tmp_dta + 2, :][0][0][0]
-                        )
+                        abs(cur_val - dataX[:, tmp_dta + 1 : tmp_dta + 2, :][0][0][0])
                     )
 
         tmparr = list(zip(tmpdiff, susp_list))
         norm_diff = [i[0] for i in tmparr if i[1] == 0]
         susp_diff = [i[0] for i in tmparr if i[1] == 1]
 
         tmpdiff = -1
@@ -289,21 +271,15 @@
         return norm_diff, susp_diff, tmpdiff
 
     def sliding_window_weight(self, normDiff, suspDiff, pnt_diff):
         weight_mag = 5
         weight_beta = 0.05
 
         if len(suspDiff) != 0 and len(normDiff) != 0:
-            r2 = (
-                1.0
-                * sum(suspDiff)
-                * len(normDiff)
-                / sum(normDiff)
-                / len(suspDiff)
-            )
+            r2 = 1.0 * sum(suspDiff) * len(normDiff) / sum(normDiff) / len(suspDiff)
             if r2 < 5:
                 r2 = 0.0
 
         if len(normDiff) != 0:
             tmpr = pnt_diff * 1.0 / (sum(normDiff) / len(normDiff))
             if tmpr > weight_mag:
                 tmpw = np.exp(-1 * weight_beta * tmpr)
@@ -374,15 +350,15 @@
 
     """
 
     def __init__(
         self,
         loss="mse",
         optimizer=tf.keras.optimizers.SGD(
-            learning_rate=0.002, momentum=0.03, decay=0.0, nesterov=True
+            learning_rate=0.002, momentum=0.03, nesterov=True
         ),
         metrics=None,
         epochs=1,
         verbose=0,
         num_of_features=1,
         hidden_layer_neurons=450,
         hidden_layer_activation="linear",
```

### Comparing `sail-0.6.4/src/sail/models/native/base.py` & `sail-0.6.6/src/sail/models/native/base.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/native/ielm.py` & `sail-0.6.6/src/sail/models/native/ielm.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/native/isvm.py` & `sail-0.6.6/src/sail/models/native/isvm.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/native/lasvm.py` & `sail-0.6.6/src/sail/models/native/lasvm.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/native/learn_pp.py` & `sail-0.6.6/src/sail/models/native/learn_pp.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/native/robust_iml.py` & `sail-0.6.6/src/sail/models/native/robust_iml.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/river/base.py` & `sail-0.6.6/src/sail/models/river/base.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/river/ensemble.py` & `sail-0.6.6/src/sail/models/river/ensemble.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/river/forest.py` & `sail-0.6.6/src/sail/models/river/forest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 import typing
 
-import river.ensemble.adaptive_random_forest as adaptive_random_forest
+from river.forest import ARFClassifier, ARFRegressor
 from river import base, metrics
-from river.drift import ADWIN
 from river.tree.splitter import Splitter
 from sail.models.river.base import SailRiverClassifier, SailRiverRegressor
 
 __all__ = [
     "AdaptiveRandomForestClassifier",
     "AdaptiveRandomForestRegressor",
 ]
 
 
 class AdaptiveRandomForestClassifier(SailRiverClassifier):
     def __init__(
         self,
         n_models: int = 10,
-        max_features: typing.Union[bool, str, int] = "sqrt",
+        max_features: bool | str | int = "sqrt",
         lambda_value: int = 6,
-        metric: metrics.base.MultiClassMetric = metrics.Accuracy(),
+        metric: metrics.base.MultiClassMetric | None = None,
         disable_weighted_vote=False,
-        drift_detector: typing.Union[base.DriftDetector, None] = ADWIN(delta=0.001),
-        warning_detector: typing.Union[base.DriftDetector, None] = ADWIN(delta=0.01),
+        drift_detector: base.DriftDetector | None = None,
+        warning_detector: base.DriftDetector | None = None,
         # Tree parameters
         grace_period: int = 50,
-        max_depth: int = None,
+        max_depth: int | None = None,
         split_criterion: str = "info_gain",
         delta: float = 0.01,
         tau: float = 0.05,
         leaf_prediction: str = "nba",
         nb_threshold: int = 0,
-        nominal_attributes: list = None,
-        splitter: Splitter = None,
+        nominal_attributes: list | None = None,
+        splitter: Splitter | None = None,
         binary_split: bool = False,
+        min_branch_fraction: float = 0.01,
+        max_share_to_split: float = 0.99,
         max_size: float = 100.0,
         memory_estimate_period: int = 2_000_000,
         stop_mem_management: bool = False,
         remove_poor_attrs: bool = False,
         merit_preprune: bool = True,
-        seed: int = None,
+        seed: int | None = None,
     ):
         super(AdaptiveRandomForestClassifier, self).__init__(
-            river_estimator=adaptive_random_forest.AdaptiveRandomForestClassifier(
+            river_estimator=ARFClassifier(
                 n_models,
                 max_features,
                 lambda_value,
                 metric,
                 disable_weighted_vote,
                 drift_detector,
                 warning_detector,
@@ -55,56 +56,59 @@
                 delta,
                 tau,
                 leaf_prediction,
                 nb_threshold,
                 nominal_attributes,
                 splitter,
                 binary_split,
+                min_branch_fraction,
+                max_share_to_split,
                 max_size,
                 memory_estimate_period,
                 stop_mem_management,
                 remove_poor_attrs,
                 merit_preprune,
                 seed,
             )
         )
 
 
 class AdaptiveRandomForestRegressor(SailRiverRegressor):
     def __init__(
         self,
+        # Forest parameters
         n_models: int = 10,
         max_features="sqrt",
         aggregation_method: str = "median",
         lambda_value: int = 6,
-        metric: metrics.base.RegressionMetric = metrics.MSE(),
+        metric: metrics.base.RegressionMetric | None = None,
         disable_weighted_vote=True,
-        drift_detector: base.DriftDetector = ADWIN(0.001),
-        warning_detector: base.DriftDetector = ADWIN(0.01),
+        drift_detector: base.DriftDetector | None = None,
+        warning_detector: base.DriftDetector | None = None,
         # Tree parameters
         grace_period: int = 50,
-        max_depth: int = None,
+        max_depth: int | None = None,
         delta: float = 0.01,
         tau: float = 0.05,
         leaf_prediction: str = "adaptive",
-        leaf_model: base.Regressor = None,
+        leaf_model: base.Regressor | None = None,
         model_selector_decay: float = 0.95,
-        nominal_attributes: list = None,
-        splitter: Splitter = None,
+        nominal_attributes: list | None = None,
+        splitter: Splitter | None = None,
         min_samples_split: int = 5,
         binary_split: bool = False,
         max_size: float = 500.0,
         memory_estimate_period: int = 2_000_000,
         stop_mem_management: bool = False,
         remove_poor_attrs: bool = False,
         merit_preprune: bool = True,
-        seed: int = None,
+        seed: int | None = None,
     ):
         super(AdaptiveRandomForestRegressor, self).__init__(
-            river_estimator=adaptive_random_forest.AdaptiveRandomForestRegressor(
+            river_estimator=ARFRegressor(
                 n_models,
                 max_features,
                 aggregation_method,
                 lambda_value,
                 metric,
                 disable_weighted_vote,
                 drift_detector,
```

### Comparing `sail-0.6.4/src/sail/models/river/linear_model.py` & `sail-0.6.6/src/sail/models/river/linear_model.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/river/naive_bayes.py` & `sail-0.6.6/src/sail/models/river/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/river/neighbors.py` & `sail-0.6.6/src/sail/models/river/neighbors.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/sklearn/base.py` & `sail-0.6.6/src/sail/models/sklearn/base.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/torch/base.py` & `sail-0.6.6/src/sail/models/torch/base.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/torch/data.py` & `sail-0.6.6/src/sail/models/torch/data.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/torch/fcn.py` & `sail-0.6.6/src/sail/models/torch/fcn.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/torch/fcn_classification.py` & `sail-0.6.6/src/sail/models/torch/fcn_classification.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/torch/inceptiontime.py` & `sail-0.6.6/src/sail/models/torch/inceptiontime.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/torch/layers.py` & `sail-0.6.6/src/sail/models/torch/layers.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/torch/light_lstm.py` & `sail-0.6.6/src/sail/models/torch/light_lstm.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/torch/lstm.py` & `sail-0.6.6/src/sail/models/torch/lstm.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/torch/lstm_fcn.py` & `sail-0.6.6/src/sail/models/torch/lstm_fcn.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/torch/nn.py` & `sail-0.6.6/src/sail/models/torch/nn.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/torch/onn_hbp.py` & `sail-0.6.6/src/sail/models/torch/onn_hbp.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/torch/os_cnn.py` & `sail-0.6.6/src/sail/models/torch/os_cnn.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/torch/rnn.py` & `sail-0.6.6/src/sail/models/torch/rnn.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/torch/rocket.py` & `sail-0.6.6/src/sail/models/torch/rocket.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/torch/tcn.py` & `sail-0.6.6/src/sail/models/torch/tcn.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/models/torch/utils.py` & `sail-0.6.6/src/sail/models/torch/utils.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/pipeline/pipeline.py` & `sail-0.6.6/src/sail/pipeline/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,15 @@
                 f"{save_location} already exists, specify overwrite=True to replace contents"
             )
         else:
             # delete old folder to avoid unwanted file overlaps
             if os.path.exists(save_location) and os.path.isdir(save_location):
                 shutil.rmtree(save_location)
 
-            LOGGER.info(f"making directory tree {save_location}")
+            LOGGER.debug(f"making directory tree {save_location}")
             os.makedirs(save_location, exist_ok=True)
             if not os.path.exists(save_location):
                 raise Exception(f"target directory {save_location} can not be created!")
 
         # -------------------------------------------
         # explicity save all the steps and steps names
         # -------------------------------------------
```

### Comparing `sail-0.6.4/src/sail/transfomers/river/feature_extraction.py` & `sail-0.6.6/src/sail/transfomers/river/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/transfomers/river/feature_selection.py` & `sail-0.6.6/src/sail/transfomers/river/feature_selection.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/transfomers/river/preprocessing.py` & `sail-0.6.6/src/sail/transfomers/river/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/transfomers/sklearn/preprocessing.py` & `sail-0.6.6/src/sail/transfomers/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/utils/logging.py` & `sail-0.6.6/src/sail/utils/logging.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/utils/progress_bar.py` & `sail-0.6.6/src/sail/utils/progress_bar.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/utils/ray_utils.py` & `sail-0.6.6/src/sail/utils/ray_utils.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/utils/scorer.py` & `sail-0.6.6/src/sail/utils/scorer.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import inspect
 import sys
 
 import numpy as np
 
 import river
 from river import metrics
-from sympy import public
 
 from sail.utils.progress_bar import SAILProgressBar
 
 
 class SAILModelScorer:
     def __init__(
         self,
```

### Comparing `sail-0.6.4/src/sail/utils/serialization.py` & `sail-0.6.6/src/sail/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/utils/ts_utils.py` & `sail-0.6.6/src/sail/utils/ts_utils.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail/visualisation/ts_plot.py` & `sail-0.6.6/src/sail/visualisation/ts_plot.py`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail.egg-info/PKG-INFO` & `sail-0.6.6/src/sail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: sail
-Version: 0.6.4
+Version: 0.6.6
 Summary: Python package for streaming data and incremental learning
 Author-email: Dhaval Salwala <dhaval.vinodbhai.salwala@ibm.com>, Seshu Tirupathi <seshutir@ie.ibm.com>
 License: MIT
 Project-URL: repository, https://github.com/IBM/sail
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: tensorflow
 Provides-Extra: tfarm64
 Provides-Extra: pytorch
 Provides-Extra: river
 Provides-Extra: ray
 Provides-Extra: dev
```

### Comparing `sail-0.6.4/src/sail.egg-info/SOURCES.txt` & `sail-0.6.6/src/sail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sail-0.6.4/src/sail.egg-info/requires.txt` & `sail-0.6.6/src/sail.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -38,29 +38,29 @@
 liac-arff
 
 [pytorch]
 torch>=2.0
 skorch
 
 [ray]
-ray<2.5,>=2.0
+ray>=2.5
 hyperopt
 tune_sklearn
 
 [river]
-river==0.14.*
+river==0.18.*
 
 [tensorflow]
-tensorflow<=2.10,>=2.7
+tensorflow<=2.13,>=2.7
 scikeras
 tensorflow-addons
 
 [tests]
 pytest
 nbmake
 pytest-xdist
 pytest-console-scripts
 
 [tfarm64]
-tensorflow-macos<2.10,>=2.7
+tensorflow-macos<=2.13,>=2.7
 scikeras
 tensorflow-addons
```


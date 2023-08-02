# Comparing `tmp/pyPhasesML-0.7.7.tar.gz` & `tmp/pyPhasesML-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPhasesML-0.7.7.tar", last modified: Mon Jul 31 14:55:44 2023, max compression
+gzip compressed data, was "pyPhasesML-0.7.8.tar", last modified: Wed Aug  2 07:24:32 2023, max compression
```

## Comparing `pyPhasesML-0.7.7.tar` & `pyPhasesML-0.7.8.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:55:44.343019 pyPhasesML-0.7.7/
--rw-rw-rw-   0 root         (0) root         (0)     1065 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3690 2023-07-31 14:55:44.343019 pyPhasesML-0.7.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3183 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:55:44.337019 pyPhasesML-0.7.7/pyPhasesML/
--rw-rw-rw-   0 root         (0) root         (0)     2410 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/DataAugmentation.py
--rw-rw-rw-   0 root         (0) root         (0)      895 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/DataSet.py
--rw-rw-rw-   0 root         (0) root         (0)     3849 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/DataversionManager.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/FeatureExtraction.py
--rw-rw-rw-   0 root         (0) root         (0)     4074 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/Model.py
--rw-rw-rw-   0 root         (0) root         (0)       94 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/ModelAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)     4952 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/ModelManager.py
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/Plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     4566 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/SignalPreprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:55:44.339018 pyPhasesML-0.7.7/pyPhasesML/adapter/
--rw-rw-rw-   0 root         (0) root         (0)    10255 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/adapter/ModelKerasAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)     7159 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/adapter/ModelTf1Adapter.py
--rw-rw-rw-   0 root         (0) root         (0)     9986 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/adapter/ModelTorchAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/adapter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:55:44.341019 pyPhasesML-0.7.7/pyPhasesML/adapter/torch/
--rw-rw-rw-   0 root         (0) root         (0)      734 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/adapter/torch/CSVLogger.py
--rw-rw-rw-   0 root         (0) root         (0)     1654 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/adapter/torch/Callback.py
--rw-rw-rw-   0 root         (0) root         (0)     3710 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/adapter/torch/CheckPoint.py
--rw-rw-rw-   0 root         (0) root         (0)     2001 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/adapter/torch/CyclicLearningrate.py
--rw-rw-rw-   0 root         (0) root         (0)     2046 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/adapter/torch/FindLearningRate.py
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/adapter/torch/LoadOptimizer.py
--rw-rw-rw-   0 root         (0) root         (0)     2430 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/adapter/torch/SystemCheckPoint.py
--rw-rw-rw-   0 root         (0) root         (0)       97 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/adapter/torch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1106 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:55:44.341019 pyPhasesML-0.7.7/pyPhasesML/datapipes/
--rw-rw-rw-   0 root         (0) root         (0)      464 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/datapipes/Augmentor.py
--rw-rw-rw-   0 root         (0) root         (0)      626 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/datapipes/DatasetXY.py
--rw-rw-rw-   0 root         (0) root         (0)      995 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/datapipes/FoldMapper.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/datapipes/RecordMap.py
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/datapipes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:55:44.342018 pyPhasesML-0.7.7/pyPhasesML/exporter/
--rw-rw-rw-   0 root         (0) root         (0)     5385 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/exporter/MemmapRecordExporter.py
--rw-rw-rw-   0 root         (0) root         (0)     3201 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/exporter/ModelExporter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/exporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:55:44.343019 pyPhasesML-0.7.7/pyPhasesML/scorer/
--rw-rw-rw-   0 root         (0) root         (0)    19017 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/scorer/Scorer.py
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/scorer/ScorerTF.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/scorer/ScorerTorch.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyPhasesML/scorer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:55:44.338019 pyPhasesML-0.7.7/pyPhasesML.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3690 2023-07-31 14:55:44.000000 pyPhasesML-0.7.7/pyPhasesML.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1398 2023-07-31 14:55:44.000000 pyPhasesML-0.7.7/pyPhasesML.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 14:55:44.000000 pyPhasesML-0.7.7/pyPhasesML.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-31 14:55:44.000000 pyPhasesML-0.7.7/pyPhasesML.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-07-31 14:55:44.000000 pyPhasesML-0.7.7/pyPhasesML.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      484 2023-07-31 14:55:25.000000 pyPhasesML-0.7.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 14:55:44.343019 pyPhasesML-0.7.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      842 2023-07-31 14:55:27.000000 pyPhasesML-0.7.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:24:32.526917 pyPhasesML-0.7.8/
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3690 2023-08-02 07:24:32.526917 pyPhasesML-0.7.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3183 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:24:32.520917 pyPhasesML-0.7.8/pyPhasesML/
+-rw-rw-rw-   0 root         (0) root         (0)     2410 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/DataAugmentation.py
+-rw-rw-rw-   0 root         (0) root         (0)      895 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/DataSet.py
+-rw-rw-rw-   0 root         (0) root         (0)     3849 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/DataversionManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/FeatureExtraction.py
+-rw-rw-rw-   0 root         (0) root         (0)     4074 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/Model.py
+-rw-rw-rw-   0 root         (0) root         (0)       94 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/ModelAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     4952 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/ModelManager.py
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4566 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/SignalPreprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:24:32.522917 pyPhasesML-0.7.8/pyPhasesML/adapter/
+-rw-rw-rw-   0 root         (0) root         (0)    10255 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/adapter/ModelKerasAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     7159 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/adapter/ModelTf1Adapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     9901 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/adapter/ModelTorchAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/adapter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:24:32.523917 pyPhasesML-0.7.8/pyPhasesML/adapter/torch/
+-rw-rw-rw-   0 root         (0) root         (0)      734 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/adapter/torch/CSVLogger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1654 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/adapter/torch/Callback.py
+-rw-rw-rw-   0 root         (0) root         (0)     3710 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/adapter/torch/CheckPoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2001 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/adapter/torch/CyclicLearningrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1549 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/adapter/torch/FindLearningRate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/adapter/torch/LoadOptimizer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2430 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/adapter/torch/SystemCheckPoint.py
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/adapter/torch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:24:32.524917 pyPhasesML-0.7.8/pyPhasesML/datapipes/
+-rw-rw-rw-   0 root         (0) root         (0)      464 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/datapipes/Augmentor.py
+-rw-rw-rw-   0 root         (0) root         (0)      626 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/datapipes/DatasetXY.py
+-rw-rw-rw-   0 root         (0) root         (0)      995 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/datapipes/FoldMapper.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/datapipes/RecordMap.py
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/datapipes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:24:32.525917 pyPhasesML-0.7.8/pyPhasesML/exporter/
+-rw-rw-rw-   0 root         (0) root         (0)     5385 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/exporter/MemmapRecordExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/exporter/ModelExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/exporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:24:32.526917 pyPhasesML-0.7.8/pyPhasesML/scorer/
+-rw-rw-rw-   0 root         (0) root         (0)    19017 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/scorer/Scorer.py
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/scorer/ScorerTF.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/scorer/ScorerTorch.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyPhasesML/scorer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:24:32.521917 pyPhasesML-0.7.8/pyPhasesML.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3690 2023-08-02 07:24:32.000000 pyPhasesML-0.7.8/pyPhasesML.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1398 2023-08-02 07:24:32.000000 pyPhasesML-0.7.8/pyPhasesML.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 07:24:32.000000 pyPhasesML-0.7.8/pyPhasesML.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-08-02 07:24:32.000000 pyPhasesML-0.7.8/pyPhasesML.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-08-02 07:24:32.000000 pyPhasesML-0.7.8/pyPhasesML.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      484 2023-08-02 07:24:15.000000 pyPhasesML-0.7.8/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-02 07:24:32.526917 pyPhasesML-0.7.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      842 2023-08-02 07:24:16.000000 pyPhasesML-0.7.8/setup.py
```

### Comparing `pyPhasesML-0.7.7/LICENSE` & `pyPhasesML-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.7/PKG-INFO` & `pyPhasesML-0.7.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.7.7
+Version: 0.7.8
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.7.7/README.md` & `pyPhasesML-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.7/pyPhasesML/DataAugmentation.py` & `pyPhasesML-0.7.8/pyPhasesML/DataAugmentation.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.7/pyPhasesML/DataSet.py` & `pyPhasesML-0.7.8/pyPhasesML/DataSet.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.7/pyPhasesML/DataversionManager.py` & `pyPhasesML-0.7.8/pyPhasesML/DataversionManager.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.7/pyPhasesML/FeatureExtraction.py` & `pyPhasesML-0.7.8/pyPhasesML/FeatureExtraction.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.7/pyPhasesML/Model.py` & `pyPhasesML-0.7.8/pyPhasesML/Model.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.7/pyPhasesML/ModelManager.py` & `pyPhasesML-0.7.8/pyPhasesML/ModelManager.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.7/pyPhasesML/Plugin.py` & `pyPhasesML-0.7.8/pyPhasesML/Plugin.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.7/pyPhasesML/SignalPreprocessing.py` & `pyPhasesML-0.7.8/pyPhasesML/SignalPreprocessing.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.7/pyPhasesML/adapter/ModelKerasAdapter.py` & `pyPhasesML-0.7.8/pyPhasesML/adapter/ModelKerasAdapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.7/pyPhasesML/adapter/ModelTf1Adapter.py` & `pyPhasesML-0.7.8/pyPhasesML/adapter/ModelTf1Adapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.7/pyPhasesML/adapter/ModelTorchAdapter.py` & `pyPhasesML-0.7.8/pyPhasesML/adapter/ModelTorchAdapter.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 class ModelTorchAdapter(ModelAdapter):
     model: torch.nn.Module
     useGPU = torch.cuda.is_available()
 
     def __init__(self, options=None) -> None:
         super().__init__(options)
         self.cbs = []
+        self.skipValidation = False
 
     def prepareX(self, x, validation=False):
         x = x.permute(0, 2, 1)
         return x
 
     def prepareDataAdapter(self, datasetOrTuple, validation=False):
         x, y = datasetOrTuple
@@ -211,18 +212,16 @@
                 currentCount = processList.n + 1
                 processList.set_postfix(ordered_dict={n: v / currentCount for n, v in self.runningStats.items()})
 
             self.runningStats = {n: v / batchesPerEpoch for n, v in self.runningStats.items()}
 
             self.epoch += 1
 
-            # Get validation accuracy
-            self.validate(dataset.validationData)
-
-            # If the validation accuracy improves, print out training and validation accuracy values and checkpoint the model
+            if not self.skipValidation:
+                self.validate(dataset.validationData)
 
             if self.finish:
                 break
 
         self.trigger("trainingEnd", self)
 
         self.fullEpochs = self.epoch
```

### Comparing `pyPhasesML-0.7.7/pyPhasesML/adapter/torch/CSVLogger.py` & `pyPhasesML-0.7.8/pyPhasesML/adapter/torch/CSVLogger.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.7/pyPhasesML/adapter/torch/Callback.py` & `pyPhasesML-0.7.8/pyPhasesML/adapter/torch/Callback.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.7/pyPhasesML/adapter/torch/CheckPoint.py` & `pyPhasesML-0.7.8/pyPhasesML/adapter/torch/CheckPoint.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.7/pyPhasesML/adapter/torch/CyclicLearningrate.py` & `pyPhasesML-0.7.8/pyPhasesML/adapter/torch/CyclicLearningrate.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.7/pyPhasesML/adapter/torch/FindLearningRate.py` & `pyPhasesML-0.7.8/pyPhasesML/adapter/torch/FindLearningRate.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,49 @@
 import math
 import numpy as np
 
 from pyPhases import classLogger
 from pyPhasesML.Model import ModelConfig
 from pyPhasesML.adapter.torch.Callback import Callback
+from pyPhases import CSVLogger as Logger
 
 
 @classLogger
 class FindLearningRate(Callback):
     def __init__(self, config: ModelConfig, minLR, maxLR, iterations=3) -> None:
         super().__init__(config)
         self.smoothing = 0.05
-        self.findLearningRatePlotPath = self.getLogPath() + "/lrRangeTest.png"
+        self.csvPath = self.getLogPath() + "/rangetest.png"
         self.minLR = minLR
         self.maxLR = maxLR
         self.iterations = iterations
+        self.logger = Logger(self.csvPath)
 
     def onTrainingStart(self, model, dataset):
         import torch
         model.maxEpochs = self.iterations
         start_lr = self.minLR
         end_lr = self.maxLR
 
         def cyclical_lr(x):
             return math.exp(x * math.log(end_lr / start_lr) / (model.maxEpochs * len(dataset.trainingData)))
 
         model.batchScheduler = torch.optim.lr_scheduler.LambdaLR(model.optimizer, cyclical_lr)
-        self.lr_find_loss = []
-        self.lr_find_lr = []
+        model.skipValidation = True
+
 
     def onBatchEnd(self, model, batchIndex):
         lr_step = model.optimizer.state_dict()["param_groups"][0]["lr"]
-        self.lr_find_lr.append(lr_step)
 
         # smooth the loss
         loss = model.runningStats["loss"]
         if batchIndex == 0 and model.epoch == 0:
-            self.lr_find_loss.append(loss)
+            loss_smooth = loss
         else:
-            loss = self.smoothing * loss + (1 - self.smoothing) * self.lr_find_loss[-1]
-            self.lr_find_loss.append(loss)
-
-    def onTrainingEnd(self, model):
-        from matplotlib import pyplot as plt
+            loss_smooth = self.smoothing * loss + (1 - self.smoothing) * self.lr_find_loss[-1]
+        
+        self.logger.addCsvRow({
+            "step": lr_step,
+            "loss": loss,
+            "loss_smooth": lr_step,
+        })
 
-        plt.ylabel("loss")
-        plt.xlabel("Learning Rate")
-        plt.xscale("log")
-        plt.plot(self.lr_find_lr, self.lr_find_loss)
-        plt.savefig(self.findLearningRatePlotPath)
-        minLr = self.lr_find_lr[np.argmin(self.lr_find_loss)]
-        print("Lowest Loss LR: %f" % minLr)
-        print("Suggested LR range max bound: %f" % minLr)
-        print("Graph save in: %s" % self.findLearningRatePlotPath)
-        self.lr_find_lr = self.lr_find_lr
-        self.lr_find_loss = self.lr_find_loss
```

### Comparing `pyPhasesML-0.7.7/pyPhasesML/adapter/torch/LoadOptimizer.py` & `pyPhasesML-0.7.8/pyPhasesML/adapter/torch/LoadOptimizer.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.7/pyPhasesML/adapter/torch/SystemCheckPoint.py` & `pyPhasesML-0.7.8/pyPhasesML/adapter/torch/SystemCheckPoint.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.7/pyPhasesML/config.yaml` & `pyPhasesML-0.7.8/pyPhasesML/config.yaml`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.7/pyPhasesML/datapipes/DatasetXY.py` & `pyPhasesML-0.7.8/pyPhasesML/datapipes/DatasetXY.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.7/pyPhasesML/datapipes/FoldMapper.py` & `pyPhasesML-0.7.8/pyPhasesML/datapipes/FoldMapper.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.7/pyPhasesML/exporter/MemmapRecordExporter.py` & `pyPhasesML-0.7.8/pyPhasesML/exporter/MemmapRecordExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.7/pyPhasesML/exporter/ModelExporter.py` & `pyPhasesML-0.7.8/pyPhasesML/exporter/ModelExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.7/pyPhasesML/scorer/Scorer.py` & `pyPhasesML-0.7.8/pyPhasesML/scorer/Scorer.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.7/pyPhasesML.egg-info/PKG-INFO` & `pyPhasesML-0.7.8/pyPhasesML.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.7.7
+Version: 0.7.8
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.7.7/pyPhasesML.egg-info/SOURCES.txt` & `pyPhasesML-0.7.8/pyPhasesML.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.7/setup.py` & `pyPhasesML-0.7.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyPhasesML",
-    version="v0.7.7"[1:],
+    version="v0.7.8"[1:],
     author="Franz Ehrlich",
     author_email="fehrlichd@gmail.com",
     description="A Framework for creating a boilerplate template for ai projects that are ready for MLOps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/",
     packages=setuptools.find_packages(),
```


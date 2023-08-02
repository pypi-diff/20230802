# Comparing `tmp/conplex_dti-0.1.6.tar.gz` & `tmp/conplex_dti-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conplex_dti-0.1.6.tar", max compression
+gzip compressed data, was "conplex_dti-0.1.7.tar", max compression
```

## Comparing `conplex_dti-0.1.6.tar` & `conplex_dti-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1074 2023-03-11 16:53:19.162872 conplex_dti-0.1.6/LICENSE
--rwxr-xr-x   0        0        0     4803 2023-08-02 16:23:54.758153 conplex_dti-0.1.6/README.md
--rw-r--r--   0        0        0     3510 2023-06-14 01:47:41.847038 conplex_dti-0.1.6/conplex_dti/MAIN_OLD.txt
--rw-r--r--   0        0        0      399 2023-06-14 01:47:41.848725 conplex_dti-0.1.6/conplex_dti/__init__.py
--rw-r--r--   0        0        0     1094 2023-07-09 05:21:18.079836 conplex_dti-0.1.6/conplex_dti/__main__.py
--rw-r--r--   0        0        0    23714 2023-06-14 01:47:41.852511 conplex_dti-0.1.6/conplex_dti/architectures.py
--rw-r--r--   0        0        0      251 2023-07-09 05:21:18.081792 conplex_dti-0.1.6/conplex_dti/cli/__init__.py
--rw-r--r--   0        0        0     3859 2023-07-09 05:21:15.929266 conplex_dti-0.1.6/conplex_dti/cli/download.py
--rw-r--r--   0        0        0     4268 2023-08-02 16:21:58.562681 conplex_dti-0.1.6/conplex_dti/cli/predict.py
--rw-r--r--   0        0        0    19588 2023-07-09 05:21:15.932012 conplex_dti-0.1.6/conplex_dti/cli/train.py
--rw-r--r--   0        0        0      171 2023-07-09 05:21:15.934053 conplex_dti-0.1.6/conplex_dti/dataset/__init__.py
--rw-r--r--   0        0        0    24300 2023-07-09 05:21:15.936761 conplex_dti-0.1.6/conplex_dti/dataset/datamodules.py
--rw-r--r--   0        0        0      421 2023-06-14 01:47:41.919180 conplex_dti-0.1.6/conplex_dti/featurizer/__init__.py
--rw-r--r--   0        0        0     7765 2023-06-14 20:00:03.681608 conplex_dti-0.1.6/conplex_dti/featurizer/base.py
--rw-r--r--   0        0        0    11422 2023-06-14 01:47:41.958730 conplex_dti-0.1.6/conplex_dti/featurizer/molecule.py
--rw-r--r--   0        0        0    11493 2023-06-14 01:47:41.996784 conplex_dti-0.1.6/conplex_dti/featurizer/protein.py
--rw-r--r--   0        0        0        0 2023-06-14 01:47:41.997856 conplex_dti-0.1.6/conplex_dti/model/__init__.py
--rw-r--r--   0        0        0    23789 2023-06-14 01:47:42.015759 conplex_dti-0.1.6/conplex_dti/model/architectures.py
--rw-r--r--   0        0        0     2125 2023-06-14 01:47:42.044312 conplex_dti-0.1.6/conplex_dti/model/margin.py
--rw-r--r--   0        0        0     4022 2023-06-14 01:47:42.059531 conplex_dti-0.1.6/conplex_dti/utils.py
--rw-r--r--   0        0        0     4195 2023-08-02 16:12:52.365251 conplex_dti-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     6444 1970-01-01 00:00:00.000000 conplex_dti-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-03-11 16:53:19.162872 conplex_dti-0.1.7/LICENSE
+-rwxr-xr-x   0        0        0     4803 2023-08-02 16:23:54.758153 conplex_dti-0.1.7/README.md
+-rw-r--r--   0        0        0     3510 2023-06-14 01:47:41.847038 conplex_dti-0.1.7/conplex_dti/MAIN_OLD.txt
+-rw-r--r--   0        0        0      399 2023-06-14 01:47:41.848725 conplex_dti-0.1.7/conplex_dti/__init__.py
+-rw-r--r--   0        0        0     1094 2023-07-09 05:21:18.079836 conplex_dti-0.1.7/conplex_dti/__main__.py
+-rw-r--r--   0        0        0    23714 2023-06-14 01:47:41.852511 conplex_dti-0.1.7/conplex_dti/architectures.py
+-rw-r--r--   0        0        0      251 2023-07-09 05:21:18.081792 conplex_dti-0.1.7/conplex_dti/cli/__init__.py
+-rw-r--r--   0        0        0     3859 2023-07-09 05:21:15.929266 conplex_dti-0.1.7/conplex_dti/cli/download.py
+-rw-r--r--   0        0        0     4264 2023-08-02 16:35:57.183801 conplex_dti-0.1.7/conplex_dti/cli/predict.py
+-rw-r--r--   0        0        0    19588 2023-07-09 05:21:15.932012 conplex_dti-0.1.7/conplex_dti/cli/train.py
+-rw-r--r--   0        0        0      171 2023-07-09 05:21:15.934053 conplex_dti-0.1.7/conplex_dti/dataset/__init__.py
+-rw-r--r--   0        0        0    24300 2023-07-09 05:21:15.936761 conplex_dti-0.1.7/conplex_dti/dataset/datamodules.py
+-rw-r--r--   0        0        0      421 2023-06-14 01:47:41.919180 conplex_dti-0.1.7/conplex_dti/featurizer/__init__.py
+-rw-r--r--   0        0        0     7765 2023-06-14 20:00:03.681608 conplex_dti-0.1.7/conplex_dti/featurizer/base.py
+-rw-r--r--   0        0        0    11422 2023-06-14 01:47:41.958730 conplex_dti-0.1.7/conplex_dti/featurizer/molecule.py
+-rw-r--r--   0        0        0    11493 2023-06-14 01:47:41.996784 conplex_dti-0.1.7/conplex_dti/featurizer/protein.py
+-rw-r--r--   0        0        0        0 2023-06-14 01:47:41.997856 conplex_dti-0.1.7/conplex_dti/model/__init__.py
+-rw-r--r--   0        0        0    23789 2023-06-14 01:47:42.015759 conplex_dti-0.1.7/conplex_dti/model/architectures.py
+-rw-r--r--   0        0        0     2125 2023-06-14 01:47:42.044312 conplex_dti-0.1.7/conplex_dti/model/margin.py
+-rw-r--r--   0        0        0     4022 2023-06-14 01:47:42.059531 conplex_dti-0.1.7/conplex_dti/utils.py
+-rw-r--r--   0        0        0     4195 2023-08-02 16:36:09.973306 conplex_dti-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     6444 1970-01-01 00:00:00.000000 conplex_dti-0.1.7/PKG-INFO
```

### Comparing `conplex_dti-0.1.6/LICENSE` & `conplex_dti-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.6/README.md` & `conplex_dti-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.6/conplex_dti/MAIN_OLD.txt` & `conplex_dti-0.1.7/conplex_dti/MAIN_OLD.txt`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.6/conplex_dti/__main__.py` & `conplex_dti-0.1.7/conplex_dti/__main__.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.6/conplex_dti/architectures.py` & `conplex_dti-0.1.7/conplex_dti/architectures.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.6/conplex_dti/cli/download.py` & `conplex_dti-0.1.7/conplex_dti/cli/download.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.6/conplex_dti/cli/predict.py` & `conplex_dti-0.1.7/conplex_dti/cli/predict.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,16 +90,16 @@
         device = torch.device(f"cuda:{device_no}" if use_cuda else "cpu")
     logg.info(f"Using CUDA device {device}")
 
     # Loading model
     logg.info(f"Loading model from {args.model_path}")
     target_featurizer = ProtBertFeaturizer(
         save_dir=args.data_cache_dir, per_tok=False
-    ).cuda(device)
-    drug_featurizer = MorganFeaturizer(save_dir=args.data_cache_dir).cuda(device)
+    ).to(device)
+    drug_featurizer = MorganFeaturizer(save_dir=args.data_cache_dir).to(device)
 
     drug_featurizer.preload(query_df["moleculeSmiles"].unique())
     target_featurizer.preload(query_df["proteinSequence"].unique())
 
     model = SimpleCoembeddingNoSigmoid(
         drug_featurizer.shape, target_featurizer.shape, 1024
     )
```

### Comparing `conplex_dti-0.1.6/conplex_dti/cli/train.py` & `conplex_dti-0.1.7/conplex_dti/cli/train.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.6/conplex_dti/dataset/datamodules.py` & `conplex_dti-0.1.7/conplex_dti/dataset/datamodules.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.6/conplex_dti/featurizer/base.py` & `conplex_dti-0.1.7/conplex_dti/featurizer/base.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.6/conplex_dti/featurizer/molecule.py` & `conplex_dti-0.1.7/conplex_dti/featurizer/molecule.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.6/conplex_dti/featurizer/protein.py` & `conplex_dti-0.1.7/conplex_dti/featurizer/protein.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.6/conplex_dti/model/architectures.py` & `conplex_dti-0.1.7/conplex_dti/model/architectures.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.6/conplex_dti/model/margin.py` & `conplex_dti-0.1.7/conplex_dti/model/margin.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.6/conplex_dti/utils.py` & `conplex_dti-0.1.7/conplex_dti/utils.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.6/pyproject.toml` & `conplex_dti-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "conplex-dti"
-version = "0.1.6"
+version = "0.1.7"
 description = "Adapting protein language models and contrastive learning for DTI prediction."
 readme = "README.md"
 authors = ["samsledje <samsl@mit.edu>"]
 license = "MIT"
 repository = "https://github.com/samsledje/ConPLex"
 homepage = "https://github.com/samsledje/ConPLex"
```

### Comparing `conplex_dti-0.1.6/PKG-INFO` & `conplex_dti-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conplex-dti
-Version: 0.1.6
+Version: 0.1.7
 Summary: Adapting protein language models and contrastive learning for DTI prediction.
 Home-page: https://github.com/samsledje/ConPLex
 License: MIT
 Keywords: protein language models,contrastive learning,drug target interaction,DTI
 Author: samsledje
 Author-email: samsl@mit.edu
 Requires-Python: >=3.9,<4.0
```


# Comparing `tmp/protloc_mex_x-0.0.5.tar.gz` & `tmp/protloc_mex_x-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protloc_mex_x-0.0.5.tar", max compression
+gzip compressed data, was "protloc_mex_x-0.0.6.tar", max compression
```

## Comparing `protloc_mex_x-0.0.5.tar` & `protloc_mex_x-0.0.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1091 2023-04-25 08:38:35.586641 protloc_mex_x-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0        2 2023-05-09 03:41:02.000000 protloc_mex_x-0.0.5/protloc_mex_X/__init__.py
--rw-r--r--   0        0        0    39068 2023-06-01 11:45:18.000000 protloc_mex_x-0.0.5/protloc_mex_X/ESM2_fr.py
--rw-r--r--   0        0        0     2999 2023-05-08 12:33:04.000000 protloc_mex_x-0.0.5/protloc_mex_X/examples/test1.txt
--rw-r--r--   0        0        0     2749 2023-05-09 03:13:02.000000 protloc_mex_x-0.0.5/protloc_mex_X/feature_corrlation.py
--rw-r--r--   0        0        0      863 2023-08-02 04:10:05.751249 protloc_mex_x-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     6573 2023-08-02 04:09:16.308133 protloc_mex_x-0.0.5/README.md
--rw-r--r--   0        0        0     7452 1970-01-01 00:00:00.000000 protloc_mex_x-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-04-25 08:38:35.586641 protloc_mex_x-0.0.6/LICENSE.txt
+-rw-r--r--   0        0        0        2 2023-05-09 03:41:02.000000 protloc_mex_x-0.0.6/protloc_mex_X/__init__.py
+-rw-r--r--   0        0        0    39068 2023-06-01 11:45:18.000000 protloc_mex_x-0.0.6/protloc_mex_X/ESM2_fr.py
+-rw-r--r--   0        0        0     2999 2023-05-08 12:33:04.000000 protloc_mex_x-0.0.6/protloc_mex_X/examples/test1.txt
+-rw-r--r--   0        0        0     2749 2023-05-09 03:13:02.000000 protloc_mex_x-0.0.6/protloc_mex_X/feature_corrlation.py
+-rw-r--r--   0        0        0      863 2023-08-02 04:19:26.691600 protloc_mex_x-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     6520 2023-08-02 04:19:08.821782 protloc_mex_x-0.0.6/README.md
+-rw-r--r--   0        0        0     7399 1970-01-01 00:00:00.000000 protloc_mex_x-0.0.6/PKG-INFO
```

### Comparing `protloc_mex_x-0.0.5/LICENSE.txt` & `protloc_mex_x-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `protloc_mex_x-0.0.5/protloc_mex_X/ESM2_fr.py` & `protloc_mex_x-0.0.6/protloc_mex_X/ESM2_fr.py`

 * *Files identical despite different names*

### Comparing `protloc_mex_x-0.0.5/protloc_mex_X/examples/test1.txt` & `protloc_mex_x-0.0.6/protloc_mex_X/examples/test1.txt`

 * *Files identical despite different names*

### Comparing `protloc_mex_x-0.0.5/protloc_mex_X/feature_corrlation.py` & `protloc_mex_x-0.0.6/protloc_mex_X/feature_corrlation.py`

 * *Files identical despite different names*

### Comparing `protloc_mex_x-0.0.5/pyproject.toml` & `protloc_mex_x-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "protloc_mex_X"
-version = "0.0.5"
+version = "0.0.6"
 description = "Internal use kit"
 authors = ["Ze Yu Luo <1024226968@qq.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/yujuan-zhang/ProtLoc-mexl"
 repository = "https://github.com/yujuan-zhang/ProtLoc-mexl"
 documentation = "https://github.com/yujuan-zhang/ProtLoc-mexl/issues"
```

### Comparing `protloc_mex_x-0.0.5/README.md` & `protloc_mex_x-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 ProtLoc-mex_X includes 2 modules: ESM2_fr and feature_corrlation.
 
 ### ESM2_fr
 
 ESM2_fr is a pre-trained deep learning model based on the ESM2 model. It is capable of extracting representation features from protein sequences and further optimizing the feature representation through weighted averaging.
 
-It contains one class and three functions. The class is named `Esm2LastHiddenFeatureExtractor`, which includes the following three methods: `get_last_hidden_features_combine()`, `get_last_hidden_phosphorylation_position_feature()`, and `get_amino_acid_representation()`. The functions present in the code are `get_last_hidden_features_single()`, `NetPhos_classic_txt_DataFrame()`, `phospho_feature_sim_cosine_weighted_average()`, and `phospho_feature_sim_cosine_weighted_average_test()`.
+It contains one class and three functions. The class is named `Esm2LastHiddenFeatureExtractor`, which includes the following three methods: `get_last_hidden_features_combine()`, `get_last_hidden_phosphorylation_position_feature()`, and `get_amino_acid_representation()`. The functions present in the code are `get_last_hidden_features_single()`, `NetPhos_classic_txt_DataFrame()`, and `phospho_feature_sim_cosine_weighted_average()`.
 
 #### Function  `get_last_hidden_features_single()`：
 
 The `get_last_hidden_features_single()` function is utilized for extracting different types of representation features from the input protein sequences. It accepts protein sequence data `X_input`, along with the model tokenizer and model as inputs, and subsequently returns a DataFrame containing the extracted features.(note: Only single-batch inputs are supported.)
 
 #### Class `Esm2LastHiddenFeatureExtractor()`：
 
@@ -106,8 +106,8 @@
 
 feature_extractor = Esm2LastHiddenFeatureExtractor(tokenizer, model,
                                                    compute_cls=True, compute_eos=True, compute_mean=True, compute_segments=True)
 
 human_df_represent = feature_extractor.get_last_hidden_features_combine(protein_sequence_df, sequence_name='Sequence', batch_size= 1)
 ```
 
-##### Due to the ongoing review process of the articles related to the toolkit, not all information can be fully disclosed at the moment. If you require additional details or have specific inquiries about the toolkit, kindly contact the author, Zeyu Luo <1024226968@qq.com> , for further information. The author will be able to provide more comprehensive and accurate details about the toolkit's functionalities and features. Thank you for your understanding.
+###### Due to the ongoing review process of the articles related to the toolkit, not all information can be fully disclosed at the moment. If you require additional details or have specific inquiries about the toolkit, kindly contact the author, Zeyu Luo <1024226968@qq.com> , for further information. The author will be able to provide more comprehensive and accurate details about the toolkit's functionalities and features. Thank you for your understanding.
```

### Comparing `protloc_mex_x-0.0.5/PKG-INFO` & `protloc_mex_x-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protloc-mex-x
-Version: 0.0.5
+Version: 0.0.6
 Summary: Internal use kit
 Home-page: https://github.com/yujuan-zhang/ProtLoc-mexl
 License: MIT
 Author: Ze Yu Luo
 Author-email: 1024226968@qq.com
 Requires-Python: >=3.9
 Classifier: Development Status :: 3 - Alpha
@@ -84,15 +84,15 @@
 
 ProtLoc-mex_X includes 2 modules: ESM2_fr and feature_corrlation.
 
 ### ESM2_fr
 
 ESM2_fr is a pre-trained deep learning model based on the ESM2 model. It is capable of extracting representation features from protein sequences and further optimizing the feature representation through weighted averaging.
 
-It contains one class and three functions. The class is named `Esm2LastHiddenFeatureExtractor`, which includes the following three methods: `get_last_hidden_features_combine()`, `get_last_hidden_phosphorylation_position_feature()`, and `get_amino_acid_representation()`. The functions present in the code are `get_last_hidden_features_single()`, `NetPhos_classic_txt_DataFrame()`, `phospho_feature_sim_cosine_weighted_average()`, and `phospho_feature_sim_cosine_weighted_average_test()`.
+It contains one class and three functions. The class is named `Esm2LastHiddenFeatureExtractor`, which includes the following three methods: `get_last_hidden_features_combine()`, `get_last_hidden_phosphorylation_position_feature()`, and `get_amino_acid_representation()`. The functions present in the code are `get_last_hidden_features_single()`, `NetPhos_classic_txt_DataFrame()`, and `phospho_feature_sim_cosine_weighted_average()`.
 
 #### Function  `get_last_hidden_features_single()`：
 
 The `get_last_hidden_features_single()` function is utilized for extracting different types of representation features from the input protein sequences. It accepts protein sequence data `X_input`, along with the model tokenizer and model as inputs, and subsequently returns a DataFrame containing the extracted features.(note: Only single-batch inputs are supported.)
 
 #### Class `Esm2LastHiddenFeatureExtractor()`：
 
@@ -132,8 +132,8 @@
 
 feature_extractor = Esm2LastHiddenFeatureExtractor(tokenizer, model,
                                                    compute_cls=True, compute_eos=True, compute_mean=True, compute_segments=True)
 
 human_df_represent = feature_extractor.get_last_hidden_features_combine(protein_sequence_df, sequence_name='Sequence', batch_size= 1)
 ```
 
-##### Due to the ongoing review process of the articles related to the toolkit, not all information can be fully disclosed at the moment. If you require additional details or have specific inquiries about the toolkit, kindly contact the author, Zeyu Luo <1024226968@qq.com> , for further information. The author will be able to provide more comprehensive and accurate details about the toolkit's functionalities and features. Thank you for your understanding.
+###### Due to the ongoing review process of the articles related to the toolkit, not all information can be fully disclosed at the moment. If you require additional details or have specific inquiries about the toolkit, kindly contact the author, Zeyu Luo <1024226968@qq.com> , for further information. The author will be able to provide more comprehensive and accurate details about the toolkit's functionalities and features. Thank you for your understanding.
```


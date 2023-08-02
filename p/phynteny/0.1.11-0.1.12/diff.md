# Comparing `tmp/Phynteny-0.1.11.tar.gz` & `tmp/phynteny-0.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Phynteny-0.1.11.tar", last modified: Wed Aug  2 00:15:16 2023, max compression
+gzip compressed data, was "phynteny-0.1.12.tar", last modified: Wed Aug  2 05:49:52 2023, max compression
```

## Comparing `Phynteny-0.1.11.tar` & `phynteny-0.1.12.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:15:16.348536 Phynteny-0.1.11/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 00:15:06.000000 Phynteny-0.1.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-02 00:15:06.000000 Phynteny-0.1.11/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-08-02 00:15:16.348536 Phynteny-0.1.11/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:15:16.340535 Phynteny-0.1.11/Phynteny.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-08-02 00:15:16.000000 Phynteny-0.1.11/Phynteny.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-02 00:15:16.000000 Phynteny-0.1.11/Phynteny.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 00:15:16.000000 Phynteny-0.1.11/Phynteny.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-02 00:15:16.000000 Phynteny-0.1.11/Phynteny.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-02 00:15:16.000000 Phynteny-0.1.11/Phynteny.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-02 00:15:16.000000 Phynteny-0.1.11/Phynteny.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 00:15:16.000000 Phynteny-0.1.11/Phynteny.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-08-02 00:15:06.000000 Phynteny-0.1.11/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-02 00:15:06.000000 Phynteny-0.1.11/VERSION
--rwxr-xr-x   0 runner    (1001) docker     (123)     3687 2023-08-02 00:15:06.000000 Phynteny-0.1.11/phynteny
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:15:16.340535 Phynteny-0.1.11/phynteny_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 00:15:06.000000 Phynteny-0.1.11/phynteny_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-02 00:15:06.000000 Phynteny-0.1.11/phynteny_utils/current_models.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10296 2023-08-02 00:15:06.000000 Phynteny-0.1.11/phynteny_utils/format_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9967 2023-08-02 00:15:06.000000 Phynteny-0.1.11/phynteny_utils/handle_genbank.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-08-02 00:15:06.000000 Phynteny-0.1.11/phynteny_utils/install_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-08-02 00:15:06.000000 Phynteny-0.1.11/phynteny_utils/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:15:16.348536 Phynteny-0.1.11/phynteny_utils/phrog_annotation_info/
--rw-r--r--   0 runner    (1001) docker     (123)  1742344 2023-08-02 00:15:06.000000 Phynteny-0.1.11/phynteny_utils/phrog_annotation_info/confidence_kde.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-08-02 00:15:06.000000 Phynteny-0.1.11/phynteny_utils/phrog_annotation_info/integer_category.pkl
--rw-r--r--   0 runner    (1001) docker     (123)  3831481 2023-08-02 00:15:06.000000 Phynteny-0.1.11/phynteny_utils/phrog_annotation_info/phrog_annot_v4.tsv
--rw-r--r--   0 runner    (1001) docker     (123)   634822 2023-08-02 00:15:06.000000 Phynteny-0.1.11/phynteny_utils/phrog_annotation_info/phrog_integer.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-08-02 00:15:06.000000 Phynteny-0.1.11/phynteny_utils/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13872 2023-08-02 00:15:06.000000 Phynteny-0.1.11/phynteny_utils/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    17672 2023-08-02 00:15:06.000000 Phynteny-0.1.11/phynteny_utils/train_model.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 00:15:16.348536 Phynteny-0.1.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-08-02 00:15:06.000000 Phynteny-0.1.11/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:15:16.348536 Phynteny-0.1.11/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)   329114 2023-08-02 00:15:06.000000 Phynteny-0.1.11/test_data/test_phage.gbk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:15:16.348536 Phynteny-0.1.11/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-08-02 00:15:06.000000 Phynteny-0.1.11/tests/test_phynteny.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:15:16.348536 Phynteny-0.1.11/train_phynteny/
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-08-02 00:15:06.000000 Phynteny-0.1.11/train_phynteny/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-08-02 00:15:06.000000 Phynteny-0.1.11/train_phynteny/compute_confidence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-08-02 00:15:06.000000 Phynteny-0.1.11/train_phynteny/generate_training_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-08-02 00:15:06.000000 Phynteny-0.1.11/train_phynteny/train_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:49:52.689887 phynteny-0.1.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 05:49:41.000000 phynteny-0.1.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-02 05:49:41.000000 phynteny-0.1.12/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-08-02 05:49:52.689887 phynteny-0.1.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-08-02 05:49:41.000000 phynteny-0.1.12/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-02 05:49:41.000000 phynteny-0.1.12/VERSION
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3687 2023-08-02 05:49:41.000000 phynteny-0.1.12/phynteny
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:49:52.677887 phynteny-0.1.12/phynteny.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-08-02 05:49:52.000000 phynteny-0.1.12/phynteny.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-02 05:49:52.000000 phynteny-0.1.12/phynteny.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 05:49:52.000000 phynteny-0.1.12/phynteny.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-02 05:49:52.000000 phynteny-0.1.12/phynteny.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-02 05:49:52.000000 phynteny-0.1.12/phynteny.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-02 05:49:52.000000 phynteny-0.1.12/phynteny.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 05:49:52.000000 phynteny-0.1.12/phynteny.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:49:52.681887 phynteny-0.1.12/phynteny_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 05:49:41.000000 phynteny-0.1.12/phynteny_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-02 05:49:41.000000 phynteny-0.1.12/phynteny_utils/current_models.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10296 2023-08-02 05:49:41.000000 phynteny-0.1.12/phynteny_utils/format_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9967 2023-08-02 05:49:41.000000 phynteny-0.1.12/phynteny_utils/handle_genbank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-08-02 05:49:41.000000 phynteny-0.1.12/phynteny_utils/install_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-08-02 05:49:41.000000 phynteny-0.1.12/phynteny_utils/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:49:52.685887 phynteny-0.1.12/phynteny_utils/phrog_annotation_info/
+-rw-r--r--   0 runner    (1001) docker     (123)  1742344 2023-08-02 05:49:41.000000 phynteny-0.1.12/phynteny_utils/phrog_annotation_info/confidence_kde.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-08-02 05:49:41.000000 phynteny-0.1.12/phynteny_utils/phrog_annotation_info/integer_category.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)  3831481 2023-08-02 05:49:41.000000 phynteny-0.1.12/phynteny_utils/phrog_annotation_info/phrog_annot_v4.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   634822 2023-08-02 05:49:41.000000 phynteny-0.1.12/phynteny_utils/phrog_annotation_info/phrog_integer.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-08-02 05:49:41.000000 phynteny-0.1.12/phynteny_utils/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13872 2023-08-02 05:49:41.000000 phynteny-0.1.12/phynteny_utils/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17672 2023-08-02 05:49:41.000000 phynteny-0.1.12/phynteny_utils/train_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 05:49:52.689887 phynteny-0.1.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-08-02 05:49:41.000000 phynteny-0.1.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:49:52.685887 phynteny-0.1.12/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   329114 2023-08-02 05:49:41.000000 phynteny-0.1.12/test_data/test_phage.gbk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:49:52.689887 phynteny-0.1.12/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-08-02 05:49:41.000000 phynteny-0.1.12/tests/test_phynteny.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:49:52.689887 phynteny-0.1.12/train_phynteny/
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-08-02 05:49:41.000000 phynteny-0.1.12/train_phynteny/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-08-02 05:49:41.000000 phynteny-0.1.12/train_phynteny/compute_confidence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-08-02 05:49:41.000000 phynteny-0.1.12/train_phynteny/generate_training_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-08-02 05:49:41.000000 phynteny-0.1.12/train_phynteny/train_model.py
```

### Comparing `Phynteny-0.1.11/LICENSE` & `phynteny-0.1.12/LICENSE`

 * *Files identical despite different names*

### Comparing `Phynteny-0.1.11/PKG-INFO` & `phynteny-0.1.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Phynteny
-Version: 0.1.11
+Name: phynteny
+Version: 0.1.12
 Summary: Phynteny: Synteny-based prediction of bacteriophage genes
 Home-page: https://github.com/susiegriggo/Phynteny
 Author: Susanna Grigson
 Author-email: susie.grigson@gmail.com
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Phynteny-0.1.11/Phynteny.egg-info/PKG-INFO` & `phynteny-0.1.12/phynteny.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Phynteny
-Version: 0.1.11
+Name: phynteny
+Version: 0.1.12
 Summary: Phynteny: Synteny-based prediction of bacteriophage genes
 Home-page: https://github.com/susiegriggo/Phynteny
 Author: Susanna Grigson
 Author-email: susie.grigson@gmail.com
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Phynteny-0.1.11/Phynteny.egg-info/SOURCES.txt` & `phynteny-0.1.12/phynteny.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 LICENSE
 MANIFEST.in
 README.md
 VERSION
 phynteny
 setup.py
-Phynteny.egg-info/PKG-INFO
-Phynteny.egg-info/SOURCES.txt
-Phynteny.egg-info/dependency_links.txt
-Phynteny.egg-info/entry_points.txt
-Phynteny.egg-info/requires.txt
-Phynteny.egg-info/top_level.txt
-Phynteny.egg-info/zip-safe
+phynteny.egg-info/PKG-INFO
+phynteny.egg-info/SOURCES.txt
+phynteny.egg-info/dependency_links.txt
+phynteny.egg-info/entry_points.txt
+phynteny.egg-info/requires.txt
+phynteny.egg-info/top_level.txt
+phynteny.egg-info/zip-safe
 phynteny_utils/__init__.py
 phynteny_utils/current_models.txt
 phynteny_utils/format_data.py
 phynteny_utils/handle_genbank.py
 phynteny_utils/install_models.py
 phynteny_utils/models.py
 phynteny_utils/predictor.py
```

### Comparing `Phynteny-0.1.11/README.md` & `phynteny-0.1.12/README.md`

 * *Files identical despite different names*

### Comparing `Phynteny-0.1.11/phynteny` & `phynteny-0.1.12/phynteny`

 * *Files identical despite different names*

### Comparing `Phynteny-0.1.11/phynteny_utils/format_data.py` & `phynteny-0.1.12/phynteny_utils/format_data.py`

 * *Files identical despite different names*

### Comparing `Phynteny-0.1.11/phynteny_utils/handle_genbank.py` & `phynteny-0.1.12/phynteny_utils/handle_genbank.py`

 * *Files identical despite different names*

### Comparing `Phynteny-0.1.11/phynteny_utils/install_models.py` & `phynteny-0.1.12/phynteny_utils/install_models.py`

 * *Files identical despite different names*

### Comparing `Phynteny-0.1.11/phynteny_utils/models.py` & `phynteny-0.1.12/phynteny_utils/models.py`

 * *Files identical despite different names*

### Comparing `Phynteny-0.1.11/phynteny_utils/phrog_annotation_info/confidence_kde.pkl` & `phynteny-0.1.12/phynteny_utils/phrog_annotation_info/confidence_kde.pkl`

 * *Files identical despite different names*

### Comparing `Phynteny-0.1.11/phynteny_utils/phrog_annotation_info/phrog_annot_v4.tsv` & `phynteny-0.1.12/phynteny_utils/phrog_annotation_info/phrog_annot_v4.tsv`

 * *Files identical despite different names*

### Comparing `Phynteny-0.1.11/phynteny_utils/phrog_annotation_info/phrog_integer.pkl` & `phynteny-0.1.12/phynteny_utils/phrog_annotation_info/phrog_integer.pkl`

 * *Files identical despite different names*

### Comparing `Phynteny-0.1.11/phynteny_utils/predictor.py` & `phynteny-0.1.12/phynteny_utils/predictor.py`

 * *Files identical despite different names*

### Comparing `Phynteny-0.1.11/phynteny_utils/statistics.py` & `phynteny-0.1.12/phynteny_utils/statistics.py`

 * *Files identical despite different names*

### Comparing `Phynteny-0.1.11/phynteny_utils/train_model.py` & `phynteny-0.1.12/phynteny_utils/train_model.py`

 * *Files identical despite different names*

### Comparing `Phynteny-0.1.11/setup.py` & `phynteny-0.1.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 	"train_phynteny": ["train_phynteny/*"]
 }
 
 model_files = glob.glob("phynteny_utils/models/*")
 data_files = [(".", ["LICENSE", "README.md"])]
 
 setuptools.setup(
-    name="Phynteny",
+    name="phynteny",
     version=get_version(),
     zip_safe=True,
     author="Susanna Grigson",
     author_email="susie.grigson@gmail.com",
     description="Phynteny: Synteny-based prediction of bacteriophage genes",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `Phynteny-0.1.11/test_data/test_phage.gbk` & `phynteny-0.1.12/test_data/test_phage.gbk`

 * *Files identical despite different names*

### Comparing `Phynteny-0.1.11/tests/test_phynteny.py` & `phynteny-0.1.12/tests/test_phynteny.py`

 * *Files identical despite different names*

### Comparing `Phynteny-0.1.11/train_phynteny/README.md` & `phynteny-0.1.12/train_phynteny/README.md`

 * *Files identical despite different names*

### Comparing `Phynteny-0.1.11/train_phynteny/compute_confidence.py` & `phynteny-0.1.12/train_phynteny/compute_confidence.py`

 * *Files identical despite different names*

### Comparing `Phynteny-0.1.11/train_phynteny/generate_training_data.py` & `phynteny-0.1.12/train_phynteny/generate_training_data.py`

 * *Files identical despite different names*

### Comparing `Phynteny-0.1.11/train_phynteny/train_model.py` & `phynteny-0.1.12/train_phynteny/train_model.py`

 * *Files identical despite different names*


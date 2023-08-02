# Comparing `tmp/rxn-chem-utils-1.2.0.tar.gz` & `tmp/rxn-chem-utils-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rxn-chem-utils-1.2.0.tar", last modified: Mon Jul 31 13:04:45 2023, max compression
+gzip compressed data, was "rxn-chem-utils-1.3.0.tar", last modified: Wed Aug  2 08:38:55 2023, max compression
```

## Comparing `rxn-chem-utils-1.2.0.tar` & `rxn-chem-utils-1.3.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:04:45.351865 rxn-chem-utils-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-31 13:04:45.351865 rxn-chem-utils-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-31 13:04:45.355865 rxn-chem-utils-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:04:45.339865 rxn-chem-utils-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:04:45.339865 rxn-chem-utils-1.2.0/src/rxn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:04:45.347865 rxn-chem-utils-1.2.0/src/rxn/chemutils/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/extended_reaction_smiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/miscellaneous.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/multicomponent_smiles.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/reaction_combiner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/reaction_equation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/reaction_smiles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:04:45.347865 rxn-chem-utils-1.2.0/src/rxn/chemutils/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/scripts/canonicalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/scripts/combine_reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/scripts/detokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/scripts/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/smiles_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/smiles_randomization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/tokenization.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/src/rxn/chemutils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:04:45.347865 rxn-chem-utils-1.2.0/src/rxn_chem_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-31 13:04:45.000000 rxn-chem-utils-1.2.0/src/rxn_chem_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-31 13:04:45.000000 rxn-chem-utils-1.2.0/src/rxn_chem_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 13:04:45.000000 rxn-chem-utils-1.2.0/src/rxn_chem_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-31 13:04:45.000000 rxn-chem-utils-1.2.0/src/rxn_chem_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 13:04:45.000000 rxn-chem-utils-1.2.0/src/rxn_chem_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-31 13:04:45.000000 rxn-chem-utils-1.2.0/src/rxn_chem_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-31 13:04:45.000000 rxn-chem-utils-1.2.0/src/rxn_chem_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:04:45.351865 rxn-chem-utils-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/tests/test_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/tests/test_extended_reaction_smiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/tests/test_miscellaneous.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/tests/test_multicomponent_smiles.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/tests/test_rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/tests/test_reaction_combiner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/tests/test_reaction_equation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/tests/test_reaction_smiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/tests/test_smiles_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/tests/test_smiles_randomization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/tests/test_tokenization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-31 13:04:33.000000 rxn-chem-utils-1.2.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:38:55.787567 rxn-chem-utils-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-08-02 08:38:55.787567 rxn-chem-utils-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-08-02 08:38:55.787567 rxn-chem-utils-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:38:55.779566 rxn-chem-utils-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:38:55.779566 rxn-chem-utils-1.3.0/src/rxn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:38:55.783567 rxn-chem-utils-1.3.0/src/rxn/chemutils/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/src/rxn/chemutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/src/rxn/chemutils/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/src/rxn/chemutils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/src/rxn/chemutils/extended_reaction_smiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/src/rxn/chemutils/miscellaneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/src/rxn/chemutils/multicomponent_smiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/src/rxn/chemutils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/src/rxn/chemutils/rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/src/rxn/chemutils/reaction_combiner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/src/rxn/chemutils/reaction_equation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/src/rxn/chemutils/reaction_smiles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:38:55.783567 rxn-chem-utils-1.3.0/src/rxn/chemutils/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/src/rxn/chemutils/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/src/rxn/chemutils/scripts/canonicalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/src/rxn/chemutils/scripts/combine_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/src/rxn/chemutils/scripts/detokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/src/rxn/chemutils/scripts/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/src/rxn/chemutils/smiles_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/src/rxn/chemutils/smiles_randomization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/src/rxn/chemutils/tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/src/rxn/chemutils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:38:55.787567 rxn-chem-utils-1.3.0/src/rxn_chem_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-08-02 08:38:55.000000 rxn-chem-utils-1.3.0/src/rxn_chem_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-08-02 08:38:55.000000 rxn-chem-utils-1.3.0/src/rxn_chem_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 08:38:55.000000 rxn-chem-utils-1.3.0/src/rxn_chem_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-02 08:38:55.000000 rxn-chem-utils-1.3.0/src/rxn_chem_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 08:38:55.000000 rxn-chem-utils-1.3.0/src/rxn_chem_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-02 08:38:55.000000 rxn-chem-utils-1.3.0/src/rxn_chem_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-02 08:38:55.000000 rxn-chem-utils-1.3.0/src/rxn_chem_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:38:55.787567 rxn-chem-utils-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/tests/test_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/tests/test_extended_reaction_smiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/tests/test_miscellaneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/tests/test_multicomponent_smiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/tests/test_rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/tests/test_reaction_combiner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/tests/test_reaction_equation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/tests/test_reaction_smiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/tests/test_smiles_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/tests/test_smiles_randomization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/tests/test_tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-02 08:38:41.000000 rxn-chem-utils-1.3.0/tests/test_utils.py
```

### Comparing `rxn-chem-utils-1.2.0/LICENSE` & `rxn-chem-utils-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.2.0/PKG-INFO` & `rxn-chem-utils-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rxn-chem-utils
-Version: 1.2.0
+Version: 1.3.0
 Summary: Chemistry-related utilities
 Author: IBM RXN team
 Author-email: rxn4chemistry@zurich.ibm.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `rxn-chem-utils-1.2.0/README.md` & `rxn-chem-utils-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.2.0/setup.cfg` & `rxn-chem-utils-1.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.2.0/src/rxn/chemutils/conversion.py` & `rxn-chem-utils-1.3.0/src/rxn/chemutils/conversion.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.2.0/src/rxn/chemutils/exceptions.py` & `rxn-chem-utils-1.3.0/src/rxn/chemutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.2.0/src/rxn/chemutils/extended_reaction_smiles.py` & `rxn-chem-utils-1.3.0/src/rxn/chemutils/extended_reaction_smiles.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.2.0/src/rxn/chemutils/miscellaneous.py` & `rxn-chem-utils-1.3.0/src/rxn/chemutils/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.2.0/src/rxn/chemutils/multicomponent_smiles.py` & `rxn-chem-utils-1.3.0/src/rxn/chemutils/multicomponent_smiles.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.2.0/src/rxn/chemutils/reaction_equation.py` & `rxn-chem-utils-1.3.0/src/rxn/chemutils/reaction_equation.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.2.0/src/rxn/chemutils/reaction_smiles.py` & `rxn-chem-utils-1.3.0/src/rxn/chemutils/reaction_smiles.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.2.0/src/rxn/chemutils/scripts/canonicalize.py` & `rxn-chem-utils-1.3.0/src/rxn/chemutils/scripts/canonicalize.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.2.0/src/rxn/chemutils/scripts/combine_reaction.py` & `rxn-chem-utils-1.3.0/src/rxn/chemutils/scripts/combine_reaction.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.2.0/src/rxn/chemutils/scripts/detokenize.py` & `rxn-chem-utils-1.3.0/src/rxn/chemutils/scripts/detokenize.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.2.0/src/rxn/chemutils/scripts/tokenize.py` & `rxn-chem-utils-1.3.0/src/rxn/chemutils/scripts/tokenize.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.2.0/src/rxn/chemutils/smiles_augmenter.py` & `rxn-chem-utils-1.3.0/src/rxn/chemutils/smiles_augmenter.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.2.0/src/rxn/chemutils/smiles_randomization.py` & `rxn-chem-utils-1.3.0/src/rxn/chemutils/smiles_randomization.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.2.0/src/rxn/chemutils/tokenization.py` & `rxn-chem-utils-1.3.0/src/rxn/chemutils/tokenization.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.2.0/src/rxn/chemutils/utils.py` & `rxn-chem-utils-1.3.0/src/rxn/chemutils/utils.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.2.0/src/rxn_chem_utils.egg-info/PKG-INFO` & `rxn-chem-utils-1.3.0/src/rxn_chem_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rxn-chem-utils
-Version: 1.2.0
+Version: 1.3.0
 Summary: Chemistry-related utilities
 Author: IBM RXN team
 Author-email: rxn4chemistry@zurich.ibm.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `rxn-chem-utils-1.2.0/src/rxn_chem_utils.egg-info/SOURCES.txt` & `rxn-chem-utils-1.3.0/src/rxn_chem_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.2.0/tests/test_conversion.py` & `rxn-chem-utils-1.3.0/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.2.0/tests/test_extended_reaction_smiles.py` & `rxn-chem-utils-1.3.0/tests/test_extended_reaction_smiles.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.2.0/tests/test_miscellaneous.py` & `rxn-chem-utils-1.3.0/tests/test_miscellaneous.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.2.0/tests/test_multicomponent_smiles.py` & `rxn-chem-utils-1.3.0/tests/test_multicomponent_smiles.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.2.0/tests/test_rdkit_utils.py` & `rxn-chem-utils-1.3.0/tests/test_rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.2.0/tests/test_reaction_equation.py` & `rxn-chem-utils-1.3.0/tests/test_reaction_equation.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.2.0/tests/test_reaction_smiles.py` & `rxn-chem-utils-1.3.0/tests/test_reaction_smiles.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.2.0/tests/test_smiles_augmenter.py` & `rxn-chem-utils-1.3.0/tests/test_smiles_augmenter.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.2.0/tests/test_smiles_randomization.py` & `rxn-chem-utils-1.3.0/tests/test_smiles_randomization.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.2.0/tests/test_tokenization.py` & `rxn-chem-utils-1.3.0/tests/test_tokenization.py`

 * *Files identical despite different names*

### Comparing `rxn-chem-utils-1.2.0/tests/test_utils.py` & `rxn-chem-utils-1.3.0/tests/test_utils.py`

 * *Files identical despite different names*


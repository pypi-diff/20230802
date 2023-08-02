# Comparing `tmp/proteinflow-2.1.1.tar.gz` & `tmp/proteinflow-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinflow-2.1.1.tar", last modified: Thu Jul 27 09:54:07 2023, max compression
+gzip compressed data, was "proteinflow-2.2.0.tar", last modified: Wed Aug  2 14:26:43 2023, max compression
```

## Comparing `proteinflow-2.1.1.tar` & `proteinflow-2.2.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:54:07.244248 proteinflow-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-27 09:53:54.000000 proteinflow-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-07-27 09:54:07.244248 proteinflow-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-07-27 09:53:54.000000 proteinflow-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:54:07.240248 proteinflow-2.1.1/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-27 09:53:54.000000 proteinflow-2.1.1/dev/bump_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-27 09:53:54.000000 proteinflow-2.1.1/dev/update_init_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:54:07.240248 proteinflow-2.1.1/proteinflow/
--rw-r--r--   0 runner    (1001) docker     (123)    27992 2023-07-27 09:53:54.000000 proteinflow-2.1.1/proteinflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-07-27 09:53:54.000000 proteinflow-2.1.1/proteinflow/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-07-27 09:53:54.000000 proteinflow-2.1.1/proteinflow/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:54:07.240248 proteinflow-2.1.1/proteinflow/data/
--rw-r--r--   0 runner    (1001) docker     (123)    71922 2023-07-27 09:53:54.000000 proteinflow-2.1.1/proteinflow/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37531 2023-07-27 09:53:54.000000 proteinflow-2.1.1/proteinflow/data/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    18133 2023-07-27 09:53:54.000000 proteinflow-2.1.1/proteinflow/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:54:07.240248 proteinflow-2.1.1/proteinflow/download/
--rw-r--r--   0 runner    (1001) docker     (123)    24607 2023-07-27 09:53:54.000000 proteinflow-2.1.1/proteinflow/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-07-27 09:53:54.000000 proteinflow-2.1.1/proteinflow/download/boto.py
--rw-r--r--   0 runner    (1001) docker     (123)    36587 2023-07-27 09:53:54.000000 proteinflow-2.1.1/proteinflow/ligand.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:54:07.244248 proteinflow-2.1.1/proteinflow/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-27 09:53:54.000000 proteinflow-2.1.1/proteinflow/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:54:07.244248 proteinflow-2.1.1/proteinflow/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-27 09:53:54.000000 proteinflow-2.1.1/proteinflow/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:54:07.244248 proteinflow-2.1.1/proteinflow/processing/
--rw-r--r--   0 runner    (1001) docker     (123)    18971 2023-07-27 09:53:54.000000 proteinflow-2.1.1/proteinflow/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:54:07.244248 proteinflow-2.1.1/proteinflow/split/
--rw-r--r--   0 runner    (1001) docker     (123)    50801 2023-07-27 09:53:54.000000 proteinflow-2.1.1/proteinflow/split/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-07-27 09:53:54.000000 proteinflow-2.1.1/proteinflow/split/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-07-27 09:53:54.000000 proteinflow-2.1.1/proteinflow/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:54:07.240248 proteinflow-2.1.1/proteinflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-07-27 09:54:07.000000 proteinflow-2.1.1/proteinflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-27 09:54:07.000000 proteinflow-2.1.1/proteinflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 09:54:07.000000 proteinflow-2.1.1/proteinflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 09:54:07.000000 proteinflow-2.1.1/proteinflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-27 09:54:07.000000 proteinflow-2.1.1/proteinflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-27 09:54:07.000000 proteinflow-2.1.1/proteinflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-27 09:53:54.000000 proteinflow-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-27 09:54:07.244248 proteinflow-2.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:54:07.244248 proteinflow-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-27 09:53:55.000000 proteinflow-2.1.1/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-27 09:53:55.000000 proteinflow-2.1.1/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-27 09:53:55.000000 proteinflow-2.1.1/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-27 09:53:55.000000 proteinflow-2.1.1/tests/test_sabdab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:26:43.440483 proteinflow-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-02 14:26:29.000000 proteinflow-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-08-02 14:26:43.440483 proteinflow-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-08-02 14:26:29.000000 proteinflow-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:26:43.436483 proteinflow-2.2.0/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-02 14:26:29.000000 proteinflow-2.2.0/dev/bump_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-02 14:26:29.000000 proteinflow-2.2.0/dev/update_init_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:26:43.440483 proteinflow-2.2.0/proteinflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    28157 2023-08-02 14:26:29.000000 proteinflow-2.2.0/proteinflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-08-02 14:26:29.000000 proteinflow-2.2.0/proteinflow/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-08-02 14:26:29.000000 proteinflow-2.2.0/proteinflow/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:26:43.440483 proteinflow-2.2.0/proteinflow/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    74235 2023-08-02 14:26:29.000000 proteinflow-2.2.0/proteinflow/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41886 2023-08-02 14:26:29.000000 proteinflow-2.2.0/proteinflow/data/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18133 2023-08-02 14:26:29.000000 proteinflow-2.2.0/proteinflow/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:26:43.440483 proteinflow-2.2.0/proteinflow/download/
+-rw-r--r--   0 runner    (1001) docker     (123)    24607 2023-08-02 14:26:29.000000 proteinflow-2.2.0/proteinflow/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-08-02 14:26:29.000000 proteinflow-2.2.0/proteinflow/download/boto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36587 2023-08-02 14:26:29.000000 proteinflow-2.2.0/proteinflow/ligand.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:26:43.440483 proteinflow-2.2.0/proteinflow/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-08-02 14:26:29.000000 proteinflow-2.2.0/proteinflow/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:26:43.440483 proteinflow-2.2.0/proteinflow/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-02 14:26:29.000000 proteinflow-2.2.0/proteinflow/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:26:43.440483 proteinflow-2.2.0/proteinflow/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)    19390 2023-08-02 14:26:29.000000 proteinflow-2.2.0/proteinflow/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:26:43.440483 proteinflow-2.2.0/proteinflow/split/
+-rw-r--r--   0 runner    (1001) docker     (123)    50801 2023-08-02 14:26:29.000000 proteinflow-2.2.0/proteinflow/split/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-08-02 14:26:29.000000 proteinflow-2.2.0/proteinflow/split/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-08-02 14:26:29.000000 proteinflow-2.2.0/proteinflow/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:26:43.440483 proteinflow-2.2.0/proteinflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-08-02 14:26:43.000000 proteinflow-2.2.0/proteinflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-08-02 14:26:43.000000 proteinflow-2.2.0/proteinflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:26:43.000000 proteinflow-2.2.0/proteinflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:26:43.000000 proteinflow-2.2.0/proteinflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-02 14:26:43.000000 proteinflow-2.2.0/proteinflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-02 14:26:43.000000 proteinflow-2.2.0/proteinflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-08-02 14:26:29.000000 proteinflow-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-02 14:26:43.444483 proteinflow-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:26:43.440483 proteinflow-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-08-02 14:26:30.000000 proteinflow-2.2.0/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-08-02 14:26:30.000000 proteinflow-2.2.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-08-02 14:26:30.000000 proteinflow-2.2.0/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-08-02 14:26:30.000000 proteinflow-2.2.0/tests/test_ligands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-08-02 14:26:30.000000 proteinflow-2.2.0/tests/test_sabdab.py
```

### Comparing `proteinflow-2.1.1/LICENSE` & `proteinflow-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.1/PKG-INFO` & `proteinflow-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteinflow
-Version: 2.1.1
+Version: 2.2.0
 Summary: Versatile pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
 License: BSD-3-Clause
 Keywords: bioinformatics,dataset,protein,PDB,deep learning
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proteinflow Version: 2.1.1 Summary: Versatile
+Metadata-Version: 2.1 Name: proteinflow Version: 2.2.0 Summary: Versatile
 pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova
 adaptyvbio.com>, Arthur Valentin
 adaptyvbio.com> License: BSD-3-Clause Keywords:
 bioinformatics,dataset,protein,PDB,deep learning Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
   ProteinFlow - A data processing pipeline for all your protein design needs
```

### Comparing `proteinflow-2.1.1/README.md` & `proteinflow-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.1/dev/bump_version.py` & `proteinflow-2.2.0/dev/bump_version.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.1/dev/update_init_docs.py` & `proteinflow-2.2.0/dev/update_init_docs.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.1/proteinflow/__init__.py` & `proteinflow-2.2.0/proteinflow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,14 +245,15 @@
     exclude_chains=None,
     exclude_threshold=0.7,
     exclude_clusters=False,
     exclude_based_on_cdr=None,
     load_ligands=False,
     exclude_chains_without_ligands=False,
     tanimoto_clustering=False,
+    require_ligand=False,
     random_seed=42,
     max_chains=10,
 ):
     """Download and parse PDB files that meet filtering criteria.
 
     The output files are pickled nested dictionaries where first-level keys are chain Ids and second-level keys are
     the following:
@@ -332,14 +333,16 @@
         if given and `exclude_clusters` is `True` + the dataset is SAbDab, exclude files based on only the given CDR clusters
     load_ligands : bool, default False
         if `True`, load ligands from the PDB files
     exclude_chains_without_ligands : bool, default False
         if `True`, exclude biounits that don't contain ligands
     tanimoto_clustering : bool, default False
         if `True`, cluster the biounits based on ligand Tanimoto similarity
+    require_ligand : bool, default False
+        if `True`, only use biounits that contain a ligand
     random_seed : int, default 42
         the random seed to use for splitting
     max_chains : int, default 10
         the maximum number of chains per biounit
 
     Returns
     -------
@@ -393,14 +396,15 @@
         load_live=load_live,
         sabdab=sabdab,
         sabdab_data_path=sabdab_data_path,
         require_antigen=require_antigen,
         max_chains=max_chains,
         pdb_id_list_path=pdb_id_list_path,
         load_ligands=load_ligands,
+        require_ligand=require_ligand,
     )
 
     if not skip_splitting:
         if tanimoto_clustering and not load_ligands:
             print(
                 "Can not use Tanimoto Clustering without load_ligands=False. Setting tanimoto_clustering to False"
             )
```

### Comparing `proteinflow-2.1.1/proteinflow/cli.py` & `proteinflow-2.2.0/proteinflow/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,14 +184,19 @@
 )
 @click.option(
     "--tanimoto_clustering",
     is_flag=True,
     help="Whether to use Tanimoto Clustering instead of MMSeqs2. Only works if load_ligands is set to True",
 )
 @click.option(
+    "--require_ligand",
+    is_flag=True,
+    help="Use this flag to require that the PDB files contain a ligand",
+)
+@click.option(
     "--random_seed",
     default=42,
     type=int,
     help="The random seed to use for splitting",
 )
 @click.option(
     "--max_chains",
```

### Comparing `proteinflow-2.1.1/proteinflow/constants.py` & `proteinflow-2.2.0/proteinflow/constants.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.1/proteinflow/data/__init__.py` & `proteinflow-2.2.0/proteinflow/data/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 import numpy as np
 import pandas as pd
 import py3Dmol
 from Bio import pairwise2
 from biopandas.pdb import PandasPdb
 from methodtools import lru_cache
-from torch import Tensor
+from torch import Tensor, from_numpy
 
 from proteinflow.constants import (
     _PMAP,
     ALPHABET,
     ALPHABET_REVERSE,
     ATOM_MASKS,
     BACKBONE_ORDER,
@@ -290,15 +290,15 @@
 
         """
         if cdr is not None and self.cdr is None:
             raise ValueError("CDR information not available")
         if cdr is not None:
             assert cdr in CDR_REVERSE, f"CDR must be one of {list(CDR_REVERSE.keys())}"
         chains = self._get_chains_list(chains)
-        seq = "".join([self.seq[c] for c in chains])
+        seq = "".join([self.seq[c] for c in chains]).replace("B", "")
         if encode:
             seq = np.array([ALPHABET_REVERSE[aa] for aa in seq])
         elif cdr is not None or only_known:
             seq = np.array(list(seq))
         if cdr is not None:
             cdr_arr = self.get_cdr(chains=chains)
             seq = seq[cdr_arr == cdr]
@@ -778,14 +778,38 @@
             A `ProteinEntry` object
 
         """
         with open(path, "rb") as f:
             data = pickle.load(f)
         return ProteinEntry.from_dict(data)
 
+    @staticmethod
+    def retrieve_ligands_from_pickle(path):
+        """Retrieve ligands from a pickle file.
+
+        Parameters
+        ----------
+        path : str
+            Path to the pickle file
+
+        Returns
+        -------
+        chain2ligand : dict
+            A dictionary where keys are chain IDs and values are ligand names
+
+        """
+        with open(path, "rb") as f:
+            data = pickle.load(f)
+        chain2ligand = {}
+        for chain in data:
+            if "ligand" not in data[chain]:
+                continue
+            chain2ligand[chain] = data[chain]["ligand"]
+        return chain2ligand
+
     def to_dict(self):
         """Convert a protein entry into a dictionary.
 
         Returns
         -------
         dictionary : dict
             A nested dictionary where first-level keys are chain IDs and
@@ -1188,14 +1212,53 @@
             chain_length = self.get_length([chain])
             index_array[start_index : start_index + chain_length] = (
                 id_dict[chain] if encode else chain
             )
             start_index += chain_length
         return index_array
 
+    def get_ligand_features(self, ligands, chains=None):
+        """Get ligand coordinates, smiles, and chain mapping.
+
+        Parameters
+        ----------
+        ligands : dict
+            A dictionary mapping from chain IDs to a list of ligands, where each ligand is a dictionary
+        chains : list of str, optional
+            If specified, only the ligands of the specified chains are returned (in the same order);
+            otherwise, all ligands are concatenated in alphabetical order of the chain IDs
+
+        Returns
+        -------
+        X_ligands : torch.Tensor
+            A `'torch'` tensor of shape `(N, 3)` with the ligand coordinates
+        ligand_smiles : str
+            A string with the ligand smiles separated by a dot
+        ligand_chains : torch.Tensor
+            A `'torch'` tensor of shape `(N, 1)` with the chain index of each atom
+        """
+        chains = self._get_chains_list(chains)
+        X_ligands = []
+        ligand_smiles = []
+        ligand_chains = []
+        for chain_i, chain in enumerate(chains):
+            all_smiles = ".".join([x["smiles"] for x in ligands[chain]])
+            ligand_smiles.append(all_smiles)
+            x_lig = np.concatenate([x["X"] for x in ligands[chain]])
+            X_ligands.append(x_lig)
+            ligand_chains += [[chain_i]] * len(x_lig)
+        ligand_smiles = ".".join(ligand_smiles)
+        X_ligands = from_numpy(np.concatenate(X_ligands, 0))
+        ligand_chains = Tensor(ligand_chains)
+        return (
+            X_ligands,
+            ligand_smiles,
+            ligand_chains,
+        )
+
     def _get_highlight_mask_dict(self, highlight_mask=None):
         """Turn mask array into a dictionary."""
         chain_arr = self.get_chain_id_array(encode=False)
         mask_arr = self.get_mask().astype(bool)
         highlight_mask_dict = {}
         if highlight_mask is not None:
             chains = self.get_chains()
@@ -1717,17 +1780,18 @@
             outstr.append(_Atom(row))
         chains = self.get_chains()
         colors = {ch: COLORS[i % len(COLORS)] for i, ch in enumerate(chains)}
         chain_counters = defaultdict(int)
         chain_last_res = defaultdict(lambda: None)
         if highlight_mask_dict is not None:
             for chain, mask in highlight_mask_dict.items():
-                assert len(mask) == len(
-                    self._pdb_sequence(chain)
-                ), "Mask length does not match sequence length"
+                if chain in self.get_chains():
+                    assert len(mask) == len(
+                        self._pdb_sequence(chain)
+                    ), "Mask length does not match sequence length"
         for at in outstr:
             if isinstance(opacity, dict):
                 op_ = opacity[at["chain"]]
             else:
                 op_ = opacity
             if at["resid"] != chain_last_res[at["chain"]]:
                 chain_last_res[at["chain"]] = at["resid"]
```

### Comparing `proteinflow-2.1.1/proteinflow/data/torch.py` & `proteinflow-2.2.0/proteinflow/data/torch.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,33 +18,42 @@
 
 class _PadCollate:
     """A variant of `collate_fn` that pads according to the longest sequence in a batch of sequences."""
 
     def pad_collate(self, batch):
         # find longest sequence
         out = {}
-        max_len = max(map(lambda x: x["S"].shape[0], batch))
 
-        # pad according to max_len
-        to_pad = [max_len - b["S"].shape[0] for b in batch]
         for key in batch[0].keys():
-            if key in ["chain_id", "chain_dict", "pdb_id", "cdr_id"]:
+            if key == "X_ligands" or key == "ligand_chains":
+                max_len = max([b[key].shape[0] for b in batch])
+                to_pad = [max_len - b[key].shape[0] for b in batch]
+            else:
+                max_len = max(map(lambda x: x["S"].shape[0], batch))
+                # pad according to max_len
+                to_pad = [max_len - b["S"].shape[0] for b in batch]
+            if key in ["chain_id", "chain_dict", "pdb_id", "cdr_id", "ligand_smiles"]:
                 continue
             out[key] = torch.stack(
                 [
                     torch.cat([b[key], torch.zeros((pad, *b[key].shape[1:]))], 0)
                     for b, pad in zip(batch, to_pad)
                 ],
                 0,
             )
         out["chain_id"] = torch.tensor([b["chain_id"] for b in batch])
         if "cdr_id" in batch[0]:
             out["cdr_id"] = torch.tensor([b["cdr_id"] for b in batch])
         out["chain_dict"] = [b["chain_dict"] for b in batch]
         out["pdb_id"] = [b["pdb_id"] for b in batch]
+        if "ligand_smiles" in batch[0]:
+            out["ligand_smiles"] = list([b["ligand_smiles"] for b in batch])
+            out["ligand_lengths"] = torch.tensor(
+                [len(b["ligand_chains"]) for b in batch]
+            )
         return out
 
     def __call__(self, batch):
         return self.pad_collate(batch)
 
 
 class ProteinLoader(DataLoader):
@@ -106,14 +115,15 @@
         mask_whole_chains=False,
         mask_frac=None,
         force_binding_sites_frac=0,
         shuffle_clusters=True,
         shuffle_batches=True,
         mask_all_cdrs=False,
         classes_dict_path=None,
+        load_ligands=False,
         *args,
         **kwargs,
     ) -> None:
         """Create a `ProteinLoader` instance with a `ProteinDataset` from the given arguments.
 
         Parameters
         ----------
@@ -158,14 +168,16 @@
             if `True`, a new representative is randomly selected for each cluster at each epoch (if `clustering_dict_path` is given)
         shuffle_batches : bool, default True
             if `True`, the batches are shuffled at each epoch
         mask_all_cdrs : bool, default False
             if `True`, all CDRs are masked instead of just the sampled one
         classes_dict_path : str, optional
             path to the pickled classes dictionary
+        load_ligands : bool, default False
+            if `True`, the ligands will be loaded from the PDB files and added to the features
         *args
             additional arguments to `torch.utils.data.DataLoader`
         **kwargs
             additional keyword arguments to `torch.utils.data.DataLoader`
 
         """
         dataset = ProteinDataset(
@@ -186,14 +198,15 @@
             lower_limit=lower_limit,
             upper_limit=upper_limit,
             mask_residues=mask_residues,
             mask_whole_chains=mask_whole_chains,
             mask_frac=mask_frac,
             force_binding_sites_frac=force_binding_sites_frac,
             mask_all_cdrs=mask_all_cdrs,
+            load_ligands=load_ligands,
         )
         return ProteinLoader(
             dataset=dataset,
             shuffle_batches=shuffle_batches,
             *args,
             **kwargs,
         )
@@ -275,14 +288,19 @@
         mask_residues=True,
         lower_limit=15,
         upper_limit=100,
         mask_frac=None,
         mask_whole_chains=False,
         force_binding_sites_frac=0.15,
         mask_all_cdrs=False,
+        load_ligands=False,
+        pyg_graph=False,
+        patch_around_mask=False,
+        initial_patch_size=128,
+        antigen_patch_size=128,
     ):
         """Initialize the dataset.
 
         Parameters
         ----------
         dataset_folder : str
             the path to the folder with proteinflow format input files (assumes that files are named {biounit_id}.pickle)
@@ -332,15 +350,18 @@
         mask_whole_chains : bool, default False
             if `True`, the whole chain is masked
         force_binding_sites_frac : float, default 0.15
             if `force_binding_sites_frac` > 0 and `mask_whole_chains` is `False`, in the fraction of cases where a chain
             from a polymer is sampled, the center of the masked region will be forced to be in a binding site (in PDB datasets)
         mask_all_cdrs : bool, default False
             if `True`, all CDRs will be masked (in SAbDab datasets)
-
+        load_ligands : bool, default False
+            if `True`, the ligands will be loaded as well
+        pyg_graph : bool, default False
+            if `True`, the output will be a `torch_geometric.data.Data` object instead of a dictionary
         """
         alphabet = ALPHABET
         self.alphabet_dict = defaultdict(lambda: 0)
         for i, letter in enumerate(alphabet):
             self.alphabet_dict[letter] = i
         self.alphabet_dict["X"] = 0
         self.files = defaultdict(lambda: defaultdict(list))  # file path by biounit id
@@ -351,14 +372,19 @@
         self.mask_residues = mask_residues
         self.lower_limit = lower_limit
         self.upper_limit = upper_limit
         self.mask_frac = mask_frac
         self.mask_whole_chains = mask_whole_chains
         self.force_binding_sites_frac = force_binding_sites_frac
         self.mask_all_cdrs = mask_all_cdrs
+        self.load_ligands = load_ligands
+        self.pyg_graph = pyg_graph
+        self.patch_around_mask = patch_around_mask
+        self.initial_patch_size = initial_patch_size
+        self.antigen_patch_size = antigen_patch_size
         self.feature_types = []
         if node_features_type is not None:
             self.feature_types = node_features_type.split("+")
         self.entry_type = entry_type
         self.shuffle_clusters = shuffle_clusters
         self.feature_functions = {
             "sidechain_orientation": self._sidechain,
@@ -621,14 +647,16 @@
         return data_entry.sidechain_coordinates(chains)
 
     def _process(self, filename, rewrite=False, max_length=None, min_cdr_length=None):
         """Process a proteinflow file and save it as ProteinMPNN features."""
         input_file = os.path.join(self.dataset_folder, filename)
         no_extension_name = filename.split(".")[0]
         data_entry = ProteinEntry.from_pickle(input_file)
+        if self.load_ligands:
+            ligands = ProteinEntry.retrieve_ligands_from_pickle(input_file)
         chains = data_entry.get_chains()
         if self.entry_type == "biounit":
             chain_sets = [chains]
         elif self.entry_type == "chain":
             chain_sets = [[x] for x in chains]
         elif self.entry_type == "pair":
             chain_sets = list(combinations(chains, 2))
@@ -697,14 +725,20 @@
             out["residue_idx"] = torch.tensor(
                 data_entry.get_index_array(chain_set, index_bump=100)
             )
             out["chain_encoding_all"] = torch.tensor(
                 data_entry.get_chain_id_array(chain_set)
             )
             out["chain_dict"] = data_entry.get_chain_id_dict(chain_set)
+            if self.load_ligands and len(ligands) != 0:
+                (
+                    out["X_ligands"],
+                    out["ligand_smiles"],
+                    out["ligand_chains"],
+                ) = data_entry.get_ligand_features(ligands, chain_set)
             cdr_chain_set = set()
             if data_entry.has_cdr():
                 out["cdr"] = torch.tensor(data_entry.get_cdr(chain_set, encode=True))
                 chain_type_dict = data_entry.get_chain_type_dict(chain_set)
                 if "heavy" in chain_type_dict:
                     cdr_chain_set.update(
                         [
@@ -766,14 +800,83 @@
                     for chain in self.files[data]:
                         if chain.split("__")[1] == cdr:
                             add = True
                             break
                     if add:
                         self.indices.append(i)
 
+    def _to_pyg_graph(self, data):
+        from torch_geometric.data import Data
+
+        pyg_data = Data(x=data["X"])
+        for key, value in data.items():
+            pyg_data[key] = value.unsqueeze(0)
+        return pyg_data
+
+    def _get_anchor_ind(self, data):
+        masked_ind = torch.where(data["masked_res"].bool())[0]
+        known_ind = torch.where(data["mask"].bool())[0]
+        start, end = masked_ind[0], masked_ind[-1]
+        start = known_ind[known_ind < start][-1]
+        end = known_ind[known_ind > end][0]
+        return start, end
+
+    def _get_antibody_mask(self, data):
+        mask = torch.zeros_like(data["mask"]).bool()
+        cdrs = data["cdr"]
+        chain_enc = data["chain_encoding_all"]
+        for chain_ind in data["chain_dict"].values():
+            chain_mask = chain_enc == chain_ind
+            chain_cdrs = cdrs[chain_mask]
+            if len(torch.unique(chain_cdrs)) > 1:
+                mask[chain_mask] = True
+        return mask
+
+    def _patch(self, data):
+        # adapted from diffab
+        pos_alpha = data["X"][:, 2]
+        start, end = self._get_anchor_ind(data)
+        anchor_points = torch.stack([pos_alpha[start], pos_alpha[end]], dim=0)
+        dist_anchor = torch.cdist(pos_alpha, anchor_points[[0]], p=2).min(dim=1)[
+            0
+        ]  # (L, )
+        dist_anchor[~data["mask"].bool()] = float("+inf")
+        initial_patch_idx = torch.topk(
+            dist_anchor,
+            k=min(self.initial_patch_size, dist_anchor.size(0)),
+            largest=False,
+            sorted=True,
+        )[
+            1
+        ]  # (initial_patch_size, )
+        patch_mask = data["masked_res"].clone()
+        patch_mask[start] = True
+        patch_mask[end] = True
+        patch_mask[initial_patch_idx] = True
+
+        if self.sabdab:
+            antibody_mask = self._get_antibody_mask(data)
+            antigen_mask = ~antibody_mask
+            dist_anchor_antigen = dist_anchor.masked_fill(
+                mask=antibody_mask, value=float("+inf")  # Fill antibody with +inf
+            )  # (L, )
+            antigen_patch_idx = torch.topk(
+                dist_anchor_antigen,
+                k=min(self.antigen_patch_size, antigen_mask.sum().item()),
+                largest=False,
+            )[
+                1
+            ]  # (ag_size, )
+            patch_mask[antigen_patch_idx] = True
+
+        for key, value in data.items():
+            if isinstance(value, torch.Tensor):
+                data[key] = value[patch_mask]
+        return data
+
     def __len__(self):
         """Return the number of clusters or data entries in the dataset."""
         return len(self.indices)
 
     def __getitem__(self, idx):
         """Return an entry from the dataset.
 
@@ -819,8 +922,12 @@
         else:
             data = deepcopy(self.loaded[file])
         data["chain_id"] = data["chain_dict"][chain_id]
         if cdr is not None:
             data["cdr_id"] = CDR_REVERSE[cdr]
         if self.mask_residues:
             data["masked_res"] = self._get_masked_sequence(data)
+        if self.patch_around_mask:
+            data = self._patch(data)
+        if self.pyg_graph:
+            data = self._to_pyg_graph(data)
         return data
```

### Comparing `proteinflow-2.1.1/proteinflow/data/utils.py` & `proteinflow-2.2.0/proteinflow/data/utils.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.1/proteinflow/download/__init__.py` & `proteinflow-2.2.0/proteinflow/download/__init__.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.1/proteinflow/download/boto.py` & `proteinflow-2.2.0/proteinflow/download/boto.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.1/proteinflow/ligand.py` & `proteinflow-2.2.0/proteinflow/ligand.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.1/proteinflow/logging/__init__.py` & `proteinflow-2.2.0/proteinflow/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.1/proteinflow/metrics/__init__.py` & `proteinflow-2.2.0/proteinflow/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.1/proteinflow/processing/__init__.py` & `proteinflow-2.2.0/proteinflow/processing/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     load_live=False,
     sabdab=False,
     sabdab_data_path=None,
     require_antigen=False,
     max_chains=5,
     pdb_id_list_path=None,
     load_ligands=False,
+    require_ligand=False,
 ):
     """Download and parse PDB files that meet filtering criteria.
 
     The output files are pickled nested dictionaries where first-level keys are chain Ids and second-level keys are
     the following:
 
     - `'crd_bb'`: a `numpy` array of shape `(L, 4, 3)` with backbone atom coordinates (N, C, CA, O),
@@ -100,14 +101,16 @@
         if `True`, only keep files with antigen chains (only used if `sabdab` is `True`)
     max_chains : int, default 5
         the maximum number of chains per biounit
     pdb_id_list_path : str, default None
         if provided, get pdb_ids from list (format pdb_id-num example: 1XYZ-1)
     load_ligands: boool, default False
         Whether or not to load the ligands in the pdbs
+    require_ligand: bool, default False
+        if `True`, only keep files with ligands
 
     Returns
     -------
     log : dict
         a dictionary where keys are recognized error names and values are lists of PDB ids that caused the errors
 
     """
@@ -203,14 +206,15 @@
             protein_dict = filter_and_convert(
                 pdb_entry,
                 min_length=MIN_LENGTH,
                 max_length=MAX_LENGTH,
                 max_missing_ends=MISSING_ENDS_THR,
                 max_missing_middle=MISSING_MIDDLE_THR,
                 load_ligands=ligand,
+                require_ligand=require_ligand,
             )
             # save
             with open(target_file, "wb") as f:
                 pickle.dump(protein_dict, f)
         except Exception as e:
             if show_error:
                 raise e
@@ -292,14 +296,15 @@
 def filter_and_convert(
     pdb_entry,
     min_length=50,
     max_length=150,
     max_missing_ends=5,
     max_missing_middle=5,
     load_ligands: bool = False,
+    require_ligand: bool = False,
 ):
     """Filter and convert a PDBEntry to a ProteinEntry.
 
     Parameters
     ----------
     pdb_entry : PDBEntry
         PDBEntry to be converted
@@ -309,27 +314,32 @@
         Maximum total length of the protein sequence
     missing_ends_thr : float, default 0.3
         The maximum fraction of missing residues at the ends
     missing_middle_thr : float, default 0.1
         The maximum fraction of missing residues in the middle (after missing ends are disregarded)
     load_ligands: boool, default False
         Whether or not to load the ligands in the pdbs
+    require_ligand: bool, default False
+        Whether or not to require the presence of ligands
 
     Returns
     -------
     ProteinEntry
         The converted ProteinEntry
 
     """
     pdb_dict = {}
     fasta_dict = pdb_entry.get_fasta()
     loaded_ligands = False
     if load_ligands and pdb_entry.get_ligands() is not None:
         ligand_dict = pdb_entry.get_ligands()
-        loaded_ligands = True
+        if len(ligand_dict) > 0:
+            loaded_ligands = True
+    if require_ligand and not loaded_ligands:
+        raise PDBError("No ligands found")
 
     if len(pdb_entry.get_chains()) == 0:
         raise PDBError("No chains found")
 
     if pdb_entry.has_unnatural_amino_acids():
         raise PDBError("Unnatural amino acids found")
```

### Comparing `proteinflow-2.1.1/proteinflow/split/__init__.py` & `proteinflow-2.2.0/proteinflow/split/__init__.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.1/proteinflow/split/utils.py` & `proteinflow-2.2.0/proteinflow/split/utils.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.1/proteinflow/visualize.py` & `proteinflow-2.2.0/proteinflow/visualize.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.1/proteinflow.egg-info/PKG-INFO` & `proteinflow-2.2.0/proteinflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteinflow
-Version: 2.1.1
+Version: 2.2.0
 Summary: Versatile pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
 License: BSD-3-Clause
 Keywords: bioinformatics,dataset,protein,PDB,deep learning
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proteinflow Version: 2.1.1 Summary: Versatile
+Metadata-Version: 2.1 Name: proteinflow Version: 2.2.0 Summary: Versatile
 pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova
 adaptyvbio.com>, Arthur Valentin
 adaptyvbio.com> License: BSD-3-Clause Keywords:
 bioinformatics,dataset,protein,PDB,deep learning Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
   ProteinFlow - A data processing pipeline for all your protein design needs
```

### Comparing `proteinflow-2.1.1/proteinflow.egg-info/SOURCES.txt` & `proteinflow-2.2.0/proteinflow.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -24,8 +24,9 @@
 proteinflow/metrics/__init__.py
 proteinflow/processing/__init__.py
 proteinflow/split/__init__.py
 proteinflow/split/utils.py
 tests/test_download.py
 tests/test_entry.py
 tests/test_generate.py
+tests/test_ligands.py
 tests/test_sabdab.py
```

### Comparing `proteinflow-2.1.1/pyproject.toml` & `proteinflow-2.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proteinflow"
-version = "2.1.1"
+version = "2.2.0"
 authors = [
     {name = "Liza Kozlova", email = "liza@adaptyvbio.com"},
     {name = "Arthur Valentin", email = "arthur@adaptyvbio.com"}
 ]
 description = "Versatile pipeline for processing protein structure data for deep learning applications."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `proteinflow-2.1.1/tests/test_download.py` & `proteinflow-2.2.0/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.1/tests/test_entry.py` & `proteinflow-2.2.0/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.1/tests/test_generate.py` & `proteinflow-2.2.0/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.1/tests/test_sabdab.py` & `proteinflow-2.2.0/tests/test_sabdab.py`

 * *Files identical despite different names*


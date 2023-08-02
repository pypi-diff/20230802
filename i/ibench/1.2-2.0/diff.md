# Comparing `tmp/ibench-1.2.tar.gz` & `tmp/ibench-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibench-1.2.tar", last modified: Mon Nov 28 15:37:07 2022, max compression
+gzip compressed data, was "ibench-2.0.tar", last modified: Wed Aug  2 17:01:57 2023, max compression
```

## Comparing `ibench-1.2.tar` & `ibench-2.0.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 john.cormican (676547) Dep16040 (116040)        0 2022-11-28 15:37:07.646640 ibench-1.2/
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    11357 2022-09-28 12:35:42.000000 ibench-1.2/LICENSE
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    10152 2022-11-28 15:37:07.642640 ibench-1.2/PKG-INFO
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     9750 2022-11-15 16:16:18.000000 ibench-1.2/README.md
-drwxr-xr-x   0 john.cormican (676547) Dep16040 (116040)        0 2022-11-28 15:37:07.642640 ibench-1.2/ibench/
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)       90 2022-11-17 10:17:39.000000 ibench-1.2/ibench/__init__.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     9089 2022-10-08 13:43:37.000000 ibench-1.2/ibench/add_seqs.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     3617 2022-11-17 10:32:51.000000 ibench-1.2/ibench/check_presence.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     3806 2022-11-15 16:16:18.000000 ibench-1.2/ibench/config.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     2076 2022-10-08 13:43:37.000000 ibench-1.2/ibench/constants.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     1051 2022-11-15 16:16:18.000000 ibench-1.2/ibench/download_data.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     8504 2022-11-15 16:16:18.000000 ibench-1.2/ibench/extract_hits.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     5126 2022-11-15 16:16:18.000000 ibench-1.2/ibench/html_report.py
-drwxr-xr-x   0 john.cormican (676547) Dep16040 (116040)        0 2022-11-28 15:37:07.642640 ibench-1.2/ibench/input/
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)        0 2022-10-07 13:41:12.000000 ibench-1.2/ibench/input/__init__.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     7659 2022-10-08 13:43:37.000000 ibench-1.2/ibench/input/mascot.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     1901 2022-10-08 13:43:37.000000 ibench-1.2/ibench/input/maxquant.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     4163 2022-11-15 16:16:18.000000 ibench-1.2/ibench/input/mgf.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     4960 2022-11-15 16:16:18.000000 ibench-1.2/ibench/input/mzml.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     2469 2022-10-08 13:43:37.000000 ibench-1.2/ibench/input/peaks.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     1516 2022-10-08 13:43:37.000000 ibench-1.2/ibench/input/percolator.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     4748 2022-10-08 13:43:37.000000 ibench-1.2/ibench/input/search_results.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    11111 2022-11-15 16:16:18.000000 ibench-1.2/ibench/modify_db.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    26766 2022-11-15 16:16:18.000000 ibench-1.2/ibench/performance.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     5533 2022-11-28 15:27:11.000000 ibench-1.2/ibench/query_table.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     1937 2022-11-15 16:16:18.000000 ibench-1.2/ibench/run.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     5562 2022-10-08 13:43:37.000000 ibench-1.2/ibench/utils.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     4132 2022-11-15 16:16:18.000000 ibench-1.2/ibench/validate_assignments.py
-drwxr-xr-x   0 john.cormican (676547) Dep16040 (116040)        0 2022-11-28 15:37:07.642640 ibench-1.2/ibench.egg-info/
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    10152 2022-11-28 15:37:07.000000 ibench-1.2/ibench.egg-info/PKG-INFO
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)      696 2022-11-28 15:37:07.000000 ibench-1.2/ibench.egg-info/SOURCES.txt
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)        1 2022-11-28 15:37:07.000000 ibench-1.2/ibench.egg-info/dependency_links.txt
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)       43 2022-11-28 15:37:07.000000 ibench-1.2/ibench.egg-info/entry_points.txt
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)      198 2022-11-28 15:37:07.000000 ibench-1.2/ibench.egg-info/requires.txt
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)        7 2022-11-28 15:37:07.000000 ibench-1.2/ibench.egg-info/top_level.txt
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)       38 2022-11-28 15:37:07.646640 ibench-1.2/setup.cfg
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     1124 2022-11-17 10:17:23.000000 ibench-1.2/setup.py
+drwxr-xr-x   0 john.cormican (676547) Dep16040 (116040)        0 2023-08-02 17:01:57.416108 ibench-2.0/
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    11357 2022-09-28 12:35:42.000000 ibench-2.0/LICENSE
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    10152 2023-08-02 17:01:57.416108 ibench-2.0/PKG-INFO
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     9750 2022-11-15 16:16:18.000000 ibench-2.0/README.md
+drwxr-xr-x   0 john.cormican (676547) Dep16040 (116040)        0 2023-08-02 17:01:57.412108 ibench-2.0/ibench/
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)       90 2023-08-02 16:38:11.000000 ibench-2.0/ibench/__init__.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     9089 2022-10-08 13:43:37.000000 ibench-2.0/ibench/add_seqs.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     4555 2023-08-02 16:38:11.000000 ibench-2.0/ibench/check_presence.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     4512 2023-08-02 16:38:11.000000 ibench-2.0/ibench/config.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     2076 2022-10-08 13:43:37.000000 ibench-2.0/ibench/constants.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     1051 2022-11-15 16:16:18.000000 ibench-2.0/ibench/download_data.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    10930 2023-08-02 16:38:11.000000 ibench-2.0/ibench/extract_hits.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     5125 2023-08-02 16:38:11.000000 ibench-2.0/ibench/html_report.py
+drwxr-xr-x   0 john.cormican (676547) Dep16040 (116040)        0 2023-08-02 17:01:57.416108 ibench-2.0/ibench/input/
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)        0 2022-10-07 13:41:12.000000 ibench-2.0/ibench/input/__init__.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     1811 2023-05-23 11:42:14.000000 ibench-2.0/ibench/input/inspire.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     6274 2023-05-23 11:44:10.000000 ibench-2.0/ibench/input/invitrospi.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     7659 2022-10-08 13:43:37.000000 ibench-2.0/ibench/input/mascot.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     1901 2022-10-08 13:43:37.000000 ibench-2.0/ibench/input/maxquant.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     4163 2022-11-15 16:16:18.000000 ibench-2.0/ibench/input/mgf.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     4960 2022-11-15 16:16:18.000000 ibench-2.0/ibench/input/mzml.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     2468 2023-08-02 16:38:11.000000 ibench-2.0/ibench/input/peaks.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     1663 2023-08-02 16:38:11.000000 ibench-2.0/ibench/input/percolator.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     4815 2023-08-02 16:38:11.000000 ibench-2.0/ibench/input/search_results.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    12094 2023-08-02 16:38:11.000000 ibench-2.0/ibench/modify_db.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    30578 2023-08-02 16:48:54.000000 ibench-2.0/ibench/performance.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     8713 2023-08-02 16:53:32.000000 ibench-2.0/ibench/query_table.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     1937 2023-08-01 14:06:33.000000 ibench-2.0/ibench/run.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     5562 2022-10-08 13:43:37.000000 ibench-2.0/ibench/utils.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     4132 2022-11-15 16:16:18.000000 ibench-2.0/ibench/validate_assignments.py
+drwxr-xr-x   0 john.cormican (676547) Dep16040 (116040)        0 2023-08-02 17:01:57.412108 ibench-2.0/ibench.egg-info/
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    10152 2023-08-02 17:01:57.000000 ibench-2.0/ibench.egg-info/PKG-INFO
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)      747 2023-08-02 17:01:57.000000 ibench-2.0/ibench.egg-info/SOURCES.txt
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)        1 2023-08-02 17:01:57.000000 ibench-2.0/ibench.egg-info/dependency_links.txt
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)       43 2023-08-02 17:01:57.000000 ibench-2.0/ibench.egg-info/entry_points.txt
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)      201 2023-08-02 17:01:57.000000 ibench-2.0/ibench.egg-info/requires.txt
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)        7 2023-08-02 17:01:57.000000 ibench-2.0/ibench.egg-info/top_level.txt
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)       38 2023-08-02 17:01:57.416108 ibench-2.0/setup.cfg
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     1127 2023-08-02 16:38:11.000000 ibench-2.0/setup.py
```

### Comparing `ibench-1.2/LICENSE` & `ibench-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ibench-1.2/PKG-INFO` & `ibench-2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibench
-Version: 1.2
+Version: 2.0
 Summary: Benchmarking for mass spectrometry identifications.
 Author: John Cormican, Juliane Liepe
 Author-email: juliane.liepe@mpinat.mpg.de
 Project-URL: Homepage, https://github.com/QuantSysBio/iBench
 Project-URL: Tracker, https://github.com/QuantSysBio/iBench/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ibench-1.2/README.md` & `ibench-2.0/README.md`

 * *Files identical despite different names*

### Comparing `ibench-1.2/ibench/add_seqs.py` & `ibench-2.0/ibench/add_seqs.py`

 * *Files identical despite different names*

### Comparing `ibench-1.2/ibench/check_presence.py` & `ibench-2.0/ibench/check_presence.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,40 @@
 """ Utility functions for checking for the presence of a peptide in a proteome.
 """
 import re
 
+def find_trans_matched(protein, splice_reactants, proteome):
+    """ Function to check if any two potential splice reactants of a peptide are present in one
+        protein and across the proteome.
+    
+    Parameters
+    ----------
+    protein : str
+        The protein sequence.
+    splice_reactants : list of tuple of str
+        A list of the possible splice reactants for the peptide.
+    proteome : list of str
+        A list of the proteins to be considered
+
+    Returns
+    -------
+    found_trans : bool
+        True if the peptide is present as a transspliced peptide, False otherwise.
+    """
+    for (sr_1, sr_2) in splice_reactants:
+        if sr_1 in protein:
+            for trans_protein in proteome:
+                if sr_2 in trans_protein:
+                    return True
+        if sr_2 in protein:
+            for trans_protein in proteome:
+                if sr_1 in trans_protein:
+                    return True
+
+
 def find_cis_matched_splice_reactants(protein, splice_reactants, max_intervening):
     """ Function to check if any two potential splice reactants of a peptide are present in
         a single protein.
 
     Parameters
     ----------
     protein : str
```

### Comparing `ibench-1.2/ibench/config.py` & `ibench-2.0/ibench/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 """ Definition of the Config class which is used to manage the iBench experiement.
 """
 import os
 
 import yaml
 
 ALL_CONFIG_KEYS = (
+    'allowTrans',
     'benchmarkResults',
     'closenessCutOff',
+    'dropDuplicates',
     'filterPTMs',
     'identifier',
+    'inspireSettings',
+    'inVitroBenchmark',
     'scanFolder',
     'scanFormat',
     'searchResults',
     'maxIntervening',
     'maxSequenceLength',
     'minSequenceLength',
     'outputFolder',
     'randomSeed',
     'scoreCutOffs',
     'qValueCutOffs',
     'canonicalFraction',
     'cissplicedFraction',
+    'resultsFiles',
     'singleScanFile',
+    'spectralAngleCutOff',
     'transsplicedFraction',
     'proteome',
     'ms2Accuracy',
     'enzyme',
 )
 
 class Config:
@@ -57,44 +63,54 @@
         config_data : dict
             The data parsed from the yaml file.
         """
         self.identifier = config_dict['identifier']
         self.search_results = config_dict.get('searchResults')
         self.output_folder = config_dict.get('outputFolder')
         self.random_seed = config_dict.get('randomSeed', 42)
+        self.results_files = config_dict.get('resultsFiles', None)
+        self.drop_duplicates = config_dict.get('dropDuplicates', True)
         self.q_cuts = config_dict.get('qValueCutOffs')
         self.discoverable_fraction = config_dict['canonicalFraction']
         self.cisspliced_fraction = config_dict.get('cissplicedFraction', 0.0)
         self.filter_ptms = config_dict.get('filterPTMs', True)
         self.transspliced_fraction = config_dict['transsplicedFraction']
         self.input_database = config_dict.get('inputDatabase')
-        self.proteome_loc = config_dict['proteome']
+        self.proteome_loc = config_dict.get('proteome')
         self.min_seq_len = config_dict.get('minSequenceLength', 7)
         self.max_seq_len = config_dict.get('maxSequenceLength', 30)
         self.scan_folder = config_dict.get('scanFolder')
         self.scan_format = config_dict.get('scanFormat')
         self.benchmark_results = config_dict.get('benchmarkResults')
         self.ms2_accuracy = config_dict.get('ms2Accuracy', 0.02)
         self.enzyme = config_dict.get('enzyme')
         self.max_intervening = config_dict.get('maxIntervening', 25)
         self.single_scan_file = config_dict.get('singleScanFile', True)
+        self.invitro_benchmark = config_dict.get('inVitroBenchmark', False)
+        self.inspire_settings = config_dict.get('inspireSettings', None)
+        self.spectral_angle_cut_offs = config_dict.get('spectralAngleCutOffs', {
+            'canonical': 0.7,
+            'cisspliced': 0.7,
+            'transspliced': 0.7,
+        })
+        self.allow_trans = config_dict.get('allowTrans', False)
 
         if self.cisspliced_fraction > 0.0:
             self.closeness_cut_off = config_dict.get('closenessCutOff', 3)
         else:
             self.closeness_cut_off = config_dict.get('closenessCutOff', 1)
 
         if not os.path.exists(self.output_folder):
             os.makedirs(self.output_folder)
 
     def validate(self, pipeline):
         """ Check the values in the config file to ensure they are valid.
         """
         if pipeline == 'createDB':
-            if not os.path.exists(self.proteome_loc):
+            if not self.invitro_benchmark and not os.path.exists(self.proteome_loc):
                 raise ValueError(f'No file at:\n\t{self.proteome_loc}')
         elif pipeline == 'analysis':
             if self.benchmark_results is None:
                 raise ValueError('No results provided to benchmark.')
         elif pipeline == 'downloadExample':
             return
         else:
```

### Comparing `ibench-1.2/ibench/constants.py` & `ibench-2.0/ibench/constants.py`

 * *Files identical despite different names*

### Comparing `ibench-1.2/ibench/download_data.py` & `ibench-2.0/ibench/download_data.py`

 * *Files identical despite different names*

### Comparing `ibench-1.2/ibench/extract_hits.py` & `ibench-2.0/ibench/extract_hits.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,24 +6,26 @@
 
 import pandas as pd
 import numpy as np
 
 from ibench.check_presence import generate_pairs
 from ibench.constants import (
     CANONICAL_KEY,
+    CHARGE_KEY,
     CISSPLICED_KEY,
     ENDC_TEXT,
     GT_SCAN_KEY,
     GT_SOURCE_KEY,
     IL_PEPTIDE_KEY,
     OKCYAN_TEXT,
     PEPTIDE_KEY,
     SOURCE_KEY,
     TRANSPLICED_KEY,
 )
+from ibench.input.invitrospi import read_invitro_spi_dbs
 from ibench.input.mzml import process_mzml_files
 from ibench.input.mgf import process_mgf_files
 from ibench.input.search_results import generic_read_df
 
 def _check_multiple_subseqs(peptide_list, max_group):
     """ Function to check if a peptide contains multiple subsequences,
         if so it shouldn't be assigned cisspliced.
@@ -201,60 +203,127 @@
     """ Helper function to get the peptide group of a peptide.
     """
     for idx, pep_grp in enumerate(peptide_groups):
         if peptide in pep_grp:
             return idx
     return -1
 
+def invitro_id_strata_filter(target_df, unique_pep_df, strata_fractions, config):
+    """ Function to filter strata sizes for invitro polypeptide identifications.
+
+    Parameters
+    ----------
+    target_df : pd.DataFrame
+        The identifications from original polypeptide digestions.
+    unique_pep_df : pd.DataFrame
+        The unique peptides identified.
+    strata_fraction : dict
+        Dictionary of the fractions of each stratum required.
+    config : ibench.config.Config
+        The config object which controls the experiment.
+
+    Returns
+    -------
+    hq_df : pd.DataFrame
+        The DataFrame of high quality identifications with the required ratios.
+    """
+    strata_ratios = {
+        'canonical': config.discoverable_fraction/strata_fractions['canonical'],
+        'cisspliced': config.cisspliced_fraction/strata_fractions['cisspliced'],
+        'transspliced': config.transspliced_fraction/strata_fractions['transspliced'],
+    }
+    divisor = max(strata_ratios.values())
+
+    strat_dfs = []
+    for stratum, strat_ratio in strata_ratios.items():
+        sample_frac = strat_ratio/divisor
+
+        strat_df = unique_pep_df[unique_pep_df['stratum'] == stratum].reset_index(drop=True)
+        strat_dfs.append(
+            strat_df.sample(
+                frac=sample_frac,
+                random_state=7,
+            )
+        )
+
+    unique_pep_df_all_strata = pd.concat(strat_dfs)
+    hq_df = pd.merge(
+        target_df,
+        unique_pep_df_all_strata[['peptide']],
+        how='inner',
+        on='peptide'
+    )
+
+    return hq_df
+
 def extract_hq_hits(config):
     """ Function to extract the high quality PSMs from the search results provided.
 
     Parameters
     ----------
     config : ibench.config.Config
         The config object which controls the experiment.
     """
     # Read in all search results:
-    target_df = generic_read_df(
-        config,
-        hq_hits_only=True,
-    )
+    if config.invitro_benchmark:
+        target_df = read_invitro_spi_dbs(
+            config,
+        )
+        target_df = target_df.drop(CHARGE_KEY, axis=1)
+    else:
+        target_df = generic_read_df(
+            config,
+            hq_hits_only=True,
+        )
 
     # Create I/L redundant peptides
     target_df[IL_PEPTIDE_KEY] = target_df[PEPTIDE_KEY].apply(
         lambda x : x.replace('I', 'L')
     )
-    target_df = target_df.drop_duplicates(subset=[IL_PEPTIDE_KEY])
-
-    peptides = target_df[IL_PEPTIDE_KEY].tolist()
-    peptide_groups = get_peptide_groups(peptides, config.closeness_cut_off)
-    target_df['peptideGroup'] = target_df[IL_PEPTIDE_KEY].apply(
-        lambda x : _get_group(x, peptide_groups)
-    )
+    if config.invitro_benchmark:
+        unique_pep_df = deepcopy(
+            target_df.drop_duplicates(subset=[IL_PEPTIDE_KEY])
+        )
+        strata_counts = unique_pep_df['stratum'].value_counts()
+        strata_fractions = (strata_counts/strata_counts.sum()).to_dict()
+        if config.discoverable_fraction != -1:
+            hq_df = invitro_id_strata_filter(target_df, unique_pep_df, strata_fractions, config)
+        else:
+            hq_df = target_df
+    else:
+        if config.drop_duplicates:
+            target_df = target_df.drop_duplicates(subset=[IL_PEPTIDE_KEY])
+        peptides = target_df[IL_PEPTIDE_KEY].unique().tolist()
+
+        peptide_groups = get_peptide_groups(peptides, config.closeness_cut_off)
+        target_df['peptideGroup'] = target_df[IL_PEPTIDE_KEY].apply(
+            lambda x : _get_group(x, peptide_groups)
+        )
+        hq_df = assign_strata(target_df, config)
 
-    hq_df = assign_strata(target_df, config)
-    hq_df = hq_df.reset_index(drop=True)
     scan_files = sorted(hq_df[SOURCE_KEY].unique().tolist())
     if config.single_scan_file:
         hq_df[GT_SOURCE_KEY] = f'ibenchGroundTruth_{config.identifier}'
     else:
         hq_df[GT_SOURCE_KEY] = hq_df[SOURCE_KEY].apply(
             lambda x : f'ibenchGroundTruth_{config.identifier}_{scan_files.index(x)}'
         )
+    hq_df = hq_df.reset_index(drop=True)
     hq_df[GT_SCAN_KEY] = hq_df.index + 1
 
     if config.scan_format == 'mgf':
         hq_df = process_mgf_files(hq_df, config, scan_files)
     else:
         hq_df = process_mzml_files(hq_df, config, scan_files)
 
     hq_df = hq_df.sort_values(by=GT_SCAN_KEY)
 
-    hq_df = hq_df.drop(
-        ['peptideGroup', 'groupOrder', 'forceCanonical'],
-        axis=1,
-    )
+    if not config.invitro_benchmark:
+        hq_df = hq_df.drop(
+            ['peptideGroup', 'groupOrder', 'forceCanonical'],
+            axis=1,
+        )
 
     hq_df.to_csv(
         f'{config.output_folder}/high_confidence.csv',
         index=False,
     )
```

### Comparing `ibench-1.2/ibench/html_report.py` & `ibench-2.0/ibench/html_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         html_string += (
             '''
                 </center>
                 <h3>
                     False Discovery Rate Estimation
                 </h3>
                 <p>
-                    This plots the estimated FDR against observed FDR for each method.
+                    This plots the reported FDR against observed FDR for each method.
                 </p>
                 <center>
             ''' + figures['fdr']
         )
 
     html_string += ('''
             </center>
```

### Comparing `ibench-1.2/ibench/input/mascot.py` & `ibench-2.0/ibench/input/mascot.py`

 * *Files identical despite different names*

### Comparing `ibench-1.2/ibench/input/maxquant.py` & `ibench-2.0/ibench/input/maxquant.py`

 * *Files identical despite different names*

### Comparing `ibench-1.2/ibench/input/mgf.py` & `ibench-2.0/ibench/input/mgf.py`

 * *Files identical despite different names*

### Comparing `ibench-1.2/ibench/input/mzml.py` & `ibench-2.0/ibench/input/mzml.py`

 * *Files identical despite different names*

### Comparing `ibench-1.2/ibench/input/peaks.py` & `ibench-2.0/ibench/input/peaks.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,9 +81,8 @@
         SOURCE_KEY,
         SCAN_KEY,
         ENGINE_SCORE_KEY,
         PEPTIDE_KEY,
         LABEL_KEY,
     ]]
 
-
     return peaks_df
```

### Comparing `ibench-1.2/ibench/input/percolator.py` & `ibench-2.0/ibench/input/percolator.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,9 +56,13 @@
         SOURCE_KEY,
         SCAN_KEY,
         ENGINE_SCORE_KEY,
         Q_VALUE_KEY,
         PEPTIDE_KEY,
         LABEL_KEY,
     ]]
+    if perc_df[PEPTIDE_KEY].iloc[0][1] == '.':
+        perc_df[PEPTIDE_KEY] = perc_df[PEPTIDE_KEY].apply(
+            lambda x : x[2:-2]
+        )
 
     return perc_df
```

### Comparing `ibench-1.2/ibench/input/search_results.py` & `ibench-2.0/ibench/input/search_results.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,18 +66,22 @@
                     how='inner',
                     on=[SOURCE_KEY, SCAN_KEY, PEPTIDE_KEY],
                 )
             merged_result_list.append(id_df)
         else:
             merged_result_list.append(all_search_results[id_group][0])
     combined_df = pd.concat(merged_result_list)
-    combined_df = combined_df.sort_values(by=ENGINE_SCORE_KEY, ascending=False)
 
     if hq_hits_only:
-        combined_df = combined_df.drop_duplicates(PEPTIDE_KEY)
+        combined_df = combined_df.sort_values(
+            by=ENGINE_SCORE_KEY, ascending=False,
+        )
+
+        if config.drop_duplicates:
+            combined_df = combined_df.drop_duplicates(PEPTIDE_KEY)
         combined_df = combined_df[
             (combined_df['sequenceLength'] >= config.min_seq_len) &
             (combined_df['sequenceLength'] <= config.max_seq_len)
         ]
 
     return combined_df
```

### Comparing `ibench-1.2/ibench/modify_db.py` & `ibench-2.0/ibench/modify_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,22 +72,51 @@
                     if replace_strings is not None:
                         for replace_string in replace_strings:
                             modified_ids.append(idx)
                             proteome[idx] = remove_substring(proteome[idx], replace_string)
 
     return proteome, modified_ids
 
+def write_single_in_silico_protein(config):
+    """ Function to write a single protein made up of concatenated polypeptides.
+
+    Parameters
+    ----------
+    config : ibench.config.Config
+        The Config object used to manage the experiment.
+    """
+    combined_prot = ''
+    for results in config.search_results:
+        results_loc = results['resultsLocation']
+        polypep_seqs = [
+            str(x.seq) for x in SeqIO.parse(
+                f'{results_loc}/polypeptides.fasta', 'fasta'
+            )
+        ]
+        for polypep_seq in polypep_seqs:
+            combined_prot += polypep_seq#.replace('I', 'L')
+        with open(
+            f'{config.output_folder}/modified_proteome.fasta',
+            'w',
+            encoding='UTF-8',
+        ) as prot_file:
+            prot_file.write('>modified_invitro_protein\n')
+            prot_file.write(f'{combined_prot}\n')
+
 def modify_db(config):
     """ Function to create the artificial reference database.
 
     Parameters
     ----------
     config : ibench.config.Config
         The Config object used to manage the experiment.
     """
+    if config.invitro_benchmark:
+        write_single_in_silico_protein(config)
+        return
     hq_df = pd.read_csv(f'{config.output_folder}/high_confidence.csv')
     peptide_strata = get_pepitde_strata(hq_df)
 
     with open(config.proteome_loc, encoding='UTF-8') as prot_file:
         fasta_sequences = [
             str(x.seq) for x in SeqIO.parse(
                 prot_file,
```

### Comparing `ibench-1.2/ibench/performance.py` & `ibench-2.0/ibench/performance.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,31 +45,40 @@
     -------
     pr_curve : go.Scatter
         Plotly graph object for the ROC curve.
     min_p : float
         The minimum precison value observed for any threshold.
     """
     name = result_dict['name']
-    cut_offs = _generate_cut_offs(qt_df, f'{name}Score', 1_000)
+    cut_offs = _generate_cut_offs(qt_df, f'{name}Score', 1000)
     true_count = qt_df[qt_df['trueStratum'] == stratum].shape[0]
     precisions = []
     recalls = []
     for cut_off in cut_offs:
         pred_count, correct_count, _ = _get_counts(
             qt_df, cut_off, name, stratum
         )
-        if pred_count > 0:
+        if pred_count/true_count > 0.02:
             precisions.append(correct_count/pred_count)
             recalls.append(correct_count/true_count)
+    
+    top_id_df = qt_df[qt_df[f'{name}Stratum'] == stratum].nlargest(n=1, columns=f'{name}Score')
+    if top_id_df[top_id_df.apply(
+        lambda x : x['truePeptide'].replace('I', 'L') == x[f'{name}Peptide'].replace('I', 'L'),
+        axis=1
+    )].shape[0]:
+        precisions.append(1.0)
+        recalls.append(1.0/true_count)
+
     min_p = min(precisions)
     return go.Scatter(
         x=recalls,
         y=precisions,
         name=f'{name} PR',
-        line={'color': result_dict['colour']}
+        line={'color': result_dict['colour'], 'dash': result_dict.get('dash')}
     ), min_p
 
 def create_roc_curve(qt_df, result_dict, stratum):
     """ Function to create a roc curve for a given result.
     Parameters
     ----------
     qt_df : pd.DataFrame
@@ -98,32 +107,79 @@
             tprs.append(correct_count/true_count)
             fprs.append(false_positives/total_negative)
     max_tpr = max(tprs)
     return go.Scatter(
         x=fprs,
         y=tprs,
         name=f'{name} ROC',
-        line={'color': result_dict['colour']}
+        line={'color': result_dict['colour'], 'dash': result_dict.get('dash')}
     ), max_tpr
 
 
+def get_pr_dots(qt_df, stratum, config):
+    """ Function to get the 1% FDR cut offs for each method to be plotted on PR curves.
+
+    Parameters
+    ----------
+    qt_df : pd.DataFrame
+        The Query Table containing ground truth assignments joined to the user's assignments.
+    stratum : str
+        The stratum for which we require precision and recall at 1% FDR.
+    config : ibench.config.Config
+        The Config object used to run the experiment.
+    """
+    pr_dots = {}
+    for results in config.benchmark_results:
+        one_pct_cut_off = None
+        name = results['name']
+        true_count = qt_df[qt_df['trueStratum'] == stratum].shape[0]
+        if 'fdrCuts' in results:
+            one_pct_cut_off = results['fdrCuts'][1.0]
+        elif results['searchEngine'] == 'percolator':
+            one_pct_cut_off = qt_df[
+                qt_df[f'{name}qValue'] < 0.01
+            ][f'{name}Score'].min() - 0.01
+        
+        if one_pct_cut_off is not None:
+            pred_count, correct_count, _ = _get_counts(
+                qt_df, one_pct_cut_off, name, stratum
+            )
+            if pred_count > 0:
+                pr_dots[name] = {
+                    'recall': correct_count/true_count,
+                    'precision': correct_count/pred_count,
+                    'colour': results['colour']
+                }
+
+    return pr_dots
+
 def plot_precision_recall(qt_df, config):
     """ Function to plot the precision recall curve of the identification method.
+
     Parameters
     ----------
     qt_df : pd.DataFrame
         The Query Table containing ground truth assignments joined to the user's assignments.
     config : ibench.config.Config
         The Config object used to run the experiment.
     """
-    strata = [x for x in qt_df['trueStratum'].unique() if x != TRANSPLICED_KEY]
+    if config.allow_trans:
+        strata = sorted(
+            list(qt_df['trueStratum'].unique())
+        )
+    else:
+        strata = sorted(
+            [x for x in qt_df['trueStratum'].unique() if x != TRANSPLICED_KEY]
+        )
 
     pr_curves = {}
+    pr_dots = {}
     min_pr = 1.0
     for stratum in strata:
+        pr_dots[stratum] = get_pr_dots(qt_df, stratum, config)
         pr_curves[stratum] = []
         for results in config.benchmark_results:
             pr_trace, pr_val = create_pr_curve(qt_df, results, stratum)
             pr_curves[stratum].append(pr_trace)
             min_pr = min(min_pr, pr_val)
 
     y_lower_lim = floor(min_pr*10)/10
@@ -137,14 +193,30 @@
     for idx, stratum in enumerate(strata):
         for pr_trace in pr_curves[stratum]:
             fig.add_trace(
                 pr_trace,
                 row=1,
                 col=idx+1,
             )
+            for name in pr_dots[stratum]:
+                fig.add_trace(
+                    go.Scatter(
+                        mode='markers',
+                        x=[pr_dots[stratum][name]['recall']],
+                        y=[pr_dots[stratum][name]['precision']],
+                        name=f'{name} 1FDR Precision-Recall',
+                        showlegend=False,
+                        marker={
+                            'color': pr_dots[stratum][name]['colour'],
+                            'size': 12,
+                        },
+                    ),
+                    row=1,
+                    col=idx+1,
+                )
 
     fig.update_layout(
         width=880*len(strata),
         height=500,
         title_x=0.5,
         plot_bgcolor='rgba(0,0,0,0)',
         yaxis_showticklabels=True,
@@ -153,15 +225,15 @@
         fig.update_layout({f'yaxis{idx}_showticklabels': True})
     fig.update_xaxes(
         showline=True,
         linewidth=0.5,
         linecolor='black',
         showgrid=False,
         ticks="outside",
-        range=[0,1],
+        range=[0.0,1],
     )
     fig.update_yaxes(
         showline=True,
         linewidth=0.5,
         linecolor='black',
         showgrid=False,
         ticks="outside",
@@ -169,79 +241,104 @@
     )
     for i in range(1, len(strata)+1):
         fig['layout'][f'xaxis{i}']['title'] = 'Recall'
         fig['layout'][f'yaxis{i}']['title'] = 'Precision'
     return fig.to_html()
 
 def create_fdr_curve(qt_df, results, stratum):
-    """ Function to create a true vs estimated fdr curve for a given result.
+    """ Function to create a true vs reported fdr curve for a given result.
     Parameters
     ----------
     qt_df : pd.DataFrame
         The Query Table containing ground truth assignments joined to the user's assignments.
     result_dict : dictionary
         Dictionary of meta-data about the method being plotted.
     stratum : str
         The stratum for which the curve is being plotted.
     Returns
     -------
-    roc_curve : go.Scatter
-        Plotly graph object for the true vs. estimated curve.
+    fdr_curve : go.Scatter
+        Plotly graph object for the true vs. reported fdr curve.
     """
     fdrs = []
     name = results['name']
     if 'fdrCuts' in results:
         goal_fdrs = results['fdrCuts'].keys()
+        fdr_dict = results['fdrCuts']
+    elif results['searchEngine'] == 'percolator':
+        name = results['name']
+        goal_fdrs = [0.005, 0.01, 0.02, 0.05]
+        fdr_dict = {
+            fdr_cut: qt_df[qt_df[f'{name}qValue'] < fdr_cut][f'{name}Score'].min() - 0.01
+            for fdr_cut in goal_fdrs
+        }
+    else:
+        goal_fdrs = []
+
+    if goal_fdrs:
         found_fdrs = []
         for gofdr in goal_fdrs:
             filtered_df = qt_df[
-                (qt_df[f'{name}Score'] > results['fdrCuts'][gofdr]) &
+                (qt_df[f'{name}Score'] > fdr_dict[gofdr]) &
                 (qt_df[f'{name}Stratum'] == stratum)
             ]
             n_found = filtered_df.shape[0]
             correct_count = filtered_df[filtered_df.apply(
                 lambda x : x['truePeptide'].replace('I', 'L') == x[f'{name}Peptide'].replace('I', 'L'),
                 axis=1
             )].shape[0]
             if n_found > 0:
                 fdrs.append(100*(1-(correct_count/n_found)))
-                found_fdrs.append(gofdr)
+                if gofdr < 0.1:
+                    found_fdrs.append(gofdr*100)
+                else:
+                    found_fdrs.append(gofdr)
+
     else:
         goal_fdrs = [0.5*i for i in range(1, 11)]
         found_fdrs = []
         for gofdr, fdr_cut in zip(goal_fdrs, [0.005*i for i in range(1, 11)]):
             filtered_df = qt_df[
                 (qt_df[f'{name}qValue'] < fdr_cut) &
                 (qt_df[f'{name}Stratum'] == stratum)
             ]
             n_found = filtered_df.shape[0]
             correct_count = filtered_df[filtered_df.apply(
-                lambda x : x['truePeptide'].replace('I', 'L') == x[f'{name}Peptide'].replace('I', 'L'),
+                lambda x : x['truePeptide'].replace(
+                    'I', 'L'
+                ) == x[f'{name}Peptide'].replace('I', 'L'),
                 axis=1
             )].shape[0]
             if n_found > 0:
                 fdrs.append(100*(1-(correct_count/n_found)))
                 found_fdrs.append(gofdr)
     return go.Scatter(
         x=found_fdrs,
         y=fdrs,
         name=f'{name} FDR',
-        line={'color': results['colour']}
+        line={'color': results['colour'], 'dash': results.get('dash')}
     )
 
 def plot_fdr_estimation(qt_df, config):
     """ Function to plot the accuracy of
     """
-    strata = [x for x in qt_df['trueStratum'].unique() if x != TRANSPLICED_KEY]
+    if config.allow_trans:
+        strata = sorted(
+            list(qt_df['trueStratum'].unique())
+        )
+    else:
+        strata = sorted(
+            [x for x in qt_df['trueStratum'].unique() if x != TRANSPLICED_KEY]
+        )
     fdr_curves = {}
 
     for stratum in strata:
         fdr_curves[stratum] = [go.Scatter(
-            x=[i*0.5 for i in range(11)],
-            y=[i*0.5 for i in range(11)],
+            x=[i*0.5 for i in range(2, 11)],
+            y=[i*0.5 for i in range(2, 11)],
             name='Perfect FDR Estimation',
             line={'color': 'black', 'dash': 'dash'}
         )]
         for results in config.benchmark_results:
             if results['searchEngine'] in ('mascot', 'percolator') or 'fdrCuts' in results:
                 fdr_trace = create_fdr_curve(qt_df, results, stratum)
                 fdr_curves[stratum].append(fdr_trace)
@@ -273,24 +370,25 @@
         fig.update_layout({f'yaxis{idx}_showticklabels': True})
     fig.update_xaxes(
         showline=True,
         linewidth=0.5,
         linecolor='black',
         showgrid=False,
         ticks="outside",
+        range=[0,5],
     )
     fig.update_yaxes(
         showline=True,
         linewidth=0.5,
         linecolor='black',
         showgrid=False,
         ticks="outside",
     )
     for i in range(1, len(strata)+1):
-        fig['layout'][f'xaxis{i}']['title'] = 'Estimated FDR'
+        fig['layout'][f'xaxis{i}']['title'] = 'Reported FDR'
         fig['layout'][f'yaxis{i}']['title'] = 'Observed FDR'
 
     return fig.to_html()
 
 def analyse_performance(config):
     """ Function to analyse performance of an identification method or methods on
         iBench ground truth datasets.
@@ -377,14 +475,15 @@
         ))
 
     return traces
 
 def plot_overall_distro(qt_df, config):
     """ Function to plot engine scores for correct and and incorrect PSMs against confounding
         variables.
+
     Parameters
     ----------
     qt_df : pd.DataFrame
         The Query Table containing ground truth assignments joined to the user's assignments.
     config : ibench.config.Config
         The Config object used to run the experiment.
     """
@@ -494,22 +593,22 @@
         The feature being plotted.
     Returns
     -------
     traces : list of go.Scatter
         list of Plotly graph objects for the violin plots.
     """
     name = results['name']
+    print(name, feature, stratum)
     grouped_df = qt_df.groupby(feature, as_index=False)[f'{name}Score'].count()
     grouped_df.columns = [feature, 'count']
     grouped_df = grouped_df[grouped_df['count'] > qt_df.shape[0]/100]
     plot_vals = grouped_df[feature].tolist()
 
     qt_df = qt_df[qt_df['trueStratum'] == stratum]
     qt_df = qt_df[qt_df[feature].apply(lambda x : x in plot_vals)]
-
     qt_df['correct'] = qt_df.apply(
         lambda x : (
             'correct' if isinstance(x[f'{name}Peptide'], str) and
             x[f'{name}Peptide'].replace('I', 'L') == x['truePeptide'].replace('I', 'L')
             else 'incorrect'
         ),
         axis=1
@@ -558,16 +657,22 @@
     Parameters
     ----------
     qt_df : pd.DataFrame
         The Query Table containing ground truth assignments joined to the user's assignments.
     config : ibench.config.Config
         The Config object used to run the experiment.
     """
-    strata = [x for x in qt_df['trueStratum'].unique() if x != TRANSPLICED_KEY]
-
+    if config.allow_trans:
+        strata = sorted(
+            list(qt_df['trueStratum'].unique())
+        )
+    else:
+        strata = sorted(
+            [x for x in qt_df['trueStratum'].unique() if x != TRANSPLICED_KEY]
+        )
     qt_df['hydrophobicity'] = qt_df['truePeptide'].apply(
         lambda x : ProteinAnalysis(x).gravy()
     )
     qt_df['peptideLength'] = qt_df['truePeptide'].apply(len)
     qt_df['peptideMass'] = qt_df['truePeptide'].apply(
         lambda pep : sum((RESIDUE_WEIGHTS[res] for res in pep))
     )
@@ -711,17 +816,17 @@
     figs = {}
     for results in config.benchmark_results:
         name = results['name']
         qt_df = qt_df.sort_values(by=f'{name}Score', ascending=False)
         qt_df.reset_index(drop=True, inplace=True)
         qt_df[f'{name}Rank'] = qt_df.index
         incorrect_df = qt_df[qt_df.apply(
-            lambda x : (
-                isinstance(x[f'{name}Peptide'], str) and
-                x[f'{name}Peptide'].replace('I', 'L') != x['truePeptide'].replace('I', 'L')
+            lambda x, na=name : (
+                isinstance(x[f'{na}Peptide'], str) and
+                x[f'{na}Peptide'].replace('I', 'L') != x['truePeptide'].replace('I', 'L')
             ),
             axis=1
         )].head(10)
         columns = [f'{name}Rank', f'{name}Peptide', f'{name}Stratum', 'truePeptide', 'trueStratum', f'{name}Score']
         fig = go.Figure(
         data=[
                 go.Table(
@@ -749,15 +854,23 @@
     Parameters
     ----------
     qt_df : pd.DataFrame
         The Query Table containing ground truth assignments joined to the user's assignments.
     config : ibench.config.Config
         The Config object used to run the experiment.
     """
-    strata = [x for x in qt_df['trueStratum'].unique() if x != TRANSPLICED_KEY]
+    # strata = [x for x in qt_df['trueStratum'].unique() if x != TRANSPLICED_KEY]
+    if config.allow_trans:
+        strata = sorted(
+            list(qt_df['trueStratum'].unique())
+        )
+    else:
+        strata = sorted(
+            [x for x in qt_df['trueStratum'].unique() if x != TRANSPLICED_KEY]
+        )
     roc_curves = {}
     max_tpr = 0.0
     for stratum in strata:
         roc_curves[stratum] = []
         for results in config.benchmark_results:
             roc_trace, tpr = create_roc_curve(qt_df, results, stratum)
             roc_curves[stratum].append(roc_trace)
```

### Comparing `ibench-1.2/ibench/query_table.py` & `ibench-2.0/ibench/query_table.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,67 @@
 """ Functions.
 """
+import multiprocessing as mp
+
 from Bio import SeqIO
 import pandas as pd
-from ibench.check_presence import find_cis_matched_splice_reactants, generate_pairs
+from ibench.check_presence import (
+    find_cis_matched_splice_reactants,
+    find_trans_matched,
+    generate_pairs,
+)
 from ibench.constants import (
     CANONICAL_KEY,
     CISSPLICED_KEY,
     ENGINE_SCORE_KEY,
     GT_SCAN_KEY,
     GT_SOURCE_KEY,
     LABEL_KEY,
     PEPTIDE_KEY,
     Q_VALUE_KEY,
+    SCAN_KEY,
     SOURCE_KEY,
+    TRANSPLICED_KEY,
 )
+from ibench.input.inspire import read_single_inspire_data
 from ibench.input.mascot import read_single_mascot_data
 from ibench.input.maxquant import read_single_mq_data
 from ibench.input.peaks import read_single_peaks_data
 from ibench.input.percolator import read_single_percolator_data
 
-def remap_to_proteome(peptide, proteome, max_intervening):
+def remap_to_canonical_proteome(peptide, proteome):
+    """ Function to remap a peptide to the canonical proteome
+    """
+    if not isinstance(peptide, str):
+        return None
+    for protein in proteome:
+        if peptide in protein:
+            return CANONICAL_KEY
+    return TRANSPLICED_KEY
+
+def remap_to_proteome(orig_peptide, proteome, max_intervening, allow_trans=False):
     """ Function to check for the presence of an identified peptide as either canonical
         or spliced in the input proteome.
     """
     accession_stratum = 'unknown'
-    splice_pairs = generate_pairs(peptide)
+    peptide = orig_peptide.replace('I', 'L')
+    splice_pairs = generate_pairs(peptide.replace('I', 'L'))
     for protein in proteome:
         if peptide in protein:
             return CANONICAL_KEY
+
+    for protein in proteome:
         if find_cis_matched_splice_reactants(protein, splice_pairs, max_intervening) is not None:
-            accession_stratum = CISSPLICED_KEY
+            return CISSPLICED_KEY
+    if allow_trans:
+        if len(proteome) == 1:
+            if find_trans_matched(proteome[0], splice_pairs, proteome):
+                return TRANSPLICED_KEY
+        else:
+            return TRANSPLICED_KEY
     return accession_stratum
 
 def read_data(location, name, engine, config, flag=''):
     """ Function to read results.
     """
     if engine=='percolator':
         target_df = read_single_percolator_data(
@@ -46,56 +74,96 @@
         target_df = read_single_mascot_data(
             location, 1.01, -1_000, hq_hits_only=False, filter_ptms=config.filter_ptms,
         )
     elif engine == 'maxquant':
         target_df = read_single_mq_data(
             location, -1_000, hq_hits_only=False, filter_ptms=config.filter_ptms,
         )
+    elif engine == 'inspire':
+        target_df = read_single_inspire_data(
+            location, 1.01,  -1_000, False,
+        )
     else:
         target_df = read_single_peaks_data(
             location, -1_000, hq_hits_only=False,  filter_ptms=config.filter_ptms,
         )
-
     if engine in ('peaks', 'maxquant'):
         if flag == 'Decoy':
             target_df = target_df[target_df[LABEL_KEY] == -1]
         else:
             target_df = target_df[target_df[LABEL_KEY] == 1]
 
+    if not target_df.shape[0]:
+        return None
+
     target_df = target_df.sort_values(by=ENGINE_SCORE_KEY, ascending=False)
     target_df = target_df.drop_duplicates(subset=['source', 'scan'])
     target_df = target_df.rename(
         columns={
             PEPTIDE_KEY: f'{name}{flag}Peptide',
             ENGINE_SCORE_KEY: f'{name}{flag}Score',
             Q_VALUE_KEY: f'{name}{flag}qValue',
-            'source': GT_SOURCE_KEY,
-            'scan': GT_SCAN_KEY,
         }
     )
-    if config.cisspliced_fraction > 0:
-        with open(config.proteome_loc, encoding='UTF-8') as prot_file:
-            modified_proteome = [
-                str(x.seq) for x in SeqIO.parse(prot_file, 'fasta')
-            ]
-        target_df[f'{name}{flag}Stratum'] = target_df[f'{name}{flag}Peptide'].apply(
-            lambda x : remap_to_proteome(x, modified_proteome, config.max_intervening)
-        )
-    else:
-        target_df[f'{name}{flag}Stratum'] = target_df[f'{name}{flag}Peptide'].apply(
-            lambda x : CANONICAL_KEY if isinstance(x, str) else None
-        )
 
-    output_columns = [
+    if target_df['source'].iloc[0].startswith('ibench') or target_df['source'].iloc[0].startswith('controllerType'):
+        target_df = target_df.rename(
+            columns={
+                'source': GT_SOURCE_KEY,
+                'scan': GT_SCAN_KEY,
+            }
+        )
+        output_columns = [
             GT_SOURCE_KEY,
             GT_SCAN_KEY,
             f'{name}{flag}Peptide',
             f'{name}{flag}Score',
             f'{name}{flag}Stratum',
         ]
+    else:
+        output_columns = [
+            SOURCE_KEY,
+            SCAN_KEY,
+            f'{name}{flag}Peptide',
+            f'{name}{flag}Score',
+            f'{name}{flag}Stratum',
+        ]
+
+    if config.cisspliced_fraction > 0 or config.discoverable_fraction == -1:
+        with open(f'{config.output_folder}/modified_proteome.fasta', encoding='UTF-8') as prot_file:
+            modified_proteome = [
+                str(x.seq).replace('I', 'L') for x in SeqIO.parse(prot_file, 'fasta')
+            ]
+
+        if flag == 'Decoy':
+            modified_proteome = [x[::-1] for x in modified_proteome]
+
+        target_df[f'{name}{flag}Stratum'] = target_df.groupby(f'{name}{flag}Peptide')[f'{name}{flag}Peptide'].transform(
+            lambda x : remap_to_proteome(x.iloc[0], modified_proteome, config.max_intervening, allow_trans=config.allow_trans)
+        )
+        if flag == 'Decoy':
+            
+            target_df[f'{name}{flag}Stratum'] = target_df[f'{name}{flag}Stratum'].apply(
+                lambda x : x if x != 'unknown' else CANONICAL_KEY
+            )
+    else:
+        
+        if config.allow_trans:
+            with open(f'{config.output_folder}/modified_proteome.fasta', encoding='UTF-8') as prot_file:
+                modified_proteome = [
+                    str(x.seq).replace('I', 'L') for x in SeqIO.parse(prot_file, 'fasta')
+                ]
+            target_df[f'{name}{flag}Stratum'] = target_df[f'{name}{flag}Peptide'].apply(
+                lambda x : remap_to_canonical_proteome(x, modified_proteome)
+            )
+        else:
+            target_df[f'{name}{flag}Stratum'] = target_df[f'{name}{flag}Peptide'].apply(
+                lambda x : CANONICAL_KEY if isinstance(x, str) else None
+            )
+
     if f'{name}qValue' in target_df.columns:
         output_columns.append(f'{name}{flag}qValue')
 
     target_df = target_df[output_columns]
 
     return target_df
 
@@ -106,66 +174,91 @@
     ----------
     config : ibench.config.Config
         The Config object used to control the experiment.
     """
     qt_df = pd.read_csv(
         f'{config.output_folder}/high_confidence.csv'
     )
+
+    if config.results_files is not None:
+        qt_df = qt_df[qt_df['gtSource'].apply(lambda x : x in config.results_files)]
+
     qt_df = qt_df.rename(columns={
         'peptide': 'truePeptide',
         'stratum': 'trueStratum',
     })
 
     scan_files = sorted(qt_df[SOURCE_KEY].unique().tolist())
     if config.single_scan_file:
         qt_df[GT_SOURCE_KEY] = f'ibenchGroundTruth_{config.identifier}'
     else:
         qt_df[GT_SOURCE_KEY] = qt_df[SOURCE_KEY].apply(
             lambda x : f'ibenchGroundTruth_{config.identifier}_{scan_files.index(x)}'
         )
 
-    for method in config.benchmark_results:
+
+    func_args = [
+        (method['resultsLocation'], method['name'], method['searchEngine'], config)
+         for method in config.benchmark_results
+    ]
+
+    with mp.Pool(processes=10) as pool:
+        mp_results = pool.starmap(read_data, func_args)
+
+
+    for method, target_df in zip(config.benchmark_results, mp_results):
         name = method['name']
-        target_df = read_data(method['resultsLocation'], name, method['searchEngine'], config)
+
+        if GT_SOURCE_KEY in target_df.columns:
+            merge_keys = [GT_SCAN_KEY]
+            target_df = target_df.drop(GT_SOURCE_KEY, axis=1)
+        else:
+            merge_keys = [SOURCE_KEY, SCAN_KEY]
 
         qt_df = pd.merge(
             qt_df,
             target_df,
             how='left',
-            on=[GT_SOURCE_KEY, GT_SCAN_KEY],
+            on=merge_keys,
         )
 
         if 'decoyLocation' in method:
             decoy_df = read_data(
                 method['decoyLocation'],
                 name,
                 method['searchEngine'],
                 config,
                 flag='Decoy',
             )
-
-            qt_df = pd.merge(
-                qt_df,
-                decoy_df,
-                how='left',
-                on=[GT_SOURCE_KEY, GT_SCAN_KEY],
-            )
+            if decoy_df is not None:
+                if GT_SOURCE_KEY in decoy_df.columns:
+                    merge_keys = [GT_SCAN_KEY]
+                    decoy_df = decoy_df.drop(GT_SOURCE_KEY, axis=1)
+                else:
+                    merge_keys = [SOURCE_KEY, SCAN_KEY]
+
+                qt_df = pd.merge(
+                    qt_df,
+                    decoy_df,
+                    how='left',
+                    on=merge_keys,
+                )
         elif method['searchEngine'] in ('peaks', 'maxquant'):
             decoy_df = read_data(
                 method['resultsLocation'],
                 name,
                 method['searchEngine'],
                 config,
                 flag='Decoy',
             )
-
-            qt_df = pd.merge(
-                qt_df,
-                decoy_df,
-                how='left',
-                on=[GT_SOURCE_KEY, GT_SCAN_KEY],
-            )
+            if decoy_df is not None:
+                qt_df = pd.merge(
+                    qt_df,
+                    decoy_df,
+                    how='left',
+                    on=merge_keys,
+                )
 
     qt_df.to_csv(
         f'{config.output_folder}/queryTable.csv',
         index=False,
     )
```

### Comparing `ibench-1.2/ibench/run.py` & `ibench-2.0/ibench/run.py`

 * *Files identical despite different names*

### Comparing `ibench-1.2/ibench/utils.py` & `ibench-2.0/ibench/utils.py`

 * *Files identical despite different names*

### Comparing `ibench-1.2/ibench/validate_assignments.py` & `ibench-2.0/ibench/validate_assignments.py`

 * *Files identical despite different names*

### Comparing `ibench-1.2/ibench.egg-info/PKG-INFO` & `ibench-2.0/ibench.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibench
-Version: 1.2
+Version: 2.0
 Summary: Benchmarking for mass spectrometry identifications.
 Author: John Cormican, Juliane Liepe
 Author-email: juliane.liepe@mpinat.mpg.de
 Project-URL: Homepage, https://github.com/QuantSysBio/iBench
 Project-URL: Tracker, https://github.com/QuantSysBio/iBench/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ibench-1.2/setup.py` & `ibench-2.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup
 
 setup(
     name='ibench',
-    version='1.2',
+    version='2.0',
     description='Benchmarking for mass spectrometry identifications.',
     author='John Cormican, Juliane Liepe',
     author_email='juliane.liepe@mpinat.mpg.de',
     packages=[
         'ibench',
         'ibench.input',
     ],
@@ -21,25 +21,25 @@
         'console_scripts': [
             'ibench=ibench.run:main'
         ]
     },
     python_requires='>=3.8',
     install_requires=[
         'biopython==1.79',
-        'certifi==2021.10.8',
+        'certifi==2022.12.7',
         'lxml==4.9.1',
-        'numpy==1.22.3',
-        'pandas==1.4.2',
-        'plotly==5.8.0',
-        'pyopenms==2.7.0',
-        'pyteomics==4.5.3',
+        'numpy==1.19.5',
+        'pandas==1.4.3',
+        'plotly==5.10.0',
+        'pyopenms==2.6.0',
+        'pyteomics==4.5.4',
         'python-dateutil==2.8.2',
-        'pytz==2022.1',
+        'pytz==2022.2.1',
         'PyYAML==6.0',
-        'six==1.16.0',
+        'six==1.15.0',
         'tenacity==8.0.1',
     ],
     project_urls={
         'Homepage': 'https://github.com/QuantSysBio/iBench',
         'Tracker': 'https://github.com/QuantSysBio/iBench/issues',
     },
 )
```


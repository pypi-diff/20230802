# Comparing `tmp/inspirems-1.4.tar.gz` & `tmp/inspirems-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inspirems-1.4.tar", last modified: Wed Dec 14 14:23:16 2022, max compression
+gzip compressed data, was "inspirems-1.5.tar", last modified: Wed Aug  2 13:52:10 2023, max compression
```

## Comparing `inspirems-1.4.tar` & `inspirems-1.5.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxr-xr-x   0 john.cormican (676547) Dep16040 (116040)        0 2022-12-14 14:23:16.195552 inspirems-1.4/
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    18092 2022-08-29 08:28:41.000000 inspirems-1.4/LICENSE
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    14190 2022-12-14 14:23:16.195552 inspirems-1.4/PKG-INFO
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    13779 2022-12-14 12:53:42.000000 inspirems-1.4/README.md
-drwxr-xr-x   0 john.cormican (676547) Dep16040 (116040)        0 2022-12-14 14:23:16.191552 inspirems-1.4/inspire/
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)       85 2022-12-14 12:06:44.000000 inspirems-1.4/inspire/__init__.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     6188 2022-12-14 13:02:52.000000 inspirems-1.4/inspire/accession.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     2601 2022-10-24 12:42:59.000000 inspirems-1.4/inspire/basic_features.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     6174 2022-12-14 13:27:22.000000 inspirems-1.4/inspire/calibration.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    11667 2022-12-14 12:06:46.000000 inspirems-1.4/inspire/config.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     9565 2022-12-14 12:53:42.000000 inspirems-1.4/inspire/constants.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     2209 2022-10-24 12:42:59.000000 inspirems-1.4/inspire/download.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    22915 2022-12-14 12:51:09.000000 inspirems-1.4/inspire/feature_creation.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    21543 2022-12-14 12:06:46.000000 inspirems-1.4/inspire/feature_selection.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     9744 2022-10-24 12:42:59.000000 inspirems-1.4/inspire/figures.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     3153 2022-12-14 12:06:46.000000 inspirems-1.4/inspire/get_spectral_angle.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     4903 2022-12-14 12:06:44.000000 inspirems-1.4/inspire/html_template.py
-drwxr-xr-x   0 john.cormican (676547) Dep16040 (116040)        0 2022-12-14 14:23:16.191552 inspirems-1.4/inspire/input/
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)        0 2022-08-29 08:28:41.000000 inspirems-1.4/inspire/input/__init__.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    19335 2022-12-14 12:06:46.000000 inspirems-1.4/inspire/input/mascot.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     7296 2022-10-24 12:42:59.000000 inspirems-1.4/inspire/input/maxquant.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     3173 2022-12-14 12:06:46.000000 inspirems-1.4/inspire/input/mgf.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     2854 2022-12-14 12:06:44.000000 inspirems-1.4/inspire/input/mhcpan.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     9001 2022-12-14 12:06:44.000000 inspirems-1.4/inspire/input/msp.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     2277 2022-11-30 16:09:48.000000 inspirems-1.4/inspire/input/mzml.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     9945 2022-12-14 12:06:44.000000 inspirems-1.4/inspire/input/peaks.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     2640 2022-12-14 12:06:46.000000 inspirems-1.4/inspire/input/search_results.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     4431 2022-11-27 21:50:28.000000 inspirems-1.4/inspire/mz_match.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    18747 2022-12-14 12:06:44.000000 inspirems-1.4/inspire/plot_spectra.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     3375 2022-12-14 12:06:46.000000 inspirems-1.4/inspire/predict_spectra.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     9641 2022-11-30 16:09:48.000000 inspirems-1.4/inspire/prepare.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    16865 2022-10-24 12:42:59.000000 inspirems-1.4/inspire/prosit.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    21100 2022-10-24 12:42:59.000000 inspirems-1.4/inspire/prosit_delta.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    16173 2022-12-14 12:06:44.000000 inspirems-1.4/inspire/report.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     8074 2022-12-14 12:51:09.000000 inspirems-1.4/inspire/rescore.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     3442 2022-12-14 12:06:46.000000 inspirems-1.4/inspire/retention_time.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     5241 2022-12-14 12:51:09.000000 inspirems-1.4/inspire/run.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    23715 2022-12-14 12:06:44.000000 inspirems-1.4/inspire/spectral_features.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    13544 2022-12-14 12:06:46.000000 inspirems-1.4/inspire/utils.py
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    12316 2022-12-14 12:51:09.000000 inspirems-1.4/inspire/validate.py
-drwxr-xr-x   0 john.cormican (676547) Dep16040 (116040)        0 2022-12-14 14:23:16.195552 inspirems-1.4/inspirems.egg-info/
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    14190 2022-12-14 14:23:16.000000 inspirems-1.4/inspirems.egg-info/PKG-INFO
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     1001 2022-12-14 14:23:16.000000 inspirems-1.4/inspirems.egg-info/SOURCES.txt
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)        1 2022-12-14 14:23:16.000000 inspirems-1.4/inspirems.egg-info/dependency_links.txt
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)       45 2022-12-14 14:23:16.000000 inspirems-1.4/inspirems.egg-info/entry_points.txt
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     1345 2022-12-14 14:23:16.000000 inspirems-1.4/inspirems.egg-info/requires.txt
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)        8 2022-12-14 14:23:16.000000 inspirems-1.4/inspirems.egg-info/top_level.txt
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)       38 2022-12-14 14:23:16.195552 inspirems-1.4/setup.cfg
--rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     2988 2022-12-14 12:06:44.000000 inspirems-1.4/setup.py
+drwxr-sr-x   0 john.cormican (676547) Dep16040 (116040)        0 2023-08-02 13:52:10.154667 inspirems-1.5/
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    18092 2023-03-10 10:09:05.000000 inspirems-1.5/LICENSE
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    14506 2023-08-02 13:52:10.154667 inspirems-1.5/PKG-INFO
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    14072 2023-03-10 10:09:05.000000 inspirems-1.5/README.md
+drwxr-sr-x   0 john.cormican (676547) Dep16040 (116040)        0 2023-08-02 13:52:10.122667 inspirems-1.5/inspire/
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)       85 2023-03-10 10:09:06.000000 inspirems-1.5/inspire/__init__.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     6083 2023-08-02 11:57:41.000000 inspirems-1.5/inspire/accession.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     2601 2023-03-10 10:09:06.000000 inspirems-1.5/inspire/basic_features.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     5991 2023-03-30 14:07:42.000000 inspirems-1.5/inspire/calibration.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    12281 2023-08-02 11:57:41.000000 inspirems-1.5/inspire/config.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     9656 2023-03-30 14:09:38.000000 inspirems-1.5/inspire/constants.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     2209 2023-03-10 10:09:06.000000 inspirems-1.5/inspire/download.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    22169 2023-08-02 11:57:41.000000 inspirems-1.5/inspire/feature_creation.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    22515 2023-08-02 11:57:41.000000 inspirems-1.5/inspire/feature_selection.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     9744 2023-03-10 10:09:06.000000 inspirems-1.5/inspire/figures.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     3086 2023-08-02 11:57:41.000000 inspirems-1.5/inspire/get_spectral_angle.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     4903 2023-03-10 10:09:06.000000 inspirems-1.5/inspire/html_template.py
+drwxr-sr-x   0 john.cormican (676547) Dep16040 (116040)        0 2023-08-02 13:52:10.138667 inspirems-1.5/inspire/input/
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)        0 2023-03-10 10:09:06.000000 inspirems-1.5/inspire/input/__init__.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    19250 2023-03-24 08:55:19.000000 inspirems-1.5/inspire/input/mascot.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     7195 2023-03-24 08:55:22.000000 inspirems-1.5/inspire/input/maxquant.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     3173 2023-03-10 10:09:06.000000 inspirems-1.5/inspire/input/mgf.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     2854 2023-03-10 10:09:06.000000 inspirems-1.5/inspire/input/mhcpan.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    10681 2023-08-02 11:57:41.000000 inspirems-1.5/inspire/input/msfragger.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     9001 2023-03-10 10:09:06.000000 inspirems-1.5/inspire/input/msp.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     2592 2023-03-29 08:45:35.000000 inspirems-1.5/inspire/input/mzml.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     9883 2023-03-24 08:55:56.000000 inspirems-1.5/inspire/input/peaks.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     3677 2023-03-30 14:05:30.000000 inspirems-1.5/inspire/input/search_results.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     4431 2023-04-25 11:19:32.000000 inspirems-1.5/inspire/mz_match.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    35535 2023-08-02 11:57:41.000000 inspirems-1.5/inspire/plot_isobars.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    33463 2023-08-02 11:57:41.000000 inspirems-1.5/inspire/plot_spectra.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     3816 2023-08-02 11:57:41.000000 inspirems-1.5/inspire/predict_spectra.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     9641 2023-03-10 10:09:06.000000 inspirems-1.5/inspire/prepare.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    16865 2023-03-10 10:09:06.000000 inspirems-1.5/inspire/prosit.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    21100 2023-03-10 10:09:06.000000 inspirems-1.5/inspire/prosit_delta.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    16174 2023-08-02 11:57:41.000000 inspirems-1.5/inspire/report.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     9244 2023-08-02 11:57:41.000000 inspirems-1.5/inspire/rescore.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     4541 2023-08-02 11:57:41.000000 inspirems-1.5/inspire/retention_time.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     5780 2023-08-02 11:57:41.000000 inspirems-1.5/inspire/run.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    23857 2023-08-02 11:57:41.000000 inspirems-1.5/inspire/spectral_features.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    15866 2023-08-02 11:57:41.000000 inspirems-1.5/inspire/utils.py
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    14398 2023-08-02 11:57:41.000000 inspirems-1.5/inspire/validate.py
+drwxr-sr-x   0 john.cormican (676547) Dep16040 (116040)        0 2023-08-02 13:52:10.150667 inspirems-1.5/inspirems.egg-info/
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)    14506 2023-08-02 13:52:10.000000 inspirems-1.5/inspirems.egg-info/PKG-INFO
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     1052 2023-08-02 13:52:10.000000 inspirems-1.5/inspirems.egg-info/SOURCES.txt
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)        1 2023-08-02 13:52:10.000000 inspirems-1.5/inspirems.egg-info/dependency_links.txt
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)       45 2023-08-02 13:52:10.000000 inspirems-1.5/inspirems.egg-info/entry_points.txt
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     1355 2023-08-02 13:52:10.000000 inspirems-1.5/inspirems.egg-info/requires.txt
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)        8 2023-08-02 13:52:10.000000 inspirems-1.5/inspirems.egg-info/top_level.txt
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)       38 2023-08-02 13:52:10.154667 inspirems-1.5/setup.cfg
+-rw-r--r--   0 john.cormican (676547) Dep16040 (116040)     3029 2023-08-02 11:57:41.000000 inspirems-1.5/setup.py
```

### Comparing `inspirems-1.4/LICENSE` & `inspirems-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `inspirems-1.4/PKG-INFO` & `inspirems-1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: inspirems
-Version: 1.4
+Version: 1.5
 Summary: Helping to integrate Spectral Predictors and Rescoring.
 Author: John Cormican, Juliane Liepe
 Author-email: juliane.liepe@mpinat.mpg.de
 Project-URL: Homepage, https://github.com/QuantSysBio/inSPIRE
 Project-URL: Tracker, https://github.com/QuantSysBio/inSPIRE/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: ms2pip
 License-File: LICENSE
 
 # inSPIRE
 
 <img src="https://raw.githubusercontent.com/QuantSysBio/inSPIRE/master/img/inSPIRE-logo.png" alt="drawing" width="200"/>
 
 <i>in silico</i> Spectral Predictor Informed REscoring
@@ -48,14 +49,20 @@
 
 4) To check your installation, run the following command (it is normal for this call to hang for a few seconds on first execution)
 
 ```
 inspire -h
 ```
 
+5) (Optional) If you wish to use Percolator for rescoring rather than Mokapot you will need to install it separately. On Linux, Percolator can be installed via conda with the command below. Otherwise see https://github.com/percolator/percolator.
+
+```
+conda install -c bioconda percolator
+```
+
 Once you have successfully installed inSPIRE you should run it specifying your pipeline and a config file. The core execution of inSPIRE will take the form:
 
 ```
 inspire --config_file path-to-config-file --pipeline pipeline-to-execute
 ```
 
 where the config file is a yaml file specifying details of the inSPIRE execution and the pipeline is one of the options described below.
```

### Comparing `inspirems-1.4/README.md` & `inspirems-1.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,20 @@
 
 4) To check your installation, run the following command (it is normal for this call to hang for a few seconds on first execution)
 
 ```
 inspire -h
 ```
 
+5) (Optional) If you wish to use Percolator for rescoring rather than Mokapot you will need to install it separately. On Linux, Percolator can be installed via conda with the command below. Otherwise see https://github.com/percolator/percolator.
+
+```
+conda install -c bioconda percolator
+```
+
 Once you have successfully installed inSPIRE you should run it specifying your pipeline and a config file. The core execution of inSPIRE will take the form:
 
 ```
 inspire --config_file path-to-config-file --pipeline pipeline-to-execute
 ```
 
 where the config file is a yaml file specifying details of the inSPIRE execution and the pipeline is one of the options described below.
```

### Comparing `inspirems-1.4/inspire/accession.py` & `inspirems-1.5/inspire/accession.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 from inspire.constants import (
     ACCESSION_STRATUM_KEY,
     ACCESSION_KEY,
     LABEL_KEY,
     PEPTIDE_KEY,
 )
 
+ACCESSION_SPLITTERS = {
+    'mascot': ',',
+    'msfragger': ',',
+    'maxquant': ';',
+    'peaks': ':',
+}
 
 def get_accession_group(accession, search_engine, accession_hierarchy, accession_groups):
     """ Function to get the accession group from the accession of a peptide.
 
     Parameters
     ----------
     accession : str
@@ -23,21 +29,16 @@
         The search engine which provided the data.
     accession_hierarchy : list of str
         The order in which groups should be assigned in case of multi-mappers.
     accession_groups : dict
         A dictionary of mapping accession groups to the flag that will be seen
         in the accession.
     """
-    if search_engine == 'peaks':
-        splitter = ':'
-    elif search_engine == 'maxquant':
-        splitter = ';'
-    elif search_engine == 'mascot':
-        splitter = ','
-    else:
+    splitter = ACCESSION_SPLITTERS.get(search_engine)
+    if splitter is None:
         raise ValueError(f'Unrecognised Search Engine: {search_engine}')
     all_possible_accessions = accession.split(splitter)
     assignment = None
     for individiual_accession in all_possible_accessions:
         found = False
         for idx, acc in enumerate(accession_hierarchy):
             if accession_groups[acc] in individiual_accession:
@@ -60,28 +61,24 @@
         The search engine from which the results were generated.
 
     Returns
     -------
     assignment : int
         The accession group index as defined by the config.accession_hierarchy.
     """
-    if search_engine == 'peaks':
-        splitter = ':'
-    elif search_engine == 'maxquant':
-        splitter = ';'
-    elif search_engine == 'mascot':
-        splitter = ','
-    else:
+    splitter = ACCESSION_SPLITTERS.get(search_engine)
+    if splitter is None:
         raise ValueError(f'Unrecognised Search Engine: {search_engine}')
+
     all_possible_accessions = accession.split(splitter)
     assignment = 0
     for individiual_accession in all_possible_accessions:
-        if 'PCP' in individiual_accession:
+        if 'PCP_' in individiual_accession:
             return 0
-        if 'PSP' in individiual_accession:
+        if 'PSP_' in individiual_accession:
             assignment = 1
     return assignment
 
 def validate_accession_stratum(df_row, proteome, rev_proteome, config):
     """ Function to validate the accession of a non-canonical PSM by checking for the
         sequence in the standard proteome.
```

### Comparing `inspirems-1.4/inspire/basic_features.py` & `inspirems-1.5/inspire/basic_features.py`

 * *Files identical despite different names*

### Comparing `inspirems-1.4/inspire/calibration.py` & `inspirems-1.5/inspire/calibration.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,53 +31,49 @@
 from inspire.utils import (
     check_bad_mods,
     get_ox_flag,
     get_cam_flag,
     remove_source_suffixes,
 )
 
-COLLISION_ENERGY_RANGE = [20 + i for i in range(21)]
+COLLISION_ENERGY_RANGE = list(range(20, 41))
 
 def _get_top_hits(config):
     """ Function to extract the top scoring hits for collision energy calibration.
 
     Parameters
     ----------
     config : inspire.config.Config
         The Config object for the experiment.
     """
     target_df, mods_df = generic_read_df(config, save_dfs=False, overwrite_reduce=True)
 
-    unknown_mods = mods_df[PTM_ID_KEY].tolist()
-    # [
-    #     (mods_df[PTM_NAME_KEY] != 'Carbamidomethylation') &
-    #     ((mods_df[PTM_NAME_KEY] != 'Carbamidomethyl (C)'))
-    # ][PTM_ID_KEY].tolist()
+    unknown_mods = mods_df[
+        (mods_df[PTM_NAME_KEY] != 'Oxidation (M)') &
+        ((mods_df[PTM_NAME_KEY] != 'Carbamidomethyl (C)'))
+    ][PTM_ID_KEY].tolist()
     unknown_mods = {str(x) for x in unknown_mods}
 
     target_df['unknownModifications'] = target_df[PTM_SEQ_KEY].apply(
         lambda x : check_bad_mods(x, unknown_mods)
     )
     target_df = target_df[~target_df['unknownModifications']]
 
     if ACCESSION_STRATUM_KEY in target_df.columns:
         target_df = target_df[target_df[ACCESSION_STRATUM_KEY] == 0]
 
-    target_df = target_df[target_df[PTM_SEQ_KEY].isna()]
     top_5_pct_cut = target_df[ENGINE_SCORE_KEY].quantile(0.95)
 
     target_df = target_df[
         (target_df[ENGINE_SCORE_KEY] > top_5_pct_cut) &
-        (target_df[LABEL_KEY] == 1)
+        (target_df[LABEL_KEY] == 1) #move this up
     ]
 
     if target_df.shape[0] > 1000:
-        target_df = target_df.sort_values(by=ENGINE_SCORE_KEY)
-        target_df = target_df.reset_index(drop=True)
-        target_df = target_df[target_df.index < 1000]
+        target_df = target_df.nlargest(1000, columns=[ENGINE_SCORE_KEY])
 
     return target_df, mods_df
 
 def prepare_calibration(config):
     """ Function to generate Prosit input for collision energy calibration.
 
     Parameters
@@ -93,49 +89,50 @@
             mods_df,
             config,
             collision_energy,
             'calibrationInput',
             overwrite=idx==0,
         )
 
+    return target_df, mods_df
+
 def calibrate(config):
     """ Function to calibrate the optimal collision energy for Prosit input.
 
     Parameters
     ----------
     config : inspire.config.Config
         The Config object for the experiment.
     """
     print(
         OKCYAN_TEXT +
         '\tSelecting top hits...' +
         ENDC_TEXT
     )
-    prepare_calibration(config)
+    target_df, mods_df = prepare_calibration(config)
     predict_spectra(config, 'calibrate')
 
-    target_df, mods_df = _get_top_hits(config)
     prosit_df = msp_to_df(
         f'{config.output_folder}/calibrationPredictions.msp', 'prosit', None,
     )
 
-    if config.combined_scans_file is not None:
-        scan_files = [remove_source_suffixes(config.combined_scans_file)]
-    else:
-        scan_files = target_df[SOURCE_KEY].unique().tolist()
-
     ox_flag = get_ox_flag(mods_df)
     cam_flag = get_cam_flag(mods_df)
 
     mods_dict = {
         0: 0.0,
         int(cam_flag): KNOWN_PTM_WEIGHTS['Carbamidomethyl (C)'],
         int(ox_flag): KNOWN_PTM_WEIGHTS['Oxidation (M)']
     }
 
+    if config.combined_scans_file is not None:
+        scan_files = [remove_source_suffixes(config.combined_scans_file)]
+    else:
+        scan_files = target_df[SOURCE_KEY].unique().tolist()
+
     scan_dfs = []
     for scan_file in scan_files:
         if config.combined_scans_file is not None:
             filtered_search_df = target_df
         else:
             filtered_search_df = target_df[target_df[SOURCE_KEY] == scan_file]
 
@@ -150,14 +147,15 @@
                 f'{config.scans_folder}/{scan_file}.{config.scans_format}',
                 set(scans.tolist()),
                 config.scan_title_format,
                 config.source_files,
                 combined_source_file=config.combined_scans_file is not None,
             )
         scan_dfs.append(scan_df.drop_duplicates(subset=[SOURCE_KEY, SCAN_KEY]))
+
     combined_scan_df = pd.concat(scan_dfs)
     print(
         OKCYAN_TEXT +
         '\t\tCombining all spectral data...' +
         ENDC_TEXT
     )
     combined_df = combine_spectral_data(
```

### Comparing `inspirems-1.4/inspire/config.py` & `inspirems-1.5/inspire/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """ Definition of Config class.
 """
+import glob
 import os
 from pathlib import Path
 
 import yaml
 
 from inspire.utils import read_distiller_log
 
 ALL_CONFIG_KEYS = [
     'accessionFormat',
     'collisionEnergy',
+    'contaminantData',
     'combinedScansFile',
     'deltaMethod',
     'distillerLog',
     'dropUnknownPTMs',
     'excludeFeatures',
     'experimentTitle',
     'falseDiscoveryRate',
@@ -25,26 +27,29 @@
     'mzAccuracy',
     'mzUnits',
     'nCores',
     'outputFolder',
     'proteome',
     'reduce',
     'rescoreMethod',
+    'resultsExport',
     'reuseInput',
+    'rtPerFile',
     'scansFolder',
     'scansFormat',
     'scanTitleFormat',
     'searchResults',
     'searchEngine',
     'sourceFileName',
     'silentExecution',
     'spectralAngleDfs',
     'spectralPredictor',
     'useAccessionStrata',
     'useBindingAffinity',
+    'useIrtDelta',
     'useMinimalFeatures',
 ]
 
 class Config:
     """ Holder for configuration of the inspire pipeline.
     """
     def __init__(self, config_file):
@@ -82,21 +87,30 @@
 
 
     def _load_data(self, config_dict):
         """ Function to load data.
         """
         # Required:
         self.experiment_title = config_dict['experimentTitle']
-        self.search_results = config_dict['searchResults']
+        if isinstance(config_dict['searchResults'], list):
+            self.search_results = []
+            for result_group in config_dict['searchResults']:
+                self.search_results.extend(glob.glob(result_group))
+        else:
+            self.search_results = config_dict['searchResults']
+
         self.search_engine = config_dict['searchEngine']
         self.output_folder = config_dict['outputFolder']
         self.scans_folder = config_dict['scansFolder']
         self.scans_format = config_dict['scansFormat']
 
         # Recommended:
+        self.results_export = config_dict.get('resultsExport', 'psm')
+        self.use_irt_diff = config_dict.get('useIrtDelta', True)
+        self.delta_rt_per_file = config_dict.get('rtPerFile', True)
         self.n_cores = config_dict.get('nCores', 1)
         self.collision_energy = config_dict.get('collisionEnergy', None)
         self.mz_accuracy = config_dict.get('mzAccuracy', 0.02)
         self.mz_units = config_dict.get('mzUnits', 'Da')
         self.fixed_modifications = config_dict.get('fixedModifications', None)
         self.spectral_predictor = config_dict.get('spectralPredictor', 'prosit')
         if self.spectral_predictor == 'prosit':
@@ -140,19 +154,20 @@
 
 
         # Accession Groups
         self.accession_groups = config_dict.get('accessionGroups')
         self.accession_hierarchy = config_dict.get('accessionHierarchy')
         self.accession_format = config_dict.get('accessionFormat')
         if self.accession_format == 'invitroSPI' and self.accession_hierarchy is None:
-            self.accession_hierarchy = ['nonspliced', 'cisspliced', 'transspliced']
+            self.accession_hierarchy = ['nonspliced', 'spliced']
 
         self.use_accession_stratum = config_dict.get('useAccessionStrata', False)
         self.proteome = config_dict.get('proteome')
         self.raw_file_groups = config_dict.get('rawFileGroupings')
+        self.contaminant_data = config_dict.get('contaminantData')
 
     def __str__(self):
         print_string = f'inSPIRE Settings for Experiment {self.experiment_title}:<br>'
         print_string += f"""<table style="width:40%">
         <tr>
             <th>Config</th>
             <th>Setting</th>
@@ -280,18 +295,18 @@
         #     print_string += f'Original Source Files:\t{", ".join(self.source_files)}\n'
 
         return print_string
 
     def validate(self):
         """ Function to validate config settings.
         """
-        if self.search_engine not in ('mascot', 'maxquant', 'peaks'):
+        if self.search_engine not in ('mascot', 'maxquant', 'peaks', 'msfragger'):
             raise ValueError(
                 f'Unsupported Search Engine: "{self.search_engine}". Supported ' +
-                'engines are "mascot", "peaks", and "maxquant".'
+                'engines are "mascot", "peaks", "msfragger", and "maxquant".'
             )
 
         if self.scans_format not in ('mgf', 'mzML'):
             raise ValueError(
                 f'Unsupported Scans Format: "{self.scans_format}". Supported ' +
                 'formats are "mgf" and "mzML".'
             )
```

### Comparing `inspirems-1.4/inspire/constants.py` & `inspirems-1.5/inspire/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -235,14 +235,15 @@
     'W': 186.079313,
     'Y': 163.06332,
     'V': 99.068414,
 }
 
 KNOWN_PTM_WEIGHTS = {
     'Deamidated (N)': 0.984016,
+    'Deamidated (Q)': 0.984016,
     'Deamidated (NQ)': 0.984016,
     'Deamidation (NQ)': 0.984016,
     'Deamidation (N)': 0.984016,
     'Oxidation (M)': 15.994915,
     'Acetyl (N-term)': 42.010565,
     'Acetylation (N-term)': 42.010565,
     'Acetyl (Protein N-term)': 42.010565,
@@ -252,14 +253,15 @@
     'Phosphorylation (STY)': 79.966331,
     'Carbamidomethyl (C)': 57.021464,
     'Carbamidomethylation': 57.021464,
 }
 
 KNOWN_PTM_LOC = {
     'Deamidated (N)': 'N',
+    'Deamidated (Q)': 'Q',
     'Deamidated (NQ)': 'NQ',
     'Deamidation (NQ)': 'NQ',
     'Deamidation (N)': 'N',
     'Oxidation (M)': 'M',
     'Acetyl (N-term)': 'N-term',
     'Phospho (Y)': 'Y',
     'Phospho (ST)': 'ST',
@@ -267,14 +269,15 @@
     'Phosphorylation (STY)': 'STY',
     'Carbamidomethyl (C)': 'C',
     'Carbamidomethylation': 'C',
 }
 
 MS2PIP_NAME_MAPPINGS = {
     'Deamidated (N)': 'Deamidation',
+    'Deamidated (Q)': 'Deamidation',
     'Deamidated (NQ)': 'Deamidation',
     'Deamidation (NQ)': 'Deamidation',
     'Deamidation (N)': 'Deamidation',
     'Oxidation (M)': 'Oxidation',
     'Acetyl (N-term)': 'Acetyl',
     'Phospho (Y)': 'Phospho',
     'Phospho (ST)': 'Phospho',
@@ -305,16 +308,16 @@
     'pkaDiff',
     'polaDiff',
     'BLOSUM6.1',
 ]
 
 MINIMAL_FEATURE_SET = [
     SPECTRAL_ANGLE_KEY,
-    'matchedCoverage',
     'deltaRT',
+    SPEARMAN_KEY,
 ]
 
 # Constants used by deltapro predictor.
 
 RESIDUE_PROPERTIES = {
     'A': {
         'polarity': 0,
```

### Comparing `inspirems-1.4/inspire/download.py` & `inspirems-1.5/inspire/download.py`

 * *Files identical despite different names*

### Comparing `inspirems-1.4/inspire/feature_creation.py` & `inspirems-1.5/inspire/feature_creation.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,23 +2,21 @@
 """
 from math import log10
 import multiprocessing
 import os
 
 import pandas as pd
 
-from inspire.accession import process_accession_groups
 from inspire.basic_features import create_basic_features
 from inspire.constants import(
     ACCESSION_STRATUM_KEY,
     ACCESSION_KEY,
     BASIC_FEATURES,
     CHARGE_KEY,
     ENDC_TEXT,
-    ENGINE_SCORE_KEY,
     LABEL_KEY,
     MINIMAL_FEATURE_SET,
     OKCYAN_TEXT,
     IN_ACCESSION_KEY,
     PEPTIDE_KEY,
     PSM_ID_KEY,
     PERC_SCAN_ID,
@@ -38,14 +36,15 @@
 from inspire.input.msp import msp_to_df
 from inspire.input.mzml import process_mzml_file
 from inspire.input.search_results import generic_read_df
 from inspire.prepare import create_prosit_mod_seq
 from inspire.retention_time import add_delta_irt
 from inspire.spectral_features import SPECTRAL_FEATURES, DELTA_FEATURES, create_spectral_features
 from inspire.utils import (
+    accession_informed_filter,
     check_bad_mods,
     get_ox_flag,
     modify_sequence_for_skyline,
     remove_source_suffixes,
     permute_seq,
     permute_ptms,
 )
@@ -140,26 +139,29 @@
     """
     psm_id_key = PSM_ID_KEY[config.rescore_method]
     if config.minimal_features:
         use_cols = [
             psm_id_key,
             LABEL_KEY,
             PERC_SCAN_ID
-        ] + BASIC_FEATURES + MINIMAL_FEATURE_SET
+        ] + BASIC_FEATURES + MINIMAL_FEATURE_SET + ['matchedCoverage']
     else:
         use_cols = [
             psm_id_key,
             LABEL_KEY,
             PERC_SCAN_ID,
         ] + BASIC_FEATURES + SPECTRAL_FEATURES
 
         if config.delta_method != 'ignore':
             use_cols += DELTA_FEATURES
 
-        use_cols += ['deltaRT']
+        use_cols.append('deltaRT')
+
+    if not config.delta_rt_per_file:
+        use_cols.append('iRT')
 
     if config.use_binding_affinity == 'asFeature':
         use_cols += ['bindingAffinity']
 
     if config.combined_scans_file is not None:
         if config.source_files is not None:
             scan_files = [remove_source_suffixes(x) for x in config.source_files]
@@ -248,14 +250,20 @@
             f'{config.output_folder}/input_all_features.tab', 'w', encoding='UTF-8'
         ) as out_file:
             for tab_file in sorted(results):
                 with open(tab_file, 'r', encoding='UTF-8') as in_file:
                     for line in in_file:
                         out_file.write(line)
                 os.remove(tab_file)
+
+    if not config.delta_rt_per_file:
+        all_features_df = pd.read_csv(f'{config.output_folder}/input_all_features.tab', sep='\t')
+        all_features_df = add_delta_irt(all_features_df, config, 'combined')
+        all_features_df.to_csv(f'{config.output_folder}/input_all_features.tab', sep='\t', index=False)
+
     print(
         OKCYAN_TEXT + '\t\t\tFull input DataFrame written to csv.' + ENDC_TEXT
     )
 
 
 def process_single_file(
         search_df, mods_df, prosit_df, config, file_idx, scan_file, max_scan, in_parallel
@@ -418,15 +426,18 @@
         return None
 
     combined_df = create_spectral_features(combined_df, mods_df, config)
     combined_df = combined_df.sort_values(by='spectralAngle', ascending=False)
     if isinstance(config.collision_energy, list):
         combined_df = combined_df.drop_duplicates(subset=['source', 'scan', 'peptide'])
 
-    combined_df = add_delta_irt(combined_df, config, scan_file)
+    if config.delta_rt_per_file:
+        combined_df = add_delta_irt(combined_df, config, scan_file)
+    else:
+        combined_df['deltaRT'] = 0
 
     print(
         OKCYAN_TEXT + '\t\t\tCreated Spectral and Delta RT Features.' + ENDC_TEXT
     )
     if config.search_engine != 'mascot':
         combined_df[PERC_SCAN_ID] = combined_df[SCAN_KEY].apply(
             lambda x, f_id=file_idx : f_id * max_scan  + x
@@ -512,15 +523,15 @@
     """
     feature_df = create_basic_features(search_df, mods_df)
 
     if config.use_binding_affinity == 'asFeature':
         mhc_pan_df = read_mhcpan_output(f'{config.output_folder}/mhcpan')
         mhc_pan_df = mhc_pan_df.rename(columns={
             'Peptide': PEPTIDE_KEY,
-            'Aff(nM)': 'bindingAffinity'
+            'Aff(nM)': 'bindingAffinity',
         })
         mhc_pan_df['bindingAffinity'] = mhc_pan_df['bindingAffinity'].apply(log10)
         mhc_pan_df = mhc_pan_df[[PEPTIDE_KEY, 'bindingAffinity']]
         feature_df = pd.merge(
             feature_df,
             mhc_pan_df,
             on=PEPTIDE_KEY,
@@ -549,22 +560,14 @@
 
     write_with_spectral_features(
         feature_df,
         mods_df,
         config,
     )
 
-def get_mod_score(df_row):
-    """ Helper function to compare different accession strata.
-    """
-    if df_row[ACCESSION_STRATUM_KEY] == 0:
-        return df_row[ENGINE_SCORE_KEY]
-    return 0.7*df_row[ENGINE_SCORE_KEY]
-
-
 def process_unknown_modifications(target_df, mods_df, config):
     """ Function to handle modifications which are unknown to the Prosit spectral predictor
         (as well as unmodified cysteines).
 
     Parameters
     ----------
     Parameters
@@ -589,39 +592,15 @@
         ][PTM_ID_KEY].tolist()
         unknown_mods = {str(x) for x in unknown_mods}
         target_df['unknownModifications'] = target_df[PTM_SEQ_KEY].apply(
             lambda x : check_bad_mods(x, unknown_mods)
         )
         count_before_drop = target_df.shape[0]
         if config.use_accession_stratum:
-            target_df['modEngineScore'] = target_df[
-                [ENGINE_SCORE_KEY, ACCESSION_STRATUM_KEY]
-            ].apply(get_mod_score, axis=1)
-            target_df['maxModScore'] = target_df.groupby(
-                [SOURCE_KEY, SCAN_KEY]
-            )['modEngineScore'].transform(max)
-
-            unknown_df = target_df[
-                (target_df['unknownModifications']) &
-                (target_df['maxModScore'] == target_df['modEngineScore'])
-            ]
-            unknown_df = unknown_df[[SOURCE_KEY, SCAN_KEY]].drop_duplicates()
-            unknown_df['drop'] = 'yes'
-            target_df = target_df[
-                ~target_df['unknownModifications']
-            ].drop(['modEngineScore', 'maxModScore', 'unknownModifications'], axis=1)
-
-            target_df = pd.merge(
-                target_df,
-                unknown_df,
-                how='left',
-                on=[SOURCE_KEY, SCAN_KEY]
-            )
-            target_df = target_df[target_df['drop'] != 'yes']
-            target_df = target_df.drop('drop', axis=1)
+            target_df = accession_informed_filter(target_df, 'unknownModifications')
         else:
             target_df = target_df[~target_df['unknownModifications']].drop(
                 ['unknownModifications'], axis=1
             )
         count_after_drop = target_df.shape[0]
         filtered_psms = count_before_drop - count_after_drop
         print(
```

### Comparing `inspirems-1.4/inspire/feature_selection.py` & `inspirems-1.5/inspire/feature_selection.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,18 @@
     LOSS_IONS_KEY,
     MASS_DIFF_KEY,
     MINIMAL_FEATURE_SET,
     NOT_ASSIGNED_KEY,
     OKCYAN_TEXT,
     OUT_SCORE_KEY,
     PEARSON_KEY,
+    PEPTIDE_KEY,
     PRECURSOR_INTE_KEY,
     PREFIX_KEYS,
+    SOURCE_KEY,
     SPEARMAN_KEY,
     SUFFIX_KEYS,
     SEQ_LEN_KEY,
     SOURCE_INDEX_KEY,
     SPECTRAL_ANGLE_KEY,
 )
 from inspire.rescore import apply_rescoring
@@ -632,14 +634,36 @@
         The Config object for the experiment.
     """
     all_features_df = pd.read_csv(
         f'{config.output_folder}/input_all_features.tab',
         sep='\t'
     )
 
+    if config.use_irt_diff:
+        all_features_df[SOURCE_KEY] = all_features_df['specID'].apply(
+            lambda x : '_'.join(x.split('_')[:-2])
+        )
+        sources = all_features_df[SOURCE_KEY].unique().tolist()
+        irt_coeffs = {}
+        for source in sources:
+            try:
+                irt_df = pd.read_csv(f'{config.output_folder}/rt_fit_{source}.csv')
+                irt_coeffs[source] = irt_df['coefficents'].mean()
+                if irt_coeffs[source] <= 0:
+                    irt_coeffs[source] = 1.0
+            except:
+                irt_coeffs[source] = 1.0
+
+        all_features_df['deltaRT'] = all_features_df[['deltaRT', 'source']].apply(
+            lambda df_row : abs(
+                df_row['deltaRT']/irt_coeffs.get(df_row['source'], 1.0) 
+            ),
+            axis=1,
+        )
+
     if config.max_for_selection < all_features_df.shape[0]:
         if config.minimal_features:
             feature_set = MINIMAL_FEATURE_SET
         else:
             feature_set = DEFAULT_FEATURE_SET
             if config.delta_method == 'ignore':
                 feature_set = [x for x in feature_set if x not in DELTA_FEATURES]
@@ -701,14 +725,17 @@
         The Config object
     """
     with open(f'{config.output_folder}/selectedFeatures.yaml', 'w', encoding='UTF-8') as file:
         yaml.dump(feature_set, file)
 
     prefix_keys = PREFIX_KEYS[config.rescore_method]
 
+    all_features_df[PEPTIDE_KEY] = all_features_df[PEPTIDE_KEY].apply(
+        lambda x : f'-.{x}.-'
+    )
     all_features_df = all_features_df[
         prefix_keys + feature_set + SUFFIX_KEYS[config.rescore_method]
     ]
 
     all_features_df.to_csv(
         f'{config.output_folder}/final_input.tab',
         sep='\t',
```

### Comparing `inspirems-1.4/inspire/figures.py` & `inspirems-1.5/inspire/figures.py`

 * *Files identical despite different names*

### Comparing `inspirems-1.4/inspire/get_spectral_angle.py` & `inspirems-1.5/inspire/get_spectral_angle.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,11 +82,11 @@
                 config.delta_method,
                 config.spectral_predictor,
                 minimal_features=True,
             ),
             axis=1,
         )
 
-        input_df = add_delta_irt(input_df, config, None)
-        input_df[input_cols + ['deltaRT', 'spectralAngle']].to_csv(
+
+        input_df[input_cols + ['spectralAngle']].to_csv(
             output_loc
         )
```

### Comparing `inspirems-1.4/inspire/html_template.py` & `inspirems-1.5/inspire/html_template.py`

 * *Files identical despite different names*

### Comparing `inspirems-1.4/inspire/input/mascot.py` & `inspirems-1.5/inspire/input/mascot.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     PTM_NAME_KEY,
     PTM_SEQ_KEY,
     RT_KEY,
     SCAN_KEY,
     SEQ_LEN_KEY,
     SOURCE_KEY,
 )
-from inspire.utils import filter_for_prosit
 
 # Define separators within Mascot output and the names for relevant columns.
 MASCOT_HEADER_MARKER = 'Header'
 MASCOT_FILENAME_MARKER = 'Peak list data path'
 MASCOT_HITS_START_MARKER = 'prot_hit_num'
 MASCOT_NO_FIXED_MODS_MARKER = '""'
 MASCOT_QUERIES_START_MARKER = 'Queries'
@@ -274,15 +273,14 @@
             MASCOT_PTM_SEQ_KEY: PTM_SEQ_KEY,
             MASCOT_PEPTIDE_KEY: PEPTIDE_KEY,
             MASCOT_MISS_KEY: 'missedCleavages',
         }
     )
 
     # Filter for Prosit and add feature columns not present.
-    hits_df = filter_for_prosit(hits_df)
     hits_df[MASS_DIFF_KEY] = hits_df[MASCOT_MASS_KEY] - hits_df[MASCOT_PRED_MASS_KEY]
     hits_df[SEQ_LEN_KEY] = hits_df[PEPTIDE_KEY].apply(len)
     hits_df['avgResidueMass'] = hits_df[MASCOT_MASS_KEY]/hits_df[SEQ_LEN_KEY]
     hits_df.drop([MASCOT_MASS_KEY, MASCOT_PRED_MASS_KEY], axis=1, inplace=True)
 
     hits_df[MASCOT_PEP_QUERY_KEY] = hits_df[MASCOT_PEP_QUERY_KEY].apply(
         lambda x : scan_file + str(x)
```

### Comparing `inspirems-1.4/inspire/input/maxquant.py` & `inspirems-1.5/inspire/input/maxquant.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     PTM_SEQ_KEY,
     PTM_WEIGHT_KEY,
     RT_KEY,
     SCAN_KEY,
     SEQ_LEN_KEY,
     SOURCE_KEY,
 )
-from inspire.utils import filter_for_prosit
 
 # Define the relevant column names from MaxQuant search results.
 MQ_ACCESSION_KEY = 'Proteins'
 MQ_CHARGE_KEY = 'Charge'
 MQ_DECOY_KEY = 'Reverse'
 MQ_DELTA_SCORE_KEY = 'Delta score'
 MQ_LEN_KEY = 'Length'
@@ -186,17 +185,15 @@
             MQ_SEQ_KEY: PEPTIDE_KEY,
             MQ_SOURCE_KEY: SOURCE_KEY,
             MQ_MISSED_CLEAVAGES_KEY: 'missedCleavages',
             MQ_INTENSITY_KEY: 'ms1Intensity',
         }
     )
 
-    # Filter for Prosit, clean up accession data, and add label.
-    mq_df = filter_for_prosit(mq_df)
-
+    # Clean up accession data, and add label.
     mq_df[ACCESSION_KEY] = mq_df[[MQ_ACCESSION_KEY, MQ_DECOY_KEY]].apply(
         lambda x : 'reverseSeq' if x[MQ_DECOY_KEY] == '+' else x[MQ_ACCESSION_KEY],
         axis=1
     )
     mq_df['scanCounts'] = mq_df.groupby([SOURCE_KEY, SCAN_KEY])[ENGINE_SCORE_KEY].transform('count')
     mq_df['fromChimera'] = mq_df['scanCounts'].apply(lambda x : 1 if x > 1 else 0)
```

### Comparing `inspirems-1.4/inspire/input/mgf.py` & `inspirems-1.5/inspire/input/mgf.py`

 * *Files identical despite different names*

### Comparing `inspirems-1.4/inspire/input/mhcpan.py` & `inspirems-1.5/inspire/input/mhcpan.py`

 * *Files identical despite different names*

### Comparing `inspirems-1.4/inspire/input/msp.py` & `inspirems-1.5/inspire/input/msp.py`

 * *Files identical despite different names*

### Comparing `inspirems-1.4/inspire/input/mzml.py` & `inspirems-1.5/inspire/input/mzml.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """ Functions for loading experimental spectra from mzml files.
 """
+import os
+
 import numpy as np
 import pandas as pd
 from pyteomics import mzml
 
 from inspire.constants import (
     CHARGE_KEY,
     INTENSITIES_KEY,
@@ -31,21 +33,28 @@
     """
     ion_list = []
     intensities_list = []
     scan_id_list = []
     mzml_filenames = []
     filename = mzml_filename.split('/')[-1]
 
+    if os.path.exists(mzml_filename.replace('.mzML', '_calibrated.mzML')):
+        input_name = mzml_filename.replace('.mzML', '_calibrated.mzML')
+    elif os.path.exists(mzml_filename):
+        input_name = mzml_filename
+    else:
+        input_name = mzml_filename.replace('.mzML', '_uncalibrated.mzML')
+
     if with_charge:
         charge_list = []
 
     if with_retention_time:
         rt_list = []
 
-    with mzml.read(mzml_filename) as reader:
+    with mzml.read(input_name) as reader:
         for spectrum in reader:
             scan_id = int(spectrum['id'].split('scan=')[1])
             if scan_ids is None or scan_id in scan_ids:
                 mzml_filenames.append(filename)
                 scan_id_list.append(scan_id)
                 intensities_list.append(np.array(list(spectrum['intensity array'])))
                 ion_list.append(np.array(list(spectrum['m/z array'])))
```

### Comparing `inspirems-1.4/inspire/input/peaks.py` & `inspirems-1.5/inspire/input/peaks.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     PTM_SEQ_KEY,
     PTM_WEIGHT_KEY,
     RT_KEY,
     SCAN_KEY,
     SEQ_LEN_KEY,
     SOURCE_KEY,
 )
-from inspire.utils import filter_for_prosit, remove_source_suffixes
+from inspire.utils import remove_source_suffixes
 
 # Define the relevant column names from PEAKS DB search results.
 PEAKS_ACCESSION_KEY = 'Accession'
 PEAKS_ASCORE_KEY = 'AScore'
 PEAKS_CHARGE_KEY = 'Z'
 PEAKS_CHIMERA_KEY = 'from Chimera'
 PEAKS_LEN_KEY = 'Length'
@@ -267,15 +267,14 @@
     # Filter for Prosit and add feature columns not present.
     peaks_df['fromChimera'] = peaks_df[PEAKS_CHIMERA_KEY].apply(
         lambda x : 1 if x == 'Yes' else 0
     )
 
     peaks_df[ACCESSION_KEY].fillna('unknown', inplace=True)
 
-    peaks_df = filter_for_prosit(peaks_df)
     adjusted_masses = peaks_df[PEAKS_MASS_KEY] + peaks_df[CHARGE_KEY]*PROTON
     peaks_df[MASS_DIFF_KEY] = (
         (peaks_df[PEAKS_MZ_KEY]*peaks_df[CHARGE_KEY]) - adjusted_masses
     )
     peaks_df['avgResidueMass'] = peaks_df[PEAKS_MASS_KEY]/peaks_df[SEQ_LEN_KEY]
     peaks_df[DELTA_SCORE_KEY] = 0
     peaks_df['missedCleavages'] = 0
```

### Comparing `inspirems-1.4/inspire/input/search_results.py` & `inspirems-1.5/inspire/input/search_results.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """ Generic functions for reading in any search results.
 """
+import multiprocessing
 import os
 
 import pandas as pd
 
 from inspire.accession import process_accession_groups
+from inspire.constants import SOURCE_KEY, SCAN_KEY, PEPTIDE_KEY, LABEL_KEY, ACCESSION_STRATUM_KEY, ENGINE_SCORE_KEY
 from inspire.input.mascot import read_mascot_data
 from inspire.input.maxquant import read_mq_data
+from inspire.input.msfragger import read_ms_fragger_data
 from inspire.input.peaks import read_peaks_data
-from inspire.utils import add_fixed_modifications
+from inspire.utils import add_fixed_modifications, filter_for_prosit
 
 def generic_read_df(config, save_dfs=True, overwrite_reduce=False):
     """ Function to read in search results from any search engine.
 
     Parameters
     ----------
     config : inspire.config.Config
@@ -48,25 +51,43 @@
                 config.source_filename,
                 with_accession=config.use_accession_stratum,
             )
         elif config.search_engine == 'maxquant':
             search_df, mods_df = read_mq_data(config.search_results)
         elif config.search_engine == 'peaks':
             search_df, mods_df = read_peaks_data(config.search_results)
+        elif config.search_engine == 'msfragger':
+            n_cores = min(config.n_cores, multiprocessing.cpu_count())
+            search_df, mods_df = read_ms_fragger_data(
+                config.search_results,
+                config.fixed_modifications,
+                n_cores,
+            )
         else:
             raise ValueError(f'Unknown Search Engine: {config.search_engine}')
 
-        if config.fixed_modifications is not None:
+        if (
+            config.fixed_modifications is not None and
+            config.search_engine != 'msfragger'
+        ):
             search_df, mods_df = add_fixed_modifications(
                 search_df,
                 mods_df,
                 config.fixed_modifications
             )
 
         if config.use_accession_stratum:
             search_df = process_accession_groups(search_df, config)
+            search_df = search_df.sort_values(by=[LABEL_KEY, ACCESSION_STRATUM_KEY, ENGINE_SCORE_KEY, PEPTIDE_KEY], ascending=[False, True, True, True])
+            search_df['ilPep'] = search_df[PEPTIDE_KEY].apply(lambda x : x.replace('I', 'L'))
+
+            search_df = search_df.drop_duplicates(
+                subset=[SOURCE_KEY, SCAN_KEY, 'ilPep']
+            )
+
+        search_df = filter_for_prosit(search_df, config.use_accession_stratum)
 
         if save_dfs and config.reuse_input:
             search_df.to_csv(f'{config.output_folder}/formated_df.csv', index=False)
             mods_df.to_csv(f'{config.output_folder}/formated_mods.csv', index=False)
 
     return search_df, mods_df
```

### Comparing `inspirems-1.4/inspire/mz_match.py` & `inspirems-1.5/inspire/mz_match.py`

 * *Files identical despite different names*

### Comparing `inspirems-1.4/inspire/plot_spectra.py` & `inspirems-1.5/inspire/prosit_delta.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,592 +1,645 @@
-""" Functions for plotting spectra.
+""" Functions for applying the prosit-delta predictor.
 """
-import os
-
-from PyPDF2 import PdfFileMerger
-import pandas as pd
+from math import acos, pi
+from copy import deepcopy
 import numpy as np
-import plotly.graph_objects as go
-from plotly.subplots import make_subplots
-import plotly.io as pio
 
 from inspire.constants import (
-    CHARGE_KEY,
+    BLOSUM6_1_VALUES,
+    INTENSITIES_KEY,
+    ION_OFFSET,
     KNOWN_PTM_WEIGHTS,
+    MZS_KEY,
     PEPTIDE_KEY,
-    PROTON,
-    SCAN_KEY,
-    SOURCE_KEY,
+    PROSIT_IONS_KEY,
+    PTM_SEQ_KEY,
+    RESIDUE_WEIGHTS,
     SPECTRAL_ANGLE_KEY,
 )
+from inspire.mz_match import match_mz
 
+DELTA_PRO_FEATURE_SET = (
+    'spectralAngle',
+    'blosumC',
+    'blosumN',
+    'nTermDist',
+    'cTermDist',
+    'charge',
+    'cNeighbourBlosum',
+    'nNeighbourBlosum',
+    'yErrsAtLoc',
+    'bErrsAtLoc',
+    'collisionEnergy',
+    'bPrositIntesAtC',
+    'yPrositIntesAtN',
+    'yPrositIntesAtLoc',
+    'bPrositIntesAtLoc',
+    'yMatchedIntesAtN',
+    'bMatchedIntesAtC',
+    'yMatchedIntesAtLoc',
+    'bMatchedIntesAtLoc',
+    'cOxidation',
+    'nOxidation',
+    'flipYNewIntensity',
+    'flipBNewIntensity',
+    'matchedCoverage',
+)
 
-from inspire.input.msp import msp_to_df
-from inspire.mz_match import get_ion_masses
-from inspire.predict_spectra import predict_spectra
-from inspire.spectral_features import calculate_spectral_features
-from inspire.utils import fetch_scan_data, convert_mod_seq_to_ptm_seq
+SPECTRAL_ANGLE_INDEX = DELTA_PRO_FEATURE_SET.index('spectralAngle')
+BLOSUM_N_INDEX = DELTA_PRO_FEATURE_SET.index('blosumN')
+BLOSUM_C_INDEX = DELTA_PRO_FEATURE_SET.index('blosumC')
+CHARGE_INDEX = DELTA_PRO_FEATURE_SET.index('charge')
+MATCHED_COV_INDEX = DELTA_PRO_FEATURE_SET.index('matchedCoverage')
+CE_INDEX = DELTA_PRO_FEATURE_SET.index('collisionEnergy')
+C_NEIGHB_INDEX = DELTA_PRO_FEATURE_SET.index('cNeighbourBlosum')
+N_NEIGHB_INDEX = DELTA_PRO_FEATURE_SET.index('nNeighbourBlosum')
+N_TERM_INDEX = DELTA_PRO_FEATURE_SET.index('nTermDist')
+C_TERM_INDEX = DELTA_PRO_FEATURE_SET.index('cTermDist')
+Y_NEW_INTE_INDEX = DELTA_PRO_FEATURE_SET.index('flipYNewIntensity')
+B_NEW_INTE_INDEX = DELTA_PRO_FEATURE_SET.index('flipBNewIntensity')
+Y_ERR_INDEX = DELTA_PRO_FEATURE_SET.index('yErrsAtLoc')
+B_ERR_INDEX = DELTA_PRO_FEATURE_SET.index('bErrsAtLoc')
+B_PROSIT_C_INTE_INDEX = DELTA_PRO_FEATURE_SET.index('bPrositIntesAtC')
+Y_PROSIT_N_INTE_INDEX = DELTA_PRO_FEATURE_SET.index('yPrositIntesAtN')
+Y_PROSIT_INTE_INDEX = DELTA_PRO_FEATURE_SET.index('yPrositIntesAtLoc')
+B_PROSIT_INTE_INDEX = DELTA_PRO_FEATURE_SET.index('bPrositIntesAtLoc')
+Y_MATCHED_N_INTE_INDEX = DELTA_PRO_FEATURE_SET.index('yMatchedIntesAtN')
+B_MATCHED_C_INTE_INDEX = DELTA_PRO_FEATURE_SET.index('bMatchedIntesAtC')
+Y_MATCHED_INTE_INDEX = DELTA_PRO_FEATURE_SET.index('yMatchedIntesAtLoc')
+B_MATCHED_INTE_INDEX = DELTA_PRO_FEATURE_SET.index('bMatchedIntesAtLoc')
+N_OX_INDEX = DELTA_PRO_FEATURE_SET.index('nOxidation')
+C_OX_INDEX = DELTA_PRO_FEATURE_SET.index('cOxidation')
+
+DELTA_PRO_RESIDUE_WEIGHTS = deepcopy(RESIDUE_WEIGHTS)
+DELTA_PRO_RESIDUE_WEIGHTS['C'] = 103.009185 + 57.021464
+DELTA_PRO_RESIDUE_WEIGHTS['m'] = DELTA_PRO_RESIDUE_WEIGHTS['M'] + KNOWN_PTM_WEIGHTS['Oxidation (M)']
+SIGNIFICANCE_THRESHOLD = -0.05
 
-PLOTS_PER_PAGE = 15
-PLOTS_PER_LINE = 3
+def check_oxidation(pep_len, ptm_seq, idx, ox_flag):
+    """ Helper function to check if resiude is oxidised.
+    """
+    if not isinstance(ptm_seq, str) or ox_flag not in ptm_seq or idx < 0 or idx > pep_len:
+        return 0
+    if ptm_seq[idx+2] == ox_flag:
+        return 1
+    return 0
 
+def get_mass_diff(peptide, ptm_seq, idx, ox_flag):
+    """ Function to find the difference between two residue masses.
+    """
+    if not isinstance(ptm_seq, str):
+        return abs(
+            DELTA_PRO_RESIDUE_WEIGHTS[peptide[idx]] - DELTA_PRO_RESIDUE_WEIGHTS[peptide[idx-1]]
+        )
 
-def convert_names_and_mzs(mod_seq, pred_names):
-    """ Function to generate plotting ion names and mzs.
+    c_wt = DELTA_PRO_RESIDUE_WEIGHTS[peptide[idx]]
+    n_wt = DELTA_PRO_RESIDUE_WEIGHTS[peptide[idx-1]]
+    if ptm_seq[idx+2] == ox_flag:
+        c_wt += KNOWN_PTM_WEIGHTS['Oxidation (M)']
+    if ptm_seq[idx+1] == ox_flag:
+        n_wt += KNOWN_PTM_WEIGHTS['Oxidation (M)']
+    return abs(c_wt - n_wt)
+
+def get_intes_at_loc(pep_len, matched_intensities, prosit_ions, loc, letter):
+    """ Function to calculate the sum of all intensities at a given location.
 
     Parameters
     ----------
-    mod_seq : str
-        The Prosit modified_sequence.
-    pred_names : list of str
-        A list of the names of the ions as read in from msp format.
+    pep_len : int
+        The length of the peptide.
+    prosit_ions : dict
+        The prosit predicted spectrum.
+    loc : int
+        The location at which to get intensities.
+    letter : str
+        The type of ion considered.
 
     Returns
     -------
-    pred_mzs : list of float
-        A list of the theoretical mz values for the prosit predicted ions.
-    plotting_names : list of str
-        A list of the annotations for the prosit predicted ions.
-    """
-    if '(ox)' not in mod_seq and 'C' not in mod_seq:
-        mods = None
-        un_mod_seq = mod_seq.replace('(ox)', '')
-    else:
-        mods = '0.'
-        un_mod_seq = ''
-        while mod_seq:
-            if len(mod_seq) > 1:
-                if mod_seq[1] == '(':
-                    un_mod_seq += 'M'
-                    mods += '1'
-                    mod_seq = mod_seq[5:]
-                    continue
-            un_mod_seq += mod_seq[0]
-            if mod_seq[0] != 'C':
-                mods += '0'
-            else:
-                mods += '2'
-            mod_seq = mod_seq[1:]
-        mods += '.0'
-    masses, _ = get_ion_masses(
-        un_mod_seq,
-        {
-            0: 0.0,
-            1: KNOWN_PTM_WEIGHTS['Oxidation (M)'],
-            2: KNOWN_PTM_WEIGHTS['Carbamidomethylation'],
-        },
-        modifications=mods
-    )
-    pred_mzs = []
-    plotting_names = []
-    for pred_ion in pred_names:
-        ion_data = pred_ion.split('^')
-        if '^' in pred_ion:
-            charge = int(ion_data[1])
-        else:
-            charge = 1
-        plotting_names.append(ion_data[0] + ('+' * charge))
-        code = ion_data[0][0]
-        idx = int(ion_data[0][1:])
-        pred_mzs.append(
-            (masses[code][idx-1] + (PROTON*charge))/charge
-        )
-    return pred_mzs, plotting_names
-
-def get_unmatched(exp_mzs, exp_intes, matched_mzs, l2_norm):
-    """ Function select and normalise the unmatched peaks from the experimental spectrum.
+    sum_inte : float
+        The sum of intensities at the location.
+    """
+    sum_inte = 0.0
+    if loc in (0, pep_len):
+        return sum_inte
+
+    if letter == 'y':
+        loc = pep_len - loc
+
+    for charge in ['', '^2', '^3']:
+        for loss in ['', '-NH3', '-H2O']:
+            full_code = letter + str(loc) + charge + loss
+            inte_val = matched_intensities[prosit_ions == full_code]
+            if inte_val.size:
+                sum_inte += inte_val[0]
+    return sum_inte
+
+def compute_single_mz(sequence, modifications, ion_type, ion_idx, ptm_id_weights):
+    """ Function to compute the molecular weights of potential fragments
+        generated from a peptide (y & b ions, charges 1,2, or 3, and H2O
+        or O2 losses).
 
     Parameters
     ----------
-    exp_mzs : list of float
-        List of the mz values of the experimental spectrum.
-    exp_intes : list of float
-        List of the intensity values of the experimental spectrum.
-    matched_mzs : list of float
-        List of the mz values matched to the Prosit spectrum.
-    l2_norm : float
-        Either the l2 norm of the matched spectrum or the maximum intensity in the
-        experimental spectrum if fewer than 5 peaks are matched.
+    sequence : str
+        The peptide sequence for which we require molecular weights.
+    modifications : str
+        A string of the ptms for the sequence which will alter
+        the potential mzs.
+    reverse : bool
+        Whether we are getting fragment mzs in the forward direction
+        (eg for b ions), or backward direction (eg. for y ions).
+    ptm_id_weights : dict
+        Mapping of ptm ids to their molecular weights.
 
     Returns
     -------
-    unmatched_mzs : list of float
-        List of the mz values of the experimental spectrum not matched
-        to the Prosit predicted spectrum.
-    exp_intes : list of float
-        List of the intensity values of the experimental spectrum not
-        matched to the Prosit predicted spectrum.
-    """
-    unmatched_mzs, unmatched_intes = [], []
-    for idx, e_mz in enumerate(exp_mzs):
-        if e_mz not in matched_mzs:
-            unmatched_mzs.append(e_mz)
-            unmatched_intes.append(exp_intes[idx]/l2_norm)
-
-    return {
-        'mzs': unmatched_mzs,
-        'intensities': unmatched_intes,
-    }
-
-def experiment_match(exp_mzs, exp_intes, pred_mzs, plotting_names, mz_accuracy, mz_units):
-    """ Function to match the mz values of the experimentally observed peaks to the
-        Prosit predicted peaks.
+    mzs : np.array of floats
+        An array of all the possible mzs that coule be observed in
+        the MS2 spectrum of a sequence.
+    """
+    if (
+        modifications and
+        isinstance(modifications, str) and
+        modifications != 'nan'
+        and modifications != 'None'
+    ):
+        ptms_list = modifications.split(".")
+        mods_list = [int(mod) for mod in ptms_list[1]]
+
+        if ion_type == 'y':
+            ptm_start = int(ptms_list[2])
+            mods_list = mods_list[::-1]
+        else:
+            ptm_start = int(ptms_list[0])
+    else:
+        mods_list = None
+        ptm_start = 0.0
+
+    if ion_type == 'y':
+        sequence = sequence[::-1]
+
+    tracking_mw = ptm_id_weights[ptm_start]
+
+    for idx in range(ion_idx):
+        tracking_mw += RESIDUE_WEIGHTS[sequence[idx]]
+        if mods_list is not None and mods_list[idx]:
+            tracking_mw += ptm_id_weights[mods_list[idx]]
+
+    return tracking_mw + ION_OFFSET[ion_type]
+
+def calculate_sa_from_dict(predicted, true):
+    """ Function to calculate the spectral angle when the predicted and true spectrum
+        are stored as dictionaries.
 
     Parameters
     ----------
-    exp_mzs : list of float
-        The experimentally observed mz values.
-    exp_intes : list of float
-        The experimentally observed intensity values.
-    pred_mzs : list of float
-        The Prosit predicted mz values.
+    predicted : dict
+        A dictionary of the prosit predicted spectrum.
+    true : dict
+        A dictionary of the experimental ions matched to the predicted spectrum.
 
     Returns
     -------
-    matched_mzs : list of float
-        The matched mz values in the experimental spectrum.
-    matched_intes : list of float
-        The matched intensity values in the experimental spectrum.
-    l2_norm : float
-        The l2 norm of the matched intensities if more than 5 peaks are matched,
-        otherwise the maximum intensity in the spectrum.
-    matched_pred_mzs : list of float
-        A list of the matched prosit predicted mz values.
-    """
-    matched_mzs, matched_intes = [], []
-    matched_pred_mzs = []
-    matched_names = []
-    for match_name, pred_m in zip(plotting_names, pred_mzs):
-        matched_ind = -1
-        min_match = 100000
-        for idx, exp_mz in enumerate(exp_mzs):
-            if abs(exp_mz-pred_m) < min_match:
-                min_match = abs(exp_mz-pred_m)
-                matched_ind = idx
+    spectral_angle : float
+        The spectral angle between spectra.
+    """
+    true_l2_norm = np.linalg.norm(np.array(list(true.values())), ord=2)
+    pred_l2_norm = np.linalg.norm(np.array(list(predicted.values())), ord=2)
 
-        if mz_units == 'ppm':
-            mz_err = pred_m*mz_accuracy*(10**-6)
-        else:
-            mz_err = mz_accuracy
+    if true_l2_norm == 0 and pred_l2_norm == 0:
+        return 0.0
+    if true_l2_norm == 0 and pred_l2_norm == 0:
+        return 1.0
+
+    if pred_l2_norm > 0.0:
+        for ion in predicted:
+            predicted[ion] /= pred_l2_norm
+    if true_l2_norm > 0.0:
+        for ion in true:
+            true[ion] /= true_l2_norm
+
+    product = 0.0
+    for ion in predicted:
+        product += (predicted[ion] * true.get(ion, 0.0))
+
+    product = max(min(product, 1.0), 0.0)
+    spectral_distance = 2*acos(product)/pi
+    return 1.0 - spectral_distance
 
-        if min_match < mz_err:
-            matched_mzs.append(exp_mzs[matched_ind])
-            matched_intes.append(exp_intes[matched_ind])
-            matched_pred_mzs.append(pred_m)
-            matched_names.append(match_name.split('+')[0])
+def convert_ptm_seq(ptm_seq, flip_idx):
+    """ Function to adjust a PTM sequence to match permutation of the sequence.
 
-    if len(matched_intes) > 5:
-        l2_norm = np.linalg.norm(np.array(matched_intes), ord=2)
-    else:
-        l2_norm = np.max(exp_intes)
+    Parameters
+    ----------
+    ptm_seq : str or None
+        The the original PTM sequence (stored as string of digits)
+    flip_idx : int
+        The index which is to be permuted.
 
-    matched_peaks = {
-        'mzs': matched_mzs,
-        'intensities': [x/l2_norm for x in matched_intes],
-    }
+    Returns
+    -------
+    ptm_seq : str or None
+        The adjusted PTM sequence.
+    """
+    if not isinstance(ptm_seq, str):
+        return ptm_seq
 
-    return matched_peaks, l2_norm, matched_pred_mzs, matched_names
+    ptm_seq = (
+        ptm_seq[:flip_idx+1] + ptm_seq[flip_idx+2] +
+        ptm_seq[flip_idx+1] + ptm_seq[flip_idx+3:]
+    )
+    return ptm_seq
 
 
-def pair_plot(df_row, mz_accuracy, mz_units):
-    """ Function to generate the traces and annotations needed for the pair plots
-        of the spectra.
+def get_brute_force_deltas(df_row, matched_dict, ptm_id_weights, mz_accuracy, spectral_predictor):
+    """ Function to calculate the Prosit delta values of PSM using the "brute force" method -
+        calculating all possible permuted spectral angles and comparing them to the original.
 
     Parameters
     ----------
     df_row : pd.Series
-        An individual row of the DataFrame.
+        A single row of the PSM dataframe.
+    matched_dict : dict
+        A dictionary of the Prosit matched ions in the experimental spectrum.
+    ptm_id_weights : dict
+        A dictionary providing the molecular weights of all PTMs.
+    mz_accuracy : float
+        The accuracy of the mass spectrometer.
+    spectral_predictor : str
+        Either prosit or ms2pip.
 
     Returns
     -------
-    traces : list of plot.graph_objects
-        The bar plot traces for experimental and prosit predicted spectra.
-    annotations : list of dict
-        A list of the annotations needed for the bar plot.
+    df_row : pd.Series
+        The input row with Prosit-delta features added.
     """
-    index = df_row['index']
-    peptide = df_row['peptide']
+    peptide = df_row[PEPTIDE_KEY]
     pep_len = len(peptide)
-    pred_intes = [-x for x in df_row['prositIons'].values()]
+    deltas = []
+    for i in range(1, 30):
+        if not isinstance(df_row[f'flip{i}'], str) or df_row[f'flip{i}'] == peptide:
+            continue
+
+        flip_peptide = df_row[f'flip{i}'].replace('m', 'M')
+        pred_ions = df_row[f'flip{i}Ions']
+        if spectral_predictor == 'prosit':
+            flip_ptm = convert_ptm_seq(df_row[PTM_SEQ_KEY], i)
+        else:
+            flip_ptm = df_row[f'flip{i}Ptms']
+        rev_i = pep_len - i
+        differing_ions = [
+            f'b{i}', f'b{i}^2', f'b{i}^3', f'y{rev_i}', f'y{rev_i}^2', f'y{rev_i}^3',
+        ]
+        flip_matched = deepcopy(matched_dict)
+        for diff_ion in differing_ions:
+            flip_matched.pop(diff_ion, None)
+        flip_pred_ions = [x for x in differing_ions if x in pred_ions]
+
+        missing_preds = [x for x in pred_ions if x not in df_row['prositIons']]
+
+        missing_finds = [x for x in df_row['prositIons'] if x not in pred_ions]
+        for miss in missing_finds:
+            flip_matched.pop(miss, None)
+
+        all_recalc_ions = flip_pred_ions + missing_preds
+        if all_recalc_ions:
+            b_wt = compute_single_mz(flip_peptide, flip_ptm, 'b', i, ptm_id_weights)
+            y_wt = compute_single_mz(flip_peptide, flip_ptm, 'y', rev_i, ptm_id_weights)
+            for ion in flip_pred_ions:
+                ion_type = ion[0]
+                if ion_type == 'b':
+                    base_mass = b_wt
+                else:
+                    base_mass = y_wt
+                ion_data = ion.split('^')
+                if len(ion_data) == 1:
+                    frag_z = 1
+                else:
+                    frag_z = int(ion_data[-1])
+                mz_match, match_idx = match_mz(base_mass, frag_z, df_row[MZS_KEY], loss=0.0)
+                if abs(mz_match) < mz_accuracy:
+                    flip_matched[ion] = df_row[INTENSITIES_KEY][match_idx]
 
-    pred_mzs, plotting_names = convert_names_and_mzs(
-        df_row['modified_sequence'],
-        list(df_row['prositIons'].keys())
-    )
+        flip_sa = calculate_sa_from_dict(pred_ions, flip_matched)
+        deltas.append(flip_sa - df_row[SPECTRAL_ANGLE_KEY])
 
-    matched_peaks, l2_norm, matched_p_mz, matched_names = experiment_match(
-        df_row['mzs'], df_row['intensities'], pred_mzs, plotting_names, mz_accuracy, mz_units
-    )
-    unmatched_peaks = get_unmatched(
-        df_row['mzs'], df_row['intensities'], matched_peaks['mzs'], l2_norm
-    )
+    return calculate_delta_features(df_row, np.array(deltas))
 
-    annotations = []
-    colours = []
-    for idx, entry in enumerate(pred_mzs):
-        if entry in matched_p_mz:
-            colour = '#0095A8'
-        else:
-            colour = '#FF7043'
-        colours.append(colour)
+def calculate_delta_features(df_row, prot_deltas):
+    """ Function to calculate the Prosit delta features.
 
-        if pred_intes[idx] < -0.05:
-            annotations.append(
-                {
-                    'x': entry,
-                    'ax': entry,
-                    'y': pred_intes[idx]-0.05,
-                    'ay': pred_intes[idx]-0.05,
-                    'xref': f'x{index+1}',
-                    'yref': f'y{index+1}',
-                    'text': plotting_names[idx],
-                    'font_size': 8,
-                    'font_color': colour,
-                    'showarrow': False,
-                }
-            )
+    Parameters
+    ----------
+    df_row : pd.Series
+        A single row of the PSM dataframe.
+    prot_deltas : np.array
+        The Prosit-delta values at each point in the sequence.
 
-    if pep_len < 20:
-        annot_height = 1.5
+    Returns
+    -------
+    df_row : pd.Series
+        The input row with Prosit-delta features added.
+    """
+    if prot_deltas.size != 0:
+        df_row['nDeltasAboveThreshold'] = len(
+            prot_deltas[prot_deltas > -0.1]
+        )/len(prot_deltas)
+        df_row['nDeltasAboveThresholdA'] = len(
+            prot_deltas[prot_deltas > -0.05]
+        )/len(prot_deltas)
+        df_row['nDeltasAboveZero'] = len(
+            prot_deltas[prot_deltas > 0.0]
+        )/len(prot_deltas)
+        delta_q1 = np.quantile(prot_deltas, 0.25)
+        delta_q3 = np.quantile(prot_deltas, 0.75)
+        df_row['prositDeltaMedian'] = np.quantile(prot_deltas, 0.5)
+        df_row['prositDeltaQuartile1'] = delta_q1
+        df_row['prositDeltaQuartile3'] = delta_q3
+        df_row['minPrositDelta'] = np.min(prot_deltas)
+        df_row['maxPrositDelta'] = np.max(prot_deltas)
     else:
-        annot_height = 0.7
+        df_row['nDeltasAboveThreshold'] = -1.0
+        df_row['nDeltasAboveThresholdA'] = -1.0
+        df_row['nDeltasAboveZero'] = -1.0
+        df_row['prositDeltaMedian'] = -1.0
+        df_row['prositDeltaQuartile1'] = -1.0
+        df_row['prositDeltaQuartile3'] = -1.0
+        df_row['maxPrositDelta'] = -1.0
+        df_row['minPrositDelta'] = -1.0
 
-    extra_traces = []
-    annotations.append({
-        'showarrow': False,
-            'text': 'Experimental Spectrum',
-            'x': 1300,
-            'ax': 1300,
-            'y': annot_height,
-            'ay': annot_height,
-            'font_size': 12,
-            'font_family': "Arial, monospace",
-            'xref': f'x{index+1}',
-            'yref': f'y{index+1}',
-            'align': 'left',
-    })
-    annotations.append({
-        'showarrow': False,
-            'text': 'Prosit Predicted Spectrum',
-            'x': 1300,
-            'ax': 1300,
-            'y': -1.1,
-            'ay': -1.1,
-            'font_size': 12,
-            'font_family': "Arial, monospace",
-            'xref': f'x{index+1}',
-            'yref': f'y{index+1}',
-            'align': 'left',
-    })
-    for idx, residue in enumerate(peptide):
-        annotations.append({
-            'showarrow': False,
-            'text': (residue),
-            'x': 50 + (idx * 50),
-            'ax': 50 + (idx * 50),
-            'y': 1.25,
-            'ay': 1.25,
-            'font_size': 12,
-            'font_family': "Arial, monospace",
-            'xref': f'x{index+1}',
-            'yref': f'y{index+1}',
-            'align': 'left',
-        })
-        if idx > 0:
-            min1_idx = idx-1
-            rev_idx = len(peptide) - idx
-            y_matched = False
-            b_matched = False
-            if f'b{idx}' in matched_names:
-                annotations.append({
-                    'showarrow': False,
-                    'text': f'b{idx}',
-                    'x': 40 + (min1_idx * 50),
-                    'ax': 40 + (min1_idx * 50),
-                    'y': 1.02,
-                    'ay': 1.02,
-                    'font_size': 10,
-                    'font_family': "Arial, monospace",
-                    'xref': f'x{index+1}',
-                    'yref': f'y{index+1}',
-                    'align': 'left',
-                })
-                b_matched = True
-            if f'y{rev_idx}' in matched_names:
-                annotations.append({
-                    'showarrow': False,
-                    'text': f'y{rev_idx}',
-                    'x': 63 + (idx * 50),
-                    'ax': 63 + (idx * 50),
-                    'y': 1.49,
-                    'ay': 1.49,
-                    'font_size': 10,
-                    'font_family': "Arial, monospace",
-                    'xref': f'x{index+1}',
-                    'yref': f'y{index+1}',
-                    'align': 'left',
-                })
-                y_matched = True
-        if idx > 0:
-            if b_matched:
-                extra_traces.append(
-                    go.Scatter(
-                        x=[50 + ((idx-1) * 50), 50 + ((idx-0.5) * 50)],
-                        y=[1.1, 1.25],
-                        mode='lines',
-                        line_color='black',
-                        line_width=0.5,
-                    )
-                )
-            if y_matched:
-                extra_traces.append(
-                    go.Scatter(
-                        x=[50 + ((idx-0.5) * 50), 50 + (idx * 50)],
-                        y=[1.25, 1.4],
-                        mode='lines',
-                        line_color='black',
-                        line_width=0.5,
-                    )
-                )
-            if b_matched:
-                extra_traces.append(
-                    go.Scatter(
-                        x=[40 + ((idx-1) * 50), 50 + ((idx-1) * 50)],
-                        y=[1.1, 1.1],
-                        mode='lines',
-                        line_color='black',
-                        line_width=0.5,
-                    )
-                )
-            if y_matched:
-                extra_traces.append(
-                    go.Scatter(
-                        x=[50 + ((idx) * 50), 60 + (idx * 50)],
-                        y=[1.4, 1.4],
-                        mode='lines',
-                        line_color='black',
-                        line_width=0.5,
-                    )
-                )
-
-    traces = [
-        go.Bar(
-            x=pred_mzs,
-            base='relative',
-            alignmentgroup='predicted',
-            y=pred_intes,
-            name='Predicted',
-            marker_color=colours,
-            textfont={
-                'size': 40,
-                'color': 'black'
-            },
-            marker_line_width=0,
-            width=4,
-            textposition='outside',
-        ),
-        go.Bar(
-            x=unmatched_peaks['mzs'],
-            y=unmatched_peaks['intensities'],
-            base='relative',
-            alignmentgroup='experimental',
-            name='Experimental Not Matched',
-            marker_color='lightgrey',
-            marker_line_width=0,
-            width=4,
-        ),
-        go.Bar(
-            x=matched_peaks['mzs'],
-            y=matched_peaks['intensities'],
-            base='relative',
-            alignmentgroup='experimental',
-            name='Experimental Matched',
-            marker_color='black',
-            marker_line_width=0,
-            width=4,
-        ),
-    ] + extra_traces
-
-    return traces, annotations
-
-
-def plot_spectra(config):
-    """ Function to generate pair plots of selected PSMs (experimental vs. Prosit
-        predicted spectra.).
+    return df_row
+
+def compute_pd_single_mw(sequence, ion_type, ion_idx):
+    """ Function to compute the mw of a single ion.
 
     Parameters
     ----------
-    config : inspire.config.Config
-        The Config object used to run the inSPIRE experiment.
+    sequence : str
+        The peptide sequence.
+    ion_type : str
+        y or b.
+    ion_idx : int
+        The index of ion.
+
+    Returns
+    -------
+    mw : float
+        The mw of the theoretical ion.
     """
-    input_df = pd.read_csv(f'{config.output_folder}/plotData.csv')
+    if ion_type == 'y':
+        sequence = sequence[::-1]
 
-    get_charge_from_scan_file = not CHARGE_KEY in input_df.columns
-    scan_df = fetch_scan_data(input_df, config, get_charge_from_scan_file)
+    tracking_mw = 0.0
 
-    input_df = pd.merge(
-        input_df,
-        scan_df,
-        how='inner',
-        on=[SOURCE_KEY, SCAN_KEY]
-    )
-    n_groups = 1 + (input_df.shape[0] // PLOTS_PER_PAGE)
+    for idx in range(ion_idx):
+        tracking_mw += DELTA_PRO_RESIDUE_WEIGHTS[sequence[idx]]
+
+    return tracking_mw + ION_OFFSET[ion_type]
 
-    input_df['modified_sequence'] = input_df['modifiedSequence'].apply(
-        lambda x : x.replace('[+16.0]', '(ox)').replace('[+57.0]', '')
-    )
-    input_df['precursor_charge'] = input_df[CHARGE_KEY]
 
-    if 'collisionEnergy' in input_df.columns:
-        input_df = input_df.rename(columns={'collisionEnergy': 'collision_energy'})
+def get_new_inte(peptide, flip_ind, df_row, mz_accuracy, ion_series):
+    """ Function to get the potential new intensity.
+    """
+    if ion_series == 'b':
+        base_mass = compute_pd_single_mw(peptide, 'b', flip_ind-1)
+        base_mass += DELTA_PRO_RESIDUE_WEIGHTS[peptide[flip_ind]]
     else:
-        input_df['collision_energy'] = config.collision_energy
+        base_mass = compute_pd_single_mw(peptide, 'y', len(peptide)-(flip_ind+1))
+        base_mass += DELTA_PRO_RESIDUE_WEIGHTS[peptide[flip_ind-1]]
+    match_inte = 0.0
+    for frag_z in range(1, min(df_row['charge'], 4)):
+        mz_match, match_idx = match_mz(base_mass, frag_z, df_row[MZS_KEY], loss=0.0)
+        if abs(mz_match) < mz_accuracy:
+            match_inte += df_row[INTENSITIES_KEY][match_idx]
+    return match_inte
+
+def get_err_at_loc(pep_len, matched_ions, prosit_ions, loc, letter):
+    """ Function to get the error at a point in a spectrum between Prosit predicted and
+        normalised experimental intensitiy.
 
-    input_df[['modified_sequence', 'precursor_charge', 'collision_energy']].to_csv(
-        f'{config.output_folder}/plotInput.csv', index=False,
-    )
+    Parameters
+    ----------
+    pep_len : int
+        Length of the peptide.
+    matched_ions : dict
+        Dictionary of the experimental intensities matched to Prosit ions.
+    prosit_ions : dict
+        Dictionary of the prosit predicted intensities.
+    loc : int
+        The location of interest.
+    letter : str
+        y or b
 
-    predict_spectra(config, pipeline='plotSpectra')
-    prosit_df = msp_to_df(f'{config.output_folder}/plotPredictions.msp', 'prosit', None)
-    prosit_df = prosit_df.drop_duplicates(subset=['modified_sequence', CHARGE_KEY])
-
-    input_df = pd.merge(
-        input_df,
-        prosit_df,
-        how='inner',
-        on=['modified_sequence', CHARGE_KEY]
-    )
+    Returns
+    -------
+    sum_error : float
+        The sum of all errors at that location.
+    """
+    sum_err = 0
+    if letter == 'y':
+        loc = pep_len - loc
+    for charge in ['', '^2', '^3']:
+        code = letter + str(loc) + charge
+        sum_err += abs(matched_ions.get(code, 0.0) - prosit_ions.get(code, 0.0))
+
+    return sum_err
+
+def get_deltas(
+        df_row,
+        prosit_ions,
+        matched_intes,
+        prosit_intes,
+        reg_model,
+        ox_flag,
+        mz_accuracy,
+        matched_dict,
+    ):
+    """ Function to get all predicted prosit-deltas.
 
-    input_df = input_df.reset_index(drop=True)
-    input_df['group'] = input_df.index // PLOTS_PER_PAGE
-    input_df['index'] = input_df.index % PLOTS_PER_PAGE
-    input_df['plot_data'] = input_df.apply(
-        lambda x : pair_plot(x, config.mz_accuracy, config.mz_units),
-        axis=1,
-    )
+    Parameters
+    ----------
+    df_row : pd.Series
+        A row of a DataFrame containing spectral data.
+    prosit_ions : dict
+        The prosit predicted spectrum.
+    reg_model : sklearn.ensemble.RandomForestRegressor
+        The trained prosit-delta model.
 
-    if SPECTRAL_ANGLE_KEY not in input_df.columns:
-        input_df['ptm_seq'] = input_df['modifiedSequence'].apply(
-            convert_mod_seq_to_ptm_seq
-        )
-        input_df = input_df.apply(
-            lambda x : calculate_spectral_features(
-                x,
-                {
-                    0: 0.0,
-                    1: KNOWN_PTM_WEIGHTS['Oxidation (M)'],
-                    2: KNOWN_PTM_WEIGHTS['Carbamidomethylation'],
-                },
-                config.mz_accuracy,
-                config.mz_units,
-                None,
-                '1',
-                config.delta_method,
-                config.spectral_predictor,
-                minimal_features=True,
-            ),
-            axis=1,
-        )
-
-    titles = []
-    for idx in range(input_df.shape[0]):
-        seq = input_df[PEPTIDE_KEY].iloc[idx]
-        scan_nr = input_df[SCAN_KEY].iloc[idx]
-        src = input_df[SOURCE_KEY].iloc[idx]
-        spectral_angle = round(input_df[SPECTRAL_ANGLE_KEY].iloc[idx], 2)
-        titles.append(
-            f'<b>Source</b> {src} <b>Scan</b> {scan_nr}<br><b>Peptide</b> {seq} ' +
-            f'<b>Spectral Angle</b> {spectral_angle}<br>'
-        )
-
-    for group_idx in range(n_groups):
-
-        start_idx = PLOTS_PER_PAGE*group_idx
-        sub_df = input_df[input_df['group'] == group_idx]
-        n_plots = sub_df.shape[0]
-        n_plot_rows = 1 + (n_plots//PLOTS_PER_LINE)
-
-        fig = make_subplots(
-            rows=n_plot_rows,
-            cols=PLOTS_PER_LINE,
-            subplot_titles = titles[start_idx:start_idx+n_plots],
-        )
-        for idx in range(1, (n_plot_rows*PLOTS_PER_LINE)+1):
-            fig.update_layout(
-                {
-                    f'xaxis{idx}':{'title_text': 'm/z'},
-                    f'yaxis{idx}':{'title_text': 'L<sup>2</sup> Normalized Intensity'},
-                }
-            )
-
-        plot_data = sub_df['plot_data'].tolist()
-        for idx, (traces, annotations) in enumerate(plot_data):
-            for trace in traces:
-                fig.add_trace(
-                    trace,
-                    row=1 + (idx//PLOTS_PER_LINE),
-                    col=1 + (idx%PLOTS_PER_LINE),
-                )
-
-            fig.layout['annotations'] += tuple(annotations)
-
-        for idx in range(sub_df.shape[0]):
-            fig.add_trace(
-                go.Scatter(
-                    x=[0, 1500],
-                    y=[0, 0],
-                    mode='lines',
-                    line={'width':0.5, 'color':'black'},
-                ),
-                row=1 + (idx//PLOTS_PER_LINE),
-                col=1 + (idx%PLOTS_PER_LINE),
-            )
-
-        fig.update_layout(
-            width=2100,
-            height=n_plot_rows*500,
-            paper_bgcolor='rgba(0,0,0,0)',
-            plot_bgcolor='rgba(0,0,0,0)',
-            showlegend=False,
-        )
-
-
-        fig.update_xaxes(
-            showticklabels=True,
-            range=[0, 1500],
-            dtick=300,
-            linecolor='black',
-            linewidth=0.5,
-            showgrid=False,
-            ticks="outside",
-        )
-
-        fig.update_yaxes(
-            showline=True,
-            linewidth=0.5,
-            linecolor='black',
-            range=[-1.2, 1.6],
-            tickvals = [-1.2+(i*0.4) for i in range(8)],
-            ticktext = [round(abs(-1.2+(i*0.4)), 1) for i in range(8)],
-            showgrid=False,
-            ticks="outside",
-        )
-
-        if not config.silent_execution:
-            fig.show()
-
-        pio.write_image(
-            fig,
-            f'{config.output_folder}/spectralPlots{group_idx}.pdf',
-            engine='kaleido',
-        )
-
-    merger = PdfFileMerger()
-    for group_idx in range(n_groups):
-        merger.append(
-            f'{config.output_folder}/spectralPlots{group_idx}.pdf'
-        )
-    merger.write(f'{config.output_folder}/spectralPlots.pdf')
-    for group_idx in range(n_groups):
-        os.remove(
-            f'{config.output_folder}/spectralPlots{group_idx}.pdf'
+    Returns
+    -------
+    df_row : pd.Series
+        The updated row containing prosit-delta features.
+    """
+    peptide = df_row[PEPTIDE_KEY]
+    mod_seq = df_row['modified_sequence'].replace('M(ox)', 'm')
+
+    true_l2_norm = np.linalg.norm(np.array(list(matched_dict.values())), ord=2)
+    normed_matched_dict = {k:v/true_l2_norm for k,v in matched_dict.items()}
+    pep_len = len(peptide)
+    flip_inds = np.array([
+        idx+1 for idx in range(
+            len(df_row[PEPTIDE_KEY])-1
+        ) if df_row[PEPTIDE_KEY][idx] != df_row[PEPTIDE_KEY][idx+1]
+    ])
+
+    if len(flip_inds):
+        input_feats = np.zeros(
+            shape=(len(flip_inds), len(DELTA_PRO_FEATURE_SET))
+        )
+        input_feats[:, SPECTRAL_ANGLE_INDEX] = df_row[SPECTRAL_ANGLE_KEY]
+        input_feats[:, BLOSUM_N_INDEX] = np.array([
+            BLOSUM6_1_VALUES[peptide[idx-1]] for idx in flip_inds
+        ])
+        input_feats[:, BLOSUM_C_INDEX] = np.array([
+            BLOSUM6_1_VALUES[peptide[idx]] for idx in flip_inds
+        ])
+        input_feats[:, CHARGE_INDEX] = df_row['charge']
+        input_feats[:, MATCHED_COV_INDEX] = df_row['matchedCoverage']
+        input_feats[:, CE_INDEX] = df_row['collisionEnergy']
+        input_feats[:, C_NEIGHB_INDEX] = np.array(
+            [-5.0 if idx > pep_len-3 else BLOSUM6_1_VALUES[peptide[idx+1]] for idx in flip_inds]
+        )
+        input_feats[:, N_NEIGHB_INDEX] = np.array(
+            [-5.0 if idx < 2 else BLOSUM6_1_VALUES[peptide[idx-2]] for idx in flip_inds]
+        )
+        input_feats[:, N_TERM_INDEX] = np.array(flip_inds)
+        input_feats[:, C_TERM_INDEX] = np.array([
+            [pep_len-idx for idx in flip_inds]
+        ])
+        input_feats[:, Y_NEW_INTE_INDEX] = np.array(
+            [get_new_inte(mod_seq, flip_ind, df_row, mz_accuracy, 'y') for flip_ind in flip_inds]
+        )
+        input_feats[:, B_NEW_INTE_INDEX] = np.array(
+            [get_new_inte(mod_seq, flip_ind, df_row, mz_accuracy, 'b') for flip_ind in flip_inds]
+        )
+        input_feats[:, Y_ERR_INDEX] = np.array(
+            [
+                get_err_at_loc(
+                    pep_len, normed_matched_dict, df_row[PROSIT_IONS_KEY], flip_ind, 'y'
+                ) for flip_ind in flip_inds
+            ]
+        )
+        input_feats[:, B_ERR_INDEX] = np.array(
+            [
+                get_err_at_loc(
+                    pep_len, normed_matched_dict, df_row[PROSIT_IONS_KEY], flip_ind, 'b'
+                ) for flip_ind in flip_inds
+            ]
+        )
+        input_feats[:, B_PROSIT_C_INTE_INDEX] = np.array(
+            [
+                get_intes_at_loc(
+                    pep_len,
+                    prosit_intes,
+                    prosit_ions,
+                    flip_idx+1,
+                    'b',
+                ) for flip_idx in flip_inds
+            ]
+        )
+        input_feats[:, Y_PROSIT_N_INTE_INDEX] = np.array(
+            [
+                get_intes_at_loc(
+                    pep_len,
+                    prosit_intes,
+                    prosit_ions,
+                    flip_idx-1,
+                    'y',
+                ) for flip_idx in flip_inds
+            ]
+        )
+        input_feats[:, Y_PROSIT_INTE_INDEX] = np.array(
+            [
+                get_intes_at_loc(
+                    pep_len,
+                    prosit_intes,
+                    prosit_ions,
+                    flip_idx,
+                    'y',
+                ) for flip_idx in flip_inds
+            ]
+        )
+        input_feats[:, B_PROSIT_INTE_INDEX] = np.array(
+            [
+                get_intes_at_loc(
+                    pep_len,
+                    prosit_intes,
+                    prosit_ions,
+                    flip_idx,
+                    'b',
+                ) for flip_idx in flip_inds
+            ]
+        )
+
+        input_feats[:, Y_MATCHED_N_INTE_INDEX] = np.array(
+            [
+                get_intes_at_loc(
+                    pep_len,
+                    matched_intes,
+                    prosit_ions,
+                    flip_idx-1,
+                    'y',
+                ) for flip_idx in flip_inds
+            ]
+        )
+        input_feats[:, B_MATCHED_C_INTE_INDEX] = np.array(
+            [
+                get_intes_at_loc(
+                    pep_len,
+                    matched_intes,
+                    prosit_ions,
+                    flip_idx+1,
+                    'b'
+                ) for flip_idx in flip_inds
+            ]
+        )
+        input_feats[:, Y_MATCHED_INTE_INDEX] = np.array(
+            [
+                get_intes_at_loc(
+                    pep_len,
+                    matched_intes,
+                    prosit_ions,
+                    flip_idx,
+                    'y'
+                ) for flip_idx in flip_inds
+            ]
+        )
+        input_feats[:, B_MATCHED_INTE_INDEX] = np.array(
+            [
+                get_intes_at_loc(
+                    pep_len,
+                    matched_intes,
+                    prosit_ions,
+                    flip_idx,
+                    'b'
+                ) for flip_idx in flip_inds
+            ]
+        )
+
+        input_feats[:, C_OX_INDEX] = np.array(
+            [
+                check_oxidation(
+                    pep_len,
+                    df_row[PTM_SEQ_KEY],
+                    flip_idx,
+                    ox_flag,
+                ) for flip_idx in flip_inds
+            ]
+        )
+        input_feats[:, N_OX_INDEX] = np.array(
+            [
+                check_oxidation(
+                    pep_len,
+                    df_row[PTM_SEQ_KEY],
+                    flip_idx-1,
+                    ox_flag,
+                ) for flip_idx in flip_inds
+            ]
         )
+
+        prot_deltas = reg_model.predict(input_feats)
+    else:
+        prot_deltas = np.array([])
+
+    return calculate_delta_features(df_row, prot_deltas)
```

### Comparing `inspirems-1.4/inspire/predict_spectra.py` & `inspirems-1.5/inspire/predict_spectra.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 """ Function for generating Prosit or MS2PIP spectral predictions.
 """
 from pathlib import Path
-from ms2pip.ms2pipC import MS2PIP
+try:
+    from ms2pip.ms2pipC import MS2PIP
+except ModuleNotFoundError:
+    print('Warning MS2PIP is not installed.')
 
 from inspire.prosit import (
     load_model, process_csv_file, prosit_predict, write_msp_file
 )
 
 PARAMS = {
     "ms2pip": {
@@ -63,20 +66,26 @@
 
         if pipeline =='core':
             input_file = f'{config.output_folder}/prositInput.csv'
             out_file = f'{config.output_folder}/prositPredictions.msp'
         elif pipeline == 'calibrate':
             input_file = f'{config.output_folder}/calibrationInput.csv'
             out_file = f'{config.output_folder}/calibrationPredictions.msp'
+        elif pipeline == 'spectralAngle':
+            input_file = f'{config.output_folder}/saInput.csv'
+            out_file = f'{config.output_folder}/saPredictions.msp'
         elif pipeline == 'validation':
             input_file = f'{config.output_folder}/validationInput.csv'
             out_file = f'{config.output_folder}/validationPredictions.msp'
-        else:
+        elif pipeline == 'plotSpectra':
             input_file = f'{config.output_folder}/plotInput.csv'
             out_file = f'{config.output_folder}/plotPredictions.msp'
+        else:
+            input_file = f'{config.output_folder}/plotisobarInput.csv'
+            out_file = f'{config.output_folder}/plotisobarPredictions.msp'
         input_df, prosit_input = process_csv_file(input_file)
 
         prosit_data = prosit_predict(prosit_input, d_irt)
         final_result = prosit_predict(prosit_data, d_spectra)
 
         write_msp_file(input_df, final_result, out_file)
```

### Comparing `inspirems-1.4/inspire/prepare.py` & `inspirems-1.5/inspire/prepare.py`

 * *Files identical despite different names*

### Comparing `inspirems-1.4/inspire/prosit.py` & `inspirems-1.5/inspire/prosit.py`

 * *Files identical despite different names*

### Comparing `inspirems-1.4/inspire/report.py` & `inspirems-1.5/inspire/report.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     )
 
     non_spectral_psm_df = apply_rescoring(
         output_folder,
         'non_spectral_perc_input.tab',
         fdr,
         rescore_method,
-        'non_spectral'
+        'non_spectral',
     ).rename(columns={OUT_PSM_ID_KEY[rescore_method]: psm_id_key})
 
     non_spectral_psm_df = pd.merge(
         non_spectral_psm_df,
         non_spectral_df[[psm_id_key, ENGINE_SCORE_KEY]],
         how='inner',
         on=psm_id_key,
```

### Comparing `inspirems-1.4/inspire/rescore.py` & `inspirems-1.5/inspire/rescore.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 def apply_rescoring(
         output_folder,
         input_filename,
         fdr,
         rescore_method,
         output_prefix,
+        results_out='psm',
     ):
     """ Function to apply percolator and return the PSMs matched.
 
     Parameters
     ----------
     perc_input_df : pd.DataFrame
         A DataFrame read for percolator input.
@@ -52,28 +53,33 @@
     -------
     results : pd.DataFrame
         The predictions from Percolator.
     """
     psm_output_key = f'{output_folder}/{output_prefix}.{rescore_method}.psms.txt'
     pep_output_key = f'{output_folder}/{output_prefix}.{rescore_method}.peptides.txt'
 
+    if results_out == 'psm':
+        export_loc = psm_output_key
+    else:
+        export_loc = pep_output_key
+
     if rescore_method == 'mokapot':
         rescore_name = 'mokapot'
         clis = (
-            f' --dest_dir {output_folder} --keep_decoys --verbosity 0 ' +
-            f' --train_fdr {fdr} -v 0 ' +
+            f' --dest_dir {output_folder} --keep_decoys  ' +
+            f' --train_fdr {fdr} ' +
             f' --test_fdr {fdr} --file_root {output_prefix} --save_models '
         )
         trailing_args = ''
     elif rescore_method == 'percolatorSeparate':
         rescore_name = 'percolator'
         percolator_decoy_key = f'{output_folder}/{output_prefix}.{rescore_method}.decoy.psms.txt'
         weights_path = f'{output_folder}/{output_prefix}.{rescore_method}.weights.csv'
         clis = (
-            f' -U -F {fdr} -t {fdr} -i 10 -M {percolator_decoy_key} --post-processing-tdc  ' +
+            f' -F {fdr} -t {fdr} -i 10 -M {percolator_decoy_key} --post-processing-tdc  ' +
             f' -w {weights_path} --override ' +
             f' --results-psms {psm_output_key} --results-peptides {pep_output_key} '
         )
         trailing_args = ''
     else:
         rescore_name = 'percolator'
         percolator_decoy_key = f'{output_folder}/{output_prefix}.{rescore_method}.decoy.psms.txt'
@@ -93,15 +99,16 @@
         subprocess.run(
             bash_command,
             check=True,
             shell=True,
             stdout=log_file,
         )
 
-    results = pd.read_csv(psm_output_key, sep='\t')
+    results = pd.read_csv(export_loc, sep='\t')
+    results[PEPTIDE_KEY] = results[PEPTIDE_KEY].apply(lambda x : x[2:-2])
 
     return results
 
 def _split_psm_ids(df_row, psm_id_key):
     """ Function for splitting a PSM Id back into its source name, scan number
         and peptide sequence.
 
@@ -165,16 +172,17 @@
         input_key,
         sep='\t',
     )
     input_df = input_df.drop_duplicates(subset=[psm_id_key, PEPTIDE_KEY])
 
     key_features = [
         SPECTRAL_ANGLE_KEY,
-        'matchedCoverage',
         RT_KEY,
+        'spearmanR',
+        'matchedCoverage',
         'deltaRT',
         ENGINE_SCORE_KEY,
         CHARGE_KEY,
     ]
     if config.use_accession_stratum:
         acc_cols = [x for x in input_df.columns if x.startswith('accession')]
         input_df[ACCESSION_STRATUM_KEY] = input_df.apply(
@@ -213,40 +221,27 @@
 
     target_psms = apply_rescoring(
         config.output_folder,
         in_path,
         config.fdr,
         config.rescore_method,
         output_prefix,
+        config.results_export,
     )
 
     if 'PSMId' in target_psms.columns:
         target_psms = target_psms.rename( # pylint: disable=no-member
             columns={'PSMId': psm_id_key}
         )
 
     print(
         OKCYAN_TEXT + '\tRescoring complete.' + ENDC_TEXT
     )
     output_df, key_features = _add_key_features(target_psms, config)
 
-    output_df = output_df.apply(
-       lambda x: _split_psm_ids(x, psm_id_key),
-       axis=1
-    ).drop(psm_id_key, axis=1)
-
-    output_df = output_df.rename(
-        columns={
-            out_score_key: FINAL_SCORE_KEY,
-            out_q_key: FINAL_Q_VALUE_KEY,
-            out_accession_key: ACCESSION_KEY,
-            out_postep_key: FINAL_POSTEP_KEY,
-        }
-    )
-
     final_columns = (
         [
             SOURCE_KEY,
             SCAN_KEY,
             PEPTIDE_KEY,
             'modifiedSequence',
             FINAL_SCORE_KEY,
@@ -254,20 +249,59 @@
             FINAL_POSTEP_KEY,
         ] + key_features +
         [
             ACCESSION_KEY
         ]
     )
 
+    output_df = output_df.apply(
+       lambda x: _split_psm_ids(x, psm_id_key),
+       axis=1
+    ).drop(psm_id_key, axis=1)
+
+    if config.results_export == 'peptide':
+        psms_df = pd.read_csv(
+            f'{config.output_folder}/final.{config.rescore_method}.psms.txt',
+            sep='\t',
+        )
+        psms_df[PEPTIDE_KEY] = psms_df[PEPTIDE_KEY].apply(lambda x : x[2:-2])
+        if 'PSMId' in psms_df.columns:
+            psms_df = psms_df.rename( # pylint: disable=no-member
+                columns={'PSMId': psm_id_key}
+            )
+        psms_df, key_features = _add_key_features(psms_df, config)
+        psms_df = psms_df.apply(
+            lambda x: _split_psm_ids(x, psm_id_key),
+            axis=1
+        ).drop(psm_id_key, axis=1)
+        psms_df = psms_df.rename(
+            columns={
+                out_score_key: FINAL_SCORE_KEY,
+                out_q_key: FINAL_Q_VALUE_KEY,
+                out_accession_key: ACCESSION_KEY,
+                out_postep_key: FINAL_POSTEP_KEY,
+                }
+        )
+
+        psms_df = psms_df[final_columns]
+        psms_df.to_csv(
+            f'{config.output_folder}/finalPsmAssignments.csv',
+            index=False
+        )
+
+    output_df = output_df.rename(
+        columns={
+            out_score_key: FINAL_SCORE_KEY,
+            out_q_key: FINAL_Q_VALUE_KEY,
+            out_accession_key: ACCESSION_KEY,
+            out_postep_key: FINAL_POSTEP_KEY,
+        }
+    )
+
     output_df = output_df[final_columns]
 
     output_df = output_df.sort_values(by=FINAL_SCORE_KEY, ascending=False)
 
-    if config.use_accession_stratum:
-        out_path = f'{config.output_folder}/pre_finalAssignments.csv'
-    else:
-        out_path = f'{config.output_folder}/finalAssignments.csv'
-
-    output_df.to_csv(out_path, index=False)
+    output_df.to_csv(f'{config.output_folder}/finalAssignments.csv', index=False)
     print(
         OKCYAN_TEXT + '\tFinal assignments written to csv.' + ENDC_TEXT
     )
```

### Comparing `inspirems-1.4/inspire/run.py` & `inspirems-1.5/inspire/run.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,45 +7,51 @@
 import pandas as pd
 import tensorflow as tf
 
 from inspire.calibration import calibrate
 from inspire.config import Config
 from inspire.constants import ENDC_TEXT, OKGREEN_TEXT
 from inspire.download import download_data, download_models
+from inspire.get_spectral_angle import get_spectral_angle
 from inspire.plot_spectra import plot_spectra
+from inspire.plot_isobars import plot_isobars
 from inspire.predict_spectra import predict_spectra
 from inspire.prepare import prepare_for_spectral_prediction, prepare_for_mhcpan
 from inspire.feature_creation import create_features
 from inspire.feature_selection import select_features
 from inspire.rescore import final_rescoring
 from inspire.report import generate_report
 from inspire.utils import fetch_collision_energy
 from inspire.validate import validate_spliced
+
 import inspire
 
 print(f'\n---> Running inSPIRE version {inspire.__version__} <---\n')
 pd.options.mode.chained_assignment = None
 tf.config.set_visible_devices([], 'GPU')
 
 PIPELINE_OPTIONS = [
     'calibrate',
     'core',
     'downloadExample',
     'prepare',
+    'plotIsobars',
     'spectralPrepare',
     'panPrepare',
     'predictSpectra',
     'rescore',
     'featureGeneration',
     'featureSelection',
     'featureSelection+',
     'finalRescoring',
     'queryTable',
     'generateReport',
     'plotSpectra',
+    'spectralAngle',
+    'validate',
 ]
 
 def get_arguments():
     """ Function to collect command line arguments.
 
     Returns
     -------
@@ -145,42 +151,59 @@
             OKGREEN_TEXT +
             'Running Finalised Rescoring...' +
             ENDC_TEXT
         )
         final_rescoring(config)
 
     if (
+        args.pipeline in ('featureSelection+', 'rescore', 'core') and not config.silent_execution
+    ) or args.pipeline == 'generateReport':
+        print(
+            OKGREEN_TEXT +
+            'Generating inSPIRE Performance Report...' +
+            ENDC_TEXT
+        )
+        generate_report(config)
+
+    if (
         args.pipeline in ('validate', 'featureSelection+', 'rescore', 'core', 'calibrate+core')
         and config.use_accession_stratum
     ):
         print(
             OKGREEN_TEXT +
             'Validating spliced assignments...' +
             ENDC_TEXT
         )
         validate_spliced(config)
 
-    if (
-        args.pipeline in ('featureSelection+', 'rescore', 'core') and not config.silent_execution
-    ) or args.pipeline == 'generateReport':
+    if args.pipeline == 'spectralAngle':
         print(
             OKGREEN_TEXT +
-            'Generating inSPIRE Performance Report...' +
+            'Calculating Spectral Angles...' +
             ENDC_TEXT
         )
-        generate_report(config)
+        get_spectral_angle(config)
 
     if args.pipeline == 'plotSpectra':
         print(
             OKGREEN_TEXT +
             'Plotting Spectra...' +
             ENDC_TEXT
         )
         plot_spectra(config)
 
+    if args.pipeline == 'plotIsobars':
+        print(
+            OKGREEN_TEXT +
+            'Plotting Isobars...' +
+            ENDC_TEXT
+        )
+        plot_isobars(config)
+
+
     print(
         OKGREEN_TEXT +
         f'inSPIRE Pipeline "{args.pipeline}" Complete!' +
         ENDC_TEXT
     )
 
 if __name__ == '__main__':
```

### Comparing `inspirems-1.4/inspire/spectral_features.py` & `inspirems-1.5/inspire/spectral_features.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,15 @@
     # Loop over observed fragments matching them to all possible prosit ions.
     ordered_prosit = np.array(list(prosit_intensities.keys()), dtype='object')
     final_intensities = np.zeros(len(prosit_intensities))
     possible_loss_ions = []
     mz_errors = []
     assigned_inds = []
 
-    max_frag_charge = min(4, precursor_z+1)
+    max_frag_charge = min(4, precursor_z+1) #TODO we only care about the Prosit  ions
     match_idx = 0
     for ion_type in all_prosit_masses:
         for charge in range(1, max_frag_charge):
             for fragment_idx in range(len(all_prosit_masses[ion_type])):
                 ion_code = f'{ion_type}{fragment_idx+1}'
                 if charge > 1:
                     ion_code += f'^{charge}'
@@ -362,14 +362,16 @@
     matched_intensities = match_info['matched_intensities']
     ordered_prosit_ions = match_info['ordered_prosit_ions']
     ordered_prosit_intes = match_info['ordered_prosit_intes']
     truly_matched_intes = matched_intensities[matched_intensities > 0.0]
 
 
     median_mz_error, mz_error_variance = get_mz_error_stats(mz_errors, min(mz_accuracy, 0.04))
+    df_row[FRAG_MZ_ERR_MED_KEY] = median_mz_error
+    df_row[FRAG_MZ_ERR_VAR_KEY] = mz_error_variance
 
     matched_l2_norm = np.linalg.norm(matched_intensities, ord=2)
     total_l2_norm = np.linalg.norm(df_row[INTENSITIES_KEY], ord=2)
 
     if matched_l2_norm:
         normed_matched_intensities = matched_intensities/matched_l2_norm
     else:
@@ -385,18 +387,37 @@
     df_row = get_coverage_features(
         df_row,
         seq_len,
         ordered_matched_ions,
         ordered_prosit_ions,
     )
 
+    if len(truly_matched_intes) > 0:
+        spearman_total = spearmanr(normed_matched_intensities, ordered_prosit_intes)[0]
+        pearson_total = pearsonr(normed_matched_intensities, ordered_prosit_intes)[0]
+        if not np.isnan(spearman_total):
+            df_row[SPEARMAN_KEY] = spearman_total
+        else:
+            df_row[SPEARMAN_KEY] = 0.0
+        if not np.isnan(pearson_total):
+            df_row[PEARSON_KEY] = pearson_total
+        else:
+            df_row[PEARSON_KEY] = -1.0
+    else:
+        df_row[SPEARMAN_KEY] = 0.0
+        df_row[PEARSON_KEY] = 0.0
+
     if minimal_features:
         return df_row
 
-    df_row['spectrumDensity'] = len(df_row[MZS_KEY])/(df_row[MZS_KEY].max() - df_row[MZS_KEY].min())
+    mz_range = (df_row[MZS_KEY].max() - df_row[MZS_KEY].min())
+    if mz_range > 0:
+        df_row['spectrumDensity'] = len(df_row[MZS_KEY])/mz_range
+    else:
+        df_row['spectrumDensity'] = 1.0
 
     major_pred_inds = (ordered_prosit_intes >= PROSIT_MAJOR_MINOR_CUT_OFF)
 
     major_prosit_preds = ordered_prosit_intes[major_pred_inds]
     minor_prosit_preds = ordered_prosit_intes[~major_pred_inds]
 
     major_matched_ions = normed_matched_intensities[major_pred_inds]
@@ -457,28 +478,14 @@
     df_row['nMajorPredNotFoundDivFrags'] = (n_major_pred - n_major_matched)/n_frags_possible
 
     df_row[MAE_KEY] = median_absolute_error(
         normed_matched_intensities,
         ordered_prosit_intes,
     )
 
-    if len(truly_matched_intes) > 0:
-        spearman_total = spearmanr(normed_matched_intensities, ordered_prosit_intes)[0]
-        pearson_total = pearsonr(normed_matched_intensities, ordered_prosit_intes)[0]
-        if not np.isnan(spearman_total):
-            df_row[SPEARMAN_KEY] = spearman_total
-        else:
-            df_row[SPEARMAN_KEY] = 0.0
-        if not np.isnan(pearson_total):
-            df_row[PEARSON_KEY] = pearson_total
-        else:
-            df_row[PEARSON_KEY] = -1.0
-    else:
-        df_row[SPEARMAN_KEY] = 0.0
-        df_row[PEARSON_KEY] = 0.0
     df_row['nMajorMatchedDivFrags'] = n_major_matched/n_frags_possible
     df_row['nMinorMatchedDivFrags'] = n_minor_matched/n_frags_possible
     df_row[MATCHED_IONS_KEY] = len(truly_matched_intes)/n_frags_possible
 
     df_row['nMajorNotMatchableDivFrags'] = n_major_not_matchable/n_frags_possible
     df_row['nMinorNotMatchableDivFrags'] = n_minor_not_matchable/n_frags_possible
 
@@ -487,16 +494,14 @@
 
 
     if precursor_inte:
         df_row[PRECURSOR_INTE_KEY] = precursor_inte/(matched_l2_norm+precursor_inte)
     else:
         df_row[PRECURSOR_INTE_KEY] = 0.0
 
-    df_row[FRAG_MZ_ERR_MED_KEY] = median_mz_error
-    df_row[FRAG_MZ_ERR_VAR_KEY] = mz_error_variance
 
     df_row = get_kr_feats(
         sequence, matched_intensities, ordered_prosit_intes, ordered_prosit_ions, df_row
     )
 
     pred_not_found_ions = ordered_prosit_ions[matched_intensities == 0.0]
```

### Comparing `inspirems-1.4/inspire/utils.py` & `inspirems-1.5/inspire/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 """
 import pickle
 import re
 
 import pandas as pd
 
 from inspire.constants import (
+    ACCESSION_STRATUM_KEY,
     CHARGE_KEY,
+    ENGINE_SCORE_KEY,
     KNOWN_PTM_LOC,
     KNOWN_PTM_WEIGHTS,
     PEPTIDE_KEY,
     PTM_ID_KEY,
     PTM_IS_VAR_KEY,
     PTM_NAME_KEY,
     PTM_SEQ_KEY,
@@ -140,15 +142,17 @@
 
     Returns
     -------
     ox_flag : int
         The flag for oxidation of methionine.
     """
     try:
-        ox_flag = mods_df[mods_df[PTM_NAME_KEY] == 'Oxidation (M)'].index[0] + 1
+        ox_flag = int(
+            mods_df[mods_df[PTM_NAME_KEY] == 'Oxidation (M)'][PTM_ID_KEY].iloc[0]
+        )
     except IndexError:
         ox_flag = -1
 
     return ox_flag
 
 def get_mokapot_weights(output_folder, inspire_step):
     """ Function to get the weights of mokapot models.
@@ -244,34 +248,103 @@
     """
     if source.endswith('.mzML'):
         return source[:-5]
     if source.endswith('.raw') or source.endswith('.mgf'):
         return source[:-4]
     return source
 
-def filter_for_prosit(search_df):
+def _check_prosit_compliant_peptide(df_row):
+    """ Helper function to check that a peptide is within the Prosit length restricitons
+        and does not contain any non-standard amino acids.
+
+    Parameters
+    ----------
+    peptide : str
+        A peptide to be checked.
+
+    Returns
+    -------
+    prosit_compliant : bool
+        Whether the peptide is within the restrictions of Prosit.
+    """ 
+    peptide = df_row[PEPTIDE_KEY]
+    if not isinstance(peptide, str):
+        return False
+    if len(peptide) < 7 or len(peptide) > 30:
+        return False
+    for non_standard_aa in 'BJOUXZ':
+        if non_standard_aa in peptide:
+            return False
+    if df_row[CHARGE_KEY] > 6:
+        return False
+    return True
+
+def get_mod_score(df_row):
+    """ Helper function to compare different accession strata.
+    """
+    if df_row[ACCESSION_STRATUM_KEY] == 0:
+        return df_row[ENGINE_SCORE_KEY]
+    return 0.7*df_row[ENGINE_SCORE_KEY]
+
+def accession_informed_filter(target_df, drop_feature_key):
+    """ Function for filtering with competitors from lower accession strata excluded.
+    """
+    target_df['modEngineScore'] = target_df[
+        [ENGINE_SCORE_KEY, ACCESSION_STRATUM_KEY]
+    ].apply(get_mod_score, axis=1)
+    target_df['maxModScore'] = target_df.groupby(
+        [SOURCE_KEY, SCAN_KEY]
+    )['modEngineScore'].transform(max)
+
+    top_rank_mod_df = target_df[
+        (target_df[drop_feature_key]) &
+        (target_df['maxModScore'] == target_df['modEngineScore'])
+    ]
+    top_rank_mod_df = top_rank_mod_df[[SOURCE_KEY, SCAN_KEY]].drop_duplicates()
+    top_rank_mod_df['drop'] = 'yes'
+    target_df = target_df[
+        ~target_df[drop_feature_key]
+    ].drop(['modEngineScore', 'maxModScore', drop_feature_key], axis=1)
+
+    target_df = pd.merge(
+        target_df,
+        top_rank_mod_df,
+        how='left',
+        on=[SOURCE_KEY, SCAN_KEY]
+    )
+    target_df = target_df[target_df['drop'] != 'yes']
+    target_df = target_df.drop('drop', axis=1)
+    return target_df
+
+def filter_for_prosit(search_df, use_accession_stratum):
     """ Function to filter sequences not suitable for Prosit input.
 
     Parameters
     ----------
     search_df : pd.DataFrame
         A DataFrame of search results from an ms search engine.
+    use_accession_stratum : bool
+        Whether accession stratum is being used as a feature.
 
     Returns
     -------
     search_df : pd.DataFrame
         The input DataFrame with sequences not suitable for Prosit input removed.
     """
     search_df = search_df.dropna(subset=[PEPTIDE_KEY, CHARGE_KEY])
-    search_df_filter = search_df[PEPTIDE_KEY].apply(
-        lambda x : isinstance(x, str) and 'U' not in x and len(x) > 6 and len(x) < 31
+    search_df_filter = search_df[[PEPTIDE_KEY, CHARGE_KEY]].apply(
+        _check_prosit_compliant_peptide, axis=1
     )
-    search_df = search_df[search_df_filter]
-    search_df = search_df[search_df[CHARGE_KEY] < 7]
-    search_df.reset_index(drop=True, inplace=True)
+    if use_accession_stratum:
+        search_df['prositNonCompliant'] = ~search_df_filter
+        search_df = accession_informed_filter(search_df, 'prositNonCompliant')
+    else:
+        search_df = search_df[search_df_filter]
+        search_df.reset_index(drop=True, inplace=True)
+
     return search_df
 
 def _modify_ptm_seq(pep_seq, ptm_seq, ptm_locs, ptm_id):
     """ Helper function to add a fixed PTM to the ptm_seq column of MS search
         result DataFrame.
 
     Parameters
```

### Comparing `inspirems-1.4/inspire/validate.py` & `inspirems-1.5/inspire/validate.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 """
 import itertools
 import re
 
 from Bio import SeqIO
 import numpy as np
 import pandas as pd
+from scipy.stats import spearmanr
 
 from inspire.constants import (
     CHARGE_KEY,
     KNOWN_PTM_WEIGHTS,
     MINIMAL_FEATURE_SET,
     PROSIT_IONS_KEY,
     PROTON,
     RESIDUE_WEIGHTS,
     SCAN_KEY,
+    SPEARMAN_KEY,
     SOURCE_KEY,
 )
 from inspire.input.msp import msp_to_df
 from inspire.predict_spectra import predict_spectra
 from inspire.spectral_features import (
     calculate_spectral_angle,
     get_coverage,
@@ -95,18 +97,21 @@
     else:
         normed_matched_intensities = matched_intensities
 
     df_row['spectralAngle'] = calculate_spectral_angle(
         normed_matched_intensities,
         ordered_prosit_intes,
     )
-    ordered_matched_ions = ordered_prosit_ions[matched_intensities > 0.0]
-    df_row['matchedCoverage'], _, __ = get_coverage(
-        seq_len, ordered_matched_ions, per_letter=True
-    )
+    spearman_total = spearmanr(normed_matched_intensities, ordered_prosit_intes)[0]
+
+    if not np.isnan(spearman_total):
+        df_row[SPEARMAN_KEY] = spearman_total
+    else:
+        df_row[SPEARMAN_KEY] = 0.0
+
     return df_row
 
 
 
 def get_cleavage_peptides(proteome_loc):
     """ Function to find all nonspliced peptides.
     """
@@ -148,35 +153,29 @@
     for possible_os in possible_oxidations:
         mod_str = pcp_pep
         for o_site in sorted(possible_os, reverse=True):
             mod_str = mod_str[:o_site+1] + '[+16.0]' + mod_str[o_site+1:]
         possible_mod_seqs.append(mod_str)
     return possible_mod_seqs
 
-def find_competitors(config):
+def find_competitors(final_df, config):
     """ Function to find isobaric nonspliced competitors to spliced peptides.
     """
-    final_df = pd.read_csv(
-        f'{config.output_folder}/pre_finalAssignments.csv'
-    )
-
     final_df = final_df[
-        (final_df['qValue'] < 0.01) &
         (final_df['accessionGroup'] == 'spliced')
     ]
 
     final_df['mw'] = final_df['peptide'].apply(
         lambda x : round(sum([RESIDUE_WEIGHTS[z] for z in x]), 2)
     )
 
     pcp_df = get_cleavage_peptides(config.proteome)
     pcp_df = pcp_df.drop_duplicates()
     pcp_df['label'] = 1
 
-
     merged_df = pd.merge(
         final_df[[
             'source',
             'scan',
             'peptide',
             'modifiedSequence',
             'charge',
@@ -196,28 +195,25 @@
     )
     merged_df = merged_df.explode('matched_pcps')
     merged_df = merged_df[merged_df['matched_pcps'].apply(lambda x : isinstance(x, str))]
     merged_df = merged_df.sort_values('peptide')
     merged_df['modified_sequence'] = merged_df['matched_pcps'].apply(
         lambda x : x.replace('[+16.0]', '(ox)').replace('[+57.0]', '')
     )
-    merged_df.to_csv(
-        f'{config.output_folder}/cleavageCompetitors.csv',
-        index=False
-    )
-    merged_df['collision_energy'] = config.collision_energy
-    merged_df = merged_df.rename(columns={'charge': 'precursor_charge'})
-    prosit_input_df = merged_df[[
+
+    prosit_input_df = merged_df.rename(columns={'charge': 'precursor_charge'})
+    prosit_input_df['collision_energy'] = config.collision_energy
+    prosit_input_df = prosit_input_df[[
         'modified_sequence', 'precursor_charge', 'collision_energy'
     ]].drop_duplicates()
     prosit_input_df.to_csv(
         f'{config.output_folder}/validationInput.csv', index=False
     )
     predict_spectra(config, 'validation')
-    return merged_df.shape[0]
+    return merged_df
 
 def calculate_competitor_spectral_data(competitors_df, config):
     """ Function to calculate spectral angles for isobaric nonspliced competitors.
     """
     scan_df = fetch_scan_data(competitors_df, config, with_charge=False)
     competitors_df = pd.merge(
         competitors_df,
@@ -245,93 +241,83 @@
         lambda x : get_sa(x, config.mz_accuracy, config.mz_units),
         axis=1
     )
     return competitors_df
 
 def validate_spliced(config):
     """ Funciton to validate spliced PSMs against isobaric nonspliced competitors.
-
     Parameters
     ----------
     config : inspire.config.Config
         The Config object for the experiment.
     """
-    n_competitors = find_competitors(config)
-
-    if not n_competitors:
-        final_df = pd.read_csv(
-            f'{config.output_folder}/pre_finalAssignments.csv'
-        )
-
-        final_df = final_df[
-            (final_df['spectralAngle'] > 0.7) &
-            (final_df['deltaRT'] < 150) &
-            (final_df['qValue'] < 0.01)
-        ]
+    final_df = pd.read_csv(
+        f'{config.output_folder}/finalAssignments.csv'
+    )
+    final_df = final_df[final_df['qValue'] < 0.01]
+    if config.contaminant_data is not None:
+        final_df = filter_contaminants(final_df, config)
+    competitors_df = find_competitors(final_df, config)
 
+    if not competitors_df.shape[0]:
         final_df.to_csv(
-            f'{config.output_folder}/finalAssignments.csv',
+            f'{config.output_folder}/filtered_finalAssignments.csv',
             index=False,
         )
-        return
 
-    competitors_df = pd.read_csv(f'{config.output_folder}/cleavageCompetitors.csv')
     competitors_df = calculate_competitor_spectral_data(competitors_df, config)
 
-    if config.combined_scans_file is None:
-        rt_ints = {}
-        rt_coefs = {}
-        for raw_file in competitors_df[SOURCE_KEY].unique().tolist():
-            rt_df = pd.read_csv(
-                f'{config.output_folder}/rt_fit_{raw_file}.csv'
-            )
-            rt_ints[raw_file] = rt_df['intercepts'].mean()
-            rt_coefs[raw_file] = rt_df['coefficents'].mean()
-
-        competitors_df['deltaRT'] = competitors_df.apply(
-            lambda x : abs(
-                x['retentionTime'] - (rt_ints[x['source']] + (rt_coefs[x['source']]*x['iRT']))
-            ),
-            axis=1,
-        )
-    else:
+    rt_ints = {}
+    rt_coefs = {}
+    for raw_file in competitors_df[SOURCE_KEY].unique().tolist():
         rt_df = pd.read_csv(
-            f'{config.output_folder}/rt_fit_{config.combined_scans_file[:-4]}.csv'
-        )
-        rt_int = rt_df['intercepts'].mean()
-        rt_coef = rt_df['coefficents'].mean()
-        competitors_df['deltaRT'] = competitors_df.apply(
-            lambda x : abs(x['retentionTime'] - (rt_int + (rt_coef*x['iRT']))),
-            axis=1
+            f'{config.output_folder}/rt_fit_{raw_file}.csv'
         )
+        rt_ints[raw_file] = rt_df['intercepts'].mean()
+
+        rt_coefs[raw_file] = rt_df['coefficents'].mean()
+
+    competitors_df['predRT'] = competitors_df.apply(
+        lambda x : rt_ints[x['source']] + (rt_coefs[x['source']]*x['iRT']),
+        axis=1,
+    )
+    competitors_df['base_deltaRT'] = competitors_df.apply(
+        lambda x : abs(
+            (x['retentionTime'] - x['predRT'])
+        ),
+        axis=1,
+    )
+    competitors_df['deltaRT'] = competitors_df.apply(
+        lambda x : abs(
+            abs(
+                x['base_deltaRT']/rt_coefs.get(x['source'], 1.0)
+            ) if rt_coefs.get(x['source'], 1.0) > 0 else x['base_deltaRT']
+        ),
+        axis=1
+    )
 
     competitors_df['accession_spliced'] = 0
     competitors_df['accession_nonspliced'] = 1
+    competitors_df.drop(
+        ['matched_pcps','intensities','mzs','prositIons','iRT'], axis=1,
+    ).sort_values(by='spectralAngle', ascending=False).to_csv(
+        f'{config.output_folder}/cleavageCompetitors.csv',
+        index=False,
+    )
 
     weights_df = pd.read_csv(
         f'{config.output_folder}/final.percolatorSeparate.weights.csv',
         skiprows=lambda x : x not in [0, 2, 5, 8],
         sep='\t',
     )
 
-    feature_set = MINIMAL_FEATURE_SET + ['accession_nonspliced', 'accession_spliced']
-    no_rt_feats = [
-        a for a in feature_set if a != 'deltaRT'
-    ]
-    if 'deltaRT' in weights_df.columns:
-        scores = np.matmul(
-            competitors_df[feature_set].values,
-            weights_df[feature_set].transpose().values
-        )
-    else:
-        scores = np.matmul(
-            competitors_df[no_rt_feats].values,
-            weights_df[no_rt_feats].transpose().values
-        )
-
+    scores = np.matmul(
+        competitors_df[MINIMAL_FEATURE_SET].values,
+        weights_df[MINIMAL_FEATURE_SET].transpose().values
+    )
 
     bias_terms = weights_df['m0'].values
     scores += bias_terms.transpose()
 
     final_scores = np.average(scores, axis=1)
 
     competitors_df['compScore'] = final_scores
@@ -339,48 +325,65 @@
     competitors_df = competitors_df.drop_duplicates(subset=[SOURCE_KEY, SCAN_KEY])
 
     competitors_df = competitors_df.reset_index(drop=True)
     competitors_df['group'] = competitors_df.index // 10
     competitors_df['index'] = competitors_df.index % 10
 
     final_df = pd.read_csv(
-        f'{config.output_folder}/pre_finalAssignments.csv'
+        f'{config.output_folder}/finalAssignments.csv'
     )
-
+    for possible_col in ['pcpPeptide',' modified_sequence']:
+        if possible_col in final_df.columns:
+            final_df = final_df.drop(possible_col, axis=1)
 
     final_df = pd.merge(
         final_df,
-        competitors_df[[SOURCE_KEY, SCAN_KEY, 'compScore', 'group', 'index']],
+        competitors_df[[SOURCE_KEY, SCAN_KEY, 'pcpPeptide', 'modified_sequence', 'compScore', 'group', 'index']],
         how='left',
         on=[SOURCE_KEY, SCAN_KEY]
     )
+    final_df[final_df['pcpPeptide'].apply(lambda x : isinstance(x, str))].to_csv(f'{config.output_folder}/competitorPsp.csv')
+    for raw_file in final_df[SOURCE_KEY].unique().tolist():
+        rt_df = pd.read_csv(
+            f'{config.output_folder}/rt_fit_{raw_file}.csv'
+        )
+        rt_ints[raw_file] = rt_df['intercepts'].mean()
+        rt_coefs[raw_file] = rt_df['coefficents'].mean()
+
+    final_df['deltaRT'] = final_df.apply(
+        lambda x : abs(
+            x['deltaRT']/rt_coefs.get(x['source'], 1.0) if rt_coefs.get(x['source'], 1.0) > 0 else x['deltaRT']
+        ),
+        axis=1,
+    )
+
     final_df['accession_nonspliced'] = final_df['accessionGroup'].apply(
         lambda x : 1 if x == 'nonspliced' else 0
     )
     final_df['accession_spliced'] = final_df['accessionGroup'].apply(
         lambda x : 1 if x == 'spliced' else 0
     )
-    if 'deltaRT' in weights_df.columns:
-        re_scores = np.matmul(
-            final_df[feature_set].values,
-            weights_df[feature_set].transpose().values
-        )
-    else:
-        re_scores = np.matmul(
-            final_df[no_rt_feats].values,
-            weights_df[no_rt_feats].transpose().values
-        )
+    re_scores = np.matmul(
+        final_df[MINIMAL_FEATURE_SET].values,
+        weights_df[MINIMAL_FEATURE_SET].transpose().values
+    )
+
     re_scores += bias_terms
     final_df['reScore1'] = re_scores[:,0]
-    final_df['reScore2'] = re_scores[:,0]
-    final_df['reScore3'] = re_scores[:,1]
+    final_df['reScore2'] = re_scores[:,1]
+    final_df['reScore3'] = re_scores[:,2]
     final_df['reScore'] = np.average(re_scores, axis=1)
 
     final_df['compScore']  = final_df['compScore'].fillna(-100_000)
 
+    final_df[final_df.apply(
+        lambda x : x['compScore'] is not None and x['reScore'] < x['compScore'],
+        axis=1,
+    )].to_csv(f'{config.output_folder}/knockout.csv', index=False)
+
     final_df = final_df[final_df.apply(
         lambda x : x['compScore'] is None or x['reScore'] > x['compScore'],
         axis=1,
     )]
 
     final_df = final_df.drop(['compScore'], axis=1)
     final_df = final_df.drop(
@@ -393,17 +396,70 @@
             'reScore2',
             'reScore3',
             'reScore',
         ],
         axis=1,
     )
 
+    final_df.to_csv(
+        f'{config.output_folder}/filtered_finalAssignments.csv',
+        index=False,
+    )
+
+
+def _separate_psm_id(df_row):
+    """ Function to separate contaminant assignments.
+    """
+    split_psm_id = df_row['specID'].split('_')
+    source = '_'.join(split_psm_id[:-2])
+    scan = int(split_psm_id[-2])
+    mod_pep = split_psm_id[-1]
+    df_row['source'] = source
+    df_row['scan'] = scan
+    df_row['contModPep'] = mod_pep
+    df_row['contPeptide'] = mod_pep.replace('[+1.0]', '').replace('[+16.0]', '').replace('[+57.0]', '')
+    return df_row
+
+def cont_filter(df_row):
+    if not isinstance(df_row['contPeptide'], str):
+        return True
+    if df_row['peptide'].replace('I', 'L') == df_row['contPeptide'].replace('I', 'L'):
+        return True
+    if df_row['spectralAngle'] < df_row['contamSA']:
+        return False
+    return True
+
+
+def filter_contaminants(final_df, config):
     final_df = final_df[
-        (final_df['spectralAngle'] > 0.7) &
-        (final_df['deltaRT'] < 150) &
         (final_df['qValue'] < 0.01)
     ]
 
-    final_df.to_csv(
-        f'{config.output_folder}/finalAssignments.csv',
-        index=False,
+    contam_df = pd.read_csv(
+        config.contaminant_data, sep='\t'
+    )
+
+    contam_df = contam_df[['specID', 'deltaRT', 'spectralAngle']]
+    contam_df = contam_df[
+        (contam_df['spectralAngle'] > final_df['spectralAngle'].min()*0.9)
+    ]
+    contam_df = contam_df.apply(_separate_psm_id, axis=1)
+    contam_df = contam_df.sort_values(by='spectralAngle', ascending=False)
+    contam_df = contam_df.drop_duplicates(subset=['source', 'scan'])
+    contam_df = contam_df.drop(['specID'], axis=1)
+    contam_df = contam_df.rename(columns={
+        'spectralAngle': 'contamSA',
+        'deltaRT': 'contamDeltaRT',
+    })
+    contam_df = contam_df[['source', 'scan', 'contPeptide', 'contamSA']]
+
+    final_df = pd.merge(
+        final_df,
+        contam_df,
+        how='left',
+        on=['source', 'scan'],
     )
+
+    filtered_final_df = final_df[final_df.apply(cont_filter, axis=1)]
+    filtered_final_df = filtered_final_df.drop(['contamSA', 'contPeptide'], axis=1)
+
+    return filtered_final_df
```

### Comparing `inspirems-1.4/inspirems.egg-info/PKG-INFO` & `inspirems-1.5/inspirems.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: inspirems
-Version: 1.4
+Version: 1.5
 Summary: Helping to integrate Spectral Predictors and Rescoring.
 Author: John Cormican, Juliane Liepe
 Author-email: juliane.liepe@mpinat.mpg.de
 Project-URL: Homepage, https://github.com/QuantSysBio/inSPIRE
 Project-URL: Tracker, https://github.com/QuantSysBio/inSPIRE/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: ms2pip
 License-File: LICENSE
 
 # inSPIRE
 
 <img src="https://raw.githubusercontent.com/QuantSysBio/inSPIRE/master/img/inSPIRE-logo.png" alt="drawing" width="200"/>
 
 <i>in silico</i> Spectral Predictor Informed REscoring
@@ -48,14 +49,20 @@
 
 4) To check your installation, run the following command (it is normal for this call to hang for a few seconds on first execution)
 
 ```
 inspire -h
 ```
 
+5) (Optional) If you wish to use Percolator for rescoring rather than Mokapot you will need to install it separately. On Linux, Percolator can be installed via conda with the command below. Otherwise see https://github.com/percolator/percolator.
+
+```
+conda install -c bioconda percolator
+```
+
 Once you have successfully installed inSPIRE you should run it specifying your pipeline and a config file. The core execution of inSPIRE will take the form:
 
 ```
 inspire --config_file path-to-config-file --pipeline pipeline-to-execute
 ```
 
 where the config file is a yaml file specifying details of the inSPIRE execution and the pipeline is one of the options described below.
```

### Comparing `inspirems-1.4/inspirems.egg-info/SOURCES.txt` & `inspirems-1.5/inspirems.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 inspire/download.py
 inspire/feature_creation.py
 inspire/feature_selection.py
 inspire/figures.py
 inspire/get_spectral_angle.py
 inspire/html_template.py
 inspire/mz_match.py
+inspire/plot_isobars.py
 inspire/plot_spectra.py
 inspire/predict_spectra.py
 inspire/prepare.py
 inspire/prosit.py
 inspire/prosit_delta.py
 inspire/report.py
 inspire/rescore.py
@@ -27,14 +28,15 @@
 inspire/utils.py
 inspire/validate.py
 inspire/input/__init__.py
 inspire/input/mascot.py
 inspire/input/maxquant.py
 inspire/input/mgf.py
 inspire/input/mhcpan.py
+inspire/input/msfragger.py
 inspire/input/msp.py
 inspire/input/mzml.py
 inspire/input/peaks.py
 inspire/input/search_results.py
 inspirems.egg-info/PKG-INFO
 inspirems.egg-info/SOURCES.txt
 inspirems.egg-info/dependency_links.txt
```

### Comparing `inspirems-1.4/inspirems.egg-info/requires.txt` & `inspirems-1.5/inspirems.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 kiwisolver==1.4.4
 llvmlite==0.39.0
 lxml==4.9.1
 Markdown==3.4.1
 MarkupSafe==2.1.1
 mokapot==0.8.3
 matplotlib==3.5.3
-ms2pip==3.9.0
 numba==0.56.0
 numexpr==2.8.3
 numpy==1.19.5
 oauthlib==3.2.0
 opt-einsum==3.3.0
 packaging==21.3
 pandas==1.4.3
@@ -71,7 +70,10 @@
 triqler==0.6.2
 typing-extensions==3.7.4.3
 urllib3==1.26.9
 Werkzeug==2.1.2
 wrapt==1.12.1
 xgboost==1.6.1
 zipp==3.8.1
+
+[ms2pip]
+ms2pip==3.9.0
```

### Comparing `inspirems-1.4/setup.py` & `inspirems-1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup
 
 setup(
     name='inspirems',
-    version=1.4,
+    version=1.5,
     description='Helping to integrate Spectral Predictors and Rescoring.',
     author='John Cormican, Juliane Liepe',
     author_email='juliane.liepe@mpinat.mpg.de',
     packages=[
         'inspire',
         'inspire.input',
     ],
@@ -50,15 +50,14 @@
         'kiwisolver==1.4.4',
         'llvmlite==0.39.0',
         'lxml==4.9.1',
         'Markdown==3.4.1',
         'MarkupSafe==2.1.1',
         'mokapot==0.8.3',
         'matplotlib==3.5.3',
-        'ms2pip==3.9.0',
         'numba==0.56.0',
         'numexpr==2.8.3',
         'numpy==1.19.5',
         'oauthlib==3.2.0',
         'opt-einsum==3.3.0',
         'packaging==21.3',
         'pandas==1.4.3',
@@ -98,12 +97,15 @@
         'typing-extensions==3.7.4.3',
         'urllib3==1.26.9',
         'Werkzeug==2.1.2',
         'wrapt==1.12.1',
         'xgboost==1.6.1',
         'zipp==3.8.1',
     ],
+    extras_require={
+        'ms2pip': ['ms2pip==3.9.0',],
+    },
     project_urls={
         'Homepage': 'https://github.com/QuantSysBio/inSPIRE',
         'Tracker': 'https://github.com/QuantSysBio/inSPIRE/issues',
     },
 )
```


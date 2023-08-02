# Comparing `tmp/scoda-tk-0.3.7.tar.gz` & `tmp/scoda-tk-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoda-tk-0.3.7.tar", last modified: Wed Aug  2 17:14:58 2023, max compression
+gzip compressed data, was "scoda-tk-0.3.8.tar", last modified: Wed Aug  2 17:22:54 2023, max compression
```

## Comparing `scoda-tk-0.3.7.tar` & `scoda-tk-0.3.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 17:14:58.275390 scoda-tk-0.3.7/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-08-02 12:34:47.000000 scoda-tk-0.3.7/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-08-02 12:34:47.000000 scoda-tk-0.3.7/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-02 17:14:58.275390 scoda-tk-0.3.7/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-08-02 12:34:48.000000 scoda-tk-0.3.7/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-08-02 17:14:36.000000 scoda-tk-0.3.7/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-08-02 17:14:58.275390 scoda-tk-0.3.7/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-08-02 12:34:47.000000 scoda-tk-0.3.7/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 17:14:58.247391 scoda-tk-0.3.7/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 17:14:58.247391 scoda-tk-0.3.7/src/scoda/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-08-02 12:34:52.000000 scoda-tk-0.3.7/src/scoda/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-08-02 12:34:49.000000 scoda-tk-0.3.7/src/scoda/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 17:14:58.271390 scoda-tk-0.3.7/src/scoda/default_optional_files/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-08-02 12:34:49.000000 scoda-tk-0.3.7/src/scoda/default_optional_files/analysis_config.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-08-02 12:34:50.000000 scoda-tk-0.3.7/src/scoda/default_optional_files/cpdb.zip
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-08-02 12:34:51.000000 scoda-tk-0.3.7/src/scoda/default_optional_files/hg38_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   216264 2023-08-02 13:29:18.000000 scoda-tk-0.3.7/src/scoda/default_optional_files/kegg_human.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   200990 2023-08-02 13:29:18.000000 scoda-tk-0.3.7/src/scoda/default_optional_files/kegg_mouse.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-08-02 12:34:49.000000 scoda-tk-0.3.7/src/scoda/default_optional_files/markers_hs.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-08-02 12:34:49.000000 scoda-tk-0.3.7/src/scoda/default_optional_files/markers_mm.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-08-02 12:34:52.000000 scoda-tk-0.3.7/src/scoda/default_optional_files/mm10_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-08-02 13:30:21.000000 scoda-tk-0.3.7/src/scoda/default_optional_files/msig.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    18849 2023-08-02 12:34:52.000000 scoda-tk-0.3.7/src/scoda/deg.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    13947 2023-08-02 14:40:32.000000 scoda-tk-0.3.7/src/scoda/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-08-02 12:34:48.000000 scoda-tk-0.3.7/src/scoda/hicat.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    33986 2023-08-02 12:34:51.000000 scoda-tk-0.3.7/src/scoda/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-08-02 12:34:52.000000 scoda-tk-0.3.7/src/scoda/misc.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    23980 2023-08-02 17:14:06.000000 scoda-tk-0.3.7/src/scoda/pipeline.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    64916 2023-08-02 16:11:38.000000 scoda-tk-0.3.7/src/scoda/viz.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 17:14:58.275390 scoda-tk-0.3.7/src/scoda_tk.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-02 17:14:58.000000 scoda-tk-0.3.7/src/scoda_tk.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      872 2023-08-02 17:14:58.000000 scoda-tk-0.3.7/src/scoda_tk.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-08-02 17:14:58.000000 scoda-tk-0.3.7/src/scoda_tk.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-08-02 17:14:58.000000 scoda-tk-0.3.7/src/scoda_tk.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-08-02 17:14:58.000000 scoda-tk-0.3.7/src/scoda_tk.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-08-02 17:14:58.000000 scoda-tk-0.3.7/src/scoda_tk.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 17:22:54.769088 scoda-tk-0.3.8/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-08-02 12:34:47.000000 scoda-tk-0.3.8/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-08-02 12:34:47.000000 scoda-tk-0.3.8/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-02 17:22:54.769088 scoda-tk-0.3.8/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-08-02 12:34:48.000000 scoda-tk-0.3.8/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-08-02 17:21:22.000000 scoda-tk-0.3.8/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-08-02 17:22:54.769088 scoda-tk-0.3.8/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-08-02 12:34:47.000000 scoda-tk-0.3.8/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 17:22:54.745088 scoda-tk-0.3.8/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 17:22:54.749088 scoda-tk-0.3.8/src/scoda/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-08-02 12:34:52.000000 scoda-tk-0.3.8/src/scoda/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-08-02 12:34:49.000000 scoda-tk-0.3.8/src/scoda/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 17:22:54.769088 scoda-tk-0.3.8/src/scoda/default_optional_files/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-08-02 12:34:49.000000 scoda-tk-0.3.8/src/scoda/default_optional_files/analysis_config.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-08-02 12:34:50.000000 scoda-tk-0.3.8/src/scoda/default_optional_files/cpdb.zip
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-08-02 12:34:51.000000 scoda-tk-0.3.8/src/scoda/default_optional_files/hg38_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   216264 2023-08-02 13:29:18.000000 scoda-tk-0.3.8/src/scoda/default_optional_files/kegg_human.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   200990 2023-08-02 13:29:18.000000 scoda-tk-0.3.8/src/scoda/default_optional_files/kegg_mouse.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-08-02 12:34:49.000000 scoda-tk-0.3.8/src/scoda/default_optional_files/markers_hs.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-08-02 12:34:49.000000 scoda-tk-0.3.8/src/scoda/default_optional_files/markers_mm.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-08-02 12:34:52.000000 scoda-tk-0.3.8/src/scoda/default_optional_files/mm10_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-08-02 13:30:21.000000 scoda-tk-0.3.8/src/scoda/default_optional_files/msig.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    18849 2023-08-02 12:34:52.000000 scoda-tk-0.3.8/src/scoda/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    13947 2023-08-02 14:40:32.000000 scoda-tk-0.3.8/src/scoda/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-08-02 12:34:48.000000 scoda-tk-0.3.8/src/scoda/hicat.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    33986 2023-08-02 12:34:51.000000 scoda-tk-0.3.8/src/scoda/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-08-02 12:34:52.000000 scoda-tk-0.3.8/src/scoda/misc.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    23980 2023-08-02 17:22:35.000000 scoda-tk-0.3.8/src/scoda/pipeline.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    64916 2023-08-02 16:11:38.000000 scoda-tk-0.3.8/src/scoda/viz.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 17:22:54.769088 scoda-tk-0.3.8/src/scoda_tk.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-02 17:22:54.000000 scoda-tk-0.3.8/src/scoda_tk.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      872 2023-08-02 17:22:54.000000 scoda-tk-0.3.8/src/scoda_tk.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-08-02 17:22:54.000000 scoda-tk-0.3.8/src/scoda_tk.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-08-02 17:22:54.000000 scoda-tk-0.3.8/src/scoda_tk.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-08-02 17:22:54.000000 scoda-tk-0.3.8/src/scoda_tk.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-08-02 17:22:54.000000 scoda-tk-0.3.8/src/scoda_tk.egg-info/top_level.txt
```

### Comparing `scoda-tk-0.3.7/LICENSE` & `scoda-tk-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.7/PKG-INFO` & `scoda-tk-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.3.7
+Version: 0.3.8
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.3.7/pyproject.toml` & `scoda-tk-0.3.8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scoda-tk"
-version = "0.3.7"
+version = "0.3.8"
 description = "Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)"
 readme = "README.md"
 authors = [{ name = "Seokhyun Yoon", email = "syoon@dku.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `scoda-tk-0.3.7/src/scoda/cpdb.py` & `scoda-tk-0.3.8/src/scoda/cpdb.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.7/src/scoda/default_optional_files/cpdb.zip` & `scoda-tk-0.3.8/src/scoda/default_optional_files/cpdb.zip`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.7/src/scoda/default_optional_files/hg38_gene_only.gtf` & `scoda-tk-0.3.8/src/scoda/default_optional_files/hg38_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.7/src/scoda/default_optional_files/kegg_human.gmt` & `scoda-tk-0.3.8/src/scoda/default_optional_files/kegg_human.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.7/src/scoda/default_optional_files/kegg_mouse.gmt` & `scoda-tk-0.3.8/src/scoda/default_optional_files/kegg_mouse.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.7/src/scoda/default_optional_files/markers_hs.tsv` & `scoda-tk-0.3.8/src/scoda/default_optional_files/markers_hs.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.7/src/scoda/default_optional_files/markers_mm.tsv` & `scoda-tk-0.3.8/src/scoda/default_optional_files/markers_mm.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.7/src/scoda/default_optional_files/mm10_gene_only.gtf` & `scoda-tk-0.3.8/src/scoda/default_optional_files/mm10_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.7/src/scoda/default_optional_files/msig.gmt` & `scoda-tk-0.3.8/src/scoda/default_optional_files/msig.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.7/src/scoda/deg.py` & `scoda-tk-0.3.8/src/scoda/deg.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.7/src/scoda/gsea.py` & `scoda-tk-0.3.8/src/scoda/gsea.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.7/src/scoda/hicat.py` & `scoda-tk-0.3.8/src/scoda/hicat.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.7/src/scoda/icnv.py` & `scoda-tk-0.3.8/src/scoda/icnv.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.7/src/scoda/misc.py` & `scoda-tk-0.3.8/src/scoda/misc.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.7/src/scoda/pipeline.py` & `scoda-tk-0.3.8/src/scoda/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,15 +304,15 @@
         adata_t.uns['CCI'] = df_dct
         
     return
 
 
 def scoda_deg_gsea( adata_t, pw_db, 
                     cond_col = 'condition', sample_col = 'sample', 
-                    deg_base = 'celltype_minor', deg_ref_group = None, deg_pval_cutoff = 0.01,
+                    deg_base = 'celltype_minor', ref_group = None, deg_pval_cutoff = 0.01,
                     gsea_pval_cutoff = 0.1, N_cells_min_per_sample = 100, 
                     N_cells_min_per_condition = 100, n_cores = 4, 
                     print_prefix = ''): 
         
     # ref_group_for_deg = ref_group
     ref_group_for_deg = None
     if ref_group is not None:
@@ -489,15 +489,15 @@
 
 def scoda_all_in_one( adata_t, mkr_db, cpdb_path, gsea_pw_db, cnv_gtf = None, 
                       cond_col = 'condition', sample_col = 'sample', cci_deg_base = 'celltype_minor',
                       cnv_ref_list = None, cnv_cmd_cutoff = 0.03, cnv_use_ref_only = False,
                       cnv_gcm = 0.05, cnv_tdec_margin = 0.05, cnv_cd_alpha = 1, 
                       cci_run_unit = 'sample', cci_n_cells_min = 40, 
                       cci_pval_cutoff = 0.1, cci_mean_cutoff = 0, cci_rth = 0.5, 
-                      deg_ref = None, deg_pval_cutoff = 0.01, deg_n_cells_min = 100, 
+                      deg_ref_group = None, deg_pval_cutoff = 0.01, deg_n_cells_min = 100, 
                       gsea_pval_cutoff = 0.1, n_cores = 4, jump = 0,
                       data_dir = '.', verbose = True, print_prefix = ''):
 
     df_mkr_db = mkr_db
     gtf_file = cnv_gtf 
     # cpdb_path = , 
     pw_db_for_gsea = gsea_pw_db 
@@ -505,15 +505,15 @@
     # sample_col = 'sample'
     tumor_id_ref_celltypes = cnv_ref_list 
     unit_of_cci_run = cci_run_unit 
     min_n_cells_for_cci = cci_n_cells_min 
     cci_pval_max = cci_pval_cutoff 
     cci_mean_min = cci_mean_cutoff 
     Rth = cci_rth 
-    deg_ref_group = deg_ref # None, 
+    # deg_ref_group = deg_ref # None, 
     # deg_pval_cutoff = 0.01, 
     min_n_cells_for_deg = deg_n_cells_min 
     n_cores_to_use = n_cores 
     # data_dir = '.', 
     # verbose = True, 
     # prefix = ''
     
@@ -578,15 +578,15 @@
     ####################
     ### DEG analysis ###
     
     if jump <= 3:
         if verbose: print('%sDEG/GSEA analysis ..       ' % print_prefix)
         scoda_deg_gsea( adata_t, pw_db = pw_db_for_gsea, 
                         cond_col = cond_col, sample_col = sample_col, 
-                        deg_base = cci_deg_base, deg_ref_group = deg_ref_group, 
+                        deg_base = cci_deg_base, ref_group = deg_ref_group, 
                         deg_pval_cutoff = deg_pval_cutoff, 
                         gsea_pval_cutoff = gsea_pval_cutoff,
                         N_cells_min_per_sample = min_n_cells_for_deg, 
                         N_cells_min_per_condition = min_n_cells_for_deg, 
                         n_cores = n_cores_to_use, print_prefix = print_prefix)
 
         ## Overwrite
```

### Comparing `scoda-tk-0.3.7/src/scoda/viz.py` & `scoda-tk-0.3.8/src/scoda/viz.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.7/src/scoda_tk.egg-info/PKG-INFO` & `scoda-tk-0.3.8/src/scoda_tk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.3.7
+Version: 0.3.8
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.3.7/src/scoda_tk.egg-info/SOURCES.txt` & `scoda-tk-0.3.8/src/scoda_tk.egg-info/SOURCES.txt`

 * *Files identical despite different names*


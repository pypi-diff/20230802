# Comparing `tmp/scoda-tk-0.3.5.tar.gz` & `tmp/scoda-tk-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoda-tk-0.3.5.tar", last modified: Wed Aug  2 14:38:42 2023, max compression
+gzip compressed data, was "scoda-tk-0.3.6.tar", last modified: Wed Aug  2 16:12:16 2023, max compression
```

## Comparing `scoda-tk-0.3.5.tar` & `scoda-tk-0.3.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 14:38:42.982785 scoda-tk-0.3.5/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-08-02 12:34:47.000000 scoda-tk-0.3.5/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-08-02 12:34:47.000000 scoda-tk-0.3.5/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-02 14:38:42.982785 scoda-tk-0.3.5/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-08-02 12:34:48.000000 scoda-tk-0.3.5/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-08-02 14:38:04.000000 scoda-tk-0.3.5/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-08-02 14:38:42.982785 scoda-tk-0.3.5/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-08-02 12:34:47.000000 scoda-tk-0.3.5/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 14:38:42.866788 scoda-tk-0.3.5/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 14:38:42.906787 scoda-tk-0.3.5/src/scoda/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-08-02 12:34:52.000000 scoda-tk-0.3.5/src/scoda/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-08-02 12:34:49.000000 scoda-tk-0.3.5/src/scoda/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 14:38:42.982785 scoda-tk-0.3.5/src/scoda/default_optional_files/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-08-02 12:34:49.000000 scoda-tk-0.3.5/src/scoda/default_optional_files/analysis_config.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-08-02 12:34:50.000000 scoda-tk-0.3.5/src/scoda/default_optional_files/cpdb.zip
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-08-02 12:34:51.000000 scoda-tk-0.3.5/src/scoda/default_optional_files/hg38_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   216264 2023-08-02 13:29:18.000000 scoda-tk-0.3.5/src/scoda/default_optional_files/kegg_human.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   200990 2023-08-02 13:29:18.000000 scoda-tk-0.3.5/src/scoda/default_optional_files/kegg_mouse.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-08-02 12:34:49.000000 scoda-tk-0.3.5/src/scoda/default_optional_files/markers_hs.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-08-02 12:34:49.000000 scoda-tk-0.3.5/src/scoda/default_optional_files/markers_mm.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-08-02 12:34:52.000000 scoda-tk-0.3.5/src/scoda/default_optional_files/mm10_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-08-02 13:30:21.000000 scoda-tk-0.3.5/src/scoda/default_optional_files/msig.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    18849 2023-08-02 12:34:52.000000 scoda-tk-0.3.5/src/scoda/deg.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    13768 2023-08-02 12:34:48.000000 scoda-tk-0.3.5/src/scoda/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-08-02 12:34:48.000000 scoda-tk-0.3.5/src/scoda/hicat.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    33986 2023-08-02 12:34:51.000000 scoda-tk-0.3.5/src/scoda/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-08-02 12:34:52.000000 scoda-tk-0.3.5/src/scoda/misc.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    23145 2023-08-02 12:34:48.000000 scoda-tk-0.3.5/src/scoda/pipeline.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    63794 2023-08-02 14:36:37.000000 scoda-tk-0.3.5/src/scoda/viz.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 14:38:42.982785 scoda-tk-0.3.5/src/scoda_tk.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-02 14:38:42.000000 scoda-tk-0.3.5/src/scoda_tk.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      872 2023-08-02 14:38:42.000000 scoda-tk-0.3.5/src/scoda_tk.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-08-02 14:38:42.000000 scoda-tk-0.3.5/src/scoda_tk.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-08-02 14:38:42.000000 scoda-tk-0.3.5/src/scoda_tk.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-08-02 14:38:42.000000 scoda-tk-0.3.5/src/scoda_tk.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-08-02 14:38:42.000000 scoda-tk-0.3.5/src/scoda_tk.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 16:12:16.044692 scoda-tk-0.3.6/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-08-02 12:34:47.000000 scoda-tk-0.3.6/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-08-02 12:34:47.000000 scoda-tk-0.3.6/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-02 16:12:16.044692 scoda-tk-0.3.6/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-08-02 12:34:48.000000 scoda-tk-0.3.6/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-08-02 16:11:50.000000 scoda-tk-0.3.6/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-08-02 16:12:16.044692 scoda-tk-0.3.6/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-08-02 12:34:47.000000 scoda-tk-0.3.6/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 16:12:16.016692 scoda-tk-0.3.6/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 16:12:16.020692 scoda-tk-0.3.6/src/scoda/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-08-02 12:34:52.000000 scoda-tk-0.3.6/src/scoda/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-08-02 12:34:49.000000 scoda-tk-0.3.6/src/scoda/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 16:12:16.040692 scoda-tk-0.3.6/src/scoda/default_optional_files/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-08-02 12:34:49.000000 scoda-tk-0.3.6/src/scoda/default_optional_files/analysis_config.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-08-02 12:34:50.000000 scoda-tk-0.3.6/src/scoda/default_optional_files/cpdb.zip
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-08-02 12:34:51.000000 scoda-tk-0.3.6/src/scoda/default_optional_files/hg38_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   216264 2023-08-02 13:29:18.000000 scoda-tk-0.3.6/src/scoda/default_optional_files/kegg_human.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   200990 2023-08-02 13:29:18.000000 scoda-tk-0.3.6/src/scoda/default_optional_files/kegg_mouse.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-08-02 12:34:49.000000 scoda-tk-0.3.6/src/scoda/default_optional_files/markers_hs.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-08-02 12:34:49.000000 scoda-tk-0.3.6/src/scoda/default_optional_files/markers_mm.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-08-02 12:34:52.000000 scoda-tk-0.3.6/src/scoda/default_optional_files/mm10_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-08-02 13:30:21.000000 scoda-tk-0.3.6/src/scoda/default_optional_files/msig.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    18849 2023-08-02 12:34:52.000000 scoda-tk-0.3.6/src/scoda/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    13947 2023-08-02 14:40:32.000000 scoda-tk-0.3.6/src/scoda/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-08-02 12:34:48.000000 scoda-tk-0.3.6/src/scoda/hicat.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    33986 2023-08-02 12:34:51.000000 scoda-tk-0.3.6/src/scoda/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-08-02 12:34:52.000000 scoda-tk-0.3.6/src/scoda/misc.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    23834 2023-08-02 16:10:46.000000 scoda-tk-0.3.6/src/scoda/pipeline.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    64916 2023-08-02 16:11:38.000000 scoda-tk-0.3.6/src/scoda/viz.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 16:12:16.040692 scoda-tk-0.3.6/src/scoda_tk.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-02 16:12:16.000000 scoda-tk-0.3.6/src/scoda_tk.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      872 2023-08-02 16:12:16.000000 scoda-tk-0.3.6/src/scoda_tk.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-08-02 16:12:16.000000 scoda-tk-0.3.6/src/scoda_tk.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-08-02 16:12:16.000000 scoda-tk-0.3.6/src/scoda_tk.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-08-02 16:12:16.000000 scoda-tk-0.3.6/src/scoda_tk.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-08-02 16:12:16.000000 scoda-tk-0.3.6/src/scoda_tk.egg-info/top_level.txt
```

### Comparing `scoda-tk-0.3.5/LICENSE` & `scoda-tk-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.5/PKG-INFO` & `scoda-tk-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.3.5
+Version: 0.3.6
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.3.5/pyproject.toml` & `scoda-tk-0.3.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scoda-tk"
-version = "0.3.5"
+version = "0.3.6"
 description = "Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)"
 readme = "README.md"
 authors = [{ name = "Seokhyun Yoon", email = "syoon@dku.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `scoda-tk-0.3.5/src/scoda/cpdb.py` & `scoda-tk-0.3.6/src/scoda/cpdb.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.5/src/scoda/default_optional_files/cpdb.zip` & `scoda-tk-0.3.6/src/scoda/default_optional_files/cpdb.zip`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.5/src/scoda/default_optional_files/hg38_gene_only.gtf` & `scoda-tk-0.3.6/src/scoda/default_optional_files/hg38_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.5/src/scoda/default_optional_files/kegg_human.gmt` & `scoda-tk-0.3.6/src/scoda/default_optional_files/kegg_human.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.5/src/scoda/default_optional_files/kegg_mouse.gmt` & `scoda-tk-0.3.6/src/scoda/default_optional_files/kegg_mouse.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.5/src/scoda/default_optional_files/markers_hs.tsv` & `scoda-tk-0.3.6/src/scoda/default_optional_files/markers_hs.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.5/src/scoda/default_optional_files/markers_mm.tsv` & `scoda-tk-0.3.6/src/scoda/default_optional_files/markers_mm.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.5/src/scoda/default_optional_files/mm10_gene_only.gtf` & `scoda-tk-0.3.6/src/scoda/default_optional_files/mm10_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.5/src/scoda/default_optional_files/msig.gmt` & `scoda-tk-0.3.6/src/scoda/default_optional_files/msig.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.5/src/scoda/deg.py` & `scoda-tk-0.3.6/src/scoda/deg.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.5/src/scoda/gsea.py` & `scoda-tk-0.3.6/src/scoda/gsea.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,14 +62,23 @@
 
 # items_to_plot = ['-log(p-val)', 'NES', '-log(q-val)']
 # lims = [[0, 2], [-5, 5], [0, 2]]
 
 # plot_gsea_res( df_res, terms_sel, items_to_plot, lims)
 
 
+def load_gmt(file):
+    dct = {}
+    with open(file, 'r') as f:
+        for line in f:
+            items = line.split('\t')
+            dct[items[0]] = items[2:]
+    return dct
+
+
 def get_gene_rank(adata_s, cond_col, group_test, 
                   log2fc_min = 0.25, pval_cutoff = 0.05, 
                   test_sel = 't-test', n_cells_min = 40, 
                   log1p = True):
     
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
```

### Comparing `scoda-tk-0.3.5/src/scoda/hicat.py` & `scoda-tk-0.3.6/src/scoda/hicat.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.5/src/scoda/icnv.py` & `scoda-tk-0.3.6/src/scoda/icnv.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.5/src/scoda/misc.py` & `scoda-tk-0.3.6/src/scoda/misc.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.5/src/scoda/pipeline.py` & `scoda-tk-0.3.6/src/scoda/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 import pandas as pd
 import scanpy as sc
 import anndata
 
 import gseapy as gp
 
-def load_gmt(file):
+def load_gmt_file(file):
     dct = {}
     with open(file, 'r') as f:
         for line in f:
             items = line.split('\t')
             dct[items[0]] = items[2:]
     return dct
 
@@ -303,16 +303,16 @@
         adata_t.uns['CCI'] = df_dct
         
     return
 
 
 def scoda_deg_gsea( adata_t, pw_db, 
                     cond_col = 'condition', sample_col = 'sample', 
-                    ref_group = None, pval_cutoff = 0.05,
-                    N_cells_min_per_sample = 100, 
+                    ref_group = None, deg_pval_cutoff = 0.01,
+                    gsea_pval_cutoff = 0.1, N_cells_min_per_sample = 100, 
                     N_cells_min_per_condition = 100, n_cores = 4, 
                     print_prefix = ''): 
         
     # ref_group_for_deg = ref_group
     ref_group_for_deg = None
     if ref_group is not None:
         if ref_group in list(adata_t.obs[cond_col].unique()):
@@ -414,60 +414,65 @@
                 ## Run gseapy.prerank
                 df_lst_enrichr = {}
                 df_lst_enrichr_up = {}
                 df_lst_enrichr_dn = {}
                 df_lst_prerank = {}
                 #'''
                 for c in df_lst.keys():
+                    
                     gene_rank = df_lst[c].copy(deep = True)
-                    gene_rank[gene_col] = list(gene_rank.index.values)
-
-                    ## Run gseapy.enrichr
-                    df_res_enr_pos = None
-                    b = gene_rank[log_fc_col] > 0
-                    if np.sum(b) > 0:
-                        df_res_enr_pos = run_enrich(gene_rank.loc[b,gene_col], pw_db_sel, genes_all, pval_max = pval_cutoff)
-                        df_res_enr_pos['Ind'] = 1
-                        # if verbose: print('  Num. of selected pathways in Enrichr (+): ', df_res_enr_pos.shape[0])
-
-                    df_res_enr_neg = None
-                    b = gene_rank[log_fc_col] < 0
-                    if np.sum(b) > 0:
-                        df_res_enr_neg = run_enrich(gene_rank.loc[b,gene_col], pw_db_sel, genes_all, pval_max = pval_cutoff)
-                        df_res_enr_neg['Ind'] = -1
-                        # if verbose: print('  Num. of selected pathways in Enrichr (-): ', df_res_enr_neg.shape[0])
-
-                    if (df_res_enr_pos is not None) & (df_res_enr_neg is not None):
-                        df_res_enr = pd.concat([df_res_enr_pos, df_res_enr_neg], axis = 0)
-                    elif (df_res_enr_pos is not None):
-                        df_res_enr = df_res_enr_pos
-                    elif (df_res_enr_neg is not None):
-                        df_res_enr = df_res_enr_neg
-                    else:
-                        df_res_enr = None
-                        
-                    if df_res_enr is not None:
-                        df_lst_enrichr[c] = df_res_enr
-                        
-                    if df_res_enr_pos is not None:
-                        df_lst_enrichr_up[c] = df_res_enr_pos
-                    if df_res_enr_neg is not None:
-                        df_lst_enrichr_dn[c] = df_res_enr_neg
-
-                    ## Run gseapy.prerank
-                    logfc = gene_rank[[log_fc_col]] ## index must be gene name
+                    b = gene_rank['pval'] <= deg_pval_cutoff
 
-                    df_res_pr, pr_res = run_prerank(logfc, pw_db_sel, pval_max = 0.1, # pval_cutoff,
+                    # print(np.sum(b), gene_rank.shape)
+                    if np.sum(b) > 1:
+                        gene_rank = gene_rank.loc[b,:]              
+                        gene_rank[gene_col] = list(gene_rank.index.values)
+
+                        ## Run gseapy.enrichr
+                        df_res_enr_pos = None
+                        b = gene_rank[log_fc_col] > 0
+                        if np.sum(b) > 0:
+                            df_res_enr_pos = run_enrich(gene_rank.loc[b,gene_col], pw_db_sel, genes_all, pval_max = gsea_pval_cutoff)
+                            df_res_enr_pos['Ind'] = 1
+                            # if verbose: print('  Num. of selected pathways in Enrichr (+): ', df_res_enr_pos.shape[0])
+
+                        df_res_enr_neg = None
+                        b = gene_rank[log_fc_col] < 0
+                        if np.sum(b) > 0:
+                            df_res_enr_neg = run_enrich(gene_rank.loc[b,gene_col], pw_db_sel, genes_all, pval_max = gsea_pval_cutoff)
+                            df_res_enr_neg['Ind'] = -1
+                            # if verbose: print('  Num. of selected pathways in Enrichr (-): ', df_res_enr_neg.shape[0])
+
+                        if (df_res_enr_pos is not None) & (df_res_enr_neg is not None):
+                            df_res_enr = pd.concat([df_res_enr_pos, df_res_enr_neg], axis = 0)
+                        elif (df_res_enr_pos is not None):
+                            df_res_enr = df_res_enr_pos
+                        elif (df_res_enr_neg is not None):
+                            df_res_enr = df_res_enr_neg
+                        else:
+                            df_res_enr = None
+
+                        if df_res_enr is not None:
+                            df_lst_enrichr[c] = df_res_enr
+
+                        if df_res_enr_pos is not None:
+                            df_lst_enrichr_up[c] = df_res_enr_pos
+                        if df_res_enr_neg is not None:
+                            df_lst_enrichr_dn[c] = df_res_enr_neg
+
+                        ## Run gseapy.prerank
+                        logfc = gene_rank[[log_fc_col]] ## index must be gene name
+                        df_res_pr, pr_res = run_prerank(logfc, pw_db_sel, pval_max = gsea_pval_cutoff,
                                         min_size = min_size, max_size = max_size, n_cores = n_cores )
-                    
-                    # df_res_pr.drop(columns = ['Tag %', 'Gene %'], inplace = True)
-                    if df_res_pr.shape[0] > 0:
-                        df_res_pr[['ES', 'NES', 'NOM p-val', 'FDR q-val', 'FWER p-val']] = \
-                            df_res_pr[['ES', 'NES', 'NOM p-val', 'FDR q-val', 'FWER p-val']].astype(float)
-                        df_lst_prerank[c] = df_res_pr                        
+
+                        # df_res_pr.drop(columns = ['Tag %', 'Gene %'], inplace = True)
+                        if df_res_pr.shape[0] > 0:
+                            df_res_pr[['ES', 'NES', 'NOM p-val', 'FDR q-val', 'FWER p-val']] = \
+                                df_res_pr[['ES', 'NES', 'NOM p-val', 'FDR q-val', 'FWER p-val']].astype(float)
+                            df_lst_prerank[c] = df_res_pr                        
 
                 df_dct_dct_enr_up[ct] = df_lst_enrichr_up
                 df_dct_dct_enr_dn[ct] = df_lst_enrichr_dn
                 df_dct_dct_enr[ct] = df_lst_enrichr
                 df_dct_dct_pr[ct] = df_lst_prerank
                 # '''
 
@@ -484,15 +489,16 @@
 def scoda_all_in_one( adata_t, mkr_db, cpdb_path, gsea_pw_db, cnv_gtf = None, 
                       cond_col = 'condition', sample_col = 'sample', 
                       cnv_ref_list = None, cnv_cmd_cutoff = 0.03, cnv_use_ref_only = False,
                       cnv_gcm = 0.05, cnv_tdec_margin = 0.05, cnv_cd_alpha = 1, 
                       cci_run_unit = 'sample', cci_n_cells_min = 40, 
                       cci_pval_cutoff = 0.1, cci_mean_cutoff = 0, cci_rth = 0.5, 
                       deg_ref = None, deg_pval_cutoff = 0.01, deg_n_cells_min = 100, 
-                      n_cores = 4, data_dir = '.', verbose = True, print_prefix = ''):
+                      gsea_pval_cutoff = 0.1, n_cores = 4, jump = 0,
+                      data_dir = '.', verbose = True, print_prefix = ''):
 
     df_mkr_db = mkr_db
     gtf_file = cnv_gtf 
     # cpdb_path = , 
     pw_db_for_gsea = gsea_pw_db 
     # cond_col = 'condition' 
     # sample_col = 'sample'
@@ -508,79 +514,81 @@
     n_cores_to_use = n_cores 
     # data_dir = '.', 
     # verbose = True, 
     # prefix = ''
     
     ################################
     ### Cell-type identification ###
+    if jump < 1:
+        if verbose: print('%sCelltype annotation running .. ' % print_prefix)
 
-    if verbose: print('%sCelltype annotation running .. ' % print_prefix)
-        
-    scoda_hicat(adata_t, df_mkr_db, verbose = False)
-    
-    if verbose: print('%sCelltype annotation done.' % print_prefix)
+        scoda_hicat(adata_t, df_mkr_db, verbose = False)
+
+        if verbose: print('%sCelltype annotation done.' % print_prefix)
+
+        # adata_t.write(file_h5ad)
 
-    # adata_t.write(file_h5ad)
-      
-    ## For client info.
-    ct_lst_maj = list(adata_t.obs['celltype_major'].unique())
-    ct_lst_min = list(adata_t.obs['celltype_minor'].unique())
-    ct_lst_sub = list(adata_t.obs['celltype_subset'].unique())
-
-    ct_lst_maj.sort()
-    s = ''
-    for c in ct_lst_maj:
-        s = s + '%s, ' % c
-    s = s[:-2]
-
-    if verbose: 
-        print('%s  %i major type, %i minor type, %i subset identified.' 
-               % (print_prefix, len(ct_lst_maj), len(ct_lst_min), len(ct_lst_sub)))
-        print('%s  Major types: %s' % (print_prefix, s))
+        ## For client info.
+        ct_lst_maj = list(adata_t.obs['celltype_major'].unique())
+        ct_lst_min = list(adata_t.obs['celltype_minor'].unique())
+        ct_lst_sub = list(adata_t.obs['celltype_subset'].unique())
+
+        ct_lst_maj.sort()
+        s = ''
+        for c in ct_lst_maj:
+            s = s + '%s, ' % c
+        s = s[:-2]
+
+        if verbose: 
+            print('%s  %i major type, %i minor type, %i subset identified.' 
+                   % (print_prefix, len(ct_lst_maj), len(ct_lst_min), len(ct_lst_sub)))
+            print('%s  Major types: %s' % (print_prefix, s))
         
     #################################
     ### tumor cell identification ###
-    
-    if cnv_gtf is not None:
+    if jump <= 1:
+        if cnv_gtf is not None:
 
-        ## Test without Reference 
-        if verbose: print('%sIdentifying tumor cells .. ' % print_prefix)
+            ## Test without Reference 
+            if verbose: print('%sIdentifying tumor cells .. ' % print_prefix)
 
-        ref_types = tumor_id_ref_celltypes
+            ref_types = tumor_id_ref_celltypes
 
-        df = scoda_icnv_addon( adata_t, gtf_file, ref_types = ref_types, 
-                               ref_key = "celltype_major", n_cores = n_cores_to_use,
-                               use_ref_only = False, cmd_cutoff = 0.03, gcm = 0.05, 
-                               tumor_dec_margin = 0.01, cd_alpha = cnv_cd_alpha )
-        
-        if verbose: print('%sTumor cells identification done. ' % print_prefix)
-        # adata_t.write(file_h5ad)
+            df = scoda_icnv_addon( adata_t, gtf_file, ref_types = ref_types, 
+                                   ref_key = "celltype_major", n_cores = n_cores_to_use,
+                                   use_ref_only = False, cmd_cutoff = 0.03, gcm = 0.05, 
+                                   tumor_dec_margin = 0.01, cd_alpha = cnv_cd_alpha )
+
+            if verbose: print('%sTumor cells identification done. ' % print_prefix)
+            # adata_t.write(file_h5ad)
            
     #############################
     ### Cell-cell interaction ###
+    if jump <= 2:
+        if verbose: print('%sInfering cell-cell interactions .. ' % print_prefix)
 
-    if verbose: print('%sInfering cell-cell interactions .. ' % print_prefix)
+        scoda_cci( adata_t, cpdb_path, cond_col = cond_col, sample_col = sample_col, 
+                   unit_of_cci_run = unit_of_cci_run, n_cores = n_cores_to_use, 
+                   min_n_cells_for_cci = min_n_cells_for_cci, Rth = Rth,
+                   pval_max = cci_pval_max, mean_min = cci_mean_min, data_dir = data_dir)
 
-    scoda_cci( adata_t, cpdb_path, cond_col = cond_col, sample_col = sample_col, 
-               unit_of_cci_run = unit_of_cci_run, n_cores = n_cores_to_use, 
-               min_n_cells_for_cci = min_n_cells_for_cci, Rth = Rth,
-               pval_max = cci_pval_max, mean_min = cci_mean_min, data_dir = data_dir)
-    
-    if verbose: print('%sInfering cell-cell interactions done. ' % print_prefix)    
-    # adata_t.write(file_h5ad)
+        if verbose: print('%sInfering cell-cell interactions done. ' % print_prefix)    
+        # adata_t.write(file_h5ad)
         
     ####################
     ### DEG analysis ###
-
-    if verbose: print('%sDEG/GSEA analysis ..       ' % print_prefix)
-    scoda_deg_gsea( adata_t, pw_db = pw_db_for_gsea, 
-                    cond_col = cond_col, sample_col = sample_col, 
-                    ref_group = deg_ref_group, pval_cutoff = deg_pval_cutoff, 
-                    N_cells_min_per_sample = min_n_cells_for_deg, 
-                    N_cells_min_per_condition = min_n_cells_for_deg, 
-                    n_cores = n_cores_to_use, print_prefix = print_prefix)
-        
-    ## Overwrite 
-    # adata_t.write(file_h5ad)        
-    if verbose: print('%sDEG/GSEA analysis done.       ' % print_prefix)
+    
+    if jump <= 3:
+        if verbose: print('%sDEG/GSEA analysis ..       ' % print_prefix)
+        scoda_deg_gsea( adata_t, pw_db = pw_db_for_gsea, 
+                        cond_col = cond_col, sample_col = sample_col, 
+                        ref_group = deg_ref_group, deg_pval_cutoff = deg_pval_cutoff, 
+                        gsea_pval_cutoff = gsea_pval_cutoff,
+                        N_cells_min_per_sample = min_n_cells_for_deg, 
+                        N_cells_min_per_condition = min_n_cells_for_deg, 
+                        n_cores = n_cores_to_use, print_prefix = print_prefix)
+
+        ## Overwrite 
+        # adata_t.write(file_h5ad)        
+        if verbose: print('%sDEG/GSEA analysis done.       ' % print_prefix)
         
     return
```

### Comparing `scoda-tk-0.3.5/src/scoda/viz.py` & `scoda-tk-0.3.6/src/scoda/viz.py`

 * *Files 2% similar despite different names*

```diff
@@ -1680,14 +1680,54 @@
             ax = plt.subplot(nr,nc,k)
             ax.axis('off')
 
     plt.show()
     return
 
 
+def get_markers_from_deg( df_dct, ref_col = 'score',  N_mkrs = 30, rem_common = True ):
+## Get markers from DEG results
+
+    df_deg = df_dct
+    mkr_dict = {}
+    b = True
+    for key in df_deg.keys():
+        if ref_col not in list(df_deg[key].columns.values):
+            b = False
+            break
+    
+    if not b:
+        print('ERROR: %s not found in column name of DEG results.' % ref_col)
+        return None
+
+    for key in df_deg.keys():
+
+        g = key.split('_')[0]
+        df = df_deg[key].copy(deep = True)
+        df = df.sort_values([ref_col], ascending = False)
+
+        mkr_dict[g] = list(df.iloc[:N_mkrs].index.values)
+
+    ## Remove common markers
+    if rem_common:
+        lst = list(mkr_dict.keys())
+        cmm = []
+        for j, k1 in enumerate(lst):
+            for i, k2 in enumerate(lst):
+                if (k1 != k2) & (j < i):
+                    lc = list(set(mkr_dict[k1]).intersection(mkr_dict[k2]))
+                    cmm = cmm + lc
+        cmm = list(set(cmm))
+
+        for j, k in enumerate(lst):
+            mkr_dict[k] = list(set(mkr_dict[k]) - set(cmm))
+
+    return mkr_dict
+
+
 def plot_gsea_res( df_res, terms_sel, items_to_plot, lims = None, title = None, 
                    title_pos = (0.5, 1), title_fs = 16, title_ha = 'center', Ax = None):
 
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         ## draw result
         sc.settings.set_figure_params(figsize = (4,(len(terms_sel) + 8)/9), dpi=100)
```

### Comparing `scoda-tk-0.3.5/src/scoda_tk.egg-info/PKG-INFO` & `scoda-tk-0.3.6/src/scoda_tk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.3.5
+Version: 0.3.6
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.3.5/src/scoda_tk.egg-info/SOURCES.txt` & `scoda-tk-0.3.6/src/scoda_tk.egg-info/SOURCES.txt`

 * *Files identical despite different names*


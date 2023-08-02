# Comparing `tmp/scoda-tk-0.3.0.tar.gz` & `tmp/scoda-tk-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoda-tk-0.3.0.tar", last modified: Wed Aug  2 08:23:08 2023, max compression
+gzip compressed data, was "scoda-tk-0.3.1.tar", last modified: Wed Aug  2 08:31:46 2023, max compression
```

## Comparing `scoda-tk-0.3.0.tar` & `scoda-tk-0.3.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 08:23:08.347008 scoda-tk-0.3.0/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-30 14:49:21.000000 scoda-tk-0.3.0/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-07-30 14:49:22.000000 scoda-tk-0.3.0/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-02 08:23:08.347008 scoda-tk-0.3.0/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-30 14:49:22.000000 scoda-tk-0.3.0/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-08-02 08:22:53.000000 scoda-tk-0.3.0/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-08-02 08:23:08.347008 scoda-tk-0.3.0/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-30 14:49:21.000000 scoda-tk-0.3.0/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 08:23:08.203011 scoda-tk-0.3.0/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 08:23:08.211011 scoda-tk-0.3.0/src/scoda/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-30 14:49:25.000000 scoda-tk-0.3.0/src/scoda/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-30 14:49:23.000000 scoda-tk-0.3.0/src/scoda/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 08:23:08.327009 scoda-tk-0.3.0/src/scoda/default_optional_files/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-07-30 14:49:23.000000 scoda-tk-0.3.0/src/scoda/default_optional_files/analysis_config.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-07-30 14:49:24.000000 scoda-tk-0.3.0/src/scoda/default_optional_files/cpdb.zip
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-07-30 14:49:24.000000 scoda-tk-0.3.0/src/scoda/default_optional_files/hg38_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-07-30 14:49:23.000000 scoda-tk-0.3.0/src/scoda/default_optional_files/markers_hs.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-07-30 14:49:23.000000 scoda-tk-0.3.0/src/scoda/default_optional_files/markers_mm.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-07-30 14:49:25.000000 scoda-tk-0.3.0/src/scoda/default_optional_files/mm10_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-07-30 14:49:23.000000 scoda-tk-0.3.0/src/scoda/default_optional_files/msig.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    17850 2023-07-30 14:49:25.000000 scoda-tk-0.3.0/src/scoda/deg.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    13716 2023-07-30 14:49:22.000000 scoda-tk-0.3.0/src/scoda/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-07-30 14:49:22.000000 scoda-tk-0.3.0/src/scoda/hicat.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    33925 2023-08-01 19:29:33.000000 scoda-tk-0.3.0/src/scoda/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-07-30 14:49:25.000000 scoda-tk-0.3.0/src/scoda/misc.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    23452 2023-08-02 08:22:29.000000 scoda-tk-0.3.0/src/scoda/pipeline.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    63555 2023-08-02 08:22:36.000000 scoda-tk-0.3.0/src/scoda/viz.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 08:23:08.347008 scoda-tk-0.3.0/src/scoda_tk.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-02 08:23:08.000000 scoda-tk-0.3.0/src/scoda_tk.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      776 2023-08-02 08:23:08.000000 scoda-tk-0.3.0/src/scoda_tk.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-08-02 08:23:08.000000 scoda-tk-0.3.0/src/scoda_tk.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-08-02 08:23:08.000000 scoda-tk-0.3.0/src/scoda_tk.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-08-02 08:23:08.000000 scoda-tk-0.3.0/src/scoda_tk.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-08-02 08:23:08.000000 scoda-tk-0.3.0/src/scoda_tk.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 08:31:46.871398 scoda-tk-0.3.1/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-30 14:49:21.000000 scoda-tk-0.3.1/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-07-30 14:49:22.000000 scoda-tk-0.3.1/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-02 08:31:46.871398 scoda-tk-0.3.1/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-30 14:49:22.000000 scoda-tk-0.3.1/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-08-02 08:31:21.000000 scoda-tk-0.3.1/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-08-02 08:31:46.871398 scoda-tk-0.3.1/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-30 14:49:21.000000 scoda-tk-0.3.1/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 08:31:46.851398 scoda-tk-0.3.1/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 08:31:46.851398 scoda-tk-0.3.1/src/scoda/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-30 14:49:25.000000 scoda-tk-0.3.1/src/scoda/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-30 14:49:23.000000 scoda-tk-0.3.1/src/scoda/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 08:31:46.871398 scoda-tk-0.3.1/src/scoda/default_optional_files/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-07-30 14:49:23.000000 scoda-tk-0.3.1/src/scoda/default_optional_files/analysis_config.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-07-30 14:49:24.000000 scoda-tk-0.3.1/src/scoda/default_optional_files/cpdb.zip
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-07-30 14:49:24.000000 scoda-tk-0.3.1/src/scoda/default_optional_files/hg38_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-07-30 14:49:23.000000 scoda-tk-0.3.1/src/scoda/default_optional_files/markers_hs.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-07-30 14:49:23.000000 scoda-tk-0.3.1/src/scoda/default_optional_files/markers_mm.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-07-30 14:49:25.000000 scoda-tk-0.3.1/src/scoda/default_optional_files/mm10_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-07-30 14:49:23.000000 scoda-tk-0.3.1/src/scoda/default_optional_files/msig.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    17850 2023-07-30 14:49:25.000000 scoda-tk-0.3.1/src/scoda/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    13716 2023-07-30 14:49:22.000000 scoda-tk-0.3.1/src/scoda/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-07-30 14:49:22.000000 scoda-tk-0.3.1/src/scoda/hicat.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    33921 2023-08-02 08:31:09.000000 scoda-tk-0.3.1/src/scoda/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-07-30 14:49:25.000000 scoda-tk-0.3.1/src/scoda/misc.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    23366 2023-08-02 08:30:16.000000 scoda-tk-0.3.1/src/scoda/pipeline.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    63555 2023-08-02 08:22:36.000000 scoda-tk-0.3.1/src/scoda/viz.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 08:31:46.871398 scoda-tk-0.3.1/src/scoda_tk.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-02 08:31:46.000000 scoda-tk-0.3.1/src/scoda_tk.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      776 2023-08-02 08:31:46.000000 scoda-tk-0.3.1/src/scoda_tk.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-08-02 08:31:46.000000 scoda-tk-0.3.1/src/scoda_tk.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-08-02 08:31:46.000000 scoda-tk-0.3.1/src/scoda_tk.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-08-02 08:31:46.000000 scoda-tk-0.3.1/src/scoda_tk.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-08-02 08:31:46.000000 scoda-tk-0.3.1/src/scoda_tk.egg-info/top_level.txt
```

### Comparing `scoda-tk-0.3.0/LICENSE` & `scoda-tk-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.0/PKG-INFO` & `scoda-tk-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.3.0
+Version: 0.3.1
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.3.0/pyproject.toml` & `scoda-tk-0.3.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scoda-tk"
-version = "0.3.0"
+version = "0.3.1"
 description = "Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)"
 readme = "README.md"
 authors = [{ name = "Seokhyun Yoon", email = "syoon@dku.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `scoda-tk-0.3.0/src/scoda/cpdb.py` & `scoda-tk-0.3.1/src/scoda/cpdb.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.0/src/scoda/default_optional_files/cpdb.zip` & `scoda-tk-0.3.1/src/scoda/default_optional_files/cpdb.zip`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.0/src/scoda/default_optional_files/hg38_gene_only.gtf` & `scoda-tk-0.3.1/src/scoda/default_optional_files/hg38_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.0/src/scoda/default_optional_files/markers_hs.tsv` & `scoda-tk-0.3.1/src/scoda/default_optional_files/markers_hs.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.0/src/scoda/default_optional_files/markers_mm.tsv` & `scoda-tk-0.3.1/src/scoda/default_optional_files/markers_mm.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.0/src/scoda/default_optional_files/mm10_gene_only.gtf` & `scoda-tk-0.3.1/src/scoda/default_optional_files/mm10_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.0/src/scoda/default_optional_files/msig.gmt` & `scoda-tk-0.3.1/src/scoda/default_optional_files/msig.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.0/src/scoda/deg.py` & `scoda-tk-0.3.1/src/scoda/deg.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.0/src/scoda/gsea.py` & `scoda-tk-0.3.1/src/scoda/gsea.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.0/src/scoda/hicat.py` & `scoda-tk-0.3.1/src/scoda/hicat.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.0/src/scoda/icnv.py` & `scoda-tk-0.3.1/src/scoda/icnv.py`

 * *Files 0% similar despite different names*

```diff
@@ -953,15 +953,15 @@
     df_res.rename(columns = {'dec': 'tumor_dec'}, inplace = True)
     df_res.drop(columns = 'b_inc', inplace = True)
     results['cnv_cluster_info'] = df_res    
     
     etime = round(time.time() - start_time_a) 
     print('done (%i) ' % etime) #, end = '', flush = True)
     
-    return df, results, cobj, X_pca
+    return results, cobj, X_pca
 
 
 def plot_td_stats( params, n_bins = 30, title = None, title_fs = 14,
                    label_fs = 12, tick_fs = 11, legend_fs = 11, 
                    legend_loc = 'upper left', bbox_to_anchor = (1, 1),
                    figsize = (4,3), log = True, alpha = 0.8 ):
```

### Comparing `scoda-tk-0.3.0/src/scoda/misc.py` & `scoda-tk-0.3.1/src/scoda/misc.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.0/src/scoda/pipeline.py` & `scoda-tk-0.3.1/src/scoda/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     #'''
     X_cnv = np.array(adata.obsm['X_cnv'].todense())
     pca = False
 
     # X_cnv = adata.obsm['X_cnv_pca']
     # pca = True
 
-    df_res, results, cobj, X_pca = identify_tumor_cells(X_cnv, ref_ind, pca = pca, 
+    results, cobj, X_pca = identify_tumor_cells(X_cnv, ref_ind, pca = pca, 
                            use_cnv_score = False, clust = None, 
                            Clustering_resolution = 1, N_clusters = 30,
                            gmm_N_comp = 20, th_min = 0, refp_min = 0.9, p_exc = 0.1, 
                            dec_margin = tumor_dec_margin, n_neighbors = 15, cmd_cutoff = cmd_cutoff, 
                            gcm = gcm, plot_stat = False, use_ref = use_ref_only, 
                            cd_alpha = cd_alpha, suffix = '', Data = None, n_cores = n_cores)
 
@@ -144,23 +144,21 @@
     # adata_t.uns['cnv_adj_mat'] = adj
 
     lst1 = list(df_res.index.values)
     lst2 = list(adata_t.obs.index.values)
     rend = dict(zip(lst1, lst2))
     df_res.rename(index = rend, inplace = True)
 
-    adata_t.obsm['cnv_addon_summary'] = df_res ## except tumor_cluster
-
     adata_t.obs['celltype_minor_rev'] = adata_t.obs['celltype_minor'].copy(deep = True).astype(str)
     b = (adata_t.obs['tumor_dec'] == 'Tumor')
     if ref_types is not None:
         b = b & (~adata_t.obs['celltype_major'].isin(ref_types))
     adata_t.obs.loc[b, 'celltype_minor_rev'] = 'Tumor cell'
 
-    return df_res
+    return 
 
 
 def scoda_cci( adata_t, cpdb_path, cond_col = 'condition', sample_col = 'sample', 
                unit_of_cci_run = 'sample', min_n_cells_for_cci = 40, 
                data_dir = '.', pval_max = 0.1, mean_min = 0, Rth = 0.5, n_cores = 4,
                print_prefix = ''):
```

### Comparing `scoda-tk-0.3.0/src/scoda/viz.py` & `scoda-tk-0.3.1/src/scoda/viz.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.0/src/scoda_tk.egg-info/PKG-INFO` & `scoda-tk-0.3.1/src/scoda_tk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.3.0
+Version: 0.3.1
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.3.0/src/scoda_tk.egg-info/SOURCES.txt` & `scoda-tk-0.3.1/src/scoda_tk.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/scoda-tk-0.3.2.tar.gz` & `tmp/scoda-tk-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoda-tk-0.3.2.tar", last modified: Wed Aug  2 08:55:27 2023, max compression
+gzip compressed data, was "scoda-tk-0.3.3.tar", last modified: Wed Aug  2 10:07:23 2023, max compression
```

## Comparing `scoda-tk-0.3.2.tar` & `scoda-tk-0.3.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 08:55:27.714121 scoda-tk-0.3.2/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-30 14:49:21.000000 scoda-tk-0.3.2/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-07-30 14:49:22.000000 scoda-tk-0.3.2/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-02 08:55:27.714121 scoda-tk-0.3.2/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-30 14:49:22.000000 scoda-tk-0.3.2/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-08-02 08:55:14.000000 scoda-tk-0.3.2/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-08-02 08:55:27.714121 scoda-tk-0.3.2/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-30 14:49:21.000000 scoda-tk-0.3.2/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 08:55:27.694122 scoda-tk-0.3.2/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 08:55:27.694122 scoda-tk-0.3.2/src/scoda/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-30 14:49:25.000000 scoda-tk-0.3.2/src/scoda/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-30 14:49:23.000000 scoda-tk-0.3.2/src/scoda/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 08:55:27.710121 scoda-tk-0.3.2/src/scoda/default_optional_files/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-07-30 14:49:23.000000 scoda-tk-0.3.2/src/scoda/default_optional_files/analysis_config.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-07-30 14:49:24.000000 scoda-tk-0.3.2/src/scoda/default_optional_files/cpdb.zip
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-07-30 14:49:24.000000 scoda-tk-0.3.2/src/scoda/default_optional_files/hg38_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-07-30 14:49:23.000000 scoda-tk-0.3.2/src/scoda/default_optional_files/markers_hs.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-07-30 14:49:23.000000 scoda-tk-0.3.2/src/scoda/default_optional_files/markers_mm.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-07-30 14:49:25.000000 scoda-tk-0.3.2/src/scoda/default_optional_files/mm10_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-07-30 14:49:23.000000 scoda-tk-0.3.2/src/scoda/default_optional_files/msig.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    17850 2023-07-30 14:49:25.000000 scoda-tk-0.3.2/src/scoda/deg.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    13716 2023-07-30 14:49:22.000000 scoda-tk-0.3.2/src/scoda/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-07-30 14:49:22.000000 scoda-tk-0.3.2/src/scoda/hicat.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    33925 2023-08-02 08:55:06.000000 scoda-tk-0.3.2/src/scoda/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-07-30 14:49:25.000000 scoda-tk-0.3.2/src/scoda/misc.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    23452 2023-08-02 08:53:56.000000 scoda-tk-0.3.2/src/scoda/pipeline.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    63580 2023-08-02 08:47:34.000000 scoda-tk-0.3.2/src/scoda/viz.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 08:55:27.714121 scoda-tk-0.3.2/src/scoda_tk.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-02 08:55:27.000000 scoda-tk-0.3.2/src/scoda_tk.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      776 2023-08-02 08:55:27.000000 scoda-tk-0.3.2/src/scoda_tk.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-08-02 08:55:27.000000 scoda-tk-0.3.2/src/scoda_tk.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-08-02 08:55:27.000000 scoda-tk-0.3.2/src/scoda_tk.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-08-02 08:55:27.000000 scoda-tk-0.3.2/src/scoda_tk.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-08-02 08:55:27.000000 scoda-tk-0.3.2/src/scoda_tk.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 10:07:23.251197 scoda-tk-0.3.3/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-30 14:49:21.000000 scoda-tk-0.3.3/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-07-30 14:49:22.000000 scoda-tk-0.3.3/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-02 10:07:23.251197 scoda-tk-0.3.3/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-30 14:49:22.000000 scoda-tk-0.3.3/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-08-02 10:07:08.000000 scoda-tk-0.3.3/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-08-02 10:07:23.251197 scoda-tk-0.3.3/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-30 14:49:21.000000 scoda-tk-0.3.3/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 10:07:23.227198 scoda-tk-0.3.3/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 10:07:23.231198 scoda-tk-0.3.3/src/scoda/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-30 14:49:25.000000 scoda-tk-0.3.3/src/scoda/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-30 14:49:23.000000 scoda-tk-0.3.3/src/scoda/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 10:07:23.251197 scoda-tk-0.3.3/src/scoda/default_optional_files/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-07-30 14:49:23.000000 scoda-tk-0.3.3/src/scoda/default_optional_files/analysis_config.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-07-30 14:49:24.000000 scoda-tk-0.3.3/src/scoda/default_optional_files/cpdb.zip
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-07-30 14:49:24.000000 scoda-tk-0.3.3/src/scoda/default_optional_files/hg38_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-07-30 14:49:23.000000 scoda-tk-0.3.3/src/scoda/default_optional_files/markers_hs.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-07-30 14:49:23.000000 scoda-tk-0.3.3/src/scoda/default_optional_files/markers_mm.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-07-30 14:49:25.000000 scoda-tk-0.3.3/src/scoda/default_optional_files/mm10_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-07-30 14:49:23.000000 scoda-tk-0.3.3/src/scoda/default_optional_files/msig.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    18849 2023-08-02 10:04:25.000000 scoda-tk-0.3.3/src/scoda/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    13768 2023-08-02 09:47:58.000000 scoda-tk-0.3.3/src/scoda/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-07-30 14:49:22.000000 scoda-tk-0.3.3/src/scoda/hicat.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    33925 2023-08-02 08:55:06.000000 scoda-tk-0.3.3/src/scoda/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-07-30 14:49:25.000000 scoda-tk-0.3.3/src/scoda/misc.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    23211 2023-08-02 10:04:19.000000 scoda-tk-0.3.3/src/scoda/pipeline.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    63576 2023-08-02 10:03:00.000000 scoda-tk-0.3.3/src/scoda/viz.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 10:07:23.251197 scoda-tk-0.3.3/src/scoda_tk.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-02 10:07:23.000000 scoda-tk-0.3.3/src/scoda_tk.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      776 2023-08-02 10:07:23.000000 scoda-tk-0.3.3/src/scoda_tk.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-08-02 10:07:23.000000 scoda-tk-0.3.3/src/scoda_tk.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-08-02 10:07:23.000000 scoda-tk-0.3.3/src/scoda_tk.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-08-02 10:07:23.000000 scoda-tk-0.3.3/src/scoda_tk.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-08-02 10:07:23.000000 scoda-tk-0.3.3/src/scoda_tk.egg-info/top_level.txt
```

### Comparing `scoda-tk-0.3.2/LICENSE` & `scoda-tk-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.2/PKG-INFO` & `scoda-tk-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.3.2
+Version: 0.3.3
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.3.2/pyproject.toml` & `scoda-tk-0.3.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scoda-tk"
-version = "0.3.2"
+version = "0.3.3"
 description = "Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)"
 readme = "README.md"
 authors = [{ name = "Seokhyun Yoon", email = "syoon@dku.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `scoda-tk-0.3.2/src/scoda/cpdb.py` & `scoda-tk-0.3.3/src/scoda/cpdb.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.2/src/scoda/default_optional_files/cpdb.zip` & `scoda-tk-0.3.3/src/scoda/default_optional_files/cpdb.zip`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.2/src/scoda/default_optional_files/hg38_gene_only.gtf` & `scoda-tk-0.3.3/src/scoda/default_optional_files/hg38_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.2/src/scoda/default_optional_files/markers_hs.tsv` & `scoda-tk-0.3.3/src/scoda/default_optional_files/markers_hs.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.2/src/scoda/default_optional_files/markers_mm.tsv` & `scoda-tk-0.3.3/src/scoda/default_optional_files/markers_mm.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.2/src/scoda/default_optional_files/mm10_gene_only.gtf` & `scoda-tk-0.3.3/src/scoda/default_optional_files/mm10_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.2/src/scoda/default_optional_files/msig.gmt` & `scoda-tk-0.3.3/src/scoda/default_optional_files/msig.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.2/src/scoda/deg.py` & `scoda-tk-0.3.3/src/scoda/deg.py`

 * *Files 4% similar despite different names*

```diff
@@ -251,14 +251,48 @@
         for k in range(nr*nc - len(items)):
             axes[nr-1][len(items)%nc + k].axis("off")
         
     plt.show()
     return
 
 
+def select_samples( adata_s, sample_col, N_min = 100, R_max = 2.5, verbose = False ):
+
+    pcnt = adata_s.obs[sample_col].value_counts()
+    b = pcnt >= N_min
+    plst = list(pcnt.index.values[b])
+
+    N_min = int(max(pcnt.min(), N_min))
+    N_max = int(N_min*R_max)
+
+    ## Check basic stats.
+    pcnt = adata_s.obs[sample_col].value_counts()
+
+    psel = []
+    cnt = 0
+    for p in list(pcnt.index):
+        b = adata_s.obs[sample_col] == p
+        pids = list(adata_s.obs.index.values[b])
+        if len(pids) > N_max:
+            pids = random.sample(pids, N_max)
+        psel = psel + pids
+        cnt += 1
+
+    adata_t = adata_s[psel,:]
+
+    if verbose:
+        print('N_min/max: %i/%i, N_cells: %i -> %i, N_samples: %i -> %i, N_cells/sample: %4.2f' % 
+              (pcnt.min(), N_max, pcnt.sum(), len(psel), len(pcnt), cnt, len(psel)/cnt))
+        if pcnt.min() < N_min:
+            pcnt = adata_t.obs[sample_col].value_counts()
+            print(pcnt)
+    
+    return adata_t
+
+
 ######## DEG ##########
 
 MIN_VALUE = 1e-10
 MIN_VALUE_EF = 1e-10
 
 def perform_deg( df_cbyg_in, groups, target_group, n = 2, min_ef = 0.05, exp_only = False ):
     
@@ -330,15 +364,15 @@
             
     df = df.sort_values(by = 'nz_pct_score', ascending = False)
         
     return df
 
 
 def deg_multi( df_cbyg_in, groups_in, ref_group = None, samples_in = None,
-               min_ef = 0.05, exp_only = False, min_frac = 0.1 ):
+               min_exp_frac = 0.05, exp_only = False, min_frac = 0.1 ):
 
     glst = list(set(list(groups_in)))
     glst.sort()
     
     if not isinstance(groups_in, pd.Series):
         groups_in = pd.Series(groups_in, index = df_cbyg_in.index.values)
 
@@ -364,15 +398,15 @@
                 b = groups_in.isin([g, ref_group])
                 groups = groups_in[b]
                 df_cbyg = df_cbyg_in.loc[b,:]
 
         n_cells_info = {g: np.sum(~b), ref_g: np.sum(b)}
                 
         df_deg = perform_deg( df_cbyg, groups, target_group = g, 
-                              min_ef = min_ef, exp_only = exp_only )
+                              min_ef = min_exp_frac, exp_only = exp_only )
         key = '%s_vs_%s' % (g, ref_g)
         df_lst[key] = df_deg
         n_cells_lst[key] = n_cells_info
 
         if samples_in is not None:
             if len(samples_in) == df_cbyg_in.shape[0]:
                 b = groups_in == g
```

### Comparing `scoda-tk-0.3.2/src/scoda/gsea.py` & `scoda-tk-0.3.3/src/scoda/gsea.py`

 * *Files 1% similar despite different names*

```diff
@@ -329,15 +329,15 @@
                         verbose = verbose )
 
     if verbose: print('  Num. of selected pathways in GSEA: ', df_gsea.shape[0])
     
     return gene_rank, df_res_enr, df_res_pr, df_gsea
 
 
-def select_samples( adata_s, sample_col, N_min = 100, R_max = 2.5 ):
+def select_samples( adata_s, sample_col, N_min = 100, R_max = 2.5, verbose = False ):
 
     pcnt = adata_s.obs[sample_col].value_counts()
     b = pcnt >= N_min
     plst = list(pcnt.index.values[b])
 
     N_min = int(max(pcnt.min(), N_min))
     N_max = int(N_min*R_max)
@@ -353,15 +353,15 @@
         if len(pids) > N_max:
             pids = random.sample(pids, N_max)
         psel = psel + pids
         cnt += 1
 
     adata_t = adata_s[psel,:]
 
-    print('N_min/max: %i/%i, N_cells: %i -> %i, N_samples: %i -> %i, N_cells/sample: %4.2f' % 
-          (pcnt.min(), N_max, pcnt.sum(), len(psel), len(pcnt), cnt, len(psel)/cnt))
-    if pcnt.min() < N_min:
-        pcnt = adata_t.obs[sample_col].value_counts()
-        print(pcnt)
+    if verbose:
+        print('N_min/max: %i/%i, N_cells: %i -> %i, N_samples: %i -> %i, N_cells/sample: %4.2f' % 
+              (pcnt.min(), N_max, pcnt.sum(), len(psel), len(pcnt), cnt, len(psel)/cnt))
+        if pcnt.min() < N_min:
+            pcnt = adata_t.obs[sample_col].value_counts()
+            print(pcnt)
     
     return adata_t
-
```

### Comparing `scoda-tk-0.3.2/src/scoda/hicat.py` & `scoda-tk-0.3.3/src/scoda/hicat.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.2/src/scoda/icnv.py` & `scoda-tk-0.3.3/src/scoda/icnv.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.2/src/scoda/misc.py` & `scoda-tk-0.3.3/src/scoda/misc.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.2/src/scoda/pipeline.py` & `scoda-tk-0.3.3/src/scoda/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,55 +104,42 @@
                      cluster_key = 'cnv_leiden', umap = False, pca = False,
                      n_cores = n_cores )
 
     #'''
     X_cnv = np.array(adata.obsm['X_cnv'].todense())
     pca = False
 
-    # X_cnv = adata.obsm['X_cnv_pca']
-    # pca = True
-
-    df_res, results, cobj, X_pca = identify_tumor_cells(X_cnv, ref_ind, pca = pca, 
+    df_res, summary, cobj, X_pca = identify_tumor_cells(X_cnv, ref_ind, pca = pca, 
                            use_cnv_score = False, clust = None, 
                            Clustering_resolution = 1, N_clusters = 30,
                            gmm_N_comp = 20, th_min = 0, refp_min = 0.9, p_exc = 0.1, 
                            dec_margin = tumor_dec_margin, n_neighbors = 15, cmd_cutoff = cmd_cutoff, 
                            gcm = gcm, plot_stat = False, use_ref = use_ref_only, 
                            cd_alpha = cd_alpha, suffix = '', Data = None, n_cores = n_cores)
 
     if not pca: adata.obsm['X_cnv_pca'] = X_pca
         
     adata_t.obsm['X_cnv'] = adata.obsm['X_cnv']
     adata_t.obsm['X_cnv_pca'] = adata.obsm['X_cnv_pca']
-
-    # adata_t.obsm['X_cnv_umap'] = adata.obsm['X_cnv_umap']
-    # adata_t.obs['cnv_leiden'] = adata.obs['cnv_leiden']
-    # adata_t.obs['cnv_score'] = adata.obs['cnv_score']
-    # adata_t.uns['cnv_neighbors'] = adata.uns['cnv_neighbors']
-    # adata_t.uns['log1p'] = adata.uns['log1p']
-    # adata_t.uns['hvg'] = adata.uns['hvg']
-    # adata_t.uns['leiden'] = adata.uns['leiden']
     adata_t.uns['cnv'] = adata.uns['cnv']
-    # adata_t.obsp = adata.obsp
 
     adata_t.obs['cnv_cluster'] = list(df_res['cnv_cluster'].astype(str))
     adata_t.obs['tumor_dec'] = list(df_res['tumor_dec'])
     adata_t.obs['tumor_score'] = list(df_res['tumor_score'])
 
     adata_t.uns['cnv_ref_celltypes'] = ref_types2
-    # adata_t.uns['cnv_clustering_obj'] = cobj
-    adata_t.uns['cnv_addon_summary'] = results
-    # adata_t.uns['cnv_adj_mat'] = adj
+    # summary['clustering_obj'] = cobj
+    adata_t.uns['cnv_addon_summary'] = summary
 
     lst1 = list(df_res.index.values)
     lst2 = list(adata_t.obs.index.values)
     rend = dict(zip(lst1, lst2))
     df_res.rename(index = rend, inplace = True)
 
-    adata_t.obsm['cnv_addon_results'] = df_res ## except tumor_cluster
+    adata_t.obsm['cnv_addon_results'] = df_res 
 
     adata_t.obs['celltype_minor_rev'] = adata_t.obs['celltype_minor'].copy(deep = True).astype(str)
     b = (adata_t.obs['tumor_dec'] == 'Tumor')
     if ref_types is not None:
         b = b & (~adata_t.obs['celltype_major'].isin(ref_types))
     adata_t.obs.loc[b, 'celltype_minor_rev'] = 'Tumor cell'
 
@@ -395,35 +382,39 @@
             s = s[:-2]
 
             print('%s   %s: %s' % (print_prefix, ct, s))
 
             bx = True
             if ref_group_for_deg is not None:
                 if ref_group_for_deg not in list(adata_s.obs[cond_col].unique()):
-                    bx = False
-                    print('%s   WARNING in GSEA: Ref group %s not present' \
+                    print('%s      WARNING in GSEA: Ref group %s not present' \
                            % (print_prefix, ref_group_for_deg))
+                    print('%s      Performing DEG in one-against-the rest mode.' \
+                           % (print_prefix))
                 
-            if ((not bx) or (pcnt.mean() < N_cells_min_per_condition)) & (ref_group_for_deg is not None):
-                print('%s   WARNING in GSEA: The number of %s looks not enough.' \
-                       % (print_prefix, ref_group_for_deg))
+            if ((not bx) or (pcnt.min() < N_cells_min_per_condition) or pcnt.shape[0] <= 1):
+                print('%s      WARNING in GSEA: The number of cells/conditions not sufficient.' \
+                       % (print_prefix))
+                print('%s      DEG for %s skipped.' % (print_prefix, ct))
             else:
 
                 df_cbyg_in = adata_s.to_df()
                 groups_in = adata_s.obs[cond_col]
                 samples_in = adata_s.obs.index.values
 
                 ref_group = ref_group_for_deg
 
                 df_lst, nc_lst = deg_multi( df_cbyg_in, groups_in, ref_group = ref_group, 
-                                    samples_in = samples_in, min_ef = 0.05, 
+                                    samples_in = samples_in, min_exp_frac = 0.05, 
                                     exp_only = False, min_frac = 0.05 )
                 df_dct_dct_deg[ct] = df_lst
                 df_dct_dct_n_cells[ct] = nc_lst
 
+                '''
+                '''
                 ## Run gseapy.prerank
                 df_lst_enrichr = {}
                 df_lst_enrichr_up = {}
                 df_lst_enrichr_dn = {}
                 df_lst_prerank = {}
                 #'''
                 for c in df_lst.keys():
@@ -495,15 +486,15 @@
 def scoda_all_in_one( adata_t, mkr_db, cpdb_path, gsea_pw_db, cnv_gtf = None, 
                       cond_col = 'condition', sample_col = 'sample', 
                       cnv_ref_list = None, cnv_cmd_cutoff = 0.03, cnv_use_ref_only = False,
                       cnv_gcm = 0.05, cnv_tdec_margin = 0.05, cnv_cd_alpha = 1, 
                       cci_run_unit = 'sample', cci_n_cells_min = 40, 
                       cci_pval_cutoff = 0.1, cci_mean_cutoff = 0, cci_rth = 0.5, 
                       deg_ref = None, deg_pval_cutoff = 0.01, deg_n_cells_min = 100, 
-                      n_cores = 4, data_dir = '.', verbose = True, prefix = ''):
+                      n_cores = 4, data_dir = '.', verbose = True, print_prefix = ''):
 
     df_mkr_db = mkr_db
     gtf_file = cnv_gtf 
     # cpdb_path = , 
     pw_db_for_gsea = gsea_pw_db 
     # cond_col = 'condition' 
     # sample_col = 'sample'
@@ -520,19 +511,19 @@
     # data_dir = '.', 
     # verbose = True, 
     # prefix = ''
     
     ################################
     ### Cell-type identification ###
 
-    if verbose: print('%sCelltype annotation running .. ' % prefix)
+    if verbose: print('%sCelltype annotation running .. ' % print_prefix)
         
     scoda_hicat(adata_t, df_mkr_db, verbose = False)
     
-    if verbose: print('%sCelltype annotation done.' % prefix)
+    if verbose: print('%sCelltype annotation done.' % print_prefix)
 
     # adata_t.write(file_h5ad)
       
     ## For client info.
     ct_lst_maj = list(adata_t.obs['celltype_major'].unique())
     ct_lst_min = list(adata_t.obs['celltype_minor'].unique())
     ct_lst_sub = list(adata_t.obs['celltype_subset'].unique())
@@ -541,57 +532,57 @@
     s = ''
     for c in ct_lst_maj:
         s = s + '%s, ' % c
     s = s[:-2]
 
     if verbose: 
         print('%s  %i major type, %i minor type, %i subset identified.' 
-               % (prefix, len(ct_lst_maj), len(ct_lst_min), len(ct_lst_sub)))
-        print('%s  Major types: %s' % (prefix, s))
+               % (print_prefix, len(ct_lst_maj), len(ct_lst_min), len(ct_lst_sub)))
+        print('%s  Major types: %s' % (print_prefix, s))
         
     #################################
     ### tumor cell identification ###
     
     if cnv_gtf is not None:
 
         ## Test without Reference 
-        if verbose: print('%sIdentifying tumor cells .. ' % prefix)
+        if verbose: print('%sIdentifying tumor cells .. ' % print_prefix)
 
         ref_types = tumor_id_ref_celltypes
 
         df = scoda_icnv_addon( adata_t, gtf_file, ref_types = ref_types, 
                                ref_key = "celltype_major", n_cores = n_cores_to_use,
                                use_ref_only = False, cmd_cutoff = 0.03, gcm = 0.05, 
                                tumor_dec_margin = 0.01, cd_alpha = cnv_cd_alpha )
         
-        if verbose: print('%sTumor cells identification done. ' % prefix)
+        if verbose: print('%sTumor cells identification done. ' % print_prefix)
         # adata_t.write(file_h5ad)
            
     #############################
     ### Cell-cell interaction ###
 
-    if verbose: print('%sInfering cell-cell interactions .. ' % prefix)
+    if verbose: print('%sInfering cell-cell interactions .. ' % print_prefix)
 
     scoda_cci( adata_t, cpdb_path, cond_col = cond_col, sample_col = sample_col, 
                unit_of_cci_run = unit_of_cci_run, n_cores = n_cores_to_use, 
                min_n_cells_for_cci = min_n_cells_for_cci, Rth = Rth,
                pval_max = cci_pval_max, mean_min = cci_mean_min, data_dir = data_dir)
     
-    if verbose: print('%sInfering cell-cell interactions done. ' % prefix)    
+    if verbose: print('%sInfering cell-cell interactions done. ' % print_prefix)    
     # adata_t.write(file_h5ad)
         
     ####################
     ### DEG analysis ###
 
-    if verbose: print('%sDEG/GSEA analysis ..       ' % prefix)
+    if verbose: print('%sDEG/GSEA analysis ..       ' % print_prefix)
     scoda_deg_gsea( adata_t, pw_db = pw_db_for_gsea, 
                     cond_col = cond_col, sample_col = sample_col, 
                     ref_group = deg_ref_group, pval_cutoff = deg_pval_cutoff, 
                     N_cells_min_per_sample = min_n_cells_for_deg, 
                     N_cells_min_per_condition = min_n_cells_for_deg, 
-                    n_cores = n_cores_to_use)
+                    n_cores = n_cores_to_use, print_prefix = print_prefix)
         
     ## Overwrite 
     # adata_t.write(file_h5ad)        
-    if verbose: print('%sDEG/GSEA analysis done.       ' % prefix)
+    if verbose: print('%sDEG/GSEA analysis done.       ' % print_prefix)
         
     return
```

### Comparing `scoda-tk-0.3.2/src/scoda/viz.py` & `scoda-tk-0.3.3/src/scoda/viz.py`

 * *Files 0% similar despite different names*

```diff
@@ -1848,16 +1848,16 @@
     plt.show()
     return
 
 
 def get_gsea_summary( gsea_res, max_log_p = 10 ):
     
     df_gse_all = {}
-    for ck in df_dct_dct.keys():
-        df_dct = df_dct_dct[ck]
+    for ck in gsea_res.keys():
+        df_dct = gsea_res[ck]
         for cs in df_dct.keys():
             case = '%s: %s' % (ck, cs)
             df_gse_all[case] = df_dct[cs]
 
     case_lst = list(df_gse_all.keys())
     pws = []
     for key in df_gse_all.keys():
```

### Comparing `scoda-tk-0.3.2/src/scoda_tk.egg-info/PKG-INFO` & `scoda-tk-0.3.3/src/scoda_tk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.3.2
+Version: 0.3.3
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.3.2/src/scoda_tk.egg-info/SOURCES.txt` & `scoda-tk-0.3.3/src/scoda_tk.egg-info/SOURCES.txt`

 * *Files identical despite different names*


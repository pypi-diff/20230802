# Comparing `tmp/scoda-tk-0.2.8.tar.gz` & `tmp/scoda-tk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoda-tk-0.2.8.tar", last modified: Tue Aug  1 19:30:20 2023, max compression
+gzip compressed data, was "scoda-tk-0.3.0.tar", last modified: Wed Aug  2 08:23:08 2023, max compression
```

## Comparing `scoda-tk-0.2.8.tar` & `scoda-tk-0.3.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-01 19:30:20.118280 scoda-tk-0.2.8/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-30 14:49:21.000000 scoda-tk-0.2.8/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-07-30 14:49:22.000000 scoda-tk-0.2.8/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-01 19:30:20.118280 scoda-tk-0.2.8/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-30 14:49:22.000000 scoda-tk-0.2.8/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-08-01 19:29:47.000000 scoda-tk-0.2.8/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-08-01 19:30:20.118280 scoda-tk-0.2.8/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-30 14:49:21.000000 scoda-tk-0.2.8/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-01 19:30:20.094281 scoda-tk-0.2.8/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-01 19:30:20.098281 scoda-tk-0.2.8/src/scoda/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-30 14:49:25.000000 scoda-tk-0.2.8/src/scoda/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-30 14:49:23.000000 scoda-tk-0.2.8/src/scoda/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-01 19:30:20.118280 scoda-tk-0.2.8/src/scoda/default_optional_files/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-07-30 14:49:23.000000 scoda-tk-0.2.8/src/scoda/default_optional_files/analysis_config.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-07-30 14:49:24.000000 scoda-tk-0.2.8/src/scoda/default_optional_files/cpdb.zip
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-07-30 14:49:24.000000 scoda-tk-0.2.8/src/scoda/default_optional_files/hg38_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-07-30 14:49:23.000000 scoda-tk-0.2.8/src/scoda/default_optional_files/markers_hs.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-07-30 14:49:23.000000 scoda-tk-0.2.8/src/scoda/default_optional_files/markers_mm.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-07-30 14:49:25.000000 scoda-tk-0.2.8/src/scoda/default_optional_files/mm10_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-07-30 14:49:23.000000 scoda-tk-0.2.8/src/scoda/default_optional_files/msig.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    17850 2023-07-30 14:49:25.000000 scoda-tk-0.2.8/src/scoda/deg.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    13716 2023-07-30 14:49:22.000000 scoda-tk-0.2.8/src/scoda/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-07-30 14:49:22.000000 scoda-tk-0.2.8/src/scoda/hicat.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    33925 2023-08-01 19:29:33.000000 scoda-tk-0.2.8/src/scoda/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-07-30 14:49:25.000000 scoda-tk-0.2.8/src/scoda/misc.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    23411 2023-08-01 19:22:11.000000 scoda-tk-0.2.8/src/scoda/pipeline.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    58085 2023-07-31 13:01:13.000000 scoda-tk-0.2.8/src/scoda/viz.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-01 19:30:20.118280 scoda-tk-0.2.8/src/scoda_tk.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-01 19:30:20.000000 scoda-tk-0.2.8/src/scoda_tk.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      776 2023-08-01 19:30:20.000000 scoda-tk-0.2.8/src/scoda_tk.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-08-01 19:30:20.000000 scoda-tk-0.2.8/src/scoda_tk.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-08-01 19:30:20.000000 scoda-tk-0.2.8/src/scoda_tk.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-08-01 19:30:20.000000 scoda-tk-0.2.8/src/scoda_tk.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-08-01 19:30:20.000000 scoda-tk-0.2.8/src/scoda_tk.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 08:23:08.347008 scoda-tk-0.3.0/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-30 14:49:21.000000 scoda-tk-0.3.0/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-07-30 14:49:22.000000 scoda-tk-0.3.0/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-02 08:23:08.347008 scoda-tk-0.3.0/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-30 14:49:22.000000 scoda-tk-0.3.0/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-08-02 08:22:53.000000 scoda-tk-0.3.0/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-08-02 08:23:08.347008 scoda-tk-0.3.0/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-30 14:49:21.000000 scoda-tk-0.3.0/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 08:23:08.203011 scoda-tk-0.3.0/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 08:23:08.211011 scoda-tk-0.3.0/src/scoda/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-30 14:49:25.000000 scoda-tk-0.3.0/src/scoda/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-30 14:49:23.000000 scoda-tk-0.3.0/src/scoda/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 08:23:08.327009 scoda-tk-0.3.0/src/scoda/default_optional_files/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-07-30 14:49:23.000000 scoda-tk-0.3.0/src/scoda/default_optional_files/analysis_config.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-07-30 14:49:24.000000 scoda-tk-0.3.0/src/scoda/default_optional_files/cpdb.zip
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-07-30 14:49:24.000000 scoda-tk-0.3.0/src/scoda/default_optional_files/hg38_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-07-30 14:49:23.000000 scoda-tk-0.3.0/src/scoda/default_optional_files/markers_hs.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-07-30 14:49:23.000000 scoda-tk-0.3.0/src/scoda/default_optional_files/markers_mm.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-07-30 14:49:25.000000 scoda-tk-0.3.0/src/scoda/default_optional_files/mm10_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-07-30 14:49:23.000000 scoda-tk-0.3.0/src/scoda/default_optional_files/msig.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    17850 2023-07-30 14:49:25.000000 scoda-tk-0.3.0/src/scoda/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    13716 2023-07-30 14:49:22.000000 scoda-tk-0.3.0/src/scoda/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-07-30 14:49:22.000000 scoda-tk-0.3.0/src/scoda/hicat.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    33925 2023-08-01 19:29:33.000000 scoda-tk-0.3.0/src/scoda/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-07-30 14:49:25.000000 scoda-tk-0.3.0/src/scoda/misc.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    23452 2023-08-02 08:22:29.000000 scoda-tk-0.3.0/src/scoda/pipeline.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    63555 2023-08-02 08:22:36.000000 scoda-tk-0.3.0/src/scoda/viz.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 08:23:08.347008 scoda-tk-0.3.0/src/scoda_tk.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-02 08:23:08.000000 scoda-tk-0.3.0/src/scoda_tk.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      776 2023-08-02 08:23:08.000000 scoda-tk-0.3.0/src/scoda_tk.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-08-02 08:23:08.000000 scoda-tk-0.3.0/src/scoda_tk.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-08-02 08:23:08.000000 scoda-tk-0.3.0/src/scoda_tk.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-08-02 08:23:08.000000 scoda-tk-0.3.0/src/scoda_tk.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-08-02 08:23:08.000000 scoda-tk-0.3.0/src/scoda_tk.egg-info/top_level.txt
```

### Comparing `scoda-tk-0.2.8/LICENSE` & `scoda-tk-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.8/PKG-INFO` & `scoda-tk-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.2.8
+Version: 0.3.0
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.2.8/src/scoda/cpdb.py` & `scoda-tk-0.3.0/src/scoda/cpdb.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.8/src/scoda/default_optional_files/cpdb.zip` & `scoda-tk-0.3.0/src/scoda/default_optional_files/cpdb.zip`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.8/src/scoda/default_optional_files/hg38_gene_only.gtf` & `scoda-tk-0.3.0/src/scoda/default_optional_files/hg38_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.8/src/scoda/default_optional_files/markers_hs.tsv` & `scoda-tk-0.3.0/src/scoda/default_optional_files/markers_hs.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.8/src/scoda/default_optional_files/markers_mm.tsv` & `scoda-tk-0.3.0/src/scoda/default_optional_files/markers_mm.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.8/src/scoda/default_optional_files/mm10_gene_only.gtf` & `scoda-tk-0.3.0/src/scoda/default_optional_files/mm10_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.8/src/scoda/default_optional_files/msig.gmt` & `scoda-tk-0.3.0/src/scoda/default_optional_files/msig.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.8/src/scoda/deg.py` & `scoda-tk-0.3.0/src/scoda/deg.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.8/src/scoda/gsea.py` & `scoda-tk-0.3.0/src/scoda/gsea.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.8/src/scoda/hicat.py` & `scoda-tk-0.3.0/src/scoda/hicat.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.8/src/scoda/icnv.py` & `scoda-tk-0.3.0/src/scoda/icnv.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.8/src/scoda/misc.py` & `scoda-tk-0.3.0/src/scoda/misc.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.2.8/src/scoda/pipeline.py` & `scoda-tk-0.3.0/src/scoda/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     ref_ind = None
 
     if ref_types is not None:
         if isinstance(ref_types, list):
             if len(ref_types) > 0:
                 ref_types2 = list(set(ref_types).intersection(adata.obs[ref_key].unique()))
                 ref_ind = adata.obs[ref_key].isin(ref_types)
-    '''
+    #'''
     adata = run_icnv(adata, ref_key, ref_types2, gtf_file, 
                      resolution = 2, N_pca = 15, n_neighbors = 10,
                      cluster_key = 'cnv_leiden', umap = False, pca = False,
                      n_cores = n_cores )
 
     #'''
     X_cnv = np.array(adata.obsm['X_cnv'].todense())
@@ -318,15 +318,16 @@
     return
 
 
 def scoda_deg_gsea( adata_t, pw_db, 
                     cond_col = 'condition', sample_col = 'sample', 
                     ref_group = None, pval_cutoff = 0.05,
                     N_cells_min_per_sample = 100, 
-                    N_cells_min_per_condition = 100, n_cores = 4): 
+                    N_cells_min_per_condition = 100, n_cores = 4, 
+                    print_prefix = ''): 
         
     # ref_group_for_deg = ref_group
     ref_group_for_deg = None
     if ref_group is not None:
         if ref_group in list(adata_t.obs[cond_col].unique()):
             ref_group_for_deg = ref_group
```

### Comparing `scoda-tk-0.2.8/src/scoda/viz.py` & `scoda-tk-0.3.0/src/scoda/viz.py`

 * *Files 3% similar despite different names*

```diff
@@ -953,25 +953,25 @@
     
     counts, bins = np.histogram(df['cmean'], bins = n_bins)
     # max_cnt = np.max(counts)
 
     legend_labels = []
     
     max_cnt = 0
-    b = df['dec'] == 'Normal'
+    b = df['tumor_dec'] == 'Normal'
     if np.sum(b) > 0:
         legend_labels.append('Normal')
         counts, bins_t, bar_t = plt.hist(df.loc[b, 'cmean'], bins = bins, alpha = alpha)
         max_cnt = max(max_cnt, np.max(counts))
-    b = df['dec'] == 'Tumor'
+    b = df['tumor_dec'] == 'Tumor'
     if np.sum(b) > 0:
         legend_labels.append('Tumor')
         counts, bins_t, bar_t = plt.hist(df.loc[b, 'cmean'], bins = bins, alpha = alpha)
         max_cnt = max(max_cnt, np.max(counts))
-    b = df['dec'] == 'unclear'
+    b = df['tumor_dec'] == 'unclear'
     if np.sum(b) > 0:
         legend_labels.append('unclear')
         counts, bins_t, bar_t = plt.hist(df.loc[b, 'cmean'], bins = bins, alpha = alpha)
         max_cnt = max(max_cnt, np.max(counts))
     
     sf = 0.9*max_cnt/max_pdf
     plt.plot(xs0, pdf0*sf)
@@ -988,15 +988,14 @@
     ax.tick_params(axis='x', labelsize=tick_fs)
     ax.tick_params(axis='y', labelsize=tick_fs)
     plt.grid()
     plt.show()
         
     return 
     
-
 ### Plot dot
 
 def remove_common( mkr_dict, prn = True ):
 
     cts = list(mkr_dict.keys())
     mkrs_all = []
     for c in cts:
@@ -1718,7 +1717,187 @@
                 ax = plt.yticks([])
                 plt.ylabel(None)
             if lims is not None: plt.xlim(lims[k])
 
         plt.show()
     return True
 
+
+import matplotlib.pyplot as plt
+import matplotlib as mpl
+
+def plot_gsea_all( df_qv, df_es, title = 'Test', title_fs = 14, 
+                   tick_fs = 10, tick_rot = 90, tick_ha = 'center',
+                   label_fs = 10, legend_fs = 10, fig_size_sf = 1,
+                   mx_pnt_size = 80, swap_ax = True ):
+                 
+    df1 = df_qv
+    df2 = df_es
+    alabel = 'Cases'
+    n = df1.shape[0]
+
+    fig_size_sf = fig_size_sf*3
+    mx_pnt_size = 20*fig_size_sf
+    
+    mn, mx = 0, 1
+    if df2 is not None:
+        mn, mx = np.floor(df2.min().min()), np.ceil(df2.max().max())
+        cbar_title = 'NES'
+    else:
+        mn, mx = np.floor(df1.min().min()), np.ceil(df1.max().max())
+        cbar_title = '-log10(P)'
+
+    mx_pv = np.ceil(df1.max().max())
+    ssf = mx_pnt_size/mx_pv
+        
+    # plt.figure(figsize = (2+1, 2*df1.shape[0]/df1.shape[1]))
+
+    if swap_ax:
+        sf = fig_size_sf/df1.shape[1]
+        xs = (df1.shape[0] + 6)
+        ys = df1.shape[1]
+        fig, ax = plt.subplots(figsize = (sf*xs, sf*ys)) 
+    else:
+        sf = fig_size_sf/df1.shape[1]
+        xs = df1.shape[1]
+        ys = (df1.shape[0] + 6)
+        fig, ax = plt.subplots(figsize = (sf*df1.shape[1], sf*(df1.shape[0] + 6))) 
+
+    norm = mpl.colors.Normalize(vmin=mn, vmax=mx)
+
+    x = []
+    y = []
+    ss = []
+    cc = []
+    for j, c in enumerate(list(df1.columns.values)):
+        if swap_ax:
+            y = y + [j]*n
+            x = x + list(np.arange(n))
+        else:
+            x = x + [j]*n
+            y = y + list(np.arange(n))
+        ss = ss + list(df1[c]*ssf)
+        if df2 is None:
+            cc = cc + list(df1[c])
+        else:
+            cc = cc + list(df2[c])
+
+    p = ax.scatter( x, y, s = ss, c = cc, cmap = plt.cm.bwr )
+
+    # plt.colorbar(p,cax=ax)
+    ax.grid('off')  
+    ax.set_title(title, fontsize = title_fs)
+
+    # Set number of ticks for x-axis
+    if swap_ax:
+        plt.ylabel(alabel)
+        ix, iy, yt_label, xt_label, fr = 0, 1, df1.columns.values, df1.index.values, 1 
+    else:
+        plt.xlabel(alabel)
+        ix, iy, yt_label, xt_label, fr = 1, 0, df1.index.values, df1.columns.values, 0.1
+
+    plt.ylim([-0.5, df1.shape[iy]-0.5])
+    plt.xlim([-0.5, df1.shape[ix]-0.5])
+
+    x = np.arange(df1.shape[ix])
+    ax.set_xticks(x)
+    # Set ticks labels for x-axis
+    x_ticks_labels = list(xt_label)
+    ax.set_xticklabels(x_ticks_labels, rotation=tick_rot, ha = tick_ha, fontsize=tick_fs)
+
+    # Set number of ticks for x-axis
+    y = np.arange(df1.shape[iy])
+    ax.set_yticks(y)
+    # Set ticks labels for x-axis
+    y_ticks_labels = list(yt_label)
+    a = ax.set_yticklabels(y_ticks_labels, rotation=0, fontsize=tick_fs)
+
+    # Adding the colorbar
+    if swap_ax:
+        lgap = 0.007
+        frac = 0.1
+        cbaxes = fig.add_axes([0.91, 0.6, 0.1*df1.shape[1]/df1.shape[0], 0.25]) 
+    else:
+        lgap = 0.02 # 0.005
+        frac = 0.2
+        r = df1.shape[1]/df1.shape[0]
+        cbaxes = fig.add_axes([0.95, 0.6, 0.1*(1-df1.shape[1]/30), 0.1]) 
+
+    cmap = p.cmap
+    cbar = plt.colorbar(mpl.cm.ScalarMappable(norm=norm, cmap=cmap),ax=ax, 
+                        fraction = frac, cax = cbaxes)
+    # if df2 is not None:
+    cbar.set_label(cbar_title, fontsize = label_fs)
+    for t in cbar.ax.get_yticklabels():
+        t.set_fontsize(tick_fs)
+
+    #'''
+    if swap_ax:
+        nn = 4 # list(np.arange(1,mx_pv,2)) 
+        kw = dict(prop="sizes", num=nn, fmt="{x:1.0f}", func=lambda s: s/ssf, color = 'grey')
+        legend = ax.legend(*p.legend_elements(**kw), title = '-log(P)',
+                       fontsize = legend_fs, title_fontsize=legend_fs,
+                       loc = 'upper left', bbox_to_anchor = (1+lgap, 0.55) )
+    else:
+        nn = int(mx_pv)
+        kw = dict(prop="sizes", num=nn, fmt="{x:1.0f}", func=lambda s: s/ssf, color = 'grey')
+        legend = ax.legend(*p.legend_elements(**kw), title = '-log(P)',
+                       fontsize = legend_fs, title_fontsize=legend_fs,
+                       loc = 'upper left', bbox_to_anchor = (1+lgap, 0.5) )
+    #'''
+    plt.show()
+    return
+
+
+def get_gsea_summary( gsea_res, max_log_p = 10 ):
+    
+    df_gse_all = {}
+    for ck in df_dct_dct.keys():
+        df_dct = df_dct_dct[ck]
+        for cs in df_dct.keys():
+            case = '%s: %s' % (ck, cs)
+            df_gse_all[case] = df_dct[cs]
+
+    case_lst = list(df_gse_all.keys())
+    pws = []
+    for key in df_gse_all.keys():
+        df = df_gse_all[key]
+        pws = list(set(pws).union(list(df.index.values)))
+
+    pws.sort(reverse = True)
+
+    dfc_qv = pd.DataFrame(0, index = pws, columns = case_lst)
+    dfc_es = pd.DataFrame(0, index = pws, columns = case_lst)
+    cnt_es = 0
+
+    for case in df_gse_all.keys():
+
+        df = df_gse_all[case]
+
+        col1 = '%s' % case
+        col2 = '%s' % case
+
+        dfc_qv.loc[:,col1] = 0
+        dfc_es.loc[:,col2] = 0
+
+        b = ~df['-log(p-val)'].isnull()
+        dfc_qv.loc[list(df.index[b]), col1] = list(df.loc[b, '-log(p-val)'])
+        if 'NES' in list(df.columns.values):
+            b = ~df['NES'].isnull()
+            cnt_es += np.sum(b)
+            dfc_es.loc[list(df.index[b]), col2] = list(df.loc[b, 'NES'])
+
+    display(dfc_qv.head())
+
+    pw_sel = pws
+
+    if cnt_es > 0:
+        b = dfc_es.max(axis = 1) > 0
+        df_qv = dfc_qv.loc[b,:] 
+        df_es = dfc_es.loc[b,:] 
+    else:
+        df_qv = dfc_qv
+        df_es = None
+
+    df_qv = df_qv.clip(upper = max_log_p)
+    
+    return df_qv, df_es
```

### Comparing `scoda-tk-0.2.8/src/scoda_tk.egg-info/PKG-INFO` & `scoda-tk-0.3.0/src/scoda_tk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.2.8
+Version: 0.3.0
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.2.8/src/scoda_tk.egg-info/SOURCES.txt` & `scoda-tk-0.3.0/src/scoda_tk.egg-info/SOURCES.txt`

 * *Files identical despite different names*


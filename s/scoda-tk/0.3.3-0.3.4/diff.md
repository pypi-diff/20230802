# Comparing `tmp/scoda-tk-0.3.3.tar.gz` & `tmp/scoda-tk-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoda-tk-0.3.3.tar", last modified: Wed Aug  2 10:07:23 2023, max compression
+gzip compressed data, was "scoda-tk-0.3.4.tar", last modified: Wed Aug  2 13:32:02 2023, max compression
```

## Comparing `scoda-tk-0.3.3.tar` & `scoda-tk-0.3.4.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 10:07:23.251197 scoda-tk-0.3.3/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-30 14:49:21.000000 scoda-tk-0.3.3/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-07-30 14:49:22.000000 scoda-tk-0.3.3/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-02 10:07:23.251197 scoda-tk-0.3.3/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-30 14:49:22.000000 scoda-tk-0.3.3/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-08-02 10:07:08.000000 scoda-tk-0.3.3/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-08-02 10:07:23.251197 scoda-tk-0.3.3/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-30 14:49:21.000000 scoda-tk-0.3.3/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 10:07:23.227198 scoda-tk-0.3.3/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 10:07:23.231198 scoda-tk-0.3.3/src/scoda/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-30 14:49:25.000000 scoda-tk-0.3.3/src/scoda/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-30 14:49:23.000000 scoda-tk-0.3.3/src/scoda/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 10:07:23.251197 scoda-tk-0.3.3/src/scoda/default_optional_files/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-07-30 14:49:23.000000 scoda-tk-0.3.3/src/scoda/default_optional_files/analysis_config.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-07-30 14:49:24.000000 scoda-tk-0.3.3/src/scoda/default_optional_files/cpdb.zip
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-07-30 14:49:24.000000 scoda-tk-0.3.3/src/scoda/default_optional_files/hg38_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-07-30 14:49:23.000000 scoda-tk-0.3.3/src/scoda/default_optional_files/markers_hs.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-07-30 14:49:23.000000 scoda-tk-0.3.3/src/scoda/default_optional_files/markers_mm.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-07-30 14:49:25.000000 scoda-tk-0.3.3/src/scoda/default_optional_files/mm10_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-07-30 14:49:23.000000 scoda-tk-0.3.3/src/scoda/default_optional_files/msig.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    18849 2023-08-02 10:04:25.000000 scoda-tk-0.3.3/src/scoda/deg.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    13768 2023-08-02 09:47:58.000000 scoda-tk-0.3.3/src/scoda/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-07-30 14:49:22.000000 scoda-tk-0.3.3/src/scoda/hicat.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    33925 2023-08-02 08:55:06.000000 scoda-tk-0.3.3/src/scoda/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-07-30 14:49:25.000000 scoda-tk-0.3.3/src/scoda/misc.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    23211 2023-08-02 10:04:19.000000 scoda-tk-0.3.3/src/scoda/pipeline.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    63576 2023-08-02 10:03:00.000000 scoda-tk-0.3.3/src/scoda/viz.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 10:07:23.251197 scoda-tk-0.3.3/src/scoda_tk.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-02 10:07:23.000000 scoda-tk-0.3.3/src/scoda_tk.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      776 2023-08-02 10:07:23.000000 scoda-tk-0.3.3/src/scoda_tk.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-08-02 10:07:23.000000 scoda-tk-0.3.3/src/scoda_tk.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-08-02 10:07:23.000000 scoda-tk-0.3.3/src/scoda_tk.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-08-02 10:07:23.000000 scoda-tk-0.3.3/src/scoda_tk.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-08-02 10:07:23.000000 scoda-tk-0.3.3/src/scoda_tk.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 13:32:02.058476 scoda-tk-0.3.4/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-08-02 12:34:47.000000 scoda-tk-0.3.4/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-08-02 12:34:47.000000 scoda-tk-0.3.4/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-02 13:32:02.058476 scoda-tk-0.3.4/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-08-02 12:34:48.000000 scoda-tk-0.3.4/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-08-02 13:31:12.000000 scoda-tk-0.3.4/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-08-02 13:32:02.058476 scoda-tk-0.3.4/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-08-02 12:34:47.000000 scoda-tk-0.3.4/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 13:32:02.034477 scoda-tk-0.3.4/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 13:32:02.038477 scoda-tk-0.3.4/src/scoda/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-08-02 12:34:52.000000 scoda-tk-0.3.4/src/scoda/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-08-02 12:34:49.000000 scoda-tk-0.3.4/src/scoda/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 13:32:02.058476 scoda-tk-0.3.4/src/scoda/default_optional_files/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-08-02 12:34:49.000000 scoda-tk-0.3.4/src/scoda/default_optional_files/analysis_config.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-08-02 12:34:50.000000 scoda-tk-0.3.4/src/scoda/default_optional_files/cpdb.zip
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-08-02 12:34:51.000000 scoda-tk-0.3.4/src/scoda/default_optional_files/hg38_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   216264 2023-08-02 13:29:18.000000 scoda-tk-0.3.4/src/scoda/default_optional_files/kegg_human.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   200990 2023-08-02 13:29:18.000000 scoda-tk-0.3.4/src/scoda/default_optional_files/kegg_mouse.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-08-02 12:34:49.000000 scoda-tk-0.3.4/src/scoda/default_optional_files/markers_hs.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-08-02 12:34:49.000000 scoda-tk-0.3.4/src/scoda/default_optional_files/markers_mm.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-08-02 12:34:52.000000 scoda-tk-0.3.4/src/scoda/default_optional_files/mm10_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-08-02 13:30:21.000000 scoda-tk-0.3.4/src/scoda/default_optional_files/msig.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    18849 2023-08-02 12:34:52.000000 scoda-tk-0.3.4/src/scoda/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    13768 2023-08-02 12:34:48.000000 scoda-tk-0.3.4/src/scoda/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-08-02 12:34:48.000000 scoda-tk-0.3.4/src/scoda/hicat.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    33986 2023-08-02 12:34:51.000000 scoda-tk-0.3.4/src/scoda/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-08-02 12:34:52.000000 scoda-tk-0.3.4/src/scoda/misc.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    23145 2023-08-02 12:34:48.000000 scoda-tk-0.3.4/src/scoda/pipeline.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    63576 2023-08-02 12:34:52.000000 scoda-tk-0.3.4/src/scoda/viz.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 13:32:02.058476 scoda-tk-0.3.4/src/scoda_tk.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-02 13:32:02.000000 scoda-tk-0.3.4/src/scoda_tk.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      872 2023-08-02 13:32:02.000000 scoda-tk-0.3.4/src/scoda_tk.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-08-02 13:32:02.000000 scoda-tk-0.3.4/src/scoda_tk.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-08-02 13:32:02.000000 scoda-tk-0.3.4/src/scoda_tk.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-08-02 13:32:02.000000 scoda-tk-0.3.4/src/scoda_tk.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-08-02 13:32:02.000000 scoda-tk-0.3.4/src/scoda_tk.egg-info/top_level.txt
```

### Comparing `scoda-tk-0.3.3/LICENSE` & `scoda-tk-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.3/PKG-INFO` & `scoda-tk-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.3.3
+Version: 0.3.4
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.3.3/pyproject.toml` & `scoda-tk-0.3.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scoda-tk"
-version = "0.3.3"
+version = "0.3.4"
 description = "Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)"
 readme = "README.md"
 authors = [{ name = "Seokhyun Yoon", email = "syoon@dku.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `scoda-tk-0.3.3/src/scoda/cpdb.py` & `scoda-tk-0.3.4/src/scoda/cpdb.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.3/src/scoda/default_optional_files/cpdb.zip` & `scoda-tk-0.3.4/src/scoda/default_optional_files/cpdb.zip`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.3/src/scoda/default_optional_files/hg38_gene_only.gtf` & `scoda-tk-0.3.4/src/scoda/default_optional_files/hg38_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.3/src/scoda/default_optional_files/markers_hs.tsv` & `scoda-tk-0.3.4/src/scoda/default_optional_files/markers_hs.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.3/src/scoda/default_optional_files/markers_mm.tsv` & `scoda-tk-0.3.4/src/scoda/default_optional_files/markers_mm.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.3/src/scoda/default_optional_files/mm10_gene_only.gtf` & `scoda-tk-0.3.4/src/scoda/default_optional_files/mm10_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.3/src/scoda/default_optional_files/msig.gmt` & `scoda-tk-0.3.4/src/scoda/default_optional_files/msig.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.3/src/scoda/deg.py` & `scoda-tk-0.3.4/src/scoda/deg.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.3/src/scoda/gsea.py` & `scoda-tk-0.3.4/src/scoda/gsea.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.3/src/scoda/hicat.py` & `scoda-tk-0.3.4/src/scoda/hicat.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.3/src/scoda/icnv.py` & `scoda-tk-0.3.4/src/scoda/icnv.py`

 * *Files 2% similar despite different names*

```diff
@@ -693,15 +693,16 @@
 from sklearn.neighbors import NearestNeighbors
 
 CLUSTERING_AGO = 'lv'
 SKNETWORK = True
 try:
     from sknetwork.clustering import Louvain
 except ImportError:
-    print('ERROR: sknetwork not installed.')
+    print('WARNING: sknetwork not installed. GMM will be used for clustering.')
+    CLUSTERING_AGO = 'gm'
     SKNETWORK = False
 
     
 def clustering_alg(X_pca, clust_algo = 'lv', N_clusters = 25, resolution = 1, N_neighbors = 10, 
                    mode='connectivity', n_cores = 4):
                    # mode='distance', n_cores = 4):
```

### Comparing `scoda-tk-0.3.3/src/scoda/misc.py` & `scoda-tk-0.3.4/src/scoda/misc.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.3/src/scoda/pipeline.py` & `scoda-tk-0.3.4/src/scoda/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -467,16 +467,14 @@
 
                 df_dct_dct_enr_up[ct] = df_lst_enrichr_up
                 df_dct_dct_enr_dn[ct] = df_lst_enrichr_dn
                 df_dct_dct_enr[ct] = df_lst_enrichr
                 df_dct_dct_pr[ct] = df_lst_prerank
                 # '''
 
-        print('%sDEG/GSEA analysis done.       ' % print_prefix)
-
         adata_t.uns['DEG_stat'] = df_dct_dct_n_cells
         adata_t.uns['DEG'] = df_dct_dct_deg
         # adata_t.uns['GSA'] = df_dct_dct_enr
         adata_t.uns['GSA_up'] = df_dct_dct_enr_up
         adata_t.uns['GSA_down'] = df_dct_dct_enr_dn
         adata_t.uns['GSEA'] = df_dct_dct_pr
```

### Comparing `scoda-tk-0.3.3/src/scoda/viz.py` & `scoda-tk-0.3.4/src/scoda/viz.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.3/src/scoda_tk.egg-info/PKG-INFO` & `scoda-tk-0.3.4/src/scoda_tk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.3.3
+Version: 0.3.4
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.3.3/src/scoda_tk.egg-info/SOURCES.txt` & `scoda-tk-0.3.4/src/scoda_tk.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 src/scoda/icnv.py
 src/scoda/misc.py
 src/scoda/pipeline.py
 src/scoda/viz.py
 src/scoda/default_optional_files/analysis_config.py
 src/scoda/default_optional_files/cpdb.zip
 src/scoda/default_optional_files/hg38_gene_only.gtf
+src/scoda/default_optional_files/kegg_human.gmt
+src/scoda/default_optional_files/kegg_mouse.gmt
 src/scoda/default_optional_files/markers_hs.tsv
 src/scoda/default_optional_files/markers_mm.tsv
 src/scoda/default_optional_files/mm10_gene_only.gtf
 src/scoda/default_optional_files/msig.gmt
 src/scoda_tk.egg-info/PKG-INFO
 src/scoda_tk.egg-info/SOURCES.txt
 src/scoda_tk.egg-info/dependency_links.txt
```


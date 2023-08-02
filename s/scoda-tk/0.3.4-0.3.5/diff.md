# Comparing `tmp/scoda-tk-0.3.4.tar.gz` & `tmp/scoda-tk-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoda-tk-0.3.4.tar", last modified: Wed Aug  2 13:32:02 2023, max compression
+gzip compressed data, was "scoda-tk-0.3.5.tar", last modified: Wed Aug  2 14:38:42 2023, max compression
```

## Comparing `scoda-tk-0.3.4.tar` & `scoda-tk-0.3.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 13:32:02.058476 scoda-tk-0.3.4/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-08-02 12:34:47.000000 scoda-tk-0.3.4/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-08-02 12:34:47.000000 scoda-tk-0.3.4/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-02 13:32:02.058476 scoda-tk-0.3.4/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-08-02 12:34:48.000000 scoda-tk-0.3.4/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-08-02 13:31:12.000000 scoda-tk-0.3.4/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-08-02 13:32:02.058476 scoda-tk-0.3.4/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-08-02 12:34:47.000000 scoda-tk-0.3.4/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 13:32:02.034477 scoda-tk-0.3.4/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 13:32:02.038477 scoda-tk-0.3.4/src/scoda/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-08-02 12:34:52.000000 scoda-tk-0.3.4/src/scoda/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-08-02 12:34:49.000000 scoda-tk-0.3.4/src/scoda/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 13:32:02.058476 scoda-tk-0.3.4/src/scoda/default_optional_files/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-08-02 12:34:49.000000 scoda-tk-0.3.4/src/scoda/default_optional_files/analysis_config.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-08-02 12:34:50.000000 scoda-tk-0.3.4/src/scoda/default_optional_files/cpdb.zip
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-08-02 12:34:51.000000 scoda-tk-0.3.4/src/scoda/default_optional_files/hg38_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   216264 2023-08-02 13:29:18.000000 scoda-tk-0.3.4/src/scoda/default_optional_files/kegg_human.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   200990 2023-08-02 13:29:18.000000 scoda-tk-0.3.4/src/scoda/default_optional_files/kegg_mouse.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-08-02 12:34:49.000000 scoda-tk-0.3.4/src/scoda/default_optional_files/markers_hs.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-08-02 12:34:49.000000 scoda-tk-0.3.4/src/scoda/default_optional_files/markers_mm.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-08-02 12:34:52.000000 scoda-tk-0.3.4/src/scoda/default_optional_files/mm10_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-08-02 13:30:21.000000 scoda-tk-0.3.4/src/scoda/default_optional_files/msig.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    18849 2023-08-02 12:34:52.000000 scoda-tk-0.3.4/src/scoda/deg.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    13768 2023-08-02 12:34:48.000000 scoda-tk-0.3.4/src/scoda/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-08-02 12:34:48.000000 scoda-tk-0.3.4/src/scoda/hicat.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    33986 2023-08-02 12:34:51.000000 scoda-tk-0.3.4/src/scoda/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-08-02 12:34:52.000000 scoda-tk-0.3.4/src/scoda/misc.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    23145 2023-08-02 12:34:48.000000 scoda-tk-0.3.4/src/scoda/pipeline.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    63576 2023-08-02 12:34:52.000000 scoda-tk-0.3.4/src/scoda/viz.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 13:32:02.058476 scoda-tk-0.3.4/src/scoda_tk.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-02 13:32:02.000000 scoda-tk-0.3.4/src/scoda_tk.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      872 2023-08-02 13:32:02.000000 scoda-tk-0.3.4/src/scoda_tk.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-08-02 13:32:02.000000 scoda-tk-0.3.4/src/scoda_tk.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-08-02 13:32:02.000000 scoda-tk-0.3.4/src/scoda_tk.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-08-02 13:32:02.000000 scoda-tk-0.3.4/src/scoda_tk.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-08-02 13:32:02.000000 scoda-tk-0.3.4/src/scoda_tk.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 14:38:42.982785 scoda-tk-0.3.5/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-08-02 12:34:47.000000 scoda-tk-0.3.5/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-08-02 12:34:47.000000 scoda-tk-0.3.5/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-02 14:38:42.982785 scoda-tk-0.3.5/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-08-02 12:34:48.000000 scoda-tk-0.3.5/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-08-02 14:38:04.000000 scoda-tk-0.3.5/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-08-02 14:38:42.982785 scoda-tk-0.3.5/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-08-02 12:34:47.000000 scoda-tk-0.3.5/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 14:38:42.866788 scoda-tk-0.3.5/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 14:38:42.906787 scoda-tk-0.3.5/src/scoda/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-08-02 12:34:52.000000 scoda-tk-0.3.5/src/scoda/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-08-02 12:34:49.000000 scoda-tk-0.3.5/src/scoda/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 14:38:42.982785 scoda-tk-0.3.5/src/scoda/default_optional_files/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-08-02 12:34:49.000000 scoda-tk-0.3.5/src/scoda/default_optional_files/analysis_config.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-08-02 12:34:50.000000 scoda-tk-0.3.5/src/scoda/default_optional_files/cpdb.zip
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-08-02 12:34:51.000000 scoda-tk-0.3.5/src/scoda/default_optional_files/hg38_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   216264 2023-08-02 13:29:18.000000 scoda-tk-0.3.5/src/scoda/default_optional_files/kegg_human.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   200990 2023-08-02 13:29:18.000000 scoda-tk-0.3.5/src/scoda/default_optional_files/kegg_mouse.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-08-02 12:34:49.000000 scoda-tk-0.3.5/src/scoda/default_optional_files/markers_hs.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-08-02 12:34:49.000000 scoda-tk-0.3.5/src/scoda/default_optional_files/markers_mm.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-08-02 12:34:52.000000 scoda-tk-0.3.5/src/scoda/default_optional_files/mm10_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-08-02 13:30:21.000000 scoda-tk-0.3.5/src/scoda/default_optional_files/msig.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    18849 2023-08-02 12:34:52.000000 scoda-tk-0.3.5/src/scoda/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    13768 2023-08-02 12:34:48.000000 scoda-tk-0.3.5/src/scoda/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-08-02 12:34:48.000000 scoda-tk-0.3.5/src/scoda/hicat.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    33986 2023-08-02 12:34:51.000000 scoda-tk-0.3.5/src/scoda/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-08-02 12:34:52.000000 scoda-tk-0.3.5/src/scoda/misc.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    23145 2023-08-02 12:34:48.000000 scoda-tk-0.3.5/src/scoda/pipeline.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    63794 2023-08-02 14:36:37.000000 scoda-tk-0.3.5/src/scoda/viz.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 14:38:42.982785 scoda-tk-0.3.5/src/scoda_tk.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-02 14:38:42.000000 scoda-tk-0.3.5/src/scoda_tk.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      872 2023-08-02 14:38:42.000000 scoda-tk-0.3.5/src/scoda_tk.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-08-02 14:38:42.000000 scoda-tk-0.3.5/src/scoda_tk.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-08-02 14:38:42.000000 scoda-tk-0.3.5/src/scoda_tk.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-08-02 14:38:42.000000 scoda-tk-0.3.5/src/scoda_tk.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-08-02 14:38:42.000000 scoda-tk-0.3.5/src/scoda_tk.egg-info/top_level.txt
```

### Comparing `scoda-tk-0.3.4/LICENSE` & `scoda-tk-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.4/PKG-INFO` & `scoda-tk-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.3.4
+Version: 0.3.5
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.3.4/pyproject.toml` & `scoda-tk-0.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scoda-tk"
-version = "0.3.4"
+version = "0.3.5"
 description = "Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)"
 readme = "README.md"
 authors = [{ name = "Seokhyun Yoon", email = "syoon@dku.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `scoda-tk-0.3.4/src/scoda/cpdb.py` & `scoda-tk-0.3.5/src/scoda/cpdb.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.4/src/scoda/default_optional_files/cpdb.zip` & `scoda-tk-0.3.5/src/scoda/default_optional_files/cpdb.zip`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.4/src/scoda/default_optional_files/hg38_gene_only.gtf` & `scoda-tk-0.3.5/src/scoda/default_optional_files/hg38_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.4/src/scoda/default_optional_files/kegg_human.gmt` & `scoda-tk-0.3.5/src/scoda/default_optional_files/kegg_human.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.4/src/scoda/default_optional_files/kegg_mouse.gmt` & `scoda-tk-0.3.5/src/scoda/default_optional_files/kegg_mouse.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.4/src/scoda/default_optional_files/markers_hs.tsv` & `scoda-tk-0.3.5/src/scoda/default_optional_files/markers_hs.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.4/src/scoda/default_optional_files/markers_mm.tsv` & `scoda-tk-0.3.5/src/scoda/default_optional_files/markers_mm.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.4/src/scoda/default_optional_files/mm10_gene_only.gtf` & `scoda-tk-0.3.5/src/scoda/default_optional_files/mm10_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.4/src/scoda/default_optional_files/msig.gmt` & `scoda-tk-0.3.5/src/scoda/default_optional_files/msig.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.4/src/scoda/deg.py` & `scoda-tk-0.3.5/src/scoda/deg.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.4/src/scoda/gsea.py` & `scoda-tk-0.3.5/src/scoda/gsea.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.4/src/scoda/hicat.py` & `scoda-tk-0.3.5/src/scoda/hicat.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.4/src/scoda/icnv.py` & `scoda-tk-0.3.5/src/scoda/icnv.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.4/src/scoda/misc.py` & `scoda-tk-0.3.5/src/scoda/misc.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.4/src/scoda/pipeline.py` & `scoda-tk-0.3.5/src/scoda/pipeline.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.4/src/scoda/viz.py` & `scoda-tk-0.3.5/src/scoda/viz.py`

 * *Files 1% similar despite different names*

```diff
@@ -1809,45 +1809,47 @@
     y = np.arange(df1.shape[iy])
     ax.set_yticks(y)
     # Set ticks labels for x-axis
     y_ticks_labels = list(yt_label)
     a = ax.set_yticklabels(y_ticks_labels, rotation=0, fontsize=tick_fs)
 
     # Adding the colorbar
+    cmap = p.cmap
     if swap_ax:
-        lgap = 0.007
-        frac = 0.1
-        cbaxes = fig.add_axes([0.91, 0.6, 0.1*df1.shape[1]/df1.shape[0], 0.25]) 
+        lgap = 0.01
+        frac = 0.08
+        # cbaxes = fig.add_axes([0.91, 0.6, 0.1*df1.shape[1]/df1.shape[0], 0.25]) 
+        cbar = plt.colorbar(mpl.cm.ScalarMappable(norm=norm, cmap=cmap),ax=ax, 
+                        fraction = frac, location = 'top', anchor = (1,1)) #, cax = cbaxes)
     else:
         lgap = 0.02 # 0.005
-        frac = 0.2
+        frac = 0.08
         r = df1.shape[1]/df1.shape[0]
-        cbaxes = fig.add_axes([0.95, 0.6, 0.1*(1-df1.shape[1]/30), 0.1]) 
-
-    cmap = p.cmap
-    cbar = plt.colorbar(mpl.cm.ScalarMappable(norm=norm, cmap=cmap),ax=ax, 
-                        fraction = frac, cax = cbaxes)
+        # cbaxes = fig.add_axes([1, 1, 0.1*(1-df1.shape[1]/30), 0.1]) 
+        cbar = plt.colorbar(mpl.cm.ScalarMappable(norm=norm, cmap=cmap),ax=ax, 
+                        fraction = frac, location = 'right', anchor = (0,0)) #, cax = cbaxes)
+        
     # if df2 is not None:
     cbar.set_label(cbar_title, fontsize = label_fs)
     for t in cbar.ax.get_yticklabels():
         t.set_fontsize(tick_fs)
 
     #'''
     if swap_ax:
         nn = 4 # list(np.arange(1,mx_pv,2)) 
         kw = dict(prop="sizes", num=nn, fmt="{x:1.0f}", func=lambda s: s/ssf, color = 'grey')
         legend = ax.legend(*p.legend_elements(**kw), title = '-log(P)',
                        fontsize = legend_fs, title_fontsize=legend_fs,
-                       loc = 'upper left', bbox_to_anchor = (1+lgap, 0.55) )
+                       loc = 'upper left', bbox_to_anchor = (1+lgap, 1) )
     else:
         nn = int(mx_pv)
         kw = dict(prop="sizes", num=nn, fmt="{x:1.0f}", func=lambda s: s/ssf, color = 'grey')
         legend = ax.legend(*p.legend_elements(**kw), title = '-log(P)',
                        fontsize = legend_fs, title_fontsize=legend_fs,
-                       loc = 'upper left', bbox_to_anchor = (1+lgap, 0.5) )
+                       loc = 'upper left', bbox_to_anchor = (1+lgap, 1) )
     #'''
     plt.show()
     return
 
 
 def get_gsea_summary( gsea_res, max_log_p = 10 ):
```

### Comparing `scoda-tk-0.3.4/src/scoda_tk.egg-info/PKG-INFO` & `scoda-tk-0.3.5/src/scoda_tk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.3.4
+Version: 0.3.5
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.3.4/src/scoda_tk.egg-info/SOURCES.txt` & `scoda-tk-0.3.5/src/scoda_tk.egg-info/SOURCES.txt`

 * *Files identical despite different names*


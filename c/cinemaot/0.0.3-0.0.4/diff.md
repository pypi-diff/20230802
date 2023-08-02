# Comparing `tmp/cinemaot-0.0.3.tar.gz` & `tmp/cinemaot-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cinemaot-0.0.3.tar", last modified: Thu Mar 30 05:40:59 2023, max compression
+gzip compressed data, was "cinemaot-0.0.4.tar", last modified: Wed Aug  2 20:59:41 2023, max compression
```

## Comparing `cinemaot-0.0.3.tar` & `cinemaot-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 guardian   (501) staff       (20)        0 2023-03-30 05:40:59.089319 cinemaot-0.0.3/
--rw-rw-r--   0 guardian   (501) staff       (20)    34522 2023-03-30 05:13:29.000000 cinemaot-0.0.3/LICENSE
--rw-r--r--   0 guardian   (501) staff       (20)     2306 2023-03-30 05:40:59.089368 cinemaot-0.0.3/PKG-INFO
-drwxr-xr-x   0 guardian   (501) staff       (20)        0 2023-03-30 05:40:59.088665 cinemaot-0.0.3/cinemaot/
--rw-rw-r--   0 guardian   (501) staff       (20)      182 2023-03-30 05:13:29.000000 cinemaot-0.0.3/cinemaot/__init__.py
--rw-rw-r--   0 guardian   (501) staff       (20)    11400 2023-03-30 05:13:29.000000 cinemaot-0.0.3/cinemaot/benchmark.py
--rw-rw-r--   0 guardian   (501) staff       (20)    24857 2023-03-30 05:13:29.000000 cinemaot-0.0.3/cinemaot/cinemaot.py
--rw-rw-r--   0 guardian   (501) staff       (20)     5315 2023-03-30 05:13:29.000000 cinemaot-0.0.3/cinemaot/sinkhorn_knopp.py
--rw-rw-r--   0 guardian   (501) staff       (20)    13937 2023-03-30 05:13:29.000000 cinemaot-0.0.3/cinemaot/utils.py
-drwxr-xr-x   0 guardian   (501) staff       (20)        0 2023-03-30 05:40:59.089218 cinemaot-0.0.3/cinemaot.egg-info/
--rw-r--r--   0 guardian   (501) staff       (20)     2306 2023-03-30 05:40:59.000000 cinemaot-0.0.3/cinemaot.egg-info/PKG-INFO
--rw-r--r--   0 guardian   (501) staff       (20)      309 2023-03-30 05:40:59.000000 cinemaot-0.0.3/cinemaot.egg-info/SOURCES.txt
--rw-r--r--   0 guardian   (501) staff       (20)        1 2023-03-30 05:40:59.000000 cinemaot-0.0.3/cinemaot.egg-info/dependency_links.txt
--rw-r--r--   0 guardian   (501) staff       (20)       54 2023-03-30 05:40:59.000000 cinemaot-0.0.3/cinemaot.egg-info/requires.txt
--rw-r--r--   0 guardian   (501) staff       (20)        9 2023-03-30 05:40:59.000000 cinemaot-0.0.3/cinemaot.egg-info/top_level.txt
--rw-rw-r--   0 guardian   (501) staff       (20)       84 2023-03-30 05:13:29.000000 cinemaot-0.0.3/pyproject.toml
--rw-rw-r--   0 guardian   (501) staff       (20)      730 2023-03-30 05:40:59.089616 cinemaot-0.0.3/setup.cfg
--rw-r--r--   0 guardian   (501) staff       (20)       67 2023-03-30 05:32:54.000000 cinemaot-0.0.3/setup.py
+drwxr-xr-x   0 guardian   (501) staff       (20)        0 2023-08-02 20:59:41.011102 cinemaot-0.0.4/
+-rw-rw-r--   0 guardian   (501) staff       (20)    34522 2023-03-30 05:13:29.000000 cinemaot-0.0.4/LICENSE
+-rw-r--r--   0 guardian   (501) staff       (20)     2306 2023-08-02 20:59:41.011162 cinemaot-0.0.4/PKG-INFO
+drwxr-xr-x   0 guardian   (501) staff       (20)        0 2023-08-02 20:59:41.010398 cinemaot-0.0.4/cinemaot/
+-rw-rw-r--   0 guardian   (501) staff       (20)      182 2023-08-02 20:56:09.000000 cinemaot-0.0.4/cinemaot/__init__.py
+-rw-rw-r--   0 guardian   (501) staff       (20)    11400 2023-03-30 05:13:29.000000 cinemaot-0.0.4/cinemaot/benchmark.py
+-rw-rw-r--   0 guardian   (501) staff       (20)    24914 2023-08-02 20:45:12.000000 cinemaot-0.0.4/cinemaot/cinemaot.py
+-rw-rw-r--   0 guardian   (501) staff       (20)     5315 2023-03-30 05:13:29.000000 cinemaot-0.0.4/cinemaot/sinkhorn_knopp.py
+-rw-rw-r--   0 guardian   (501) staff       (20)    13937 2023-03-30 05:13:29.000000 cinemaot-0.0.4/cinemaot/utils.py
+drwxr-xr-x   0 guardian   (501) staff       (20)        0 2023-08-02 20:59:41.011013 cinemaot-0.0.4/cinemaot.egg-info/
+-rw-r--r--   0 guardian   (501) staff       (20)     2306 2023-08-02 20:59:40.000000 cinemaot-0.0.4/cinemaot.egg-info/PKG-INFO
+-rw-r--r--   0 guardian   (501) staff       (20)      309 2023-08-02 20:59:40.000000 cinemaot-0.0.4/cinemaot.egg-info/SOURCES.txt
+-rw-r--r--   0 guardian   (501) staff       (20)        1 2023-08-02 20:59:40.000000 cinemaot-0.0.4/cinemaot.egg-info/dependency_links.txt
+-rw-r--r--   0 guardian   (501) staff       (20)       54 2023-08-02 20:59:40.000000 cinemaot-0.0.4/cinemaot.egg-info/requires.txt
+-rw-r--r--   0 guardian   (501) staff       (20)        9 2023-08-02 20:59:40.000000 cinemaot-0.0.4/cinemaot.egg-info/top_level.txt
+-rw-rw-r--   0 guardian   (501) staff       (20)       84 2023-03-30 05:13:29.000000 cinemaot-0.0.4/pyproject.toml
+-rw-rw-r--   0 guardian   (501) staff       (20)      730 2023-08-02 20:59:41.011412 cinemaot-0.0.4/setup.cfg
+-rw-r--r--   0 guardian   (501) staff       (20)       67 2023-03-30 05:32:54.000000 cinemaot-0.0.4/setup.py
```

### Comparing `cinemaot-0.0.3/LICENSE` & `cinemaot-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cinemaot-0.0.3/PKG-INFO` & `cinemaot-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cinemaot
-Version: 0.0.3
+Version: 0.0.4
 Summary: Causal INdependent Effect Module Attribution + Optimal Transport
 Home-page: https://github.com/vandijklab/CINEMA-OT
 Author: Mingze Dong
 Author-email: mingze.dong@yale.edu
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/vandijklab/CINEMA-OT/issues
 Platform: UNKNOWN
```

### Comparing `cinemaot-0.0.3/cinemaot/benchmark.py` & `cinemaot-0.0.4/cinemaot/benchmark.py`

 * *Files identical despite different names*

### Comparing `cinemaot-0.0.3/cinemaot/cinemaot.py` & `cinemaot-0.0.4/cinemaot/cinemaot.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         vm = (1e-3 + data + c * data * data)/(1+c)
         P = sk.fit(vm)
         wm = np.dot(np.dot(np.sqrt(sk._D1),vm),np.sqrt(sk._D2))
         u,s,vt = np.linalg.svd(wm)
         dim = np.min(sum(s > (np.sqrt(data.shape[0])+np.sqrt(data.shape[1]))),adata.obsm['X_pca'].shape[1])
 
 
-    transformer = FastICA(n_components=dim, random_state=0)
+    transformer = FastICA(n_components=dim, random_state=0,whiten="arbitrary-variance")
     X_transformed = transformer.fit_transform(adata.obsm['X_pca'][:,:dim])
     #importr("XICOR")
     #xicor = ro.r["xicor"]
     groupvec = (adata.obs[obs_label]==ref_label *1).values #control
     xi = np.zeros(dim)
     #pval = np.zeros(dim)
     j = 0
@@ -236,15 +236,15 @@
                 idx = idx.append(adata_[(adata_.obs['leiden']==i) & (adata_.obs[obs_label]==ref_label)].obs.index)
                 j = j + 1
             else:
                 idx_tmp = sc.pp.subsample(adata_[(adata_.obs['leiden']==i) & (adata_.obs[obs_label]==expr_label)],n_obs = adata_[(adata_.obs['leiden']==i) & (adata_.obs[obs_label]==ref_label)].shape[0],copy=True).obs.index
                 idx_tmp = idx_tmp.append(adata_[(adata_.obs['leiden']==i) & (adata_.obs[obs_label]==ref_label)].obs.index)
                 idx = idx.append(idx_tmp)
 
-    transformer = FastICA(n_components=dim, random_state=0)
+    transformer = FastICA(n_components=dim, random_state=0, whiten="arbitrary-variance")
     X_transformed = transformer.fit_transform(adata_[idx].obsm['X_pca'][:,:dim])
     #importr("XICOR")
     #xicor = ro.r["xicor"]
     groupvec = (adata_[idx].obs[obs_label]==ref_label *1).values #control
     xi = np.zeros(dim)
     #pval = np.zeros(dim)
     j = 0
```

### Comparing `cinemaot-0.0.3/cinemaot/sinkhorn_knopp.py` & `cinemaot-0.0.4/cinemaot/sinkhorn_knopp.py`

 * *Files identical despite different names*

### Comparing `cinemaot-0.0.3/cinemaot/utils.py` & `cinemaot-0.0.4/cinemaot/utils.py`

 * *Files identical despite different names*

### Comparing `cinemaot-0.0.3/cinemaot.egg-info/PKG-INFO` & `cinemaot-0.0.4/cinemaot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cinemaot
-Version: 0.0.3
+Version: 0.0.4
 Summary: Causal INdependent Effect Module Attribution + Optimal Transport
 Home-page: https://github.com/vandijklab/CINEMA-OT
 Author: Mingze Dong
 Author-email: mingze.dong@yale.edu
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/vandijklab/CINEMA-OT/issues
 Platform: UNKNOWN
```

### Comparing `cinemaot-0.0.3/setup.cfg` & `cinemaot-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cinemaot
-version = 0.0.3
+version = 0.0.4
 author = Mingze Dong
 author_email = mingze.dong@yale.edu
 description = Causal INdependent Effect Module Attribution + Optimal Transport
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/vandijklab/CINEMA-OT
 project_urls =
```


# Comparing `tmp/emobject-0.7.0b4.tar.gz` & `tmp/emobject-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emobject-0.7.0b4.tar", last modified: Fri Jul 28 20:23:08 2023, max compression
+gzip compressed data, was "emobject-0.7.1.tar", last modified: Wed Aug  2 15:57:54 2023, max compression
```

## Comparing `emobject-0.7.0b4.tar` & `emobject-0.7.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 20:23:08.863490 emobject-0.7.0b4/
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-28 20:22:58.000000 emobject-0.7.0b4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4225 2023-07-28 20:23:08.863490 emobject-0.7.0b4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3826 2023-07-28 20:22:58.000000 emobject-0.7.0b4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 20:23:08.861490 emobject-0.7.0b4/emobject/
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    39419 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/core.py
--rw-rw-rw-   0 root         (0) root         (0)    15643 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/database.py
--rw-rw-rw-   0 root         (0) root         (0)    32512 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/emexperiment.py
--rw-rw-rw-   0 root         (0) root         (0)    14806 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/emimage.py
--rw-rw-rw-   0 root         (0) root         (0)     9750 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/emlayer.py
--rw-rw-rw-   0 root         (0) root         (0)    49374 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/emobject.py
--rw-rw-rw-   0 root         (0) root         (0)     6759 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/empublicaccess.py
--rw-rw-rw-   0 root         (0) root         (0)     9493 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/emroitools.py
--rw-rw-rw-   0 root         (0) root         (0)       96 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 20:23:08.862490 emobject-0.7.0b4/emobject/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3543 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/utils/graph.py
--rw-rw-rw-   0 root         (0) root         (0)     2447 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/utils/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    24229 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/utils/io.py
--rw-rw-rw-   0 root         (0) root         (0)    11201 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/utils/visualization.py
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 20:23:08.861490 emobject-0.7.0b4/emobject.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4225 2023-07-28 20:23:08.000000 emobject-0.7.0b4/emobject.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      559 2023-07-28 20:23:08.000000 emobject-0.7.0b4/emobject.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 20:23:08.000000 emobject-0.7.0b4/emobject.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      229 2023-07-28 20:23:08.000000 emobject-0.7.0b4/emobject.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-28 20:23:08.000000 emobject-0.7.0b4/emobject.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-28 20:23:08.863490 emobject-0.7.0b4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1263 2023-07-28 20:22:58.000000 emobject-0.7.0b4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:57:54.171496 emobject-0.7.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-08-02 15:57:44.000000 emobject-0.7.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4312 2023-08-02 15:57:54.171496 emobject-0.7.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3915 2023-08-02 15:57:44.000000 emobject-0.7.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:57:54.169496 emobject-0.7.1/emobject/
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    39544 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/core.py
+-rw-rw-rw-   0 root         (0) root         (0)    15643 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/database.py
+-rw-rw-rw-   0 root         (0) root         (0)    32512 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/emexperiment.py
+-rw-rw-rw-   0 root         (0) root         (0)    14806 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/emimage.py
+-rw-rw-rw-   0 root         (0) root         (0)     9750 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/emlayer.py
+-rw-rw-rw-   0 root         (0) root         (0)    49374 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/emobject.py
+-rw-rw-rw-   0 root         (0) root         (0)     6759 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/empublicaccess.py
+-rw-rw-rw-   0 root         (0) root         (0)     9493 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/emroitools.py
+-rw-rw-rw-   0 root         (0) root         (0)       96 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:57:54.171496 emobject-0.7.1/emobject/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3543 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/utils/graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     2447 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/utils/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    24229 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/utils/io.py
+-rw-rw-rw-   0 root         (0) root         (0)    11201 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/utils/visualization.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:57:54.170496 emobject-0.7.1/emobject.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4312 2023-08-02 15:57:54.000000 emobject-0.7.1/emobject.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      559 2023-08-02 15:57:54.000000 emobject-0.7.1/emobject.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 15:57:54.000000 emobject-0.7.1/emobject.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      229 2023-08-02 15:57:54.000000 emobject-0.7.1/emobject.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-08-02 15:57:54.000000 emobject-0.7.1/emobject.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-08-02 15:57:54.172496 emobject-0.7.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1263 2023-08-02 15:57:44.000000 emobject-0.7.1/setup.py
```

### Comparing `emobject-0.7.0b4/LICENSE` & `emobject-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b4/PKG-INFO` & `emobject-0.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emobject
-Version: 0.7.0b4
+Version: 0.7.1
 Summary: data abstraction and libraries for spatial omics
 Home-page: https://gitlab.com/enable-medicine/rnd-subgroup/emobject/
 Author: Ethan A. G. Baker
 Author-email: ethan.baker@enablemedicine.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7, <4
@@ -71,17 +71,25 @@
 If you use `pipenv` as a package manager, you can install via:
 
 ```
 pipenv install '-e .' --dev
 ```
 from within the `emobject` repository. 
 
-You can also install directly via PyPI
+You can also install directly via PyPI:
 
-(Coming soon)
+```
+pip install emobject
+```
+
+or, if you use `pipenv` (recommended):
+
+```
+pipenv install emobject
+```
 
 ## Using emObject
 See the `./notebooks` directory for tutorials to get started with emObject. The complete emObject documentation is available at [docs.enablemedicine.com](docs.enablemedicine.com).
 
 ## Using emMorphology extension
 See the morphology extension package [here](https://gitlab.com/enable-medicine-public/emobject-morphology-extension).
```

### Comparing `emobject-0.7.0b4/README.md` & `emobject-0.7.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -57,17 +57,25 @@
 If you use `pipenv` as a package manager, you can install via:
 
 ```
 pipenv install '-e .' --dev
 ```
 from within the `emobject` repository. 
 
-You can also install directly via PyPI
+You can also install directly via PyPI:
 
-(Coming soon)
+```
+pip install emobject
+```
+
+or, if you use `pipenv` (recommended):
+
+```
+pipenv install emobject
+```
 
 ## Using emObject
 See the `./notebooks` directory for tutorials to get started with emObject. The complete emObject documentation is available at [docs.enablemedicine.com](docs.enablemedicine.com).
 
 ## Using emMorphology extension
 See the morphology extension package [here](https://gitlab.com/enable-medicine-public/emobject-morphology-extension).
```

### Comparing `emobject-0.7.0b4/emobject/core.py` & `emobject-0.7.1/emobject/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,15 @@
                  segmentation_version: Optional[int] = None,
                  biomarker_version: Optional[int] = None,
                  biomarkers: Optional[Union[list, np.ndarray, str]] = None,
                  annotations: Optional[Union[list, np.ndarray, str]] = None,
                  include_img: Optional[bool] = False,
                  include_masks: Optional[bool] = False,
                  include_seg_mask: Optional[bool] = False,
+                 include_metadata: Optional[bool] = True,
                  seg_mask_type: Optional[str] = 'nucleus',
                  img_format: Optional[str] = 'zarr',
                  img_res: Optional[int] = 0,
                  img_to_disk: Optional[bool] = False,
                  img_path: Optional[str] = None,
                  mask_names: Optional[Union[list, np.ndarray, str]] = None,
                  name: Optional[str] = None,
@@ -220,15 +221,19 @@
         config.masks = build_emmask_from_enable_db(acquisition_id=config.acquisition_id,
                                                    study_id=config.study_id,
                                                    include_masks=config.include_masks,
                                                    include_seg_masks=config.include_seg_mask,
                                                    seg_mask_type=config.seg_mask_type,
                                                    segmentation_version=config.segmentation_version,
                                                    biomarker_version=config.biomarker_version)
-    meta = run_metadata_queries(config.acquisition_id)
+
+    if config.include_metadata:
+        meta = run_metadata_queries(config.acquisition_id)
+    else:
+        meta = None
 
     return EMObject(
         data=bm_df,
         obs=anno_df,
         var=None,
         pos=coord_df,
         mask=config.masks,
```

### Comparing `emobject-0.7.0b4/emobject/database.py` & `emobject-0.7.1/emobject/database.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b4/emobject/emexperiment.py` & `emobject-0.7.1/emobject/emexperiment.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b4/emobject/emimage.py` & `emobject-0.7.1/emobject/emimage.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b4/emobject/emlayer.py` & `emobject-0.7.1/emobject/emlayer.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b4/emobject/emobject.py` & `emobject-0.7.1/emobject/emobject.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b4/emobject/empublicaccess.py` & `emobject-0.7.1/emobject/empublicaccess.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b4/emobject/emroitools.py` & `emobject-0.7.1/emobject/emroitools.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b4/emobject/utils/graph.py` & `emobject-0.7.1/emobject/utils/graph.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b4/emobject/utils/helpers.py` & `emobject-0.7.1/emobject/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b4/emobject/utils/io.py` & `emobject-0.7.1/emobject/utils/io.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b4/emobject/utils/visualization.py` & `emobject-0.7.1/emobject/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b4/emobject.egg-info/PKG-INFO` & `emobject-0.7.1/emobject.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emobject
-Version: 0.7.0b4
+Version: 0.7.1
 Summary: data abstraction and libraries for spatial omics
 Home-page: https://gitlab.com/enable-medicine/rnd-subgroup/emobject/
 Author: Ethan A. G. Baker
 Author-email: ethan.baker@enablemedicine.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7, <4
@@ -71,17 +71,25 @@
 If you use `pipenv` as a package manager, you can install via:
 
 ```
 pipenv install '-e .' --dev
 ```
 from within the `emobject` repository. 
 
-You can also install directly via PyPI
+You can also install directly via PyPI:
 
-(Coming soon)
+```
+pip install emobject
+```
+
+or, if you use `pipenv` (recommended):
+
+```
+pipenv install emobject
+```
 
 ## Using emObject
 See the `./notebooks` directory for tutorials to get started with emObject. The complete emObject documentation is available at [docs.enablemedicine.com](docs.enablemedicine.com).
 
 ## Using emMorphology extension
 See the morphology extension package [here](https://gitlab.com/enable-medicine-public/emobject-morphology-extension).
```

### Comparing `emobject-0.7.0b4/emobject.egg-info/SOURCES.txt` & `emobject-0.7.1/emobject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b4/setup.py` & `emobject-0.7.1/setup.py`

 * *Files identical despite different names*


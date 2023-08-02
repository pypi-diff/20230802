# Comparing `tmp/emobject-0.7.1.tar.gz` & `tmp/emobject-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emobject-0.7.1.tar", last modified: Wed Aug  2 15:57:54 2023, max compression
+gzip compressed data, was "emobject-0.7.2.tar", last modified: Wed Aug  2 21:30:26 2023, max compression
```

## Comparing `emobject-0.7.1.tar` & `emobject-0.7.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:57:54.171496 emobject-0.7.1/
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-08-02 15:57:44.000000 emobject-0.7.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4312 2023-08-02 15:57:54.171496 emobject-0.7.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3915 2023-08-02 15:57:44.000000 emobject-0.7.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:57:54.169496 emobject-0.7.1/emobject/
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    39544 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/core.py
--rw-rw-rw-   0 root         (0) root         (0)    15643 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/database.py
--rw-rw-rw-   0 root         (0) root         (0)    32512 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/emexperiment.py
--rw-rw-rw-   0 root         (0) root         (0)    14806 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/emimage.py
--rw-rw-rw-   0 root         (0) root         (0)     9750 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/emlayer.py
--rw-rw-rw-   0 root         (0) root         (0)    49374 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/emobject.py
--rw-rw-rw-   0 root         (0) root         (0)     6759 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/empublicaccess.py
--rw-rw-rw-   0 root         (0) root         (0)     9493 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/emroitools.py
--rw-rw-rw-   0 root         (0) root         (0)       96 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:57:54.171496 emobject-0.7.1/emobject/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3543 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/utils/graph.py
--rw-rw-rw-   0 root         (0) root         (0)     2447 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/utils/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    24229 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/utils/io.py
--rw-rw-rw-   0 root         (0) root         (0)    11201 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/utils/visualization.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-08-02 15:57:44.000000 emobject-0.7.1/emobject/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:57:54.170496 emobject-0.7.1/emobject.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4312 2023-08-02 15:57:54.000000 emobject-0.7.1/emobject.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      559 2023-08-02 15:57:54.000000 emobject-0.7.1/emobject.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 15:57:54.000000 emobject-0.7.1/emobject.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      229 2023-08-02 15:57:54.000000 emobject-0.7.1/emobject.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-08-02 15:57:54.000000 emobject-0.7.1/emobject.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-08-02 15:57:54.172496 emobject-0.7.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1263 2023-08-02 15:57:44.000000 emobject-0.7.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 21:30:26.492400 emobject-0.7.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-08-02 21:30:16.000000 emobject-0.7.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4312 2023-08-02 21:30:26.492400 emobject-0.7.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3915 2023-08-02 21:30:16.000000 emobject-0.7.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 21:30:26.489400 emobject-0.7.2/emobject/
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    39593 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/core.py
+-rw-rw-rw-   0 root         (0) root         (0)    15643 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/database.py
+-rw-rw-rw-   0 root         (0) root         (0)    32512 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/emexperiment.py
+-rw-rw-rw-   0 root         (0) root         (0)    14806 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/emimage.py
+-rw-rw-rw-   0 root         (0) root         (0)     9750 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/emlayer.py
+-rw-rw-rw-   0 root         (0) root         (0)    49374 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/emobject.py
+-rw-rw-rw-   0 root         (0) root         (0)     6759 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/empublicaccess.py
+-rw-rw-rw-   0 root         (0) root         (0)     9493 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/emroitools.py
+-rw-rw-rw-   0 root         (0) root         (0)       96 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 21:30:26.491400 emobject-0.7.2/emobject/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3543 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/utils/graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     2447 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/utils/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    24229 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/utils/io.py
+-rw-rw-rw-   0 root         (0) root         (0)    11201 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/utils/visualization.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 21:30:26.490400 emobject-0.7.2/emobject.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4312 2023-08-02 21:30:26.000000 emobject-0.7.2/emobject.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      559 2023-08-02 21:30:26.000000 emobject-0.7.2/emobject.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 21:30:26.000000 emobject-0.7.2/emobject.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      229 2023-08-02 21:30:26.000000 emobject-0.7.2/emobject.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-08-02 21:30:26.000000 emobject-0.7.2/emobject.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-08-02 21:30:26.492400 emobject-0.7.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1263 2023-08-02 21:30:16.000000 emobject-0.7.2/setup.py
```

### Comparing `emobject-0.7.1/LICENSE` & `emobject-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `emobject-0.7.1/PKG-INFO` & `emobject-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emobject
-Version: 0.7.1
+Version: 0.7.2
 Summary: data abstraction and libraries for spatial omics
 Home-page: https://gitlab.com/enable-medicine/rnd-subgroup/emobject/
 Author: Ethan A. G. Baker
 Author-email: ethan.baker@enablemedicine.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7, <4
```

### Comparing `emobject-0.7.1/README.md` & `emobject-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `emobject-0.7.1/emobject/core.py` & `emobject-0.7.2/emobject/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
         self.segmentation_version = segmentation_version
         self.biomarker_version = biomarker_version
         self.biomarkers = biomarkers
         self.annotations = annotations
         self.include_img = include_img
         self.include_masks = include_masks
         self.include_seg_mask = include_seg_mask
+        self.include_metadata = include_metadata
         self.seg_mask_type = seg_mask_type
         self.img_format = img_format
         self.img_res = img_res
         self.img_to_disk = img_to_disk
         self.img_path = img_path
         self.mask_names = mask_names
         self.name = name
```

### Comparing `emobject-0.7.1/emobject/database.py` & `emobject-0.7.2/emobject/database.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.1/emobject/emexperiment.py` & `emobject-0.7.2/emobject/emexperiment.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.1/emobject/emimage.py` & `emobject-0.7.2/emobject/emimage.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.1/emobject/emlayer.py` & `emobject-0.7.2/emobject/emlayer.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.1/emobject/emobject.py` & `emobject-0.7.2/emobject/emobject.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.1/emobject/empublicaccess.py` & `emobject-0.7.2/emobject/empublicaccess.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.1/emobject/emroitools.py` & `emobject-0.7.2/emobject/emroitools.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.1/emobject/utils/graph.py` & `emobject-0.7.2/emobject/utils/graph.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.1/emobject/utils/helpers.py` & `emobject-0.7.2/emobject/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.1/emobject/utils/io.py` & `emobject-0.7.2/emobject/utils/io.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.1/emobject/utils/visualization.py` & `emobject-0.7.2/emobject/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.1/emobject.egg-info/PKG-INFO` & `emobject-0.7.2/emobject.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emobject
-Version: 0.7.1
+Version: 0.7.2
 Summary: data abstraction and libraries for spatial omics
 Home-page: https://gitlab.com/enable-medicine/rnd-subgroup/emobject/
 Author: Ethan A. G. Baker
 Author-email: ethan.baker@enablemedicine.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7, <4
```

### Comparing `emobject-0.7.1/emobject.egg-info/SOURCES.txt` & `emobject-0.7.2/emobject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emobject-0.7.1/setup.py` & `emobject-0.7.2/setup.py`

 * *Files identical despite different names*


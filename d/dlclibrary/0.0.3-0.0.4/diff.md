# Comparing `tmp/dlclibrary-0.0.3.tar.gz` & `tmp/dlclibrary-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlclibrary-0.0.3.tar", last modified: Wed May  3 12:04:27 2023, max compression
+gzip compressed data, was "dlclibrary-0.0.4.tar", last modified: Wed Aug  2 16:37:09 2023, max compression
```

## Comparing `dlclibrary-0.0.3.tar` & `dlclibrary-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-03 12:04:27.285834 dlclibrary-0.0.3/
--rw-r--r--   0 alex       (501) staff       (20)     7652 2022-11-27 10:48:36.000000 dlclibrary-0.0.3/LICENSE
--rw-r--r--   0 alex       (501) staff       (20)      441 2022-11-27 10:54:12.000000 dlclibrary-0.0.3/NOTICE.yml
--rw-r--r--   0 alex       (501) staff       (20)     1212 2023-05-03 12:04:27.285666 dlclibrary-0.0.3/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      686 2023-05-02 16:26:26.000000 dlclibrary-0.0.3/README.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-03 12:04:27.283018 dlclibrary-0.0.3/dlclibrary/
--rw-r--r--   0 alex       (501) staff       (20)      449 2023-05-02 16:26:26.000000 dlclibrary-0.0.3/dlclibrary/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-03 12:04:27.284682 dlclibrary-0.0.3/dlclibrary/dlcmodelzoo/
--rw-r--r--   0 alex       (501) staff       (20)      274 2022-12-20 20:16:30.000000 dlclibrary-0.0.3/dlclibrary/dlcmodelzoo/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     2984 2023-05-03 12:03:32.000000 dlclibrary-0.0.3/dlclibrary/dlcmodelzoo/modelzoo_download.py
--rw-r--r--   0 alex       (501) staff       (20)     1913 2023-05-02 16:27:02.000000 dlclibrary-0.0.3/dlclibrary/dlcmodelzoo/modelzoo_urls.yaml
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-03 12:04:27.285195 dlclibrary-0.0.3/dlclibrary/dlcmodelzoo/superanimal_configs/
--rw-r--r--   0 alex       (501) staff       (20)     2329 2023-05-02 16:26:26.000000 dlclibrary-0.0.3/dlclibrary/dlcmodelzoo/superanimal_configs/superquadruped.yaml
--rw-r--r--   0 alex       (501) staff       (20)     1962 2023-05-02 16:26:26.000000 dlclibrary-0.0.3/dlclibrary/dlcmodelzoo/superanimal_configs/supertopview.yaml
--rw-r--r--   0 alex       (501) staff       (20)      108 2023-05-02 16:26:26.000000 dlclibrary-0.0.3/dlclibrary/dlcmodelzoo/superanimal_models.json
--rw-r--r--   0 alex       (501) staff       (20)      319 2023-05-03 12:03:32.000000 dlclibrary-0.0.3/dlclibrary/version.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-03 12:04:27.283696 dlclibrary-0.0.3/dlclibrary.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)     1212 2023-05-03 12:04:27.000000 dlclibrary-0.0.3/dlclibrary.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      571 2023-05-03 12:04:27.000000 dlclibrary-0.0.3/dlclibrary.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2023-05-03 12:04:27.000000 dlclibrary-0.0.3/dlclibrary.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)       36 2023-05-03 12:04:27.000000 dlclibrary-0.0.3/dlclibrary.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)       11 2023-05-03 12:04:27.000000 dlclibrary-0.0.3/dlclibrary.egg-info/top_level.txt
--rw-r--r--   0 alex       (501) staff       (20)       38 2023-05-03 12:04:27.285877 dlclibrary-0.0.3/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)     1492 2023-05-03 12:03:32.000000 dlclibrary-0.0.3/setup.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-03 12:04:27.285345 dlclibrary-0.0.3/tests/
--rw-r--r--   0 alex       (501) staff       (20)     1330 2023-05-02 16:26:26.000000 dlclibrary-0.0.3/tests/test_modeldownload.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-08-02 16:37:09.319081 dlclibrary-0.0.4/
+-rw-r--r--   0 alex       (501) staff       (20)     7652 2022-11-27 10:48:36.000000 dlclibrary-0.0.4/LICENSE
+-rw-r--r--   0 alex       (501) staff       (20)      441 2022-11-27 10:54:12.000000 dlclibrary-0.0.4/NOTICE.yml
+-rw-r--r--   0 alex       (501) staff       (20)     2229 2023-08-02 16:37:09.318873 dlclibrary-0.0.4/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     1703 2023-08-02 16:29:25.000000 dlclibrary-0.0.4/README.md
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-08-02 16:37:09.308162 dlclibrary-0.0.4/dlclibrary/
+-rw-r--r--   0 alex       (501) staff       (20)      449 2023-05-02 16:26:26.000000 dlclibrary-0.0.4/dlclibrary/__init__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-08-02 16:37:09.317800 dlclibrary-0.0.4/dlclibrary/dlcmodelzoo/
+-rw-r--r--   0 alex       (501) staff       (20)      274 2022-12-20 20:16:30.000000 dlclibrary-0.0.4/dlclibrary/dlcmodelzoo/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     2984 2023-05-03 12:03:32.000000 dlclibrary-0.0.4/dlclibrary/dlcmodelzoo/modelzoo_download.py
+-rw-r--r--   0 alex       (501) staff       (20)     1913 2023-08-02 15:54:19.000000 dlclibrary-0.0.4/dlclibrary/dlcmodelzoo/modelzoo_urls.yaml
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-08-02 16:37:09.318374 dlclibrary-0.0.4/dlclibrary/dlcmodelzoo/superanimal_configs/
+-rw-r--r--   0 alex       (501) staff       (20)     2329 2023-05-02 16:26:26.000000 dlclibrary-0.0.4/dlclibrary/dlcmodelzoo/superanimal_configs/superquadruped.yaml
+-rw-r--r--   0 alex       (501) staff       (20)     1962 2023-05-02 16:26:26.000000 dlclibrary-0.0.4/dlclibrary/dlcmodelzoo/superanimal_configs/supertopview.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      108 2023-05-02 16:26:26.000000 dlclibrary-0.0.4/dlclibrary/dlcmodelzoo/superanimal_models.json
+-rw-r--r--   0 alex       (501) staff       (20)      319 2023-08-02 15:56:28.000000 dlclibrary-0.0.4/dlclibrary/version.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-08-02 16:37:09.311634 dlclibrary-0.0.4/dlclibrary.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)     2229 2023-08-02 16:37:09.000000 dlclibrary-0.0.4/dlclibrary.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      571 2023-08-02 16:37:09.000000 dlclibrary-0.0.4/dlclibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2023-08-02 16:37:09.000000 dlclibrary-0.0.4/dlclibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)       36 2023-08-02 16:37:09.000000 dlclibrary-0.0.4/dlclibrary.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)       11 2023-08-02 16:37:09.000000 dlclibrary-0.0.4/dlclibrary.egg-info/top_level.txt
+-rw-r--r--   0 alex       (501) staff       (20)       38 2023-08-02 16:37:09.319188 dlclibrary-0.0.4/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)     1492 2023-08-02 15:56:28.000000 dlclibrary-0.0.4/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-08-02 16:37:09.318660 dlclibrary-0.0.4/tests/
+-rw-r--r--   0 alex       (501) staff       (20)     1397 2023-08-02 16:30:04.000000 dlclibrary-0.0.4/tests/test_modeldownload.py
```

### Comparing `dlclibrary-0.0.3/LICENSE` & `dlclibrary-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dlclibrary-0.0.3/dlclibrary/dlcmodelzoo/modelzoo_download.py` & `dlclibrary-0.0.4/dlclibrary/dlcmodelzoo/modelzoo_download.py`

 * *Files identical despite different names*

### Comparing `dlclibrary-0.0.3/dlclibrary/dlcmodelzoo/modelzoo_urls.yaml` & `dlclibrary-0.0.4/dlclibrary/dlcmodelzoo/modelzoo_urls.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -28,11 +28,11 @@
 horse_sideview: mwmathis/DeepLabCutModelZoo-horse_sideview/DLC_Horses_resnet_50_iteration-1_shuffle-1.tar.gz
 horse_sideview_commit: fd0329b2ffc8fe7a5e6eb3d4850ebca75987e92c
 
 full_macaque: mwmathis/DeepLabCutModelZoo-macaque_full/DLC_macaque_full_resnet50.tar.gz
 full_macaque_commit: 4c7ebf2628d5b7eb0483356595256fb01b7e1a9e
 
 superanimal_topviewmouse: mwmathis/DeepLabCutModelZoo-SuperAnimal-TopViewMouse/DLC_ma_supertopview5k_resnet_50_iteration-0_shuffle-1.tar.gz
-superanimal_topviewmouse_commit: a7d7df40c3307a3c7a0ceeb2593d46a783235b28
+superanimal_topviewmouse_commit: 1781f384b56ddb9b58c0d4acae98993b9a17e901
 
 superanimal_quadruped: mwmathis/DeepLabCutModelZoo-SuperAnimal-Quadruped/DLC_ma_superquadruped_resnet_50_iteration-0_shuffle-1.tar.gz
-superanimal_quadruped_commit: 829b336a52fff0e03f2f87c75b1e2638989122c7
+superanimal_quadruped_commit: 673140e6dd9f7be492d77cab957f31c73a192f67
```

### Comparing `dlclibrary-0.0.3/dlclibrary/dlcmodelzoo/superanimal_configs/superquadruped.yaml` & `dlclibrary-0.0.4/dlclibrary/dlcmodelzoo/superanimal_configs/superquadruped.yaml`

 * *Files identical despite different names*

### Comparing `dlclibrary-0.0.3/dlclibrary/dlcmodelzoo/superanimal_configs/supertopview.yaml` & `dlclibrary-0.0.4/dlclibrary/dlcmodelzoo/superanimal_configs/supertopview.yaml`

 * *Files identical despite different names*

### Comparing `dlclibrary-0.0.3/dlclibrary.egg-info/SOURCES.txt` & `dlclibrary-0.0.4/dlclibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dlclibrary-0.0.3/setup.py` & `dlclibrary-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dlclibrary",
-    version="0.0.3",
+    version="0.0.4",
     author="A. & M. Mathis Labs",
     author_email="alexander@deeplabcut.org",
     description="Lightweight library supporting universal functions for the DeepLabCut ecosystem",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/DeepLabCut/DLClib",
     install_requires=[
```

### Comparing `dlclibrary-0.0.3/tests/test_modeldownload.py` & `dlclibrary-0.0.4/tests/test_modeldownload.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,11 +31,12 @@
 
 def test_parse_superanimal_models():
     dict_ = dlclibrary.parse_available_supermodels()
     assert "superanimal_quadruped" in dict_
     assert "superanimal_topviewmouse" in dict_
 
 
-@pytest.mark.skip
+#@pytest.mark.skip # Not skipping as rarely run!
 @pytest.mark.parametrize("model", MODELOPTIONS)
 def test_download_all_models(tmp_path_factory, model):
+    print("Downloading ...", model)
     test_download_huggingface_model(tmp_path_factory, model)
```


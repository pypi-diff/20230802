# Comparing `tmp/biofilm-0.0.97.tar.gz` & `tmp/biofilm-0.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/biofilm-0.0.97.tar", last modified: Thu Nov 17 13:28:22 2022, max compression
+gzip compressed data, was "dist/biofilm-0.0.98.tar", last modified: Thu Nov 17 16:02:37 2022, max compression
```

## Comparing `biofilm-0.0.97.tar` & `biofilm-0.0.98.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 ikea      (1000) ikea      (1000)        0 2022-11-17 13:28:22.220562 biofilm-0.0.97/
--rw-r--r--   0 ikea      (1000) ikea      (1000)      256 2022-11-17 13:28:22.220562 biofilm-0.0.97/PKG-INFO
--rw-r--r--   0 ikea      (1000) ikea      (1000)     1173 2022-01-27 13:39:21.000000 biofilm-0.0.97/README.md
-drwxr-xr-x   0 ikea      (1000) ikea      (1000)        0 2022-11-17 13:28:22.220562 biofilm-0.0.97/biofilm/
--rw-r--r--   0 ikea      (1000) ikea      (1000)     2017 2021-10-21 15:03:14.000000 biofilm-0.0.97/biofilm/FTBOXPLOT.fish
--rw-r--r--   0 ikea      (1000) ikea      (1000)      179 2022-11-17 13:28:22.000000 biofilm-0.0.97/biofilm/_version.py
-drwxr-xr-x   0 ikea      (1000) ikea      (1000)        0 2022-11-17 13:28:22.220562 biofilm-0.0.97/biofilm/algo/
--rw-r--r--   0 ikea      (1000) ikea      (1000)     3541 2022-01-18 20:18:35.000000 biofilm-0.0.97/biofilm/algo/feature_inspection.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)     9096 2022-01-18 20:18:35.000000 biofilm-0.0.97/biofilm/algo/feature_selection.py
-drwxr-xr-x   0 ikea      (1000) ikea      (1000)        0 2022-11-17 13:28:22.220562 biofilm-0.0.97/biofilm/binsearch/
--rw-r--r--   0 ikea      (1000) ikea      (1000)     3294 2022-01-18 20:18:35.000000 biofilm-0.0.97/biofilm/binsearch/binsearch.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)     2179 2021-06-04 13:52:22.000000 biofilm-0.0.97/biofilm/binsearch/limit.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)     1016 2021-12-20 18:39:59.000000 biofilm-0.0.97/biofilm/biofilm-cv.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)      715 2022-01-27 13:41:31.000000 biofilm-0.0.97/biofilm/biofilm-featurefiles.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)     1486 2022-01-18 20:18:35.000000 biofilm-0.0.97/biofilm/biofilm-features.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)      854 2021-12-13 13:15:33.000000 biofilm-0.0.97/biofilm/biofilm-inspect.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)     1242 2021-10-21 15:03:14.000000 biofilm-0.0.97/biofilm/biofilm-optimize.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)     1673 2021-06-04 13:52:22.000000 biofilm-0.0.97/biofilm/biofilm-optimize2.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)     1068 2021-06-04 13:52:22.000000 biofilm-0.0.97/biofilm/biofilm-optimize3.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)     2009 2021-06-04 13:52:22.000000 biofilm-0.0.97/biofilm/biofilm-optimize4.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)     3381 2022-11-17 13:15:46.000000 biofilm-0.0.97/biofilm/biofilm-optimize6.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)     3626 2022-01-27 13:41:33.000000 biofilm-0.0.97/biofilm/biofilm-out.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)      849 2021-12-16 20:13:48.000000 biofilm-0.0.97/biofilm/biofilm-test.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)     1753 2021-10-21 15:03:14.000000 biofilm-0.0.97/biofilm/biofilm_mlp.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)     1180 2021-10-21 15:03:14.000000 biofilm-0.0.97/biofilm/runall.fish
--rw-r--r--   0 ikea      (1000) ikea      (1000)     7189 2021-06-04 13:52:22.000000 biofilm-0.0.97/biofilm/searchspace.py
-drwxr-xr-x   0 ikea      (1000) ikea      (1000)        0 2022-11-17 13:28:22.220562 biofilm-0.0.97/biofilm/util/
--rw-r--r--   0 ikea      (1000) ikea      (1000)      416 2021-11-15 13:27:56.000000 biofilm-0.0.97/biofilm/util/__init__.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)     3065 2022-01-22 14:44:25.000000 biofilm-0.0.97/biofilm/util/data.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)     1543 2021-11-18 22:59:05.000000 biofilm-0.0.97/biofilm/util/draw.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)     2763 2022-04-08 12:43:28.000000 biofilm-0.0.97/biofilm/util/out.py
-drwxr-xr-x   0 ikea      (1000) ikea      (1000)        0 2022-11-17 13:28:22.220562 biofilm-0.0.97/biofilm.egg-info/
--rw-r--r--   0 ikea      (1000) ikea      (1000)      256 2022-11-17 13:28:22.000000 biofilm-0.0.97/biofilm.egg-info/PKG-INFO
--rw-r--r--   0 ikea      (1000) ikea      (1000)      952 2022-11-17 13:28:22.000000 biofilm-0.0.97/biofilm.egg-info/SOURCES.txt
--rw-r--r--   0 ikea      (1000) ikea      (1000)        1 2022-11-17 13:28:22.000000 biofilm-0.0.97/biofilm.egg-info/dependency_links.txt
--rw-r--r--   0 ikea      (1000) ikea      (1000)      160 2022-11-17 13:28:22.000000 biofilm-0.0.97/biofilm.egg-info/requires.txt
--rw-r--r--   0 ikea      (1000) ikea      (1000)        8 2022-11-17 13:28:22.000000 biofilm-0.0.97/biofilm.egg-info/top_level.txt
--rw-r--r--   0 ikea      (1000) ikea      (1000)     7012 2022-06-17 12:54:10.000000 biofilm-0.0.97/cherry1C20.spy
--rw-r--r--   0 ikea      (1000) ikea      (1000)     2363 2021-12-20 19:12:11.000000 biofilm-0.0.97/cherryNOG1B26.xsh
--rw-r--r--   0 ikea      (1000) ikea      (1000)     2389 2021-10-21 15:03:14.000000 biofilm-0.0.97/cherryexample.xsh
--rw-r--r--   0 ikea      (1000) ikea      (1000)     4124 2021-12-13 13:15:33.000000 biofilm-0.0.97/cherryexampleNOG.xsh
-drwxr-xr-x   0 ikea      (1000) ikea      (1000)        0 2022-11-17 13:28:22.220562 biofilm-0.0.97/examples/
--rw-r--r--   0 ikea      (1000) ikea      (1000)     4260 2022-04-08 12:43:28.000000 biofilm-0.0.97/examples/cherriload.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)      149 2021-10-21 15:03:14.000000 biofilm-0.0.97/examples/npzloader.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)     1723 2021-10-21 15:03:14.000000 biofilm-0.0.97/examples/pigdataframe.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)       38 2022-11-17 13:28:22.223896 biofilm-0.0.97/setup.cfg
--rw-r--r--   0 ikea      (1000) ikea      (1000)     3768 2022-08-23 13:56:12.000000 biofilm-0.0.97/setup.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)      202 2022-04-08 12:43:28.000000 biofilm-0.0.97/showmodels.spy
+drwxr-xr-x   0 ikea      (1000) ikea      (1000)        0 2022-11-17 16:02:37.540019 biofilm-0.0.98/
+-rw-r--r--   0 ikea      (1000) ikea      (1000)      256 2022-11-17 16:02:37.536685 biofilm-0.0.98/PKG-INFO
+-rw-r--r--   0 ikea      (1000) ikea      (1000)     1173 2022-01-27 13:39:21.000000 biofilm-0.0.98/README.md
+drwxr-xr-x   0 ikea      (1000) ikea      (1000)        0 2022-11-17 16:02:37.536685 biofilm-0.0.98/biofilm/
+-rw-r--r--   0 ikea      (1000) ikea      (1000)     2017 2021-10-21 15:03:14.000000 biofilm-0.0.98/biofilm/FTBOXPLOT.fish
+-rw-r--r--   0 ikea      (1000) ikea      (1000)      179 2022-11-17 16:02:37.000000 biofilm-0.0.98/biofilm/_version.py
+drwxr-xr-x   0 ikea      (1000) ikea      (1000)        0 2022-11-17 16:02:37.536685 biofilm-0.0.98/biofilm/algo/
+-rw-r--r--   0 ikea      (1000) ikea      (1000)     3541 2022-01-18 20:18:35.000000 biofilm-0.0.98/biofilm/algo/feature_inspection.py
+-rw-r--r--   0 ikea      (1000) ikea      (1000)     9096 2022-01-18 20:18:35.000000 biofilm-0.0.98/biofilm/algo/feature_selection.py
+drwxr-xr-x   0 ikea      (1000) ikea      (1000)        0 2022-11-17 16:02:37.536685 biofilm-0.0.98/biofilm/binsearch/
+-rw-r--r--   0 ikea      (1000) ikea      (1000)     3294 2022-01-18 20:18:35.000000 biofilm-0.0.98/biofilm/binsearch/binsearch.py
+-rw-r--r--   0 ikea      (1000) ikea      (1000)     2179 2021-06-04 13:52:22.000000 biofilm-0.0.98/biofilm/binsearch/limit.py
+-rw-r--r--   0 ikea      (1000) ikea      (1000)     1016 2021-12-20 18:39:59.000000 biofilm-0.0.98/biofilm/biofilm-cv.py
+-rw-r--r--   0 ikea      (1000) ikea      (1000)      715 2022-01-27 13:41:31.000000 biofilm-0.0.98/biofilm/biofilm-featurefiles.py
+-rw-r--r--   0 ikea      (1000) ikea      (1000)     1486 2022-01-18 20:18:35.000000 biofilm-0.0.98/biofilm/biofilm-features.py
+-rw-r--r--   0 ikea      (1000) ikea      (1000)      854 2021-12-13 13:15:33.000000 biofilm-0.0.98/biofilm/biofilm-inspect.py
+-rw-r--r--   0 ikea      (1000) ikea      (1000)     1242 2021-10-21 15:03:14.000000 biofilm-0.0.98/biofilm/biofilm-optimize.py
+-rw-r--r--   0 ikea      (1000) ikea      (1000)     1673 2021-06-04 13:52:22.000000 biofilm-0.0.98/biofilm/biofilm-optimize2.py
+-rw-r--r--   0 ikea      (1000) ikea      (1000)     1068 2021-06-04 13:52:22.000000 biofilm-0.0.98/biofilm/biofilm-optimize3.py
+-rw-r--r--   0 ikea      (1000) ikea      (1000)     2009 2021-06-04 13:52:22.000000 biofilm-0.0.98/biofilm/biofilm-optimize4.py
+-rw-r--r--   0 ikea      (1000) ikea      (1000)     3381 2022-11-17 13:15:46.000000 biofilm-0.0.98/biofilm/biofilm-optimize6.py
+-rw-r--r--   0 ikea      (1000) ikea      (1000)     3626 2022-01-27 13:41:33.000000 biofilm-0.0.98/biofilm/biofilm-out.py
+-rw-r--r--   0 ikea      (1000) ikea      (1000)      849 2021-12-16 20:13:48.000000 biofilm-0.0.98/biofilm/biofilm-test.py
+-rw-r--r--   0 ikea      (1000) ikea      (1000)     1753 2021-10-21 15:03:14.000000 biofilm-0.0.98/biofilm/biofilm_mlp.py
+-rw-r--r--   0 ikea      (1000) ikea      (1000)     1180 2021-10-21 15:03:14.000000 biofilm-0.0.98/biofilm/runall.fish
+-rw-r--r--   0 ikea      (1000) ikea      (1000)     7189 2021-06-04 13:52:22.000000 biofilm-0.0.98/biofilm/searchspace.py
+drwxr-xr-x   0 ikea      (1000) ikea      (1000)        0 2022-11-17 16:02:37.536685 biofilm-0.0.98/biofilm/util/
+-rw-r--r--   0 ikea      (1000) ikea      (1000)      416 2021-11-15 13:27:56.000000 biofilm-0.0.98/biofilm/util/__init__.py
+-rw-r--r--   0 ikea      (1000) ikea      (1000)     3065 2022-01-22 14:44:25.000000 biofilm-0.0.98/biofilm/util/data.py
+-rw-r--r--   0 ikea      (1000) ikea      (1000)     1543 2021-11-18 22:59:05.000000 biofilm-0.0.98/biofilm/util/draw.py
+-rw-r--r--   0 ikea      (1000) ikea      (1000)     2763 2022-04-08 12:43:28.000000 biofilm-0.0.98/biofilm/util/out.py
+drwxr-xr-x   0 ikea      (1000) ikea      (1000)        0 2022-11-17 16:02:37.536685 biofilm-0.0.98/biofilm.egg-info/
+-rw-r--r--   0 ikea      (1000) ikea      (1000)      256 2022-11-17 16:02:37.000000 biofilm-0.0.98/biofilm.egg-info/PKG-INFO
+-rw-r--r--   0 ikea      (1000) ikea      (1000)      952 2022-11-17 16:02:37.000000 biofilm-0.0.98/biofilm.egg-info/SOURCES.txt
+-rw-r--r--   0 ikea      (1000) ikea      (1000)        1 2022-11-17 16:02:37.000000 biofilm-0.0.98/biofilm.egg-info/dependency_links.txt
+-rw-r--r--   0 ikea      (1000) ikea      (1000)      155 2022-11-17 16:02:37.000000 biofilm-0.0.98/biofilm.egg-info/requires.txt
+-rw-r--r--   0 ikea      (1000) ikea      (1000)        8 2022-11-17 16:02:37.000000 biofilm-0.0.98/biofilm.egg-info/top_level.txt
+-rw-r--r--   0 ikea      (1000) ikea      (1000)     7012 2022-06-17 12:54:10.000000 biofilm-0.0.98/cherry1C20.spy
+-rw-r--r--   0 ikea      (1000) ikea      (1000)     2363 2021-12-20 19:12:11.000000 biofilm-0.0.98/cherryNOG1B26.xsh
+-rw-r--r--   0 ikea      (1000) ikea      (1000)     2389 2021-10-21 15:03:14.000000 biofilm-0.0.98/cherryexample.xsh
+-rw-r--r--   0 ikea      (1000) ikea      (1000)     4124 2021-12-13 13:15:33.000000 biofilm-0.0.98/cherryexampleNOG.xsh
+drwxr-xr-x   0 ikea      (1000) ikea      (1000)        0 2022-11-17 16:02:37.536685 biofilm-0.0.98/examples/
+-rw-r--r--   0 ikea      (1000) ikea      (1000)     4260 2022-04-08 12:43:28.000000 biofilm-0.0.98/examples/cherriload.py
+-rw-r--r--   0 ikea      (1000) ikea      (1000)      149 2021-10-21 15:03:14.000000 biofilm-0.0.98/examples/npzloader.py
+-rw-r--r--   0 ikea      (1000) ikea      (1000)     1723 2021-10-21 15:03:14.000000 biofilm-0.0.98/examples/pigdataframe.py
+-rw-r--r--   0 ikea      (1000) ikea      (1000)       38 2022-11-17 16:02:37.540019 biofilm-0.0.98/setup.cfg
+-rw-r--r--   0 ikea      (1000) ikea      (1000)     3763 2022-11-17 16:01:32.000000 biofilm-0.0.98/setup.py
+-rw-r--r--   0 ikea      (1000) ikea      (1000)      202 2022-04-08 12:43:28.000000 biofilm-0.0.98/showmodels.spy
```

### Comparing `biofilm-0.0.97/README.md` & `biofilm-0.0.98/README.md`

 * *Files identical despite different names*

### Comparing `biofilm-0.0.97/biofilm/FTBOXPLOT.fish` & `biofilm-0.0.98/biofilm/FTBOXPLOT.fish`

 * *Files identical despite different names*

### Comparing `biofilm-0.0.97/biofilm/algo/feature_inspection.py` & `biofilm-0.0.98/biofilm/algo/feature_inspection.py`

 * *Files identical despite different names*

### Comparing `biofilm-0.0.97/biofilm/algo/feature_selection.py` & `biofilm-0.0.98/biofilm/algo/feature_selection.py`

 * *Files identical despite different names*

### Comparing `biofilm-0.0.97/biofilm/binsearch/binsearch.py` & `biofilm-0.0.98/biofilm/binsearch/binsearch.py`

 * *Files identical despite different names*

### Comparing `biofilm-0.0.97/biofilm/binsearch/limit.py` & `biofilm-0.0.98/biofilm/binsearch/limit.py`

 * *Files identical despite different names*

### Comparing `biofilm-0.0.97/biofilm/biofilm-cv.py` & `biofilm-0.0.98/biofilm/biofilm-cv.py`

 * *Files identical despite different names*

### Comparing `biofilm-0.0.97/biofilm/biofilm-featurefiles.py` & `biofilm-0.0.98/biofilm/biofilm-featurefiles.py`

 * *Files identical despite different names*

### Comparing `biofilm-0.0.97/biofilm/biofilm-features.py` & `biofilm-0.0.98/biofilm/biofilm-features.py`

 * *Files identical despite different names*

### Comparing `biofilm-0.0.97/biofilm/biofilm-inspect.py` & `biofilm-0.0.98/biofilm/biofilm-inspect.py`

 * *Files identical despite different names*

### Comparing `biofilm-0.0.97/biofilm/biofilm-optimize.py` & `biofilm-0.0.98/biofilm/biofilm-optimize.py`

 * *Files identical despite different names*

### Comparing `biofilm-0.0.97/biofilm/biofilm-optimize2.py` & `biofilm-0.0.98/biofilm/biofilm-optimize2.py`

 * *Files identical despite different names*

### Comparing `biofilm-0.0.97/biofilm/biofilm-optimize3.py` & `biofilm-0.0.98/biofilm/biofilm-optimize3.py`

 * *Files identical despite different names*

### Comparing `biofilm-0.0.97/biofilm/biofilm-optimize4.py` & `biofilm-0.0.98/biofilm/biofilm-optimize4.py`

 * *Files identical despite different names*

### Comparing `biofilm-0.0.97/biofilm/biofilm-optimize6.py` & `biofilm-0.0.98/biofilm/biofilm-optimize6.py`

 * *Files identical despite different names*

### Comparing `biofilm-0.0.97/biofilm/biofilm-out.py` & `biofilm-0.0.98/biofilm/biofilm-out.py`

 * *Files identical despite different names*

### Comparing `biofilm-0.0.97/biofilm/biofilm-test.py` & `biofilm-0.0.98/biofilm/biofilm-test.py`

 * *Files identical despite different names*

### Comparing `biofilm-0.0.97/biofilm/biofilm_mlp.py` & `biofilm-0.0.98/biofilm/biofilm_mlp.py`

 * *Files identical despite different names*

### Comparing `biofilm-0.0.97/biofilm/runall.fish` & `biofilm-0.0.98/biofilm/runall.fish`

 * *Files identical despite different names*

### Comparing `biofilm-0.0.97/biofilm/searchspace.py` & `biofilm-0.0.98/biofilm/searchspace.py`

 * *Files identical despite different names*

### Comparing `biofilm-0.0.97/biofilm/util/data.py` & `biofilm-0.0.98/biofilm/util/data.py`

 * *Files identical despite different names*

### Comparing `biofilm-0.0.97/biofilm/util/draw.py` & `biofilm-0.0.98/biofilm/util/draw.py`

 * *Files identical despite different names*

### Comparing `biofilm-0.0.97/biofilm/util/out.py` & `biofilm-0.0.98/biofilm/util/out.py`

 * *Files identical despite different names*

### Comparing `biofilm-0.0.97/biofilm.egg-info/SOURCES.txt` & `biofilm-0.0.98/biofilm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biofilm-0.0.97/cherry1C20.spy` & `biofilm-0.0.98/cherry1C20.spy`

 * *Files identical despite different names*

### Comparing `biofilm-0.0.97/cherryNOG1B26.xsh` & `biofilm-0.0.98/cherryNOG1B26.xsh`

 * *Files identical despite different names*

### Comparing `biofilm-0.0.97/cherryexample.xsh` & `biofilm-0.0.98/cherryexample.xsh`

 * *Files identical despite different names*

### Comparing `biofilm-0.0.97/cherryexampleNOG.xsh` & `biofilm-0.0.98/cherryexampleNOG.xsh`

 * *Files identical despite different names*

### Comparing `biofilm-0.0.97/examples/cherriload.py` & `biofilm-0.0.98/examples/cherriload.py`

 * *Files identical despite different names*

### Comparing `biofilm-0.0.97/examples/pigdataframe.py` & `biofilm-0.0.98/examples/pigdataframe.py`

 * *Files identical despite different names*

### Comparing `biofilm-0.0.97/setup.py` & `biofilm-0.0.98/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,14 @@
     install_requires=[
         'scikit-learn >= 0.24.2',
         'ubergauss==0.0.43',
         'lmz==0.1.12',
         'dirtyopts==0.0.18',
         'numpy >= 1.22.0',
         'structout==0.1.44',
-        'auto-sklearn == 0.14.2',
+        'auto-sklearn == 0.15',
         "eden-kernel==0.3.1348",
-        "pynisher==0.6.4" # automl 14.2 doesnt pick the right versionhere..
+        "pynisher<=.7" # automl 14.2 doesnt pick the right versionhere..
         ],
     #entry_points = { 'console_scripts': ['biofilmop=biofilm.biofilm-optimize:main','biofilmft=biofilm.biofilm-features:main'] },
     cmdclass={'sdist': sdist, 'install': install}
 )
```


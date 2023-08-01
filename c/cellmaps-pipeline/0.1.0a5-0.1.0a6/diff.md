# Comparing `tmp/cellmaps_pipeline-0.1.0a5.tar.gz` & `tmp/cellmaps_pipeline-0.1.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_pipeline-0.1.0a5.tar", last modified: Mon Jul 24 23:42:38 2023, max compression
+gzip compressed data, was "dist/cellmaps_pipeline-0.1.0a6.tar", last modified: Tue Aug  1 22:27:37 2023, max compression
```

## Comparing `cellmaps_pipeline-0.1.0a5.tar` & `cellmaps_pipeline-0.1.0a6.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:42:38.562969 cellmaps_pipeline-0.1.0a5/
--rw-r--r--   0 churas     (504) staff       (20)      266 2023-06-08 20:06:13.000000 cellmaps_pipeline-0.1.0a5/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3641 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a5/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-22 23:49:21.000000 cellmaps_pipeline-0.1.0a5/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a5/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a5/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     6081 2023-07-24 23:42:38.563137 cellmaps_pipeline-0.1.0a5/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     4079 2023-07-17 23:45:49.000000 cellmaps_pipeline-0.1.0a5/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:42:38.554401 cellmaps_pipeline-0.1.0a5/cellmaps_pipeline/
--rw-r--r--   0 churas     (504) staff       (20)      279 2023-07-24 23:42:04.000000 cellmaps_pipeline-0.1.0a5/cellmaps_pipeline/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     8923 2023-07-17 20:25:30.000000 cellmaps_pipeline-0.1.0a5/cellmaps_pipeline/cellmaps_pipelinecmd.py
--rw-r--r--   0 churas     (504) staff       (20)      132 2023-04-04 23:01:54.000000 cellmaps_pipeline-0.1.0a5/cellmaps_pipeline/exceptions.py
--rw-r--r--   0 churas     (504) staff       (20)    12687 2023-07-17 20:25:30.000000 cellmaps_pipeline-0.1.0a5/cellmaps_pipeline/runner.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:42:38.555945 cellmaps_pipeline-0.1.0a5/cellmaps_pipeline.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     6081 2023-07-24 23:42:38.000000 cellmaps_pipeline-0.1.0a5/cellmaps_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     1105 2023-07-24 23:42:38.000000 cellmaps_pipeline-0.1.0a5/cellmaps_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-07-24 23:42:38.000000 cellmaps_pipeline-0.1.0a5/cellmaps_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-07-24 23:42:38.000000 cellmaps_pipeline-0.1.0a5/cellmaps_pipeline.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)      243 2023-07-24 23:42:38.000000 cellmaps_pipeline-0.1.0a5/cellmaps_pipeline.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       18 2023-07-24 23:42:38.000000 cellmaps_pipeline-0.1.0a5/cellmaps_pipeline.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:42:38.560254 cellmaps_pipeline-0.1.0a5/docs/
--rw-r--r--   0 churas     (504) staff       (20)      618 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a5/docs/Makefile
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:42:38.551017 cellmaps_pipeline-0.1.0a5/docs/_build/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:42:38.551245 cellmaps_pipeline-0.1.0a5/docs/_build/html/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:42:38.560514 cellmaps_pipeline-0.1.0a5/docs/_build/html/_images/
--rw-r--r--   0 churas     (504) staff       (20)    29975 2023-07-18 21:25:06.000000 cellmaps_pipeline-0.1.0a5/docs/_build/html/_images/pipeline_overview.png
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:42:38.561359 cellmaps_pipeline-0.1.0a5/docs/_build/html/_static/
--rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a5/docs/_build/html/_static/file.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a5/docs/_build/html/_static/minus.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a5/docs/_build/html/_static/plus.png
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a5/docs/authors.rst
--rw-r--r--   0 churas     (504) staff       (20)      744 2023-05-22 23:59:43.000000 cellmaps_pipeline-0.1.0a5/docs/cellmaps_pipeline.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     6035 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a5/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a5/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a5/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      285 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a5/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a5/docs/history.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:42:38.561608 cellmaps_pipeline-0.1.0a5/docs/images/
--rw-r--r--   0 churas     (504) staff       (20)    29975 2023-07-18 21:25:06.000000 cellmaps_pipeline-0.1.0a5/docs/images/pipeline_overview.png
--rw-r--r--   0 churas     (504) staff       (20)     1783 2023-07-18 21:44:38.000000 cellmaps_pipeline-0.1.0a5/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1189 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a5/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      451 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a5/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      815 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a5/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       76 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a5/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4340 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a5/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      787 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a5/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)      653 2023-07-18 21:56:02.000000 cellmaps_pipeline-0.1.0a5/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a5/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      400 2023-07-24 23:42:38.564432 cellmaps_pipeline-0.1.0a5/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     2460 2023-07-24 23:41:04.000000 cellmaps_pipeline-0.1.0a5/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:42:38.562735 cellmaps_pipeline-0.1.0a5/tests/
--rw-r--r--   0 churas     (504) staff       (20)       72 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a5/tests/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     1296 2023-06-07 18:25:27.000000 cellmaps_pipeline-0.1.0a5/tests/test_cellmaps_pipelinecmd.py
--rw-r--r--   0 churas     (504) staff       (20)      896 2023-06-07 18:25:27.000000 cellmaps_pipeline-0.1.0a5/tests/test_cellmapspipeline.py
--rw-r--r--   0 churas     (504) staff       (20)      772 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a5/tests/test_integration_cellmaps_pipeline.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-01 22:27:37.890920 cellmaps_pipeline-0.1.0a6/
+-rw-r--r--   0 churas     (504) staff       (20)      266 2023-06-08 20:06:13.000000 cellmaps_pipeline-0.1.0a6/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3641 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a6/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-22 23:49:21.000000 cellmaps_pipeline-0.1.0a6/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a6/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a6/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     6081 2023-08-01 22:27:37.891053 cellmaps_pipeline-0.1.0a6/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     4079 2023-08-01 00:51:41.000000 cellmaps_pipeline-0.1.0a6/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-01 22:27:37.881792 cellmaps_pipeline-0.1.0a6/cellmaps_pipeline/
+-rw-r--r--   0 churas     (504) staff       (20)      279 2023-08-01 22:27:17.000000 cellmaps_pipeline-0.1.0a6/cellmaps_pipeline/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     8923 2023-07-17 20:25:30.000000 cellmaps_pipeline-0.1.0a6/cellmaps_pipeline/cellmaps_pipelinecmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      132 2023-04-04 23:01:54.000000 cellmaps_pipeline-0.1.0a6/cellmaps_pipeline/exceptions.py
+-rw-r--r--   0 churas     (504) staff       (20)    12687 2023-07-17 20:25:30.000000 cellmaps_pipeline-0.1.0a6/cellmaps_pipeline/runner.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-01 22:27:37.883806 cellmaps_pipeline-0.1.0a6/cellmaps_pipeline.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     6081 2023-08-01 22:27:37.000000 cellmaps_pipeline-0.1.0a6/cellmaps_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     1105 2023-08-01 22:27:37.000000 cellmaps_pipeline-0.1.0a6/cellmaps_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-08-01 22:27:37.000000 cellmaps_pipeline-0.1.0a6/cellmaps_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-08-01 22:27:37.000000 cellmaps_pipeline-0.1.0a6/cellmaps_pipeline.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)      243 2023-08-01 22:27:37.000000 cellmaps_pipeline-0.1.0a6/cellmaps_pipeline.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       18 2023-08-01 22:27:37.000000 cellmaps_pipeline-0.1.0a6/cellmaps_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-01 22:27:37.888386 cellmaps_pipeline-0.1.0a6/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      618 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a6/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-01 22:27:37.878167 cellmaps_pipeline-0.1.0a6/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-01 22:27:37.878352 cellmaps_pipeline-0.1.0a6/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-01 22:27:37.888658 cellmaps_pipeline-0.1.0a6/docs/_build/html/_images/
+-rw-r--r--   0 churas     (504) staff       (20)    29975 2023-07-18 21:25:06.000000 cellmaps_pipeline-0.1.0a6/docs/_build/html/_images/pipeline_overview.png
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-01 22:27:37.889481 cellmaps_pipeline-0.1.0a6/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a6/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a6/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a6/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a6/docs/authors.rst
+-rw-r--r--   0 churas     (504) staff       (20)      744 2023-05-22 23:59:43.000000 cellmaps_pipeline-0.1.0a6/docs/cellmaps_pipeline.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     6035 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a6/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a6/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a6/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      285 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a6/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a6/docs/history.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-01 22:27:37.889760 cellmaps_pipeline-0.1.0a6/docs/images/
+-rw-r--r--   0 churas     (504) staff       (20)    29975 2023-08-01 00:51:42.000000 cellmaps_pipeline-0.1.0a6/docs/images/pipeline_overview.png
+-rw-r--r--   0 churas     (504) staff       (20)     1783 2023-08-01 00:51:42.000000 cellmaps_pipeline-0.1.0a6/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1189 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a6/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      451 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a6/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      815 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a6/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       76 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a6/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4340 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a6/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      787 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a6/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)      884 2023-08-01 00:51:42.000000 cellmaps_pipeline-0.1.0a6/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a6/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      400 2023-08-01 22:27:37.892075 cellmaps_pipeline-0.1.0a6/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     2460 2023-08-01 22:27:17.000000 cellmaps_pipeline-0.1.0a6/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-01 22:27:37.890695 cellmaps_pipeline-0.1.0a6/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       72 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a6/tests/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     1296 2023-06-07 18:25:27.000000 cellmaps_pipeline-0.1.0a6/tests/test_cellmaps_pipelinecmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      896 2023-06-07 18:25:27.000000 cellmaps_pipeline-0.1.0a6/tests/test_cellmapspipeline.py
+-rw-r--r--   0 churas     (504) staff       (20)      772 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a6/tests/test_integration_cellmaps_pipeline.py
```

### Comparing `cellmaps_pipeline-0.1.0a5/CONTRIBUTING.rst` & `cellmaps_pipeline-0.1.0a6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a5/LICENSE` & `cellmaps_pipeline-0.1.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a5/PKG-INFO` & `cellmaps_pipeline-0.1.0a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps_pipeline
-Version: 0.1.0a5
+Version: 0.1.0a6
 Summary: Runs full Cellmaps CM4AI pipeline
 Home-page: https://github.com/idekerlab/cellmaps_pipeline
 Author: Ideker Lab CM4AI team
 Author-email: tools@cm4ai.org
 License: MIT license
 Description: ===================
         Cell Maps Pipeline
```

### Comparing `cellmaps_pipeline-0.1.0a5/README.rst` & `cellmaps_pipeline-0.1.0a6/README.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a5/cellmaps_pipeline/cellmaps_pipelinecmd.py` & `cellmaps_pipeline-0.1.0a6/cellmaps_pipeline/cellmaps_pipelinecmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a5/cellmaps_pipeline/runner.py` & `cellmaps_pipeline-0.1.0a6/cellmaps_pipeline/runner.py`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a5/cellmaps_pipeline.egg-info/PKG-INFO` & `cellmaps_pipeline-0.1.0a6/cellmaps_pipeline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps-pipeline
-Version: 0.1.0a5
+Version: 0.1.0a6
 Summary: Runs full Cellmaps CM4AI pipeline
 Home-page: https://github.com/idekerlab/cellmaps_pipeline
 Author: Ideker Lab CM4AI team
 Author-email: tools@cm4ai.org
 License: MIT license
 Description: ===================
         Cell Maps Pipeline
```

### Comparing `cellmaps_pipeline-0.1.0a5/cellmaps_pipeline.egg-info/SOURCES.txt` & `cellmaps_pipeline-0.1.0a6/cellmaps_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a5/docs/Makefile` & `cellmaps_pipeline-0.1.0a6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a5/docs/_build/html/_images/pipeline_overview.png` & `cellmaps_pipeline-0.1.0a6/docs/_build/html/_images/pipeline_overview.png`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a5/docs/cellmaps_pipeline.rst` & `cellmaps_pipeline-0.1.0a6/docs/cellmaps_pipeline.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a5/docs/conf.py` & `cellmaps_pipeline-0.1.0a6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a5/docs/images/pipeline_overview.png` & `cellmaps_pipeline-0.1.0a6/docs/images/pipeline_overview.png`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a5/docs/index.rst` & `cellmaps_pipeline-0.1.0a6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a5/docs/installation.rst` & `cellmaps_pipeline-0.1.0a6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a5/docs/make.bat` & `cellmaps_pipeline-0.1.0a6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a5/docs/newrelease.rst` & `cellmaps_pipeline-0.1.0a6/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a5/docs/pypircfile.rst` & `cellmaps_pipeline-0.1.0a6/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a5/docs/versioningscheme.rst` & `cellmaps_pipeline-0.1.0a6/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a5/setup.py` & `cellmaps_pipeline-0.1.0a6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
-requirements = ['cellmaps_utils==0.1.0a13',
-                'cellmaps_imagedownloader==0.1.0a6',
+requirements = ['cellmaps_utils==0.1.0a14',
+                'cellmaps_imagedownloader==0.1.0a7',
                 'cellmaps_ppidownloader==0.1.0a3',
                 'cellmaps_image_embedding==0.1.0a7',
                 'cellmaps_ppi_embedding==0.1.0a4',
                 'cellmaps_coembedding==0.1.0a4',
                 'cellmaps_generate_hierarchy==0.1.0a6',
                 'networkx>=2.8,<2.9']
```

### Comparing `cellmaps_pipeline-0.1.0a5/tests/test_cellmaps_pipelinecmd.py` & `cellmaps_pipeline-0.1.0a6/tests/test_cellmaps_pipelinecmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a5/tests/test_cellmapspipeline.py` & `cellmaps_pipeline-0.1.0a6/tests/test_cellmapspipeline.py`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a5/tests/test_integration_cellmaps_pipeline.py` & `cellmaps_pipeline-0.1.0a6/tests/test_integration_cellmaps_pipeline.py`

 * *Files identical despite different names*


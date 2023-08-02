# Comparing `tmp/cellmaps_image_embedding-0.1.0a7.tar.gz` & `tmp/cellmaps_image_embedding-0.1.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_image_embedding-0.1.0a7.tar", last modified: Mon Jul 17 19:15:09 2023, max compression
+gzip compressed data, was "dist/cellmaps_image_embedding-0.1.0a8.tar", last modified: Wed Aug  2 01:47:59 2023, max compression
```

## Comparing `cellmaps_image_embedding-0.1.0a7.tar` & `cellmaps_image_embedding-0.1.0a8.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:15:09.914353 cellmaps_image_embedding-0.1.0a7/
--rw-r--r--   0 churas     (504) staff       (20)      266 2023-07-17 19:14:35.000000 cellmaps_image_embedding-0.1.0a7/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3731 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-18 23:31:36.000000 cellmaps_image_embedding-0.1.0a7/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     6288 2023-07-17 19:15:09.914637 cellmaps_image_embedding-0.1.0a7/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     4186 2023-06-07 21:49:02.000000 cellmaps_image_embedding-0.1.0a7/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:15:09.904662 cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding/
--rw-r--r--   0 churas     (504) staff       (20)      312 2023-06-07 21:49:02.000000 cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     6564 2023-06-15 20:35:46.000000 cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding/cellmaps_image_embeddingcmd.py
--rw-r--r--   0 churas     (504) staff       (20)     5706 2023-06-15 20:35:46.000000 cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding/dataset.py
--rw-r--r--   0 churas     (504) staff       (20)      143 2023-03-30 21:25:53.000000 cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding/exceptions.py
--rw-r--r--   0 churas     (504) staff       (20)     7602 2023-05-16 19:18:42.000000 cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding/models.py
--rw-r--r--   0 churas     (504) staff       (20)    20356 2023-06-15 20:35:46.000000 cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding/runner.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:15:09.906363 cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     6288 2023-07-17 19:15:09.000000 cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     1207 2023-07-17 19:15:09.000000 cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-07-17 19:15:09.000000 cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-07-17 19:15:09.000000 cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)      121 2023-07-17 19:15:09.000000 cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       25 2023-07-17 19:15:09.000000 cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:15:09.911823 cellmaps_image_embedding-0.1.0a7/docs/
--rw-r--r--   0 churas     (504) staff       (20)      625 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/Makefile
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:15:09.900261 cellmaps_image_embedding-0.1.0a7/docs/_build/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:15:09.900333 cellmaps_image_embedding-0.1.0a7/docs/_build/html/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:15:09.912843 cellmaps_image_embedding-0.1.0a7/docs/_build/html/_static/
--rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_image_embedding-0.1.0a7/docs/_build/html/_static/file.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_image_embedding-0.1.0a7/docs/_build/html/_static/minus.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_image_embedding-0.1.0a7/docs/_build/html/_static/plus.png
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/authors.rst
--rw-r--r--   0 churas     (504) staff       (20)     1234 2023-05-18 23:15:22.000000 cellmaps_image_embedding-0.1.0a7/docs/cellmaps_image_embedding.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     6131 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      292 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/history.rst
--rw-r--r--   0 churas     (504) staff       (20)      986 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1254 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      472 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      822 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       83 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4424 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      794 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)      739 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      407 2023-07-17 19:15:09.915253 cellmaps_image_embedding-0.1.0a7/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     2463 2023-06-15 20:35:46.000000 cellmaps_image_embedding-0.1.0a7/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:15:09.914066 cellmaps_image_embedding-0.1.0a7/tests/
--rw-r--r--   0 churas     (504) staff       (20)       79 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/tests/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     1630 2023-05-08 16:58:10.000000 cellmaps_image_embedding-0.1.0a7/tests/test_cellmaps_image_embeddingcmd.py
--rw-r--r--   0 churas     (504) staff       (20)     1394 2023-05-15 20:45:32.000000 cellmaps_image_embedding-0.1.0a7/tests/test_cellmaps_image_embeddingrunner.py
--rw-r--r--   0 churas     (504) staff       (20)      821 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a7/tests/test_integration_cellmaps_image_embedding.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 01:47:59.617403 cellmaps_image_embedding-0.1.0a8/
+-rw-r--r--   0 churas     (504) staff       (20)      266 2023-07-17 19:14:35.000000 cellmaps_image_embedding-0.1.0a8/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3731 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-18 23:31:36.000000 cellmaps_image_embedding-0.1.0a8/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     6446 2023-08-02 01:47:59.617558 cellmaps_image_embedding-0.1.0a8/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     4360 2023-07-26 17:56:48.000000 cellmaps_image_embedding-0.1.0a8/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 01:47:59.606394 cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding/
+-rw-r--r--   0 churas     (504) staff       (20)      312 2023-08-02 01:47:05.000000 cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     6564 2023-06-15 20:35:46.000000 cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding/cellmaps_image_embeddingcmd.py
+-rw-r--r--   0 churas     (504) staff       (20)     5706 2023-06-15 20:35:46.000000 cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding/dataset.py
+-rw-r--r--   0 churas     (504) staff       (20)      143 2023-03-30 21:25:53.000000 cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding/exceptions.py
+-rw-r--r--   0 churas     (504) staff       (20)     7602 2023-05-16 19:18:42.000000 cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding/models.py
+-rw-r--r--   0 churas     (504) staff       (20)    20431 2023-08-02 01:47:05.000000 cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding/runner.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 01:47:59.607975 cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     6446 2023-08-02 01:47:59.000000 cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     1207 2023-08-02 01:47:59.000000 cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-08-02 01:47:59.000000 cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-08-02 01:47:59.000000 cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)      121 2023-08-02 01:47:59.000000 cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       25 2023-08-02 01:47:59.000000 cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 01:47:59.614837 cellmaps_image_embedding-0.1.0a8/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      625 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 01:47:59.601784 cellmaps_image_embedding-0.1.0a8/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 01:47:59.601870 cellmaps_image_embedding-0.1.0a8/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 01:47:59.616062 cellmaps_image_embedding-0.1.0a8/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_image_embedding-0.1.0a8/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_image_embedding-0.1.0a8/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_image_embedding-0.1.0a8/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/docs/authors.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1234 2023-05-18 23:15:22.000000 cellmaps_image_embedding-0.1.0a8/docs/cellmaps_image_embedding.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     6131 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      292 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/docs/history.rst
+-rw-r--r--   0 churas     (504) staff       (20)      849 2023-07-26 17:56:48.000000 cellmaps_image_embedding-0.1.0a8/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1254 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      472 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      822 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       83 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4424 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      794 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)      739 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      407 2023-08-02 01:47:59.618089 cellmaps_image_embedding-0.1.0a8/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     2463 2023-06-15 20:35:46.000000 cellmaps_image_embedding-0.1.0a8/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 01:47:59.617179 cellmaps_image_embedding-0.1.0a8/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       79 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/tests/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     1630 2023-05-08 16:58:10.000000 cellmaps_image_embedding-0.1.0a8/tests/test_cellmaps_image_embeddingcmd.py
+-rw-r--r--   0 churas     (504) staff       (20)     1394 2023-05-15 20:45:32.000000 cellmaps_image_embedding-0.1.0a8/tests/test_cellmaps_image_embeddingrunner.py
+-rw-r--r--   0 churas     (504) staff       (20)      821 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/tests/test_integration_cellmaps_image_embedding.py
```

### Comparing `cellmaps_image_embedding-0.1.0a7/CONTRIBUTING.rst` & `cellmaps_image_embedding-0.1.0a8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a7/LICENSE` & `cellmaps_image_embedding-0.1.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a7/PKG-INFO` & `cellmaps_image_embedding-0.1.0a8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 Metadata-Version: 2.1
 Name: cellmaps_image_embedding
-Version: 0.1.0a7
+Version: 0.1.0a8
 Summary: A tool to generate embeddings from HPA IF images
 Home-page: https://github.com/idekerlab/cellmaps_image_embedding
 Author: Ideker Lab CM4AI team
 Author-email: tools@cm4ai.org
 License: MIT license
-Description: =========================
-        cellmaps_image_embedding
-        =========================
+Description: =============================================
+        Cell Maps ImmunoFluorescent Image Embedder
+        =============================================
         
         
         .. image:: https://img.shields.io/pypi/v/cellmaps_image_embedding.svg
                 :target: https://pypi.python.org/pypi/cellmaps_image_embedding
         
         .. image:: https://img.shields.io/travis/idekerlab/cellmaps_image_embedding.svg
                 :target: https://travis-ci.com/idekerlab/cellmaps_image_embedding
         
         .. image:: https://readthedocs.org/projects/cellmaps-image-embedding/badge/?version=latest
                 :target: https://cellmaps-image-embedding.readthedocs.io/en/latest/?badge=latest
                 :alt: Documentation Status
         
         
-        A tool to generate embeddings from HPA IF images
-        
+        Generate embeddings from ImmunoFluorescent image data from `Human Protein Atlas <https://www.proteinatlas.org/>`__
+        for `Cell Maps for AI (CM4AI) <https://cm4ai.org>`__
         
         * Free software: MIT license
         * Documentation: https://cellmaps-image-embedding.readthedocs.io.
         
-        
-        
         Dependencies
         ------------
         
         * `cellmaps_utils <https://pypi.org/project/cellmaps-utils>`__
         * `tqdm <https://pypi.org/project/tqdm>`__
         * `numpy <https://pypi.org/project/numpy>`__
         * `pandas>=0.23.1 <https://pypi.org/project/pandas>`__
```

### Comparing `cellmaps_image_embedding-0.1.0a7/README.rst` & `cellmaps_image_embedding-0.1.0a8/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-=========================
-cellmaps_image_embedding
-=========================
+=============================================
+Cell Maps ImmunoFluorescent Image Embedder
+=============================================
 
 
 .. image:: https://img.shields.io/pypi/v/cellmaps_image_embedding.svg
         :target: https://pypi.python.org/pypi/cellmaps_image_embedding
 
 .. image:: https://img.shields.io/travis/idekerlab/cellmaps_image_embedding.svg
         :target: https://travis-ci.com/idekerlab/cellmaps_image_embedding
 
 .. image:: https://readthedocs.org/projects/cellmaps-image-embedding/badge/?version=latest
         :target: https://cellmaps-image-embedding.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 
-A tool to generate embeddings from HPA IF images
-
+Generate embeddings from ImmunoFluorescent image data from `Human Protein Atlas <https://www.proteinatlas.org/>`__
+for `Cell Maps for AI (CM4AI) <https://cm4ai.org>`__
 
 * Free software: MIT license
 * Documentation: https://cellmaps-image-embedding.readthedocs.io.
 
-
-
 Dependencies
 ------------
 
 * `cellmaps_utils <https://pypi.org/project/cellmaps-utils>`__
 * `tqdm <https://pypi.org/project/tqdm>`__
 * `numpy <https://pypi.org/project/numpy>`__
 * `pandas>=0.23.1 <https://pypi.org/project/pandas>`__
```

### Comparing `cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding/cellmaps_image_embeddingcmd.py` & `cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding/cellmaps_image_embeddingcmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding/dataset.py` & `cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding/dataset.py`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding/models.py` & `cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding/models.py`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding/runner.py` & `cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #! /usr/bin/env python
 
 import os
 import sys
 import time
 from datetime import date
+import numpy as np
 import logging
 import csv
 import random
 import warnings
 import torch
 from torch.autograd import Variable
 from torch.nn import DataParallel
@@ -148,17 +149,17 @@
         """
         for image_id in self._get_image_id_list():
             if image_id not in self._img_emd_translator.get_name_mapping():
                 continue
             g =  self._img_emd_translator.get_name_mapping()[image_id]
 
             row = [g]
-            row.extend([random.random() for x in range(0, self.get_dimensions())]) ## check on the range of embeddings
+            row.extend(np.random.normal(size=self.get_dimensions()))  # sample normal distribution
             prob = [g]
-            prob.extend([random.random() for x in range(0,len(ABB_LABEL_INDEX.keys()))]) ## might need to add to one
+            prob.extend([random.random() for x in range(0, len(ABB_LABEL_INDEX.keys()))])  # might need to add to one
             yield row, prob
 
 
 class DensenetEmbeddingGenerator(EmbeddingGenerator):
     """
     Runs densenet bundled with this tool via command line to
     generate embedding. Why do it this way? Easier transition
@@ -209,17 +210,16 @@
         self._num_classes = 28
         self._seeds = [0]
         self._augments = ['default']
         self._model = self._initialize_model()
         self._dataset = self._initialize_dataset()
         self._dataloader = self._initialize_dataloader()
         if img_emd_translator is None:
-            self._img_emd_translator = ImageEmbeddingFilterAndNameTranslator(image_downloaddir=inputdir, fold=fold)
-
-
+            self._img_emd_translator = ImageEmbeddingFilterAndNameTranslator(image_downloaddir=inputdir,
+                                                                             fold=fold)
 
     def _initialize_model(self):
         """
 
         """
         model = class_densenet121_large_dropout(num_classes=self._num_classes,
                                                 in_channels=self._channels,
```

### Comparing `cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding.egg-info/PKG-INFO` & `cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 Metadata-Version: 2.1
 Name: cellmaps-image-embedding
-Version: 0.1.0a7
+Version: 0.1.0a8
 Summary: A tool to generate embeddings from HPA IF images
 Home-page: https://github.com/idekerlab/cellmaps_image_embedding
 Author: Ideker Lab CM4AI team
 Author-email: tools@cm4ai.org
 License: MIT license
-Description: =========================
-        cellmaps_image_embedding
-        =========================
+Description: =============================================
+        Cell Maps ImmunoFluorescent Image Embedder
+        =============================================
         
         
         .. image:: https://img.shields.io/pypi/v/cellmaps_image_embedding.svg
                 :target: https://pypi.python.org/pypi/cellmaps_image_embedding
         
         .. image:: https://img.shields.io/travis/idekerlab/cellmaps_image_embedding.svg
                 :target: https://travis-ci.com/idekerlab/cellmaps_image_embedding
         
         .. image:: https://readthedocs.org/projects/cellmaps-image-embedding/badge/?version=latest
                 :target: https://cellmaps-image-embedding.readthedocs.io/en/latest/?badge=latest
                 :alt: Documentation Status
         
         
-        A tool to generate embeddings from HPA IF images
-        
+        Generate embeddings from ImmunoFluorescent image data from `Human Protein Atlas <https://www.proteinatlas.org/>`__
+        for `Cell Maps for AI (CM4AI) <https://cm4ai.org>`__
         
         * Free software: MIT license
         * Documentation: https://cellmaps-image-embedding.readthedocs.io.
         
-        
-        
         Dependencies
         ------------
         
         * `cellmaps_utils <https://pypi.org/project/cellmaps-utils>`__
         * `tqdm <https://pypi.org/project/tqdm>`__
         * `numpy <https://pypi.org/project/numpy>`__
         * `pandas>=0.23.1 <https://pypi.org/project/pandas>`__
```

### Comparing `cellmaps_image_embedding-0.1.0a7/cellmaps_image_embedding.egg-info/SOURCES.txt` & `cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a7/docs/Makefile` & `cellmaps_image_embedding-0.1.0a8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a7/docs/cellmaps_image_embedding.rst` & `cellmaps_image_embedding-0.1.0a8/docs/cellmaps_image_embedding.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a7/docs/conf.py` & `cellmaps_image_embedding-0.1.0a8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a7/docs/installation.rst` & `cellmaps_image_embedding-0.1.0a8/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a7/docs/make.bat` & `cellmaps_image_embedding-0.1.0a8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a7/docs/newrelease.rst` & `cellmaps_image_embedding-0.1.0a8/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a7/docs/pypircfile.rst` & `cellmaps_image_embedding-0.1.0a8/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a7/docs/usage.rst` & `cellmaps_image_embedding-0.1.0a8/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a7/docs/versioningscheme.rst` & `cellmaps_image_embedding-0.1.0a8/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a7/setup.py` & `cellmaps_image_embedding-0.1.0a8/setup.py`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a7/tests/test_cellmaps_image_embeddingcmd.py` & `cellmaps_image_embedding-0.1.0a8/tests/test_cellmaps_image_embeddingcmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a7/tests/test_cellmaps_image_embeddingrunner.py` & `cellmaps_image_embedding-0.1.0a8/tests/test_cellmaps_image_embeddingrunner.py`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a7/tests/test_integration_cellmaps_image_embedding.py` & `cellmaps_image_embedding-0.1.0a8/tests/test_integration_cellmaps_image_embedding.py`

 * *Files identical despite different names*


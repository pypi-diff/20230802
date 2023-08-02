# Comparing `tmp/cellmaps_ppi_embedding-0.1.0a4.tar.gz` & `tmp/cellmaps_ppi_embedding-0.1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_ppi_embedding-0.1.0a4.tar", last modified: Mon May 22 19:40:12 2023, max compression
+gzip compressed data, was "dist/cellmaps_ppi_embedding-0.1.0a5.tar", last modified: Wed Aug  2 02:22:50 2023, max compression
```

## Comparing `cellmaps_ppi_embedding-0.1.0a4.tar` & `cellmaps_ppi_embedding-0.1.0a5.tar`

### file list

```diff
@@ -1,44 +1,51 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:40:12.765277 cellmaps_ppi_embedding-0.1.0a4/
--rw-r--r--   0 churas     (504) staff       (20)      192 2023-05-15 16:45:40.000000 cellmaps_ppi_embedding-0.1.0a4/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3707 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-15 16:45:40.000000 cellmaps_ppi_embedding-0.1.0a4/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a4/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a4/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     5779 2023-05-22 19:40:12.765393 cellmaps_ppi_embedding-0.1.0a4/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     3743 2023-05-15 16:46:17.000000 cellmaps_ppi_embedding-0.1.0a4/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:40:12.758388 cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding/
--rw-r--r--   0 churas     (504) staff       (20)      296 2023-05-22 19:36:45.000000 cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     4915 2023-05-20 00:05:39.000000 cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding/cellmaps_ppi_embeddingcmd.py
--rw-r--r--   0 churas     (504) staff       (20)      139 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding/exceptions.py
--rw-r--r--   0 churas     (504) staff       (20)    10746 2023-05-22 19:36:34.000000 cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding/runner.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:40:12.760033 cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     5779 2023-05-22 19:40:12.000000 cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)      981 2023-05-22 19:40:12.000000 cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-22 19:40:12.000000 cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-22 19:40:12.000000 cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-05-22 19:40:12.000000 cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       23 2023-05-22 19:40:12.000000 cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:40:12.764219 cellmaps_ppi_embedding-0.1.0a4/docs/
--rw-r--r--   0 churas     (504) staff       (20)      623 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/docs/Makefile
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a4/docs/authors.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     6093 2023-05-15 16:45:40.000000 cellmaps_ppi_embedding-0.1.0a4/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a4/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a4/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      290 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a4/docs/history.rst
--rw-r--r--   0 churas     (504) staff       (20)      972 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1238 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      470 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      820 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       81 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4400 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      792 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)      725 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a4/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      405 2023-05-22 19:40:12.765815 cellmaps_ppi_embedding-0.1.0a4/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     1860 2023-05-15 16:48:06.000000 cellmaps_ppi_embedding-0.1.0a4/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:40:12.765100 cellmaps_ppi_embedding-0.1.0a4/tests/
--rw-r--r--   0 churas     (504) staff       (20)       77 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/tests/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     1897 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/tests/test_cellmaps_network_embeddingcmd.py
--rw-r--r--   0 churas     (504) staff       (20)     2804 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/tests/test_cellmapsnetworkembeddingrunner.py
--rw-r--r--   0 churas     (504) staff       (20)      819 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a4/tests/test_integration_cellmaps_network_embedding.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 02:22:50.369271 cellmaps_ppi_embedding-0.1.0a5/
+-rw-r--r--   0 churas     (504) staff       (20)      299 2023-07-26 18:06:16.000000 cellmaps_ppi_embedding-0.1.0a5/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3707 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a5/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-15 16:45:40.000000 cellmaps_ppi_embedding-0.1.0a5/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a5/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a5/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     5840 2023-08-02 02:22:50.369395 cellmaps_ppi_embedding-0.1.0a5/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     3797 2023-07-26 18:06:16.000000 cellmaps_ppi_embedding-0.1.0a5/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 02:22:50.362127 cellmaps_ppi_embedding-0.1.0a5/cellmaps_ppi_embedding/
+-rw-r--r--   0 churas     (504) staff       (20)      302 2023-08-02 02:22:32.000000 cellmaps_ppi_embedding-0.1.0a5/cellmaps_ppi_embedding/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     5325 2023-08-02 02:22:32.000000 cellmaps_ppi_embedding-0.1.0a5/cellmaps_ppi_embedding/cellmaps_ppi_embeddingcmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      139 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a5/cellmaps_ppi_embedding/exceptions.py
+-rw-r--r--   0 churas     (504) staff       (20)    12418 2023-08-02 02:22:32.000000 cellmaps_ppi_embedding-0.1.0a5/cellmaps_ppi_embedding/runner.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 02:22:50.363618 cellmaps_ppi_embedding-0.1.0a5/cellmaps_ppi_embedding.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     5840 2023-08-02 02:22:50.000000 cellmaps_ppi_embedding-0.1.0a5/cellmaps_ppi_embedding.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     1116 2023-08-02 02:22:50.000000 cellmaps_ppi_embedding-0.1.0a5/cellmaps_ppi_embedding.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-08-02 02:22:50.000000 cellmaps_ppi_embedding-0.1.0a5/cellmaps_ppi_embedding.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-08-02 02:22:50.000000 cellmaps_ppi_embedding-0.1.0a5/cellmaps_ppi_embedding.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-08-02 02:22:50.000000 cellmaps_ppi_embedding-0.1.0a5/cellmaps_ppi_embedding.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       23 2023-08-02 02:22:50.000000 cellmaps_ppi_embedding-0.1.0a5/cellmaps_ppi_embedding.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 02:22:50.367526 cellmaps_ppi_embedding-0.1.0a5/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      623 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a5/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 02:22:50.358955 cellmaps_ppi_embedding-0.1.0a5/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 02:22:50.359041 cellmaps_ppi_embedding-0.1.0a5/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 02:22:50.368185 cellmaps_ppi_embedding-0.1.0a5/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_ppi_embedding-0.1.0a5/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_ppi_embedding-0.1.0a5/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_ppi_embedding-0.1.0a5/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a5/docs/authors.rst
+-rw-r--r--   0 churas     (504) staff       (20)      829 2023-05-22 23:59:49.000000 cellmaps_ppi_embedding-0.1.0a5/docs/cellmaps_ppi_embedding.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     6093 2023-05-15 16:45:40.000000 cellmaps_ppi_embedding-0.1.0a5/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a5/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a5/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      290 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a5/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a5/docs/history.rst
+-rw-r--r--   0 churas     (504) staff       (20)      734 2023-07-26 18:06:16.000000 cellmaps_ppi_embedding-0.1.0a5/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1238 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a5/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      470 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a5/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      820 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a5/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       81 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a5/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4400 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a5/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      792 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a5/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)      725 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a5/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-05-12 17:31:33.000000 cellmaps_ppi_embedding-0.1.0a5/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      405 2023-08-02 02:22:50.369863 cellmaps_ppi_embedding-0.1.0a5/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     2190 2023-07-26 18:06:16.000000 cellmaps_ppi_embedding-0.1.0a5/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 02:22:50.369051 cellmaps_ppi_embedding-0.1.0a5/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       77 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a5/tests/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     1897 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a5/tests/test_cellmaps_network_embeddingcmd.py
+-rw-r--r--   0 churas     (504) staff       (20)     3221 2023-08-02 02:22:32.000000 cellmaps_ppi_embedding-0.1.0a5/tests/test_cellmapsnetworkembeddingrunner.py
+-rw-r--r--   0 churas     (504) staff       (20)      819 2023-05-12 17:41:23.000000 cellmaps_ppi_embedding-0.1.0a5/tests/test_integration_cellmaps_network_embedding.py
```

### Comparing `cellmaps_ppi_embedding-0.1.0a4/CONTRIBUTING.rst` & `cellmaps_ppi_embedding-0.1.0a5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a4/LICENSE` & `cellmaps_ppi_embedding-0.1.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a4/PKG-INFO` & `cellmaps_ppi_embedding-0.1.0a5/cellmaps_ppi_embedding.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
-Name: cellmaps_ppi_embedding
-Version: 0.1.0a4
-Summary: A tool to generate embeddings from networks for CM4AI pipeline
+Name: cellmaps-ppi-embedding
+Version: 0.1.0a5
+Summary: A tool to generate embeddings from networks
 Home-page: https://github.com/idekerlab/cellmaps_ppi_embedding
-Author: Mayank Jain
-Author-email: maj014@ucsd.edu
+Author: Ideker Lab CM4AI team
+Author-email: tools@cm4ai.org
 License: MIT license
 Description: ==========================
-        cellmaps_ppi_embedding
+        Cell Maps PPI Embedder
         ==========================
         
         
         .. image:: https://img.shields.io/pypi/v/cellmaps_ppi_embedding.svg
                 :target: https://pypi.python.org/pypi/cellmaps_ppi_embedding
         
         .. image:: https://img.shields.io/travis/idekerlab/cellmaps_ppi_embedding.svg
@@ -20,15 +20,17 @@
         .. image:: https://readthedocs.org/projects/cellmaps-ppi-embedding/badge/?version=latest
                 :target: https://cellmaps-ppi-embedding.readthedocs.io/en/latest/?badge=latest
                 :alt: Documentation Status
         
         
         
         
-        A tool to generate embeddings from networks for CM4AI pipeline
+        Generate embeddings from Protein-Protein interaction networks used by
+        `Cell Maps for AI (CM4AI) <https://cm4ai.org>`__
+        
         
         * Free software: MIT license
         * Documentation: https://cellmaps-ppi-embedding.readthedocs.io.
         
         
         
         Dependencies
@@ -47,15 +49,15 @@
         ------------
         
         .. code-block::
         
            git clone https://github.com/idekerlab/cellmaps_ppi_embedding
            cd cellmaps_ppi_embedding
            make dist
-           pip install dist/cellmaps_ppi_embeddingcmd*whl
+           pip install dist/cellmaps_ppi_embedding*whl
         
         
         Run **make** command with no arguments to see other build/deploy options including creation of Docker image 
         
         .. code-block::
         
            make
```

### Comparing `cellmaps_ppi_embedding-0.1.0a4/README.rst` & `cellmaps_ppi_embedding-0.1.0a5/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ==========================
-cellmaps_ppi_embedding
+Cell Maps PPI Embedder
 ==========================
 
 
 .. image:: https://img.shields.io/pypi/v/cellmaps_ppi_embedding.svg
         :target: https://pypi.python.org/pypi/cellmaps_ppi_embedding
 
 .. image:: https://img.shields.io/travis/idekerlab/cellmaps_ppi_embedding.svg
@@ -12,15 +12,17 @@
 .. image:: https://readthedocs.org/projects/cellmaps-ppi-embedding/badge/?version=latest
         :target: https://cellmaps-ppi-embedding.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 
 
 
-A tool to generate embeddings from networks for CM4AI pipeline
+Generate embeddings from Protein-Protein interaction networks used by
+`Cell Maps for AI (CM4AI) <https://cm4ai.org>`__
+
 
 * Free software: MIT license
 * Documentation: https://cellmaps-ppi-embedding.readthedocs.io.
 
 
 
 Dependencies
@@ -39,15 +41,15 @@
 ------------
 
 .. code-block::
 
    git clone https://github.com/idekerlab/cellmaps_ppi_embedding
    cd cellmaps_ppi_embedding
    make dist
-   pip install dist/cellmaps_ppi_embeddingcmd*whl
+   pip install dist/cellmaps_ppi_embedding*whl
 
 
 Run **make** command with no arguments to see other build/deploy options including creation of Docker image 
 
 .. code-block::
 
    make
```

### Comparing `cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding/cellmaps_ppi_embeddingcmd.py` & `cellmaps_ppi_embedding-0.1.0a5/cellmaps_ppi_embedding/cellmaps_ppi_embeddingcmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import logging.config
 import networkx as nx
 from cellmaps_utils import logutils
 from cellmaps_utils import constants
 import cellmaps_ppi_embedding
 from cellmaps_ppi_embedding.runner import Node2VecEmbeddingGenerator
 from cellmaps_ppi_embedding.runner import CellMapsPPIEmbedder
+from cellmaps_ppi_embedding.runner import FakeEmbeddingGenerator
 
 logger = logging.getLogger(__name__)
 
 
 def _parse_arguments(desc, args):
     """
     Parses command line arguments
@@ -25,27 +26,29 @@
     :return: arguments parsed by :py:mod:`argparse`
     :rtype: :py:class:`argparse.Namespace`
     """
     parser = argparse.ArgumentParser(description=desc,
                                      formatter_class=constants.ArgParseFormatter)
     parser.add_argument('outdir', help='Output directory')
     parser.add_argument('--inputdir', required=True,
-                        help='Directory where apms_edgelist.tsv file resides')
+                        help='Directory where ppi_edgelist.tsv file resides')
     parser.add_argument('--dimensions', type=int, default=1024,
                         help='Size of embedding to generate')
     parser.add_argument('--walk_length', type=int, default=80,
                         help='Walk Length')
     parser.add_argument('--num_walks', type=int, default=10,
                         help='Num walks')
     parser.add_argument('--workers', type=int, default=8,
                         help='Number of workers')
     parser.add_argument('--p', type=int, default=2,
                         help='--p value to pass to node2vec')
     parser.add_argument('--q', type=int, default=1,
                         help='--q value to pass to node2vec')
+    parser.add_argument('--fake_embedder', action='store_true',
+                        help='If set, generate fake embedding')
     parser.add_argument('--skip_logging', action='store_true',
                         help='If set, output.log, error.log and '
                              'task_#_start/finish.json '
                              'files will not be created')
     parser.add_argument('--logconf', default=None,
                         help='Path to python logging configuration file in '
                              'this format: https://docs.python.org/3/library/'
@@ -85,23 +88,26 @@
     """.format(version=cellmaps_ppi_embedding.__version__)
     theargs = _parse_arguments(desc, args[1:])
     theargs.program = args[0]
     theargs.version = cellmaps_ppi_embedding.__version__
 
     try:
         logutils.setup_cmd_logging(theargs)
-
-        gen = Node2VecEmbeddingGenerator(nx_network=nx.read_edgelist(CellMapsPPIEmbedder.get_apms_edgelist_file(theargs.inputdir),
-                                                                     delimiter='\t'),
-                                         dimensions=theargs.dimensions,
-                                         p=theargs.p,
-                                         q=theargs.q,
-                                         walk_length=theargs.walk_length,
-                                         num_walks=theargs.num_walks,
-                                         workers=theargs.workers)
+        if theargs.fake_embedder is True:
+            gen = FakeEmbeddingGenerator(theargs.inputdir,
+                                         dimensions=theargs.dimensions)
+        else:
+            gen = Node2VecEmbeddingGenerator(nx_network=nx.read_edgelist(CellMapsPPIEmbedder.get_apms_edgelist_file(theargs.inputdir),
+                                                                         delimiter='\t'),
+                                             dimensions=theargs.dimensions,
+                                             p=theargs.p,
+                                             q=theargs.q,
+                                             walk_length=theargs.walk_length,
+                                             num_walks=theargs.num_walks,
+                                             workers=theargs.workers)
 
         return CellMapsPPIEmbedder(outdir=theargs.outdir,
                                    embedding_generator=gen,
                                    skip_logging=theargs.skip_logging,
                                    inputdir=theargs.inputdir,
                                    input_data_dict=theargs.__dict__).run()
     except Exception as e:
```

### Comparing `cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding/runner.py` & `cellmaps_ppi_embedding-0.1.0a5/cellmaps_ppi_embedding/runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 #! /usr/bin/env python
 
 import os
-
+import numpy as np
 import time
 from datetime import date
 import logging
 import csv
 import networkx as nx
 from node2vec import Node2Vec
 from cellmaps_utils import constants
 from cellmaps_utils import logutils
 from cellmaps_utils.provenance import ProvenanceUtil
+import warnings
+
 
 import cellmaps_ppi_embedding
 from cellmaps_ppi_embedding.exceptions import CellMapsPPIEmbeddingError
 
 
 logger = logging.getLogger(__name__)
 
@@ -101,14 +103,63 @@
         model = n2v_obj.fit(window=10, min_count=0, sg=1, epochs=1)
         for key in model.wv.index_to_key:
             row = [key]
             row.extend(model.wv[key].tolist())
             yield row
 
 
+class FakeEmbeddingGenerator(EmbeddingGenerator):
+    """
+    Fakes PPI embedding
+    """
+    def __init__(self, ppi_downloaddir,  dimensions=1024):
+        """
+        Constructor
+        
+        :param dimensions: Desired size of output embedding
+        :type dimensions: int
+        """
+        super().__init__(dimensions=dimensions)
+        
+        self._ppi_downloaddir = ppi_downloaddir
+        self._gene_list = self._get_gene_list()
+            
+        warnings.warn(constants.PPI_EMBEDDING_FILE +
+                      ' contains FAKE DATA!!!!\n'
+                      'You have been warned\nHave a nice day\n')
+        logger.error(constants.PPI_EMBEDDING_FILE +
+                     ' contains FAKE DATA!!!! '
+                     'You have been warned. Have a nice day')
+    
+    def _get_gene_list(self):
+        
+        ppi_gene_node_attrs_file = os.path.join(self._ppi_downloaddir, constants.PPI_GENE_NODE_ATTR_FILE)
+        gene_list = []
+
+        with open(ppi_gene_node_attrs_file, 'r') as f:
+            reader = csv.DictReader(f, delimiter='\t')
+            for row in reader:
+                gene_list.append(row['name'])
+        return gene_list
+
+    def get_next_embedding(self):
+        """
+        Generator method for getting next embedding.
+        Caller should implement with ``yield`` operator
+
+        :raises: NotImplementedError: Subclasses should implement this
+        :return: Embedding
+        :rtype: list
+        """
+        for g in self._gene_list:
+            row = [g]
+            row.extend(np.random.normal(size=self.get_dimensions())) # sample normal distribution
+            yield row
+
+
 class CellMapsPPIEmbedder(object):
     """
     Class to run algorithm
     """
     def __init__(self, outdir=None,
                  embedding_generator=None,
                  inputdir=None,
@@ -236,18 +287,18 @@
         data_dict = {'name': cellmaps_ppi_embedding.__name__ + ' output file',
                      'description': 'PPI Embedding file',
                      'data-format': 'tsv',
                      'author': cellmaps_ppi_embedding.__name__,
                      'version': cellmaps_ppi_embedding.__version__,
                      'date-published': date.today().strftime('%m-%d-%Y')}
         self._embedding_file_id = self._provenance_utils.register_dataset(self._outdir,
-                                                                          source_file=self.get_ppi_embeddding_file(),
+                                                                          source_file=self.get_ppi_embedding_file(),
                                                                           data_dict=data_dict)
 
-    def get_ppi_embeddding_file(self):
+    def get_ppi_embedding_file(self):
         """
         Gets PPI embedding file in output directory
 
         :return:
         :rtype: str
         """
         return os.path.join(self._outdir, constants.PPI_EMBEDDING_FILE)
@@ -270,15 +321,15 @@
                                           handlerprefix='cellmaps_ppi_embedding')
                 self._write_task_start_json()
 
             self._create_run_crate()
 
             self._register_software()
 
-            with open(self.get_ppi_embeddding_file(), 'w', newline='') as f:
+            with open(self.get_ppi_embedding_file(), 'w', newline='') as f:
                 writer = csv.writer(f, delimiter='\t')
                 header_line = ['']
                 header_line.extend([x for x in range(1, self._embedding_generator.get_dimensions())])
                 writer.writerow(header_line)
                 for row in self._embedding_generator.get_next_embedding():
                     writer.writerow(row)
```

### Comparing `cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding.egg-info/PKG-INFO` & `cellmaps_ppi_embedding-0.1.0a5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
-Name: cellmaps-ppi-embedding
-Version: 0.1.0a4
-Summary: A tool to generate embeddings from networks for CM4AI pipeline
+Name: cellmaps_ppi_embedding
+Version: 0.1.0a5
+Summary: A tool to generate embeddings from networks
 Home-page: https://github.com/idekerlab/cellmaps_ppi_embedding
-Author: Mayank Jain
-Author-email: maj014@ucsd.edu
+Author: Ideker Lab CM4AI team
+Author-email: tools@cm4ai.org
 License: MIT license
 Description: ==========================
-        cellmaps_ppi_embedding
+        Cell Maps PPI Embedder
         ==========================
         
         
         .. image:: https://img.shields.io/pypi/v/cellmaps_ppi_embedding.svg
                 :target: https://pypi.python.org/pypi/cellmaps_ppi_embedding
         
         .. image:: https://img.shields.io/travis/idekerlab/cellmaps_ppi_embedding.svg
@@ -20,15 +20,17 @@
         .. image:: https://readthedocs.org/projects/cellmaps-ppi-embedding/badge/?version=latest
                 :target: https://cellmaps-ppi-embedding.readthedocs.io/en/latest/?badge=latest
                 :alt: Documentation Status
         
         
         
         
-        A tool to generate embeddings from networks for CM4AI pipeline
+        Generate embeddings from Protein-Protein interaction networks used by
+        `Cell Maps for AI (CM4AI) <https://cm4ai.org>`__
+        
         
         * Free software: MIT license
         * Documentation: https://cellmaps-ppi-embedding.readthedocs.io.
         
         
         
         Dependencies
@@ -47,15 +49,15 @@
         ------------
         
         .. code-block::
         
            git clone https://github.com/idekerlab/cellmaps_ppi_embedding
            cd cellmaps_ppi_embedding
            make dist
-           pip install dist/cellmaps_ppi_embeddingcmd*whl
+           pip install dist/cellmaps_ppi_embedding*whl
         
         
         Run **make** command with no arguments to see other build/deploy options including creation of Docker image 
         
         .. code-block::
         
            make
```

### Comparing `cellmaps_ppi_embedding-0.1.0a4/cellmaps_ppi_embedding.egg-info/SOURCES.txt` & `cellmaps_ppi_embedding-0.1.0a5/cellmaps_ppi_embedding.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -14,25 +14,29 @@
 cellmaps_ppi_embedding.egg-info/SOURCES.txt
 cellmaps_ppi_embedding.egg-info/dependency_links.txt
 cellmaps_ppi_embedding.egg-info/not-zip-safe
 cellmaps_ppi_embedding.egg-info/requires.txt
 cellmaps_ppi_embedding.egg-info/top_level.txt
 docs/Makefile
 docs/authors.rst
+docs/cellmaps_ppi_embedding.rst
 docs/conf.py
 docs/contributing.rst
 docs/devbranches.rst
 docs/developer.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/integrationtesting.rst
 docs/make.bat
 docs/modules.rst
 docs/newrelease.rst
 docs/pypircfile.rst
 docs/usage.rst
 docs/versioningscheme.rst
+docs/_build/html/_static/file.png
+docs/_build/html/_static/minus.png
+docs/_build/html/_static/plus.png
 tests/__init__.py
 tests/test_cellmaps_network_embeddingcmd.py
 tests/test_cellmapsnetworkembeddingrunner.py
 tests/test_integration_cellmaps_network_embedding.py
```

### Comparing `cellmaps_ppi_embedding-0.1.0a4/docs/Makefile` & `cellmaps_ppi_embedding-0.1.0a5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a4/docs/conf.py` & `cellmaps_ppi_embedding-0.1.0a5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a4/docs/installation.rst` & `cellmaps_ppi_embedding-0.1.0a5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a4/docs/make.bat` & `cellmaps_ppi_embedding-0.1.0a5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a4/docs/newrelease.rst` & `cellmaps_ppi_embedding-0.1.0a5/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a4/docs/pypircfile.rst` & `cellmaps_ppi_embedding-0.1.0a5/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a4/docs/usage.rst` & `cellmaps_ppi_embedding-0.1.0a5/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a4/docs/versioningscheme.rst` & `cellmaps_ppi_embedding-0.1.0a5/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a4/tests/test_cellmaps_network_embeddingcmd.py` & `cellmaps_ppi_embedding-0.1.0a5/tests/test_cellmaps_network_embeddingcmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_ppi_embedding-0.1.0a4/tests/test_cellmapsnetworkembeddingrunner.py` & `cellmaps_ppi_embedding-0.1.0a5/tests/test_cellmapsnetworkembeddingrunner.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 """Tests for `cellmaps_ppi_embedding` package."""
 
 import os
 import unittest
 import tempfile
 import shutil
 import csv
+
+from cellmaps_utils.provenance import ProvenanceUtil
 from cellmaps_ppi_embedding.runner import CellMapsPPIEmbedder
 from cellmaps_ppi_embedding.runner import Node2VecEmbeddingGenerator
 from cellmaps_ppi_embedding.exceptions import CellMapsPPIEmbeddingError
 
 
 class TestCellmapsNetworkEmbeddingRunner(unittest.TestCase):
     """Tests for `cellmaps_ppi_embedding` package."""
@@ -39,17 +41,24 @@
             self.fail('Expected exception')
         except CellMapsPPIEmbeddingError as ce:
             self.assertEqual('outdir is None', str(ce))
 
     def test_run_no_edgelist(self):
         temp_dir = tempfile.mkdtemp()
         try:
+            inputdir = os.path.join(temp_dir, 'input')
+            os.makedirs(inputdir, mode=0o755)
+            prov = ProvenanceUtil()
+            prov.register_rocrate(inputdir, name='name',
+                         organization_name='org', project_name='proj',
+                         guid='12345')
             rundir = os.path.join(temp_dir, 'run')
             gen = Node2VecEmbeddingGenerator(None)
             myobj = CellMapsPPIEmbedder(outdir=rundir,
+                                        inputdir=inputdir,
                                         embedding_generator=gen)
             myobj.run()
             self.fail('Expected exception')
         except CellMapsPPIEmbeddingError as ce:
             self.assertEqual('network is None', str(ce))
         finally:
             shutil.rmtree(temp_dir)
```

### Comparing `cellmaps_ppi_embedding-0.1.0a4/tests/test_integration_cellmaps_network_embedding.py` & `cellmaps_ppi_embedding-0.1.0a5/tests/test_integration_cellmaps_network_embedding.py`

 * *Files identical despite different names*


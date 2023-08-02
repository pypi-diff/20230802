# Comparing `tmp/cellmaps_coembedding-0.1.0a4.tar.gz` & `tmp/cellmaps_coembedding-0.1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_coembedding-0.1.0a4.tar", last modified: Mon Jul 24 23:41:37 2023, max compression
+gzip compressed data, was "dist/cellmaps_coembedding-0.1.0a5.tar", last modified: Wed Aug  2 00:12:43 2023, max compression
```

## Comparing `cellmaps_coembedding-0.1.0a4.tar` & `cellmaps_coembedding-0.1.0a5.tar`

### file list

```diff
@@ -1,59 +1,58 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:41:37.893308 cellmaps_coembedding-0.1.0a4/
--rw-r--r--   0 churas     (504) staff       (20)      266 2023-06-15 20:38:12.000000 cellmaps_coembedding-0.1.0a4/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3679 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a4/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-19 18:46:09.000000 cellmaps_coembedding-0.1.0a4/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a4/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a4/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     6208 2023-07-24 23:41:37.893469 cellmaps_coembedding-0.1.0a4/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     4115 2023-07-17 23:14:29.000000 cellmaps_coembedding-0.1.0a4/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:41:37.883761 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/
--rw-r--r--   0 churas     (504) staff       (20)      336 2023-07-24 23:41:10.000000 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     6496 2023-06-15 20:38:12.000000 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/cellmaps_coembeddingcmd.py
--rw-r--r--   0 churas     (504) staff       (20)      138 2023-05-02 23:53:50.000000 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/exceptions.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:41:37.886547 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/muse_sc/
--rw-r--r--   0 churas     (504) staff       (20)    12539 2023-06-15 20:38:12.000000 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/muse_sc/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     3639 2023-06-15 20:38:12.000000 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/muse_sc/architecture.py
--rw-r--r--   0 churas     (504) staff       (20)     3697 2023-03-16 18:20:58.000000 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/muse_sc/df_utils.py
--rw-r--r--   0 churas     (504) staff       (20)     1186 2023-03-16 18:20:58.000000 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/muse_sc/file_utils.py
--rw-r--r--   0 churas     (504) staff       (20)     7854 2023-06-15 20:38:12.000000 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/muse_sc/triplet_loss.py
--rw-r--r--   0 churas     (504) staff       (20)    16118 2023-06-15 20:38:12.000000 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/runner.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:41:37.885269 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     6208 2023-07-24 23:41:37.000000 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     1372 2023-07-24 23:41:37.000000 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-07-24 23:41:37.000000 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-07-24 23:41:37.000000 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)       66 2023-07-24 23:41:37.000000 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       21 2023-07-24 23:41:37.000000 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:41:37.891114 cellmaps_coembedding-0.1.0a4/docs/
--rw-r--r--   0 churas     (504) staff       (20)      622 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a4/docs/Makefile
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:41:37.880595 cellmaps_coembedding-0.1.0a4/docs/_build/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:41:37.880680 cellmaps_coembedding-0.1.0a4/docs/_build/html/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:41:37.891855 cellmaps_coembedding-0.1.0a4/docs/_build/html/_static/
--rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_coembedding-0.1.0a4/docs/_build/html/_static/file.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_coembedding-0.1.0a4/docs/_build/html/_static/minus.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_coembedding-0.1.0a4/docs/_build/html/_static/plus.png
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a4/docs/authors.rst
--rw-r--r--   0 churas     (504) staff       (20)     1086 2023-05-19 18:14:05.000000 cellmaps_coembedding-0.1.0a4/docs/cellmaps_coembedding.muse_sc.rst
--rw-r--r--   0 churas     (504) staff       (20)      877 2023-05-19 18:14:05.000000 cellmaps_coembedding-0.1.0a4/docs/cellmaps_coembedding.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     6062 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a4/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a4/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a4/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      288 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a4/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a4/docs/history.rst
--rw-r--r--   0 churas     (504) staff       (20)      849 2023-07-17 23:14:29.000000 cellmaps_coembedding-0.1.0a4/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1216 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a4/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      460 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a4/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      819 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a4/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       79 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a4/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4376 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a4/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      790 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a4/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)      709 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a4/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a4/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      403 2023-07-24 23:41:37.894007 cellmaps_coembedding-0.1.0a4/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     2370 2023-05-19 18:48:26.000000 cellmaps_coembedding-0.1.0a4/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:41:37.893088 cellmaps_coembedding-0.1.0a4/tests/
--rw-r--r--   0 churas     (504) staff       (20)       75 2023-05-02 23:53:50.000000 cellmaps_coembedding-0.1.0a4/tests/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     2551 2023-05-09 23:51:08.000000 cellmaps_coembedding-0.1.0a4/tests/test_cellmaps_coembeddingcmd.py
--rw-r--r--   0 churas     (504) staff       (20)      911 2023-05-09 21:38:49.000000 cellmaps_coembedding-0.1.0a4/tests/test_cellmapscoembedder.py
--rw-r--r--   0 churas     (504) staff       (20)     2441 2023-05-09 23:46:41.000000 cellmaps_coembedding-0.1.0a4/tests/test_imagembeddingfilterandnametranslator.py
--rw-r--r--   0 churas     (504) staff       (20)      794 2023-05-03 00:02:48.000000 cellmaps_coembedding-0.1.0a4/tests/test_integration_cellmaps_coembedding.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 00:12:43.127183 cellmaps_coembedding-0.1.0a5/
+-rw-r--r--   0 churas     (504) staff       (20)      266 2023-06-15 20:38:12.000000 cellmaps_coembedding-0.1.0a5/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3679 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a5/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-19 18:46:09.000000 cellmaps_coembedding-0.1.0a5/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a5/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a5/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     6208 2023-08-02 00:12:43.127318 cellmaps_coembedding-0.1.0a5/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     4115 2023-07-17 23:14:29.000000 cellmaps_coembedding-0.1.0a5/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 00:12:43.116476 cellmaps_coembedding-0.1.0a5/cellmaps_coembedding/
+-rw-r--r--   0 churas     (504) staff       (20)      336 2023-08-02 00:12:18.000000 cellmaps_coembedding-0.1.0a5/cellmaps_coembedding/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     6821 2023-08-02 00:12:18.000000 cellmaps_coembedding-0.1.0a5/cellmaps_coembedding/cellmaps_coembeddingcmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      138 2023-05-02 23:53:50.000000 cellmaps_coembedding-0.1.0a5/cellmaps_coembedding/exceptions.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 00:12:43.120411 cellmaps_coembedding-0.1.0a5/cellmaps_coembedding/muse_sc/
+-rw-r--r--   0 churas     (504) staff       (20)    12539 2023-06-15 20:38:12.000000 cellmaps_coembedding-0.1.0a5/cellmaps_coembedding/muse_sc/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     3639 2023-06-15 20:38:12.000000 cellmaps_coembedding-0.1.0a5/cellmaps_coembedding/muse_sc/architecture.py
+-rw-r--r--   0 churas     (504) staff       (20)     3697 2023-03-16 18:20:58.000000 cellmaps_coembedding-0.1.0a5/cellmaps_coembedding/muse_sc/df_utils.py
+-rw-r--r--   0 churas     (504) staff       (20)     1186 2023-03-16 18:20:58.000000 cellmaps_coembedding-0.1.0a5/cellmaps_coembedding/muse_sc/file_utils.py
+-rw-r--r--   0 churas     (504) staff       (20)     7854 2023-06-15 20:38:12.000000 cellmaps_coembedding-0.1.0a5/cellmaps_coembedding/muse_sc/triplet_loss.py
+-rw-r--r--   0 churas     (504) staff       (20)    16681 2023-08-02 00:12:18.000000 cellmaps_coembedding-0.1.0a5/cellmaps_coembedding/runner.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 00:12:43.118283 cellmaps_coembedding-0.1.0a5/cellmaps_coembedding.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     6208 2023-08-02 00:12:43.000000 cellmaps_coembedding-0.1.0a5/cellmaps_coembedding.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     1321 2023-08-02 00:12:43.000000 cellmaps_coembedding-0.1.0a5/cellmaps_coembedding.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-08-02 00:12:43.000000 cellmaps_coembedding-0.1.0a5/cellmaps_coembedding.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-08-02 00:12:43.000000 cellmaps_coembedding-0.1.0a5/cellmaps_coembedding.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)       66 2023-08-02 00:12:43.000000 cellmaps_coembedding-0.1.0a5/cellmaps_coembedding.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       21 2023-08-02 00:12:43.000000 cellmaps_coembedding-0.1.0a5/cellmaps_coembedding.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 00:12:43.125381 cellmaps_coembedding-0.1.0a5/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      622 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a5/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 00:12:43.112854 cellmaps_coembedding-0.1.0a5/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 00:12:43.112926 cellmaps_coembedding-0.1.0a5/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 00:12:43.126066 cellmaps_coembedding-0.1.0a5/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_coembedding-0.1.0a5/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_coembedding-0.1.0a5/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_coembedding-0.1.0a5/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a5/docs/authors.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1086 2023-05-19 18:14:05.000000 cellmaps_coembedding-0.1.0a5/docs/cellmaps_coembedding.muse_sc.rst
+-rw-r--r--   0 churas     (504) staff       (20)      877 2023-05-19 18:14:05.000000 cellmaps_coembedding-0.1.0a5/docs/cellmaps_coembedding.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     6062 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a5/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a5/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a5/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      288 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a5/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a5/docs/history.rst
+-rw-r--r--   0 churas     (504) staff       (20)      849 2023-07-17 23:14:29.000000 cellmaps_coembedding-0.1.0a5/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1216 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a5/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      460 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a5/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      819 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a5/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       79 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a5/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4376 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a5/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      790 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a5/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)      709 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a5/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a5/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      403 2023-08-02 00:12:43.127832 cellmaps_coembedding-0.1.0a5/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     2370 2023-05-19 18:48:26.000000 cellmaps_coembedding-0.1.0a5/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 00:12:43.126984 cellmaps_coembedding-0.1.0a5/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       75 2023-05-02 23:53:50.000000 cellmaps_coembedding-0.1.0a5/tests/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     2154 2023-08-02 00:12:18.000000 cellmaps_coembedding-0.1.0a5/tests/test_cellmaps_coembeddingcmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      911 2023-05-09 21:38:49.000000 cellmaps_coembedding-0.1.0a5/tests/test_cellmapscoembedder.py
+-rw-r--r--   0 churas     (504) staff       (20)      794 2023-05-03 00:02:48.000000 cellmaps_coembedding-0.1.0a5/tests/test_integration_cellmaps_coembedding.py
```

### Comparing `cellmaps_coembedding-0.1.0a4/CONTRIBUTING.rst` & `cellmaps_coembedding-0.1.0a5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a4/LICENSE` & `cellmaps_coembedding-0.1.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a4/PKG-INFO` & `cellmaps_coembedding-0.1.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps_coembedding
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: A tool to generate coembeddings from IF image embeddings and PPI network embeddings
 Home-page: https://github.com/idekerlab/cellmaps_coembedding
 Author: Ideker Lab CM4AI team
 Author-email: tools@cm4ai.org
 License: MIT license
 Description: =====================
         Cell Maps CoEmbedder
```

### Comparing `cellmaps_coembedding-0.1.0a4/README.rst` & `cellmaps_coembedding-0.1.0a5/README.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/cellmaps_coembeddingcmd.py` & `cellmaps_coembedding-0.1.0a5/cellmaps_coembedding/cellmaps_coembeddingcmd.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,17 @@
                              'file resides')
     parser.add_argument('--latent_dimension', type=int, default=128,
                         help='Output dimension of embedding')
     parser.add_argument('--n_epochs_init', default=200, type=int,
                         help='# of init training epochs')
     parser.add_argument('--n_epochs', default=500, type=int,
                         help='# of training epochs')
-
+    parser.add_argument('--jackknife_percent', default=0.0, type=float,
+                        help='Percentage of data to withhold from training'
+                             'a value of 0.1 means to withhold 10 percent of the data')
     parser.add_argument('--fake_embedding', action='store_true',
                         help='If set, generate fake coembeddings')
     parser.add_argument('--logconf', default=None,
                         help='Path to python logging configuration file in '
                              'this format: https://docs.python.org/3/library/'
                              'logging.config.html#logging-config-fileformat '
                              'Setting this overrides -v parameter which uses '
@@ -120,14 +122,15 @@
             gen = FakeCoEmbeddingGenerator(dimensions=theargs.latent_dimension,
                                            ppi_embeddingdir=theargs.ppi_embeddingdir,
                                            image_embeddingdir=theargs.image_embeddingdir)
         else:
             gen = MuseCoEmbeddingGenerator(dimensions=theargs.latent_dimension,
                                            n_epochs=theargs.n_epochs,
                                            n_epochs_init=theargs.n_epochs_init,
+                                           jackknife_percent = theargs.jackknife_percent,
                                            outdir=os.path.abspath(theargs.outdir),
                                            ppi_embeddingdir=theargs.ppi_embeddingdir,
                                            image_embeddingdir=theargs.image_embeddingdir)
         return CellmapsCoEmbedder(outdir=theargs.outdir,
                                   inputdirs=[theargs.image_embeddingdir, theargs.ppi_embeddingdir],
                                   embedding_generator=gen,
                                   input_data_dict=theargs.__dict__).run()
```

### Comparing `cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/muse_sc/__init__.py` & `cellmaps_coembedding-0.1.0a5/cellmaps_coembedding/muse_sc/__init__.py`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/muse_sc/architecture.py` & `cellmaps_coembedding-0.1.0a5/cellmaps_coembedding/muse_sc/architecture.py`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/muse_sc/df_utils.py` & `cellmaps_coembedding-0.1.0a5/cellmaps_coembedding/muse_sc/df_utils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/muse_sc/file_utils.py` & `cellmaps_coembedding-0.1.0a5/cellmaps_coembedding/muse_sc/file_utils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/muse_sc/triplet_loss.py` & `cellmaps_coembedding-0.1.0a5/cellmaps_coembedding/muse_sc/triplet_loss.py`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/runner.py` & `cellmaps_coembedding-0.1.0a5/cellmaps_coembedding/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 import cellmaps_coembedding
 import cellmaps_coembedding.muse_sc as muse
 from cellmaps_coembedding.exceptions import CellmapsCoEmbeddingError
 
 logger = logging.getLogger(__name__)
 
 
-
 class EmbeddingGenerator(object):
     """
     Base class for implementations that generate
     network embeddings
     """
     def __init__(self, dimensions=1024,
                  ppi_embeddingdir=None,
@@ -128,37 +127,40 @@
     Generats co-embedding using MUSE
     """
     def __init__(self, dimensions=128,
                  k=10, triplet_margin=0.1, dropout=0.25, n_epochs=500,
                  n_epochs_init=200,
                  outdir=None,
                  ppi_embeddingdir=None,
-                 image_embeddingdir=None
+                 image_embeddingdir=None,
+                 jackknife_percent = 0
                 ):
         """
 
         :param dimensions:
         :param k: k nearest neighbors value used for clustering - clustering used for triplet loss
         :param triplet_margin: margin for triplet loss
         :param dropout: dropout between neural net layers
         :param n_epochs: training epochs
         :param n_epochs_init: initialization training epochs
         :param outdir:
         :param ppi_embeddingdir:
         :param image_embeddingdir:
+        :param jackknife_percent: percent of data to withhold from training
         """
         super().__init__(dimensions=dimensions,
                          ppi_embeddingdir=ppi_embeddingdir,
                          image_embeddingdir=image_embeddingdir)
         self._outdir = outdir
         self._k = k
         self.triplet_margin = triplet_margin
         self._dropout = dropout
         self._n_epochs = n_epochs
         self._n_epochs_init = n_epochs_init
+        self._jackknife_percent = jackknife_percent
 
     def get_next_embedding(self):
         """
 
         :return:
         """
         ppi_embeddings = self._get_ppi_embeddings()
@@ -176,19 +178,25 @@
 
         name_index = [x[0] for x in ppi_embeddings if x[0] in intersection_name_set]
 
         ppi_embeddings_array = np.array([np.array([float(e) for e in xi[1:]]) for xi in ppi_embeddings if xi[0] in intersection_name_set])
         image_embeddings_array = np.array([np.array([float(e) for e in xi[1:]]) for xi in image_embeddings if xi[0] in intersection_name_set])
 
         resultsdir = os.path.join(self._outdir, 'muse')
+        
+        test_subset = random.sample(list(np.arange(len(name_index))), int(self._jackknife_percent * len(name_index)))
+        if self._jackknife_percent > 0:
+            with open('{}_test_genes.txt'.format(resultsdir), 'w') as file:
+                file.write('\n'.join(np.array(name_index)[test_subset]))
 
         model, res_embedings = muse.muse_fit_predict(resultsdir=resultsdir,
                                                      data_x=ppi_embeddings_array,
                                                      data_y=image_embeddings_array,
                                                      name_index=name_index, 
+                                                     test_subset = test_subset,
                                                      latent_dim=self.get_dimensions(),
                                                      n_epochs=self._n_epochs,
                                                      n_epochs_init=self._n_epochs_init,
                                                      triplet_margin=self.triplet_margin,
                                                      k=self._k, dropout=self._dropout)
         for index, embedding in enumerate(res_embedings):
             row = [name_index[index]]
```

### Comparing `cellmaps_coembedding-0.1.0a4/cellmaps_coembedding.egg-info/PKG-INFO` & `cellmaps_coembedding-0.1.0a5/cellmaps_coembedding.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps-coembedding
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: A tool to generate coembeddings from IF image embeddings and PPI network embeddings
 Home-page: https://github.com/idekerlab/cellmaps_coembedding
 Author: Ideker Lab CM4AI team
 Author-email: tools@cm4ai.org
 License: MIT license
 Description: =====================
         Cell Maps CoEmbedder
```

### Comparing `cellmaps_coembedding-0.1.0a4/cellmaps_coembedding.egg-info/SOURCES.txt` & `cellmaps_coembedding-0.1.0a5/cellmaps_coembedding.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -41,9 +41,8 @@
 docs/versioningscheme.rst
 docs/_build/html/_static/file.png
 docs/_build/html/_static/minus.png
 docs/_build/html/_static/plus.png
 tests/__init__.py
 tests/test_cellmaps_coembeddingcmd.py
 tests/test_cellmapscoembedder.py
-tests/test_imagembeddingfilterandnametranslator.py
 tests/test_integration_cellmaps_coembedding.py
```

### Comparing `cellmaps_coembedding-0.1.0a4/docs/Makefile` & `cellmaps_coembedding-0.1.0a5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a4/docs/cellmaps_coembedding.muse_sc.rst` & `cellmaps_coembedding-0.1.0a5/docs/cellmaps_coembedding.muse_sc.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a4/docs/cellmaps_coembedding.rst` & `cellmaps_coembedding-0.1.0a5/docs/cellmaps_coembedding.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a4/docs/conf.py` & `cellmaps_coembedding-0.1.0a5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a4/docs/index.rst` & `cellmaps_coembedding-0.1.0a5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a4/docs/installation.rst` & `cellmaps_coembedding-0.1.0a5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a4/docs/make.bat` & `cellmaps_coembedding-0.1.0a5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a4/docs/newrelease.rst` & `cellmaps_coembedding-0.1.0a5/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a4/docs/pypircfile.rst` & `cellmaps_coembedding-0.1.0a5/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a4/docs/usage.rst` & `cellmaps_coembedding-0.1.0a5/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a4/docs/versioningscheme.rst` & `cellmaps_coembedding-0.1.0a5/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a4/setup.py` & `cellmaps_coembedding-0.1.0a5/setup.py`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a4/tests/test_cellmaps_coembeddingcmd.py` & `cellmaps_coembedding-0.1.0a5/tests/test_cellmaps_coembeddingcmd.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,46 +22,41 @@
 
     def test_parse_arguments(self):
         """Tests parse arguments"""
         res = cellmaps_coembeddingcmd._parse_arguments('hi', ['foo',
                                                                '--ppi_embeddingdir',
                                                                'apms',
                                                                '--image_embeddingdir',
-                                                               'image',
-                                                               '--image_downloaddir',
-                                                               'download'])
+                                                               'image'])
 
         self.assertEqual(res.verbose, 0)
         self.assertEqual(res.logconf, None)
 
         someargs = ['-vv', '--logconf', 'hi',
                     'foo',
                     '--ppi_embeddingdir',
                     'apms',
                     '--image_embeddingdir',
-                    'image', '--image_downloaddir', 'download']
+                    'image']
         res = cellmaps_coembeddingcmd._parse_arguments('hi', someargs)
 
         self.assertEqual(2, res.verbose)
         self.assertEqual('hi', res.logconf)
         self.assertEqual('foo', res.outdir)
         self.assertEqual('apms', res.ppi_embeddingdir)
         self.assertEqual('image', res.image_embeddingdir)
-        self.assertEqual('download', res.image_downloaddir)
 
     def test_main(self):
         """Tests main function"""
 
         # try where loading config is successful
         try:
             temp_dir = tempfile.mkdtemp()
             res = cellmaps_coembeddingcmd.main(['myprog.py',
-                                                 'foo',
-                                                  '--ppi_embeddingdir',
-                                                  'apms',
-                                                  '--image_embeddingdir',
-                                                  'image',
-                                                 '--image_downloaddir',
-                                                'download'])
+                                                'foo',
+                                                '--ppi_embeddingdir',
+                                                'apms',
+                                                '--image_embeddingdir',
+                                                'image'])
             self.assertEqual(2, res)
         finally:
             shutil.rmtree(temp_dir)
```

### Comparing `cellmaps_coembedding-0.1.0a4/tests/test_cellmapscoembedder.py` & `cellmaps_coembedding-0.1.0a5/tests/test_cellmapscoembedder.py`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a4/tests/test_integration_cellmaps_coembedding.py` & `cellmaps_coembedding-0.1.0a5/tests/test_integration_cellmaps_coembedding.py`

 * *Files identical despite different names*


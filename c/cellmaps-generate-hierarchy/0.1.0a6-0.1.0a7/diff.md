# Comparing `tmp/cellmaps_generate_hierarchy-0.1.0a6.tar.gz` & `tmp/cellmaps_generate_hierarchy-0.1.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_generate_hierarchy-0.1.0a6.tar", last modified: Mon Jul 17 19:17:10 2023, max compression
+gzip compressed data, was "dist/cellmaps_generate_hierarchy-0.1.0a7.tar", last modified: Wed Aug  2 00:00:08 2023, max compression
```

## Comparing `cellmaps_generate_hierarchy-0.1.0a6.tar` & `cellmaps_generate_hierarchy-0.1.0a7.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:17:10.066891 cellmaps_generate_hierarchy-0.1.0a6/
--rw-r--r--   0 churas     (504) staff       (20)      266 2023-06-12 20:22:02.000000 cellmaps_generate_hierarchy-0.1.0a6/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3761 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-19 20:13:29.000000 cellmaps_generate_hierarchy-0.1.0a6/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     6212 2023-07-17 19:17:10.067054 cellmaps_generate_hierarchy-0.1.0a6/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     4098 2023-06-12 20:22:02.000000 cellmaps_generate_hierarchy-0.1.0a6/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:17:10.056083 cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy/
--rw-r--r--   0 churas     (504) staff       (20)      341 2023-06-12 20:22:02.000000 cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     7220 2023-07-17 19:16:50.000000 cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy/cellmaps_generate_hierarchycmd.py
--rw-r--r--   0 churas     (504) staff       (20)      151 2023-05-10 16:59:50.000000 cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy/exceptions.py
--rw-r--r--   0 churas     (504) staff       (20)    20579 2023-07-17 19:16:50.000000 cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy/hierarchy.py
--rw-r--r--   0 churas     (504) staff       (20)    25885 2023-07-17 19:16:50.000000 cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy/maturehierarchy.py
--rw-r--r--   0 churas     (504) staff       (20)     3877 2023-07-17 19:16:50.000000 cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy/ppi.py
--rw-r--r--   0 churas     (504) staff       (20)    12203 2023-05-26 18:13:01.000000 cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy/runner.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:17:10.057457 cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     6212 2023-07-17 19:17:09.000000 cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     1521 2023-07-17 19:17:10.000000 cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-07-17 19:17:09.000000 cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-07-17 19:17:09.000000 cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)       62 2023-07-17 19:17:09.000000 cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-07-17 19:17:09.000000 cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:17:10.062993 cellmaps_generate_hierarchy-0.1.0a6/docs/
--rw-r--r--   0 churas     (504) staff       (20)      628 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/Makefile
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:17:10.051189 cellmaps_generate_hierarchy-0.1.0a6/docs/_build/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:17:10.051256 cellmaps_generate_hierarchy-0.1.0a6/docs/_build/html/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:17:10.063971 cellmaps_generate_hierarchy-0.1.0a6/docs/_build/html/_static/
--rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/_build/html/_static/file.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/_build/html/_static/minus.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/_build/html/_static/plus.png
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/authors.rst
--rw-r--r--   0 churas     (504) staff       (20)     1294 2023-05-22 23:59:36.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/cellmaps_generate_hierarchy.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     6155 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      295 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/history.rst
--rw-r--r--   0 churas     (504) staff       (20)     1004 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1269 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      481 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      825 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       86 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4460 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      797 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)      757 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      133 2023-07-17 19:16:50.000000 cellmaps_generate_hierarchy-0.1.0a6/pyproject.toml
--rw-r--r--   0 churas     (504) staff       (20)      410 2023-07-17 19:17:10.067602 cellmaps_generate_hierarchy-0.1.0a6/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     2335 2023-06-08 20:03:18.000000 cellmaps_generate_hierarchy-0.1.0a6/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:17:10.065823 cellmaps_generate_hierarchy-0.1.0a6/tests/
--rw-r--r--   0 churas     (504) staff       (20)       82 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/tests/__init__.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 19:17:10.066647 cellmaps_generate_hierarchy-0.1.0a6/tests/data/
--rw-r--r--   0 churas     (504) staff       (20)    10232 2023-05-10 19:56:53.000000 cellmaps_generate_hierarchy-0.1.0a6/tests/data/fake_4_node_coembedding.tsv
--rw-r--r--   0 churas     (504) staff       (20)       30 2023-05-27 00:03:19.000000 cellmaps_generate_hierarchy-0.1.0a6/tests/data/hidef_output.edges
--rw-r--r--   0 churas     (504) staff       (20)       62 2023-05-27 00:03:19.000000 cellmaps_generate_hierarchy-0.1.0a6/tests/data/hidef_output.nodes
--rw-r--r--   0 churas     (504) staff       (20)    12745 2023-07-17 19:16:50.000000 cellmaps_generate_hierarchy-0.1.0a6/tests/test_cdapshierarchygenerator.py
--rw-r--r--   0 churas     (504) staff       (20)     1840 2023-05-19 20:32:56.000000 cellmaps_generate_hierarchy-0.1.0a6/tests/test_cellmaps_generate_hierarchycmd.py
--rw-r--r--   0 churas     (504) staff       (20)      787 2023-05-11 00:02:17.000000 cellmaps_generate_hierarchy-0.1.0a6/tests/test_cellmapsgeneratehierarchy.py
--rw-r--r--   0 churas     (504) staff       (20)     1512 2023-05-10 21:34:27.000000 cellmaps_generate_hierarchy-0.1.0a6/tests/test_cosinesimilarityppigenerator.py
--rw-r--r--   0 churas     (504) staff       (20)      842 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a6/tests/test_integration_cellmaps_generate_hierarchy.py
--rw-r--r--   0 churas     (504) staff       (20)     5638 2023-07-17 19:16:50.000000 cellmaps_generate_hierarchy-0.1.0a6/tests/test_maturehierarchy.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 00:00:08.265099 cellmaps_generate_hierarchy-0.1.0a7/
+-rw-r--r--   0 churas     (504) staff       (20)      266 2023-06-12 20:22:02.000000 cellmaps_generate_hierarchy-0.1.0a7/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3761 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a7/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-19 20:13:29.000000 cellmaps_generate_hierarchy-0.1.0a7/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a7/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a7/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     6291 2023-08-02 00:00:08.265242 cellmaps_generate_hierarchy-0.1.0a7/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     4185 2023-07-26 17:54:15.000000 cellmaps_generate_hierarchy-0.1.0a7/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 00:00:08.252626 cellmaps_generate_hierarchy-0.1.0a7/cellmaps_generate_hierarchy/
+-rw-r--r--   0 churas     (504) staff       (20)      341 2023-08-01 23:59:50.000000 cellmaps_generate_hierarchy-0.1.0a7/cellmaps_generate_hierarchy/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     7317 2023-07-26 17:54:15.000000 cellmaps_generate_hierarchy-0.1.0a7/cellmaps_generate_hierarchy/cellmaps_generate_hierarchycmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      151 2023-05-10 16:59:50.000000 cellmaps_generate_hierarchy-0.1.0a7/cellmaps_generate_hierarchy/exceptions.py
+-rw-r--r--   0 churas     (504) staff       (20)    20579 2023-07-17 19:16:50.000000 cellmaps_generate_hierarchy-0.1.0a7/cellmaps_generate_hierarchy/hierarchy.py
+-rw-r--r--   0 churas     (504) staff       (20)    25885 2023-07-17 19:16:50.000000 cellmaps_generate_hierarchy-0.1.0a7/cellmaps_generate_hierarchy/maturehierarchy.py
+-rw-r--r--   0 churas     (504) staff       (20)     4374 2023-07-26 17:54:15.000000 cellmaps_generate_hierarchy-0.1.0a7/cellmaps_generate_hierarchy/ppi.py
+-rw-r--r--   0 churas     (504) staff       (20)    12536 2023-07-26 17:54:15.000000 cellmaps_generate_hierarchy-0.1.0a7/cellmaps_generate_hierarchy/runner.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 00:00:08.254752 cellmaps_generate_hierarchy-0.1.0a7/cellmaps_generate_hierarchy.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     6291 2023-08-02 00:00:08.000000 cellmaps_generate_hierarchy-0.1.0a7/cellmaps_generate_hierarchy.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     1521 2023-08-02 00:00:08.000000 cellmaps_generate_hierarchy-0.1.0a7/cellmaps_generate_hierarchy.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-08-02 00:00:08.000000 cellmaps_generate_hierarchy-0.1.0a7/cellmaps_generate_hierarchy.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-08-02 00:00:08.000000 cellmaps_generate_hierarchy-0.1.0a7/cellmaps_generate_hierarchy.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)       62 2023-08-02 00:00:08.000000 cellmaps_generate_hierarchy-0.1.0a7/cellmaps_generate_hierarchy.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-08-02 00:00:08.000000 cellmaps_generate_hierarchy-0.1.0a7/cellmaps_generate_hierarchy.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 00:00:08.261440 cellmaps_generate_hierarchy-0.1.0a7/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      628 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a7/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 00:00:08.246463 cellmaps_generate_hierarchy-0.1.0a7/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 00:00:08.246588 cellmaps_generate_hierarchy-0.1.0a7/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 00:00:08.262462 cellmaps_generate_hierarchy-0.1.0a7/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_generate_hierarchy-0.1.0a7/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_generate_hierarchy-0.1.0a7/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_generate_hierarchy-0.1.0a7/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a7/docs/authors.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1294 2023-05-22 23:59:36.000000 cellmaps_generate_hierarchy-0.1.0a7/docs/cellmaps_generate_hierarchy.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     6155 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a7/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a7/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a7/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      295 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a7/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a7/docs/history.rst
+-rw-r--r--   0 churas     (504) staff       (20)      798 2023-07-26 17:54:15.000000 cellmaps_generate_hierarchy-0.1.0a7/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1269 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a7/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      481 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a7/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      825 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a7/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       86 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a7/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4460 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a7/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      797 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a7/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)      757 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a7/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a7/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      133 2023-07-17 19:16:50.000000 cellmaps_generate_hierarchy-0.1.0a7/pyproject.toml
+-rw-r--r--   0 churas     (504) staff       (20)      410 2023-08-02 00:00:08.265754 cellmaps_generate_hierarchy-0.1.0a7/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     2335 2023-06-08 20:03:18.000000 cellmaps_generate_hierarchy-0.1.0a7/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 00:00:08.264211 cellmaps_generate_hierarchy-0.1.0a7/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       82 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a7/tests/__init__.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 00:00:08.264889 cellmaps_generate_hierarchy-0.1.0a7/tests/data/
+-rw-r--r--   0 churas     (504) staff       (20)    10232 2023-05-10 19:56:53.000000 cellmaps_generate_hierarchy-0.1.0a7/tests/data/fake_4_node_coembedding.tsv
+-rw-r--r--   0 churas     (504) staff       (20)       30 2023-05-27 00:03:19.000000 cellmaps_generate_hierarchy-0.1.0a7/tests/data/hidef_output.edges
+-rw-r--r--   0 churas     (504) staff       (20)       62 2023-05-27 00:03:19.000000 cellmaps_generate_hierarchy-0.1.0a7/tests/data/hidef_output.nodes
+-rw-r--r--   0 churas     (504) staff       (20)    12745 2023-07-17 19:16:50.000000 cellmaps_generate_hierarchy-0.1.0a7/tests/test_cdapshierarchygenerator.py
+-rw-r--r--   0 churas     (504) staff       (20)     1846 2023-07-26 17:54:15.000000 cellmaps_generate_hierarchy-0.1.0a7/tests/test_cellmaps_generate_hierarchycmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      787 2023-05-11 00:02:17.000000 cellmaps_generate_hierarchy-0.1.0a7/tests/test_cellmapsgeneratehierarchy.py
+-rw-r--r--   0 churas     (504) staff       (20)     1515 2023-07-26 17:54:15.000000 cellmaps_generate_hierarchy-0.1.0a7/tests/test_cosinesimilarityppigenerator.py
+-rw-r--r--   0 churas     (504) staff       (20)      842 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a7/tests/test_integration_cellmaps_generate_hierarchy.py
+-rw-r--r--   0 churas     (504) staff       (20)     5638 2023-07-17 19:16:50.000000 cellmaps_generate_hierarchy-0.1.0a7/tests/test_maturehierarchy.py
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a6/CONTRIBUTING.rst` & `cellmaps_generate_hierarchy-0.1.0a7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a6/LICENSE` & `cellmaps_generate_hierarchy-0.1.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a6/PKG-INFO` & `cellmaps_generate_hierarchy-0.1.0a7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: cellmaps_generate_hierarchy
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: A tool to generate hierarchies from protein to protein interaction networks
 Home-page: https://github.com/idekerlab/cellmaps_generate_hierarchy
 Author: Ideker Lab CM4AI team
 Author-email: tools@cm4ai.org
 License: MIT license
-Description: ========================
-        CM4AI Generate Hierarchy
-        ========================
+Description: =============================
+        Cell Maps Generate Hierarchy
+        =============================
         
         
         .. image:: https://img.shields.io/pypi/v/cellmaps_generate_hierarchy.svg
                 :target: https://pypi.python.org/pypi/cellmaps_generate_hierarchy
         
         .. image:: https://img.shields.io/travis/idekerlab/cellmaps_generate_hierarchy.svg
                 :target: https://travis-ci.com/idekerlab/cellmaps_generate_hierarchy
         
         .. image:: https://readthedocs.org/projects/cellmaps-generate-hierarchy/badge/?version=latest
                 :target: https://cellmaps-generate-hierarchy.readthedocs.io/en/latest/?badge=latest
                 :alt: Documentation Status
         
-        A tool to generate hierarchies from protein to protein interaction networks
+        Generates hierarchy from `Cell Maps Coembedding <https://cellmaps-coembedding.readthedocs.io/>`__
+        for `Cell Maps for AI (CM4AI) <https://cm4ai.org>`__
         
         * Free software: MIT license
         * Documentation: https://cellmaps-generate-hierarchy.readthedocs.io.
         
-        
-        
         Dependencies
         ------------
         
         * `cellmaps_utils <https://pypi.org/project/cellmaps-utils>`__
         * `tqdm <https://pypi.org/project/tqdm>`__
         * `pandas <https://pypi.org/project/pandas>`__
         * `numpy <https://pypi.org/project/numpy>`__
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a6/README.rst` & `cellmaps_generate_hierarchy-0.1.0a7/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-========================
-CM4AI Generate Hierarchy
-========================
+=============================
+Cell Maps Generate Hierarchy
+=============================
 
 
 .. image:: https://img.shields.io/pypi/v/cellmaps_generate_hierarchy.svg
         :target: https://pypi.python.org/pypi/cellmaps_generate_hierarchy
 
 .. image:: https://img.shields.io/travis/idekerlab/cellmaps_generate_hierarchy.svg
         :target: https://travis-ci.com/idekerlab/cellmaps_generate_hierarchy
 
 .. image:: https://readthedocs.org/projects/cellmaps-generate-hierarchy/badge/?version=latest
         :target: https://cellmaps-generate-hierarchy.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
-A tool to generate hierarchies from protein to protein interaction networks
+Generates hierarchy from `Cell Maps Coembedding <https://cellmaps-coembedding.readthedocs.io/>`__
+for `Cell Maps for AI (CM4AI) <https://cm4ai.org>`__
 
 * Free software: MIT license
 * Documentation: https://cellmaps-generate-hierarchy.readthedocs.io.
 
-
-
 Dependencies
 ------------
 
 * `cellmaps_utils <https://pypi.org/project/cellmaps-utils>`__
 * `tqdm <https://pypi.org/project/tqdm>`__
 * `pandas <https://pypi.org/project/pandas>`__
 * `numpy <https://pypi.org/project/numpy>`__
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy/cellmaps_generate_hierarchycmd.py` & `cellmaps_generate_hierarchy-0.1.0a7/cellmaps_generate_hierarchy/cellmaps_generate_hierarchycmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from cellmaps_generate_hierarchy.hierarchy import CDAPSHiDeFHierarchyGenerator
 from cellmaps_generate_hierarchy.maturehierarchy import HiDeFHierarchyRefiner
 from cellmaps_generate_hierarchy.runner import CellmapsGenerateHierarchy
 
 logger = logging.getLogger(__name__)
 
 
-CO_EMBEDDINGDIR='--coembedding_dir'
+CO_EMBEDDINGDIRS='--coembedding_dirs'
 
 
 def _parse_arguments(desc, args):
     """
     Parses command line arguments
 
     :param desc: description to display on command line
@@ -30,16 +30,16 @@
     :type args: list
     :return: arguments parsed by :py:mod:`argparse`
     :rtype: :py:class:`argparse.Namespace`
     """
     parser = argparse.ArgumentParser(description=desc,
                                      formatter_class=constants.ArgParseFormatter)
     parser.add_argument('outdir', help='Output directory')
-    parser.add_argument(CO_EMBEDDINGDIR, required=True,
-                        help='Directory where coembedding was run')
+    parser.add_argument(CO_EMBEDDINGDIRS, required=True, nargs="+",
+                        help='Directories where coembedding was run')
     parser.add_argument('--name',
                         help='Name of this run, needed for FAIRSCAPE. If '
                              'unset, name value from specified '
                              'by --coembedding_dir directory will be used')
     parser.add_argument('--organization_name',
                         help='Name of organization running this tool, needed '
                              'for FAIRSCAPE. If unset, organization name specified '
@@ -95,15 +95,15 @@
     :return: return value of :py:meth:`cellmaps_generate_hierarchy.runner.CellmapsGenerateHierarchy.run`
              or ``2`` if an exception is raised
     :rtype: int
     """
     desc = """
     Version {version}
 
-    Takes a coembedding file {coembedding_file} file from {coembedding_dir} directory that
+    Takes a list of coembedding file {coembedding_file} files from {coembedding_dirs} directories (corresponding to multiple folds of the same data) that
     is in TSV format and generates several interaction networks that are fed via -g flag
     to HiDeF to create a hierarchy.
     
     Format of {coembedding_file} where 1st line is header:
     
     ''\t1\t2\t3\t4\t5...1024
     GENESYMBOL\tEMBEDDING1\tEMBEDDING2...
@@ -111,38 +111,38 @@
     Example:
     
             1       2       3       4       5
     AAAS    -0.35026753     -0.1307554      -0.046265163    0.3758623       0.22126552
 
     """.format(version=cellmaps_generate_hierarchy.__version__,
                coembedding_file=constants.CO_EMBEDDING_FILE,
-               coembedding_dir=CO_EMBEDDINGDIR)
+               coembedding_dirs=', '.join(CO_EMBEDDINGDIRS))
     theargs = _parse_arguments(desc, args[1:])
     theargs.program = args[0]
     theargs.version = cellmaps_generate_hierarchy.__version__
 
     try:
         logutils.setup_cmd_logging(theargs)
         provenance = ProvenanceUtil()
-        ppigen = CosineSimilarityPPIGenerator(embeddingdir=theargs.coembedding_dir,
+        ppigen = CosineSimilarityPPIGenerator(embeddingdirs=theargs.coembedding_dirs, 
                                               cutoffs=theargs.ppi_cutoffs)
 
         refiner = HiDeFHierarchyRefiner(ci_thre=theargs.containment_threshold,
                                         ji_thre=theargs.jaccard_threshold,
                                         min_term_size=theargs.min_system_size,
                                         min_diff=theargs.min_diff,
                                         provenance_utils=provenance)
 
         hiergen = CDAPSHiDeFHierarchyGenerator(author='cellmaps_generate_hierarchy',
                                                refiner=refiner,
                                                version=cellmaps_generate_hierarchy.__version__,
                                                provenance_utils=provenance)
 
         return CellmapsGenerateHierarchy(outdir=theargs.outdir,
-                                         inputdir=theargs.coembedding_dir,
+                                         inputdirs=theargs.coembedding_dirs,
                                          ppigen=ppigen,
                                          hiergen=hiergen,
                                          input_data_dict=theargs.__dict__,
                                          provenance_utils=provenance).run()
     except Exception as e:
         logger.exception('Caught exception: ' + str(e))
         return 2
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy/hierarchy.py` & `cellmaps_generate_hierarchy-0.1.0a7/cellmaps_generate_hierarchy/hierarchy.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy/maturehierarchy.py` & `cellmaps_generate_hierarchy-0.1.0a7/cellmaps_generate_hierarchy/maturehierarchy.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy/ppi.py` & `cellmaps_generate_hierarchy-0.1.0a7/cellmaps_generate_hierarchy/ppi.py`

 * *Files 19% similar despite different names*

```diff
@@ -38,39 +38,53 @@
     .. code-block::
 
         ID # # # #
 
     Where ID is gene and #'s is embedding vector
     """
 
-    def __init__(self, embeddingdir=None,
-                 cutoffs=[0.001, 0.002, 0.003, 0.004, 0.005,
-                          0.006, 0.007, 0.008, 0.009, 0.01,
-                          0.02, 0.03, 0.04, 0.05, 0.10]):
+    def __init__(self, embeddingdirs=[],
+                 cutoffs=[0.001, 0.002, 0.003, 0.004, 0.005, 0.006, 0.007, 0.008, 0.009, 0.01, 0.02, 0.03, 0.04, 0.05, 0.10]):
         """
         Constructor
         """
         super().__init__()
-        if embeddingdir is None:
+        if embeddingdirs is None or len(embeddingdirs) < 1 :
             raise CellmapsGenerateHierarchyError('embeddingdir is None')
 
-        self._embeddingfile = os.path.join(embeddingdir,
-                                           constants.CO_EMBEDDING_FILE)
+        self._embeddingdirs = embeddingdirs
         self._cutoffs = cutoffs
 
     def _get_ppi_dataframe(self):
         """
 
         :return:
         """
-        z = pd.read_table(self._embeddingfile, sep='\t', index_col=0)
-        sim_mat = music_utils.cosine_similarity_scaled(z)
-        keep = np.triu(np.ones(sim_mat.shape)).astype(bool)
-        sim_mat = sim_mat.where(keep)
-
+        sim_mats = []
+        index = []
+        
+        for embeddingdir in self._embeddingdirs:
+            embeddingfile = os.path.join(embeddingdir,
+                                               constants.CO_EMBEDDING_FILE)
+            z = pd.read_table(embeddingfile, sep='\t', index_col=0)
+            
+            #give the same ordering
+            if len(index) == 0:
+                index = z.index.values
+            else: 
+                z = z.loc[index]
+                
+            sim_mat = music_utils.cosine_similarity_scaled(z)
+            keep = np.triu(np.ones(sim_mat.shape)).astype(bool)
+            sim_mat = sim_mat.where(keep)
+            sim_mats.append(sim_mat)
+        
+        #take mean across folds
+        sim_mat = pd.DataFrame(np.array(sim_mats).mean(axis=0), index=index, columns=index)
+        
         pairs = sim_mat.stack().reset_index().rename(columns={'level_0': constants.PPI_EDGELIST_GENEA_COL,
                                                               'level_1': constants.PPI_EDGELIST_GENEB_COL,
                                                               0: constants.WEIGHTED_PPI_EDGELIST_WEIGHT_COL})
 
         pairs = pairs[pairs[constants.PPI_EDGELIST_GENEA_COL] != pairs[constants.PPI_EDGELIST_GENEB_COL]]
         return pairs.sort_values(constants.WEIGHTED_PPI_EDGELIST_WEIGHT_COL, ascending=False)
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy/runner.py` & `cellmaps_generate_hierarchy-0.1.0a7/cellmaps_generate_hierarchy/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 class CellmapsGenerateHierarchy(object):
     """
     Runs steps necessary to create PPI from embedding and to
     generate a hierarchy
     """
     def __init__(self, outdir=None,
-                 inputdir=None,
+                 inputdirs=[],
                  ppigen=None,
                  hiergen=None,
                  name=None,
                  organization_name=None,
                  project_name=None,
                  provenance_utils=ProvenanceUtil(),
                  input_data_dict=None):
@@ -44,15 +44,15 @@
         :param project_name:
         :param provenance_utils:
         """
         logger.debug('In constructor')
         if outdir is None:
             raise CellmapsGenerateHierarchyError('outdir is None')
         self._outdir = os.path.abspath(outdir)
-        self._inputdir = inputdir
+        self._inputdirs = inputdirs
         self._start_time = int(time.time())
         self._ppigen = ppigen
         self._hiergen = hiergen
         self._name = name
         self._project_name = project_name
         self._organization_name = organization_name
         self._input_data_dict = input_data_dict
@@ -61,33 +61,34 @@
     def _create_rocrate(self):
         """
         Creates rocrate for output directory
 
         :raises CellMapsProvenanceError: If there is an error
         """
         logger.debug('Registering rocrate with FAIRSCAPE')
-        name, proj_name, org_name = self._provenance_utils.get_name_project_org_of_rocrate(self._inputdir)
+        for inputdir in self._inputdirs:
+            name, proj_name, org_name = self._provenance_utils.get_name_project_org_of_rocrate(inputdir)
 
-        if self._name is not None:
-            name = self._name
+            if self._name is not None:
+                name = self._name
 
-        if self._organization_name is not None:
-            org_name = self._organization_name
+            if self._organization_name is not None:
+                org_name = self._organization_name
 
-        if self._project_name is not None:
-            proj_name = self._project_name
-        try:
-            self._provenance_utils.register_rocrate(self._outdir,
-                                                    name=name,
-                                                    organization_name=org_name,
-                                                    project_name=proj_name)
-        except TypeError as te:
-            raise CellmapsGenerateHierarchyError('Invalid provenance: ' + str(te))
-        except KeyError as ke:
-            raise CellmapsGenerateHierarchyError('Key missing in provenance: ' + str(ke))
+            if self._project_name is not None:
+                proj_name = self._project_name
+            try:
+                self._provenance_utils.register_rocrate(self._outdir,
+                                                        name=name,
+                                                        organization_name=org_name,
+                                                        project_name=proj_name)
+            except TypeError as te:
+                raise CellmapsGenerateHierarchyError('Invalid provenance: ' + str(te))
+            except KeyError as ke:
+                raise CellmapsGenerateHierarchyError('Key missing in provenance: ' + str(ke))
 
     def _register_software(self):
         """
         Registers this tool
 
         :raises CellMapsImageEmbeddingError: If fairscape call fails
         """
@@ -101,22 +102,27 @@
 
     def _register_computation(self, generated_dataset_ids=[]):
         """
         # Todo: added in used dataset, software and what is being generated
         :return:
         """
         logger.debug('Getting id of input rocrate')
-        input_dataset_id = self._provenance_utils.get_id_of_rocrate(self._inputdir)
+        input_dataset_ids = []
+        if isinstance(self._inputdirs, list):
+            for i_dir in self._inputdirs:
+                input_dataset_ids.append(self._provenance_utils.get_id_of_rocrate(i_dir))
+        else:
+            input_dataset_ids.append(self._provenance_utils.get_id_of_rocrate(self._inputdirs))
         self._provenance_utils.register_computation(self._outdir,
                                                     name=cellmaps_generate_hierarchy.__name__ + ' computation',
                                                     run_by=str(self._provenance_utils.get_login()),
                                                     command=str(self._input_data_dict),
                                                     description='run of ' + cellmaps_generate_hierarchy.__name__,
                                                     used_software=[self._softwareid],
-                                                    used_dataset=[input_dataset_id],
+                                                    used_dataset=input_dataset_ids,
                                                     generated=generated_dataset_ids)
 
     def get_ppi_network_dest_file(self, ppi_network):
         """
         Gets the path where the PPI network should be written to
 
         :param ppi_network: PPI Network
@@ -229,15 +235,14 @@
         """
         exitcode = 99
         try:
             logger.debug('In run method')
 
             if os.path.isdir(self._outdir):
                 raise CellmapsGenerateHierarchyError(self._outdir + ' already exists')
-
             if not os.path.isdir(self._outdir):
                 os.makedirs(self._outdir, mode=0o755)
 
             logutils.setup_filelogger(outdir=self._outdir,
                                       handlerprefix='cellmaps_image_embedding')
             logutils.write_task_start_json(outdir=self._outdir,
                                            start_time=self._start_time,
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy.egg-info/PKG-INFO` & `cellmaps_generate_hierarchy-0.1.0a7/cellmaps_generate_hierarchy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: cellmaps-generate-hierarchy
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: A tool to generate hierarchies from protein to protein interaction networks
 Home-page: https://github.com/idekerlab/cellmaps_generate_hierarchy
 Author: Ideker Lab CM4AI team
 Author-email: tools@cm4ai.org
 License: MIT license
-Description: ========================
-        CM4AI Generate Hierarchy
-        ========================
+Description: =============================
+        Cell Maps Generate Hierarchy
+        =============================
         
         
         .. image:: https://img.shields.io/pypi/v/cellmaps_generate_hierarchy.svg
                 :target: https://pypi.python.org/pypi/cellmaps_generate_hierarchy
         
         .. image:: https://img.shields.io/travis/idekerlab/cellmaps_generate_hierarchy.svg
                 :target: https://travis-ci.com/idekerlab/cellmaps_generate_hierarchy
         
         .. image:: https://readthedocs.org/projects/cellmaps-generate-hierarchy/badge/?version=latest
                 :target: https://cellmaps-generate-hierarchy.readthedocs.io/en/latest/?badge=latest
                 :alt: Documentation Status
         
-        A tool to generate hierarchies from protein to protein interaction networks
+        Generates hierarchy from `Cell Maps Coembedding <https://cellmaps-coembedding.readthedocs.io/>`__
+        for `Cell Maps for AI (CM4AI) <https://cm4ai.org>`__
         
         * Free software: MIT license
         * Documentation: https://cellmaps-generate-hierarchy.readthedocs.io.
         
-        
-        
         Dependencies
         ------------
         
         * `cellmaps_utils <https://pypi.org/project/cellmaps-utils>`__
         * `tqdm <https://pypi.org/project/tqdm>`__
         * `pandas <https://pypi.org/project/pandas>`__
         * `numpy <https://pypi.org/project/numpy>`__
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a6/cellmaps_generate_hierarchy.egg-info/SOURCES.txt` & `cellmaps_generate_hierarchy-0.1.0a7/cellmaps_generate_hierarchy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a6/docs/Makefile` & `cellmaps_generate_hierarchy-0.1.0a7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a6/docs/cellmaps_generate_hierarchy.rst` & `cellmaps_generate_hierarchy-0.1.0a7/docs/cellmaps_generate_hierarchy.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a6/docs/conf.py` & `cellmaps_generate_hierarchy-0.1.0a7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a6/docs/installation.rst` & `cellmaps_generate_hierarchy-0.1.0a7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a6/docs/make.bat` & `cellmaps_generate_hierarchy-0.1.0a7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a6/docs/newrelease.rst` & `cellmaps_generate_hierarchy-0.1.0a7/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a6/docs/pypircfile.rst` & `cellmaps_generate_hierarchy-0.1.0a7/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a6/docs/usage.rst` & `cellmaps_generate_hierarchy-0.1.0a7/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a6/docs/versioningscheme.rst` & `cellmaps_generate_hierarchy-0.1.0a7/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a6/setup.py` & `cellmaps_generate_hierarchy-0.1.0a7/setup.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a6/tests/data/fake_4_node_coembedding.tsv` & `cellmaps_generate_hierarchy-0.1.0a7/tests/data/fake_4_node_coembedding.tsv`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a6/tests/test_cdapshierarchygenerator.py` & `cellmaps_generate_hierarchy-0.1.0a7/tests/test_cdapshierarchygenerator.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a6/tests/test_cellmaps_generate_hierarchycmd.py` & `cellmaps_generate_hierarchy-0.1.0a7/tests/test_cellmaps_generate_hierarchycmd.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,35 +20,35 @@
     def tearDown(self):
         """Tear down test fixtures, if any."""
 
     def test_parse_arguments(self):
         """Tests parse arguments"""
         res = cellmaps_generate_hierarchycmd._parse_arguments('hi',
                                                               ['outdir',
-                                                               '--coembedding_dir',
+                                                               '--coembedding_dirs',
                                                                'foo'])
 
         self.assertEqual('outdir', res.outdir)
-        self.assertEqual('foo', res.coembedding_dir)
+        self.assertEqual(['foo'], res.coembedding_dirs)
         self.assertEqual(0, res.verbose)
         self.assertEqual(None, res.logconf)
 
         someargs = ['outdir', '-vv', '--logconf', 'hi',
-                    '--coembedding_dir', 'blah']
+                    '--coembedding_dirs', 'blah']
         res = cellmaps_generate_hierarchycmd._parse_arguments('hi', someargs)
 
         self.assertEqual(2, res.verbose)
         self.assertEqual('hi', res.logconf)
 
     def test_main(self):
         """Tests main function"""
 
         # try where loading config is successful
         try:
             temp_dir = tempfile.mkdtemp()
             res = cellmaps_generate_hierarchycmd.main(['myprog.py',
                                                        temp_dir,
-                                                       '--coembedding_dir',
+                                                       '--coembedding_dirs',
                                                        'foo'])
             self.assertEqual(res, 2)
         finally:
             shutil.rmtree(temp_dir)
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a6/tests/test_cellmapsgeneratehierarchy.py` & `cellmaps_generate_hierarchy-0.1.0a7/tests/test_cellmapsgeneratehierarchy.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a6/tests/test_cosinesimilarityppigenerator.py` & `cellmaps_generate_hierarchy-0.1.0a7/tests/test_cosinesimilarityppigenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                             'fake_4_node_coembedding.tsv')
 
     def test_fake_five_line_coembedding(self):
         temp_dir = tempfile.mkdtemp()
         try:
             shutil.copy(self.get_fake_five_line_coembedding_file(),
                         os.path.join(temp_dir, constants.CO_EMBEDDING_FILE))
-            gen = CosineSimilarityPPIGenerator(embeddingdir=temp_dir,
+            gen = CosineSimilarityPPIGenerator(embeddingdirs=[temp_dir],
                                                cutoffs=[1.0])
 
             itr = gen.get_next_network()
             net = next(itr, None)
             self.assertEqual('cellmaps_generate_hierarchy PPI 1.0 cutoff', net.get_name())
             self.assertEqual(6, len(net.get_edges()))
             self.assertEqual(4, len(net.get_nodes()))
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a6/tests/test_integration_cellmaps_generate_hierarchy.py` & `cellmaps_generate_hierarchy-0.1.0a7/tests/test_integration_cellmaps_generate_hierarchy.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a6/tests/test_maturehierarchy.py` & `cellmaps_generate_hierarchy-0.1.0a7/tests/test_maturehierarchy.py`

 * *Files identical despite different names*


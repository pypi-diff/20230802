# Comparing `tmp/rastermap-0.9.2.tar.gz` & `tmp/rastermap-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rastermap-0.9.2.tar", last modified: Fri Jul 28 18:48:46 2023, max compression
+gzip compressed data, was "rastermap-0.9.3.tar", last modified: Wed Aug  2 13:25:26 2023, max compression
```

## Comparing `rastermap-0.9.2.tar` & `rastermap-0.9.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:48:46.114566 rastermap-0.9.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:48:46.102566 rastermap-0.9.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:48:46.106566 rastermap-0.9.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-28 18:48:33.000000 rastermap-0.9.2/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-28 18:48:33.000000 rastermap-0.9.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-28 18:48:33.000000 rastermap-0.9.2/.style.yapf
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-28 18:48:33.000000 rastermap-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17024 2023-07-28 18:48:46.114566 rastermap-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16507 2023-07-28 18:48:33.000000 rastermap-0.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-28 18:48:33.000000 rastermap-0.9.2/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-28 18:48:33.000000 rastermap-0.9.2/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:48:46.106566 rastermap-0.9.2/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-07-28 18:48:33.000000 rastermap-0.9.2/notebooks/rastermap_largescale.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-07-28 18:48:33.000000 rastermap-0.9.2/notebooks/rastermap_singleneurons.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-07-28 18:48:33.000000 rastermap-0.9.2/notebooks/rastermap_widefield.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9793 2023-07-28 18:48:33.000000 rastermap-0.9.2/notebooks/rastermap_zebrafish.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    27163 2023-07-28 18:48:33.000000 rastermap-0.9.2/notebooks/tutorial.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:48:46.110566 rastermap-0.9.2/paper/
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/fig1.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    21793 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/fig1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/fig2.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/fig2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/fig3.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/fig3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/fig4.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    20581 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/fig4.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/fig5.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/fig5.py
--rw-r--r--   0 runner    (1001) docker     (123)    14408 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/fig_splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/fig_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/other_upsampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/qrdqn.py
--rw-r--r--   0 runner    (1001) docker     (123)    17359 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/simulations.py
--rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/splitting.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:48:46.110566 rastermap-0.9.2/rastermap/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:48:46.114566 rastermap-0.9.2/rastermap/gui/
--rw-r--r--   0 runner    (1001) docker     (123)   118393 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/gui/colormaps.py
--rw-r--r--   0 runner    (1001) docker     (123)    28224 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/gui/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/gui/guiparts.py
--rw-r--r--   0 runner    (1001) docker     (123)    17531 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/gui/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/gui/menus.py
--rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/gui/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/gui/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    22028 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/rastermap.py
--rw-r--r--   0 runner    (1001) docker     (123)    14994 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:48:46.114566 rastermap-0.9.2/rastermap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17024 2023-07-28 18:48:46.000000 rastermap-0.9.2/rastermap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-28 18:48:46.000000 rastermap-0.9.2/rastermap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 18:48:46.000000 rastermap-0.9.2/rastermap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-28 18:48:46.000000 rastermap-0.9.2/rastermap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 18:48:46.000000 rastermap-0.9.2/rastermap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 18:48:46.114566 rastermap-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-28 18:48:33.000000 rastermap-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:48:46.114566 rastermap-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-28 18:48:33.000000 rastermap-0.9.2/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-28 18:48:33.000000 rastermap-0.9.2/tests/test_rastermap.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-28 18:48:33.000000 rastermap-0.9.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:25:26.782590 rastermap-0.9.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:25:26.774589 rastermap-0.9.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:25:26.778589 rastermap-0.9.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-08-02 13:25:16.000000 rastermap-0.9.3/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-02 13:25:16.000000 rastermap-0.9.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-02 13:25:16.000000 rastermap-0.9.3/.style.yapf
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-08-02 13:25:16.000000 rastermap-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17782 2023-08-02 13:25:26.782590 rastermap-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17265 2023-08-02 13:25:16.000000 rastermap-0.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-02 13:25:16.000000 rastermap-0.9.3/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-08-02 13:25:16.000000 rastermap-0.9.3/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:25:26.778589 rastermap-0.9.3/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-08-02 13:25:16.000000 rastermap-0.9.3/notebooks/rastermap_largescale.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-08-02 13:25:16.000000 rastermap-0.9.3/notebooks/rastermap_singleneurons.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-08-02 13:25:16.000000 rastermap-0.9.3/notebooks/rastermap_widefield.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9793 2023-08-02 13:25:16.000000 rastermap-0.9.3/notebooks/rastermap_zebrafish.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    27163 2023-08-02 13:25:16.000000 rastermap-0.9.3/notebooks/tutorial.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:25:26.778589 rastermap-0.9.3/paper/
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/fig1.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    21793 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/fig1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/fig2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/fig2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/fig3.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/fig3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/fig4.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20581 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/fig4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/fig5.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/fig5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14408 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/fig_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/fig_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/other_upsampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/qrdqn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17359 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/simulations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-08-02 13:25:16.000000 rastermap-0.9.3/paper/splitting.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:25:26.782590 rastermap-0.9.3/rastermap/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:25:26.782590 rastermap-0.9.3/rastermap/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)   118393 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/gui/colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28224 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/gui/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/gui/guiparts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17546 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/gui/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/gui/menus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/gui/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/gui/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22028 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/rastermap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14994 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-08-02 13:25:16.000000 rastermap-0.9.3/rastermap/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:25:26.782590 rastermap-0.9.3/rastermap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17782 2023-08-02 13:25:26.000000 rastermap-0.9.3/rastermap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-08-02 13:25:26.000000 rastermap-0.9.3/rastermap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 13:25:26.000000 rastermap-0.9.3/rastermap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-02 13:25:26.000000 rastermap-0.9.3/rastermap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-02 13:25:26.000000 rastermap-0.9.3/rastermap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 13:25:26.782590 rastermap-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-08-02 13:25:16.000000 rastermap-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:25:26.782590 rastermap-0.9.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-02 13:25:16.000000 rastermap-0.9.3/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-08-02 13:25:16.000000 rastermap-0.9.3/tests/test_rastermap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-02 13:25:16.000000 rastermap-0.9.3/tox.ini
```

### Comparing `rastermap-0.9.2/.github/workflows/test_and_deploy.yml` & `rastermap-0.9.3/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/.gitignore` & `rastermap-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/LICENSE` & `rastermap-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/PKG-INFO` & `rastermap-0.9.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: rastermap
-Version: 0.9.2
-Summary: Unsupervised clustering algorithm for 2D data (neurons by time)
-Home-page: https://github.com/MouseLand/rastermap
-Author: Marius Pachitariu and Carsen Stringer
-Author-email: carsen.stringer@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Provides-Extra: gui
-License-File: LICENSE
-
 # Rastermap
 
 ![tests](https://github.com/mouseland/rastermap/actions/workflows/test_and_deploy.yml/badge.svg)
 [![codecov](https://codecov.io/gh/MouseLand/rastermap/branch/main/graph/badge.svg?token=9FFo4zNtYP)](https://codecov.io/gh/MouseLand/rastermap)
 [![PyPI version](https://badge.fury.io/py/rastermap.svg)](https://badge.fury.io/py/rastermap)
 [![Downloads](https://pepy.tech/badge/rastermap)](https://pepy.tech/project/rastermap)
 [![Downloads](https://pepy.tech/badge/rastermap/month)](https://pepy.tech/project/rastermap)
@@ -23,25 +9,26 @@
 [![Licence: GPL v3](https://img.shields.io/github/license/MouseLand/rastermap)](https://github.com/MouseLand/rastermap/blob/main/LICENSE)
 [![Contributors](https://img.shields.io/github/contributors-anon/MouseLand/rastermap)](https://github.com/MouseLand/rastermap/graphs/contributors)
 [![repo size](https://img.shields.io/github/repo-size/MouseLand/rastermap)](https://github.com/MouseLand/rastermap/)
 [![GitHub stars](https://img.shields.io/github/stars/MouseLand/rastermap?style=social)](https://github.com/MouseLand/rastermap/)
 [![GitHub forks](https://img.shields.io/github/forks/MouseLand/rastermap?style=social)](https://github.com/MouseLand/rastermap/)
 
 
-Rastermap is a discovry algorithm for neural data. The algorithm was written by 
-Carsen Stringer and Marius Pachitariu. To learn about Rastermap, read the [paper]() or watch the [talk](). For support,  please open an [issue](https://github.com/MouseLand/rastermap/issues). Please see install instructions [below](README.md/#Installation).
+Rastermap is a discovery algorithm for neural data. The algorithm was written by Carsen Stringer and Marius Pachitariu. For support,  please open an [issue](https://github.com/MouseLand/rastermap/issues). Please see install instructions [below](README.md/#Installation). If you use Rastermap in your work, please cite the [paper](https://www.biorxiv.org/content/10.1101/2023.07.25.550571v1):
+
+Stringer C., Zhong L., Syeda A., Du F., & Pachitariu M. (2023). Rastermap: a discovery method for neural population recordings. *bioRxiv* 2023.07.25.550571; doi: https://doi.org/10.1101/2023.07.25.550571
 
 Rastermap runs in python 3.8+ and has a graphical user interface (GUI) for running it easily. Rastermap can also be run in a jupyter notebook locally or on google colab, see these demos:
 * [rastermap_largescale.ipynb](notebooks/rastermap_largescale.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_largescale.ipynb) shows how to use it with large-scale data from mouse cortex (> 200 neurons) 
 * [rastermap_singleneurons.ipynb](notebooks/rastermap_singleneurons.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_singleneurons.ipynb) shows how to use it with small to medium sized data (< 200 neurons), in this case recorded from rat hippocampus 
 * [rastermap_zebrafish.ipynb](notebooks/rastermap_zebrafish.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_zebrafish.ipynb) shows how to use it with large-scale data from zebrafish 
 * [rastermap_widefield.ipynb](notebooks/rastermap_widefield.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_widefield.ipynb) shows how to use it with widefield imaging data, or other types of datasets that are too large to fit into memory 
 * [tutorial.ipynb](notebooks/tutorial.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/tutorial.ipynb) is a guided tutorial for integrating rastermap and facemap to visualize behavioral representations 
 
-**all demo data available [here](https://osf.io/xn4cm/)**
+All demo data available [here](https://osf.io/xn4cm/).
 
 Here is what the output looks like for a segment of a mesoscope recording in a mouse during spontaneous activity (3.2Hz sampling rate), compared to random neural sorting:
 
 <img src="https://www.suite2p.org/static/images/rastermap_spont.png" width="800" alt="random sorting and rastermap sorting of spontaneous activity"/>
 
 Here is what the output looks like for a recording of wholebrain neural activity in a larval zebrafish from Chen, Mu, Hu, Kuan et al 2018 (dataset [here](https://figshare.com/articles/Whole-brain_light-sheet_imaging_data/7272617/1)). The plot on the left shows the sorted activity, and the right plot is the 2D positions of the neurons in the tissue, divided into 18 clusters according to their 1D position in the Rastermap embedding:
 
@@ -105,19 +92,36 @@
 To start using the GUI, save your data into an npy file that is just a matrix that is neurons x timepoints. Then "File > Load data matrix" and choose this file (or drag and drop your file). Next click "Run > Run rastermap" and click run. See the parameters section to learn about the parameters.
 
 The GUI will start with a highlighted region that you can drag to visualize the average activity of neurons in a given part of the plot. To draw more regions, you right-click to start a region, then right-click to end it. The neurons' activity traces then show up on the botton of the GUI, and if the neuron positions are loaded, you will see them colored by the region color. You can delete a region by holding CTRL and clicking on it. You can save the ROIs you've drawn with the "Save > Save processed data" button. They will save along with the embedding so you can reload the file with the "Load processed data" option.
 
 NOTE: If you are using suite2p "spks.npy", then the GUI will automatically use the "iscell.npy" file in the same folder to subsample your recording with the chosen neurons, and will automatically load 
 the neuron positions from the "stat.npy" file.
 
-## In a notebook
+GUI examples:
+
+zebrafish:
+
+<img src="https://www.suite2p.org/static/images/fish.gif" width="600" alt="wholebrain neural activity from a zebrafish sorted by rastermap"/>
+
+mouse sensorimotor activity:
+
+<img src="https://www.suite2p.org/static/images/spont.gif" width="600" alt="sensorimotor neural activity from a mouse sorted by rastermap"/>
 
-For this, `pip install notebook` and `pip install matpltolib`.
+rat hippocampus:
+
+<img src="https://www.suite2p.org/static/images/hippocampus.gif" width="600" alt="hippocampal neural activity from a rat sorted by rastermap"/>
+
+mouse widefield:
+
+<img src="https://www.suite2p.org/static/images/widefield.gif" width="600" alt="widefield neural activity from a mouse sorted by rastermap"/>
+
+
+## In a notebook
 
-See example notebooks for more details: [run_rastermap_largescale.ipynb](notebooks/run_rastermap_largescale.ipynb), [run_rastermap.ipynb](notebooks/run_rastermap.ipynb), and [tutorial.ipynb](notebooks/tutorial.ipynb).
+For this, `pip install notebook` and `pip install matplotlib`. See example [notebooks](notebooks/) for full examples.
 
 Short example code snippet for running rastermap:
 
 ```
 import numpy as np
 import matplotlib.pyplot as plt
 from rastermap import Rastermap, utils
```

### Comparing `rastermap-0.9.2/README.md` & `rastermap-0.9.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: rastermap
+Version: 0.9.3
+Summary: Unsupervised clustering algorithm for 2D data (neurons by time)
+Home-page: https://github.com/MouseLand/rastermap
+Author: Marius Pachitariu and Carsen Stringer
+Author-email: carsen.stringer@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+Provides-Extra: gui
+License-File: LICENSE
+
 # Rastermap
 
 ![tests](https://github.com/mouseland/rastermap/actions/workflows/test_and_deploy.yml/badge.svg)
 [![codecov](https://codecov.io/gh/MouseLand/rastermap/branch/main/graph/badge.svg?token=9FFo4zNtYP)](https://codecov.io/gh/MouseLand/rastermap)
 [![PyPI version](https://badge.fury.io/py/rastermap.svg)](https://badge.fury.io/py/rastermap)
 [![Downloads](https://pepy.tech/badge/rastermap)](https://pepy.tech/project/rastermap)
 [![Downloads](https://pepy.tech/badge/rastermap/month)](https://pepy.tech/project/rastermap)
@@ -9,25 +23,26 @@
 [![Licence: GPL v3](https://img.shields.io/github/license/MouseLand/rastermap)](https://github.com/MouseLand/rastermap/blob/main/LICENSE)
 [![Contributors](https://img.shields.io/github/contributors-anon/MouseLand/rastermap)](https://github.com/MouseLand/rastermap/graphs/contributors)
 [![repo size](https://img.shields.io/github/repo-size/MouseLand/rastermap)](https://github.com/MouseLand/rastermap/)
 [![GitHub stars](https://img.shields.io/github/stars/MouseLand/rastermap?style=social)](https://github.com/MouseLand/rastermap/)
 [![GitHub forks](https://img.shields.io/github/forks/MouseLand/rastermap?style=social)](https://github.com/MouseLand/rastermap/)
 
 
-Rastermap is a discovry algorithm for neural data. The algorithm was written by 
-Carsen Stringer and Marius Pachitariu. To learn about Rastermap, read the [paper]() or watch the [talk](). For support,  please open an [issue](https://github.com/MouseLand/rastermap/issues). Please see install instructions [below](README.md/#Installation).
+Rastermap is a discovery algorithm for neural data. The algorithm was written by Carsen Stringer and Marius Pachitariu. For support,  please open an [issue](https://github.com/MouseLand/rastermap/issues). Please see install instructions [below](README.md/#Installation). If you use Rastermap in your work, please cite the [paper](https://www.biorxiv.org/content/10.1101/2023.07.25.550571v1):
+
+Stringer C., Zhong L., Syeda A., Du F., & Pachitariu M. (2023). Rastermap: a discovery method for neural population recordings. *bioRxiv* 2023.07.25.550571; doi: https://doi.org/10.1101/2023.07.25.550571
 
 Rastermap runs in python 3.8+ and has a graphical user interface (GUI) for running it easily. Rastermap can also be run in a jupyter notebook locally or on google colab, see these demos:
 * [rastermap_largescale.ipynb](notebooks/rastermap_largescale.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_largescale.ipynb) shows how to use it with large-scale data from mouse cortex (> 200 neurons) 
 * [rastermap_singleneurons.ipynb](notebooks/rastermap_singleneurons.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_singleneurons.ipynb) shows how to use it with small to medium sized data (< 200 neurons), in this case recorded from rat hippocampus 
 * [rastermap_zebrafish.ipynb](notebooks/rastermap_zebrafish.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_zebrafish.ipynb) shows how to use it with large-scale data from zebrafish 
 * [rastermap_widefield.ipynb](notebooks/rastermap_widefield.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_widefield.ipynb) shows how to use it with widefield imaging data, or other types of datasets that are too large to fit into memory 
 * [tutorial.ipynb](notebooks/tutorial.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/tutorial.ipynb) is a guided tutorial for integrating rastermap and facemap to visualize behavioral representations 
 
-**all demo data available [here](https://osf.io/xn4cm/)**
+All demo data available [here](https://osf.io/xn4cm/).
 
 Here is what the output looks like for a segment of a mesoscope recording in a mouse during spontaneous activity (3.2Hz sampling rate), compared to random neural sorting:
 
 <img src="https://www.suite2p.org/static/images/rastermap_spont.png" width="800" alt="random sorting and rastermap sorting of spontaneous activity"/>
 
 Here is what the output looks like for a recording of wholebrain neural activity in a larval zebrafish from Chen, Mu, Hu, Kuan et al 2018 (dataset [here](https://figshare.com/articles/Whole-brain_light-sheet_imaging_data/7272617/1)). The plot on the left shows the sorted activity, and the right plot is the 2D positions of the neurons in the tissue, divided into 18 clusters according to their 1D position in the Rastermap embedding:
 
@@ -91,19 +106,36 @@
 To start using the GUI, save your data into an npy file that is just a matrix that is neurons x timepoints. Then "File > Load data matrix" and choose this file (or drag and drop your file). Next click "Run > Run rastermap" and click run. See the parameters section to learn about the parameters.
 
 The GUI will start with a highlighted region that you can drag to visualize the average activity of neurons in a given part of the plot. To draw more regions, you right-click to start a region, then right-click to end it. The neurons' activity traces then show up on the botton of the GUI, and if the neuron positions are loaded, you will see them colored by the region color. You can delete a region by holding CTRL and clicking on it. You can save the ROIs you've drawn with the "Save > Save processed data" button. They will save along with the embedding so you can reload the file with the "Load processed data" option.
 
 NOTE: If you are using suite2p "spks.npy", then the GUI will automatically use the "iscell.npy" file in the same folder to subsample your recording with the chosen neurons, and will automatically load 
 the neuron positions from the "stat.npy" file.
 
-## In a notebook
+GUI examples:
+
+zebrafish:
+
+<img src="https://www.suite2p.org/static/images/fish.gif" width="600" alt="wholebrain neural activity from a zebrafish sorted by rastermap"/>
+
+mouse sensorimotor activity:
+
+<img src="https://www.suite2p.org/static/images/spont.gif" width="600" alt="sensorimotor neural activity from a mouse sorted by rastermap"/>
 
-For this, `pip install notebook` and `pip install matpltolib`.
+rat hippocampus:
+
+<img src="https://www.suite2p.org/static/images/hippocampus.gif" width="600" alt="hippocampal neural activity from a rat sorted by rastermap"/>
+
+mouse widefield:
+
+<img src="https://www.suite2p.org/static/images/widefield.gif" width="600" alt="widefield neural activity from a mouse sorted by rastermap"/>
+
+
+## In a notebook
 
-See example notebooks for more details: [run_rastermap_largescale.ipynb](notebooks/run_rastermap_largescale.ipynb), [run_rastermap.ipynb](notebooks/run_rastermap.ipynb), and [tutorial.ipynb](notebooks/tutorial.ipynb).
+For this, `pip install notebook` and `pip install matplotlib`. See example [notebooks](notebooks/) for full examples.
 
 Short example code snippet for running rastermap:
 
 ```
 import numpy as np
 import matplotlib.pyplot as plt
 from rastermap import Rastermap, utils
```

### Comparing `rastermap-0.9.2/conftest.py` & `rastermap-0.9.3/conftest.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/notebooks/rastermap_largescale.ipynb` & `rastermap-0.9.3/notebooks/rastermap_largescale.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/notebooks/rastermap_singleneurons.ipynb` & `rastermap-0.9.3/notebooks/rastermap_singleneurons.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/notebooks/rastermap_widefield.ipynb` & `rastermap-0.9.3/notebooks/rastermap_widefield.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/notebooks/rastermap_zebrafish.ipynb` & `rastermap-0.9.3/notebooks/rastermap_zebrafish.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/notebooks/tutorial.ipynb` & `rastermap-0.9.3/notebooks/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/paper/fig1.ipynb` & `rastermap-0.9.3/paper/fig1.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/paper/fig1.py` & `rastermap-0.9.3/paper/fig1.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/paper/fig2.ipynb` & `rastermap-0.9.3/paper/fig2.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/paper/fig2.py` & `rastermap-0.9.3/paper/fig2.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/paper/fig3.ipynb` & `rastermap-0.9.3/paper/fig3.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/paper/fig3.py` & `rastermap-0.9.3/paper/fig3.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/paper/fig4.ipynb` & `rastermap-0.9.3/paper/fig4.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/paper/fig4.py` & `rastermap-0.9.3/paper/fig4.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/paper/fig5.ipynb` & `rastermap-0.9.3/paper/fig5.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/paper/fig5.py` & `rastermap-0.9.3/paper/fig5.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/paper/fig_splitting.py` & `rastermap-0.9.3/paper/fig_splitting.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/paper/fig_utils.py` & `rastermap-0.9.3/paper/fig_utils.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/paper/loaders.py` & `rastermap-0.9.3/paper/loaders.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/paper/metrics.py` & `rastermap-0.9.3/paper/metrics.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/paper/other_upsampling.py` & `rastermap-0.9.3/paper/other_upsampling.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/paper/qrdqn.py` & `rastermap-0.9.3/paper/qrdqn.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/paper/simulations.py` & `rastermap-0.9.3/paper/simulations.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/paper/splitting.ipynb` & `rastermap-0.9.3/paper/splitting.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/rastermap/__main__.py` & `rastermap-0.9.3/rastermap/__main__.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/rastermap/cluster.py` & `rastermap-0.9.3/rastermap/cluster.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/rastermap/gui/colormaps.py` & `rastermap-0.9.3/rastermap/gui/colormaps.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/rastermap/gui/gui.py` & `rastermap-0.9.3/rastermap/gui/gui.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/rastermap/gui/guiparts.py` & `rastermap-0.9.3/rastermap/gui/guiparts.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/rastermap/gui/io.py` & `rastermap-0.9.3/rastermap/gui/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             
         parent.update_status_bar(
             f"PCs of activity loaded: {Usv.shape[0]} samples by {Vsv.shape[0]} timepoints")
         
     else:
         raise ValueError("file missing keys / data")
 
-    parent.neuron_pos = xy if igood is None else xy[igood]
+    parent.neuron_pos = xy if (igood is None or xy is None) else xy[igood]
 
     parent.n_samples = (parent.sp.shape[0] if parent.sp is not None 
                         else parent.Usv.shape[0])
     parent.n_time = (parent.sp.shape[1] if parent.sp is not None 
                         else parent.Vsv.shape[0])
     parent.embedding = np.arange(0, parent.n_samples).astype(np.int64)[:, np.newaxis]
     parent.sorting = np.arange(0, parent.n_samples).astype(np.int64)
@@ -87,15 +87,14 @@
 #    
 #    fs = fsspec.filesystem("http")
 
     #X, Usv, Vsv, xy = load_activity(parent.fname)
     #_load_activity_gui(parent, X, Usv, Vsv, xy)
 
 
-
 def _load_sp(parent):
     if parent.n_samples < 100:
         smooth = 1
     elif parent.n_samples < 1000:
         smooth = 5
     else:
         smooth = int(parent.n_samples / 200)
```

### Comparing `rastermap-0.9.2/rastermap/gui/menus.py` & `rastermap-0.9.3/rastermap/gui/menus.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/rastermap/gui/run.py` & `rastermap-0.9.3/rastermap/gui/run.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/rastermap/gui/views.py` & `rastermap-0.9.3/rastermap/gui/views.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/rastermap/io.py` & `rastermap-0.9.3/rastermap/io.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/rastermap/rastermap.py` & `rastermap-0.9.3/rastermap/rastermap.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/rastermap/sort.py` & `rastermap-0.9.3/rastermap/sort.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/rastermap/svd.py` & `rastermap-0.9.3/rastermap/svd.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/rastermap/upsample.py` & `rastermap-0.9.3/rastermap/upsample.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/rastermap/utils.py` & `rastermap-0.9.3/rastermap/utils.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/rastermap.egg-info/PKG-INFO` & `rastermap-0.9.3/rastermap.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rastermap
-Version: 0.9.2
+Version: 0.9.3
 Summary: Unsupervised clustering algorithm for 2D data (neurons by time)
 Home-page: https://github.com/MouseLand/rastermap
 Author: Marius Pachitariu and Carsen Stringer
 Author-email: carsen.stringer@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -23,25 +23,26 @@
 [![Licence: GPL v3](https://img.shields.io/github/license/MouseLand/rastermap)](https://github.com/MouseLand/rastermap/blob/main/LICENSE)
 [![Contributors](https://img.shields.io/github/contributors-anon/MouseLand/rastermap)](https://github.com/MouseLand/rastermap/graphs/contributors)
 [![repo size](https://img.shields.io/github/repo-size/MouseLand/rastermap)](https://github.com/MouseLand/rastermap/)
 [![GitHub stars](https://img.shields.io/github/stars/MouseLand/rastermap?style=social)](https://github.com/MouseLand/rastermap/)
 [![GitHub forks](https://img.shields.io/github/forks/MouseLand/rastermap?style=social)](https://github.com/MouseLand/rastermap/)
 
 
-Rastermap is a discovry algorithm for neural data. The algorithm was written by 
-Carsen Stringer and Marius Pachitariu. To learn about Rastermap, read the [paper]() or watch the [talk](). For support,  please open an [issue](https://github.com/MouseLand/rastermap/issues). Please see install instructions [below](README.md/#Installation).
+Rastermap is a discovery algorithm for neural data. The algorithm was written by Carsen Stringer and Marius Pachitariu. For support,  please open an [issue](https://github.com/MouseLand/rastermap/issues). Please see install instructions [below](README.md/#Installation). If you use Rastermap in your work, please cite the [paper](https://www.biorxiv.org/content/10.1101/2023.07.25.550571v1):
+
+Stringer C., Zhong L., Syeda A., Du F., & Pachitariu M. (2023). Rastermap: a discovery method for neural population recordings. *bioRxiv* 2023.07.25.550571; doi: https://doi.org/10.1101/2023.07.25.550571
 
 Rastermap runs in python 3.8+ and has a graphical user interface (GUI) for running it easily. Rastermap can also be run in a jupyter notebook locally or on google colab, see these demos:
 * [rastermap_largescale.ipynb](notebooks/rastermap_largescale.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_largescale.ipynb) shows how to use it with large-scale data from mouse cortex (> 200 neurons) 
 * [rastermap_singleneurons.ipynb](notebooks/rastermap_singleneurons.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_singleneurons.ipynb) shows how to use it with small to medium sized data (< 200 neurons), in this case recorded from rat hippocampus 
 * [rastermap_zebrafish.ipynb](notebooks/rastermap_zebrafish.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_zebrafish.ipynb) shows how to use it with large-scale data from zebrafish 
 * [rastermap_widefield.ipynb](notebooks/rastermap_widefield.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_widefield.ipynb) shows how to use it with widefield imaging data, or other types of datasets that are too large to fit into memory 
 * [tutorial.ipynb](notebooks/tutorial.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/tutorial.ipynb) is a guided tutorial for integrating rastermap and facemap to visualize behavioral representations 
 
-**all demo data available [here](https://osf.io/xn4cm/)**
+All demo data available [here](https://osf.io/xn4cm/).
 
 Here is what the output looks like for a segment of a mesoscope recording in a mouse during spontaneous activity (3.2Hz sampling rate), compared to random neural sorting:
 
 <img src="https://www.suite2p.org/static/images/rastermap_spont.png" width="800" alt="random sorting and rastermap sorting of spontaneous activity"/>
 
 Here is what the output looks like for a recording of wholebrain neural activity in a larval zebrafish from Chen, Mu, Hu, Kuan et al 2018 (dataset [here](https://figshare.com/articles/Whole-brain_light-sheet_imaging_data/7272617/1)). The plot on the left shows the sorted activity, and the right plot is the 2D positions of the neurons in the tissue, divided into 18 clusters according to their 1D position in the Rastermap embedding:
 
@@ -105,19 +106,36 @@
 To start using the GUI, save your data into an npy file that is just a matrix that is neurons x timepoints. Then "File > Load data matrix" and choose this file (or drag and drop your file). Next click "Run > Run rastermap" and click run. See the parameters section to learn about the parameters.
 
 The GUI will start with a highlighted region that you can drag to visualize the average activity of neurons in a given part of the plot. To draw more regions, you right-click to start a region, then right-click to end it. The neurons' activity traces then show up on the botton of the GUI, and if the neuron positions are loaded, you will see them colored by the region color. You can delete a region by holding CTRL and clicking on it. You can save the ROIs you've drawn with the "Save > Save processed data" button. They will save along with the embedding so you can reload the file with the "Load processed data" option.
 
 NOTE: If you are using suite2p "spks.npy", then the GUI will automatically use the "iscell.npy" file in the same folder to subsample your recording with the chosen neurons, and will automatically load 
 the neuron positions from the "stat.npy" file.
 
-## In a notebook
+GUI examples:
+
+zebrafish:
+
+<img src="https://www.suite2p.org/static/images/fish.gif" width="600" alt="wholebrain neural activity from a zebrafish sorted by rastermap"/>
+
+mouse sensorimotor activity:
+
+<img src="https://www.suite2p.org/static/images/spont.gif" width="600" alt="sensorimotor neural activity from a mouse sorted by rastermap"/>
 
-For this, `pip install notebook` and `pip install matpltolib`.
+rat hippocampus:
+
+<img src="https://www.suite2p.org/static/images/hippocampus.gif" width="600" alt="hippocampal neural activity from a rat sorted by rastermap"/>
+
+mouse widefield:
+
+<img src="https://www.suite2p.org/static/images/widefield.gif" width="600" alt="widefield neural activity from a mouse sorted by rastermap"/>
+
+
+## In a notebook
 
-See example notebooks for more details: [run_rastermap_largescale.ipynb](notebooks/run_rastermap_largescale.ipynb), [run_rastermap.ipynb](notebooks/run_rastermap.ipynb), and [tutorial.ipynb](notebooks/tutorial.ipynb).
+For this, `pip install notebook` and `pip install matplotlib`. See example [notebooks](notebooks/) for full examples.
 
 Short example code snippet for running rastermap:
 
 ```
 import numpy as np
 import matplotlib.pyplot as plt
 from rastermap import Rastermap, utils
```

### Comparing `rastermap-0.9.2/rastermap.egg-info/SOURCES.txt` & `rastermap-0.9.3/rastermap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/setup.py` & `rastermap-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.2/tox.ini` & `rastermap-0.9.3/tox.ini`

 * *Files identical despite different names*


# Comparing `tmp/clusterX-1.0.0.dev8.tar.gz` & `tmp/clusterX-2.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/clusterX-1.0.0.dev8.tar", last modified: Fri Feb 15 19:17:23 2019, max compression
+gzip compressed data, was "clusterX-2.1.0rc1.tar", last modified: Wed Aug  2 08:55:17 2023, max compression
```

## Comparing `clusterX-1.0.0.dev8.tar` & `clusterX-2.1.0rc1.tar`

### file list

```diff
@@ -1,78 +1,77 @@
-drwxr-xr-x   0 sr         (501) staff       (20)        0 2019-02-15 19:17:23.000000 clusterX-1.0.0.dev8/
--rw-r--r--   0 sr         (501) staff       (20)      435 2019-02-15 19:17:23.000000 clusterX-1.0.0.dev8/PKG-INFO
--rw-r--r--   0 sr         (501) staff       (20)       60 2018-04-03 11:26:47.000000 clusterX-1.0.0.dev8/MANIFEST.in
--rw-r--r--   0 sr         (501) staff       (20)    11477 2019-02-15 16:13:21.000000 clusterX-1.0.0.dev8/COPYING
--rw-r--r--   0 sr         (501) staff       (20)      709 2019-02-15 19:17:20.000000 clusterX-1.0.0.dev8/setup.py
--rw-r--r--   0 sr         (501) staff       (20)       38 2019-02-15 19:17:23.000000 clusterX-1.0.0.dev8/setup.cfg
-drwxr-xr-x   0 sr         (501) staff       (20)        0 2019-02-15 19:17:22.000000 clusterX-1.0.0.dev8/clusterx/
--rw-r--r--   0 sr         (501) staff       (20)     3032 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/symmetry.py
--rw-r--r--   0 sr         (501) staff       (20)    14412 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/nested_sampling.py
--rw-r--r--   0 sr         (501) staff       (20)    15646 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/clusters_selector_with_splitbregman.py
--rw-r--r--   0 sr         (501) staff       (20)     2283 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/lattices.py
--rw-r--r--   0 sr         (501) staff       (20)     1360 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/config.py
-drwxr-xr-x   0 sr         (501) staff       (20)        0 2019-02-15 19:17:23.000000 clusterX-1.0.0.dev8/clusterx/test/
--rw-r--r--   0 sr         (501) staff       (20)    11514 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/test/test_cluster_orbit.py
--rw-r--r--   0 sr         (501) staff       (20)     2120 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/test/test_concentration.py
--rw-r--r--   0 sr         (501) staff       (20)     2925 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/test/test_emt2_calculator.py
--rw-r--r--   0 sr         (501) staff       (20)     7405 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/test/test_cluster_expansion.py
--rw-r--r--   0 sr         (501) staff       (20)     3044 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/test/test_clathrate_mc.py
--rw-r--r--   0 sr         (501) staff       (20)     3994 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/test/test_lattice_representation.py
--rw-r--r--   0 sr         (501) staff       (20)     7148 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/test/test_clusters_selector.py
--rw-r--r--   0 sr         (501) staff       (20)     1491 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/test/test_get_all_hnf.py
--rw-r--r--   0 sr         (501) staff       (20)      434 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/test/__init__.py
--rw-r--r--   0 sr         (501) staff       (20)     1418 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/test/test_is_nary.py
--rw-r--r--   0 sr         (501) staff       (20)     8623 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/test/test_parent_lattice_creation.py
--rw-r--r--   0 sr         (501) staff       (20)     5663 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/test/test_cluster_selector_split_bregman.py
--rw-r--r--   0 sr         (501) staff       (20)     7606 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/test/test_clusters_selector_lasso.py
--rw-r--r--   0 sr         (501) staff       (20)     2199 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/test/test_cluster.py
--rw-r--r--   0 sr         (501) staff       (20)    10725 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/test/_test_nested_sampling.py
--rw-r--r--   0 sr         (501) staff       (20)     5390 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/test/test_cluster_correlations.py
--rw-r--r--   0 sr         (501) staff       (20)     3866 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/test/test_get_unique_supercells.py
--rw-r--r--   0 sr         (501) staff       (20)     7381 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/test/test_structure_selector.py
--rw-r--r--   0 sr         (501) staff       (20)    15530 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/test/test_metropolis.py
--rw-r--r--   0 sr         (501) staff       (20)    10332 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/test/test_clusters_generation.py
--rw-r--r--   0 sr         (501) staff       (20)     2243 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/test/test_folders.py
--rw-r--r--   0 sr         (501) staff       (20)     9646 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/super_cell.py
--rw-r--r--   0 sr         (501) staff       (20)    11069 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/structure_selector.py
-drwxr-xr-x   0 sr         (501) staff       (20)        0 2019-02-15 19:17:23.000000 clusterX-1.0.0.dev8/clusterx/clusters/
--rw-r--r--   0 sr         (501) staff       (20)    34956 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/clusters/clusters_pool.py
--rw-r--r--   0 sr         (501) staff       (20)        0 2019-02-15 18:19:42.000000 clusterX-1.0.0.dev8/clusterx/clusters/__init__.py
--rw-r--r--   0 sr         (501) staff       (20)    10275 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/clusters/cluster.py
-drwxr-xr-x   0 sr         (501) staff       (20)        0 2019-02-15 19:17:23.000000 clusterX-1.0.0.dev8/clusterx/io/
--rw-r--r--   0 sr         (501) staff       (20)     1393 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/io/atat.py
--rw-r--r--   0 sr         (501) staff       (20)      208 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/io/__init__.py
--rw-r--r--   0 sr         (501) staff       (20)      484 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/io/formats.py
--rw-r--r--   0 sr         (501) staff       (20)    20026 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/parent_lattice.py
--rw-r--r--   0 sr         (501) staff       (20)      626 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/__init__.py
--rw-r--r--   0 sr         (501) staff       (20)    21830 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/monte_carlo.py
--rw-r--r--   0 sr         (501) staff       (20)    27831 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/structures_set.py
-drwxr-xr-x   0 sr         (501) staff       (20)        0 2019-02-15 19:17:23.000000 clusterX-1.0.0.dev8/clusterx/cli/
--rw-r--r--   0 sr         (501) staff       (20)      208 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/cli/__init__.py
--rw-r--r--   0 sr         (501) staff       (20)      914 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/cli/test.py
--rw-r--r--   0 sr         (501) staff       (20)     1251 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/cli/spacegroup.py
--rw-r--r--   0 sr         (501) staff       (20)     1303 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/cli/plot_clusters.py
--rw-r--r--   0 sr         (501) staff       (20)      670 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/cli/main.py
--rw-r--r--   0 sr         (501) staff       (20)     1956 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/cli/commands.py
--rw-r--r--   0 sr         (501) staff       (20)    14558 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/visualization.py
--rw-r--r--   0 sr         (501) staff       (20)    14783 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/model.py
--rw-r--r--   0 sr         (501) staff       (20)    31151 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/utils.py
-drwxr-xr-x   0 sr         (501) staff       (20)        0 2019-02-15 19:17:23.000000 clusterX-1.0.0.dev8/clusterx/estimators/
--rw-r--r--   0 sr         (501) staff       (20)     4597 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/estimators/split_bregman.py
--rw-r--r--   0 sr         (501) staff       (20)        0 2019-02-15 18:19:59.000000 clusterX-1.0.0.dev8/clusterx/estimators/__init__.py
--rw-r--r--   0 sr         (501) staff       (20)      962 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/estimators/estimator_factory.py
-drwxr-xr-x   0 sr         (501) staff       (20)        0 2019-02-15 19:17:22.000000 clusterX-1.0.0.dev8/clusterx/calculators/
--rw-r--r--   0 sr         (501) staff       (20)      294 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/calculators/__init__.py
--rw-r--r--   0 sr         (501) staff       (20)     2125 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/calculators/emt.py
--rw-r--r--   0 sr         (501) staff       (20)     8973 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/structure.py
--rw-r--r--   0 sr         (501) staff       (20)    11980 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/correlations.py
--rw-r--r--   0 sr         (501) staff       (20)    12187 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/clusters_selector.py
--rw-r--r--   0 sr         (501) staff       (20)      352 2019-02-15 16:53:25.000000 clusterX-1.0.0.dev8/clusterx/cross_validation.py
--rw-r--r--   0 sr         (501) staff       (20)      219 2019-02-15 16:15:55.000000 clusterX-1.0.0.dev8/README.rst
-drwxr-xr-x   0 sr         (501) staff       (20)        0 2019-02-15 19:17:22.000000 clusterX-1.0.0.dev8/clusterX.egg-info/
--rw-r--r--   0 sr         (501) staff       (20)      435 2019-02-15 19:17:22.000000 clusterX-1.0.0.dev8/clusterX.egg-info/PKG-INFO
--rw-r--r--   0 sr         (501) staff       (20)     1991 2019-02-15 19:17:22.000000 clusterX-1.0.0.dev8/clusterX.egg-info/SOURCES.txt
--rw-r--r--   0 sr         (501) staff       (20)       49 2019-02-15 19:17:22.000000 clusterX-1.0.0.dev8/clusterX.egg-info/entry_points.txt
--rw-r--r--   0 sr         (501) staff       (20)       79 2019-02-15 19:17:22.000000 clusterX-1.0.0.dev8/clusterX.egg-info/requires.txt
--rw-r--r--   0 sr         (501) staff       (20)        9 2019-02-15 19:17:22.000000 clusterX-1.0.0.dev8/clusterX.egg-info/top_level.txt
--rw-r--r--   0 sr         (501) staff       (20)        1 2019-02-15 19:17:22.000000 clusterX-1.0.0.dev8/clusterX.egg-info/dependency_links.txt
--rw-r--r--   0 sr         (501) staff       (20)    11477 2019-02-15 16:12:01.000000 clusterX-1.0.0.dev8/LICENSE.txt
+drwxr-xr-x   0 sr         (501) staff       (20)        0 2023-08-02 08:55:17.264779 clusterX-2.1.0rc1/
+-rw-r--r--   0 sr         (501) staff       (20)    11477 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/COPYING
+-rw-r--r--   0 sr         (501) staff       (20)    11477 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/LICENSE.txt
+-rw-r--r--   0 sr         (501) staff       (20)       60 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/MANIFEST.in
+-rw-r--r--   0 sr         (501) staff       (20)      442 2023-08-02 08:55:17.264555 clusterX-2.1.0rc1/PKG-INFO
+-rw-r--r--   0 sr         (501) staff       (20)      219 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/README.rst
+drwxr-xr-x   0 sr         (501) staff       (20)        0 2023-08-02 08:55:17.234489 clusterX-2.1.0rc1/clusterX.egg-info/
+-rw-r--r--   0 sr         (501) staff       (20)      442 2023-08-02 08:55:17.000000 clusterX-2.1.0rc1/clusterX.egg-info/PKG-INFO
+-rw-r--r--   0 sr         (501) staff       (20)     1938 2023-08-02 08:55:17.000000 clusterX-2.1.0rc1/clusterX.egg-info/SOURCES.txt
+-rw-r--r--   0 sr         (501) staff       (20)        1 2023-08-02 08:55:17.000000 clusterX-2.1.0rc1/clusterX.egg-info/dependency_links.txt
+-rw-r--r--   0 sr         (501) staff       (20)       48 2023-08-02 08:55:17.000000 clusterX-2.1.0rc1/clusterX.egg-info/entry_points.txt
+-rw-r--r--   0 sr         (501) staff       (20)      101 2023-08-02 08:55:17.000000 clusterX-2.1.0rc1/clusterX.egg-info/requires.txt
+-rw-r--r--   0 sr         (501) staff       (20)        9 2023-08-02 08:55:17.000000 clusterX-2.1.0rc1/clusterX.egg-info/top_level.txt
+drwxr-xr-x   0 sr         (501) staff       (20)        0 2023-08-02 08:55:17.240407 clusterX-2.1.0rc1/clusterx/
+-rw-r--r--   0 sr         (501) staff       (20)      626 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/__init__.py
+drwxr-xr-x   0 sr         (501) staff       (20)        0 2023-08-02 08:55:17.240983 clusterX-2.1.0rc1/clusterx/calculators/
+-rw-r--r--   0 sr         (501) staff       (20)      294 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/calculators/__init__.py
+-rw-r--r--   0 sr         (501) staff       (20)     2270 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/calculators/emt.py
+drwxr-xr-x   0 sr         (501) staff       (20)        0 2023-08-02 08:55:17.251721 clusterX-2.1.0rc1/clusterx/cli/
+-rw-r--r--   0 sr         (501) staff       (20)      208 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/cli/__init__.py
+-rw-r--r--   0 sr         (501) staff       (20)     1648 2023-05-12 15:03:35.000000 clusterX-2.1.0rc1/clusterx/cli/commands.py
+-rw-r--r--   0 sr         (501) staff       (20)      670 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/cli/main.py
+-rw-r--r--   0 sr         (501) staff       (20)     1303 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/cli/plot_clusters.py
+-rw-r--r--   0 sr         (501) staff       (20)     1251 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/cli/spacegroup.py
+-rw-r--r--   0 sr         (501) staff       (20)     1068 2023-02-20 09:42:30.000000 clusterX-2.1.0rc1/clusterx/cli/test.py
+drwxr-xr-x   0 sr         (501) staff       (20)        0 2023-08-02 08:55:17.257886 clusterX-2.1.0rc1/clusterx/clusters/
+-rw-r--r--   0 sr         (501) staff       (20)        0 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/clusters/__init__.py
+-rw-r--r--   0 sr         (501) staff       (20)     9764 2023-05-09 10:16:28.000000 clusterX-2.1.0rc1/clusterx/clusters/cluster.py
+-rw-r--r--   0 sr         (501) staff       (20)    62837 2023-08-01 14:57:17.000000 clusterX-2.1.0rc1/clusterx/clusters/clusters_pool.py
+-rw-r--r--   0 sr         (501) staff       (20)    25723 2023-08-01 15:24:59.000000 clusterX-2.1.0rc1/clusterx/clusters_selector.py
+-rw-r--r--   0 sr         (501) staff       (20)     1360 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/config.py
+-rw-r--r--   0 sr         (501) staff       (20)    19100 2023-08-01 21:47:18.000000 clusterX-2.1.0rc1/clusterx/correlations.py
+-rw-r--r--   0 sr         (501) staff       (20)      352 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/cross_validation.py
+-rw-r--r--   0 sr         (501) staff       (20)    13889 2023-07-13 19:27:18.000000 clusterX-2.1.0rc1/clusterx/derivative_structures.py
+drwxr-xr-x   0 sr         (501) staff       (20)        0 2023-08-02 08:55:17.258622 clusterX-2.1.0rc1/clusterx/estimators/
+-rw-r--r--   0 sr         (501) staff       (20)        0 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/estimators/__init__.py
+-rw-r--r--   0 sr         (501) staff       (20)     2984 2023-04-19 22:26:52.000000 clusterX-2.1.0rc1/clusterx/estimators/estimator_factory.py
+drwxr-xr-x   0 sr         (501) staff       (20)        0 2023-08-02 08:55:17.259427 clusterX-2.1.0rc1/clusterx/io/
+-rw-r--r--   0 sr         (501) staff       (20)      208 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/io/__init__.py
+-rw-r--r--   0 sr         (501) staff       (20)     1393 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/io/atat.py
+-rw-r--r--   0 sr         (501) staff       (20)      484 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/io/formats.py
+-rw-r--r--   0 sr         (501) staff       (20)     2283 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/lattices.py
+-rw-r--r--   0 sr         (501) staff       (20)    27785 2023-08-01 21:28:28.000000 clusterX-2.1.0rc1/clusterx/model.py
+-rw-r--r--   0 sr         (501) staff       (20)    25400 2023-06-05 13:52:00.000000 clusterX-2.1.0rc1/clusterx/parent_lattice.py
+-rw-r--r--   0 sr         (501) staff       (20)    14639 2023-05-20 07:55:32.000000 clusterX-2.1.0rc1/clusterx/structure.py
+-rw-r--r--   0 sr         (501) staff       (20)    11069 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/structure_selector.py
+-rw-r--r--   0 sr         (501) staff       (20)    35864 2023-06-29 08:23:54.000000 clusterX-2.1.0rc1/clusterx/structures_set.py
+-rw-r--r--   0 sr         (501) staff       (20)    21924 2023-04-24 21:21:23.000000 clusterX-2.1.0rc1/clusterx/super_cell.py
+-rw-r--r--   0 sr         (501) staff       (20)     3653 2023-03-24 12:44:22.000000 clusterX-2.1.0rc1/clusterx/symmetry.py
+drwxr-xr-x   0 sr         (501) staff       (20)        0 2023-08-02 08:55:17.264294 clusterX-2.1.0rc1/clusterx/test/
+-rw-r--r--   0 sr         (501) staff       (20)      434 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/__init__.py
+-rw-r--r--   0 sr         (501) staff       (20)     3071 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_clathrate_mc.py
+-rw-r--r--   0 sr         (501) staff       (20)     2315 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_cluster.py
+-rw-r--r--   0 sr         (501) staff       (20)     5390 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_cluster_correlations.py
+-rw-r--r--   0 sr         (501) staff       (20)     7527 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_cluster_expansion.py
+-rw-r--r--   0 sr         (501) staff       (20)    14654 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_cluster_orbit.py
+-rw-r--r--   0 sr         (501) staff       (20)    12876 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_cluster_orbit2.py
+-rw-r--r--   0 sr         (501) staff       (20)    13813 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_clusters_generation.py
+-rw-r--r--   0 sr         (501) staff       (20)     7628 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_clusters_selector.py
+-rw-r--r--   0 sr         (501) staff       (20)     7744 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_clusters_selector_lasso.py
+-rw-r--r--   0 sr         (501) staff       (20)     2132 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_concentration.py
+-rw-r--r--   0 sr         (501) staff       (20)     2926 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_emt2_calculator.py
+-rw-r--r--   0 sr         (501) staff       (20)     2346 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_folders.py
+-rw-r--r--   0 sr         (501) staff       (20)     1491 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_get_all_hnf.py
+-rw-r--r--   0 sr         (501) staff       (20)     3954 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_get_unique_supercells.py
+-rw-r--r--   0 sr         (501) staff       (20)     1418 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_is_nary.py
+-rw-r--r--   0 sr         (501) staff       (20)     3994 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_lattice_representation.py
+-rw-r--r--   0 sr         (501) staff       (20)    23113 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_metropolis.py
+-rw-r--r--   0 sr         (501) staff       (20)     8623 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_parent_lattice_creation.py
+-rw-r--r--   0 sr         (501) staff       (20)     4577 2023-02-16 09:24:07.000000 clusterX-2.1.0rc1/clusterx/test/test_predict_swap.py
+-rw-r--r--   0 sr         (501) staff       (20)     7625 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_structure_selector.py
+-rw-r--r--   0 sr         (501) staff       (20)     1834 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_structures_set.py
+-rw-r--r--   0 sr         (501) staff       (20)     5713 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_wanglandau.py
+-rw-r--r--   0 sr         (501) staff       (20)    40776 2023-07-13 13:01:52.000000 clusterX-2.1.0rc1/clusterx/utils.py
+-rw-r--r--   0 sr         (501) staff       (20)    26128 2023-08-01 16:48:54.000000 clusterX-2.1.0rc1/clusterx/visualization.py
+-rw-r--r--   0 sr         (501) staff       (20)       38 2023-08-02 08:55:17.264830 clusterX-2.1.0rc1/setup.cfg
+-rw-r--r--   0 sr         (501) staff       (20)      735 2023-08-02 08:50:16.000000 clusterX-2.1.0rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `clusterX-1.0.0.dev8/COPYING` & `clusterX-2.1.0rc1/COPYING`

 * *Files identical despite different names*

### Comparing `clusterX-1.0.0.dev8/setup.py` & `clusterX-2.1.0rc1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(name='clusterX',
-      version='1.0.0.dev8',
+      version='2.1.0.rc1',
       description='CELL (aka clusterX) is a python package for building Cluster Expansion models of simple and complex alloys and performing thermodynamical analyses of materials.',
       url='http://sol.physik.hu-berlin.de/cell/',
       author='CELL Developers',
       author_email='srigamonti@physik.hu-berlin.de',
       license='http://www.apache.org/licenses/LICENSE-2.0',
       packages=find_packages(),
-      install_requires=['numpy', 'scipy', 'sklearn', 'matplotlib','ase','plac','pytest','spglib','sympy','nglview','ipywidgets'],
+      install_requires=['numpy', 'scipy', 'scikit-learn', 'matplotlib','ase','plac','pytest','spglib','sympy','nglview','ipywidgets','pytest-html', 'tqdm'],
       entry_points={'console_scripts': ['cell=clusterx.cli.main:main']}
 )
```

### Comparing `clusterX-1.0.0.dev8/clusterx/symmetry.py` & `clusterX-2.1.0rc1/clusterx/symmetry.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 # See accompanying license for details or visit https://www.apache.org/licenses/LICENSE-2.0.txt.
 
 import numpy as np
 import spglib
 
 def get_spacegroup(parent_lattice):
     """
-    Get space symmetry of a ParentLattice object. Sites allowing different substitutional species are treated as symetrically distinct.
+    Get space symmetry of a ParentLattice object. 
+    
+    Sites allowing different substitutional species are treated as symetrically distinct.
+
+    Uses ``spglib`` library.
     """
 
     atoms = parent_lattice.get_pristine().copy()
     
     # Break possible symmetries along non-periodic directions to get correct
     # symmetries with spglib.
     new_cell = []
@@ -24,16 +28,21 @@
 
     atoms.set_cell(new_cell,scale_atoms=False)
     # Create a fictitious atoms object with species set to site type.
     # This way, two sites which are symetrically equivalent in the pristine lattice
     # become inequivalent if those sites can be occupied by different species.
     atoms.set_atomic_numbers(parent_lattice.get_tags() + 1)
 
-    sg = spglib.get_spacegroup(atoms)
-    sym = spglib.get_symmetry(atoms)
+    lattice = atoms.get_cell()
+    positions = atoms.get_scaled_positions()
+    numbers = atoms.get_atomic_numbers()
+    spglib_input = (lattice, positions, numbers)
+    
+    sg = spglib.get_spacegroup(spglib_input)
+    sym = spglib.get_symmetry(spglib_input)
 
     # After finding symmetries, undo the previous re-scaling done to break
     # symmetries
     for it in range(len(sym['translations'])):
         for i, bc in enumerate(atoms.get_pbc()):
             if not bc:
                 sym['translations'][it][i] = sym['translations'][it][i]*np.pi
@@ -63,30 +72,41 @@
 
     return s
 
 
 def get_internal_translations(parent_lattice, super_cell):
     """
     Return the internal translations of a parent lattice with respect to a super cell.
+
     Translations are expressed in scaled coordinates with respect to the super cell.
+
+    The function returns a numpy array containing three-dimensional vectors representing the 
+    internal translation symmetries of the super cell.
+
+    **Parameters:**
+    ``parent_lattice``: ParentLattice instance
+        The ParentLattice object
+    
+    ``super_cell``: SuperCell instance
+        The SuperCell object. Must be a supercell of the parent lattice given as first argument. 
     """
     from ase import Atoms
     from clusterx.super_cell import SuperCell
     from clusterx.parent_lattice import ParentLattice
 
     atoms0 = Atoms(symbols=['H'], positions=[(0,0,0)], cell=parent_lattice.get_cell(), pbc=parent_lattice.get_pbc())
     atoms1 = ParentLattice(atoms=atoms0,pbc=parent_lattice.get_pbc())
     atoms2 = SuperCell(atoms1, super_cell.get_transformation())
 
     tra0 = atoms2.get_scaled_positions(wrap=True)
     tra1 = []
     for tr in tra0:
         include_tr = True
-        for id, bd in enumerate(parent_lattice.get_pbc()):
-            if tr[id] != 0 and not bd: # exclude translation vectors along non-periodic directions
+        for id_, bd in enumerate(parent_lattice.get_pbc()):
+            if tr[id_] != 0 and not bd: # exclude translation vectors along non-periodic directions
                 include_tr = False
                 break
 
         if include_tr:
             tra1.append(tr)
 
     return np.array(tra1)
```

### Comparing `clusterX-1.0.0.dev8/clusterx/lattices.py` & `clusterX-2.1.0rc1/clusterx/lattices.py`

 * *Files identical despite different names*

### Comparing `clusterX-1.0.0.dev8/clusterx/config.py` & `clusterX-2.1.0rc1/clusterx/config.py`

 * *Files identical despite different names*

### Comparing `clusterX-1.0.0.dev8/clusterx/test/test_cluster_orbit.py` & `clusterX-2.1.0rc1/clusterx/test/test_cluster_orbit2.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,59 +7,60 @@
 from clusterx.super_cell import SuperCell
 from clusterx.clusters.clusters_pool import ClustersPool
 from ase import Atoms
 from ase.spacegroup import crystal
 from ase.build import bulk
 import sys
 
-def test_cluster_orbit():
+def test_cluster_orbit2():
     """Test creation of cluster orbit in supercell using spglib
 
     After running the test, the orbit can be visualized with the command::
 
         ase gui test_cluster_orbit_#.json
     """
     tassert = True
     #tassert = False
     test_cases = [0,1,2,3,4,5]
     #test_cases = [0]
     orbits = [None,None,None,None,None,None]
+    mults = [None,None,None,None,None,None]
     for test_case in test_cases:
         if test_case == 0:
             # Perfect cubic lattice. The tested cluster is such that many interactions
             # with the periodic images of the crystal are present.
             a = 3.62/np.sqrt(2.0)
             positions = [(0,0,0)]
             cell = [(a,0,0),(0,a,0),(0,0,a)]
             pbc = (True,True,True)
             pri = Atoms('Cu', positions=positions, cell= cell, pbc= pbc)
             sub = Atoms('Al', positions=positions, cell= cell, pbc= pbc)
             sub2 = Atoms('Na', positions=positions, cell= cell, pbc= pbc)
 
             plat = ParentLattice(pri, substitutions=[sub,sub2], pbc=pbc)
-            scell = SuperCell(plat,[(5,0,0),(0,2,0),(0,0,1)])
+            scell = SuperCell(plat,[(5,0,0),(0,2,0),(0,0,1)], sym_table = True)
 
             cl = ClustersPool(plat)
 
-            orbit,mult = cl.get_cluster_orbit(scell, [0,2], [11,11])
+            orbit,mult = cl.get_cluster_orbit2(scell, [0,2], [11,11])
             db_name = "test_cluster_orbit_%s.json"%(test_case)
             cl.write_clusters_db(orbit, scell, db_name)
             orbits[test_case] = orbit
 
         if test_case == 1:
             # FCC lattice
             pri = bulk('Cu', 'fcc', a=3.6)
             sub = bulk('Al', 'fcc', a=3.6)
 
             plat = ParentLattice(pri, substitutions=[sub], pbc=pri.get_pbc())
-            scell = SuperCell(plat,np.diag([2,2,2]))
+            scell = SuperCell(plat,np.diag([2,2,2]), sym_table = True)
 
             cl = ClustersPool(plat)
 
-            orbit,mult = cl.get_cluster_orbit(scell, [0,2],[13,13])
+            orbit,mult = cl.get_cluster_orbit2(scell, [0,2],[13,13])
             db_name = "test_cluster_orbit_%s.json"%(test_case)
             cl.write_clusters_db(orbit, scell, db_name)
             orbits[test_case] = orbit
 
         if test_case == 2:
             # Clathrate 2x1x1 supercell. This contains spectator atoms.
             a = 10.515
@@ -72,36 +73,36 @@
                 (0, 0 , 0) #2a
             ]
 
             pri = crystal(['Si','Si','Si','Ba','Ba'], wyckoff, spacegroup=223, cellpar=[a, a, a, 90, 90, 90])
             sub = crystal(['Al','Al','Al','Ba','Ba'], wyckoff, spacegroup=223, cellpar=[a, a, a, 90, 90, 90])
 
             plat = ParentLattice(atoms=pri,substitutions=[sub])
-            scell = SuperCell(plat,[(2,0,0),(0,1,0),(0,0,1)])
+            scell = SuperCell(plat,[(2,0,0),(0,1,0),(0,0,1)], sym_table = True)
 
             cl = ClustersPool(plat)
-            orbit,mult = cl.get_cluster_orbit(scell, [19,17],[13,13]) # 24k-24k pair cluster
+            orbit,mult = cl.get_cluster_orbit2(scell, [19,17],[13,13]) # 24k-24k pair cluster
             db_name = "test_cluster_orbit_%s.json"%(test_case)
             cl.write_clusters_db(orbit, scell, db_name)
             orbits[test_case] = orbit
 
         if test_case == 3:
             # Al(111) surface with Na substitution on the first layer. Test a 3-point cluster.
             from ase.build import fcc111, add_adsorbate
             pri = fcc111('Al', size=(1,1,3), vacuum=10.0)
             sub = pri.copy()
             for atom in sub:
                 if atom.tag == 1:
                     atom.number = 11
 
             plat = ParentLattice(atoms=pri,substitutions=[sub])
-            scell = SuperCell(plat,[(4,0,0),(0,4,0),(0,0,1)])
+            scell = SuperCell(plat,[(4,0,0),(0,4,0),(0,0,1)], sym_table = True)
 
             cl = ClustersPool(plat)
-            orbit,mult = cl.get_cluster_orbit(scell, [2,14,5],[11,11,11])
+            orbit,mult = cl.get_cluster_orbit2(scell, [2,14,5],[11,11,11])
             db_name = "test_cluster_orbit_%s.json"%(test_case)
             cl.write_clusters_db(orbit, scell, db_name)
             orbits[test_case] = orbit
 
         if test_case == 4:
             # Al(111) surface with Na substitution on the first layer and on-top Oxygen adsorption.
             from ase.build import fcc111, add_adsorbate
@@ -118,18 +119,18 @@
 
             sub2 = pri.copy() # O on-top adsorbates
             for atom in sub2:
                 if atom.tag == 0:
                     atom.number = 8
 
             plat = ParentLattice(atoms=pri,substitutions=[sub1,sub2])
-            scell = SuperCell(plat,[(4,0,0),(0,4,0),(0,0,1)])
+            scell = SuperCell(plat,[(4,0,0),(0,4,0),(0,0,1)], sym_table = True)
 
             cl = ClustersPool(plat)
-            orbit,mult = cl.get_cluster_orbit(scell, [3,18],[8,11])
+            orbit,mult = cl.get_cluster_orbit2(scell, [3,18],[8,11])
             db_name = "test_cluster_orbit_%s.json"%(test_case)
             cl.write_clusters_db(orbit, scell, db_name)
             orbits[test_case] = orbit
 
         if test_case == 5:
             # Perfect cubic lattice. The tested cluster is such that many interactions
             # with the periodic images of the crystal are present.
@@ -138,28 +139,42 @@
             cell = [(a,0,0),(0,a,0),(0,0,a)]
             pbc = (True,True,True)
             pri = Atoms('Cu', positions=positions, cell= cell, pbc= pbc)
             sub = Atoms('Al', positions=positions, cell= cell, pbc= pbc)
             sub2 = Atoms('Na', positions=positions, cell= cell, pbc= pbc)
 
             plat = ParentLattice(pri, substitutions=[sub,sub2], pbc=pbc)
-            scell = SuperCell(plat,[(5,0,0),(0,2,0),(0,0,1)])
+            scell = SuperCell(plat,[(5,0,0),(0,2,0),(0,0,1)], sym_table = True)
             sites = scell.get_sites()
             cl = ClustersPool(plat)
 
             atom_idxs = [0,2]
             atom_species = [sites[0][1],sites[2][2]]
-            orbit,mult = cl.get_cluster_orbit(scell, atom_idxs, atom_species)
+            orbit,mult = cl.get_cluster_orbit2(scell, atom_idxs, atom_species)
             db_name = "test_cluster_orbit_%s.json"%(test_case)
             cl.write_clusters_db(orbit, scell, db_name)
             orbits[test_case] = orbit
 
+        
+        orbits[test_case] = orbit
+        mults[test_case] = mult
+
+        gen_ref = False
+        if gen_ref:
+            print("********++++++++   test_case = "+str(test_case)+"   ++++++++*********")
+            _orbit_nrs = []
+            _orbit_idxs = []
+            for i in range(len(orbit)):
+                _orbit_nrs.append(orbit[i].get_nrs())
+                _orbit_idxs.append(orbit[i].get_idxs())
+            print(np.array2string(np.array(_orbit_idxs),separator=","))
+            print(mult)
 
     print ("\n\n========Test writes========")
-    print (test_cluster_orbit.__doc__)
+    print (test_cluster_orbit2.__doc__)
     #print(np.array2string(orbit1,separator=","))
     print ("===========================\n")
 
     print ("========Asserts========")
 
     if tassert:
         for test_case in test_cases:
@@ -167,18 +182,18 @@
             assert check_result(test_case, orbits[test_case])
 
 
 def check_result(testnr, orbit):
     isok = True
     orbit_nrs = []
     orbit_idxs = []
-    for cluster in orbit:
-        orbit_nrs.append(cluster.get_nrs())
-        orbit_idxs.append(cluster.get_idxs())
-
+    for i in range(0,len(orbit)):
+        orbit_nrs.append(orbit[i].get_nrs())
+        orbit_idxs.append(orbit[i].get_idxs())
+    
     if testnr == 0:
         rorbit = np.array([
             [0,2],
             [1,3],
             [2,4],
             [3,5],
             [4,6],
@@ -201,39 +216,38 @@
             [6,6],
             [7,7],
             [8,8],
             [9,9]])
 
 
     if testnr == 1:
-        rorbit = np.array([
-            [0,2],
-            [1,3],
-            [4,6],
-            [5,7],
-            [0,5],
-            [1,4],
-            [2,7],
-            [3,6],
-            [0,4],
-            [1,5],
-            [2,6],
-            [3,7],
-            [0,3],
-            [1,2],
-            [4,7],
-            [5,6],
-            [0,6],
-            [1,7],
-            [2,4],
-            [3,5],
-            [0,1],
-            [2,3],
-            [4,5],
-            [6,7]])
+        rorbit = np.array([[0,2],
+                           [1,3],
+                           [4,6],
+                           [5,7],
+                           [0,4],
+                           [1,5],
+                           [2,6],
+                           [3,7],
+                           [0,5],
+                           [1,4],
+                           [2,7],
+                           [3,6],
+                           [0,3],
+                           [1,2],
+                           [4,7],
+                           [5,6],
+                           [0,1],
+                           [2,3],
+                           [4,5],
+                           [6,7],
+                           [0,6],
+                           [1,7],
+                           [2,4],
+                           [3,5]])
 
     if testnr == 2:
         rorbit = np.array(
             [[19,17],
              [73,71],
              [70,72],
              [16,18],
@@ -376,20 +390,31 @@
              [55, 58],
              [59, 62],
              [63, 50]])
 
     if testnr == 5:
         return True
 
-    if len(orbit) != len(rorbit):
+    if len(orbit_idxs) != len(rorbit):
         return False
-
+    
+    #sorted_rorbit = [sorted(x) for x in rorbit]
+    
+    #for cl in sorted(orbit_idxs, key=lambda x: x[0]):
+    #    if cl not in sorted_rorbit:
+    #        isok = False
+    #        break
+        
     for cl,rcl in zip(orbit_idxs,rorbit):
         if (cl != np.sort(rcl)).any():
-            isok = False
-            break
+            return False
 
+    #for cl,rcl in zip(orbit_idxs,rorbit):
+    #    print(cl,rcl)
+    #    if (cl != np.sort(rcl)).any():
+    #        isok = False
+    #        break
     return isok
 
 
 #if __name__ == "__main__":
 #    test_cluster_orbit()
```

### Comparing `clusterX-1.0.0.dev8/clusterx/test/test_concentration.py` & `clusterX-2.1.0rc1/clusterx/test/test_concentration.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     su1 = Atoms(['C','H','H'], positions=positions, cell=cell, pbc=pbc)
     su2 = Atoms(['H','He','H'], positions=positions, cell=cell, pbc=pbc)
     su3 = Atoms(['H','N','H'], positions=positions, cell=cell, pbc=pbc)
 
     plat = ParentLattice(pri,substitutions=[su1,su2,su3],pbc=pbc)
 
     scell = SuperCell(plat,np.array([(1,0,0),(0,3,0),(0,0,1)]))
-    strset = StructuresSet(plat, filename="test_cluster_selector_structures_set.json")
+    strset = StructuresSet(plat)
     nstr = 20
     #for i in range(nstr):
     #    strset.add_structure(scell.gen_random(nsubs={}))
     strset.add_structure(
         Structure(scell,
                   decoration_symbols=["H","H","H",
                                       "C","He","H",
@@ -52,14 +52,14 @@
                   )
         )
 
     fc_ref = [
         {1: [0.33333, 0.66666, 0.0], 2: [0.33333, 0.66666]},
         {1: [0.33333, 0.33333, 0.33333], 2: [0.0, 1.0]}
     ]
-    
+    strset.serialize(path="test_cluster_selector_structures_set.json")
     isok = True
     for i,s in enumerate(strset):
         fc = s.get_fractional_concentrations()
         isok *= dict_compare(fc,fc_ref[i],tol=1e-5)
 
     assert isok
```

### Comparing `clusterX-1.0.0.dev8/clusterx/test/test_emt2_calculator.py` & `clusterX-2.1.0rc1/clusterx/test/test_emt2_calculator.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 from clusterx.correlations import CorrelationsCalculator
 from clusterx.calculators.emt import EMT2
 from ase import Atoms
 import numpy as np
 
 def test_emt2_calculator():
     """Test calcualtion of energies with EMT2 calculator.
-    
+
     After successful execution of the test, the generated structures may be visualized with the command::
-        
+
         ase gui test_emt2_calculator#.json
 
     """
 
     cell = [[3,0,0],
             [0,1,0],
             [0,0,5]]
@@ -35,35 +35,34 @@
     su1 = Atoms(['C','H','H'], positions=positions, cell=cell, pbc=pbc)
     su2 = Atoms(['H','He','H'], positions=positions, cell=cell, pbc=pbc)
     su3 = Atoms(['H','N','H'], positions=positions, cell=cell, pbc=pbc)
 
     plat = ParentLattice(pri,substitutions=[su1,su2,su3],pbc=pbc)
 
     scell = SuperCell(plat,np.array([(1,0,0),(0,3,0),(0,0,1)]))
-    strset = StructuresSet(plat, filename="test_cluster_expansion_structures_set.json")
+    strset = StructuresSet(plat)
     strset.add_structure(Structure(scell,[1,2,1,6,7,1,1,2,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[6,1,1,1,1,1,1,1,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[1,2,1,1,7,1,6,7,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[1,1,1,6,1,1,1,7,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[6,7,1,6,7,1,6,2,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[1,7,1,6,2,1,1,1,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[6,1,1,1,1,1,1,1,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[1,1,1,1,7,1,6,7,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[1,2,1,6,2,1,6,2,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[6,1,1,6,2,1,1,1,1]),write_to_db=True)
+    strset.serialize(path="test_cluster_expansion_structures_set.json")
 
-    
     strset.set_calculator(EMT2())
     energies = strset.calculate_property()
-    
+
     # Generate output
     print ("\n\n========Test writes========")
     print(test_emt2_calculator.__doc__)
     print("Energies:\n")
-    print(np.array2string(energies,separator=",",max_line_width=1000))
+    print(np.array2string(np.array(energies),separator=",",max_line_width=1000))
     print ("===========================\n")
 
     print ("========Asserts========")
-    
+
     assert np.allclose( [ 420.02464215,  11.85279614, 200.11679975,  27.15487534, 162.41156144, 193.56777501,  11.85279614,  35.84803264, 585.51975722, 213.05311213], energies,atol=1e-5)
     #print(comat)
-
```

### Comparing `clusterX-1.0.0.dev8/clusterx/test/test_cluster_expansion.py` & `clusterX-2.1.0rc1/clusterx/test/test_cluster_expansion.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,16 @@
     plat = ParentLattice(pri,substitutions=[su1,su2,su3],pbc=pbc)
     #cpool = ClustersPool(plat, npoints=[0,1,2,3,4], radii=[0,0,2.3,1.42,1.42])
     cpool = ClustersPool(plat, npoints=[1,2,3,4], radii=[0,2.3,1.42,1.42])
     cpool.write_clusters_db(cpool.get_cpool(),cpool.get_cpool_scell(),"cpool.json")
     corrcal = CorrelationsCalculator("trigonometric", plat, cpool)
 
     scell = SuperCell(plat,np.array([(1,0,0),(0,3,0),(0,0,1)]))
-    strset = StructuresSet(plat, filename="test_cluster_expansion_structures_set.json")
+    #strset = StructuresSet(plat, filename="test_cluster_expansion_structures_set.json")
+    strset = StructuresSet(plat)
     nstr = 20
     #for i in range(nstr):
     #    strset.add_structure(scell.gen_random(nsubs={}))
     strset.add_structure(Structure(scell,[1,2,1,6,7,1,1,2,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[6,1,1,1,1,1,1,1,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[1,2,1,1,7,1,6,7,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[1,1,1,6,1,1,1,7,1]),write_to_db=True)
@@ -68,14 +69,15 @@
     strset.add_structure(Structure(scell,[1,2,1,6,7,1,6,2,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[1,7,1,1,2,1,1,1,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[6,7,1,1,7,1,1,1,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[6,2,1,6,1,1,6,7,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[1,7,1,1,1,1,6,2,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[6,1,1,1,7,1,1,1,1]),write_to_db=True)
 
+    strset.serialize(path="test_cluster_expansion_structures_set.json", overwrite=True)
     # Get the DATA(comat) + TARGET(energies)
     comat = corrcal.get_correlation_matrix(strset)
     strset.set_calculator(EMT2())
     energies = strset.calculate_property()
 
     #fitter_model = Fitter(method = "skl_LinearRegression")
```

### Comparing `clusterX-1.0.0.dev8/clusterx/test/test_clathrate_mc.py` & `clusterX-2.1.0rc1/clusterx/test/test_clathrate_mc.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,21 +66,23 @@
         0.0108175321899,
         0.0101521144776,
         0.00121744613474,
         0.000413664306204
     ]
     multE = [1,24,16,6,12,8,48,24,24,24]
     corcE = CorrelationsCalculator("binary-linear",plat,cpoolE)
+    corcE.reset_mc(mc = True)
+
     scellE = SuperCell(plat,[(2,0,0),(0,2,0),(0,0,2)])
 
     nmc = 10
-
+    
     for i in range(nmc):
         struc = scellE.gen_random({0:[16]})
-        corrs = corcE.get_cluster_correlations(struc,mc=True)
+        corrs = corcE.get_cluster_correlations(struc)
         print(corrs)
         erg = 0
         for j in range(len(ecisE)):
             erg += multE[j] * ecisE[j] * corrs[j]
 
         print(i,erg)
```

### Comparing `clusterX-1.0.0.dev8/clusterx/test/test_lattice_representation.py` & `clusterX-2.1.0rc1/clusterx/test/test_lattice_representation.py`

 * *Files identical despite different names*

### Comparing `clusterX-1.0.0.dev8/clusterx/test/test_clusters_selector.py` & `clusterX-2.1.0rc1/clusterx/test/test_clusters_selector.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     plat = ParentLattice(pri,substitutions=[su1,su2,su3],pbc=pbc)
     cpool = ClustersPool(plat, npoints=[0,1,2,3,4], radii=[0,0,2.3,2.3,1.42])
     #cpool = ClustersPool(plat, npoints=[1,2,3,4], radii=[0,2.3,1.42,1.42])
     cpool.write_clusters_db(cpool.get_cpool(),cpool.get_cpool_scell(),"cpool.json")
     corrcal = CorrelationsCalculator("trigonometric", plat, cpool)
 
     scell = SuperCell(plat,np.array([(1,0,0),(0,3,0),(0,0,1)]))
-    strset = StructuresSet(plat, filename="test_cluster_selector_structures_set.json")
+    strset = StructuresSet(plat)
     nstr = 20
     #for i in range(nstr):
     #    strset.add_structure(scell.gen_random(nsubs={}))
     strset.add_structure(Structure(scell,[1,2,1,6,7,1,1,2,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[6,1,1,1,1,1,1,1,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[1,2,1,1,7,1,6,7,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[1,1,1,6,1,1,1,7,1]),write_to_db=True)
@@ -72,25 +72,25 @@
     strset.add_structure(Structure(scell,[6,1,1,1,7,1,1,7,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[1,2,1,6,7,1,6,2,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[1,7,1,1,2,1,1,1,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[6,7,1,1,7,1,1,1,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[6,2,1,6,1,1,6,7,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[1,7,1,1,1,1,6,2,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[6,1,1,1,7,1,1,1,1]),write_to_db=True)
-
+    strset.serialize(path="test_cluster_selector_structures_set.json", overwrite=True)
     # Get the DATA(comat) + TARGET(energies)
     comat = corrcal.get_correlation_matrix(strset)
     strset.set_calculator(EMT2())
     energies = strset.calculate_property()
 
     #fitter_model = Fitter(method = "skl_LinearRegression")
 
 
     clsel = ClustersSelector(method='linreg', clusters_sets = "size")
-    
+
     clsel.select_clusters(strset,cpool,"energy")
 
     #clsets.get_subpool(clsel.get_optimal_clusters())
 
     cp2 = clsel.optimal_clusters._cpool
     clset=[]
     npoints=[]
@@ -139,9 +139,23 @@
     print("CV-----------------------")
     print(clsel.opt_mean_cv,ropt_mean_cv)
 
     print(isclose(rcvs, clsel.cvs))
     """
 
     #isok = isclose(rclset,clset) and isclose(rnpoints, npoints) and isclose(rradius, radius) and isclose(rrmse, clsel.rmse) and isclose(rcvs, clsel.cvs) and isclose(recis, clsel.opt_ecis) and isclose(ropt_rmse, clsel.opt_rmse) and isclose(ropt_mean_cv, clsel.opt_mean_cv).all()
-    isok = isclose(rclset,clset) and isclose(rnpoints, npoints) and isclose(rradius, radius) and isclose(rrmse, clsel.rmse) and isclose(rcvs, clsel.cvs)
-    assert(isok)
+
+    isok1 = isclose(rclset,clset) and isclose(rnpoints, npoints) and isclose(rradius, radius) and isclose(rrmse, clsel.rmse) and isclose(rcvs, clsel.cvs)
+    assert(isok1)
+
+    opt_cpool = clsel.get_optimal_cpool()
+    opt_cpool.serialize(db_name = "cpool.json")
+
+    opt2_cpool = ClustersPool(json_db_filepath = "cpool.json")
+    dictcpool = opt2_cpool.get_cpool_dict()
+
+    npoints2 = dictcpool.get('npoints')
+    radii2 = dictcpool.get('radii')
+    nclusters2 = dictcpool.get('nclusters')
+    
+    isok2 =  isclose(len(rclset),nclusters2) and isclose(rnpoints, npoints2) and isclose(rradius, radii2)
+    assert(isok2)
```

### Comparing `clusterX-1.0.0.dev8/clusterx/test/test_get_all_hnf.py` & `clusterX-2.1.0rc1/clusterx/test/test_get_all_hnf.py`

 * *Files identical despite different names*

### Comparing `clusterX-1.0.0.dev8/clusterx/test/test_is_nary.py` & `clusterX-2.1.0rc1/clusterx/test/test_is_nary.py`

 * *Files identical despite different names*

### Comparing `clusterX-1.0.0.dev8/clusterx/test/test_parent_lattice_creation.py` & `clusterX-2.1.0rc1/clusterx/test/test_parent_lattice_creation.py`

 * *Files identical despite different names*

### Comparing `clusterX-1.0.0.dev8/clusterx/test/test_clusters_selector_lasso.py` & `clusterX-2.1.0rc1/clusterx/test/test_clusters_selector_lasso.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     plat = ParentLattice(pri,substitutions=[su1,su2,su3],pbc=pbc)
     cpool = ClustersPool(plat, npoints=[0,1,2,3,4], radii=[0,0,2.3,2.3,2.3])
     #cpool = ClustersPool(plat, npoints=[1,2,3,4], radii=[0,2.3,1.42,1.42])
     cpool.write_clusters_db(cpool.get_cpool(),cpool.get_cpool_scell(),"cpool.json")
     corrcal = CorrelationsCalculator("trigonometric", plat, cpool)
 
     scell = SuperCell(plat,np.array([(1,0,0),(0,3,0),(0,0,1)]))
-    strset = StructuresSet(plat, filename="test_cluster_selector_structures_set.json")
+    strset = StructuresSet(plat)
     nstr = 20
     #for i in range(nstr):
     #    strset.add_structure(scell.gen_random(nsubs={}))
     strset.add_structure(Structure(scell,[1,2,1,6,7,1,1,2,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[6,1,1,1,1,1,1,1,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[1,2,1,1,7,1,6,7,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[1,1,1,6,1,1,1,7,1]),write_to_db=True)
@@ -73,21 +73,21 @@
     strset.add_structure(Structure(scell,[6,1,1,1,7,1,1,7,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[1,2,1,6,7,1,6,2,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[1,7,1,1,2,1,1,1,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[6,7,1,1,7,1,1,1,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[6,2,1,6,1,1,6,7,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[1,7,1,1,1,1,6,2,1]),write_to_db=True)
     strset.add_structure(Structure(scell,[6,1,1,1,7,1,1,1,1]),write_to_db=True)
-
+    strset.serialize(path="test_cluster_selector_structures_set.json")
     # Get the DATA(comat) + TARGET(energies)
     comat = corrcal.get_correlation_matrix(strset)
     strset.set_calculator(EMT2())
     energies = strset.calculate_property()
 
-    clsel = ClustersSelector(method='lasso', sparsity_max=0.10, sparsity_min=0.01)
+    clsel = ClustersSelector(method='lasso', sparsity_max=0.10, sparsity_min=0.01, max_iter=1000000000, tol=1e-12, sparsity_scale = "piece_log", cv_splits=None)
     #clsel = ClustersSelector('combinations', cpool, fitter_size = "linreg", nclmax=2)
     #clsel = ClustersSelector('size+combinations', cpool, fitter_size = "linreg", nclmax = 2, set0 = [2,1])
     #clsel.select_clusters(comat,energies)
     clsel.select_clusters(strset,cpool,"energy")
 
     #clsets.get_subpool(clsel.get_optimal_clusters())
 
@@ -130,10 +130,11 @@
     print("sparsities-----------------------")
     for i,(r,rr) in enumerate(zip(clsel.ecis,recis)):
         print("line:  ",i,r,rr,r-rr)
 
     isok = isclose(rsparsities,clsel.lasso_sparsities) and isclose(rnpoints, npoints) and isclose(rradius, radius) and isclose(rrmse, clsel.rmse) and isclose(rcvs, clsel.cvs) and isclose(recis, clsel.ecis) and isclose(ropt_rmse, clsel.opt_rmse) and isclose(ropt_mean_cv, clsel.opt_mean_cv).all()
     """
     #isok = isclose(rsparsities,clsel.lasso_sparsities) and isclose(rrmse, clsel.rmse) and isclose(rcvs, clsel.cvs) and isclose(ropt_rmse, clsel.opt_rmse) and isclose(ropt_mean_cv, clsel.opt_mean_cv).all()
-    isok = isclose(rsparsities,clsel.lasso_sparsities) and isclose(rrmse, clsel.rmse) and isclose(rcvs, clsel.cvs)
+    rtol=1e-2
+    isok = isclose(rsparsities,clsel.lasso_sparsities,rtol=rtol) and isclose(rrmse, clsel.rmse,rtol=rtol) and isclose(rcvs, clsel.cvs,rtol=rtol)
 
     assert(isok)
```

### Comparing `clusterX-1.0.0.dev8/clusterx/test/test_cluster.py` & `clusterX-2.1.0rc1/clusterx/test/test_cluster.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 def test_cluster():
     """
     Test cluster class
     """
     try:
         c1 = Cluster([0,1,2,1],[13,14,15,13])
-        is_multiple_species_in_site = False
+        repeated_atom_index_detected = False
     except:
-        is_multiple_species_in_site = True
+        repeated_atom_index_detected = True
 
     try:
         c1 = Cluster([0,1,2,1],[13,14,15])
         is_consistent_length = False
     except:
         is_consistent_length = True
 
@@ -42,41 +42,46 @@
     c1 = Cluster([],[])
     c2 = Cluster([0,2,1,3],[13,14,14,16])
     eq4 = c1!=c2
     
     c1 = Cluster([0,1,2,1],[13,14,15,14])
     c2 = Cluster([1,1,0,2],[14,14,13,15])
     eq5 = c1==c2
-    
+
     c1 = Cluster([0,1,2],[13,14,15])
     c2 = Cluster([0,1,2,3],[13,14,15,16])
     eq6 = c1!=c2
 
+    c1 = Cluster([0,1,2,1],[13,14,15,14])
+    c2 = Cluster([1,0,2],[14,13,15])
+    eq7 = c1!=c2
+    
     c3 = Cluster([0,1,2],[13,14,15]) 
     c4 = Cluster([0,1,3],[13,14,15]) 
     clusters = [c1,c2]
     in1 = c3 in clusters
     in2 = c4 not in clusters
     print("end test inclusion")
     
     print ("\n\n========Test writes========")
     print (test_cluster.__doc__)
     print ("===========================\n")
 
     print ("========Asserts========")
 
-    print("test is_multiple_species_in_site: ",is_multiple_species_in_site)
-    assert is_multiple_species_in_site
+    print("test is_multiple_species_in_site: ",repeated_atom_index_detected)
+    assert repeated_atom_index_detected
     print("test is_consistent_length: ",is_consistent_length)
     assert is_consistent_length
     print("test can_create_empty: ",can_create_empty)
     assert can_create_empty
     print("test equalities:", eq1,eq2,eq3,eq4,eq5,eq6)
     assert eq1
     assert eq2
     assert eq3
     assert eq4
     assert eq5
     assert eq6
+    assert eq7
     print("test array inclusion:", in1,in2)
     assert in1
     assert in2
```

### Comparing `clusterX-1.0.0.dev8/clusterx/test/test_cluster_correlations.py` & `clusterX-2.1.0rc1/clusterx/test/test_cluster_correlations.py`

 * *Files identical despite different names*

### Comparing `clusterX-1.0.0.dev8/clusterx/test/test_get_unique_supercells.py` & `clusterX-2.1.0rc1/clusterx/test/test_get_unique_supercells.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,158 +85,164 @@
 00000540: 0a0a 2020 2020 2020 2020 2020 2020 756e  ..            un
 00000550: 6971 7565 5f73 6373 2c20 756e 6971 7565  ique_scs, unique
 00000560: 5f74 7261 666f 7320 3d20 7574 696c 732e  _trafos = utils.
 00000570: 6765 745f 756e 6971 7565 5f73 7570 6572  get_unique_super
 00000580: 6365 6c6c 7328 696e 6465 782c 706c 290a  cells(index,pl).
 00000590: 0a20 2020 2020 2020 2020 2020 2073 7365  .            sse
 000005a0: 7420 3d20 5374 7275 6374 7572 6573 5365  t = StructuresSe
-000005b0: 7428 706c 2c66 696c 656e 616d 653d 2274  t(pl,filename="t
-000005c0: 6573 745f 6765 745f 756e 6971 7565 5f73  est_get_unique_s
-000005d0: 7570 6572 6365 6c6c 732d 7371 7561 7265  upercells-square
-000005e0: 5f6c 6174 7469 6365 2e6a 736f 6e22 290a  _lattice.json").
-000005f0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00000600: 7420 696e 2075 6e69 7175 655f 7472 6166  t in unique_traf
-00000610: 6f73 3a0a 2020 2020 2020 2020 2020 2020  os:.            
-00000620: 2020 2020 7363 656c 6c20 3d20 5375 7065      scell = Supe
-00000630: 7243 656c 6c28 706c 2c74 290a 2020 2020  rCell(pl,t).    
-00000640: 2020 2020 2020 2020 2020 2020 7373 6574              sset
-00000650: 2e61 6464 5f73 7472 7563 7475 7265 2853  .add_structure(S
-00000660: 7472 7563 7475 7265 2873 6365 6c6c 2c73  tructure(scell,s
-00000670: 6365 6c6c 2e67 6574 5f61 746f 6d69 635f  cell.get_atomic_
-00000680: 6e75 6d62 6572 7328 2929 2c77 7269 7465  numbers()),write
-00000690: 5f74 6f5f 6462 203d 2054 7275 6529 0a0a  _to_db = True)..
-000006a0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-000006b0: 7428 225c 6e46 6f75 6e64 2022 2c6c 656e  t("\nFound ",len
-000006c0: 2875 6e69 7175 655f 7363 7329 2c20 2220  (unique_scs), " 
-000006d0: 756e 6971 7565 2048 4e46 7320 666f 7220  unique HNFs for 
-000006e0: 6120 3244 2073 7175 6172 6520 6c61 7474  a 2D square latt
-000006f0: 6963 6520 6f66 2069 6e64 6578 2022 2c69  ice of index ",i
-00000700: 6e64 6578 290a 2020 2020 2020 2020 2020  ndex).          
-00000710: 2020 2370 7269 6e74 2822 5343 533a 2022    #print("SCS: "
-00000720: 2c20 756e 6971 7565 5f73 6373 290a 2020  , unique_scs).  
+000005b0: 7428 706c 290a 2020 2020 2020 2020 2020  t(pl).          
+000005c0: 2020 666f 7220 7420 696e 2075 6e69 7175    for t in uniqu
+000005d0: 655f 7472 6166 6f73 3a0a 2020 2020 2020  e_trafos:.      
+000005e0: 2020 2020 2020 2020 2020 7363 656c 6c20            scell 
+000005f0: 3d20 5375 7065 7243 656c 6c28 706c 2c74  = SuperCell(pl,t
+00000600: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00000610: 2020 7373 6574 2e61 6464 5f73 7472 7563    sset.add_struc
+00000620: 7475 7265 2853 7472 7563 7475 7265 2873  ture(Structure(s
+00000630: 6365 6c6c 2c73 6365 6c6c 2e67 6574 5f61  cell,scell.get_a
+00000640: 746f 6d69 635f 6e75 6d62 6572 7328 2929  tomic_numbers())
+00000650: 2c77 7269 7465 5f74 6f5f 6462 203d 2054  ,write_to_db = T
+00000660: 7275 6529 0a0a 2020 2020 2020 2020 2020  rue)..          
+00000670: 2020 7373 6574 2e73 6572 6961 6c69 7a65    sset.serialize
+00000680: 2870 6174 683d 2274 6573 745f 6765 745f  (path="test_get_
+00000690: 756e 6971 7565 5f73 7570 6572 6365 6c6c  unique_supercell
+000006a0: 732d 7371 7561 7265 5f6c 6174 7469 6365  s-square_lattice
+000006b0: 2e6a 736f 6e22 2c20 6f76 6572 7772 6974  .json", overwrit
+000006c0: 653d 5472 7565 290a 2020 2020 2020 2020  e=True).        
+000006d0: 2020 2020 7072 696e 7428 225c 6e46 6f75      print("\nFou
+000006e0: 6e64 2022 2c6c 656e 2875 6e69 7175 655f  nd ",len(unique_
+000006f0: 7363 7329 2c20 2220 756e 6971 7565 2048  scs), " unique H
+00000700: 4e46 7320 666f 7220 6120 3244 2073 7175  NFs for a 2D squ
+00000710: 6172 6520 6c61 7474 6963 6520 6f66 2069  are lattice of i
+00000720: 6e64 6578 2022 2c69 6e64 6578 290a 2020  ndex ",index).  
 00000730: 2020 2020 2020 2020 2020 2370 7269 6e74            #print
-00000740: 2822 5452 413a 2022 2c20 756e 6971 7565  ("TRA: ", unique
-00000750: 5f74 7261 666f 7329 0a20 2020 2020 2020  _trafos).       
-00000760: 2020 2020 2069 736f 6b30 203d 206c 656e       isok0 = len
-00000770: 2875 6e69 7175 655f 7363 7329 203d 3d20  (unique_scs) == 
-00000780: 3420 616e 6420 756e 6971 7565 5f73 6373  4 and unique_scs
-00000790: 5b31 5d5b 315d 5b31 5d20 3d3d 2031 322e  [1][1][1] == 12.
-000007a0: 340a 0a20 2020 2020 2020 2069 6620 6361  4..        if ca
-000007b0: 7365 203d 3d20 313a 2023 4643 430a 2020  se == 1: #FCC.  
-000007c0: 2020 2020 2020 2020 2020 613d 330a 2020            a=3.  
-000007d0: 2020 2020 2020 2020 2020 696e 6465 7820            index 
-000007e0: 3d20 340a 2020 2020 2020 2020 2020 2020  = 4.            
-000007f0: 6365 6c6c 203d 206e 702e 6172 7261 7928  cell = np.array(
-00000800: 5b5b 302e 352c 302e 352c 302e 305d 2c5b  [[0.5,0.5,0.0],[
-00000810: 302e 352c 302e 302c 302e 355d 2c5b 302e  0.5,0.0,0.5],[0.
-00000820: 302c 302e 352c 302e 355d 5d29 0a20 2020  0,0.5,0.5]]).   
-00000830: 2020 2020 2020 2020 2070 6f73 6974 696f           positio
-00000840: 6e73 203d 206e 702e 6172 7261 7928 5b5b  ns = np.array([[
-00000850: 302c 302c 305d 5d29 0a20 2020 2020 2020  0,0,0]]).       
-00000860: 2020 2020 2073 6974 6573 203d 205b 5b61       sites = [[a
-00000870: 6e5b 2243 7522 5d2c 616e 5b22 4175 225d  n["Cu"],an["Au"]
-00000880: 5d5d 0a20 2020 2020 2020 2020 2020 2070  ]].            p
-00000890: 7269 735f 6663 6320 3d20 4174 6f6d 7328  ris_fcc = Atoms(
-000008a0: 6365 6c6c 3d63 656c 6c2a 612c 706f 7369  cell=cell*a,posi
-000008b0: 7469 6f6e 733d 706f 7369 7469 6f6e 732a  tions=positions*
-000008c0: 612c 7062 633d 2831 2c31 2c31 2929 0a0a  a,pbc=(1,1,1))..
-000008d0: 2020 2020 2020 2020 2020 2020 706c 203d              pl =
-000008e0: 2050 6172 656e 744c 6174 7469 6365 2870   ParentLattice(p
-000008f0: 7269 735f 6663 632c 7369 7465 733d 7369  ris_fcc,sites=si
-00000900: 7465 7329 0a0a 2020 2020 2020 2020 2020  tes)..          
-00000910: 2020 756e 6971 7565 5f73 6373 2c20 756e    unique_scs, un
-00000920: 6971 7565 5f74 7261 666f 7320 3d20 7574  ique_trafos = ut
-00000930: 696c 732e 6765 745f 756e 6971 7565 5f73  ils.get_unique_s
-00000940: 7570 6572 6365 6c6c 7328 696e 6465 782c  upercells(index,
-00000950: 706c 290a 0a20 2020 2020 2020 2020 2020  pl)..           
-00000960: 2073 7365 7420 3d20 5374 7275 6374 7572   sset = Structur
-00000970: 6573 5365 7428 706c 2c66 696c 656e 616d  esSet(pl,filenam
-00000980: 653d 2274 6573 745f 6765 745f 756e 6971  e="test_get_uniq
-00000990: 7565 5f73 7570 6572 6365 6c6c 732d 6663  ue_supercells-fc
-000009a0: 632e 6a73 6f6e 2229 0a20 2020 2020 2020  c.json").       
-000009b0: 2020 2020 2066 6f72 2074 2069 6e20 756e       for t in un
-000009c0: 6971 7565 5f74 7261 666f 733a 0a20 2020  ique_trafos:.   
-000009d0: 2020 2020 2020 2020 2020 2020 2073 6365               sce
-000009e0: 6c6c 203d 2053 7570 6572 4365 6c6c 2870  ll = SuperCell(p
-000009f0: 6c2c 7429 0a20 2020 2020 2020 2020 2020  l,t).           
-00000a00: 2020 2020 2073 7365 742e 6164 645f 7374       sset.add_st
-00000a10: 7275 6374 7572 6528 5374 7275 6374 7572  ructure(Structur
-00000a20: 6528 7363 656c 6c2c 7363 656c 6c2e 6765  e(scell,scell.ge
-00000a30: 745f 6174 6f6d 6963 5f6e 756d 6265 7273  t_atomic_numbers
-00000a40: 2829 292c 7772 6974 655f 746f 5f64 6220  ()),write_to_db 
-00000a50: 3d20 5472 7565 290a 0a20 2020 2020 2020  = True)..       
-00000a60: 2020 2020 2070 7269 6e74 2822 466f 756e       print("Foun
-00000a70: 6420 222c 6c65 6e28 756e 6971 7565 5f73  d ",len(unique_s
-00000a80: 6373 292c 2022 2075 6e69 7175 6520 484e  cs), " unique HN
-00000a90: 4673 2066 6f72 2061 2046 4343 206c 6174  Fs for a FCC lat
-00000aa0: 7469 6365 206f 6620 696e 6465 7820 222c  tice of index ",
-00000ab0: 696e 6465 7829 0a20 2020 2020 2020 2020  index).         
-00000ac0: 2020 2023 7072 696e 7428 2253 4353 3a20     #print("SCS: 
-00000ad0: 222c 2075 6e69 7175 655f 7363 7329 0a20  ", unique_scs). 
-00000ae0: 2020 2020 2020 2020 2020 2023 7072 696e             #prin
-00000af0: 7428 2254 5241 3a20 222c 2075 6e69 7175  t("TRA: ", uniqu
-00000b00: 655f 7472 6166 6f73 290a 2020 2020 2020  e_trafos).      
-00000b10: 2020 2020 2020 6973 6f6b 3120 3d20 6c65        isok1 = le
-00000b20: 6e28 756e 6971 7565 5f73 6373 2920 3d3d  n(unique_scs) ==
-00000b30: 2037 2061 6e64 2075 6e69 7175 655f 7472   7 and unique_tr
-00000b40: 6166 6f73 5b34 5d5b 325d 5b32 5d20 3d3d  afos[4][2][2] ==
-00000b50: 2034 0a0a 2020 2020 2020 2020 6966 2063   4..        if c
-00000b60: 6173 6520 3d3d 2032 3a20 2353 696d 706c  ase == 2: #Simpl
-00000b70: 6520 6375 6269 630a 2020 2020 2020 2020  e cubic.        
-00000b80: 2020 2020 613d 332e 310a 2020 2020 2020      a=3.1.      
-00000b90: 2020 2020 2020 696e 6465 7820 3d20 340a        index = 4.
-00000ba0: 2020 2020 2020 2020 2020 2020 6365 6c6c              cell
-00000bb0: 203d 206e 702e 6172 7261 7928 5b5b 312c   = np.array([[1,
-00000bc0: 302c 305d 2c5b 302c 312c 305d 2c5b 302c  0,0],[0,1,0],[0,
-00000bd0: 302c 315d 5d29 0a20 2020 2020 2020 2020  0,1]]).         
-00000be0: 2020 2070 6f73 6974 696f 6e73 203d 206e     positions = n
-00000bf0: 702e 6172 7261 7928 5b5b 302c 302c 305d  p.array([[0,0,0]
-00000c00: 5d29 0a20 2020 2020 2020 2020 2020 2073  ]).            s
-00000c10: 6974 6573 203d 205b 5b31 322c 3133 5d5d  ites = [[12,13]]
-00000c20: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00000c30: 7320 3d20 4174 6f6d 7328 6365 6c6c 3d63  s = Atoms(cell=c
-00000c40: 656c 6c2a 612c 2070 6f73 6974 696f 6e73  ell*a, positions
-00000c50: 3d70 6f73 6974 696f 6e73 2a61 290a 0a20  =positions*a).. 
-00000c60: 2020 2020 2020 2020 2020 2070 6c20 3d20             pl = 
-00000c70: 5061 7265 6e74 4c61 7474 6963 6528 7072  ParentLattice(pr
-00000c80: 6973 2c20 7369 7465 733d 7369 7465 732c  is, sites=sites,
-00000c90: 2070 6263 3d28 312c 312c 3129 290a 0a20   pbc=(1,1,1)).. 
-00000ca0: 2020 2020 2020 2020 2020 2075 6e69 7175             uniqu
-00000cb0: 655f 7363 732c 2075 6e69 7175 655f 7472  e_scs, unique_tr
-00000cc0: 6166 6f73 203d 2075 7469 6c73 2e67 6574  afos = utils.get
-00000cd0: 5f75 6e69 7175 655f 7375 7065 7263 656c  _unique_supercel
-00000ce0: 6c73 2869 6e64 6578 2c70 6c29 0a0a 2020  ls(index,pl)..  
-00000cf0: 2020 2020 2020 2020 2020 7373 6574 203d            sset =
-00000d00: 2053 7472 7563 7475 7265 7353 6574 2870   StructuresSet(p
-00000d10: 6c2c 6669 6c65 6e61 6d65 3d22 7465 7374  l,filename="test
-00000d20: 5f67 6574 5f75 6e69 7175 655f 7375 7065  _get_unique_supe
-00000d30: 7263 656c 6c73 2d73 632e 6a73 6f6e 2229  rcells-sc.json")
-00000d40: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00000d50: 2074 2069 6e20 756e 6971 7565 5f74 7261   t in unique_tra
-00000d60: 666f 733a 0a20 2020 2020 2020 2020 2020  fos:.           
-00000d70: 2020 2020 2073 6365 6c6c 203d 2053 7570       scell = Sup
-00000d80: 6572 4365 6c6c 2870 6c2c 7429 0a20 2020  erCell(pl,t).   
-00000d90: 2020 2020 2020 2020 2020 2020 2073 7365               sse
-00000da0: 742e 6164 645f 7374 7275 6374 7572 6528  t.add_structure(
-00000db0: 5374 7275 6374 7572 6528 7363 656c 6c2c  Structure(scell,
-00000dc0: 7363 656c 6c2e 6765 745f 6174 6f6d 6963  scell.get_atomic
-00000dd0: 5f6e 756d 6265 7273 2829 292c 7772 6974  _numbers()),writ
-00000de0: 655f 746f 5f64 6220 3d20 5472 7565 290a  e_to_db = True).
-00000df0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00000e00: 6e74 2822 466f 756e 6420 222c 6c65 6e28  nt("Found ",len(
-00000e10: 756e 6971 7565 5f73 6373 292c 2022 2075  unique_scs), " u
-00000e20: 6e69 7175 6520 484e 4673 2066 6f72 2061  nique HNFs for a
-00000e30: 2073 696d 706c 6520 6375 6269 6320 6c61   simple cubic la
-00000e40: 7474 6963 6520 6f66 2069 6e64 6578 2022  ttice of index "
-00000e50: 2c69 6e64 6578 290a 2020 2020 2020 2020  ,index).        
-00000e60: 2020 2020 2370 7269 6e74 2822 5343 533a      #print("SCS:
-00000e70: 2022 2c20 756e 6971 7565 5f73 6373 290a   ", unique_scs).
-00000e80: 2020 2020 2020 2020 2020 2020 2370 7269              #pri
-00000e90: 6e74 2822 5452 413a 2022 2c20 756e 6971  nt("TRA: ", uniq
-00000ea0: 7565 5f74 7261 666f 7329 0a20 2020 2020  ue_trafos).     
-00000eb0: 2020 2020 2020 2069 736f 6b32 203d 206c         isok2 = l
-00000ec0: 656e 2875 6e69 7175 655f 7363 7329 203d  en(unique_scs) =
-00000ed0: 3d20 3920 616e 6420 756e 6971 7565 5f73  = 9 and unique_s
-00000ee0: 6373 5b34 5d5b 325d 5b32 5d20 3d3d 2031  cs[4][2][2] == 1
-00000ef0: 322e 340a 0a20 2020 2061 7373 6572 7420  2.4..    assert 
-00000f00: 6973 6f6b 3020 616e 6420 6973 6f6b 3120  isok0 and isok1 
-00000f10: 616e 6420 6973 6f6b 320a                 and isok2.
+00000740: 2822 5343 533a 2022 2c20 756e 6971 7565  ("SCS: ", unique
+00000750: 5f73 6373 290a 2020 2020 2020 2020 2020  _scs).          
+00000760: 2020 2370 7269 6e74 2822 5452 413a 2022    #print("TRA: "
+00000770: 2c20 756e 6971 7565 5f74 7261 666f 7329  , unique_trafos)
+00000780: 0a20 2020 2020 2020 2020 2020 2069 736f  .            iso
+00000790: 6b30 203d 206c 656e 2875 6e69 7175 655f  k0 = len(unique_
+000007a0: 7363 7329 203d 3d20 3420 616e 6420 756e  scs) == 4 and un
+000007b0: 6971 7565 5f73 6373 5b31 5d5b 315d 5b31  ique_scs[1][1][1
+000007c0: 5d20 3d3d 2031 322e 340a 0a20 2020 2020  ] == 12.4..     
+000007d0: 2020 2069 6620 6361 7365 203d 3d20 313a     if case == 1:
+000007e0: 2023 4643 430a 2020 2020 2020 2020 2020   #FCC.          
+000007f0: 2020 613d 330a 2020 2020 2020 2020 2020    a=3.          
+00000800: 2020 696e 6465 7820 3d20 340a 2020 2020    index = 4.    
+00000810: 2020 2020 2020 2020 6365 6c6c 203d 206e          cell = n
+00000820: 702e 6172 7261 7928 5b5b 302e 352c 302e  p.array([[0.5,0.
+00000830: 352c 302e 305d 2c5b 302e 352c 302e 302c  5,0.0],[0.5,0.0,
+00000840: 302e 355d 2c5b 302e 302c 302e 352c 302e  0.5],[0.0,0.5,0.
+00000850: 355d 5d29 0a20 2020 2020 2020 2020 2020  5]]).           
+00000860: 2070 6f73 6974 696f 6e73 203d 206e 702e   positions = np.
+00000870: 6172 7261 7928 5b5b 302c 302c 305d 5d29  array([[0,0,0]])
+00000880: 0a20 2020 2020 2020 2020 2020 2073 6974  .            sit
+00000890: 6573 203d 205b 5b61 6e5b 2243 7522 5d2c  es = [[an["Cu"],
+000008a0: 616e 5b22 4175 225d 5d5d 0a20 2020 2020  an["Au"]]].     
+000008b0: 2020 2020 2020 2070 7269 735f 6663 6320         pris_fcc 
+000008c0: 3d20 4174 6f6d 7328 6365 6c6c 3d63 656c  = Atoms(cell=cel
+000008d0: 6c2a 612c 706f 7369 7469 6f6e 733d 706f  l*a,positions=po
+000008e0: 7369 7469 6f6e 732a 612c 7062 633d 2831  sitions*a,pbc=(1
+000008f0: 2c31 2c31 2929 0a0a 2020 2020 2020 2020  ,1,1))..        
+00000900: 2020 2020 706c 203d 2050 6172 656e 744c      pl = ParentL
+00000910: 6174 7469 6365 2870 7269 735f 6663 632c  attice(pris_fcc,
+00000920: 7369 7465 733d 7369 7465 7329 0a0a 2020  sites=sites)..  
+00000930: 2020 2020 2020 2020 2020 756e 6971 7565            unique
+00000940: 5f73 6373 2c20 756e 6971 7565 5f74 7261  _scs, unique_tra
+00000950: 666f 7320 3d20 7574 696c 732e 6765 745f  fos = utils.get_
+00000960: 756e 6971 7565 5f73 7570 6572 6365 6c6c  unique_supercell
+00000970: 7328 696e 6465 782c 706c 290a 0a20 2020  s(index,pl)..   
+00000980: 2020 2020 2020 2020 2073 7365 7420 3d20           sset = 
+00000990: 5374 7275 6374 7572 6573 5365 7428 706c  StructuresSet(pl
+000009a0: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
+000009b0: 7220 7420 696e 2075 6e69 7175 655f 7472  r t in unique_tr
+000009c0: 6166 6f73 3a0a 2020 2020 2020 2020 2020  afos:.          
+000009d0: 2020 2020 2020 7363 656c 6c20 3d20 5375        scell = Su
+000009e0: 7065 7243 656c 6c28 706c 2c74 290a 2020  perCell(pl,t).  
+000009f0: 2020 2020 2020 2020 2020 2020 2020 7373                ss
+00000a00: 6574 2e61 6464 5f73 7472 7563 7475 7265  et.add_structure
+00000a10: 2853 7472 7563 7475 7265 2873 6365 6c6c  (Structure(scell
+00000a20: 2c73 6365 6c6c 2e67 6574 5f61 746f 6d69  ,scell.get_atomi
+00000a30: 635f 6e75 6d62 6572 7328 2929 2c77 7269  c_numbers()),wri
+00000a40: 7465 5f74 6f5f 6462 203d 2054 7275 6529  te_to_db = True)
+00000a50: 0a0a 2020 2020 2020 2020 2020 2020 7373  ..            ss
+00000a60: 6574 2e73 6572 6961 6c69 7a65 2870 6174  et.serialize(pat
+00000a70: 683d 2274 6573 745f 6765 745f 756e 6971  h="test_get_uniq
+00000a80: 7565 5f73 7570 6572 6365 6c6c 732d 6663  ue_supercells-fc
+00000a90: 632e 6a73 6f6e 2229 0a20 2020 2020 2020  c.json").       
+00000aa0: 2020 2020 2070 7269 6e74 2822 466f 756e       print("Foun
+00000ab0: 6420 222c 6c65 6e28 756e 6971 7565 5f73  d ",len(unique_s
+00000ac0: 6373 292c 2022 2075 6e69 7175 6520 484e  cs), " unique HN
+00000ad0: 4673 2066 6f72 2061 2046 4343 206c 6174  Fs for a FCC lat
+00000ae0: 7469 6365 206f 6620 696e 6465 7820 222c  tice of index ",
+00000af0: 696e 6465 7829 0a20 2020 2020 2020 2020  index).         
+00000b00: 2020 2023 7072 696e 7428 2253 4353 3a20     #print("SCS: 
+00000b10: 222c 2075 6e69 7175 655f 7363 7329 0a20  ", unique_scs). 
+00000b20: 2020 2020 2020 2020 2020 2023 7072 696e             #prin
+00000b30: 7428 2254 5241 3a20 222c 2075 6e69 7175  t("TRA: ", uniqu
+00000b40: 655f 7472 6166 6f73 290a 2020 2020 2020  e_trafos).      
+00000b50: 2020 2020 2020 6973 6f6b 3120 3d20 6c65        isok1 = le
+00000b60: 6e28 756e 6971 7565 5f73 6373 2920 3d3d  n(unique_scs) ==
+00000b70: 2037 2061 6e64 2075 6e69 7175 655f 7472   7 and unique_tr
+00000b80: 6166 6f73 5b34 5d5b 325d 5b32 5d20 3d3d  afos[4][2][2] ==
+00000b90: 2034 0a0a 2020 2020 2020 2020 6966 2063   4..        if c
+00000ba0: 6173 6520 3d3d 2032 3a20 2353 696d 706c  ase == 2: #Simpl
+00000bb0: 6520 6375 6269 630a 2020 2020 2020 2020  e cubic.        
+00000bc0: 2020 2020 613d 332e 310a 2020 2020 2020      a=3.1.      
+00000bd0: 2020 2020 2020 696e 6465 7820 3d20 340a        index = 4.
+00000be0: 2020 2020 2020 2020 2020 2020 6365 6c6c              cell
+00000bf0: 203d 206e 702e 6172 7261 7928 5b5b 312c   = np.array([[1,
+00000c00: 302c 305d 2c5b 302c 312c 305d 2c5b 302c  0,0],[0,1,0],[0,
+00000c10: 302c 315d 5d29 0a20 2020 2020 2020 2020  0,1]]).         
+00000c20: 2020 2070 6f73 6974 696f 6e73 203d 206e     positions = n
+00000c30: 702e 6172 7261 7928 5b5b 302c 302c 305d  p.array([[0,0,0]
+00000c40: 5d29 0a20 2020 2020 2020 2020 2020 2073  ]).            s
+00000c50: 6974 6573 203d 205b 5b31 322c 3133 5d5d  ites = [[12,13]]
+00000c60: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00000c70: 7320 3d20 4174 6f6d 7328 6365 6c6c 3d63  s = Atoms(cell=c
+00000c80: 656c 6c2a 612c 2070 6f73 6974 696f 6e73  ell*a, positions
+00000c90: 3d70 6f73 6974 696f 6e73 2a61 290a 0a20  =positions*a).. 
+00000ca0: 2020 2020 2020 2020 2020 2070 6c20 3d20             pl = 
+00000cb0: 5061 7265 6e74 4c61 7474 6963 6528 7072  ParentLattice(pr
+00000cc0: 6973 2c20 7369 7465 733d 7369 7465 732c  is, sites=sites,
+00000cd0: 2070 6263 3d28 312c 312c 3129 290a 0a20   pbc=(1,1,1)).. 
+00000ce0: 2020 2020 2020 2020 2020 2075 6e69 7175             uniqu
+00000cf0: 655f 7363 732c 2075 6e69 7175 655f 7472  e_scs, unique_tr
+00000d00: 6166 6f73 203d 2075 7469 6c73 2e67 6574  afos = utils.get
+00000d10: 5f75 6e69 7175 655f 7375 7065 7263 656c  _unique_supercel
+00000d20: 6c73 2869 6e64 6578 2c70 6c29 0a0a 2020  ls(index,pl)..  
+00000d30: 2020 2020 2020 2020 2020 7373 6574 203d            sset =
+00000d40: 2053 7472 7563 7475 7265 7353 6574 2870   StructuresSet(p
+00000d50: 6c29 0a20 2020 2020 2020 2020 2020 2066  l).            f
+00000d60: 6f72 2074 2069 6e20 756e 6971 7565 5f74  or t in unique_t
+00000d70: 7261 666f 733a 0a20 2020 2020 2020 2020  rafos:.         
+00000d80: 2020 2020 2020 2073 6365 6c6c 203d 2053         scell = S
+00000d90: 7570 6572 4365 6c6c 2870 6c2c 7429 0a20  uperCell(pl,t). 
+00000da0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00000db0: 7365 742e 6164 645f 7374 7275 6374 7572  set.add_structur
+00000dc0: 6528 5374 7275 6374 7572 6528 7363 656c  e(Structure(scel
+00000dd0: 6c2c 7363 656c 6c2e 6765 745f 6174 6f6d  l,scell.get_atom
+00000de0: 6963 5f6e 756d 6265 7273 2829 292c 7772  ic_numbers()),wr
+00000df0: 6974 655f 746f 5f64 6220 3d20 5472 7565  ite_to_db = True
+00000e00: 290a 0a20 2020 2020 2020 2020 2020 2073  )..            s
+00000e10: 7365 742e 7365 7269 616c 697a 6528 7061  set.serialize(pa
+00000e20: 7468 3d22 7465 7374 5f67 6574 5f75 6e69  th="test_get_uni
+00000e30: 7175 655f 7375 7065 7263 656c 6c73 2d73  que_supercells-s
+00000e40: 632e 6a73 6f6e 2229 0a20 2020 2020 2020  c.json").       
+00000e50: 2020 2020 2070 7269 6e74 2822 466f 756e       print("Foun
+00000e60: 6420 222c 6c65 6e28 756e 6971 7565 5f73  d ",len(unique_s
+00000e70: 6373 292c 2022 2075 6e69 7175 6520 484e  cs), " unique HN
+00000e80: 4673 2066 6f72 2061 2073 696d 706c 6520  Fs for a simple 
+00000e90: 6375 6269 6320 6c61 7474 6963 6520 6f66  cubic lattice of
+00000ea0: 2069 6e64 6578 2022 2c69 6e64 6578 290a   index ",index).
+00000eb0: 2020 2020 2020 2020 2020 2020 2370 7269              #pri
+00000ec0: 6e74 2822 5343 533a 2022 2c20 756e 6971  nt("SCS: ", uniq
+00000ed0: 7565 5f73 6373 290a 2020 2020 2020 2020  ue_scs).        
+00000ee0: 2020 2020 2370 7269 6e74 2822 5452 413a      #print("TRA:
+00000ef0: 2022 2c20 756e 6971 7565 5f74 7261 666f   ", unique_trafo
+00000f00: 7329 0a20 2020 2020 2020 2020 2020 2069  s).            i
+00000f10: 736f 6b32 203d 206c 656e 2875 6e69 7175  sok2 = len(uniqu
+00000f20: 655f 7363 7329 203d 3d20 3920 616e 6420  e_scs) == 9 and 
+00000f30: 756e 6971 7565 5f73 6373 5b34 5d5b 325d  unique_scs[4][2]
+00000f40: 5b32 5d20 3d3d 2031 322e 340a 0a20 2020  [2] == 12.4..   
+00000f50: 2061 7373 6572 7420 6973 6f6b 3020 616e   assert isok0 an
+00000f60: 6420 6973 6f6b 3120 616e 6420 6973 6f6b  d isok1 and isok
+00000f70: 320a                                     2.
```

### Comparing `clusterX-1.0.0.dev8/clusterx/test/test_structure_selector.py` & `clusterX-2.1.0rc1/clusterx/test/test_structure_selector.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,30 +41,33 @@
         [2,0,0]]
     pbc = [True,True,False]
 
     pri = Atoms(['H','H','H'], positions=positions, cell=cell, pbc=pbc)
     su1 = Atoms(['C','H','H'], positions=positions, cell=cell, pbc=pbc)
     su2 = Atoms(['H','He','H'], positions=positions, cell=cell, pbc=pbc)
     su3 = Atoms(['H','N','H'], positions=positions, cell=cell, pbc=pbc)
-    
+
     plat = ParentLattice(pri,substitutions=[su1,su2,su3],pbc=pbc)
     """
     #cpool = ClustersPool(plat, npoints=[0,1,2,3,4], radii=[0,0,2.3,1.42,1.42])
     cpool = ClustersPool(plat, npoints=[1,2], radii=[0,1.1])
-    
+
     cpool.write_clusters_db(cpool.get_cpool(),cpool.get_cpool_scell(),"cpool.json")
     corrcal = CorrelationsCalculator("trigonometric", plat, cpool)
 
     scell = SuperCell(plat,np.array([(3,0,0),(0,3,0),(0,0,1)]))
-    training_set = StructuresSet(plat, filename="test_structure_selection_training_set.json")
+    #training_set = StructuresSet(plat, filename="test_structure_selection_training_set.json")
+    training_set = StructuresSet(plat)
     ntrainingstr = 14
-    
+
     for idx in range(ntrainingstr):
         training_set.add_structure(scell.gen_random(nsubs={0:[5]}))
-    
+
+    training_set.serialize(path="test_structure_selection_training_set.json", overwrite=True)
+
     structure_selector = StructureSelector(cluster_pool = cpool, training_set = training_set)
 
     comat = corrcal.get_correlation_matrix(training_set)
     covariance_matrix_inv = np.dot(comat.T, comat)
 
     'Test 1'
     covariance_correct = np.allclose(np.identity(len(cpool)), np.dot(structure_selector._covariance_matrix, covariance_matrix_inv))
@@ -92,77 +95,80 @@
 
         if not(isinstance(tau, float)):
             print('tau is no float!')
             sys.exit()
         elif(tau < 0):
             print('tau is negative!')
             sys.exit()
-        
+
     'Test 4'
     test_str = 'global_averagedConcentration'
     'TODO: WHAT IS THE DIIFERENCE BETWEEN is AND ==???'
     if(test_str.replace('global_','') is 'averagedConcentration'):
         print(test_str[7:])
         print('Test for transmitting domain_matrix_method failed!')
         sys.exit()
 
     test_str = 'global_averagedConcentration'
     global_or_greedy = test_str[:6]
     if not (global_or_greedy == 'global'):
         print('Second transmitting test failed as well.')
         sys.exit()
 
-    'Test 5'    
+    'Test 5'
 
-    candidate_set = StructuresSet(plat, filename="test_structure_selection_candidate_set.json")
+    #candidate_set = StructuresSet(plat, filename="test_structure_selection_candidate_set.json")
+    candidate_set = StructuresSet(plat)
     ncandidatestr = 6
     for idx in range(ncandidatestr):
         candidate_set.add_structure(scell.gen_random(nsubs={0:[5]}))
 
-        
+    candidate_set.serialize(path="test_structure_selection_candidate_set.json", overwrite=False, rm_vac=False)
+
     structure_selector.set_candidate_set(candidate_set)
     method_list = ['global_averagedConcentration', 'global_infiniteCrystalFiniteClusters', 'global_byConcentration', 'global_vdWalleAndCeder', 'greedy']
-    for method in method_list:                   
+    for method in method_list:
         structure = candidate_set.get_structure(structure_selector.select_structure(method = method, concentration = 0.2))
         if not(isinstance(structure, Structure)):
             print('Returned structure is not structure object! "structure_selector.select_structure()"')
             sys.exit()
 
     'Test 6'
     'Does this selection optimally reduce the selector criterion with the tau?'
     method_list = ['global_averagedConcentration', 'global_infiniteCrystalFiniteClusters', 'global_byConcentration', 'global_vdWalleAndCeder', 'greedy']
     for method in method_list:
         structure_idx = structure_selector.select_structure(method = method, concentration = 0.2)
         if(method == 'greedy'):
-            print('Do not worry about the next error msg.')
-        
+            print('Ignore next error msgs.')
+
         try:
             calculate_tau_method = method[7:]
 
             tau = np.zeros(ncandidatestr)
             for candidate_idx in range(ncandidatestr):
                 candidate = candidate_set.get_structure(candidate_idx)
                 dummy_file_str = "test_structure_selection_dummy_set"+str(candidate_idx)+".json"
-                dummy_set = StructuresSet(plat, filename=dummy_file_str)
-                dummy_set.add_structures(json_db_filepath = "test_structure_selection_training_set.json") 
-                dummy_set.add_structure(candidate, write_to_db = True)
+                dummy_set = StructuresSet(plat)
+                dummy_set.add_structures(structures = "test_structure_selection_training_set.json")
+                dummy_set.add_structure(candidate)
+                dummy_set.serialize(path="test_structure_selection_dummy_set"+str(candidate_idx)+".json", overwrite=True)
                 dummy_structure_selector = StructureSelector(cluster_pool = cpool, training_set = dummy_set)
                 tau[candidate_idx] = dummy_structure_selector.calculate_population_variance(domain_calculation_method = calculate_tau_method, concentration = 0.2)
-            
+
             structure_chosen = np.argmin(tau)
 
             if not(structure_chosen == structure_idx):
                 print('structure selection failed. Criteria are not optimally reducing prediction variance according to themselves.')
                 print(structure_chosen)
                 print(structure_idx)
                 print(method)
                 sys.exit()
             else:
                 print('Test succeeded')
-            
+
         except:
             pass
 
 
     'Test 7'
 
     test = True
@@ -187,10 +193,7 @@
 
     if not(test):
         print('Calculate domain matrix reacts unexpectedly.')
         sys.exit()
 
     domain_matrix = structure_selector._calculate_domain_matrix(method = 'byConcentration', concentration = 0.2)
     print(domain_matrix)
-    
-
-
```

### Comparing `clusterX-1.0.0.dev8/clusterx/test/test_metropolis.py` & `clusterX-2.1.0rc1/clusterx/test/test_metropolis.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from ase.spacegroup import crystal
 from clusterx.parent_lattice import ParentLattice
 from clusterx.super_cell import SuperCell
 from clusterx.clusters.clusters_pool import ClustersPool
 from clusterx.clusters.cluster import Cluster
 from clusterx.correlations import CorrelationsCalculator
 from clusterx.model import Model
-from clusterx.monte_carlo import MonteCarlo
-from clusterx.monte_carlo import MonteCarloTrajectory
+from clusterx.thermodynamics.monte_carlo import MonteCarlo
+from clusterx.thermodynamics.monte_carlo import MonteCarloTrajectory
 from clusterx.utils import isclose
 from clusterx.utils import dict_compare
 
 from ase.data import atomic_numbers as cn
 from ase import Atoms
 import numpy as np
 import os
@@ -116,105 +116,160 @@
     cpoolBonds = ClustersPool(plat, npoints=[0,1], radii=[0,0])
     corcBonds = CorrelationsCalculator("binary-linear", plat, cpoolBonds)
 
     multB=[1,24,16,6]
     cemodelBkk=Model(corcBonds, 'bond_kk', ecis=np.multiply(ecisBkk, multB))
     cemodelBii=Model(corcBonds, 'bond_ii', ecis=np.multiply(ecisBii, multB))
 
-    mc = MonteCarlo(cemodelE, scellE, nsubs, models = [cemodelBkk, cemodelBii])
+    mc = MonteCarlo(cemodelE, scellE, ensemble = "canonical", nsubs = nsubs, models = [cemodelBkk, cemodelBii])
 
     nmc=50
     # Boltzmann constant in Ha/K
     kb = float(3.16681009610757e-6)
     # temperature in K
     temp = 1000
-
+    info_units = {'temp':'K','kb':'Ha/K','energy':'Ha','scale_factor':None}
+    
     print("Samplings steps",nmc)
     print("Temperature",temp)
-
-    traj = mc.metropolis([kb,temp], nmc, write_to_db = True)
+    scale_factor = None
+    traj = mc.metropolis(scale_factor, nmc, temp, kb, serialize = True, info_units = info_units)
 
     steps = traj.get_sampling_step_nos()
-    energies = traj.get_model_total_energies()
-
-    #traj.write_to_file()
+    energies = traj.get_energies()
 
     structure = traj.get_structure(0)
     print("Initial structure: ",structure.decor)
 
-    bondskk1 = traj.get_model_properties('bond_kk')
-    bondsii1 = traj.get_model_properties('bond_ii')
+    bondskk1 = traj.get_properties('bond_kk')
+    bondsii1 = traj.get_properties('bond_ii')
     print(bondskk1)
     print(bondsii1)
 
     print("Total energy at sampling step", steps[2], ": ", energies[2])
     struc1 = traj.get_structure_at_step(steps[2])
     print("Decoration at sampling step", steps[2],": ", struc1.decor)
     decoration1 = struc1.decor
     print("Decoration at sampling step", steps[2], "read from atoms object: ", struc1.get_atomic_numbers())
     struc1.serialize(fname="configuration2.json")
 
-    strucmin = traj.get_lowest_non_degenerate_structure()
+    strucmin = traj.get_lowest_energy_structure()
     print("\nDecoration with the lowest energy: ", strucmin.get_atomic_numbers())
     print("Energy of this structure: ", min(energies))
     strucmin.serialize(fname="lowest-non-generate-configuration.json")
 
     print("Configurations accepted at steps: ",steps)
     last_sampling_entry = traj.get_sampling_step_entry_at_step(steps[-1])
     last_structure = traj.get_structure_at_step(steps[-1])
 
-    rsteps = [0, 1, 2, 3, 4, 6, 10, 11, 16, 17, 18, 26, 27, 34, 37, 38, 44, 45, 47, 48, 50]
-    renergies = [-77652.59664207128, -77652.61184305252, -77652.62022569243, -77652.61912760629, -77652.62737663009, -77652.63009501049, -77652.63158443688, -77652.64240196907, -77652.64240196907, -77652.64348105107, -77652.64714764676, -77652.64959679516, -77652.64959679516, -77652.65458138083, -77652.66173231734, -77652.65458138083, -77652.65946542152, -77652.6702829537, -77652.66812810961, -77652.67298251796, -77652.66622624162]
-    rlast_decoration = np.int8([14, 14, 13, 14, 14, 13, 14, 14, 14, 13, 13, 14, 14, 14, 13, 14, 14, 14, 13, 13, 14, 13, 14, 14, 13, 14, 14, 14, 14, 14, 14, 13, 13, 14, 14, 14, 13, 14, 13, 14, 13, 13, 14, 14, 13, 14, 56, 56, 56, 56, 56, 56, 56, 56])
-    rlast_sampling_entry = {'sampling_step_no': 50, 'model_total_energy': -77652.66622624162, 'swapped_positions': [[5, 43]], 'key_value_pairs': {'bond_kk': 2.49116603472051, 'bond_ii': 2.397621971688995}}
+    #rsteps = [0, 1, 2, 3, 4, 6, 10, 11, 16, 17, 18, 26, 27, 34, 37, 38, 44, 45, 47, 48, 50]
+    rsteps = [0, 1, 2, 3, 4, 5, 10, 11, 14, 16, 18, 19, 22, 24, 26, 31, 34, 37, 38, 43, 45]
+#    print("energies",energies)
+    print("steps", steps)
+    print("last_structure.decor",last_structure.decor)
+    print(last_sampling_entry)
+    
+    #renergies = [-77652.59664207128, -77652.61184305252, -77652.62022569243, -77652.61912760629, -77652.62737663009, -77652.63009501049, -77652.63158443688, -77652.64240196907, -77652.64240196907, -77652.64348105107, -77652.64714764676, -77652.64959679516, -77652.64959679516, -77652.65458138083, -77652.66173231734, -77652.65458138083, -77652.65946542152, -77652.6702829537, -77652.66812810961, -77652.67298251796, -77652.66622624162]
+    renergies = [-77652.59664207, -77652.61184305, -77652.62022569, -77652.61912761, -77652.62737663, -77652.63941161, -77652.6413147, -77652.6413147, -77652.6413147, -77652.64023562, -77652.63585217, -77652.63585217, -77652.63369732, -77652.62652738, -77652.63709316, -77652.64142517, -77652.63927033, -77652.6445384, -77652.64132329, -77652.64132329, -77652.65963884]
+    #rlast_decoration = np.int8([14, 14, 13, 14, 14, 13, 14, 14, 14, 13, 13, 14, 14, 14, 13, 14, 14, 14, 13, 13, 14, 13, 14, 14, 13, 14, 14, 14, 14, 14, 14, 13, 13, 14, 14, 14, 13, 14, 13, 14, 13, 13, 14, 14, 13, 14, 56, 56, 56, 56, 56, 56, 56, 56])
+    rlast_decoration = np.int8([14, 14, 14, 13, 14, 13, 14, 14, 14, 14, 13, 13, 14, 14, 14, 14, 14, 13, 13, 13, 14, 14, 13, 14, 13, 14, 14, 14, 13, 14, 13, 14, 14, 14, 14, 13, 14, 14, 14, 14, 13, 13, 14, 14, 13, 13, 56, 56, 56, 56, 56, 56, 56, 56])
+    #rlast_sampling_entry = {'sampling_step_no': 50, 'model_total_energy': -77652.66622624162, 'swapped_positions': [[5, 43]], 'key_value_pairs': {'bond_kk': 2.49116603472051, 'bond_ii': 2.397621971688995}}
+    rlast_sampling_entry = {'sampling_step_no': 45, 'energy': -77652.65963884031, 'swapped_positions': [[3, 25]], 'key_value_pairs': {'bond_kk': 2.4897160745744795, 'bond_ii': 2.3909922581598044}}
+
+    rtraj_info={'number_of_sampling_steps': nmc, 'temperature': temp, 'boltzmann_constant': kb}
+    rtraj_info.update({'info_units':info_units})
+    print(rtraj_info)
+    traj_info={}
+    traj_info.update({'number_of_sampling_steps': traj._nmc})
+    traj_info.update({'temperature': traj._temperature})
+    traj_info.update({'boltzmann_constant': traj._boltzmann_constant})
+    if traj._scale_factor is not None:
+        traj_info.update({'scale_factor': traj._scale_factor})
+    if traj._acceptance_ratio is not None:
+        traj_info.update({'scale_factor': traj._acceptance_ratio})
+    for key in traj._keyword_arguments:
+        traj_info.update({key:traj._keyword_arguments[key]})
+    print(traj_info)
 
-    isok1 = isclose(rsteps,steps) and isclose(renergies, energies) and isclose(rlast_decoration,last_structure.decor) and dict_compare(last_sampling_entry, rlast_sampling_entry, tol=float(1e-7) )
+    isok1 = isclose(rsteps,steps) and isclose(renergies, energies) and isclose(rlast_decoration,last_structure.decor) and dict_compare(last_sampling_entry, rlast_sampling_entry, tol=float(1e-7) ) and dict_compare(traj_info,rtraj_info)
     assert(isok1)
-
+    #assert(True)
+    
+    print("before set none", traj.get_properties('bond_kk'))
+    print("before set none", traj.get_properties('bond_ii'))
     traj._models =[]
     for i in range(len(traj._trajectory)):
         traj._trajectory[i]['key_value_pairs']={}
 
-    bondskk2 = traj.get_model_properties('bond_kk')
-    bondsii2 = traj.get_model_properties('bond_ii')
+    bondskk2 = traj.get_properties('bond_kk')
+    bondsii2 = traj.get_properties('bond_ii')
     print(bondskk2)
     print(bondsii2)
 
-    traj.calculate_model_properties([cemodelBkk,cemodelBii])
+    traj.calculate_properties([cemodelBkk,cemodelBii])
 
     print("Cluster expansion models for the properties: ",[mo.property for mo in traj._models])
 
     #Tests of functions in MonteCarloTrajector
     print("\nTests of functions in MonteCarloTrajector:")
-    ids = traj.get_id_sampling_step(steps[2])
+    ids = traj.get_nid_sampling_step(steps[2])
     print(ids)
-    prop_at_id = traj.get_model_property(2,'bond_kk')
+    prop_at_id = traj.get_property(2,'bond_kk')
     print(prop_at_id)
-    stepx = traj.get_id('bond_kk',2.4772699399288944)
+    stepx = traj.get_nids('bond_kk',2.4772699399288944)
     print(stepx)
-    stepx = traj.get_id('model_total_energy',-77652.65458138083)
+    stepx = traj.get_nids('energy',-77652.65458138083)
     print(stepx)
 
-    bondskk = traj.get_model_properties('bond_kk')
-    bondsii = traj.get_model_properties('bond_ii')
-
-    rbondskk = [2.4772699399288944, 2.4772699399288944, 2.4772699399288944, 2.4787199000749247, 2.4648238052830997, 2.4648238052830997, 2.4787199000749247, 2.4787199000749247, 2.4787199000749247, 2.4787199000749247, 2.49116603472051, 2.5036121693663045, 2.5036121693663045, 2.49116603472051, 2.4787199000749247, 2.49116603472051, 2.5036121693663045, 2.5036121693663045, 2.4897160745744795, 2.4772699399288944, 2.49116603472051]
-    rbondsii = [2.400461156502162, 2.400461156502162, 2.400461156502162, 2.4070908700313525, 2.4099300548444713, 2.4099300548444713, 2.4070908700313525, 2.4070908700313525, 2.4070908700313525, 2.4070908700313525, 2.397621971688995, 2.3881530733466856, 2.3881530733466856, 2.397621971688995, 2.4070908700313525, 2.397621971688995, 2.3881530733466856, 2.3881530733466856, 2.3909922581598044, 2.400461156502162, 2.397621971688995]
+    bondskk = traj.get_properties('bond_kk')
+    bondsii = traj.get_properties('bond_ii')
+    print("2",bondskk,bondsii)
+    
+
+    #rbondskk=[2.4772699399288944, 2.4772699399288944, 2.4772699399288944, 2.4787199000749247, 2.4648238052830997, 2.4648238052830997, 2.4787199000749247, 2.4787199000749247, 2.4787199000749247, 2.4787199000749247, 2.49116603472051, 2.5036121693663045, 2.5036121693663045, 2.49116603472051, 2.4787199000749247, 2.49116603472051, 2.5036121693663045, 2.5036121693663045, 2.4897160745744795, 2.4772699399288944, 2.49116603472051]
+    rbondskk = [2.47726994, 2.47726994, 2.47726994, 2.4787199,  2.46482381, 2.46482381, 2.4787199, 2.4787199, 2.4787199, 2.4787199, 2.4787199, 2.4787199, 2.46482381, 2.4787199, 2.4787199, 2.49116603, 2.47726994, 2.46482381, 2.47726994, 2.47726994, 2.48971607]
+    #rbondsii = [2.400461156502162, 2.400461156502162, 2.400461156502162, 2.4070908700313525, 2.4099300548444713, 2.4099300548444713, 2.4070908700313525, 2.4070908700313525, 2.4070908700313525, 2.4070908700313525, 2.397621971688995, 2.3881530733466856, 2.3881530733466856, 2.397621971688995, 2.4070908700313525, 2.397621971688995, 2.3881530733466856, 2.3881530733466856, 2.3909922581598044, 2.400461156502162, 2.397621971688995]
+    rbondsii = [2.40046116, 2.40046116, 2.40046116, 2.40709087, 2.40993005, 2.40993005, 2.40709087, 2.40709087, 2.40709087, 2.40709087, 2.40709087, 2.40709087, 2.40993005, 2.40709087, 2.40709087, 2.39762197, 2.40046116, 2.40993005, 2.40046116, 2.40046116, 2.39099226]
 
     isok2 = isclose(rbondskk,bondskk) and isclose(rbondsii,bondsii)
     assert(isok2)
 
+    cp = traj.calculate_average_property(prop_name = 'C_p', no_of_equilibration_steps = 2)
+    u = traj.calculate_average_property(prop_name = 'U', no_of_equilibration_steps = 2)
+    avg_bond_kk = traj.calculate_average_property(prop_name = 'bond_kk', no_of_equilibration_steps = 2)
+    avg_bond_ii = traj.calculate_average_property(prop_name = 'bond_ii', no_of_equilibration_steps = 2)
+    u2 = traj.calculate_average_property(prop_name = 'energy', no_of_equilibration_steps = 2)
+    averages1 = [cp, u, avg_bond_kk, avg_bond_ii, u2]
+    print("averages1",cp,u, avg_bond_kk, avg_bond_ii, u2)
+    raverages1 = [7.939914262878631, -77652.64031004661, 2.4779505334667857, 2.4035730628525886, -77652.64031004661]
+    
+    def test_average(prop_array, **kwargs):
+        bondskk = np.average(prop_array[0])
+        bondsii = np.average(prop_array[1])
+        energy = np.average(prop_array[2])
+        temperature = float(kwargs['temperature'])
+        return  bondskk, bondsii, energy, (bondsii+bondskk)/(1.0*2), energy/(1.0*temperature)
+    
+    avg_bond_kk2, avg_bond_ii2, u3, avg_bond, ut = traj.calculate_average_property(average_func=test_average, no_of_equilibration_steps = 2, props_list=['bond_kk','bond_ii','energy'], temperature = traj._temperature )
+    averages2 = [avg_bond_kk2, avg_bond_ii2, u3, avg_bond, ut]
+    print("averages2", avg_bond_kk2, avg_bond_ii2, u3, avg_bond, ut)
+    raverages2 = [2.4779505334667884, 2.403573062852589, -77652.64031004666, 2.4407617981596887, -77.65264031004665]
+
+    isok22 = isclose(averages1,raverages1) and isclose(averages2,raverages2)
+    assert(isok22)
+    
+
     trajx = MonteCarloTrajectory()
 
     if os.path.isfile("trajectory.json"):
         trajx.read()
         #print(trajx._trajectory[0])
         #print(trajx._scell._plat.get_nsites_per_type())
 
-        energies2 = trajx.get_model_total_energies()
+        energies2 = trajx.get_energies()
         steps2 = trajx.get_sampling_step_nos()
 
         struc2 = trajx.get_structure_at_step(steps2[2])
         decoration2 = struc2.decor
         last_sampling_entry2 = trajx.get_sampling_step_entry_at_step(steps2[-1])
 
         isok3 = isclose(renergies, energies2) and isclose(decoration2,decoration1) and isclose(steps2,rsteps) and dict_compare(last_sampling_entry,last_sampling_entry2, tol = float(1.0e-7))
@@ -265,62 +320,84 @@
         23.09
     ]
 
     cemodelE2=Model(corcE2, "energy2",ecis=np.multiply(ecisE2, smultT2))
 
     # Sampling in sublattice with index 0 - ternary sampling
     print("Start sampling in sublattice with index 0:")
-    mc2 = MonteCarlo(cemodelE2, scellE2, {0:[112,16],1:[0]}, sublattice_indices=[0], filename = "trajectory-ternary.json")
+    mc2 = MonteCarlo(cemodelE2, scellE2, ensemble = "canonical", nsubs = {0:[112,16],1:[0]})
 
     nmc=30
     # temperature in K
     temp = 600
     print("Samplings steps ",nmc)
     print("Temperature ",temp)
 
-    traj2 = mc2.metropolis([kb,temp], nmc)
+    traj2 = mc2.metropolis(scale_factor, nmc, temp, kb, serialize = True, filename = "trajectory-ternary.json")
 
     steps2 = traj2.get_sampling_step_nos()
-    energies2 = traj2.get_model_total_energies()
+    energies2 = traj2.get_energies()
     last_entry2 = traj2.get_sampling_step_entry_at_step(steps2[-1])
     last_structure2 = traj2.get_structure_at_step(steps2[-1])
 
-    traj2.write_to_file()
+    traj2.serialize()
+    print(last_structure2.decor)
 
     print("Configurations accepted at steps: ",steps2)
 
-    rsteps2 = [0, 1, 3, 7, 8, 12, 14, 18, 21, 23, 24, 25, 26, 28, 29, 30]
-    renergies2 = [-634734.608306379, -634734.608306379, -634734.608306379, -634734.620985871, -634734.620985871, -634734.620985871, -634734.620985871, -634734.620985871, -634734.620985871, -634734.633665363, -634734.633665363, -634734.6683063792, -634734.6683063792, -634734.680985871, -634734.680985871, -634734.7156268872]
-
-    rlast_entry2={'sampling_step_no': 30, 'model_total_energy': -634734.7156268872, 'swapped_positions': [[351, 4]], 'key_value_pairs': {}}
-    rlast_decoration2 = np.int8([14, 14, 14, 14, 13, 14, 14, 14, 14, 14, 14, 13, 14, 14, 14, 14, 14, 13, 14, 13,  0, 13, 14, 14, 14, 13, 14, 13, 13, 13, 14, 13, 13, 13, 14, 13, 13, 14, 14, 14, 14, 14, 14, 13, 14, 13, 56, 56, 56, 56, 56, 56, 56, 56,
-                                 13, 13, 14, 14, 14, 14, 14, 13, 14, 14, 14, 14, 13, 14, 13, 13,  0, 13, 13, 14, 14, 13, 14, 13, 14, 13, 13, 14, 13, 14,  0, 14, 14, 14, 14, 13, 14, 13, 14, 14, 13, 13, 14, 14, 14, 14, 56, 56, 56, 56, 56, 56, 56, 56,
-                                 14, 13, 13, 14, 14, 13, 14,  0, 14, 14, 14, 13, 14,  0, 14, 14, 14, 14, 13, 14, 13, 14, 14,  0, 14, 14, 13, 13, 13, 13, 14, 13, 14, 14, 14, 13, 14, 14, 13, 14,  0, 14, 13, 14, 14, 14, 56, 56, 56, 56, 56, 56, 56, 56,
-                                 14, 13, 14, 14, 13, 14, 14, 13, 14, 14, 14, 14, 14, 13, 14, 13, 14, 14, 13, 14, 14, 14, 13, 14, 13, 14, 14, 13, 14, 14, 14, 14, 14, 14, 14, 13, 13, 14, 14, 14, 14, 13, 14, 14, 14, 14, 56, 56, 56, 56, 56, 56, 56, 56,
-                                 14, 14, 14, 14, 13, 14, 14, 14, 13, 14, 14, 13, 14, 13, 14, 14, 14, 13, 13, 13, 14, 14, 14, 13, 14, 14, 14,  0, 14,  0,  0, 14, 13, 14, 13, 13, 13, 14, 13, 14, 14, 14, 14, 14, 14, 13, 56, 56, 56, 56, 56, 56, 56, 56,
-                                 13, 14, 13, 13, 13, 14, 14, 14, 14, 13, 14, 13, 14, 14, 14, 14, 14, 14, 13, 14, 14, 14, 14, 14, 13, 14, 14, 14, 14, 14, 14, 13, 14, 13, 14, 13, 14, 13, 13, 14,  0,  0, 14, 14, 14, 14, 56, 56, 56, 56, 56, 56, 56, 56,
-                                 14, 14, 13, 14, 14, 14, 13, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 13, 14, 14, 14, 13, 13, 14, 14,  0, 13, 14, 14, 13, 13, 14, 13, 14, 13, 13, 13, 14, 13, 13, 13, 14, 14, 14, 56, 56, 56, 56, 56, 56, 56, 56,
-                                 14, 14, 14, 13, 14, 14, 13, 14, 14,  0, 14, 14, 13, 14, 13, 14, 14, 14, 14, 14, 14, 13, 14, 14, 13, 14, 14, 14, 14, 14, 14, 14,  0, 14, 14, 13, 14, 13,  0, 14, 13, 13, 14, 13, 14, 14, 56, 56, 56, 56, 56, 56, 56, 56])
+    #rsteps2 = [0, 1, 3, 7, 8, 12, 14, 18, 21, 23, 24, 25, 26, 28, 29, 30]
+    rsteps2 = [0, 1, 3, 7, 8, 10, 12, 16, 17, 22, 23, 24, 25, 26, 29]
+    #renergies2 = [-634734.608306379, -634734.608306379, -634734.608306379, -634734.620985871, -634734.620985871, -634734.620985871, -634734.620985871, -634734.620985871, -634734.620985871, -634734.633665363, -634734.633665363, -634734.6683063792, -634734.6683063792, -634734.680985871, -634734.680985871, -634734.7156268872]
+    renergies2 = [-634734.60830638, -634734.60830638, -634734.60830638, -634734.62098587, -634734.62098587, -634734.62098587, -634734.62098587, -634734.62098587, -634734.62098587, -634734.62098587, -634734.62098587, -634734.62098587, -634734.62098587, -634734.65562689, -634734.65562689]
+    #rlast_entry2={'sampling_step_no': 30, 'model_total_energy': -634734.7156268872, 'swapped_positions': [[351, 4]], 'key_value_pairs': {}}
+    rlast_entry2={'sampling_step_no': 29, 'energy': -634734.6556268871, 'swapped_positions': [[247, 243]], 'key_value_pairs': {}}
+    #rlast_decoration2 = np.int8([14, 14, 14, 14, 13, 14, 14, 14, 14, 14, 14, 13, 14, 14, 14, 14, 14, 13, 14, 13,  0, 13, 14, 14, 14, 13, 14, 13, 13, 13, 14, 13, 13, 13, 14, 13, 13, 14, 14, 14, 14, 14, 14, 13, 14, 13, 56, 56, 56, 56, 56, 56, 56, 56,
+    #                             13, 13, 14, 14, 14, 14, 14, 13, 14, 14, 14, 14, 13, 14, 13, 13,  0, 13, 13, 14, 14, 13, 14, 13, 14, 13, 13, 14, 13, 14,  0, 14, 14, 14, 14, 13, 14, 13, 14, 14, 13, 13, 14, 14, 14, 14, 56, 56, 56, 56, 56, 56, 56, 56,
+    #                             14, 13, 13, 14, 14, 13, 14,  0, 14, 14, 14, 13, 14,  0, 14, 14, 14, 14, 13, 14, 13, 14, 14,  0, 14, 14, 13, 13, 13, 13, 14, 13, 14, 14, 14, 13, 14, 14, 13, 14,  0, 14, 13, 14, 14, 14, 56, 56, 56, 56, 56, 56, 56, 56,
+    #                             14, 13, 14, 14, 13, 14, 14, 13, 14, 14, 14, 14, 14, 13, 14, 13, 14, 14, 13, 14, 14, 14, 13, 14, 13, 14, 14, 13, 14, 14, 14, 14, 14, 14, 14, 13, 13, 14, 14, 14, 14, 13, 14, 14, 14, 14, 56, 56, 56, 56, 56, 56, 56, 56,
+    #                             14, 14, 14, 14, 13, 14, 14, 14, 13, 14, 14, 13, 14, 13, 14, 14, 14, 13, 13, 13, 14, 14, 14, 13, 14, 14, 14,  0, 14,  0,  0, 14, 13, 14, 13, 13, 13, 14, 13, 14, 14, 14, 14, 14, 14, 13, 56, 56, 56, 56, 56, 56, 56, 56,
+    #                             13, 14, 13, 13, 13, 14, 14, 14, 14, 13, 14, 13, 14, 14, 14, 14, 14, 14, 13, 14, 14, 14, 14, 14, 13, 14, 14, 14, 14, 14, 14, 13, 14, 13, 14, 13, 14, 13, 13, 14,  0,  0, 14, 14, 14, 14, 56, 56, 56, 56, 56, 56, 56, 56,
+    #                             14, 14, 13, 14, 14, 14, 13, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 13, 14, 14, 14, 13, 13, 14, 14,  0, 13, 14, 14, 13, 13, 14, 13, 14, 13, 13, 13, 14, 13, 13, 13, 14, 14, 14, 56, 56, 56, 56, 56, 56, 56, 56,
+    #                             14, 14, 14, 13, 14, 14, 13, 14, 14,  0, 14, 14, 13, 14, 13, 14, 14, 14, 14, 14, 14, 13, 14, 14, 13, 14, 14, 14, 14, 14, 14, 14,  0, 14, 14, 13, 14, 13,  0, 14, 13, 13, 14, 13, 14, 14, 56, 56, 56, 56, 56, 56, 56, 56])
+    rlast_decoration2 = np.int8([14, 14, 14, 14,  0, 14, 14, 13, 14,  0, 14, 13, 14, 14, 14, 14, 14,  0, 14, 13, 13, 13, 14, 14, 14, 13, 14, 13, 13, 13, 14, 13, 13, 13, 14, 13, 14, 14, 14, 14, 14, 14, 14, 13, 14, 13, 56, 56, 56, 56, 56, 56, 56, 56,
+                                 13,  0, 14, 14, 14, 14, 14, 13, 14, 14, 14, 14, 13, 14,  0, 13, 13, 13, 13, 13, 14, 13, 14, 13, 14, 13, 13, 14, 13, 14,  0, 14, 14, 14, 14, 13, 14, 13, 14, 14, 13, 13, 14, 14, 14, 14, 56, 56, 56, 56, 56, 56, 56, 56,
+                                 14, 13, 13, 14, 13, 13, 14,  0, 14, 14, 14, 13, 14, 13, 14, 14, 14, 14, 13, 14, 13, 14, 14, 13, 14, 14, 13, 13, 13,  0, 14, 13, 14, 14, 14, 13, 14, 14, 13, 14,  0, 14, 13, 14, 14, 14, 56, 56, 56, 56, 56, 56, 56, 56,
+                                 14, 13, 14, 14, 13, 14, 14, 13, 14, 14, 14, 14, 14, 14, 14, 14, 13, 14, 13, 14, 14, 14, 14, 14, 13, 14, 14, 13, 14, 14, 14, 14, 14, 14, 14,  0, 13, 14, 14, 14, 14, 13, 14, 14, 14, 14, 56, 56, 56, 56, 56, 56, 56, 56,
+                                 14, 14, 14, 14, 13, 14, 14, 14, 13, 14, 14, 13, 14, 13, 14, 14, 14, 13, 13,  0, 14, 14, 14, 13, 14, 14, 14, 14, 14,  0, 13,  0, 13, 13, 13, 13, 13, 14, 13, 14, 14, 14, 14, 14, 14, 13, 56, 56, 56, 56, 56, 56, 56, 56,
+                                 13, 14, 13, 13, 13, 14, 14, 14, 14, 14, 14, 13, 14, 14, 14, 14, 14, 14, 13, 14, 14, 13, 14, 14, 13, 14, 14, 14, 14, 14, 14, 13, 14, 13, 14, 13, 14, 13, 13, 14,  0,  0, 14, 14, 14, 14, 56, 56, 56, 56, 56, 56, 56, 56,
+                                 14, 14, 13, 14, 14, 14, 13, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 13, 14, 14, 13, 13, 14, 13, 14, 13, 13, 14, 14, 13, 14, 14, 14, 14, 13, 13, 13, 14, 13, 13, 13, 14, 14, 14, 56, 56, 56, 56, 56, 56, 56, 56,
+                                 14, 14, 14, 13, 14, 14, 13, 14, 14, 14, 14, 14, 13, 14, 13, 14, 14, 14, 14, 14, 14, 13, 14, 14, 13, 14, 14, 14, 14, 14, 14, 14, 13, 14, 13, 14, 14, 13,  0, 14, 13, 13, 14, 13, 14, 14, 56, 56, 56, 56, 56, 56, 56, 56])
 
     isok4 = isclose(rsteps2,steps2) and isclose(renergies2, energies2) and isclose(last_structure2.decor,rlast_decoration2) and dict_compare(last_entry2,rlast_entry2, tol=float(1.0e-7))
     assert(isok4)
 
     # Sampling in the sublattices with indizes 0 and 1 - ternary sampling in sublattice 0 and binary sampling in sublattice 1
     print("\nStart sampling in the two sublattices with indices 0 and 1:")
     print("Samplings steps",nmc)
     print("Temperature",temp)
 
-    mc3 = MonteCarlo(cemodelE2, scellE2, {0:[112,16],1:[8]}, filename = "trajectory-multi-lattice.json", last_visited_structure_name = "last-visited-structure-mc-multi-lattice.json")
-    traj3 = mc3.metropolis([kb,temp], nmc, write_to_db = True)
+    mc3 = MonteCarlo(cemodelE2, scellE2,ensemble = "canonical", nsubs = {0:[112,16],1:[8]})
+    traj3 = mc3.metropolis(scale_factor, nmc, temp, kb, serialize = True, filename = "trajectory-multi-lattice.json")
 
     steps3 = traj3.get_sampling_step_nos()
-    energies3 = traj3.get_model_total_energies()
-
-    #traj3.write_to_file()
+    energies3 = traj3.get_energies()
+    print(steps3)
+    print(energies3)
 
     print("Configurations accepted at steps: ",steps3)
 
-    rsteps3 = [0, 1, 2, 4, 5, 7, 9, 10, 11, 12, 13, 14, 16, 17, 18, 20, 21, 22, 23, 24, 26, 27, 28]
-    renergies3 = [-634365.0390243438, -634365.0390243438, -634365.0590243443, -634365.0590243443, -634365.0590243443, -634365.0590243443, -634365.0590243443, -634365.1063448524, -634365.1063448524, -634365.1409858714, -634365.1536653634, -634365.1536653634, -634365.1536653634, -634365.1536653634, -634365.2229473958, -634365.2229473958, -634365.2483063795, -634365.2483063795, -634365.2483063795, -634365.2683063787, -634365.2883063791, -634365.2883063791, -634365.2883063791]
-
+    #rsteps3 = [0, 1, 2, 4, 5, 7, 9, 10, 11, 12, 13, 14, 16, 17, 18, 20, 21, 22, 23, 24, 26, 27, 28]
+    rsteps3 = [0, 1, 2, 4, 5, 7, 9, 10, 14, 15, 16, 17, 18, 19, 21, 23, 24, 25, 27, 28, 29]
+    #renergies3 = [-634365.0390243438, -634365.0390243438, -634365.0590243443, -634365.0590243443, -634365.0590243443, -634365.0590243443, -634365.0590243443, -634365.1063448524, -634365.1063448524, -634365.1409858714, -634365.1536653634, -634365.1536653634, -634365.1536653634, -634365.1536653634, -634365.2229473958, -634365.2229473958, -634365.2483063795, -634365.2483063795, -634365.2483063795, -634365.2683063787, -634365.2883063791, -634365.2883063791, -634365.2883063791]
+    renergies3 = [-634365.03902434, -634365.03902434, -634365.05902434, -634365.07902434, -634365.07902434, -634365.07902434, -634365.07902434, -634365.12634485, -634365.12634485, -634365.12634485, -634365.12634485, -634365.12634485, -634365.16098587, -634365.16098587, -634365.18634485, -634365.20634486, -634365.20634486, -634365.20634486, -634365.20634486, -634365.20634486, -634365.20634486]
+    
     isok5 = isclose(rsteps3,steps3) and isclose(renergies3, energies3)
     assert(isok5)
+
+
+    print ("\n\n========Test writing cluster expansion model========")
+
+    cemodelE.serialize(db_name = "model-clath.json")
+    cemodelEread = Model( json_db_filepath = "model-clath.json")
+    isok6 = isclose(np.multiply(ecisE, multT), cemodelEread.get_ecis()) and (cemodelE.property == 'energy') and (cemodelE.corrc.basis == 'binary-linear')
+    assert(isok6)
+
```

### Comparing `clusterX-1.0.0.dev8/clusterx/test/test_clusters_generation.py` & `clusterX-2.1.0rc1/clusterx/test/test_clusters_generation.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,253 +17,329 @@
 
     After successful execution of the test, the generated clusters may be visualized with the command::
 
         ase gui test_clusters_generation_#.json
 
     """
     tassert = True
-    #######################################################
-    # Part 1: 2D, radii.
-    #######################################################
-    """
-    print("\nPart I")
-    cell = [[3,0,0],
-            [0,1,0],
-            [0,0,5]]
-    positions = [
-        [0,0,0],
-        [1,0,0],
-        [2,0,0]]
-    pbc = [True,True,False]
-
-    pri = Atoms(['H','H','H'], positions=positions, cell=cell, pbc=pbc)
-    su1 = Atoms(['C','H','H'], positions=positions, cell=cell, pbc=pbc)
-    su2 = Atoms(['H','He','H'], positions=positions, cell=cell, pbc=pbc)
-    su3 = Atoms(['H','N','H'], positions=positions, cell=cell, pbc=pbc)
-
-    pl = ParentLattice(pri,substitutions=[su1,su2,su3],pbc=pbc)
-
-    cp = ClustersPool(pl, npoints=[1,2,3], radii=[0,2.1,2.1])
-    cp.write_clusters_db(db_name="test_clusters_generation_1.json")
-
-    print("\nMult: ", cp.get_multiplicities())
-    print("\nMult2: ", cp.get_cluster_multiplicities())
-
-    if tassert:
-        atom_idxs, atom_nrs = cp.get_cpool_arrays()
-    """
-    #######################################################
-    # Part 2: 1D, supercell.
-    #######################################################
-    print("Part II")
-    a=3.0
-    cell = np.array([[1,0,0],[0,4,0],[0,0,1]])
-    positions = np.array([[0,0,0],[0,1,0],[0,2,0],[0,3,0]])
-    sites = [[12,13],[12,13],[12,13],[12,13]]
-    pris = Atoms(cell=cell*a, positions=positions*a)
-
-    pl = ParentLattice(pris, sites=sites, pbc=(1,0,0))
-    sc = SuperCell(pl,[[4,0,0],[0,1,0],[0,0,1]])
-
-
-    cp = ClustersPool(pl,npoints=[1,2],super_cell=sc) # Here radii are not given, therefore all the clusters which can fit in the supercell are generated.
-    #cp = ClustersPool(pl,npoints=[0,1,2],radii=[0,0,3.9*a]) # Here radii are not given, therefore all the clusters which can fit in the supercell are generated.
-    cp.write_clusters_db(db_name="test_clusters_generation_2.json")
-
-    mult = cp.get_multiplicities()
-    radii = cp.get_all_radii()
-    npoints = cp.get_all_npoints()
-
-    #atom_idxs, atom_nrs = cp.get_cpool_arrays()
-    #print(atom_idxs[1][0],atom_idxs[7][0],atom_idxs[12][1],len(atom_nrs[17]),len(cp))
-
-    if tassert:
-        atom_idxs, atom_nrs = cp.get_cpool_arrays()
-        isok2 = atom_idxs[1][0] == 1 and atom_idxs[7][0] == 2 and atom_idxs[12][1] == 8 and len(atom_nrs[17]) == 2 and len(cp) == 18
-
-    #######################################################
-    # Part 3: FCC, radii.
-    #######################################################
-    print("Part III")
-
-    from ase.data import atomic_numbers as an
-    a=4.1
-    pris = bulk("Cu",crystalstructure="fcc", a=a)
-    sites = [[an["Cu"],an["Au"]]]
-    pl = ParentLattice(pris,sites=sites)
-
-    cp = ClustersPool(pl,npoints=[0,1,2,3],radii=[0,0,5.0,5.0])
-    cp.write_clusters_db(db_name="test_clusters_generation_3.json")
-
-    mult = cp.get_multiplicities()
-    npoints = cp.get_all_npoints()
-    radii = cp.get_all_radii()
-
-    rmult = np.array([1,1,6,3,8,12])
-    rnpoints = np.array([0,1,2,2,3,3])
-    rradii = np.array([0.       , 0.       , 2.8991378, 4.1      , 2.8991378, 4.1      ])
-
-    if tassert:
-        isok3 = len(cp) == 6 and (mult == rmult).all() and (npoints == rnpoints).all() and isclose(radii,rradii)
-
-    """
-    #######################################################
-    # Part 4: 2D cell with acute angle.
-    #######################################################
-    print("Part IV")
-    from ase.io import write
-
-    a=4.1
-    cell = np.array([[5,0,0],[4,1,0],[0,0,1]])
-    positions = np.array([[0,0,0],[1,0,0],[2,0,0],[3,0,0],[4,0,0]])
-    pbc = (1,1,0)
-    #sites = [[an["Cu"],an["Au"]]]*5
-    sites = [[an["Cu"],an["Au"]],[an["Cu"],an["Au"]],[12],[12],[12]]
-    pris = Atoms(cell=cell*a,positions=positions*a,pbc=pbc)
-    pl = ParentLattice(pris,sites=sites,pbc=pbc)
-
-    #cp = ClustersPool(pl,npoints=[0,1,2,3],radii=[0,0,4.5*a,4.5*a])
-    cp = ClustersPool(pl,npoints=[2],radii=[2.0*a])
-    write(filename="test_clusters_generation_scell_part4.json",images=cp.get_cpool_scell().get_atoms(),format="json")
-    cp.write_clusters_db(db_name="test_clusters_generation_4.json")
-
-    print("\nMult: ", cp.get_multiplicities())
-    print("\nMult2: ", cp.get_cluster_multiplicities())
-    if tassert:
-        atom_idxs, atom_nrs = cp.get_cpool_arrays()
-        isok4 = atom_idxs[2][0] == 30 and atom_idxs[3][1] == 16 and atom_idxs[4][0] == 10
-    """
-    #######################################################
-    # Part 5: Pt on O(111)
-    #######################################################
-    print("Part V")
-    from ase.io import write
-
-    cell = np.array([[2.785200119, 0.0, 0.0], [-1.3926000595, 2.4120540577, 0.0], [0.0, 0.0, 7.2740998268]])
-    positions = np.array([[0.0, 0.0, 2.274101], [1.392600, 0.804018, 0.0], [0.0, 0.0, 2.916914], [1.392600, 0.804018, 2.924188], [0.0, 1.608036, 2.931462]])
-    pbc = (1,1,0)
-    sites = [[78], [78], [0,8], [0,8], [0,8]]
-    pris = Atoms(cell=cell,positions=positions,pbc=pbc)
-    pl = ParentLattice(pris,sites=sites,pbc=pbc)
-
-    cp = ClustersPool(pl,npoints=[0,1,2,3],radii=[0,0,3.3,3.0])
-    #write(filename="test_clusters_generation_scell_part5.json",images=cp.get_cpool_scell().get_atoms(),format="json")
-    cp.write_clusters_db(db_name="test_clusters_generation_5.json")
-
-    mult = cp.get_multiplicities()
-    radii = cp.get_all_radii()
-    npoints = cp.get_all_npoints()
-
-    #print(repr(mult))
-    #print(repr(radii))
-    #print(repr(npoints))
-
-    mult_ref = np.array([1, 1, 1, 1, 3, 3, 3, 3, 3, 3, 3, 3, 3, 6, 3, 3, 3, 3, 3, 1, 3, 1, 1, 1, 1, 1])
-    radii_ref = np.array(
-        [0.        , 0.        , 0.        , 0.        , 1.60805243,
-        1.60805243, 1.60810181, 2.78520012, 2.78520012, 2.78520012,
-        3.21608028, 3.21608028, 3.21610496, 1.60810181, 2.78520012,
-        2.78520012, 2.78520012, 2.78520012, 2.78520012, 2.78520012,
-        2.78520012, 2.78520012, 2.78520012, 2.78520012, 2.78520012,
-        2.78520012])
-    npoints_ref = np.array([0, 1, 1, 1, 2, 2, 2, 2, 2, 2, 2, 2, 2, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3])
-
-    if tassert:
-        isok5 = True
-        if (mult != mult_ref).any() or not isclose(radii,radii_ref) or (npoints != npoints_ref).any():
-            isok5 = False
-
-    #######################################################
-    # Part 6: Clathrate
-    #######################################################
-    print("Part VI")
-    from ase.io import write
-    from ase.spacegroup import crystal
-    a = 10.515
-    #x = 0.185; y = 0.304; z = 0.116
-    x = 0.1847; y = 0.2977; z = 0.1067
-    wyckoff = [
-        (0, y, z), #24k
-        (x, x, x), #16i
-        (1/4., 0, 1/2.), #6c
-        (1/4., 1/2., 0), #6d
-        (0, 0 , 0) #2a
-    ]
-
-    pri = crystal(['Si','Si','Si','Ba','Ba'], wyckoff, spacegroup=223, cellpar=[a, a, a, 90, 90, 90])
-    sub = crystal(['Al','Al','Al','Ba','Ba'], wyckoff, spacegroup=223, cellpar=[a, a, a, 90, 90, 90])
-
-    plat = ParentLattice(atoms=pri,substitutions=[sub])
-
-    #cp = ClustersPool(plat,npoints=[1,2],radii=[0,5.7],super_cell=SuperCell(plat,np.diag([2,1,1])))
-    cp = ClustersPool(plat,npoints=[0,1,2],radii=[0,0,5.0])
-    cp.write_clusters_db(db_name="test_clusters_generation_6.json")
-
-    mult = cp.get_multiplicities()
-    radii = cp.get_all_radii()
-    npoints = cp.get_all_npoints()
-
-    mult_ref = np.array([1, 24, 16, 6, 12, 8, 48, 24, 48, 24, 48, 48, 48, 12, 24, 24])
-    radii_ref = np.array([0.0,0.0,0.0,0.0,2.243901, 2.378554359,2.419983103,2.606790868,3.817351239, 3.88424099, 3.88473654, 3.90320808, 3.979588005, 4.254368999, 4.258122441, 4.31192162])
-    npoints_ref = np.array([0, 1, 1, 1, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2])
-
-    if tassert:
-        isok6 = True
-        if (mult != mult_ref).any() or not isclose(radii,radii_ref) or (npoints != npoints_ref).any():
-            isok6 = False
-
-    #######################################################
-    # Part 7: Negative radii
-    #######################################################
-
-    print("Part VII")
-
-    plat = ParentLattice(
-        Atoms(cell=np.diag([2,2,5]),positions=[[0,0,0]]),
-        site_symbols=[["Cu","Al"]],
-        pbc=(1,1,0)
-        )
-
-    scell = SuperCell(plat,np.array([(6,0,0),(0,6,0),(0,0,1)]))
-    cp = ClustersPool(plat, npoints=[0,1,2,3,4], radii=[0,0,-1,4.1,2.9], super_cell=scell)
-
-    cp.write_clusters_db(db_name="test_clusters_generation_7.json")
-
-    mult = cp.get_multiplicities()
-    radii = cp.get_all_radii()
-    npoints = cp.get_all_npoints()
-
-    #print(repr(mult))
-    #print(repr(radii))
-    #print(repr(npoints))
-
-    mult_ref = np.array([1, 1, 2, 2, 2, 4, 2, 2, 2, 2, 1, 4, 2, 4, 1])
-    radii_ref = np.array([0.        , 0.        , 2.        , 2.82842712, 4.        ,
-       4.47213595, 5.65685425, 6.        , 6.32455532, 7.21110255,
-       8.48528137, 2.82842712, 4.        , 4.        , 2.82842712])
-    npoints_ref = np.array([0, 1, 2, 2, 2, 2, 2, 2, 2, 2, 2, 3, 3, 3, 4])
-
-    if tassert:
-        isok7 = True
-        if (mult != mult_ref).any() or not isclose(radii,radii_ref) or (npoints != npoints_ref).any():
-            isok7 = False
+    doparts = [2,3,5,6,7]
+    #doparts = [8]
+    isok = []
+    if 1 in doparts:
+        #######################################################
+        # Part 1: 2D, radii.
+        #######################################################
+        print("\nPart I")
+        cell = [[3,0,0],
+                [0,1,0],
+                [0,0,5]]
+        positions = [
+            [0,0,0],
+            [1,0,0],
+            [2,0,0]]
+        pbc = [True,True,False]
+
+        pri = Atoms(['H','H','H'], positions=positions, cell=cell, pbc=pbc)
+        su1 = Atoms(['C','H','H'], positions=positions, cell=cell, pbc=pbc)
+        su2 = Atoms(['H','He','H'], positions=positions, cell=cell, pbc=pbc)
+        su3 = Atoms(['H','N','H'], positions=positions, cell=cell, pbc=pbc)
+
+        pl = ParentLattice(pri,substitutions=[su1,su2,su3],pbc=pbc)
+
+        cp = ClustersPool(pl, npoints=[1,2,3], radii=[0,2.1,2.1])
+        cp.write_clusters_db(db_name="test_clusters_generation_1.json")
+
+        print("\nMult: ", cp.get_multiplicities())
+        print("\nMult2: ", cp.get_cluster_multiplicities())
+
+        if tassert:
+            try:
+                atom_idxs, atom_nrs = cp.get_cpool_arrays()
+                isok.append(True)
+            except:
+                isok.append(False)
+
+    if 2 in doparts:
+        #######################################################
+        # Part 2: 1D, supercell.
+        #######################################################
+        print("Part II")
+        a=3.0
+        cell = np.array([[1,0,0],[0,4,0],[0,0,1]])
+        positions = np.array([[0,0,0],[0,1,0],[0,2,0],[0,3,0]])
+        sites = [[12,13],[12,13],[12,13],[12,13]]
+        pris = Atoms(cell=cell*a, positions=positions*a)
+
+        pl = ParentLattice(pris, sites=sites, pbc=(1,0,0))
+        sc = SuperCell(pl,[[4,0,0],[0,1,0],[0,0,1]])
+
+
+        cp = ClustersPool(pl,npoints=[1,2],super_cell=sc) # Here radii are not given, therefore all the clusters which can fit in the supercell are generated.
+        #cp = ClustersPool(pl,npoints=[0,1,2],radii=[0,0,3.9*a]) # Here radii are not given, therefore all the clusters which can fit in the supercell are generated.
+        cp.write_clusters_db(db_name="test_clusters_generation_2.json")
+
+        mult = cp.get_multiplicities()
+        radii = cp.get_all_radii()
+        npoints = cp.get_all_npoints()
+
+        #atom_idxs, atom_nrs = cp.get_cpool_arrays()
+        #print(atom_idxs[1][0],atom_idxs[7][0],atom_idxs[12][1],len(atom_nrs[17]),len(cp))
+
+        if tassert:
+            atom_idxs, atom_nrs = cp.get_cpool_arrays()
+            isok2 = atom_idxs[1][0] == 1 and atom_idxs[7][0] == 2 and atom_idxs[12][1] == 8 and len(atom_nrs[17]) == 2 and len(cp) == 18
+            isok.append(isok2)
+
+    if 3 in doparts:
+        #######################################################
+        # Part 3: FCC, radii.
+        #######################################################
+        print("Part III")
+
+        from ase.data import atomic_numbers as an
+        a=4.1
+        pris = bulk("Cu",crystalstructure="fcc", a=a)
+        sites = [[an["Cu"],an["Au"]]]
+        pl = ParentLattice(pris,sites=sites)
+
+        cp = ClustersPool(pl,npoints=[0,1,2,3],radii=[0,0,5.0,5.0])
+        cp.write_clusters_db(db_name="test_clusters_generation_3.json")
+
+        mult = cp.get_multiplicities()
+        npoints = cp.get_all_npoints()
+        radii = cp.get_all_radii()
+
+        rmult = np.array([1,1,6,3,8,12])
+        rnpoints = np.array([0,1,2,2,3,3])
+        rradii = np.array([0.       , 0.       , 2.8991378, 4.1      , 2.8991378, 4.1      ])
+
+        if tassert:
+            isok3 = len(cp) == 6 and (mult == rmult).all() and (npoints == rnpoints).all() and isclose(radii,rradii)
+            isok.append(isok3)
+
+    if 4 in doparts:
+        #######################################################
+        # Part 4: 2D cell with acute angle.
+        #######################################################
+        print("Part IV")
+        from ase.io import write
+
+        a=4.1
+        cell = np.array([[5,0,0],[4,1,0],[0,0,1]])
+        positions = np.array([[0,0,0],[1,0,0],[2,0,0],[3,0,0],[4,0,0]])
+        pbc = (1,1,0)
+        #sites = [[an["Cu"],an["Au"]]]*5
+        sites = [[an["Cu"],an["Au"]],[an["Cu"],an["Au"]],[12],[12],[12]]
+        pris = Atoms(cell=cell*a,positions=positions*a,pbc=pbc)
+        pl = ParentLattice(pris,sites=sites,pbc=pbc)
+
+        #cp = ClustersPool(pl,npoints=[0,1,2,3],radii=[0,0,4.5*a,4.5*a])
+        cp = ClustersPool(pl,npoints=[2],radii=[2.0*a])
+        write(filename="test_clusters_generation_scell_part4.json",images=cp.get_cpool_scell().get_atoms(),format="json")
+        cp.write_clusters_db(db_name="test_clusters_generation_4.json")
+
+        print("\nMult: ", cp.get_multiplicities())
+        print("\nMult2: ", cp.get_cluster_multiplicities())
+        if tassert:
+            atom_idxs, atom_nrs = cp.get_cpool_arrays()
+            isok4 = atom_idxs[2][0] == 30 and atom_idxs[3][1] == 16 and atom_idxs[4][0] == 10
+            isok.append(isok4)
+
+    if 5 in doparts:
+        #######################################################
+        # Part 5: O on Pt(111)
+        #######################################################
+        print("Part V")
+        from ase.io import write
+
+        cell = np.array([[2.785200119, 0.0, 0.0], [-1.3926000595, 2.4120540577, 0.0], [0.0, 0.0, 7.2740998268]])
+        positions = np.array([[0.0, 0.0, 2.274101], [1.392600, 0.804018, 0.0], [0.0, 0.0, 2.916914], [1.392600, 0.804018, 2.924188], [0.0, 1.608036, 2.931462]])
+        pbc = (1,1,0)
+        sites = [[78], [78], [0,8], [0,8], [0,8]]
+        pris = Atoms(cell=cell,positions=positions,pbc=pbc)
+        pl = ParentLattice(pris,sites=sites,pbc=pbc)
+
+        cp = ClustersPool(pl,npoints=[0,1,2,3],radii=[0,0,3.3,3.0])
+        #cp = ClustersPool(pl,npoints=[0,1,2],radii=[0,0,3.3])
+        #write(filename="test_clusters_generation_scell_part5.json",images=cp.get_cpool_scell().get_atoms(),format="json")
+        cp.write_clusters_db(db_name="test_clusters_generation_5.json")
+
+        mult = cp.get_multiplicities()
+        radii = cp.get_all_radii()
+        npoints = cp.get_all_npoints()
+
+        #print(repr(mult))
+        #print(repr(radii))
+        #print(repr(npoints))
+
+        mult_ref = np.array([1, 1, 1, 1, 3, 3, 3, 3, 3, 3, 3, 3, 3, 6, 3, 3, 3, 3, 3, 1, 3, 1, 1, 1, 1, 1])
+        radii_ref = np.array(
+            [0.        , 0.        , 0.        , 0.        , 1.60805243,
+            1.60805243, 1.60810181, 2.78520012, 2.78520012, 2.78520012,
+            3.21608028, 3.21608028, 3.21610496, 1.60810181, 2.78520012,
+            2.78520012, 2.78520012, 2.78520012, 2.78520012, 2.78520012,
+            2.78520012, 2.78520012, 2.78520012, 2.78520012, 2.78520012,
+            2.78520012])
+        npoints_ref = np.array([0, 1, 1, 1, 2, 2, 2, 2, 2, 2, 2, 2, 2, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3])
+
+        if tassert:
+            isok5 = True
+            if len(mult) != len(mult_ref) or len(npoints) != len(npoints_ref):
+                isok5 = False
+            elif (mult != mult_ref).any() or not isclose(radii,radii_ref) or (npoints != npoints_ref).any():
+                isok5 = False
+            isok.append(isok5)
+
+    if 6 in doparts:
+        #######################################################
+        # Part 6: Clathrate
+        #######################################################
+        print("Part VI")
+        from ase.io import write
+        from ase.spacegroup import crystal
+        a = 10.515
+        #x = 0.185; y = 0.304; z = 0.116
+        x = 0.1847; y = 0.2977; z = 0.1067
+        wyckoff = [
+            (0, y, z), #24k
+            (x, x, x), #16i
+            (1/4., 0, 1/2.), #6c
+            (1/4., 1/2., 0), #6d
+            (0, 0 , 0) #2a
+        ]
+
+        pri = crystal(['Si','Si','Si','Ba','Ba'], wyckoff, spacegroup=223, cellpar=[a, a, a, 90, 90, 90])
+        sub = crystal(['Al','Al','Al','Ba','Ba'], wyckoff, spacegroup=223, cellpar=[a, a, a, 90, 90, 90])
+
+        plat = ParentLattice(atoms=pri,substitutions=[sub])
+
+        #cp = ClustersPool(plat,npoints=[1,2],radii=[0,5.7],super_cell=SuperCell(plat,np.diag([2,1,1])))
+        cp = ClustersPool(plat,npoints=[0,1,2],radii=[0,0,5.0])
+        cp.write_clusters_db(db_name="test_clusters_generation_6.json")
+
+        mult = cp.get_multiplicities()
+        radii = cp.get_all_radii()
+        npoints = cp.get_all_npoints()
+
+        mult_ref = np.array([1, 24, 16, 6, 12, 8, 48, 24, 48, 24, 48, 48, 48, 12, 24, 24])
+        radii_ref = np.array([0.0,0.0,0.0,0.0,2.243901, 2.378554359,2.419983103,2.606790868,3.817351239, 3.88424099, 3.88473654, 3.90320808, 3.979588005, 4.254368999, 4.258122441, 4.31192162])
+        npoints_ref = np.array([0, 1, 1, 1, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2])
+
+        if tassert:
+            isok6 = True
+            if len(mult) != len(mult_ref) or len(npoints) != len(npoints_ref):
+                isok6 = False
+            elif (mult != mult_ref).any() or not isclose(radii,radii_ref) or (npoints != npoints_ref).any():
+                isok6 = False
+            isok.append(isok6)
+
+    if 7 in doparts:
+        #######################################################
+        # Part 7: Negative radii
+        #######################################################
+
+        print("Part VII")
+
+        plat = ParentLattice(
+            Atoms(cell=np.diag([2,2,5]),positions=[[0,0,0]]),
+            site_symbols=[["Cu","Al"]],
+            pbc=(1,1,0)
+            )
+
+        scell = SuperCell(plat,np.array([(6,0,0),(0,6,0),(0,0,1)]))
+        cp = ClustersPool(plat, npoints=[0,1,2,3,4], radii=[0,0,-1,4.1,2.9], super_cell=scell)
+
+        cp.write_clusters_db(db_name="test_clusters_generation_7.json")
+
+        mult = cp.get_multiplicities()
+        radii = cp.get_all_radii()
+        npoints = cp.get_all_npoints()
+
+        print(repr(mult))
+        print(repr(radii))
+        print(repr(npoints))
+
+        mult_ref = np.array([1, 1, 2, 2, 2, 4, 2, 2, 4, 4, 2, 4, 2, 4, 1])
+        radii_ref = np.array([0.        , 0.        , 2.        , 2.82842712, 4.        ,
+           4.47213595, 5.65685425, 6.        , 6.32455532, 7.21110255,
+           8.48528137, 2.82842712, 4.        , 4.        , 2.82842712])
+        npoints_ref = np.array([0, 1, 2, 2, 2, 2, 2, 2, 2, 2, 2, 3, 3, 3, 4])
+
+        if tassert:
+            isok7 = True
+            if len(mult) != len(mult_ref) or len(npoints) != len(npoints_ref):
+                isok7 = False
+            elif (mult != mult_ref).any() or not isclose(radii,radii_ref) or (npoints != npoints_ref).any():
+                isok7 = False
+            isok.append(isok7)
+
+    if 8 in doparts:
+        #######################################################
+        # Part 8: FCC(111) with alloying and Adsorption in hollow sites
+        #######################################################
+
+        print("Part VIII")
+        from ase.build import fcc111, add_adsorbate
+
+        pristine = fcc111('Re', size=(1,1,3), a=3.2) # 3-atomic-layer Al slab
+        add_adsorbate(pristine,'X',1.7,position='fcc') # Hollow FCC vacancy site
+        pristine.center(vacuum=10.0, axis=2) # add vacuum along z-axis
+
+        symbols = [['Co'],['Co'],['Co','Ni'],['X','Al']]
+        platt = ParentLattice(pristine, symbols=symbols)
+
+        scell = SuperCell(platt,[[5,0],[0,2]])
+        scell.serialize(fname="scell.json")
+        print(scell.get_sublattice_types())
+
+        npoints = [2]
+        radii = [-1]
+        cp = ClustersPool(platt, npoints=npoints, radii=radii, super_cell=scell,method=1)
+
+        cp.write_clusters_db(db_name="test_clusters_generation_8.json")
+
+        mult = cp.get_multiplicities()
+        radii = cp.get_all_radii()
+        npoints = cp.get_all_npoints()
+
+        #print(repr(mult))
+        #print(repr(radii))
+        #print(repr(npoints))
+
+        mult_ref = np.array([3, 3, 3, 2, 3, 3, 2, 2, 5])
+        radii_ref = np.array([2.14398383, 2.2627417 , 2.2627417 , 3.11715682, 3.91918359,
+       3.91918359, 4.5254834 , 4.5254834 , 5.0076608 ])
+        npoints_ref = np.array([2, 2, 2, 2, 2, 2, 2, 2, 2])
+
+        if tassert:
+            isok8 = True
+            if len(mult) != len(mult_ref) or len(npoints) != len(npoints_ref):
+                isok8 = False
+            elif (mult != mult_ref).any() or not isclose(radii,radii_ref) or (npoints != npoints_ref).any():
+                isok8 = False
+            isok.append(isok8)
 
     print ("\n\n========Test writes========")
     print (test_clusters_generation.__doc__)
     print ("===========================\n")
 
     print ("========Asserts========")
     if tassert:
+        for i,p in enumerate(doparts):
+            print("Test part ",p)
+            assert isok[i]
+        """
         #print("test part 1")
         #assert isok1
         print("test part 2")
         assert isok2
         print("test part 3")
         assert isok3
         #print("test part 4")
         #assert isok4
         print("test part 5")
         assert isok5
         print("test part 6")
         assert isok6
         print("test part 7")
         assert isok7
+        """
```

### Comparing `clusterX-1.0.0.dev8/clusterx/test/test_folders.py` & `clusterX-2.1.0rc1/clusterx/test/test_folders.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,22 +31,23 @@
 
     sset1.write_files(prefix = "random_strs-") # tests folder creation and writing of structure files
     sset1.calculate_energies(EMT2()) # test iterating over folders and calculating energies and writing energy files
     sset1.read_property_values(property_name = "my_total_energy") # test
     e1 = sset1.get_property_values("my_total_energy")
 
     sset2 = StructuresSet(plat)
-    sset2.add_structures(structures=sset1.get_folders_db_fname()) # Test adding structures from json database file
+    sset2.add_structures(structures=sset1.get_db_fname()) # Test adding structures from json database file
     for s1,s2 in zip(sset1,sset2):
         print((s1.get_atomic_numbers()==s2.get_atomic_numbers()).all())
 
-    sset3 = StructuresSet(plat, folders_db_fname=sset1.get_folders_db_fname()) # Test init structures set from folders database
+    #sset3 = StructuresSet(plat, db_fname=sset1.get_db_fname()) # Test init structures set from folders database
+    sset3 = StructuresSet(db_fname=sset1.get_db_fname()) # Test init structures set from folders database
     e3 = sset3.get_property_values("my_total_energy")
 
-    print((e1==e3).all())
+    print((np.array(e1)==np.array(e3)).all())
 
 
 
     """
     for s1,s2 in zip(sset1,sset2):
         print(s1,s2)
         print(s1.get_atomic_numbers(),s2.get_atomic_numbers())
```

### Comparing `clusterX-1.0.0.dev8/clusterx/structure_selector.py` & `clusterX-2.1.0rc1/clusterx/structure_selector.py`

 * *Files identical despite different names*

### Comparing `clusterX-1.0.0.dev8/clusterx/clusters/cluster.py` & `clusterX-2.1.0rc1/clusterx/clusters/cluster.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,35 +34,30 @@
         to speed up the calculation of the cluster radius on initialization, the
         distances between all pairs of atoms in the supercell may be passed in
         this argument.
 
 
     **Methods:**
     """
-    def __new__(cls, atom_indexes, atom_numbers, super_cell=None, distances=None):
-        for iai, ai in enumerate(atom_indexes):
-            for _iai, _ai in enumerate(atom_indexes):
-                if ai == _ai and atom_numbers[iai] != atom_numbers[_iai]:
-                    raise ValueError("Cluster may not have different species on the same site.")
+
+    def __init__(self, atom_indexes, atom_numbers, super_cell=None, distances=None):
 
         if len(atom_indexes) != len(atom_numbers):
             raise ValueError("Initialization error, number of sites in cluster different from number of species.")
 
-        cl = super(Cluster,cls).__new__(cls)
-        cl.__init__(atom_indexes, atom_numbers, super_cell, distances)
-        return cl
-
-    def __init__(self, atom_indexes, atom_numbers, super_cell=None, distances=None):
-        #self.ais = np.array(atom_indexes)
-        #self.ans = np.array(atom_numbers)
         if len(atom_indexes)!=0:
-            self.ais, self.ans = (list(t) for t in zip(*sorted(zip(atom_indexes, atom_numbers))))
+            try:
+                self.ais,self.ans = list(zip(*sorted(zip(np.array(atom_indexes),np.array(atom_numbers)))))
+            except:
+                raise ValueError("Cluster initialization failed")
+
         else:
             self.ais = np.array(atom_indexes)
             self.ans = np.array(atom_numbers)
+
         self.npoints = len(atom_numbers)
         self.positions_cartesian = None
         self.alphas = None
         #self.positions_scaled = None
         self.radius = None
         if super_cell is not None:
             # Set alphas, site_type, and positions
@@ -71,60 +66,84 @@
             sites = super_cell.get_sites()
             idx_subs = super_cell.get_idx_subs()
             tags = super_cell.get_tags()
 
             self.positions_cartesian = np.zeros((self.npoints,3))
             #self.positions_scaled = np.zeros((self.npoints,3))
             for ip, idx in enumerate(atom_indexes):
-                self.positions_cartesian[ip] = super_cell.get_positions(wrap=True)[idx]
+                #self.positions_cartesian[ip] = super_cell.get_positions(wrap=True)[idx]
+                self.positions_cartesian[ip] = super_cell.get_positions()[idx]
                 #self.positions_scaled[ip] = super_cell.get_scaled_positions(wrap=True)[idx]
                 self.site_type[ip] = tags[idx]
                 self.alphas[ip] = np.argwhere(sites[idx] == self.ans[ip])
 
+            """
             # Set radius
             r = 0.0
             if self.npoints > 1:
                 for i1, idx1 in enumerate(self.ais):
                     for idx2 in self.ais[i1+1:]:
                         if distances is not None:
                             d = distances[idx1,idx2]
                         else:
                             d = super_cell.get_distance(idx1,idx2,mic=False,vector=False)
                         if r < d:
                             r = d
             self.radius = r
+            """
+            
+            # Set radius
+            # FIX this! Radius cannot be based on distance in supercell, as it will fail for small supercells and large clusters wrapped into it.
+            r = 0.0
+            if self.npoints > 1:
+                if distances is not None:
+                    for i1, idx1 in enumerate(self.ais):
+                        for idx2 in self.ais[i1+1:]:
+                            d = distances[idx1,idx2]
+                            if r < d:
+                                r = d
+                else:
+                    for i1 in range(self.npoints-1):
+                        for i2 in range(i1+1, self.npoints):
+                            d = np.linalg.norm(self.positions_cartesian[i1]-self.positions_cartesian[i2])
+                            if r < d:
+                                r = d
+            self.radius = r
 
     """
     def __lt__(self,other):
         if self.npoints == other.npoints:
             return self.radius < other.radius
         else:
             return self.npoints < other.npoints
     """
 
     def get_alphas(self):
         """Return labels of point basis-functions of cluster
         """
         return self.alphas
 
-    def set_radius(self,distances):
+    def _compute_radius(self,distances):
         r = 0.0
         if self.npoints > 1:
             for i1, idx1 in enumerate(self.ais):
                 for idx2 in self.ais[i1+1:]:
                     d = distances[idx1,idx2]
                     if r < d:
                         r = d
         self.radius = r
 
     def get_radius(self,distances=None):
+        """Return cluster radius
+        The radius of a cluster is the maximum distance between any pair of its points.
+        """
         if self.radius is not None:
             return self.radius
         elif distances is not None:
-            self.set_radius(distances)
+            self._compute_radius(distances)
             return self.radius
 
     def _get_idxs_norm(self):
         return np.linalg.norm(self.ais)
 
     def __lt__(self,other):
         if self.npoints == other.npoints and abs(self.radius-other.radius)<1e-5:
@@ -132,53 +151,22 @@
             no = other._get_idxs_norm()
             return ns < no
         elif self.npoints == other.npoints:
             return self.radius < other.radius
         else:
             return self.npoints < other.npoints
 
+    def __repr__(self):
+        return "Cluster["+str(list(zip(self.ais,self.ans)))+"]"
+        
+    def __hash__(self):
+        return hash(str(list(zip(self.ais,self.ans))))
+        
     def __eq__(self, other):
-        if isinstance(other, self.__class__):
-            ais = self.ais
-            ans = self.ans
-            oais = other.ais
-            oans = other.ans
-            npoints = self.npoints
-
-            ns = len(ais)
-            no = len(oais)
-            if ns != no:
-                return False
-
-            #if Counter(ais) != Counter(oais):
-            #    return False
-
-            #if sorted(ais) != sorted(oais):
-            #    return False
-
-            for i in range(ns):
-                if ais[i] != oais[i] or ans[i] != oans[i]:
-                    return False
-
-            #if (ais != oais).any():
-            #    return False
-
-            #if (ans != oans).any():
-            #    return False
-
-            """
-            for i in range(npoints):
-                for j in range(npoints):
-                    if ais[i] == oais[j] and ans[i] != oans[j]:
-                        return False
-            """
-            return True
-
-        else:
-            return False
+        return self.__hash__ == other.__hash__ 
 
     def __len__(self):
         return len(self.ais)
 
     def get_idxs(self):
         """Return array of atom indices referred to the defining supercell.
         """
@@ -209,26 +197,16 @@
             correspond with each other, e.g. , the second symmetry operation is
             organized by the set of the second rotation matrix and second
             translation vector in the respective arrays.
         ``cell``: 3x3 matrix
             The symmetry operations ``rr`` and ``tt`` refer to scaled coordinates.
             The parameter ``cell`` contains row-wise the corresponding cartesian
             coordinates of the cell vectors.
-
-        **Example:**
-        Getting the multiplicities of clusters in a clusters pool::
-
-            from clusterx.symmetry import get_spacegroup
-            sc_sg, sc_sym = get_spacegroup(parent_lattice) # Scaled to parent_lattice
-            m = []
-            for cl in clusters_pool.get_cpool():
-                m.append(cl.get_multiplicity(sc_sym["rotations"],sc_sym["translations"]))
-
         """
-        from clusterx.symmetry import get_spacegroup, get_scaled_positions, get_internal_translations, wrap_scaled_positions
+        from clusterx.symmetry import get_scaled_positions, get_internal_translations, wrap_scaled_positions
 
         orbit = []
         for r,t in zip(rr,tt):
             ts = np.tile(t,(self.npoints,1)).T
             #sp0 = np.dot(self.positions_cartesian,np.linalg.inv(cell))
             sp0 = get_scaled_positions(self.positions_cartesian, cell, pbc=pbc, wrap=True)
             sp1 = np.add(np.dot(r,sp0.T),ts).T
```

### Comparing `clusterX-1.0.0.dev8/clusterx/io/atat.py` & `clusterX-2.1.0rc1/clusterx/io/atat.py`

 * *Files identical despite different names*

### Comparing `clusterX-1.0.0.dev8/clusterx/parent_lattice.py` & `clusterX-2.1.0rc1/clusterx/parent_lattice.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # Copyright (c) 2015-2019, CELL Developers.
 # This work is licensed under the terms of the Apache 2.0 license
 # See accompanying license for details or visit https://www.apache.org/licenses/LICENSE-2.0.txt.
 
 from ase import Atoms
-import clusterx as c
 import numpy as np
-import sys
-import io
-import tempfile
 import copy
 from clusterx.utils import _is_integrable
-#from ase.db.core import connect
 from ase.db import connect
+from clusterx.symmetry import get_spacegroup
+import warnings
+warnings.filterwarnings("ignore", category=np.VisibleDeprecationWarning) 
 
 def unique_non_sorted(a):
     _, idx = np.unique(a, return_index=True)
     return a[np.sort(idx)]
 
 class ParentLattice(Atoms):
     """**Parent lattice class**
@@ -32,29 +30,31 @@
         ``site_symbols`` is not None, then the passed ``Atoms`` objects may not
         contain a definition of atomic species, i.e., can be initialized by only
         indicating atomic positions, unit cell, and periodic boundary conditions.
     ``substitutions``: list of ASE's ``Atoms`` objects.
         Every ``Atoms`` object in the list, corresponds to a possible full
         substitution of only one sublattice. If set, overrides ``sites`` (see
         below).
-    ``sites``: list of integer arrays
+    ``numbers``: list of integer arrays or dict
         This is an array of length equal to the number of atoms in the parent
         lattice. Every element in the array is an array with species numbers,
         representing the species which can occupy the crystal
         sites (see examples below). This is overriden by ``substitutions``
-        if set.
-    ``site_symbols``: list of strings
+        if set. If a dict, the dict keys must be the site indices.
+    ``symbols``: list of strings
         This is an array of length equal to the number of atoms in the parent
         lattice. Every element in the array is an array with species symbols
         (e.g. ``[["Cu","Au"]]``),
         representing the species which can occupy the crystal
         sites (see examples below). This is overriden by ``substitutions``
         if set.
     ``json_db_filepath``: string
-        Json database file. Overrides all the above.
+        Path to a Json database file, as created by ``ParentLattice.serialize()``.
+        Overrides all the above. Allows to create a ``ParentLattice`` object
+        from file.
     ``pbc``: three bool
         Periodic boundary conditions flags. Examples:
         (1, 1, 0), (True, False, False). Default value: (1,1,1)
 
     **Examples:**
 
     In all the examples below, you may visualize the created parent lattice
@@ -124,31 +124,44 @@
 
         * Add in metadata the tags, and the idx_tags relation.
 
         * override get_distance and get_distances from Atoms. Such that if get_all_distances
             was ever called, it sets a self.distances attribute which is used for get_distance
             and get_distances, saving computation time. Care should be paid in cases where
             positions are updated either by relaxation or deformation of the lattice.
+        * remove deprecated sites and site_symbols parameters from __init__(), calls around the code,
+            and documentation / tutorials
 
     **Methods:**
     """
 
-    def __init__(self, atoms=None, substitutions=None, sites=None, site_symbols=None, json_db_filepath=None, pbc=None):
-
+    def __init__(self, atoms=None, substitutions=None, numbers=None, symbols=None, json_db_filepath=None, pbc=None, sites=None, site_symbols=None):
+        if numbers is not None:
+            if isinstance(numbers, dict):
+                sites = []
+                for i in range(len(atoms)):
+                    sites.append(None)
+                for site_index, nrs in numbers.items():
+                    sites[int(site_index)] = list(nrs)
+            else:
+                sites = numbers
+        if symbols is not None:
+            site_symbols = symbols
         if json_db_filepath is not None:
             db = connect(json_db_filepath)
             substitutions = []
             for i,row in enumerate(db.select()):
                 if i == 0:
                     atoms = row.toatoms()
                 else:
                     substitutions.append(row.toatoms())
 
         if pbc is None:
             pbc = atoms.get_pbc()
+            
         super(ParentLattice,self).__init__(symbols=atoms,pbc=pbc)
 
         if atoms is not None:
             self._atoms = atoms.copy()
             self._atoms.set_pbc(pbc)
         else:
             self._atoms = None
@@ -165,15 +178,15 @@
                         sites[i][j] = an[sym]
 
             if sites is not None:
                 try:
                     unique_sites = np.unique(sites,axis=0)
                 except:
                     try:
-                        unique_sites = np.unique(sites)
+                        unique_sites = np.unique(np.array(sites,dtype=object))
                     except AttributeError:
                         raise AttributeError("sites array has problems, look at the documentation.")
 
             tags = np.zeros(self._natoms).astype(int)
             for ius, us in enumerate(unique_sites):
                 for idx in range(self._natoms):
                     if (np.array_equal(sites[idx], us)):
@@ -194,14 +207,15 @@
                         if tags[idx] == ius:
                             numbers[idx] = us[isp]
                         else:
                             numbers[idx] = sites[idx][0]
 
                     substitutions.append(Atoms(positions=self.get_positions(),cell=self.get_cell(),pbc=self.get_pbc(),numbers=numbers))
 
+
         if substitutions is None:
             substitutions = []
         self._subs = []
         self._set_substitutions(substitutions)
 
     def __eq__(self, other):
         """Check identity of two ParentLattice objects
@@ -233,18 +247,36 @@
 
     """
     def get_atoms(self):
         "Get a copy of the Atoms object representing the pristine parent lattice."
         return self._atoms.copy()
     """
 
+    def get_sym(self):
+        """Get space symmetry of a ParentLattice object.
+        """
+        try:
+            return self.sc_sg, self.sc_sym
+        except:
+            self.sc_sg, self.sc_sym = self._compute_sym()
+            return self.sc_sg, self.sc_sym
+
+    def _compute_sym(self):
+        return get_spacegroup(self)
+
     def get_natoms(self):
         """Get the total number of atoms."""
         return len(self._atoms)
 
+    def get_positions(self, wrap=False, **wrap_kw):
+        return super(ParentLattice, self).get_positions(wrap, **wrap_kw)
+    
+    def get_cell(self, complete = False):
+        return super(ParentLattice, self).get_cell(complete)
+
     def _set_substitutions(self,substitutions=[]):
         if len(substitutions) != 0:
             for atoms in substitutions:
                 if self._natoms != len(atoms):
                     raise ValueError('Substitutions array has wrong length: %d != %d.' %
                                      (len(self._atoms), len(substitutions)))
                 else:
@@ -352,18 +384,42 @@
         st = self.get_substitutional_tags()
         ss = []
         for i,tag in enumerate(self.get_tags()):
             if tag in st:
                 ss.append(i)
         return ss
 
-    def get_n_sub_sites(self):
+    def get_substitutional_atoms(self):
+        """Return Atoms object for pristine lattice containing only sites which may be substituted
+        """
+        ats = Atoms(cell=self.get_cell(), pbc=self.get_pbc())
+        pats = self.get_pristine()
+        ss = self.get_substitutional_sites()
+        for i in ss:
+            ats.append(pats[i])
+        return ats
+
+    def get_n_sub_sites(self, unique=True):
         """Return total number of substitutional sites
+
+        **Parameters:**
+
+        ``unique``: Boolean (default ``True``)
+            If ``True``, return the number of site-types which may be substituted.
+            If ``False``, return the number of sites which may be substituted.
         """
-        return len(self.get_substitutional_tags())
+        if unique:
+            return len(self.get_substitutional_tags())
+        else:
+            st = []
+            for tag in self.get_tags():
+                if len(self.idx_subs[tag]) > 1:
+                    st.append(tag)
+
+            return len(st)
 
     def get_spectator_sites(self):
         """Return atom indexes which may not be substituted
         """
         st = self.get_spectator_tags()
         ss = []
         for i,tag in enumerate(self.get_tags()):
@@ -431,14 +487,21 @@
         the first three positions can be occupied by species 14 or 13, the 4th
         and 5th positions by species 56, vacant or species 38, and the 6th position
         can be only occupied by species 11, then the sites dictionary reads::
 
             sites = {0: [14,13], 1: [14,13], 2: [14,13], 3: [56,0,38], 4: [56,0,38], 5:[11]}
         """
         return self.sites
+    
+    def get_ems(self):
+        nspt = self.get_sites()
+        ems = np.zeros(len(nspt), dtype=int)
+        for k,v in nspt.items():
+            ems[k] = len(v)
+        return ems
 
     def get_substitutions(self):
         """Return array of (references to) Atoms objects corresponding to fully
         substituted configurations.
         """
         return self._subs
 
@@ -470,14 +533,16 @@
 
         **Parameters:**
 
         ``pretty_print``: boolean
             Whether to return a dictionary or a self-explanatory and nicely
             formatted string.
 
+            DEPRECATED: Use `print_sublattice_types()` instead.
+
         **Examples:**
         For instance, if a ParentLattice object consists of six positions, such that
         the first three positions can be occupied by species 14 or 13, the 4th
         and 5th positions by species 56, vacant or species 38, and the 6th position
         can be only occupied by species 11, then there are three site types, and the
         returned dictionary will look like::
 
@@ -485,65 +550,137 @@
 
         .. todo::
             give option to also print the list of atom indexes for every site type.
         """
         if not pretty_print:
             return self.idx_subs
         else:
-            from ase.data import chemical_symbols as cs
-            sld = self.idx_subs
-            cs = np.array(cs)
-            print("\n+--------------------------------------------------------------------+")
-            print("|{0:^68s}|".format("The structure consists of "+str(len(sld))+" sublattices"))
-            print("+--------------------------------------------------------------------+")
-            print("|{0:^17s}|{1:^30s}|{2:^19s}|".format("Sublattice type","Chemical symbols","Atomic numbers"))
-            print("+--------------------------------------------------------------------+")
-
-            for slind,slsps in self.idx_subs.items():
-                print("|{0:^17s}|{1:^30s}|{2:^19s}|".format(str(slind),str(cs[slsps]),str(slsps)))
-            print("+--------------------------------------------------------------------+\n")
+            warnings.warn("Using `pretty_print=True` is deprecated. Use `print_sublattice_types()` instead.", category=FutureWarning)
+            self.print_sublattice_types()
 
+    def print_sublattice_types(self):
+        """Print chemical symbols and atomic numbers for each sublattice type.
+        """
+        from ase.data import chemical_symbols as cs
+        sld = self.idx_subs
+        cs = np.array(cs)
+        print("\n+--------------------------------------------------------------------+")
+        print("|{0:^68s}|".format("The structure consists of "+str(len(sld))+" sublattices"))
+        print("+--------------------------------------------------------------------+")
+        print("|{0:^17s}|{1:^30s}|{2:^19s}|".format("Sublattice type","Chemical symbols","Atomic numbers"))
+        print("+--------------------------------------------------------------------+")
+
+        for slind,slsps in self.idx_subs.items():
+            print("|{0:^17s}|{1:^30s}|{2:^19s}|".format(str(slind),str(cs[slsps]),str(slsps)))
+        print("+--------------------------------------------------------------------+\n")
 
+    # Deprecated, use get_sublattice_types instead
     def get_idx_subs(self):
         return self.get_sublattice_types()
 
     def as_dict(self):
         """Return dictionary with object definition
         """
         dict = {}
         dict.update({"unit_cell" : self.get_cell()})
         dict.update({"pbc" : self.get_pbc()})
         dict.update({"positions" : self.get_positions()})
-        dict.update({"sites" : self.get_sites()})
+        dict.update({"numbers" : self.get_sites()})
 
         return dict
 
+    def plat_from_dict_obsolete(dict):
+        cell = np.array(dict["parent_lattice_pristine_unit_cell"])
+        pbc = dict["parent_lattice_pbc"]
+        positions = np.array(dict["parent_lattice_pristine_positions"])
+        _site_types = dict["parent_lattice_idx_subs"]
+        _tags = np.array(dict["parent_lattice_tags"])
+
+        #numbers = np.zeros(len(positions), dtype=int)
+        numbers = []
+        for site_index,tag in enumerate(_tags):
+            numbers.append(_site_types[tag])
+            #numbers[site_index] = _site_types[tag]
+        numbers_pris = []
+        for nrs in numbers:
+            numbers_pris.append(nrs[0])
+
+        prist = Atoms(positions=positions, numbers=numbers_pris, cell=cell, pbc=pbc)
+        return ParentLattice(atoms=prist, numbers=numbers, pbc=pbc)
+
+    def plat_from_dict(dict):
+        """Generates ParentLattice object from a dictionary as returned by ParentLattice.as_dict()
+        """
+        cell = np.array(dict["unit_cell"])
+        pbc = dict["pbc"]
+        positions = np.array(dict["positions"])
+        _numbers = dict["numbers"]
+
+        numbers = np.zeros(len(positions), dtype=int)
+        for site_index, nrs in _numbers.items():
+            numbers[site_index] = nrs[0]
+
+        prist = Atoms(positions=positions, numbers=numbers, cell=cell, pbc=pbc)
+        return ParentLattice(atoms=prist, numbers=_numbers, pbc=pbc)
+
     def get_atom_indices_for_site_type(self, site_type):
         """Return atom indices of the structure of a certain given site type
         """
         return np.where(self.get_tags() == site_type)
 
-    def serialize(self,fname="plat.json"):
-        """
-        Serialize a ParentLattice object
+    def round_coords(self, decimals = 12):
+        """ Round cell vectors and lattice positions coordinates.
+            
+        Uses ``numpy.around()`` method.
+            
+        **Parameters:**
+        
+        ``decimals``: integer
+            Number of decimal places to round to (default: 0). If decimals is negative, 
+            it specifies the number of positions to the left of the decimal point.
+        
+        **Return:**
+            Returns a new ParentLattice object with rounded coordinates.
+        """
+
+        atomss = self.get_all_atoms()
+        cell0 = np.around(self.get_cell(), decimals)
+        pbc0 = self.get_pbc()
+        
+        atomss0 = []
+        for at in atomss:
+            pos0 = np.around(at.get_positions(), decimals)
+            ans0 = at.get_atomic_numbers()
+            atomss0.append(Atoms(positions = pos0, numbers = ans0, cell = cell0, pbc = pbc0))
+            
+        return ParentLattice(atoms = atomss0[0], substitutions = atomss0[1:], pbc = pbc0)
+		
+    def serialize(self, filepath="plat.json", fname=None):
+        """Serialize a ParentLattice object
 
         Writes a `ASE's json database <https://wiki.fysik.dtu.dk/ase/ase/db/db.html>`_
         file containing a representation of the parent lattice.
         An instance of the ParentLattice class can be initialized from the created file.
         The created database can be visualized using
         `ASE's gui <https://wiki.fysik.dtu.dk/ase/ase/gui/gui.html>`_, e.g.: ::
-
+        
             ase gui plat.json
 
         **Parameters:**
 
-        ``fname``: string
+        ``filepath``: string
             Output file name.
+
+        ``fname``: string
+            *DEPRECATED*, use ``filepath`` instead. Output file name.
         """
-        db = connect(fname, type="json", append=False)
+        if fname is not None:
+            filepath = fname
+        
+        db = connect(filepath, type="json", append=False)
 
         images = []
         db.write(self.get_pristine())
         for sub in self.get_substitutions():
             db.write(sub)
 
         db.metadata = self.as_dict()
```

### Comparing `clusterX-1.0.0.dev8/clusterx/__init__.py` & `clusterX-2.1.0rc1/clusterx/__init__.py`

 * *Files identical despite different names*

### Comparing `clusterX-1.0.0.dev8/clusterx/monte_carlo.py` & `clusterX-2.1.0rc1/clusterx/super_cell.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,595 +1,561 @@
 # Copyright (c) 2015-2019, CELL Developers.
 # This work is licensed under the terms of the Apache 2.0 license
 # See accompanying license for details or visit https://www.apache.org/licenses/LICENSE-2.0.txt.
 
-## packages needed for MonteCarlo
-import random
-#from clusterx.structures_set import StructuresSet
-from clusterx.structure import Structure
-
-## packages needed for MonteCarloTrajectory
-import json
+from ase import Atoms
 import numpy as np
-from copy import deepcopy
-
-class MonteCarlo():
-    """MonteCarlo class
-
-    Description:
-        Perform MonteCarlo samplings
-
-    Parameters:
-
-    ``energy_model``: Model object
-        Model used for acceptance and rejection. Usually, the Model enables to
-        calculate the total energy of a given configuration.
+import sys
+from ase.visualize import view
+#from ase.build import make_supercell
+from clusterx.utils import make_supercell
+from clusterx.parent_lattice import ParentLattice
+from clusterx.symmetry import get_internal_translations, get_scaled_positions, wrap_scaled_positions, get_spacegroup
 
-    ``scell``: SuperCell object
-        Super cell in which the sampling is performed.
 
-    ``nsubs``: dictionary
-        The format of the dictionary is as follows::
 
-            {site_type1:[n11,n12,...], site_type2:[n21,n22,...], ...}
+from clusterx.utils import get_cl_idx_sc
+import clusterx
+from ase.db import connect
 
-        It indicates how many substitutional atoms of every kind (n#1, n#2, ...)
-        may replace the pristine species for sites of site_type#.
 
-        The list of site types can be obtained with the method ``ParentLattice.get_idx_subs()``
-        (see related documentation).
-
-        Defines the number of substituted atoms in each sublattice
-        Supercell in which the sampling is performed.
+class SuperCell(ParentLattice):
+    """
+    **Build a super cell**
 
-    ``filename``: string
-        Trajectory can be written to a json file with the name ``filename``.
+    A :class:`SuperCell <clusterx.super_cell.SuperCell>` object acts as a blue-print for the creation of structures
+    with arbitrary decorations. 
 
-    ``last_visited_structure_name``: string
-        The structure visited at the final step of the sampling can be saved to a json file.
-        Default name: last-visited-structure-mc.json
+    The :class:`SuperCell <clusterx.super_cell.SuperCell>` class inherits from the :class:`ParentLattice <clusterx.parent_lattice.ParentLattice>` class. Therefore,
+    all methods available to the :class:`ParentLattice <clusterx.parent_lattice.ParentLattice>` class are available to the
+    :class:`SuperCell <clusterx.super_cell.SuperCell>` class. Refer to the documentation of :class:`ParentLattice <clusterx.parent_lattice.ParentLattice>` for more
+    methods.
+
+    **Parameters:**
+
+    ``parent_lattice``: :class:`ParentLattice <clusterx.parent_lattice.ParentLattice>` object
+        In **CELL**, a super cell is a periodic repetition of a parent lattice
+        object. This parameter defines such a parent lattice for the created
+        super cell.
+    ``p``: integer, or 1x3, 2x2, or 3x3 integer array
+        Transformation matrix :math:`P`. The cartesian coordinates of the
+        latttice vectors defining the created SuperCell object, are the rows of
+        the matrix :math:`S` defined by :math:`S = PV` where the rows of
+        :math:`V` are the cartesian coordinates of the lattice
+        vectors of the ParentLattice object. That is, the value of
+        :py:meth:`ParentLattice.get_cell() <clusterx.parent_lattice.ParentLattice.get_cell()>`. The given matrix ``p`` must be compatible
+        with the periodic boundary conditions of the parent lattice, i.e. the
+        resulting super cell must not contain translations along the
+        non-periodic directions.
+    ``sort_key``: list of three integers, optional
+        Create supercell object with sorted atomic coordinates
+
+        Example:``sort_key=(2,1,0)`` will result in atoms sorted
+        according to increasing z-coordinate first, increasing
+        y-coordinate second, increasing x-coordinate third. Useful to get
+        well ordered slab structures, for instance. Sorting can be changed
+        by appropriately setting the ``sort_key`` argument, with the same
+        effect as in the argument to ``itemgetter`` below::
+
+            from operator import itemgetter
+            sp = sorted(p, key=itemgetter(2,1,0))
+
+        here p is a Nx3 array of vector coordinates.
+    ``json_db_filepath``: string (default: None)
+        Overrides all the above. Used to initialize from file. Path of a json
+        file containing a serialized superCell object, as generated
+        by the ``SuperCell.serialize()`` method.
 
-    ``sublattice_indices``: list of int
-        Sampled sublattices. Each index in the list gives the site_type defining the sublattice.
-        If the list is empty (default), the site_type of the sublattices are read from ``nsubs``
-        Non-substituted sublattices are excluded for canonical samplings.
+    .. todo::
+        Proper check of pbc when building the super cell. Either ignore
+        translation in ``p`` along non-periodic directions or warn in some way
+        if ``p`` is not compatible with pbc.
 
-    ``models``: Model object
-        List of Models for structural dependent properties. Models of properties
-        can also be defined and calculated after the sampling is finished
-        by using the Class MonteCarloTrajectory
 
-    ``no_of_swaps``: int
-        Number of swaps per sampling step
+    **Methods:**
+    """
 
-    ``ensemble``: string
-        "canonical" allows only for swapping of atoms inside scell
-        "grandcanonical"  allows for replacing atoms within the given scell
-        (the number of substitutents in each sublattice is not kept)
+    def __init__(self, parent_lattice=None, p=None, sort_key=None, json_db_filepath=None, sym_table=False):
 
-    .. todo:
-        Samplings in the grand canonical ensemble are not yet possible.
+        if json_db_filepath is not None:
+            db = connect(json_db_filepath)
 
-        Properties given in models are not calculated during the sampling.
+            plat_dict = db.metadata.get("parent_lattice",{})
+            self._plat = ParentLattice.plat_from_dict(plat_dict)
+            p = db.metadata.get("tmat",np.identity(3,dtype=int))
+            self._sort_key = db.metadata.get("sort_key",None)
+        else:
+            self._plat = parent_lattice
+            self._sort_key = sort_key
 
-        SR: notes from using the class by reading the documentation:
+        pbc = self._plat.get_pbc()
         
-            * Initialization with both nsubs and sublattice_indices is confusing: What happens if I specify a site_type in sublattice_indices and do not put the corresponding sitetype in nsubs, or viceversa?
-            * ensemble parameter needs more extensive documentation. Is a chemical potential defined at some point to adjust average concentration in grandcanonical?
-
-
-    """
-
-    def __init__(self, energy_model, scell, nsubs, filename = "trajectory.json", last_visited_structure_name = "last-visited-structure-mc.json", sublattice_indices = [], models = [], no_of_swaps = 1, ensemble = "canonical", mc = False, error_reset = False):
-        self._em = energy_model
-        self._scell = scell
-        self._nsubs = nsubs
-        print(self._nsubs)
-        self._filename = filename
-        self._last_visited_structure_name = last_visited_structure_name
-
-        if not sublattice_indices:
-            try:
-                self._sublattice_indices = [k for k in self._nsubs.keys()]
-
-                if ensemble == "canonical":
-                    for key in self._nsubs.keys():
-                        if all([ subs == 0 for subs in self._nsubs[key] ]):
-                            self._sublattice_indices.remove(key)
+        if not isinstance(p,int):
+            p = np.array(p)
+            if p.shape == (1,):
+                self._p = np.diag([p[0],1,1])
+            elif p.shape == (2,):
+                self._p = np.diag([p[0],p[1],1])
+            elif p.shape == (3,):
+                self._p = np.diag(p)
+            elif p.shape == (2,2):
+                self._p = np.array([[p[0,0],p[0,1],0],[p[1,0],p[1,1],0],[0,0,1]])
+            elif p.shape == (3,3):
+                self._p = p
+
+        if isinstance(p,int):
+            if pbc[0]==1 and pbc[1]==0 and pbc[2]==0:
+                self._p = np.diag([p,1,1])
+            elif pbc[0]==1 and pbc[1]==1 and pbc[2]==0:
+                self._p = np.diag([p,p,1])
+            elif pbc[0]==1 and pbc[1]==1 and pbc[2]==1:
+                self._p = np.diag([p,p,p])
+            else:
+                sys.exit("SuperCell(Error)")
 
-            except AttributeError:
-                raise AttributeError("Index of sublattice is not properly assigned, look at the documentation.")
+        self.index = int(round(np.linalg.det(self._p)))
+        prist = make_supercell(self._plat.get_pristine(),self._p)
+        subs = [make_supercell(atoms,self._p) for atoms in self._plat.get_substitutions()]
+
+        prist.wrap()
+        for i in range(len(subs)):
+            subs[i].wrap()
+
+        if self._sort_key is not None:
+            from clusterx.utils import sort_atoms
+            prist = sort_atoms(prist,key=self._sort_key)
+            for i in range(len(subs)):
+                subs[i] = sort_atoms(subs[i],key=self._sort_key)
+
+        super(SuperCell,self).__init__(atoms = prist, substitutions = subs)
+        self._natoms = len(self)
+        self.set_pbc(self._plat.get_pbc())
+        
+        if sym_table == True:
+            self._sym_table = self.get_symmetry_table()
+        else: 
+            self._sym_table = []
+
+        self.sc_sg, self.sc_sym = self.get_sym()
+        self.sc_sg_pl, self.sc_sym_pl = self.get_sym_platt()
+        #self.internal_trans = get_internal_translations(self._plat, self) # Scaled to super_cell
+        self.internal_trans = None # Scaled to super_cell
+        #self.all_distances_mic = None
+        #self.all_distances_nomic = None
+        #self.scaled_positions = None
+        self.sym_perm = None
+        self.sym_perm_platt = None
+
+    def compute_sym_perm(self, include_sc_trans = True):
+        if include_sc_trans:
+            self.sym_perm = []
         else:
-            self._sublattice_indices = sublattice_indices
-
-        if not self._sublattice_indices:
-            import sys
-            sys.exit('Indices of sublattice are not correctly assigned, look at the documatation.')
+            self.sym_perm_platt = []
 
-        self._models = []
-        if models:
-            self._models = models
+        tol = 1e-3/np.cbrt(self.get_natoms())
+        internal_trans = self.get_internal_translations() # Scaled to super_cell
+        spos1 = get_scaled_positions(self.get_positions(wrap = True), self.get_cell(), pbc = self.get_pbc(), wrap = True) # Super-cell scaled positions
+        spos = np.around(spos1,6) # Wrapping in ASE doesn't always work. Here a hard external fix by rounding and then applying again ASE's style wrapping.
+
+        for i, periodic in enumerate(self.get_pbc()):
+            if periodic:
+                spos[:, i] %= 1.0
+                spos[:, i] %= 1.0
 
-        self._ensemble = ensemble
-        self._no_of_swaps = no_of_swaps
-        self._mc = mc
-
-        self._error_reset = error_reset
-
-    def metropolis(self, scale_factor, nmc, initial_decoration = None, write_to_db = False, acceptance_ratio = None):
-        """Perform metropolis simulation
-
-        **Description**: Perfom Metropolis sampling for nmc sampling
-             steps at scale factor :math:`k_B T`.  The total energy
-             :math:`E` for visited structures in the sampling is
-             calculated from the Model ``energ_model`` of the total
-             energy. During the sampling, a new structure at step i is accepted
-             with the probability given by :math:`\min( 1, \exp( - (E_i - E_{i-1})/(k_B T)) )`
-
-        **Parameters**:
-
-        ``scale_factor``: list of floats
-            From the product of the float in the list, the scale factor for the energy :math:`k_B T` is obtained.
-
-            E.g. [:math:`k_B`, :math:`T`] with :math:`k_B` as the Boltzmann constant and :math:`T` as the temperature for the Metropolis simulation.
-            The product :math:`k_B T` defines the scale factor in the Boltzmann distribution.
-
-            Note: The unit of the product :math:`k_B T` must be the same as for the total energy :math:`E`.
-
-        ``nmc``: integer
-            Number of sampling steps
-
-        ``initial_decoration``: Structure object
-            Sampling starts with the structure defined by this Structure object.
-            If initial_structure = None: Sampling starts with a structure randomly generated.
-
-        ``write_to_db``: boolean (default: False)
-            Whether to add the structure to the json database (see ``filename`` parameter for MonteCarloTrajectory initialization)
-
-        ``acceptance_ratio``: float (default: None)
-            Real number between 0 and 100. Represents the percentage of accepted moves.
-            If not ``None``, the initial temperature will be adjusted to match the given
-            acceptance ratio. The acceptance ratio during the simulation is computed using
-            the last 100 moves.
-
-        **Returns**: MonteCarloTrajectory object
-            Trajectory containing all information of the structures visited during the sampling
-
-        """
-        import math
-        from clusterx.utils import poppush
-
-        scale_factor_product = 1
-        for el in scale_factor:
-            scale_factor_product *= float(el)
-
-        if initial_decoration is not None:
-            struc = Structure(self._scell, initial_decoration, mc = self._mc)
+        if include_sc_trans:
+            sg, sym = self.get_sym()
         else:
-            struc = self._scell.gen_random(self._nsubs, mc = self._mc)
-
-        e = self._em.predict(struc)
-        print(e)
+            sg, sym = self.get_sym_platt()
+            
+        rot = sym["rotations"]
+        tra = sym["translations"]
+
+        _sym_perm = []
+        #for r,t_ in zip(rot,internal_trans):
+        for r,t_ in zip(rot,tra):
+            t = np.round(t_, decimals=8)
+            ts = np.tile(t,(len(spos),1)).T # Every column represents the same translation for every cluster site
+            spos_rt = np.add(np.dot(r,spos.T),ts).T # Apply rotation, then translation
+
+            _sp1_ = wrap_scaled_positions(spos_rt, self.get_pbc())
+
+            _sp1 = np.around(_sp1_,5) # Wrapping in ASE doesn't always work. Here a hard external fix by rounding and then applying again ASE's style wrapping.
+                        
+            for i, periodic in enumerate(self.get_pbc()):
+                if periodic:
+                    _sp1[:, i] %= 1.0
+                    _sp1[:, i] %= 1.0
 
-        traj = MonteCarloTrajectory(self._scell, filename=self._filename, models = self._models)
-
-        if self._models:
-            key_value_pairs = {}
-            for m, mo in enumerate(self._models):
-                key_value_pairs.update({mo.property: mo.predict(struc)})
-            traj.add_decoration(0, e, [], decoration = struc.decor, key_value_pairs = key_value_pairs)
+            _cl = get_cl_idx_sc(_sp1, spos, method=1, tol=tol)
+            _sym_perm.append(_cl)
 
+        if include_sc_trans:
+            self.sym_perm = np.unique(_sym_perm, axis = 0)
         else:
-            traj.add_decoration(0, e, [], decoration = struc.decor)
-
-        if acceptance_ratio:
-            nar = 100
-            ar = acceptance_ratio
-            hist = np.zeros(nar,dtype=int)
+            self.sym_perm_platt = np.unique(_sym_perm, axis = 0)
+        #self.sym_perm = _sym_perm
 
-        if self._no_of_swaps > 1:
-            control_flag = False
-        else:
-            control_flag = True
-            if self._error_reset:
-                errorsteps = 50000
-                x = 1
-
-
-        for i in range(1,nmc+1):
-            indices_list = []
-            for j in range(self._no_of_swaps):
-                if self._mc:
-                    ind1, ind2, site_type, rindices = struc.swap_random(self._sublattice_indices)
-                    indices_list.append([ind1, ind2, site_type, rindices])
-                else:
-                    ind1,ind2 = struc.swap_random(self._sublattice_indices)
-                    indices_list.append([ind1, ind2])
-
-            if control_flag:
-                if self._error_reset:
-                    if (x > errorsteps):
-                        x = 1
-                        e1 = self._em.predict(struc)
-                    else:
-                        x += 1
-                        #de = self._em.predict_swap_binary_linear(struc, ind1 = ind1 , ind2 = ind2)
-                        de = self._em.predict_swap(struc, ind1 = ind1 , ind2 = ind2)
-                        e1 = e+de
-                else:
-                    de = self._em.predict_swap(struc, ind1 = ind1 , ind2 = ind2)
-                    e1 = e+de
+    def get_sym_perm(self, include_sc_trans = True):
+        if include_sc_trans:
+            if self.sym_perm is None:
+                self.compute_sym_perm(include_sc_trans = True)
+                return self.sym_perm
             else:
-                e1 = self._em.predict(struc)
-
-            if e >= e1:
-                accept_swap = True
-                boltzmann_factor = 0
+                return self.sym_perm
+        else:
+            if self.sym_perm_platt is None:
+                self.compute_sym_perm(include_sc_trans = False)
+                return self.sym_perm_platt
             else:
-                boltzmann_factor = math.exp((e-e1)/(scale_factor_product))
+                return self.sym_perm_platt
 
-                if np.random.uniform(0,1) <= boltzmann_factor:
-                    accept_swap = True
-                else:
-                    accept_swap = False
-
-            if accept_swap:
-                e = e1
-
-                if self._models:
-                    key_value_pairs = {}
-                    for m, mo in enumerate(self._models):
-                        key_value_pairs.update({mo.property: mo.predict(struc)})
-                    traj.add_decoration(i, e, indices_list, key_value_pairs = key_value_pairs)
+    def get_sym(self):
+        """Get space symmetry of a ParentLattice object.
+        """
+        try:
+            return self.sc_sg, self.sc_sym
+        except:
+            self.sc_sg, self.sc_sym = self._compute_sym()
+            return self.sc_sg, self.sc_sym
 
-                else:
-                    traj.add_decoration(i, e, [[li[0],li[1]] for li in indices_list])
+    def get_sym_platt(self):
+        """Get space symmetry of a ParentLattice object.
+        """
+        try:
+            return self.sc_sg_pl, self.sc_sym_pl
+        except:
+            self.sc_sg_pl, self.sc_sym_pl = self.get_parent_lattice()._compute_sym()
+            return self.sc_sg_pl, self.sc_sym_pl
 
-                if acceptance_ratio:
-                    ar = poppush(hist,1)
+    def _compute_sym(self):
+        return get_spacegroup(self)
 
+    """
+    def get_scaled_positions():
+        if self.scaled_positions == None:
+            self.scaled_positions = get_scaled_positions(wrap = True)
+            return self.scaled_positions
+        else:
+            return self.scaled_positions
+    
+    def get_all_distances(self, mic=False):
+        vector = False
+        if mic:
+            if self.all_distances_mic == None:
+                self.all_distances_mic = super(ParentLattice, self).get_all_distances(mic, vector)
+                return self.all_distances_mic
             else:
-                for j in range(self._no_of_swaps-1,-1,-1):
-                    if self._mc:
-                        struc.swap(indices_list[j][0],indices_list[j][1], site_type = indices_list[j][2], rindices = indices_list[j][3])
-                    else:
-                        struc.swap(indices_list[j][0],indices_list[j][1])
-
-                if acceptance_ratio:
-                    ar = poppush(hist,0)
-
-            if acceptance_ratio:
-                if i%10 == 0 and i >= nar:
-                    scale_factor_product *= math.exp((acceptance_ratio/100.0-ar)/10.0)
-                #if acceptance_ratio and i%100 == 0:
-                #    print(i,acceptance_ratio,ar*100,scale_factor_product)
-
-        if write_to_db:
-            traj.write_to_file()
-            struc.serialize(fname=self._last_visited_structure_name)
-
-        return traj
-
-
-
-class MonteCarloTrajectory():
-    """MonteCarloTrajectory class
-
-    **Description**:
-        Trajectory of decorations visited during the sampling performed in the supercell scell.
-        For each visited decoration, it is retained the sampling step number (sampling_step_no),
-        the decoration (decor), the total energy predicted from a cluster expansion model (energy_model),
-        and additional properties stored as key-value pair in dictionary key_value_pairs.
-
-    **Parameters**:
-
-    ``scell``: SuperCell object
-        Super cell in which the sampling is performed.
-
-    ``filename``: string
-        The trajectoy can be stored in a json file with the path given by ``filename``.
-
-    ``**kwargs``: keyword arguments
-
-        ``save_nsteps``: integer
-            Trajectory is saved after save_nsteps.
-
-        ``models``: List of Model objects
-
-    .. todo::
-        Saving the trajectory after ``save_steps`` is not yet implemented.
-
-        Improve appearance of json file - decoration array in one line
+                return self.all_distances_mic
 
+        if not mic:
+            if self.all_distances_nomic == None:
+                self.all_distances_nomic = super(ParentLattice, self).get_all_distances(mic, vector)
+                return self.all_distances_nomic
+            else:
+                return self.all_distances_nomic
     """
 
-    def __init__(self, scell = None, filename="trajectory.json", **kwargs):
-        self._trajectory = []
-
-        self._scell = scell
-        self._save_nsteps = kwargs.pop("save_nsteps",10)
-        self._write_no = 0
-
-        self._models = kwargs.pop("models",[])
-
-        self._filename = filename
-
-    def calculate_model_properties(self, models):
-        """Calculate the property for all decoration in the trajectory
+    def get_internal_translations(self):
+        """Get internal translations of parent lattice in supercell, scaled to supercell
+        """
+        if self.internal_trans is None:
+            self.internal_trans = get_internal_translations(self._plat, self)
+            return self.internal_trans
+        else:
+            return self.internal_trans
+        
+        
+    def copy(self):
+        """Return a copy
         """
-        for mo in models:
-            if mo not in self._models:
-                self._models.append(mo)
-
-        sx = Structure(self._scell, decoration = self._trajectory[0]['decoration'])
-
-        for t,tr in enumerate(self._trajectory):
-            indices_list = tr['swapped_positions']
-            for j in range(len(indices_list)):
-                sx.swap(indices_list[j][0],indices_list[j][1])
 
-            sdict={}
-            for m,mo in enumerate(self._models):
-                sdict.update({mo.property: mo.predict(sx)})
+        sc = self.__class__(self._plat, self._p, sort_key = self._sort_key)
 
-            self._trajectory[t]['key_value_pairs'] = sdict
-        print(sx.decor)
+        return sc
 
-    def add_decoration(self, step, energy, indices_list, decoration = None, key_value_pairs = {}):
-        """Add decoration of Structure object to the trajectory
+    def scell_from_dict(dict):
+        """Generates SuperCell object from a dictionary as returned by SuperCell.as_dict()
         """
+        plat_dict = dict.get("parent_lattice",{})
+        plat = ParentLattice.plat_from_dict(plat_dict)
+        p = dict.get("tmat",np.identity(3,dtype=int))
+        sort_key = dict.get("sort_key",None)
 
-        if indices_list:
-            self._trajectory.append(dict([('sampling_step_no', int(step)), ('model_total_energy', energy), ('swapped_positions', indices_list), ('key_value_pairs', key_value_pairs)]))
-        else:
-            self._trajectory.append(dict([('sampling_step_no', int(step)), ('model_total_energy', energy), ('swapped_positions', [[0,0]]) , ('decoration', deepcopy(decoration)), ('super_cell_definition', self._scell.as_dict()), ('key_value_pairs', key_value_pairs)]))
+        return SuperCell(plat,p,sort_key)
 
+    def as_dict(self):
+        """Return dictionary with object definition
+        """
+        plat_dict = self._plat.as_dict()
+        self._dict = {"tmat":self._p,"parent_lattice":plat_dict,"sort_key":self._sort_key}
 
-    def get_sampling_step_entry_at_step(self, nstep):
-        """Get the dictionary at the n-th sampling step in the trajectory
-
-        **Parameters:**
-
-        ``nstep``: int
-            sampling step
+        return self._dict
 
-        **Returns:**
-            Dictionary at the n-th sampling step.
+    def get_index(self):
+        """Return index of the SuperCell
 
+        The index of the supercell is an integer number, equal to the super cell
+        volume in units of the parent cell volume.
         """
-        return self.get_sampling_step_entry(self.get_id_sampling_step(nstep))
+        return self.index
 
-    def get_sampling_step_entry(self, nid):
-        """Get the dictionary (entry) at index nid in the trajectory
+    def get_parent_lattice(self):
+        """Return the parent lattice object which defines the supercell.
         """
-        return self._trajectory[nid]
-
-    def get_structure_at_step(self, nstep):
-        """Get the structure from decoration at the n-th sampling step in the trajectory.
-
-        **Parameters:**
-
-        ``nstep``: integer
-            sampling step
-
-        **Returns:**
-            Structure object at the n-th sampling step.
+        return self._plat
 
+    def get_transformation(self):
+        """Return the transformation matrix that defines the supercell from the
+        defining parent lattice.
         """
-        return self.get_structure(self.get_id_sampling_step(nstep))
-
-    def get_structure(self, nid):
-        """Get structure from entry at index nid in the trajectory
-
-        **Parameters:**
+        return self._p
 
-        ``nid``: integer
-            index of structure in the trajectory.
-
-        **Returns:**
-            Structure object at index nid.
+    def get_positions(self, wrap=False, **wrap_kw):
+        return super(SuperCell, self).get_positions(wrap, **wrap_kw)
 
+    def plot(self):
+        """Plot the pristine supercell object.
         """
-        decoration = deepcopy(self._trajectory[0]['decoration'])
+        view(self)
 
-        for t,tr in enumerate(self._trajectory[0:nid+1]):
-            indices_list = tr['swapped_positions']
-            for j in range(len(indices_list)):
-                idx1 = indices_list[j][0]
-                idx2 = indices_list[j][1]
-                decoration[idx1], decoration[idx2] = decoration[idx2], decoration[idx1]
+    def get_pristine_structure(self):
+        """Return Structure object corresponding to pristine structure.
+        """
+        return self.gen_structure(sigmas=np.zeros(len(self.get_tags()),dtype=np.int8))
 
-        sx = Structure(self._scell, decoration = decoration)
-        return sx
 
-    def get_structure2(self, nid):
-        """Get structure from entry at index nid in the trajectory
+    def gen_structure(self, sigmas = None, mc = False):
+        """
+        Generate a Structure with given configuration.
 
         **Parameters:**
 
-        ``nid``: integer
-            index of structure in the trajectory.
-
-        **Returns:**
-            Structure object at index nid.
+        ``sigmas``: array of integers
+            sigmas[idx] must be the ocupation variable for crystal site idx.
+            For instance, supose that::
+                
+                ThisObject.get_sublattice_types()
+
+            returns ``{0:[14,13], 1:[56,47,38]}``, and that::
+                
+                ThisObject.get_tags()
+
+            returns ``[0,0,1,1,0]``, meaning that for atom idx=0,1,4 the sublattice types are 0
+            and for idx=2,3 the sublattice types is 1.
+            Then, the argument ``sigmas=[0,1,0,2,1]`` will produce the configuration::
 
+                [14,13,56,38,13]
+        
         """
-        sx = Structure(self._scell, decoration = deepcopy(self._trajectory[0]['decoration']))
-
-        for t,tr in enumerate(self._trajectory[0:nid+1]):
-            indices_list = tr['swapped_positions']
-            for j in range(len(indices_list)):
-                sx.swap(indices_list[j][0],indices_list[j][1])
-
-        return sx
-
-    def get_lowest_non_degenerate_structure(self):
-        """Get lowest-non-degenerate structure from trajectory
-
-        **Returns:**
-            Structure object.
-
+        import clusterx.structure
+        return clusterx.structure.Structure(SuperCell(self._plat, self._p, self._sort_key, sym_table = bool(self._sym_table)), sigmas=sigmas, mc = mc)
+        
+    def gen_random(self, nsubs = None, mc = False):
+        return self.gen_random_structure(nsubs = nsubs, mc = mc)
+        
+    def gen_random_structure(self, nsubs = None, mc = False):
         """
-        _energies = self.get_model_total_energies()
-        _emin = np.min(_energies)
-        _nid = np.where(_energies == _emin)[0][0]
+        Generate a random Structure with given number of substitutions.
 
-        return self.get_structure(_nid)
+        **Parameters:**
 
-    def get_sampling_step_nos(self):
-        """Get sampling step numbers of all entries in trajectory
-        """
-        steps=[]
-        for tr in self._trajectory:
-            steps.append(tr['sampling_step_no'])
+        ``nsubs``: None, int or dictionary (default: None)
+            If dictionary, the ``nsubs`` argument must have the format ``{site_type0:[nsub01,nsub02,...], site_type1: ...}``
+            where ``site_type#`` and ``nsub##`` are, respectively, an integer indicating
+            the site type index and the number of substitutional species of each kind, as returned by
+            ``SuperCell.get_sublattice_types()``.
 
-        return np.int_(steps)
+            If integer, the SuperCell object must be correspond to a binary, i.e.
+            the output of ``scell.is_nary(2)`` must be True. In this case, nsub indicates
+            the number of substitutional atoms in the binary.
 
-    def get_sampling_step_no(self, nid):
-        """Get sampling step number of entry at index nid in trajectory
-        """
-        return self._trajectory[nid]['sampling_step_no']
+            If ``None``, the number of substitutions in each sublattice is
+            generated at random.
 
+        **Notes:**
 
-    def get_id_sampling_step(self, nstep):
-        """Get entry index at the n-th sampling step.
+        This function can be also called with the method ``gen_random``, with the same signature. 
+        Use ``gen_random_structure``, since ``gen_random`` is deprecated.
         """
-        steps = self.get_sampling_step_nos()
-        nid=0
-        try:
-            nid = np.where(steps == nstep)[0][0]
-        except:
-            if nstep > steps[-1]:
-                nid = len(steps)-1
-            else:
-                for i,s in enumerate(steps):
-                    if s > nstep:
-                        nid = i-1
-                        break
-        return nid
+        import clusterx.structure
+        
+        if nsubs is None:
+            import numpy as np
+            slts = self.get_sublattice_types() #  e.g.  {0: [14,13], 1: [56,0,38], 2:[11]}
+            tags = self.get_tags()  # tags[atom_index] = site_type
+            _nsubs = {}
+            for k,v in slts.items():
+                if len(v) != 1:
+                    _nsubs[k] = [np.random.randint(0,len(np.where(self.get_tags() == k)[0])+1)]
+
+        elif isinstance(nsubs,int):
+            if self.is_nary(2):
+                slts = self.get_sublattice_types()
+                _nsubs = {}
+                for k,v in slts.items():
+                    if len(v) != 1:
+                        _nsubs[k] = [nsubs]
 
-    def get_model_total_energies(self):
-        """Get total energies of all entries in trajectory.
-        """
-        energies = []
-        for tr in self._trajectory:
-            energies.append(tr['model_total_energy'])
+            else:
+                return None
+        else:
+            _nsubs = nsubs
 
-        return np.asarray(energies)
+        decoration, sigmas = self.gen_random_decoration(_nsubs)
 
-    def get_model_total_energy(self, nid):
-        """Get total energy of entry at index nid in trajectory.
-        """
-        return self._trajectory[nid]['model_total_energy']
+        return clusterx.structure.Structure(SuperCell(self._plat, self._p, self._sort_key, sym_table = bool(self._sym_table)), sigmas=sigmas, mc = mc)
 
-    def get_model_properties(self, prop):
-        """Get property of all entries in the trajectory.
-        """
-        try:
-            props = []
-            for tr in self._trajectory:
-                props.append(tr['key_value_pairs'][prop])
-            return np.asarray(props)
+    def gen_random_decoration(self,nsubs):
+        """Generate a random decoration of the super cell with given number of substitutions.
 
-        except:
-            if prop not in [mo.property for mo in self._models]:
-                print("Model of property is not given, look at the documentation.")
-            else:
-                print("Property not calculated, look at the documentation.")
+        Parameters:
 
-    def get_model_property(self, nid, prop):
-        """Get property of entry at index nid in trajectory.
-        """
-        return self._trajectory[nid]['key_value_pairs'][prop]
+        nsubs: dictionary
+            The format of the dictionary is as follows::
 
-    def get_id(self, prop, value):
-        """Get indices of entries in trajectory which contain the key-value pair trajectory.
+                {site_type1:[n11,n12,...], site_type2:[n21,n22,...], ...}
 
-        **Parameters:**
+            it indicates how many substitutional atoms of every kind (n#1, n#2, ...)
+            may replace the pristine species for sites of site_type#.
 
-        ``prop``: string
-            property of interest
-
-        ``value``: float
-            value of the property
-
-        **Returns:**
-            array of int.
+        Returns:
 
+        decoration: list of int
+            list with the same length as the pristine structure.
+            decoration[atom_idx] = species number sitting at site idx.
+        sigmas: list of int
+            sigma[atom_index] is an integer between 0 and M-1, where M is the
+            total number of different species which may substitute an atom
+            in this position.
         """
-        arrayid = []
+        idx_subs = self.get_idx_subs()
+        tags = self.get_tags() # tags[atom_index] = site_type
 
-        if prop in ['sampling_step_no','swapped_positions','model_total_energy','decoration']:
-            for i,tr in enumerate(self._trajectory):
-                if tr[prop] == value:
-                    arrayid.append(i)
-        else:
-            for i,tr in enumerate(self._trajectory):
-                if tr['key_value_pairs'][prop] == value:
-                    arrayid.append(i)
+        decoration = self.get_atomic_numbers()
+        sigmas = np.zeros(len(tags),dtype=np.int8)
+        for tag, nsub in nsubs.items():
+            #list all atom indices with the given tag or site_type
+            sub_idxs = np.where(tags==tag)[0]
 
-        return np.asarray(arrayid)
+            #select nsub such indices for each substitutional
+            #atom of given site tag
+            sub_list = np.asarray([])
+            for i,n in enumerate(nsub):
+                sub_idxs = np.setdiff1d(sub_idxs,sub_list)
+                sub_list = np.random.choice(sub_idxs,n,replace=False)
 
-    def write_to_file(self, filename = None):
-        """Write trajectory to file (default filename trajectory.json).
-        """
+                for atom_index in sub_list:
+                    decoration[atom_index] = idx_subs[tag][i+1]
+                    sigmas[atom_index] = i+1
+        return decoration, sigmas
 
-        if filename is not None:
-            self._filename = filename
 
-        trajdic={}
-        for j,dec in enumerate(self._trajectory):
-            trajdic.update({str(j):dec})
+    def enumerate_decorations(self, npoints=None, radii=None):
+        from ase.db.jsondb import JSONDatabase
+        from ase.neighborlist import NeighborList
+        from subprocess import call
 
-        with open(self._filename, 'w+', encoding='utf-8') as outfile:
-            json.dump(trajdic,outfile, cls=NumpyEncoder, indent = 2 , separators = (',',':'))
+        atoms = self.get_pristine()
+        natoms = len(atoms)
+        sites = self.get_sites()
+        call(["rm","-f","neighbors.json"])
+        atoms_db = JSONDatabase(filename="neighbors.json") # For visualization
 
-    def read(self, filename = None , append = False):
-        """Read trajectory from file (default filename trajectory.json)
-        """
-        if filename is not None:
-            trajfile = open(filename,'r')
-        else:
-            trajfile = open(self._filename,'r')
+        rmax = np.full(len(atoms),np.amax(radii)/2.0)
+        nl = NeighborList(rmax, self_interaction=True, bothways=True, skin=0.0)
+        nl.build(atoms)
+        distances = atoms.get_all_distances(mic=True)
 
-        data = json.load(trajfile)
+        for id1 in range(natoms):
+            neigs = atoms.copy()
+            indices, offsets = nl.get_neighbors(id1)
 
-        if not append:
-            self._trajectory = []
+            for i, offset in zip(indices,offsets):
+                #pos.append(atoms.positions[i] + np.dot(offset, atoms.get_cell()))
+                #pos.append(atoms.positions[i])
+                #chem_num.append(atoms.numbers[i])
+                spi = len(sites[i])-1
+                neigs[i].number = sites[i][spi]
+                neigs[i].position = atoms.positions[i] + np.dot(offset, atoms.get_cell())
 
-        data_keys = sorted([int(el) for el in set(data.keys())])
 
-        for key in data_keys:
-            tr = data[str(key)]
-            self._trajectory.append(tr)
+            #neigs = Atoms(numbers=chem_num,positions=pos,cell=self.get_cell(),pbc=self.get_pbc())
 
-        if self._scell is None:
-            from ase.atoms import Atoms
-            from clusterx.parent_lattice import ParentLattice
-            from clusterx.super_cell import SuperCell
-            _trajz = self._trajectory[0]
+            atoms_db.write(neigs)
 
-            nsp = sorted([int(el) for el in set(_trajz['super_cell_definition']['parent_lattice']['sites'])])
-            species = []
-            for n in nsp:
-                species.append(_trajz['super_cell_definition']['parent_lattice']['sites'][str(n)])
+    def serialize(self,filepath="scell.json", fname=None):
+        """
+        Serialize a SuperCell object
 
-            _plat = ParentLattice(atoms = Atoms(positions = _trajz['super_cell_definition']['parent_lattice']['positions'], cell = _trajz['super_cell_definition']['parent_lattice']['unit_cell'], numbers=np.zeros(len(species)), pbc = np.asarray(_trajz['super_cell_definition']['parent_lattice']['pbc'])), sites  = np.asarray(species), pbc = np.asarray(_trajz['super_cell_definition']['parent_lattice']['pbc']))
-            self._scell = SuperCell(_plat, np.asarray(_trajz['super_cell_definition']['tmat']))
+        Writes a `ASE's json database <https://wiki.fysik.dtu.dk/ase/ase/db/db.html>`_
+        file containing a representation of the super cell.
+        The created database can be visualized using
+        `ASE's gui <https://wiki.fysik.dtu.dk/ase/ase/gui/gui.html>`_, e.g.: ::
 
+            ase gui scell.json
 
-class NumpyEncoder(json.JSONEncoder):
-    """ Special json encoder for numpy types
-    https://stackoverflow.com/questions/26646362/numpy-array-is-not-json-serializable/32850511
+        **Parameters:**
 
-    """
-    def default(self, obj):
-        if isinstance(obj, list):
-            return obj.tolist()
-        elif isinstance(obj, (np.int_, np.intc, np.intp, np.int8, np.int16, np.int32, np.int64, np.uint8, np.uint16, np.uint32, np.uint64)):
-            return int(obj)
-        elif isinstance(obj, (np.float_, np.float16, np.float32, np.float64)):
-            return float(obj)
-        elif isinstance(obj,(np.ndarray,)):
-            return obj.tolist()
+        ``filepath``: string
+            Output file name.
 
-        return json.JSONEncoder.default(self, obj)
+        ``fname``: string
+            *DEPRECATED*, use filepath instead. Output file name.
+        """
+        if fname is not None:
+            filepath = fname
+            
+        super(SuperCell,self).serialize(filepath = filepath)
+    
+    def get_symmetry_table(self, symprec=1e-12, tol=1e-3):
+        '''
+        Takes a SuperCell as a parameter and returns the final indices of every atom 
+        after all symmetry operations have been applied, see below:
+        {(index of the atom, index of the symmetry operation): index of the atom after the symmetry operation}
+        '''
+        
+        import numpy as np
+        from clusterx.parent_lattice import ParentLattice
+        from clusterx.symmetry import get_scaled_positions, wrap_scaled_positions, get_internal_translations
+        from clusterx.utils import get_cl_idx_sc
+        
+        table = {}
+        space_group, symmetry = self._plat.get_sym()
+        rotations = symmetry['rotations']
+        translations = symmetry['translations']
+        internal_trans = get_internal_translations(self._plat, self)
+        #Get rotations and translations
+        pos = self.get_positions(wrap=True)
+        p0 = pos
+        
+        spos1 = self.get_scaled_positions() # Super-cell scaled positions
+        spos = np.around(spos1,8) 
+        for i, periodic in enumerate(self.get_pbc()):
+            if periodic:
+                spos[:, i] %= 1.0
+                spos[:, i] %= 1.0
+        
+        sp0 = get_scaled_positions(p0, self._plat.get_cell(), pbc = self.get_pbc(), wrap = False)
+        
+        atom_index = 0
+        rot_index = 0
+        intt_index = 0
+        for r,t in zip(rotations,translations):
+            ts = np.tile(t,(len(sp0),1)).T # Every column represents the same translation for every cluster site
+            sp1 = np.add(np.dot(r,sp0.T),ts).T # Apply rotation, then translation
+            # Get cartesian, then scaled to supercell
+            p1 = np.dot(sp1, self._plat.get_cell())
+            sp1 = get_scaled_positions(p1, self.get_cell(), pbc = self.get_pbc(), wrap = True)
+        
+            for itr,tr in enumerate(internal_trans): # Now apply the internal translations
+                sp2 = np.add(sp1, tr)
+                sp2 = wrap_scaled_positions(sp2,self.get_pbc())
+                new_pos = get_cl_idx_sc(sp2, spos, method=1, tol=1e-3) #Get indices
+                for new_idx in new_pos:
+                    table[atom_index, rot_index, intt_index] = new_idx #Create the table object
+                    atom_index += 1
+                atom_index = 0
+                intt_index += 1
+            intt_index = 0
+            rot_index += 1
+            
+        return table
```

### Comparing `clusterX-1.0.0.dev8/clusterx/cli/test.py` & `clusterX-2.1.0rc1/clusterx/cli/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,12 +21,12 @@
         return()
     else:
         if name is not "":
             path = os.path.join(os.path.dirname(tm.__file__),name+".py")
             print(path)
         else:
             path = os.path.dirname(tm.__file__)
-            
-        pytest.main([path,"-v","--cache-clear","--capture=no","--disable-warnings","--junit-xml=testlog.xml"])
-        return ()
-
 
+        exit_code = pytest.main([path,"-v","--cache-clear","--capture=no","--disable-warnings","--junit-xml=testlog.xml","--html=testlog.html"])
+        if not exit_code == pytest.ExitCode.OK:
+            raise AssertionError(f"Tests have failed! pytest exit code: {exit_code}")
+        return ()
```

### Comparing `clusterX-1.0.0.dev8/clusterx/cli/spacegroup.py` & `clusterX-2.1.0rc1/clusterx/cli/spacegroup.py`

 * *Files identical despite different names*

### Comparing `clusterX-1.0.0.dev8/clusterx/cli/plot_clusters.py` & `clusterX-2.1.0rc1/clusterx/cli/plot_clusters.py`

 * *Files identical despite different names*

### Comparing `clusterX-1.0.0.dev8/clusterx/cli/main.py` & `clusterX-2.1.0rc1/clusterx/cli/main.py`

 * *Files identical despite different names*

### Comparing `clusterX-1.0.0.dev8/clusterx/cli/commands.py` & `clusterX-2.1.0rc1/clusterx/cli/commands.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,26 +9,20 @@
 # This performs dynamical function creations from the modules contained in this clusterx/cli/,
 # i.e. it performs dynamically imports like:
 # from clusterx.cli.plot_clusters import plot_clusters1, as needed by plac
 #First we get the list of modules
 from os.path import dirname, basename, isfile
 import glob
 mods = glob.glob(dirname(__file__)+"/*.py")
-#print('mods',mods)
 
 modules = [ basename(f)[:-3] for f in mods if isfile(f) and not f.endswith('__init__.py') and not f.endswith('main.py') and not f.endswith('commands.py')]
-#print('modules',modules)
-
 
 # Finally the functions are included here
 commands = [] # This array is needed by plac
 for module in modules:
-    #print('#########################')
-    #print("module in for: ", #print('#########################')                                                   odule)
-    #print("commands: ",getattr(__import__('clusterx.cli.'+module,fromlist=[module]),'commands'))
     for command in getattr(__import__('clusterx.cli.'+module,fromlist=[module]),'commands'):
         commands.append(command)
         setattr(sys.modules[__name__], command, getattr(__import__('clusterx.cli.'+module,fromlist=[module]),command))
 ##########################################
 
 def __init__():
     """
```

### Comparing `clusterX-1.0.0.dev8/clusterx/utils.py` & `clusterX-2.1.0rc1/clusterx/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,1936 +12,2538 @@
 000000b0: 2e6f 7267 2f6c 6963 656e 7365 732f 4c49  .org/licenses/LI
 000000c0: 4345 4e53 452d 322e 302e 7478 742e 0a0a  CENSE-2.0.txt...
 000000d0: 696d 706f 7274 206e 756d 7079 2061 7320  import numpy as 
 000000e0: 6e70 0a69 6d70 6f72 7420 6f73 0a69 6d70  np.import os.imp
 000000f0: 6f72 7420 636f 7079 0a66 726f 6d20 6173  ort copy.from as
 00000100: 652e 6461 7461 2069 6d70 6f72 7420 6368  e.data import ch
 00000110: 656d 6963 616c 5f73 796d 626f 6c73 2061  emical_symbols a
-00000120: 7320 6373 0a0a 6465 6620 6973 636c 6f73  s cs..def isclos
-00000130: 6528 7231 2c72 322c 7274 6f6c 3d31 652d  e(r1,r2,rtol=1e-
-00000140: 3429 3a0a 2020 2020 2222 2244 6574 6572  4):.    """Deter
-00000150: 6d69 6e65 2077 6865 7468 6572 2074 776f  mine whether two
-00000160: 2076 6563 746f 7273 2061 7265 2073 696d   vectors are sim
-00000170: 696c 6172 0a0a 2020 2020 2a2a 5061 7261  ilar..    **Para
-00000180: 6d65 7465 7273 3a2a 2a0a 0a20 2020 2060  meters:**..    `
-00000190: 6072 312c 7232 6060 3a20 3144 2061 7272  `r1,r2``: 1D arr
-000001a0: 6179 7320 6f66 2069 6e74 6567 6572 206f  ays of integer o
-000001b0: 7220 666c 6f61 740a 2020 2020 2020 2020  r float.        
-000001c0: 5665 6374 6f72 7320 746f 2062 6520 636f  Vectors to be co
-000001d0: 6d70 6172 6564 0a20 2020 2060 6072 746f  mpared.    ``rto
-000001e0: 6c60 603a 2066 6c6f 6174 0a20 2020 2020  l``: float.     
-000001f0: 2020 2054 6f6c 6572 616e 6365 2e0a 0a20     Tolerance... 
-00000200: 2020 202a 2a52 6574 7572 6e73 3a2a 2a0a     **Returns:**.
-00000210: 0a20 2020 2042 6f6f 6c65 616e 3a20 6966  .    Boolean: if
-00000220: 2074 6865 2065 7563 6c69 6465 616e 2064   the euclidean d
-00000230: 6973 7461 6e63 6520 6265 7477 6565 6e20  istance between 
-00000240: 6060 7231 6060 2061 6e64 2060 6072 3260  ``r1`` and ``r2`
-00000250: 6020 6973 2073 6d61 6c6c 6572 2074 6861  ` is smaller tha
-00000260: 6e0a 2020 2020 6060 7274 6f6c 6060 2c20  n.    ``rtol``, 
-00000270: 6060 5472 7565 6060 2069 7320 7265 7475  ``True`` is retu
-00000280: 726e 6564 2c20 6f74 6865 7277 6973 6520  rned, otherwise 
-00000290: 6060 4661 6c73 6560 6020 6973 2072 6574  ``False`` is ret
-000002a0: 7572 6e65 642e 0a20 2020 2022 2222 0a20  urned..    """. 
-000002b0: 2020 2072 6574 7572 6e20 6e70 2e6c 696e     return np.lin
-000002c0: 616c 672e 6e6f 726d 286e 702e 7375 6274  alg.norm(np.subt
-000002d0: 7261 6374 2872 312c 7232 2929 203c 2072  ract(r1,r2)) < r
-000002e0: 746f 6c0a 0a0a 6465 6620 6469 6374 5f63  tol...def dict_c
-000002f0: 6f6d 7061 7265 2864 312c 2064 322c 2074  ompare(d1, d2, t
-00000300: 6f6c 3d4e 6f6e 6529 3a0a 2020 2020 2222  ol=None):.    ""
-00000310: 2243 6f6d 7061 7265 2074 776f 2064 6963  "Compare two dic
-00000320: 7469 6f6e 6172 6965 7320 636f 6e74 6169  tionaries contai
-00000330: 6e69 6e67 206d 7574 6162 6c65 206f 626a  ning mutable obj
-00000340: 6563 7473 2e0a 0a20 2020 2054 6869 7320  ects...    This 
-00000350: 636f 6d70 6172 6573 2074 776f 2064 6963  compares two dic
-00000360: 7469 6f6e 6172 6965 732e 2054 776f 2064  tionaries. Two d
-00000370: 6963 7469 6f6e 6172 6965 7320 6172 6520  ictionaries are 
-00000380: 636f 6e73 6964 6572 6564 2065 7175 616c  considered equal
-00000390: 0a20 2020 2065 7665 6e20 6966 2074 6865  .    even if the
-000003a0: 2070 6f73 6974 696f 6e20 6f66 206b 6579   position of key
-000003b0: 7320 6469 6666 6572 2e20 4861 6e64 6c65  s differ. Handle
-000003c0: 7320 6d75 7461 626c 6520 7661 6c75 6573  s mutable values
-000003d0: 2069 6e20 7468 6520 6469 6374 2e0a 2020   in the dict..  
-000003e0: 2020 536f 6d65 2070 6172 7473 2061 7265    Some parts are
-000003f0: 2074 616b 656e 2066 726f 6d3a 0a0a 2020   taken from:..  
-00000400: 2020 6874 7470 733a 2f2f 7374 6163 6b6f    https://stacko
-00000410: 7665 7266 6c6f 772e 636f 6d2f 7175 6573  verflow.com/ques
-00000420: 7469 6f6e 732f 3435 3237 3934 322f 636f  tions/4527942/co
-00000430: 6d70 6172 696e 672d 7477 6f2d 6469 6374  mparing-two-dict
-00000440: 696f 6e61 7269 6573 2d69 6e2d 7079 7468  ionaries-in-pyth
-00000450: 6f6e 0a0a 2020 2020 2a2a 5061 7261 6d65  on..    **Parame
-00000460: 7465 7273 3a2a 2a0a 0a20 2020 2060 6064  ters:**..    ``d
-00000470: 312c 6432 6060 3a20 7079 7468 6f6e 2064  1,d2``: python d
-00000480: 6963 7469 6f6e 6172 6965 730a 2020 2020  ictionaries.    
-00000490: 2020 2020 6469 6374 696f 6e61 7269 6573      dictionaries
-000004a0: 2074 6f20 6265 2063 6f6d 7061 7265 640a   to be compared.
-000004b0: 0a20 2020 2060 6074 6f6c 6060 3a20 666c  .    ``tol``: fl
-000004c0: 6f61 740a 2020 2020 2020 2020 6120 736d  oat.        a sm
-000004d0: 616c 6c20 666c 6f61 7420 6e75 6d62 6572  all float number
-000004e0: 2e20 4966 206e 6f74 2060 604e 6f6e 6560  . If not ``None`
-000004f0: 602c 2074 6865 2063 6f6d 7061 7269 736f  `, the compariso
-00000500: 6e20 6f66 2064 6963 7469 6f6e 6172 790a  n of dictionary.
-00000510: 2020 2020 2020 2020 7661 6c75 6573 2069          values i
-00000520: 7320 7265 6761 7264 6564 2061 7320 6120  s regarded as a 
-00000530: 7665 6374 6f72 2063 6f6d 7061 7269 736f  vector compariso
-00000540: 6e20 616e 6420 646f 6e65 2077 6974 680a  n and done with.
-00000550: 2020 2020 2020 2020 6060 7574 696c 732e          ``utils.
-00000560: 6973 636c 6f73 6528 2960 602e 2046 6f72  isclose()``. For
-00000570: 2074 6865 206d 6561 6e69 6e67 206f 6620   the meaning of 
-00000580: 6060 746f 6c60 602c 2072 6561 6420 7468  ``tol``, read th
-00000590: 6520 646f 6375 6d65 6e74 6174 696f 6e0a  e documentation.
-000005a0: 2020 2020 2020 2020 666f 7220 6060 7274          for ``rt
-000005b0: 6f6c 6060 2070 6172 616d 6574 6572 206f  ol`` parameter o
-000005c0: 6620 6060 7574 696c 732e 6973 636c 6f73  f ``utils.isclos
-000005d0: 6528 2960 602e 0a0a 2020 2020 5265 7475  e()``...    Retu
-000005e0: 726e 3a20 626f 6f6c 6561 6e0a 2020 2020  rn: boolean.    
-000005f0: 2020 2020 6060 5472 7565 6060 2069 6620      ``True`` if 
-00000600: 6469 6374 7320 6172 6520 6571 7561 6c2c  dicts are equal,
-00000610: 2060 6046 616c 7365 6060 2069 6620 7468   ``False`` if th
-00000620: 6579 2061 7265 2064 6966 6665 7265 6e74  ey are different
-00000630: 2e0a 2020 2020 2222 220a 2020 2020 6172  ..    """.    ar
-00000640: 6565 7120 3d20 5472 7565 0a0a 2020 2020  eeq = True..    
-00000650: 6966 206c 656e 2864 3129 2021 3d20 6c65  if len(d1) != le
-00000660: 6e28 6432 293a 0a20 2020 2020 2020 2072  n(d2):.        r
-00000670: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
-00000680: 2064 315f 6b65 7973 203d 2073 6574 2864   d1_keys = set(d
-00000690: 312e 6b65 7973 2829 290a 2020 2020 6432  1.keys()).    d2
-000006a0: 5f6b 6579 7320 3d20 7365 7428 6432 2e6b  _keys = set(d2.k
-000006b0: 6579 7328 2929 0a20 2020 2069 6e74 6572  eys()).    inter
-000006c0: 7365 6374 5f6b 6579 7320 3d20 6431 5f6b  sect_keys = d1_k
-000006d0: 6579 732e 696e 7465 7273 6563 7469 6f6e  eys.intersection
-000006e0: 2864 325f 6b65 7973 290a 2020 2020 6966  (d2_keys).    if
-000006f0: 206c 656e 2864 3129 2021 3d20 6c65 6e28   len(d1) != len(
-00000700: 696e 7465 7273 6563 745f 6b65 7973 293a  intersect_keys):
-00000710: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00000720: 4661 6c73 650a 0a20 2020 2066 6f72 206b  False..    for k
-00000730: 2069 6e20 6431 5f6b 6579 733a 0a20 2020   in d1_keys:.   
-00000740: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-00000750: 2020 2020 2020 666f 7220 7631 2c76 3220        for v1,v2 
-00000760: 696e 207a 6970 2864 315b 6b5d 2c64 325b  in zip(d1[k],d2[
-00000770: 6b5d 293a 0a20 2020 2020 2020 2020 2020  k]):.           
-00000780: 2020 2020 2069 6620 746f 6c20 6973 204e       if tol is N
-00000790: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000007a0: 2020 2020 2020 2020 2069 6620 7631 2021           if v1 !
-000007b0: 3d20 7632 3a0a 2020 2020 2020 2020 2020  = v2:.          
-000007c0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000007d0: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
-000007e0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000007f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000800: 2020 2020 2069 6620 6e6f 7420 6973 636c       if not iscl
-00000810: 6f73 6528 7631 2c76 322c 746f 6c29 3a0a  ose(v1,v2,tol):.
-00000820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000830: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-00000840: 616c 7365 0a0a 2020 2020 2020 2020 6578  alse..        ex
-00000850: 6365 7074 2054 7970 6545 7272 6f72 3a0a  cept TypeError:.
-00000860: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-00000870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000880: 2069 6620 5f69 735f 696e 7465 6772 6162   if _is_integrab
-00000890: 6c65 2864 315b 6b5d 293a 0a20 2020 2020  le(d1[k]):.     
-000008a0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000008b0: 6620 6e6f 7420 6973 636c 6f73 6528 6431  f not isclose(d1
-000008c0: 5b6b 5d2c 6432 5b6b 5d2c 746f 6c29 3a0a  [k],d2[k],tol):.
-000008d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008e0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-000008f0: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
-00000900: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
-00000910: 2020 2020 2020 2020 2069 6620 7479 7065           if type
-00000920: 2864 315b 6b5d 2920 6973 2064 6963 743a  (d1[k]) is dict:
-00000930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000940: 2020 2020 2066 6f72 2073 7562 6b65 7973       for subkeys
-00000950: 2069 6e20 6431 5b6b 5d2e 6b65 7973 2829   in d1[k].keys()
-00000960: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00000970: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00000980: 2069 7363 6c6f 7365 2864 315b 6b5d 5b73   isclose(d1[k][s
-00000990: 7562 6b65 7973 5d2c 6432 5b6b 5d5b 7375  ubkeys],d2[k][su
-000009a0: 626b 6579 735d 2c74 6f6c 293a 0a20 2020  bkeys],tol):.   
-000009b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009c0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000009d0: 4661 6c73 650a 0a20 2020 2072 6574 7572  False..    retur
-000009e0: 6e20 6172 6565 710a 0a0a 6465 6620 7375  n areeq...def su
-000009f0: 625f 666f 6c64 6572 7328 726f 6f74 293a  b_folders(root):
-00000a00: 0a20 2020 2022 2222 5265 7475 726e 206c  .    """Return l
-00000a10: 6973 7420 6f66 2073 7562 666f 6c64 6572  ist of subfolder
-00000a20: 730a 0a20 2020 2050 6172 616d 6574 6572  s..    Parameter
-00000a30: 733a 0a0a 2020 2020 726f 6f74 3a20 7374  s:..    root: st
-00000a40: 7269 6e67 0a20 2020 2020 2020 2070 6174  ring.        pat
-00000a50: 6820 6f66 2074 6865 2061 6273 6f6c 7574  h of the absolut
-00000a60: 6520 666f 6c64 6572 2066 6f72 2077 6869  e folder for whi
-00000a70: 6368 2079 6f75 2077 616e 7420 746f 2067  ch you want to g
-00000a80: 6574 2074 6865 206c 6973 7420 6f66 0a20  et the list of. 
-00000a90: 2020 2020 2020 2073 7562 666f 6c64 6572         subfolder
-00000aa0: 732e 0a20 2020 2022 2222 0a20 2020 2023  s..    """.    #
-00000ab0: 7265 7475 726e 206f 732e 7761 6c6b 2872  return os.walk(r
-00000ac0: 6f6f 7429 2e6e 6578 7428 295b 315d 2023  oot).next()[1] #
-00000ad0: 7079 7468 6f6e 2032 2e37 0a20 2020 2072  python 2.7.    r
-00000ae0: 6574 7572 6e20 6e65 7874 286f 732e 7761  eturn next(os.wa
-00000af0: 6c6b 2872 6f6f 7429 295b 315d 0a0a 6465  lk(root))[1]..de
-00000b00: 6620 5f69 735f 696e 7465 6772 6162 6c65  f _is_integrable
-00000b10: 2873 293a 0a20 2020 2022 2222 4465 7465  (s):.    """Dete
-00000b20: 726d 696e 6520 7768 6574 6865 7220 6172  rmine whether ar
-00000b30: 6775 6d65 6e74 2069 7320 696e 7465 6765  gument is intege
-00000b40: 7220 6f72 2063 616e 2062 6520 636f 6e76  r or can be conv
-00000b50: 6572 7465 6420 746f 2069 6e74 6567 6572  erted to integer
-00000b60: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
-00000b70: 3a0a 0a20 2020 2073 3a20 6f62 6a65 6374  :..    s: object
-00000b80: 0a20 2020 2020 2020 2043 616e 2062 6520  .        Can be 
-00000b90: 616e 7920 6f62 6a65 6374 2066 6f72 2077  any object for w
-00000ba0: 6869 6368 2077 6520 7761 6e74 2074 6f20  hich we want to 
-00000bb0: 6465 7465 726d 696e 6520 7768 6574 6865  determine whethe
-00000bc0: 7220 6973 2069 6e74 6567 6572 206f 720a  r is integer or.
-00000bd0: 2020 2020 2020 2020 6361 6e20 6265 2063          can be c
-00000be0: 6f6e 7665 7274 6564 2074 6f20 696e 7465  onverted to inte
-00000bf0: 6765 722e 0a20 2020 2022 2222 0a20 2020  ger..    """.   
-00000c00: 2074 7279 3a0a 2020 2020 2020 2020 696e   try:.        in
-00000c10: 7428 7329 0a20 2020 2020 2020 2072 6574  t(s).        ret
-00000c20: 7572 6e20 5472 7565 0a20 2020 2065 7863  urn True.    exc
-00000c30: 6570 7420 5661 6c75 6545 7272 6f72 3a0a  ept ValueError:.
-00000c40: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-00000c50: 616c 7365 0a0a 6465 6620 6c69 7374 5f69  alse..def list_i
-00000c60: 6e74 6567 6572 5f6e 616d 6564 5f66 6f6c  nteger_named_fol
-00000c70: 6465 7273 2872 6f6f 743d 222e 222c 2070  ders(root=".", p
-00000c80: 7265 6669 783d 2727 2c20 7375 6666 6978  refix='', suffix
-00000c90: 3d27 272c 2063 6f6e 7461 696e 696e 675f  ='', containing_
-00000ca0: 6669 6c65 733d 5b5d 2c20 6e6f 745f 636f  files=[], not_co
-00000cb0: 6e74 6169 6e69 6e67 5f66 696c 6573 3d5b  ntaining_files=[
-00000cc0: 5d29 3a0a 2020 2020 2222 2252 6574 7572  ]):.    """Retur
-00000cd0: 6e20 6172 7261 7920 6f66 2069 6e74 6567  n array of integ
-00000ce0: 6572 206e 616d 6564 2066 6f6c 6465 7273  er named folders
-00000cf0: 2e0a 0a20 2020 2053 6361 6e73 2066 6f6c  ...    Scans fol
-00000d00: 6465 7273 2069 6e20 6060 726f 6f74 6060  ders in ``root``
-00000d10: 2061 6e64 2064 6574 6563 7473 2074 686f   and detects tho
-00000d20: 7365 2077 6869 6368 2061 7265 206e 616d  se which are nam
-00000d30: 6564 0a20 2020 2077 6974 6820 616e 2069  ed.    with an i
-00000d40: 6e74 6567 6572 206e 756d 6265 722e 2049  nteger number. I
-00000d50: 7420 7265 7475 726e 7320 7468 656e 2061  t returns then a
-00000d60: 2073 6f72 7465 6420 6c69 7374 206f 6620   sorted list of 
-00000d70: 7468 650a 2020 2020 666f 756e 6420 696e  the.    found in
-00000d80: 7465 6765 7273 2c20 652e 672e 202c 2069  tegers, e.g. , i
-00000d90: 6620 7468 6520 666f 6c64 6572 2073 7472  f the folder str
-00000da0: 7563 7475 7265 2069 733a 3a0a 0a20 2020  ucture is::..   
-00000db0: 2020 2020 2072 6f6f 742f 0a20 2020 2020       root/.     
-00000dc0: 2020 2020 2020 2031 2f0a 2020 2020 2020         1/.      
-00000dd0: 2020 2020 2020 322f 0a20 2020 2020 2020        2/.       
-00000de0: 2020 2020 2035 2f0a 2020 2020 2020 2020       5/.        
-00000df0: 2020 2020 372f 0a20 2020 2020 2020 2020      7/.         
-00000e00: 2020 2038 2f0a 2020 2020 2020 2020 2020     8/.          
-00000e10: 2020 7275 6e5f 322f 0a20 2020 2020 2020    run_2/.       
-00000e20: 2020 2020 2072 756e 5f33 2f0a 2020 2020       run_3/.    
-00000e30: 2020 2020 2020 2020 7275 6e5f 342f 0a20          run_4/. 
-00000e40: 2020 2020 2020 2020 2020 2072 756e 5f35             run_5
-00000e50: 2f0a 2020 2020 2020 2020 2020 2020 7275  /.            ru
-00000e60: 6e5f 6f6c 642f 0a20 2020 2020 2020 2020  n_old/.         
-00000e70: 2020 2066 6f6c 6465 7278 2f0a 2020 2020     folderx/.    
-00000e80: 2020 2020 2020 2020 666f 6c64 6572 792f          foldery/
-00000e90: 0a0a 0a20 2020 2074 6865 6e20 7468 6520  ...    then the 
-00000ea0: 666f 6c6c 6f77 696e 6720 6172 7261 7920  following array 
-00000eb0: 6973 2072 6574 7572 6e65 643a 3a0a 0a20  is returned::.. 
-00000ec0: 2020 2020 2020 205b 312c 322c 352c 372c         [1,2,5,7,
-00000ed0: 385d 2e0a 0a20 2020 2049 6620 6060 7072  8]...    If ``pr
-00000ee0: 6566 6978 6060 2069 7320 7365 7420 746f  efix`` is set to
-00000ef0: 2073 6f6d 6520 7374 7269 6e67 2c20 7468   some string, th
-00000f00: 656e 2069 7420 7265 7475 726e 7320 6120  en it returns a 
-00000f10: 2873 6f72 7465 6429 0a20 2020 206c 6973  (sorted).    lis
-00000f20: 7420 6f66 2073 7472 696e 6773 2e20 466f  t of strings. Fo
-00000f30: 7220 6578 616d 706c 652c 2069 6620 7072  r example, if pr
-00000f40: 6570 656e 6420 6973 2073 6574 2074 6f20  epend is set to 
-00000f50: 6060 2272 756e 5f22 6060 2c20 7468 656e  ``"run_"``, then
-00000f60: 2074 6869 730a 2020 2020 7769 6c6c 2072   this.    will r
-00000f70: 6574 7572 6e20 7468 6520 6172 7261 793a  eturn the array:
-00000f80: 3a0a 0a20 2020 2020 2020 205b 2272 756e  :..        ["run
-00000f90: 5f32 222c 2272 756e 5f33 222c 2272 756e  _2","run_3","run
-00000fa0: 5f34 222c 2272 756e 5f35 225d 0a0a 2020  _4","run_5"]..  
-00000fb0: 2020 5061 7261 6d65 7465 7273 3a0a 0a20    Parameters:.. 
-00000fc0: 2020 2060 6072 6f6f 7460 603a 2073 7472     ``root``: str
-00000fd0: 696e 670a 2020 2020 2020 2020 7061 7468  ing.        path
-00000fe0: 206f 6620 7468 6520 726f 6f74 2066 6f6c   of the root fol
-00000ff0: 6465 7220 696e 2077 6869 6368 2074 6f20  der in which to 
-00001000: 7363 616e 2066 6f72 2069 6e74 6567 6572  scan for integer
-00001010: 206e 616d 6564 2066 6f6c 6465 7273 2e0a   named folders..
-00001020: 2020 2020 6060 7072 6566 6978 6060 3a20      ``prefix``: 
-00001030: 7374 7269 6e67 0a20 2020 2020 2020 2073  string.        s
-00001040: 6361 6e20 666f 7220 666f 6c64 6572 7320  can for folders 
-00001050: 7768 6f73 6520 6e61 6d65 2073 7461 7274  whose name start
-00001060: 7320 7769 7468 2074 6865 2073 7472 696e  s with the strin
-00001070: 6720 6060 7072 6566 6978 6060 2066 6f6c  g ``prefix`` fol
-00001080: 6c6f 7765 640a 2020 2020 2020 2020 6279  lowed.        by
-00001090: 2061 6e64 2069 6e74 6567 6572 206e 756d   and integer num
-000010a0: 6265 7220 2861 6e64 2070 6f73 7369 626c  ber (and possibl
-000010b0: 7920 7468 6520 7374 7269 6e67 2060 6073  y the string ``s
-000010c0: 7566 6669 7860 6029 2e0a 2020 2020 6060  uffix``)..    ``
-000010d0: 7375 6666 6978 6060 3a20 7374 7269 6e67  suffix``: string
-000010e0: 0a20 2020 2020 2020 2073 6361 6e20 666f  .        scan fo
-000010f0: 7220 666f 6c64 6572 7320 7768 6f73 6520  r folders whose 
-00001100: 6e61 6d65 2065 6e64 7320 7769 7468 2074  name ends with t
-00001110: 6865 2073 7472 696e 6720 6060 7375 6666  he string ``suff
-00001120: 6978 6060 2061 6e64 0a20 2020 2020 2020  ix`` and.       
-00001130: 2069 7320 7072 6563 6564 6564 2062 7920   is preceded by 
-00001140: 616e 2069 6e74 6567 6572 206e 756d 6265  an integer numbe
-00001150: 7220 2861 6e64 2070 6f73 7369 626c 7920  r (and possibly 
-00001160: 7468 6520 7374 7269 6e67 2060 6070 7265  the string ``pre
-00001170: 6669 7860 6029 2e0a 2020 2020 6060 636f  fix``)..    ``co
-00001180: 6e74 6169 6e69 6e67 5f66 696c 6573 6060  ntaining_files``
-00001190: 3a20 6172 7261 7920 6f66 2073 7472 696e  : array of strin
-000011a0: 6773 0a20 2020 2020 2020 2061 206c 6973  gs.        a lis
-000011b0: 7420 6f66 2066 696c 6520 6e61 6d65 7320  t of file names 
-000011c0: 7468 6174 2073 686f 756c 6420 6265 2063  that should be c
-000011d0: 6f6e 7461 696e 6564 2069 6e20 7468 6520  ontained in the 
-000011e0: 7265 7475 726e 6564 2066 6f6c 6465 7273  returned folders
-000011f0: 2e0a 2020 2020 6060 6e6f 745f 636f 6e74  ..    ``not_cont
-00001200: 6169 6e69 6e67 5f66 696c 6573 6060 3a20  aining_files``: 
-00001210: 6172 7261 7920 6f66 2073 7472 696e 6773  array of strings
-00001220: 0a20 2020 2020 2020 2061 206c 6973 7420  .        a list 
-00001230: 6f66 2066 696c 6520 6e61 6d65 7320 7468  of file names th
-00001240: 6174 2073 686f 756c 6420 6e6f 7420 6265  at should not be
-00001250: 2063 6f6e 7461 696e 6564 2069 6e20 7468   contained in th
-00001260: 6520 7265 7475 726e 6564 2066 6f6c 6465  e returned folde
-00001270: 7273 2e0a 0a20 2020 2052 6574 7572 6e73  rs...    Returns
-00001280: 3a0a 2020 2020 2020 2020 6172 7261 7920  :.        array 
-00001290: 6f66 2069 6e74 6567 6572 7320 6966 2064  of integers if d
-000012a0: 6566 6175 6c74 2076 616c 7565 2066 6f72  efault value for
-000012b0: 2060 6070 7265 7065 6e64 6060 2069 7320   ``prepend`` is 
-000012c0: 7573 6564 2e20 4f74 6865 7277 6973 650a  used. Otherwise.
-000012d0: 2020 2020 2020 2020 7265 7475 726e 7320          returns 
-000012e0: 616e 2061 7272 6179 206f 6620 7374 7269  an array of stri
-000012f0: 6e67 730a 0a20 2020 2022 2222 0a20 2020  ngs..    """.   
-00001300: 2066 6f6c 6465 7273 203d 2073 7562 5f66   folders = sub_f
-00001310: 6f6c 6465 7273 2872 6f6f 7429 0a0a 2020  olders(root)..  
-00001320: 2020 666c 6973 7420 3d20 5b5d 0a20 2020    flist = [].   
-00001330: 2066 6f72 2066 6f6c 6465 7220 696e 2066   for folder in f
-00001340: 6f6c 6465 7273 3a0a 2020 2020 2020 2020  olders:.        
-00001350: 696e 636c 7564 6520 3d20 5472 7565 0a20  include = True. 
-00001360: 2020 2020 2020 2066 6f72 2066 6e20 696e         for fn in
-00001370: 206e 6f74 5f63 6f6e 7461 696e 696e 675f   not_containing_
-00001380: 6669 6c65 733a 0a20 2020 2020 2020 2020  files:.         
-00001390: 2020 2069 6620 6f73 2e70 6174 682e 6578     if os.path.ex
-000013a0: 6973 7473 286f 732e 7061 7468 2e6a 6f69  ists(os.path.joi
-000013b0: 6e28 726f 6f74 2c66 6f6c 6465 722c 666e  n(root,folder,fn
-000013c0: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-000013d0: 2020 2020 696e 636c 7564 6520 3d20 4661      include = Fa
-000013e0: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
-000013f0: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
-00001400: 2020 6966 206e 6f74 2069 6e63 6c75 6465    if not include
-00001410: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
-00001420: 6e74 696e 7565 0a0a 2020 2020 2020 2020  ntinue..        
-00001430: 666f 7220 666e 2069 6e20 636f 6e74 6169  for fn in contai
-00001440: 6e69 6e67 5f66 696c 6573 3a0a 2020 2020  ning_files:.    
-00001450: 2020 2020 2020 2020 6966 206e 6f74 206f          if not o
-00001460: 732e 7061 7468 2e65 7869 7374 7328 6f73  s.path.exists(os
-00001470: 2e70 6174 682e 6a6f 696e 2872 6f6f 742c  .path.join(root,
-00001480: 666f 6c64 6572 2c66 6e29 293a 0a20 2020  folder,fn)):.   
-00001490: 2020 2020 2020 2020 2020 2020 2069 6e63               inc
-000014a0: 6c75 6465 203d 2046 616c 7365 0a20 2020  lude = False.   
-000014b0: 2020 2020 2020 2020 2020 2020 2062 7265               bre
-000014c0: 616b 0a20 2020 2020 2020 2069 6620 6e6f  ak.        if no
-000014d0: 7420 696e 636c 7564 653a 0a20 2020 2020  t include:.     
-000014e0: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
-000014f0: 0a20 2020 2020 2020 2069 6620 7072 6566  .        if pref
-00001500: 6978 2021 3d20 2727 206f 7220 7375 6666  ix != '' or suff
-00001510: 6978 2021 3d20 2727 3a0a 2020 2020 2020  ix != '':.      
-00001520: 2020 2020 2020 6420 3d20 666f 6c64 6572        d = folder
-00001530: 5b6c 656e 2870 7265 6669 7829 3a5d 5b3a  [len(prefix):][:
-00001540: 2d6c 656e 2873 7566 6669 7829 5d0a 2020  -len(suffix)].  
-00001550: 2020 2020 2020 2020 2020 6966 205f 6973            if _is
-00001560: 5f69 6e74 6567 7261 626c 6528 6429 3a0a  _integrable(d):.
-00001570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001580: 666c 6973 742e 6170 7065 6e64 2869 6e74  flist.append(int
-00001590: 2864 2929 0a20 2020 2020 2020 2065 6c73  (d)).        els
-000015a0: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
-000015b0: 6620 5f69 735f 696e 7465 6772 6162 6c65  f _is_integrable
-000015c0: 2866 6f6c 6465 7229 3a0a 2020 2020 2020  (folder):.      
-000015d0: 2020 2020 2020 2020 2020 666c 6973 742e            flist.
-000015e0: 6170 7065 6e64 2869 6e74 2866 6f6c 6465  append(int(folde
-000015f0: 7229 290a 0a20 2020 2066 6c69 7374 2e73  r))..    flist.s
-00001600: 6f72 7428 290a 0a20 2020 2069 6620 7072  ort()..    if pr
-00001610: 6566 6978 2021 3d20 2727 206f 7220 7375  efix != '' or su
-00001620: 6666 6978 2021 3d20 2727 3a0a 2020 2020  ffix != '':.    
-00001630: 2020 2020 736c 6973 7420 3d20 5b5d 0a20      slist = []. 
-00001640: 2020 2020 2020 2066 6f72 2066 2069 6e20         for f in 
-00001650: 666c 6973 743a 0a20 2020 2020 2020 2020  flist:.         
-00001660: 2020 2073 6c69 7374 2e61 7070 656e 6428     slist.append(
-00001670: 7072 6566 6978 202b 2073 7472 2866 2920  prefix + str(f) 
-00001680: 2b20 7375 6666 6978 290a 0a20 2020 2020  + suffix)..     
-00001690: 2020 2072 6574 7572 6e20 736c 6973 740a     return slist.
-000016a0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-000016b0: 2020 2072 6574 7572 6e20 666c 6973 740a     return flist.
-000016c0: 0a0a 0a64 6566 2061 7461 745f 746f 5f63  ...def atat_to_c
-000016d0: 656c 6c28 6669 6c65 5f70 6174 683d 226c  ell(file_path="l
-000016e0: 6174 2e69 6e22 2c20 696e 7465 7270 7265  at.in", interpre
-000016f0: 745f 6173 3d22 7061 7265 6e74 5f6c 6174  t_as="parent_lat
-00001700: 7469 6365 222c 2070 6172 656e 745f 6c61  tice", parent_la
-00001710: 7474 6963 653d 4e6f 6e65 2c70 6263 3d4e  ttice=None,pbc=N
-00001720: 6f6e 652c 7772 6170 3d54 7275 6529 3a0a  one,wrap=True):.
-00001730: 2020 2020 2222 2250 6172 7365 2061 2060      """Parse a `
-00001740: 606c 6174 2e69 6e60 6020 6f72 2060 6073  `lat.in`` or ``s
-00001750: 7472 2e6f 7574 6060 2066 696c 6520 6672  tr.out`` file fr
-00001760: 6f6d 2060 6041 5441 5460 602e 0a0a 2020  om ``ATAT``...  
-00001770: 2020 6060 4154 4154 6060 2075 7365 7273    ``ATAT`` users
-00001780: 206d 6179 2075 7365 2074 6865 2069 6e70   may use the inp
-00001790: 7574 2066 696c 6573 2066 726f 6d20 6060  ut files from ``
-000017a0: 4154 4154 6060 2074 6f20 7065 7266 6f72  ATAT`` to perfor
-000017b0: 6d20 6120 636c 7573 7465 720a 2020 2020  m a cluster.    
-000017c0: 6578 7061 6e73 696f 6e20 7769 7468 202a  expansion with *
-000017d0: 2a43 454c 4c2a 2a2e 2054 6869 7320 6675  *CELL**. This fu
-000017e0: 6e63 7469 6f6e 2061 6c6c 6f77 7320 746f  nction allows to
-000017f0: 2063 6f6e 7665 7274 2061 6e20 696e 7075   convert an inpu
-00001800: 7420 6060 6c61 742e 696e 6060 0a20 2020  t ``lat.in``.   
-00001810: 2066 696c 6520 6672 6f6d 2060 6041 5441   file from ``ATA
-00001820: 5460 6020 746f 2061 2060 6050 6172 656e  T`` to a ``Paren
-00001830: 744c 6174 7469 6365 6060 206f 626a 6563  tLattice`` objec
-00001840: 7420 696e 2043 454c 4c2e 204f 6e65 206d  t in CELL. One m
-00001850: 6179 2061 6c73 6f20 7265 6164 0a20 2020  ay also read.   
-00001860: 2060 6073 7472 2e6f 7574 6060 2066 696c   ``str.out`` fil
-00001870: 6573 2c20 7768 6963 6820 6172 6520 636f  es, which are co
-00001880: 6e76 6572 7465 6420 746f 2060 6053 7472  nverted to ``Str
-00001890: 7563 7475 7265 6060 206f 626a 6563 7473  ucture`` objects
-000018a0: 2069 6e20 6060 4345 4c4c 6060 2e0a 0a20   in ``CELL``... 
-000018b0: 2020 202a 2a50 6172 616d 6574 6572 733a     **Parameters:
-000018c0: 2a2a 0a0a 2020 2020 6060 6669 6c65 5f70  **..    ``file_p
-000018d0: 6174 6860 603a 2073 7472 696e 670a 2020  ath``: string.  
-000018e0: 2020 2020 2020 7374 7269 6e67 2063 6f6e        string con
-000018f0: 7461 696e 696e 6720 7468 6520 7061 7468  taining the path
-00001900: 206f 6620 7468 6520 6669 6c65 2074 6f20   of the file to 
-00001910: 6265 2070 6172 7365 642e 2054 6865 2066  be parsed. The f
-00001920: 696c 6520 6d75 7374 2068 6176 650a 2020  ile must have.  
-00001930: 2020 2020 2020 666f 726d 6174 2063 6f72        format cor
-00001940: 7265 7370 6f6e 6469 6e67 2074 6f20 6120  responding to a 
-00001950: 6060 6c61 742e 696e 6060 206f 7220 6060  ``lat.in`` or ``
-00001960: 7374 722e 6f75 7460 6020 6669 6c65 2066  str.out`` file f
-00001970: 726f 6d20 4154 4154 2e0a 2020 2020 6060  rom ATAT..    ``
-00001980: 696e 7465 7270 7265 745f 6173 6060 3a20  interpret_as``: 
-00001990: 7374 7269 6e67 206f 7220 4e6f 6e65 0a20  string or None. 
-000019a0: 2020 2020 2020 2049 6e64 6963 6174 6520         Indicate 
-000019b0: 686f 7720 746f 2069 6e74 6572 7072 6574  how to interpret
-000019c0: 2074 6865 2066 696c 6520 696e 2060 6066   the file in ``f
-000019d0: 696c 655f 7061 7468 6060 2e20 506f 7373  ile_path``. Poss
-000019e0: 6962 6c65 2076 616c 7565 7320 6172 653a  ible values are:
-000019f0: 0a0a 2020 2020 2020 2020 2a20 6060 4e6f  ..        * ``No
-00001a00: 6e65 6060 3a0a 2020 2020 2020 2020 2020  ne``:.          
-00001a10: 2020 5468 7265 6520 6172 7261 7973 2061    Three arrays a
-00001a20: 7265 2072 6574 7572 6e65 643a 2060 6063  re returned: ``c
-00001a30: 656c 6c60 602c 2060 6072 6060 2c20 616e  ell``, ``r``, an
-00001a40: 6420 6060 7370 6563 6965 7360 602e 0a20  d ``species``.. 
-00001a50: 2020 2020 2020 202a 2060 6070 6172 656e         * ``paren
-00001a60: 745f 6c61 7474 6963 6560 603a 0a20 2020  t_lattice``:.   
-00001a70: 2020 2020 2020 2020 2054 6865 2072 6563           The rec
-00001a80: 6f6d 6d65 6e64 6564 2076 616c 7565 2069  ommended value i
-00001a90: 6620 6060 6669 6c65 5f70 6174 6860 6020  f ``file_path`` 
-00001aa0: 636f 7272 6573 706f 6e64 7320 746f 0a20  corresponds to. 
-00001ab0: 2020 2020 2020 2020 2020 2061 2060 606c             a ``l
-00001ac0: 6174 2e69 6e60 6020 696e 7075 7420 6669  at.in`` input fi
-00001ad0: 6c65 2066 726f 6d20 4154 4154 2e20 4120  le from ATAT. A 
-00001ae0: 6060 5061 7265 6e74 4c61 7474 6963 6560  ``ParentLattice`
-00001af0: 6020 2a2a 4345 4c4c 2a2a 0a20 2020 2020  ` **CELL**.     
-00001b00: 2020 2020 2020 206f 626a 6563 7420 7769         object wi
-00001b10: 6c6c 2062 6520 7265 7475 726e 6564 2e0a  ll be returned..
-00001b20: 2020 2020 2020 2020 2a20 6060 7375 7065          * ``supe
-00001b30: 725f 6365 6c6c 6060 3a0a 2020 2020 2020  r_cell``:.      
-00001b40: 2020 2020 2020 5468 6520 7265 636f 6d6d        The recomm
-00001b50: 656e 6465 6420 7661 6c75 6520 6966 2060  ended value if `
-00001b60: 6066 696c 655f 7061 7468 6060 2063 6f72  `file_path`` cor
-00001b70: 7265 7370 6f6e 6473 2074 6f0a 2020 2020  responds to.    
-00001b80: 2020 2020 2020 2020 6120 6060 6c61 742e          a ``lat.
-00001b90: 696e 6060 2066 696c 6520 7769 7468 2061  in`` file with a
-00001ba0: 206d 6174 7269 7820 6f66 206c 6174 7469   matrix of latti
-00001bb0: 6365 2076 6563 746f 7273 2028 6060 752c  ce vectors (``u,
-00001bc0: 762c 7760 6020 696e 0a20 2020 2020 2020  v,w`` in.       
-00001bd0: 2020 2020 2060 4154 4154 2064 6f63 203c       `ATAT doc <
-00001be0: 6874 7470 733a 2f2f 7777 772e 6272 6f77  https://www.brow
-00001bf0: 6e2e 6564 752f 4465 7061 7274 6d65 6e74  n.edu/Department
-00001c00: 732f 456e 6769 6e65 6572 696e 672f 4c61  s/Engineering/La
-00001c10: 6273 2f61 7664 772f 6174 6174 2f6d 616e  bs/avdw/atat/man
-00001c20: 7561 6c2f 6e6f 6465 3335 2e68 746d 6c3e  ual/node35.html>
-00001c30: 605f 290a 2020 2020 2020 2020 2020 2020  `_).            
-00001c40: 6469 6666 6572 656e 7420 746f 2074 6865  different to the
-00001c50: 2069 6465 6e74 6974 792c 206f 7220 6966   identity, or if
-00001c60: 2069 7420 6973 206b 6e6f 776e 2074 6861   it is known tha
-00001c70: 7420 7468 6520 7374 7275 6374 7572 6520  t the structure 
-00001c80: 6973 0a20 2020 2020 2020 2020 2020 2061  is.            a
-00001c90: 2070 6572 696f 6469 6320 7265 7065 7469   periodic repeti
-00001ca0: 7469 6f6e 206f 6620 6120 7061 7265 6e74  tion of a parent
-00001cb0: 206c 6174 7469 6365 2e20 466f 7220 7468   lattice. For th
-00001cc0: 6973 206f 7074 696f 6e2c 2074 6865 2070  is option, the p
-00001cd0: 6172 656e 740a 2020 2020 2020 2020 2020  arent.          
-00001ce0: 2020 6c61 7474 6963 6520 6d75 7374 2062    lattice must b
-00001cf0: 6520 7072 6f76 6964 6564 2028 7365 6520  e provided (see 
-00001d00: 6060 7061 7265 6e74 5f6c 6174 7469 6365  ``parent_lattice
-00001d10: 6060 2070 6172 616d 6574 6572 2062 656c  `` parameter bel
-00001d20: 6f77 292e 0a20 2020 2020 2020 2020 2020  ow)..           
-00001d30: 2041 2060 6053 7570 6572 4365 6c6c 6060   A ``SuperCell``
-00001d40: 206f 626a 6563 7420 7769 6c6c 2062 6520   object will be 
-00001d50: 7265 7475 726e 6564 2e0a 2020 2020 2020  returned..      
-00001d60: 2020 2a20 6060 7374 7275 6374 7572 6560    * ``structure`
-00001d70: 603a 0a20 2020 2020 2020 2020 2020 2054  `:.            T
-00001d80: 6865 2072 6563 6f6d 6d65 6e64 6564 2076  he recommended v
-00001d90: 616c 7565 2069 6620 6060 6669 6c65 5f70  alue if ``file_p
-00001da0: 6174 6860 6020 636f 7272 6573 706f 6e64  ath`` correspond
-00001db0: 7320 746f 0a20 2020 2020 2020 2020 2020  s to.           
-00001dc0: 2061 2060 6073 7472 2e6f 7574 6060 2066   a ``str.out`` f
-00001dd0: 696c 6520 6672 6f6d 2041 5441 542e 2046  ile from ATAT. F
-00001de0: 6f72 2074 6869 7320 6f70 7469 6f6e 2c20  or this option, 
-00001df0: 7468 6520 7061 7265 6e74 0a20 2020 2020  the parent.     
-00001e00: 2020 2020 2020 206c 6174 7469 6365 206d         lattice m
-00001e10: 7573 7420 6265 2070 726f 7669 6465 6420  ust be provided 
-00001e20: 2873 6565 2060 6070 6172 656e 745f 6c61  (see ``parent_la
-00001e30: 7474 6963 6560 6020 7061 7261 6d65 7465  ttice`` paramete
-00001e40: 7220 6265 6c6f 7729 2e0a 2020 2020 2020  r below)..      
-00001e50: 2020 2020 2020 496e 2074 6869 7320 6361        In this ca
-00001e60: 7365 2061 2060 6053 7472 7563 7475 7265  se a ``Structure
-00001e70: 6060 206f 626a 6563 7420 7769 6c6c 2062  `` object will b
-00001e80: 6520 7265 7475 726e 6564 2e0a 0a20 2020  e returned...   
-00001e90: 2060 6070 6172 656e 745f 6c61 7474 6963   ``parent_lattic
-00001ea0: 6560 603a 2050 6172 656e 744c 6174 7469  e``: ParentLatti
-00001eb0: 6365 206f 626a 6563 740a 2020 2020 2020  ce object.      
-00001ec0: 2020 4966 2060 6069 6e74 6572 7072 6574    If ``interpret
-00001ed0: 5f61 7360 6020 6973 2060 6073 7570 6572  _as`` is ``super
-00001ee0: 5f63 656c 6c60 6020 6f72 2060 6073 7472  _cell`` or ``str
-00001ef0: 7563 7475 7265 6060 2c20 6120 7061 7265  ucture``, a pare
-00001f00: 6e74 206c 6174 7469 6365 0a20 2020 2020  nt lattice.     
-00001f10: 2020 206d 7573 7420 6265 2070 726f 7669     must be provi
-00001f20: 6465 642e 2054 6869 7320 6d75 7374 2062  ded. This must b
-00001f30: 6520 636f 6d70 6174 6962 6c65 2077 6974  e compatible wit
-00001f40: 6820 7468 6520 696e 666f 726d 6174 696f  h the informatio
-00001f50: 6e20 696e 2074 6865 0a20 2020 2020 2020  n in the.       
-00001f60: 2060 606c 6174 2e69 6e60 6020 6669 6c65   ``lat.in`` file
-00001f70: 2074 6861 7420 7761 7320 7573 6564 2074   that was used t
-00001f80: 6f20 6372 6561 7465 2074 6865 2060 6073  o create the ``s
-00001f90: 7472 2e6f 7574 6060 2066 696c 6573 2e20  tr.out`` files. 
-00001fa0: 5365 6520 7468 650a 2020 2020 2020 2020  See the.        
-00001fb0: 6578 616d 706c 6573 2062 656c 6f77 2e0a  examples below..
-00001fc0: 2020 2020 6060 7062 6360 603a 206f 6e65      ``pbc``: one
-00001fd0: 206f 7220 7468 7265 6520 626f 6f6c 2028   or three bool (
-00001fe0: 7361 6d65 2061 7320 4153 4527 7320 4174  same as ASE's At
-00001ff0: 6f6d 7320 6f62 6a65 6374 290a 2020 2020  oms object).    
-00002000: 2020 2020 5065 7269 6f64 6963 2062 6f75      Periodic bou
-00002010: 6e64 6172 7920 636f 6e64 6974 696f 6e73  ndary conditions
-00002020: 2066 6c61 6773 2e20 4578 616d 706c 6573   flags. Examples
-00002030: 3a20 5472 7565 2c20 4661 6c73 652c 2030  : True, False, 0
-00002040: 2c20 312c 0a20 2020 2020 2020 2028 312c  , 1,.        (1,
-00002050: 2031 2c20 3029 2c20 2854 7275 652c 2046   1, 0), (True, F
-00002060: 616c 7365 2c20 4661 6c73 6529 2e20 4465  alse, False). De
-00002070: 6661 756c 7420 7661 6c75 653a 2046 616c  fault value: Fal
-00002080: 7365 2e20 5468 6520 7265 7475 726e 6564  se. The returned
-00002090: 0a20 2020 2020 2020 202a 2a43 454c 4c2a  .        **CELL*
-000020a0: 2a20 6f62 6a65 6374 7320 7769 6c6c 2068  * objects will h
-000020b0: 6176 6520 7468 6573 6520 7062 6327 7320  ave these pbc's 
-000020c0: 7365 7420 7570 2e0a 2020 2020 6060 7772  set up..    ``wr
-000020d0: 6170 6060 3a20 626f 6f6c 6561 6e20 2864  ap``: boolean (d
-000020e0: 6566 6175 6c74 3a60 6054 7275 6560 6029  efault:``True``)
-000020f0: 0a20 2020 2020 2020 2057 7261 7020 6174  .        Wrap at
-00002100: 6f6d 6963 2063 6f6f 7264 696e 6174 6573  omic coordinates
-00002110: 2e20 4966 2070 6263 2069 7320 6060 4e6f  . If pbc is ``No
-00002120: 6e65 6060 2c20 7062 6320 6973 2073 6574  ne``, pbc is set
-00002130: 2074 6f20 2831 2c31 2c31 292e 0a20 2020   to (1,1,1)..   
-00002140: 2020 2020 2053 6574 2060 6077 7261 7060       Set ``wrap`
-00002150: 6020 746f 2060 6046 616c 7365 6060 2069  ` to ``False`` i
-00002160: 6620 7374 7275 6374 7572 6520 636f 7272  f structure corr
-00002170: 6573 706f 6e64 730a 2020 2020 2020 2020  esponds.        
-00002180: 746f 2061 2073 7570 6572 6365 6c6c 2c20  to a supercell, 
-00002190: 692e 652e 2c20 6966 2074 6865 2073 6563  i.e., if the sec
-000021a0: 6f6e 6420 6d61 7472 6978 206f 6620 7468  ond matrix of th
-000021b0: 6520 7374 7275 6374 7572 6520 6465 6669  e structure defi
-000021c0: 6e69 7469 6f6e 0a20 2020 2020 2020 2069  nition.        i
-000021d0: 6e20 6569 7468 6572 2074 6865 206c 6174  n either the lat
-000021e0: 2e69 6e20 6f72 2073 7472 2e6f 7574 2066  .in or str.out f
-000021f0: 696c 6520 6973 2064 6966 6665 7265 6e74  ile is different
-00002200: 2066 726f 6d20 7468 6520 6964 656e 7469   from the identi
-00002210: 7479 0a20 2020 2020 2020 206d 6174 7269  ty.        matri
-00002220: 782e 0a0a 2020 2020 2a2a 5265 7475 726e  x...    **Return
-00002230: 733a 2a2a 0a0a 2020 2020 4465 7065 6e64  s:**..    Depend
-00002240: 696e 6720 6f6e 2074 6865 2076 616c 7565  ing on the value
-00002250: 206f 6620 6060 696e 7465 7270 7265 745f   of ``interpret_
-00002260: 6173 6060 2c20 7468 6520 7265 7475 726e  as``, the return
-00002270: 6564 206f 626a 6563 7420 6361 6e20 6265  ed object can be
-00002280: 2070 7974 686f 6e0a 2020 2020 6172 7261   python.    arra
-00002290: 7973 2028 6060 696e 7465 7270 7265 745f  ys (``interpret_
-000022a0: 6173 3d4e 6f6e 6560 6029 2c20 6120 6060  as=None``), a ``
-000022b0: 5061 7265 6e74 4c61 7474 6963 6560 600a  ParentLattice``.
-000022c0: 2020 2020 2860 6069 6e74 6572 7072 6574      (``interpret
-000022d0: 5f61 733d 2270 6172 656e 745f 6c61 7474  _as="parent_latt
-000022e0: 6963 6522 6060 292c 2061 2060 6053 7570  ice"``), a ``Sup
-000022f0: 6572 4365 6c6c 6060 0a20 2020 2028 6060  erCell``.    (``
-00002300: 696e 7465 7270 7265 745f 6173 3d22 7375  interpret_as="su
-00002310: 7065 725f 6365 6c6c 2260 6029 2c20 6f72  per_cell"``), or
-00002320: 2061 2060 6053 7472 7563 7475 7265 6060   a ``Structure``
-00002330: 0a20 2020 2028 6060 696e 7465 7270 7265  .    (``interpre
-00002340: 745f 6173 3d22 5374 7275 6374 7572 6522  t_as="Structure"
-00002350: 6060 292e 0a0a 2020 2020 2a2a 4578 616d  ``)...    **Exam
-00002360: 706c 6573 3a2a 2a0a 0a20 2020 202e 2e20  ples:**..    .. 
-00002370: 746f 646f 3a3a 0a20 2020 2020 2020 2043  todo::.        C
-00002380: 6c61 7269 6679 2077 7261 7020 6f70 7469  larify wrap opti
-00002390: 6f6e 2e20 5269 6768 7420 6e6f 7720 6974  on. Right now it
-000023a0: 2069 7320 6e6f 7420 6775 6172 616e 7465   is not guarante
-000023b0: 6564 2074 6f0a 2020 2020 2020 2020 776f  ed to.        wo
-000023c0: 726b 2077 6865 6e20 7468 6520 7375 7065  rk when the supe
-000023d0: 7263 656c 6c20 6465 6669 6e69 7469 6f6e  rcell definition
-000023e0: 2069 6e20 6c61 742e 696e 2069 7320 6e6f   in lat.in is no
-000023f0: 7420 7468 650a 2020 2020 2020 2020 6964  t the.        id
-00002400: 656e 7469 7479 206d 6174 7269 782e 2054  entity matrix. T
-00002410: 6869 7320 6973 2073 6f2c 2062 6563 6175  his is so, becau
-00002420: 7365 2069 6e20 7468 6520 6c61 742e 696e  se in the lat.in
-00002430: 2066 6f72 6d61 740a 2020 2020 2020 2020   format.        
-00002440: 7468 6520 7363 616c 6564 2063 6f6f 7264  the scaled coord
-00002450: 696e 6174 6573 2061 7265 2067 6976 656e  inates are given
-00002460: 2069 6e20 7265 6665 7265 6e63 6520 746f   in reference to
-00002470: 2074 6865 0a20 2020 2020 2020 2063 6172   the.        car
-00002480: 7465 7369 616e 2076 6563 746f 7273 206f  tesian vectors o
-00002490: 6620 7468 6520 7061 7265 6e74 206c 6174  f the parent lat
-000024a0: 7469 6365 2c20 6275 7420 6d61 7920 6465  tice, but may de
-000024b0: 6669 6e65 2061 0a20 2020 2020 2020 2073  fine a.        s
-000024c0: 7570 6572 6365 6c6c 2e20 4669 7820 6974  upercell. Fix it
-000024d0: 2073 7563 6820 7468 6174 2074 6865 2078   such that the x
-000024e0: 206d 6174 7269 7820 6265 6c6f 7720 7265   matrix below re
-000024f0: 6665 7272 7320 746f 0a20 2020 2020 2020  ferrs to.       
-00002500: 2061 2a62 2061 6e64 206e 6f74 2062 2061   a*b and not b a
-00002510: 7320 6974 2069 7320 6e6f 772e 0a0a 2020  s it is now...  
-00002520: 2020 2222 220a 2020 2020 6672 6f6d 2061    """.    from a
-00002530: 7365 2e64 6174 6120 696d 706f 7274 2061  se.data import a
-00002540: 746f 6d69 635f 6e75 6d62 6572 730a 2020  tomic_numbers.  
-00002550: 2020 6672 6f6d 2063 6f70 7920 696d 706f    from copy impo
-00002560: 7274 2064 6565 7063 6f70 790a 2020 2020  rt deepcopy.    
-00002570: 6672 6f6d 2061 7365 2069 6d70 6f72 7420  from ase import 
-00002580: 4174 6f6d 730a 2020 2020 6620 3d20 6f70  Atoms.    f = op
-00002590: 656e 2866 696c 655f 7061 7468 290a 2020  en(file_path).  
-000025a0: 2020 6c69 6e65 7320 3d20 662e 7265 6164    lines = f.read
-000025b0: 6c69 6e65 7328 290a 2020 2020 662e 636c  lines().    f.cl
-000025c0: 6f73 6528 290a 0a20 2020 206c 6174 203d  ose()..    lat =
-000025d0: 205b 5d0a 0a20 2020 206c 6174 2e61 7070   []..    lat.app
-000025e0: 656e 6428 5b5d 290a 2020 2020 6c6e 6e3d  end([]).    lnn=
-000025f0: 300a 2020 2020 666f 7220 6c6e 2c6c 696e  0.    for ln,lin
-00002600: 6520 696e 2065 6e75 6d65 7261 7465 286c  e in enumerate(l
-00002610: 696e 6573 293a 0a20 2020 2020 2020 206c  ines):.        l
-00002620: 7320 3d20 6c69 6e65 2e73 706c 6974 2829  s = line.split()
-00002630: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-00002640: 6c73 293e 303a 0a20 2020 2020 2020 2020  ls)>0:.         
-00002650: 2020 2069 6620 6c6e 203c 2033 3a0a 2020     if ln < 3:.  
-00002660: 2020 2020 2020 2020 2020 2020 2020 6c61                la
-00002670: 745b 305d 2e61 7070 656e 6428 5b66 6c6f  t[0].append([flo
-00002680: 6174 286c 735b 305d 292c 666c 6f61 7428  at(ls[0]),float(
-00002690: 6c73 5b31 5d29 2c66 6c6f 6174 286c 735b  ls[1]),float(ls[
-000026a0: 325d 295d 290a 2020 2020 2020 2020 2020  2])]).          
-000026b0: 2020 6966 206c 6e20 3d3d 2032 3a20 6c61    if ln == 2: la
-000026c0: 742e 6170 7065 6e64 285b 5d29 0a20 2020  t.append([]).   
-000026d0: 2020 2020 2020 2020 2069 6620 6c6e 203e           if ln >
-000026e0: 2032 2061 6e64 206c 6e20 3c20 363a 0a20   2 and ln < 6:. 
-000026f0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00002700: 6174 5b31 5d2e 6170 7065 6e64 285b 666c  at[1].append([fl
-00002710: 6f61 7428 6c73 5b30 5d29 2c66 6c6f 6174  oat(ls[0]),float
-00002720: 286c 735b 315d 292c 666c 6f61 7428 6c73  (ls[1]),float(ls
-00002730: 5b32 5d29 5d29 0a20 2020 2020 2020 2020  [2])]).         
-00002740: 2020 2069 6620 6c6e 203d 3d20 353a 206c     if ln == 5: l
-00002750: 6174 2e61 7070 656e 6428 5b5d 290a 2020  at.append([]).  
-00002760: 2020 2020 2020 2020 2020 6966 206c 6e20            if ln 
-00002770: 3e3d 2036 3a0a 2020 2020 2020 2020 2020  >= 6:.          
-00002780: 2020 2020 2020 6c61 745b 325d 2e61 7070        lat[2].app
-00002790: 656e 6428 5b5d 290a 2020 2020 2020 2020  end([]).        
-000027a0: 2020 2020 2020 2020 733d 2727 2e6a 6f69          s=''.joi
-000027b0: 6e28 6c73 5b33 3a5d 292e 7370 6c69 7428  n(ls[3:]).split(
-000027c0: 272c 2729 0a20 2020 2020 2020 2020 2020  ',').           
-000027d0: 2020 2020 206c 6174 5b32 5d5b 6c6e 6e5d       lat[2][lnn]
-000027e0: 2e61 7070 656e 6428 5b66 6c6f 6174 286c  .append([float(l
-000027f0: 735b 305d 292c 666c 6f61 7428 6c73 5b31  s[0]),float(ls[1
-00002800: 5d29 2c66 6c6f 6174 286c 735b 325d 295d  ]),float(ls[2])]
-00002810: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00002820: 2020 6c61 745b 325d 5b6c 6e6e 5d2e 6170    lat[2][lnn].ap
-00002830: 7065 6e64 2873 290a 2020 2020 2020 2020  pend(s).        
-00002840: 2020 2020 2020 2020 6c6e 6e20 3d20 6c6e          lnn = ln
-00002850: 6e20 2b20 310a 0a20 2020 2073 7472 7563  n + 1..    struc
-00002860: 203d 2064 6565 7063 6f70 7928 6c61 7429   = deepcopy(lat)
-00002870: 0a0a 2020 2020 2320 5772 6974 6520 636f  ..    # Write co
-00002880: 6f72 6469 6e61 7465 2073 7973 7465 6d0a  ordinate system.
-00002890: 2020 2020 7061 7265 6e74 3d5b 5d0a 2020      parent=[].  
-000028a0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-000028b0: 2833 293a 0a20 2020 2020 2020 2020 2020  (3):.           
-000028c0: 2070 6172 656e 742e 6170 7065 6e64 285b   parent.append([
-000028d0: 7374 7275 635b 305d 5b69 5d5b 305d 2c73  struc[0][i][0],s
-000028e0: 7472 7563 5b30 5d5b 695d 5b31 5d2c 7374  truc[0][i][1],st
-000028f0: 7275 635b 305d 5b69 5d5b 325d 5d29 0a0a  ruc[0][i][2]])..
-00002900: 2020 2020 2320 5772 6974 6520 6c61 7474      # Write latt
-00002910: 6963 650a 2020 2020 7363 656c 6c20 3d20  ice.    scell = 
-00002920: 5b5d 0a20 2020 2066 6f72 2069 2069 6e20  [].    for i in 
-00002930: 7261 6e67 6528 3329 3a0a 2020 2020 2020  range(3):.      
-00002940: 2020 7363 656c 6c2e 6170 7065 6e64 285b    scell.append([
-00002950: 7374 7275 635b 315d 5b69 5d5b 305d 2c73  struc[1][i][0],s
-00002960: 7472 7563 5b31 5d5b 695d 5b31 5d2c 7374  truc[1][i][1],st
-00002970: 7275 635b 315d 5b69 5d5b 325d 5d29 0a0a  ruc[1][i][2]])..
-00002980: 2020 2020 2320 5772 6974 6520 6174 6f6d      # Write atom
-00002990: 730a 2020 2020 7820 3d20 5b5d 0a20 2020  s.    x = [].   
-000029a0: 2073 7065 6369 6573 203d 205b 5d0a 2020   species = [].  
-000029b0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-000029c0: 286c 656e 2873 7472 7563 5b32 5d29 293a  (len(struc[2])):
-000029d0: 0a20 2020 2020 2020 2078 2e61 7070 656e  .        x.appen
-000029e0: 6428 5b73 7472 7563 5b32 5d5b 695d 5b30  d([struc[2][i][0
-000029f0: 5d5b 305d 2c73 7472 7563 5b32 5d5b 695d  ][0],struc[2][i]
-00002a00: 5b30 5d5b 315d 2c73 7472 7563 5b32 5d5b  [0][1],struc[2][
-00002a10: 695d 5b30 5d5b 325d 5d29 0a20 2020 2020  i][0][2]]).     
-00002a20: 2020 206e 7273 203d 205b 5d0a 2020 2020     nrs = [].    
-00002a30: 2020 2020 666f 7220 7370 2069 6e20 7374      for sp in st
-00002a40: 7275 635b 325d 5b69 5d5b 315d 3a0a 2020  ruc[2][i][1]:.  
-00002a50: 2020 2020 2020 2020 2020 6966 2073 7020            if sp 
-00002a60: 3d3d 2022 5661 6322 206f 7220 7370 203d  == "Vac" or sp =
-00002a70: 3d20 2256 223a 0a20 2020 2020 2020 2020  = "V":.         
-00002a80: 2020 2020 2020 2073 7020 3d20 2258 220a         sp = "X".
-00002a90: 2020 2020 2020 2020 2020 2020 6e72 732e              nrs.
-00002aa0: 6170 7065 6e64 2861 746f 6d69 635f 6e75  append(atomic_nu
-00002ab0: 6d62 6572 735b 7370 5d29 0a20 2020 2020  mbers[sp]).     
-00002ac0: 2020 2073 7065 6369 6573 2e61 7070 656e     species.appen
-00002ad0: 6428 6e72 7329 0a0a 2020 2020 7820 3d20  d(nrs)..    x = 
-00002ae0: 6e70 2e6d 6174 7269 7828 7829 0a20 2020  np.matrix(x).   
-00002af0: 2062 203d 206e 702e 6d61 7472 6978 2870   b = np.matrix(p
-00002b00: 6172 656e 7429 0a20 2020 2061 203d 206e  arent).    a = n
-00002b10: 702e 6d61 7472 6978 2873 6365 6c6c 290a  p.matrix(scell).
-00002b20: 0a20 2020 2023 2323 2323 2323 2323 2323  .    ###########
-00002b30: 2323 2323 2323 2323 230a 2020 2020 2320  #########.    # 
-00002b40: 4361 6c63 756c 6174 6520 7265 616c 2063  Calculate real c
-00002b50: 6172 7465 7369 616e 2063 6f6f 7264 696e  artesian coordin
-00002b60: 6174 6573 0a20 2020 2069 6620 7772 6170  ates.    if wrap
-00002b70: 3a0a 2020 2020 2020 2020 6672 6f6d 2063  :.        from c
-00002b80: 6c75 7374 6572 782e 7379 6d6d 6574 7279  lusterx.symmetry
-00002b90: 2069 6d70 6f72 7420 7772 6170 5f73 6361   import wrap_sca
-00002ba0: 6c65 645f 706f 7369 7469 6f6e 730a 2020  led_positions.  
-00002bb0: 2020 2020 2020 6966 2070 6263 203d 3d20        if pbc == 
-00002bc0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00002bd0: 2020 7062 6320 3d20 2831 2c31 2c31 290a    pbc = (1,1,1).
-00002be0: 2020 2020 2020 2020 7820 3d20 7772 6170          x = wrap
-00002bf0: 5f73 6361 6c65 645f 706f 7369 7469 6f6e  _scaled_position
-00002c00: 7328 782c 7062 6329 0a20 2020 2072 203d  s(x,pbc).    r =
-00002c10: 2078 2a62 0a0a 2020 2020 6365 6c6c 203d   x*b..    cell =
-00002c20: 2061 2a62 0a20 2020 2069 6620 696e 7465   a*b.    if inte
-00002c30: 7270 7265 745f 6173 203d 3d20 4e6f 6e65  rpret_as == None
-00002c40: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00002c50: 2063 656c 6c2c 2072 2c20 7370 6563 6965   cell, r, specie
-00002c60: 730a 2020 2020 6966 2069 6e74 6572 7072  s.    if interpr
-00002c70: 6574 5f61 7320 3d3d 2022 7061 7265 6e74  et_as == "parent
-00002c80: 5f6c 6174 7469 6365 223a 0a20 2020 2020  _lattice":.     
-00002c90: 2020 2066 726f 6d20 636c 7573 7465 7278     from clusterx
-00002ca0: 2e70 6172 656e 745f 6c61 7474 6963 6520  .parent_lattice 
-00002cb0: 696d 706f 7274 2050 6172 656e 744c 6174  import ParentLat
-00002cc0: 7469 6365 0a20 2020 2020 2020 206e 7273  tice.        nrs
-00002cd0: 203d 206e 702e 7a65 726f 7328 6c65 6e28   = np.zeros(len(
-00002ce0: 7370 6563 6965 7329 290a 2020 2020 2020  species)).      
-00002cf0: 2020 666f 7220 696e 722c 206e 7220 696e    for inr, nr in
-00002d00: 2065 6e75 6d65 7261 7465 2873 7065 6369   enumerate(speci
-00002d10: 6573 293a 0a20 2020 2020 2020 2020 2020  es):.           
-00002d20: 206e 7273 5b69 6e72 5d3d 696e 7428 6e72   nrs[inr]=int(nr
-00002d30: 5b30 5d29 0a0a 2020 2020 2020 2020 706c  [0])..        pl
-00002d40: 6174 203d 2050 6172 656e 744c 6174 7469  at = ParentLatti
-00002d50: 6365 2841 746f 6d73 2870 6f73 6974 696f  ce(Atoms(positio
-00002d60: 6e73 3d72 2c63 656c 6c3d 6365 6c6c 2c6e  ns=r,cell=cell,n
-00002d70: 756d 6265 7273 3d6e 7273 2c70 6263 3d70  umbers=nrs,pbc=p
-00002d80: 6263 292c 7369 7465 733d 7370 6563 6965  bc),sites=specie
-00002d90: 732c 7062 633d 7062 6329 0a20 2020 2020  s,pbc=pbc).     
-00002da0: 2020 2072 6574 7572 6e20 706c 6174 0a20     return plat. 
-00002db0: 2020 2069 6620 696e 7465 7270 7265 745f     if interpret_
-00002dc0: 6173 203d 3d20 2273 7570 6572 5f63 656c  as == "super_cel
-00002dd0: 6c22 3a0a 2020 2020 2020 2020 6672 6f6d  l":.        from
-00002de0: 2063 6c75 7374 6572 782e 7374 7275 6374   clusterx.struct
-00002df0: 7572 6520 696d 706f 7274 2053 7472 7563  ure import Struc
-00002e00: 7475 7265 0a20 2020 2020 2020 2070 6365  ture.        pce
-00002e10: 6c6c 203d 2070 6172 656e 745f 6c61 7474  ll = parent_latt
-00002e20: 6963 652e 6765 745f 6365 6c6c 2829 0a20  ice.get_cell(). 
-00002e30: 2020 2020 2020 2074 6d61 7420 3d20 6e70         tmat = np
-00002e40: 2e61 7361 7272 6179 286e 702e 7269 6e74  .asarray(np.rint
-00002e50: 286e 702e 646f 7428 6365 6c6c 2c6e 702e  (np.dot(cell,np.
-00002e60: 6c69 6e61 6c67 2e69 6e76 2870 6365 6c6c  linalg.inv(pcell
-00002e70: 2929 292e 6173 7479 7065 2869 6e74 2929  ))).astype(int))
-00002e80: 0a20 2020 2020 2020 2066 726f 6d20 636c  .        from cl
-00002e90: 7573 7465 7278 2e73 7570 6572 5f63 656c  usterx.super_cel
-00002ea0: 6c20 696d 706f 7274 2053 7570 6572 4365  l import SuperCe
-00002eb0: 6c6c 0a20 2020 2020 2020 2073 6365 6c6c  ll.        scell
-00002ec0: 203d 2053 7570 6572 4365 6c6c 2870 6172   = SuperCell(par
-00002ed0: 656e 745f 6c61 7474 6963 652c 746d 6174  ent_lattice,tmat
-00002ee0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00002ef0: 2073 6365 6c6c 0a20 2020 2069 6620 696e   scell.    if in
-00002f00: 7465 7270 7265 745f 6173 203d 3d20 2273  terpret_as == "s
-00002f10: 7472 7563 7475 7265 223a 0a20 2020 2020  tructure":.     
-00002f20: 2020 2066 726f 6d20 636c 7573 7465 7278     from clusterx
-00002f30: 2e73 7472 7563 7475 7265 2069 6d70 6f72  .structure impor
-00002f40: 7420 5374 7275 6374 7572 650a 2020 2020  t Structure.    
-00002f50: 2020 2020 7063 656c 6c20 3d20 7061 7265      pcell = pare
-00002f60: 6e74 5f6c 6174 7469 6365 2e67 6574 5f63  nt_lattice.get_c
-00002f70: 656c 6c28 290a 2020 2020 2020 2020 746d  ell().        tm
-00002f80: 6174 203d 206e 702e 6173 6172 7261 7928  at = np.asarray(
-00002f90: 6e70 2e72 696e 7428 6e70 2e64 6f74 2863  np.rint(np.dot(c
-00002fa0: 656c 6c2c 6e70 2e6c 696e 616c 672e 696e  ell,np.linalg.in
-00002fb0: 7628 7063 656c 6c29 2929 2e61 7374 7970  v(pcell))).astyp
-00002fc0: 6528 696e 7429 290a 2020 2020 2020 2020  e(int)).        
-00002fd0: 6672 6f6d 2063 6c75 7374 6572 782e 7375  from clusterx.su
-00002fe0: 7065 725f 6365 6c6c 2069 6d70 6f72 7420  per_cell import 
-00002ff0: 5375 7065 7243 656c 6c0a 2020 2020 2020  SuperCell.      
-00003000: 2020 7363 656c 6c20 3d20 5375 7065 7243    scell = SuperC
-00003010: 656c 6c28 7061 7265 6e74 5f6c 6174 7469  ell(parent_latti
-00003020: 6365 2c74 6d61 7429 0a20 2020 2020 2020  ce,tmat).       
-00003030: 2070 7269 7320 3d20 7363 656c 6c2e 6765   pris = scell.ge
-00003040: 745f 7072 6973 7469 6e65 2829 0a0a 2020  t_pristine()..  
-00003050: 2020 2020 2020 706f 7320 3d20 7072 6973        pos = pris
-00003060: 2e67 6574 5f70 6f73 6974 696f 6e73 2829  .get_positions()
-00003070: 0a20 2020 2020 2020 206e 6577 5f6e 7273  .        new_nrs
-00003080: 203d 206e 702e 7a65 726f 7328 6c65 6e28   = np.zeros(len(
-00003090: 706f 7329 290a 2020 2020 2020 2020 666f  pos)).        fo
-000030a0: 7220 6970 2c70 2069 6e20 656e 756d 6572  r ip,p in enumer
-000030b0: 6174 6528 7229 3a0a 2020 2020 2020 2020  ate(r):.        
-000030c0: 2020 2020 6e72 203d 2073 7065 6369 6573      nr = species
-000030d0: 5b69 705d 5b30 5d0a 2020 2020 2020 2020  [ip][0].        
-000030e0: 2020 2020 666f 7220 6932 2c70 3220 696e      for i2,p2 in
-000030f0: 2065 6e75 6d65 7261 7465 2870 6f73 293a   enumerate(pos):
-00003100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003110: 2069 6620 6973 636c 6f73 6528 702c 7032   if isclose(p,p2
-00003120: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00003130: 2020 2020 2020 206e 6577 5f6e 7273 5b69         new_nrs[i
-00003140: 325d 203d 206e 720a 0a20 2020 2020 2020  2] = nr..       
-00003150: 2073 7472 7563 203d 2053 7472 7563 7475   struc = Structu
-00003160: 7265 2873 6365 6c6c 2c64 6563 6f72 6174  re(scell,decorat
-00003170: 696f 6e3d 6e65 775f 6e72 7329 0a20 2020  ion=new_nrs).   
-00003180: 2020 2020 2072 6574 7572 6e20 7374 7275       return stru
-00003190: 630a 0a64 6566 2067 6574 5f75 6e69 7175  c..def get_uniqu
-000031a0: 655f 7375 7065 7263 656c 6c73 286e 2c70  e_supercells(n,p
-000031b0: 6172 656e 745f 6c61 7474 6963 6529 3a0a  arent_lattice):.
-000031c0: 2020 2020 2222 2246 696e 6420 6675 6c6c      """Find full
-000031d0: 206c 6973 7420 6f66 2075 6e69 7175 6520   list of unique 
-000031e0: 7375 7065 7263 656c 6c73 206f 6620 696e  supercells of in
-000031f0: 6465 7820 6e2e 0a0a 2020 2020 466f 6c6c  dex n...    Foll
-00003200: 6f77 696e 6720 5265 662e 5b31 5d2c 2074  owing Ref.[1], t
-00003210: 6865 2063 6f6d 706c 6574 6520 7365 7420  he complete set 
-00003220: 6f66 2073 796d 6d65 7472 6963 616c 6c79  of symmetrically
-00003230: 2069 6e65 7175 6976 616c 656e 7420 484e   inequivalent HN
-00003240: 4673 206f 660a 2020 2020 696e 6465 7820  Fs of.    index 
-00003250: 6060 6e60 602c 2066 6f72 2061 2067 6976  ``n``, for a giv
-00003260: 656e 2060 6070 6172 656e 745f 6c61 7474  en ``parent_latt
-00003270: 6963 6560 602c 2069 7320 6465 7465 726d  ice``, is determ
-00003280: 696e 6564 2061 6e64 2072 6574 7572 6e65  ined and returne
-00003290: 642e 0a0a 2020 2020 5b31 5d20 4775 7320  d...    [1] Gus 
-000032a0: 4c2e 2057 2e20 4861 7274 2061 6e64 2052  L. W. Hart and R
-000032b0: 6f64 6e65 7920 572e 2046 6f72 6361 6465  odney W. Forcade
-000032c0: 202a 5068 7973 2e20 5265 762e 2042 2a0a   *Phys. Rev. B*.
-000032d0: 2020 2020 2a2a 3830 2a2a 2c20 3031 3431      **80**, 0141
-000032e0: 3230 2028 3230 3039 292e 0a0a 2020 2020  20 (2009)...    
-000032f0: 2a2a 5061 7261 6d65 7465 7273 3a2a 2a0a  **Parameters:**.
-00003300: 0a20 2020 2060 606e 6060 3a20 696e 7465  .    ``n``: inte
-00003310: 6765 720a 2020 2020 2020 2020 696e 6465  ger.        inde
-00003320: 7820 6f66 2074 6865 2073 7570 6572 6365  x of the superce
-00003330: 6c6c 732c 2069 2e65 2e2c 2074 6865 206e  lls, i.e., the n
-00003340: 756d 6265 7220 6f66 2061 746f 6d73 2069  umber of atoms i
-00003350: 6e20 7468 6520 7375 7065 7263 656c 6c73  n the supercells
-00003360: 2069 730a 2020 2020 2020 2020 6060 6e2a   is.        ``n*
-00003370: 7061 7265 6e74 5f6c 6174 7469 6365 2e67  parent_lattice.g
-00003380: 6574 5f6e 6174 6f6d 7328 2960 602e 0a20  et_natoms()``.. 
-00003390: 2020 2060 6070 6172 656e 745f 6c61 7474     ``parent_latt
-000033a0: 6963 6560 603a 2050 6172 656e 744c 6174  ice``: ParentLat
-000033b0: 7469 6365 206f 626a 6563 740a 2020 2020  tice object.    
-000033c0: 2020 2020 5468 6520 7061 7265 6e74 206c      The parent l
-000033d0: 6174 7469 6365 0a0a 2020 2020 2a2a 5265  attice..    **Re
-000033e0: 7475 726e 733a 2a2a 2074 776f 2061 7272  turns:** two arr
-000033f0: 6179 7320 636f 6e74 6169 6e69 6e67 2033  ays containing 3
-00003400: 7833 206d 6174 7269 6365 732e 2054 6865  x3 matrices. The
-00003410: 206d 6174 7269 6365 7320 6060 5360 6020   matrices ``S`` 
-00003420: 6f66 2074 6865 0a20 2020 2066 6972 7374  of the.    first
-00003430: 2061 7272 6179 2063 6f6e 7461 696e 2074   array contain t
-00003440: 6865 2063 6172 7465 7369 616e 2063 6f6f  he cartesian coo
-00003450: 7264 696e 6174 6573 206f 6620 7468 6520  rdinates of the 
-00003460: 7375 7065 7263 656c 6c20 7665 6374 6f72  supercell vector
-00003470: 7320 2872 6f77 0a20 2020 2077 6973 6529  s (row.    wise)
-00003480: 2c20 7768 696c 6520 7468 6520 6d61 7472  , while the matr
-00003490: 6963 6573 2060 6048 6060 2069 6e20 7468  ices ``H`` in th
-000034a0: 6520 7365 636f 6e64 2061 7272 6179 2061  e second array a
-000034b0: 7265 2074 6865 2028 696e 7465 6765 7229  re the (integer)
-000034c0: 0a20 2020 2074 7261 6e73 6f72 6d61 7469  .    transormati
-000034d0: 6f6e 206d 6174 7269 6365 7320 7769 7468  on matrices with
-000034e0: 2072 6573 7065 6374 2074 6f20 7468 6520   respect to the 
-000034f0: 7061 7265 6e74 206c 6174 7469 6365 2060  parent lattice `
-00003500: 6055 6060 2e20 5468 6174 2069 732c 0a20  `U``. That is,. 
-00003510: 2020 203a 6d61 7468 3a60 533d 4855 600a     :math:`S=HU`.
-00003520: 0a20 2020 202a 2a45 7861 6d70 6c65 3a2a  .    **Example:*
-00003530: 2a0a 2020 2020 496e 2074 6865 2066 6f6c  *.    In the fol
-00003540: 6c6f 7769 6e67 2065 7861 6d70 6c65 2c20  lowing example, 
-00003550: 616c 6c20 7468 6520 7375 7065 7263 656c  all the supercel
-00003560: 6c73 206f 6620 696e 6465 7820 3420 666f  ls of index 4 fo
-00003570: 7220 7468 6520 4643 4320 6c61 7474 6963  r the FCC lattic
-00003580: 650a 2020 2020 6172 6520 666f 756e 642e  e.    are found.
-00003590: 2054 6865 2073 7570 6572 6365 6c6c 7320   The supercells 
-000035a0: 6172 6520 7374 6f72 6564 2069 6e20 7468  are stored in th
-000035b0: 6520 6669 6c65 0a20 2020 2060 6075 6e69  e file.    ``uni
-000035c0: 7175 655f 7375 7065 7263 656c 6c73 2d66  que_supercells-f
-000035d0: 6363 2e6a 736f 6e60 6020 666f 7220 7669  cc.json`` for vi
-000035e0: 7375 616c 697a 6174 696f 6e20 7769 7468  sualization with
-000035f0: 2074 6865 2063 6f6d 6d61 6e64 0a20 2020   the command.   
-00003600: 2060 6024 3e61 7365 2067 7569 2075 6e69   ``$>ase gui uni
-00003610: 7175 655f 7375 7065 7263 656c 6c73 2d66  que_supercells-f
-00003620: 6363 2e6a 736f 6e60 6020 3a3a 0a0a 2020  cc.json`` ::..  
-00003630: 2020 2020 2020 6672 6f6d 2063 6c75 7374        from clust
-00003640: 6572 7820 696d 706f 7274 2075 7469 6c73  erx import utils
-00003650: 0a20 2020 2020 2020 2066 726f 6d20 636c  .        from cl
-00003660: 7573 7465 7278 2e70 6172 656e 745f 6c61  usterx.parent_la
-00003670: 7474 6963 6520 696d 706f 7274 2050 6172  ttice import Par
-00003680: 656e 744c 6174 7469 6365 0a20 2020 2020  entLattice.     
-00003690: 2020 2066 726f 6d20 636c 7573 7465 7278     from clusterx
-000036a0: 2e73 7472 7563 7475 7265 735f 7365 7420  .structures_set 
-000036b0: 696d 706f 7274 2053 7472 7563 7475 7265  import Structure
-000036c0: 7353 6574 0a20 2020 2020 2020 2066 726f  sSet.        fro
-000036d0: 6d20 636c 7573 7465 7278 2e73 7570 6572  m clusterx.super
-000036e0: 5f63 656c 6c20 696d 706f 7274 2053 7570  _cell import Sup
-000036f0: 6572 4365 6c6c 0a20 2020 2020 2020 2066  erCell.        f
-00003700: 726f 6d20 636c 7573 7465 7278 2e73 7472  rom clusterx.str
-00003710: 7563 7475 7265 2069 6d70 6f72 7420 5374  ucture import St
-00003720: 7275 6374 7572 650a 2020 2020 2020 2020  ructure.        
-00003730: 6672 6f6d 2061 7365 2e64 6174 6120 696d  from ase.data im
-00003740: 706f 7274 2061 746f 6d69 635f 6e75 6d62  port atomic_numb
-00003750: 6572 7320 6173 2061 6e0a 2020 2020 2020  ers as an.      
-00003760: 2020 6672 6f6d 2061 7365 2069 6d70 6f72    from ase impor
-00003770: 7420 4174 6f6d 730a 2020 2020 2020 2020  t Atoms.        
-00003780: 696d 706f 7274 206e 756d 7079 2061 7320  import numpy as 
-00003790: 6e70 0a0a 2020 2020 2020 2020 613d 330a  np..        a=3.
-000037a0: 2020 2020 2020 2020 6365 6c6c 203d 206e          cell = n
-000037b0: 702e 6172 7261 7928 5b5b 302e 352c 302e  p.array([[0.5,0.
-000037c0: 352c 302e 305d 2c5b 302e 352c 302e 302c  5,0.0],[0.5,0.0,
-000037d0: 302e 355d 2c5b 302e 302c 302e 352c 302e  0.5],[0.0,0.5,0.
-000037e0: 355d 5d29 0a20 2020 2020 2020 2070 6f73  5]]).        pos
-000037f0: 6974 696f 6e73 203d 206e 702e 6172 7261  itions = np.arra
-00003800: 7928 5b5b 302c 302c 305d 5d29 0a20 2020  y([[0,0,0]]).   
-00003810: 2020 2020 2073 6974 6573 203d 205b 5b61       sites = [[a
-00003820: 6e5b 2243 7522 5d2c 616e 5b22 4175 225d  n["Cu"],an["Au"]
-00003830: 5d5d 0a20 2020 2020 2020 2070 7269 735f  ]].        pris_
-00003840: 6663 6320 3d20 4174 6f6d 7328 6365 6c6c  fcc = Atoms(cell
-00003850: 3d63 656c 6c2a 612c 706f 7369 7469 6f6e  =cell*a,position
-00003860: 733d 706f 7369 7469 6f6e 732a 6129 0a0a  s=positions*a)..
-00003870: 2020 2020 2020 2020 706c 203d 2050 6172          pl = Par
-00003880: 656e 744c 6174 7469 6365 2870 7269 735f  entLattice(pris_
-00003890: 6663 632c 7369 7465 733d 7369 7465 7329  fcc,sites=sites)
-000038a0: 0a0a 2020 2020 2020 2020 756e 6971 7565  ..        unique
-000038b0: 5f73 6373 2c20 756e 6971 7565 5f74 7261  _scs, unique_tra
-000038c0: 666f 7320 3d20 7574 696c 732e 6765 745f  fos = utils.get_
-000038d0: 756e 6971 7565 5f73 7570 6572 6365 6c6c  unique_supercell
-000038e0: 7328 342c 706c 290a 0a20 2020 2020 2020  s(4,pl)..       
-000038f0: 2073 7365 7420 3d20 5374 7275 6374 7572   sset = Structur
-00003900: 6573 5365 7428 706c 2c66 696c 656e 616d  esSet(pl,filenam
-00003910: 653d 2275 6e69 7175 655f 7375 7065 7263  e="unique_superc
-00003920: 656c 6c73 2d66 6363 2e6a 736f 6e22 290a  ells-fcc.json").
-00003930: 2020 2020 2020 2020 666f 7220 7420 696e          for t in
-00003940: 2075 6e69 7175 655f 7472 6166 6f73 3a0a   unique_trafos:.
-00003950: 2020 2020 2020 2020 2020 2020 7363 656c              scel
-00003960: 6c20 3d20 5375 7065 7243 656c 6c28 706c  l = SuperCell(pl
-00003970: 2c74 290a 2020 2020 2020 2020 2020 2020  ,t).            
-00003980: 7373 6574 2e61 6464 5f73 7472 7563 7475  sset.add_structu
-00003990: 7265 2853 7472 7563 7475 7265 2873 6365  re(Structure(sce
-000039a0: 6c6c 2c73 6365 6c6c 2e67 6574 5f61 746f  ll,scell.get_ato
-000039b0: 6d69 635f 6e75 6d62 6572 7328 2929 2c77  mic_numbers()),w
-000039c0: 7269 7465 5f74 6f5f 6462 203d 2054 7275  rite_to_db = Tru
-000039d0: 6529 0a0a 2020 2020 5468 6520 6765 6e65  e)..    The gene
-000039e0: 7261 7465 6420 7374 7275 6374 7572 6573  rated structures
-000039f0: 2061 7265 2074 6865 2073 616d 6520 6173   are the same as
-00003a00: 2074 686f 7365 2066 6f75 6e64 2069 6e20   those found in 
-00003a10: 4669 672e 2032 2061 6e64 2054 6162 6c65  Fig. 2 and Table
-00003a20: 2049 560a 2020 2020 6f66 2050 6879 732e   IV.    of Phys.
-00003a30: 2052 6576 2e20 4220 3737 2c20 3232 3431   Rev. B 77, 2241
-00003a40: 3135 2001 3230 3038 2e0a 0a20 2020 2054  15 .2008...    T
-00003a50: 6865 206e 6578 7420 6578 616d 706c 652c  he next example,
-00003a60: 2073 686f 7773 2061 2063 6173 6520 6f66   shows a case of
-00003a70: 2072 6564 7563 6564 2064 696d 656e 7369   reduced dimensi
-00003a80: 6f6e 616c 6974 792c 2074 6861 7420 6f66  onality, that of
-00003a90: 2061 2032 440a 2020 2020 7371 7561 7265   a 2D.    square
-00003aa0: 206c 6174 7469 6365 3a3a 0a0a 2020 2020   lattice::..    
-00003ab0: 2020 2020 613d 332e 310a 2020 2020 2020      a=3.1.      
-00003ac0: 2020 6365 6c6c 203d 206e 702e 6172 7261    cell = np.arra
-00003ad0: 7928 5b5b 312c 302c 305d 2c5b 302c 312c  y([[1,0,0],[0,1,
-00003ae0: 305d 2c5b 302c 302c 315d 5d29 0a20 2020  0],[0,0,1]]).   
-00003af0: 2020 2020 2070 6f73 6974 696f 6e73 203d       positions =
-00003b00: 206e 702e 6172 7261 7928 5b5b 302c 302c   np.array([[0,0,
-00003b10: 305d 5d29 0a20 2020 2020 2020 2073 6974  0]]).        sit
-00003b20: 6573 203d 205b 5b31 322c 3133 5d5d 0a20  es = [[12,13]]. 
-00003b30: 2020 2020 2020 2070 7269 7320 3d20 4174         pris = At
-00003b40: 6f6d 7328 6365 6c6c 3d63 656c 6c2a 612c  oms(cell=cell*a,
-00003b50: 2070 6f73 6974 696f 6e73 3d70 6f73 6974   positions=posit
-00003b60: 696f 6e73 2a61 290a 0a20 2020 2020 2020  ions*a)..       
-00003b70: 2070 6c20 3d20 5061 7265 6e74 4c61 7474   pl = ParentLatt
-00003b80: 6963 6528 7072 6973 2c20 7369 7465 733d  ice(pris, sites=
-00003b90: 7369 7465 732c 2070 6263 3d28 312c 312c  sites, pbc=(1,1,
-00003ba0: 3029 290a 0a20 2020 2020 2020 2075 6e69  0))..        uni
-00003bb0: 7175 655f 7363 732c 2075 6e69 7175 655f  que_scs, unique_
-00003bc0: 7472 6166 6f73 203d 2075 7469 6c73 2e67  trafos = utils.g
-00003bd0: 6574 5f75 6e69 7175 655f 7375 7065 7263  et_unique_superc
-00003be0: 656c 6c73 2834 2c70 6c29 0a0a 2020 2020  ells(4,pl)..    
-00003bf0: 2020 2020 7373 6574 203d 2053 7472 7563      sset = Struc
-00003c00: 7475 7265 7353 6574 2870 6c2c 6669 6c65  turesSet(pl,file
-00003c10: 6e61 6d65 3d22 7465 7374 5f67 6574 5f75  name="test_get_u
-00003c20: 6e69 7175 655f 7375 7065 7263 656c 6c73  nique_supercells
-00003c30: 2d73 7175 6172 655f 6c61 7474 6963 652e  -square_lattice.
-00003c40: 6a73 6f6e 2229 0a20 2020 2020 2020 2066  json").        f
-00003c50: 6f72 2074 2069 6e20 756e 6971 7565 5f74  or t in unique_t
-00003c60: 7261 666f 733a 0a20 2020 2020 2020 2020  rafos:.         
-00003c70: 2020 2073 6365 6c6c 203d 2053 7570 6572     scell = Super
-00003c80: 4365 6c6c 2870 6c2c 7429 0a20 2020 2020  Cell(pl,t).     
-00003c90: 2020 2020 2020 2073 7365 742e 6164 645f         sset.add_
-00003ca0: 7374 7275 6374 7572 6528 5374 7275 6374  structure(Struct
-00003cb0: 7572 6528 7363 656c 6c2c 7363 656c 6c2e  ure(scell,scell.
-00003cc0: 6765 745f 6174 6f6d 6963 5f6e 756d 6265  get_atomic_numbe
-00003cd0: 7273 2829 292c 7772 6974 655f 746f 5f64  rs()),write_to_d
-00003ce0: 6220 3d20 5472 7565 290a 0a20 2020 2020  b = True)..     
-00003cf0: 2020 2023 6973 6f6b 3020 3d20 6c65 6e28     #isok0 = len(
-00003d00: 756e 6971 7565 5f73 6373 2920 3d3d 2034  unique_scs) == 4
-00003d10: 2061 6e64 0a20 2020 2020 2020 2070 7269   and.        pri
-00003d20: 6e74 2822 6e3a 2022 2c6c 656e 2875 6e69  nt("n: ",len(uni
-00003d30: 7175 655f 7363 7329 290a 2020 2020 2020  que_scs)).      
-00003d40: 2020 7072 696e 7428 2253 4353 3a20 222c    print("SCS: ",
-00003d50: 2075 6e69 7175 655f 7363 7329 0a20 2020   unique_scs).   
-00003d60: 2020 2020 2070 7269 6e74 2822 5452 413a       print("TRA:
-00003d70: 2022 2c20 756e 6971 7565 5f74 7261 666f   ", unique_trafo
-00003d80: 7329 0a0a 2020 2020 5468 6520 7265 7375  s)..    The resu
-00003d90: 6c74 696e 6720 7375 7065 7263 656c 6c73  lting supercells
-00003da0: 2069 6e20 7468 6973 2065 7861 6d70 6c65   in this example
-00003db0: 2063 6f72 7265 7370 6f6e 6420 746f 2046   correspond to F
-00003dc0: 6967 2e20 3120 6f66 0a20 2020 2043 6f6d  ig. 1 of.    Com
-00003dd0: 7075 7461 7469 6f6e 616c 204d 6174 6572  putational Mater
-00003de0: 6961 6c73 2053 6369 656e 6365 2035 3920  ials Science 59 
-00003df0: 2832 3031 3229 2031 3031 e280 9331 3037  (2012) 101...107
-00003e00: 0a0a 2020 2020 2222 220a 2020 2020 6672  ..    """.    fr
-00003e10: 6f6d 2063 6c75 7374 6572 782e 7379 6d6d  om clusterx.symm
-00003e20: 6574 7279 2069 6d70 6f72 7420 6765 745f  etry import get_
-00003e30: 7370 6163 6567 726f 7570 0a20 2020 2070  spacegroup.    p
-00003e40: 6c5f 6365 6c6c 203d 2070 6172 656e 745f  l_cell = parent_
-00003e50: 6c61 7474 6963 652e 6765 745f 6365 6c6c  lattice.get_cell
-00003e60: 2829 0a0a 2020 2020 686e 6673 203d 2067  ()..    hnfs = g
-00003e70: 6574 5f61 6c6c 5f48 4e46 286e 2c70 6263  et_all_HNF(n,pbc
-00003e80: 3d70 6172 656e 745f 6c61 7474 6963 652e  =parent_lattice.
-00003e90: 6765 745f 7062 6328 2929 0a0a 2020 2020  get_pbc())..    
-00003ea0: 616c 6c5f 7363 7320 3d20 5b5d 0a20 2020  all_scs = [].   
-00003eb0: 2066 6f72 2068 6e66 2069 6e20 686e 6673   for hnf in hnfs
-00003ec0: 3a0a 2020 2020 2020 2020 616c 6c5f 7363  :.        all_sc
-00003ed0: 732e 6170 7065 6e64 286e 702e 646f 7428  s.append(np.dot(
-00003ee0: 686e 662c 706c 5f63 656c 6c29 290a 0a20  hnf,pl_cell)).. 
-00003ef0: 2020 206e 5f73 6373 203d 206c 656e 2861     n_scs = len(a
-00003f00: 6c6c 5f73 6373 290a 2020 2020 756e 6971  ll_scs).    uniq
-00003f10: 7565 5f73 6373 203d 205b 5d0a 2020 2020  ue_scs = [].    
-00003f20: 756e 6971 7565 5f74 7261 666f 7320 3d20  unique_trafos = 
-00003f30: 5b5d 0a20 2020 2073 635f 7367 2c20 7363  [].    sc_sg, sc
-00003f40: 5f73 796d 203d 2067 6574 5f73 7061 6365  _sym = get_space
-00003f50: 6772 6f75 7028 7061 7265 6e74 5f6c 6174  group(parent_lat
-00003f60: 7469 6365 2920 2320 5363 616c 6564 2074  tice) # Scaled t
-00003f70: 6f20 7061 7265 6e74 5f6c 6174 7469 6365  o parent_lattice
-00003f80: 0a20 2020 206e 6578 7473 203d 206e 702e  .    nexts = np.
-00003f90: 6173 6172 7261 7928 6e70 2e61 7261 6e67  asarray(np.arang
-00003fa0: 6528 6e5f 7363 7329 290a 2020 2020 756e  e(n_scs)).    un
-00003fb0: 6971 7565 5f73 6373 2e61 7070 656e 6428  ique_scs.append(
-00003fc0: 616c 6c5f 7363 735b 305d 290a 2020 2020  all_scs[0]).    
-00003fd0: 756e 6971 7565 5f74 7261 666f 732e 6170  unique_trafos.ap
-00003fe0: 7065 6e64 2868 6e66 735b 305d 290a 0a20  pend(hnfs[0]).. 
-00003ff0: 2020 2077 6869 6c65 206c 656e 286e 6578     while len(nex
-00004000: 7473 2920 3e20 313a 0a20 2020 2020 2020  ts) > 1:.       
-00004010: 2069 203d 206e 6578 7473 5b30 5d0a 2020   i = nexts[0].  
-00004020: 2020 2020 2020 7468 655f 6c69 7374 203d        the_list =
-00004030: 206e 6578 7473 5b31 3a5d 0a20 2020 2020   nexts[1:].     
-00004040: 2020 206e 6578 7473 3d5b 5d0a 2020 2020     nexts=[].    
-00004050: 2020 2020 6269 203d 2061 6c6c 5f73 6373      bi = all_scs
-00004060: 5b69 5d0a 2020 2020 2020 2020 666f 7220  [i].        for 
-00004070: 6a20 696e 2074 6865 5f6c 6973 743a 0a20  j in the_list:. 
-00004080: 2020 2020 2020 2020 2020 2062 6a20 3d20             bj = 
-00004090: 616c 6c5f 7363 735b 6a5d 0a20 2020 2020  all_scs[j].     
-000040a0: 2020 2020 2020 206a 5f69 735f 6e65 7874         j_is_next
-000040b0: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
-000040c0: 2020 2020 666f 7220 7220 696e 2073 635f      for r in sc_
-000040d0: 7379 6d5b 2772 6f74 6174 696f 6e73 275d  sym['rotations']
-000040e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000040f0: 2020 7272 203d 206e 702e 646f 7428 706c    rr = np.dot(pl
-00004100: 5f63 656c 6c2c 6e70 2e64 6f74 2872 2c6e  _cell,np.dot(r,n
-00004110: 702e 6c69 6e61 6c67 2e69 6e76 2870 6c5f  p.linalg.inv(pl_
-00004120: 6365 6c6c 2929 2920 2320 526f 7461 7469  cell))) # Rotati
-00004130: 6f6e 7320 6172 6520 696e 206c 6174 7469  ons are in latti
-00004140: 6365 2063 6f6f 7264 696e 6174 6573 2c20  ce coordinates, 
-00004150: 736f 2077 6520 6861 7665 2074 6f20 7472  so we have to tr
-00004160: 616e 736f 726d 2074 6865 6d20 746f 2063  ansorm them to c
-00004170: 6172 7465 7369 616e 2e0a 2020 2020 2020  artesian..      
-00004180: 2020 2020 2020 2020 2020 6d20 3d20 6e70            m = np
-00004190: 2e61 726f 756e 6428 6e70 2e64 6f74 286e  .around(np.dot(n
-000041a0: 702e 6c69 6e61 6c67 2e69 6e76 2862 692e  p.linalg.inv(bi.
-000041b0: 5429 2c6e 702e 646f 7428 7272 2c62 6a2e  T),np.dot(rr,bj.
-000041c0: 5429 292c 3529 0a20 2020 2020 2020 2020  T)),5).         
-000041d0: 2020 2020 2020 2069 6620 5f69 735f 696e         if _is_in
-000041e0: 7465 6765 725f 6d61 7472 6978 286d 293a  teger_matrix(m):
-000041f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004200: 2020 2020 206a 5f69 735f 6e65 7874 203d       j_is_next =
-00004210: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
-00004220: 2020 2020 2020 2020 2020 2062 7265 616b             break
-00004230: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00004240: 206a 5f69 735f 6e65 7874 3a0a 2020 2020   j_is_next:.    
-00004250: 2020 2020 2020 2020 2020 2020 6e65 7874              next
-00004260: 732e 6170 7065 6e64 286a 290a 0a20 2020  s.append(j)..   
-00004270: 2020 2020 2069 6620 6c65 6e28 6e65 7874       if len(next
-00004280: 7329 203e 2030 3a0a 2020 2020 2020 2020  s) > 0:.        
-00004290: 2020 2020 756e 6971 7565 5f73 6373 2e61      unique_scs.a
-000042a0: 7070 656e 6428 616c 6c5f 7363 735b 6e65  ppend(all_scs[ne
-000042b0: 7874 735b 305d 5d29 0a20 2020 2020 2020  xts[0]]).       
-000042c0: 2020 2020 2075 6e69 7175 655f 7472 6166       unique_traf
-000042d0: 6f73 2e61 7070 656e 6428 686e 6673 5b6e  os.append(hnfs[n
-000042e0: 6578 7473 5b30 5d5d 290a 0a20 2020 2072  exts[0]])..    r
-000042f0: 6574 7572 6e20 756e 6971 7565 5f73 6373  eturn unique_scs
-00004300: 2c20 756e 6971 7565 5f74 7261 666f 730a  , unique_trafos.
-00004310: 0a64 6566 205f 6973 5f69 6e74 6567 6572  .def _is_integer
-00004320: 5f6d 6174 7269 7828 6d2c 726e 643d 3529  _matrix(m,rnd=5)
-00004330: 3a0a 2020 2020 6d69 203d 206e 702e 6172  :.    mi = np.ar
-00004340: 6f75 6e64 286d 2c72 6e64 290a 2020 2020  ound(m,rnd).    
-00004350: 666f 7220 6b20 696e 2072 616e 6765 2833  for k in range(3
-00004360: 293a 0a20 2020 2020 2020 2066 6f72 206c  ):.        for l
-00004370: 2069 6e20 7261 6e67 6528 3329 3a0a 2020   in range(3):.  
-00004380: 2020 2020 2020 2020 2020 2369 6620 6e6f            #if no
-00004390: 7420 726f 756e 6428 6d5b 6b2c 6c5d 2c72  t round(m[k,l],r
-000043a0: 6e64 292e 6973 5f69 6e74 6567 6572 2829  nd).is_integer()
-000043b0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-000043c0: 206e 6f74 206d 695b 6b2c 6c5d 2e69 735f   not mi[k,l].is_
-000043d0: 696e 7465 6765 7228 293a 0a20 2020 2020  integer():.     
-000043e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000043f0: 6e20 4661 6c73 650a 2020 2020 7265 7475  n False.    retu
-00004400: 726e 2054 7275 650a 0a64 6566 2067 6574  rn True..def get
-00004410: 5f61 6c6c 5f48 4e46 286e 2c70 6263 3d28  _all_HNF(n,pbc=(
-00004420: 312c 312c 3129 293a 0a20 2020 2022 2222  1,1,1)):.    """
-00004430: 5265 7475 726e 2063 6f6d 706c 6574 6520  Return complete 
-00004440: 7365 7420 6f66 2048 6572 6d69 7465 206e  set of Hermite n
-00004450: 6f72 6d61 6c20 666f 726d 2028 484e 4629  ormal form (HNF)
-00004460: 203a 6d61 7468 3a60 3378 3360 206d 6174   :math:`3x3` mat
-00004470: 7269 6365 730a 2020 2020 6f66 2069 6e64  rices.    of ind
-00004480: 6578 2060 606e 6060 2e0a 0a20 2020 2054  ex ``n``...    T
-00004490: 6865 2061 6c67 6f72 6974 686d 2068 6572  he algorithm her
-000044a0: 6520 6973 2062 6173 6564 206f 6e20 4571  e is based on Eq
-000044b0: 7561 7469 6f6e 2031 206f 6620 4775 7320  uation 1 of Gus 
-000044c0: 4c2e 2057 2e20 4861 7274 2061 6e64 2052  L. W. Hart and R
-000044d0: 6f64 6e65 7920 572e 0a20 2020 2046 6f72  odney W..    For
-000044e0: 6361 6465 2c20 2a50 6879 732e 2052 6576  cade, *Phys. Rev
-000044f0: 2e20 422a 202a 2a37 372a 2a2c 2032 3234  . B* **77**, 224
-00004500: 3131 3520 2832 3030 3829 2e0a 0a20 2020  115 (2008)...   
-00004510: 202a 2a50 6172 616d 6574 6572 733a 2a2a   **Parameters:**
-00004520: 0a0a 2020 2020 6060 6e60 603a 2069 6e74  ..    ``n``: int
-00004530: 6567 6572 0a20 2020 2020 2020 2069 6e64  eger.        ind
-00004540: 6578 206f 6620 7468 6520 484e 4620 6d61  ex of the HNF ma
-00004550: 7472 6963 6573 2e0a 2020 2020 6060 7062  trices..    ``pb
-00004560: 6360 603a 2074 6872 6565 2062 6f6f 6c0a  c``: three bool.
-00004570: 2020 2020 2020 2020 5065 7269 6f64 6963          Periodic
-00004580: 2062 6f75 6e64 6172 7920 636f 6e64 6974   boundary condit
-00004590: 696f 6e73 2066 6c61 6773 2e20 4578 616d  ions flags. Exam
-000045a0: 706c 6573 3a0a 2020 2020 2020 2020 2831  ples:.        (1
-000045b0: 2c20 312c 2030 292c 2028 5472 7565 2c20  , 1, 0), (True, 
-000045c0: 4661 6c73 652c 2046 616c 7365 292e 2044  False, False). D
-000045d0: 6566 6175 6c74 2076 616c 7565 3a20 2831  efault value: (1
-000045e0: 2c31 2c31 290a 2020 2020 2222 220a 0a20  ,1,1).    """.. 
-000045f0: 2020 205f 686e 6673 203d 205b 5d0a 2020     _hnfs = [].  
-00004600: 2020 666f 7220 6120 696e 205f 6469 7669    for a in _divi
-00004610: 736f 7273 286e 293a 0a20 2020 2020 2020  sors(n):.       
-00004620: 2066 6f72 2063 2069 6e20 5f64 6976 6973   for c in _divis
-00004630: 6f72 7328 696e 7428 6e2f 6129 293a 0a20  ors(int(n/a)):. 
-00004640: 2020 2020 2020 2020 2020 2066 203d 2069             f = i
-00004650: 6e74 286e 2f28 612a 6329 290a 2020 2020  nt(n/(a*c)).    
-00004660: 2020 2020 2020 2020 666f 7220 6220 696e          for b in
-00004670: 2072 616e 6765 2863 293a 0a20 2020 2020   range(c):.     
-00004680: 2020 2020 2020 2020 2020 2066 6f72 2064             for d
-00004690: 2069 6e20 7261 6e67 6528 6629 3a0a 2020   in range(f):.  
-000046a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046b0: 2020 666f 7220 6520 696e 2072 616e 6765    for e in range
-000046c0: 2866 293a 0a20 2020 2020 2020 2020 2020  (f):.           
-000046d0: 2020 2020 2020 2020 2020 2020 2068 6e66               hnf
-000046e0: 203d 205b 5d0a 2020 2020 2020 2020 2020   = [].          
-000046f0: 2020 2020 2020 2020 2020 2020 2020 686e                hn
-00004700: 662e 6170 7065 6e64 285b 612c 302c 305d  f.append([a,0,0]
-00004710: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00004720: 2020 2020 2020 2020 2020 686e 662e 6170            hnf.ap
-00004730: 7065 6e64 285b 622c 632c 305d 290a 2020  pend([b,c,0]).  
-00004740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004750: 2020 2020 2020 686e 662e 6170 7065 6e64        hnf.append
-00004760: 285b 642c 652c 665d 290a 2020 2020 2020  ([d,e,f]).      
-00004770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004780: 2020 5f68 6e66 732e 6170 7065 6e64 286e    _hnfs.append(n
-00004790: 702e 6172 7261 7928 686e 6629 2e54 290a  p.array(hnf).T).
-000047a0: 0a20 2020 2068 6e66 7320 3d20 5b5d 0a20  .    hnfs = []. 
-000047b0: 2020 2066 6f72 2068 6e66 2069 6e20 5f68     for hnf in _h
-000047c0: 6e66 733a 0a20 2020 2020 2020 2069 6e63  nfs:.        inc
-000047d0: 6c75 6465 203d 2054 7275 650a 2020 2020  lude = True.    
-000047e0: 2020 2020 666f 7220 692c 2062 6320 696e      for i, bc in
-000047f0: 2065 6e75 6d65 7261 7465 2870 6263 293a   enumerate(pbc):
-00004800: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00004810: 6e6f 7420 6263 2061 6e64 2028 686e 665b  not bc and (hnf[
-00004820: 695d 2021 3d20 6e70 2e69 6465 6e74 6974  i] != np.identit
-00004830: 7928 332c 6474 7970 653d 2269 6e74 2229  y(3,dtype="int")
-00004840: 5b69 5d29 2e61 6e79 2829 3a0a 2020 2020  [i]).any():.    
-00004850: 2020 2020 2020 2020 2020 2020 696e 636c              incl
-00004860: 7564 6520 3d20 4661 6c73 650a 2020 2020  ude = False.    
-00004870: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-00004880: 6b0a 2020 2020 2020 2020 6966 2069 6e63  k.        if inc
-00004890: 6c75 6465 3a0a 2020 2020 2020 2020 2020  lude:.          
-000048a0: 2020 686e 6673 2e61 7070 656e 6428 686e    hnfs.append(hn
-000048b0: 6629 0a0a 2020 2020 7265 7475 726e 2868  f)..    return(h
-000048c0: 6e66 7329 0a0a 6465 6620 5f64 6976 6973  nfs)..def _divis
-000048d0: 6f72 7328 6e29 3a0a 2020 2020 2320 6765  ors(n):.    # ge
-000048e0: 7420 6661 6374 6f72 7320 616e 6420 7468  t factors and th
-000048f0: 6569 7220 636f 756e 7473 0a20 2020 2023  eir counts.    #
-00004900: 204d 6169 6e6c 7920 7461 6b65 6e20 6672   Mainly taken fr
-00004910: 6f6d 2068 7474 7073 3a2f 2f73 7461 636b  om https://stack
-00004920: 6f76 6572 666c 6f77 2e63 6f6d 2f61 2f33  overflow.com/a/3
-00004930: 3730 3538 3734 350a 2020 2020 6661 6374  7058745.    fact
-00004940: 6f72 7320 3d20 7b7d 0a20 2020 206e 6e20  ors = {}.    nn 
-00004950: 3d20 6e0a 2020 2020 6920 3d20 320a 2020  = n.    i = 2.  
-00004960: 2020 7768 696c 6520 692a 6920 3c3d 206e    while i*i <= n
-00004970: 6e3a 0a20 2020 2020 2020 2077 6869 6c65  n:.        while
-00004980: 206e 6e20 2520 6920 3d3d 2030 3a0a 2020   nn % i == 0:.  
-00004990: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-000049a0: 2069 2069 6e20 6661 6374 6f72 733a 0a20   i in factors:. 
-000049b0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000049c0: 6163 746f 7273 5b69 5d20 3d20 300a 2020  actors[i] = 0.  
-000049d0: 2020 2020 2020 2020 2020 6661 6374 6f72            factor
-000049e0: 735b 695d 202b 3d20 310a 2020 2020 2020  s[i] += 1.      
-000049f0: 2020 2020 2020 6e6e 202f 2f3d 2069 0a20        nn //= i. 
-00004a00: 2020 2020 2020 2069 202b 3d20 310a 2020         i += 1.  
-00004a10: 2020 6966 206e 6e20 3e20 313a 0a20 2020    if nn > 1:.   
-00004a20: 2020 2020 2066 6163 746f 7273 5b6e 6e5d       factors[nn]
-00004a30: 203d 2031 0a0a 2020 2020 7072 696d 6573   = 1..    primes
-00004a40: 203d 206c 6973 7428 6661 6374 6f72 732e   = list(factors.
-00004a50: 6b65 7973 2829 290a 0a20 2020 2023 2067  keys())..    # g
-00004a60: 656e 6572 6174 6573 2066 6163 746f 7273  enerates factors
-00004a70: 2066 726f 6d20 7072 696d 6573 5b6b 3a5d   from primes[k:]
-00004a80: 2073 7562 7365 740a 2020 2020 6465 6620   subset.    def 
-00004a90: 6765 6e65 7261 7465 286b 293a 0a20 2020  generate(k):.   
-00004aa0: 2020 2020 2069 6620 6b20 3d3d 206c 656e       if k == len
-00004ab0: 2870 7269 6d65 7329 3a0a 2020 2020 2020  (primes):.      
-00004ac0: 2020 2020 2020 7969 656c 6420 310a 2020        yield 1.  
-00004ad0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00004ae0: 2020 2020 2020 2020 7265 7374 203d 2067          rest = g
-00004af0: 656e 6572 6174 6528 6b2b 3129 0a20 2020  enerate(k+1).   
-00004b00: 2020 2020 2020 2020 2070 7269 6d65 203d           prime =
-00004b10: 2070 7269 6d65 735b 6b5d 0a20 2020 2020   primes[k].     
-00004b20: 2020 2020 2020 2066 6f72 2066 6163 746f         for facto
-00004b30: 7220 696e 2072 6573 743a 0a20 2020 2020  r in rest:.     
-00004b40: 2020 2020 2020 2020 2020 2070 7269 6d65             prime
-00004b50: 5f74 6f5f 6920 3d20 310a 2020 2020 2020  _to_i = 1.      
-00004b60: 2020 2020 2020 2020 2020 2320 7072 696d            # prim
-00004b70: 655f 746f 5f69 2069 7465 7261 7465 7320  e_to_i iterates 
-00004b80: 7072 696d 652a 2a69 2076 616c 7565 732c  prime**i values,
-00004b90: 2069 2062 6569 6e67 2061 6c6c 2070 6f73   i being all pos
-00004ba0: 7369 626c 6520 6578 706f 6e65 6e74 730a  sible exponents.
-00004bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004bc0: 666f 7220 5f20 696e 2072 616e 6765 2866  for _ in range(f
-00004bd0: 6163 746f 7273 5b70 7269 6d65 5d20 2b20  actors[prime] + 
-00004be0: 3129 3a0a 2020 2020 2020 2020 2020 2020  1):.            
-00004bf0: 2020 2020 2020 2020 7969 656c 6420 6661          yield fa
-00004c00: 6374 6f72 202a 2070 7269 6d65 5f74 6f5f  ctor * prime_to_
-00004c10: 690a 2020 2020 2020 2020 2020 2020 2020  i.              
-00004c20: 2020 2020 2020 7072 696d 655f 746f 5f69        prime_to_i
-00004c30: 202a 3d20 7072 696d 650a 0a20 2020 2023   *= prime..    #
-00004c40: 2069 6e20 7079 7468 6f6e 332c 2060 7969   in python3, `yi
-00004c50: 656c 6420 6672 6f6d 2067 656e 6572 6174  eld from generat
-00004c60: 6528 3029 6020 776f 756c 6420 616c 736f  e(0)` would also
-00004c70: 2077 6f72 6b0a 2020 2020 2366 6f72 2066   work.    #for f
-00004c80: 6163 746f 7220 696e 2067 656e 6572 6174  actor in generat
-00004c90: 6528 3029 3a0a 2020 2020 2320 2020 2079  e(0):.    #    y
-00004ca0: 6965 6c64 2066 6163 746f 720a 0a20 2020  ield factor..   
-00004cb0: 2072 203d 205b 5d0a 2020 2020 666f 7220   r = [].    for 
-00004cc0: 6661 6374 6f72 2069 6e20 6765 6e65 7261  factor in genera
-00004cd0: 7465 2830 293a 0a20 2020 2020 2020 2072  te(0):.        r
-00004ce0: 2e61 7070 656e 6428 6661 6374 6f72 290a  .append(factor).
-00004cf0: 0a20 2020 2072 6574 7572 6e20 736f 7274  .    return sort
-00004d00: 6564 2872 290a 0a64 6566 2067 6574 5f63  ed(r)..def get_c
-00004d10: 6c5f 6964 785f 7363 2863 6c2c 2073 632c  l_idx_sc(cl, sc,
-00004d20: 206d 6574 686f 643d 302c 2074 6f6c 3d31   method=0, tol=1
-00004d30: 652d 3329 3a0a 2020 2020 2222 2252 6574  e-3):.    """Ret
-00004d40: 7572 6e20 6174 6f6d 2069 6e64 6578 6573  urn atom indexes
-00004d50: 206f 6620 636c 7573 7465 7220 706f 696e   of cluster poin
-00004d60: 7473 2069 6e20 5375 7065 7243 656c 6c0a  ts in SuperCell.
-00004d70: 0a20 2020 202a 2a50 6172 616d 6574 6572  .    **Parameter
-00004d80: 733a 2a2a 0a0a 2020 2020 6060 636c 6060  s:**..    ``cl``
-00004d90: 3a20 6e70 6f69 6e74 7320 7820 3320 6d61  : npoints x 3 ma
-00004da0: 7472 6978 0a20 2020 2020 2020 206d 6174  trix.        mat
-00004db0: 7269 7820 6f66 2063 6172 7465 7369 616e  rix of cartesian
-00004dc0: 206f 7220 7363 616c 6564 2063 6f6f 7264   or scaled coord
-00004dd0: 696e 6174 6573 206f 6620 636c 7573 7465  inates of cluste
-00004de0: 7220 706f 696e 7473 2e20 436c 7573 7465  r points. Cluste
-00004df0: 720a 2020 2020 2020 2020 706f 7369 7469  r.        positi
-00004e00: 6f6e 7320 6172 6520 6578 7065 6374 6564  ons are expected
-00004e10: 2074 6f20 6265 2077 7261 7070 6564 2069   to be wrapped i
-00004e20: 6e73 6964 6520 7375 7065 7263 656c 6c20  nside supercell 
-00004e30: 6060 7363 6060 0a20 2020 2060 6073 6360  ``sc``.    ``sc`
-00004e40: 603a 206e 6174 6f6d 7320 7820 3320 6d61  `: natoms x 3 ma
-00004e50: 7472 6978 0a20 2020 2020 2020 206d 6174  trix.        mat
-00004e60: 7269 7820 6f66 2063 6172 7465 7369 616e  rix of cartesian
-00004e70: 206f 7220 7363 616c 6564 2063 6f6f 7264   or scaled coord
-00004e80: 696e 6174 6573 206f 6620 7375 7065 7263  inates of superc
-00004e90: 656c 6c20 6174 6f6d 6963 2070 6f73 6974  ell atomic posit
-00004ea0: 696f 6e73 2e0a 2020 2020 2020 2020 5468  ions..        Th
-00004eb0: 6520 7479 7065 206f 6620 636f 6f72 6469  e type of coordi
-00004ec0: 6e61 7465 7320 2865 6974 6865 7220 6361  nates (either ca
-00004ed0: 7274 6573 696f 6e20 6f72 2073 6361 6c65  rtesion or scale
-00004ee0: 6429 206d 7573 7420 636f 696e 6369 6465  d) must coincide
-00004ef0: 2077 6974 680a 2020 2020 2020 2020 7468   with.        th
-00004f00: 6174 206f 6620 6060 636c 6060 0a20 2020  at of ``cl``.   
-00004f10: 2060 606d 6574 686f 6460 603a 2069 6e74   ``method``: int
-00004f20: 6567 6572 0a20 2020 2020 2020 204d 6574  eger.        Met
-00004f30: 686f 6420 746f 2075 7365 2e20 303a 2028  hod to use. 0: (
-00004f40: 736c 6f77 2920 6e65 7374 6564 2066 6f72  slow) nested for
-00004f50: 206c 6f6f 7020 7573 696e 6720 6e75 6d70   loop using nump
-00004f60: 7920 616c 6c63 6c6f 7365 2e20 313a 2028  y allclose. 1: (
-00004f70: 6661 7374 290a 2020 2020 2020 2020 6361  fast).        ca
-00004f80: 6c63 756c 6174 6573 2061 6c6c 2064 6973  lculates all dis
-00004f90: 7461 6e63 6573 2066 726f 6d20 706f 696e  tances from poin
-00004fa0: 7473 2069 6e20 6060 636c 6060 2074 6f20  ts in ``cl`` to 
-00004fb0: 6174 6f6d 7320 696e 2060 6073 6360 602c  atoms in ``sc``,
-00004fc0: 2061 6e64 0a20 2020 2020 2020 2072 6574   and.        ret
-00004fd0: 7572 6e20 696e 6469 6365 7320 666f 7220  urn indices for 
-00004fe0: 7768 6963 6820 6469 7374 616e 6365 7320  which distances 
-00004ff0: 6172 6520 7a65 726f 2e0a 2020 2020 6060  are zero..    ``
-00005000: 746f 6c60 603a 2072 6561 6c20 706f 7369  tol``: real posi
-00005010: 7469 7665 206e 756d 6265 720a 2020 2020  tive number.    
-00005020: 2020 2020 746f 6c65 7261 6e63 6520 746f      tolerance to
-00005030: 2064 6574 6572 6d69 6e65 2077 6865 7468   determine wheth
-00005040: 6572 2063 6c75 7374 6572 2061 6e64 2061  er cluster and a
-00005050: 746f 6d20 706f 7369 7469 6f6e 7320 6172  tom positions ar
-00005060: 6520 7468 6520 7361 6d65 2e0a 2020 2020  e the same..    
-00005070: 2222 220a 2020 2020 6672 6f6d 2073 6369  """.    from sci
-00005080: 7079 2e73 7061 7469 616c 2e64 6973 7461  py.spatial.dista
-00005090: 6e63 6520 696d 706f 7274 2063 6469 7374  nce import cdist
-000050a0: 0a0a 2020 2020 6966 206d 6574 686f 6420  ..    if method 
-000050b0: 3d3d 2030 3a0a 2020 2020 2020 2020 6964  == 0:.        id
-000050c0: 7873 203d 206e 702e 7a65 726f 7328 6c65  xs = np.zeros(le
-000050d0: 6e28 636c 292c 6474 7970 653d 2269 6e74  n(cl),dtype="int
-000050e0: 2229 0a20 2020 2020 2020 2066 6f72 2069  ").        for i
-000050f0: 636c 2c63 6c70 2069 6e20 656e 756d 6572  cl,clp in enumer
-00005100: 6174 6528 636c 293a 0a20 2020 2020 2020  ate(cl):.       
-00005110: 2020 2020 2066 6f72 2069 7363 2c20 7363       for isc, sc
-00005120: 7020 696e 2065 6e75 6d65 7261 7465 2873  p in enumerate(s
-00005130: 6329 3a0a 2020 2020 2020 2020 2020 2020  c):.            
-00005140: 2020 2020 6966 206e 702e 616c 6c63 6c6f      if np.allclo
-00005150: 7365 2863 6c70 2c73 6370 2c61 746f 6c3d  se(clp,scp,atol=
-00005160: 746f 6c29 3a0a 2020 2020 2020 2020 2020  tol):.          
-00005170: 2020 2020 2020 2020 2020 6964 7873 5b69            idxs[i
-00005180: 636c 5d20 3d20 6973 630a 2020 2020 2020  cl] = isc.      
-00005190: 2020 2020 2020 2020 2020 2020 2020 6272                br
-000051a0: 6561 6b0a 0a20 2020 2069 6620 6d65 7468  eak..    if meth
-000051b0: 6f64 203d 3d20 313a 0a20 2020 2020 2020  od == 1:.       
-000051c0: 2073 6469 7374 616e 6365 7320 3d20 6364   sdistances = cd
-000051d0: 6973 7428 636c 2c20 7363 2c20 6d65 7472  ist(cl, sc, metr
-000051e0: 6963 3d27 6575 636c 6964 6561 6e27 2920  ic='euclidean') 
-000051f0: 2320 4576 616c 7561 7465 2061 6c6c 2028  # Evaluate all (
-00005200: 7363 616c 6564 2920 6469 7374 616e 6365  scaled) distance
-00005210: 7320 6265 7477 6565 6e20 636c 7573 7465  s between cluste
-00005220: 7220 706f 696e 7473 2074 6f20 7363 656c  r points to scel
-00005230: 6c20 7369 7465 730a 2020 2020 2020 2020  l sites.        
-00005240: 6964 7873 203d 206e 702e 6172 6777 6865  idxs = np.argwhe
-00005250: 7265 286e 702e 6162 7328 7364 6973 7461  re(np.abs(sdista
-00005260: 6e63 6573 2920 3c20 746f 6c29 5b3a 2c31  nces) < tol)[:,1
-00005270: 5d20 2320 4174 6f6d 2069 6e64 6578 6573  ] # Atom indexes
-00005280: 206f 6620 7468 6520 7472 616e 7366 6f72   of the transfor
-00005290: 6d65 6420 636c 7573 7465 720a 0a20 2020  med cluster..   
-000052a0: 2072 6574 7572 6e20 6964 7873 0a0a 6465   return idxs..de
-000052b0: 6620 6164 645f 6e6f 6973 6528 762c 6e6f  f add_noise(v,no
-000052c0: 6973 655f 6c65 7665 6c29 3a0a 2020 2020  ise_level):.    
-000052d0: 2222 2241 6464 2072 616e 646f 6d6c 7920  """Add randomly 
-000052e0: 6469 7374 7269 6275 7465 6420 6e6f 6973  distributed nois
-000052f0: 6520 746f 2076 6563 746f 7220 636f 6f72  e to vector coor
-00005300: 6469 6e61 7465 730a 0a20 2020 2054 6f20  dinates..    To 
-00005310: 6561 6368 2063 6f6f 7264 696e 6174 6520  each coordinate 
-00005320: 6f66 2074 6865 2069 6e70 7574 2076 6563  of the input vec
-00005330: 746f 7220 6060 7660 602c 2072 616e 646f  tor ``v``, rando
-00005340: 6d20 6e6f 6973 6520 756e 6966 6f72 6d6c  m noise uniforml
-00005350: 790a 2020 2020 6469 7374 7269 6275 7465  y.    distribute
-00005360: 6420 6265 7477 6565 6e20 2d60 606e 6f69  d between -``noi
-00005370: 7365 5f6c 6576 656c 6060 2061 6e64 2060  se_level`` and `
-00005380: 606e 6f69 7365 5f6c 6576 656c 6060 2069  `noise_level`` i
-00005390: 7320 6164 6465 642e 2054 6865 2069 6e70  s added. The inp
-000053a0: 7574 0a20 2020 2076 6563 746f 7220 6060  ut.    vector ``
-000053b0: 7660 6020 6973 206c 6566 7420 756e 6368  v`` is left unch
-000053c0: 616e 6765 642e 2054 6865 206d 6f64 6966  anged. The modif
-000053d0: 6965 6420 7665 6374 6f72 2069 7320 7265  ied vector is re
-000053e0: 7475 726e 6564 2e0a 0a20 2020 202a 2a50  turned...    **P
-000053f0: 6172 616d 6574 6572 733a 2a2a 0a0a 2020  arameters:**..  
-00005400: 2020 6060 7660 603a 206c 6973 7420 6f66    ``v``: list of
-00005410: 2066 6c6f 6174 730a 2020 2020 2020 2020   floats.        
-00005420: 5468 6520 696e 7075 7420 7665 6374 6f72  The input vector
-00005430: 0a0a 2020 2020 6060 6e6f 6973 655f 6c65  ..    ``noise_le
-00005440: 7665 6c60 603a 2066 6c6f 6174 0a20 2020  vel``: float.   
-00005450: 2020 2020 2057 6964 7468 206f 6620 7468       Width of th
-00005460: 6520 756e 6966 6f72 6d20 6469 7374 7269  e uniform distri
-00005470: 6275 7469 6f6e 2075 7365 6420 746f 2061  bution used to a
-00005480: 6464 206e 6f69 7365 2e0a 2020 2020 2222  dd noise..    ""
-00005490: 220a 2020 2020 696d 706f 7274 2072 616e  ".    import ran
-000054a0: 646f 6d0a 2020 2020 656e 6572 6769 6573  dom.    energies
-000054b0: 203d 205b 5d0a 2020 2020 666f 7220 6520   = [].    for e 
-000054c0: 696e 2076 3a0a 2020 2020 2020 2020 656e  in v:.        en
-000054d0: 6572 6769 6573 2e61 7070 656e 6428 652b  ergies.append(e+
-000054e0: 7261 6e64 6f6d 2e75 6e69 666f 726d 282d  random.uniform(-
-000054f0: 312c 3129 2a6e 6f69 7365 5f6c 6576 656c  1,1)*noise_level
-00005500: 290a 2020 2020 7265 7475 726e 2065 6e65  ).    return ene
-00005510: 7267 6965 730a 0a64 6566 2063 616c 6375  rgies..def calcu
-00005520: 6c61 7465 5f74 7261 666f 5f6d 6174 7269  late_trafo_matri
-00005530: 7828 7063 656c 6c2c 7363 656c 6c2c 726e  x(pcell,scell,rn
-00005540: 643d 3529 3a0a 2020 2020 2222 2243 616c  d=5):.    """Cal
-00005550: 6375 6c61 7465 2069 6e74 6567 6572 2074  culate integer t
-00005560: 7261 6e73 666f 726d 6174 696f 6e20 6d61  ransformation ma
-00005570: 7472 6978 2067 6976 656e 2061 2070 7269  trix given a pri
-00005580: 6d69 7469 7665 2063 656c 6c20 616e 6420  mitive cell and 
-00005590: 6120 7375 7065 722d 6365 6c6c 0a0a 2020  a super-cell..  
-000055a0: 2020 4966 203a 6d61 7468 3a60 5360 2061    If :math:`S` a
-000055b0: 6e64 203a 6d61 7468 3a60 5660 2061 7265  nd :math:`V` are
-000055c0: 2c20 7265 7370 6563 7469 7665 6c79 2c20  , respectively, 
-000055d0: 6120 6d61 7472 6978 2077 686f 7365 2072  a matrix whose r
-000055e0: 6f77 7320 6172 6520 7468 6520 6361 7274  ows are the cart
-000055f0: 6573 6961 6e20 636f 6f72 6469 6e61 7465  esian coordinate
-00005600: 730a 2020 2020 6f66 2074 6865 2070 6172  s.    of the par
-00005610: 656e 7420 6c61 7474 6963 6520 7665 6374  ent lattice vect
-00005620: 6f72 7320 616e 6420 6120 6d61 7472 6978  ors and a matrix
-00005630: 2077 686f 7365 2072 6f77 7320 6172 6520   whose rows are 
-00005640: 7468 6520 6361 7274 6573 6961 6e20 636f  the cartesian co
-00005650: 6f72 6469 6e61 7465 730a 2020 2020 6f66  ordinates.    of
-00005660: 2074 6865 2073 7570 6572 2d63 656c 6c20   the super-cell 
-00005670: 6c61 7474 6963 6520 7665 6374 6f72 733b  lattice vectors;
-00005680: 2074 6865 6e2c 2074 6869 7320 6675 6e63   then, this func
-00005690: 7469 6f6e 2072 6574 7572 6e73 2074 6865  tion returns the
-000056a0: 206d 6174 7269 7820 3a6d 6174 683a 6050   matrix :math:`P
-000056b0: 3d53 565e 7b2d 317d 602e 0a20 2020 2049  =SV^{-1}`..    I
-000056c0: 6620 7468 6520 7265 7375 6c74 696e 6720  f the resulting 
-000056d0: 6d61 7472 6978 2069 7320 6e6f 7420 696e  matrix is not in
-000056e0: 7465 6765 7220 2873 6565 2060 6072 6e64  teger (see ``rnd
-000056f0: 6060 2070 6172 616d 6574 6572 292c 2074  `` parameter), t
-00005700: 6865 6e20 6060 4e6f 6e65 6060 2069 7320  hen ``None`` is 
-00005710: 7265 7475 726e 6564 2e0a 0a20 2020 202a  returned...    *
-00005720: 2a50 6172 616d 6574 6572 733a 2a2a 0a0a  *Parameters:**..
-00005730: 2020 2020 6060 7063 656c 6c60 603a 2033      ``pcell``: 3
-00005740: 7833 2061 7272 6179 206f 6620 666c 6f61  x3 array of floa
-00005750: 740a 2020 2020 2020 2020 5468 6520 726f  t.        The ro
-00005760: 7773 206f 6620 7468 6973 206d 6174 7269  ws of this matri
-00005770: 7820 636f 7272 6573 706f 6e64 2074 6f20  x correspond to 
-00005780: 7468 6520 6361 7274 6573 6961 6e20 636f  the cartesian co
-00005790: 6f72 6469 6e61 7465 7320 6f66 2061 2070  ordinates of a p
-000057a0: 6172 656e 7420 6c61 7474 6963 650a 0a20  arent lattice.. 
-000057b0: 2020 2060 6073 6365 6c6c 6060 3a20 3378     ``scell``: 3x
-000057c0: 3320 6172 7261 7920 6f66 2066 6c6f 6174  3 array of float
-000057d0: 0a20 2020 2020 2020 2054 6865 2072 6f77  .        The row
-000057e0: 7320 6f66 2074 6869 7320 6d61 7472 6978  s of this matrix
-000057f0: 2063 6f72 7265 7370 6f6e 6420 746f 2074   correspond to t
-00005800: 6865 2063 6172 7465 7369 616e 2063 6f6f  he cartesian coo
-00005810: 7264 696e 6174 6573 206f 6620 6120 7375  rdinates of a su
-00005820: 7065 7263 656c 6c0a 0a20 2020 2060 6072  percell..    ``r
-00005830: 6e64 6060 3a20 696e 7465 6765 7220 286f  nd``: integer (o
-00005840: 7074 696f 6e61 6c29 0a20 2020 2020 2020  ptional).       
-00005850: 2020 5468 6520 6d61 7472 6978 203a 6d61    The matrix :ma
-00005860: 7468 3a60 503d 5356 5e7b 2d31 7d60 2069  th:`P=SV^{-1}` i
-00005870: 7320 726f 756e 6465 6420 746f 2060 6072  s rounded to ``r
-00005880: 6e64 6060 2064 6563 696d 616c 2070 6c61  nd`` decimal pla
-00005890: 6365 7320 616e 6420 6368 6563 6b65 6420  ces and checked 
-000058a0: 666f 7220 696e 7465 6772 6974 792e 0a20  for integrity.. 
-000058b0: 2020 2022 2222 0a20 2020 2074 6d61 7420     """.    tmat 
-000058c0: 3d20 6e70 2e64 6f74 2873 6365 6c6c 2c6e  = np.dot(scell,n
-000058d0: 702e 6c69 6e61 6c67 2e69 6e76 2870 6365  p.linalg.inv(pce
-000058e0: 6c6c 2929 0a20 2020 2069 6620 5f69 735f  ll)).    if _is_
-000058f0: 696e 7465 6765 725f 6d61 7472 6978 2874  integer_matrix(t
-00005900: 6d61 742c 726e 6429 3a0a 2020 2020 2020  mat,rnd):.      
-00005910: 2020 7265 7475 726e 206e 702e 6173 6172    return np.asar
-00005920: 7261 7928 6e70 2e72 696e 7428 746d 6174  ray(np.rint(tmat
-00005930: 292e 6173 7479 7065 2869 6e74 2929 0a20  ).astype(int)). 
-00005940: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00005950: 2072 6574 7572 6e20 4e6f 6e65 0a0a 6465   return None..de
-00005960: 6620 5f73 7472 5f67 7265 7028 696e 7075  f _str_grep(inpu
-00005970: 745f 7374 722c 2073 6561 7263 685f 7374  t_str, search_st
-00005980: 722c 2070 7265 7065 6e64 3d27 2729 3a0a  r, prepend=''):.
-00005990: 2020 2020 6f75 745f 7374 7220 3d20 2727      out_str = ''
-000059a0: 0a20 2020 2066 6f72 206c 2069 6e20 696e  .    for l in in
-000059b0: 7075 745f 7374 722e 7370 6c69 7428 275c  put_str.split('\
-000059c0: 6e27 293a 0a20 2020 2020 2020 2069 6620  n'):.        if 
-000059d0: 7365 6172 6368 5f73 7472 2069 6e20 6c3a  search_str in l:
-000059e0: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
-000059f0: 5f73 7472 203d 206f 7574 5f73 7472 202b  _str = out_str +
-00005a00: 2070 7265 7065 6e64 202b 206c 2e73 7472   prepend + l.str
-00005a10: 6970 2829 202b 2027 5c6e 270a 0a20 2020  ip() + '\n'..   
-00005a20: 2072 6574 7572 6e20 6f75 745f 7374 722e   return out_str.
-00005a30: 7273 7472 6970 2829 0a0a 6465 6620 6d67  rstrip()..def mg
-00005a40: 7265 7028 6670 6174 682c 2073 6561 7263  rep(fpath, searc
-00005a50: 685f 6172 7261 792c 2070 7265 7065 6e64  h_array, prepend
-00005a60: 3d27 272c 726f 6f74 3d27 2e27 293a 0a20  ='',root='.'):. 
-00005a70: 2020 2022 2222 0a20 2020 2047 7265 7020     """.    Grep 
-00005a80: 7374 7269 6e67 7320 696e 2066 696c 6520  strings in file 
-00005a90: 616e 6420 7265 7475 726e 206d 6174 6368  and return match
-00005aa0: 696e 6720 6c69 6e65 732e 0a0a 2020 2020  ing lines...    
-00005ab0: 2a2a 5061 7261 6d65 7465 7273 3a2a 2a0a  **Parameters:**.
-00005ac0: 2020 2020 0a20 2020 2060 6066 7061 7468      .    ``fpath
-00005ad0: 6060 3a20 7374 7269 6e67 0a20 2020 2020  ``: string.     
-00005ae0: 2020 2046 696c 6520 7061 7468 2074 6f20     File path to 
-00005af0: 6772 6570 0a20 2020 2060 6073 6561 7263  grep.    ``searc
-00005b00: 685f 6172 7261 7960 603a 2061 7272 6179  h_array``: array
-00005b10: 206f 6620 7374 7269 6e67 730a 2020 2020   of strings.    
-00005b20: 2020 2020 4561 6368 2065 6c65 6d65 6e74      Each element
-00005b30: 206f 6620 7468 6520 6172 7261 7920 6973   of the array is
-00005b40: 2061 6e20 7374 7269 6e67 2074 6f20 6772   an string to gr
-00005b50: 6570 2069 6e20 6060 6670 6174 6860 602e  ep in ``fpath``.
-00005b60: 0a20 2020 2060 6070 7265 7065 6e64 6060  .    ``prepend``
-00005b70: 3a20 7374 7269 6e67 0a20 2020 2020 2020  : string.       
-00005b80: 2070 7265 7065 6e64 2073 7472 696e 6720   prepend string 
-00005b90: 6060 7072 6570 656e 6460 6020 746f 2065  ``prepend`` to e
-00005ba0: 6163 6820 6d61 7463 6869 6e67 206c 696e  ach matching lin
-00005bb0: 652e 0a20 2020 2060 6072 6f6f 7460 603a  e..    ``root``:
-00005bc0: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
-00005bd0: 4669 6c65 2074 6f20 6772 6570 2073 686f  File to grep sho
-00005be0: 756c 6420 6265 2069 6e20 6060 726f 6f74  uld be in ``root
-00005bf0: 2f66 7061 7468 6060 2e0a 2020 2020 2222  /fpath``..    ""
-00005c00: 220a 2020 2020 6162 735f 7061 7468 203d  ".    abs_path =
-00005c10: 206f 732e 7061 7468 2e6a 6f69 6e28 726f   os.path.join(ro
-00005c20: 6f74 2c66 7061 7468 290a 2020 2020 6f75  ot,fpath).    ou
-00005c30: 745f 7374 7220 3d20 2727 0a20 2020 2069  t_str = ''.    i
-00005c40: 6620 6f73 2e70 6174 682e 6973 6669 6c65  f os.path.isfile
-00005c50: 2861 6273 5f70 6174 6829 3a0a 2020 2020  (abs_path):.    
-00005c60: 2020 2020 6673 7472 203d 206f 7065 6e28      fstr = open(
-00005c70: 6162 735f 7061 7468 292e 7265 6164 2829  abs_path).read()
-00005c80: 0a0a 2020 2020 2020 2020 666f 7220 6174  ..        for at
-00005c90: 7472 2069 6e20 7365 6172 6368 5f61 7272  tr in search_arr
-00005ca0: 6179 3a0a 2020 2020 2020 2020 2020 2020  ay:.            
-00005cb0: 6f73 7472 203d 205f 7374 725f 6772 6570  ostr = _str_grep
-00005cc0: 2866 7374 722c 6174 7472 2c70 7265 7065  (fstr,attr,prepe
-00005cd0: 6e64 3d70 7265 7065 6e64 290a 0a20 2020  nd=prepend)..   
-00005ce0: 2020 2020 2020 2020 2069 6620 6f73 7472           if ostr
-00005cf0: 2021 3d20 2727 3a0a 2020 2020 2020 2020   != '':.        
-00005d00: 2020 2020 2020 2020 6f75 745f 7374 7220          out_str 
-00005d10: 3d20 6f75 745f 7374 7220 2b20 7072 6570  = out_str + prep
-00005d20: 656e 6420 2b20 6f73 7472 2e73 7472 6970  end + ostr.strip
-00005d30: 2829 202b 2027 5c6e 270a 0a20 2020 2072  () + '\n'..    r
-00005d40: 6574 7572 6e20 6f75 745f 7374 722e 7273  eturn out_str.rs
-00005d50: 7472 6970 2829 0a0a 0a64 6566 2070 6172  trip()...def par
-00005d60: 656e 745f 6c61 7474 6963 655f 746f 5f61  ent_lattice_to_a
-00005d70: 7461 7428 706c 6174 2c20 6f75 745f 666e  tat(plat, out_fn
-00005d80: 616d 653d 226c 6174 2e69 6e22 2c20 666f  ame="lat.in", fo
-00005d90: 725f 7374 7220 3d20 4661 6c73 6529 3a0a  r_str = False):.
-00005da0: 2020 2020 2222 2253 6572 6961 6c69 7a65      """Serialize
-00005db0: 7320 5061 7265 6e74 4c61 7474 6963 6520  s ParentLattice 
-00005dc0: 6f62 6a65 6374 2074 6f20 4154 4154 2069  object to ATAT i
-00005dd0: 6e70 7574 2066 696c 650a 0a20 2020 202a  nput file..    *
-00005de0: 2a50 6172 616d 6574 6572 733a 2a2a 0a0a  *Parameters:**..
-00005df0: 2020 2020 6060 706c 6174 6060 3a20 5061      ``plat``: Pa
-00005e00: 7265 6e74 4c61 7474 6963 6520 6f62 6a65  rentLattice obje
-00005e10: 6374 0a20 2020 2020 2020 2050 6172 656e  ct.        Paren
-00005e20: 744c 6174 7469 6365 206f 626a 6563 7420  tLattice object 
-00005e30: 746f 2062 6520 7365 7269 616c 697a 6564  to be serialized
-00005e40: 0a20 2020 2060 606f 7574 5f66 6e61 6d65  .    ``out_fname
-00005e50: 6060 3a20 7374 7269 6e67 0a20 2020 2020  ``: string.     
-00005e60: 2020 204f 7574 7075 7420 6669 6c65 2070     Output file p
-00005e70: 6174 680a 2020 2020 2222 220a 2020 2020  ath.    """.    
-00005e80: 6365 6c6c 203d 2070 6c61 742e 6765 745f  cell = plat.get_
-00005e90: 6365 6c6c 2829 0a20 2020 2070 6f73 6974  cell().    posit
-00005ea0: 696f 6e73 203d 2070 6c61 742e 6765 745f  ions = plat.get_
-00005eb0: 7363 616c 6564 5f70 6f73 6974 696f 6e73  scaled_positions
-00005ec0: 2829 0a20 2020 2069 6620 666f 725f 7374  ().    if for_st
-00005ed0: 723a 0a20 2020 2020 2020 2073 6974 6573  r:.        sites
-00005ee0: 203d 2070 6c61 742e 6765 745f 6174 6f6d   = plat.get_atom
-00005ef0: 6963 5f6e 756d 6265 7273 2829 0a20 2020  ic_numbers().   
-00005f00: 2065 6c73 653a 0a20 2020 2020 2020 2073   else:.        s
-00005f10: 6974 6573 203d 2070 6c61 742e 6765 745f  ites = plat.get_
-00005f20: 7369 7465 7328 290a 0a20 2020 2066 203d  sites()..    f =
-00005f30: 206f 7065 6e28 6f75 745f 666e 616d 652c   open(out_fname,
-00005f40: 2777 2b27 290a 0a20 2020 2066 6f72 2063  'w+')..    for c
-00005f50: 656c 6c76 2069 6e20 6365 6c6c 3a0a 2020  ellv in cell:.  
-00005f60: 2020 2020 2020 662e 7772 6974 6528 7522        f.write(u"
-00005f70: 2532 2e31 3266 5c74 2532 2e31 3266 5c74  %2.12f\t%2.12f\t
-00005f80: 2532 2e31 3266 5c6e 2225 2863 656c 6c76  %2.12f\n"%(cellv
-00005f90: 5b30 5d2c 6365 6c6c 765b 315d 2c63 656c  [0],cellv[1],cel
-00005fa0: 6c76 5b32 5d29 290a 0a20 2020 2066 2e77  lv[2]))..    f.w
-00005fb0: 7269 7465 2875 2231 2e30 3030 3030 3030  rite(u"1.0000000
-00005fc0: 3030 3030 305c 7430 2e30 3030 3030 3030  00000\t0.0000000
-00005fd0: 3030 3030 305c 7430 2e30 3030 3030 3030  00000\t0.0000000
-00005fe0: 3030 3030 305c 6e22 290a 2020 2020 662e  00000\n").    f.
-00005ff0: 7772 6974 6528 7522 302e 3030 3030 3030  write(u"0.000000
-00006000: 3030 3030 3030 5c74 312e 3030 3030 3030  000000\t1.000000
-00006010: 3030 3030 3030 5c74 302e 3030 3030 3030  000000\t0.000000
-00006020: 3030 3030 3030 5c6e 2229 0a20 2020 2066  000000\n").    f
-00006030: 2e77 7269 7465 2875 2230 2e30 3030 3030  .write(u"0.00000
-00006040: 3030 3030 3030 305c 7430 2e30 3030 3030  0000000\t0.00000
-00006050: 3030 3030 3030 305c 7431 2e30 3030 3030  0000000\t1.00000
-00006060: 3030 3030 3030 305c 6e22 290a 0a20 2020  0000000\n")..   
-00006070: 2066 6f72 2069 2c70 6f73 2069 6e20 656e   for i,pos in en
-00006080: 756d 6572 6174 6528 706f 7369 7469 6f6e  umerate(position
-00006090: 7329 3a0a 2020 2020 2020 2020 7374 7269  s):.        stri
-000060a0: 203d 2075 2225 322e 3132 665c 7425 322e   = u"%2.12f\t%2.
-000060b0: 3132 665c 7425 322e 3132 665c 7422 2528  12f\t%2.12f\t"%(
-000060c0: 706f 735b 305d 2c70 6f73 5b31 5d2c 706f  pos[0],pos[1],po
-000060d0: 735b 325d 290a 2020 2020 2020 2020 6966  s[2]).        if
-000060e0: 2066 6f72 5f73 7472 3a0a 2020 2020 2020   for_str:.      
-000060f0: 2020 2020 2020 7374 7269 203d 2073 7472        stri = str
-00006100: 6920 2b20 2225 735c 6e22 2563 735b 7369  i + "%s\n"%cs[si
-00006110: 7465 735b 695d 5d0a 2020 2020 2020 2020  tes[i]].        
-00006120: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00006130: 2020 6966 206c 656e 2873 6974 6573 5b69    if len(sites[i
-00006140: 5d29 3e31 3a0a 2020 2020 2020 2020 2020  ])>1:.          
-00006150: 2020 2020 2020 666f 7220 7a20 696e 2073        for z in s
-00006160: 6974 6573 5b69 5d5b 3a2d 315d 3a0a 2020  ites[i][:-1]:.  
-00006170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006180: 2020 7374 7269 203d 2073 7472 6920 2b20    stri = stri + 
-00006190: 2225 732c 2225 6373 5b7a 5d0a 2020 2020  "%s,"%cs[z].    
-000061a0: 2020 2020 2020 2020 7374 7269 203d 2073          stri = s
-000061b0: 7472 6920 2b20 2225 735c 6e22 2563 735b  tri + "%s\n"%cs[
-000061c0: 7369 7465 735b 695d 5b2d 315d 5d0a 0a20  sites[i][-1]].. 
-000061d0: 2020 2020 2020 2066 2e77 7269 7465 2873         f.write(s
-000061e0: 7472 6929 0a0a 2020 2020 662e 636c 6f73  tri)..    f.clos
-000061f0: 6528 290a 0a63 6c61 7373 2045 7870 6f6e  e()..class Expon
-00006200: 656e 7469 616c 2829 3a0a 2020 2020 2222  ential():.    ""
-00006210: 2242 6173 6963 2065 7870 6f6e 656e 7469  "Basic exponenti
-00006220: 616c 206f 626a 6563 7420 6f66 2074 7970  al object of typ
-00006230: 6520 6060 636f 6566 6669 6369 656e 7460  e ``coefficient`
-00006240: 6020 2a20 6060 7860 6020 5e20 6060 6578  ` * ``x`` ^ ``ex
-00006250: 706f 6e65 6e74 6060 202e 204e 756d 6572  ponent`` . Numer
-00006260: 6963 616c 6c79 2065 7661 6c75 6574 6564  ically evalueted
-00006270: 2075 7369 6e67 2074 6865 206d 6574 686f   using the metho
-00006280: 6420 6060 6576 616c 7561 7465 6060 2028  d ``evaluate`` (
-00006290: 2060 6078 6060 2029 202e 0a0a 2020 2020   ``x`` ) ...    
-000062a0: 2a2a 5061 7261 6d65 7465 7273 3a2a 2a0a  **Parameters:**.
-000062b0: 0a20 2020 2060 6065 7870 6f6e 656e 7460  .    ``exponent`
-000062c0: 603a 2065 7870 6f6e 656e 7420 6f66 2074  `: exponent of t
-000062d0: 6865 2065 7870 6f6e 656e 7469 616c 0a0a  he exponential..
-000062e0: 2020 2020 6060 636f 6566 6669 6369 656e      ``coefficien
-000062f0: 7460 603a 2063 6f65 6666 6963 6965 6e74  t``: coefficient
-00006300: 206f 6620 7468 6520 6578 706f 6e65 6e74   of the exponent
-00006310: 6961 6c0a 0a20 2020 2022 2222 0a0a 2020  ial..    """..  
-00006320: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00006330: 656c 662c 2065 7870 6f6e 656e 742c 2063  elf, exponent, c
-00006340: 6f65 6666 6963 6965 6e74 203d 2031 293a  oefficient = 1):
-00006350: 0a20 2020 2020 2020 2073 656c 662e 6578  .        self.ex
-00006360: 706f 6e65 6e74 203d 2065 7870 6f6e 656e  ponent = exponen
-00006370: 740a 2020 2020 2020 2020 7365 6c66 2e63  t.        self.c
-00006380: 6f65 6666 6963 6965 6e74 203d 2063 6f65  oefficient = coe
-00006390: 6666 6963 6965 6e74 0a0a 2020 2020 6465  fficient..    de
-000063a0: 6620 6576 616c 7561 7465 2873 656c 662c  f evaluate(self,
-000063b0: 2078 293a 0a20 2020 2020 2020 2072 6574   x):.        ret
-000063c0: 7572 6e20 7365 6c66 2e63 6f65 6666 6963  urn self.coeffic
-000063d0: 6965 6e74 202a 206e 702e 706f 7765 7228  ient * np.power(
-000063e0: 782c 7365 6c66 2e65 7870 6f6e 656e 7429  x,self.exponent)
-000063f0: 0a0a 2020 2020 6465 6620 6469 7669 6465  ..    def divide
-00006400: 5f73 6361 6c61 7228 7365 6c66 2c20 7661  _scalar(self, va
-00006410: 6c75 6529 3a0a 2020 2020 2020 2020 7365  lue):.        se
-00006420: 6c66 2e63 6f65 6666 6963 6965 6e74 203d  lf.coefficient =
-00006430: 2073 656c 662e 636f 6566 6669 6369 656e   self.coefficien
-00006440: 7420 2f20 7661 6c75 650a 0a20 2020 2064  t / value..    d
-00006450: 6566 206d 756c 7469 706c 795f 7363 616c  ef multiply_scal
-00006460: 6172 2873 656c 662c 2073 6361 6c61 7229  ar(self, scalar)
-00006470: 3a0a 2020 2020 2020 2020 7365 6c66 2e63  :.        self.c
-00006480: 6f65 6666 6963 6965 6e74 203d 2073 656c  oefficient = sel
-00006490: 662e 636f 6566 6669 6369 656e 7420 2a20  f.coefficient * 
-000064a0: 7363 616c 6172 0a0a 0a63 6c61 7373 2050  scalar...class P
-000064b0: 6f6c 796e 6f6d 6961 6c46 756e 6374 696f  olynomialFunctio
-000064c0: 6e28 293a 0a20 2020 2022 2222 506f 6c79  n():.    """Poly
-000064d0: 6e6f 6d69 616c 2066 756e 6374 696f 6e2c  nomial function,
-000064e0: 2062 7569 6c64 2066 726f 6d20 6060 4578   build from ``Ex
-000064f0: 706f 6e65 6e74 6961 6c28 2960 6020 2e0a  ponential()`` ..
-00006500: 2020 2020 2222 220a 0a0a 2020 2020 6465      """...    de
-00006510: 6620 5f5f 696e 6974 5f5f 2873 656c 6629  f __init__(self)
-00006520: 3a0a 2020 2020 2020 2020 7365 6c66 2e65  :.        self.e
-00006530: 7870 6f6e 656e 7469 616c 7320 3d20 5b5d  xponentials = []
-00006540: 0a0a 2020 2020 6465 6620 6164 645f 6578  ..    def add_ex
-00006550: 706f 6e65 6e74 6961 6c28 7365 6c66 2c20  ponential(self, 
-00006560: 6f72 6465 722c 2063 6f65 6666 6963 6965  order, coefficie
-00006570: 6e74 203d 2031 293a 0a20 2020 2020 2020  nt = 1):.       
-00006580: 2069 6e5f 7375 6d20 3d20 4661 6c73 650a   in_sum = False.
-00006590: 2020 2020 2020 2020 666f 7220 6578 706f          for expo
-000065a0: 6e65 6e74 6961 6c20 696e 2073 656c 662e  nential in self.
-000065b0: 6578 706f 6e65 6e74 6961 6c73 3a0a 2020  exponentials:.  
-000065c0: 2020 2020 2020 2020 2020 6966 2065 7870            if exp
-000065d0: 6f6e 656e 7469 616c 2e65 7870 6f6e 656e  onential.exponen
-000065e0: 7420 3d3d 206f 7264 6572 3a0a 2020 2020  t == order:.    
-000065f0: 2020 2020 2020 2020 2020 2020 6578 706f              expo
-00006600: 6e65 6e74 6961 6c2e 636f 6566 6669 6369  nential.coeffici
-00006610: 656e 7420 2b3d 2063 6f65 6666 6963 6965  ent += coefficie
-00006620: 6e74 0a20 2020 2020 2020 2020 2020 2020  nt.             
-00006630: 2020 2069 6e5f 7375 6d20 3d20 5472 7565     in_sum = True
-00006640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006650: 2062 7265 616b 0a20 2020 2020 2020 2069   break.        i
-00006660: 6620 6e6f 7420 696e 5f73 756d 3a0a 2020  f not in_sum:.  
-00006670: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
-00006680: 7870 6f6e 656e 7469 616c 732e 6170 7065  xponentials.appe
-00006690: 6e64 2845 7870 6f6e 656e 7469 616c 286f  nd(Exponential(o
-000066a0: 7264 6572 2c20 636f 6566 6669 6369 656e  rder, coefficien
-000066b0: 7429 290a 0a20 2020 2064 6566 2063 6c65  t))..    def cle
-000066c0: 6172 5f65 7870 6f6e 656e 7469 616c 7328  ar_exponentials(
-000066d0: 7365 6c66 293a 0a20 2020 2020 2020 2066  self):.        f
-000066e0: 6f72 2065 7870 6f6e 656e 7469 616c 2069  or exponential i
-000066f0: 6e20 7365 6c66 2e65 7870 6f6e 656e 7469  n self.exponenti
-00006700: 616c 733a 0a20 2020 2020 2020 2020 2020  als:.           
-00006710: 2069 6620 6162 7328 6578 706f 6e65 6e74   if abs(exponent
-00006720: 6961 6c2e 636f 6566 6669 6369 656e 7429  ial.coefficient)
-00006730: 203c 2031 302a 2a28 2d31 3529 3a0a 2020   < 10**(-15):.  
-00006740: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00006750: 6c66 2e65 7870 6f6e 656e 7469 616c 732e  lf.exponentials.
-00006760: 7265 6d6f 7665 2865 7870 6f6e 656e 7469  remove(exponenti
-00006770: 616c 290a 0a20 2020 2064 6566 2065 7661  al)..    def eva
-00006780: 6c75 6174 6528 7365 6c66 2c20 7829 3a0a  luate(self, x):.
-00006790: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
-000067a0: 300a 2020 2020 2020 2020 666f 7220 6578  0.        for ex
-000067b0: 706f 6e65 6e74 6961 6c20 696e 2073 656c  ponential in sel
-000067c0: 662e 6578 706f 6e65 6e74 6961 6c73 3a0a  f.exponentials:.
-000067d0: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
-000067e0: 6520 2b3d 2065 7870 6f6e 656e 7469 616c  e += exponential
-000067f0: 2e65 7661 6c75 6174 6528 7829 0a20 2020  .evaluate(x).   
-00006800: 2020 2020 2072 6574 7572 6e20 7661 6c75       return valu
-00006810: 650a 0a20 2020 2064 6566 206e 6f72 6d61  e..    def norma
-00006820: 6c69 7a65 2873 656c 662c 2073 6361 6c61  lize(self, scala
-00006830: 725f 7072 6f64 7563 742c 206d 293a 0a20  r_product, m):. 
-00006840: 2020 2020 2020 206c 656e 6774 6820 3d20         length = 
-00006850: 7363 616c 6172 5f70 726f 6475 6374 2873  scalar_product(s
-00006860: 656c 662e 6576 616c 7561 7465 2c20 7365  elf.evaluate, se
-00006870: 6c66 2e65 7661 6c75 6174 652c 206d 290a  lf.evaluate, m).
-00006880: 2020 2020 2020 2020 6c65 6e67 7468 203d          length =
-00006890: 206e 702e 7371 7274 286c 656e 6774 6829   np.sqrt(length)
-000068a0: 0a20 2020 2020 2020 2066 6f72 2065 7870  .        for exp
-000068b0: 6f6e 656e 7469 616c 2069 6e20 7365 6c66  onential in self
-000068c0: 2e65 7870 6f6e 656e 7469 616c 733a 0a20  .exponentials:. 
-000068d0: 2020 2020 2020 2020 2020 2065 7870 6f6e             expon
-000068e0: 656e 7469 616c 2e64 6976 6964 655f 7363  ential.divide_sc
-000068f0: 616c 6172 286c 656e 6774 6829 0a0a 2020  alar(length)..  
-00006900: 2020 6465 6620 6d75 6c74 6970 6c79 5f73    def multiply_s
-00006910: 6361 6c61 7228 7365 6c66 2c20 7363 616c  calar(self, scal
-00006920: 6172 293a 0a20 2020 2020 2020 2066 6f72  ar):.        for
-00006930: 2065 7870 6f6e 656e 7469 616c 2069 6e20   exponential in 
-00006940: 7365 6c66 2e65 7870 6f6e 656e 7469 616c  self.exponential
-00006950: 733a 0a20 2020 2020 2020 2020 2020 2065  s:.            e
-00006960: 7870 6f6e 656e 7469 616c 2e6d 756c 7469  xponential.multi
-00006970: 706c 795f 7363 616c 6172 2873 6361 6c61  ply_scalar(scala
-00006980: 7229 0a0a 2020 2020 6465 6620 6164 645f  r)..    def add_
-00006990: 706f 6c79 6e6f 6d69 616c 5f66 756e 6374  polynomial_funct
-000069a0: 696f 6e28 7365 6c66 2c20 706f 6c79 6e6f  ion(self, polyno
-000069b0: 6d69 616c 5f66 756e 6374 696f 6e29 3a0a  mial_function):.
-000069c0: 2020 2020 2020 2020 666f 7220 6578 706f          for expo
-000069d0: 6e65 6e74 6961 6c20 696e 2070 6f6c 796e  nential in polyn
-000069e0: 6f6d 6961 6c5f 6675 6e63 7469 6f6e 2e65  omial_function.e
-000069f0: 7870 6f6e 656e 7469 616c 733a 0a20 2020  xponentials:.   
-00006a00: 2020 2020 2020 2020 2073 656c 662e 6164           self.ad
-00006a10: 645f 6578 706f 6e65 6e74 6961 6c28 6578  d_exponential(ex
-00006a20: 706f 6e65 6e74 6961 6c2e 6578 706f 6e65  ponential.expone
-00006a30: 6e74 2c20 6578 706f 6e65 6e74 6961 6c2e  nt, exponential.
-00006a40: 636f 6566 6669 6369 656e 7429 0a0a 2020  coefficient)..  
-00006a50: 2020 6465 6620 7072 696e 745f 706f 6c79    def print_poly
-00006a60: 6e6f 6d69 616c 2873 656c 6629 3a0a 2020  nomial(self):.  
-00006a70: 2020 2020 2020 6f75 7473 7472 696e 6720        outstring 
-00006a80: 3d20 2727 0a20 2020 2020 2020 2066 6f72  = ''.        for
-00006a90: 2065 7870 6f6e 656e 7469 616c 2069 6e20   exponential in 
-00006aa0: 7365 6c66 2e65 7870 6f6e 656e 7469 616c  self.exponential
-00006ab0: 733a 0a20 2020 2020 2020 2020 2020 206f  s:.            o
-00006ac0: 7574 7374 7269 6e67 202b 3d20 7374 7228  utstring += str(
-00006ad0: 6578 706f 6e65 6e74 6961 6c2e 636f 6566  exponential.coef
-00006ae0: 6669 6369 656e 7429 202b 2027 202a 2020  ficient) + ' *  
-00006af0: 785e 2720 2b20 7374 7228 6578 706f 6e65  x^' + str(expone
-00006b00: 6e74 6961 6c2e 6578 706f 6e65 6e74 2920  ntial.exponent) 
-00006b10: 2b20 2720 2b20 270a 2020 2020 2020 2020  + ' + '.        
-00006b20: 6f75 7473 7472 696e 6720 3d20 6f75 7473  outstring = outs
-00006b30: 7472 696e 675b 3a2d 335d 0a20 2020 2020  tring[:-3].     
-00006b40: 2020 2070 7269 6e74 286f 7574 7374 7269     print(outstri
-00006b50: 6e67 290a 0a0a 636c 6173 7320 506f 6c79  ng)...class Poly
-00006b60: 6e6f 6d69 616c 4261 7369 7328 293a 0a20  nomialBasis():. 
-00006b70: 2020 2022 2222 506f 6c79 6e6f 6d69 616c     """Polynomial
-00006b80: 2062 6173 6973 2c20 636f 6e73 7472 7563   basis, construc
-00006b90: 7465 6420 6672 6f6d 2073 6576 6572 616c  ted from several
-00006ba0: 2060 6050 6f6c 796e 6f6d 6961 6c46 756e   ``PolynomialFun
-00006bb0: 6374 696f 6e28 2960 602e 0a20 2020 2043  ction()``..    C
-00006bc0: 6f6e 7374 7275 6374 7320 6f72 7468 6f6e  onstructs orthon
-00006bd0: 6f72 6d61 6c20 6261 7369 7320 7365 7473  ormal basis sets
-00006be0: 2075 7369 6e67 2060 6073 6361 6c63 6172   using ``scalcar
-00006bf0: 5f70 726f 6475 6374 6060 202e 0a20 2020  _product`` ..   
-00006c00: 2057 6865 6e20 696e 6974 6961 6c69 7a65   When initialize
-00006c10: 642c 2061 6c6c 206f 7274 686f 6e6f 726d  d, all orthonorm
-00006c20: 616c 2062 6173 6973 2073 6574 7320 746f  al basis sets to
-00006c30: 2074 6865 206f 7264 6572 2060 606d 6178   the order ``max
-00006c40: 5f6f 7264 6572 6060 2061 7265 2067 656e  _order`` are gen
-00006c50: 6572 6174 6564 2e0a 0a20 2020 202a 2a50  erated...    **P
-00006c60: 6172 616d 6574 6572 732a 2a0a 0a20 2020  arameters**..   
-00006c70: 2060 606d 6178 5f6f 7264 6572 6060 3a20   ``max_order``: 
-00006c80: 4d61 7869 6d61 6c20 6f72 6465 7220 746f  Maximal order to
-00006c90: 2077 6869 6368 2074 6865 2062 6173 6973   which the basis
-00006ca0: 2073 6574 2069 7320 696e 6974 6961 6c69   set is initiali
-00006cb0: 7a65 642e 0a0a 2020 2020 6060 7379 6d6d  zed...    ``symm
-00006cc0: 6574 7269 6360 603a 2044 6566 696e 6573  etric``: Defines
-00006cd0: 2069 6620 7468 6520 7363 616c 6172 2070   if the scalar p
-00006ce0: 726f 6475 6374 2075 7365 7320 7369 676d  roduct uses sigm
-00006cf0: 6173 2073 796d 6d65 7472 697a 6564 2061  as symmetrized a
-00006d00: 726f 756e 6420 3020 6f72 2061 7363 656e  round 0 or ascen
-00006d10: 6469 6e67 2066 726f 6d20 302e 0a0a 2020  ding from 0...  
-00006d20: 2020 2222 220a 0a20 2020 2064 6566 205f    """..    def _
-00006d30: 5f69 6e69 745f 5f28 7365 6c66 2c20 6d61  _init__(self, ma
-00006d40: 785f 6f72 6465 7220 3d20 3130 2c20 7379  x_order = 10, sy
-00006d50: 6d6d 6574 7269 6320 3d20 4661 6c73 6529  mmetric = False)
-00006d60: 3a0a 2020 2020 2020 2020 7365 6c66 2e6d  :.        self.m
-00006d70: 203d 206d 6178 5f6f 7264 6572 0a20 2020   = max_order.   
-00006d80: 2020 2020 2073 656c 662e 7379 6d6d 6574       self.symmet
-00006d90: 7269 6320 3d20 7379 6d6d 6574 7269 630a  ric = symmetric.
-00006da0: 2020 2020 2020 2020 7365 6c66 2e62 6173          self.bas
-00006db0: 6973 5f66 756e 6374 696f 6e5f 7365 7420  is_function_set 
-00006dc0: 3d20 7b7d 0a20 2020 2020 2020 2066 6f72  = {}.        for
-00006dd0: 206f 7264 6572 2069 6e20 7261 6e67 6528   order in range(
-00006de0: 312c 6d61 785f 6f72 6465 722b 3129 3a0a  1,max_order+1):.
-00006df0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00006e00: 2e62 6173 6973 5f66 756e 6374 696f 6e5f  .basis_function_
-00006e10: 7365 745b 7374 7228 6f72 6465 7229 5d20  set[str(order)] 
-00006e20: 3d20 7365 6c66 2e63 6f6e 7374 7275 6374  = self.construct
-00006e30: 286f 7264 6572 290a 0a20 2020 2064 6566  (order)..    def
-00006e40: 2063 6f6e 7374 7275 6374 2873 656c 662c   construct(self,
-00006e50: 206d 293a 0a20 2020 2020 2020 2062 6173   m):.        bas
-00006e60: 6973 5f66 756e 6374 696f 6e73 203d 205b  is_functions = [
-00006e70: 5d0a 2020 2020 2020 2020 666f 7220 6465  ].        for de
-00006e80: 6772 6565 2069 6e20 7261 6e67 6528 6d29  gree in range(m)
-00006e90: 3a0a 2020 2020 2020 2020 2020 2020 6e65  :.            ne
-00006ea0: 775f 6675 6e63 7469 6f6e 203d 2050 6f6c  w_function = Pol
-00006eb0: 796e 6f6d 6961 6c46 756e 6374 696f 6e28  ynomialFunction(
-00006ec0: 290a 2020 2020 2020 2020 2020 2020 6e65  ).            ne
-00006ed0: 775f 6675 6e63 7469 6f6e 2e61 6464 5f65  w_function.add_e
-00006ee0: 7870 6f6e 656e 7469 616c 2864 6567 7265  xponential(degre
-00006ef0: 6529 0a20 2020 2020 2020 2020 2020 2063  e).            c
-00006f00: 6869 203d 2045 7870 6f6e 656e 7469 616c  hi = Exponential
-00006f10: 2864 6567 7265 6529 0a20 2020 2020 2020  (degree).       
-00006f20: 2020 2020 2066 6f72 2062 6173 6973 5f66       for basis_f
-00006f30: 756e 6374 696f 6e20 696e 2062 6173 6973  unction in basis
-00006f40: 5f66 756e 6374 696f 6e73 3a0a 2020 2020  _functions:.    
-00006f50: 2020 2020 2020 2020 2020 2020 6f76 6572              over
-00006f60: 6c61 7020 3d20 7365 6c66 2e73 6361 6c61  lap = self.scala
-00006f70: 725f 7072 6f64 7563 7428 6261 7369 735f  r_product(basis_
-00006f80: 6675 6e63 7469 6f6e 2e65 7661 6c75 6174  function.evaluat
-00006f90: 652c 6368 692e 6576 616c 7561 7465 2c20  e,chi.evaluate, 
-00006fa0: 6d29 0a20 2020 2020 2020 2020 2020 2020  m).             
-00006fb0: 2020 206f 7665 726c 6170 203d 206f 7665     overlap = ove
-00006fc0: 726c 6170 202a 2028 2d31 290a 2020 2020  rlap * (-1).    
-00006fd0: 2020 2020 2020 2020 2020 2020 7375 6d6d              summ
-00006fe0: 616e 6420 3d20 636f 7079 2e64 6565 7063  and = copy.deepc
-00006ff0: 6f70 7928 6261 7369 735f 6675 6e63 7469  opy(basis_functi
-00007000: 6f6e 290a 2020 2020 2020 2020 2020 2020  on).            
-00007010: 2020 2020 7375 6d6d 616e 642e 6d75 6c74      summand.mult
-00007020: 6970 6c79 5f73 6361 6c61 7228 6f76 6572  iply_scalar(over
-00007030: 6c61 7029 0a20 2020 2020 2020 2020 2020  lap).           
-00007040: 2020 2020 206e 6577 5f66 756e 6374 696f       new_functio
-00007050: 6e2e 6164 645f 706f 6c79 6e6f 6d69 616c  n.add_polynomial
-00007060: 5f66 756e 6374 696f 6e28 7375 6d6d 616e  _function(summan
-00007070: 6429 0a20 2020 2020 2020 2020 2020 206e  d).            n
-00007080: 6577 5f66 756e 6374 696f 6e2e 6e6f 726d  ew_function.norm
-00007090: 616c 697a 6528 7365 6c66 2e73 6361 6c61  alize(self.scala
-000070a0: 725f 7072 6f64 7563 742c 206d 290a 2020  r_product, m).  
-000070b0: 2020 2020 2020 2020 2020 6e65 775f 6675            new_fu
-000070c0: 6e63 7469 6f6e 2e63 6c65 6172 5f65 7870  nction.clear_exp
-000070d0: 6f6e 656e 7469 616c 7328 290a 2020 2020  onentials().    
-000070e0: 2020 2020 2020 2020 6261 7369 735f 6675          basis_fu
-000070f0: 6e63 7469 6f6e 732e 6170 7065 6e64 286e  nctions.append(n
-00007100: 6577 5f66 756e 6374 696f 6e29 0a20 2020  ew_function).   
-00007110: 2020 2020 2072 6574 7572 6e20 6261 7369       return basi
-00007120: 735f 6675 6e63 7469 6f6e 730a 0a20 2020  s_functions..   
-00007130: 2064 6566 2073 6361 6c61 725f 7072 6f64   def scalar_prod
-00007140: 7563 7428 7365 6c66 2c20 6675 6e63 7469  uct(self, functi
-00007150: 6f6e 312c 2066 756e 6374 696f 6e32 2c20  on1, function2, 
-00007160: 6d29 3a0a 2020 2020 2020 2020 2222 220a  m):.        """.
-00007170: 2020 2020 2020 2020 7265 7475 726e 7320          returns 
-00007180: 7468 6520 7265 7375 6c74 206f 6620 7468  the result of th
-00007190: 6520 7363 616c 6172 2070 726f 6475 6374  e scalar product
-000071a0: 2031 2f6d 2073 756d 5f7b 7369 676d 617d   1/m sum_{sigma}
-000071b0: 2066 5f31 2873 6967 6d61 2920 2a20 665f   f_1(sigma) * f_
-000071c0: 3228 7369 676d 6129 0a20 2020 2020 2020  2(sigma).       
-000071d0: 2022 2222 0a20 2020 2020 2020 2073 6361   """.        sca
-000071e0: 6c69 6e67 203d 2031 202f 206d 0a20 2020  ling = 1 / m.   
-000071f0: 2020 2020 2069 6620 7365 6c66 2e73 796d       if self.sym
-00007200: 6d65 7472 6963 3a0a 2020 2020 2020 2020  metric:.        
-00007210: 2020 2020 7369 676d 6173 203d 205b 7820      sigmas = [x 
-00007220: 666f 7220 7820 696e 2072 616e 6765 282d  for x in range(-
-00007230: 696e 7428 6d2f 3229 2c20 696e 7428 6d2f  int(m/2), int(m/
-00007240: 3229 2b31 295d 0a20 2020 2020 2020 2020  2)+1)].         
-00007250: 2020 2069 6620 6d20 2520 3220 3d3d 2030     if m % 2 == 0
-00007260: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00007270: 2020 7369 676d 6173 2e72 656d 6f76 6528    sigmas.remove(
-00007280: 3029 0a20 2020 2020 2020 2065 6c73 653a  0).        else:
-00007290: 0a20 2020 2020 2020 2020 2020 2073 6967  .            sig
-000072a0: 6d61 7320 3d20 7261 6e67 6528 6d29 0a20  mas = range(m). 
-000072b0: 2020 2020 2020 2073 6361 6c61 725f 7072         scalar_pr
-000072c0: 6f64 7563 7420 3d20 300a 2020 2020 2020  oduct = 0.      
-000072d0: 2020 666f 7220 7369 676d 6120 696e 2073    for sigma in s
-000072e0: 6967 6d61 733a 0a20 2020 2020 2020 2020  igmas:.         
-000072f0: 2020 2073 6361 6c61 725f 7072 6f64 7563     scalar_produc
-00007300: 7420 2b3d 2066 756e 6374 696f 6e31 2873  t += function1(s
-00007310: 6967 6d61 2920 2a20 6675 6e63 7469 6f6e  igma) * function
-00007320: 3228 7369 676d 6129 0a20 2020 2020 2020  2(sigma).       
-00007330: 2073 6361 6c61 725f 7072 6f64 7563 7420   scalar_product 
-00007340: 3d20 7363 616c 6172 5f70 726f 6475 6374  = scalar_product
-00007350: 202a 2073 6361 6c69 6e67 0a20 2020 2020   * scaling.     
-00007360: 2020 2072 6574 7572 6e20 7363 616c 6172     return scalar
-00007370: 5f70 726f 6475 6374 0a0a 2020 2020 6465  _product..    de
-00007380: 6620 7072 696e 745f 6261 7369 735f 6675  f print_basis_fu
-00007390: 6e63 7469 6f6e 7328 7365 6c66 2c20 6d29  nctions(self, m)
-000073a0: 3a0a 2020 2020 2020 2020 666f 7220 6675  :.        for fu
-000073b0: 6e63 7469 6f6e 2069 6e20 7365 6c66 2e62  nction in self.b
-000073c0: 6173 6973 5f66 756e 6374 696f 6e5f 7365  asis_function_se
-000073d0: 745b 7374 7228 6d29 5d3a 0a20 2020 2020  t[str(m)]:.     
-000073e0: 2020 2020 2020 2066 756e 6374 696f 6e2e         function.
-000073f0: 7072 696e 745f 706f 6c79 6e6f 6d69 616c  print_polynomial
-00007400: 2829 0a0a 2020 2020 6465 6620 6576 616c  ()..    def eval
-00007410: 7561 7465 2873 656c 662c 2061 6c70 6861  uate(self, alpha
-00007420: 2c20 7369 676d 612c 206d 293a 0a20 2020  , sigma, m):.   
-00007430: 2020 2020 2069 6620 6d20 3e20 7365 6c66       if m > self
-00007440: 2e6d 3a0a 2020 2020 2020 2020 2020 2020  .m:.            
-00007450: 7365 6c66 2e62 6173 6973 5f66 756e 6374  self.basis_funct
-00007460: 696f 6e5f 7365 745b 7374 7228 6d29 5d20  ion_set[str(m)] 
-00007470: 3d20 7365 6c66 2e63 6f6e 7374 7275 6374  = self.construct
-00007480: 286d 290a 2020 2020 2020 2020 7265 7475  (m).        retu
-00007490: 726e 2073 656c 662e 6261 7369 735f 6675  rn self.basis_fu
-000074a0: 6e63 7469 6f6e 5f73 6574 5b73 7472 286d  nction_set[str(m
-000074b0: 295d 5b69 6e74 2861 6c70 6861 295d 2e65  )][int(alpha)].e
-000074c0: 7661 6c75 6174 6528 7369 676d 6129 0a0a  valuate(sigma)..
-000074d0: 0a64 6566 2070 6f70 7075 7368 2878 2c20  .def poppush(x, 
-000074e0: 7661 6c29 3a0a 2020 2020 2222 224c 6566  val):.    """Lef
-000074f0: 742d 7368 6966 7420 6172 7261 7920 6f6e  t-shift array on
-00007500: 6520 706f 7369 7469 6f6e 2061 6e64 2077  e position and w
-00007510: 7269 7465 7320 6e65 7720 7661 6c75 6520  rites new value 
-00007520: 746f 2074 6865 2072 6967 6874 2e20 5265  to the right. Re
-00007530: 7475 726e 7320 6176 6572 6167 652e 0a0a  turns average...
-00007540: 2020 2020 2a2a 5061 7261 6d65 7465 7273      **Parameters
-00007550: 3a2a 2a0a 2020 2020 6060 7860 603a 206e  :**.    ``x``: n
-00007560: 756d 7079 2061 7272 6179 0a20 2020 2060  umpy array.    `
-00007570: 6076 616c 6060 3a20 696e 7420 6f72 2066  `val``: int or f
-00007580: 6c6f 6174 0a20 2020 2022 2222 0a20 2020  loat.    """.   
-00007590: 2078 5b3a 2d31 5d20 3d20 785b 313a 5d3b   x[:-1] = x[1:];
-000075a0: 2078 5b2d 315d 203d 2076 616c 0a20 2020   x[-1] = val.   
-000075b0: 2072 6574 7572 6e20 782e 6d65 616e 2829   return x.mean()
-000075c0: 0a0a 6465 6620 736f 7274 5f61 746f 6d73  ..def sort_atoms
-000075d0: 2861 746f 6d73 2c20 6b65 7920 3d20 2832  (atoms, key = (2
-000075e0: 2c31 2c30 2929 3a0a 2020 2020 2222 2252  ,1,0)):.    """R
-000075f0: 6574 7572 6e20 6174 6f6d 7320 6f62 6a65  eturn atoms obje
-00007600: 6374 2077 6974 6820 736f 7274 6564 2061  ct with sorted a
-00007610: 746f 6d69 6320 636f 6f72 6469 6e61 7465  tomic coordinate
-00007620: 730a 0a20 2020 2054 6865 2064 6566 6175  s..    The defau
-00007630: 6c74 2073 6f72 7469 6e67 2069 733a 2069  lt sorting is: i
-00007640: 6e63 7265 6173 696e 6720 7a2d 636f 6f72  ncreasing z-coor
-00007650: 6469 6e61 7465 2066 6972 7374 2c20 696e  dinate first, in
-00007660: 6372 6561 7369 6e67 0a20 2020 2079 2d63  creasing.    y-c
-00007670: 6f6f 7264 696e 6174 6520 7365 636f 6e64  oordinate second
-00007680: 2c20 696e 6372 6561 7369 6e67 2078 2d63  , increasing x-c
-00007690: 6f6f 7264 696e 6174 6520 7468 6972 642e  oordinate third.
-000076a0: 2055 7365 6675 6c20 746f 2067 6574 0a20   Useful to get. 
-000076b0: 2020 2077 656c 6c20 6f72 6465 7265 6420     well ordered 
-000076c0: 736c 6162 2073 7472 7563 7475 7265 732c  slab structures,
-000076d0: 2066 6f72 2069 6e73 7461 6e63 652e 2053   for instance. S
-000076e0: 6f72 7469 6e67 2063 616e 2062 6520 6368  orting can be ch
-000076f0: 616e 6765 640a 2020 2020 6279 2061 7070  anged.    by app
-00007700: 726f 7072 6961 7465 6c79 2073 6574 7469  ropriately setti
-00007710: 6e67 2074 6865 2060 606b 6579 6060 2061  ng the ``key`` a
-00007720: 7267 756d 656e 742c 2077 6974 6820 7468  rgument, with th
-00007730: 6520 7361 6d65 0a20 2020 2065 6666 6563  e same.    effec
-00007740: 7420 6173 2069 6e3a 3a0a 0a20 2020 2020  t as in::..     
-00007750: 2020 2066 726f 6d20 6f70 6572 6174 6f72     from operator
-00007760: 2069 6d70 6f72 7420 6974 656d 6765 7474   import itemgett
-00007770: 6572 0a20 2020 2020 2020 2073 7020 3d20  er.        sp = 
-00007780: 736f 7274 6564 2870 2c20 6b65 793d 6974  sorted(p, key=it
-00007790: 656d 6765 7474 6572 2832 2c31 2c30 2929  emgetter(2,1,0))
-000077a0: 0a0a 2020 2020 7768 6572 6520 7020 6973  ..    where p is
-000077b0: 2061 204e 7833 2061 7272 6179 206f 6620   a Nx3 array of 
-000077c0: 7665 6374 6f72 2063 6f6f 7264 696e 6174  vector coordinat
-000077d0: 6573 2e0a 2020 2020 2222 220a 2020 2020  es..    """.    
-000077e0: 6e72 7320 3d20 6174 6f6d 732e 6765 745f  nrs = atoms.get_
-000077f0: 6174 6f6d 6963 5f6e 756d 6265 7273 2829  atomic_numbers()
-00007800: 0a20 2020 2070 6f73 7320 3d20 6174 6f6d  .    poss = atom
-00007810: 732e 6765 745f 706f 7369 7469 6f6e 7328  s.get_positions(
-00007820: 290a 2020 2020 706e 203d 205b 5d0a 2020  ).    pn = [].  
-00007830: 2020 666f 7220 702c 6e20 696e 207a 6970    for p,n in zip
-00007840: 2870 6f73 732c 6e72 7329 3a0a 2020 2020  (poss,nrs):.    
-00007850: 2020 2020 706e 2e61 7070 656e 6428 5b70      pn.append([p
-00007860: 5b30 5d2c 705b 315d 2c70 5b32 5d2c 6e5d  [0],p[1],p[2],n]
-00007870: 290a 2020 2020 6672 6f6d 206f 7065 7261  ).    from opera
-00007880: 746f 7220 696d 706f 7274 2069 7465 6d67  tor import itemg
-00007890: 6574 7465 720a 2020 2020 696d 706f 7274  etter.    import
-000078a0: 206e 756d 7079 2061 7320 6e70 0a20 2020   numpy as np.   
-000078b0: 205f 706e 203d 2073 6f72 7465 6428 706e   _pn = sorted(pn
-000078c0: 2c20 6b65 793d 6974 656d 6765 7474 6572  , key=itemgetter
-000078d0: 282a 6b65 7929 290a 2020 2020 5f70 6f73  (*key)).    _pos
-000078e0: 7320 3d20 6e70 2e64 656c 6574 6528 6e70  s = np.delete(np
-000078f0: 2e61 7272 6179 285f 706e 292c 332c 3129  .array(_pn),3,1)
-00007900: 0a20 2020 205f 6e72 7320 3d20 6e70 2e64  .    _nrs = np.d
-00007910: 656c 6574 6528 6e70 2e61 7272 6179 285f  elete(np.array(_
-00007920: 706e 292c 5b30 2c31 2c32 5d2c 3129 2e66  pn),[0,1,2],1).f
-00007930: 6c61 7474 656e 2829 0a20 2020 2066 726f  latten().    fro
-00007940: 6d20 6173 6520 696d 706f 7274 2041 746f  m ase import Ato
-00007950: 6d73 0a20 2020 2072 6574 7572 6e20 4174  ms.    return At
-00007960: 6f6d 7328 706f 7369 7469 6f6e 733d 5f70  oms(positions=_p
-00007970: 6f73 732c 206e 756d 6265 7273 3d5f 6e72  oss, numbers=_nr
-00007980: 732c 2063 656c 6c3d 6174 6f6d 732e 6765  s, cell=atoms.ge
-00007990: 745f 6365 6c6c 2829 2c20 7062 633d 6174  t_cell(), pbc=at
-000079a0: 6f6d 732e 6765 745f 7062 6328 2929 0a    oms.get_pbc()).
+00000120: 7320 6373 0a66 726f 6d20 6173 652e 6275  s cs.from ase.bu
+00000130: 696c 642e 7375 7065 7263 656c 6c73 2069  ild.supercells i
+00000140: 6d70 6f72 7420 636c 6561 6e5f 6d61 7472  mport clean_matr
+00000150: 6978 2c20 6c61 7474 6963 655f 706f 696e  ix, lattice_poin
+00000160: 7473 5f69 6e5f 7375 7065 7263 656c 6c20  ts_in_supercell 
+00000170: 2320 6e65 6564 6564 2062 7920 6d61 6b65  # needed by make
+00000180: 5f73 7570 6572 6365 6c6c 0a66 726f 6d20  _supercell.from 
+00000190: 6173 6520 696d 706f 7274 2041 746f 6d73  ase import Atoms
+000001a0: 0a0a 636c 6173 7320 5375 7065 7263 656c  ..class Supercel
+000001b0: 6c45 7272 6f72 2845 7863 6570 7469 6f6e  lError(Exception
+000001c0: 293a 0a20 2020 2070 6173 730a 0a64 6566  ):.    pass..def
+000001d0: 2066 696e 646d 6178 282a 6172 6773 293a   findmax(*args):
+000001e0: 0a20 2020 2076 616c 7320 3d20 5b5d 0a20  .    vals = []. 
+000001f0: 2020 2066 6f72 2076 2069 6e20 6172 6773     for v in args
+00000200: 3a0a 2020 2020 2020 2020 6966 2068 6173  :.        if has
+00000210: 6174 7472 2876 2c22 5f5f 6c65 6e5f 5f22  attr(v,"__len__"
+00000220: 293a 0a20 2020 2020 2020 2020 2020 2076  ):.            v
+00000230: 616c 732e 6170 7065 6e64 286e 702e 616d  als.append(np.am
+00000240: 6178 2876 2929 0a20 2020 2020 2020 2065  ax(v)).        e
+00000250: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00000260: 2076 616c 732e 6170 7065 6e64 2876 290a   vals.append(v).
+00000270: 0a20 2020 2072 6574 7572 6e20 6e70 2e61  .    return np.a
+00000280: 6d61 7828 7661 6c73 290a 0a64 6566 2066  max(vals)..def f
+00000290: 696e 646d 696e 282a 6172 6773 293a 0a20  indmin(*args):. 
+000002a0: 2020 2076 616c 7320 3d20 5b5d 0a20 2020     vals = [].   
+000002b0: 2066 6f72 2076 2069 6e20 6172 6773 3a0a   for v in args:.
+000002c0: 2020 2020 2020 2020 6966 2068 6173 6174          if hasat
+000002d0: 7472 2876 2c22 5f5f 6c65 6e5f 5f22 293a  tr(v,"__len__"):
+000002e0: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+000002f0: 732e 6170 7065 6e64 286e 702e 616d 696e  s.append(np.amin
+00000300: 2876 2929 0a20 2020 2020 2020 2065 6c73  (v)).        els
+00000310: 653a 0a20 2020 2020 2020 2020 2020 2076  e:.            v
+00000320: 616c 732e 6170 7065 6e64 2876 290a 0a20  als.append(v).. 
+00000330: 2020 2072 6574 7572 6e20 6e70 2e61 6d69     return np.ami
+00000340: 6e28 7661 6c73 290a 2020 2020 2020 2020  n(vals).        
+00000350: 0a64 6566 2069 7363 6c6f 7365 2872 312c  .def isclose(r1,
+00000360: 7232 2c72 746f 6c3d 3165 2d34 293a 0a20  r2,rtol=1e-4):. 
+00000370: 2020 2022 2222 4465 7465 726d 696e 6520     """Determine 
+00000380: 7768 6574 6865 7220 7477 6f20 7665 6374  whether two vect
+00000390: 6f72 7320 6172 6520 7369 6d69 6c61 720a  ors are similar.
+000003a0: 0a20 2020 202a 2a50 6172 616d 6574 6572  .    **Parameter
+000003b0: 733a 2a2a 0a0a 2020 2020 6060 7231 2c72  s:**..    ``r1,r
+000003c0: 3260 603a 2031 4420 6172 7261 7973 206f  2``: 1D arrays o
+000003d0: 6620 696e 7465 6765 7220 6f72 2066 6c6f  f integer or flo
+000003e0: 6174 0a20 2020 2020 2020 2056 6563 746f  at.        Vecto
+000003f0: 7273 2074 6f20 6265 2063 6f6d 7061 7265  rs to be compare
+00000400: 640a 2020 2020 6060 7274 6f6c 6060 3a20  d.    ``rtol``: 
+00000410: 666c 6f61 740a 2020 2020 2020 2020 546f  float.        To
+00000420: 6c65 7261 6e63 652e 0a0a 2020 2020 2a2a  lerance...    **
+00000430: 5265 7475 726e 733a 2a2a 0a0a 2020 2020  Returns:**..    
+00000440: 426f 6f6c 6561 6e3a 2069 6620 7468 6520  Boolean: if the 
+00000450: 6575 636c 6964 6561 6e20 6469 7374 616e  euclidean distan
+00000460: 6365 2062 6574 7765 656e 2060 6072 3160  ce between ``r1`
+00000470: 6020 616e 6420 6060 7232 6060 2069 7320  ` and ``r2`` is 
+00000480: 736d 616c 6c65 7220 7468 616e 0a20 2020  smaller than.   
+00000490: 2060 6072 746f 6c60 602c 2060 6054 7275   ``rtol``, ``Tru
+000004a0: 6560 6020 6973 2072 6574 7572 6e65 642c  e`` is returned,
+000004b0: 206f 7468 6572 7769 7365 2060 6046 616c   otherwise ``Fal
+000004c0: 7365 6060 2069 7320 7265 7475 726e 6564  se`` is returned
+000004d0: 2e0a 2020 2020 2222 220a 2020 2020 7472  ..    """.    tr
+000004e0: 793a 0a20 2020 2020 2020 2069 6620 6c65  y:.        if le
+000004f0: 6e28 7231 2920 213d 206c 656e 2872 3229  n(r1) != len(r2)
+00000500: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00000510: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
+00000520: 2020 2072 6574 7572 6e20 6e70 2e6c 696e     return np.lin
+00000530: 616c 672e 6e6f 726d 286e 702e 7375 6274  alg.norm(np.subt
+00000540: 7261 6374 2872 312c 7232 2929 203c 2072  ract(r1,r2)) < r
+00000550: 746f 6c0a 2020 2020 6578 6365 7074 3a0a  tol.    except:.
+00000560: 2020 2020 2020 2020 7265 7475 726e 206e          return n
+00000570: 702e 6c69 6e61 6c67 2e6e 6f72 6d28 6e70  p.linalg.norm(np
+00000580: 2e73 7562 7472 6163 7428 7231 2c72 3229  .subtract(r1,r2)
+00000590: 2920 3c20 7274 6f6c 0a0a 0a64 6566 2064  ) < rtol...def d
+000005a0: 6963 745f 636f 6d70 6172 6528 6431 2c20  ict_compare(d1, 
+000005b0: 6432 2c20 746f 6c3d 4e6f 6e65 293a 0a20  d2, tol=None):. 
+000005c0: 2020 2022 2222 436f 6d70 6172 6520 7477     """Compare tw
+000005d0: 6f20 6469 6374 696f 6e61 7269 6573 2063  o dictionaries c
+000005e0: 6f6e 7461 696e 696e 6720 6d75 7461 626c  ontaining mutabl
+000005f0: 6520 6f62 6a65 6374 732e 0a0a 2020 2020  e objects...    
+00000600: 5468 6973 2063 6f6d 7061 7265 7320 7477  This compares tw
+00000610: 6f20 6469 6374 696f 6e61 7269 6573 2e20  o dictionaries. 
+00000620: 5477 6f20 6469 6374 696f 6e61 7269 6573  Two dictionaries
+00000630: 2061 7265 2063 6f6e 7369 6465 7265 6420   are considered 
+00000640: 6571 7561 6c0a 2020 2020 6576 656e 2069  equal.    even i
+00000650: 6620 7468 6520 706f 7369 7469 6f6e 206f  f the position o
+00000660: 6620 6b65 7973 2064 6966 6665 722e 2048  f keys differ. H
+00000670: 616e 646c 6573 206d 7574 6162 6c65 2076  andles mutable v
+00000680: 616c 7565 7320 696e 2074 6865 2064 6963  alues in the dic
+00000690: 742e 0a20 2020 2053 6f6d 6520 7061 7274  t..    Some part
+000006a0: 7320 6172 6520 7461 6b65 6e20 6672 6f6d  s are taken from
+000006b0: 3a0a 0a20 2020 2068 7474 7073 3a2f 2f73  :..    https://s
+000006c0: 7461 636b 6f76 6572 666c 6f77 2e63 6f6d  tackoverflow.com
+000006d0: 2f71 7565 7374 696f 6e73 2f34 3532 3739  /questions/45279
+000006e0: 3432 2f63 6f6d 7061 7269 6e67 2d74 776f  42/comparing-two
+000006f0: 2d64 6963 7469 6f6e 6172 6965 732d 696e  -dictionaries-in
+00000700: 2d70 7974 686f 6e0a 0a20 2020 202a 2a50  -python..    **P
+00000710: 6172 616d 6574 6572 733a 2a2a 0a0a 2020  arameters:**..  
+00000720: 2020 6060 6431 2c64 3260 603a 2070 7974    ``d1,d2``: pyt
+00000730: 686f 6e20 6469 6374 696f 6e61 7269 6573  hon dictionaries
+00000740: 0a20 2020 2020 2020 2064 6963 7469 6f6e  .        diction
+00000750: 6172 6965 7320 746f 2062 6520 636f 6d70  aries to be comp
+00000760: 6172 6564 0a0a 2020 2020 6060 746f 6c60  ared..    ``tol`
+00000770: 603a 2066 6c6f 6174 0a20 2020 2020 2020  `: float.       
+00000780: 2061 2073 6d61 6c6c 2066 6c6f 6174 206e   a small float n
+00000790: 756d 6265 722e 2049 6620 6e6f 7420 6060  umber. If not ``
+000007a0: 4e6f 6e65 6060 2c20 7468 6520 636f 6d70  None``, the comp
+000007b0: 6172 6973 6f6e 206f 6620 6469 6374 696f  arison of dictio
+000007c0: 6e61 7279 0a20 2020 2020 2020 2076 616c  nary.        val
+000007d0: 7565 7320 6973 2072 6567 6172 6465 6420  ues is regarded 
+000007e0: 6173 2061 2076 6563 746f 7220 636f 6d70  as a vector comp
+000007f0: 6172 6973 6f6e 2061 6e64 2064 6f6e 6520  arison and done 
+00000800: 7769 7468 0a20 2020 2020 2020 2060 6075  with.        ``u
+00000810: 7469 6c73 2e69 7363 6c6f 7365 2829 6060  tils.isclose()``
+00000820: 2e20 466f 7220 7468 6520 6d65 616e 696e  . For the meanin
+00000830: 6720 6f66 2060 6074 6f6c 6060 2c20 7265  g of ``tol``, re
+00000840: 6164 2074 6865 2064 6f63 756d 656e 7461  ad the documenta
+00000850: 7469 6f6e 0a20 2020 2020 2020 2066 6f72  tion.        for
+00000860: 2060 6072 746f 6c60 6020 7061 7261 6d65   ``rtol`` parame
+00000870: 7465 7220 6f66 2060 6075 7469 6c73 2e69  ter of ``utils.i
+00000880: 7363 6c6f 7365 2829 6060 2e0a 0a20 2020  sclose()``...   
+00000890: 2052 6574 7572 6e3a 2062 6f6f 6c65 616e   Return: boolean
+000008a0: 0a20 2020 2020 2020 2060 6054 7275 6560  .        ``True`
+000008b0: 6020 6966 2064 6963 7473 2061 7265 2065  ` if dicts are e
+000008c0: 7175 616c 2c20 6060 4661 6c73 6560 6020  qual, ``False`` 
+000008d0: 6966 2074 6865 7920 6172 6520 6469 6666  if they are diff
+000008e0: 6572 656e 742e 0a20 2020 2022 2222 0a20  erent..    """. 
+000008f0: 2020 2061 7265 6571 203d 2054 7275 650a     areeq = True.
+00000900: 0a20 2020 2069 6620 6c65 6e28 6431 2920  .    if len(d1) 
+00000910: 213d 206c 656e 2864 3229 3a0a 2020 2020  != len(d2):.    
+00000920: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+00000930: 0a0a 2020 2020 6431 5f6b 6579 7320 3d20  ..    d1_keys = 
+00000940: 7365 7428 6431 2e6b 6579 7328 2929 0a20  set(d1.keys()). 
+00000950: 2020 2064 325f 6b65 7973 203d 2073 6574     d2_keys = set
+00000960: 2864 322e 6b65 7973 2829 290a 2020 2020  (d2.keys()).    
+00000970: 696e 7465 7273 6563 745f 6b65 7973 203d  intersect_keys =
+00000980: 2064 315f 6b65 7973 2e69 6e74 6572 7365   d1_keys.interse
+00000990: 6374 696f 6e28 6432 5f6b 6579 7329 0a20  ction(d2_keys). 
+000009a0: 2020 2069 6620 6c65 6e28 6431 2920 213d     if len(d1) !=
+000009b0: 206c 656e 2869 6e74 6572 7365 6374 5f6b   len(intersect_k
+000009c0: 6579 7329 3a0a 2020 2020 2020 2020 7265  eys):.        re
+000009d0: 7475 726e 2046 616c 7365 0a0a 2020 2020  turn False..    
+000009e0: 666f 7220 6b20 696e 2064 315f 6b65 7973  for k in d1_keys
+000009f0: 3a0a 2020 2020 2020 2020 7472 793a 0a20  :.        try:. 
+00000a00: 2020 2020 2020 2020 2020 2066 6f72 2076             for v
+00000a10: 312c 7632 2069 6e20 7a69 7028 6431 5b6b  1,v2 in zip(d1[k
+00000a20: 5d2c 6432 5b6b 5d29 3a0a 2020 2020 2020  ],d2[k]):.      
+00000a30: 2020 2020 2020 2020 2020 6966 2028 6973            if (is
+00000a40: 696e 7374 616e 6365 2876 312c 206c 6973  instance(v1, lis
+00000a50: 7429 2920 6f72 2028 6973 696e 7374 616e  t)) or (isinstan
+00000a60: 6365 2876 312c 6e70 2e6e 6461 7272 6179  ce(v1,np.ndarray
+00000a70: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+00000a80: 2020 2020 2020 2020 666f 7220 692c 7620          for i,v 
+00000a90: 696e 2065 6e75 6d65 7261 7465 2876 3129  in enumerate(v1)
+00000aa0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00000ab0: 2020 2020 2020 2020 2020 6966 2074 6f6c            if tol
+00000ac0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00000ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ae0: 2020 2020 2020 6966 2076 2021 3d20 7632        if v != v2
+00000af0: 5b69 5d3a 0a20 2020 2020 2020 2020 2020  [i]:.           
+00000b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b10: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00000b20: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00000b30: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00000b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b50: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00000b60: 6f74 2069 7363 6c6f 7365 2876 202c 7632  ot isclose(v ,v2
+00000b70: 5b69 5d2c 2074 6f6c 293a 0a20 2020 2020  [i], tol):.     
+00000b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b90: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00000ba0: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
+00000bb0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00000bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000bd0: 2020 6966 2074 6f6c 2069 7320 4e6f 6e65    if tol is None
+00000be0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00000bf0: 2020 2020 2020 2020 2020 6966 2076 3120            if v1 
+00000c00: 213d 2076 323a 0a20 2020 2020 2020 2020  != v2:.         
+00000c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c20: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+00000c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c40: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00000c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c60: 2020 6966 206e 6f74 2069 7363 6c6f 7365    if not isclose
+00000c70: 2876 312c 7632 2c74 6f6c 293a 0a20 2020  (v1,v2,tol):.   
+00000c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c90: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00000ca0: 4661 6c73 650a 0a20 2020 2020 2020 2065  False..        e
+00000cb0: 7863 6570 7420 5479 7065 4572 726f 723a  xcept TypeError:
+00000cc0: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
+00000cd0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00000ce0: 2020 6966 205f 6973 5f69 6e74 6567 7261    if _is_integra
+00000cf0: 626c 6528 6431 5b6b 5d29 3a0a 2020 2020  ble(d1[k]):.    
+00000d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d10: 6966 206e 6f74 2069 7363 6c6f 7365 2864  if not isclose(d
+00000d20: 315b 6b5d 2c64 325b 6b5d 2c74 6f6c 293a  1[k],d2[k],tol):
+00000d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000d40: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00000d50: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
+00000d60: 2020 6578 6365 7074 3a0a 2020 2020 2020    except:.      
+00000d70: 2020 2020 2020 2020 2020 6966 2074 7970            if typ
+00000d80: 6528 6431 5b6b 5d29 2069 7320 6469 6374  e(d1[k]) is dict
+00000d90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00000da0: 2020 2020 2020 666f 7220 7375 626b 6579        for subkey
+00000db0: 7320 696e 2064 315b 6b5d 2e6b 6579 7328  s in d1[k].keys(
+00000dc0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00000dd0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00000de0: 7420 6973 636c 6f73 6528 6431 5b6b 5d5b  t isclose(d1[k][
+00000df0: 7375 626b 6579 735d 2c64 325b 6b5d 5b73  subkeys],d2[k][s
+00000e00: 7562 6b65 7973 5d2c 746f 6c29 3a0a 2020  ubkeys],tol):.  
+00000e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e20: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00000e30: 2046 616c 7365 0a0a 2020 2020 7265 7475   False..    retu
+00000e40: 726e 2061 7265 6571 0a0a 0a64 6566 2073  rn areeq...def s
+00000e50: 7562 5f66 6f6c 6465 7273 2872 6f6f 7429  ub_folders(root)
+00000e60: 3a0a 2020 2020 2222 2252 6574 7572 6e20  :.    """Return 
+00000e70: 6c69 7374 206f 6620 7375 6266 6f6c 6465  list of subfolde
+00000e80: 7273 0a0a 2020 2020 5061 7261 6d65 7465  rs..    Paramete
+00000e90: 7273 3a0a 0a20 2020 2072 6f6f 743a 2073  rs:..    root: s
+00000ea0: 7472 696e 670a 2020 2020 2020 2020 7061  tring.        pa
+00000eb0: 7468 206f 6620 7468 6520 6162 736f 6c75  th of the absolu
+00000ec0: 7465 2066 6f6c 6465 7220 666f 7220 7768  te folder for wh
+00000ed0: 6963 6820 796f 7520 7761 6e74 2074 6f20  ich you want to 
+00000ee0: 6765 7420 7468 6520 6c69 7374 206f 660a  get the list of.
+00000ef0: 2020 2020 2020 2020 7375 6266 6f6c 6465          subfolde
+00000f00: 7273 2e0a 2020 2020 2222 220a 2020 2020  rs..    """.    
+00000f10: 2372 6574 7572 6e20 6f73 2e77 616c 6b28  #return os.walk(
+00000f20: 726f 6f74 292e 6e65 7874 2829 5b31 5d20  root).next()[1] 
+00000f30: 2370 7974 686f 6e20 322e 370a 2020 2020  #python 2.7.    
+00000f40: 7265 7475 726e 206e 6578 7428 6f73 2e77  return next(os.w
+00000f50: 616c 6b28 726f 6f74 2929 5b31 5d0a 0a64  alk(root))[1]..d
+00000f60: 6566 205f 6973 5f69 6e74 6567 7261 626c  ef _is_integrabl
+00000f70: 6528 7329 3a0a 2020 2020 2222 2244 6574  e(s):.    """Det
+00000f80: 6572 6d69 6e65 2077 6865 7468 6572 2061  ermine whether a
+00000f90: 7267 756d 656e 7420 6973 2069 6e74 6567  rgument is integ
+00000fa0: 6572 206f 7220 6361 6e20 6265 2063 6f6e  er or can be con
+00000fb0: 7665 7274 6564 2074 6f20 696e 7465 6765  verted to intege
+00000fc0: 720a 0a20 2020 2050 6172 616d 6574 6572  r..    Parameter
+00000fd0: 733a 0a0a 2020 2020 733a 206f 626a 6563  s:..    s: objec
+00000fe0: 740a 2020 2020 2020 2020 4361 6e20 6265  t.        Can be
+00000ff0: 2061 6e79 206f 626a 6563 7420 666f 7220   any object for 
+00001000: 7768 6963 6820 7765 2077 616e 7420 746f  which we want to
+00001010: 2064 6574 6572 6d69 6e65 2077 6865 7468   determine wheth
+00001020: 6572 2069 7320 696e 7465 6765 7220 6f72  er is integer or
+00001030: 0a20 2020 2020 2020 2063 616e 2062 6520  .        can be 
+00001040: 636f 6e76 6572 7465 6420 746f 2069 6e74  converted to int
+00001050: 6567 6572 2e0a 2020 2020 2222 220a 2020  eger..    """.  
+00001060: 2020 7472 793a 0a20 2020 2020 2020 2069    try:.        i
+00001070: 6e74 2873 290a 2020 2020 2020 2020 7265  nt(s).        re
+00001080: 7475 726e 2054 7275 650a 2020 2020 6578  turn True.    ex
+00001090: 6365 7074 2056 616c 7565 4572 726f 723a  cept ValueError:
+000010a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000010b0: 4661 6c73 650a 0a64 6566 206c 6973 745f  False..def list_
+000010c0: 696e 7465 6765 725f 6e61 6d65 645f 666f  integer_named_fo
+000010d0: 6c64 6572 7328 726f 6f74 3d22 2e22 2c20  lders(root=".", 
+000010e0: 7072 6566 6978 3d27 272c 2073 7566 6669  prefix='', suffi
+000010f0: 783d 2727 2c20 636f 6e74 6169 6e69 6e67  x='', containing
+00001100: 5f66 696c 6573 3d5b 5d2c 206e 6f74 5f63  _files=[], not_c
+00001110: 6f6e 7461 696e 696e 675f 6669 6c65 733d  ontaining_files=
+00001120: 5b5d 293a 0a20 2020 2022 2222 5265 7475  []):.    """Retu
+00001130: 726e 2061 7272 6179 206f 6620 696e 7465  rn array of inte
+00001140: 6765 7220 6e61 6d65 6420 666f 6c64 6572  ger named folder
+00001150: 732e 0a0a 2020 2020 5363 616e 7320 666f  s...    Scans fo
+00001160: 6c64 6572 7320 696e 2060 6072 6f6f 7460  lders in ``root`
+00001170: 6020 616e 6420 6465 7465 6374 7320 7468  ` and detects th
+00001180: 6f73 6520 7768 6963 6820 6172 6520 6e61  ose which are na
+00001190: 6d65 640a 2020 2020 7769 7468 2061 6e20  med.    with an 
+000011a0: 696e 7465 6765 7220 6e75 6d62 6572 2e20  integer number. 
+000011b0: 4974 2072 6574 7572 6e73 2074 6865 6e20  It returns then 
+000011c0: 6120 736f 7274 6564 206c 6973 7420 6f66  a sorted list of
+000011d0: 2074 6865 0a20 2020 2066 6f75 6e64 2069   the.    found i
+000011e0: 6e74 6567 6572 732c 2065 2e67 2e20 2c20  ntegers, e.g. , 
+000011f0: 6966 2074 6865 2066 6f6c 6465 7220 7374  if the folder st
+00001200: 7275 6374 7572 6520 6973 3a3a 0a0a 2020  ructure is::..  
+00001210: 2020 2020 2020 726f 6f74 2f0a 2020 2020        root/.    
+00001220: 2020 2020 2020 2020 312f 0a20 2020 2020          1/.     
+00001230: 2020 2020 2020 2032 2f0a 2020 2020 2020         2/.      
+00001240: 2020 2020 2020 352f 0a20 2020 2020 2020        5/.       
+00001250: 2020 2020 2037 2f0a 2020 2020 2020 2020       7/.        
+00001260: 2020 2020 382f 0a20 2020 2020 2020 2020      8/.         
+00001270: 2020 2072 756e 5f32 2f0a 2020 2020 2020     run_2/.      
+00001280: 2020 2020 2020 7275 6e5f 332f 0a20 2020        run_3/.   
+00001290: 2020 2020 2020 2020 2072 756e 5f34 2f0a           run_4/.
+000012a0: 2020 2020 2020 2020 2020 2020 7275 6e5f              run_
+000012b0: 352f 0a20 2020 2020 2020 2020 2020 2072  5/.            r
+000012c0: 756e 5f6f 6c64 2f0a 2020 2020 2020 2020  un_old/.        
+000012d0: 2020 2020 666f 6c64 6572 782f 0a20 2020      folderx/.   
+000012e0: 2020 2020 2020 2020 2066 6f6c 6465 7279           foldery
+000012f0: 2f0a 0a0a 2020 2020 7468 656e 2074 6865  /...    then the
+00001300: 2066 6f6c 6c6f 7769 6e67 2061 7272 6179   following array
+00001310: 2069 7320 7265 7475 726e 6564 3a3a 0a0a   is returned::..
+00001320: 2020 2020 2020 2020 5b31 2c32 2c35 2c37          [1,2,5,7
+00001330: 2c38 5d2e 0a0a 2020 2020 4966 2060 6070  ,8]...    If ``p
+00001340: 7265 6669 7860 6020 6973 2073 6574 2074  refix`` is set t
+00001350: 6f20 736f 6d65 2073 7472 696e 672c 2074  o some string, t
+00001360: 6865 6e20 6974 2072 6574 7572 6e73 2061  hen it returns a
+00001370: 2028 736f 7274 6564 290a 2020 2020 6c69   (sorted).    li
+00001380: 7374 206f 6620 7374 7269 6e67 732e 2046  st of strings. F
+00001390: 6f72 2065 7861 6d70 6c65 2c20 6966 2070  or example, if p
+000013a0: 7265 6669 7820 6973 2073 6574 2074 6f20  refix is set to 
+000013b0: 6060 2272 756e 5f22 6060 2c20 7468 656e  ``"run_"``, then
+000013c0: 2074 6869 730a 2020 2020 7769 6c6c 2072   this.    will r
+000013d0: 6574 7572 6e20 7468 6520 6172 7261 793a  eturn the array:
+000013e0: 3a0a 0a20 2020 2020 2020 205b 2272 756e  :..        ["run
+000013f0: 5f32 222c 2272 756e 5f33 222c 2272 756e  _2","run_3","run
+00001400: 5f34 222c 2272 756e 5f35 225d 0a0a 2020  _4","run_5"]..  
+00001410: 2020 5061 7261 6d65 7465 7273 3a0a 0a20    Parameters:.. 
+00001420: 2020 2060 6072 6f6f 7460 603a 2073 7472     ``root``: str
+00001430: 696e 670a 2020 2020 2020 2020 7061 7468  ing.        path
+00001440: 206f 6620 7468 6520 726f 6f74 2066 6f6c   of the root fol
+00001450: 6465 7220 696e 2077 6869 6368 2074 6f20  der in which to 
+00001460: 7363 616e 2066 6f72 2069 6e74 6567 6572  scan for integer
+00001470: 206e 616d 6564 2066 6f6c 6465 7273 2e0a   named folders..
+00001480: 2020 2020 6060 7072 6566 6978 6060 3a20      ``prefix``: 
+00001490: 7374 7269 6e67 0a20 2020 2020 2020 2073  string.        s
+000014a0: 6361 6e20 666f 7220 666f 6c64 6572 7320  can for folders 
+000014b0: 7768 6f73 6520 6e61 6d65 2073 7461 7274  whose name start
+000014c0: 7320 7769 7468 2074 6865 2073 7472 696e  s with the strin
+000014d0: 6720 6060 7072 6566 6978 6060 2066 6f6c  g ``prefix`` fol
+000014e0: 6c6f 7765 640a 2020 2020 2020 2020 6279  lowed.        by
+000014f0: 2061 6e64 2069 6e74 6567 6572 206e 756d   and integer num
+00001500: 6265 7220 2861 6e64 2070 6f73 7369 626c  ber (and possibl
+00001510: 7920 7468 6520 7374 7269 6e67 2060 6073  y the string ``s
+00001520: 7566 6669 7860 6029 2e0a 2020 2020 6060  uffix``)..    ``
+00001530: 7375 6666 6978 6060 3a20 7374 7269 6e67  suffix``: string
+00001540: 0a20 2020 2020 2020 2073 6361 6e20 666f  .        scan fo
+00001550: 7220 666f 6c64 6572 7320 7768 6f73 6520  r folders whose 
+00001560: 6e61 6d65 2065 6e64 7320 7769 7468 2074  name ends with t
+00001570: 6865 2073 7472 696e 6720 6060 7375 6666  he string ``suff
+00001580: 6978 6060 2061 6e64 0a20 2020 2020 2020  ix`` and.       
+00001590: 2069 7320 7072 6563 6564 6564 2062 7920   is preceded by 
+000015a0: 616e 2069 6e74 6567 6572 206e 756d 6265  an integer numbe
+000015b0: 7220 2861 6e64 2070 6f73 7369 626c 7920  r (and possibly 
+000015c0: 7468 6520 7374 7269 6e67 2060 6070 7265  the string ``pre
+000015d0: 6669 7860 6029 2e0a 2020 2020 6060 636f  fix``)..    ``co
+000015e0: 6e74 6169 6e69 6e67 5f66 696c 6573 6060  ntaining_files``
+000015f0: 3a20 6172 7261 7920 6f66 2073 7472 696e  : array of strin
+00001600: 6773 0a20 2020 2020 2020 2061 206c 6973  gs.        a lis
+00001610: 7420 6f66 2066 696c 6520 6e61 6d65 7320  t of file names 
+00001620: 7468 6174 2073 686f 756c 6420 6265 2063  that should be c
+00001630: 6f6e 7461 696e 6564 2069 6e20 7468 6520  ontained in the 
+00001640: 7265 7475 726e 6564 2066 6f6c 6465 7273  returned folders
+00001650: 2e0a 2020 2020 6060 6e6f 745f 636f 6e74  ..    ``not_cont
+00001660: 6169 6e69 6e67 5f66 696c 6573 6060 3a20  aining_files``: 
+00001670: 6172 7261 7920 6f66 2073 7472 696e 6773  array of strings
+00001680: 0a20 2020 2020 2020 2061 206c 6973 7420  .        a list 
+00001690: 6f66 2066 696c 6520 6e61 6d65 7320 7468  of file names th
+000016a0: 6174 2073 686f 756c 6420 6e6f 7420 6265  at should not be
+000016b0: 2063 6f6e 7461 696e 6564 2069 6e20 7468   contained in th
+000016c0: 6520 7265 7475 726e 6564 2066 6f6c 6465  e returned folde
+000016d0: 7273 2e0a 0a20 2020 2052 6574 7572 6e73  rs...    Returns
+000016e0: 3a0a 2020 2020 2020 2020 6172 7261 7920  :.        array 
+000016f0: 6f66 2069 6e74 6567 6572 7320 6966 2064  of integers if d
+00001700: 6566 6175 6c74 2076 616c 7565 2066 6f72  efault value for
+00001710: 2060 6070 7265 6669 7860 6020 6973 2075   ``prefix`` is u
+00001720: 7365 642e 204f 7468 6572 7769 7365 0a20  sed. Otherwise. 
+00001730: 2020 2020 2020 2072 6574 7572 6e73 2061         returns a
+00001740: 6e20 6172 7261 7920 6f66 2073 7472 696e  n array of strin
+00001750: 6773 0a0a 2020 2020 2222 220a 2020 2020  gs..    """.    
+00001760: 666f 6c64 6572 7320 3d20 7375 625f 666f  folders = sub_fo
+00001770: 6c64 6572 7328 726f 6f74 290a 0a20 2020  lders(root)..   
+00001780: 2066 6c69 7374 203d 205b 5d0a 2020 2020   flist = [].    
+00001790: 666f 7220 666f 6c64 6572 2069 6e20 666f  for folder in fo
+000017a0: 6c64 6572 733a 0a20 2020 2020 2020 2069  lders:.        i
+000017b0: 6e63 6c75 6465 203d 2054 7275 650a 2020  nclude = True.  
+000017c0: 2020 2020 2020 666f 7220 666e 2069 6e20        for fn in 
+000017d0: 6e6f 745f 636f 6e74 6169 6e69 6e67 5f66  not_containing_f
+000017e0: 696c 6573 3a0a 2020 2020 2020 2020 2020  iles:.          
+000017f0: 2020 6966 206f 732e 7061 7468 2e65 7869    if os.path.exi
+00001800: 7374 7328 6f73 2e70 6174 682e 6a6f 696e  sts(os.path.join
+00001810: 2872 6f6f 742c 666f 6c64 6572 2c66 6e29  (root,folder,fn)
+00001820: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00001830: 2020 2069 6e63 6c75 6465 203d 2046 616c     include = Fal
+00001840: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
+00001850: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
+00001860: 2069 6620 6e6f 7420 696e 636c 7564 653a   if not include:
+00001870: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+00001880: 7469 6e75 650a 0a20 2020 2020 2020 2066  tinue..        f
+00001890: 6f72 2066 6e20 696e 2063 6f6e 7461 696e  or fn in contain
+000018a0: 696e 675f 6669 6c65 733a 0a20 2020 2020  ing_files:.     
+000018b0: 2020 2020 2020 2069 6620 6e6f 7420 6f73         if not os
+000018c0: 2e70 6174 682e 6578 6973 7473 286f 732e  .path.exists(os.
+000018d0: 7061 7468 2e6a 6f69 6e28 726f 6f74 2c66  path.join(root,f
+000018e0: 6f6c 6465 722c 666e 2929 3a0a 2020 2020  older,fn)):.    
+000018f0: 2020 2020 2020 2020 2020 2020 696e 636c              incl
+00001900: 7564 6520 3d20 4661 6c73 650a 2020 2020  ude = False.    
+00001910: 2020 2020 2020 2020 2020 2020 6272 6561              brea
+00001920: 6b0a 2020 2020 2020 2020 6966 206e 6f74  k.        if not
+00001930: 2069 6e63 6c75 6465 3a0a 2020 2020 2020   include:.      
+00001940: 2020 2020 2020 636f 6e74 696e 7565 0a0a        continue..
+00001950: 2020 2020 2020 2020 6966 2070 7265 6669          if prefi
+00001960: 7820 3d3d 2066 6f6c 6465 725b 3a6c 656e  x == folder[:len
+00001970: 2870 7265 6669 7829 5d20 616e 6420 7375  (prefix)] and su
+00001980: 6666 6978 203d 3d20 666f 6c64 6572 5b2d  ffix == folder[-
+00001990: 6c65 6e28 7375 6666 6978 293a 5d3a 0a20  len(suffix):]:. 
+000019a0: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+000019b0: 6e28 7072 6566 6978 2920 213d 2030 2061  n(prefix) != 0 a
+000019c0: 6e64 206c 656e 2873 7566 6669 7829 2021  nd len(suffix) !
+000019d0: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+000019e0: 2020 2020 2064 203d 2066 6f6c 6465 725b       d = folder[
+000019f0: 6c65 6e28 7072 6566 6978 293a 5d5b 3a2d  len(prefix):][:-
+00001a00: 6c65 6e28 7375 6666 6978 295d 0a20 2020  len(suffix)].   
+00001a10: 2020 2020 2020 2020 2065 6c69 6620 6c65           elif le
+00001a20: 6e28 7072 6566 6978 2920 213d 2030 2061  n(prefix) != 0 a
+00001a30: 6e64 206c 656e 2873 7566 6669 7829 203d  nd len(suffix) =
+00001a40: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+00001a50: 2020 2020 2064 203d 2066 6f6c 6465 725b       d = folder[
+00001a60: 6c65 6e28 7072 6566 6978 293a 5d0a 2020  len(prefix):].  
+00001a70: 2020 2020 2020 2020 2020 656c 6966 206c            elif l
+00001a80: 656e 2870 7265 6669 7829 203d 3d20 3020  en(prefix) == 0 
+00001a90: 616e 6420 6c65 6e28 7375 6666 6978 2920  and len(suffix) 
+00001aa0: 213d 2030 3a0a 2020 2020 2020 2020 2020  != 0:.          
+00001ab0: 2020 2020 2020 6420 3d20 666f 6c64 6572        d = folder
+00001ac0: 5b3a 2d6c 656e 2873 7566 6669 7829 5d0a  [:-len(suffix)].
+00001ad0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00001ae0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00001af0: 2020 6420 3d20 666f 6c64 6572 5b3a 5d0a    d = folder[:].
+00001b00: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00001b10: 5f69 735f 696e 7465 6772 6162 6c65 2864  _is_integrable(d
+00001b20: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00001b30: 2020 2066 6c69 7374 2e61 7070 656e 6428     flist.append(
+00001b40: 696e 7428 6429 290a 2020 2020 2020 2020  int(d)).        
+00001b50: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00001b60: 2020 6966 205f 6973 5f69 6e74 6567 7261    if _is_integra
+00001b70: 626c 6528 666f 6c64 6572 293a 0a20 2020  ble(folder):.   
+00001b80: 2020 2020 2020 2020 2020 2020 2066 6c69               fli
+00001b90: 7374 2e61 7070 656e 6428 696e 7428 666f  st.append(int(fo
+00001ba0: 6c64 6572 2929 0a0a 2020 2020 666c 6973  lder))..    flis
+00001bb0: 742e 736f 7274 2829 0a0a 2020 2020 6966  t.sort()..    if
+00001bc0: 2070 7265 6669 7820 213d 2027 2720 6f72   prefix != '' or
+00001bd0: 2073 7566 6669 7820 213d 2027 273a 0a20   suffix != '':. 
+00001be0: 2020 2020 2020 2073 6c69 7374 203d 205b         slist = [
+00001bf0: 5d0a 2020 2020 2020 2020 666f 7220 6620  ].        for f 
+00001c00: 696e 2066 6c69 7374 3a0a 2020 2020 2020  in flist:.      
+00001c10: 2020 2020 2020 736c 6973 742e 6170 7065        slist.appe
+00001c20: 6e64 2870 7265 6669 7820 2b20 7374 7228  nd(prefix + str(
+00001c30: 6629 202b 2073 7566 6669 7829 0a0a 2020  f) + suffix)..  
+00001c40: 2020 2020 2020 7265 7475 726e 2073 6c69        return sli
+00001c50: 7374 0a0a 2020 2020 656c 7365 3a0a 2020  st..    else:.  
+00001c60: 2020 2020 2020 7265 7475 726e 2066 6c69        return fli
+00001c70: 7374 0a0a 0a0a 6465 6620 6174 6174 5f74  st....def atat_t
+00001c80: 6f5f 6365 6c6c 2866 696c 655f 7061 7468  o_cell(file_path
+00001c90: 3d22 6c61 742e 696e 222c 2069 6e74 6572  ="lat.in", inter
+00001ca0: 7072 6574 5f61 733d 2270 6172 656e 745f  pret_as="parent_
+00001cb0: 6c61 7474 6963 6522 2c20 7061 7265 6e74  lattice", parent
+00001cc0: 5f6c 6174 7469 6365 3d4e 6f6e 652c 7062  _lattice=None,pb
+00001cd0: 633d 4e6f 6e65 2c77 7261 703d 5472 7565  c=None,wrap=True
+00001ce0: 293a 0a20 2020 2022 2222 5061 7273 6520  ):.    """Parse 
+00001cf0: 6120 6060 6c61 742e 696e 6060 206f 7220  a ``lat.in`` or 
+00001d00: 6060 7374 722e 6f75 7460 6020 6669 6c65  ``str.out`` file
+00001d10: 2066 726f 6d20 6060 4154 4154 6060 2e0a   from ``ATAT``..
+00001d20: 0a20 2020 2060 6041 5441 5460 6020 7573  .    ``ATAT`` us
+00001d30: 6572 7320 6d61 7920 7573 6520 7468 6520  ers may use the 
+00001d40: 696e 7075 7420 6669 6c65 7320 6672 6f6d  input files from
+00001d50: 2060 6041 5441 5460 6020 746f 2070 6572   ``ATAT`` to per
+00001d60: 666f 726d 2061 2063 6c75 7374 6572 0a20  form a cluster. 
+00001d70: 2020 2065 7870 616e 7369 6f6e 2077 6974     expansion wit
+00001d80: 6820 2a2a 4345 4c4c 2a2a 2e20 5468 6973  h **CELL**. This
+00001d90: 2066 756e 6374 696f 6e20 616c 6c6f 7773   function allows
+00001da0: 2074 6f20 636f 6e76 6572 7420 616e 2069   to convert an i
+00001db0: 6e70 7574 2060 606c 6174 2e69 6e60 600a  nput ``lat.in``.
+00001dc0: 2020 2020 6669 6c65 2066 726f 6d20 6060      file from ``
+00001dd0: 4154 4154 6060 2074 6f20 6120 6060 5061  ATAT`` to a ``Pa
+00001de0: 7265 6e74 4c61 7474 6963 6560 6020 6f62  rentLattice`` ob
+00001df0: 6a65 6374 2069 6e20 4345 4c4c 2e20 4f6e  ject in CELL. On
+00001e00: 6520 6d61 7920 616c 736f 2072 6561 640a  e may also read.
+00001e10: 2020 2020 6060 7374 722e 6f75 7460 6020      ``str.out`` 
+00001e20: 6669 6c65 732c 2077 6869 6368 2061 7265  files, which are
+00001e30: 2063 6f6e 7665 7274 6564 2074 6f20 6060   converted to ``
+00001e40: 5374 7275 6374 7572 6560 6020 6f62 6a65  Structure`` obje
+00001e50: 6374 7320 696e 2060 6043 454c 4c60 602e  cts in ``CELL``.
+00001e60: 0a0a 2020 2020 2a2a 5061 7261 6d65 7465  ..    **Paramete
+00001e70: 7273 3a2a 2a0a 0a20 2020 2060 6066 696c  rs:**..    ``fil
+00001e80: 655f 7061 7468 6060 3a20 7374 7269 6e67  e_path``: string
+00001e90: 0a20 2020 2020 2020 2073 7472 696e 6720  .        string 
+00001ea0: 636f 6e74 6169 6e69 6e67 2074 6865 2070  containing the p
+00001eb0: 6174 6820 6f66 2074 6865 2066 696c 6520  ath of the file 
+00001ec0: 746f 2062 6520 7061 7273 6564 2e20 5468  to be parsed. Th
+00001ed0: 6520 6669 6c65 206d 7573 7420 6861 7665  e file must have
+00001ee0: 0a20 2020 2020 2020 2066 6f72 6d61 7420  .        format 
+00001ef0: 636f 7272 6573 706f 6e64 696e 6720 746f  corresponding to
+00001f00: 2061 2060 606c 6174 2e69 6e60 6020 6f72   a ``lat.in`` or
+00001f10: 2060 6073 7472 2e6f 7574 6060 2066 696c   ``str.out`` fil
+00001f20: 6520 6672 6f6d 2041 5441 542e 0a20 2020  e from ATAT..   
+00001f30: 2060 6069 6e74 6572 7072 6574 5f61 7360   ``interpret_as`
+00001f40: 603a 2073 7472 696e 6720 6f72 204e 6f6e  `: string or Non
+00001f50: 650a 2020 2020 2020 2020 496e 6469 6361  e.        Indica
+00001f60: 7465 2068 6f77 2074 6f20 696e 7465 7270  te how to interp
+00001f70: 7265 7420 7468 6520 6669 6c65 2069 6e20  ret the file in 
+00001f80: 6060 6669 6c65 5f70 6174 6860 602e 2050  ``file_path``. P
+00001f90: 6f73 7369 626c 6520 7661 6c75 6573 2061  ossible values a
+00001fa0: 7265 3a0a 0a20 2020 2020 2020 202a 2060  re:..        * `
+00001fb0: 604e 6f6e 6560 603a 0a20 2020 2020 2020  `None``:.       
+00001fc0: 2020 2020 2054 6872 6565 2061 7272 6179       Three array
+00001fd0: 7320 6172 6520 7265 7475 726e 6564 3a20  s are returned: 
+00001fe0: 6060 6365 6c6c 6060 2c20 6060 7260 602c  ``cell``, ``r``,
+00001ff0: 2061 6e64 2060 6073 7065 6369 6573 6060   and ``species``
+00002000: 2e0a 2020 2020 2020 2020 2a20 6060 7061  ..        * ``pa
+00002010: 7265 6e74 5f6c 6174 7469 6365 6060 3a0a  rent_lattice``:.
+00002020: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+00002030: 7265 636f 6d6d 656e 6465 6420 7661 6c75  recommended valu
+00002040: 6520 6966 2060 6066 696c 655f 7061 7468  e if ``file_path
+00002050: 6060 2063 6f72 7265 7370 6f6e 6473 2074  `` corresponds t
+00002060: 6f0a 2020 2020 2020 2020 2020 2020 6120  o.            a 
+00002070: 6060 6c61 742e 696e 6060 2069 6e70 7574  ``lat.in`` input
+00002080: 2066 696c 6520 6672 6f6d 2041 5441 542e   file from ATAT.
+00002090: 2041 2060 6050 6172 656e 744c 6174 7469   A ``ParentLatti
+000020a0: 6365 6060 202a 2a43 454c 4c2a 2a0a 2020  ce`` **CELL**.  
+000020b0: 2020 2020 2020 2020 2020 6f62 6a65 6374            object
+000020c0: 2077 696c 6c20 6265 2072 6574 7572 6e65   will be returne
+000020d0: 642e 0a20 2020 2020 2020 202a 2060 6073  d..        * ``s
+000020e0: 7570 6572 5f63 656c 6c60 603a 0a20 2020  uper_cell``:.   
+000020f0: 2020 2020 2020 2020 2054 6865 2072 6563           The rec
+00002100: 6f6d 6d65 6e64 6564 2076 616c 7565 2069  ommended value i
+00002110: 6620 6060 6669 6c65 5f70 6174 6860 6020  f ``file_path`` 
+00002120: 636f 7272 6573 706f 6e64 7320 746f 0a20  corresponds to. 
+00002130: 2020 2020 2020 2020 2020 2061 2060 606c             a ``l
+00002140: 6174 2e69 6e60 6020 6669 6c65 2077 6974  at.in`` file wit
+00002150: 6820 6120 6d61 7472 6978 206f 6620 6c61  h a matrix of la
+00002160: 7474 6963 6520 7665 6374 6f72 7320 2860  ttice vectors (`
+00002170: 6075 2c76 2c77 6060 2069 6e0a 2020 2020  `u,v,w`` in.    
+00002180: 2020 2020 2020 2020 6041 5441 5420 646f          `ATAT do
+00002190: 6320 3c68 7474 7073 3a2f 2f77 7777 2e62  c <https://www.b
+000021a0: 726f 776e 2e65 6475 2f44 6570 6172 746d  rown.edu/Departm
+000021b0: 656e 7473 2f45 6e67 696e 6565 7269 6e67  ents/Engineering
+000021c0: 2f4c 6162 732f 6176 6477 2f61 7461 742f  /Labs/avdw/atat/
+000021d0: 6d61 6e75 616c 2f6e 6f64 6533 352e 6874  manual/node35.ht
+000021e0: 6d6c 3e60 5f29 0a20 2020 2020 2020 2020  ml>`_).         
+000021f0: 2020 2064 6966 6665 7265 6e74 2074 6f20     different to 
+00002200: 7468 6520 6964 656e 7469 7479 2c20 6f72  the identity, or
+00002210: 2069 6620 6974 2069 7320 6b6e 6f77 6e20   if it is known 
+00002220: 7468 6174 2074 6865 2073 7472 7563 7475  that the structu
+00002230: 7265 2069 730a 2020 2020 2020 2020 2020  re is.          
+00002240: 2020 6120 7065 7269 6f64 6963 2072 6570    a periodic rep
+00002250: 6574 6974 696f 6e20 6f66 2061 2070 6172  etition of a par
+00002260: 656e 7420 6c61 7474 6963 652e 2046 6f72  ent lattice. For
+00002270: 2074 6869 7320 6f70 7469 6f6e 2c20 7468   this option, th
+00002280: 6520 7061 7265 6e74 0a20 2020 2020 2020  e parent.       
+00002290: 2020 2020 206c 6174 7469 6365 206d 7573       lattice mus
+000022a0: 7420 6265 2070 726f 7669 6465 6420 2873  t be provided (s
+000022b0: 6565 2060 6070 6172 656e 745f 6c61 7474  ee ``parent_latt
+000022c0: 6963 6560 6020 7061 7261 6d65 7465 7220  ice`` parameter 
+000022d0: 6265 6c6f 7729 2e0a 2020 2020 2020 2020  below)..        
+000022e0: 2020 2020 4120 6060 5375 7065 7243 656c      A ``SuperCel
+000022f0: 6c60 6020 6f62 6a65 6374 2077 696c 6c20  l`` object will 
+00002300: 6265 2072 6574 7572 6e65 642e 0a20 2020  be returned..   
+00002310: 2020 2020 202a 2060 6073 7472 7563 7475       * ``structu
+00002320: 7265 6060 3a0a 2020 2020 2020 2020 2020  re``:.          
+00002330: 2020 5468 6520 7265 636f 6d6d 656e 6465    The recommende
+00002340: 6420 7661 6c75 6520 6966 2060 6066 696c  d value if ``fil
+00002350: 655f 7061 7468 6060 2063 6f72 7265 7370  e_path`` corresp
+00002360: 6f6e 6473 2074 6f0a 2020 2020 2020 2020  onds to.        
+00002370: 2020 2020 6120 6060 7374 722e 6f75 7460      a ``str.out`
+00002380: 6020 6669 6c65 2066 726f 6d20 4154 4154  ` file from ATAT
+00002390: 2e20 466f 7220 7468 6973 206f 7074 696f  . For this optio
+000023a0: 6e2c 2074 6865 2070 6172 656e 740a 2020  n, the parent.  
+000023b0: 2020 2020 2020 2020 2020 6c61 7474 6963            lattic
+000023c0: 6520 6d75 7374 2062 6520 7072 6f76 6964  e must be provid
+000023d0: 6564 2028 7365 6520 6060 7061 7265 6e74  ed (see ``parent
+000023e0: 5f6c 6174 7469 6365 6060 2070 6172 616d  _lattice`` param
+000023f0: 6574 6572 2062 656c 6f77 292e 0a20 2020  eter below)..   
+00002400: 2020 2020 2020 2020 2049 6e20 7468 6973           In this
+00002410: 2063 6173 6520 6120 6060 5374 7275 6374   case a ``Struct
+00002420: 7572 6560 6020 6f62 6a65 6374 2077 696c  ure`` object wil
+00002430: 6c20 6265 2072 6574 7572 6e65 642e 0a0a  l be returned...
+00002440: 2020 2020 6060 7061 7265 6e74 5f6c 6174      ``parent_lat
+00002450: 7469 6365 6060 3a20 5061 7265 6e74 4c61  tice``: ParentLa
+00002460: 7474 6963 6520 6f62 6a65 6374 0a20 2020  ttice object.   
+00002470: 2020 2020 2049 6620 6060 696e 7465 7270       If ``interp
+00002480: 7265 745f 6173 6060 2069 7320 6060 7375  ret_as`` is ``su
+00002490: 7065 725f 6365 6c6c 6060 206f 7220 6060  per_cell`` or ``
+000024a0: 7374 7275 6374 7572 6560 602c 2061 2070  structure``, a p
+000024b0: 6172 656e 7420 6c61 7474 6963 650a 2020  arent lattice.  
+000024c0: 2020 2020 2020 6d75 7374 2062 6520 7072        must be pr
+000024d0: 6f76 6964 6564 2e20 5468 6973 206d 7573  ovided. This mus
+000024e0: 7420 6265 2063 6f6d 7061 7469 626c 6520  t be compatible 
+000024f0: 7769 7468 2074 6865 2069 6e66 6f72 6d61  with the informa
+00002500: 7469 6f6e 2069 6e20 7468 650a 2020 2020  tion in the.    
+00002510: 2020 2020 6060 6c61 742e 696e 6060 2066      ``lat.in`` f
+00002520: 696c 6520 7468 6174 2077 6173 2075 7365  ile that was use
+00002530: 6420 746f 2063 7265 6174 6520 7468 6520  d to create the 
+00002540: 6060 7374 722e 6f75 7460 6020 6669 6c65  ``str.out`` file
+00002550: 732e 2053 6565 2074 6865 0a20 2020 2020  s. See the.     
+00002560: 2020 2065 7861 6d70 6c65 7320 6265 6c6f     examples belo
+00002570: 772e 0a20 2020 2060 6070 6263 6060 3a20  w..    ``pbc``: 
+00002580: 6f6e 6520 6f72 2074 6872 6565 2062 6f6f  one or three boo
+00002590: 6c20 2873 616d 6520 6173 2041 5345 2773  l (same as ASE's
+000025a0: 2041 746f 6d73 206f 626a 6563 7429 0a20   Atoms object). 
+000025b0: 2020 2020 2020 2050 6572 696f 6469 6320         Periodic 
+000025c0: 626f 756e 6461 7279 2063 6f6e 6469 7469  boundary conditi
+000025d0: 6f6e 7320 666c 6167 732e 2045 7861 6d70  ons flags. Examp
+000025e0: 6c65 733a 2054 7275 652c 2046 616c 7365  les: True, False
+000025f0: 2c20 302c 2031 2c0a 2020 2020 2020 2020  , 0, 1,.        
+00002600: 2831 2c20 312c 2030 292c 2028 5472 7565  (1, 1, 0), (True
+00002610: 2c20 4661 6c73 652c 2046 616c 7365 292e  , False, False).
+00002620: 2044 6566 6175 6c74 2076 616c 7565 3a20   Default value: 
+00002630: 4661 6c73 652e 2054 6865 2072 6574 7572  False. The retur
+00002640: 6e65 640a 2020 2020 2020 2020 2a2a 4345  ned.        **CE
+00002650: 4c4c 2a2a 206f 626a 6563 7473 2077 696c  LL** objects wil
+00002660: 6c20 6861 7665 2074 6865 7365 2070 6263  l have these pbc
+00002670: 2773 2073 6574 2075 702e 0a20 2020 2060  's set up..    `
+00002680: 6077 7261 7060 603a 2062 6f6f 6c65 616e  `wrap``: boolean
+00002690: 2028 6465 6661 756c 743a 6060 5472 7565   (default:``True
+000026a0: 6060 290a 2020 2020 2020 2020 5772 6170  ``).        Wrap
+000026b0: 2061 746f 6d69 6320 636f 6f72 6469 6e61   atomic coordina
+000026c0: 7465 732e 2049 6620 7062 6320 6973 2060  tes. If pbc is `
+000026d0: 604e 6f6e 6560 602c 2070 6263 2069 7320  `None``, pbc is 
+000026e0: 7365 7420 746f 2028 312c 312c 3129 2e0a  set to (1,1,1)..
+000026f0: 2020 2020 2020 2020 5365 7420 6060 7772          Set ``wr
+00002700: 6170 6060 2074 6f20 6060 4661 6c73 6560  ap`` to ``False`
+00002710: 6020 6966 2073 7472 7563 7475 7265 2063  ` if structure c
+00002720: 6f72 7265 7370 6f6e 6473 0a20 2020 2020  orresponds.     
+00002730: 2020 2074 6f20 6120 7375 7065 7263 656c     to a supercel
+00002740: 6c2c 2069 2e65 2e2c 2069 6620 7468 6520  l, i.e., if the 
+00002750: 7365 636f 6e64 206d 6174 7269 7820 6f66  second matrix of
+00002760: 2074 6865 2073 7472 7563 7475 7265 2064   the structure d
+00002770: 6566 696e 6974 696f 6e0a 2020 2020 2020  efinition.      
+00002780: 2020 696e 2065 6974 6865 7220 7468 6520    in either the 
+00002790: 6c61 742e 696e 206f 7220 7374 722e 6f75  lat.in or str.ou
+000027a0: 7420 6669 6c65 2069 7320 6469 6666 6572  t file is differ
+000027b0: 656e 7420 6672 6f6d 2074 6865 2069 6465  ent from the ide
+000027c0: 6e74 6974 790a 2020 2020 2020 2020 6d61  ntity.        ma
+000027d0: 7472 6978 2e0a 0a20 2020 202a 2a52 6574  trix...    **Ret
+000027e0: 7572 6e73 3a2a 2a0a 0a20 2020 2044 6570  urns:**..    Dep
+000027f0: 656e 6469 6e67 206f 6e20 7468 6520 7661  ending on the va
+00002800: 6c75 6520 6f66 2060 6069 6e74 6572 7072  lue of ``interpr
+00002810: 6574 5f61 7360 602c 2074 6865 2072 6574  et_as``, the ret
+00002820: 7572 6e65 6420 6f62 6a65 6374 2063 616e  urned object can
+00002830: 2062 6520 7079 7468 6f6e 0a20 2020 2061   be python.    a
+00002840: 7272 6179 7320 2860 6069 6e74 6572 7072  rrays (``interpr
+00002850: 6574 5f61 733d 4e6f 6e65 6060 292c 2061  et_as=None``), a
+00002860: 2060 6050 6172 656e 744c 6174 7469 6365   ``ParentLattice
+00002870: 6060 0a20 2020 2028 6060 696e 7465 7270  ``.    (``interp
+00002880: 7265 745f 6173 3d22 7061 7265 6e74 5f6c  ret_as="parent_l
+00002890: 6174 7469 6365 2260 6029 2c20 6120 6060  attice"``), a ``
+000028a0: 5375 7065 7243 656c 6c60 600a 2020 2020  SuperCell``.    
+000028b0: 2860 6069 6e74 6572 7072 6574 5f61 733d  (``interpret_as=
+000028c0: 2273 7570 6572 5f63 656c 6c22 6060 292c  "super_cell"``),
+000028d0: 206f 7220 6120 6060 5374 7275 6374 7572   or a ``Structur
+000028e0: 6560 600a 2020 2020 2860 6069 6e74 6572  e``.    (``inter
+000028f0: 7072 6574 5f61 733d 2253 7472 7563 7475  pret_as="Structu
+00002900: 7265 2260 6029 2e0a 0a20 2020 202a 2a45  re"``)...    **E
+00002910: 7861 6d70 6c65 733a 2a2a 0a0a 2020 2020  xamples:**..    
+00002920: 2e2e 2074 6f64 6f3a 3a0a 2020 2020 2020  .. todo::.      
+00002930: 2020 436c 6172 6966 7920 7772 6170 206f    Clarify wrap o
+00002940: 7074 696f 6e2e 2052 6967 6874 206e 6f77  ption. Right now
+00002950: 2069 7420 6973 206e 6f74 2067 7561 7261   it is not guara
+00002960: 6e74 6565 6420 746f 0a20 2020 2020 2020  nteed to.       
+00002970: 2077 6f72 6b20 7768 656e 2074 6865 2073   work when the s
+00002980: 7570 6572 6365 6c6c 2064 6566 696e 6974  upercell definit
+00002990: 696f 6e20 696e 206c 6174 2e69 6e20 6973  ion in lat.in is
+000029a0: 206e 6f74 2074 6865 0a20 2020 2020 2020   not the.       
+000029b0: 2069 6465 6e74 6974 7920 6d61 7472 6978   identity matrix
+000029c0: 2e20 5468 6973 2069 7320 736f 2c20 6265  . This is so, be
+000029d0: 6361 7573 6520 696e 2074 6865 206c 6174  cause in the lat
+000029e0: 2e69 6e20 666f 726d 6174 0a20 2020 2020  .in format.     
+000029f0: 2020 2074 6865 2073 6361 6c65 6420 636f     the scaled co
+00002a00: 6f72 6469 6e61 7465 7320 6172 6520 6769  ordinates are gi
+00002a10: 7665 6e20 696e 2072 6566 6572 656e 6365  ven in reference
+00002a20: 2074 6f20 7468 650a 2020 2020 2020 2020   to the.        
+00002a30: 6361 7274 6573 6961 6e20 7665 6374 6f72  cartesian vector
+00002a40: 7320 6f66 2074 6865 2070 6172 656e 7420  s of the parent 
+00002a50: 6c61 7474 6963 652c 2062 7574 206d 6179  lattice, but may
+00002a60: 2064 6566 696e 6520 610a 2020 2020 2020   define a.      
+00002a70: 2020 7375 7065 7263 656c 6c2e 2046 6978    supercell. Fix
+00002a80: 2069 7420 7375 6368 2074 6861 7420 7468   it such that th
+00002a90: 6520 7820 6d61 7472 6978 2062 656c 6f77  e x matrix below
+00002aa0: 2072 6566 6572 7273 2074 6f0a 2020 2020   referrs to.    
+00002ab0: 2020 2020 612a 6220 616e 6420 6e6f 7420      a*b and not 
+00002ac0: 6220 6173 2069 7420 6973 206e 6f77 2e0a  b as it is now..
+00002ad0: 0a20 2020 2022 2222 0a20 2020 2066 726f  .    """.    fro
+00002ae0: 6d20 6173 652e 6461 7461 2069 6d70 6f72  m ase.data impor
+00002af0: 7420 6174 6f6d 6963 5f6e 756d 6265 7273  t atomic_numbers
+00002b00: 0a20 2020 2066 726f 6d20 636f 7079 2069  .    from copy i
+00002b10: 6d70 6f72 7420 6465 6570 636f 7079 0a20  mport deepcopy. 
+00002b20: 2020 2066 726f 6d20 6173 6520 696d 706f     from ase impo
+00002b30: 7274 2041 746f 6d73 0a20 2020 2066 203d  rt Atoms.    f =
+00002b40: 206f 7065 6e28 6669 6c65 5f70 6174 6829   open(file_path)
+00002b50: 0a20 2020 206c 696e 6573 203d 2066 2e72  .    lines = f.r
+00002b60: 6561 646c 696e 6573 2829 0a20 2020 2066  eadlines().    f
+00002b70: 2e63 6c6f 7365 2829 0a0a 2020 2020 6c61  .close()..    la
+00002b80: 7420 3d20 5b5d 0a0a 2020 2020 6c61 742e  t = []..    lat.
+00002b90: 6170 7065 6e64 285b 5d29 0a20 2020 206c  append([]).    l
+00002ba0: 6e6e 3d30 0a20 2020 2066 6f72 206c 6e2c  nn=0.    for ln,
+00002bb0: 6c69 6e65 2069 6e20 656e 756d 6572 6174  line in enumerat
+00002bc0: 6528 6c69 6e65 7329 3a0a 2020 2020 2020  e(lines):.      
+00002bd0: 2020 6c73 203d 206c 696e 652e 7370 6c69    ls = line.spli
+00002be0: 7428 290a 2020 2020 2020 2020 6966 206c  t().        if l
+00002bf0: 656e 286c 7329 3e30 3a0a 2020 2020 2020  en(ls)>0:.      
+00002c00: 2020 2020 2020 6966 206c 6e20 3c20 333a        if ln < 3:
+00002c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002c20: 206c 6174 5b30 5d2e 6170 7065 6e64 285b   lat[0].append([
+00002c30: 666c 6f61 7428 6c73 5b30 5d29 2c66 6c6f  float(ls[0]),flo
+00002c40: 6174 286c 735b 315d 292c 666c 6f61 7428  at(ls[1]),float(
+00002c50: 6c73 5b32 5d29 5d29 0a20 2020 2020 2020  ls[2])]).       
+00002c60: 2020 2020 2069 6620 6c6e 203d 3d20 323a       if ln == 2:
+00002c70: 206c 6174 2e61 7070 656e 6428 5b5d 290a   lat.append([]).
+00002c80: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+00002c90: 6e20 3e20 3220 616e 6420 6c6e 203c 2036  n > 2 and ln < 6
+00002ca0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00002cb0: 2020 6c61 745b 315d 2e61 7070 656e 6428    lat[1].append(
+00002cc0: 5b66 6c6f 6174 286c 735b 305d 292c 666c  [float(ls[0]),fl
+00002cd0: 6f61 7428 6c73 5b31 5d29 2c66 6c6f 6174  oat(ls[1]),float
+00002ce0: 286c 735b 325d 295d 290a 2020 2020 2020  (ls[2])]).      
+00002cf0: 2020 2020 2020 6966 206c 6e20 3d3d 2035        if ln == 5
+00002d00: 3a20 6c61 742e 6170 7065 6e64 285b 5d29  : lat.append([])
+00002d10: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00002d20: 6c6e 203e 3d20 363a 0a20 2020 2020 2020  ln >= 6:.       
+00002d30: 2020 2020 2020 2020 206c 6174 5b32 5d2e           lat[2].
+00002d40: 6170 7065 6e64 285b 5d29 0a20 2020 2020  append([]).     
+00002d50: 2020 2020 2020 2020 2020 2073 3d27 272e             s=''.
+00002d60: 6a6f 696e 286c 735b 333a 5d29 2e73 706c  join(ls[3:]).spl
+00002d70: 6974 2827 2c27 290a 2020 2020 2020 2020  it(',').        
+00002d80: 2020 2020 2020 2020 6c61 745b 325d 5b6c          lat[2][l
+00002d90: 6e6e 5d2e 6170 7065 6e64 285b 666c 6f61  nn].append([floa
+00002da0: 7428 6c73 5b30 5d29 2c66 6c6f 6174 286c  t(ls[0]),float(l
+00002db0: 735b 315d 292c 666c 6f61 7428 6c73 5b32  s[1]),float(ls[2
+00002dc0: 5d29 5d29 0a20 2020 2020 2020 2020 2020  ])]).           
+00002dd0: 2020 2020 206c 6174 5b32 5d5b 6c6e 6e5d       lat[2][lnn]
+00002de0: 2e61 7070 656e 6428 7329 0a20 2020 2020  .append(s).     
+00002df0: 2020 2020 2020 2020 2020 206c 6e6e 203d             lnn =
+00002e00: 206c 6e6e 202b 2031 0a0a 2020 2020 7374   lnn + 1..    st
+00002e10: 7275 6320 3d20 6465 6570 636f 7079 286c  ruc = deepcopy(l
+00002e20: 6174 290a 0a20 2020 2023 2057 7269 7465  at)..    # Write
+00002e30: 2063 6f6f 7264 696e 6174 6520 7379 7374   coordinate syst
+00002e40: 656d 0a20 2020 2070 6172 656e 743d 5b5d  em.    parent=[]
+00002e50: 0a20 2020 2066 6f72 2069 2069 6e20 7261  .    for i in ra
+00002e60: 6e67 6528 3329 3a0a 2020 2020 2020 2020  nge(3):.        
+00002e70: 2020 2020 7061 7265 6e74 2e61 7070 656e      parent.appen
+00002e80: 6428 5b73 7472 7563 5b30 5d5b 695d 5b30  d([struc[0][i][0
+00002e90: 5d2c 7374 7275 635b 305d 5b69 5d5b 315d  ],struc[0][i][1]
+00002ea0: 2c73 7472 7563 5b30 5d5b 695d 5b32 5d5d  ,struc[0][i][2]]
+00002eb0: 290a 0a20 2020 2023 2057 7269 7465 206c  )..    # Write l
+00002ec0: 6174 7469 6365 0a20 2020 2073 6365 6c6c  attice.    scell
+00002ed0: 203d 205b 5d0a 2020 2020 666f 7220 6920   = [].    for i 
+00002ee0: 696e 2072 616e 6765 2833 293a 0a20 2020  in range(3):.   
+00002ef0: 2020 2020 2073 6365 6c6c 2e61 7070 656e       scell.appen
+00002f00: 6428 5b73 7472 7563 5b31 5d5b 695d 5b30  d([struc[1][i][0
+00002f10: 5d2c 7374 7275 635b 315d 5b69 5d5b 315d  ],struc[1][i][1]
+00002f20: 2c73 7472 7563 5b31 5d5b 695d 5b32 5d5d  ,struc[1][i][2]]
+00002f30: 290a 0a20 2020 2023 2057 7269 7465 2061  )..    # Write a
+00002f40: 746f 6d73 0a20 2020 2078 203d 205b 5d0a  toms.    x = [].
+00002f50: 2020 2020 7370 6563 6965 7320 3d20 5b5d      species = []
+00002f60: 0a20 2020 2066 6f72 2069 2069 6e20 7261  .    for i in ra
+00002f70: 6e67 6528 6c65 6e28 7374 7275 635b 325d  nge(len(struc[2]
+00002f80: 2929 3a0a 2020 2020 2020 2020 782e 6170  )):.        x.ap
+00002f90: 7065 6e64 285b 7374 7275 635b 325d 5b69  pend([struc[2][i
+00002fa0: 5d5b 305d 5b30 5d2c 7374 7275 635b 325d  ][0][0],struc[2]
+00002fb0: 5b69 5d5b 305d 5b31 5d2c 7374 7275 635b  [i][0][1],struc[
+00002fc0: 325d 5b69 5d5b 305d 5b32 5d5d 290a 2020  2][i][0][2]]).  
+00002fd0: 2020 2020 2020 6e72 7320 3d20 5b5d 0a20        nrs = []. 
+00002fe0: 2020 2020 2020 2066 6f72 2073 7020 696e         for sp in
+00002ff0: 2073 7472 7563 5b32 5d5b 695d 5b31 5d3a   struc[2][i][1]:
+00003000: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00003010: 7370 203d 3d20 2256 6163 2220 6f72 2073  sp == "Vac" or s
+00003020: 7020 3d3d 2022 5622 3a0a 2020 2020 2020  p == "V":.      
+00003030: 2020 2020 2020 2020 2020 7370 203d 2022            sp = "
+00003040: 5822 0a20 2020 2020 2020 2020 2020 206e  X".            n
+00003050: 7273 2e61 7070 656e 6428 6174 6f6d 6963  rs.append(atomic
+00003060: 5f6e 756d 6265 7273 5b73 705d 290a 2020  _numbers[sp]).  
+00003070: 2020 2020 2020 7370 6563 6965 732e 6170        species.ap
+00003080: 7065 6e64 286e 7273 290a 0a20 2020 2078  pend(nrs)..    x
+00003090: 203d 206e 702e 6d61 7472 6978 2878 290a   = np.matrix(x).
+000030a0: 2020 2020 6220 3d20 6e70 2e6d 6174 7269      b = np.matri
+000030b0: 7828 7061 7265 6e74 290a 2020 2020 6120  x(parent).    a 
+000030c0: 3d20 6e70 2e6d 6174 7269 7828 7363 656c  = np.matrix(scel
+000030d0: 6c29 0a0a 2020 2020 2323 2323 2323 2323  l)..    ########
+000030e0: 2323 2323 2323 2323 2323 2323 0a20 2020  ############.   
+000030f0: 2023 2043 616c 6375 6c61 7465 2072 6561   # Calculate rea
+00003100: 6c20 6361 7274 6573 6961 6e20 636f 6f72  l cartesian coor
+00003110: 6469 6e61 7465 730a 2020 2020 6966 2077  dinates.    if w
+00003120: 7261 703a 0a20 2020 2020 2020 2066 726f  rap:.        fro
+00003130: 6d20 636c 7573 7465 7278 2e73 796d 6d65  m clusterx.symme
+00003140: 7472 7920 696d 706f 7274 2077 7261 705f  try import wrap_
+00003150: 7363 616c 6564 5f70 6f73 6974 696f 6e73  scaled_positions
+00003160: 0a20 2020 2020 2020 2069 6620 7062 6320  .        if pbc 
+00003170: 3d3d 204e 6f6e 653a 0a20 2020 2020 2020  == None:.       
+00003180: 2020 2020 2070 6263 203d 2028 312c 312c       pbc = (1,1,
+00003190: 3129 0a20 2020 2020 2020 2078 203d 2077  1).        x = w
+000031a0: 7261 705f 7363 616c 6564 5f70 6f73 6974  rap_scaled_posit
+000031b0: 696f 6e73 2878 2c70 6263 290a 2020 2020  ions(x,pbc).    
+000031c0: 7220 3d20 782a 620a 0a20 2020 2063 656c  r = x*b..    cel
+000031d0: 6c20 3d20 612a 620a 2020 2020 6966 2069  l = a*b.    if i
+000031e0: 6e74 6572 7072 6574 5f61 7320 3d3d 204e  nterpret_as == N
+000031f0: 6f6e 653a 0a20 2020 2020 2020 2072 6574  one:.        ret
+00003200: 7572 6e20 6365 6c6c 2c20 722c 2073 7065  urn cell, r, spe
+00003210: 6369 6573 0a20 2020 2069 6620 696e 7465  cies.    if inte
+00003220: 7270 7265 745f 6173 203d 3d20 2270 6172  rpret_as == "par
+00003230: 656e 745f 6c61 7474 6963 6522 3a0a 2020  ent_lattice":.  
+00003240: 2020 2020 2020 6672 6f6d 2063 6c75 7374        from clust
+00003250: 6572 782e 7061 7265 6e74 5f6c 6174 7469  erx.parent_latti
+00003260: 6365 2069 6d70 6f72 7420 5061 7265 6e74  ce import Parent
+00003270: 4c61 7474 6963 650a 2020 2020 2020 2020  Lattice.        
+00003280: 6e72 7320 3d20 6e70 2e7a 6572 6f73 286c  nrs = np.zeros(l
+00003290: 656e 2873 7065 6369 6573 2929 0a20 2020  en(species)).   
+000032a0: 2020 2020 2066 6f72 2069 6e72 2c20 6e72       for inr, nr
+000032b0: 2069 6e20 656e 756d 6572 6174 6528 7370   in enumerate(sp
+000032c0: 6563 6965 7329 3a0a 2020 2020 2020 2020  ecies):.        
+000032d0: 2020 2020 6e72 735b 696e 725d 3d69 6e74      nrs[inr]=int
+000032e0: 286e 725b 305d 290a 0a20 2020 2020 2020  (nr[0])..       
+000032f0: 2070 6c61 7420 3d20 5061 7265 6e74 4c61   plat = ParentLa
+00003300: 7474 6963 6528 4174 6f6d 7328 706f 7369  ttice(Atoms(posi
+00003310: 7469 6f6e 733d 722c 6365 6c6c 3d63 656c  tions=r,cell=cel
+00003320: 6c2c 6e75 6d62 6572 733d 6e72 732c 7062  l,numbers=nrs,pb
+00003330: 633d 7062 6329 2c73 6974 6573 3d73 7065  c=pbc),sites=spe
+00003340: 6369 6573 2c70 6263 3d70 6263 290a 2020  cies,pbc=pbc).  
+00003350: 2020 2020 2020 7265 7475 726e 2070 6c61        return pla
+00003360: 740a 2020 2020 6966 2069 6e74 6572 7072  t.    if interpr
+00003370: 6574 5f61 7320 3d3d 2022 7375 7065 725f  et_as == "super_
+00003380: 6365 6c6c 223a 0a20 2020 2020 2020 2066  cell":.        f
+00003390: 726f 6d20 636c 7573 7465 7278 2e73 7472  rom clusterx.str
+000033a0: 7563 7475 7265 2069 6d70 6f72 7420 5374  ucture import St
+000033b0: 7275 6374 7572 650a 2020 2020 2020 2020  ructure.        
+000033c0: 7063 656c 6c20 3d20 7061 7265 6e74 5f6c  pcell = parent_l
+000033d0: 6174 7469 6365 2e67 6574 5f63 656c 6c28  attice.get_cell(
+000033e0: 290a 2020 2020 2020 2020 746d 6174 203d  ).        tmat =
+000033f0: 206e 702e 6173 6172 7261 7928 6e70 2e72   np.asarray(np.r
+00003400: 696e 7428 6e70 2e64 6f74 2863 656c 6c2c  int(np.dot(cell,
+00003410: 6e70 2e6c 696e 616c 672e 696e 7628 7063  np.linalg.inv(pc
+00003420: 656c 6c29 2929 2e61 7374 7970 6528 696e  ell))).astype(in
+00003430: 7429 290a 2020 2020 2020 2020 6672 6f6d  t)).        from
+00003440: 2063 6c75 7374 6572 782e 7375 7065 725f   clusterx.super_
+00003450: 6365 6c6c 2069 6d70 6f72 7420 5375 7065  cell import Supe
+00003460: 7243 656c 6c0a 2020 2020 2020 2020 7363  rCell.        sc
+00003470: 656c 6c20 3d20 5375 7065 7243 656c 6c28  ell = SuperCell(
+00003480: 7061 7265 6e74 5f6c 6174 7469 6365 2c74  parent_lattice,t
+00003490: 6d61 7429 0a20 2020 2020 2020 2072 6574  mat).        ret
+000034a0: 7572 6e20 7363 656c 6c0a 2020 2020 6966  urn scell.    if
+000034b0: 2069 6e74 6572 7072 6574 5f61 7320 3d3d   interpret_as ==
+000034c0: 2022 7374 7275 6374 7572 6522 3a0a 2020   "structure":.  
+000034d0: 2020 2020 2020 6672 6f6d 2063 6c75 7374        from clust
+000034e0: 6572 782e 7374 7275 6374 7572 6520 696d  erx.structure im
+000034f0: 706f 7274 2053 7472 7563 7475 7265 0a20  port Structure. 
+00003500: 2020 2020 2020 2070 6365 6c6c 203d 2070         pcell = p
+00003510: 6172 656e 745f 6c61 7474 6963 652e 6765  arent_lattice.ge
+00003520: 745f 6365 6c6c 2829 0a20 2020 2020 2020  t_cell().       
+00003530: 2074 6d61 7420 3d20 6e70 2e61 7361 7272   tmat = np.asarr
+00003540: 6179 286e 702e 7269 6e74 286e 702e 646f  ay(np.rint(np.do
+00003550: 7428 6365 6c6c 2c6e 702e 6c69 6e61 6c67  t(cell,np.linalg
+00003560: 2e69 6e76 2870 6365 6c6c 2929 292e 6173  .inv(pcell))).as
+00003570: 7479 7065 2869 6e74 2929 0a20 2020 2020  type(int)).     
+00003580: 2020 2066 726f 6d20 636c 7573 7465 7278     from clusterx
+00003590: 2e73 7570 6572 5f63 656c 6c20 696d 706f  .super_cell impo
+000035a0: 7274 2053 7570 6572 4365 6c6c 0a20 2020  rt SuperCell.   
+000035b0: 2020 2020 2073 6365 6c6c 203d 2053 7570       scell = Sup
+000035c0: 6572 4365 6c6c 2870 6172 656e 745f 6c61  erCell(parent_la
+000035d0: 7474 6963 652c 746d 6174 290a 2020 2020  ttice,tmat).    
+000035e0: 2020 2020 7072 6973 203d 2073 6365 6c6c      pris = scell
+000035f0: 2e67 6574 5f70 7269 7374 696e 6528 290a  .get_pristine().
+00003600: 0a20 2020 2020 2020 2070 6f73 203d 2070  .        pos = p
+00003610: 7269 732e 6765 745f 706f 7369 7469 6f6e  ris.get_position
+00003620: 7328 290a 2020 2020 2020 2020 6e65 775f  s().        new_
+00003630: 6e72 7320 3d20 6e70 2e7a 6572 6f73 286c  nrs = np.zeros(l
+00003640: 656e 2870 6f73 2929 0a20 2020 2020 2020  en(pos)).       
+00003650: 2066 6f72 2069 702c 7020 696e 2065 6e75   for ip,p in enu
+00003660: 6d65 7261 7465 2872 293a 0a20 2020 2020  merate(r):.     
+00003670: 2020 2020 2020 206e 7220 3d20 7370 6563         nr = spec
+00003680: 6965 735b 6970 5d5b 305d 0a20 2020 2020  ies[ip][0].     
+00003690: 2020 2020 2020 2066 6f72 2069 322c 7032         for i2,p2
+000036a0: 2069 6e20 656e 756d 6572 6174 6528 706f   in enumerate(po
+000036b0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+000036c0: 2020 2020 6966 2069 7363 6c6f 7365 286e      if isclose(n
+000036d0: 702e 6173 6172 7261 7928 7029 2e72 6573  p.asarray(p).res
+000036e0: 6861 7065 282d 3129 2c70 3229 3a0a 2020  hape(-1),p2):.  
+000036f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003700: 2020 6e65 775f 6e72 735b 6932 5d20 3d20    new_nrs[i2] = 
+00003710: 6e72 0a0a 2020 2020 2020 2020 7374 7275  nr..        stru
+00003720: 6320 3d20 5374 7275 6374 7572 6528 7363  c = Structure(sc
+00003730: 656c 6c2c 6465 636f 7261 7469 6f6e 3d6e  ell,decoration=n
+00003740: 6577 5f6e 7273 290a 2020 2020 2020 2020  ew_nrs).        
+00003750: 7265 7475 726e 2073 7472 7563 0a0a 0a64  return struc...d
+00003760: 6566 205f 6973 5f69 6e74 6567 6572 5f6d  ef _is_integer_m
+00003770: 6174 7269 7828 6d2c 726e 643d 3529 3a0a  atrix(m,rnd=5):.
+00003780: 2020 2020 6d69 203d 206e 702e 6172 6f75      mi = np.arou
+00003790: 6e64 286d 2c72 6e64 290a 2020 2020 666f  nd(m,rnd).    fo
+000037a0: 7220 6b20 696e 2072 616e 6765 2833 293a  r k in range(3):
+000037b0: 0a20 2020 2020 2020 2066 6f72 206c 2069  .        for l i
+000037c0: 6e20 7261 6e67 6528 3329 3a0a 2020 2020  n range(3):.    
+000037d0: 2020 2020 2020 2020 2369 6620 6e6f 7420          #if not 
+000037e0: 726f 756e 6428 6d5b 6b2c 6c5d 2c72 6e64  round(m[k,l],rnd
+000037f0: 292e 6973 5f69 6e74 6567 6572 2829 3a0a  ).is_integer():.
+00003800: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00003810: 6f74 206d 695b 6b2c 6c5d 2e69 735f 696e  ot mi[k,l].is_in
+00003820: 7465 6765 7228 293a 0a20 2020 2020 2020  teger():.       
+00003830: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00003840: 4661 6c73 650a 2020 2020 7265 7475 726e  False.    return
+00003850: 2054 7275 650a 0a64 6566 2067 6574 5f63   True..def get_c
+00003860: 6c5f 6964 785f 7363 2863 6c2c 2073 632c  l_idx_sc(cl, sc,
+00003870: 206d 6574 686f 643d 302c 2074 6f6c 3d31   method=0, tol=1
+00003880: 652d 3329 3a0a 2020 2020 2222 2252 6574  e-3):.    """Ret
+00003890: 7572 6e20 6174 6f6d 2069 6e64 6578 6573  urn atom indexes
+000038a0: 206f 6620 636c 7573 7465 7220 706f 696e   of cluster poin
+000038b0: 7473 2069 6e20 5375 7065 7243 656c 6c0a  ts in SuperCell.
+000038c0: 0a20 2020 202a 2a50 6172 616d 6574 6572  .    **Parameter
+000038d0: 733a 2a2a 0a0a 2020 2020 6060 636c 6060  s:**..    ``cl``
+000038e0: 3a20 6e70 6f69 6e74 7320 7820 3320 6d61  : npoints x 3 ma
+000038f0: 7472 6978 0a20 2020 2020 2020 206d 6174  trix.        mat
+00003900: 7269 7820 6f66 2063 6172 7465 7369 616e  rix of cartesian
+00003910: 206f 7220 7363 616c 6564 2063 6f6f 7264   or scaled coord
+00003920: 696e 6174 6573 206f 6620 636c 7573 7465  inates of cluste
+00003930: 7220 706f 696e 7473 2e20 436c 7573 7465  r points. Cluste
+00003940: 720a 2020 2020 2020 2020 706f 7369 7469  r.        positi
+00003950: 6f6e 7320 6172 6520 6578 7065 6374 6564  ons are expected
+00003960: 2074 6f20 6265 2077 7261 7070 6564 2069   to be wrapped i
+00003970: 6e73 6964 6520 7375 7065 7263 656c 6c20  nside supercell 
+00003980: 6060 7363 6060 0a20 2020 2060 6073 6360  ``sc``.    ``sc`
+00003990: 603a 206e 6174 6f6d 7320 7820 3320 6d61  `: natoms x 3 ma
+000039a0: 7472 6978 0a20 2020 2020 2020 206d 6174  trix.        mat
+000039b0: 7269 7820 6f66 2063 6172 7465 7369 616e  rix of cartesian
+000039c0: 206f 7220 7363 616c 6564 2063 6f6f 7264   or scaled coord
+000039d0: 696e 6174 6573 206f 6620 7375 7065 7263  inates of superc
+000039e0: 656c 6c20 6174 6f6d 6963 2070 6f73 6974  ell atomic posit
+000039f0: 696f 6e73 2e0a 2020 2020 2020 2020 5468  ions..        Th
+00003a00: 6520 7479 7065 206f 6620 636f 6f72 6469  e type of coordi
+00003a10: 6e61 7465 7320 2865 6974 6865 7220 6361  nates (either ca
+00003a20: 7274 6573 696f 6e20 6f72 2073 6361 6c65  rtesion or scale
+00003a30: 6429 206d 7573 7420 636f 696e 6369 6465  d) must coincide
+00003a40: 2077 6974 680a 2020 2020 2020 2020 7468   with.        th
+00003a50: 6174 206f 6620 6060 636c 6060 0a20 2020  at of ``cl``.   
+00003a60: 2060 606d 6574 686f 6460 603a 2069 6e74   ``method``: int
+00003a70: 6567 6572 0a20 2020 2020 2020 204d 6574  eger.        Met
+00003a80: 686f 6420 746f 2075 7365 2e20 303a 2028  hod to use. 0: (
+00003a90: 736c 6f77 2920 6e65 7374 6564 2066 6f72  slow) nested for
+00003aa0: 206c 6f6f 7020 7573 696e 6720 6e75 6d70   loop using nump
+00003ab0: 7920 616c 6c63 6c6f 7365 2e20 313a 2028  y allclose. 1: (
+00003ac0: 6661 7374 290a 2020 2020 2020 2020 6361  fast).        ca
+00003ad0: 6c63 756c 6174 6573 2061 6c6c 2064 6973  lculates all dis
+00003ae0: 7461 6e63 6573 2066 726f 6d20 706f 696e  tances from poin
+00003af0: 7473 2069 6e20 6060 636c 6060 2074 6f20  ts in ``cl`` to 
+00003b00: 6174 6f6d 7320 696e 2060 6073 6360 602c  atoms in ``sc``,
+00003b10: 2061 6e64 0a20 2020 2020 2020 2072 6574   and.        ret
+00003b20: 7572 6e20 696e 6469 6365 7320 666f 7220  urn indices for 
+00003b30: 7768 6963 6820 6469 7374 616e 6365 7320  which distances 
+00003b40: 6172 6520 7a65 726f 2e0a 2020 2020 6060  are zero..    ``
+00003b50: 746f 6c60 603a 2072 6561 6c20 706f 7369  tol``: real posi
+00003b60: 7469 7665 206e 756d 6265 720a 2020 2020  tive number.    
+00003b70: 2020 2020 746f 6c65 7261 6e63 6520 746f      tolerance to
+00003b80: 2064 6574 6572 6d69 6e65 2077 6865 7468   determine wheth
+00003b90: 6572 2063 6c75 7374 6572 2061 6e64 2061  er cluster and a
+00003ba0: 746f 6d20 706f 7369 7469 6f6e 7320 6172  tom positions ar
+00003bb0: 6520 7468 6520 7361 6d65 2e0a 2020 2020  e the same..    
+00003bc0: 2222 220a 2020 2020 6672 6f6d 2073 6369  """.    from sci
+00003bd0: 7079 2e73 7061 7469 616c 2e64 6973 7461  py.spatial.dista
+00003be0: 6e63 6520 696d 706f 7274 2063 6469 7374  nce import cdist
+00003bf0: 0a20 2020 2073 6469 7374 616e 6365 7320  .    sdistances 
+00003c00: 3d20 4e6f 6e65 0a20 2020 206d 6574 686f  = None.    metho
+00003c10: 6420 3d20 310a 2020 2020 6966 206d 6574  d = 1.    if met
+00003c20: 686f 6420 3d3d 2030 3a0a 2020 2020 2020  hod == 0:.      
+00003c30: 2020 6964 7873 203d 206e 702e 7a65 726f    idxs = np.zero
+00003c40: 7328 6c65 6e28 636c 292c 6474 7970 653d  s(len(cl),dtype=
+00003c50: 2269 6e74 2229 0a20 2020 2020 2020 2066  "int").        f
+00003c60: 6f72 2069 636c 2c63 6c70 2069 6e20 656e  or icl,clp in en
+00003c70: 756d 6572 6174 6528 636c 293a 0a20 2020  umerate(cl):.   
+00003c80: 2020 2020 2020 2020 2066 6f72 2069 7363           for isc
+00003c90: 2c20 7363 7020 696e 2065 6e75 6d65 7261  , scp in enumera
+00003ca0: 7465 2873 6329 3a0a 2020 2020 2020 2020  te(sc):.        
+00003cb0: 2020 2020 2020 2020 6966 206e 702e 616c          if np.al
+00003cc0: 6c63 6c6f 7365 2863 6c70 2c73 6370 2c61  lclose(clp,scp,a
+00003cd0: 746f 6c3d 746f 6c29 3a0a 2020 2020 2020  tol=tol):.      
+00003ce0: 2020 2020 2020 2020 2020 2020 2020 6964                id
+00003cf0: 7873 5b69 636c 5d20 3d20 6973 630a 2020  xs[icl] = isc.  
+00003d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d10: 2020 6272 6561 6b0a 0a20 2020 2069 6620    break..    if 
+00003d20: 6d65 7468 6f64 203d 3d20 313a 0a20 2020  method == 1:.   
+00003d30: 2020 2020 2073 6469 7374 616e 6365 7320       sdistances 
+00003d40: 3d20 6364 6973 7428 636c 2c20 7363 2c20  = cdist(cl, sc, 
+00003d50: 6d65 7472 6963 3d27 6575 636c 6964 6561  metric='euclidea
+00003d60: 6e27 2920 2320 4576 616c 7561 7465 2061  n') # Evaluate a
+00003d70: 6c6c 2028 7363 616c 6564 2920 6469 7374  ll (scaled) dist
+00003d80: 616e 6365 7320 6265 7477 6565 6e20 636c  ances between cl
+00003d90: 7573 7465 7220 706f 696e 7473 2074 6f20  uster points to 
+00003da0: 7363 656c 6c20 7369 7465 730a 2020 2020  scell sites.    
+00003db0: 2020 2020 6964 7873 203d 206e 702e 6172      idxs = np.ar
+00003dc0: 6777 6865 7265 286e 702e 6162 7328 7364  gwhere(np.abs(sd
+00003dd0: 6973 7461 6e63 6573 2920 3c20 746f 6c29  istances) < tol)
+00003de0: 5b3a 2c31 5d20 2320 4174 6f6d 2069 6e64  [:,1] # Atom ind
+00003df0: 6578 6573 206f 6620 7468 6520 7472 616e  exes of the tran
+00003e00: 7366 6f72 6d65 6420 636c 7573 7465 720a  sformed cluster.
+00003e10: 0a20 2020 2072 6574 7572 6e20 6964 7873  .    return idxs
+00003e20: 0a0a 6465 6620 6164 645f 6e6f 6973 6528  ..def add_noise(
+00003e30: 762c 6e6f 6973 655f 6c65 7665 6c29 3a0a  v,noise_level):.
+00003e40: 2020 2020 2222 2241 6464 2072 616e 646f      """Add rando
+00003e50: 6d6c 7920 6469 7374 7269 6275 7465 6420  mly distributed 
+00003e60: 6e6f 6973 6520 746f 2076 6563 746f 7220  noise to vector 
+00003e70: 636f 6f72 6469 6e61 7465 730a 0a20 2020  coordinates..   
+00003e80: 2054 6f20 6561 6368 2063 6f6f 7264 696e   To each coordin
+00003e90: 6174 6520 6f66 2074 6865 2069 6e70 7574  ate of the input
+00003ea0: 2076 6563 746f 7220 6060 7660 602c 2072   vector ``v``, r
+00003eb0: 616e 646f 6d20 6e6f 6973 6520 756e 6966  andom noise unif
+00003ec0: 6f72 6d6c 790a 2020 2020 6469 7374 7269  ormly.    distri
+00003ed0: 6275 7465 6420 6265 7477 6565 6e20 2d60  buted between -`
+00003ee0: 606e 6f69 7365 5f6c 6576 656c 6060 2061  `noise_level`` a
+00003ef0: 6e64 2060 606e 6f69 7365 5f6c 6576 656c  nd ``noise_level
+00003f00: 6060 2069 7320 6164 6465 642e 2054 6865  `` is added. The
+00003f10: 2069 6e70 7574 0a20 2020 2076 6563 746f   input.    vecto
+00003f20: 7220 6060 7660 6020 6973 206c 6566 7420  r ``v`` is left 
+00003f30: 756e 6368 616e 6765 642e 2054 6865 206d  unchanged. The m
+00003f40: 6f64 6966 6965 6420 7665 6374 6f72 2069  odified vector i
+00003f50: 7320 7265 7475 726e 6564 2e0a 0a20 2020  s returned...   
+00003f60: 202a 2a50 6172 616d 6574 6572 733a 2a2a   **Parameters:**
+00003f70: 0a0a 2020 2020 6060 7660 603a 206c 6973  ..    ``v``: lis
+00003f80: 7420 6f66 2066 6c6f 6174 730a 2020 2020  t of floats.    
+00003f90: 2020 2020 5468 6520 696e 7075 7420 7665      The input ve
+00003fa0: 6374 6f72 0a0a 2020 2020 6060 6e6f 6973  ctor..    ``nois
+00003fb0: 655f 6c65 7665 6c60 603a 2066 6c6f 6174  e_level``: float
+00003fc0: 0a20 2020 2020 2020 2057 6964 7468 206f  .        Width o
+00003fd0: 6620 7468 6520 756e 6966 6f72 6d20 6469  f the uniform di
+00003fe0: 7374 7269 6275 7469 6f6e 2075 7365 6420  stribution used 
+00003ff0: 746f 2061 6464 206e 6f69 7365 2e0a 2020  to add noise..  
+00004000: 2020 2222 220a 2020 2020 696d 706f 7274    """.    import
+00004010: 2072 616e 646f 6d0a 2020 2020 656e 6572   random.    ener
+00004020: 6769 6573 203d 205b 5d0a 2020 2020 666f  gies = [].    fo
+00004030: 7220 6520 696e 2076 3a0a 2020 2020 2020  r e in v:.      
+00004040: 2020 656e 6572 6769 6573 2e61 7070 656e    energies.appen
+00004050: 6428 652b 7261 6e64 6f6d 2e75 6e69 666f  d(e+random.unifo
+00004060: 726d 282d 312c 3129 2a6e 6f69 7365 5f6c  rm(-1,1)*noise_l
+00004070: 6576 656c 290a 2020 2020 7265 7475 726e  evel).    return
+00004080: 2065 6e65 7267 6965 730a 0a64 6566 2063   energies..def c
+00004090: 616c 6375 6c61 7465 5f74 7261 666f 5f6d  alculate_trafo_m
+000040a0: 6174 7269 7828 7063 656c 6c2c 7363 656c  atrix(pcell,scel
+000040b0: 6c2c 726e 643d 3529 3a0a 2020 2020 2222  l,rnd=5):.    ""
+000040c0: 2243 616c 6375 6c61 7465 2069 6e74 6567  "Calculate integ
+000040d0: 6572 2074 7261 6e73 666f 726d 6174 696f  er transformatio
+000040e0: 6e20 6d61 7472 6978 2067 6976 656e 2061  n matrix given a
+000040f0: 2070 7269 6d69 7469 7665 2063 656c 6c20   primitive cell 
+00004100: 616e 6420 6120 7375 7065 722d 6365 6c6c  and a super-cell
+00004110: 0a0a 2020 2020 4966 203a 6d61 7468 3a60  ..    If :math:`
+00004120: 5360 2061 6e64 203a 6d61 7468 3a60 5660  S` and :math:`V`
+00004130: 2061 7265 2c20 7265 7370 6563 7469 7665   are, respective
+00004140: 6c79 2c20 6120 6d61 7472 6978 2077 686f  ly, a matrix who
+00004150: 7365 2072 6f77 7320 6172 6520 7468 6520  se rows are the 
+00004160: 6361 7274 6573 6961 6e20 636f 6f72 6469  cartesian coordi
+00004170: 6e61 7465 730a 2020 2020 6f66 2074 6865  nates.    of the
+00004180: 2070 6172 656e 7420 6c61 7474 6963 6520   parent lattice 
+00004190: 7665 6374 6f72 7320 616e 6420 6120 6d61  vectors and a ma
+000041a0: 7472 6978 2077 686f 7365 2072 6f77 7320  trix whose rows 
+000041b0: 6172 6520 7468 6520 6361 7274 6573 6961  are the cartesia
+000041c0: 6e20 636f 6f72 6469 6e61 7465 730a 2020  n coordinates.  
+000041d0: 2020 6f66 2074 6865 2073 7570 6572 2d63    of the super-c
+000041e0: 656c 6c20 6c61 7474 6963 6520 7665 6374  ell lattice vect
+000041f0: 6f72 733b 2074 6865 6e2c 2074 6869 7320  ors; then, this 
+00004200: 6675 6e63 7469 6f6e 2072 6574 7572 6e73  function returns
+00004210: 2074 6865 206d 6174 7269 7820 3a6d 6174   the matrix :mat
+00004220: 683a 6050 3d53 565e 7b2d 317d 602e 0a20  h:`P=SV^{-1}`.. 
+00004230: 2020 2049 6620 7468 6520 7265 7375 6c74     If the result
+00004240: 696e 6720 6d61 7472 6978 2069 7320 6e6f  ing matrix is no
+00004250: 7420 696e 7465 6765 7220 2873 6565 2060  t integer (see `
+00004260: 6072 6e64 6060 2070 6172 616d 6574 6572  `rnd`` parameter
+00004270: 292c 2074 6865 6e20 6060 4e6f 6e65 6060  ), then ``None``
+00004280: 2069 7320 7265 7475 726e 6564 2e0a 0a20   is returned... 
+00004290: 2020 202a 2a50 6172 616d 6574 6572 733a     **Parameters:
+000042a0: 2a2a 0a0a 2020 2020 6060 7063 656c 6c60  **..    ``pcell`
+000042b0: 603a 2033 7833 2061 7272 6179 206f 6620  `: 3x3 array of 
+000042c0: 666c 6f61 740a 2020 2020 2020 2020 5468  float.        Th
+000042d0: 6520 726f 7773 206f 6620 7468 6973 206d  e rows of this m
+000042e0: 6174 7269 7820 636f 7272 6573 706f 6e64  atrix correspond
+000042f0: 2074 6f20 7468 6520 6361 7274 6573 6961   to the cartesia
+00004300: 6e20 636f 6f72 6469 6e61 7465 7320 6f66  n coordinates of
+00004310: 2061 2070 6172 656e 7420 6c61 7474 6963   a parent lattic
+00004320: 650a 0a20 2020 2060 6073 6365 6c6c 6060  e..    ``scell``
+00004330: 3a20 3378 3320 6172 7261 7920 6f66 2066  : 3x3 array of f
+00004340: 6c6f 6174 0a20 2020 2020 2020 2054 6865  loat.        The
+00004350: 2072 6f77 7320 6f66 2074 6869 7320 6d61   rows of this ma
+00004360: 7472 6978 2063 6f72 7265 7370 6f6e 6420  trix correspond 
+00004370: 746f 2074 6865 2063 6172 7465 7369 616e  to the cartesian
+00004380: 2063 6f6f 7264 696e 6174 6573 206f 6620   coordinates of 
+00004390: 6120 7375 7065 7263 656c 6c0a 0a20 2020  a supercell..   
+000043a0: 2060 6072 6e64 6060 3a20 696e 7465 6765   ``rnd``: intege
+000043b0: 7220 286f 7074 696f 6e61 6c29 0a20 2020  r (optional).   
+000043c0: 2020 2020 2020 5468 6520 6d61 7472 6978        The matrix
+000043d0: 203a 6d61 7468 3a60 503d 5356 5e7b 2d31   :math:`P=SV^{-1
+000043e0: 7d60 2069 7320 726f 756e 6465 6420 746f  }` is rounded to
+000043f0: 2060 6072 6e64 6060 2064 6563 696d 616c   ``rnd`` decimal
+00004400: 2070 6c61 6365 7320 616e 6420 6368 6563   places and chec
+00004410: 6b65 6420 666f 7220 696e 7465 6772 6974  ked for integrit
+00004420: 792e 0a20 2020 2022 2222 0a20 2020 2074  y..    """.    t
+00004430: 6d61 7420 3d20 6e70 2e64 6f74 2873 6365  mat = np.dot(sce
+00004440: 6c6c 2c6e 702e 6c69 6e61 6c67 2e69 6e76  ll,np.linalg.inv
+00004450: 2870 6365 6c6c 2929 0a20 2020 2069 6620  (pcell)).    if 
+00004460: 5f69 735f 696e 7465 6765 725f 6d61 7472  _is_integer_matr
+00004470: 6978 2874 6d61 742c 726e 6429 3a0a 2020  ix(tmat,rnd):.  
+00004480: 2020 2020 2020 7265 7475 726e 206e 702e        return np.
+00004490: 6173 6172 7261 7928 6e70 2e72 696e 7428  asarray(np.rint(
+000044a0: 746d 6174 292e 6173 7479 7065 2869 6e74  tmat).astype(int
+000044b0: 2929 0a20 2020 2065 6c73 653a 0a20 2020  )).    else:.   
+000044c0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+000044d0: 0a0a 6465 6620 5f73 7472 5f67 7265 7028  ..def _str_grep(
+000044e0: 696e 7075 745f 7374 722c 2073 6561 7263  input_str, searc
+000044f0: 685f 7374 722c 2070 7265 7065 6e64 3d27  h_str, prepend='
+00004500: 2729 3a0a 2020 2020 6f75 745f 7374 7220  '):.    out_str 
+00004510: 3d20 2727 0a20 2020 2066 6f72 206c 2069  = ''.    for l i
+00004520: 6e20 696e 7075 745f 7374 722e 7370 6c69  n input_str.spli
+00004530: 7428 275c 6e27 293a 0a20 2020 2020 2020  t('\n'):.       
+00004540: 2069 6620 7365 6172 6368 5f73 7472 2069   if search_str i
+00004550: 6e20 6c3a 0a20 2020 2020 2020 2020 2020  n l:.           
+00004560: 206f 7574 5f73 7472 203d 206f 7574 5f73   out_str = out_s
+00004570: 7472 202b 2070 7265 7065 6e64 202b 206c  tr + prepend + l
+00004580: 2e73 7472 6970 2829 202b 2027 5c6e 270a  .strip() + '\n'.
+00004590: 0a20 2020 2072 6574 7572 6e20 6f75 745f  .    return out_
+000045a0: 7374 722e 7273 7472 6970 2829 0a0a 6465  str.rstrip()..de
+000045b0: 6620 6d67 7265 7028 6670 6174 682c 2073  f mgrep(fpath, s
+000045c0: 6561 7263 685f 6172 7261 792c 2070 7265  earch_array, pre
+000045d0: 7065 6e64 3d27 272c 726f 6f74 3d27 2e27  pend='',root='.'
+000045e0: 293a 0a20 2020 2022 2222 0a20 2020 2047  ):.    """.    G
+000045f0: 7265 7020 7374 7269 6e67 7320 696e 2066  rep strings in f
+00004600: 696c 6520 616e 6420 7265 7475 726e 206d  ile and return m
+00004610: 6174 6368 696e 6720 6c69 6e65 732e 0a0a  atching lines...
+00004620: 2020 2020 2a2a 5061 7261 6d65 7465 7273      **Parameters
+00004630: 3a2a 2a0a 0a20 2020 2060 6066 7061 7468  :**..    ``fpath
+00004640: 6060 3a20 7374 7269 6e67 0a20 2020 2020  ``: string.     
+00004650: 2020 2046 696c 6520 7061 7468 2074 6f20     File path to 
+00004660: 6772 6570 0a20 2020 2060 6073 6561 7263  grep.    ``searc
+00004670: 685f 6172 7261 7960 603a 2061 7272 6179  h_array``: array
+00004680: 206f 6620 7374 7269 6e67 730a 2020 2020   of strings.    
+00004690: 2020 2020 4561 6368 2065 6c65 6d65 6e74      Each element
+000046a0: 206f 6620 7468 6520 6172 7261 7920 6973   of the array is
+000046b0: 2061 6e20 7374 7269 6e67 2074 6f20 6772   an string to gr
+000046c0: 6570 2069 6e20 6060 6670 6174 6860 602e  ep in ``fpath``.
+000046d0: 0a20 2020 2060 6070 7265 7065 6e64 6060  .    ``prepend``
+000046e0: 3a20 7374 7269 6e67 0a20 2020 2020 2020  : string.       
+000046f0: 2070 7265 7065 6e64 2073 7472 696e 6720   prepend string 
+00004700: 6060 7072 6570 656e 6460 6020 746f 2065  ``prepend`` to e
+00004710: 6163 6820 6d61 7463 6869 6e67 206c 696e  ach matching lin
+00004720: 652e 0a20 2020 2060 6072 6f6f 7460 603a  e..    ``root``:
+00004730: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
+00004740: 4669 6c65 2074 6f20 6772 6570 2073 686f  File to grep sho
+00004750: 756c 6420 6265 2069 6e20 6060 726f 6f74  uld be in ``root
+00004760: 2f66 7061 7468 6060 2e0a 2020 2020 2222  /fpath``..    ""
+00004770: 220a 2020 2020 6162 735f 7061 7468 203d  ".    abs_path =
+00004780: 206f 732e 7061 7468 2e6a 6f69 6e28 726f   os.path.join(ro
+00004790: 6f74 2c66 7061 7468 290a 2020 2020 6f75  ot,fpath).    ou
+000047a0: 745f 7374 7220 3d20 2727 0a20 2020 2069  t_str = ''.    i
+000047b0: 6620 6f73 2e70 6174 682e 6973 6669 6c65  f os.path.isfile
+000047c0: 2861 6273 5f70 6174 6829 3a0a 2020 2020  (abs_path):.    
+000047d0: 2020 2020 6673 7472 203d 206f 7065 6e28      fstr = open(
+000047e0: 6162 735f 7061 7468 292e 7265 6164 2829  abs_path).read()
+000047f0: 0a0a 2020 2020 2020 2020 666f 7220 6174  ..        for at
+00004800: 7472 2069 6e20 7365 6172 6368 5f61 7272  tr in search_arr
+00004810: 6179 3a0a 2020 2020 2020 2020 2020 2020  ay:.            
+00004820: 6f73 7472 203d 205f 7374 725f 6772 6570  ostr = _str_grep
+00004830: 2866 7374 722c 6174 7472 2c70 7265 7065  (fstr,attr,prepe
+00004840: 6e64 3d70 7265 7065 6e64 290a 0a20 2020  nd=prepend)..   
+00004850: 2020 2020 2020 2020 2069 6620 6f73 7472           if ostr
+00004860: 2021 3d20 2727 3a0a 2020 2020 2020 2020   != '':.        
+00004870: 2020 2020 2020 2020 6f75 745f 7374 7220          out_str 
+00004880: 3d20 6f75 745f 7374 7220 2b20 7072 6570  = out_str + prep
+00004890: 656e 6420 2b20 6f73 7472 2e73 7472 6970  end + ostr.strip
+000048a0: 2829 202b 2027 5c6e 270a 0a20 2020 2072  () + '\n'..    r
+000048b0: 6574 7572 6e20 6f75 745f 7374 722e 7273  eturn out_str.rs
+000048c0: 7472 6970 2829 0a0a 0a64 6566 2070 6172  trip()...def par
+000048d0: 656e 745f 6c61 7474 6963 655f 746f 5f61  ent_lattice_to_a
+000048e0: 7461 7428 706c 6174 2c20 6f75 745f 666e  tat(plat, out_fn
+000048f0: 616d 653d 226c 6174 2e69 6e22 2c20 666f  ame="lat.in", fo
+00004900: 725f 7374 7220 3d20 4661 6c73 6529 3a0a  r_str = False):.
+00004910: 2020 2020 2222 2253 6572 6961 6c69 7a65      """Serialize
+00004920: 7320 5061 7265 6e74 4c61 7474 6963 6520  s ParentLattice 
+00004930: 6f62 6a65 6374 2074 6f20 4154 4154 2069  object to ATAT i
+00004940: 6e70 7574 2066 696c 650a 0a20 2020 202a  nput file..    *
+00004950: 2a50 6172 616d 6574 6572 733a 2a2a 0a0a  *Parameters:**..
+00004960: 2020 2020 6060 706c 6174 6060 3a20 5061      ``plat``: Pa
+00004970: 7265 6e74 4c61 7474 6963 6520 6f62 6a65  rentLattice obje
+00004980: 6374 0a20 2020 2020 2020 2050 6172 656e  ct.        Paren
+00004990: 744c 6174 7469 6365 206f 626a 6563 7420  tLattice object 
+000049a0: 746f 2062 6520 7365 7269 616c 697a 6564  to be serialized
+000049b0: 0a20 2020 2060 606f 7574 5f66 6e61 6d65  .    ``out_fname
+000049c0: 6060 3a20 7374 7269 6e67 0a20 2020 2020  ``: string.     
+000049d0: 2020 204f 7574 7075 7420 6669 6c65 2070     Output file p
+000049e0: 6174 680a 2020 2020 2222 220a 2020 2020  ath.    """.    
+000049f0: 6365 6c6c 203d 2070 6c61 742e 6765 745f  cell = plat.get_
+00004a00: 6365 6c6c 2829 0a20 2020 2070 6f73 6974  cell().    posit
+00004a10: 696f 6e73 203d 2070 6c61 742e 6765 745f  ions = plat.get_
+00004a20: 7363 616c 6564 5f70 6f73 6974 696f 6e73  scaled_positions
+00004a30: 2829 0a20 2020 2069 6620 666f 725f 7374  ().    if for_st
+00004a40: 723a 0a20 2020 2020 2020 2073 6974 6573  r:.        sites
+00004a50: 203d 2070 6c61 742e 6765 745f 6174 6f6d   = plat.get_atom
+00004a60: 6963 5f6e 756d 6265 7273 2829 0a20 2020  ic_numbers().   
+00004a70: 2065 6c73 653a 0a20 2020 2020 2020 2073   else:.        s
+00004a80: 6974 6573 203d 2070 6c61 742e 6765 745f  ites = plat.get_
+00004a90: 7369 7465 7328 290a 0a20 2020 2066 203d  sites()..    f =
+00004aa0: 206f 7065 6e28 6f75 745f 666e 616d 652c   open(out_fname,
+00004ab0: 2777 2b27 290a 0a20 2020 2066 6f72 2063  'w+')..    for c
+00004ac0: 656c 6c76 2069 6e20 6365 6c6c 3a0a 2020  ellv in cell:.  
+00004ad0: 2020 2020 2020 662e 7772 6974 6528 7522        f.write(u"
+00004ae0: 2532 2e31 3266 5c74 2532 2e31 3266 5c74  %2.12f\t%2.12f\t
+00004af0: 2532 2e31 3266 5c6e 2225 2863 656c 6c76  %2.12f\n"%(cellv
+00004b00: 5b30 5d2c 6365 6c6c 765b 315d 2c63 656c  [0],cellv[1],cel
+00004b10: 6c76 5b32 5d29 290a 0a20 2020 2066 2e77  lv[2]))..    f.w
+00004b20: 7269 7465 2875 2231 2e30 3030 3030 3030  rite(u"1.0000000
+00004b30: 3030 3030 305c 7430 2e30 3030 3030 3030  00000\t0.0000000
+00004b40: 3030 3030 305c 7430 2e30 3030 3030 3030  00000\t0.0000000
+00004b50: 3030 3030 305c 6e22 290a 2020 2020 662e  00000\n").    f.
+00004b60: 7772 6974 6528 7522 302e 3030 3030 3030  write(u"0.000000
+00004b70: 3030 3030 3030 5c74 312e 3030 3030 3030  000000\t1.000000
+00004b80: 3030 3030 3030 5c74 302e 3030 3030 3030  000000\t0.000000
+00004b90: 3030 3030 3030 5c6e 2229 0a20 2020 2066  000000\n").    f
+00004ba0: 2e77 7269 7465 2875 2230 2e30 3030 3030  .write(u"0.00000
+00004bb0: 3030 3030 3030 305c 7430 2e30 3030 3030  0000000\t0.00000
+00004bc0: 3030 3030 3030 305c 7431 2e30 3030 3030  0000000\t1.00000
+00004bd0: 3030 3030 3030 305c 6e22 290a 0a20 2020  0000000\n")..   
+00004be0: 2066 6f72 2069 2c70 6f73 2069 6e20 656e   for i,pos in en
+00004bf0: 756d 6572 6174 6528 706f 7369 7469 6f6e  umerate(position
+00004c00: 7329 3a0a 2020 2020 2020 2020 7374 7269  s):.        stri
+00004c10: 203d 2075 2225 322e 3132 665c 7425 322e   = u"%2.12f\t%2.
+00004c20: 3132 665c 7425 322e 3132 665c 7422 2528  12f\t%2.12f\t"%(
+00004c30: 706f 735b 305d 2c70 6f73 5b31 5d2c 706f  pos[0],pos[1],po
+00004c40: 735b 325d 290a 2020 2020 2020 2020 6966  s[2]).        if
+00004c50: 2066 6f72 5f73 7472 3a0a 2020 2020 2020   for_str:.      
+00004c60: 2020 2020 2020 7374 7269 203d 2073 7472        stri = str
+00004c70: 6920 2b20 2225 735c 6e22 2563 735b 7369  i + "%s\n"%cs[si
+00004c80: 7465 735b 695d 5d0a 2020 2020 2020 2020  tes[i]].        
+00004c90: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00004ca0: 2020 6966 206c 656e 2873 6974 6573 5b69    if len(sites[i
+00004cb0: 5d29 3e31 3a0a 2020 2020 2020 2020 2020  ])>1:.          
+00004cc0: 2020 2020 2020 666f 7220 7a20 696e 2073        for z in s
+00004cd0: 6974 6573 5b69 5d5b 3a2d 315d 3a0a 2020  ites[i][:-1]:.  
+00004ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cf0: 2020 7374 7269 203d 2073 7472 6920 2b20    stri = stri + 
+00004d00: 2225 732c 2225 6373 5b7a 5d0a 2020 2020  "%s,"%cs[z].    
+00004d10: 2020 2020 2020 2020 7374 7269 203d 2073          stri = s
+00004d20: 7472 6920 2b20 2225 735c 6e22 2563 735b  tri + "%s\n"%cs[
+00004d30: 7369 7465 735b 695d 5b2d 315d 5d0a 0a20  sites[i][-1]].. 
+00004d40: 2020 2020 2020 2066 2e77 7269 7465 2873         f.write(s
+00004d50: 7472 6929 0a0a 2020 2020 662e 636c 6f73  tri)..    f.clos
+00004d60: 6528 290a 0a63 6c61 7373 2045 7870 6f6e  e()..class Expon
+00004d70: 656e 7469 616c 2829 3a0a 2020 2020 2222  ential():.    ""
+00004d80: 2242 6173 6963 2065 7870 6f6e 656e 7469  "Basic exponenti
+00004d90: 616c 206f 626a 6563 7420 6f66 2074 7970  al object of typ
+00004da0: 6520 6060 636f 6566 6669 6369 656e 7460  e ``coefficient`
+00004db0: 6020 2a20 6060 7860 6020 5e20 6060 6578  ` * ``x`` ^ ``ex
+00004dc0: 706f 6e65 6e74 6060 202e 204e 756d 6572  ponent`` . Numer
+00004dd0: 6963 616c 6c79 2065 7661 6c75 6574 6564  ically evalueted
+00004de0: 2075 7369 6e67 2074 6865 206d 6574 686f   using the metho
+00004df0: 6420 6060 6576 616c 7561 7465 6060 2028  d ``evaluate`` (
+00004e00: 2060 6078 6060 2029 202e 0a0a 2020 2020   ``x`` ) ...    
+00004e10: 2a2a 5061 7261 6d65 7465 7273 3a2a 2a0a  **Parameters:**.
+00004e20: 0a20 2020 2060 6065 7870 6f6e 656e 7460  .    ``exponent`
+00004e30: 603a 2065 7870 6f6e 656e 7420 6f66 2074  `: exponent of t
+00004e40: 6865 2065 7870 6f6e 656e 7469 616c 0a0a  he exponential..
+00004e50: 2020 2020 6060 636f 6566 6669 6369 656e      ``coefficien
+00004e60: 7460 603a 2063 6f65 6666 6963 6965 6e74  t``: coefficient
+00004e70: 206f 6620 7468 6520 6578 706f 6e65 6e74   of the exponent
+00004e80: 6961 6c0a 0a20 2020 2022 2222 0a0a 2020  ial..    """..  
+00004e90: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+00004ea0: 656c 662c 2065 7870 6f6e 656e 742c 2063  elf, exponent, c
+00004eb0: 6f65 6666 6963 6965 6e74 203d 2031 293a  oefficient = 1):
+00004ec0: 0a20 2020 2020 2020 2073 656c 662e 6578  .        self.ex
+00004ed0: 706f 6e65 6e74 203d 2065 7870 6f6e 656e  ponent = exponen
+00004ee0: 740a 2020 2020 2020 2020 7365 6c66 2e63  t.        self.c
+00004ef0: 6f65 6666 6963 6965 6e74 203d 2063 6f65  oefficient = coe
+00004f00: 6666 6963 6965 6e74 0a0a 2020 2020 6465  fficient..    de
+00004f10: 6620 6576 616c 7561 7465 2873 656c 662c  f evaluate(self,
+00004f20: 2078 293a 0a20 2020 2020 2020 2072 6574   x):.        ret
+00004f30: 7572 6e20 7365 6c66 2e63 6f65 6666 6963  urn self.coeffic
+00004f40: 6965 6e74 202a 206e 702e 706f 7765 7228  ient * np.power(
+00004f50: 782c 7365 6c66 2e65 7870 6f6e 656e 7429  x,self.exponent)
+00004f60: 0a0a 2020 2020 6465 6620 6469 7669 6465  ..    def divide
+00004f70: 5f73 6361 6c61 7228 7365 6c66 2c20 7661  _scalar(self, va
+00004f80: 6c75 6529 3a0a 2020 2020 2020 2020 7365  lue):.        se
+00004f90: 6c66 2e63 6f65 6666 6963 6965 6e74 203d  lf.coefficient =
+00004fa0: 2073 656c 662e 636f 6566 6669 6369 656e   self.coefficien
+00004fb0: 7420 2f20 7661 6c75 650a 0a20 2020 2064  t / value..    d
+00004fc0: 6566 206d 756c 7469 706c 795f 7363 616c  ef multiply_scal
+00004fd0: 6172 2873 656c 662c 2073 6361 6c61 7229  ar(self, scalar)
+00004fe0: 3a0a 2020 2020 2020 2020 7365 6c66 2e63  :.        self.c
+00004ff0: 6f65 6666 6963 6965 6e74 203d 2073 656c  oefficient = sel
+00005000: 662e 636f 6566 6669 6369 656e 7420 2a20  f.coefficient * 
+00005010: 7363 616c 6172 0a0a 0a63 6c61 7373 2050  scalar...class P
+00005020: 6f6c 796e 6f6d 6961 6c46 756e 6374 696f  olynomialFunctio
+00005030: 6e28 293a 0a20 2020 2022 2222 506f 6c79  n():.    """Poly
+00005040: 6e6f 6d69 616c 2066 756e 6374 696f 6e2c  nomial function,
+00005050: 2062 7569 6c64 2066 726f 6d20 6060 4578   build from ``Ex
+00005060: 706f 6e65 6e74 6961 6c28 2960 6020 2e0a  ponential()`` ..
+00005070: 2020 2020 2222 220a 0a0a 2020 2020 6465      """...    de
+00005080: 6620 5f5f 696e 6974 5f5f 2873 656c 6629  f __init__(self)
+00005090: 3a0a 2020 2020 2020 2020 7365 6c66 2e65  :.        self.e
+000050a0: 7870 6f6e 656e 7469 616c 7320 3d20 5b5d  xponentials = []
+000050b0: 0a0a 2020 2020 6465 6620 6164 645f 6578  ..    def add_ex
+000050c0: 706f 6e65 6e74 6961 6c28 7365 6c66 2c20  ponential(self, 
+000050d0: 6f72 6465 722c 2063 6f65 6666 6963 6965  order, coefficie
+000050e0: 6e74 203d 2031 293a 0a20 2020 2020 2020  nt = 1):.       
+000050f0: 2069 6e5f 7375 6d20 3d20 4661 6c73 650a   in_sum = False.
+00005100: 2020 2020 2020 2020 666f 7220 6578 706f          for expo
+00005110: 6e65 6e74 6961 6c20 696e 2073 656c 662e  nential in self.
+00005120: 6578 706f 6e65 6e74 6961 6c73 3a0a 2020  exponentials:.  
+00005130: 2020 2020 2020 2020 2020 6966 2065 7870            if exp
+00005140: 6f6e 656e 7469 616c 2e65 7870 6f6e 656e  onential.exponen
+00005150: 7420 3d3d 206f 7264 6572 3a0a 2020 2020  t == order:.    
+00005160: 2020 2020 2020 2020 2020 2020 6578 706f              expo
+00005170: 6e65 6e74 6961 6c2e 636f 6566 6669 6369  nential.coeffici
+00005180: 656e 7420 2b3d 2063 6f65 6666 6963 6965  ent += coefficie
+00005190: 6e74 0a20 2020 2020 2020 2020 2020 2020  nt.             
+000051a0: 2020 2069 6e5f 7375 6d20 3d20 5472 7565     in_sum = True
+000051b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000051c0: 2062 7265 616b 0a20 2020 2020 2020 2069   break.        i
+000051d0: 6620 6e6f 7420 696e 5f73 756d 3a0a 2020  f not in_sum:.  
+000051e0: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
+000051f0: 7870 6f6e 656e 7469 616c 732e 6170 7065  xponentials.appe
+00005200: 6e64 2845 7870 6f6e 656e 7469 616c 286f  nd(Exponential(o
+00005210: 7264 6572 2c20 636f 6566 6669 6369 656e  rder, coefficien
+00005220: 7429 290a 0a20 2020 2064 6566 2063 6c65  t))..    def cle
+00005230: 6172 5f65 7870 6f6e 656e 7469 616c 7328  ar_exponentials(
+00005240: 7365 6c66 293a 0a20 2020 2020 2020 2066  self):.        f
+00005250: 6f72 2065 7870 6f6e 656e 7469 616c 2069  or exponential i
+00005260: 6e20 7365 6c66 2e65 7870 6f6e 656e 7469  n self.exponenti
+00005270: 616c 733a 0a20 2020 2020 2020 2020 2020  als:.           
+00005280: 2069 6620 6162 7328 6578 706f 6e65 6e74   if abs(exponent
+00005290: 6961 6c2e 636f 6566 6669 6369 656e 7429  ial.coefficient)
+000052a0: 203c 2031 302a 2a28 2d31 3529 3a0a 2020   < 10**(-15):.  
+000052b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000052c0: 6c66 2e65 7870 6f6e 656e 7469 616c 732e  lf.exponentials.
+000052d0: 7265 6d6f 7665 2865 7870 6f6e 656e 7469  remove(exponenti
+000052e0: 616c 290a 0a20 2020 2064 6566 2065 7661  al)..    def eva
+000052f0: 6c75 6174 6528 7365 6c66 2c20 7829 3a0a  luate(self, x):.
+00005300: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
+00005310: 300a 2020 2020 2020 2020 666f 7220 6578  0.        for ex
+00005320: 706f 6e65 6e74 6961 6c20 696e 2073 656c  ponential in sel
+00005330: 662e 6578 706f 6e65 6e74 6961 6c73 3a0a  f.exponentials:.
+00005340: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+00005350: 6520 2b3d 2065 7870 6f6e 656e 7469 616c  e += exponential
+00005360: 2e65 7661 6c75 6174 6528 7829 0a20 2020  .evaluate(x).   
+00005370: 2020 2020 2072 6574 7572 6e20 7661 6c75       return valu
+00005380: 650a 0a20 2020 2064 6566 206e 6f72 6d61  e..    def norma
+00005390: 6c69 7a65 2873 656c 662c 2073 6361 6c61  lize(self, scala
+000053a0: 725f 7072 6f64 7563 742c 206d 293a 0a20  r_product, m):. 
+000053b0: 2020 2020 2020 206c 656e 6774 6820 3d20         length = 
+000053c0: 7363 616c 6172 5f70 726f 6475 6374 2873  scalar_product(s
+000053d0: 656c 662e 6576 616c 7561 7465 2c20 7365  elf.evaluate, se
+000053e0: 6c66 2e65 7661 6c75 6174 652c 206d 290a  lf.evaluate, m).
+000053f0: 2020 2020 2020 2020 6c65 6e67 7468 203d          length =
+00005400: 206e 702e 7371 7274 286c 656e 6774 6829   np.sqrt(length)
+00005410: 0a20 2020 2020 2020 2066 6f72 2065 7870  .        for exp
+00005420: 6f6e 656e 7469 616c 2069 6e20 7365 6c66  onential in self
+00005430: 2e65 7870 6f6e 656e 7469 616c 733a 0a20  .exponentials:. 
+00005440: 2020 2020 2020 2020 2020 2065 7870 6f6e             expon
+00005450: 656e 7469 616c 2e64 6976 6964 655f 7363  ential.divide_sc
+00005460: 616c 6172 286c 656e 6774 6829 0a0a 2020  alar(length)..  
+00005470: 2020 6465 6620 6d75 6c74 6970 6c79 5f73    def multiply_s
+00005480: 6361 6c61 7228 7365 6c66 2c20 7363 616c  calar(self, scal
+00005490: 6172 293a 0a20 2020 2020 2020 2066 6f72  ar):.        for
+000054a0: 2065 7870 6f6e 656e 7469 616c 2069 6e20   exponential in 
+000054b0: 7365 6c66 2e65 7870 6f6e 656e 7469 616c  self.exponential
+000054c0: 733a 0a20 2020 2020 2020 2020 2020 2065  s:.            e
+000054d0: 7870 6f6e 656e 7469 616c 2e6d 756c 7469  xponential.multi
+000054e0: 706c 795f 7363 616c 6172 2873 6361 6c61  ply_scalar(scala
+000054f0: 7229 0a0a 2020 2020 6465 6620 6164 645f  r)..    def add_
+00005500: 706f 6c79 6e6f 6d69 616c 5f66 756e 6374  polynomial_funct
+00005510: 696f 6e28 7365 6c66 2c20 706f 6c79 6e6f  ion(self, polyno
+00005520: 6d69 616c 5f66 756e 6374 696f 6e29 3a0a  mial_function):.
+00005530: 2020 2020 2020 2020 666f 7220 6578 706f          for expo
+00005540: 6e65 6e74 6961 6c20 696e 2070 6f6c 796e  nential in polyn
+00005550: 6f6d 6961 6c5f 6675 6e63 7469 6f6e 2e65  omial_function.e
+00005560: 7870 6f6e 656e 7469 616c 733a 0a20 2020  xponentials:.   
+00005570: 2020 2020 2020 2020 2073 656c 662e 6164           self.ad
+00005580: 645f 6578 706f 6e65 6e74 6961 6c28 6578  d_exponential(ex
+00005590: 706f 6e65 6e74 6961 6c2e 6578 706f 6e65  ponential.expone
+000055a0: 6e74 2c20 6578 706f 6e65 6e74 6961 6c2e  nt, exponential.
+000055b0: 636f 6566 6669 6369 656e 7429 0a0a 2020  coefficient)..  
+000055c0: 2020 6465 6620 7072 696e 745f 706f 6c79    def print_poly
+000055d0: 6e6f 6d69 616c 2873 656c 6629 3a0a 2020  nomial(self):.  
+000055e0: 2020 2020 2020 6f75 7473 7472 696e 6720        outstring 
+000055f0: 3d20 2727 0a20 2020 2020 2020 2066 6f72  = ''.        for
+00005600: 2065 7870 6f6e 656e 7469 616c 2069 6e20   exponential in 
+00005610: 7365 6c66 2e65 7870 6f6e 656e 7469 616c  self.exponential
+00005620: 733a 0a20 2020 2020 2020 2020 2020 206f  s:.            o
+00005630: 7574 7374 7269 6e67 202b 3d20 7374 7228  utstring += str(
+00005640: 6578 706f 6e65 6e74 6961 6c2e 636f 6566  exponential.coef
+00005650: 6669 6369 656e 7429 202b 2027 202a 2020  ficient) + ' *  
+00005660: 785e 2720 2b20 7374 7228 6578 706f 6e65  x^' + str(expone
+00005670: 6e74 6961 6c2e 6578 706f 6e65 6e74 2920  ntial.exponent) 
+00005680: 2b20 2720 2b20 270a 2020 2020 2020 2020  + ' + '.        
+00005690: 6f75 7473 7472 696e 6720 3d20 6f75 7473  outstring = outs
+000056a0: 7472 696e 675b 3a2d 335d 0a20 2020 2020  tring[:-3].     
+000056b0: 2020 2070 7269 6e74 286f 7574 7374 7269     print(outstri
+000056c0: 6e67 290a 0a0a 636c 6173 7320 506f 6c79  ng)...class Poly
+000056d0: 6e6f 6d69 616c 4261 7369 7328 293a 0a20  nomialBasis():. 
+000056e0: 2020 2022 2222 506f 6c79 6e6f 6d69 616c     """Polynomial
+000056f0: 2062 6173 6973 2c20 636f 6e73 7472 7563   basis, construc
+00005700: 7465 6420 6672 6f6d 2073 6576 6572 616c  ted from several
+00005710: 2060 6050 6f6c 796e 6f6d 6961 6c46 756e   ``PolynomialFun
+00005720: 6374 696f 6e28 2960 602e 0a20 2020 2043  ction()``..    C
+00005730: 6f6e 7374 7275 6374 7320 6f72 7468 6f6e  onstructs orthon
+00005740: 6f72 6d61 6c20 6261 7369 7320 7365 7473  ormal basis sets
+00005750: 2075 7369 6e67 2060 6073 6361 6c63 6172   using ``scalcar
+00005760: 5f70 726f 6475 6374 6060 202e 0a20 2020  _product`` ..   
+00005770: 2057 6865 6e20 696e 6974 6961 6c69 7a65   When initialize
+00005780: 642c 2061 6c6c 206f 7274 686f 6e6f 726d  d, all orthonorm
+00005790: 616c 2062 6173 6973 2073 6574 7320 746f  al basis sets to
+000057a0: 2074 6865 206f 7264 6572 2060 606d 6178   the order ``max
+000057b0: 5f6f 7264 6572 6060 2061 7265 2067 656e  _order`` are gen
+000057c0: 6572 6174 6564 2e0a 0a20 2020 202a 2a50  erated...    **P
+000057d0: 6172 616d 6574 6572 732a 2a0a 0a20 2020  arameters**..   
+000057e0: 2060 606d 6178 5f6f 7264 6572 6060 3a20   ``max_order``: 
+000057f0: 4d61 7869 6d61 6c20 6f72 6465 7220 746f  Maximal order to
+00005800: 2077 6869 6368 2074 6865 2062 6173 6973   which the basis
+00005810: 2073 6574 2069 7320 696e 6974 6961 6c69   set is initiali
+00005820: 7a65 642e 0a0a 2020 2020 6060 7379 6d6d  zed...    ``symm
+00005830: 6574 7269 6360 603a 2044 6566 696e 6573  etric``: Defines
+00005840: 2069 6620 7468 6520 7363 616c 6172 2070   if the scalar p
+00005850: 726f 6475 6374 2075 7365 7320 7369 676d  roduct uses sigm
+00005860: 6173 2073 796d 6d65 7472 697a 6564 2061  as symmetrized a
+00005870: 726f 756e 6420 3020 6f72 2061 7363 656e  round 0 or ascen
+00005880: 6469 6e67 2066 726f 6d20 302e 0a0a 2020  ding from 0...  
+00005890: 2020 2222 220a 0a20 2020 2064 6566 205f    """..    def _
+000058a0: 5f69 6e69 745f 5f28 7365 6c66 2c20 6d61  _init__(self, ma
+000058b0: 785f 6f72 6465 7220 3d20 3130 2c20 7379  x_order = 10, sy
+000058c0: 6d6d 6574 7269 6320 3d20 4661 6c73 6529  mmetric = False)
+000058d0: 3a0a 2020 2020 2020 2020 7365 6c66 2e6d  :.        self.m
+000058e0: 203d 206d 6178 5f6f 7264 6572 0a20 2020   = max_order.   
+000058f0: 2020 2020 2073 656c 662e 7379 6d6d 6574       self.symmet
+00005900: 7269 6320 3d20 7379 6d6d 6574 7269 630a  ric = symmetric.
+00005910: 2020 2020 2020 2020 7365 6c66 2e62 6173          self.bas
+00005920: 6973 5f66 756e 6374 696f 6e5f 7365 7420  is_function_set 
+00005930: 3d20 7b7d 0a20 2020 2020 2020 2066 6f72  = {}.        for
+00005940: 206f 7264 6572 2069 6e20 7261 6e67 6528   order in range(
+00005950: 312c 6d61 785f 6f72 6465 722b 3129 3a0a  1,max_order+1):.
+00005960: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00005970: 2e62 6173 6973 5f66 756e 6374 696f 6e5f  .basis_function_
+00005980: 7365 745b 7374 7228 6f72 6465 7229 5d20  set[str(order)] 
+00005990: 3d20 7365 6c66 2e63 6f6e 7374 7275 6374  = self.construct
+000059a0: 286f 7264 6572 290a 0a20 2020 2064 6566  (order)..    def
+000059b0: 2063 6f6e 7374 7275 6374 2873 656c 662c   construct(self,
+000059c0: 206d 293a 0a20 2020 2020 2020 2062 6173   m):.        bas
+000059d0: 6973 5f66 756e 6374 696f 6e73 203d 205b  is_functions = [
+000059e0: 5d0a 2020 2020 2020 2020 666f 7220 6465  ].        for de
+000059f0: 6772 6565 2069 6e20 7261 6e67 6528 6d29  gree in range(m)
+00005a00: 3a0a 2020 2020 2020 2020 2020 2020 6e65  :.            ne
+00005a10: 775f 6675 6e63 7469 6f6e 203d 2050 6f6c  w_function = Pol
+00005a20: 796e 6f6d 6961 6c46 756e 6374 696f 6e28  ynomialFunction(
+00005a30: 290a 2020 2020 2020 2020 2020 2020 6e65  ).            ne
+00005a40: 775f 6675 6e63 7469 6f6e 2e61 6464 5f65  w_function.add_e
+00005a50: 7870 6f6e 656e 7469 616c 2864 6567 7265  xponential(degre
+00005a60: 6529 0a20 2020 2020 2020 2020 2020 2063  e).            c
+00005a70: 6869 203d 2045 7870 6f6e 656e 7469 616c  hi = Exponential
+00005a80: 2864 6567 7265 6529 0a20 2020 2020 2020  (degree).       
+00005a90: 2020 2020 2066 6f72 2062 6173 6973 5f66       for basis_f
+00005aa0: 756e 6374 696f 6e20 696e 2062 6173 6973  unction in basis
+00005ab0: 5f66 756e 6374 696f 6e73 3a0a 2020 2020  _functions:.    
+00005ac0: 2020 2020 2020 2020 2020 2020 6f76 6572              over
+00005ad0: 6c61 7020 3d20 7365 6c66 2e73 6361 6c61  lap = self.scala
+00005ae0: 725f 7072 6f64 7563 7428 6261 7369 735f  r_product(basis_
+00005af0: 6675 6e63 7469 6f6e 2e65 7661 6c75 6174  function.evaluat
+00005b00: 652c 6368 692e 6576 616c 7561 7465 2c20  e,chi.evaluate, 
+00005b10: 6d29 0a20 2020 2020 2020 2020 2020 2020  m).             
+00005b20: 2020 206f 7665 726c 6170 203d 206f 7665     overlap = ove
+00005b30: 726c 6170 202a 2028 2d31 290a 2020 2020  rlap * (-1).    
+00005b40: 2020 2020 2020 2020 2020 2020 7375 6d6d              summ
+00005b50: 616e 6420 3d20 636f 7079 2e64 6565 7063  and = copy.deepc
+00005b60: 6f70 7928 6261 7369 735f 6675 6e63 7469  opy(basis_functi
+00005b70: 6f6e 290a 2020 2020 2020 2020 2020 2020  on).            
+00005b80: 2020 2020 7375 6d6d 616e 642e 6d75 6c74      summand.mult
+00005b90: 6970 6c79 5f73 6361 6c61 7228 6f76 6572  iply_scalar(over
+00005ba0: 6c61 7029 0a20 2020 2020 2020 2020 2020  lap).           
+00005bb0: 2020 2020 206e 6577 5f66 756e 6374 696f       new_functio
+00005bc0: 6e2e 6164 645f 706f 6c79 6e6f 6d69 616c  n.add_polynomial
+00005bd0: 5f66 756e 6374 696f 6e28 7375 6d6d 616e  _function(summan
+00005be0: 6429 0a20 2020 2020 2020 2020 2020 206e  d).            n
+00005bf0: 6577 5f66 756e 6374 696f 6e2e 6e6f 726d  ew_function.norm
+00005c00: 616c 697a 6528 7365 6c66 2e73 6361 6c61  alize(self.scala
+00005c10: 725f 7072 6f64 7563 742c 206d 290a 2020  r_product, m).  
+00005c20: 2020 2020 2020 2020 2020 6e65 775f 6675            new_fu
+00005c30: 6e63 7469 6f6e 2e63 6c65 6172 5f65 7870  nction.clear_exp
+00005c40: 6f6e 656e 7469 616c 7328 290a 2020 2020  onentials().    
+00005c50: 2020 2020 2020 2020 6261 7369 735f 6675          basis_fu
+00005c60: 6e63 7469 6f6e 732e 6170 7065 6e64 286e  nctions.append(n
+00005c70: 6577 5f66 756e 6374 696f 6e29 0a20 2020  ew_function).   
+00005c80: 2020 2020 2072 6574 7572 6e20 6261 7369       return basi
+00005c90: 735f 6675 6e63 7469 6f6e 730a 0a20 2020  s_functions..   
+00005ca0: 2064 6566 2073 6361 6c61 725f 7072 6f64   def scalar_prod
+00005cb0: 7563 7428 7365 6c66 2c20 6675 6e63 7469  uct(self, functi
+00005cc0: 6f6e 312c 2066 756e 6374 696f 6e32 2c20  on1, function2, 
+00005cd0: 6d29 3a0a 2020 2020 2020 2020 2222 220a  m):.        """.
+00005ce0: 2020 2020 2020 2020 7265 7475 726e 7320          returns 
+00005cf0: 7468 6520 7265 7375 6c74 206f 6620 7468  the result of th
+00005d00: 6520 7363 616c 6172 2070 726f 6475 6374  e scalar product
+00005d10: 2031 2f6d 2073 756d 5f7b 7369 676d 617d   1/m sum_{sigma}
+00005d20: 2066 5f31 2873 6967 6d61 2920 2a20 665f   f_1(sigma) * f_
+00005d30: 3228 7369 676d 6129 0a20 2020 2020 2020  2(sigma).       
+00005d40: 2022 2222 0a20 2020 2020 2020 2073 6361   """.        sca
+00005d50: 6c69 6e67 203d 2031 202f 206d 0a20 2020  ling = 1 / m.   
+00005d60: 2020 2020 2069 6620 7365 6c66 2e73 796d       if self.sym
+00005d70: 6d65 7472 6963 3a0a 2020 2020 2020 2020  metric:.        
+00005d80: 2020 2020 7369 676d 6173 203d 205b 7820      sigmas = [x 
+00005d90: 666f 7220 7820 696e 2072 616e 6765 282d  for x in range(-
+00005da0: 696e 7428 6d2f 3229 2c20 696e 7428 6d2f  int(m/2), int(m/
+00005db0: 3229 2b31 295d 0a20 2020 2020 2020 2020  2)+1)].         
+00005dc0: 2020 2069 6620 6d20 2520 3220 3d3d 2030     if m % 2 == 0
+00005dd0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00005de0: 2020 7369 676d 6173 2e72 656d 6f76 6528    sigmas.remove(
+00005df0: 3029 0a20 2020 2020 2020 2065 6c73 653a  0).        else:
+00005e00: 0a20 2020 2020 2020 2020 2020 2073 6967  .            sig
+00005e10: 6d61 7320 3d20 5b78 2066 6f72 2078 2069  mas = [x for x i
+00005e20: 6e20 7261 6e67 6528 6d29 5d0a 2020 2020  n range(m)].    
+00005e30: 2020 2020 7363 616c 6172 5f70 726f 6475      scalar_produ
+00005e40: 6374 203d 2030 0a20 2020 2020 2020 2066  ct = 0.        f
+00005e50: 6f72 2073 6967 6d61 2069 6e20 7369 676d  or sigma in sigm
+00005e60: 6173 3a0a 2020 2020 2020 2020 2020 2020  as:.            
+00005e70: 7363 616c 6172 5f70 726f 6475 6374 202b  scalar_product +
+00005e80: 3d20 6675 6e63 7469 6f6e 3128 7369 676d  = function1(sigm
+00005e90: 6129 202a 2066 756e 6374 696f 6e32 2873  a) * function2(s
+00005ea0: 6967 6d61 290a 2020 2020 2020 2020 7363  igma).        sc
+00005eb0: 616c 6172 5f70 726f 6475 6374 203d 2073  alar_product = s
+00005ec0: 6361 6c61 725f 7072 6f64 7563 7420 2a20  calar_product * 
+00005ed0: 7363 616c 696e 670a 2020 2020 2020 2020  scaling.        
+00005ee0: 7265 7475 726e 2073 6361 6c61 725f 7072  return scalar_pr
+00005ef0: 6f64 7563 740a 0a20 2020 2064 6566 2070  oduct..    def p
+00005f00: 7269 6e74 5f62 6173 6973 5f66 756e 6374  rint_basis_funct
+00005f10: 696f 6e73 2873 656c 662c 206d 293a 0a20  ions(self, m):. 
+00005f20: 2020 2020 2020 2066 6f72 2066 756e 6374         for funct
+00005f30: 696f 6e20 696e 2073 656c 662e 6261 7369  ion in self.basi
+00005f40: 735f 6675 6e63 7469 6f6e 5f73 6574 5b73  s_function_set[s
+00005f50: 7472 286d 295d 3a0a 2020 2020 2020 2020  tr(m)]:.        
+00005f60: 2020 2020 6675 6e63 7469 6f6e 2e70 7269      function.pri
+00005f70: 6e74 5f70 6f6c 796e 6f6d 6961 6c28 290a  nt_polynomial().
+00005f80: 0a20 2020 2064 6566 2065 7661 6c75 6174  .    def evaluat
+00005f90: 6528 7365 6c66 2c20 616c 7068 612c 2073  e(self, alpha, s
+00005fa0: 6967 6d61 2c20 6d29 3a0a 2020 2020 2020  igma, m):.      
+00005fb0: 2020 6966 206d 203e 2073 656c 662e 6d3a    if m > self.m:
+00005fc0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00005fd0: 662e 6261 7369 735f 6675 6e63 7469 6f6e  f.basis_function
+00005fe0: 5f73 6574 5b73 7472 286d 295d 203d 2073  _set[str(m)] = s
+00005ff0: 656c 662e 636f 6e73 7472 7563 7428 6d29  elf.construct(m)
+00006000: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00006010: 7365 6c66 2e62 6173 6973 5f66 756e 6374  self.basis_funct
+00006020: 696f 6e5f 7365 745b 7374 7228 6d29 5d5b  ion_set[str(m)][
+00006030: 696e 7428 616c 7068 6129 5d2e 6576 616c  int(alpha)].eval
+00006040: 7561 7465 2873 6967 6d61 290a 0a0a 6465  uate(sigma)...de
+00006050: 6620 706f 7070 7573 6828 782c 2076 616c  f poppush(x, val
+00006060: 293a 0a20 2020 2022 2222 4c65 6674 2d73  ):.    """Left-s
+00006070: 6869 6674 2061 7272 6179 206f 6e65 2070  hift array one p
+00006080: 6f73 6974 696f 6e20 616e 6420 7772 6974  osition and writ
+00006090: 6573 206e 6577 2076 616c 7565 2074 6f20  es new value to 
+000060a0: 7468 6520 7269 6768 742e 2052 6574 7572  the right. Retur
+000060b0: 6e73 2061 7665 7261 6765 2e0a 0a20 2020  ns average...   
+000060c0: 202a 2a50 6172 616d 6574 6572 733a 2a2a   **Parameters:**
+000060d0: 0a20 2020 2060 6078 6060 3a20 6e75 6d70  .    ``x``: nump
+000060e0: 7920 6172 7261 790a 2020 2020 6060 7661  y array.    ``va
+000060f0: 6c60 603a 2069 6e74 206f 7220 666c 6f61  l``: int or floa
+00006100: 740a 2020 2020 2222 220a 2020 2020 785b  t.    """.    x[
+00006110: 3a2d 315d 203d 2078 5b31 3a5d 3b20 785b  :-1] = x[1:]; x[
+00006120: 2d31 5d20 3d20 7661 6c0a 2020 2020 7265  -1] = val.    re
+00006130: 7475 726e 2078 2e6d 6561 6e28 290a 0a64  turn x.mean()..d
+00006140: 6566 2073 6f72 745f 6174 6f6d 7328 6174  ef sort_atoms(at
+00006150: 6f6d 732c 206b 6579 203d 2028 322c 312c  oms, key = (2,1,
+00006160: 3029 293a 0a20 2020 2022 2222 5265 7475  0)):.    """Retu
+00006170: 726e 2061 746f 6d73 206f 626a 6563 7420  rn atoms object 
+00006180: 7769 7468 2073 6f72 7465 6420 6174 6f6d  with sorted atom
+00006190: 6963 2063 6f6f 7264 696e 6174 6573 0a0a  ic coordinates..
+000061a0: 2020 2020 5468 6520 6465 6661 756c 7420      The default 
+000061b0: 736f 7274 696e 6720 6973 3a20 696e 6372  sorting is: incr
+000061c0: 6561 7369 6e67 207a 2d63 6f6f 7264 696e  easing z-coordin
+000061d0: 6174 6520 6669 7273 742c 2069 6e63 7265  ate first, incre
+000061e0: 6173 696e 670a 2020 2020 792d 636f 6f72  asing.    y-coor
+000061f0: 6469 6e61 7465 2073 6563 6f6e 642c 2069  dinate second, i
+00006200: 6e63 7265 6173 696e 6720 782d 636f 6f72  ncreasing x-coor
+00006210: 6469 6e61 7465 2074 6869 7264 2e20 5573  dinate third. Us
+00006220: 6566 756c 2074 6f20 6765 740a 2020 2020  eful to get.    
+00006230: 7765 6c6c 206f 7264 6572 6564 2073 6c61  well ordered sla
+00006240: 6220 7374 7275 6374 7572 6573 2c20 666f  b structures, fo
+00006250: 7220 696e 7374 616e 6365 2e20 536f 7274  r instance. Sort
+00006260: 696e 6720 6361 6e20 6265 2063 6861 6e67  ing can be chang
+00006270: 6564 0a20 2020 2062 7920 6170 7072 6f70  ed.    by approp
+00006280: 7269 6174 656c 7920 7365 7474 696e 6720  riately setting 
+00006290: 7468 6520 6060 6b65 7960 6020 6172 6775  the ``key`` argu
+000062a0: 6d65 6e74 2c20 7769 7468 2074 6865 2073  ment, with the s
+000062b0: 616d 650a 2020 2020 6566 6665 6374 2061  ame.    effect a
+000062c0: 7320 696e 3a3a 0a0a 2020 2020 2020 2020  s in::..        
+000062d0: 6672 6f6d 206f 7065 7261 746f 7220 696d  from operator im
+000062e0: 706f 7274 2069 7465 6d67 6574 7465 720a  port itemgetter.
+000062f0: 2020 2020 2020 2020 7370 203d 2073 6f72          sp = sor
+00006300: 7465 6428 702c 206b 6579 3d69 7465 6d67  ted(p, key=itemg
+00006310: 6574 7465 7228 322c 312c 3029 290a 0a20  etter(2,1,0)).. 
+00006320: 2020 2077 6865 7265 2070 2069 7320 6120     where p is a 
+00006330: 4e78 3320 6172 7261 7920 6f66 2076 6563  Nx3 array of vec
+00006340: 746f 7220 636f 6f72 6469 6e61 7465 732e  tor coordinates.
+00006350: 0a20 2020 2022 2222 0a20 2020 2069 6620  .    """.    if 
+00006360: 6b65 7920 6973 204e 6f6e 653a 0a20 2020  key is None:.   
+00006370: 2020 2020 2072 6574 7572 6e20 6174 6f6d       return atom
+00006380: 730a 2020 2020 656c 7365 3a0a 2020 2020  s.    else:.    
+00006390: 2020 2020 6e72 7320 3d20 6174 6f6d 732e      nrs = atoms.
+000063a0: 6765 745f 6174 6f6d 6963 5f6e 756d 6265  get_atomic_numbe
+000063b0: 7273 2829 0a20 2020 2020 2020 2070 6f73  rs().        pos
+000063c0: 7320 3d20 6174 6f6d 732e 6765 745f 706f  s = atoms.get_po
+000063d0: 7369 7469 6f6e 7328 290a 2020 2020 2020  sitions().      
+000063e0: 2020 706e 203d 205b 5d0a 2020 2020 2020    pn = [].      
+000063f0: 2020 666f 7220 702c 6e20 696e 207a 6970    for p,n in zip
+00006400: 2870 6f73 732c 6e72 7329 3a0a 2020 2020  (poss,nrs):.    
+00006410: 2020 2020 2020 2020 706e 2e61 7070 656e          pn.appen
+00006420: 6428 5b70 5b30 5d2c 705b 315d 2c70 5b32  d([p[0],p[1],p[2
+00006430: 5d2c 6e5d 290a 2020 2020 2020 2020 6672  ],n]).        fr
+00006440: 6f6d 206f 7065 7261 746f 7220 696d 706f  om operator impo
+00006450: 7274 2069 7465 6d67 6574 7465 720a 2020  rt itemgetter.  
+00006460: 2020 2020 2020 696d 706f 7274 206e 756d        import num
+00006470: 7079 2061 7320 6e70 0a20 2020 2020 2020  py as np.       
+00006480: 205f 706e 203d 2073 6f72 7465 6428 706e   _pn = sorted(pn
+00006490: 2c20 6b65 793d 6974 656d 6765 7474 6572  , key=itemgetter
+000064a0: 282a 6b65 7929 290a 2020 2020 2020 2020  (*key)).        
+000064b0: 5f70 6f73 7320 3d20 6e70 2e64 656c 6574  _poss = np.delet
+000064c0: 6528 6e70 2e61 7272 6179 285f 706e 292c  e(np.array(_pn),
+000064d0: 332c 3129 0a20 2020 2020 2020 205f 6e72  3,1).        _nr
+000064e0: 7320 3d20 6e70 2e64 656c 6574 6528 6e70  s = np.delete(np
+000064f0: 2e61 7272 6179 285f 706e 292c 5b30 2c31  .array(_pn),[0,1
+00006500: 2c32 5d2c 3129 2e66 6c61 7474 656e 2829  ,2],1).flatten()
+00006510: 0a20 2020 2020 2020 2066 726f 6d20 6173  .        from as
+00006520: 6520 696d 706f 7274 2041 746f 6d73 0a20  e import Atoms. 
+00006530: 2020 2020 2020 2072 6574 7572 6e20 4174         return At
+00006540: 6f6d 7328 706f 7369 7469 6f6e 733d 5f70  oms(positions=_p
+00006550: 6f73 732c 206e 756d 6265 7273 3d5f 6e72  oss, numbers=_nr
+00006560: 732c 2063 656c 6c3d 6174 6f6d 732e 6765  s, cell=atoms.ge
+00006570: 745f 6365 6c6c 2829 2c20 7062 633d 6174  t_cell(), pbc=at
+00006580: 6f6d 732e 6765 745f 7062 6328 2929 0a0a  oms.get_pbc())..
+00006590: 6465 6620 7265 6d6f 7665 5f76 6163 616e  def remove_vacan
+000065a0: 6369 6573 2861 7429 3a0a 2020 2020 2222  cies(at):.    ""
+000065b0: 2252 656d 6f76 6520 6576 6572 7920 4174  "Remove every At
+000065c0: 6f6d 2063 6f6e 7461 696e 696e 6720 2758  om containing 'X
+000065d0: 2720 6173 2073 7065 6369 6573 2073 796d  ' as species sym
+000065e0: 626f 6c20 6f72 2030 2061 7320 6174 6f6d  bol or 0 as atom
+000065f0: 6963 206e 756d 6265 720a 2020 2020 6672  ic number.    fr
+00006600: 6f6d 2061 6e20 4174 6f6d 7320 6f62 6a65  om an Atoms obje
+00006610: 6374 2061 6e64 2072 6574 7572 6e20 7468  ct and return th
+00006620: 6520 7265 7375 6c74 696e 6720 4174 6f6d  e resulting Atom
+00006630: 7320 6f62 6a65 6374 2e0a 0a20 2020 202a  s object...    *
+00006640: 2a50 6172 616d 6574 6572 733a 2a2a 0a20  *Parameters:**. 
+00006650: 2020 2060 6061 7460 603a 2041 746f 6d73     ``at``: Atoms
+00006660: 206f 626a 6563 740a 0a20 2020 202e 2e20   object..    .. 
+00006670: 746f 646f 3a3a 0a20 2020 2020 2020 2066  todo::.        f
+00006680: 696e 6420 636c 6561 6e65 7220 7761 7920  ind cleaner way 
+00006690: 746f 2064 6f20 7468 6973 2e2e 2e0a 2020  to do this....  
+000066a0: 2020 2222 220a 2020 2020 6672 6f6d 2061    """.    from a
+000066b0: 7365 2069 6d70 6f72 7420 4174 6f6d 730a  se import Atoms.
+000066c0: 2020 2020 706f 7369 7469 6f6e 7320 3d20      positions = 
+000066d0: 5b5d 0a20 2020 206e 756d 6265 7273 203d  [].    numbers =
+000066e0: 205b 5d0a 2020 2020 696e 6469 6365 7320   [].    indices 
+000066f0: 3d20 5b5d 0a20 2020 2074 6167 7320 3d20  = [].    tags = 
+00006700: 5b5d 0a20 2020 2074 6167 7330 203d 2061  [].    tags0 = a
+00006710: 742e 6765 745f 7461 6773 2829 0a20 2020  t.get_tags().   
+00006720: 206d 6f6d 656e 7461 203d 205b 5d0a 2020   momenta = [].  
+00006730: 2020 6d6f 6d65 6e74 6130 203d 2061 742e    momenta0 = at.
+00006740: 6765 745f 6d6f 6d65 6e74 6128 290a 2020  get_momenta().  
+00006750: 2020 6d61 7373 6573 203d 205b 5d0a 2020    masses = [].  
+00006760: 2020 6d61 7373 6573 3020 3d20 6174 2e67    masses0 = at.g
+00006770: 6574 5f6d 6173 7365 7328 290a 0a20 2020  et_masses()..   
+00006780: 2066 6f72 2069 2c61 746f 6d20 696e 2065   for i,atom in e
+00006790: 6e75 6d65 7261 7465 2861 7429 3a0a 2020  numerate(at):.  
+000067a0: 2020 2020 2020 6e72 203d 2061 746f 6d2e        nr = atom.
+000067b0: 6765 7428 276e 756d 6265 7227 290a 2020  get('number').  
+000067c0: 2020 2020 2020 6966 206e 7220 213d 2030        if nr != 0
+000067d0: 3a0a 2020 2020 2020 2020 2020 2020 696e  :.            in
+000067e0: 6469 6365 732e 6170 7065 6e64 2869 290a  dices.append(i).
+000067f0: 2020 2020 2020 2020 2020 2020 706f 7369              posi
+00006800: 7469 6f6e 732e 6170 7065 6e64 2861 746f  tions.append(ato
+00006810: 6d2e 6765 7428 2770 6f73 6974 696f 6e27  m.get('position'
+00006820: 2929 0a20 2020 2020 2020 2020 2020 2074  )).            t
+00006830: 6167 732e 6170 7065 6e64 2874 6167 7330  ags.append(tags0
+00006840: 5b69 5d29 0a20 2020 2020 2020 2020 2020  [i]).           
+00006850: 206d 6f6d 656e 7461 2e61 7070 656e 6428   momenta.append(
+00006860: 6d6f 6d65 6e74 6130 5b69 5d29 0a20 2020  momenta0[i]).   
+00006870: 2020 2020 2020 2020 206d 6173 7365 732e           masses.
+00006880: 6170 7065 6e64 286d 6173 7365 7330 5b69  append(masses0[i
+00006890: 5d29 0a20 2020 2020 2020 2020 2020 206e  ]).            n
+000068a0: 756d 6265 7273 2e61 7070 656e 6428 6e72  umbers.append(nr
+000068b0: 290a 0a20 2020 2072 6574 7572 6e20 4174  )..    return At
+000068c0: 6f6d 7328 6365 6c6c 3d61 742e 6765 745f  oms(cell=at.get_
+000068d0: 6365 6c6c 2829 2c0a 2020 2020 2020 2020  cell(),.        
+000068e0: 2020 2020 2020 2020 2070 6263 3d61 742e           pbc=at.
+000068f0: 6765 745f 7062 6328 292c 0a20 2020 2020  get_pbc(),.     
+00006900: 2020 2020 2020 2020 2020 2020 6e75 6d62              numb
+00006910: 6572 733d 6e75 6d62 6572 732c 0a20 2020  ers=numbers,.   
+00006920: 2020 2020 2020 2020 2020 2020 2020 706f                po
+00006930: 7369 7469 6f6e 733d 706f 7369 7469 6f6e  sitions=position
+00006940: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+00006950: 2020 2020 6361 6c63 756c 6174 6f72 3d61      calculator=a
+00006960: 742e 6765 745f 6361 6c63 756c 6174 6f72  t.get_calculator
+00006970: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
+00006980: 2020 2020 2074 6167 733d 7461 6773 2c0a       tags=tags,.
+00006990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000069a0: 206d 6f6d 656e 7461 3d6d 6f6d 656e 7461   momenta=momenta
+000069b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000069c0: 2020 206d 6173 7365 733d 6d61 7373 6573     masses=masses
+000069d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000069e0: 2020 2063 656c 6c64 6973 703d 6174 2e67     celldisp=at.g
+000069f0: 6574 5f63 656c 6c64 6973 7028 292c 0a20  et_celldisp(),. 
+00006a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a10: 636f 6e73 7472 6169 6e74 3d61 742e 636f  constraint=at.co
+00006a20: 6e73 7472 6169 6e74 732c 0a20 2020 2020  nstraints,.     
+00006a30: 2020 2020 2020 2020 2020 2020 696e 666f              info
+00006a40: 3d61 742e 696e 666f 290a 0a0a 0a64 6566  =at.info)....def
+00006a50: 206d 616b 655f 7375 7065 7263 656c 6c28   make_supercell(
+00006a60: 7072 696d 2c20 502c 2077 7261 703d 5472  prim, P, wrap=Tr
+00006a70: 7565 2c20 746f 6c3d 3165 2d35 293a 0a20  ue, tol=1e-5):. 
+00006a80: 2020 2022 2222 4765 6e65 7261 7465 2061     """Generate a
+00006a90: 2073 7570 6572 6365 6c6c 2062 7920 6170   supercell by ap
+00006aa0: 706c 7969 6e67 2061 2067 656e 6572 616c  plying a general
+00006ab0: 2074 7261 6e73 666f 726d 6174 696f 6e20   transformation 
+00006ac0: 282a 502a 2920 746f 0a20 2020 2074 6865  (*P*) to.    the
+00006ad0: 2069 6e70 7574 2063 6f6e 6669 6775 7261   input configura
+00006ae0: 7469 6f6e 2028 2a70 7269 6d2a 292e 0a0a  tion (*prim*)...
+00006af0: 2020 2020 5468 6973 2066 756e 6374 696f      This functio
+00006b00: 6e20 6973 2061 206d 6f64 6966 6965 6420  n is a modified 
+00006b10: 7665 7273 696f 6e20 6f66 2041 5345 7320  version of ASEs 
+00006b20: 6275 696c 642f 7375 7065 7263 656c 6c73  build/supercells
+00006b30: 2e70 792e 0a20 2020 2054 6865 206d 6f64  .py..    The mod
+00006b40: 6966 6963 6174 696f 6e20 6865 7265 2066  ification here f
+00006b50: 6978 6573 2061 2062 7567 2069 6e20 4153  ixes a bug in AS
+00006b60: 4573 2069 6d70 6c65 6d65 6e74 6174 696f  Es implementatio
+00006b70: 6e2c 2069 6e74 726f 6475 6365 6420 696e  n, introduced in
+00006b80: 0a20 2020 2041 5345 7320 7665 7273 696f  .    ASEs versio
+00006b90: 6e20 332e 3138 2e30 3a20 666f 7220 6365  n 3.18.0: for ce
+00006ba0: 7274 6169 6e20 7472 616e 7366 6f72 6d61  rtain transforma
+00006bb0: 7469 6f6e 206d 6174 7269 6365 732c 2074  tion matrices, t
+00006bc0: 6865 2064 6574 6572 6d69 6e61 6e74 206f  he determinant o
+00006bd0: 660a 2020 2020 7468 6520 6d61 7472 6978  f.    the matrix
+00006be0: 2069 7320 6e65 6761 7469 7665 2c20 616e   is negative, an
+00006bf0: 6420 7468 6520 6675 6e63 7469 6f6e 2065  d the function e
+00006c00: 7869 7473 2077 6974 6820 6572 726f 722c  xits with error,
+00006c10: 2073 696e 6365 2061 206e 6567 6174 6976   since a negativ
+00006c20: 650a 2020 2020 6e75 6d62 6572 206f 6620  e.    number of 
+00006c30: 6174 6f6d 7320 6973 206f 6274 6169 6e65  atoms is obtaine
+00006c40: 642e 0a20 2020 2041 6e20 6578 616d 706c  d..    An exampl
+00006c50: 6520 7363 7269 7074 2064 656d 6f6e 7374  e script demonst
+00006c60: 7261 7469 6e67 2074 6865 2065 7272 6f72  rating the error
+00006c70: 2069 733a 3a0a 0a20 2020 2020 2020 6672   is::..       fr
+00006c80: 6f6d 2061 7365 2e62 7569 6c64 2069 6d70  om ase.build imp
+00006c90: 6f72 7420 6d61 6b65 5f73 7570 6572 6365  ort make_superce
+00006ca0: 6c6c 0a20 2020 2020 2020 6672 6f6d 2061  ll.       from a
+00006cb0: 7365 2e61 746f 6d73 2020 696d 706f 7274  se.atoms  import
+00006cc0: 2041 746f 6d73 0a0a 2020 2020 2020 2070   Atoms..       p
+00006cd0: 7269 6d20 3d20 4174 6f6d 7328 7379 6d62  rim = Atoms(symb
+00006ce0: 6f6c 733d 2743 7527 2c0a 2020 2020 2020  ols='Cu',.      
+00006cf0: 2020 2020 2020 2070 6263 3d54 7275 652c         pbc=True,
+00006d00: 0a20 2020 2020 2020 2020 2020 2020 6365  .             ce
+00006d10: 6c6c 3d5b 5b30 2e30 2c20 312e 3830 352c  ll=[[0.0, 1.805,
+00006d20: 2031 2e38 3035 5d2c 205b 312e 3830 352c   1.805], [1.805,
+00006d30: 2030 2e30 2c20 312e 3830 355d 2c20 5b31   0.0, 1.805], [1
+00006d40: 2e38 3035 2c20 312e 3830 352c 2030 2e30  .805, 1.805, 0.0
+00006d50: 5d5d 290a 0a20 2020 2020 2020 7363 203d  ]])..       sc =
+00006d60: 206d 616b 655f 7375 7065 7263 656c 6c28   make_supercell(
+00006d70: 7072 696d 2c20 5020 3d20 5b5b 2032 2c20  prim, P = [[ 2, 
+00006d80: 2032 2c20 2d32 5d2c 5b20 322c 202d 322c   2, -2],[ 2, -2,
+00006d90: 2020 325d 2c5b 2d32 2c20 2032 2c20 2032    2],[-2,  2,  2
+00006da0: 5d5d 2c20 7772 6170 203d 2054 7275 652c  ]], wrap = True,
+00006db0: 2074 6f6c 203d 2031 652d 3035 290a 0a20   tol = 1e-05).. 
+00006dc0: 2020 2054 6865 2072 656c 6561 7365 2033     The release 3
+00006dd0: 2e32 322e 3020 6f66 2041 5345 2073 7469  .22.0 of ASE sti
+00006de0: 6c6c 2063 6f6e 7461 696e 7320 7468 6520  ll contains the 
+00006df0: 6275 672e 0a20 2020 2049 7420 7761 7320  bug..    It was 
+00006e00: 696e 666f 726d 6564 2074 6f20 4153 4573  informed to ASEs
+00006e10: 2064 6576 656c 6f70 6572 7320 6f6e 2074   developers on t
+00006e20: 6865 2033 2e37 2e32 3032 310a 0a20 2020  he 3.7.2021..   
+00006e30: 2054 6865 2074 7261 6e73 666f 726d 6174   The transformat
+00006e40: 696f 6e20 6973 2064 6573 6372 6962 6564  ion is described
+00006e50: 2062 7920 6120 3378 3320 696e 7465 6765   by a 3x3 intege
+00006e60: 7220 6d61 7472 6978 0a20 2020 2060 5c6d  r matrix.    `\m
+00006e70: 6174 6862 667b 507d 602e 2053 7065 6369  athbf{P}`. Speci
+00006e80: 6669 6361 6c6c 792c 2074 6865 206e 6577  fically, the new
+00006e90: 2063 656c 6c20 6d65 7472 6963 0a20 2020   cell metric.   
+00006ea0: 2060 5c6d 6174 6862 667b 687d 6020 6973   `\mathbf{h}` is
+00006eb0: 2067 6976 656e 2069 6e20 7465 726d 7320   given in terms 
+00006ec0: 6f66 2074 6865 206d 6574 7269 6320 6f66  of the metric of
+00006ed0: 2074 6865 2069 6e70 7574 0a20 2020 2063   the input.    c
+00006ee0: 6f6e 6669 6775 7261 7469 6f6e 2060 5c6d  onfiguration `\m
+00006ef0: 6174 6862 667b 687d 5f70 6020 6279 2060  athbf{h}_p` by `
+00006f00: 5c6d 6174 6862 667b 5020 687d 5f70 203d  \mathbf{P h}_p =
+00006f10: 0a20 2020 205c 6d61 7468 6266 7b68 7d60  .    \mathbf{h}`
+00006f20: 2e0a 0a20 2020 202a 2a50 6172 616d 6574  ...    **Paramet
+00006f30: 6572 733a 2a2a 0a0a 2020 2020 6060 7072  ers:**..    ``pr
+00006f40: 696d 6060 3a20 4153 4520 4174 6f6d 7320  im``: ASE Atoms 
+00006f50: 6f62 6a65 6374 0a20 2020 2020 2020 2049  object.        I
+00006f60: 6e70 7574 2063 6f6e 6669 6775 7261 7469  nput configurati
+00006f70: 6f6e 2e0a 2020 2020 6060 5060 603a 2033  on..    ``P``: 3
+00006f80: 7833 2069 6e74 6567 6572 206d 6174 7269  x3 integer matri
+00006f90: 780a 2020 2020 2020 2020 5472 616e 7366  x.        Transf
+00006fa0: 6f72 6d61 7469 6f6e 206d 6174 7269 7820  ormation matrix 
+00006fb0: 605c 6d61 7468 6266 7b50 7d60 2e0a 2020  `\mathbf{P}`..  
+00006fc0: 2020 6060 7772 6170 6060 3a20 626f 6f6c    ``wrap``: bool
+00006fd0: 0a20 2020 2020 2020 2077 7261 7020 696e  .        wrap in
+00006fe0: 2074 6865 2065 6e64 0a20 2020 2060 6074   the end.    ``t
+00006ff0: 6f6c 6060 3a20 666c 6f61 740a 2020 2020  ol``: float.    
+00007000: 2020 2020 746f 6c65 7261 6e63 6520 666f      tolerance fo
+00007010: 7220 7772 6170 7069 6e67 0a20 2020 2022  r wrapping.    "
+00007020: 2222 0a0a 2020 2020 7375 7065 7263 656c  ""..    supercel
+00007030: 6c5f 6d61 7472 6978 203d 2050 0a20 2020  l_matrix = P.   
+00007040: 2073 7570 6572 6365 6c6c 203d 2063 6c65   supercell = cle
+00007050: 616e 5f6d 6174 7269 7828 7375 7065 7263  an_matrix(superc
+00007060: 656c 6c5f 6d61 7472 6978 2040 2070 7269  ell_matrix @ pri
+00007070: 6d2e 6365 6c6c 290a 0a20 2020 2023 2063  m.cell)..    # c
+00007080: 6172 7465 7369 616e 206c 6174 7469 6365  artesian lattice
+00007090: 2070 6f69 6e74 730a 2020 2020 6c61 7474   points.    latt
+000070a0: 6963 655f 706f 696e 7473 5f66 7261 6320  ice_points_frac 
+000070b0: 3d20 6c61 7474 6963 655f 706f 696e 7473  = lattice_points
+000070c0: 5f69 6e5f 7375 7065 7263 656c 6c28 7375  _in_supercell(su
+000070d0: 7065 7263 656c 6c5f 6d61 7472 6978 290a  percell_matrix).
+000070e0: 2020 2020 6c61 7474 6963 655f 706f 696e      lattice_poin
+000070f0: 7473 203d 206e 702e 646f 7428 6c61 7474  ts = np.dot(latt
+00007100: 6963 655f 706f 696e 7473 5f66 7261 632c  ice_points_frac,
+00007110: 2073 7570 6572 6365 6c6c 290a 0a20 2020   supercell)..   
+00007120: 2073 7570 6572 6174 6f6d 7320 3d20 4174   superatoms = At
+00007130: 6f6d 7328 6365 6c6c 3d73 7570 6572 6365  oms(cell=superce
+00007140: 6c6c 2c20 7062 633d 7072 696d 2e70 6263  ll, pbc=prim.pbc
+00007150: 290a 0a20 2020 2066 6f72 206c 7020 696e  )..    for lp in
+00007160: 206c 6174 7469 6365 5f70 6f69 6e74 733a   lattice_points:
+00007170: 0a20 2020 2020 2020 2073 6869 6674 6564  .        shifted
+00007180: 5f61 746f 6d73 203d 2070 7269 6d2e 636f  _atoms = prim.co
+00007190: 7079 2829 0a20 2020 2020 2020 2073 6869  py().        shi
+000071a0: 6674 6564 5f61 746f 6d73 2e70 6f73 6974  fted_atoms.posit
+000071b0: 696f 6e73 202b 3d20 6c70 0a20 2020 2020  ions += lp.     
+000071c0: 2020 2073 7570 6572 6174 6f6d 732e 6578     superatoms.ex
+000071d0: 7465 6e64 2873 6869 6674 6564 5f61 746f  tend(shifted_ato
+000071e0: 6d73 290a 0a20 2020 2023 2063 6865 636b  ms)..    # check
+000071f0: 206e 756d 6265 7220 6f66 2061 746f 6d73   number of atoms
+00007200: 2069 7320 636f 7272 6563 740a 2020 2020   is correct.    
+00007210: 6e5f 7461 7267 6574 203d 206e 702e 6162  n_target = np.ab
+00007220: 7328 696e 7428 6e70 2e72 6f75 6e64 286e  s(int(np.round(n
+00007230: 702e 6c69 6e61 6c67 2e64 6574 2873 7570  p.linalg.det(sup
+00007240: 6572 6365 6c6c 5f6d 6174 7269 7829 202a  ercell_matrix) *
+00007250: 206c 656e 2870 7269 6d29 2929 290a 2020   len(prim)))).  
+00007260: 2020 6966 206e 5f74 6172 6765 7420 213d    if n_target !=
+00007270: 206c 656e 2873 7570 6572 6174 6f6d 7329   len(superatoms)
+00007280: 3a0a 2020 2020 2020 2020 6d73 6720 3d20  :.        msg = 
+00007290: 224e 756d 6265 7220 6f66 2061 746f 6d73  "Number of atoms
+000072a0: 2069 6e20 7375 7065 7263 656c 6c3a 207b   in supercell: {
+000072b0: 7d2c 2065 7870 6563 7465 643a 207b 7d22  }, expected: {}"
+000072c0: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
+000072d0: 2020 2020 206e 5f74 6172 6765 742c 206c       n_target, l
+000072e0: 656e 2873 7570 6572 6174 6f6d 7329 0a20  en(superatoms). 
+000072f0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00007300: 2072 6169 7365 2053 7570 6572 6365 6c6c   raise Supercell
+00007310: 4572 726f 7228 6d73 6729 0a0a 2020 2020  Error(msg)..    
+00007320: 6966 2077 7261 703a 0a20 2020 2020 2020  if wrap:.       
+00007330: 2073 7570 6572 6174 6f6d 732e 7772 6170   superatoms.wrap
+00007340: 2865 7073 3d74 6f6c 290a 0a20 2020 2072  (eps=tol)..    r
+00007350: 6574 7572 6e20 7375 7065 7261 746f 6d73  eturn superatoms
+00007360: 0a0a 6465 6620 6465 636f 7261 7465 5f73  ..def decorate_s
+00007370: 7570 6572 6365 6c6c 2873 6365 6c6c 2c20  upercell(scell, 
+00007380: 6174 6f6d 7329 3a0a 2020 2020 2222 2220  atoms):.    """ 
+00007390: 4372 6561 7465 2061 2053 7472 7563 7475  Create a Structu
+000073a0: 7265 2069 6e73 7461 6e63 6520 6279 2064  re instance by d
+000073b0: 6563 6f72 6174 696e 6720 6120 5375 7065  ecorating a Supe
+000073c0: 7243 656c 6c20 7769 7468 2061 6e20 4174  rCell with an At
+000073d0: 6f6d 7320 6f62 6a65 6374 2066 726f 6d20  oms object from 
+000073e0: 4153 452e 0a20 2020 2022 2222 0a20 2020  ASE..    """.   
+000073f0: 2066 726f 6d20 636c 7573 7465 7278 2e73   from clusterx.s
+00007400: 7472 7563 7475 7265 2069 6d70 6f72 7420  tructure import 
+00007410: 5374 7275 6374 7572 650a 0a20 2020 2061  Structure..    a
+00007420: 6e73 203d 205b 5d0a 2020 2020 666f 7220  ns = [].    for 
+00007430: 6931 2c20 7031 2069 6e20 656e 756d 6572  i1, p1 in enumer
+00007440: 6174 6528 7363 656c 6c2e 6765 745f 706f  ate(scell.get_po
+00007450: 7369 7469 6f6e 7328 2929 3a0a 2020 2020  sitions()):.    
+00007460: 2020 2020 666f 7220 6932 2c20 7032 2069      for i2, p2 i
+00007470: 6e20 656e 756d 6572 6174 6528 6174 6f6d  n enumerate(atom
+00007480: 732e 6765 745f 706f 7369 7469 6f6e 7328  s.get_positions(
+00007490: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+000074a0: 6966 206e 702e 6c69 6e61 6c67 2e6e 6f72  if np.linalg.nor
+000074b0: 6d28 7031 2d70 3229 203c 2031 652d 353a  m(p1-p2) < 1e-5:
+000074c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000074d0: 2061 6e73 2e61 7070 656e 6428 6174 6f6d   ans.append(atom
+000074e0: 732e 6765 745f 6174 6f6d 6963 5f6e 756d  s.get_atomic_num
+000074f0: 6265 7273 2829 5b69 325d 290a 0a20 2020  bers()[i2])..   
+00007500: 2072 6574 7572 6e20 5374 7275 6374 7572   return Structur
+00007510: 6528 7363 656c 6c2c 2061 6e73 290a 0a64  e(scell, ans)..d
+00007520: 6566 2073 7570 6572 5f73 7472 7563 7475  ef super_structu
+00007530: 7265 2873 7472 7563 302c 2064 293a 0a20  re(struc0, d):. 
+00007540: 2020 2022 2222 2043 7265 6174 6520 6120     """ Create a 
+00007550: 7375 7065 7220 7374 7275 6374 7572 650a  super structure.
+00007560: 0a20 2020 2054 6869 7320 6675 6e63 7469  .    This functi
+00007570: 6f6e 2074 616b 6573 2061 2060 6053 7472  on takes a ``Str
+00007580: 7563 7475 7265 6060 2069 6e73 7461 6e63  ucture`` instanc
+00007590: 6520 2860 6073 7472 7563 3060 6029 2061  e (``struc0``) a
+000075a0: 6e64 2063 7265 6174 6573 2061 206e 6577  nd creates a new
+000075b0: 2073 7472 7563 7475 7265 0a20 2020 2077   structure.    w
+000075c0: 6869 6368 2069 7320 6f62 7461 696e 6564  hich is obtained
+000075d0: 2061 7320 7468 6520 7065 7269 6f64 6963   as the periodic
+000075e0: 2072 6570 6574 6974 696f 6e20 6f66 2074   repetition of t
+000075f0: 6865 206f 7269 6769 6e61 6c20 7374 7275  he original stru
+00007600: 6374 7572 650a 2020 2020 616c 6f6e 6720  cture.    along 
+00007610: 6974 7320 756e 6974 2063 656c 6c20 7665  its unit cell ve
+00007620: 6374 6f72 732e 2054 6865 206e 756d 6265  ctors. The numbe
+00007630: 7220 6f66 2072 6570 6574 6974 696f 6e73  r of repetitions
+00007640: 2061 6c6f 6e67 2065 6163 6820 6365 6c6c   along each cell
+00007650: 2076 6563 746f 7220 6973 2067 6976 656e   vector is given
+00007660: 0a20 2020 2062 7920 7468 6520 7468 7265  .    by the thre
+00007670: 6520 636f 6d70 6f6e 656e 7473 206f 6620  e components of 
+00007680: 7468 6520 696e 7075 7420 696e 7465 6765  the input intege
+00007690: 7220 7665 6374 6f72 2060 6064 6060 2e0a  r vector ``d``..
+000076a0: 0a20 2020 202a 2a50 6172 616d 6574 6572  .    **Parameter
+000076b0: 733a 2a2a 0a0a 2020 2020 6060 7374 7275  s:**..    ``stru
+000076c0: 6330 6060 3a20 5374 7275 6374 7572 6520  c0``: Structure 
+000076d0: 6f62 6a65 6374 0a20 2020 2020 2020 204f  object.        O
+000076e0: 7269 6769 6e61 6c20 7374 7275 6374 7572  riginal structur
+000076f0: 6520 666f 7220 7468 6520 7375 7065 7273  e for the supers
+00007700: 7472 7563 7475 7265 2e0a 2020 2020 6060  tructure..    ``
+00007710: 6460 603a 2069 6e74 2c20 7468 7265 652d  d``: int, three-
+00007720: 636f 6d70 6f6e 656e 7420 696e 7465 6765  component intege
+00007730: 7220 6172 7261 792c 206f 7220 3378 3320  r array, or 3x3 
+00007740: 696e 7465 6765 7220 6172 7261 790a 2020  integer array.  
+00007750: 2020 2020 2020 5468 6520 7375 7065 7220        The super 
+00007760: 7374 7275 6374 7572 6520 6973 206f 6274  structure is obt
+00007770: 6169 6e65 6420 6279 2074 6865 2074 7261  ained by the tra
+00007780: 6e73 666f 726d 6174 696f 6e20 6420 532c  nsformation d S,
+00007790: 2077 6974 6820 6420 610a 2020 2020 2020   with d a.      
+000077a0: 2020 3378 3320 6d61 7472 6978 206f 6620    3x3 matrix of 
+000077b0: 696e 7465 6765 7220 616e 6420 5320 7468  integer and S th
+000077c0: 6520 7375 7065 7263 656c 6c20 6365 6c6c  e supercell cell
+000077d0: 2076 6563 746f 7273 2e0a 2020 2020 2222   vectors..    ""
+000077e0: 220a 2020 2020 6672 6f6d 2063 6c75 7374  ".    from clust
+000077f0: 6572 782e 7374 7275 6374 7572 6520 696d  erx.structure im
+00007800: 706f 7274 2053 7472 7563 7475 7265 0a20  port Structure. 
+00007810: 2020 2066 726f 6d20 636c 7573 7465 7278     from clusterx
+00007820: 2e73 7570 6572 5f63 656c 6c20 696d 706f  .super_cell impo
+00007830: 7274 2053 7570 6572 4365 6c6c 0a20 2020  rt SuperCell.   
+00007840: 2066 726f 6d20 6173 652e 6275 696c 6420   from ase.build 
+00007850: 696d 706f 7274 206d 616b 655f 7375 7065  import make_supe
+00007860: 7263 656c 6c0a 0a20 2020 2069 6620 6e70  rcell..    if np
+00007870: 2e73 6861 7065 2864 2920 3d3d 2028 293a  .shape(d) == ():
+00007880: 0a20 2020 2020 2020 206e 203d 206e 702e  .        n = np.
+00007890: 7a65 726f 7328 2833 2c33 292c 2069 6e74  zeros((3,3), int
+000078a0: 290a 2020 2020 2020 2020 6e70 2e66 696c  ).        np.fil
+000078b0: 6c5f 6469 6167 6f6e 616c 286e 2c20 5b64  l_diagonal(n, [d
+000078c0: 2c64 2c64 5d29 0a20 2020 2065 6c69 6620  ,d,d]).    elif 
+000078d0: 6e70 2e73 6861 7065 2864 2920 3d3d 2028  np.shape(d) == (
+000078e0: 332c 293a 0a20 2020 2020 2020 206e 203d  3,):.        n =
+000078f0: 206e 702e 7a65 726f 7328 2833 2c33 292c   np.zeros((3,3),
+00007900: 2069 6e74 290a 2020 2020 2020 2020 6e70   int).        np
+00007910: 2e66 696c 6c5f 6469 6167 6f6e 616c 286e  .fill_diagonal(n
+00007920: 2c20 6429 0a20 2020 2065 6c69 6620 6e70  , d).    elif np
+00007930: 2e73 6861 7065 2864 2920 3d3d 2028 332c  .shape(d) == (3,
+00007940: 3329 3a0a 2020 2020 2020 2020 6e20 3d20  3):.        n = 
+00007950: 6e70 2e61 7272 6179 2864 290a 2020 2020  np.array(d).    
+00007960: 656c 7365 3a0a 2020 2020 2020 2020 7072  else:.        pr
+00007970: 696e 7428 2245 5252 4f52 2028 636c 7573  int("ERROR (clus
+00007980: 7465 7278 2e75 7469 6c73 2e73 7570 6572  terx.utils.super
+00007990: 5f73 7472 7563 7475 7265 2829 293a 2022  _structure()): "
+000079a0: 290a 0a20 2020 2070 3020 3d20 7374 7275  )..    p0 = stru
+000079b0: 6330 2e67 6574 5f73 7570 6572 6365 6c6c  c0.get_supercell
+000079c0: 2829 2e67 6574 5f74 7261 6e73 666f 726d  ().get_transform
+000079d0: 6174 696f 6e28 290a 2020 2020 7031 203d  ation().    p1 =
+000079e0: 206e 2040 2070 300a 0a20 2020 2061 746f   n @ p0..    ato
+000079f0: 6d73 3020 3d20 7374 7275 6330 2e67 6574  ms0 = struc0.get
+00007a00: 5f61 746f 6d73 2829 0a20 2020 2061 746f  _atoms().    ato
+00007a10: 6d73 3120 3d20 6d61 6b65 5f73 7570 6572  ms1 = make_super
+00007a20: 6365 6c6c 2861 746f 6d73 302c 206e 290a  cell(atoms0, n).
+00007a30: 0a20 2020 2073 6365 6c6c 3120 3d20 5375  .    scell1 = Su
+00007a40: 7065 7243 656c 6c28 7374 7275 6330 2e67  perCell(struc0.g
+00007a50: 6574 5f70 6172 656e 745f 6c61 7474 6963  et_parent_lattic
+00007a60: 6528 292c 2070 3129 0a0a 2020 2020 7265  e(), p1)..    re
+00007a70: 7475 726e 2064 6563 6f72 6174 655f 7375  turn decorate_su
+00007a80: 7065 7263 656c 6c28 7363 656c 6c31 2c20  percell(scell1, 
+00007a90: 6174 6f6d 7331 290a 0a64 6566 2073 7365  atoms1)..def sse
+00007aa0: 745f 6571 7569 7661 6c65 6e63 655f 6368  t_equivalence_ch
+00007ab0: 6563 6b28 7373 6574 2c20 746f 5f70 7269  eck(sset, to_pri
+00007ac0: 6d69 7469 7665 203d 2054 7275 652c 2063  mitive = True, c
+00007ad0: 706f 6f6c 203d 204e 6f6e 652c 2062 6173  pool = None, bas
+00007ae0: 6973 203d 2022 7472 6967 6f6e 6f6d 6574  is = "trigonomet
+00007af0: 7269 6322 2c20 636f 6d61 7420 3d20 4e6f  ric", comat = No
+00007b00: 6e65 2c20 7072 6574 7479 5f70 7269 6e74  ne, pretty_print
+00007b10: 203d 2046 616c 7365 293a 0a20 2020 2022   = False):.    "
+00007b20: 2222 4669 6e64 2065 7175 6976 616c 656e  ""Find equivalen
+00007b30: 7420 7374 7275 6374 7572 6573 2069 6e20  t structures in 
+00007b40: 6120 5374 7275 6374 7572 6573 5365 7420  a StructuresSet 
+00007b50: 6f62 6a65 6374 0a0a 2020 2020 4571 7569  object..    Equi
+00007b60: 7661 6c65 6e63 6520 6973 2064 6574 6572  valence is deter
+00007b70: 6d69 6e65 6420 2a69 292a 2069 6e20 7465  mined *i)* in te
+00007b80: 726d 7320 6f66 2073 796d 6d65 7472 7920  rms of symmetry 
+00007b90: 6265 7477 6565 6e20 7374 7275 6374 7572  between structur
+00007ba0: 6573 0a20 2020 206f 7220 2a69 6929 2a20  es.    or *ii)* 
+00007bb0: 696e 2074 6572 6d73 206f 6620 636c 7573  in terms of clus
+00007bc0: 7465 7220 6261 7369 7320 7265 7072 6573  ter basis repres
+00007bd0: 656e 7461 7469 6f6e 2028 6966 2061 2043  entation (if a C
+00007be0: 6c75 7374 6572 7350 6f6f 6c20 6f62 6a65  lustersPool obje
+00007bf0: 6374 0a20 2020 206f 7220 6120 636f 7272  ct.    or a corr
+00007c00: 656c 6174 696f 6e20 6d61 7472 6978 2069  elation matrix i
+00007c10: 7320 6769 7665 6e29 2e0a 0a20 2020 2049  s given)...    I
+00007c20: 6e20 7468 6520 6669 7273 7420 6361 7365  n the first case
+00007c30: 2c20 7468 6520 6053 796d 6d65 7472 7945  , the `SymmetryE
+00007c40: 7175 6976 616c 656e 6365 4368 6563 6b20  quivalenceCheck 
+00007c50: 746f 6f6c 206f 6620 4153 4520 3c68 7474  tool of ASE <htt
+00007c60: 7073 3a2f 2f77 696b 692e 6679 7369 6b2e  ps://wiki.fysik.
+00007c70: 6474 752e 646b 2f61 7365 2f61 7365 2f75  dtu.dk/ase/ase/u
+00007c80: 7469 6c73 2e68 746d 6c23 6173 652e 7574  tils.html#ase.ut
+00007c90: 696c 732e 7374 7275 6374 7572 655f 636f  ils.structure_co
+00007ca0: 6d70 6172 6174 6f72 2e53 796d 6d65 7472  mparator.Symmetr
+00007cb0: 7945 7175 6976 616c 656e 6365 4368 6563  yEquivalenceChec
+00007cc0: 6b3e 605f 2069 7320 7573 6564 2e0a 0a20  k>`_ is used... 
+00007cd0: 2020 202a 2a50 6172 616d 6574 6572 733a     **Parameters:
+00007ce0: 2a2a 0a0a 2020 2020 6060 7373 6574 6060  **..    ``sset``
+00007cf0: 3a20 5374 7275 6374 7572 6573 5365 7420  : StructuresSet 
+00007d00: 6f62 6a65 6374 0a20 2020 2020 2020 2054  object.        T
+00007d10: 6865 2073 7472 7563 7475 7265 7320 7365  he structures se
+00007d20: 7420 6f62 6a65 6374 2074 6f20 6265 2061  t object to be a
+00007d30: 6e61 6c79 7a65 642e 0a0a 2020 2020 6060  nalyzed...    ``
+00007d40: 746f 5f70 7269 6d69 7469 7665 6060 3a20  to_primitive``: 
+00007d50: 426f 6f6c 6561 6e20 2864 6566 6175 6c74  Boolean (default
+00007d60: 3a20 6060 5472 7565 6060 290a 2020 2020  : ``True``).    
+00007d70: 2020 2020 4966 2060 6054 7275 6560 6020      If ``True`` 
+00007d80: 7468 6520 7374 7275 6374 7572 6573 2061  the structures a
+00007d90: 7265 2072 6564 7563 6564 2074 6f20 7468  re reduced to th
+00007da0: 6569 7220 7072 696d 6974 6976 6520 6365  eir primitive ce
+00007db0: 6c6c 732e 0a20 2020 2020 2020 2054 6869  lls..        Thi
+00007dc0: 7320 6665 6174 7572 6520 7265 7175 6972  s feature requir
+00007dd0: 6573 2060 6073 7067 6c69 6260 6020 746f  es ``spglib`` to
+00007de0: 2069 6e73 7461 6c6c 6564 0a20 2020 2020   installed.     
+00007df0: 2020 2028 2a63 662e 2a20 6041 5345 2773     (*cf.* `ASE's
+00007e00: 2053 796d 6d65 7472 7945 7175 6976 616c   SymmetryEquival
+00007e10: 656e 6365 4368 6563 6b20 3c68 7474 7073  enceCheck <https
+00007e20: 3a2f 2f77 696b 692e 6679 7369 6b2e 6474  ://wiki.fysik.dt
+00007e30: 752e 646b 2f61 7365 2f61 7365 2f75 7469  u.dk/ase/ase/uti
+00007e40: 6c73 2e68 746d 6c3f 6869 6768 6c69 6768  ls.html?highligh
+00007e50: 743d 746f 5f70 7269 6d69 7469 7665 2361  t=to_primitive#a
+00007e60: 7365 2e75 7469 6c73 2e73 7472 7563 7475  se.utils.structu
+00007e70: 7265 5f63 6f6d 7061 7261 746f 722e 5379  re_comparator.Sy
+00007e80: 6d6d 6574 7279 4571 7569 7661 6c65 6e63  mmetryEquivalenc
+00007e90: 6543 6865 636b 3e60 5f29 0a0a 2020 2020  eCheck>`_)..    
+00007ea0: 6060 6370 6f6f 6c60 603a 2043 6c75 7374  ``cpool``: Clust
+00007eb0: 6572 7350 6f6f 6c20 6f62 6a65 6374 2028  ersPool object (
+00007ec0: 6465 6661 756c 743a 2060 604e 6f6e 6560  default: ``None`
+00007ed0: 6029 0a20 2020 2020 2020 2054 6869 7320  `).        This 
+00007ee0: 7061 7261 6d65 7465 7220 6973 206f 7074  parameter is opt
+00007ef0: 696f 6e61 6c2e 2049 6620 6769 7665 6e2c  ional. If given,
+00007f00: 2074 6865 2065 7175 6976 616c 656e 6365   the equivalence
+00007f10: 206f 6620 6120 7061 6972 206f 6620 7374   of a pair of st
+00007f20: 7275 6374 7572 6573 0a20 2020 2020 2020  ructures.       
+00007f30: 2069 7320 6465 7465 726d 696e 6564 2061   is determined a
+00007f40: 6363 6f72 6469 6e67 2074 6f20 7468 6569  ccording to thei
+00007f50: 7220 636c 7573 7465 7220 6261 7369 7320  r cluster basis 
+00007f60: 7265 7072 6573 656e 7461 7469 6f6e 3a20  representation: 
+00007f70: 7477 6f0a 2020 2020 2020 2020 7374 7275  two.        stru
+00007f80: 6374 7572 6573 2077 6974 6820 7468 6520  ctures with the 
+00007f90: 7361 6d65 2063 6c75 7374 6572 2063 6f72  same cluster cor
+00007fa0: 7265 6c61 7469 6f6e 7320 666f 7220 7468  relations for th
+00007fb0: 6520 636c 7573 7465 7273 2069 6e20 6060  e clusters in ``
+00007fc0: 6370 6f6f 6c60 600a 2020 2020 2020 2020  cpool``.        
+00007fd0: 6172 6520 636f 6e73 6964 6572 6564 2065  are considered e
+00007fe0: 7175 6976 616c 656e 742e 0a0a 2020 2020  quivalent...    
+00007ff0: 6060 6261 7369 7360 603a 2073 7472 696e  ``basis``: strin
+00008000: 6720 2864 6566 6175 6c74 3a20 6060 2274  g (default: ``"t
+00008010: 7269 676f 6e6f 6d65 7472 6963 2260 6029  rigonometric"``)
+00008020: 0a20 2020 2020 2020 204f 6e6c 7920 7573  .        Only us
+00008030: 6564 2069 6620 6060 6370 6f6f 6c60 6020  ed if ``cpool`` 
+00008040: 6973 206e 6f74 2060 604e 6f6e 6560 602e  is not ``None``.
+00008050: 2053 6974 6520 6261 7369 7320 6675 6e63   Site basis func
+00008060: 7469 6f6e 7320 7573 6564 2069 6e20 7468  tions used in th
+00008070: 6520 6465 7465 726d 696e 6174 696f 6e0a  e determination.
+00008080: 2020 2020 2020 2020 6f66 2063 6c75 7374          of clust
+00008090: 6572 2063 6f72 7265 6c61 7469 6f6e 732e  er correlations.
+000080a0: 0a0a 2020 2020 6060 636f 6d61 7460 603a  ..    ``comat``:
+000080b0: 2032 4420 6172 7261 7920 6f66 2066 6c6f   2D array of flo
+000080c0: 6174 7320 2864 6566 6175 6c74 3a20 6060  ats (default: ``
+000080d0: 4e6f 6e65 6060 290a 2020 2020 2020 2020  None``).        
+000080e0: 4974 206f 7665 7272 6964 6573 2060 6063  It overrides ``c
+000080f0: 706f 6f6c 6060 2061 6e64 2060 6062 6173  pool`` and ``bas
+00008100: 6973 6060 2e20 4966 2061 2063 6f72 7265  is``. If a corre
+00008110: 6c61 7469 6f6e 206d 6174 7269 7820 666f  lation matrix fo
+00008120: 7220 7468 650a 2020 2020 2020 2020 7374  r the.        st
+00008130: 7275 6374 7572 6573 2073 6574 2073 7365  ructures set sse
+00008140: 7420 7761 7320 7072 652d 636f 6d70 7574  t was pre-comput
+00008150: 6564 2c20 7468 6520 6571 7569 7661 6c65  ed, the equivale
+00008160: 6e63 6520 696e 2074 6572 6d73 206f 6620  nce in terms of 
+00008170: 636c 7573 7465 720a 2020 2020 2020 2020  cluster.        
+00008180: 6261 7369 7320 7265 7072 6573 656e 7461  basis representa
+00008190: 7469 6f6e 2069 7320 7065 7266 6f72 6d65  tion is performe
+000081a0: 6420 6279 2063 6f6d 7061 7269 6e67 2074  d by comparing t
+000081b0: 6865 2072 6f77 7320 6f66 2074 6869 7320  he rows of this 
+000081c0: 6d61 7472 6978 2028 6561 6368 0a20 2020  matrix (each.   
+000081d0: 2020 2020 2072 6f77 206d 7573 7420 636f       row must co
+000081e0: 7272 6573 706f 6e64 2074 6f20 6120 7374  rrespond to a st
+000081f0: 7275 6374 7572 6520 696e 2074 6865 2073  ructure in the s
+00008200: 7472 7563 7475 7265 7320 7365 7429 2e0a  tructures set)..
+00008210: 0a0a 2020 2020 2a2a 5265 7475 726e 733a  ..    **Returns:
+00008220: 2a2a 0a20 2020 2052 6574 7572 6e73 2061  **.    Returns a
+00008230: 2064 6963 7469 6f6e 6172 792e 2054 6865   dictionary. The
+00008240: 206b 6579 7320 286b 2920 6172 6520 7374   keys (k) are st
+00008250: 7275 6374 7572 6520 696e 6469 6365 7320  ructure indices 
+00008260: 6f66 2075 6e69 7175 6520 7265 7072 6573  of unique repres
+00008270: 656e 7461 7469 7665 2073 7472 7563 7475  entative structu
+00008280: 7265 732c 0a20 2020 2061 6e64 2074 6865  res,.    and the
+00008290: 2076 616c 7565 7320 2876 2920 6172 6520   values (v) are 
+000082a0: 6172 7261 7973 206f 6620 696e 7465 6765  arrays of intege
+000082b0: 722c 2069 6e64 6963 6174 696e 6720 616c  r, indicating al
+000082c0: 6c20 7374 7275 6374 7572 6520 696e 6469  l structure indi
+000082d0: 6365 7320 6571 7569 7661 6c65 6e74 2074  ces equivalent t
+000082e0: 6f20 6b0a 2020 2020 2863 6f6e 7461 696e  o k.    (contain
+000082f0: 696e 6720 6b20 6974 7365 6c66 2074 6f6f  ing k itself too
+00008300: 292e 2046 6f72 2069 6e73 7461 6e63 652c  ). For instance,
+00008310: 2074 6865 2064 6963 7469 6f6e 6172 793a   the dictionary:
+00008320: 3a0a 0a20 2020 2020 2020 207b 2230 223a  :..        {"0":
+00008330: 205b 302c 2031 2c20 332c 2038 2c20 395d   [0, 1, 3, 8, 9]
+00008340: 2c0a 2020 2020 2020 2020 2022 3222 3a20  ,.         "2": 
+00008350: 5b32 2c20 352c 2036 5d2c 0a20 2020 2020  [2, 5, 6],.     
+00008360: 2020 2020 2234 223a 205b 342c 2037 5d7d      "4": [4, 7]}
+00008370: 0a0a 2020 2020 7c20 696e 6469 6361 7465  ..    | indicate
+00008380: 7320 7468 6174 2069 6e20 7468 6520 7374  s that in the st
+00008390: 7275 6374 7572 6573 2073 6574 2077 6974  ructures set wit
+000083a0: 6820 696e 6469 6365 7320 5b30 2c20 312c  h indices [0, 1,
+000083b0: 2032 2c20 332c 2034 2c20 352c 2036 2c20   2, 3, 4, 5, 6, 
+000083c0: 372c 2038 2c20 395d 2074 6865 7265 2061  7, 8, 9] there a
+000083d0: 7265 0a20 2020 2020 206a 7573 7420 7468  re.      just th
+000083e0: 7265 6520 6469 7374 696e 6374 2073 7472  ree distinct str
+000083f0: 7563 7475 7265 732e 2054 6865 7365 2063  uctures. These c
+00008400: 616e 2062 6520 7265 7072 6573 656e 7465  an be represente
+00008410: 6420 6279 2073 7472 7563 7574 7265 7320  d by strucutres 
+00008420: 302c 2032 2061 6e64 2034 2e0a 2020 2020  0, 2 and 4..    
+00008430: 2020 5468 6520 7374 7275 6374 7572 6573    The structures
+00008440: 205b 302c 2031 2c20 332c 2038 2c20 395d   [0, 1, 3, 8, 9]
+00008450: 2061 7265 2061 6c6c 2065 7175 6976 616c   are all equival
+00008460: 656e 742c 2065 7463 2e0a 2020 2020 7c20  ent, etc..    | 
+00008470: 4e6f 7469 6365 2074 6861 7420 6865 7265  Notice that here
+00008480: 2065 7175 6976 616c 656e 6365 2069 7320   equivalence is 
+00008490: 7573 6564 2069 6e20 7468 6520 7365 6e73  used in the sens
+000084a0: 6520 6578 706c 6169 6e65 6420 6162 6f76  e explained abov
+000084b0: 653a 2049 7420 6973 2073 796d 6d65 7472  e: It is symmetr
+000084c0: 6963 616c 0a20 2020 2020 2065 7175 6976  ical.      equiv
+000084d0: 616c 656e 6365 206f 6e6c 7920 6966 2060  alence only if `
+000084e0: 6063 706f 6f6c 6060 2061 6e64 2060 6063  `cpool`` and ``c
+000084f0: 6f6d 6174 6060 2061 7265 204e 6f6e 652e  omat`` are None.
+00008500: 0a20 2020 2022 2222 0a20 2020 2069 6d70  .    """.    imp
+00008510: 6f72 7420 6e75 6d70 7920 6173 206e 700a  ort numpy as np.
+00008520: 0a20 2020 2063 6f6d 7020 3d20 4e6f 6e65  .    comp = None
+00008530: 0a20 2020 2066 726f 6d20 636c 7573 7465  .    from cluste
+00008540: 7278 2e75 7469 6c73 2069 6d70 6f72 7420  rx.utils import 
+00008550: 6973 636c 6f73 650a 0a20 2020 2069 6620  isclose..    if 
+00008560: 6370 6f6f 6c20 6973 204e 6f6e 6520 616e  cpool is None an
+00008570: 6420 636f 6d61 7420 6973 204e 6f6e 653a  d comat is None:
+00008580: 0a20 2020 2020 2020 2066 726f 6d20 6173  .        from as
+00008590: 652e 7574 696c 732e 7374 7275 6374 7572  e.utils.structur
+000085a0: 655f 636f 6d70 6172 6174 6f72 2069 6d70  e_comparator imp
+000085b0: 6f72 7420 5379 6d6d 6574 7279 4571 7569  ort SymmetryEqui
+000085c0: 7661 6c65 6e63 6543 6865 636b 0a20 2020  valenceCheck.   
+000085d0: 2020 2020 2063 6f6d 7020 3d20 5379 6d6d       comp = Symm
+000085e0: 6574 7279 4571 7569 7661 6c65 6e63 6543  etryEquivalenceC
+000085f0: 6865 636b 2874 6f5f 7072 696d 6974 6976  heck(to_primitiv
+00008600: 6520 3d20 746f 5f70 7269 6d69 7469 7665  e = to_primitive
+00008610: 290a 2020 2020 656c 6966 2063 6f6d 6174  ).    elif comat
+00008620: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00008630: 2020 6672 6f6d 2063 6c75 7374 6572 782e    from clusterx.
+00008640: 636f 7272 656c 6174 696f 6e73 2069 6d70  correlations imp
+00008650: 6f72 7420 436f 7272 656c 6174 696f 6e73  ort Correlations
+00008660: 4361 6c63 756c 6174 6f72 0a20 2020 2020  Calculator.     
+00008670: 2020 2063 6361 6c63 203d 2043 6f72 7265     ccalc = Corre
+00008680: 6c61 7469 6f6e 7343 616c 6375 6c61 746f  lationsCalculato
+00008690: 7228 6261 7369 7320 3d20 6261 7369 732c  r(basis = basis,
+000086a0: 2070 6172 656e 745f 6c61 7474 6963 6520   parent_lattice 
+000086b0: 3d20 7373 6574 2e67 6574 5f70 6172 656e  = sset.get_paren
+000086c0: 745f 6c61 7474 6963 6528 292c 2063 6c75  t_lattice(), clu
+000086d0: 7374 6572 735f 706f 6f6c 203d 2063 706f  sters_pool = cpo
+000086e0: 6f6c 290a 2020 2020 2020 2020 636f 6d61  ol).        coma
+000086f0: 7420 3d20 6363 616c 632e 6765 745f 636f  t = ccalc.get_co
+00008700: 7272 656c 6174 696f 6e5f 6d61 7472 6978  rrelation_matrix
+00008710: 2873 7365 7429 0a0a 2020 2020 6e73 7472  (sset)..    nstr
+00008720: 203d 206c 656e 2873 7365 7429 0a0a 2020   = len(sset)..  
+00008730: 2020 6372 6f73 7365 646f 7574 203d 205b    crossedout = [
+00008740: 5d0a 2020 2020 6964 5f73 7472 5f6c 6973  ].    id_str_lis
+00008750: 7420 3d20 7b7d 0a20 2020 2066 6f72 2069  t = {}.    for i
+00008760: 2069 6e20 7261 6e67 6528 6e73 7472 293a   in range(nstr):
+00008770: 0a20 2020 2020 2020 2069 6620 6920 6e6f  .        if i no
+00008780: 7420 696e 2063 726f 7373 6564 6f75 743a  t in crossedout:
+00008790: 0a20 2020 2020 2020 2020 2020 2063 726f  .            cro
+000087a0: 7373 6564 6f75 742e 6170 7065 6e64 2869  ssedout.append(i
+000087b0: 290a 2020 2020 2020 2020 2020 2020 7375  ).            su
+000087c0: 6273 6574 203d 205b 695d 0a0a 2020 2020  bset = [i]..    
+000087d0: 2020 2020 2020 2020 6966 2063 6f6d 6174          if comat
+000087e0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000087f0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00008800: 7272 5f69 203d 2063 6f6d 6174 5b69 2c3a  rr_i = comat[i,:
+00008810: 5d0a 2020 2020 2020 2020 2020 2020 656c  ].            el
+00008820: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00008830: 2020 2020 6174 6f6d 735f 6920 3d20 7373      atoms_i = ss
+00008840: 6574 5b69 5d2e 6765 745f 6174 6f6d 7328  et[i].get_atoms(
+00008850: 290a 0a20 2020 2020 2020 2020 2020 2066  )..            f
+00008860: 6f72 206a 2069 6e20 7261 6e67 6528 692b  or j in range(i+
+00008870: 312c 206e 7374 7229 3a0a 0a20 2020 2020  1, nstr):..     
+00008880: 2020 2020 2020 2020 2020 2069 6620 636f             if co
+00008890: 6d61 7420 6973 206e 6f74 204e 6f6e 653a  mat is not None:
+000088a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000088b0: 2020 2020 2063 6f72 725f 6a20 3d20 636f       corr_j = co
+000088c0: 6d61 745b 6a2c 3a5d 0a20 2020 2020 2020  mat[j,:].       
+000088d0: 2020 2020 2020 2020 2020 2020 2063 6865               che
+000088e0: 636b 203d 2069 7363 6c6f 7365 2863 6f72  ck = isclose(cor
+000088f0: 725f 692c 2063 6f72 725f 6a29 0a20 2020  r_i, corr_j).   
+00008900: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00008910: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00008920: 2020 2020 2020 2061 746f 6d73 5f6a 203d         atoms_j =
+00008930: 2073 7365 745b 6a5d 2e67 6574 5f61 746f   sset[j].get_ato
+00008940: 6d73 2829 0a20 2020 2020 2020 2020 2020  ms().           
+00008950: 2020 2020 2020 2020 2063 6865 636b 203d           check =
+00008960: 2063 6f6d 702e 636f 6d70 6172 6528 6174   comp.compare(at
+00008970: 6f6d 735f 692c 2061 746f 6d73 5f6a 290a  oms_i, atoms_j).
+00008980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008990: 2069 6620 6368 6563 6b3a 0a20 2020 2020   if check:.     
+000089a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000089b0: 726f 7373 6564 6f75 742e 6170 7065 6e64  rossedout.append
+000089c0: 286a 290a 2020 2020 2020 2020 2020 2020  (j).            
+000089d0: 2020 2020 2020 2020 7375 6273 6574 2e61          subset.a
+000089e0: 7070 656e 6428 6a29 0a0a 2020 2020 2020  ppend(j)..      
+000089f0: 2020 2020 2020 6964 5f73 7472 5f6c 6973        id_str_lis
+00008a00: 745b 695d 203d 206e 702e 6172 7261 7928  t[i] = np.array(
+00008a10: 7375 6273 6574 2c20 6474 7970 653d 2769  subset, dtype='i
+00008a20: 3427 290a 0a20 2020 2069 6620 7072 6574  4')..    if pret
+00008a30: 7479 5f70 7269 6e74 3a0a 2020 2020 2020  ty_print:.      
+00008a40: 2020 7072 696e 7428 6964 5f73 7472 5f6c    print(id_str_l
+00008a50: 6973 7429 0a0a 2020 2020 7265 7475 726e  ist)..    return
+00008a60: 2069 645f 7374 725f 6c69 7374 0a0a 6465   id_str_list..de
+00008a70: 6620 6174 6f6d 735f 6571 7569 7661 6c65  f atoms_equivale
+00008a80: 6e63 655f 6368 6563 6b28 6174 6f6d 732c  nce_check(atoms,
+00008a90: 2074 6f5f 7072 696d 6974 6976 6520 3d20   to_primitive = 
+00008aa0: 5472 7565 2c20 7072 6574 7479 5f70 7269  True, pretty_pri
+00008ab0: 6e74 203d 2046 616c 7365 293a 0a20 2020  nt = False):.   
+00008ac0: 2022 2222 4669 6e64 2065 7175 6976 616c   """Find equival
+00008ad0: 656e 7420 7374 7275 6374 7572 6573 2069  ent structures i
+00008ae0: 6e20 616e 2061 7272 6179 206f 6620 4174  n an array of At
+00008af0: 6f6d 7320 6f62 6a65 6374 730a 0a20 2020  oms objects..   
+00008b00: 2045 7175 6976 616c 656e 6365 2069 7320   Equivalence is 
+00008b10: 6465 7465 726d 696e 6564 2069 6e20 7465  determined in te
+00008b20: 726d 7320 6f66 2073 796d 6d65 7472 7920  rms of symmetry 
+00008b30: 6265 7477 6565 6e20 7374 7275 6374 7572  between structur
+00008b40: 6573 0a0a 2020 2020 5468 6520 6053 796d  es..    The `Sym
+00008b50: 6d65 7472 7945 7175 6976 616c 656e 6365  metryEquivalence
+00008b60: 4368 6563 6b20 746f 6f6c 206f 6620 4153  Check tool of AS
+00008b70: 4520 3c68 7474 7073 3a2f 2f77 696b 692e  E <https://wiki.
+00008b80: 6679 7369 6b2e 6474 752e 646b 2f61 7365  fysik.dtu.dk/ase
+00008b90: 2f61 7365 2f75 7469 6c73 2e68 746d 6c23  /ase/utils.html#
+00008ba0: 6173 652e 7574 696c 732e 7374 7275 6374  ase.utils.struct
+00008bb0: 7572 655f 636f 6d70 6172 6174 6f72 2e53  ure_comparator.S
+00008bc0: 796d 6d65 7472 7945 7175 6976 616c 656e  ymmetryEquivalen
+00008bd0: 6365 4368 6563 6b3e 605f 2069 7320 7573  ceCheck>`_ is us
+00008be0: 6564 2e0a 0a20 2020 202a 2a50 6172 616d  ed...    **Param
+00008bf0: 6574 6572 733a 2a2a 0a0a 2020 2020 6060  eters:**..    ``
+00008c00: 6174 6f6d 7360 603a 2061 7272 6179 206f  atoms``: array o
+00008c10: 6620 4174 6f6d 7320 6f62 6a65 6374 730a  f Atoms objects.
+00008c20: 2020 2020 2020 2020 5468 6520 7374 7275          The stru
+00008c30: 6374 7572 6573 2074 6f20 6265 2061 6e61  ctures to be ana
+00008c40: 6c79 7a65 642e 0a0a 2020 2020 6060 746f  lyzed...    ``to
+00008c50: 5f70 7269 6d69 7469 7665 6060 3a20 426f  _primitive``: Bo
+00008c60: 6f6c 6561 6e20 2864 6566 6175 6c74 3a20  olean (default: 
+00008c70: 6060 5472 7565 6060 290a 2020 2020 2020  ``True``).      
+00008c80: 2020 4966 2060 6054 7275 6560 6020 7468    If ``True`` th
+00008c90: 6520 7374 7275 6374 7572 6573 2061 7265  e structures are
+00008ca0: 2072 6564 7563 6564 2074 6f20 7468 6569   reduced to thei
+00008cb0: 7220 7072 696d 6974 6976 6520 6365 6c6c  r primitive cell
+00008cc0: 732e 0a20 2020 2020 2020 2054 6869 7320  s..        This 
+00008cd0: 6665 6174 7572 6520 7265 7175 6972 6573  feature requires
+00008ce0: 2060 6073 7067 6c69 6260 6020 746f 2069   ``spglib`` to i
+00008cf0: 6e73 7461 6c6c 6564 0a20 2020 2020 2020  nstalled.       
+00008d00: 2028 2a63 662e 2a20 6041 5345 2773 2053   (*cf.* `ASE's S
+00008d10: 796d 6d65 7472 7945 7175 6976 616c 656e  ymmetryEquivalen
+00008d20: 6365 4368 6563 6b20 3c68 7474 7073 3a2f  ceCheck <https:/
+00008d30: 2f77 696b 692e 6679 7369 6b2e 6474 752e  /wiki.fysik.dtu.
+00008d40: 646b 2f61 7365 2f61 7365 2f75 7469 6c73  dk/ase/ase/utils
+00008d50: 2e68 746d 6c3f 6869 6768 6c69 6768 743d  .html?highlight=
+00008d60: 746f 5f70 7269 6d69 7469 7665 2361 7365  to_primitive#ase
+00008d70: 2e75 7469 6c73 2e73 7472 7563 7475 7265  .utils.structure
+00008d80: 5f63 6f6d 7061 7261 746f 722e 5379 6d6d  _comparator.Symm
+00008d90: 6574 7279 4571 7569 7661 6c65 6e63 6543  etryEquivalenceC
+00008da0: 6865 636b 3e60 5f29 0a0a 0a20 2020 202a  heck>`_)...    *
+00008db0: 2a52 6574 7572 6e73 3a2a 2a0a 2020 2020  *Returns:**.    
+00008dc0: 5265 7475 726e 7320 6120 6469 6374 696f  Returns a dictio
+00008dd0: 6e61 7279 2e20 5468 6520 6b65 7973 2028  nary. The keys (
+00008de0: 6b29 2061 7265 2073 7472 7563 7475 7265  k) are structure
+00008df0: 2069 6e64 6963 6573 206f 6620 756e 6971   indices of uniq
+00008e00: 7565 2072 6570 7265 7365 6e74 6174 6976  ue representativ
+00008e10: 6520 7374 7275 6374 7572 6573 2c0a 2020  e structures,.  
+00008e20: 2020 616e 6420 7468 6520 7661 6c75 6573    and the values
+00008e30: 2028 7629 2061 7265 2061 7272 6179 7320   (v) are arrays 
+00008e40: 6f66 2069 6e74 6567 6572 2c20 696e 6469  of integer, indi
+00008e50: 6361 7469 6e67 2061 6c6c 2073 7472 7563  cating all struc
+00008e60: 7475 7265 2069 6e64 6963 6573 2065 7175  ture indices equ
+00008e70: 6976 616c 656e 7420 746f 206b 0a20 2020  ivalent to k.   
+00008e80: 2028 636f 6e74 6169 6e69 6e67 206b 2069   (containing k i
+00008e90: 7473 656c 6620 746f 6f29 2e20 466f 7220  tself too). For 
+00008ea0: 696e 7374 616e 6365 2c20 7468 6520 6469  instance, the di
+00008eb0: 6374 696f 6e61 7279 3a3a 0a0a 2020 2020  ctionary::..    
+00008ec0: 2020 2020 7b22 3022 3a20 5b30 2c20 312c      {"0": [0, 1,
+00008ed0: 2033 2c20 382c 2039 5d2c 0a20 2020 2020   3, 8, 9],.     
+00008ee0: 2020 2020 2232 223a 205b 322c 2035 2c20      "2": [2, 5, 
+00008ef0: 365d 2c0a 2020 2020 2020 2020 2022 3422  6],.         "4"
+00008f00: 3a20 5b34 2c20 375d 7d0a 0a20 2020 207c  : [4, 7]}..    |
+00008f10: 2069 6e64 6963 6174 6573 2074 6861 7420   indicates that 
+00008f20: 696e 2074 6865 2073 7472 7563 7475 7265  in the structure
+00008f30: 7320 7365 7420 7769 7468 2069 6e64 6963  s set with indic
+00008f40: 6573 205b 302c 2031 2c20 322c 2033 2c20  es [0, 1, 2, 3, 
+00008f50: 342c 2035 2c20 362c 2037 2c20 382c 2039  4, 5, 6, 7, 8, 9
+00008f60: 5d20 7468 6572 6520 6172 650a 2020 2020  ] there are.    
+00008f70: 2020 6a75 7374 2074 6872 6565 2064 6973    just three dis
+00008f80: 7469 6e63 7420 7374 7275 6374 7572 6573  tinct structures
+00008f90: 2e20 5468 6573 6520 6361 6e20 6265 2072  . These can be r
+00008fa0: 6570 7265 7365 6e74 6564 2062 7920 7374  epresented by st
+00008fb0: 7275 6375 7472 6573 2030 2c20 3220 616e  rucutres 0, 2 an
+00008fc0: 6420 342e 0a20 2020 2020 2054 6865 2073  d 4..      The s
+00008fd0: 7472 7563 7475 7265 7320 5b30 2c20 312c  tructures [0, 1,
+00008fe0: 2033 2c20 382c 2039 5d20 6172 6520 616c   3, 8, 9] are al
+00008ff0: 6c20 6571 7569 7661 6c65 6e74 2c20 6574  l equivalent, et
+00009000: 632e 0a20 2020 207c 204e 6f74 6963 6520  c..    | Notice 
+00009010: 7468 6174 2068 6572 6520 6571 7569 7661  that here equiva
+00009020: 6c65 6e63 6520 6973 2075 7365 6420 696e  lence is used in
+00009030: 2074 6865 2073 656e 7365 2065 7870 6c61   the sense expla
+00009040: 696e 6564 2061 626f 7665 3a20 4974 2069  ined above: It i
+00009050: 7320 7379 6d6d 6574 7269 6361 6c0a 2020  s symmetrical.  
+00009060: 2020 2020 6571 7569 7661 6c65 6e63 6520      equivalence 
+00009070: 6f6e 6c79 2069 6620 6060 6370 6f6f 6c60  only if ``cpool`
+00009080: 6020 616e 6420 6060 636f 6d61 7460 6020  ` and ``comat`` 
+00009090: 6172 6520 4e6f 6e65 2e0a 2020 2020 2222  are None..    ""
+000090a0: 220a 2020 2020 696d 706f 7274 206e 756d  ".    import num
+000090b0: 7079 2061 7320 6e70 0a0a 2020 2020 6672  py as np..    fr
+000090c0: 6f6d 2063 6c75 7374 6572 782e 7574 696c  om clusterx.util
+000090d0: 7320 696d 706f 7274 2069 7363 6c6f 7365  s import isclose
+000090e0: 0a0a 2020 2020 6672 6f6d 2061 7365 2e75  ..    from ase.u
+000090f0: 7469 6c73 2e73 7472 7563 7475 7265 5f63  tils.structure_c
+00009100: 6f6d 7061 7261 746f 7220 696d 706f 7274  omparator import
+00009110: 2053 796d 6d65 7472 7945 7175 6976 616c   SymmetryEquival
+00009120: 656e 6365 4368 6563 6b0a 2020 2020 636f  enceCheck.    co
+00009130: 6d70 203d 2053 796d 6d65 7472 7945 7175  mp = SymmetryEqu
+00009140: 6976 616c 656e 6365 4368 6563 6b28 746f  ivalenceCheck(to
+00009150: 5f70 7269 6d69 7469 7665 203d 2074 6f5f  _primitive = to_
+00009160: 7072 696d 6974 6976 6529 0a0a 2020 2020  primitive)..    
+00009170: 6e73 7472 203d 206c 656e 2861 746f 6d73  nstr = len(atoms
+00009180: 290a 0a20 2020 2063 726f 7373 6564 6f75  )..    crossedou
+00009190: 7420 3d20 5b5d 0a20 2020 2069 645f 7374  t = [].    id_st
+000091a0: 725f 6c69 7374 203d 207b 7d0a 2020 2020  r_list = {}.    
+000091b0: 666f 7220 6920 696e 2072 616e 6765 286e  for i in range(n
+000091c0: 7374 7229 3a0a 2020 2020 2020 2020 6966  str):.        if
+000091d0: 2069 206e 6f74 2069 6e20 6372 6f73 7365   i not in crosse
+000091e0: 646f 7574 3a0a 2020 2020 2020 2020 2020  dout:.          
+000091f0: 2020 6372 6f73 7365 646f 7574 2e61 7070    crossedout.app
+00009200: 656e 6428 6929 0a20 2020 2020 2020 2020  end(i).         
+00009210: 2020 2073 7562 7365 7420 3d20 5b69 5d0a     subset = [i].
+00009220: 0a20 2020 2020 2020 2020 2020 2061 746f  .            ato
+00009230: 6d73 5f69 203d 2061 746f 6d73 5b69 5d0a  ms_i = atoms[i].
+00009240: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00009250: 206a 2069 6e20 7261 6e67 6528 692b 312c   j in range(i+1,
+00009260: 206e 7374 7229 3a0a 0a20 2020 2020 2020   nstr):..       
+00009270: 2020 2020 2020 2020 2061 746f 6d73 5f6a           atoms_j
+00009280: 203d 2061 746f 6d73 5b6a 5d0a 2020 2020   = atoms[j].    
+00009290: 2020 2020 2020 2020 2020 2020 6368 6563              chec
+000092a0: 6b20 3d20 636f 6d70 2e63 6f6d 7061 7265  k = comp.compare
+000092b0: 2861 746f 6d73 5f69 2c20 6174 6f6d 735f  (atoms_i, atoms_
+000092c0: 6a29 0a0a 2020 2020 2020 2020 2020 2020  j)..            
+000092d0: 2020 2020 6966 2063 6865 636b 3a0a 2020      if check:.  
+000092e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000092f0: 2020 6372 6f73 7365 646f 7574 2e61 7070    crossedout.app
+00009300: 656e 6428 6a29 0a20 2020 2020 2020 2020  end(j).         
+00009310: 2020 2020 2020 2020 2020 2073 7562 7365             subse
+00009320: 742e 6170 7065 6e64 286a 290a 0a20 2020  t.append(j)..   
+00009330: 2020 2020 2020 2020 2069 645f 7374 725f           id_str_
+00009340: 6c69 7374 5b69 5d20 3d20 6e70 2e61 7272  list[i] = np.arr
+00009350: 6179 2873 7562 7365 742c 2064 7479 7065  ay(subset, dtype
+00009360: 3d27 6934 2729 0a0a 2020 2020 6966 2070  ='i4')..    if p
+00009370: 7265 7474 795f 7072 696e 743a 0a20 2020  retty_print:.   
+00009380: 2020 2020 2070 7269 6e74 2869 645f 7374       print(id_st
+00009390: 725f 6c69 7374 290a 0a20 2020 2072 6574  r_list)..    ret
+000093a0: 7572 6e20 6964 5f73 7472 5f6c 6973 740a  urn id_str_list.
+000093b0: 0a0a 6465 6620 7265 706f 7274 5f73 7365  ..def report_sse
+000093c0: 745f 6571 7569 7661 6c65 6e63 655f 6368  t_equivalence_ch
+000093d0: 6563 6b28 7373 6574 2c20 7373 6574 5f65  eck(sset, sset_e
+000093e0: 7175 6976 616c 656e 6365 5f63 6865 636b  quivalence_check
+000093f0: 5f6f 7574 7075 742c 2070 726f 7065 7274  _output, propert
+00009400: 795f 6e61 6d65 203d 204e 6f6e 652c 2074  y_name = None, t
+00009410: 6f6c 203d 2030 2e30 293a 0a20 2020 2022  ol = 0.0):.    "
+00009420: 2222 4765 6e65 7261 7465 2072 6570 6f72  ""Generate repor
+00009430: 7420 6f66 2065 7175 6976 616c 656e 7420  t of equivalent 
+00009440: 7374 7275 6374 7572 6573 0a0a 2020 2020  structures..    
+00009450: 5772 6974 6573 2074 6f20 6669 6c65 733a  Writes to files:
+00009460: 2060 6073 7365 745f 756e 6971 7565 5f73   ``sset_unique_s
+00009470: 796d 2e6a 736f 6e60 6020 616e 6420 6060  ym.json`` and ``
+00009480: 7373 6574 5f75 6e69 7175 655f 6773 732e  sset_unique_gss.
+00009490: 6a73 6f6e 6060 2e0a 0a20 2020 2054 6865  json``...    The
+000094a0: 2066 6972 7374 2063 6f6e 7461 696e 7320   first contains 
+000094b0: 7468 6520 7374 7275 6374 7572 6573 2077  the structures w
+000094c0: 686f 7365 2069 6e64 6578 2061 7265 2067  hose index are g
+000094d0: 6976 656e 2062 7920 7468 6520 6b65 7973  iven by the keys
+000094e0: 206f 6620 7468 6520 6469 6374 696f 6e61   of the dictiona
+000094f0: 7279 0a20 2020 2072 6574 7572 6e65 6420  ry.    returned 
+00009500: 6279 2060 6073 7365 745f 6571 7569 7661  by ``sset_equiva
+00009510: 6c65 6e63 655f 6368 6563 6b28 2960 602e  lence_check()``.
+00009520: 0a0a 2020 2020 5468 6520 7365 636f 6e64  ..    The second
+00009530: 2063 6f6e 7461 696e 7320 7468 6520 7374   contains the st
+00009540: 7275 6374 7572 6573 206f 6620 6576 6572  ructures of ever
+00009550: 7920 6571 7569 7661 6c65 6e63 6520 7375  y equivalence su
+00009560: 6273 6574 2077 6865 7265 2074 6865 2076  bset where the v
+00009570: 616c 7565 206f 660a 2020 2020 6060 7072  alue of.    ``pr
+00009580: 6f70 6572 7479 5f6e 616d 6560 6020 6973  operty_name`` is
+00009590: 206d 696e 696d 616c 2e20 536f 2c20 6966   minimal. So, if
+000095a0: 2074 6865 2070 726f 7065 7274 7920 6973   the property is
+000095b0: 2061 6e20 656e 6572 6779 2c20 7468 6520   an energy, the 
+000095c0: 6669 6e61 6c20 7365 7420 7769 6c6c 2063  final set will c
+000095d0: 6f6e 7461 696e 2061 6c6c 0a20 2020 206c  ontain all.    l
+000095e0: 6f77 6573 7420 656e 6572 6779 2073 7472  owest energy str
+000095f0: 7563 7475 7265 7320 6f66 2065 7665 7279  uctures of every
+00009600: 2065 7175 6976 616c 656e 6365 2073 7562   equivalence sub
+00009610: 7365 742e 0a0a 2020 2020 2222 220a 2020  set...    """.  
+00009620: 2020 696d 706f 7274 206f 7065 7261 746f    import operato
+00009630: 720a 0a20 2020 2066 6f6c 6465 7273 203d  r..    folders =
+00009640: 2073 7365 742e 6765 745f 666f 6c64 6572   sset.get_folder
+00009650: 7328 290a 0a20 2020 2069 645f 7374 725f  s()..    id_str_
+00009660: 6c69 7374 203d 2073 7365 745f 6571 7569  list = sset_equi
+00009670: 7661 6c65 6e63 655f 6368 6563 6b5f 6f75  valence_check_ou
+00009680: 7470 7574 0a0a 2020 2020 756e 6971 7565  tput..    unique
+00009690: 203d 205b 5d0a 2020 2020 666f 7220 6b2c   = [].    for k,
+000096a0: 2076 2069 6e20 6964 5f73 7472 5f6c 6973   v in id_str_lis
+000096b0: 742e 6974 656d 7328 293a 0a20 2020 2020  t.items():.     
+000096c0: 2020 2075 6e69 7175 652e 6170 7065 6e64     unique.append
+000096d0: 2876 5b30 5d29 0a0a 2020 2020 7373 6574  (v[0])..    sset
+000096e0: 5f75 6e69 7175 6520 3d20 7373 6574 2e67  _unique = sset.g
+000096f0: 6574 5f73 7562 7365 7428 756e 6971 7565  et_subset(unique
+00009700: 290a 2020 2020 7373 6574 5f75 6e69 7175  ).    sset_uniqu
+00009710: 652e 7365 7269 616c 697a 6528 2273 7365  e.serialize("sse
+00009720: 745f 756e 6971 7565 5f73 796d 2e6a 736f  t_unique_sym.jso
+00009730: 6e22 2c20 6f76 6572 7772 6974 6520 3d20  n", overwrite = 
+00009740: 5472 7565 290a 0a20 2020 2075 6e69 7175  True)..    uniqu
+00009750: 655f 6773 7320 3d20 5b5d 2023 2043 6f6c  e_gss = [] # Col
+00009760: 6c65 6374 2074 6865 206c 6f77 6573 7420  lect the lowest 
+00009770: 656e 6572 6779 2073 7472 7563 7475 7265  energy structure
+00009780: 2066 726f 6d20 6561 6368 2073 7562 7365   from each subse
+00009790: 740a 2020 2020 7076 616c 7320 3d20 7373  t.    pvals = ss
+000097a0: 6574 2e67 6574 5f70 726f 7065 7274 795f  et.get_property_
+000097b0: 7661 6c75 6573 2870 726f 7065 7274 795f  values(property_
+000097c0: 6e61 6d65 290a 2020 2020 666f 7220 6b2c  name).    for k,
+000097d0: 2076 2069 6e20 6964 5f73 7472 5f6c 6973   v in id_str_lis
+000097e0: 742e 6974 656d 7328 293a 0a20 2020 2020  t.items():.     
+000097f0: 2020 2069 6620 6c65 6e28 7629 203e 2031     if len(v) > 1
+00009800: 3a0a 2020 2020 2020 2020 2020 2020 7076  :.            pv
+00009810: 616c 735f 7375 6273 6574 203d 206f 7065  als_subset = ope
+00009820: 7261 746f 722e 6974 656d 6765 7474 6572  rator.itemgetter
+00009830: 282a 7629 2870 7661 6c73 290a 2020 2020  (*v)(pvals).    
+00009840: 2020 2020 2020 2020 695f 6d69 6e20 3d20          i_min = 
+00009850: 6e70 2e61 7267 6d69 6e28 7076 616c 735f  np.argmin(pvals_
+00009860: 7375 6273 6574 290a 2020 2020 2020 2020  subset).        
+00009870: 2020 2020 2375 6e69 7175 655f 6773 732e      #unique_gss.
+00009880: 6170 7065 6e64 2869 5f6d 696e 290a 2020  append(i_min).  
+00009890: 2020 2020 2020 2020 2020 756e 6971 7565            unique
+000098a0: 5f67 7373 2e61 7070 656e 6428 765b 695f  _gss.append(v[i_
+000098b0: 6d69 6e5d 290a 2020 2020 2020 2020 656c  min]).        el
+000098c0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000098d0: 756e 6971 7565 5f67 7373 2e61 7070 656e  unique_gss.appen
+000098e0: 6428 765b 305d 290a 0a20 2020 2073 7365  d(v[0])..    sse
+000098f0: 745f 756e 6971 7565 5f67 7373 203d 2073  t_unique_gss = s
+00009900: 7365 742e 6765 745f 7375 6273 6574 2875  set.get_subset(u
+00009910: 6e69 7175 655f 6773 7329 0a20 2020 2073  nique_gss).    s
+00009920: 7365 745f 756e 6971 7565 5f67 7373 2e73  set_unique_gss.s
+00009930: 6572 6961 6c69 7a65 2822 7373 6574 5f75  erialize("sset_u
+00009940: 6e69 7175 655f 6773 732e 6a73 6f6e 222c  nique_gss.json",
+00009950: 206f 7665 7277 7269 7465 203d 2054 7275   overwrite = Tru
+00009960: 6529 0a0a 2020 2020 6465 6369 6d20 3d20  e)..    decim = 
+00009970: 350a 2020 2020 746f 6c20 3d20 746f 6c0a  5.    tol = tol.
+00009980: 2020 2020 7072 696e 7428 2253 7472 7563      print("Struc
+00009990: 7475 7265 2069 6e64 6963 6573 2073 7461  ture indices sta
+000099a0: 7274 2066 726f 6d20 3120 2863 6f72 7265  rt from 1 (corre
+000099b0: 7370 6f6e 6469 6e67 2074 6f20 7373 6574  sponding to sset
+000099c0: 5b30 5d29 2e22 290a 2020 2020 7072 696e  [0]).").    prin
+000099d0: 7428 6627 666c 6f61 7473 2073 686f 776e  t(f'floats shown
+000099e0: 2062 656c 6f77 2061 7265 2072 6f75 6e64   below are round
+000099f0: 6564 2074 6f20 7b64 6563 696d 7d20 6465  ed to {decim} de
+00009a00: 6369 6d61 6c73 2e27 290a 2020 2020 7072  cimals.').    pr
+00009a10: 696e 7428 6627 5368 6f77 206f 6e6c 7920  int(f'Show only 
+00009a20: 7365 7473 2077 6865 7265 206d 6178 696d  sets where maxim
+00009a30: 756d 2065 6e65 7267 7920 7661 7269 6174  um energy variat
+00009a40: 696f 6e20 6973 206c 6172 6765 7220 7468  ion is larger th
+00009a50: 616e 207b 746f 6c7d 2e27 290a 2020 2020  an {tol}.').    
+00009a60: 666f 7220 6b2c 2076 2069 6e20 6964 5f73  for k, v in id_s
+00009a70: 7472 5f6c 6973 742e 6974 656d 7328 293a  tr_list.items():
+00009a80: 0a20 2020 2020 2020 2073 7562 7365 7420  .        subset 
+00009a90: 3d20 7373 6574 2e67 6574 5f73 7562 7365  = sset.get_subse
+00009aa0: 7428 7629 0a20 2020 2020 2020 2070 7661  t(v).        pva
+00009ab0: 6c73 203d 2073 7562 7365 742e 6765 745f  ls = subset.get_
+00009ac0: 7072 6f70 6572 7479 5f76 616c 7565 7328  property_values(
+00009ad0: 7072 6f70 6572 7479 5f6e 616d 6529 0a20  property_name). 
+00009ae0: 2020 2020 2020 2065 6469 6666 203d 2072         ediff = r
+00009af0: 6f75 6e64 286e 702e 616d 6178 2870 7661  ound(np.amax(pva
+00009b00: 6c73 292d 6e70 2e61 6d69 6e28 7076 616c  ls)-np.amin(pval
+00009b10: 7329 2c64 6563 696d 290a 2020 2020 2020  s),decim).      
+00009b20: 2020 6966 206c 656e 2876 2920 3e20 3120    if len(v) > 1 
+00009b30: 616e 6420 6564 6966 663e 3d74 6f6c 3a0a  and ediff>=tol:.
+00009b40: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00009b50: 7428 225c 6e3d 3d3d 3d3d 3d3d 3d3d 3d3d  t("\n===========
+00009b60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00009b70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00009b80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d22 290a  =============").
+00009b90: 2020 2020 2020 2020 2020 2020 2373 7562              #sub
+00009ba0: 7365 7420 3d20 7373 6574 2e67 6574 5f73  set = sset.get_s
+00009bb0: 7562 7365 7428 7629 0a20 2020 2020 2020  ubset(v).       
+00009bc0: 2020 2020 2073 7562 7365 742e 7365 7269       subset.seri
+00009bd0: 616c 697a 6528 6627 7265 7065 7469 7469  alize(f'repetiti
+00009be0: 6f6e 732d 7b6b 7d2e 6a73 6f6e 2729 0a20  ons-{k}.json'). 
+00009bf0: 2020 2020 2020 2020 2020 2023 7076 616c             #pval
+00009c00: 7320 3d20 7375 6273 6574 2e67 6574 5f70  s = subset.get_p
+00009c10: 726f 7065 7274 795f 7661 6c75 6573 2827  roperty_values('
+00009c20: 656e 6572 6779 5f6d 6978 696e 675f 6174  energy_mixing_at
+00009c30: 6f6d 2729 0a20 2020 2020 2020 2020 2020  om').           
+00009c40: 2023 7072 696e 7428 6b2c 2070 7661 6c73   #print(k, pvals
+00009c50: 290a 2020 2020 2020 2020 2020 2020 2370  ).            #p
+00009c60: 7269 6e74 286b 2c20 726f 756e 6428 6e70  rint(k, round(np
+00009c70: 2e61 6d61 7828 7076 616c 7329 2d6e 702e  .amax(pvals)-np.
+00009c80: 616d 696e 2870 7661 6c73 292c 3529 2c20  amin(pvals),5), 
+00009c90: 6e70 2e61 726f 756e 6428 7076 616c 732c  np.around(pvals,
+00009ca0: 2064 6563 696d 616c 7320 3d20 3529 290a   decimals = 5)).
+00009cb0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00009cc0: 7428 6627 466f 756e 6420 7b6c 656e 2870  t(f'Found {len(p
+00009cd0: 7661 6c73 297d 2073 7472 7563 7475 7265  vals)} structure
+00009ce0: 7320 706f 7373 6962 6c79 2065 7175 6976  s possibly equiv
+00009cf0: 616c 656e 7420 746f 2073 7472 7563 7475  alent to structu
+00009d00: 7265 3a27 290a 2020 2020 2020 2020 2020  re:').          
+00009d10: 2020 7072 696e 7428 6b2b 3129 0a20 2020    print(k+1).   
+00009d20: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
+00009d30: 4c69 7374 206f 6620 7374 7220 696e 6469  List of str indi
+00009d40: 6365 733a 2229 0a20 2020 2020 2020 2020  ces:").         
+00009d50: 2020 2070 7269 6e74 286e 702e 6172 7261     print(np.arra
+00009d60: 7928 6964 5f73 7472 5f6c 6973 745b 6b5d  y(id_str_list[k]
+00009d70: 292b 3129 0a20 2020 2020 2020 2020 2020  )+1).           
+00009d80: 2070 7269 6e74 2822 456e 6572 6769 6573   print("Energies
+00009d90: 2066 6f72 2074 6865 7365 2073 7472 7563   for these struc
+00009da0: 7475 7265 733a 2229 0a20 2020 2020 2020  tures:").       
+00009db0: 2020 2020 2070 7269 6e74 286e 702e 6172       print(np.ar
+00009dc0: 6f75 6e64 2870 7661 6c73 2c20 6465 6369  ound(pvals, deci
+00009dd0: 6d61 6c73 203d 2064 6563 696d 2929 0a20  mals = decim)). 
+00009de0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00009df0: 2822 4469 6666 6572 656e 6365 2062 6574  ("Difference bet
+00009e00: 7765 656e 206d 6178 696d 756d 2061 6e64  ween maximum and
+00009e10: 206d 696e 696d 756d 2065 6e65 7267 6965   minimum energie
+00009e20: 733a 2229 0a20 2020 2020 2020 2020 2020  s:").           
+00009e30: 2023 7072 696e 7428 726f 756e 6428 6e70   #print(round(np
+00009e40: 2e61 6d61 7828 7076 616c 7329 2d6e 702e  .amax(pvals)-np.
+00009e50: 616d 696e 2870 7661 6c73 292c 6465 6369  amin(pvals),deci
+00009e60: 6d29 290a 2020 2020 2020 2020 2020 2020  m)).            
+00009e70: 7072 696e 7428 6564 6966 6629 0a20 2020  print(ediff).   
+00009e80: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
+00009e90: 466f 6c64 6572 733a 2229 0a20 2020 2020  Folders:").     
+00009ea0: 2020 2020 2020 2070 7269 6e74 286f 7065         print(ope
+00009eb0: 7261 746f 722e 6974 656d 6765 7474 6572  rator.itemgetter
+00009ec0: 282a 6964 5f73 7472 5f6c 6973 745b 6b5d  (*id_str_list[k]
+00009ed0: 2928 666f 6c64 6572 7329 290a 2020 2020  )(folders)).    
+00009ee0: 2020 2020 2020 2020 2370 7269 6e74 2866          #print(f
+00009ef0: 6f6c 6465 7273 290a 2020 2020 2020 2020  olders).        
+00009f00: 2020 2020 2370 7269 6e74 286d 6170 2866      #print(map(f
+00009f10: 6f6c 6465 7273 2e5f 5f67 6574 6974 656d  olders.__getitem
+00009f20: 5f5f 2c20 6e70 2e61 7272 6179 2869 645f  __, np.array(id_
+00009f30: 7374 725f 6c69 7374 5b6b 5d29 2e74 6f6c  str_list[k]).tol
+00009f40: 6973 7428 2929 290a                      ist())).
```

### Comparing `clusterX-1.0.0.dev8/clusterx/calculators/emt.py` & `clusterX-2.1.0rc1/clusterx/calculators/emt.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,16 @@
     'Fe': (-3.28, 3.00, 1.493, 1.240, 2.000, 1.169, 0.00700),#same as Al
     'Si': (-3.51, 2.67, 2.476, 1.652, 2.740, 1.906, 0.00910),#same as Cu
     'Ge': (-2.96, 3.01, 2.132, 1.652, 2.790, 1.892, 0.00547),#same as Ag
     'Sn': (-3.90, 2.87, 2.773, 1.818, 3.107, 2.155, 0.00688),#same as Pd
     'Ba': (-3.80, 3.00, 2.321, 1.674, 2.873, 2.182, 0.00703),#same as Au
     'He': (-4.44, 2.60, 3.673, 1.669, 2.757, 1.948, 0.01030), #same as Ni
     'Na': (-5.10, 1.88, 0.132, 1.652, 2.790, 1.892, 0.01222), #same as N
+    'Zn': (-3.51, 2.77, 2.376, 1.652, 2.740, 1.976, 0.01010), #very similar to Cu
+    'B': (-4.80, 1.83, 0.232, 1.652, 2.790, 1.892, 0.01252), #
     'X': (-3.50, 1.81, 0.332, 1.652, 2.790, 1.892, 0.01322) #same as C
 })
 
 
 class EMT2(EMT):
     def __init__(self, **kwargs):
         EMT.__init__(self, **kwargs)
```

### Comparing `clusterX-1.0.0.dev8/LICENSE.txt` & `clusterX-2.1.0rc1/LICENSE.txt`

 * *Files identical despite different names*


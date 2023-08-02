# Comparing `tmp/clusterX-2.1.0rc1.tar.gz` & `tmp/clusterX-2.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clusterX-2.1.0rc1.tar", last modified: Wed Aug  2 08:55:17 2023, max compression
+gzip compressed data, was "clusterX-2.1.0rc2.tar", last modified: Wed Aug  2 17:10:49 2023, max compression
```

## Comparing `clusterX-2.1.0rc1.tar` & `clusterX-2.1.0rc2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 sr         (501) staff       (20)        0 2023-08-02 08:55:17.264779 clusterX-2.1.0rc1/
--rw-r--r--   0 sr         (501) staff       (20)    11477 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/COPYING
--rw-r--r--   0 sr         (501) staff       (20)    11477 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/LICENSE.txt
--rw-r--r--   0 sr         (501) staff       (20)       60 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/MANIFEST.in
--rw-r--r--   0 sr         (501) staff       (20)      442 2023-08-02 08:55:17.264555 clusterX-2.1.0rc1/PKG-INFO
--rw-r--r--   0 sr         (501) staff       (20)      219 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/README.rst
-drwxr-xr-x   0 sr         (501) staff       (20)        0 2023-08-02 08:55:17.234489 clusterX-2.1.0rc1/clusterX.egg-info/
--rw-r--r--   0 sr         (501) staff       (20)      442 2023-08-02 08:55:17.000000 clusterX-2.1.0rc1/clusterX.egg-info/PKG-INFO
--rw-r--r--   0 sr         (501) staff       (20)     1938 2023-08-02 08:55:17.000000 clusterX-2.1.0rc1/clusterX.egg-info/SOURCES.txt
--rw-r--r--   0 sr         (501) staff       (20)        1 2023-08-02 08:55:17.000000 clusterX-2.1.0rc1/clusterX.egg-info/dependency_links.txt
--rw-r--r--   0 sr         (501) staff       (20)       48 2023-08-02 08:55:17.000000 clusterX-2.1.0rc1/clusterX.egg-info/entry_points.txt
--rw-r--r--   0 sr         (501) staff       (20)      101 2023-08-02 08:55:17.000000 clusterX-2.1.0rc1/clusterX.egg-info/requires.txt
--rw-r--r--   0 sr         (501) staff       (20)        9 2023-08-02 08:55:17.000000 clusterX-2.1.0rc1/clusterX.egg-info/top_level.txt
-drwxr-xr-x   0 sr         (501) staff       (20)        0 2023-08-02 08:55:17.240407 clusterX-2.1.0rc1/clusterx/
--rw-r--r--   0 sr         (501) staff       (20)      626 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/__init__.py
-drwxr-xr-x   0 sr         (501) staff       (20)        0 2023-08-02 08:55:17.240983 clusterX-2.1.0rc1/clusterx/calculators/
--rw-r--r--   0 sr         (501) staff       (20)      294 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/calculators/__init__.py
--rw-r--r--   0 sr         (501) staff       (20)     2270 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/calculators/emt.py
-drwxr-xr-x   0 sr         (501) staff       (20)        0 2023-08-02 08:55:17.251721 clusterX-2.1.0rc1/clusterx/cli/
--rw-r--r--   0 sr         (501) staff       (20)      208 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/cli/__init__.py
--rw-r--r--   0 sr         (501) staff       (20)     1648 2023-05-12 15:03:35.000000 clusterX-2.1.0rc1/clusterx/cli/commands.py
--rw-r--r--   0 sr         (501) staff       (20)      670 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/cli/main.py
--rw-r--r--   0 sr         (501) staff       (20)     1303 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/cli/plot_clusters.py
--rw-r--r--   0 sr         (501) staff       (20)     1251 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/cli/spacegroup.py
--rw-r--r--   0 sr         (501) staff       (20)     1068 2023-02-20 09:42:30.000000 clusterX-2.1.0rc1/clusterx/cli/test.py
-drwxr-xr-x   0 sr         (501) staff       (20)        0 2023-08-02 08:55:17.257886 clusterX-2.1.0rc1/clusterx/clusters/
--rw-r--r--   0 sr         (501) staff       (20)        0 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/clusters/__init__.py
--rw-r--r--   0 sr         (501) staff       (20)     9764 2023-05-09 10:16:28.000000 clusterX-2.1.0rc1/clusterx/clusters/cluster.py
--rw-r--r--   0 sr         (501) staff       (20)    62837 2023-08-01 14:57:17.000000 clusterX-2.1.0rc1/clusterx/clusters/clusters_pool.py
--rw-r--r--   0 sr         (501) staff       (20)    25723 2023-08-01 15:24:59.000000 clusterX-2.1.0rc1/clusterx/clusters_selector.py
--rw-r--r--   0 sr         (501) staff       (20)     1360 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/config.py
--rw-r--r--   0 sr         (501) staff       (20)    19100 2023-08-01 21:47:18.000000 clusterX-2.1.0rc1/clusterx/correlations.py
--rw-r--r--   0 sr         (501) staff       (20)      352 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/cross_validation.py
--rw-r--r--   0 sr         (501) staff       (20)    13889 2023-07-13 19:27:18.000000 clusterX-2.1.0rc1/clusterx/derivative_structures.py
-drwxr-xr-x   0 sr         (501) staff       (20)        0 2023-08-02 08:55:17.258622 clusterX-2.1.0rc1/clusterx/estimators/
--rw-r--r--   0 sr         (501) staff       (20)        0 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/estimators/__init__.py
--rw-r--r--   0 sr         (501) staff       (20)     2984 2023-04-19 22:26:52.000000 clusterX-2.1.0rc1/clusterx/estimators/estimator_factory.py
-drwxr-xr-x   0 sr         (501) staff       (20)        0 2023-08-02 08:55:17.259427 clusterX-2.1.0rc1/clusterx/io/
--rw-r--r--   0 sr         (501) staff       (20)      208 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/io/__init__.py
--rw-r--r--   0 sr         (501) staff       (20)     1393 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/io/atat.py
--rw-r--r--   0 sr         (501) staff       (20)      484 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/io/formats.py
--rw-r--r--   0 sr         (501) staff       (20)     2283 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/lattices.py
--rw-r--r--   0 sr         (501) staff       (20)    27785 2023-08-01 21:28:28.000000 clusterX-2.1.0rc1/clusterx/model.py
--rw-r--r--   0 sr         (501) staff       (20)    25400 2023-06-05 13:52:00.000000 clusterX-2.1.0rc1/clusterx/parent_lattice.py
--rw-r--r--   0 sr         (501) staff       (20)    14639 2023-05-20 07:55:32.000000 clusterX-2.1.0rc1/clusterx/structure.py
--rw-r--r--   0 sr         (501) staff       (20)    11069 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/structure_selector.py
--rw-r--r--   0 sr         (501) staff       (20)    35864 2023-06-29 08:23:54.000000 clusterX-2.1.0rc1/clusterx/structures_set.py
--rw-r--r--   0 sr         (501) staff       (20)    21924 2023-04-24 21:21:23.000000 clusterX-2.1.0rc1/clusterx/super_cell.py
--rw-r--r--   0 sr         (501) staff       (20)     3653 2023-03-24 12:44:22.000000 clusterX-2.1.0rc1/clusterx/symmetry.py
-drwxr-xr-x   0 sr         (501) staff       (20)        0 2023-08-02 08:55:17.264294 clusterX-2.1.0rc1/clusterx/test/
--rw-r--r--   0 sr         (501) staff       (20)      434 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/__init__.py
--rw-r--r--   0 sr         (501) staff       (20)     3071 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_clathrate_mc.py
--rw-r--r--   0 sr         (501) staff       (20)     2315 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_cluster.py
--rw-r--r--   0 sr         (501) staff       (20)     5390 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_cluster_correlations.py
--rw-r--r--   0 sr         (501) staff       (20)     7527 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_cluster_expansion.py
--rw-r--r--   0 sr         (501) staff       (20)    14654 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_cluster_orbit.py
--rw-r--r--   0 sr         (501) staff       (20)    12876 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_cluster_orbit2.py
--rw-r--r--   0 sr         (501) staff       (20)    13813 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_clusters_generation.py
--rw-r--r--   0 sr         (501) staff       (20)     7628 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_clusters_selector.py
--rw-r--r--   0 sr         (501) staff       (20)     7744 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_clusters_selector_lasso.py
--rw-r--r--   0 sr         (501) staff       (20)     2132 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_concentration.py
--rw-r--r--   0 sr         (501) staff       (20)     2926 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_emt2_calculator.py
--rw-r--r--   0 sr         (501) staff       (20)     2346 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_folders.py
--rw-r--r--   0 sr         (501) staff       (20)     1491 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_get_all_hnf.py
--rw-r--r--   0 sr         (501) staff       (20)     3954 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_get_unique_supercells.py
--rw-r--r--   0 sr         (501) staff       (20)     1418 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_is_nary.py
--rw-r--r--   0 sr         (501) staff       (20)     3994 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_lattice_representation.py
--rw-r--r--   0 sr         (501) staff       (20)    23113 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_metropolis.py
--rw-r--r--   0 sr         (501) staff       (20)     8623 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_parent_lattice_creation.py
--rw-r--r--   0 sr         (501) staff       (20)     4577 2023-02-16 09:24:07.000000 clusterX-2.1.0rc1/clusterx/test/test_predict_swap.py
--rw-r--r--   0 sr         (501) staff       (20)     7625 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_structure_selector.py
--rw-r--r--   0 sr         (501) staff       (20)     1834 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_structures_set.py
--rw-r--r--   0 sr         (501) staff       (20)     5713 2022-04-12 09:51:53.000000 clusterX-2.1.0rc1/clusterx/test/test_wanglandau.py
--rw-r--r--   0 sr         (501) staff       (20)    40776 2023-07-13 13:01:52.000000 clusterX-2.1.0rc1/clusterx/utils.py
--rw-r--r--   0 sr         (501) staff       (20)    26128 2023-08-01 16:48:54.000000 clusterX-2.1.0rc1/clusterx/visualization.py
--rw-r--r--   0 sr         (501) staff       (20)       38 2023-08-02 08:55:17.264830 clusterX-2.1.0rc1/setup.cfg
--rw-r--r--   0 sr         (501) staff       (20)      735 2023-08-02 08:50:16.000000 clusterX-2.1.0rc1/setup.py
+drwx------   0 srigamonti  (6002) sol       (6001)        0 2023-08-02 17:10:49.411579 clusterX-2.1.0rc2/
+-rw-------   0 srigamonti  (6002) sol       (6001)    11477 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/COPYING
+-rw-------   0 srigamonti  (6002) sol       (6001)    11477 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/LICENSE.txt
+-rw-------   0 srigamonti  (6002) sol       (6001)       60 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/MANIFEST.in
+-rw-------   0 srigamonti  (6002) sol       (6001)      442 2023-08-02 17:10:49.411579 clusterX-2.1.0rc2/PKG-INFO
+-rw-------   0 srigamonti  (6002) sol       (6001)      219 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/README.rst
+drwx------   0 srigamonti  (6002) sol       (6001)        0 2023-08-02 17:10:49.391579 clusterX-2.1.0rc2/clusterX.egg-info/
+-rw-------   0 srigamonti  (6002) sol       (6001)      442 2023-08-02 17:10:48.000000 clusterX-2.1.0rc2/clusterX.egg-info/PKG-INFO
+-rw-------   0 srigamonti  (6002) sol       (6001)     1938 2023-08-02 17:10:48.000000 clusterX-2.1.0rc2/clusterX.egg-info/SOURCES.txt
+-rw-------   0 srigamonti  (6002) sol       (6001)        1 2023-08-02 17:10:48.000000 clusterX-2.1.0rc2/clusterX.egg-info/dependency_links.txt
+-rw-------   0 srigamonti  (6002) sol       (6001)       48 2023-08-02 17:10:48.000000 clusterX-2.1.0rc2/clusterX.egg-info/entry_points.txt
+-rw-------   0 srigamonti  (6002) sol       (6001)      101 2023-08-02 17:10:48.000000 clusterX-2.1.0rc2/clusterX.egg-info/requires.txt
+-rw-------   0 srigamonti  (6002) sol       (6001)        9 2023-08-02 17:10:48.000000 clusterX-2.1.0rc2/clusterX.egg-info/top_level.txt
+drwx------   0 srigamonti  (6002) sol       (6001)        0 2023-08-02 17:10:49.399579 clusterX-2.1.0rc2/clusterx/
+-rw-------   0 srigamonti  (6002) sol       (6001)      626 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/__init__.py
+drwx------   0 srigamonti  (6002) sol       (6001)        0 2023-08-02 17:10:49.399579 clusterX-2.1.0rc2/clusterx/calculators/
+-rw-------   0 srigamonti  (6002) sol       (6001)      294 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/calculators/__init__.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     2270 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/calculators/emt.py
+drwx------   0 srigamonti  (6002) sol       (6001)        0 2023-08-02 17:10:49.403579 clusterX-2.1.0rc2/clusterx/cli/
+-rw-------   0 srigamonti  (6002) sol       (6001)      208 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/cli/__init__.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     1648 2023-05-17 17:23:39.000000 clusterX-2.1.0rc2/clusterx/cli/commands.py
+-rw-------   0 srigamonti  (6002) sol       (6001)      670 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/cli/main.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     1303 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/cli/plot_clusters.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     1251 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/cli/spacegroup.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     1068 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/cli/test.py
+drwx------   0 srigamonti  (6002) sol       (6001)        0 2023-08-02 17:10:49.403579 clusterX-2.1.0rc2/clusterx/clusters/
+-rw-------   0 srigamonti  (6002) sol       (6001)        0 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/clusters/__init__.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     9798 2023-08-02 17:06:09.000000 clusterX-2.1.0rc2/clusterx/clusters/cluster.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    62833 2023-08-02 16:45:14.000000 clusterX-2.1.0rc2/clusterx/clusters/clusters_pool.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    25723 2023-08-02 16:27:57.000000 clusterX-2.1.0rc2/clusterx/clusters_selector.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     1360 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/config.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    19100 2023-08-02 16:27:57.000000 clusterX-2.1.0rc2/clusterx/correlations.py
+-rw-------   0 srigamonti  (6002) sol       (6001)      352 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/cross_validation.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    13889 2023-07-20 22:00:43.000000 clusterX-2.1.0rc2/clusterx/derivative_structures.py
+drwx------   0 srigamonti  (6002) sol       (6001)        0 2023-08-02 17:10:49.403579 clusterX-2.1.0rc2/clusterx/estimators/
+-rw-------   0 srigamonti  (6002) sol       (6001)        0 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/estimators/__init__.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     2984 2023-05-08 09:57:44.000000 clusterX-2.1.0rc2/clusterx/estimators/estimator_factory.py
+drwx------   0 srigamonti  (6002) sol       (6001)        0 2023-08-02 17:10:49.407580 clusterX-2.1.0rc2/clusterx/io/
+-rw-------   0 srigamonti  (6002) sol       (6001)      208 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/io/__init__.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     1393 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/io/atat.py
+-rw-------   0 srigamonti  (6002) sol       (6001)      484 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/io/formats.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     2283 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/lattices.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    27785 2023-08-02 16:27:57.000000 clusterX-2.1.0rc2/clusterx/model.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    25400 2023-06-05 11:08:41.000000 clusterX-2.1.0rc2/clusterx/parent_lattice.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    14639 2023-05-10 17:03:30.000000 clusterX-2.1.0rc2/clusterx/structure.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    11069 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/structure_selector.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    35864 2023-06-23 15:37:16.000000 clusterX-2.1.0rc2/clusterx/structures_set.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    21924 2023-05-08 09:57:44.000000 clusterX-2.1.0rc2/clusterx/super_cell.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     3653 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/symmetry.py
+drwx------   0 srigamonti  (6002) sol       (6001)        0 2023-08-02 17:10:49.411579 clusterX-2.1.0rc2/clusterx/test/
+-rw-------   0 srigamonti  (6002) sol       (6001)      434 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/test/__init__.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     3071 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/test/test_clathrate_mc.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     2315 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/test/test_cluster.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     5390 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/test/test_cluster_correlations.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     7527 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/test/test_cluster_expansion.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    14654 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/test/test_cluster_orbit.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    12876 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/test/test_cluster_orbit2.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    13813 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/test/test_clusters_generation.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     7628 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/test/test_clusters_selector.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     7744 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/test/test_clusters_selector_lasso.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     2132 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/test/test_concentration.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     2926 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/test/test_emt2_calculator.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     2346 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/test/test_folders.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     1491 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/test/test_get_all_hnf.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     3954 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/test/test_get_unique_supercells.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     1418 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/test/test_is_nary.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     3994 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/test/test_lattice_representation.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    23113 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/test/test_metropolis.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     8623 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/test/test_parent_lattice_creation.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     4577 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/test/test_predict_swap.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     7625 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/test/test_structure_selector.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     1834 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/test/test_structures_set.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     5713 2023-05-08 09:50:06.000000 clusterX-2.1.0rc2/clusterx/test/test_wanglandau.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    40776 2023-07-20 22:00:43.000000 clusterX-2.1.0rc2/clusterx/utils.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    26128 2023-08-02 16:27:57.000000 clusterX-2.1.0rc2/clusterx/visualization.py
+-rw-------   0 srigamonti  (6002) sol       (6001)       38 2023-08-02 17:10:49.411579 clusterX-2.1.0rc2/setup.cfg
+-rw-------   0 srigamonti  (6002) sol       (6001)      735 2023-08-02 17:09:22.000000 clusterX-2.1.0rc2/setup.py
```

### Comparing `clusterX-2.1.0rc1/COPYING` & `clusterX-2.1.0rc2/COPYING`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/LICENSE.txt` & `clusterX-2.1.0rc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterX.egg-info/SOURCES.txt` & `clusterX-2.1.0rc2/clusterX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/__init__.py` & `clusterX-2.1.0rc2/clusterx/__init__.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/calculators/emt.py` & `clusterX-2.1.0rc2/clusterx/calculators/emt.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/cli/commands.py` & `clusterX-2.1.0rc2/clusterx/cli/commands.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/cli/main.py` & `clusterX-2.1.0rc2/clusterx/cli/main.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/cli/plot_clusters.py` & `clusterX-2.1.0rc2/clusterx/cli/plot_clusters.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/cli/spacegroup.py` & `clusterX-2.1.0rc2/clusterx/cli/spacegroup.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/cli/test.py` & `clusterX-2.1.0rc2/clusterx/cli/test.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/clusters/cluster.py` & `clusterX-2.1.0rc2/clusterx/clusters/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,16 @@
                     for i1 in range(self.npoints-1):
                         for i2 in range(i1+1, self.npoints):
                             d = np.linalg.norm(self.positions_cartesian[i1]-self.positions_cartesian[i2])
                             if r < d:
                                 r = d
             self.radius = r
 
+        self.myhash = self.__hash__()
+
     """
     def __lt__(self,other):
         if self.npoints == other.npoints:
             return self.radius < other.radius
         else:
             return self.npoints < other.npoints
     """
@@ -158,15 +160,15 @@
     def __repr__(self):
         return "Cluster["+str(list(zip(self.ais,self.ans)))+"]"
         
     def __hash__(self):
         return hash(str(list(zip(self.ais,self.ans))))
         
     def __eq__(self, other):
-        return self.__hash__ == other.__hash__ 
+        return self.myhash == other.myhash
 
     def __len__(self):
         return len(self.ais)
 
     def get_idxs(self):
         """Return array of atom indices referred to the defining supercell.
         """
```

### Comparing `clusterX-2.1.0rc1/clusterx/clusters/clusters_pool.py` & `clusterX-2.1.0rc2/clusterx/clusters/clusters_pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -1375,15 +1375,15 @@
             if i not in crossedout:
                 weights.append(1)
                 orbit.append(Cluster(_orbit[i].get_idxs(),_orbit[i].get_nrs(),super_cell,distances))
                 cnt += 1
             
                 for j in range(i+1, ncl):
                     if j not in crossedout:
-                        if _orbit[i].__hash__ == _orbit[j].__hash__:
+                        if _orbit[i].myhash == _orbit[j].myhash:
                             weights[cnt-1] += 1
                             crossedout.add(j)
                         
 
         for cl in orbit:
             self.add_cluster(cl)
```

### Comparing `clusterX-2.1.0rc1/clusterx/clusters_selector.py` & `clusterX-2.1.0rc2/clusterx/clusters_selector.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/config.py` & `clusterX-2.1.0rc2/clusterx/config.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/correlations.py` & `clusterX-2.1.0rc2/clusterx/correlations.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/derivative_structures.py` & `clusterX-2.1.0rc2/clusterx/derivative_structures.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/estimators/estimator_factory.py` & `clusterX-2.1.0rc2/clusterx/estimators/estimator_factory.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/io/atat.py` & `clusterX-2.1.0rc2/clusterx/io/atat.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/lattices.py` & `clusterX-2.1.0rc2/clusterx/lattices.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/model.py` & `clusterX-2.1.0rc2/clusterx/model.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/parent_lattice.py` & `clusterX-2.1.0rc2/clusterx/parent_lattice.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/structure.py` & `clusterX-2.1.0rc2/clusterx/structure.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/structure_selector.py` & `clusterX-2.1.0rc2/clusterx/structure_selector.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/structures_set.py` & `clusterX-2.1.0rc2/clusterx/structures_set.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/super_cell.py` & `clusterX-2.1.0rc2/clusterx/super_cell.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/symmetry.py` & `clusterX-2.1.0rc2/clusterx/symmetry.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/test/test_clathrate_mc.py` & `clusterX-2.1.0rc2/clusterx/test/test_clathrate_mc.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/test/test_cluster.py` & `clusterX-2.1.0rc2/clusterx/test/test_cluster.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/test/test_cluster_correlations.py` & `clusterX-2.1.0rc2/clusterx/test/test_cluster_correlations.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/test/test_cluster_expansion.py` & `clusterX-2.1.0rc2/clusterx/test/test_cluster_expansion.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/test/test_cluster_orbit.py` & `clusterX-2.1.0rc2/clusterx/test/test_cluster_orbit.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/test/test_cluster_orbit2.py` & `clusterX-2.1.0rc2/clusterx/test/test_cluster_orbit2.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/test/test_clusters_generation.py` & `clusterX-2.1.0rc2/clusterx/test/test_clusters_generation.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/test/test_clusters_selector.py` & `clusterX-2.1.0rc2/clusterx/test/test_clusters_selector.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/test/test_clusters_selector_lasso.py` & `clusterX-2.1.0rc2/clusterx/test/test_clusters_selector_lasso.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/test/test_concentration.py` & `clusterX-2.1.0rc2/clusterx/test/test_concentration.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/test/test_emt2_calculator.py` & `clusterX-2.1.0rc2/clusterx/test/test_emt2_calculator.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/test/test_folders.py` & `clusterX-2.1.0rc2/clusterx/test/test_folders.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/test/test_get_all_hnf.py` & `clusterX-2.1.0rc2/clusterx/test/test_get_all_hnf.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/test/test_get_unique_supercells.py` & `clusterX-2.1.0rc2/clusterx/test/test_get_unique_supercells.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/test/test_is_nary.py` & `clusterX-2.1.0rc2/clusterx/test/test_is_nary.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/test/test_lattice_representation.py` & `clusterX-2.1.0rc2/clusterx/test/test_lattice_representation.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/test/test_metropolis.py` & `clusterX-2.1.0rc2/clusterx/test/test_metropolis.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/test/test_parent_lattice_creation.py` & `clusterX-2.1.0rc2/clusterx/test/test_parent_lattice_creation.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/test/test_predict_swap.py` & `clusterX-2.1.0rc2/clusterx/test/test_predict_swap.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/test/test_structure_selector.py` & `clusterX-2.1.0rc2/clusterx/test/test_structure_selector.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/test/test_structures_set.py` & `clusterX-2.1.0rc2/clusterx/test/test_structures_set.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/test/test_wanglandau.py` & `clusterX-2.1.0rc2/clusterx/test/test_wanglandau.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/utils.py` & `clusterX-2.1.0rc2/clusterx/utils.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/clusterx/visualization.py` & `clusterX-2.1.0rc2/clusterx/visualization.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc1/setup.py` & `clusterX-2.1.0rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='clusterX',
-      version='2.1.0.rc1',
+      version='2.1.0.rc2',
       description='CELL (aka clusterX) is a python package for building Cluster Expansion models of simple and complex alloys and performing thermodynamical analyses of materials.',
       url='http://sol.physik.hu-berlin.de/cell/',
       author='CELL Developers',
       author_email='srigamonti@physik.hu-berlin.de',
       license='http://www.apache.org/licenses/LICENSE-2.0',
       packages=find_packages(),
       install_requires=['numpy', 'scipy', 'scikit-learn', 'matplotlib','ase','plac','pytest','spglib','sympy','nglview','ipywidgets','pytest-html', 'tqdm'],
```


# Comparing `tmp/vivarium-core-1.5.6.tar.gz` & `tmp/vivarium-core-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vivarium-core-1.5.6.tar", last modified: Tue May 16 13:45:18 2023, max compression
+gzip compressed data, was "vivarium-core-1.5.7.tar", last modified: Wed Aug  2 19:42:56 2023, max compression
```

## Comparing `vivarium-core-1.5.6.tar` & `vivarium-core-1.5.7.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-05-16 13:45:18.130659 vivarium-core-1.5.6/
--rw-r--r--   0 eranagmon   (502) staff       (20)      733 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/AUTHORS.md
--rw-r--r--   0 eranagmon   (502) staff       (20)    11357 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/LICENSE.txt
--rw-r--r--   0 eranagmon   (502) staff       (20)     6265 2023-05-16 13:45:18.130518 vivarium-core-1.5.6/PKG-INFO
--rw-r--r--   0 eranagmon   (502) staff       (20)     4124 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/README.md
--rw-r--r--   0 eranagmon   (502) staff       (20)       38 2023-05-16 13:45:18.130711 vivarium-core-1.5.6/setup.cfg
--rw-r--r--   0 eranagmon   (502) staff       (20)     2836 2023-05-16 13:45:05.000000 vivarium-core-1.5.6/setup.py
-drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-05-16 13:45:18.117496 vivarium-core-1.5.6/vivarium/
--rw-r--r--   0 eranagmon   (502) staff       (20)     4085 2023-05-02 22:25:02.000000 vivarium-core-1.5.6/vivarium/__init__.py
-drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-05-16 13:45:18.118086 vivarium-core-1.5.6/vivarium/composites/
--rw-r--r--   0 eranagmon   (502) staff       (20)        0 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/composites/__init__.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     1369 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/composites/injected_glc_phosphorylation.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    26070 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/composites/toys.py
-drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-05-16 13:45:18.121284 vivarium-core-1.5.6/vivarium/core/
--rw-r--r--   0 eranagmon   (502) staff       (20)        0 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/core/__init__.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    18947 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/core/composer.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    12095 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/core/composition.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     9131 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/core/control.py
--rw-r--r--   0 eranagmon   (502) staff       (20)      394 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/core/directories.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    26791 2023-05-02 22:25:02.000000 vivarium-core-1.5.6/vivarium/core/emitter.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    44691 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/core/engine.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    32987 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/core/process.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    13882 2023-05-02 22:25:02.000000 vivarium-core-1.5.6/vivarium/core/registry.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    10214 2023-05-16 13:45:05.000000 vivarium-core-1.5.6/vivarium/core/serialize.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     7123 2023-05-02 22:25:02.000000 vivarium-core-1.5.6/vivarium/core/serialize_test.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    72491 2023-05-16 13:45:05.000000 vivarium-core-1.5.6/vivarium/core/store.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     1588 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/core/types.py
-drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-05-16 13:45:18.123400 vivarium-core-1.5.6/vivarium/experiments/
--rw-r--r--   0 eranagmon   (502) staff       (20)        0 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/experiments/__init__.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     2823 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/experiments/bigraph_view.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     1005 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/experiments/composite_merge.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    36860 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/experiments/engine_tests.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     2663 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/experiments/glucose_phosphorylation.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     3446 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/experiments/hierarchy_composite_division.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     3055 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/experiments/large_experiment.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     2955 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/experiments/profile_image.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    20995 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/experiments/profile_runtime.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     8444 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/experiments/store_api.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     1429 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/experiments/test_profiler.py
-drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-05-16 13:45:18.125476 vivarium-core-1.5.6/vivarium/library/
--rw-r--r--   0 eranagmon   (502) staff       (20)        0 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/library/__init__.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     1897 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/library/datum.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    11391 2023-05-02 22:25:02.000000 vivarium-core-1.5.6/vivarium/library/dict_utils.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     3255 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/library/filepath.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     5183 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/library/make_network.py
--rw-r--r--   0 eranagmon   (502) staff       (20)      145 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/library/path.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     1803 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/library/pretty.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     1789 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/library/schema.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    11820 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/library/timeseries.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    11352 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/library/topology.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     2948 2023-05-02 22:25:02.000000 vivarium-core-1.5.6/vivarium/library/units.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     2209 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/library/wrappers.py
-drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-05-16 13:45:18.126020 vivarium-core-1.5.6/vivarium/plots/
--rw-r--r--   0 eranagmon   (502) staff       (20)        0 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/plots/__init__.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    11417 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/plots/agents_multigen.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    11493 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/plots/simulation_output.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    26041 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/plots/topology.py
-drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-05-16 13:45:18.129551 vivarium-core-1.5.6/vivarium/processes/
--rw-r--r--   0 eranagmon   (502) staff       (20)        0 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/processes/__init__.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     6105 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/processes/alternator.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     5018 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/processes/burst.py
--rw-r--r--   0 eranagmon   (502) staff       (20)      538 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/processes/clock.py
--rw-r--r--   0 eranagmon   (502) staff       (20)      949 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/processes/divide_condition.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     2413 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/processes/division.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     5685 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/processes/ecoli_shape_deriver.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     5077 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/processes/engulf.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     3480 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/processes/glucose_phosphorylation.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     3080 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/processes/growth_rate.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     3235 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/processes/injector.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     6894 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/processes/mass_adaptor.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     6681 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/processes/meta_division.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     3423 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/processes/molarity_deriver.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     2432 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/processes/nonspatial_environment.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     3244 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/processes/remove.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     1403 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/processes/strip_units.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     5558 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/processes/swap_processes.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     3745 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/processes/template_process.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     3260 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/processes/timeline.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     7701 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/processes/toy_gillespie.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     4600 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/processes/tree_mass.py
-drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-05-16 13:45:18.130318 vivarium-core-1.5.6/vivarium_core.egg-info/
--rw-r--r--   0 eranagmon   (502) staff       (20)     6265 2023-05-16 13:45:18.000000 vivarium-core-1.5.6/vivarium_core.egg-info/PKG-INFO
--rw-r--r--   0 eranagmon   (502) staff       (20)     2408 2023-05-16 13:45:18.000000 vivarium-core-1.5.6/vivarium_core.egg-info/SOURCES.txt
--rw-r--r--   0 eranagmon   (502) staff       (20)        1 2023-05-16 13:45:18.000000 vivarium-core-1.5.6/vivarium_core.egg-info/dependency_links.txt
--rw-r--r--   0 eranagmon   (502) staff       (20)       20 2023-05-16 13:45:18.000000 vivarium-core-1.5.6/vivarium_core.egg-info/entry_points.txt
--rw-r--r--   0 eranagmon   (502) staff       (20)      115 2023-05-16 13:45:18.000000 vivarium-core-1.5.6/vivarium_core.egg-info/requires.txt
--rw-r--r--   0 eranagmon   (502) staff       (20)        9 2023-05-16 13:45:18.000000 vivarium-core-1.5.6/vivarium_core.egg-info/top_level.txt
+drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-08-02 19:42:56.294458 vivarium-core-1.5.7/
+-rw-r--r--   0 eranagmon   (502) staff       (20)      733 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/AUTHORS.md
+-rw-r--r--   0 eranagmon   (502) staff       (20)    11357 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/LICENSE.txt
+-rw-r--r--   0 eranagmon   (502) staff       (20)     6266 2023-08-02 19:42:56.294339 vivarium-core-1.5.7/PKG-INFO
+-rw-r--r--   0 eranagmon   (502) staff       (20)     4124 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/README.md
+-rw-r--r--   0 eranagmon   (502) staff       (20)       38 2023-08-02 19:42:56.294505 vivarium-core-1.5.7/setup.cfg
+-rw-r--r--   0 eranagmon   (502) staff       (20)     2837 2023-08-02 19:42:18.000000 vivarium-core-1.5.7/setup.py
+drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-08-02 19:42:56.282982 vivarium-core-1.5.7/vivarium/
+-rw-r--r--   0 eranagmon   (502) staff       (20)     4085 2023-05-02 22:25:02.000000 vivarium-core-1.5.7/vivarium/__init__.py
+drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-08-02 19:42:56.283588 vivarium-core-1.5.7/vivarium/composites/
+-rw-r--r--   0 eranagmon   (502) staff       (20)        0 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/vivarium/composites/__init__.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     1369 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/vivarium/composites/injected_glc_phosphorylation.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    26072 2023-08-02 19:42:18.000000 vivarium-core-1.5.7/vivarium/composites/toys.py
+drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-08-02 19:42:56.285943 vivarium-core-1.5.7/vivarium/core/
+-rw-r--r--   0 eranagmon   (502) staff       (20)        0 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/vivarium/core/__init__.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    19080 2023-08-02 19:42:18.000000 vivarium-core-1.5.7/vivarium/core/composer.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    12165 2023-08-02 19:42:18.000000 vivarium-core-1.5.7/vivarium/core/composition.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     9133 2023-08-02 19:42:18.000000 vivarium-core-1.5.7/vivarium/core/control.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)      394 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/vivarium/core/directories.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    27151 2023-08-02 19:42:18.000000 vivarium-core-1.5.7/vivarium/core/emitter.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    44553 2023-08-02 19:42:18.000000 vivarium-core-1.5.7/vivarium/core/engine.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    33237 2023-08-02 19:42:18.000000 vivarium-core-1.5.7/vivarium/core/process.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    13882 2023-05-02 22:25:02.000000 vivarium-core-1.5.7/vivarium/core/registry.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    10248 2023-08-02 19:42:18.000000 vivarium-core-1.5.7/vivarium/core/serialize.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     7123 2023-05-02 22:25:02.000000 vivarium-core-1.5.7/vivarium/core/serialize_test.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    72491 2023-05-16 13:45:05.000000 vivarium-core-1.5.7/vivarium/core/store.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     1588 2023-05-16 13:18:03.000000 vivarium-core-1.5.7/vivarium/core/types.py
+drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-08-02 19:42:56.287987 vivarium-core-1.5.7/vivarium/experiments/
+-rw-r--r--   0 eranagmon   (502) staff       (20)        0 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/vivarium/experiments/__init__.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     2823 2023-05-16 13:18:03.000000 vivarium-core-1.5.7/vivarium/experiments/bigraph_view.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     1005 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/vivarium/experiments/composite_merge.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    36866 2023-08-02 19:42:18.000000 vivarium-core-1.5.7/vivarium/experiments/engine_tests.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     2663 2023-05-16 13:18:03.000000 vivarium-core-1.5.7/vivarium/experiments/glucose_phosphorylation.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     3451 2023-08-02 19:42:18.000000 vivarium-core-1.5.7/vivarium/experiments/hierarchy_composite_division.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     3055 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/vivarium/experiments/large_experiment.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     2955 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/vivarium/experiments/profile_image.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    20995 2023-05-16 13:18:03.000000 vivarium-core-1.5.7/vivarium/experiments/profile_runtime.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     8444 2023-05-16 13:18:03.000000 vivarium-core-1.5.7/vivarium/experiments/store_api.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     1429 2023-05-16 13:18:03.000000 vivarium-core-1.5.7/vivarium/experiments/test_profiler.py
+drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-08-02 19:42:56.289763 vivarium-core-1.5.7/vivarium/library/
+-rw-r--r--   0 eranagmon   (502) staff       (20)        0 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/vivarium/library/__init__.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     1897 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/vivarium/library/datum.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    11401 2023-08-02 19:42:18.000000 vivarium-core-1.5.7/vivarium/library/dict_utils.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     3255 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/vivarium/library/filepath.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     5183 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/vivarium/library/make_network.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)      145 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/vivarium/library/path.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     1803 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/vivarium/library/pretty.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     1789 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/vivarium/library/schema.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    11820 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/vivarium/library/timeseries.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    11352 2023-05-16 13:18:03.000000 vivarium-core-1.5.7/vivarium/library/topology.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     2948 2023-05-02 22:25:02.000000 vivarium-core-1.5.7/vivarium/library/units.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     2209 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/vivarium/library/wrappers.py
+drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-08-02 19:42:56.290299 vivarium-core-1.5.7/vivarium/plots/
+-rw-r--r--   0 eranagmon   (502) staff       (20)        0 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/vivarium/plots/__init__.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    11417 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/vivarium/plots/agents_multigen.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    11493 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/vivarium/plots/simulation_output.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    26041 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/vivarium/plots/topology.py
+drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-08-02 19:42:56.293432 vivarium-core-1.5.7/vivarium/processes/
+-rw-r--r--   0 eranagmon   (502) staff       (20)        0 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/vivarium/processes/__init__.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     6105 2023-05-16 13:18:03.000000 vivarium-core-1.5.7/vivarium/processes/alternator.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     5018 2023-05-16 13:18:03.000000 vivarium-core-1.5.7/vivarium/processes/burst.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)      538 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/vivarium/processes/clock.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)      949 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/vivarium/processes/divide_condition.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     2413 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/vivarium/processes/division.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     5685 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/vivarium/processes/ecoli_shape_deriver.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     5077 2023-05-16 13:18:03.000000 vivarium-core-1.5.7/vivarium/processes/engulf.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     3480 2023-05-16 13:18:03.000000 vivarium-core-1.5.7/vivarium/processes/glucose_phosphorylation.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     3080 2023-05-16 13:18:03.000000 vivarium-core-1.5.7/vivarium/processes/growth_rate.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     3235 2023-05-16 13:18:03.000000 vivarium-core-1.5.7/vivarium/processes/injector.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     6894 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/vivarium/processes/mass_adaptor.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     6681 2023-05-16 13:18:03.000000 vivarium-core-1.5.7/vivarium/processes/meta_division.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     3421 2023-08-02 19:42:18.000000 vivarium-core-1.5.7/vivarium/processes/molarity_deriver.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     2432 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/vivarium/processes/nonspatial_environment.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     3244 2023-05-16 13:18:03.000000 vivarium-core-1.5.7/vivarium/processes/remove.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     1403 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/vivarium/processes/strip_units.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     5558 2023-05-16 13:18:03.000000 vivarium-core-1.5.7/vivarium/processes/swap_processes.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     3745 2023-05-16 13:18:03.000000 vivarium-core-1.5.7/vivarium/processes/template_process.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     3260 2022-09-07 22:46:45.000000 vivarium-core-1.5.7/vivarium/processes/timeline.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     7701 2023-08-02 19:42:50.000000 vivarium-core-1.5.7/vivarium/processes/toy_gillespie.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     4600 2023-05-16 13:18:03.000000 vivarium-core-1.5.7/vivarium/processes/tree_mass.py
+drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-08-02 19:42:56.294150 vivarium-core-1.5.7/vivarium_core.egg-info/
+-rw-r--r--   0 eranagmon   (502) staff       (20)     6266 2023-08-02 19:42:56.000000 vivarium-core-1.5.7/vivarium_core.egg-info/PKG-INFO
+-rw-r--r--   0 eranagmon   (502) staff       (20)     2408 2023-08-02 19:42:56.000000 vivarium-core-1.5.7/vivarium_core.egg-info/SOURCES.txt
+-rw-r--r--   0 eranagmon   (502) staff       (20)        1 2023-08-02 19:42:56.000000 vivarium-core-1.5.7/vivarium_core.egg-info/dependency_links.txt
+-rw-r--r--   0 eranagmon   (502) staff       (20)       20 2023-08-02 19:42:56.000000 vivarium-core-1.5.7/vivarium_core.egg-info/entry_points.txt
+-rw-r--r--   0 eranagmon   (502) staff       (20)      115 2023-08-02 19:42:56.000000 vivarium-core-1.5.7/vivarium_core.egg-info/requires.txt
+-rw-r--r--   0 eranagmon   (502) staff       (20)        9 2023-08-02 19:42:56.000000 vivarium-core-1.5.7/vivarium_core.egg-info/top_level.txt
```

### Comparing `vivarium-core-1.5.6/AUTHORS.md` & `vivarium-core-1.5.7/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/LICENSE.txt` & `vivarium-core-1.5.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/PKG-INFO` & `vivarium-core-1.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vivarium-core
-Version: 1.5.6
+Version: 1.5.7
 Summary: Engine for composing and simulating computational biology models with the Vivarium interface.
 Home-page: https://github.com/vivarium-collective/vivarium-core
 Author: Eran Agmon, Ryan Spangler
 Author-email: eagmon@stanford.edu, ryan.spangler@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/vivarium-collective/vivarium-core
 Project-URL: Documentation, https://vivarium-core.readthedocs.io/en/latest/
@@ -93,13 +93,13 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.8, <3.11
+Requires-Python: >=3.9, <3.12
 Description-Content-Type: text/markdown
```

### Comparing `vivarium-core-1.5.6/README.md` & `vivarium-core-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/setup.py` & `vivarium-core-1.5.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 from setuptools import setup
 
 
-VERSION = '1.5.6'
+VERSION = '1.5.7'
 
 
 if __name__ == '__main__':
     with open("README.md", 'r') as readme:
         description = readme.read()
         # Patch the relative links to absolute URLs that will work on PyPI.
         description2 = re.sub(
@@ -45,15 +45,15 @@
             'Engine for composing and simulating computational biology '
             'models with the Vivarium interface.'
         ),
         long_description=long_description,
         long_description_content_type='text/markdown',
         package_data={},
         include_package_data=True,
-        python_requires='>=3.8, <3.11',
+        python_requires='>=3.9, <3.12',
         install_requires=[
             'matplotlib>=3.5.1',
             'networkx>=2.6.3',
             'numpy>=1.22.1',
             'Pint>=0.18',
             'pymongo>=4.0.1',
             'scipy>=1.7.3',
@@ -65,14 +65,14 @@
             'Intended Audience :: Developers',
             'Intended Audience :: Education',
             'Intended Audience :: Science/Research',
             'License :: OSI Approved :: MIT License',
             'Operating System :: OS Independent',
             'Programming Language :: Python',
             'Programming Language :: Python :: 3',
-            'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3.9',
             'Programming Language :: Python :: 3.10',
+            'Programming Language :: Python :: 3.11',
             'Topic :: Scientific/Engineering',
         ],
         keywords='vivarium multi-scale computational-biology biology simulation framework',
     )
```

### Comparing `vivarium-core-1.5.6/vivarium/__init__.py` & `vivarium-core-1.5.7/vivarium/__init__.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/composites/injected_glc_phosphorylation.py` & `vivarium-core-1.5.7/vivarium/composites/injected_glc_phosphorylation.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/composites/toys.py` & `vivarium-core-1.5.7/vivarium/composites/toys.py`

 * *Files 1% similar despite different names*

```diff
@@ -747,21 +747,21 @@
         assert key in composite['processes']
         assert isinstance(composite['processes'][key], ToyProcess)
 
 
 def test_get_composite() -> None:
     process1 = ToyProcess({'name': 'process1'})
 
-    composite = Composite(dict(
-        processes={'process2': ToyProcess()},
-        topology={
+    composite = Composite({
+        'processes': {'process2': ToyProcess()},
+        'topology': {
             'process2': {
                 'port1': ('store_A',),
                 'port2': ('store_B',)}}
-    ))
+    })
     composite.merge(
         processes={process1.name: process1},
         topology={
             process1.name: {
                 'port1': ('store_A',),
                 'port2': ('store_B',)}})
```

### Comparing `vivarium-core-1.5.6/vivarium/core/composer.py` & `vivarium-core-1.5.7/vivarium/core/composer.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,16 @@
             elif state_type == 'default':
                 process_state = node.default_state()
             # Prevent multiupdates from forming when a single process has
             # multiple ports to the same stores holding a dictionary
             sub_state = inverse_topology(
                 path, process_state, sub_topology, multi_updates=False)
         else:
-            Exception(f'invalid processes {sub_processes} or steps {sub_steps}')
+            raise ValueError(f'invalid processes {sub_processes} or steps'
+                             + str(sub_steps))
         state = deep_merge(state, sub_state)
     return state
 
 
 def _get_composite_state(
         processes: Processes,
         steps: Steps,
@@ -328,14 +329,15 @@
 
         Returns:
             Subclass implementations should return a dictionary mapping
             step names to instantiated and configured
             :py:class:`vivarium.core.process.Step` objects.
         '''
         _ = config
+        _ = self # Silence pylint no-self-use
         return {}  # pragma: no cover
 
     def generate_flow(self, config: Optional[dict]) -> Flow:
         '''Generate the flow of :term:`step` dependencies.
 
         Args:
             config: A dictionary of configuration options. All
@@ -349,14 +351,15 @@
             included,** but they should be mapped to an empty sequence.
             Any steps returned by :py:meth:`generate_steps` or
             :py:meth:`generate_processes` that are not included in the
             flow will be treated as if they depend on every step
             previously added to the :term:`engine`.
         '''
         _ = config
+        _ = self # Silence pylint no-self-use
         return {}  # pragma: no cover
 
     @abc.abstractmethod
     def generate_topology(self, config: Optional[dict]) -> Topology:
         """Generate topology dictionary.
 
         Every subclass must override this method.
```

### Comparing `vivarium-core-1.5.6/vivarium/core/composition.py` & `vivarium-core-1.5.7/vivarium/core/composition.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,16 +109,16 @@
         overide_topology)
     topology.update({
         environment_process.name: environment_topology})
 
 
 def process_in_experiment(
         process: Process,
-        settings: Dict[str, Any] = None,
-        initial_state: Dict[str, Any] = None,
+        settings: Optional[Dict[str, Any]] = None,
+        initial_state: Optional[Dict[str, Any]] = None,
 ) -> Engine:
     """Put a Process in an Engine
 
     Args:
         process: the Process to put into the Engine
         settings: a dictionary of optional configuration options,
             keywords include timeline, environment, and topology that
@@ -147,16 +147,16 @@
         settings=settings,
         initial_state=initial_state
     )
 
 
 def composite_in_experiment(
         composite: Composite,
-        settings: Dict[str, Any] = None,
-        initial_state: Dict[str, Any] = None,
+        settings: Optional[Dict[str, Any]] = None,
+        initial_state: Optional[Dict[str, Any]] = None,
 ) -> Engine:
     """Put a Composite in an Engine
 
     Args:
         composite: the :term:`Composite` object.
         settings: a dictionary of options, including composite_config
             for configuring the composite. Additional  keywords include
@@ -191,17 +191,17 @@
         if key in experiment_config_keys:
             experiment_config[key] = setting
     return Engine(**experiment_config)  # type: ignore
 
 
 def composer_in_experiment(
         composer: Composer,
-        settings: Dict[str, Any] = None,
-        initial_state: Dict[str, Any] = None,
-        config: Dict[str, Any] = None,
+        settings: Optional[Dict[str, Any]] = None,
+        initial_state: Optional[Dict[str, Any]] = None,
+        config: Optional[Dict[str, Any]] = None,
         outer_path: HierarchyPath = (),
 ) -> Engine:
     """Generate a Composite in an Engine
 
     Args:
         composer: a :term:`Composer` object.
         settings: a dictionary of options, including composite_config
```

### Comparing `vivarium-core-1.5.6/vivarium/core/control.py` & `vivarium-core-1.5.7/vivarium/core/control.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 
         if isinstance(experiment_config, str):
             experiment = self.experiments_library[experiment_config]
             if isinstance(experiment, dict):
                 experiment = experiment.pop('experiment')
             return experiment()
 
-        raise Exception(f'invalid experiment config: {experiment_config}')
+        raise ValueError(f'invalid experiment config: {experiment_config}')
 
     def run_one_plot(
             self,
             plot_config: Union[str, dict],
             data: OutputDict,
             out_dir: Optional[str] = None,
     ) -> None:
@@ -134,15 +134,15 @@
 
         elif callable(plot_config):
             # call plot directly
             plot_config(
                 data=data_copy,
                 out_dir=out_dir)
         else:
-            raise Exception(f'invalid plot config: {plot_config}')
+            raise ValueError(f'invalid plot config: {plot_config}')
 
     def run_plots(
             self,
             plot_ids: Union[list, str],
             data: OutputDict,
             out_dir: Optional[str] = None,
     ) -> None:
```

### Comparing `vivarium-core-1.5.6/vivarium/core/emitter.py` & `vivarium-core-1.5.7/vivarium/core/emitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 SECRETS_PATH = 'secrets.json'
 
 
 def breakdown_data(
         limit: float,
         data: Any,
         path: Tuple = (),
-        size: float = None,
+        size: Optional[float] = None,
 ) -> list:
     size = size or len(str(data))
     if size > limit:
         if isinstance(data, dict):
             output = []
             subsizes = {}
             total = 0
@@ -114,15 +114,15 @@
 
     * ``database``: :py:class:`DatabaseEmitter`
     * ``null``: :py:class:`NullEmitter`
     * ``print``: :py:class:`Emitter`, prints to stdout
     * ``timeseries``: :py:class:`RAMEmitter`
 
     Arguments:
-        config: Must comtain the ``type`` key, which specifies the emitter
+        config: Must contain the ``type`` key, which specifies the emitter
             type name (e.g. ``database``).
 
     Returns:
         A new Emitter instance.
     """
 
     if config is None:
@@ -174,57 +174,59 @@
     def emit(self, data: Dict[str, Any]) -> None:
         """Emit data.
 
         Args:
             data: The data to emit. This gets called by the Vivarium
                 engine with a snapshot of the simulation state.
         """
+        _ = self # Silence pylint no-self-use
         print(data)
 
-    def get_data(self, query: list = None) -> dict:
+    def get_data(self, query: Optional[list] = None) -> dict:
         """Get the emitted data.
 
         Returns:
             The data that has been emitted to the database in the
             :term:`raw data` format. For this particular class, an empty
             dictionary is returned.
         """
         _ = query
+        _ = self # Silence pylint no-self-use
         return {}
 
-    def get_data_deserialized(self, query: list = None) -> Any:
+    def get_data_deserialized(self, query: Optional[list] = None) -> Any:
         """Get the emitted data with variable values deserialized.
 
         Returns:
             The data that has been emitted to the database in the
             :term:`raw data` format. Before being returned, serialized
             values in the data are deserialized.
         """
         return deserialize_value(self.get_data(query))
 
-    def get_data_unitless(self, query: list = None) -> Any:
+    def get_data_unitless(self, query: Optional[list] = None) -> Any:
         """Get the emitted data with units stripped from variable values.
 
         Returns:
             The data that has been emitted to the database in the
             :term:`raw data` format. Before being returned, units are
             stripped from values.
         """
         return remove_units(self.get_data_deserialized(query))
 
-    def get_path_timeseries(self, query: list = None) -> dict:
+    def get_path_timeseries(self, query: Optional[list] = None) -> dict:
         """Get the deserialized data as a :term:`path timeseries`.
 
         Returns:
             The deserialized emitted data, formatted as a
             :term:`path timeseries`.
         """
         return path_timeseries_from_data(self.get_data_deserialized(query))
 
-    def get_timeseries(self, query: list = None) -> dict:
+    def get_timeseries(self, query: Optional[list] = None) -> dict:
         """Get the deserialized data as an :term:`embedded timeseries`.
 
         Returns:
             The deserialized emitted data, formatted as an
             :term:`embedded timeseries`.
         """
         return timeseries_from_data(self.get_data_deserialized(query))
@@ -262,15 +264,15 @@
             data_at_time = assoc_path({}, self.embed_path, emit_data)
             self.saved_data.setdefault(time, {})
             data_at_time = serialize_value(
                 data_at_time, self.fallback_serializer)
             deep_merge_check(
                 self.saved_data[time], data_at_time, check_equality=True)
 
-    def get_data(self, query: list = None) -> dict:
+    def get_data(self, query: Optional[list] = None) -> dict:
         """ Return the accumulated timeseries history of "emitted" data. """
         if query:
             returned_data = {}
             for t, data in self.saved_data.items():
                 paths_data = []
                 for path in query:
                     datum = get_in(data, path)
@@ -385,15 +387,15 @@
                 d['assembly_id'] = assembly_id
                 d['experiment_id'] = experiment_id
                 if time:
                     d.setdefault('data', {})
                     d['data']['time'] = time
                 table.insert_one(d)
 
-    def get_data(self, query: list = None) -> dict:
+    def get_data(self, query: Optional[list] = None) -> dict:
         return get_history_data_db(self.history, self.experiment_id, query)
 
 
 def get_experiment_database(
         port: Any = 27017,
         database_name: str = 'simulations'
 ) -> Any:
@@ -415,15 +417,15 @@
     db = emitter.db
     return db
 
 
 def delete_experiment(
     host: str = 'localhost',
     port: Any = 27017,
-    query: dict = None
+    query: Optional[dict] = None
 ) -> None:
     """Helper function to delete experiment data in parallel
 
     Args:
         host: Host name of database. This can usually be left as the default.
         port: Port number of database. This can usually be left as the
             default.
@@ -486,15 +488,15 @@
             assembly[assembly_id] = datum['data']
     return assembly
 
 
 def apply_func(
     document: Any,
     field: Tuple,
-    f: Callable[..., Any] = None,
+    f: Optional[Callable[..., Any]] = None,
 ) -> Any:
     if field[0] not in document:
         return document
     if len(field) != 1:
         document[field[0]] = apply_func(document[field[0]], field[1:], f)
     elif f is not None:
         document[field[0]] = f(document[field[0]])
@@ -555,17 +557,17 @@
     id_ranges.append((id_cutoffs[-1], MaxKey()))
     return id_ranges
 
 
 def get_history_data_db(
     history_collection: Any,
     experiment_id: Any,
-    query: list = None,
-    func_dict: dict = None,
-    f: Callable[..., Any] = None,
+    query: Optional[list] = None,
+    func_dict: Optional[dict[tuple, Callable[..., Any]]] = None,
+    f: Optional[Callable[..., Any]] = None,
     filters: Optional[dict] = None,
     start_time: Union[int, MinKey] = MinKey(),
     end_time: Union[int, MaxKey] = MaxKey(),
     cpus: int = 1,
     host: str ='localhost',
     port: Any = '27017'
 ) -> Dict[float, dict]:
@@ -618,15 +620,15 @@
         cursor = itertools.chain.from_iterable(queried_chunks)
     else:
         cursor = history_collection.find(experiment_query, projection)
     raw_data = []
     for document in cursor:
         assert document.get('assembly_id'), \
             "all database documents require an assembly_id"
-        if (f or func_dict) and query:
+        if ((f is not None) or (func_dict is not None)) and query:
             for field in query:
                 if func_dict:  # func_dict takes priority over f
                     func = func_dict.get(field)
                 else:
                     func = f
 
                 document["data"] = apply_func(
@@ -655,30 +657,30 @@
 def get_atlas_client(secrets_path: str) -> Any:
     """Open a MongoDB client using the named secrets config JSON file."""
     with open(secrets_path, 'r') as f:
         secrets = json.load(f)
     emitter_config = get_atlas_database_emitter_config(
         **secrets['database'])
     uri = emitter_config['host']
-    client = MongoClient(uri)
+    client: MongoClient = MongoClient(uri)
     return client[emitter_config['database']]
 
 
 def get_local_client(host: str, port: Any, database_name: str) -> Any:
     """Open a MongoDB client onto the given host, port, and DB."""
-    client = MongoClient('{}:{}'.format(host, port))
+    client: MongoClient = MongoClient('{}:{}'.format(host, port))
     return client[database_name]
 
 
 def data_from_database(
     experiment_id: str,
     client: Any,
-    query: list = None,
-    func_dict: dict = None,
-    f: Callable[..., Any] = None,
+    query: Optional[list] = None,
+    func_dict: Optional[dict[tuple, Callable[..., Any]]] = None,
+    f: Optional[Callable[..., Any]] = None,
     filters: Optional[dict] = None,
     start_time: Union[int, MinKey] = MinKey(),
     end_time: Union[int, MaxKey] = MaxKey(),
     cpus: int = 1
 ) -> Tuple[dict, Any]:
     """Fetch something from a MongoDB.
```

### Comparing `vivarium-core-1.5.6/vivarium/core/engine.py` & `vivarium-core-1.5.7/vivarium/core/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,16 @@
         return self.f(
             self.defer.get_command_result(),
             self.args)
 
 
 class EmptyDefer(Defer):
     def __init__(self) -> None:
-        function = lambda update, arg: update
+        def function(update: dict, _: tuple) -> dict:
+            return update
         args = ()
         super().__init__(None, function, args)
 
     def get(self) -> Update:
         return {}
 
 
@@ -488,26 +489,26 @@
                 Engine._validate_steps_and_flow(
                     step_paths, sub_flow, path + (key,))
             else:
                 assert isinstance(sub_flow, list)
                 for dependency in sub_flow:
                     dependency = path + dependency
                     if dependency not in step_paths:
-                        raise Exception(
+                        raise ValueError(
                             f'Unknown dependency step {dependency} is '
                             'in the flow')
 
     def _make_store(
             self,
-            store: Store = None,
-            composite: Composite = None,
-            processes: Processes = None,
-            steps: Steps = None,
-            flow: Flow = None,
-            topology: Topology = None,
+            store: Optional[Store] = None,
+            composite: Optional[Composite] = None,
+            processes: Optional[Processes] = None,
+            steps: Optional[Steps] = None,
+            flow: Optional[Flow] = None,
+            topology: Optional[Topology] = None,
     ) -> None:
         """
         If a :term:`Store` is provided, retrieve the :term:`Processes`,
         :term:`Steps`, :term:`Flow`, and :term:`Topology`. If a
         :term:`Composite` or its attributes are provided, create a
         store. These are interchangeable.
         """
@@ -520,15 +521,15 @@
             elif composite:
                 self.processes = composite['processes']
                 self.steps = composite['steps']
                 self.flow = composite['flow']
                 self.topology = composite['topology']
                 self.initial_state = composite['state'] or self.initial_state
             else:
-                raise Exception(
+                raise ValueError(
                     'load either composite, store, or '
                     '(processes and topology) into Engine')
 
             self.processes = cast(
                 Dict[str, Any],
                 self._parallelize_processes(self.processes)
             )
@@ -662,79 +663,14 @@
         data.update({
             'time': self.global_time})
         emit_config = {
             'table': 'history',
             'data': data}
         self.emitter.emit(emit_config)
 
-    def _invoke_process(
-            self,
-            process: Process,
-            interval: float,
-            states: State,
-    ) -> Any:
-        """Trigger computation of a process's update.
-
-        To allow processes to run in parallel, this function only
-        triggers update computation. When the function exits,
-        computation may not be complete.
-
-        Args:
-            process: The process.
-            interval: The timestep for which to compute the update.
-            states: The simulation state to pass to
-                :py:meth:`vivarium.core.process.Process.next_update`.
-
-        Returns:
-            The deferred simulation update, for example a
-            :py:class:`vivarium.core.process.ParallelProcess`.
-        """
-        process.send_command('next_update', (interval, states))
-        return process
-
-    def _process_update(
-            self,
-            path: HierarchyPath,
-            process: Process,
-            store: Store,
-            states: State,
-            interval: float,
-    ) -> Tuple[Defer, Store]:
-        """Start generating a process's update.
-
-        This function is similar to :py:meth:`_invoke_process` except in
-        addition to triggering the computation of the process's update
-        (by calling ``_invoke_process``), it also generates a
-        :py:class:`Defer` object to transform the update into absolute
-        terms.
-
-        Args:
-            path: Path to process.
-            process: The process.
-            store: The store at ``path``.
-            states: Simulation state to pass to process's
-                ``next_update`` method.
-            interval: Timestep for which to compute the update.
-
-        Returns:
-            Tuple of the deferred update (in absolute terms) and
-            ``store``.
-        """
-        process = self._invoke_process(
-            process,
-            interval,
-            states)
-
-        absolute = Defer(
-            process,
-            invert_topology,
-            (path, store.topology))
-
-        return absolute, store
-
     def _process_state(
             self,
             path: HierarchyPath,
     ) -> Tuple[Store, State]:
         """Get the simulation state for a process's ``next_update``.
 
         Before computing an update, we have to collect the simulation
@@ -774,15 +710,15 @@
 
         Returns:
             Tuple of the deferred update (relative to the root of
             ``path``) and the store at ``path``.
         """
         store, states = self._process_state(path)
         if process.update_condition(interval, states):
-            return self._process_update(
+            return _process_update(
                 path, process, store, states, interval)
         return (EmptyDefer(), store)
 
     def apply_update(
             self,
             update: Update,
             state: Store
@@ -938,15 +874,15 @@
         self.run_for(
             interval=interval,
             force_complete=True,
         )
         self._check_complete()
         runtime = clock.time() - clock_start
         if self.display_info:
-            self._print_summary(runtime)
+            _print_summary(runtime)
 
     def _check_complete(self) -> None:
         """Check that all processes completed"""
         for path, advance in self.front.items():
             assert advance['time'] == self.global_time, \
                 f"the process at path {path} is at time {advance['time']} " \
                 f"instead of completing at global time {self.global_time}"
@@ -1015,15 +951,15 @@
                         # set future time based on global_time_precision
                         future = round(future, self.global_time_precision)
 
                     if future <= end_time:
 
                         # calculate the update for this process
                         if process.update_condition(process_timestep, states):
-                            update = self._process_update(
+                            update = _process_update(
                                 path, process, store, states, process_timestep)
 
                             # update front, to be applied at its projected time
                             self.front[path]['time'] = future
                             self.front[path]['update'] = update
 
                             # absolute timestep
@@ -1106,14 +1042,16 @@
         This MUST be called at the end of any simulation with parallel
         processes. This function also ends profiling and computes
         profiling stats, including stats from parallel sub-processes.
         These stats are stored in ``self.stats``.
         """
         apply_func_to_leaves(
             self.processes, self._end_process_if_parallel)
+        apply_func_to_leaves(
+            self.steps, self._end_process_if_parallel)
         if self.profiler:
             self.profiler.disable()
             total_stats = pstats.Stats(self.profiler)
             for stats in self.stats_objs:
                 total_stats.add(stats)
             self.stats = total_stats
 
@@ -1125,24 +1063,14 @@
             date[4:6] + '/' + date[6:8] + '/' + date[0:4],
             time[0:2] + ':' + time[2:4] + ':' + time[4:6]))
         if self.experiment_name is not self.experiment_id:
             print('Name: {}'.format(self.experiment_name))
         if self.description:
             print('Description: {}'.format(self.description))
 
-    def _print_summary(
-            self,
-            runtime: float
-    ) -> None:
-        """Print summary of simulation runtime."""
-        if runtime < 1:
-            print('Completed in {:.6f} seconds'.format(runtime))
-        else:
-            print('Completed in {:.2f} seconds'.format(runtime))
-
 
 def print_progress_bar(
         iteration: float,
         total: float,
         decimals: float = 1,
         length: int = 50,
 ) -> None:
@@ -1160,14 +1088,85 @@
     print(
         f'\rProgress:|{filled_bar}| {progress}/{float(total)} '
         f'simulated seconds remaining    ', end='\r')
     # Print New Line on Complete
     if iteration == total:
         print()
 
+def _print_summary(
+        runtime: float
+) -> None:
+    """Print summary of simulation runtime."""
+    if runtime < 1:
+        print('Completed in {:.6f} seconds'.format(runtime))
+    else:
+        print('Completed in {:.2f} seconds'.format(runtime))
+
+def _invoke_process(
+        process: Process,
+        interval: float,
+        states: State,
+) -> Any:
+    """Trigger computation of a process's update.
+
+    To allow processes to run in parallel, this function only
+    triggers update computation. When the function exits,
+    computation may not be complete.
+
+    Args:
+        process: The process.
+        interval: The timestep for which to compute the update.
+        states: The simulation state to pass to
+            :py:meth:`vivarium.core.process.Process.next_update`.
+
+    Returns:
+        The deferred simulation update, for example a
+        :py:class:`vivarium.core.process.ParallelProcess`.
+    """
+    process.send_command('next_update', (interval, states))
+    return process
+
+def _process_update(
+        path: HierarchyPath,
+        process: Process,
+        store: Store,
+        states: State,
+        interval: float,
+) -> Tuple[Defer, Store]:
+    """Start generating a process's update.
+
+    This function is similar to :py:func:`_invoke_process` except in
+    addition to triggering the computation of the process's update
+    (by calling ``_invoke_process``), it also generates a
+    :py:class:`Defer` object to transform the update into absolute
+    terms.
+
+    Args:
+        path: Path to process.
+        process: The process.
+        store: The store at ``path``.
+        states: Simulation state to pass to process's
+            ``next_update`` method.
+        interval: Timestep for which to compute the update.
+
+    Returns:
+        Tuple of the deferred update (in absolute terms) and
+        ``store``.
+    """
+    process = _invoke_process(
+        process,
+        interval,
+        states)
+
+    absolute = Defer(
+        process,
+        invert_topology,
+        (path, store.topology))
+
+    return absolute, store
 
 def test_flow_with_extra_step() -> None:
     class StepA(Step):
 
         def ports_schema(self) -> Schema:
             return {
                 'a': {'_default': 1}
```

### Comparing `vivarium-core-1.5.6/vivarium/core/process.py` & `vivarium-core-1.5.7/vivarium/core/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -347,14 +347,15 @@
                 some may ignore it.
 
         Returns:
             dict: Subclass implementations must return a dictionary
             mapping state paths to initial values.
         """
         _ = config
+        _ = self # Silence pylint no-self-use
         return {}
 
     def generate_processes(
             self, config: Optional[dict] = None) -> Dict[str, Any]:
         """Do not override this method."""
         if not self.is_step():
             config = config or {}
@@ -380,14 +381,15 @@
         return {
             name: {
                 port: override_topology.get(port, (port,))
                 for port in ports.keys()}}
 
     def generate_flow(self, config: Optional[dict] = None) -> Flow:
         _ = config
+        _ = self # Silence pylint no-self-use
         return {}
 
     def generate(
             self,
             config: Optional[dict] = None,
             path: HierarchyPath = ()) -> Dict:
         if config is None:
@@ -488,14 +490,15 @@
            please override ``is_step`` instead of ``is_deriver``.
            Support for Derivers may be removed in a future release.
 
         Returns:
             Whether this process is a deriver. This class always returns
             ``False``, but subclasses may change this.
         """
+        _ = self # Silence pylint no-self-use
         return False
 
     def is_step(self) -> bool:
         """Check whether this process is a :term:`step`.
 
         Returns:
             Whether this process is a step. This class always returns
@@ -520,14 +523,15 @@
         other processes. You can override this function to let
         :term:`experiments` emit the process's private state.
 
         Returns:
             An empty dictionary. You may override this behavior to
             return your process's private state.
         """
+        _ = self # Silence pylint no-self-use
         return {}  # pragma: no cover
 
     @abc.abstractmethod
     def ports_schema(self) -> Schema:
         """Get the schemas for each port.
 
         This must be overridden by any subclasses.
@@ -773,19 +777,19 @@
         return self.run_command('parameters')
 
     @property
     def condition_path(self) -> Optional[HierarchyPath]:
         return self.run_command('condition_path')
 
     @property
-    def schema(self) -> Schema:
+    def schema(self) -> Optional[Schema]:
         return self.run_command('schema')
 
     @schema.setter
-    def schema(self, value: Schema) -> None:
+    def schema(self, value: Optional[Schema]) -> None:
         self.run_command('set_schema', (value,))
 
     def merge_overrides(self, override: Schema) -> None:
         self.run_command('merge_overrides', (override,))
 
     def calculate_timestep(self, states: Optional[State]) -> float:
         return self.run_command('calculate_timestep', (states,))
@@ -864,14 +868,15 @@
     def next_update(self, timestep: float, states: State) -> Update:
         return {}
 
 
 class ToyParallelProcess(Process):
 
     def compare_pid(self, pid: float) -> bool:
+        _ = self # Silence pylint no-self-use
         return os.getpid() == pid
 
     def send_command(
             self, command: str, args: Optional[tuple] = None,
             kwargs: Optional[dict] = None,
             run_pre_check: bool = True) -> None:
         if run_pre_check:
```

### Comparing `vivarium-core-1.5.6/vivarium/core/registry.py` & `vivarium-core-1.5.7/vivarium/core/registry.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/core/serialize.py` & `vivarium-core-1.5.7/vivarium/core/serialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Collection of serializers that transform Python data into
 a BSON-compatible form.
 """
 
 import re
 import math
 import warnings
-from typing import Any, List, Union
+from typing import Any, List, Optional, Union
 from collections.abc import Callable
 
 import orjson
 import numpy as np
 # from pint import Unit
 # try:
 #     from pint.quantity import Quantity
@@ -24,15 +24,15 @@
 from vivarium.library.units import units
 from vivarium.core.registry import serializer_registry, Serializer
 
 
 def find_numpy_and_non_strings(
     d: dict,
     curr_path: tuple=tuple(),
-    saved_paths: List[tuple]=None
+    saved_paths: Optional[List[tuple]]=None
 ) -> List[tuple]:
     """Return list of paths which terminate in a non-string or Numpy string
     dictionary key. Orjson does not handle these types of keys by default."""
     if not saved_paths:
         saved_paths = []
     if isinstance(d, dict):
         for key in d.keys():
@@ -43,30 +43,30 @@
             saved_paths = find_numpy_and_non_strings(
                 d[key], curr_path+(key,), saved_paths)
     return saved_paths
 
 
 def serialize_value(
     value: Any,
-    default: Callable=None,
+    default: Optional[Callable]=None,
 ) -> Any:
     """Apply orjson-based serialization routine on ``value``.
 
     Args:
         value (Any): Data to be serialized. All keys must be strings. Notably,
             Numpy strings (``np.str_``) are not acceptable keys.
         default (Callable): A function that is called on any data of a type
             that is not natively supported by orjson. Returns an object that
             can be handled by default up to 254 times before an exception is
             raised.
 
     Returns:
         Any: Serialized data
     """
-    if not default:
+    if default is None:
         default = make_fallback_serializer_function()
     try:
         value = orjson.dumps(value, option=orjson.OPT_SERIALIZE_NUMPY,
             default=default)
         return orjson.loads(value)
     except TypeError as e:
         bad_keys = find_numpy_and_non_strings(value)
```

### Comparing `vivarium-core-1.5.6/vivarium/core/serialize_test.py` & `vivarium-core-1.5.7/vivarium/core/serialize_test.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/core/store.py` & `vivarium-core-1.5.7/vivarium/core/store.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/core/types.py` & `vivarium-core-1.5.7/vivarium/core/types.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/experiments/bigraph_view.py` & `vivarium-core-1.5.7/vivarium/experiments/bigraph_view.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/experiments/composite_merge.py` & `vivarium-core-1.5.7/vivarium/experiments/composite_merge.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/experiments/engine_tests.py` & `vivarium-core-1.5.7/vivarium/experiments/engine_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -874,15 +874,15 @@
         agent_ids = set(state['agents'].keys())
         env_agents = set(state['log_update'].get('agents', {}).keys())
         if env_agents != agent_ids:
             if not once_different:
                 once_different = True
             else:
                 # the values have been different for more than one update
-                ValueError(
+                raise ValueError(
                     f'environment sees {env_agents} instead of {agent_ids}')
         else:
             once_different = False
 
 
 class AddDelete(Process):
     def ports_schema(self) -> Schema:
```

### Comparing `vivarium-core-1.5.6/vivarium/experiments/glucose_phosphorylation.py` & `vivarium-core-1.5.7/vivarium/experiments/glucose_phosphorylation.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/experiments/hierarchy_composite_division.py` & `vivarium-core-1.5.7/vivarium/experiments/hierarchy_composite_division.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,18 @@
             'threshold': 2.5 * units.fL},
         'agents_path': ('..', '..', 'agents',),
         'boundary_path': ('boundary',),
         'daughter_path': tuple(),
     }
 
     def generate_processes(self, config) -> dict:
-        division_config = dict(
-            daughter_path=config['daughter_path'],
-            agent_id=config['agent_id'],
-            composer=self)
+        division_config = {
+            'daughter_path': config['daughter_path'],
+            'agent_id': config['agent_id'],
+            'composer': self}
         time_step_config = {'time_step': config['time_step']}
         return {
             'growth': GrowthRate({**config['growth'], **time_step_config}),
             'divide_condition': DivideCondition(config['divide_condition']),
             'division': MetaDivision(division_config)}
 
     def generate_topology(self, config) -> dict:
```

### Comparing `vivarium-core-1.5.6/vivarium/experiments/large_experiment.py` & `vivarium-core-1.5.7/vivarium/experiments/large_experiment.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/experiments/profile_image.py` & `vivarium-core-1.5.7/vivarium/experiments/profile_image.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/experiments/profile_runtime.py` & `vivarium-core-1.5.7/vivarium/experiments/profile_runtime.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/experiments/store_api.py` & `vivarium-core-1.5.7/vivarium/experiments/store_api.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/experiments/test_profiler.py` & `vivarium-core-1.5.7/vivarium/experiments/test_profiler.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/library/datum.py` & `vivarium-core-1.5.7/vivarium/library/datum.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/library/dict_utils.py` & `vivarium-core-1.5.7/vivarium/library/dict_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,15 +258,15 @@
 def keys_list(d: dict) -> list:
     """Return list(d.keys())."""
     return list(d.keys())
 
 
 def value_in_embedded_dict(
         data: dict,
-        timeseries: dict = None,
+        timeseries: Optional[dict] = None,
         time_index: Optional[float] = None) -> dict:
     """
     converts data from a single time step into an embedded dictionary with lists
     of values.
     If the value has a unit, saves under a key with (key, unit_string).
     """
     # TODO(jerry): ^^^ Explain this further. Note that this function modifies
```

### Comparing `vivarium-core-1.5.6/vivarium/library/filepath.py` & `vivarium-core-1.5.7/vivarium/library/filepath.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/library/make_network.py` & `vivarium-core-1.5.7/vivarium/library/make_network.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/library/pretty.py` & `vivarium-core-1.5.7/vivarium/library/pretty.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/library/schema.py` & `vivarium-core-1.5.7/vivarium/library/schema.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/library/timeseries.py` & `vivarium-core-1.5.7/vivarium/library/timeseries.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/library/topology.py` & `vivarium-core-1.5.7/vivarium/library/topology.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/library/units.py` & `vivarium-core-1.5.7/vivarium/library/units.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/library/wrappers.py` & `vivarium-core-1.5.7/vivarium/library/wrappers.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/plots/agents_multigen.py` & `vivarium-core-1.5.7/vivarium/plots/agents_multigen.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/plots/simulation_output.py` & `vivarium-core-1.5.7/vivarium/plots/simulation_output.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/plots/topology.py` & `vivarium-core-1.5.7/vivarium/plots/topology.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/processes/alternator.py` & `vivarium-core-1.5.7/vivarium/processes/alternator.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/processes/burst.py` & `vivarium-core-1.5.7/vivarium/processes/burst.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/processes/clock.py` & `vivarium-core-1.5.7/vivarium/processes/clock.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/processes/divide_condition.py` & `vivarium-core-1.5.7/vivarium/processes/divide_condition.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/processes/division.py` & `vivarium-core-1.5.7/vivarium/processes/division.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/processes/ecoli_shape_deriver.py` & `vivarium-core-1.5.7/vivarium/processes/ecoli_shape_deriver.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/processes/engulf.py` & `vivarium-core-1.5.7/vivarium/processes/engulf.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/processes/glucose_phosphorylation.py` & `vivarium-core-1.5.7/vivarium/processes/glucose_phosphorylation.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/processes/growth_rate.py` & `vivarium-core-1.5.7/vivarium/processes/growth_rate.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/processes/injector.py` & `vivarium-core-1.5.7/vivarium/processes/injector.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/processes/mass_adaptor.py` & `vivarium-core-1.5.7/vivarium/processes/mass_adaptor.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/processes/meta_division.py` & `vivarium-core-1.5.7/vivarium/processes/meta_division.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/processes/molarity_deriver.py` & `vivarium-core-1.5.7/vivarium/processes/molarity_deriver.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         'keys': [],
     }
 
     def initial_state(self, config=None):
         mass = 1000 * units.fg
         density = 1100 * units.g / units.L
         volume = mass / density
-        mmol_to_counts = (AVOGADRO * volume)
+        mmol_to_counts = AVOGADRO * volume
         return {
             'global': {
                 'volume': volume.to('fL'),
                 'mmol_to_counts': mmol_to_counts.to('L/mmol')
             }}
 
     def ports_schema(self):
```

### Comparing `vivarium-core-1.5.6/vivarium/processes/nonspatial_environment.py` & `vivarium-core-1.5.7/vivarium/processes/nonspatial_environment.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/processes/remove.py` & `vivarium-core-1.5.7/vivarium/processes/remove.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/processes/strip_units.py` & `vivarium-core-1.5.7/vivarium/processes/strip_units.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/processes/swap_processes.py` & `vivarium-core-1.5.7/vivarium/processes/swap_processes.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/processes/template_process.py` & `vivarium-core-1.5.7/vivarium/processes/template_process.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/processes/timeline.py` & `vivarium-core-1.5.7/vivarium/processes/timeline.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/processes/toy_gillespie.py` & `vivarium-core-1.5.7/vivarium/processes/toy_gillespie.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium/processes/tree_mass.py` & `vivarium-core-1.5.7/vivarium/processes/tree_mass.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.6/vivarium_core.egg-info/PKG-INFO` & `vivarium-core-1.5.7/vivarium_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vivarium-core
-Version: 1.5.6
+Version: 1.5.7
 Summary: Engine for composing and simulating computational biology models with the Vivarium interface.
 Home-page: https://github.com/vivarium-collective/vivarium-core
 Author: Eran Agmon, Ryan Spangler
 Author-email: eagmon@stanford.edu, ryan.spangler@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/vivarium-collective/vivarium-core
 Project-URL: Documentation, https://vivarium-core.readthedocs.io/en/latest/
@@ -93,13 +93,13 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.8, <3.11
+Requires-Python: >=3.9, <3.12
 Description-Content-Type: text/markdown
```

### Comparing `vivarium-core-1.5.6/vivarium_core.egg-info/SOURCES.txt` & `vivarium-core-1.5.7/vivarium_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*


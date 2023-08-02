# Comparing `tmp/daggerpy-0.0.5.tar.gz` & `tmp/daggerpy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daggerpy-0.0.5.tar", last modified: Mon Jul 31 10:22:18 2023, max compression
+gzip compressed data, was "daggerpy-0.0.6.tar", last modified: Wed Aug  2 09:42:58 2023, max compression
```

## Comparing `daggerpy-0.0.5.tar` & `daggerpy-0.0.6.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-31 10:22:18.183649 daggerpy-0.0.5/
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      171 2023-07-20 08:04:31.000000 daggerpy-0.0.5/AUTHORS.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      731 2023-07-20 08:15:21.000000 daggerpy-0.0.5/CONTRIBUTING.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      318 2023-07-26 19:47:04.000000 daggerpy-0.0.5/HISTORY.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1589 2023-07-20 08:53:44.000000 daggerpy-0.0.5/LICENSE
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      290 2023-07-20 09:04:51.000000 daggerpy-0.0.5/MANIFEST.in
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2641 2023-07-31 10:22:18.183649 daggerpy-0.0.5/PKG-INFO
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1383 2023-07-20 08:53:44.000000 daggerpy-0.0.5/README.rst
-drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-31 10:22:18.179649 daggerpy-0.0.5/daggerpy.egg-info/
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2641 2023-07-31 10:22:18.000000 daggerpy-0.0.5/daggerpy.egg-info/PKG-INFO
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1502 2023-07-31 10:22:18.000000 daggerpy-0.0.5/daggerpy.egg-info/SOURCES.txt
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        1 2023-07-31 10:22:18.000000 daggerpy-0.0.5/daggerpy.egg-info/dependency_links.txt
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       43 2023-07-31 10:22:18.000000 daggerpy-0.0.5/daggerpy.egg-info/entry_points.txt
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        1 2023-07-20 09:12:14.000000 daggerpy-0.0.5/daggerpy.egg-info/not-zip-safe
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       20 2023-07-31 10:22:18.000000 daggerpy-0.0.5/daggerpy.egg-info/requires.txt
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        7 2023-07-31 10:22:18.000000 daggerpy-0.0.5/daggerpy.egg-info/top_level.txt
-drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-31 10:22:18.179649 daggerpy-0.0.5/docs/
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      607 2023-07-20 08:04:31.000000 daggerpy-0.0.5/docs/Makefile
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       28 2023-07-20 08:04:31.000000 daggerpy-0.0.5/docs/authors.rst
--rwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)     4771 2023-07-20 08:53:44.000000 daggerpy-0.0.5/docs/conf.py
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       33 2023-07-20 08:04:31.000000 daggerpy-0.0.5/docs/contributing.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       28 2023-07-20 08:04:31.000000 daggerpy-0.0.5/docs/history.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      303 2023-07-20 08:04:31.000000 daggerpy-0.0.5/docs/index.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1114 2023-07-20 08:04:31.000000 daggerpy-0.0.5/docs/installation.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      804 2023-07-20 08:04:31.000000 daggerpy-0.0.5/docs/make.bat
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       27 2023-07-20 08:04:31.000000 daggerpy-0.0.5/docs/readme.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       67 2023-07-20 08:04:31.000000 daggerpy-0.0.5/docs/usage.rst
-drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-31 10:22:18.183649 daggerpy-0.0.5/includes/
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    44464 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/D4connector.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)   121966 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/D8connector.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    24570 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/PerlinNoise.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    93396 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/_D8connector.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    26031 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/_cordonnier_versatile_2019.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    55463 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/_graph.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    96777 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/_old_D8connector.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     7069 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/_priority_flood.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     5399 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/boost_spread_sort.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     6875 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/boundary_conditions.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     3199 2023-07-31 10:19:21.000000 daggerpy-0.0.5/includes/connector_checker.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    26439 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/cordonnier_versatile_2019.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    14121 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/depression_hierarchy.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)   126078 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/fastflood.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     6277 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/fastflood_recorder.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    64124 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/graph.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    96313 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/graphflood.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     7040 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/hillshading.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    18391 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/npy.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    18092 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/popscape.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2692 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/popscape_utils.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    15619 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/priority_flood.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     3764 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/river_tools_python.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    27928 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/simple_depression_solver.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    94626 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/trackscape.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      369 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/trackscape_enum.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2363 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/trackscape_utils.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    14552 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/utils.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1061 2023-07-31 10:19:21.000000 daggerpy-0.0.5/includes/veclike_holder.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    41822 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/veque.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      968 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/wrap_helper.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     4191 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/wrap_helper_MATLAB.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      390 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/wrap_helper_cpp.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2649 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/wrap_helper_julia.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2734 2023-07-31 10:18:38.000000 daggerpy-0.0.5/includes/wrap_helper_python.hpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    82665 2023-07-31 10:19:21.000000 daggerpy-0.0.5/main.cpp
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      374 2023-07-31 10:22:18.183649 daggerpy-0.0.5/setup.cfg
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     3708 2023-07-31 10:20:14.000000 daggerpy-0.0.5/setup.py
-drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-31 10:22:18.183649 daggerpy-0.0.5/tests/
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       36 2023-07-20 08:04:31.000000 daggerpy-0.0.5/tests/__init__.py
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      845 2023-07-20 10:48:58.000000 daggerpy-0.0.5/tests/test_dagger.py
+drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-08-02 09:42:58.638401 daggerpy-0.0.6/
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      171 2023-07-20 08:04:31.000000 daggerpy-0.0.6/AUTHORS.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      731 2023-07-20 08:15:21.000000 daggerpy-0.0.6/CONTRIBUTING.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      416 2023-08-02 09:42:50.000000 daggerpy-0.0.6/HISTORY.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1589 2023-07-20 08:53:44.000000 daggerpy-0.0.6/LICENSE
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      290 2023-07-20 09:04:51.000000 daggerpy-0.0.6/MANIFEST.in
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2739 2023-08-02 09:42:58.638401 daggerpy-0.0.6/PKG-INFO
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1383 2023-07-20 08:53:44.000000 daggerpy-0.0.6/README.rst
+drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-08-02 09:42:58.634401 daggerpy-0.0.6/daggerpy.egg-info/
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2739 2023-08-02 09:42:58.000000 daggerpy-0.0.6/daggerpy.egg-info/PKG-INFO
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1502 2023-08-02 09:42:58.000000 daggerpy-0.0.6/daggerpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        1 2023-08-02 09:42:58.000000 daggerpy-0.0.6/daggerpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       43 2023-08-02 09:42:58.000000 daggerpy-0.0.6/daggerpy.egg-info/entry_points.txt
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        1 2023-07-20 09:12:14.000000 daggerpy-0.0.6/daggerpy.egg-info/not-zip-safe
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       20 2023-08-02 09:42:58.000000 daggerpy-0.0.6/daggerpy.egg-info/requires.txt
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        7 2023-08-02 09:42:58.000000 daggerpy-0.0.6/daggerpy.egg-info/top_level.txt
+drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-08-02 09:42:58.638401 daggerpy-0.0.6/docs/
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      607 2023-07-20 08:04:31.000000 daggerpy-0.0.6/docs/Makefile
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       28 2023-07-20 08:04:31.000000 daggerpy-0.0.6/docs/authors.rst
+-rwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)     4771 2023-07-20 08:53:44.000000 daggerpy-0.0.6/docs/conf.py
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       33 2023-07-20 08:04:31.000000 daggerpy-0.0.6/docs/contributing.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       28 2023-07-20 08:04:31.000000 daggerpy-0.0.6/docs/history.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      303 2023-07-20 08:04:31.000000 daggerpy-0.0.6/docs/index.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1114 2023-07-20 08:04:31.000000 daggerpy-0.0.6/docs/installation.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      804 2023-07-20 08:04:31.000000 daggerpy-0.0.6/docs/make.bat
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       27 2023-07-20 08:04:31.000000 daggerpy-0.0.6/docs/readme.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       67 2023-07-20 08:04:31.000000 daggerpy-0.0.6/docs/usage.rst
+drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-08-02 09:42:58.638401 daggerpy-0.0.6/includes/
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    44464 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/D4connector.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)   115031 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/D8connector.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    24570 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/PerlinNoise.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    93396 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/_D8connector.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    26031 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/_cordonnier_versatile_2019.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    55463 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/_graph.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    96777 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/_old_D8connector.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     7069 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/_priority_flood.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     5399 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/boost_spread_sort.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     6875 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/boundary_conditions.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     3156 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/connector_checker.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    26439 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/cordonnier_versatile_2019.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    14121 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/depression_hierarchy.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)   126078 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/fastflood.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     6277 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/fastflood_recorder.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    64124 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/graph.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    96313 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/graphflood.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     7040 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/hillshading.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    18391 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/npy.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    18092 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/popscape.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2692 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/popscape_utils.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    15619 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/priority_flood.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     5231 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/river_tools_python.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    27928 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/simple_depression_solver.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    94626 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/trackscape.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      369 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/trackscape_enum.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2363 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/trackscape_utils.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    14552 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/utils.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1110 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/veclike_holder.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    41822 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/veque.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      968 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/wrap_helper.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     4191 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/wrap_helper_MATLAB.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      390 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/wrap_helper_cpp.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2649 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/wrap_helper_julia.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2734 2023-08-02 09:38:35.000000 daggerpy-0.0.6/includes/wrap_helper_python.hpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    75589 2023-08-02 09:38:35.000000 daggerpy-0.0.6/main.cpp
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      374 2023-08-02 09:42:58.638401 daggerpy-0.0.6/setup.cfg
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     3708 2023-08-02 09:40:13.000000 daggerpy-0.0.6/setup.py
+drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-08-02 09:42:58.638401 daggerpy-0.0.6/tests/
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       36 2023-07-20 08:04:31.000000 daggerpy-0.0.6/tests/__init__.py
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      845 2023-07-20 10:48:58.000000 daggerpy-0.0.6/tests/test_dagger.py
```

### Comparing `daggerpy-0.0.5/CONTRIBUTING.rst` & `daggerpy-0.0.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/LICENSE` & `daggerpy-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/PKG-INFO` & `daggerpy-0.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daggerpy
-Version: 0.0.5
+Version: 0.0.6
 Summary: DAG tools to process numerical topography and landscape evolution models
 Home-page: https://github.com/bgailleton/DAGGER
 Author: Boris Gailleton
 Author-email: boris.gailleton@univ-rennes.fr
 License: GNU General Public License v3
 Keywords: dagger
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -72,14 +72,19 @@
 Some I/O operations are using `libnpy <https://github.com/llohse/libnpy>`_ (MIT), a header-only c++ library to write/load simple `numpy` arrays.
 
 
 =======
 History
 =======
 
+0.0.6 (01/08/2023)
+------------------
+
+* Adding quick river and drainage divide extraction tools
+
 0.0.4 (20/07/2023)
 ------------------
 
 * Hot fix (still developping the CI/CD toolchain)
 
 0.0.3 (20/07/2023)
 ------------------
```

### Comparing `daggerpy-0.0.5/README.rst` & `daggerpy-0.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/daggerpy.egg-info/PKG-INFO` & `daggerpy-0.0.6/daggerpy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daggerpy
-Version: 0.0.5
+Version: 0.0.6
 Summary: DAG tools to process numerical topography and landscape evolution models
 Home-page: https://github.com/bgailleton/DAGGER
 Author: Boris Gailleton
 Author-email: boris.gailleton@univ-rennes.fr
 License: GNU General Public License v3
 Keywords: dagger
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -72,14 +72,19 @@
 Some I/O operations are using `libnpy <https://github.com/llohse/libnpy>`_ (MIT), a header-only c++ library to write/load simple `numpy` arrays.
 
 
 =======
 History
 =======
 
+0.0.6 (01/08/2023)
+------------------
+
+* Adding quick river and drainage divide extraction tools
+
 0.0.4 (20/07/2023)
 ------------------
 
 * Hot fix (still developping the CI/CD toolchain)
 
 0.0.3 (20/07/2023)
 ------------------
```

### Comparing `daggerpy-0.0.5/daggerpy.egg-info/SOURCES.txt` & `daggerpy-0.0.6/daggerpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/docs/Makefile` & `daggerpy-0.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/docs/conf.py` & `daggerpy-0.0.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/docs/installation.rst` & `daggerpy-0.0.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/docs/make.bat` & `daggerpy-0.0.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/includes/D4connector.hpp` & `daggerpy-0.0.6/includes/D4connector.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/includes/D8connector.hpp` & `daggerpy-0.0.6/includes/_old_D8connector.hpp`

 * *Files 19% similar despite different names*

```diff
@@ -33,31 +33,21 @@
 namespace DAGGER {
 
 // Useful namespace for my priority queue
 using PQ_i_d = std::priority_queue<PQ_helper<int, double>,
                                    std::vector<PQ_helper<int, double>>,
                                    std::greater<PQ_helper<int, double>>>;
 
-int fast_mod(const int input, const int ceil) {
-  // apply the modulo operator only when needed
-  // (i.e. when the input is greater than the ceiling)
-  return input < ceil ? input : input % ceil;
-  // NB: the assumption here is that the numbers are positive
-}
-
-template <class T, class uI_t = std::uint8_t> class D8connector {
+template <class T> class D8connector {
 public:
   // General informations about the graph
   // #-> number of nodes (integer and unsized int for loops or list innit).
   int nnodes = 0;
-  int nlinks() { return this->nnodes * 4; };
   size_t nnodes_t = 0;
 
-  int nxy() const { return this->nnodes; }
-
   static const int nneighbours = 8;
   static const size_t nneighbours_t = 8;
 
   // #-> number of nodes in x direction.
   int nx = 0;
   // #-> number of nodes in x direction.
   int ny = 0;
@@ -99,57 +89,46 @@
   // // #--->	3 = in, can out but can also give to neighbours
   // std::vector<int> boundary;
 
   // NEW BOUNDARY SYSTEM
   CodeBC boundaries;
 
   // Helpers for neighbouring operations
-  // -> oldneighbourer holdsthe indices to loop through for each boundary
-  // condition
-  std::vector<std::vector<int>> oldneighbourer;
-
-  std::array<int, 81> neighbourer;
-  std::array<int, 81> reruobhgien;
-
-  // vector of linksize pointing to the neighbourer
-  std::vector<uI_t> linkdir, ridknil;
-
+  // -> neighbourer holdsthe indices to loop through for each boundary condition
+  std::vector<std::vector<int>> neighbourer;
   // -> lengthener is the dx on each directions
-  std::array<T, 8> lengthener;
+  std::vector<T> lengthener;
 
   // uint8_t vector for each link indicating its directionality:
-  // - 0 is inverse (2 --> 1)
-  // - 1 is normal (1 --> 2)
-  // - 2 is forced inverse (linknode 2 --> linknode 1, no recomputing)
-  // - 3 is forced normal (linknode 1 --> linknode 2, no recomputing)
-  // - 4 is temporary invalid (for example a node can only receive flux and its
-  // neighbour is lower elevation
-  // - 5 is invalid (link index may exist, but is either inexsitant (index is
+  // - 0 is inverse (linknode 2 --> linknode 1)
+  // - 1 is normal (linknode 1 --> linknode 2)
+  // - 3 is invalid (link index may exist, but is either inexsitant (index is
   // conserved for speed reason when the link index is calculated from node
-  // index) ) see dedicated function to convert node and link indices
-  std::vector<uI_t> links;
+  // index) ) or temporarily invalid due to dynamic boundary conditions The
+  // index itself is calculated from a connector
+  std::vector<std::uint8_t> links;
+
+  // integer vector of 2*links size with the node indices of each link
+  // for example, the nodes of link #42 would be indices 84 and 85
+  std::vector<int> linknodes;
 
   // Single graph receivers
   // -> Sreceivers: steepest recervers (nnodes size),
   // -> number of donors (nnodes size),
   // -> Steepest donors (nnodes * nneighbours size)
   // --> Sdonors of node i are located from index i*nneighbours to index
   // i*nneighbours + nSdonors[i] not included
-  std::vector<int> _Sreceivers, nSdonors, Sdonors;
+  std::vector<int> Sreceivers, nSdonors, Sdonors;
 
   // Single graph distance to receivers
   std::vector<T> Sdistance2receivers;
 
   // Steepest slope
   std::vector<T> SS;
 
-  std::unordered_map<int, uI_t> converter;
-
-  bool default_permissive = false;
-
   // Coordinate stuff
   // Xs and Ys are vectors of nx and ny size converting row to y and col to X
   // Extents holds the cxmin,xmax,ymin,ymax (extent is an option in matplotlib
   // imshow plots)
   std::vector<T> Xs, Ys, extents;
 
   std::shared_ptr<easyRand> randu = std::make_shared<easyRand>();
@@ -158,1047 +137,113 @@
   D8connector(){};
 
   // construct directly from dimensions
   D8connector(int nx, int ny, T dx, T dy, T xmin, T ymin) {
     // initialisation is offset to dedicated function because some languages
     // like Julia are complicating non default constructor initialisation.
     this->init_dimensions(nx, ny, dx, dy, xmin, ymin);
-
-    // this->_allocate_vectors();
-    // this->precompute_links();
+    this->_allocate_vectors();
+    this->fill_linknodes();
   }
 
-  // Complying to the standard
-  int Sreceivers(int i) const { return this->_Sreceivers[i]; };
-
   template <class topo_t> void update_links_from_topo(topo_t &ttopo) {
     auto topo = format_input(ttopo);
     this->update_links(topo);
   }
 
   // initialise with dimension
   void init_dimensions(int nx, int ny, T dx, T dy, T xmin, T ymin) {
     int nnodes = nx * ny;
     this->set_dimensions(nx, ny, nnodes, dx, dy, xmin, ymin);
-    // std::cout << "YOLO" << std::endl;
-    this->initialise_neighbourer();
-    // std::cout << "YOLO2" << std::endl;
     this->set_default_boundaries("4edges");
   }
 
-  /// @Description: Initialising the "oldneighbourer", a data structure managing
+  /// @Description: Initialising the "neighbourer", a data structure managing
   /// the iterations though the neighbours of a given node Function of boundary
-  /// conditions, one can feed the oldneighbourer with an indice which returns
-  /// the index to ADD to the node to get its neighbour. The neighbour order is
-  /// (in table referential, be careful if Y axis is inverted) top-left, top,
+  /// conditions, one can feed the neighbourer with an indice which returns the
+  /// index to ADD to the node to get its neighbour. The neighbour order is (in
+  /// table referential, be careful if Y axis is inverted) top-left, top,
   /// top-right, left, right, bottom-left, bottom, bottom-right
   /// @Authors: B.G.
   /// @Date: 2021
-  void initialise_oldneighbourer() {
+  void initialise_neighbourer() {
     T diag = std::sqrt(std::pow(dx, 2) + std::pow(dy, 2));
     this->dxy = diag;
     this->dxmin = std::min(this->dx, this->dy);
     this->dxmax = std::max(this->dx, this->dy);
 
-    this->lengthener = std::array<T, 8>{diag, dy, diag, dx, dx, diag, dy, diag};
-    this->oldneighbourer.clear();
+    this->lengthener =
+        std::initializer_list<T>{diag, dy, diag, dx, dx, diag, dy, diag};
+    this->neighbourer.clear();
 
     // these vectors are additioned to the node indice to test the neighbors
-    this->oldneighbourer.emplace_back(std::initializer_list<int>{
+    this->neighbourer.emplace_back(std::initializer_list<int>{
         -this->nx - 1, -this->nx, -this->nx + 1, -1, 1, this->nx - 1, this->nx,
         this->nx + 1}); // internal node 0
-    this->oldneighbourer.emplace_back(std::initializer_list<int>{
+    this->neighbourer.emplace_back(std::initializer_list<int>{
         (this->ny - 1) * this->nx - 1, (this->ny - 1) * this->nx,
         (this->ny - 1) * this->nx + 1, -1, 1, this->nx - 1, this->nx,
         this->nx + 1}); // periodic_first_row 1
-    this->oldneighbourer.emplace_back(std::initializer_list<int>{
+    this->neighbourer.emplace_back(std::initializer_list<int>{
         -this->nx - 1, -this->nx, -this->nx + 1, -1, 1,
         -(this->ny - 1) * this->nx - 1, -(this->ny - 1) * this->nx,
         -(this->ny - 1) * this->nx + 1}); // periodic_last_row 2
-    this->oldneighbourer.emplace_back(std::initializer_list<int>{
+    this->neighbourer.emplace_back(std::initializer_list<int>{
         -1, -this->nx, -this->nx + 1, (this->nx - 1), 1, 2 * this->nx - 1,
         this->nx, this->nx + 1}); // periodic_first_col 3
-    this->oldneighbourer.emplace_back(std::initializer_list<int>{
+    this->neighbourer.emplace_back(std::initializer_list<int>{
         -this->nx - 1, -this->nx, -2 * this->nx + 1, -1, -this->nx + 1,
         this->nx - 1, this->nx, 1}); // periodic last_col 4
-    this->oldneighbourer.emplace_back(std::initializer_list<int>{
+    this->neighbourer.emplace_back(std::initializer_list<int>{
         this->not_a_node, this->not_a_node, this->not_a_node, -1, 1,
         this->nx - 1, this->nx, this->nx + 1}); // normal_first_row 5
-    this->oldneighbourer.emplace_back(std::initializer_list<int>{
+    this->neighbourer.emplace_back(std::initializer_list<int>{
         -this->nx - 1, -this->nx, -this->nx + 1, -1, 1, this->not_a_node,
         this->not_a_node, this->not_a_node}); // normal_last_row 6
-    this->oldneighbourer.emplace_back(std::initializer_list<int>{
+    this->neighbourer.emplace_back(std::initializer_list<int>{
         this->not_a_node, -this->nx, -this->nx + 1, this->not_a_node, 1,
         this->not_a_node, this->nx, this->nx + 1}); // normal_first_col 7
-    this->oldneighbourer.emplace_back(std::initializer_list<int>{
+    this->neighbourer.emplace_back(std::initializer_list<int>{
         -this->nx - 1, -this->nx, this->not_a_node, -1, this->not_a_node,
         this->nx - 1, this->nx, this->not_a_node}); // normal_last_col 8
-    this->oldneighbourer.emplace_back(std::initializer_list<int>{
+    this->neighbourer.emplace_back(std::initializer_list<int>{
         this->not_a_node, this->not_a_node, this->not_a_node, this->not_a_node,
         1, this->not_a_node, this->nx, this->nx + 1}); // normal_top_left 9
-    this->oldneighbourer.emplace_back(std::initializer_list<int>{
+    this->neighbourer.emplace_back(std::initializer_list<int>{
         this->not_a_node, this->not_a_node, this->not_a_node, -1,
         this->not_a_node, this->nx - 1, this->nx,
         this->not_a_node}); // normal_top_right 10
-    this->oldneighbourer.emplace_back(std::initializer_list<int>{
+    this->neighbourer.emplace_back(std::initializer_list<int>{
         this->not_a_node, -this->nx, -this->nx + 1, this->not_a_node, 1,
         this->not_a_node, this->not_a_node,
         this->not_a_node}); // normal_bottom_left 11
-    this->oldneighbourer.emplace_back(std::initializer_list<int>{
+    this->neighbourer.emplace_back(std::initializer_list<int>{
         -this->nx - 1, -this->nx, this->not_a_node, -1, this->not_a_node,
         this->not_a_node, this->not_a_node,
         this->not_a_node}); // normal_bottom_right 12
-    this->oldneighbourer.emplace_back(std::initializer_list<int>{
+    this->neighbourer.emplace_back(std::initializer_list<int>{
         this->ny * this->nx - 1, (this->ny - 1) * this->nx,
         (this->ny - 1) * this->nx + 1, this->nx - 1, 1, 2 * this->nx - 1,
         this->nx, this->nx + 1}); // top_left_periodic 13
-    this->oldneighbourer.emplace_back(std::initializer_list<int>{
+    this->neighbourer.emplace_back(std::initializer_list<int>{
         (this->ny - 1) * this->nx - 1, (this->ny - 1) * this->nx,
         (this->ny - 2) * this->nx + 1, -1, -this->nx + 1, this->nx - 1,
         this->nx, 1}); // top_right_periodic 14
-    this->oldneighbourer.emplace_back(std::initializer_list<int>{
+    this->neighbourer.emplace_back(std::initializer_list<int>{
         -1, -this->nx, -this->nx + 1, this->nx - 1, 1,
         -(this->ny - 2) * this->nx - 1, -(this->ny - 1) * this->nx,
         -(this->ny - 1) * this->nx + 1}); // periodic_bottom_left 15
-    this->oldneighbourer.emplace_back(std::initializer_list<int>{
+    this->neighbourer.emplace_back(std::initializer_list<int>{
         -this->nx - 1, -this->nx, -this->nx + 1, -1, 1 - this->nx + 1,
         -(this->ny - 1) * this->nx - 1, -(this->ny - 1) * this->nx,
         -(this->ny) * this->nx + 1}); // periodic_bottom_right 16
   }
 
-  void initialise_neighbourer() {
-
-    T diag = std::sqrt(std::pow(dx, 2) + std::pow(dy, 2));
-    this->dxy = diag;
-    this->dxmin = std::min(this->dx, this->dy);
-    this->dxmax = std::max(this->dx, this->dy);
-
-    for (int i = 0; i < 81; ++i) {
-      this->neighbourer[i] = 0;
-      this->reruobhgien[i] = 0;
-    }
-
-    // this->lengthener =
-    // std::initializer_list<T>{diag,dy,diag,dx,dx,diag,dy,diag};
-    this->lengthener = std::array<T, 8>{diag, dy, diag, dx, dx, diag, dy, diag};
-
-    // Array of adder for neighbouring:
-    // normal neighbouring
-    this->neighbourer[0] = std::numeric_limits<int>::min(); // nodata 0
-    this->converter.reserve(81);
-    this->converter[this->neighbourer[0]] = 0;
-    int aa = 1;
-    this->neighbourer[0 + aa] = 1; // right 1
-    this->converter[this->neighbourer[0 + aa]] = 0 + aa;
-    this->neighbourer[1 + aa] = this->nx + 1; // bottom right 2
-    this->converter[this->neighbourer[1 + aa]] = 1 + aa;
-    this->neighbourer[2 + aa] = this->nx; // bottom3
-    this->converter[this->neighbourer[2 + aa]] = 2 + aa;
-    this->neighbourer[3 + aa] = this->nx - 1; // bottom left4
-    this->converter[this->neighbourer[3 + aa]] = 3 + aa;
-    this->neighbourer[4 + aa] = -1; // left5
-    this->converter[this->neighbourer[4 + aa]] = 4 + aa;
-    this->neighbourer[5 + aa] = -this->nx - 1; // top left6
-    this->converter[this->neighbourer[5 + aa]] = 5 + aa;
-    this->neighbourer[6 + aa] = -this->nx; // top7
-    this->converter[this->neighbourer[6 + aa]] = 6 + aa;
-    this->neighbourer[7 + aa] = -this->nx + 1; // top right8
-    this->converter[this->neighbourer[7 + aa]] = 7 + aa;
-    // periodic neighbouring top row
-    aa += 8;
-    this->neighbourer[0 + aa] = 1; // right 9
-    this->converter[this->neighbourer[0 + aa]] = 0 + aa;
-    this->neighbourer[1 + aa] = this->nx + 1; // bottom right10
-    this->converter[this->neighbourer[1 + aa]] = 1 + aa;
-    this->neighbourer[2 + aa] = this->nx; // bottom11
-    this->converter[this->neighbourer[2 + aa]] = 2 + aa;
-    this->neighbourer[3 + aa] = this->nx - 1; // bottom left12
-    this->converter[this->neighbourer[3 + aa]] = 3 + aa;
-    this->neighbourer[4 + aa] = -1; // left13
-    this->converter[this->neighbourer[4 + aa]] = 4 + aa;
-    this->neighbourer[5 + aa] = this->nnodes - this->nx - 1; // top left14
-    this->converter[this->neighbourer[5 + aa]] = 5 + aa;
-    this->neighbourer[6 + aa] = this->nnodes - this->nx; // top15
-    this->converter[this->neighbourer[6 + aa]] = 6 + aa;
-    this->neighbourer[7 + aa] = this->nnodes - this->nx + 1; // top right16
-    this->converter[this->neighbourer[7 + aa]] = 7 + aa;
-    // periodic neighbouring bottom row
-    aa += 8;
-    this->neighbourer[0 + aa] = 1; // right 17
-    this->converter[this->neighbourer[0 + aa]] = 0 + aa;
-    this->neighbourer[1 + aa] = -this->nnodes + this->nx + 1; // bottom right18
-    this->converter[this->neighbourer[1 + aa]] = 1 + aa;
-    this->neighbourer[2 + aa] = -this->nnodes + this->nx; // bottom19
-    this->converter[this->neighbourer[2 + aa]] = 2 + aa;
-    this->neighbourer[3 + aa] = -this->nnodes + this->nx - 1; // bottom left20
-    this->converter[this->neighbourer[3 + aa]] = 3 + aa;
-    this->neighbourer[4 + aa] = -1; // left21
-    this->converter[this->neighbourer[4 + aa]] = 4 + aa;
-    this->neighbourer[5 + aa] = -this->nx - 1; // top left22
-    this->converter[this->neighbourer[5 + aa]] = 5 + aa;
-    this->neighbourer[6 + aa] = -this->nx; // top23
-    this->converter[this->neighbourer[6 + aa]] = 6 + aa;
-    this->neighbourer[7 + aa] = -this->nx + 1; // top right24
-    this->converter[this->neighbourer[7 + aa]] = 7 + aa;
-    // periodic neighbouring topleft_corner
-    aa += 8;
-    this->neighbourer[0 + aa] = 1; // right 25
-    this->converter[this->neighbourer[0 + aa]] = 0 + aa;
-    this->neighbourer[1 + aa] = this->nx + 1; // bottom right26
-    this->converter[this->neighbourer[1 + aa]] = 1 + aa;
-    this->neighbourer[2 + aa] = this->nx; // bottom27
-    this->converter[this->neighbourer[2 + aa]] = 2 + aa;
-    this->neighbourer[3 + aa] = 2 * this->nx - 1; // bottom left28
-    this->converter[this->neighbourer[3 + aa]] = 3 + aa;
-    this->neighbourer[4 + aa] = this->nx - 1; // left29
-    this->converter[this->neighbourer[4 + aa]] = 4 + aa;
-    this->neighbourer[5 + aa] = this->nnodes - 1; // top left30
-    this->converter[this->neighbourer[5 + aa]] = 5 + aa;
-    this->neighbourer[6 + aa] = this->nnodes - this->nx; // top31
-    this->converter[this->neighbourer[6 + aa]] = 6 + aa;
-    this->neighbourer[7 + aa] = this->nnodes - this->nx + 1; // top right32
-    this->converter[this->neighbourer[7 + aa]] = 7 + aa;
-    // periodic neighbouring topright_corner
-    aa += 8;
-    this->neighbourer[0 + aa] = -this->nx + 1; // right 33
-    this->converter[this->neighbourer[0 + aa]] = 0 + aa;
-    this->neighbourer[1 + aa] = 1; // bottom right34
-    this->converter[this->neighbourer[1 + aa]] = 1 + aa;
-    this->neighbourer[2 + aa] = this->nx; // bottom35
-    this->converter[this->neighbourer[2 + aa]] = 2 + aa;
-    this->neighbourer[3 + aa] = this->nx - 1; // bottom left36
-    this->converter[this->neighbourer[3 + aa]] = 3 + aa;
-    this->neighbourer[4 + aa] = -1; // left37
-    this->converter[this->neighbourer[4 + aa]] = 4 + aa;
-    this->neighbourer[5 + aa] = this->nnodes - this->nx - 1; // top left38
-    this->converter[this->neighbourer[5 + aa]] = 5 + aa;
-    this->neighbourer[6 + aa] = this->nnodes - this->nx; // top39
-    this->converter[this->neighbourer[6 + aa]] = 6 + aa;
-    this->neighbourer[7 + aa] = this->nnodes - 2 * this->nx + 1; // top right40
-    this->converter[this->neighbourer[7 + aa]] = 7 + aa;
-    // periodic neighbouring left col
-    aa += 8;
-    this->neighbourer[0 + aa] = 1; // right 41
-    this->converter[this->neighbourer[0 + aa]] = 0 + aa;
-    this->neighbourer[1 + aa] = this->nx + 1; // bottom right42
-    this->converter[this->neighbourer[1 + aa]] = 1 + aa;
-    this->neighbourer[2 + aa] = this->nx; // bottom43
-    this->converter[this->neighbourer[2 + aa]] = 2 + aa;
-    this->neighbourer[3 + aa] = 2 * this->nx - 1; // bottom left44
-    this->converter[this->neighbourer[3 + aa]] = 3 + aa;
-    this->neighbourer[4 + aa] = this->nx - 1; // left45
-    this->converter[this->neighbourer[4 + aa]] = 4 + aa;
-    this->neighbourer[5 + aa] = -1; // top left46
-    this->converter[this->neighbourer[5 + aa]] = 5 + aa;
-    this->neighbourer[6 + aa] = -this->nx; // top47
-    this->converter[this->neighbourer[6 + aa]] = 6 + aa;
-    this->neighbourer[7 + aa] = -this->nx + 1; // top right48
-    this->converter[this->neighbourer[7 + aa]] = 7 + aa;
-    // periodic neighbouring right col
-    aa += 8;
-    this->neighbourer[0 + aa] = -this->nx + 1; // right 49
-    this->converter[this->neighbourer[0 + aa]] = 0 + aa;
-    this->neighbourer[1 + aa] = 1; // bottom right50
-    this->converter[this->neighbourer[1 + aa]] = 1 + aa;
-    this->neighbourer[2 + aa] = this->nx; // bottom51
-    this->converter[this->neighbourer[2 + aa]] = 2 + aa;
-    this->neighbourer[3 + aa] = this->nx - 1; // bottom left52
-    this->converter[this->neighbourer[3 + aa]] = 3 + aa;
-    this->neighbourer[4 + aa] = -1; // left53
-    this->converter[this->neighbourer[4 + aa]] = 4 + aa;
-    this->neighbourer[5 + aa] = -this->nx - 1; // top left54
-    this->converter[this->neighbourer[5 + aa]] = 5 + aa;
-    this->neighbourer[6 + aa] = -this->nx; // top55
-    this->converter[this->neighbourer[6 + aa]] = 6 + aa;
-    this->neighbourer[7 + aa] = -1; // top right56
-    this->converter[this->neighbourer[7 + aa]] = 7 + aa;
-    // periodic neighbouring left col
-    aa += 8;
-    this->neighbourer[0 + aa] = 1; // right 57
-    this->converter[this->neighbourer[0 + aa]] = 0 + aa;
-    this->neighbourer[1 + aa] = this->nx + 1; // bottom right58
-    this->converter[this->neighbourer[1 + aa]] = 1 + aa;
-    this->neighbourer[2 + aa] = this->nx; // bottom59
-    this->converter[this->neighbourer[2 + aa]] = 2 + aa;
-    this->neighbourer[3 + aa] = 2 * this->nx - 1; // bottom left60
-    this->converter[this->neighbourer[3 + aa]] = 3 + aa;
-    this->neighbourer[4 + aa] = this->nx - 1; // left61
-    this->converter[this->neighbourer[4 + aa]] = 4 + aa;
-    this->neighbourer[5 + aa] = -1; // top left62
-    this->converter[this->neighbourer[5 + aa]] = 5 + aa;
-    this->neighbourer[6 + aa] = -this->nx; // top63
-    this->converter[this->neighbourer[6 + aa]] = 6 + aa;
-    this->neighbourer[7 + aa] = -this->nx + 1; // top right64
-    this->converter[this->neighbourer[7 + aa]] = 7 + aa;
-    // periodic neighbouring bottomleft_corner
-    aa += 8;
-    this->neighbourer[0 + aa] = 1; // right 65
-    this->converter[this->neighbourer[0 + aa]] = 0 + aa;
-    this->neighbourer[1 + aa] = -this->nnodes + this->nx + 1; // bottom right66
-    this->converter[this->neighbourer[1 + aa]] = 1 + aa;
-    this->neighbourer[2 + aa] = -this->nnodes + this->nx; // bottom67
-    this->converter[this->neighbourer[2 + aa]] = 2 + aa;
-    this->neighbourer[3 + aa] =
-        -this->nnodes + 2 * this->nx - 1; // bottom left68
-    this->converter[this->neighbourer[3 + aa]] = 3 + aa;
-    this->neighbourer[4 + aa] = this->nx - 1; // left69
-    this->converter[this->neighbourer[4 + aa]] = 4 + aa;
-    this->neighbourer[5 + aa] = -1; // top left70
-    this->converter[this->neighbourer[5 + aa]] = 5 + aa;
-    this->neighbourer[6 + aa] = -this->nx; // top71
-    this->converter[this->neighbourer[6 + aa]] = 6 + aa;
-    this->neighbourer[7 + aa] = -this->nx + 1; // top right72
-    this->converter[this->neighbourer[7 + aa]] = 7 + aa;
-    // periodic neighbouring bottomright_corner
-    aa += 8;
-    this->neighbourer[0 + aa] = -this->nx + 1; // right 73
-    this->converter[this->neighbourer[0 + aa]] = 0 + aa;
-    this->neighbourer[1 + aa] = -this->nnodes + 1; // bottom right74
-    this->converter[this->neighbourer[1 + aa]] = 1 + aa;
-    this->neighbourer[2 + aa] = -this->nnodes + this->nx; // bottom75
-    this->converter[this->neighbourer[2 + aa]] = 2 + aa;
-    this->neighbourer[3 + aa] = -this->nnodes + this->nx - 1; // bottom left76
-    this->converter[this->neighbourer[3 + aa]] = 3 + aa;
-    this->neighbourer[4 + aa] = -1; // left77
-    this->converter[this->neighbourer[4 + aa]] = 4 + aa;
-    this->neighbourer[5 + aa] = -this->nx - 1; // top left78
-    this->converter[this->neighbourer[5 + aa]] = 5 + aa;
-    this->neighbourer[6 + aa] = -this->nx; // top79
-    this->converter[this->neighbourer[6 + aa]] = 6 + aa;
-    this->neighbourer[7 + aa] = -2 * this->nx + 1; // top right80
-    this->converter[this->neighbourer[7 + aa]] = 7 + aa;
-
-    for (int i = 0; i < 81; ++i) {
-      this->reruobhgien[i] = -1 * this->neighbourer[i];
-    }
-  }
-
-  int get_right_idx_links(int i) { return i * 4; }
-  int get_bottomright_idx_links(int i) { return i * 4 + 1; }
-  int get_bottom_idx_links(int i) { return i * 4 + 2; }
-  int get_bottomleft_idx_links(int i) { return i * 4 + 3; }
-
-  int get_left_idx_links(int i) {
-    int modi = fast_mod(i, this->nx);
-    return this->get_left_idx_links(i, modi);
-  }
-
-  int get_left_idx_links(int i, int modi) {
-    int o = -1;
-    if (i > this->nx && i < this->nnodes - this->nx - 1 && modi > 0 &&
-        modi != (this->nx - 1)) {
-      o = i + this->neighbourer[5];
-    } else if (i == 0) {
-      o = i + this->neighbourer[29];
-    } else if (i == this->nx - 1) {
-      o = i + this->neighbourer[37];
-    } else if (i == this->nnodes - this->nx) {
-      o = i + this->neighbourer[69]; // woooo
-    } else if (i == this->nnodes - 1) {
-      o = i + this->neighbourer[77];
-    } else if (this->is_on_top_row(i)) {
-      o = i + this->neighbourer[13];
-    } else if (this->is_on_bottom_row(i)) {
-      o = i + this->neighbourer[21];
-    } else if (modi == 0) {
-      o = i + this->neighbourer[45];
-    } else if (modi == this->nx - 1) {
-      o = i + this->neighbourer[53];
-    }
-    return this->get_right_idx_links(o);
-  }
-
-  int get_topleft_idx_links(int i) {
-    int modi = fast_mod(i, this->nx);
-    return this->get_topleft_idx_links(i, modi);
-  }
-
-  int get_topleft_idx_links(int i, int modi) {
-    int o = -1;
-    if (i > this->nx && i < this->nnodes - this->nx - 1 && modi > 0 &&
-        modi != (this->nx - 1)) {
-      o = i + this->neighbourer[6];
-    } else if (i == 0) {
-      o = i + this->neighbourer[30];
-    } else if (i == this->nx - 1) {
-      o = i + this->neighbourer[38];
-    } else if (i == this->nnodes - this->nx) {
-      o = i + this->neighbourer[70]; // woooo
-    } else if (i == this->nnodes - 1) {
-      o = i + this->neighbourer[78];
-    } else if (this->is_on_top_row(i)) {
-      o = i + this->neighbourer[14];
-    } else if (this->is_on_bottom_row(i)) {
-      o = i + this->neighbourer[22];
-    } else if (modi == 0) {
-      o = i + this->neighbourer[46];
-    } else if (modi == this->nx - 1) {
-      o = i + this->neighbourer[54];
-    }
-    return this->get_bottomright_idx_links(o);
-  }
-
-  int get_top_idx_links(int i) {
-    int modi = fast_mod(i, this->nx);
-    return this->get_top_idx_links(i, modi);
-  }
-
-  int get_top_idx_links(int i, int modi) {
-    int o = -1;
-    if (i > this->nx && i < this->nnodes - this->nx - 1 && modi > 0 &&
-        modi != (this->nx - 1)) {
-      o = i + this->neighbourer[7];
-    } else if (i == 0) {
-      o = i + this->neighbourer[31];
-    } else if (i == this->nx - 1) {
-      o = i + this->neighbourer[39];
-    } else if (i == this->nnodes - this->nx) {
-      o = i + this->neighbourer[71]; // woooo
-    } else if (i == this->nnodes - 1) {
-      o = i + this->neighbourer[79];
-    } else if (this->is_on_top_row(i)) {
-      o = i + this->neighbourer[15];
-    } else if (this->is_on_bottom_row(i)) {
-      o = i + this->neighbourer[23];
-    } else if (modi == 0) {
-      o = i + this->neighbourer[47];
-    } else if (modi == this->nx - 1) {
-      o = i + this->neighbourer[55];
-    }
-    return this->get_bottom_idx_links(o);
-  }
-
-  int get_topright_idx_links(int i) {
-    int modi = fast_mod(i, this->nx);
-    return this->get_topright_idx_links(i, modi);
-  }
-
-  int get_topright_idx_links(int i, int modi) {
-    int o = -1;
-    if (i > this->nx && i < this->nnodes - this->nx - 1 && modi > 0 &&
-        modi != (this->nx - 1)) {
-      o = i + this->neighbourer[8];
-    } else if (i == 0) {
-      o = i + this->neighbourer[32];
-    } else if (i == this->nx - 1) {
-      o = i + this->neighbourer[40];
-    } else if (i == this->nnodes - this->nx) {
-      o = i + this->neighbourer[72]; // woooo
-    } else if (i == this->nnodes - 1) {
-      o = i + this->neighbourer[80];
-    } else if (this->is_on_top_row(i)) {
-      o = i + this->neighbourer[16];
-    } else if (this->is_on_bottom_row(i)) {
-      o = i + this->neighbourer[24];
-    } else if (modi == 0) {
-      o = i + this->neighbourer[48];
-    } else if (modi == this->nx - 1) {
-      o = i + this->neighbourer[56];
-    }
-    return this->get_bottomleft_idx_links(o);
-  }
-
-  int get_left_idx(int i) {
-    int li = this->get_left_idx_links(i);
-    if (this->is_link_valid(li) == false)
-      return -1;
-    else
-      return i + this->reruobhgien[this->ridknil[li]];
-  }
-
-  int get_top_idx(int i) {
-    int li = this->get_top_idx_links(i);
-    if (this->is_link_valid(li) == false)
-      return -1;
-    else {
-      return i + this->reruobhgien[this->ridknil[li]];
-    }
-  }
-
-  int get_right_idx(int i) {
-    int li = this->get_right_idx_links(i);
-    if (this->is_link_valid(li) == false)
-      return -1;
-    else {
-      return i + this->neighbourer[this->linkdir[li]];
-    }
-  }
-
-  int get_bottom_idx(int i) {
-    int li = this->get_bottom_idx_links(i);
-    if (this->is_link_valid(li) == false)
-      return -1;
-    else {
-      return i + this->neighbourer[this->linkdir[li]];
-    }
-  }
-
-  // D8 single neighbour extra routines
-  int get_topleft_idx(int i) {
-    int li = this->get_topleft_idx_links(i);
-    if (this->is_link_valid(li) == false)
-      return -1;
-    else
-      return i + this->reruobhgien[this->ridknil[li]];
-  }
-
-  int get_topright_idx(int i) {
-    int li = this->get_topright_idx_links(i);
-    if (this->is_link_valid(li) == false)
-      return -1;
-    else
-      return i + this->reruobhgien[this->ridknil[li]];
-  }
-
-  int get_bottomleft_idx(int i) {
-    int li = this->get_bottomleft_idx_links(i);
-    if (this->is_link_valid(li) == false)
-      return -1;
-    else
-      return i + this->reruobhgien[this->ridknil[li]];
-  }
-
-  int get_bottomright_idx(int i) {
-    int li = this->get_bottomright_idx_links(i);
-    if (this->is_link_valid(li) == false)
-      return -1;
-    else
-      return i + this->neighbourer[this->linkdir[li]];
-  }
-
-  int get_raw_right_idx(int i) {
-    int modi = fast_mod(i, this->nx);
-    return this->get_raw_right_idx(i, modi);
-  }
-
-  int get_raw_right_idx(int i, int modi) {
-    int o;
-    if (i > this->nx && i < this->nnodes - this->nx - 1 && modi > 0 &&
-        modi != (this->nx - 1)) {
-      o = i + this->neighbourer[1];
-    } else if (i == 0) {
-      o = i + this->neighbourer[25];
-    } else if (i == this->nx - 1) {
-      o = i + this->neighbourer[33];
-    } else if (i == this->nnodes - this->nx) {
-      o = i + this->neighbourer[65]; // woooo
-    } else if (i == this->nnodes - 1) {
-      o = i + this->neighbourer[73];
-    } else if (this->is_on_top_row(i)) {
-      o = i + this->neighbourer[9];
-    } else if (this->is_on_bottom_row(i)) {
-      o = i + this->neighbourer[17];
-    } else if (modi == 0) {
-      o = i + this->neighbourer[41];
-    } else if (modi == this->nx - 1) {
-      o = i + this->neighbourer[49];
-    }
-
-    return o;
-  }
-
-  int get_raw_bottomright_idx(int i) {
-    int modi = fast_mod(i, this->nx);
-    return this->get_raw_bottomright_idx(i, modi);
-  }
-
-  int get_raw_bottomright_idx(int i, int modi) {
-    int o;
-    if (i > this->nx && i < this->nnodes - this->nx - 1 && modi > 0 &&
-        modi != (this->nx - 1)) {
-      o = i + this->neighbourer[2];
-    } else if (i == 0) {
-      o = i + this->neighbourer[26];
-    } else if (i == this->nx - 1) {
-      o = i + this->neighbourer[34];
-    } else if (i == this->nnodes - this->nx) {
-      o = i + this->neighbourer[66]; // woooo
-    } else if (i == this->nnodes - 1) {
-      o = i + this->neighbourer[74];
-    } else if (this->is_on_top_row(i)) {
-      o = i + this->neighbourer[10];
-    } else if (this->is_on_bottom_row(i)) {
-      o = i + this->neighbourer[18];
-    } else if (modi == 0) {
-      o = i + this->neighbourer[42];
-    } else if (modi == this->nx - 1) {
-      o = i + this->neighbourer[50];
-    }
-
-    return o;
-  }
-
-  int get_raw_bottom_idx(int i) {
-    int modi = fast_mod(i, this->nx);
-    return this->get_raw_bottom_idx(i, modi);
-  }
-
-  int get_raw_bottom_idx(int i, int modi) {
-    int o;
-    if (i > this->nx && i < this->nnodes - this->nx - 1 && modi > 0 &&
-        modi != (this->nx - 1)) {
-      o = i + this->neighbourer[3];
-    } else if (i == 0) {
-      o = i + this->neighbourer[27];
-    } else if (i == this->nx - 1) {
-      o = i + this->neighbourer[35];
-    } else if (i == this->nnodes - this->nx) {
-      o = i + this->neighbourer[67]; // woooo
-    } else if (i == this->nnodes - 1) {
-      o = i + this->neighbourer[75];
-    } else if (this->is_on_top_row(i)) {
-      o = i + this->neighbourer[11];
-    } else if (this->is_on_bottom_row(i)) {
-      o = i + this->neighbourer[19];
-    } else if (modi == 0) {
-      o = i + this->neighbourer[43];
-    } else if (modi == this->nx - 1) {
-      o = i + this->neighbourer[51];
-    }
-
-    return o;
-  }
-
-  int get_raw_bottomleft_idx(int i) {
-    int modi = fast_mod(i, this->nx);
-    return this->get_raw_bottomleft_idx(i, modi);
-  }
-
-  int get_raw_bottomleft_idx(int i, int modi) {
-    int o;
-    if (i > this->nx && i < this->nnodes - this->nx - 1 && modi > 0 &&
-        modi != (this->nx - 1)) {
-      o = i + this->neighbourer[4];
-    } else if (i == 0) {
-      o = i + this->neighbourer[28];
-    } else if (i == this->nx - 1) {
-      o = i + this->neighbourer[36];
-    } else if (i == this->nnodes - this->nx) {
-      o = i + this->neighbourer[68]; // woooo
-    } else if (i == this->nnodes - 1) {
-      o = i + this->neighbourer[76];
-    } else if (this->is_on_top_row(i)) {
-      o = i + this->neighbourer[12];
-    } else if (this->is_on_bottom_row(i)) {
-      o = i + this->neighbourer[20];
-    } else if (modi == 0) {
-      o = i + this->neighbourer[44];
-    } else if (modi == this->nx - 1) {
-      o = i + this->neighbourer[52];
-    }
-
-    return o;
-  }
-
-  int get_raw_left_idx(int i) {
-    int modi = fast_mod(i, this->nx);
-    return this->get_raw_left_idx(i, modi);
-  }
-
-  int get_raw_left_idx(int i, int modi) {
-    int o;
-    if (i > this->nx && i < this->nnodes - this->nx - 1 && modi > 0 &&
-        modi != (this->nx - 1)) {
-      o = i + this->neighbourer[5];
-    } else if (i == 0) {
-      o = i + this->neighbourer[29];
-    } else if (i == this->nx - 1) {
-      o = i + this->neighbourer[37];
-    } else if (i == this->nnodes - this->nx) {
-      o = i + this->neighbourer[69]; // woooo
-    } else if (i == this->nnodes - 1) {
-      o = i + this->neighbourer[77];
-    } else if (this->is_on_top_row(i)) {
-      o = i + this->neighbourer[13];
-    } else if (this->is_on_bottom_row(i)) {
-      o = i + this->neighbourer[21];
-    } else if (modi == 0) {
-      o = i + this->neighbourer[45];
-    } else if (modi == this->nx - 1) {
-      o = i + this->neighbourer[53];
-    }
-
-    return o;
-  }
-
-  int get_raw_topleft_idx(int i) {
-    int modi = fast_mod(i, this->nx);
-    return this->get_raw_topleft_idx(i, modi);
-  }
-
-  int get_raw_topleft_idx(int i, int modi) {
-    int o;
-    if (i > this->nx && i < this->nnodes - this->nx - 1 && modi > 0 &&
-        modi != (this->nx - 1)) {
-      o = i + this->neighbourer[6];
-    } else if (i == 0) {
-      o = i + this->neighbourer[30];
-    } else if (i == this->nx - 1) {
-      o = i + this->neighbourer[38];
-    } else if (i == this->nnodes - this->nx) {
-      o = i + this->neighbourer[70]; // woooo
-    } else if (i == this->nnodes - 1) {
-      o = i + this->neighbourer[78];
-    } else if (this->is_on_top_row(i)) {
-      o = i + this->neighbourer[14];
-    } else if (this->is_on_bottom_row(i)) {
-      o = i + this->neighbourer[22];
-    } else if (modi == 0) {
-      o = i + this->neighbourer[46];
-    } else if (modi == this->nx - 1) {
-      o = i + this->neighbourer[54];
-    }
-
-    return o;
-  }
-
-  int get_raw_top_idx(int i) {
-    int modi = fast_mod(i, this->nx);
-    return this->get_raw_top_idx(i, modi);
-  }
-
-  int get_raw_top_idx(int i, int modi) {
-    int o;
-    if (i > this->nx && i < this->nnodes - this->nx - 1 && modi > 0 &&
-        modi != (this->nx - 1)) {
-      o = i + this->neighbourer[7];
-    } else if (i == 0) {
-      o = i + this->neighbourer[31];
-    } else if (i == this->nx - 1) {
-      o = i + this->neighbourer[39];
-    } else if (i == this->nnodes - this->nx) {
-      o = i + this->neighbourer[71]; // woooo
-    } else if (i == this->nnodes - 1) {
-      o = i + this->neighbourer[79];
-    } else if (this->is_on_top_row(i)) {
-      o = i + this->neighbourer[15];
-    } else if (this->is_on_bottom_row(i)) {
-      o = i + this->neighbourer[23];
-    } else if (modi == 0) {
-      o = i + this->neighbourer[47];
-    } else if (modi == this->nx - 1) {
-      o = i + this->neighbourer[55];
-    }
-
-    return o;
-  }
-
-  int get_raw_topright_idx(int i) {
-    int modi = fast_mod(i, this->nx);
-    return this->get_raw_topright_idx(i, modi);
-  }
-
-  int get_raw_topright_idx(int i, int modi) {
-    int o;
-    if (i > this->nx && i < this->nnodes - this->nx - 1 && modi > 0 &&
-        modi != (this->nx - 1)) {
-      o = i + this->neighbourer[8];
-    } else if (i == 0) {
-      o = i + this->neighbourer[32];
-    } else if (i == this->nx - 1) {
-      o = i + this->neighbourer[40];
-    } else if (i == this->nnodes - this->nx) {
-      o = i + this->neighbourer[72]; // woooo
-    } else if (i == this->nnodes - 1) {
-      o = i + this->neighbourer[80];
-    } else if (this->is_on_top_row(i)) {
-      o = i + this->neighbourer[16];
-    } else if (this->is_on_bottom_row(i)) {
-      o = i + this->neighbourer[24];
-    } else if (modi == 0) {
-      o = i + this->neighbourer[48];
-    } else if (modi == this->nx - 1) {
-      o = i + this->neighbourer[56];
-    }
-
-    return o;
-  }
-
-  int get_raw_right_idx(int i, int modi, uI_t &dir) {
-    int o;
-    if (i > this->nx && i < this->nnodes - this->nx - 1 && modi > 0 &&
-        modi != (this->nx - 1)) {
-      o = i + this->neighbourer[1];
-      dir = 1;
-    } else if (i == 0) {
-      o = i + this->neighbourer[25];
-      dir = 25;
-    } else if (i == this->nx - 1) {
-      o = i + this->neighbourer[33];
-      dir = 33;
-    } else if (i == this->nnodes - this->nx) {
-      o = i + this->neighbourer[65]; // woooo
-      dir = 65;
-    } else if (i == this->nnodes - 1) {
-      o = i + this->neighbourer[73];
-      dir = 73;
-    } else if (this->is_on_top_row(i)) {
-      o = i + this->neighbourer[9];
-      dir = 9;
-    } else if (this->is_on_bottom_row(i)) {
-      o = i + this->neighbourer[17];
-      dir = 17;
-    } else if (modi == 0) {
-      o = i + this->neighbourer[41];
-      dir = 41;
-    } else if (modi == this->nx - 1) {
-      o = i + this->neighbourer[49];
-      dir = 49;
-    }
-
-    return o;
-  }
-
-  int get_raw_bottomright_idx(int i, int modi, uI_t &dir) {
-    int o;
-    if (i > this->nx && i < this->nnodes - this->nx - 1 && modi > 0 &&
-        modi != (this->nx - 1)) {
-      o = i + this->neighbourer[2];
-      dir = 2;
-    } else if (i == 0) {
-      o = i + this->neighbourer[26];
-      dir = 26;
-    } else if (i == this->nx - 1) {
-      o = i + this->neighbourer[34];
-      dir = 34;
-    } else if (i == this->nnodes - this->nx) {
-      o = i + this->neighbourer[66]; // woooo
-      dir = 66;
-    } else if (i == this->nnodes - 1) {
-      o = i + this->neighbourer[74];
-      dir = 74;
-    } else if (this->is_on_top_row(i)) {
-      o = i + this->neighbourer[10];
-      dir = 10;
-    } else if (this->is_on_bottom_row(i)) {
-      o = i + this->neighbourer[18];
-      dir = 18;
-    } else if (modi == 0) {
-      o = i + this->neighbourer[42];
-      dir = 42;
-    } else if (modi == this->nx - 1) {
-      o = i + this->neighbourer[50];
-      dir = 50;
-    }
-
-    return o;
-  }
-
-  int get_raw_bottom_idx(int i, int modi, uI_t &dir) {
-    int o;
-    if (i > this->nx && i < this->nnodes - this->nx - 1 && modi > 0 &&
-        modi != (this->nx - 1)) {
-      o = i + this->neighbourer[3];
-      dir = 3;
-    } else if (i == 0) {
-      o = i + this->neighbourer[27];
-      dir = 27;
-    } else if (i == this->nx - 1) {
-      o = i + this->neighbourer[35];
-      dir = 35;
-    } else if (i == this->nnodes - this->nx) {
-      o = i + this->neighbourer[67]; // woooo
-      dir = 67;
-    } else if (i == this->nnodes - 1) {
-      o = i + this->neighbourer[75];
-      dir = 75;
-    } else if (this->is_on_top_row(i)) {
-      o = i + this->neighbourer[11];
-      dir = 11;
-    } else if (this->is_on_bottom_row(i)) {
-      o = i + this->neighbourer[19];
-      dir = 19;
-    } else if (modi == 0) {
-      o = i + this->neighbourer[43];
-      dir = 43;
-    } else if (modi == this->nx - 1) {
-      o = i + this->neighbourer[51];
-      dir = 51;
-    }
-
-    return o;
-  }
-
-  int get_raw_bottomleft_idx(int i, int modi, uI_t &dir) {
-    int o;
-    if (i > this->nx && i < this->nnodes - this->nx - 1 && modi > 0 &&
-        modi != (this->nx - 1)) {
-      o = i + this->neighbourer[4];
-      dir = 4;
-    } else if (i == 0) {
-      o = i + this->neighbourer[28];
-      dir = 28;
-    } else if (i == this->nx - 1) {
-      o = i + this->neighbourer[36];
-      dir = 36;
-    } else if (i == this->nnodes - this->nx) {
-      o = i + this->neighbourer[68]; // woooo
-      dir = 68;
-    } else if (i == this->nnodes - 1) {
-      o = i + this->neighbourer[76];
-      dir = 76;
-    } else if (this->is_on_top_row(i)) {
-      o = i + this->neighbourer[12];
-      dir = 12;
-    } else if (this->is_on_bottom_row(i)) {
-      o = i + this->neighbourer[20];
-      dir = 20;
-    } else if (modi == 0) {
-      o = i + this->neighbourer[44];
-      dir = 44;
-    } else if (modi == this->nx - 1) {
-      o = i + this->neighbourer[52];
-      dir = 52;
-    }
-
-    return o;
-  }
-
-  int get_raw_left_idx(int i, int modi, uI_t &dir) {
-    int o;
-    if (i > this->nx && i < this->nnodes - this->nx - 1 && modi > 0 &&
-        modi != (this->nx - 1)) {
-      o = i + this->neighbourer[5];
-      dir = 5;
-    } else if (i == 0) {
-      o = i + this->neighbourer[29];
-      dir = 29;
-    } else if (i == this->nx - 1) {
-      o = i + this->neighbourer[37];
-      dir = 37;
-    } else if (i == this->nnodes - this->nx) {
-      o = i + this->neighbourer[69]; // woooo
-      dir = 69;
-    } else if (i == this->nnodes - 1) {
-      o = i + this->neighbourer[77];
-      dir = 77;
-    } else if (this->is_on_top_row(i)) {
-      o = i + this->neighbourer[13];
-      dir = 13;
-    } else if (this->is_on_bottom_row(i)) {
-      o = i + this->neighbourer[21];
-      dir = 21;
-    } else if (modi == 0) {
-      o = i + this->neighbourer[45];
-      dir = 45;
-    } else if (modi == this->nx - 1) {
-      o = i + this->neighbourer[53];
-      dir = 53;
-    }
-
-    return o;
-  }
-
-  int get_raw_topleft_idx(int i, int modi, uI_t &dir) {
-    int o;
-    if (i > this->nx && i < this->nnodes - this->nx - 1 && modi > 0 &&
-        modi != (this->nx - 1)) {
-      o = i + this->neighbourer[6];
-      dir = 6;
-    } else if (i == 0) {
-      o = i + this->neighbourer[30];
-      dir = 30;
-    } else if (i == this->nx - 1) {
-      o = i + this->neighbourer[38];
-      dir = 38;
-    } else if (i == this->nnodes - this->nx) {
-      o = i + this->neighbourer[70]; // woooo
-      dir = 70;
-    } else if (i == this->nnodes - 1) {
-      o = i + this->neighbourer[78];
-      dir = 78;
-    } else if (this->is_on_top_row(i)) {
-      o = i + this->neighbourer[14];
-      dir = 14;
-    } else if (this->is_on_bottom_row(i)) {
-      o = i + this->neighbourer[22];
-      dir = 22;
-    } else if (modi == 0) {
-      o = i + this->neighbourer[46];
-      dir = 46;
-    } else if (modi == this->nx - 1) {
-      o = i + this->neighbourer[54];
-      dir = 54;
-    }
-
-    return o;
-  }
-
-  int get_raw_top_idx(int i, int modi, uI_t &dir) {
-    int o;
-    if (i > this->nx && i < this->nnodes - this->nx - 1 && modi > 0 &&
-        modi != (this->nx - 1)) {
-      o = i + this->neighbourer[7];
-      dir = 7;
-    } else if (i == 0) {
-      o = i + this->neighbourer[31];
-      dir = 31;
-    } else if (i == this->nx - 1) {
-      o = i + this->neighbourer[39];
-      dir = 39;
-    } else if (i == this->nnodes - this->nx) {
-      o = i + this->neighbourer[71]; // woooo
-      dir = 71;
-    } else if (i == this->nnodes - 1) {
-      o = i + this->neighbourer[79];
-      dir = 79;
-    } else if (this->is_on_top_row(i)) {
-      o = i + this->neighbourer[15];
-      dir = 15;
-    } else if (this->is_on_bottom_row(i)) {
-      o = i + this->neighbourer[23];
-      dir = 23;
-    } else if (modi == 0) {
-      o = i + this->neighbourer[47];
-      dir = 47;
-    } else if (modi == this->nx - 1) {
-      o = i + this->neighbourer[55];
-      dir = 55;
-    }
-
-    return o;
-  }
-
-  int get_raw_topright_idx(int i, int modi, uI_t &dir) {
-    int o;
-    if (i > this->nx && i < this->nnodes - this->nx - 1 && modi > 0 &&
-        modi != (this->nx - 1)) {
-      o = i + this->neighbourer[8];
-      dir = 8;
-    } else if (i == 0) {
-      o = i + this->neighbourer[32];
-      dir = 32;
-    } else if (i == this->nx - 1) {
-      o = i + this->neighbourer[40];
-      dir = 40;
-    } else if (i == this->nnodes - this->nx) {
-      o = i + this->neighbourer[72]; // woooo
-      dir = 72;
-    } else if (i == this->nnodes - 1) {
-      o = i + this->neighbourer[80];
-      dir = 80;
-    } else if (this->is_on_top_row(i)) {
-      o = i + this->neighbourer[16];
-      dir = 16;
-    } else if (this->is_on_bottom_row(i)) {
-      o = i + this->neighbourer[24];
-      dir = 24;
-    } else if (modi == 0) {
-      o = i + this->neighbourer[48];
-      dir = 48;
-    } else if (modi == this->nx - 1) {
-      o = i + this->neighbourer[56];
-      dir = 56;
-    }
-
-    return o;
-  }
-
   /// @description: Sets the dimension of the graph and initialise the
-  /// oldneighbourer
+  /// neighbourer
   void set_dimensions(int nx, int ny, int nnodes, T dx, T dy, T xmin, T ymin) {
     this->nx = nx;
     this->ny = ny;
     this->nnodes = nnodes;
     this->nnodes_t = size_t(nnodes);
     this->dx = dx;
     this->dy = dy;
@@ -1206,15 +251,15 @@
     this->Xmin = xmin;
     this->Ymin = ymin;
 
     // Not a node is utilised to detect when a neighbouring operation returns
     // not a node
     this->not_a_node = -nx * ny * 2;
 
-    // this->initialise_oldneighbourer();
+    this->initialise_neighbourer();
 
     // Initialise coordinate stuff
     this->Xs = std::vector<T>(this->nx);
     this->Ys = std::vector<T>(this->ny);
     // this->extents = std::vector<T>(4,0);
 
     for (int i = 0; i < this->nx; ++i)
@@ -1235,832 +280,792 @@
   void set_default_boundaries(std::string bountype) {
 
     this->boundaries.codes = std::vector<BC>(this->nnodes_t, BC::FLOW);
 
     if (bountype == "4edges") {
       for (size_t i = 0; i < this->nnodes_t; ++i) {
         if (this->is_on_dem_edge(i))
-          this->boundaries.codes[i] =
-              (this->default_permissive) ? BC::CAN_OUT : BC::OUT;
+          this->boundaries.codes[i] = BC::FORCE_OUT;
       }
     } else if (bountype == "periodic_EW") {
       for (int i = 0; i < this->nnodes; ++i) {
         if (this->is_on_top_row(i) || this->is_on_bottom_row(i))
-          this->boundaries.codes[i] =
-              (this->default_permissive) ? BC::CAN_OUT : BC::OUT;
+          this->boundaries.codes[i] = BC::FORCE_OUT;
         else if (this->is_on_leftest_col(i) || this->is_on_rightest_col(i))
           this->boundaries.codes[i] = BC::PERIODIC_BORDER;
       }
     } else if (bountype == "periodic_NS") {
       for (int i = 0; i < this->nnodes; ++i) {
         if (this->is_on_leftest_col(i) || this->is_on_rightest_col(i))
-          this->boundaries.codes[i] =
-              (this->default_permissive) ? BC::CAN_OUT : BC::OUT;
+          this->boundaries.codes[i] = BC::FORCE_OUT;
         else if (this->is_on_top_row(i) || this->is_on_bottom_row(i))
           this->boundaries.codes[i] = BC::PERIODIC_BORDER;
       }
     } else {
       throw std::runtime_error("invalid periodic boundaries");
     }
 
-    this->precompute_links();
+    // Recomputing fillnodes
+    // this->fill_linknodes();
+    this->_allocate_vectors();
+    this->fill_linknodes();
   }
 
   // Set all the out boundaries to 3, meaning they can now give to lower
   // elevation neighbours
   void set_out_boundaries_to_permissive() {
     for (auto &v : this->boundaries.codes) {
       if (v == BC::FORCE_OUT)
         v = BC::OUT;
     }
-    this->precompute_links();
   }
 
   template <class bou_t> void set_custom_boundaries(bou_t &tbound) {
     auto bound = format_input(tbound);
 
     std::vector<BC> ubound(bound.size(), BC::FLOW);
-    for (size_t i = 0; i < ubound.size(); ++i)
+    for (int i = 0; i < tbound.size(); ++i)
       ubound[i] = static_cast<BC>(bound[i]);
 
     this->boundaries.set_codes(ubound);
-    this->precompute_links();
+    this->_allocate_vectors();
+    this->fill_linknodes();
   }
 
   BC get_boundary_at_node(int i) { return this->boundaries.codes[i]; }
 
   bool is_in_bound(int i) {
     return (i >= 0 && i < this->nnodes) ? true : false;
   }
 
-  // Checks the validity of a link
-  template <class ti_t> bool is_link_valid(ti_t i) {
-    if (this->links[i] > 3) {
-      return false;
-    }
-    return true;
-  }
-  // Checks the validity of a link
-
-  template <class ti_t> bool is_link_normal(ti_t i) {
-    if (this->links[i] == 1 || this->links[i] == 3)
-      return true;
-    return false;
-  }
-
-  template <class ti_t> bool is_link_inverse(ti_t i) {
-    if (this->links[i] == 0 || this->links[i] == 2)
-      return true;
-    return false;
-  }
-
-  template <class ti_t> bool is_link_forced(ti_t i) {
-    if (this->links[i] == 2 || this->links[i] == 3)
-      return true;
-    return false;
-  }
-
-  template <class ti_t> void reverse_link(ti_t i) {
-    if (this->links[i] == 0)
-      this->links[i] = 1;
-    else if (this->links[i] == 1)
-      this->links[i] = 0;
-  }
-
-  template <class ti_t, class topo_t>
-  void update_local_link(ti_t i, topo_t &topo) {
-
-    if (this->link_needs_processing(i) == false)
-      return;
-
-    int O, A;
-    this->node_idx_from_link_idx(i, O, A);
-    if (topo[O] > topo[A])
-      this->links[i] = 1;
-    else
-      this->links[i] = 0;
-  }
-
-  // This version informs in place O and A, the two link nodes
-  template <class ti_t, class topo_t>
-  void update_local_link(ti_t i, topo_t &topo, int &O, int &A) {
-
-    if (this->link_needs_processing(i) == false)
-      return;
-
-    this->node_idx_from_link_idx(i, O, A);
-    if (topo[O] > topo[A])
-      this->links[i] = 1;
-    else
-      this->links[i] = 0;
-  }
-
-  template <class ti_t> bool link_needs_processing(ti_t i) {
-    if (this->links[i] == 5)
-      return false;
-
-    return true;
-  }
-
-  // DEPRECATED
-  // void fill_linknodes(){;}
-
-  int get_neighbour_idx_links_nochecks(int i, std::array<int, 8> &tin) {
-    tin[0] = this->get_right_idx_links(i);
-    tin[1] = this->get_bottomright_idx_links(i);
-    tin[2] = this->get_bottom_idx_links(i);
-    tin[3] = this->get_bottomleft_idx_links(i);
-    tin[4] = this->get_left_idx_links(i);
-    tin[5] = this->get_topleft_idx_links(i);
-    tin[6] = this->get_top_idx_links(i);
-    tin[7] = this->get_topright_idx_links(i);
-    return 8;
-  }
-
-  int get_neighbour_idx_links(int i, std::array<int, 8> &tin) {
-    int size = 0;
-
-    for (int j = 0; j < 4; ++j) {
-      int li = i * 4 + j;
-      if (this->is_link_valid(li)) {
-        tin[size] = li;
-        ++size;
-      }
-      int oli = (i + this->reruobhgien[this->ridknil[li]]) * 4 + j;
-      if (this->is_link_valid(oli)) {
-        tin[size] = oli;
-        ++size;
-      }
-    }
-    return size;
-  }
-
-  int get_neighbour_idx_nodes_and_links(int i, std::array<int, 8> &tin_nodes,
-                                        std::array<int, 8> &tin_links) {
-    int size = 0;
-
-    for (int j = 0; j < 4; ++j) {
-      int li = i * 4 + j;
-      if (this->is_link_valid(li)) {
-        tin_links[size] = li;
-        tin_nodes[size] = i + this->neighbourer[this->linkdir[li]];
-        ++size;
-      }
-      int oli = (i + this->reruobhgien[this->ridknil[li]]) * 4 + j;
-      if (this->is_link_valid(oli)) {
-        tin_links[size] = oli;
-        tin_nodes[size] = i + this->reruobhgien[this->ridknil[li]];
-        ;
-        ++size;
-      }
-    }
-    return size;
-  }
-
-  template <class tfT, class topo_t>
-  int get_neighbour_idx_nodes_links_external_array(
-      int i, std::array<int, 8> &tin_nodes, std::array<int, 8> &tin_links,
-      std::array<tfT, 8> &tin_arr, topo_t &datat) {
-    int size = 0;
-
-    for (int j = 0; j < 4; ++j) {
-      int li = i * 4 + j;
-      if (this->is_link_valid(li)) {
-        tin_links[size] = li;
-        tin_nodes[size] = i + this->neighbourer[this->linkdir[li]];
-        tin_arr[size] = datat[tin_nodes[size]];
-        ++size;
-      }
-      int oli = (i + this->reruobhgien[this->ridknil[li]]) * 4 + j;
-      if (this->is_link_valid(oli)) {
-        tin_links[size] = oli;
-        tin_nodes[size] = i + this->reruobhgien[this->ridknil[li]];
-        ;
-        tin_arr[size] = datat[tin_nodes[size]];
-        ++size;
-      }
-    }
-    return size;
-  }
-
-  int get_receivers_idx_links(int i, std::array<int, 8> &tin) {
-    int size = 0;
-
-    for (int j = 0; j < 4; ++j) {
-      int li = i * 4 + j;
-      if (this->is_link_valid(li) && this->is_link_normal(li)) {
-        tin[size] = li;
-        ++size;
-      }
-      int oli = (i + this->reruobhgien[this->ridknil[li]]) * 4 + j;
-      if (this->is_link_valid(oli) && !this->is_link_normal(oli)) {
-        tin[size] = oli;
-        ++size;
-      }
-    }
-    return size;
-  }
-
-  int get_donors_idx_links(int i, std::array<int, 8> &tin) {
-    int size = 0;
-
-    for (int j = 0; j < 4; ++j) {
-      int li = i * 4 + j;
-      if (this->is_link_valid(li) && !this->is_link_normal(li)) {
-        tin[size] = li;
-        ++size;
-      }
-      int oli = (i + this->reruobhgien[this->ridknil[li]]) * 4 + j;
-      if (this->is_link_valid(oli) && this->is_link_normal(oli)) {
-        tin[size] = oli;
-        ++size;
-      }
-    }
-    return size;
-  }
-
-  int get_neighbour_idx(int i, std::array<int, 8> &tin) {
-    int size = 0;
-
-    for (int j = 0; j < 4; ++j) {
-      int li = i * 4 + j;
-      if (this->is_link_valid(li)) {
-        tin[size] = i + this->neighbourer[this->linkdir[li]];
-        ++size;
-      }
-      // else
-      // 	std::cout << "nope:" << li << "|";
+  // void fill_linknodes()
+  // {
+  // 	bool peridic = false;
+  // 	for(int i=0; i<this->nnodes; ++i)
+  // 	{
 
-      int oli = (i + this->reruobhgien[this->ridknil[li]]) * 4 + j;
-      if (this->is_link_valid(oli)) {
-        tin[size] = i + this->reruobhgien[this->ridknil[li]];
-        ;
-        ++size;
-      }
-      // else
-      // 	std::cout << "epon:" << li << "|";
-    }
-    return size;
-  }
+  // 		if(this->boundaries.is_periodic(i))
+  // 			peridic = true;
 
-  int get_n_potential_receivers(int i) {
-    int size = 0;
+  // 		bool NDT = this->boundaries.can_create_link(i);
+  // 		bool i_forcing = this->boundaries.forcing_io(i);
 
-    for (int j = 0; j < 4; ++j) {
-      int li = i * 4 + j;
-      if (this->is_link_valid(li)) {
-        int on = i + this->neighbourer[this->linkdir[li]];
-        if (this->boundaries.can_receive(on) || this->boundaries.can_give(on))
-          ++size;
-      }
-      // else
-      // 	std::cout << "nope:" << li << "|";
+  // 		int o = this->get_right_idx(i);
+  // 		bool linkvalid = (NDT &&
+  // this->is_in_bound_and_can_create_link(o)); 		bool
+  // both_same_forcing
+  // =
+  // i_forcing && this->boundaries.forcing_io(o);
+  // if(both_same_forcing
+  // &&
+  // ((this->boundaries.force_giving(o) && this->boundaries.force_giving(i)) ||
+  // 					 (this->boundaries.force_receiving(o) &&
+  // this->boundaries.force_receiving(i)))) 			linkvalid =
+  // false; 		this->linknodes[i*8] = (linkvalid) ? i:-1;
+  // this->linknodes[i*8 + 1] = (linkvalid) ? o:-1;
+
+  // 		o = this->get_bottomright_idx(i);
+  // 		linkvalid = (NDT &&  this->is_in_bound_and_can_create_link(o));
+  // 		both_same_forcing = i_forcing && this->boundaries.forcing_io(o);
+  // 		if(both_same_forcing && ((this->boundaries.force_giving(o) &&
+  // this->boundaries.force_giving(i)) ||
+  // (this->boundaries.force_receiving(o)
+  // && this->boundaries.force_receiving(i)))) 			linkvalid =
+  // false; 		this->linknodes[i*8 + 2] = (linkvalid) ? i:-1;
+  // this->linknodes[i*8 + 3] = (linkvalid) ? o:-1;
+
+  // 		o = this->get_bottom_idx(i);
+  // 		linkvalid = (NDT &&  this->is_in_bound_and_can_create_link(o));
+  // 		both_same_forcing = i_forcing && this->boundaries.forcing_io(o);
+  // 		if(both_same_forcing && ((this->boundaries.force_giving(o) &&
+  // this->boundaries.force_giving(i)) ||
+  // (this->boundaries.force_receiving(o)
+  // && this->boundaries.force_receiving(i)))) 			linkvalid =
+  // false; 		this->linknodes[i*8 + 4] = (linkvalid) ? i:-1;
+  // this->linknodes[i*8 + 5] = (linkvalid) ? o:-1;
+
+  // 		o = this->get_bottomleft_idx(i);
+  // 		linkvalid = (NDT &&  this->is_in_bound_and_can_create_link(o));
+  // 		both_same_forcing = i_forcing && this->boundaries.forcing_io(o);
+  // 		if(both_same_forcing && ((this->boundaries.force_giving(o) &&
+  // this->boundaries.force_giving(i)) ||
+  // (this->boundaries.force_receiving(o)
+  // && this->boundaries.force_receiving(i)))) 			linkvalid =
+  // false; 		this->linknodes[i*8 + 6] = (linkvalid) ? i:-1;
+  // this->linknodes[i*8 + 7] = (linkvalid) ? o:-1;
 
-      int oli = (i + this->reruobhgien[this->ridknil[li]]) * 4 + j;
-      if (this->is_link_valid(oli)) {
-        int on = i + this->reruobhgien[this->ridknil[li]];
-        ;
-        if (this->boundaries.can_receive(on) || this->boundaries.can_give(on))
-          ++size;
-      }
-      // else
-      // 	std::cout << "epon:" << li << "|";
-    }
-    return size;
-  }
-
-  int get_receivers_idx(int i, std::array<int, 8> &tin) {
-    int size = 0;
-
-    for (int j = 0; j < 4; ++j) {
-      int li = i * 4 + j;
-      if (this->is_link_valid(li) && this->is_link_normal(li)) {
-        tin[size] = i + this->neighbourer[this->linkdir[li]];
-        ++size;
-      }
-      int oli = (i + this->reruobhgien[this->ridknil[li]]) * 4 + j;
-      if (this->is_link_valid(oli) && !this->is_link_normal(oli)) {
-        tin[size] = i + this->reruobhgien[this->ridknil[li]];
-        ++size;
-      }
-    }
-    return size;
-  }
+  // 	}
 
-  int get_receivers_idx_nodes_and_links(int i, std::array<int, 8> &tin,
-                                        std::array<int, 8> &tlin) {
-    int size = 0;
+  // 	if(peridic == false)
+  // 		return;
 
-    for (int j = 0; j < 4; ++j) {
-      int li = i * 4 + j;
-      if (this->is_link_valid(li) && this->is_link_normal(li)) {
-        tin[size] = i + this->neighbourer[this->linkdir[li]];
-        tlin[size] = li;
-        ++size;
-      }
-      int oli = (i + this->reruobhgien[this->ridknil[li]]) * 4 + j;
-      if (this->is_link_valid(oli) && !this->is_link_normal(oli)) {
-        tin[size] = i + this->reruobhgien[this->ridknil[li]];
-        tlin[size] = oli;
-        ++size;
-      }
-    }
-    return size;
-  }
+  // 	// for(int i=0; i<this->nnodes; ++i)
+  // 	// {
 
-  int get_donors_idx(int i, std::array<int, 8> &tin) {
-    int size = 0;
+  // 	// }
 
-    for (int j = 0; j < 4; ++j) {
-      int li = i * 4 + j;
-      if (this->is_link_valid(li) && !this->is_link_normal(li)) {
-        tin[size] = i + this->neighbourer[this->linkdir[li]];
-        ++size;
-      }
-      int oli = (i + this->reruobhgien[this->ridknil[li]]) * 4 + j;
-      if (this->is_link_valid(oli) && this->is_link_normal(oli)) {
-        tin[size] = i + this->reruobhgien[this->ridknil[li]];
-        ++size;
-      }
-    }
-    return size;
-  }
+  // }
 
-  int get_donors_idx_nodes_and_links(int i, std::array<int, 8> &tin,
-                                     std::array<int, 8> &tlin) {
-    int size = 0;
+  void fill_linknodes() {
+    for (int i = 0; i < this->nnodes; ++i) {
+      if (this->is_in_bound_and_can_create_link(i) == false)
+        continue;
 
-    for (int j = 0; j < 4; ++j) {
-      int li = i * 4 + j;
-      if (this->is_link_valid(li) && !this->is_link_normal(li)) {
-        tin[size] = i + this->neighbourer[this->linkdir[li]];
-        tlin[size] = li;
-        ++size;
-      }
-      int oli = (i + this->reruobhgien[this->ridknil[li]]) * 4 + j;
-      if (this->is_link_valid(oli) && this->is_link_normal(oli)) {
-        tin[size] = i + this->reruobhgien[this->ridknil[li]];
-        tlin[size] = oli;
-        ++size;
+      int o = this->get_right_idx(i);
+      this->_fill_linknode(i, o, 0);
+      o = this->get_bottomright_idx(i);
+      this->_fill_linknode(i, o, 2);
+      o = this->get_bottom_idx(i);
+      this->_fill_linknode(i, o, 4);
+      o = this->get_bottomleft_idx(i);
+      this->_fill_linknode(i, o, 6);
+
+      if (this->boundaries.is_periodic(i))
+      // if(true)
+      {
+        o = this->get_left_idx(i);
+        this->_fill_linknode(o, i, 0);
+        o = this->get_topleft_idx(i);
+        this->_fill_linknode(o, i, 2);
+        o = this->get_top_idx(i);
+        this->_fill_linknode(o, i, 4);
+        o = this->get_topright_idx(i);
+        this->_fill_linknode(o, i, 6);
       }
     }
-    return size;
-  }
-
-  void node_idx_from_link_idx(int li, int &banh, int &bao) {
-    if (this->is_link_valid(li) == false) {
-      banh = -1;
-      bao = -1;
-    } else {
-      banh = static_cast<int>(li / 4.);
-      bao = banh + this->neighbourer[this->linkdir[li]];
-    }
   }
 
-  void node_idx_from_link_idx_nocheck(int li, int &banh, int &bao) {
+  void _fill_linknode(int f, int o, int add) {
+
+    // if(this->is_in_bound_and_can_create_link(f) == false ||
+    // 	this->is_in_bound_and_can_create_link(o) == false ||
+    // 	(this->boundaries.force_giving(f) && this->boundaries.force_giving(o))
+    // || 	(this->boundaries.force_receiving(f) &&
+    // this->boundaries.force_receiving(o))
+    // 	)
 
-    banh = static_cast<int>(li / 4.);
-    bao = banh + this->neighbourer[this->linkdir[li]];
-  }
-
-  template <class ti_t> ti_t get_from_links(ti_t i) {
-    if (this->is_link_normal(i))
-      return static_cast<int>(i / 4.);
-    else
-      return static_cast<int>(i / 4.) + this->neighbourer[this->linkdir[i]];
-  }
-
-  template <class ti_t> ti_t get_from_links(ti_t i, int onode) {
-    if (this->is_link_normal(i))
-      return onode;
-    else
-      return onode + this->neighbourer[this->linkdir[i]];
-  }
-
-  template <class ti_t> ti_t get_to_links(ti_t i) {
-    if (this->is_link_inverse(i))
-      return static_cast<int>(i / 4.);
-    else
-      return static_cast<int>(i / 4.) + this->neighbourer[this->linkdir[i]];
-  }
-
-  template <class ti_t> ti_t get_other_node_from_links(ti_t li, ti_t ni) {
-    ti_t no, on;
-    this->node_idx_from_link_idx(li, on, no);
-    if (no == ni)
-      return on;
-    if (on == ni)
-      return no;
-    return -1;
-  }
-
-  void from_to_from_link_index(int li, int &from, int &to) {
-    this->node_idx_from_link_idx(li, from, to);
-    if (from == -1)
+    if (this->is_in_bound_and_can_create_link(f) == false ||
+        this->is_in_bound_and_can_create_link(o) == false)
       return;
 
-    if (this->is_link_normal(li))
+    if (this->linknodes[f * 8 + add] != -1)
       return;
-    else
-      std::swap(from, to);
-  }
-
-  void raw_node_idx_from_link_idx(int li, int &banh, int &bao) {
-
-    int modi = li % 4;
-    banh = static_cast<int>(li / 4.);
-
-    int palu = banh % this->nx;
-
-    if (modi == 0)
-      bao = this->get_raw_right_idx(banh, palu);
-    else if (modi == 1)
-      bao = this->get_raw_bottomright_idx(banh, palu);
-    else if (modi == 2)
-      bao = this->get_raw_bottom_idx(banh, palu);
-    else if (modi == 3)
-      bao = this->get_raw_bottomleft_idx(banh, palu);
-  }
-
-  void raw_node_idx_from_link_idx(int li, int &banh, int &bao, uI_t &dir) {
 
-    int modi = li % 4;
-    banh = static_cast<int>(li / 4.);
-
-    int palu = banh % this->nx;
-
-    if (modi == 0)
-      bao = this->get_raw_right_idx(banh, palu, dir);
-    else if (modi == 1)
-      bao = this->get_raw_bottomright_idx(banh, palu, dir);
-    else if (modi == 2)
-      bao = this->get_raw_bottom_idx(banh, palu, dir);
-    else if (modi == 3)
-      bao = this->get_raw_bottomleft_idx(banh, palu, dir);
-  }
-
-  void precompute_links() {
-
-    // initialising all the links to not_processed
-    uI_t maxu = std::numeric_limits<uI_t>::max();
-
-    this->links = std::vector<uI_t>(this->nnodes * 4, maxu);
-
-    this->linkdir = std::vector<uI_t>(this->nnodes * 4, maxu);
-    this->ridknil = std::vector<uI_t>(this->nnodes * 4, maxu);
-    this->_Sreceivers = std::vector<int>(this->nnodes, -1);
-    for (int i = 0; i < this->nnodes; ++i)
-      this->_Sreceivers[i] = i;
-    this->Sdistance2receivers = std::vector<T>(this->nnodes, -1);
-    this->SS = std::vector<T>(this->nnodes, 0.);
-
-    // int tocheck = 9876;
-    // auto lix = this->get_empty_neighbour<int>();
-    for (int i = 0; i < this->nnodes * 4; ++i) {
-
-      // getting link nodes
-      // std::cout << "Processing " << i << std::endl;
-      int a, b;
-      uI_t dir;
-      this->raw_node_idx_from_link_idx(i, a, b, dir);
-      // uI_t convdir = this->converter[delta];
-      int modi = i % 4;
-      int lib = b * 4 + modi;
-      this->linkdir[i] = dir;
-      this->ridknil[lib] = dir;
-
-      // std::cout << "a:" << a << "and b:" << b << " dir:" << int(dir) <<
-      // std::endl; if (a == 9876) if (b == 1999) std::cout << "a:" << a << "and
-      // b:" << b << " dir:" << int(dir) << " adder:" << this->neighbourer[dir]
-      // << std::endl;
-
-      // checking for permanently non valid link
-      if (this->boundaries.no_data(a) || this->boundaries.no_data(b) ||
-          (this->boundaries.force_giving(a) &&
-           this->boundaries.force_giving(b)) ||
-          (this->boundaries.force_receiving(a) &&
-           this->boundaries.force_receiving(b))) {
-        this->links[i] = 5;
-        continue;
-      }
+    if ((this->boundaries.can_give(f) && this->boundaries.can_receive(o)) ||
+        (this->boundaries.can_give(o) && this->boundaries.can_receive(f))) {
+      this->linknodes[f * 8 + add] = f;
+      this->linknodes[f * 8 + add + 1] = o;
+    }
 
-      // chekcing for forcing links
-      if ((this->boundaries.force_giving(a) ||
-           this->boundaries.force_receiving(b)) &&
-          ((this->is_on_top_row(a) && this->is_on_bottom_row(b)) == false &&
-           (this->is_on_top_row(b) && this->is_on_bottom_row(a)) == false &&
-           (this->is_on_leftest_col(a) && this->is_on_rightest_col(b)) ==
-               false &&
-           (this->is_on_leftest_col(b) && this->is_on_rightest_col(a)) ==
-               false &&
-           (a == 0 && (this->is_on_bottom_row(b) ||
-                       this->is_on_rightest_col(b))) == false &&
-           (b == 0 && (this->is_on_bottom_row(a) ||
-                       this->is_on_rightest_col(a))) == false &&
-           (b == this->nx - 1 && (this->is_on_bottom_row(a) ||
-                                  this->is_on_leftest_col(a))) == false &&
-           (a == this->nx - 1 && (this->is_on_bottom_row(b) ||
-                                  this->is_on_leftest_col(b))) == false &&
-           (a == this->nnodes - this->nx &&
-            (this->is_on_top_row(b) || this->is_on_rightest_col(b))) == false &&
-           (b == this->nnodes - this->nx &&
-            (this->is_on_top_row(a) || this->is_on_rightest_col(a))) == false &&
-           (b == this->nnodes - 1 &&
-            (this->is_on_top_row(a) || this->is_on_leftest_col(a))) == false &&
-           (a == this->nnodes - 1 &&
-            (this->is_on_top_row(b) || this->is_on_leftest_col(b))) == false)
-
-      ) {
-        this->links[i] = 3;
-      }
-
-      else if ((this->boundaries.force_receiving(a) ||
-                this->boundaries.force_giving(b)) &&
-               ((this->is_on_top_row(a) && this->is_on_bottom_row(b)) ==
-                    false &&
-                (this->is_on_top_row(b) && this->is_on_bottom_row(a)) ==
-                    false &&
-                (this->is_on_leftest_col(a) && this->is_on_rightest_col(b)) ==
-                    false &&
-                (this->is_on_leftest_col(b) && this->is_on_rightest_col(a)) ==
-                    false &&
-                (a == 0 && (this->is_on_bottom_row(b) ||
-                            this->is_on_rightest_col(b))) == false &&
-                (b == 0 && (this->is_on_bottom_row(a) ||
-                            this->is_on_rightest_col(a))) == false &&
-                (b == this->nx - 1 && (this->is_on_bottom_row(a) ||
-                                       this->is_on_leftest_col(a))) == false &&
-                (a == this->nx - 1 && (this->is_on_bottom_row(b) ||
-                                       this->is_on_leftest_col(b))) == false &&
-                (a == this->nnodes - this->nx &&
-                 (this->is_on_top_row(b) || this->is_on_rightest_col(b))) ==
-                    false &&
-                (b == this->nnodes - this->nx &&
-                 (this->is_on_top_row(a) || this->is_on_rightest_col(a))) ==
-                    false &&
-                (b == this->nnodes - 1 &&
-                 (this->is_on_top_row(a) || this->is_on_leftest_col(a))) ==
-                    false &&
-                (a == this->nnodes - 1 &&
-                 (this->is_on_top_row(b) || this->is_on_leftest_col(b))) ==
-                    false)) {
-        this->links[i] = 2;
-      } else if (((this->is_on_rightest_col(a) || this->is_on_bottom_row(a) ||
-                   i == 4) &&
-                  (!this->boundaries.is_periodic(a) &&
-                   !this->boundaries.is_periodic(b))) ||
-                 (this->boundaries.is_periodic(a) &&
-                  this->boundaries.forcing_io(b)) ||
-                 (this->boundaries.is_periodic(b) &&
-                  this->boundaries.forcing_io(a))) {
-        this->links[i] = 5;
-      } else {
-        this->links[i] = 0; // is temporary yo
-      }
+    else {
+      this->linknodes[f * 8 + add] = -1;
+      this->linknodes[f * 8 + add + 1] = -1;
     }
+
+    // if( this->boundaries.force_giving(f) && this->boundaries.can_receive(o) )
   }
 
   template <class i_t>
   void get_nodes_from_linkidx_implicit(int li, int &n1, int &n2) {
-    throw std::runtime_error("get_nodes_from_linkidx_implicit::unavailable");
-    // n1 = floor(li/4);
-    // n2 = n1 + fast_mod(li,4);
-
-    // bool nodes_can_create_links = (this->is_in_bound_and_can_create_link(n1)
-    // == false || this->is_in_bound_and_can_create_link(n1) == false); bool
-    // both_forced = false; if(nodes_can_create_links)
-    // {
-    // 	if(this->boundaries.forcing_io(n1) && this->boundaries.forcing_io(n2))
-    // 		both_forced = true;
-    // }
+    n1 = floor(li / 4);
+    n2 = n1 + li % 4;
 
-    // // Then not a valid link
-    // if(nodes_can_create_links || both_forced)
-    // {
-    // 	n1 = -1;
-    // 	n2 = -1;
-    // }
+    bool nodes_can_create_links =
+        (this->is_in_bound_and_can_create_link(n1) == false ||
+         this->is_in_bound_and_can_create_link(n1) == false);
+    bool both_forced = false;
+    if (nodes_can_create_links) {
+      if (this->boundaries.forcing_io(n1) && this->boundaries.forcing_io(n2))
+        both_forced = true;
+    }
+
+    // Then not a valid link
+    if (nodes_can_create_links || both_forced) {
+      n1 = -1;
+      n2 = -1;
+    }
   }
 
   // Function updating ONLY the MFD receivers
   // This is useful in the cases where SFD recs are conditionned by an other
   // mean and cannot be touched (e.g. Cordonnier)
   template <class topo_t> void update_links_MFD_only(topo_t &topography) {
-
     // iterating though every links
-    int node = 0;
-    int incr = 0;
     for (size_t i = 0; i < this->links.size(); ++i) {
+      // Getting hte 2 nodes of the current link
+      int from = this->linknodes[i * 2];
+      int to = this->linknodes[i * 2 + 1];
 
-      // checking if the link is valid
-      if (this->link_needs_processing(i) == false) {
-        ++incr;
-        if (incr == 4) {
-          ++node;
-          incr = 0;
-        }
+      if (from == -1) {
+        this->links[i] = 2;
         continue;
       }
 
-      // Getting hte 2 nodes of the current link
-      // int from,to; this->node_idx_from_link_idx(i,from,to);
-      int from = node;
-      int to = this->neighbourer[this->linkdir[i]] + from;
-      ++incr;
-      if (incr == 4) {
-        ++node;
-        incr = 0;
+      if (this->boundaries.forcing_io(from) ||
+          this->boundaries.forcing_io(to)) {
+
+        if (this->boundaries.force_giving(from) ||
+            this->boundaries.force_receiving(to))
+          this->links[i] = 1;
+        else if (this->boundaries.force_giving(to) ||
+                 this->boundaries.force_receiving(from))
+          this->links[i] = 0;
+        else {
+          throw std::runtime_error("Should not happen 777");
+          this->links[i] = 2;
+        }
+
+        continue;
       }
 
       // by convention true -> topo1 > topo2
       if (topography[from] > topography[to] &&
           this->boundaries.can_give(from) && this->boundaries.can_receive(to))
         this->links[i] = 1;
       else if (this->boundaries.can_give(to) &&
                this->boundaries.can_receive(from))
         this->links[i] = 0;
       // If the configuration cannot allow the link, it is temporarily disabled
       else
-        this->links[i] = 4;
+        this->links[i] = 2;
     }
     // done
   }
 
   // Updates all the link and the SFD info
   template <class topo_t> void update_links(topo_t &topography) {
+    // std::cout << "BUNT" << std::endl;
 
     // am I using a stochastic adjustment for deciding on the steepest slope
     // iterating through all the nodes
-    int node = 0;
-    int incr = 0;
     for (size_t i = 0; i < this->links.size(); ++i) {
 
-      // checking if the link is valid
-      if (this->link_needs_processing(i) == false) {
-        ++incr;
-        if (incr == 4) {
-          ++node;
-          incr = 0;
-        }
+      // Checking the validity of the link
+      if (this->linknodes[i * 2] < 0) {
+        this->links[i] = 2;
         continue;
       }
 
-      // Getting hte 2 nodes of the current link
-      // int from,to; this->node_idx_from_link_idx(i,from,to);
-      int from = node;
-      int to = this->neighbourer[this->linkdir[i]] + from;
-
-      // if(to < 0 || to >= this->nnodes)
-      // {
-      // 	std::cout << "HAPPENS::" << from << "/" << to << " dir:" <<
-      // int(this->linkdir[i]) << std::endl;
-      // 	// std::cout << i << " vs " << node * 4
-      // }
+      // Getting ht etwo nodes of the links
+      int from = this->linknodes[i * 2];
+      int to = this->linknodes[i * 2 + 1];
+
+      // std::cout << std::setprecision(18);
+
+      // if( 808 * this->nx + 733 == from)
+      // 	std::cout << i <<" TESTED NODE from:: " << topography[from] << "
+      // v " << topography[to]  << "||" << (topography[from] > topography[to])
+      // << std::endl; if( 808 * this->nx + 733 == to) 	std::cout << i <<"
+      // TESTED NODE to:: " << topography[to] << " v " << topography[from] <<
+      // "||" << (topography[to] > topography[from]) << std::endl;
+
+      // std::cout << from << "|" << to << "||";
 
       // getting the link infos
       // -> dx
       T dx = this->get_dx_from_links_idx(i);
-
-      ++incr;
-      if (incr == 4) {
-        ++node;
-        incr = 0;
-      }
-
       // -> slope
       T slope = (topography[from] - topography[to]) / dx;
 
-      bool FORCED = this->is_link_forced(i);
+      if (this->boundaries.forcing_io(from) ||
+          this->boundaries.forcing_io(to)) {
 
-      if (FORCED) {
-        slope = this->randu->get();
-        if (this->is_link_inverse(i)) {
-          if (this->SS[to] < slope) {
-            this->_Sreceivers[to] = from;
-            this->Sdistance2receivers[to] = dx;
-            this->SS[to] = slope;
-          }
-        } else if (this->SS[from] < slope) {
-          // saving the Sreceivers info as temporary best choice
-          this->_Sreceivers[from] = to;
-          this->Sdistance2receivers[from] = dx;
-          this->SS[from] = slope;
-        }
-
-        continue;
+        if (this->boundaries.force_giving(from) ||
+            this->boundaries.force_receiving(to))
+          slope = 1 / std::abs(slope);
+
+        else if (this->boundaries.force_giving(to) ||
+                 this->boundaries.force_receiving(from))
+          slope = -1 / std::abs(slope);
       }
 
       if (this->stochastic_slope_on)
         slope *= (this->randu->get() * this->stochastic_slope_coeff) + 1e-6;
 
       // if slope is positive, to is the receiver by convention
       if (slope > 0 && this->boundaries.can_give(from) &&
           this->boundaries.can_receive(to)) {
         // Conventional direction
         this->links[i] = 1;
         // if Steepest Slope is higher than the current recorded one
         if (this->SS[from] < slope) {
           // saving the Sreceivers info as temporary best choice
-          this->_Sreceivers[from] = to;
+          this->Sreceivers[from] = to;
           this->Sdistance2receivers[from] = dx;
           this->SS[from] = slope;
         }
       } else if (this->boundaries.can_give(to) &&
-                 this->boundaries.can_receive(from) && slope < 0) {
+                 this->boundaries.can_receive(from)) {
         // Otherwise the convention is inverted:
         // isrec is falese and to is giving to from
         this->links[i] = 0;
         // NOte that slope is absolute values
         slope = std::abs(slope);
         if (this->SS[to] < slope) {
-          this->_Sreceivers[to] = from;
+          this->Sreceivers[to] = from;
           this->Sdistance2receivers[to] = dx;
           this->SS[to] = slope;
         }
       } else
-        this->links[i] = 4;
+        this->links[i] = 2;
     }
 
     // Finally inverting the Sreceivers into the Sdonors info
     // Required for several routines
-    // this->compute_SF_donors_from_receivers();
     this->compute_SF_donors_from_receivers();
   }
 
   // Fucntion inverting the SFD receivers into donors
   void compute_SF_donors_from_receivers() {
     // Initialising the graph dimesions for the donors
     // All of thenm have the graph dimension
     this->Sdonors = std::vector<int>(this->nnodes * this->nneighbours, -1);
     this->nSdonors = std::vector<int>(this->nnodes, 0);
 
     // iterating through all the nodes
     for (int i = 0; i < this->nnodes; ++i) {
       // SF so rid == i cause there is only 1 rec
-      int trec = this->_Sreceivers[i];
+      int trec = this->Sreceivers[i];
       if (trec == i)
         continue;
 
       // feeding the Sdonors array at rec position with current node and...
       this->Sdonors[trec * this->nneighbours + this->nSdonors[trec]] = i;
       // ... incrementing the number of Sdonors
       this->nSdonors[trec] += 1;
     }
     // done
   }
 
   // Same function than above but without reallocating the memory (can save a
   // bit of time depending on the context)
   void recompute_SF_donors_from_receivers() {
-    if (this->nSdonors.size() == 0) {
-      this->Sdonors = std::vector<int>(this->nnodes * this->nneighbours, -1);
-      this->nSdonors = std::vector<int>(this->nnodes, 0);
-    }
 
     for (int i = 0; i < this->nnodes; ++i) {
-      // for(int j=0; j < this->nneighbours; ++j)
-      // 	this->Sdonors[i * this->nneighbours + j] = -1;
+      for (int j = 0; j < this->nneighbours; ++j)
+        this->Sdonors[i * this->nneighbours + j] = -1;
       this->nSdonors[i] = 0;
     }
 
     for (int i = 0; i < this->nnodes; ++i) {
       // SF so rid == i cause there is only 1 rec
-      int trec = this->_Sreceivers[i];
+      int trec = this->Sreceivers[i];
       if (trec == i)
         continue;
       this->Sdonors[trec * this->nneighbours + this->nSdonors[trec]] = i;
       this->nSdonors[trec] += 1;
     }
   }
 
+  // Helper functions to allocate and reallocate vectors when
+  // computing/recomputing the graph
+  void _allocate_vectors() {
+    this->links =
+        std::vector<std::uint8_t>(int(this->nnodes * this->nneighbours / 2), 2);
+    this->linknodes =
+        std::vector<int>(int(this->nnodes * this->nneighbours), -1);
+    this->Sreceivers = std::vector<int>(this->nnodes, -1);
+    for (int i = 0; i < this->nnodes; ++i)
+      this->Sreceivers[i] = i;
+    this->Sdistance2receivers = std::vector<T>(this->nnodes, -1);
+    this->SS = std::vector<T>(this->nnodes, 0.);
+  }
+
   void _reallocate_vectors() {
     for (int i = 0; i < this->nnodes; ++i) {
-      this->_Sreceivers[i] = i;
+      this->Sreceivers[i] = i;
       this->Sdistance2receivers[i] = 0;
       this->SS[i] = 0;
     }
   }
 
   bool is_in_bound_and_can_create_link(int o) {
     bool linkvalid = (this->is_in_bound(o));
     if (linkvalid)
       linkvalid = this->boundaries.can_create_link(o);
     return linkvalid;
   }
 
-  template <class U = int> std::array<U, 8> get_empty_neighbour() {
-    return std::array<U, 8>();
+  int get_right_idx_links(int i) { return i * 4; }
+  int get_bottomright_idx_links(int i) { return i * 4 + 1; }
+  int get_bottom_idx_links(int i) { return i * 4 + 2; }
+  int get_bottomleft_idx_links(int i) { return i * 4 + 3; }
+  int get_left_idx_links(int i) {
+    int yolo = this->get_left_idx(i);
+    if (yolo >= 0) {
+      return this->get_right_idx_links(yolo);
+    } else {
+      return this->not_a_node;
+    }
+  }
+  int get_topleft_idx_links(int i) {
+    int yolo = this->get_topleft_idx(i);
+    if (yolo >= 0) {
+      return this->get_bottomright_idx_links(yolo);
+    } else {
+      return this->not_a_node;
+    }
+  }
+  int get_top_idx_links(int i) {
+    int yolo = this->get_top_idx(i);
+    if (yolo >= 0) {
+      return this->get_bottom_idx_links(yolo);
+    } else {
+      return this->not_a_node;
+    }
+  }
+  int get_topright_idx_links(int i) {
+    int yolo = this->get_topright_idx(i);
+    if (yolo >= 0) {
+      return this->get_bottomleft_idx_links(yolo);
+    } else {
+      return this->not_a_node;
+    }
+  }
+  int get_right_idx_linknodes(int i) { return 2 * i * 4; }
+  int get_bottomright_idx_linknodes(int i) { return 2 * (i * 4 + 1); }
+  int get_bottom_idx_linknodes(int i) { return 2 * (i * 4 + 2); }
+  int get_bottomleft_idx_linknodes(int i) { return 2 * (i * 4 + 3); }
+  int get_left_idx_linknodes(int i) {
+    int yolo = this->get_left_idx(i);
+    if (yolo >= 0) {
+      return 2 * this->get_right_idx_links(yolo);
+    } else {
+      return this->not_a_node;
+    }
+  }
+  int get_topleft_idx_linknodes(int i) {
+    int yolo = this->get_topleft_idx(i);
+    if (yolo >= 0) {
+      return 2 * this->get_bottomright_idx_links(yolo);
+    } else {
+      return this->not_a_node;
+    }
+  }
+  int get_top_idx_linknodes(int i) {
+    int yolo = this->get_top_idx(i);
+    if (yolo >= 0) {
+      return 2 * this->get_bottom_idx_links(yolo);
+    } else {
+      return this->not_a_node;
+    }
+  }
+  int get_topright_idx_linknodes(int i) {
+    int yolo = this->get_topright_idx(i);
+    if (yolo >= 0) {
+      return 2 * this->get_bottomleft_idx_links(yolo);
+    } else {
+      return this->not_a_node;
+    }
+  }
+
+  std::vector<int> get_empty_neighbour() { return std::vector<int>(8, 0); }
+
+  int get_neighbour_idx(int i, std::vector<int> &out) {
+
+    int n = 0;
+
+    int next = this->get_right_idx(i);
+    if (this->is_in_bound(next)) {
+      if (!this->boundaries.no_data(next)) {
+        out[n] = next;
+        ++n;
+      }
+    }
+    next = this->get_bottomright_idx(i);
+    if (this->is_in_bound(next)) {
+      if (!this->boundaries.no_data(next)) {
+        out[n] = next;
+        ++n;
+      }
+    }
+    next = this->get_bottom_idx(i);
+    if (this->is_in_bound(next)) {
+      if (!this->boundaries.no_data(next)) {
+        out[n] = next;
+        ++n;
+      }
+    }
+    next = this->get_bottomleft_idx(i);
+    if (this->is_in_bound(next)) {
+      if (!this->boundaries.no_data(next)) {
+        out[n] = next;
+        ++n;
+      }
+    }
+    next = this->get_left_idx(i);
+    if (this->is_in_bound(next)) {
+      if (!this->boundaries.no_data(next)) {
+        out[n] = next;
+        ++n;
+      }
+    }
+    next = this->get_topleft_idx(i);
+    if (this->is_in_bound(next)) {
+      if (!this->boundaries.no_data(next)) {
+        out[n] = next;
+        ++n;
+      }
+    }
+    next = this->get_top_idx(i);
+    if (this->is_in_bound(next)) {
+      if (!this->boundaries.no_data(next)) {
+        out[n] = next;
+        ++n;
+      }
+    }
+    next = this->get_topright_idx(i);
+    if (this->is_in_bound(next)) {
+      if (!this->boundaries.no_data(next)) {
+        out[n] = next;
+        ++n;
+      }
+    }
+
+    return n;
+  }
+
+  int get_neighbour_idx_links(int i, std::vector<int> &out) {
+    int n = 0;
+    int next = this->get_right_idx_links(i);
+    if (next >= 0 && next < this->nnodes * 4) {
+      out[n] = next;
+      ++n;
+    }
+    next = this->get_bottomright_idx_links(i);
+    if (next >= 0 && next < this->nnodes * 4) {
+      out[n] = next;
+      ++n;
+    }
+    next = this->get_bottom_idx_links(i);
+    if (next >= 0 && next < this->nnodes * 4) {
+      out[n] = next;
+      ++n;
+    }
+    next = this->get_bottomleft_idx_links(i);
+    if (next >= 0 && next < this->nnodes * 4) {
+      out[n] = next;
+      ++n;
+    }
+    next = this->get_left_idx_links(i);
+    if (next >= 0 && next < this->nnodes * 4) {
+      out[n] = next;
+      ++n;
+    }
+    next = this->get_topleft_idx_links(i);
+    if (next >= 0 && next < this->nnodes * 4) {
+      out[n] = next;
+      ++n;
+    }
+    next = this->get_top_idx_links(i);
+    if (next >= 0 && next < this->nnodes * 4) {
+      out[n] = next;
+      ++n;
+    }
+    next = this->get_topright_idx_links(i);
+    if (next >= 0 && next < this->nnodes * 4) {
+      out[n] = next;
+      ++n;
+    }
+
+    if (this->is_on_dem_edge(i)) {
+    }
+
+    return n;
+  }
+
+  int get_neighbour_idx_linknodes(int i, std::vector<int> &out) {
+    int n = 0;
+    int next = this->get_right_idx_linknodes(i);
+    if (next >= 0 && next < this->nnodes * 8) {
+      out[n] = next;
+      ++n;
+    }
+    next = this->get_bottomright_idx_linknodes(i);
+    if (next >= 0 && next < this->nnodes * 8) {
+      out[n] = next;
+      ++n;
+    }
+    next = this->get_bottom_idx_linknodes(i);
+    if (next >= 0 && next < this->nnodes * 8) {
+      out[n] = next;
+      ++n;
+    }
+    next = this->get_bottomleft_idx_linknodes(i);
+    if (next >= 0 && next < this->nnodes * 8) {
+      out[n] = next;
+      ++n;
+    }
+    next = this->get_left_idx_linknodes(i);
+    if (next >= 0 && next < this->nnodes * 8) {
+      out[n] = next;
+      ++n;
+    }
+    next = this->get_topleft_idx_linknodes(i);
+    if (next >= 0 && next < this->nnodes * 8) {
+      out[n] = next;
+      ++n;
+    }
+    next = this->get_top_idx_linknodes(i);
+    if (next >= 0 && next < this->nnodes * 8) {
+      out[n] = next;
+      ++n;
+    }
+    next = this->get_topright_idx_linknodes(i);
+    if (next >= 0 && next < this->nnodes * 8) {
+      out[n] = next;
+      ++n;
+    }
+    return n;
+  }
+
+  int get_neighbour_idx_distance(int i, std::vector<std::pair<int, T>> &out) {
+    int n = 0;
+    int next = this->get_right_idx(i);
+
+    if (!this->boundaries.no_data(next) && this->is_in_bound(next)) {
+      out[n] = std::make_pair(next, this->dx);
+      ++n;
+    }
+    next = this->get_bottomright_idx(i);
+    if (!this->boundaries.no_data(next) && this->is_in_bound(next)) {
+      out[n] = std::make_pair(next, this->dxy);
+      ++n;
+    }
+    next = this->get_bottom_idx(i);
+    if (!this->boundaries.no_data(next) && this->is_in_bound(next)) {
+      out[n] = std::make_pair(next, this->dy);
+      ++n;
+    }
+    next = this->get_bottomleft_idx(i);
+    if (!this->boundaries.no_data(next) && this->is_in_bound(next)) {
+      out[n] = std::make_pair(next, this->dxy);
+      ++n;
+    }
+    next = this->get_left_idx(i);
+    if (!this->boundaries.no_data(next) && this->is_in_bound(next)) {
+      out[n] = std::make_pair(next, this->dx);
+      ++n;
+    }
+    next = this->get_topleft_idx(i);
+    if (!this->boundaries.no_data(next) && this->is_in_bound(next)) {
+      out[n] = std::make_pair(next, this->dxy);
+      ++n;
+    }
+    next = this->get_top_idx(i);
+    if (!this->boundaries.no_data(next) && this->is_in_bound(next)) {
+      out[n] = std::make_pair(next, this->dy);
+      ++n;
+    }
+    next = this->get_topright_idx(i);
+    if (!this->boundaries.no_data(next) && this->is_in_bound(next)) {
+      out[n] = std::make_pair(next, this->dxy);
+      ++n;
+    }
+
+    return n;
+  }
+
+  int get_neighbour_idx_distance_links(int i,
+                                       std::vector<std::pair<int, T>> &out) {
+    int n = 0;
+    int next = this->get_right_idx_links(i);
+    if (next >= 0 && next < this->nnodes * 4) {
+      out[n] = std::make_pair(next, this->dx);
+      ++n;
+    }
+    next = this->get_bottomright_idx_links(i);
+    if (next >= 0 && next < this->nnodes * 4) {
+      out[n] = std::make_pair(next, this->dxy);
+      ++n;
+    }
+    next = this->get_bottom_idx_links(i);
+    if (next >= 0 && next < this->nnodes * 4) {
+      out[n] = std::make_pair(next, this->dy);
+      ++n;
+    }
+    next = this->get_bottomleft_idx_links(i);
+    if (next >= 0 && next < this->nnodes * 4) {
+      out[n] = std::make_pair(next, this->dxy);
+      ++n;
+    }
+    next = this->get_left_idx_links(i);
+    if (next >= 0 && next < this->nnodes * 4) {
+      out[n] = std::make_pair(next, this->dx);
+      ++n;
+    }
+    next = this->get_topleft_idx_links(i);
+    if (next >= 0 && next < this->nnodes * 4) {
+      out[n] = std::make_pair(next, this->dxy);
+      ++n;
+    }
+    next = this->get_top_idx_links(i);
+    if (next >= 0 && next < this->nnodes * 4) {
+      out[n] = std::make_pair(next, this->dy);
+      ++n;
+    }
+    next = this->get_topright_idx_links(i);
+    if (next >= 0 && next < this->nnodes * 4) {
+      out[n] = std::make_pair(next, this->dxy);
+      ++n;
+    }
+    return n;
+  }
+
+  int get_neighbour_idx_distance_linknodes(
+      int i, std::vector<std::pair<int, T>> &out) {
+    int n = 0;
+    int next = this->get_right_idx_linknodes(i);
+    if (next >= 0 && next < this->nnodes * 8) {
+      out[n] = std::make_pair(next, this->dx);
+      ++n;
+    }
+    next = this->get_bottomright_idx_linknodes(i);
+    if (next >= 0 && next < this->nnodes * 8) {
+      out[n] = std::make_pair(next, this->dxy);
+      ++n;
+    }
+    next = this->get_bottom_idx_linknodes(i);
+    if (next >= 0 && next < this->nnodes * 8) {
+      out[n] = std::make_pair(next, this->dy);
+      ++n;
+    }
+    next = this->get_bottomleft_idx_linknodes(i);
+    if (next >= 0 && next < this->nnodes * 8) {
+      out[n] = std::make_pair(next, this->dxy);
+      ++n;
+    }
+    next = this->get_left_idx_linknodes(i);
+    if (next >= 0 && next < this->nnodes * 8) {
+      out[n] = std::make_pair(next, this->dx);
+      ++n;
+    }
+    next = this->get_topleft_idx_linknodes(i);
+    if (next >= 0 && next < this->nnodes * 8) {
+      out[n] = std::make_pair(next, this->dxy);
+      ++n;
+    }
+    next = this->get_top_idx_linknodes(i);
+    if (next >= 0 && next < this->nnodes * 8) {
+      out[n] = std::make_pair(next, this->dy);
+      ++n;
+    }
+    next = this->get_topright_idx_linknodes(i);
+    if (next >= 0 && next < this->nnodes * 8) {
+      out[n] = std::make_pair(next, this->dxy);
+      ++n;
+    }
+    return n;
   }
 
   // Takes a node index as input and a normalised displacement in the X and Y
   // direction (between -1 and 1) Returns the neighbouring node in the given
   // direction
   template <class ii_t>
   ii_t get_neighbour_idx_from_normalised_dxdy(ii_t node, T normdx, T normdy) {
-    // NEEDS FURTHER CHECKS -> EXPERIMENTATL
     if (normdx >= 0.5) {
       if (normdy <= -0.5)
         return this->get_topright_idx(node);
       else if (normdy <= 0.5)
         return this->get_right_idx(node);
       else
         return this->get_bottomright_idx(node);
@@ -2075,28 +1080,150 @@
       else if (normdy < 0.5)
         return this->get_left_idx(node);
       else
         return this->get_bottomleft_idx(node);
     }
   }
 
+  // get receivers of node i and put them in the recs vector fed in
+  // It returns the number of receivers in the recs vector
+  // THis whole process optimises repeated receiver fetching, by never
+  // reallocating/initialising the vector recs
+  int get_receivers_idx(int i, std::vector<int> &recs) {
+    // getting the related links stroing them temporarily in the rec vec
+    int nli = this->get_neighbour_idx_links(i, recs);
+
+    // going through the linksß
+    // The idx is the idx of insertion in the recs vectors
+    // the idx of insertion is always <= of the index of reading (both receivers
+    // and links-to-assess are stored in the recs vector)
+    int idx = 0;
+    // counter used to keep track of the number of receivers: starts at the
+    // number of links related to the given node and get decremented at each
+    // donor link
+    int newli = nli;
+
+    // Iterating through the links
+    for (int ti = 0; ti < nli; ++ti) {
+      // current link index
+      int li = recs[ti];
+
+      // this link is a rec if the node is the first of the linknode and links
+      // is true
+      if (i == this->linknodes[li * 2] && this->links[li] == 1) {
+        // in which case the receiver of the current node is the +  1
+        recs[idx] = this->linknodes[li * 2 + 1];
+        ++idx;
+      }
+      // OR if the current node is the +1 and the links false
+      else if (this->links[li] == 0 && i == this->linknodes[li * 2 + 1]) {
+        // in which case the receivers is the 0 node
+        recs[idx] = this->linknodes[li * 2];
+        ++idx;
+      } else {
+        // otherwise, it's not a rec and we decrease the newli
+        --newli;
+      }
+    }
+    // recs is changed in place, and we return the number of recs newli
+    return newli;
+  }
+
+  // Getting the id of the receivers in the links array
+  // see get_receivers_idx for full comments about the section
+  int get_receivers_idx_links(int i, std::vector<int> &recs) {
+    // getting the related links
+    int nli = this->get_neighbour_idx_links(i, recs);
+
+    // going through the linksß
+    int idx = 0;
+    int newli = nli;
+
+    for (int ti = 0; ti < nli; ++ti) {
+      // checking the orientation
+      int li = recs[ti];
+      if (i == this->linknodes[li * 2] && this->links[li]) {
+        recs[idx] = li;
+        ++idx;
+      } else if (this->links[li] == 0 && i == this->linknodes[li * 2 + 1]) {
+        recs[idx] = li;
+        ++idx;
+      } else {
+        --newli;
+      }
+    }
+    return newli;
+  }
+
   int get_nth_steepest_donors_of_node(int node, int j) {
     return this->Sdonors[node * this->nneighbours + j];
   }
 
+  // Getting donor indicies
+  // see get_receivers_idx for full comments about the section
+  int get_donors_idx(int i, std::vector<int> &dons) {
+    // getting the related links
+    int nli = this->get_neighbour_idx_links(i, dons);
+
+    // going through the links
+    int idx = 0;
+    int newli = nli;
+
+    for (int ti = 0; ti < nli; ++ti) {
+      // checking the orientation
+      int li = dons[ti];
+      if (i == this->linknodes[li * 2] && this->links[li] == 0) {
+        dons[idx] = this->linknodes[li * 2 + 1];
+        ++idx;
+      } else if (this->links[li] == 1 && i == this->linknodes[li * 2 + 1]) {
+        dons[idx] = this->linknodes[li * 2];
+        ++idx;
+      } else {
+        --newli;
+      }
+    }
+    return newli;
+  }
+
+  // getting links indices of hte donors (in the links array)
+  // see get_receivers_idx for full comments about the section
+  int get_donors_idx_links(int i, std::vector<int> &dons) {
+    // getting the related links
+    int nli = this->get_neighbour_idx_links(i, dons);
+
+    // going through the linksß
+    int idx = 0;
+    int newli = nli;
+
+    for (int ti = 0; ti < nli; ++ti) {
+      // checking the orientation
+      int li = dons[ti];
+      if (i == this->linknodes[li * 2] && this->links[li] == 0) {
+        dons[idx] = li;
+        ++idx;
+      } else if (this->links[li] == 1 && i == this->linknodes[li * 2 + 1]) {
+        dons[idx] = li;
+        ++idx;
+      } else {
+        --newli;
+      }
+    }
+    return newli;
+  }
+
   // Debug function printing to the prompt the single receiver of a node
   // Will probably get deprecated
   std::vector<int> get_rowcol_Sreceivers(int row, int col) {
     int node = this->nodeid_from_row_col(row, col);
     std::vector<int> out_receivers;
     int trow, tcol;
-    this->rowcol_from_node_id(this->_Sreceivers[node], trow, tcol);
+    this->rowcol_from_node_id(this->Sreceivers[node], trow, tcol);
     out_receivers = std::vector<int>{trow, tcol};
 
-    std::cout << "Srec is " << this->_Sreceivers[node] << " node was " << node
+    std::cout << "Srec is " << this->Sreceivers[node] << " node was " << node
               << std::endl;
     return out_receivers;
   }
 
   template <class topo_t> void print_receivers(int i, topo_t &ttopography) {
     std::cout << std::setprecision(12);
     auto topography = format_input<topo_t>(ttopography);
@@ -2121,17 +1248,14 @@
     for (int tr = 0; tr < nn; ++tr) {
       int r = neighbours[tr];
       int row, col;
       this->rowcol_from_node_id(r, row, col);
       std::cout << "Neighbour " << r << " row " << row << " col " << col
                 << " topo " << topography[r] << std::endl;
     }
-
-    std::cout << "And finally Srec is " << this->_Sreceivers[i] << std::endl;
-    ;
   }
 
   // Returns the number of links stored in the graph
   // Note that it comprises some unvalid linked!
   int get_rec_array_size() { return int(this->links.size()); }
 
   /// Takes an array of nnodes size and sum the values at the outlets
@@ -2142,15 +1266,15 @@
   U sum_at_outlets(array_t &tarray, bool include_internal_pits = true) {
     std::cout << "DEPRECATION WARNING::sum_at_outlets::should be moved as a "
                  "standalone algorithm"
               << std::endl;
     auto array = format_input<array_t>(tarray);
     U out = 0;
     for (int i = 0; i < this->nnodes; ++i) {
-      if (this->_Sreceivers[i] == i) {
+      if (this->Sreceivers[i] == i) {
         if (include_internal_pits) {
           out += array[i];
         } else if (this->flow_out_model(i)) {
           out += array[i];
         }
       }
     }
@@ -2163,66 +1287,120 @@
   /// pits, wether they are on purpose or not
   template <class array_t, class out_t>
   out_t keep_only_at_outlets(array_t &tarray,
                              bool include_internal_pits = true) {
     auto array = format_input<array_t>(tarray);
     std::vector<T> out = std::vector<T>(this->nnodes, 0);
     for (int i = 0; i < this->nnodes; ++i) {
-      if (this->_Sreceivers[i] == i) {
+      if (this->Sreceivers[i] == i) {
         if (include_internal_pits)
           out[i] = array[i];
         else if (this->flow_out_model(i))
           out[i] = array[i];
       }
     }
     return format_output<decltype(out), out_t>(out);
   }
 
+  // Checks the validity of a link
+  // Invalid links have a linknode value of -1
+  template <class ti_t> bool is_link_valid(ti_t i) {
+    return (this->links[i] == 2) ? false : true;
+  }
+
   // return true is the node is active: i.e. flow transfer through it
   // reflects the connector version of the function, but adds extra graph
   // specific checks. For example a node with permissive outletting border will
   // be active in the connector sense, but can be inactive in the graph if it
   // has no downstream neighbours.
   template <class ti_t> bool flow_out_model(ti_t node) {
 
     bool con_val = this->boundaries.can_out(node);
-    if (con_val && this->_Sreceivers[node] == int(node)) {
+    if (con_val && this->Sreceivers[node] == int(node))
       return true;
-    }
     return false;
   }
 
   template <class ti_t> bool is_pit(ti_t node) {
 
     bool con_val = this->boundaries.can_out(node);
-    if (!con_val && this->_Sreceivers[node] == int(node))
+    if (!con_val && this->Sreceivers[node] == int(node))
       return true;
     return false;
   }
 
   template <class ti_t> bool flow_out_or_pit(ti_t node) {
-    if (this->_Sreceivers[node] == int(node))
+    if (this->Sreceivers[node] == int(node))
       return true;
     return false;
   }
 
+  // Returns the pair of node making a link, starting from the donor to the
+  // receiver
+  template <class ti_t> std::pair<ti_t, ti_t> get_from_to_links(ti_t i) {
+    if (this->links[i] == 1)
+      return std::make_pair(this->linknodes[i * 2], this->linknodes[i * 2 + 1]);
+    else if (this->links[i] == 0)
+      return std::make_pair(this->linknodes[i * 2 + 1], this->linknodes[i * 2]);
+    else
+      return {-1, -1};
+  }
+
+  template <class ti_t>
+  void get_from_to_links(ti_t i, std::pair<ti_t, ti_t> &fromto) {
+    if (this->links[i] == 1) {
+      fromto.first = this->linknodes[i * 2];
+      fromto.second = this->linknodes[i * 2 + 1];
+    } else if (this->links[i] == 2) {
+      fromto.first = this->linknodes[i * 2 + 1];
+      fromto.second = this->linknodes[i * 2];
+    } else
+      fromto = {-1, -1};
+  }
+
+  template <class ti_t> ti_t get_from_links(ti_t i) {
+    if (this->links[i] == 1)
+      return this->linknodes[i * 2];
+    else if (this->links[i] == 0)
+      return this->linknodes[i * 2 + 1];
+    else
+      return -1;
+  }
+
+  template <class ti_t> ti_t get_to_links(ti_t i) {
+    if (this->links[i] == 0)
+      return this->linknodes[i * 2];
+    else if (this->links[i] == 1)
+      return this->linknodes[i * 2 + 1];
+    else
+      return -1;
+  }
+
+  template <class ti_t> ti_t get_other_node_from_links(ti_t li, ti_t ni) {
+    if (this->linknodes[li * 2 + 1] == ni)
+      return this->linknodes[li * 2];
+    else if (this->linknodes[li * 2] == ni)
+      return this->linknodes[li * 2 + 1];
+    else
+      return -1;
+  }
+
   std::vector<int> get_n_receivers() {
     std::vector<int> nrecs(this->nnodes, 0);
     for (size_t i = 0; i < this->links.size(); ++i) {
       if (this->is_link_valid(i)) {
-
-        auto frto = this->get_from_links(i);
-        ++nrecs[frto];
+        auto frto = this->get_from_to_links(i);
+        ++nrecs[frto.first];
       }
     }
     return nrecs;
   }
 
   template <class out_t> out_t get_SFD_receivers() {
-    return format_output<std::vector<int>, out_t>(this->_Sreceivers);
+    return format_output<std::vector<int>, out_t>(this->Sreceivers);
   }
 
   template <class out_t> out_t get_SFD_dx() {
     return format_output<std::vector<T>, out_t>(this->Sdistance2receivers);
   }
 
   template <class out_t> out_t get_SFD_ndonors() {
@@ -2244,20 +1422,34 @@
 
     return out;
   }
 
   template <class out_t> out_t get_links() { return this->links; }
 
   template <class out_t> out_t get_linknodes_flat() {
-    std::vector<int> out;
-    return format_output<std::vector<int>, out_t>(out);
+    return format_output<std::vector<int>, out_t>(this->linknodes);
   }
 
   template <class out_t> out_t get_linknodes_flat_D4() {
-    std::vector<int> temp(int(this->links.size() / 2), -1);
+    std::vector<int> temp(int(this->linknodes.size() / 2), -1);
+    int j = 0;
+    int counter = -1;
+    for (int i = 0; i < int(this->linknodes.size()); i += 2) {
+      ++counter;
+      if (counter == 0 || counter == 2) {
+        temp[j] = this->linknodes[i];
+        ++j;
+        temp[j] = this->linknodes[i + 1];
+        ++j;
+      }
+
+      if (counter == 3)
+        counter = -1;
+    }
+
     return format_output<std::vector<int>, out_t>(temp);
   }
 
   template <class out_t> out_t get_linkdx_flat_D4() {
     std::vector<T> temp(int(this->links.size() / 2), -1);
     int j = 0;
     int counter = -1;
@@ -2275,33 +1467,34 @@
     }
 
     return format_output<std::vector<T>, out_t>(temp);
   }
 
   template <class out_t> out_t get_linknodes_list() {
     std::vector<std::vector<int>> out(this->links.size());
-    // for(size_t i=0; i<this->links.size();++i)
-    // {
-    // 	out[i] = std::vector<int>{this->linknodes[i*2], this->linknodes[i*2+1]};
-    // }
+    for (size_t i = 0; i < this->links.size(); ++i) {
+      out[i] =
+          std::vector<int>{this->linknodes[i * 2], this->linknodes[i * 2 + 1]};
+    }
     return out;
   }
 
   template <class out_t> out_t get_linknodes_list_oriented() {
     std::vector<std::vector<int>> out(this->links.size());
-    // for(size_t i=0; i<this->links.size();++i)
-    // {
-    // 	out[i] = (this->links[i] >= 1)? std::vector<int>{this->linknodes[i*2],
-    // this->linknodes[i*2+1]} :  std::vector<int>{this->linknodes[i*2 + 1],
-    // this->linknodes[i*2]};
-    // }
+    for (size_t i = 0; i < this->links.size(); ++i) {
+      out[i] = (this->links[i] >= 1)
+                   ? std::vector<int>{this->linknodes[i * 2],
+                                      this->linknodes[i * 2 + 1]}
+                   : std::vector<int>{this->linknodes[i * 2 + 1],
+                                      this->linknodes[i * 2]};
+    }
     return out;
   }
 
-  int get_SFD_receivers_at_node(int i) { return this->_Sreceivers[i]; }
+  int get_SFD_receivers_at_node(int i) { return this->Sreceivers[i]; }
 
   int get_SFD_dx_at_node(int i) { return this->Sdistance2receivers[i]; }
 
   int get_SFD_ndonors_at_node(int i) { return this->nSdonors[i]; }
 
   template <class out_t> out_t get_SFD_donors_at_node(int i) {
     std::vector<int> out(this->nneighbours);
@@ -2338,16 +1531,16 @@
     auto gradient = this->_get_SFD_gradient(topography);
     return format_output<decltype(gradient), out_t>(gradient);
   }
 
   template <class topo_t> std::vector<T> _get_SFD_gradient(topo_t &topography) {
     std::vector<T> gradient(this->nnodes, 0.);
     for (int i = 0; i < this->nnodes; ++i) {
-      if (this->_Sreceivers[i] != i)
-        gradient[i] = (topography[i] - topography[this->_Sreceivers[i]]) /
+      if (this->Sreceivers[i] != i)
+        gradient[i] = (topography[i] - topography[this->Sreceivers[i]]) /
                       this->Sdistance2receivers[i];
     }
     return gradient;
   }
 
   template <class out_t, class topo_t>
   out_t get_links_gradient(topo_t &ttopography, T min_slope) {
@@ -2359,17 +1552,16 @@
   template <class topo_t>
   std::vector<T> _get_links_gradient(topo_t &topography, T min_slope) {
 
     std::vector<T> gradient = std::vector<T>(this->links.size(), 0);
 
     for (size_t i = 0; i < this->links.size(); ++i) {
       if (this->is_link_valid(i)) {
-        int from, to;
-        this->from_to_from_link_index(i, from, to);
-        gradient[i] = std::max((topography[from] - topography[to]) /
+        gradient[i] = std::max((topography[this->linknodes[i * 2]] -
+                                topography[this->linknodes[i * 2 + 1]]) /
                                    this->get_dx_from_links_idx(i),
                                min_slope);
       }
     }
 
     return gradient;
   }
@@ -2385,20 +1577,20 @@
   std::vector<T> _get_MFD_mean_gradient(topo_t &topography) {
 
     std::vector<T> gradient = std::vector<T>(this->nnodes, 0);
     std::vector<int> ngradient = std::vector<int>(this->nnodes, 0);
 
     for (size_t i = 0; i < this->links.size(); ++i) {
       if (this->is_link_valid(i)) {
-        int from, to;
-        this->from_to_from_link_index(i, from, to);
-        T this_gradient = std::abs(topography[from] - topography[to]) /
+        T this_gradient = std::abs(topography[this->linknodes[i * 2] -
+                                              this->linknodes[i * 2 + 1]]) /
                           this->get_dx_from_links_idx(i);
-        gradient[from] += this_gradient;
-        ++ngradient[from];
+        auto frto = this->get_from_to_links(i);
+        gradient[frto.first] += this_gradient;
+        ++ngradient[frto.first];
       }
     }
 
     for (int i = 0; i < this->nnodes; ++i) {
       if (ngradient[i] > 0)
         gradient[i] = gradient[i] / ngradient[i];
     }
@@ -2419,20 +1611,20 @@
                                             topo_t &weights) {
 
     std::vector<T> gradient = std::vector<T>(this->nnodes, 0);
     std::vector<T> wgradient = std::vector<T>(this->nnodes, 0.);
 
     for (size_t i = 0; i < this->links.size(); ++i) {
       if (this->is_link_valid(i)) {
-        int from, to;
-        this->from_to_from_link_index(i, from, to);
-        T this_gradient = std::abs(topography[from] - topography[to]) /
+        T this_gradient = std::abs(topography[this->linknodes[i * 2] -
+                                              this->linknodes[i * 2 + 1]]) /
                           this->get_dx_from_links_idx(i);
-        gradient[from] += this_gradient * weights[i];
-        wgradient[from] += weights[i];
+        auto frto = this->get_from_to_links(i);
+        gradient[frto.first] += this_gradient * weights[i];
+        wgradient[frto.first] += weights[i];
       }
     }
 
     for (int i = 0; i < this->nnodes; ++i) {
       if (wgradient[i] > 0)
         gradient[i] = gradient[i] / wgradient[i];
     }
@@ -2531,15 +1723,15 @@
   //                               /__.-'|_|--|_|
 
   // All the methods related to geometrical conversions
   // ------------------------------------------------
   // WILL NEED SOME WORK HERE DEPENDING ON THE GRAPH ORIENTATION AND ALL
 
   inline void rowcol_from_node_id(int node_index, int &row, int &col) {
-    col = fast_mod(node_index, this->nx);
+    col = node_index % this->nx;
     row = (int)std::floor(node_index / this->nx);
   }
 
   inline int nodeid_from_row_col(int row, int col) {
     return row * this->nx + col;
   }
 
@@ -2558,15 +1750,15 @@
 
   inline void XY_from_rowcol(int row, int col, T &tX, T &tY) {
     tX = this->Xs[col];
     tY = this->Ys[row];
   }
 
   inline T get_X_from_i(int i) {
-    int col = fast_mod(i, this->nx);
+    int col = i % this->nx;
     return this->Xs[col];
   }
 
   inline T get_Y_from_i(int i) {
     int row = (int)std::floor(i / this->nx);
     return this->Ys[row];
   }
@@ -2579,314 +1771,358 @@
   //   Neighbouring METHODS            /         /
   //                                __/ (  | (  |
   //                               /__.-'|_|--|_|
 
   // All the methods related to accessing and calculating neighbours
   // ------------------------------------------------
 
-  // std::vector<Neighbour<int,T> > get_neighbours(int i, bool ignore_nodata =
-  // false)
-  // {
-
-  // 	// preformatting the output
-  // 	std::vector<Neighbour<int,T> > neighbours;
-
-  // 	// Reserving size depending on the flow topology
-  // 	neighbours.reserve(8);
+  std::vector<Neighbour<int, T>> get_neighbours(int i,
+                                                bool ignore_nodata = false) {
 
-  // 	size_t id_oldneighbourer = this->_get_oldneighbourer_id(i);
+    // preformatting the output
+    std::vector<Neighbour<int, T>> neighbours;
 
-  // 	// Now I need to determine the index of the oldneighbourer vector
-  // 	// Which provides adder to determine the neighbours
-  // f(boundary_conditions)
-  // 	// internal node 0
-  // 	// periodic_first_row 1
-  // 	// periodic_last_row 2
-  // 	// periodic_first_col 3
-  // 	// periodic last_col 4
-  // 	// normal_first_row 5
-  // 	// normal_last_row 6
-  // 	// normal_first_col 7
-  // 	// normal_last_col 8
-  // 	// normal_top_left 9
-  // 	// normal_top_right 10
-  // 	// normal_bottom_left 11
-  // 	// normal_bottom_right 12
-  // 	// top_left_periodic 13
-  // 	// top_right_periodic 14
-  // 	// periodic_bottom_left 15
-  // 	// periodic_bottom_right 16
+    // Reserving size depending on the flow topology
+    neighbours.reserve(8);
 
-  // 		this->set_neighbours_in_vector(neighbours, i, id_oldneighbourer,
-  // ignore_nodata);
-
-  // 	// and return it
-  // 	return neighbours;
-  // }
-
-  // // This function is the helper of the neighbouring function: it fills the
-  // neighbours vector with the actul values. void
-  // set_neighbours_in_vector(std::vector<Neighbour<int,T> >& neighbours, int&
-  // i, size_t& id_oldneighbourer, bool ignore_nodata)
-  // {
-  // 	// node index of the current neighbour
-  // 	int tn;
-
-  // 	// If you wonder why I am not iterating with a vector and everything
-  // here, it is for the small perf gain of doing it this way 	tn =
-  // this->oldneighbourer[id_oldneighbourer][1]; 	if(tn !=
-  // this->not_a_node
-  // && (ignore_nodata == false || (ignore_nodata &&
-  // !this->boundaries.no_data(tn))))
-  // neighbours.emplace_back(Neighbour<int, T>(tn + i, this->lengthener[1]));
-  // tn = this->oldneighbourer[id_oldneighbourer][3]; 	if(tn !=
-  // this->not_a_node && (ignore_nodata == false || (ignore_nodata &&
-  // !this->boundaries.no_data(tn))))
-  // neighbours.emplace_back(Neighbour<int, T>(tn + i, this->lengthener[3]));
-  // tn = this->oldneighbourer[id_oldneighbourer][4]; 	if(tn !=
-  // this->not_a_node && (ignore_nodata == false || (ignore_nodata &&
-  // !this->boundaries.no_data(tn))))
-  // neighbours.emplace_back(Neighbour<int, T>(tn + i, this->lengthener[4]));
-  // tn = this->oldneighbourer[id_oldneighbourer][6]; 	if(tn !=
-  // this->not_a_node && (ignore_nodata == false || (ignore_nodata &&
-  // !this->boundaries.no_data(tn))))
-  // neighbours.emplace_back(Neighbour<int, T>(tn + i, this->lengthener[6]));
-  // tn = this->oldneighbourer[id_oldneighbourer][0]; 	if(tn !=
-  // this->not_a_node && (ignore_nodata == false || (ignore_nodata &&
-  // !this->boundaries.no_data(tn))))
-  // neighbours.emplace_back(Neighbour<int, T>(tn + i, this->lengthener[0]));
-  // tn = this->oldneighbourer[id_oldneighbourer][2]; 	if(tn !=
-  // this->not_a_node && (ignore_nodata == false || (ignore_nodata &&
-  // !this->boundaries.no_data(tn))))
-  // neighbours.emplace_back(Neighbour<int, T>(tn + i, this->lengthener[2]));
-  // tn = this->oldneighbourer[id_oldneighbourer][5]; 	if(tn !=
-  // this->not_a_node && (ignore_nodata == false || (ignore_nodata &&
-  // !this->boundaries.no_data(tn))))
-  // neighbours.emplace_back(Neighbour<int, T>(tn + i, this->lengthener[5]));
-  // tn = this->oldneighbourer[id_oldneighbourer][7]; 	if(tn !=
-  // this->not_a_node && (ignore_nodata == false || (ignore_nodata &&
-  // !this->boundaries.no_data(tn))))
-  // neighbours.emplace_back(Neighbour<int, T>(tn + i, this->lengthener[7]));
-
-  // }
+    size_t id_neighbourer = this->_get_neighbourer_id(i);
+
+    // Now I need to determine the index of the neighbourer vector
+    // Which provides adder to determine the neighbours f(boundary_conditions)
+    // internal node 0
+    // periodic_first_row 1
+    // periodic_last_row 2
+    // periodic_first_col 3
+    // periodic last_col 4
+    // normal_first_row 5
+    // normal_last_row 6
+    // normal_first_col 7
+    // normal_last_col 8
+    // normal_top_left 9
+    // normal_top_right 10
+    // normal_bottom_left 11
+    // normal_bottom_right 12
+    // top_left_periodic 13
+    // top_right_periodic 14
+    // periodic_bottom_left 15
+    // periodic_bottom_right 16
+
+    this->set_neighbours_in_vector(neighbours, i, id_neighbourer,
+                                   ignore_nodata);
+
+    // and return it
+    return neighbours;
+  }
+
+  // This function is the helper of the neighbouring function: it fills the
+  // neighbours vector with the actul values.
+  void set_neighbours_in_vector(std::vector<Neighbour<int, T>> &neighbours,
+                                int &i, size_t &id_neighbourer,
+                                bool ignore_nodata) {
+    // node index of the current neighbour
+    int tn;
+
+    // If you wonder why I am not iterating with a vector and everything here,
+    // it is for the small perf gain of doing it this way
+    tn = this->neighbourer[id_neighbourer][1];
+    if (tn != this->not_a_node &&
+        (ignore_nodata == false ||
+         (ignore_nodata && !this->boundaries.no_data(tn))))
+      neighbours.emplace_back(Neighbour<int, T>(tn + i, this->lengthener[1]));
+    tn = this->neighbourer[id_neighbourer][3];
+    if (tn != this->not_a_node &&
+        (ignore_nodata == false ||
+         (ignore_nodata && !this->boundaries.no_data(tn))))
+      neighbours.emplace_back(Neighbour<int, T>(tn + i, this->lengthener[3]));
+    tn = this->neighbourer[id_neighbourer][4];
+    if (tn != this->not_a_node &&
+        (ignore_nodata == false ||
+         (ignore_nodata && !this->boundaries.no_data(tn))))
+      neighbours.emplace_back(Neighbour<int, T>(tn + i, this->lengthener[4]));
+    tn = this->neighbourer[id_neighbourer][6];
+    if (tn != this->not_a_node &&
+        (ignore_nodata == false ||
+         (ignore_nodata && !this->boundaries.no_data(tn))))
+      neighbours.emplace_back(Neighbour<int, T>(tn + i, this->lengthener[6]));
+    tn = this->neighbourer[id_neighbourer][0];
+    if (tn != this->not_a_node &&
+        (ignore_nodata == false ||
+         (ignore_nodata && !this->boundaries.no_data(tn))))
+      neighbours.emplace_back(Neighbour<int, T>(tn + i, this->lengthener[0]));
+    tn = this->neighbourer[id_neighbourer][2];
+    if (tn != this->not_a_node &&
+        (ignore_nodata == false ||
+         (ignore_nodata && !this->boundaries.no_data(tn))))
+      neighbours.emplace_back(Neighbour<int, T>(tn + i, this->lengthener[2]));
+    tn = this->neighbourer[id_neighbourer][5];
+    if (tn != this->not_a_node &&
+        (ignore_nodata == false ||
+         (ignore_nodata && !this->boundaries.no_data(tn))))
+      neighbours.emplace_back(Neighbour<int, T>(tn + i, this->lengthener[5]));
+    tn = this->neighbourer[id_neighbourer][7];
+    if (tn != this->not_a_node &&
+        (ignore_nodata == false ||
+         (ignore_nodata && !this->boundaries.no_data(tn))))
+      neighbours.emplace_back(Neighbour<int, T>(tn + i, this->lengthener[7]));
+  }
 
-  inline size_t _get_oldneighbourer_id(int i) {
+  inline size_t _get_neighbourer_id(int i) {
 
-    size_t id_oldneighbourer = -1;
-    // internal node, so oldneighbourer is 0
+    size_t id_neighbourer = -1;
+    // internal node, so neighbourer is 0
     if (this->boundaries.is_normal_node(i))
-      id_oldneighbourer = 0;
+      id_neighbourer = 0;
     else {
       // Case top left corner
       if (i == 0) {
         // Case Periodic
         if (this->boundaries.is_periodic(i))
-          id_oldneighbourer = 13;
+          id_neighbourer = 13;
         // Case Noraml
         else if (this->boundaries.normal_neighbouring_at_boundary(i))
-          id_oldneighbourer = 9;
+          id_neighbourer = 9;
       }
       // Case top right corner
       else if (i == this->nx - 1) {
         // Case Periodic
         if (this->boundaries.is_periodic(i))
-          id_oldneighbourer = 14;
+          id_neighbourer = 14;
         // Case Noraml
         else if (this->boundaries.normal_neighbouring_at_boundary(i))
-          id_oldneighbourer = 10;
+          id_neighbourer = 10;
       }
       // Case bottom left corner
       else if (i == (this->nnodes - this->nx)) {
         // Case Periodic
         if (this->boundaries.is_periodic(i))
-          id_oldneighbourer = 15;
+          id_neighbourer = 15;
         // Case Noraml
         else if (this->boundaries.normal_neighbouring_at_boundary(i))
-          id_oldneighbourer = 11;
+          id_neighbourer = 11;
       }
       // Case bottom right corner
       else if (i == (this->nnodes - 1)) {
         // Case Periodic
         if (this->boundaries.is_periodic(i))
-          id_oldneighbourer = 16;
+          id_neighbourer = 16;
         // Case Noraml
         else if (this->boundaries.normal_neighbouring_at_boundary(i))
-          id_oldneighbourer = 12;
+          id_neighbourer = 12;
       }
       // Cases first row (no corner)
       else if (i < this->nx - 1) {
         // Case periodic
         if (this->boundaries.is_periodic(i))
-          id_oldneighbourer = 1;
+          id_neighbourer = 1;
         // Case normal
         else if (this->boundaries.normal_neighbouring_at_boundary(i))
-          id_oldneighbourer = 5;
+          id_neighbourer = 5;
       }
       // Cases last row (no corner)
       else if (i > (this->ny - 1) * this->nx) {
         // Case periodic
         if (this->boundaries.is_periodic(i))
-          id_oldneighbourer = 2;
+          id_neighbourer = 2;
         // Case normal
         else if (this->boundaries.normal_neighbouring_at_boundary(i))
-          id_oldneighbourer = 6;
+          id_neighbourer = 6;
       }
       // Cases first col (no corner)
       else if (i % this->nx == 0) {
         // Case periodic
         if (this->boundaries.is_periodic(i))
-          id_oldneighbourer = 3;
+          id_neighbourer = 3;
         // Case normal
         else if (this->boundaries.normal_neighbouring_at_boundary(i))
-          id_oldneighbourer = 7;
+          id_neighbourer = 7;
       }
       // Cases last col (no corner)
       else if (i % this->nx == this->nx - 1) {
         // Case periodic
         if (this->boundaries.is_periodic(i))
-          id_oldneighbourer = 4;
+          id_neighbourer = 4;
         // Case normal
         else if (this->boundaries.normal_neighbouring_at_boundary(i))
-          id_oldneighbourer = 8;
+          id_neighbourer = 8;
       } else
-        id_oldneighbourer = 0;
+        id_neighbourer = 0;
     }
 
-    // if(id_oldneighbourer == -1)
+    // if(id_neighbourer == -1)
     // {
     // 	int row,col;
     // 	this->rowcol_from_node_id(i,row,col);
     // 	std::cout << "boundary was " << this->boundary[i] << " i: " << i << "/"
     // << this->nnodes << " row: " << row << " col: " << col << std::endl;
     // throw std::runtime_error("neighbouring issue");
     // }
 
-    return id_oldneighbourer;
+    return id_neighbourer;
   }
 
-  inline size_t _get_oldneighbourer_id_assume_periodic(int i) {
+  inline size_t _get_neighbourer_id_assume_periodic(int i) {
 
-    size_t id_oldneighbourer = -1;
-    // internal node, so oldneighbourer is 0
+    size_t id_neighbourer = -1;
+    // internal node, so neighbourer is 0
     if (this->boundaries.is_normal_node(i))
-      id_oldneighbourer = 0;
+      id_neighbourer = 0;
     else {
       // Case top left corner
       if (i == 0) {
         // Case Periodic
-        id_oldneighbourer = 13;
+        id_neighbourer = 13;
       }
       // Case top right corner
       else if (i == this->nx - 1) {
         // Case Periodic
 
-        id_oldneighbourer = 14;
+        id_neighbourer = 14;
 
       }
       // Case bottom left corner
       else if (i == (this->nnodes - this->nx)) {
 
-        id_oldneighbourer = 15;
+        id_neighbourer = 15;
 
       }
       // Case bottom right corner
       else if (i == (this->nnodes - 1)) {
 
-        id_oldneighbourer = 16;
+        id_neighbourer = 16;
 
       }
       // Cases first row (no corner)
       else if (i < this->nx - 1) {
 
-        id_oldneighbourer = 1;
+        id_neighbourer = 1;
 
       }
       // Cases last row (no corner)
       else if (i > (this->ny - 1) * this->nx) {
 
-        id_oldneighbourer = 2;
+        id_neighbourer = 2;
 
       }
       // Cases first col (no corner)
       else if (i % this->nx == 0) {
 
-        id_oldneighbourer = 3;
+        id_neighbourer = 3;
 
       }
       // Cases last col (no corner)
       else if (i % this->nx == this->nx - 1) {
-        id_oldneighbourer = 4;
+        id_neighbourer = 4;
 
       } else
-        id_oldneighbourer = 0;
+        id_neighbourer = 0;
     }
 
-    // if(id_oldneighbourer == -1)
+    // if(id_neighbourer == -1)
     // {
     // 	int row,col;
     // 	this->rowcol_from_node_id(i,row,col);
     // 	std::cout << "boundary was " << this->boundary[i] << " i: " << i << "/"
     // << this->nnodes << " row: " << row << " col: " << col << std::endl;
     // throw std::runtime_error("neighbouring issue");
     // }
 
-    return id_oldneighbourer;
+    return id_neighbourer;
   }
 
   // D4 single neighbour routines
   Neighbour<int, T> get_left_neighbour(int i) {
-    size_t id_oldneighbourer = this->_get_oldneighbourer_id(i);
-    return Neighbour<int, T>(this->oldneighbourer[id_oldneighbourer][3] + i,
+    size_t id_neighbourer = this->_get_neighbourer_id(i);
+    return Neighbour<int, T>(this->neighbourer[id_neighbourer][3] + i,
                              this->dx);
   }
 
   Neighbour<int, T> get_top_neighbour(int i) {
-    size_t id_oldneighbourer = this->_get_oldneighbourer_id(i);
-    return Neighbour<int, T>(this->oldneighbourer[id_oldneighbourer][1] + i,
+    size_t id_neighbourer = this->_get_neighbourer_id(i);
+    return Neighbour<int, T>(this->neighbourer[id_neighbourer][1] + i,
                              this->dy);
   }
 
   Neighbour<int, T> get_right_neighbour(int i) {
-    size_t id_oldneighbourer = this->_get_oldneighbourer_id(i);
-    return Neighbour<int, T>(this->oldneighbourer[id_oldneighbourer][4] + i,
+    size_t id_neighbourer = this->_get_neighbourer_id(i);
+    return Neighbour<int, T>(this->neighbourer[id_neighbourer][4] + i,
                              this->dx);
   }
 
   Neighbour<int, T> get_bottom_neighbour(int i) {
-    size_t id_oldneighbourer = this->_get_oldneighbourer_id(i);
-    return Neighbour<int, T>(this->oldneighbourer[id_oldneighbourer][6] + i,
+    size_t id_neighbourer = this->_get_neighbourer_id(i);
+    return Neighbour<int, T>(this->neighbourer[id_neighbourer][6] + i,
                              this->dy);
   }
 
   // D8 single neighbour extra routines
   Neighbour<int, T> get_topleft_neighbour(int i) {
-    size_t id_oldneighbourer = this->_get_oldneighbourer_id(i);
-    return Neighbour<int, T>(this->oldneighbourer[id_oldneighbourer][0] + i,
+    size_t id_neighbourer = this->_get_neighbourer_id(i);
+    return Neighbour<int, T>(this->neighbourer[id_neighbourer][0] + i,
                              this->dxy);
   }
 
   Neighbour<int, T> get_topright_neighbour(int i) {
-    size_t id_oldneighbourer = this->_get_oldneighbourer_id(i);
-    return Neighbour<int, T>(this->oldneighbourer[id_oldneighbourer][2] + i,
+    size_t id_neighbourer = this->_get_neighbourer_id(i);
+    return Neighbour<int, T>(this->neighbourer[id_neighbourer][2] + i,
                              this->dxy);
   }
 
   Neighbour<int, T> get_bottomleft_neighbour(int i) {
-    size_t id_oldneighbourer = this->_get_oldneighbourer_id(i);
-    return Neighbour<int, T>(this->oldneighbourer[id_oldneighbourer][5] + i,
+    size_t id_neighbourer = this->_get_neighbourer_id(i);
+    return Neighbour<int, T>(this->neighbourer[id_neighbourer][5] + i,
                              this->dxy);
   }
 
   Neighbour<int, T> get_bottomright_neighbour(int i) {
-    size_t id_oldneighbourer = this->_get_oldneighbourer_id(i);
-    return Neighbour<int, T>(this->oldneighbourer[id_oldneighbourer][7] + i,
+    size_t id_neighbourer = this->_get_neighbourer_id(i);
+    return Neighbour<int, T>(this->neighbourer[id_neighbourer][7] + i,
                              this->dxy);
   }
 
   // D4 single neighbour routines
+  int get_left_idx(int i) {
+    size_t id_neighbourer = this->_get_neighbourer_id(i);
+    return this->neighbourer[id_neighbourer][3] + i;
+  }
+
+  int get_top_idx(int i) {
+    size_t id_neighbourer = this->_get_neighbourer_id(i);
+    return this->neighbourer[id_neighbourer][1] + i;
+  }
+
+  int get_right_idx(int i) {
+    size_t id_neighbourer = this->_get_neighbourer_id(i);
+    return this->neighbourer[id_neighbourer][4] + i;
+  }
+
+  int get_bottom_idx(int i) {
+    size_t id_neighbourer = this->_get_neighbourer_id(i);
+    return this->neighbourer[id_neighbourer][6] + i;
+  }
+
+  // D8 single neighbour extra routines
+  int get_topleft_idx(int i) {
+    size_t id_neighbourer = this->_get_neighbourer_id(i);
+    return this->neighbourer[id_neighbourer][0] + i;
+  }
+
+  int get_topright_idx(int i) {
+    size_t id_neighbourer = this->_get_neighbourer_id(i);
+    return this->neighbourer[id_neighbourer][2] + i;
+  }
+
+  int get_bottomleft_idx(int i) {
+    size_t id_neighbourer = this->_get_neighbourer_id(i);
+    return this->neighbourer[id_neighbourer][5] + i;
+  }
+
+  int get_bottomright_idx(int i) {
+    size_t id_neighbourer = this->_get_neighbourer_id(i);
+    return this->neighbourer[id_neighbourer][7] + i;
+  }
 
   std::vector<int> get_D4_neighbours_only_id(int i) {
     std::vector<int> neighs;
     neighs.reserve(4);
     int tn = this->get_left_idx(i);
     if (tn >= 0)
       neighs.emplace_back(tn);
@@ -2932,15 +2168,15 @@
 
   // 	return neighs;
   // }
 
   // Some of my algorithm are adapted from richdem and require iterating through
   // neighbours the way they do starting from left and going clockwise around
   // the node
-  int get_neighbours_idx_richdemlike(int i, std::array<int, 8> &neighs) {
+  int get_neighbours_idx_richdemlike(int i, std::vector<int> &neighs) {
     int j = 0;
     neighs[j] = (this->get_left_idx(i));
     ++j;
     neighs[j] = (this->get_topleft_idx(i));
     ++j;
     neighs[j] = (this->get_top_idx(i));
     ++j;
@@ -2993,23 +2229,17 @@
   // 		return true;
   // 	return false;
   // }
 
   // Returns true if the node is on the dem edge
   // (i.e. one of the 4 lines)
   bool is_on_dem_edge(int i) {
-    if (this->is_on_top_row(i))
-      return true;
-    else if (this->is_on_bottom_row(i))
+    if (this->is_on_top_row(i) || this->is_on_bottom_row(i) ||
+        this->is_on_leftest_col(i) || this->is_on_rightest_col(i))
       return true;
-    else if (this->is_on_leftest_col(i))
-      return true;
-    else if (this->is_on_rightest_col(i))
-      return true;
-
     return false;
   }
 
   bool is_on_top_row(int i) {
     if (i < this->nx)
       return true;
     return false;
@@ -3019,22 +2249,22 @@
     if (i >= this->nnodes - this->nx)
       return true;
     else
       return false;
   }
 
   bool is_on_leftest_col(int i) {
-    if (fast_mod(i, this->nx) == 0)
+    if (i % this->nx == 0)
       return true;
     else
       return false;
   }
 
   bool is_on_rightest_col(int i) {
-    if (fast_mod(i, this->nx) == this->nx - 1)
+    if (i % this->nx == this->nx - 1)
       return true;
     else
       return false;
   }
 
   void print_dim() {
     std::cout << "nx:" << this->nx << std::endl;
@@ -3114,75 +2344,39 @@
   // varying cellarea
   template <class i_t> T get_area_at_node(i_t i) { return this->cellarea; }
 
   // template<>
   // void fill_neighbour_matrices()
 
   template <class i_t> T get_dx_from_links_idx(i_t i) {
-    int modi = i % 4;
-    if (modi == 0)
+    if (i % 4 == 0)
       return this->dx;
-    else if (modi == 1)
+    else if (i % 4 == 1)
       return this->dxy;
-    else if (modi == 2)
+    else if (i % 4 == 2)
       return this->dy;
-    else if (modi == 3)
+    else if (i % 4 == 3)
       return this->dxy;
     else
       return this->dx;
   }
 
   template <class i_t> T get_traverse_dx_from_links_idx(i_t i) {
-    if (fast_mod(i, 4) == 0)
+    if (i % 4 == 0)
       return this->dy;
-    else if (fast_mod(i, 4) == 1)
+    else if (i % 4 == 1)
       return this->dxy;
-    else if (fast_mod(i, 4) == 2)
+    else if (i % 4 == 2)
       return this->dx;
-    else if (fast_mod(i, 4) == 3)
+    else if (i % 4 == 3)
       return this->dxy;
     else
       return this->dy;
   }
 
-  template <class i_t>
-  void get_dxdy_from_links_idx(i_t i, i_t node, std::pair<T, T> &dxdy,
-                               bool unit = false) {
-    int modi = i % 4;
-    // auto sqrt2 = std::sqrt(2.);
-
-    T tdx = this->dx;
-    T tdy = this->dy;
-
-    if (unit) {
-      T normdxdy = std::max(tdx, tdy);
-      tdx /= normdxdy;
-      tdy /= normdxdy;
-    }
-
-    if (modi == 0) {
-      dxdy.first = tdx;
-      dxdy.second = 0.;
-    } else if (modi == 1) {
-      dxdy.first = tdx;
-      dxdy.second = -tdy;
-    } else if (modi == 2) {
-      dxdy.first = 0.;
-      dxdy.second = -tdy;
-    } else if (modi == 3) {
-      dxdy.first = -tdx;
-      dxdy.second = -tdy;
-    }
-
-    if (node != static_cast<int>(i / 4.)) {
-      dxdy.first = -1 * dxdy.first;
-      dxdy.second = -1 * dxdy.second;
-    }
-  }
-
   // return the orthogonal node from a pair of node / link indices
   template <class i_t>
   std::pair<i_t, i_t> get_orthogonal_nodes(i_t node_from, i_t node_to) {
 
     if (node_to == this->get_top_idx(node_from))
       return {this->get_left_idx(node_from), this->get_right_idx(node_from)};
     if (node_to == this->get_topright_idx(node_from))
@@ -3221,42 +2415,41 @@
     // }
   }
 
   template <class i_t, class ii_t>
   std::pair<T, T> get_directed_dxdy_from_links_idx(i_t li, ii_t original_node,
                                                    ii_t n1, ii_t n2) {
     int C_C = (original_node == n1) ? 1 : -1;
-    if (fast_mod(li, 4) == 0)
+    if (li % 4 == 0)
       return std::make_pair(C_C * this->dx, C_C * 0.);
-    else if (fast_mod(li, 4) == 1)
+    else if (li % 4 == 1)
       return std::make_pair(C_C * this->dx, C_C * this->dy);
-    else if (fast_mod(li, 4) == 2)
+    else if (li % 4 == 2)
       return std::make_pair(C_C * 0., C_C * this->dy);
-    else if (fast_mod(li, 4) == 3)
+    else if (li % 4 == 3)
       return std::make_pair(-1 * C_C * this->dx, C_C * this->dy);
     else
       return std::make_pair(C_C * this->dx, C_C * 0.);
   }
 
   template <class i_t, class ii_t>
   std::pair<T, T> get_dxdy_from_links_idx(i_t li) {
-    if (fast_mod(li, 4) == 0)
+    if (li % 4 == 0)
       return std::make_pair(this->dx, 0.);
-    else if (fast_mod(li, 4) == 1)
+    else if (li % 4 == 1)
       return std::make_pair(this->dx, this->dy);
-    else if (fast_mod(li, 4) == 2)
+    else if (li % 4 == 2)
       return std::make_pair(0., this->dy);
-    else if (fast_mod(li, 4) == 3)
+    else if (li % 4 == 3)
       return std::make_pair(this->dx, this->dy);
     else
       return std::make_pair(this->dx, 0.);
   }
 
   template <class i_t> T get_dx_from_linknodes_idx(i_t i) {
-    throw std::runtime_error("DEPRECATED");
     int j = std::floor(i / 2);
     return this->get_dx_from_links_idx(j);
   }
 
   T get_travers_dy_from_dx(T tdx) {
     if (tdx == this->dx)
       return this->dy;
@@ -3283,14 +2476,194 @@
     else if (delta == this->nx - 1)
       return n1 * 4 + 3;
     else
       throw std::runtime_error(
           "Fatal error in DAGGER::D8connector::linkidx_from_nodes");
   }
 
+  std::vector<int> get_ilinknodes_from_node_v1(int i) {
+    std::vector<int> out;
+    out.reserve(8);
+    int tn = this->get_right_idx_links(i);
+    if (tn > 0 && tn < this->nnodes * 4)
+      out.emplace_back(tn);
+    tn = this->get_bottomright_idx_links(i);
+    if (tn > 0 && tn < this->nnodes * 4)
+      out.emplace_back(tn);
+    tn = this->get_bottom_idx_links(i);
+    if (tn > 0 && tn < this->nnodes * 4)
+      out.emplace_back(tn);
+    tn = this->get_bottomleft_idx_links(i);
+    if (tn > 0 && tn < this->nnodes * 4)
+      out.emplace_back(tn);
+    tn = this->get_left_idx_links(i);
+    if (tn > 0 && tn < this->nnodes * 4)
+      out.emplace_back(tn);
+    tn = this->get_topleft_idx_links(i);
+    if (tn > 0 && tn < this->nnodes * 4)
+      out.emplace_back(tn);
+    tn = this->get_top_idx_links(i);
+    if (tn > 0 && tn < this->nnodes * 4)
+      out.emplace_back(tn);
+    tn = this->get_topright_idx_links(i);
+    if (tn > 0 && tn < this->nnodes * 4)
+      out.emplace_back(tn);
+    return out;
+  }
+
+  std::vector<std::pair<int, bool>> get_ilinknodes_from_nodev2(int i) {
+    std::vector<std::pair<int, bool>> out;
+    out.reserve(8);
+
+    if (!this->boundaries.normal_neighbouring_at_boundary(i) &&
+        !this->boundaries.is_normal_node(i)) {
+      int tn = this->get_right_idx_links(i);
+      bool val = false;
+      if (tn > 0 && tn < this->nnodes * 4)
+        val = true;
+      out.emplace_back(std::make_pair(tn, val));
+      tn = this->get_bottomright_idx_links(i);
+      if (tn > 0 && tn < this->nnodes * 4)
+        val = true;
+      out.emplace_back(std::make_pair(tn, val));
+      tn = this->get_bottom_idx_links(i);
+      if (tn > 0 && tn < this->nnodes * 4)
+        val = true;
+      out.emplace_back(std::make_pair(tn, val));
+      tn = this->get_bottomleft_idx_links(i);
+      if (tn > 0 && tn < this->nnodes * 4)
+        val = true;
+      out.emplace_back(std::make_pair(tn, val));
+      tn = this->get_left_idx_links(i);
+      if (tn > 0 && tn < this->nnodes * 4)
+        val = true;
+      out.emplace_back(std::make_pair(tn, val));
+      tn = this->get_topleft_idx_links(i);
+      if (tn > 0 && tn < this->nnodes * 4)
+        val = true;
+      out.emplace_back(std::make_pair(tn, val));
+      tn = this->get_top_idx_links(i);
+      if (tn > 0 && tn < this->nnodes * 4)
+        val = true;
+      out.emplace_back(std::make_pair(tn, val));
+      tn = this->get_topright_idx_links(i);
+      if (tn > 0 && tn < this->nnodes * 4)
+        val = true;
+      out.emplace_back(std::make_pair(tn, val));
+    } else
+      out = {std::make_pair(this->get_right_idx_links(i), true),
+             std::make_pair(this->get_bottomright_idx_links(i), true),
+             std::make_pair(this->get_bottom_idx_links(i), true),
+             std::make_pair(this->get_bottomleft_idx_links(i), true),
+             std::make_pair(this->get_left_idx_links(i), true),
+             std::make_pair(this->get_topleft_idx_links(i), true),
+             std::make_pair(this->get_top_idx_links(i), true),
+             std::make_pair(this->get_topright_idx_links(i), true)};
+
+    return out;
+  }
+
+  void get_ilinknodes_from_nodev3(int i,
+                                  std::vector<std::pair<int, bool>> &out) {
+
+    int tn = this->get_right_idx_links(i);
+    bool val = false;
+    if (tn > 0 && tn < this->nnodes * 4)
+      val = true;
+    out[0].first = tn;
+    out[0].second = val;
+    tn = this->get_bottomright_idx_links(i);
+    val = false;
+    if (tn > 0 && tn < this->nnodes * 4)
+      val = true;
+    out[1].first = tn;
+    out[1].second = val;
+    tn = this->get_bottom_idx_links(i);
+    val = false;
+    if (tn > 0 && tn < this->nnodes * 4)
+      val = true;
+    out[2].first = tn;
+    out[2].second = val;
+    tn = this->get_bottomleft_idx_links(i);
+    val = false;
+    if (tn > 0 && tn < this->nnodes * 4)
+      val = true;
+    out[3].first = tn;
+    out[3].second = val;
+    tn = this->get_left_idx_links(i);
+    val = false;
+    if (tn > 0 && tn < this->nnodes * 4)
+      val = true;
+    out[4].first = tn;
+    out[4].second = val;
+    tn = this->get_topleft_idx_links(i);
+    val = false;
+    if (tn > 0 && tn < this->nnodes * 4)
+      val = true;
+    out[5].first = tn;
+    out[5].second = val;
+    tn = this->get_top_idx_links(i);
+    val = false;
+    if (tn > 0 && tn < this->nnodes * 4)
+      val = true;
+    out[6].first = tn;
+    out[6].second = val;
+    tn = this->get_topright_idx_links(i);
+    val = false;
+    if (tn > 0 && tn < this->nnodes * 4)
+      val = true;
+    out[7].first = tn;
+    out[7].second = val;
+  }
+
+  int get_ilinknodes_from_node(int i, std::vector<int> &out) {
+    int nn = 0;
+    int tn = this->get_right_idx_links(i);
+    if (tn > 0 && tn < this->nnodes * 4) {
+      out[nn] = tn;
+      ++nn;
+    }
+    tn = this->get_bottomright_idx_links(i);
+    if (tn > 0 && tn < this->nnodes * 4) {
+      out[nn] = tn;
+      ++nn;
+    }
+    tn = this->get_bottom_idx_links(i);
+    if (tn > 0 && tn < this->nnodes * 4) {
+      out[nn] = tn;
+      ++nn;
+    }
+    tn = this->get_bottomleft_idx_links(i);
+    if (tn > 0 && tn < this->nnodes * 4) {
+      out[nn] = tn;
+      ++nn;
+    }
+    tn = this->get_left_idx_links(i);
+    if (tn > 0 && tn < this->nnodes * 4) {
+      out[nn] = tn;
+      ++nn;
+    }
+    tn = this->get_topleft_idx_links(i);
+    if (tn > 0 && tn < this->nnodes * 4) {
+      out[nn] = tn;
+      ++nn;
+    }
+    tn = this->get_top_idx_links(i);
+    if (tn > 0 && tn < this->nnodes * 4) {
+      out[nn] = tn;
+      ++nn;
+    }
+    tn = this->get_topright_idx_links(i);
+    if (tn > 0 && tn < this->nnodes * 4) {
+      out[nn] = tn;
+      ++nn;
+    }
+    return nn;
+  }
+
   // returns a 1D bool array, false where no data
   std::vector<bool> get_mask_array() {
     std::vector<bool> mask(this->nnodes, true);
     for (int i = 0; i < this->nnodes; ++i) {
       if (this->boundaries.no_data(i))
         mask[i] = false;
     }
@@ -3302,74 +2675,14 @@
     for (int i = 0; i < this->nnodes; ++i) {
       if (this->boundaries.can_out(i))
         array[i] = val;
     }
   }
 
   int get_nneighbours() { return 8; }
-
-  void debug_print_neighbours(int i) {
-    std::cout << "neighbours of " << i << " -> ";
-    auto neigh = this->get_empty_neighbour();
-    int nn = this->get_neighbour_idx(i, neigh);
-    for (int j = 0; j < nn; ++j)
-      std::cout << "::" << neigh[j];
-    std::cout << std::endl;
-
-    std::cout << "receivers of " << i << " -> ";
-    neigh = this->get_empty_neighbour();
-    nn = this->get_receivers_idx(i, neigh);
-    for (int j = 0; j < nn; ++j)
-      std::cout << "::" << neigh[j];
-    std::cout << std::endl;
-
-    std::cout << "donors of " << i << " -> ";
-    neigh = this->get_empty_neighbour();
-    nn = this->get_donors_idx(i, neigh);
-    for (int j = 0; j < nn; ++j)
-      std::cout << "::" << neigh[j];
-    std::cout << std::endl;
-
-    std::cout << "neighbours links of " << i << " -> ";
-    neigh = this->get_empty_neighbour();
-    nn = this->get_neighbour_idx_links(i, neigh);
-    for (int j = 0; j < nn; ++j)
-      std::cout << "::" << neigh[j] << "(" << int(this->links[neigh[j]]) << "|"
-                << int(this->linkdir[neigh[j]]) << "|"
-                << int(this->ridknil[neigh[j]]) << ")";
-    std::cout << std::endl;
-  }
-
-  void debug_print_row_col(int i) {
-    int row, col;
-    this->rowcol_from_node_id(i, row, col);
-    std::cout << "row: " << row << " col: " << col;
-  }
-
-  // void debug
-};
-
-template <class Connector_t, class topo_t, class fT>
-void set_BC_to_remove_seas(Connector_t &connector, topo_t &ttopography,
-                           fT sea_level) {
-  auto topography = format_input(ttopography);
-  // # first label the no-data
-  for (int i = 0; i < connector.nnodes; ++i)
-    if (topography[i] < sea_level)
-      connector.boundaries.codes[i] = BC::NO_FLOW;
-
-  auto neighbours = connector.get_empty_neighbour();
-  for (int i = 0; i < connector.nnodes; ++i) {
-    if (connector.boundaries.no_data(i))
-      continue;
-    int nn = connector.get_neighbour_idx(i, neighbours);
-    for (int j = 0; j < nn; ++j)
-      if (connector.boundaries.no_data(neighbours[j]))
-        connector.boundaries.codes[i] = BC::OUT;
-  }
 };
 
 //  DEPRECATED AND MOVED OUTSIDE OF THE CONNECTOR
 // 	template <class topo_t>
 // 	std::vector<double> PriorityFlood(topo_t& ttopography)
 // 	{
 // 		std::random_device rd; // obtain a random number from hardware
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `daggerpy-0.0.5/includes/PerlinNoise.hpp` & `daggerpy-0.0.6/includes/PerlinNoise.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/includes/_D8connector.hpp` & `daggerpy-0.0.6/includes/_D8connector.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/includes/_cordonnier_versatile_2019.hpp` & `daggerpy-0.0.6/includes/_cordonnier_versatile_2019.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/includes/_graph.hpp` & `daggerpy-0.0.6/includes/_graph.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/includes/_old_D8connector.hpp` & `daggerpy-0.0.6/includes/graphflood.hpp`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-//=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=
-#ifndef D8connector_HPP
-#define D8connector_HPP
+#pragma once
 
 // STL imports
 #include <array>
 #include <cmath>
 #include <ctime>
 #include <fstream>
 #include <initializer_list>
-#include <iomanip>
 #include <iostream>
 #include <map>
 #include <numeric>
 #include <queue>
 #include <stack>
 #include <stdlib.h>
 #include <string>
@@ -20,2977 +17,2965 @@
 #include <vector>
 
 // local includes
 // -> General routines and data structures
 #include "utils.hpp"
 // -> Depression solvers
 #include "cordonnier_versatile_2019.hpp"
-
-#include "boundary_conditions.hpp"
+// -> The connector classes
+#include "D8connector.hpp"
 
 // defines all the format_input depnding on the eventual wrapper
+#include "fastflood_recorder.hpp"
 #include "wrap_helper.hpp"
 
 namespace DAGGER {
 
-// Useful namespace for my priority queue
-using PQ_i_d = std::priority_queue<PQ_helper<int, double>,
-                                   std::vector<PQ_helper<int, double>>,
-                                   std::greater<PQ_helper<int, double>>>;
+enum class HYDRO // : std::uint8_t
+{
+  GRAPH_SFD,
+  GRAPH_MFD,
+  GRAPH_HYBRID,
+};
 
-template <class T> class D8connector {
-public:
-  // General informations about the graph
-  // #-> number of nodes (integer and unsized int for loops or list innit).
-  int nnodes = 0;
-  size_t nnodes_t = 0;
-
-  static const int nneighbours = 8;
-  static const size_t nneighbours_t = 8;
-
-  // #-> number of nodes in x direction.
-  int nx = 0;
-  // #-> number of nodes in x direction.
-  int ny = 0;
-  // #-> length in the x direction.
-  T dx;
-  // #-> length in the y direction.
-  T dy;
-  T dxy;
-  T dxmax;
-  T dxmin;
-  // #-> cell area
-  T cellarea;
-  T Xmin;
-  T Ymin;
-  T Xmax;
-  T Ymax;
-  int not_a_node;
-
-  bool stochastic_slope_on = false;
-  T stochastic_slope_coeff = 1.; // (0 -> deactivates)
-  void set_stochaticiy_for_SFD(T val) {
-    if (val <= 0) {
-      this->stochastic_slope_on = false;
-      this->stochastic_slope_coeff = 1.;
-    } else {
-      this->stochastic_slope_on = true;
-      this->stochastic_slope_coeff = val;
-    }
-  }
+enum class MORPHO // : std::uint8_t
+{
+  NONE,
+  TL,
+};
 
-  // DEPRECATED BOUNDARY SYSTEM
-  // // Bearer of values
-  // // #->boundary: index: node index, value: boundary value
-  // // #-->The possible values are:
-  // // #---> -1 = no in, no out, not process, internal or external
-  // // #--->  0 = in, no out, all fluxes leave the system, internal or external
-  // // #--->  1 = "normal" cell, in, out, internal
-  // // #--->  2 = external periodic boundary
-  // // #--->	3 = in, can out but can also give to neighbours
-  // std::vector<int> boundary;
-
-  // NEW BOUNDARY SYSTEM
-  CodeBC boundaries;
-
-  // Helpers for neighbouring operations
-  // -> neighbourer holdsthe indices to loop through for each boundary condition
-  std::vector<std::vector<int>> neighbourer;
-  // -> lengthener is the dx on each directions
-  std::vector<T> lengthener;
-
-  // uint8_t vector for each link indicating its directionality:
-  // - 0 is inverse (linknode 2 --> linknode 1)
-  // - 1 is normal (linknode 1 --> linknode 2)
-  // - 3 is invalid (link index may exist, but is either inexsitant (index is
-  // conserved for speed reason when the link index is calculated from node
-  // index) ) or temporarily invalid due to dynamic boundary conditions The
-  // index itself is calculated from a connector
-  std::vector<std::uint8_t> links;
-
-  // integer vector of 2*links size with the node indices of each link
-  // for example, the nodes of link #42 would be indices 84 and 85
-  std::vector<int> linknodes;
-
-  // Single graph receivers
-  // -> Sreceivers: steepest recervers (nnodes size),
-  // -> number of donors (nnodes size),
-  // -> Steepest donors (nnodes * nneighbours size)
-  // --> Sdonors of node i are located from index i*nneighbours to index
-  // i*nneighbours + nSdonors[i] not included
-  std::vector<int> Sreceivers, nSdonors, Sdonors;
-
-  // Single graph distance to receivers
-  std::vector<T> Sdistance2receivers;
-
-  // Steepest slope
-  std::vector<T> SS;
-
-  // Coordinate stuff
-  // Xs and Ys are vectors of nx and ny size converting row to y and col to X
-  // Extents holds the cxmin,xmax,ymin,ymax (extent is an option in matplotlib
-  // imshow plots)
-  std::vector<T> Xs, Ys, extents;
-
-  std::shared_ptr<easyRand> randu = std::make_shared<easyRand>();
-
-  // Default constructor, empty
-  D8connector(){};
-
-  // construct directly from dimensions
-  D8connector(int nx, int ny, T dx, T dy, T xmin, T ymin) {
-    // initialisation is offset to dedicated function because some languages
-    // like Julia are complicating non default constructor initialisation.
-    this->init_dimensions(nx, ny, dx, dy, xmin, ymin);
-    this->_allocate_vectors();
-    this->fill_linknodes();
-  }
-
-  template <class topo_t> void update_links_from_topo(topo_t &ttopo) {
-    auto topo = format_input(ttopo);
-    this->update_links(topo);
-  }
-
-  // initialise with dimension
-  void init_dimensions(int nx, int ny, T dx, T dy, T xmin, T ymin) {
-    int nnodes = nx * ny;
-    this->set_dimensions(nx, ny, nnodes, dx, dy, xmin, ymin);
-    this->set_default_boundaries("4edges");
-  }
-
-  /// @Description: Initialising the "neighbourer", a data structure managing
-  /// the iterations though the neighbours of a given node Function of boundary
-  /// conditions, one can feed the neighbourer with an indice which returns the
-  /// index to ADD to the node to get its neighbour. The neighbour order is (in
-  /// table referential, be careful if Y axis is inverted) top-left, top,
-  /// top-right, left, right, bottom-left, bottom, bottom-right
-  /// @Authors: B.G.
-  /// @Date: 2021
-  void initialise_neighbourer() {
-    T diag = std::sqrt(std::pow(dx, 2) + std::pow(dy, 2));
-    this->dxy = diag;
-    this->dxmin = std::min(this->dx, this->dy);
-    this->dxmax = std::max(this->dx, this->dy);
-
-    this->lengthener =
-        std::initializer_list<T>{diag, dy, diag, dx, dx, diag, dy, diag};
-    this->neighbourer.clear();
-
-    // these vectors are additioned to the node indice to test the neighbors
-    this->neighbourer.emplace_back(std::initializer_list<int>{
-        -this->nx - 1, -this->nx, -this->nx + 1, -1, 1, this->nx - 1, this->nx,
-        this->nx + 1}); // internal node 0
-    this->neighbourer.emplace_back(std::initializer_list<int>{
-        (this->ny - 1) * this->nx - 1, (this->ny - 1) * this->nx,
-        (this->ny - 1) * this->nx + 1, -1, 1, this->nx - 1, this->nx,
-        this->nx + 1}); // periodic_first_row 1
-    this->neighbourer.emplace_back(std::initializer_list<int>{
-        -this->nx - 1, -this->nx, -this->nx + 1, -1, 1,
-        -(this->ny - 1) * this->nx - 1, -(this->ny - 1) * this->nx,
-        -(this->ny - 1) * this->nx + 1}); // periodic_last_row 2
-    this->neighbourer.emplace_back(std::initializer_list<int>{
-        -1, -this->nx, -this->nx + 1, (this->nx - 1), 1, 2 * this->nx - 1,
-        this->nx, this->nx + 1}); // periodic_first_col 3
-    this->neighbourer.emplace_back(std::initializer_list<int>{
-        -this->nx - 1, -this->nx, -2 * this->nx + 1, -1, -this->nx + 1,
-        this->nx - 1, this->nx, 1}); // periodic last_col 4
-    this->neighbourer.emplace_back(std::initializer_list<int>{
-        this->not_a_node, this->not_a_node, this->not_a_node, -1, 1,
-        this->nx - 1, this->nx, this->nx + 1}); // normal_first_row 5
-    this->neighbourer.emplace_back(std::initializer_list<int>{
-        -this->nx - 1, -this->nx, -this->nx + 1, -1, 1, this->not_a_node,
-        this->not_a_node, this->not_a_node}); // normal_last_row 6
-    this->neighbourer.emplace_back(std::initializer_list<int>{
-        this->not_a_node, -this->nx, -this->nx + 1, this->not_a_node, 1,
-        this->not_a_node, this->nx, this->nx + 1}); // normal_first_col 7
-    this->neighbourer.emplace_back(std::initializer_list<int>{
-        -this->nx - 1, -this->nx, this->not_a_node, -1, this->not_a_node,
-        this->nx - 1, this->nx, this->not_a_node}); // normal_last_col 8
-    this->neighbourer.emplace_back(std::initializer_list<int>{
-        this->not_a_node, this->not_a_node, this->not_a_node, this->not_a_node,
-        1, this->not_a_node, this->nx, this->nx + 1}); // normal_top_left 9
-    this->neighbourer.emplace_back(std::initializer_list<int>{
-        this->not_a_node, this->not_a_node, this->not_a_node, -1,
-        this->not_a_node, this->nx - 1, this->nx,
-        this->not_a_node}); // normal_top_right 10
-    this->neighbourer.emplace_back(std::initializer_list<int>{
-        this->not_a_node, -this->nx, -this->nx + 1, this->not_a_node, 1,
-        this->not_a_node, this->not_a_node,
-        this->not_a_node}); // normal_bottom_left 11
-    this->neighbourer.emplace_back(std::initializer_list<int>{
-        -this->nx - 1, -this->nx, this->not_a_node, -1, this->not_a_node,
-        this->not_a_node, this->not_a_node,
-        this->not_a_node}); // normal_bottom_right 12
-    this->neighbourer.emplace_back(std::initializer_list<int>{
-        this->ny * this->nx - 1, (this->ny - 1) * this->nx,
-        (this->ny - 1) * this->nx + 1, this->nx - 1, 1, 2 * this->nx - 1,
-        this->nx, this->nx + 1}); // top_left_periodic 13
-    this->neighbourer.emplace_back(std::initializer_list<int>{
-        (this->ny - 1) * this->nx - 1, (this->ny - 1) * this->nx,
-        (this->ny - 2) * this->nx + 1, -1, -this->nx + 1, this->nx - 1,
-        this->nx, 1}); // top_right_periodic 14
-    this->neighbourer.emplace_back(std::initializer_list<int>{
-        -1, -this->nx, -this->nx + 1, this->nx - 1, 1,
-        -(this->ny - 2) * this->nx - 1, -(this->ny - 1) * this->nx,
-        -(this->ny - 1) * this->nx + 1}); // periodic_bottom_left 15
-    this->neighbourer.emplace_back(std::initializer_list<int>{
-        -this->nx - 1, -this->nx, -this->nx + 1, -1, 1 - this->nx + 1,
-        -(this->ny - 1) * this->nx - 1, -(this->ny - 1) * this->nx,
-        -(this->ny) * this->nx + 1}); // periodic_bottom_right 16
-  }
-
-  /// @description: Sets the dimension of the graph and initialise the
-  /// neighbourer
-  void set_dimensions(int nx, int ny, int nnodes, T dx, T dy, T xmin, T ymin) {
-    this->nx = nx;
-    this->ny = ny;
-    this->nnodes = nnodes;
-    this->nnodes_t = size_t(nnodes);
-    this->dx = dx;
-    this->dy = dy;
-    this->cellarea = this->dx * this->dy;
-    this->Xmin = xmin;
-    this->Ymin = ymin;
-
-    // Not a node is utilised to detect when a neighbouring operation returns
-    // not a node
-    this->not_a_node = -nx * ny * 2;
-
-    this->initialise_neighbourer();
-
-    // Initialise coordinate stuff
-    this->Xs = std::vector<T>(this->nx);
-    this->Ys = std::vector<T>(this->ny);
-    // this->extents = std::vector<T>(4,0);
-
-    for (int i = 0; i < this->nx; ++i)
-      this->Xs[i] = this->Xmin + this->dx / 2 + i * this->dx;
-    for (int i = this->ny - 1; i >= 0; --i) {
-      this->Ys[i] = this->Ymin + this->dy / 2 + i * this->dy;
-    }
-
-    this->Xmax = this->Xs.back() + this->dx / 2;
-    this->Ymax = this->Ys.back() + this->dy / 2;
-
-    std::reverse(this->Ys.begin(), this->Ys.end());
-
-    this->extents = {this->Xmin, this->Xmin + (this->nx + 1) * this->dx,
-                     this->Ymin, this->Ymin + (this->ny + 1) * this->dy};
-  }
-
-  void set_default_boundaries(std::string bountype) {
-
-    this->boundaries.codes = std::vector<BC>(this->nnodes_t, BC::FLOW);
-
-    if (bountype == "4edges") {
-      for (size_t i = 0; i < this->nnodes_t; ++i) {
-        if (this->is_on_dem_edge(i))
-          this->boundaries.codes[i] = BC::FORCE_OUT;
-      }
-    } else if (bountype == "periodic_EW") {
-      for (int i = 0; i < this->nnodes; ++i) {
-        if (this->is_on_top_row(i) || this->is_on_bottom_row(i))
-          this->boundaries.codes[i] = BC::FORCE_OUT;
-        else if (this->is_on_leftest_col(i) || this->is_on_rightest_col(i))
-          this->boundaries.codes[i] = BC::PERIODIC_BORDER;
-      }
-    } else if (bountype == "periodic_NS") {
-      for (int i = 0; i < this->nnodes; ++i) {
-        if (this->is_on_leftest_col(i) || this->is_on_rightest_col(i))
-          this->boundaries.codes[i] = BC::FORCE_OUT;
-        else if (this->is_on_top_row(i) || this->is_on_bottom_row(i))
-          this->boundaries.codes[i] = BC::PERIODIC_BORDER;
-      }
-    } else {
-      throw std::runtime_error("invalid periodic boundaries");
-    }
+enum class PARAM_KE // : std::uint8_t
+{
+  CONSTANT,
+  VARIABLE,
+  EROSION,
+};
 
-    // Recomputing fillnodes
-    // this->fill_linknodes();
-    this->_allocate_vectors();
-    this->fill_linknodes();
-  }
-
-  // Set all the out boundaries to 3, meaning they can now give to lower
-  // elevation neighbours
-  void set_out_boundaries_to_permissive() {
-    for (auto &v : this->boundaries.codes) {
-      if (v == BC::FORCE_OUT)
-        v = BC::OUT;
-    }
-  }
-
-  template <class bou_t> void set_custom_boundaries(bou_t &tbound) {
-    auto bound = format_input(tbound);
-
-    std::vector<BC> ubound(bound.size(), BC::FLOW);
-    for (int i = 0; i < tbound.size(); ++i)
-      ubound[i] = static_cast<BC>(bound[i]);
-
-    this->boundaries.set_codes(ubound);
-    this->_allocate_vectors();
-    this->fill_linknodes();
-  }
-
-  BC get_boundary_at_node(int i) { return this->boundaries.codes[i]; }
-
-  bool is_in_bound(int i) {
-    return (i >= 0 && i < this->nnodes) ? true : false;
-  }
-
-  // void fill_linknodes()
-  // {
-  // 	bool peridic = false;
-  // 	for(int i=0; i<this->nnodes; ++i)
-  // 	{
-
-  // 		if(this->boundaries.is_periodic(i))
-  // 			peridic = true;
-
-  // 		bool NDT = this->boundaries.can_create_link(i);
-  // 		bool i_forcing = this->boundaries.forcing_io(i);
-
-  // 		int o = this->get_right_idx(i);
-  // 		bool linkvalid = (NDT &&
-  // this->is_in_bound_and_can_create_link(o)); 		bool
-  // both_same_forcing
-  // =
-  // i_forcing && this->boundaries.forcing_io(o);
-  // if(both_same_forcing
-  // &&
-  // ((this->boundaries.force_giving(o) && this->boundaries.force_giving(i)) ||
-  // 					 (this->boundaries.force_receiving(o) &&
-  // this->boundaries.force_receiving(i)))) 			linkvalid =
-  // false; 		this->linknodes[i*8] = (linkvalid) ? i:-1;
-  // this->linknodes[i*8 + 1] = (linkvalid) ? o:-1;
-
-  // 		o = this->get_bottomright_idx(i);
-  // 		linkvalid = (NDT &&  this->is_in_bound_and_can_create_link(o));
-  // 		both_same_forcing = i_forcing && this->boundaries.forcing_io(o);
-  // 		if(both_same_forcing && ((this->boundaries.force_giving(o) &&
-  // this->boundaries.force_giving(i)) ||
-  // (this->boundaries.force_receiving(o)
-  // && this->boundaries.force_receiving(i)))) 			linkvalid =
-  // false; 		this->linknodes[i*8 + 2] = (linkvalid) ? i:-1;
-  // this->linknodes[i*8 + 3] = (linkvalid) ? o:-1;
-
-  // 		o = this->get_bottom_idx(i);
-  // 		linkvalid = (NDT &&  this->is_in_bound_and_can_create_link(o));
-  // 		both_same_forcing = i_forcing && this->boundaries.forcing_io(o);
-  // 		if(both_same_forcing && ((this->boundaries.force_giving(o) &&
-  // this->boundaries.force_giving(i)) ||
-  // (this->boundaries.force_receiving(o)
-  // && this->boundaries.force_receiving(i)))) 			linkvalid =
-  // false; 		this->linknodes[i*8 + 4] = (linkvalid) ? i:-1;
-  // this->linknodes[i*8 + 5] = (linkvalid) ? o:-1;
-
-  // 		o = this->get_bottomleft_idx(i);
-  // 		linkvalid = (NDT &&  this->is_in_bound_and_can_create_link(o));
-  // 		both_same_forcing = i_forcing && this->boundaries.forcing_io(o);
-  // 		if(both_same_forcing && ((this->boundaries.force_giving(o) &&
-  // this->boundaries.force_giving(i)) ||
-  // (this->boundaries.force_receiving(o)
-  // && this->boundaries.force_receiving(i)))) 			linkvalid =
-  // false; 		this->linknodes[i*8 + 6] = (linkvalid) ? i:-1;
-  // this->linknodes[i*8 + 7] = (linkvalid) ? o:-1;
-
-  // 	}
-
-  // 	if(peridic == false)
-  // 		return;
-
-  // 	// for(int i=0; i<this->nnodes; ++i)
-  // 	// {
-
-  // 	// }
-
-  // }
-
-  void fill_linknodes() {
-    for (int i = 0; i < this->nnodes; ++i) {
-      if (this->is_in_bound_and_can_create_link(i) == false)
-        continue;
+enum class PARAM_DT_HYDRO // : std::uint8_t
+{
+  CONSTANT,
+  VARIABLE,
+  COURANT,
+};
 
-      int o = this->get_right_idx(i);
-      this->_fill_linknode(i, o, 0);
-      o = this->get_bottomright_idx(i);
-      this->_fill_linknode(i, o, 2);
-      o = this->get_bottom_idx(i);
-      this->_fill_linknode(i, o, 4);
-      o = this->get_bottomleft_idx(i);
-      this->_fill_linknode(i, o, 6);
-
-      if (this->boundaries.is_periodic(i))
-      // if(true)
-      {
-        o = this->get_left_idx(i);
-        this->_fill_linknode(o, i, 0);
-        o = this->get_topleft_idx(i);
-        this->_fill_linknode(o, i, 2);
-        o = this->get_top_idx(i);
-        this->_fill_linknode(o, i, 4);
-        o = this->get_topright_idx(i);
-        this->_fill_linknode(o, i, 6);
-      }
-    }
-  }
+enum class PARAM_DT_MORPHO // : std::uint8_t
+{
+  CONSTANT,
+  VARIABLE,
+  COURANT,
+  HYDRO,
+};
 
-  void _fill_linknode(int f, int o, int add) {
-
-    // if(this->is_in_bound_and_can_create_link(f) == false ||
-    // 	this->is_in_bound_and_can_create_link(o) == false ||
-    // 	(this->boundaries.force_giving(f) && this->boundaries.force_giving(o))
-    // || 	(this->boundaries.force_receiving(f) &&
-    // this->boundaries.force_receiving(o))
-    // 	)
+enum class HYDROGRAPH_LM {
+  IGNORE,
+  REROUTE,
+  FILL,
+};
 
-    if (this->is_in_bound_and_can_create_link(f) == false ||
-        this->is_in_bound_and_can_create_link(o) == false)
-      return;
+enum class MFD_PARTITIONNING {
+  PROPOSLOPE,
+  SQRTSLOPE,
+  PROPOREC,
+};
 
-    if (this->linknodes[f * 8 + add] != -1)
-      return;
+enum class WATER_INPUT {
+  PRECIPITATIONS_CONSTANT,
+  PRECIPITATIONS_VARIABLE,
+  ENTRY_POINTS_H,
+};
 
-    if ((this->boundaries.can_give(f) && this->boundaries.can_receive(o)) ||
-        (this->boundaries.can_give(o) && this->boundaries.can_receive(f))) {
-      this->linknodes[f * 8 + add] = f;
-      this->linknodes[f * 8 + add + 1] = o;
-    }
+enum class SED_INPUT {
+  NONE,
+  ENTRY_POINTS_Q,
+};
 
-    else {
-      this->linknodes[f * 8 + add] = -1;
-      this->linknodes[f * 8 + add + 1] = -1;
-    }
+enum class BOUNDARY_HW {
+  FIXED_HW,
+  FIXED_SLOPE,
+};
 
-    // if( this->boundaries.force_giving(f) && this->boundaries.can_receive(o) )
-  }
+enum class CONVERGENCE { NONE, DHW, QWR, ALL };
 
-  template <class i_t>
-  void get_nodes_from_linkidx_implicit(int li, int &n1, int &n2) {
-    n1 = floor(li / 4);
-    n2 = n1 + li % 4;
+constexpr double GRAVITY = 9.81, FIVETHIRD = 5. / 3., TWOTHIRD = 2. / 3.;
 
-    bool nodes_can_create_links =
-        (this->is_in_bound_and_can_create_link(n1) == false ||
-         this->is_in_bound_and_can_create_link(n1) == false);
-    bool both_forced = false;
-    if (nodes_can_create_links) {
-      if (this->boundaries.forcing_io(n1) && this->boundaries.forcing_io(n2))
-        both_forced = true;
+template <class fT, class Graph_t, class Connector_t> class graphflood {
+public:
+  // Underlying connector and graph objects:
+  Graph_t *graph;
+  Connector_t *connector;
+
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  //~=~=~=~=~=~ Main data holders ~=~=~=~=~=~~=~=~=~=~=~~=~=~=
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+
+  // # Hydraulic Surface elevation (bedrock + sed + water)
+  std::vector<fT> _surface;
+
+  // # Water depth
+  std::vector<fT> _hw;
+
+  // # Water discharge
+  std::vector<fT> _Qw;
+
+  // # Sediment discahrge
+  std::vector<fT> _Qs;
+
+  // # Sediment height
+  std::vector<fT> _hs;
+
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  //~=~=~=~=~=~=~= Hydro params and related functions ~=~=~=~=
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  // _      _      _      _      _      _      _      _
+  // )`'-.,_)`'-.,_)`'-.,_)`'-.,_)`'-.,_)`'-.,_)`'-.,_)`'-.,_
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+
+  // Model options
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+
+  // # Is the graph SFD or MFD (or else)
+  HYDRO hydromode = HYDRO::GRAPH_MFD;
+
+  // # Is morpho activated (potentially deprecated)
+  MORPHO morphomode = MORPHO::NONE;
+  // # How to deal with local minima, from graphflood point of view (the
+  // rerouting is managed by the graph)
+  HYDROGRAPH_LM depression_management = HYDROGRAPH_LM::FILL;
+
+  // # How to partition flow in MFD: proportional to the slope, sqrt, ...
+  MFD_PARTITIONNING weight_management = MFD_PARTITIONNING::PROPOSLOPE;
+
+  // # How to manage tthe time step for hydrological calculation
+  PARAM_DT_HYDRO mode_dt_hydro = PARAM_DT_HYDRO::COURANT;
+
+  // # How to manage Water inputs
+  WATER_INPUT water_input_mode = WATER_INPUT::PRECIPITATIONS_CONSTANT;
+
+  // # How to manage boundary conditions
+  BOUNDARY_HW boundhw = BOUNDARY_HW::FIXED_HW;
+
+  // # method to check convergence (Experimental)
+  CONVERGENCE convergence_mode = CONVERGENCE::NONE;
+
+  // Param value holder
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+
+  // # Hydro timestep
+  std::vector<fT> _dt_hydro = {1e-3};
+
+  // # courant stuff
+  // ## actual courant number
+  fT courant_number = 5e-4;
+  // ## maximum dt under courant conditions
+  fT max_courant_dt_hydro = 1e3;
+  // ## minimum dt under courant conditions
+  fT min_courant_dt_hydro = 1e-4;
+  // ## actual time step (default -1 means not calculated yet)
+  fT courant_dt_hydro = -1;
+
+  // # minimum slope for manning's calculation
+  fT minslope = 0.;
+
+  // # Stochasticity management (experimental)
+  // ## Enable stochasticity added to the slope
+  bool stochaslope = false;
+  // # Stochasticity magnitude
+  fT stochaslope_coeff = 1.;
+  // # Stochasticity magnitude
+  fT bou_fixed_val = 0.;
+
+  // # Convergence checekrs
+  // ## nodes used to check convergence
+  std::vector<int> conv_nodes;
+  // ## Initial discharge at convergence nodes
+  std::vector<fT> conv_ini_Qw;
+  // ## tracking delta hw at convergence nodes
+  std::vector<std::vector<fT>> conv_dhw;
+  // ## tracking discharge ratio at convergence nodes
+  std::vector<std::vector<fT>> conv_Qr;
+  // ## tracking which nodes have converged
+  std::vector<std::uint8_t> converged;
+
+  // # Manning's constant
+  // ## is manning spatially constant
+  bool mode_mannings = false;
+  // ## Data holder
+  std::vector<fT> _mannings = {0.033};
+
+  // # Input discharge water
+  // ## As precipitations
+  std::vector<fT> _precipitations = {1e-4};
+  // ## As discrete entry points
+  // ### Entry points
+  std::vector<int> _water_entry_nodes;
+  // ### Entry discahrge
+  std::vector<fT> _water_entries;
+
+  // # Topological number correcting for MFD (see paper)
+  fT topological_number = 4. / 8.;
+
+  // # Use flow depth sensu Caesar Lisflood (only taking the height where water
+  // can flow)
+  bool hflow = false;
+
+  // # Is the model in hydrostationary mode
+  bool hydrostationary = true;
+  // # Experimental
+  fT Qwin_crit = 0.;
+
+  // # Debugging temp holder
+  bool debugntopo = true;
+  std::vector<fT> DEBUGNTOPO;
+  fT debug_CFL = 0.;
+
+  // # Create random device and Mersenne Twister engine
+  std::random_device rd;
+  std::mt19937 gen;
+  std::uniform_int_distribution<> dis;
+
+  // Randomiser helper
+  DAGGER::easyRand randu;
+
+  // # Precipitons stuff (will wvolve or get remove or remain experimental
+  // anyway)
+  std::vector<fT> last_Smax;
+  std::vector<fT> last_dt_prec;
+  std::vector<fT> last_dt_prec_e;
+  std::vector<fT> last_sw_prec;
+  std::vector<fT> last_dx_prec;
+  fT current_dt_prec = 0.;
+  fT Vp = 0.;
+
+  // Setters and Getters
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+
+  // # Export flow depth
+  template <class out_t> out_t get_hw() {
+    return DAGGER::format_output<std::vector<fT>, out_t>(this->_hw);
+  }
+
+  // # Export Surface
+  template <class out_t> out_t get_surface_topo() {
+    return DAGGER::format_output<std::vector<fT>, out_t>(this->_surface);
+  }
+
+  // # Export topographic surface
+  template <class out_t> out_t get_bedrock_topo() {
+    std::vector<fT> diff(this->_surface);
+
+    for (int i = 0; i < this->graph->nnodes; ++i)
+      diff[i] -= this->_hw[i];
+
+    return DAGGER::format_output<std::vector<fT>, out_t>(diff);
+  }
+
+  // # Export Qwin
+  template <class out_t> out_t get_Qwin() {
+    return DAGGER::format_output<std::vector<fT>, out_t>(this->_Qw);
+  }
+
+  // # Export Debug info (changes from time to time)
+  template <class out_t> out_t get_SSTACKDEBUG() {
+    return DAGGER::format_output<std::vector<size_t>, out_t>(
+        this->graph->Sstack);
+  }
+
+  // # Manning's setter
+  void set_mannings(fT val) { this->_mannings = {val}; }
+
+  // # Hydro constant timestep getter
+  fT get_dt_hydro() const { return this->_dt_hydro[0]; }
+  // # Setting the hydrologic time step to courant number
+  void enable_courant_dt_hydro() {
+    this->mode_dt_hydro = PARAM_DT_HYDRO::COURANT;
+  }
+  // # Setting the hydrologic time step to courant number
+  void disable_courant_dt_hydro() {
+    this->mode_dt_hydro = PARAM_DT_HYDRO::CONSTANT;
+  }
+
+  // # Setting the courant number
+  void set_courant_number(fT val) { this->courant_number = val; };
+
+  // # Setting the max dt courant can set
+  void set_max_courant_dt_hydro(fT val) { this->max_courant_dt_hydro = val; };
+
+  // # Setting the min dt courant can set
+  void set_min_courant_dt_hydro(fT val) { this->min_courant_dt_hydro = val; };
+
+  // # Getting the courant dt used for the last time step
+  fT get_courant_dt_hydro() const { return this->courant_dt_hydro; }
+
+  // # Experimental
+  int n_nodes_convergence() const {
+    return static_cast<int>(conv_nodes.size());
+  }
+  int n_stack_convergence() const {
+    if (this->convergence_mode == CONVERGENCE::ALL ||
+        this->convergence_mode == CONVERGENCE::QWR)
+      return static_cast<int>(this->conv_Qr[0].size());
+    if (this->convergence_mode == CONVERGENCE::ALL ||
+        this->convergence_mode == CONVERGENCE::DHW)
+      return static_cast<int>(this->conv_dhw[0].size());
+    return 0;
+  }
+
+  // # Set topological number (deprecated, now dynamically calculated)
+  void set_topological_number(fT val) { this->topological_number = val; };
+
+  // # get topological number (deprecated, now dynamically calculated)
+  fT get_topological_number() const { return this->topological_number; };
+
+  // # Set partition method
+  void set_partition_method(MFD_PARTITIONNING &tmffmeth) {
+    this->weight_management = tmffmeth;
+  }
+
+  // # Set the stochasticity coeff (de facto enable stochaslope stuff)
+  void set_stochaslope(fT val) {
+    this->stochaslope = true;
+    this->stochaslope_coeff = val;
+    this->connector->set_stochaticiy_for_SFD(val);
+  }
+
+  // # Disable the stochasticity on slope calculations
+  void disable_stochaslope() { this->stochaslope = false; }
+
+  // # Set the model to hydrostationary mode
+  void enable_hydrostationary() { this->hydrostationary = true; };
+
+  // # Set the model to dynamic mode
+  void disable_hydrostationary() { this->hydrostationary = false; };
+
+  // # (Past experiment, does not work) Set the model to Qwincrit
+  void set_Qwin_crit(fT val) {
+    this->Qwin_crit = val;
+    this->hydromode = HYDRO::GRAPH_HYBRID;
+  }
+
+  // # set the boundaries to a constant flow depth
+  void set_fixed_hw_at_boundaries(fT val) {
+    this->boundhw = BOUNDARY_HW::FIXED_HW;
+    this->bou_fixed_val = val;
+  }
+
+  // # set the boundaries to a constant hydraulic slope
+  void set_fixed_slope_at_boundaries(fT val) {
+    this->boundhw = BOUNDARY_HW::FIXED_SLOPE;
+    this->bou_fixed_val = val;
+  }
+
+  // # get the array of topological numbers
+  std::vector<fT> get_nT() { return this->DEBUGNTOPO; }
+
+  // # Setting the timestep for constant hydro (does not have any effect if
+  // courant is on)
+  void set_dt_hydro(fT tdt) { this->_dt_hydro = {tdt}; }
+
+  // # Setting dicrete entry point for water discharge
+  template <class out_t, class in_t>
+  void set_water_input_by_entry_points(out_t &hw_entry, in_t &hw_indices) {
+    // preformatting the inputs
+    auto tin = DAGGER::format_input(hw_entry);
+    auto tin_idx = DAGGER::format_input(hw_indices);
+
+    // Setting the general mode
+    this->water_input_mode = WATER_INPUT::ENTRY_POINTS_H;
+    this->_water_entry_nodes = DAGGER::to_vec(tin_idx);
+    this->_water_entries = DAGGER::to_vec(tin);
+
+    // Correcting boundary conditions
+    for (size_t i = 0; i < this->_water_entry_nodes.size(); ++i) {
+      this->connector->boundaries.codes[this->_water_entry_nodes[i]] =
+          BC::FORCE_IN;
+    }
+  }
+
+  // # Setting global constant precipitation rates
+  void set_water_input_by_constant_precipitation_rate(fT precipitations) {
+    this->water_input_mode = WATER_INPUT::PRECIPITATIONS_CONSTANT;
+    this->_precipitations = {precipitations};
+  }
+
+  // # Setting global constant precipitation rates
+  template <class out_t>
+  void set_water_input_by_variable_precipitation_rate(out_t &precipitations) {
+    this->water_input_mode = WATER_INPUT::PRECIPITATIONS_VARIABLE;
+    auto tin = format_input(precipitations);
+    this->_precipitations = DAGGER::to_vec(tin);
+  }
+
+  // # Setting Flow partition to MFD
+  void enable_MFD() { this->hydromode = HYDRO::GRAPH_MFD; }
+
+  // # Setting Flow partition to SFD
+  void enable_SFD() { this->hydromode = HYDRO::GRAPH_SFD; }
+
+  // # Local Minima will be filled with water automatically
+  void fill_minima() { this->depression_management = HYDROGRAPH_LM::FILL; }
+
+  // # Flow will route through local minimas, negative slopes will be treated as
+  // 1e-6
+  void reroute_minima() {
+    this->depression_management = HYDROGRAPH_LM::REROUTE;
+  }
+
+  // # Flow stops at local minimas
+  void ignore_minima() { this->depression_management = HYDROGRAPH_LM::IGNORE; }
+
+  // Optional hydraulic model monitoring
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+
+  // # Tracking the total input of water added to the model
+  fT tot_Qw_input = 0;
+  fT get_tot_Qw_input() const { return this->tot_Qw_input; }
+
+  // # Tracking the total Qwin exiting the model (for mass balance cheking for
+  // example)
+  fT tot_Qwin_output = 0;
+  fT get_tot_Qwin_output() const { return this->tot_Qwin_output; }
+
+  // # Tracking the total Qwout exiting the model (for mass balance cheking for
+  // example)
+  fT tot_Qw_output = 0;
+  fT get_tot_Qw_output() const { return this->tot_Qw_output; }
+
+  // # Tracking the total Qs exiting the model (for mass balance cheking for
+  // example)
+  fT tot_Qs_output = 0;
+  fT get_tot_Qs_output() const { return this->tot_Qs_output; }
+
+  // # Qw_out recorder for the whole landscape
+  // ## switch activating the recording
+  bool record_Qw_out = false;
+  // ## Data holder
+  std::vector<fT> _rec_Qwout;
+  // ## Switching on the recording
+  void enable_Qwout_recording() { this->record_Qw_out = true; };
+  // ## Switching off the recording
+  void disable_Qwout_recording() {
+    this->record_Qw_out = false;
+    this->_rec_Qwout.clear();
+  };
+  // ## Exporting the output
+  template <class out_t> out_t get_Qwout_recording() {
+    return DAGGER::format_output<std::vector<fT>, out_t>(this->_rec_Qwout);
+  }
+
+  // # Hydraulic slope recorder for the whole landscape
+  // ## switch activating the recording
+  bool record_Sw = false;
+  // ## Data holder
+  std::vector<fT> _rec_Sw;
+  // ## Switching on the recording
+  void enable_Sw_recording() { this->record_Sw = true; };
+  // ## Switching off the recording
+  void disable_Sw_recording() {
+    this->record_Sw = false;
+    this->_rec_Sw.clear();
+  };
+  // ## Exporting the output
+  template <class out_t> out_t get_Sw_recording() {
+    return DAGGER::format_output<std::vector<fT>, out_t>(this->_rec_Sw);
+  }
+
+  // # Flow depth increment recorder for the whole landscape
+  // ## switch activating the recording
+  bool record_dhw = false;
+  // ## Data holder
+  std::vector<fT> _rec_dhw;
+  // ## Switching on the recording
+  void enable_dhw_recording() { this->record_dhw = true; };
+  // ## Switching off the recording
+  void disable_dhw_recording() {
+    this->record_dhw = false;
+    this->_rec_dhw.clear();
+  };
+  // ## Exporting the output
+  template <class out_t> out_t get_dhw_recording() {
+    return DAGGER::format_output<std::vector<fT>, out_t>(this->_rec_dhw);
+  }
+
+  // # Local minima initial filling recorder for the whole landscape
+  // ## switch activating the recording
+  bool record_filling = false;
+  // ## Data holder
+  std::vector<fT> _rec_filling;
+  // ## Switching on the recording
+  void enable_filling_recording() { this->record_filling = true; };
+  // ## Switching off the recording
+  void disable_filling_recording() {
+    this->record_filling = false;
+    this->_rec_filling.clear();
+  };
+  // ## Exporting the output
+  template <class out_t> out_t get_filling_recording() {
+    return DAGGER::format_output<std::vector<fT>, out_t>(this->_rec_filling);
+  }
+
+  // # FLow vector recorder for the whole landscape
+  // ## switch activating the recording
+  bool record_flowvec = false;
+  // ## Data holder
+  std::vector<fT> _rec_flowvec;
+  // ## Switching on the recording
+  void enable_flowvec_recording() { this->record_flowvec = true; };
+  // ## Switching off the recording
+  void disable_flowvec_recording() {
+    this->record_flowvec = false;
+    this->_rec_flowvec.clear();
+  };
+  // ## Exporting the output
+  template <class out_t> out_t get_flowvec_recording() {
+    return DAGGER::format_output<std::vector<fT>, out_t>(this->_rec_flowvec);
+  }
+
+  // =~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~
+  // =~=~=~=~=~= Morpho params and related functions =~=~=~=~=~=~=~
+  // =~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~
+  //                   . - ~ ~ ~ - .
+  //         _     .-~               ~- .
+  //         \ `..~                       ` .
+  //           }  }              /       \   \
+// (\   \\ \~^..'                 |       }  \
+// \`.-~  o      /       }       |        /  \
+// (__          |       /        |       /    `.
+  // `- - ~ ~ -._|      /_ - ~ ~ ^|   ____/- _    `.
+  //         |     /          |     /     ~-.     ~- _
+  //         |_____|          |_____|         ~ - . _ _~_-_
+  // =~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~
+  // =~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~
+  // =~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~
+
+  // The whole morpho section is highly WIP and not really detailed yet as it
+  // will really evolve
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+
+  // # method to manage time steps for the morpho (WIP)
+  PARAM_DT_MORPHO mode_dt_morpho = PARAM_DT_MORPHO::HYDRO;
+
+  // # method to manage sediment input (WIP)
+  SED_INPUT sed_input_mode = SED_INPUT::NONE;
+
+  fT tau_max = 0.;
+  fT current_dt_prec_e = 0.;
+  fT Vps = 0.;
+
+  std::vector<int> _sed_entry_nodes;
+  std::vector<fT> _sed_entries;
+
+  bool record_edot = false;
+  std::vector<fT> _rec_edot;
+  void enable_edot_recording() { this->record_edot = true; };
+  void disable_edot_recording() {
+    this->record_edot = false;
+    this->_rec_edot.clear();
+  };
+  template <class out_t> out_t get_edot_recording() {
+    return DAGGER::format_output<std::vector<fT>, out_t>(this->_rec_edot);
+  }
+
+  bool record_ddot = false;
+  std::vector<fT> _rec_ddot;
+  void enable_ddot_recording() { this->record_ddot = true; };
+  void disable_ddot_recording() {
+    this->record_ddot = false;
+    this->_rec_ddot.clear();
+  };
+  template <class out_t> out_t get_ddot_recording() {
+    return DAGGER::format_output<std::vector<fT>, out_t>(this->_rec_ddot);
+  }
+
+  // # a exponent for erosion
+  bool mode_aexp = false;
+  std::vector<fT> _aexp = {1.5};
+
+  // # ke (coefficient for erosion)
+  PARAM_KE mode_ke = PARAM_KE::CONSTANT;
+  std::vector<fT> _ke = {1e-4};
+
+  // # ke (coefficient for erosion)
+  bool mode_ke_lateral = false;
+  std::vector<fT> _ke_lateral = {0.1};
+
+  // # ke (coefficient for erosion)
+  bool mode_kd = false;
+  std::vector<fT> _kd = {100};
+  ;
+
+  // # kd (coefficient for erosion)
+  bool mode_kd_lateral = false;
+  std::vector<fT> _kd_lateral = {0.1};
+  ;
+
+  // # ke (coefficient for erosion)
+  bool mode_rho = false;
+  std::vector<fT> _rho = {1000};
+  ;
+
+  // # ke (coefficient for erosion)
+  bool mode_tau_c = false;
+  std::vector<fT> _tau_c = {6};
+  ;
+
+  // # ke (coefficient for erosion)
+  fT dt_morpho_multiplier = 1.;
+  void set_dt_morpho_multiplier(fT val) { this->dt_morpho_multiplier = val; }
+  std::vector<fT> _dt_morpho = {1e-3};
+
+  void set_dt_morpho(fT tdt) {
+    this->mode_dt_morpho = PARAM_DT_MORPHO::CONSTANT;
+    this->_dt_morpho = {tdt};
+  }
+
+  template <class out_t, class in_t>
+  void set_sed_input_by_entry_points(out_t &sed_entry, in_t &sed_indices) {
+    // preformatting the inputs
+    auto tin = DAGGER::format_input(sed_entry);
+    auto tin_idx = DAGGER::format_input(sed_indices);
+
+    // Setting the general mode
+    this->sed_input_mode = SED_INPUT::ENTRY_POINTS_Q;
+
+    this->_sed_entry_nodes = DAGGER::to_vec(tin_idx);
+    this->_sed_entries = DAGGER::to_vec(tin);
+  }
+
+  void enable_morpho() { this->morphomode = MORPHO::TL; }
+  void disable_morpho() { this->morphomode = MORPHO::NONE; }
+
+  void set_single_aexp(fT ta) {
+    this->mode_aexp = false;
+    this->_aexp = {ta};
+  }
+  void set_single_ke(fT ta) {
+    this->mode_ke = PARAM_KE::CONSTANT;
+    this->_ke = {ta};
+  }
+  void set_single_ke_lateral(fT ta) {
+    this->mode_ke_lateral = false;
+    this->_ke_lateral = {ta};
+  }
+  void set_single_kd(fT ta) {
+    this->mode_kd = false;
+    this->_kd = {ta};
+  }
+  void set_single_kd_lateral(fT ta) {
+    this->mode_kd_lateral = false;
+    this->_kd_lateral = {ta};
+  }
+  void set_single_tau_c(fT ta) {
+    this->mode_tau_c = false;
+    this->_tau_c = {ta};
+  }
+
+  template <class topo_t> void set_variable_ke(topo_t &variable_ke) {
+    auto tke = format_input(variable_ke);
+    this->_ke = to_vec(tke);
+    this->mode_ke = PARAM_KE::VARIABLE;
+  }
+
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  //~=~=~=~= Functions setting up the model ~=~=~=~=~=~=~=~=~=
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  // _      _      _      _      _      _      _      _
+  // )`'-.,_)`'-.,_)`'-.,_)`'-.,_)`'-.,_)`'-.,_)`'-.,_)`'-.,_
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+
+  // Constructors
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+
+  // # Model constructor without any params (need to seed the randomiser though)
+  graphflood() { this->gen = std::mt19937(this->rd()); };
+
+  // # Model classic constructor from existing graph and connector objects
+  graphflood(Graph_t &graph, Connector_t &connector) {
+    // Ingesting graph and connectors
+    this->graph = &graph;
+    this->connector = &connector;
+
+    // Seeding the random engine
+    this->gen = std::mt19937(this->rd());
+  }
+
+  // # Setting initial topo (or updating topo from external sources)
+  template <class topo_t> void set_topo(topo_t &topo) {
+    // formatting input from higher level languages to c++ veclike stuff
+    auto tin = DAGGER::format_input(topo);
+    std::vector<fT> temp = DAGGER::to_vec(tin);
+
+    // Initialising flow depth if not done yet
+    bool inithw = false;
+    if (this->_hw.size() == 0) {
+      inithw = true;
+      this->_hw = std::vector<fT>(this->graph->nnodes, 0);
+    }
+
+    // Fedding the surface (and correcting to eventual existing flow depth)
+    this->_surface = std::vector<fT>(temp);
+    if (inithw == false) {
+      for (int i = 0; i < this->graph->nnodes; ++i) {
+        this->_surface[i] += this->_hw[i];
+      }
+    }
+
+    // Done
+  }
+
+  // # Setting the flow depth to an external value
+  template <class topo_t> void set_hw(topo_t &thw) {
+    // formatting input from higher level languages to c++ veclike stuff
+    auto tin = DAGGER::format_input(thw);
+    std::vector<fT> temp = DAGGER::to_vec(tin);
+
+    // case one: no preexisting flow depth, adding hw to hydraulic surface
+    if (this->_hw.size() == 0) {
+      this->_hw = std::move(temp);
+      for (int i = 0; i < this->graph->nnodes; ++i)
+        this->_surface[i] += this->_hw[i];
     }
-
-    // Then not a valid link
-    if (nodes_can_create_links || both_forced) {
-      n1 = -1;
-      n2 = -1;
+    // case two: preexisting flow depth, correcting to hw
+    else {
+      for (int i = 0; i < this->graph->nnodes; ++i)
+        this->_surface[i] += temp[i] - this->_hw[i];
+      this->_hw = std::move(temp);
     }
   }
 
-  // Function updating ONLY the MFD receivers
-  // This is useful in the cases where SFD recs are conditionned by an other
-  // mean and cannot be touched (e.g. Cordonnier)
-  template <class topo_t> void update_links_MFD_only(topo_t &topography) {
-    // iterating though every links
-    for (size_t i = 0; i < this->links.size(); ++i) {
-      // Getting hte 2 nodes of the current link
-      int from = this->linknodes[i * 2];
-      int to = this->linknodes[i * 2 + 1];
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  //~=~=~=~= Generic accessors for internal use ~=~=~=~=~=~=~=
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  // _      _      _      _      _      _      _      _
+  // )`'-.,_)`'-.,_)`'-.,_)`'-.,_)`'-.,_)`'-.,_)`'-.,_)`'-.,_
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
 
-      if (from == -1) {
-        this->links[i] = 2;
-        continue;
-      }
+  // Surfaces and Hydraulic components
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
 
-      if (this->boundaries.forcing_io(from) ||
-          this->boundaries.forcing_io(to)) {
+  // # get local flow depth at node
+  fT hw(int i) { return this->_hw[i]; }
 
-        if (this->boundaries.force_giving(from) ||
-            this->boundaries.force_receiving(to))
-          this->links[i] = 1;
-        else if (this->boundaries.force_giving(to) ||
-                 this->boundaries.force_receiving(from))
-          this->links[i] = 0;
-        else {
-          throw std::runtime_error("Should not happen 777");
-          this->links[i] = 2;
-        }
+  // # get local input flow discharge at node
+  fT Qw(int i) { return this->_Qw[i]; }
 
-        continue;
-      }
+  // # get local sediment input discharge at node
+  fT Qs(int i) { return this->_Qs[i]; }
 
-      // by convention true -> topo1 > topo2
-      if (topography[from] > topography[to] &&
-          this->boundaries.can_give(from) && this->boundaries.can_receive(to))
-        this->links[i] = 1;
-      else if (this->boundaries.can_give(to) &&
-               this->boundaries.can_receive(from))
-        this->links[i] = 0;
-      // If the configuration cannot allow the link, it is temporarily disabled
-      else
-        this->links[i] = 2;
-    }
-    // done
+  // # get local topographic + water surface at node
+  fT surface(int i) { return this->_surface[i]; }
+
+  // # Manning's coefficient at node
+  fT mannings(int i) {
+    if (this->mode_mannings)
+      return this->_mannings[i];
+    else
+      return this->_mannings[0];
   }
 
-  // Updates all the link and the SFD info
-  template <class topo_t> void update_links(topo_t &topography) {
-    // std::cout << "BUNT" << std::endl;
+  // # Precipitation rate at node
+  fT precipitations(int i) {
+    if (this->water_input_mode == WATER_INPUT::PRECIPITATIONS_VARIABLE)
+      return this->_precipitations[i];
+    else
+      return this->_precipitations[0];
+  }
 
-    // am I using a stochastic adjustment for deciding on the steepest slope
-    // iterating through all the nodes
-    for (size_t i = 0; i < this->links.size(); ++i) {
+  // small helper function returning node index from the right stack
+  int get_istack_node(int i) {
+    if (this->hydromode != HYDRO::GRAPH_SFD)
+      return this->graph->stack[i];
+    else
+      return this->graph->Sstack[i];
+  }
 
-      // Checking the validity of the link
-      if (this->linknodes[i * 2] < 0) {
-        this->links[i] = 2;
-        continue;
-      }
+  fT get_Sw(int lix, fT minslope) {
+    int from, to;
+    this->connector->from_to_from_link_index(lix, from, to);
+    return std::max((this->_surface[from] - this->_surface[to]) /
+                        this->connector->get_dx_from_links_idx(lix),
+                    minslope);
+  }
 
-      // Getting ht etwo nodes of the links
-      int from = this->linknodes[i * 2];
-      int to = this->linknodes[i * 2 + 1];
-
-      // std::cout << std::setprecision(18);
-
-      // if( 808 * this->nx + 733 == from)
-      // 	std::cout << i <<" TESTED NODE from:: " << topography[from] << "
-      // v " << topography[to]  << "||" << (topography[from] > topography[to])
-      // << std::endl; if( 808 * this->nx + 733 == to) 	std::cout << i <<"
-      // TESTED NODE to:: " << topography[to] << " v " << topography[from] <<
-      // "||" << (topography[to] > topography[from]) << std::endl;
-
-      // std::cout << from << "|" << to << "||";
-
-      // getting the link infos
-      // -> dx
-      T dx = this->get_dx_from_links_idx(i);
-      // -> slope
-      T slope = (topography[from] - topography[to]) / dx;
-
-      if (this->boundaries.forcing_io(from) ||
-          this->boundaries.forcing_io(to)) {
-
-        if (this->boundaries.force_giving(from) ||
-            this->boundaries.force_receiving(to))
-          slope = 1 / std::abs(slope);
-
-        else if (this->boundaries.force_giving(to) ||
-                 this->boundaries.force_receiving(from))
-          slope = -1 / std::abs(slope);
-      }
-
-      if (this->stochastic_slope_on)
-        slope *= (this->randu->get() * this->stochastic_slope_coeff) + 1e-6;
-
-      // if slope is positive, to is the receiver by convention
-      if (slope > 0 && this->boundaries.can_give(from) &&
-          this->boundaries.can_receive(to)) {
-        // Conventional direction
-        this->links[i] = 1;
-        // if Steepest Slope is higher than the current recorded one
-        if (this->SS[from] < slope) {
-          // saving the Sreceivers info as temporary best choice
-          this->Sreceivers[from] = to;
-          this->Sdistance2receivers[from] = dx;
-          this->SS[from] = slope;
-        }
-      } else if (this->boundaries.can_give(to) &&
-                 this->boundaries.can_receive(from)) {
-        // Otherwise the convention is inverted:
-        // isrec is falese and to is giving to from
-        this->links[i] = 0;
-        // NOte that slope is absolute values
-        slope = std::abs(slope);
-        if (this->SS[to] < slope) {
-          this->Sreceivers[to] = from;
-          this->Sdistance2receivers[to] = dx;
-          this->SS[to] = slope;
-        }
-      } else
-        this->links[i] = 2;
-    }
+  fT get_Sw(int node, int rec, fT dx, fT minslope) {
+    return std::max((this->_surface[node] - this->_surface[rec]) / dx,
+                    minslope);
+  }
 
-    // Finally inverting the Sreceivers into the Sdonors info
-    // Required for several routines
-    this->compute_SF_donors_from_receivers();
-  }
-
-  // Fucntion inverting the SFD receivers into donors
-  void compute_SF_donors_from_receivers() {
-    // Initialising the graph dimesions for the donors
-    // All of thenm have the graph dimension
-    this->Sdonors = std::vector<int>(this->nnodes * this->nneighbours, -1);
-    this->nSdonors = std::vector<int>(this->nnodes, 0);
-
-    // iterating through all the nodes
-    for (int i = 0; i < this->nnodes; ++i) {
-      // SF so rid == i cause there is only 1 rec
-      int trec = this->Sreceivers[i];
-      if (trec == i)
-        continue;
+  fT get_Sw(int node, int rec, fT dx) {
+    return (this->_surface[node] - this->_surface[rec]) / dx;
+  }
 
-      // feeding the Sdonors array at rec position with current node and...
-      this->Sdonors[trec * this->nneighbours + this->nSdonors[trec]] = i;
-      // ... incrementing the number of Sdonors
-      this->nSdonors[trec] += 1;
-    }
-    // done
+  fT get_Stopo(int node, int rec, fT dx) {
+    return (this->_surface[node] - this->_hw[node] -
+            (this->_surface[rec] - this->_hw[rec])) /
+           dx;
   }
 
-  // Same function than above but without reallocating the memory (can save a
-  // bit of time depending on the context)
-  void recompute_SF_donors_from_receivers() {
+  // Morpho params (WIP, no working version yet)
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
 
-    for (int i = 0; i < this->nnodes; ++i) {
-      for (int j = 0; j < this->nneighbours; ++j)
-        this->Sdonors[i * this->nneighbours + j] = -1;
-      this->nSdonors[i] = 0;
-    }
+  // # get topographic + water surface
+  fT aexp(int i) {
+    if (this->mode_aexp)
+      return this->_aexp[i];
+    else
+      return this->_aexp[0];
+  }
 
-    for (int i = 0; i < this->nnodes; ++i) {
-      // SF so rid == i cause there is only 1 rec
-      int trec = this->Sreceivers[i];
-      if (trec == i)
-        continue;
-      this->Sdonors[trec * this->nneighbours + this->nSdonors[trec]] = i;
-      this->nSdonors[trec] += 1;
-    }
+  fT ke(int i) {
+    if (PARAM_KE::VARIABLE == this->mode_ke)
+      return this->_ke[i];
+    else
+      return this->_ke[0];
   }
 
-  // Helper functions to allocate and reallocate vectors when
-  // computing/recomputing the graph
-  void _allocate_vectors() {
-    this->links =
-        std::vector<std::uint8_t>(int(this->nnodes * this->nneighbours / 2), 2);
-    this->linknodes =
-        std::vector<int>(int(this->nnodes * this->nneighbours), -1);
-    this->Sreceivers = std::vector<int>(this->nnodes, -1);
-    for (int i = 0; i < this->nnodes; ++i)
-      this->Sreceivers[i] = i;
-    this->Sdistance2receivers = std::vector<T>(this->nnodes, -1);
-    this->SS = std::vector<T>(this->nnodes, 0.);
-  }
-
-  void _reallocate_vectors() {
-    for (int i = 0; i < this->nnodes; ++i) {
-      this->Sreceivers[i] = i;
-      this->Sdistance2receivers[i] = 0;
-      this->SS[i] = 0;
-    }
+  fT ke_lateral(int i) {
+    if (this->mode_ke_lateral)
+      return this->_ke_lateral[i];
+    else
+      return this->_ke_lateral[0];
   }
 
-  bool is_in_bound_and_can_create_link(int o) {
-    bool linkvalid = (this->is_in_bound(o));
-    if (linkvalid)
-      linkvalid = this->boundaries.can_create_link(o);
-    return linkvalid;
-  }
-
-  int get_right_idx_links(int i) { return i * 4; }
-  int get_bottomright_idx_links(int i) { return i * 4 + 1; }
-  int get_bottom_idx_links(int i) { return i * 4 + 2; }
-  int get_bottomleft_idx_links(int i) { return i * 4 + 3; }
-  int get_left_idx_links(int i) {
-    int yolo = this->get_left_idx(i);
-    if (yolo >= 0) {
-      return this->get_right_idx_links(yolo);
-    } else {
-      return this->not_a_node;
-    }
+  fT kd(int i) {
+    if (this->mode_kd)
+      return this->_kd[i];
+    else
+      return this->_kd[0];
   }
-  int get_topleft_idx_links(int i) {
-    int yolo = this->get_topleft_idx(i);
-    if (yolo >= 0) {
-      return this->get_bottomright_idx_links(yolo);
-    } else {
-      return this->not_a_node;
-    }
+
+  fT kd_lateral(int i) {
+    if (this->mode_kd_lateral)
+      return this->_kd_lateral[i];
+    else
+      return this->_kd_lateral[0];
   }
-  int get_top_idx_links(int i) {
-    int yolo = this->get_top_idx(i);
-    if (yolo >= 0) {
-      return this->get_bottom_idx_links(yolo);
-    } else {
-      return this->not_a_node;
-    }
+
+  fT dt_hydro(int i) {
+    if (this->mode_dt_hydro == PARAM_DT_HYDRO::VARIABLE)
+      return this->_dt_hydro[i];
+    else if (this->mode_dt_hydro == PARAM_DT_HYDRO::COURANT) {
+      return this->courant_dt_hydro;
+    } else
+      return this->_dt_hydro[0];
   }
-  int get_topright_idx_links(int i) {
-    int yolo = this->get_topright_idx(i);
-    if (yolo >= 0) {
-      return this->get_bottomleft_idx_links(yolo);
-    } else {
-      return this->not_a_node;
-    }
+
+  fT dt_morpho(int i) {
+    return this->dt_hydro(i) * this->dt_morpho_multiplier;
+    // if (this->mode_dt_morpho == PARAM_DT_MORPHO::VARIABLE)
+    // 	return this->_dt_morpho[i];
+    // else if (this->mode_dt_morpho == PARAM_DT_MORPHO::HYDRO)
+    // 	return this->dt_hydro(i);
+    // else
+    // 	return this->_dt_morpho[0];
   }
-  int get_right_idx_linknodes(int i) { return 2 * i * 4; }
-  int get_bottomright_idx_linknodes(int i) { return 2 * (i * 4 + 1); }
-  int get_bottom_idx_linknodes(int i) { return 2 * (i * 4 + 2); }
-  int get_bottomleft_idx_linknodes(int i) { return 2 * (i * 4 + 3); }
-  int get_left_idx_linknodes(int i) {
-    int yolo = this->get_left_idx(i);
-    if (yolo >= 0) {
-      return 2 * this->get_right_idx_links(yolo);
-    } else {
-      return this->not_a_node;
-    }
+
+  fT tau_c(int i) {
+    if (this->mode_tau_c)
+      return this->_tau_c[i];
+    else
+      return this->_tau_c[0];
   }
-  int get_topleft_idx_linknodes(int i) {
-    int yolo = this->get_topleft_idx(i);
-    if (yolo >= 0) {
-      return 2 * this->get_bottomright_idx_links(yolo);
-    } else {
-      return this->not_a_node;
-    }
+
+  fT rho(int i) {
+    if (this->mode_rho)
+      return this->_rho[i];
+    else
+      return this->_rho[0];
   }
-  int get_top_idx_linknodes(int i) {
-    int yolo = this->get_top_idx(i);
-    if (yolo >= 0) {
-      return 2 * this->get_bottom_idx_links(yolo);
-    } else {
-      return this->not_a_node;
+
+  void block_uplift(fT val) {
+    for (int i = 0; i < this->connector->nnodes; ++i) {
+      if (this->connector->boundaries.can_out(i) == false)
+        this->_surface[i] += this->dt_morpho(i) * val;
     }
   }
-  int get_topright_idx_linknodes(int i) {
-    int yolo = this->get_topright_idx(i);
-    if (yolo >= 0) {
-      return 2 * this->get_bottomleft_idx_links(yolo);
-    } else {
-      return this->not_a_node;
+
+  template <class topo_t> void variable_uplift(topo_t &ival) {
+    auto val = format_input(ival);
+    for (int i = 0; i < this->connector->nnodes; ++i) {
+      // if(this->connector->boundaries.can_out(i) == false)
+      this->_surface[i] += this->dt_morpho(i) * val[i];
     }
   }
 
-  std::vector<int> get_empty_neighbour() { return std::vector<int>(8, 0); }
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  //~=~=~=~= Running and helper functions ~=~=~=~=~=~=~=~=~=~=
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  // _      _      _      _      _      _      _      _
+  // )`'-.,_)`'-.,_)`'-.,_)`'-.,_)`'-.,_)`'-.,_)`'-.,_)`'-.,_
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
 
-  int get_neighbour_idx(int i, std::vector<int> &out) {
+  // # MAin running function
+  void run() {
+    // Saving the topological number if needed
+    if (this->debugntopo)
+      this->DEBUGNTOPO = std::vector<fT>(this->connector->nnodes, 0);
 
-    int n = 0;
+    this->debug_CFL = 0.;
 
-    int next = this->get_right_idx(i);
-    if (this->is_in_bound(next)) {
-      if (!this->boundaries.no_data(next)) {
-        out[n] = next;
-        ++n;
-      }
-    }
-    next = this->get_bottomright_idx(i);
-    if (this->is_in_bound(next)) {
-      if (!this->boundaries.no_data(next)) {
-        out[n] = next;
-        ++n;
-      }
-    }
-    next = this->get_bottom_idx(i);
-    if (this->is_in_bound(next)) {
-      if (!this->boundaries.no_data(next)) {
-        out[n] = next;
-        ++n;
-      }
+    this->tau_max = 0.;
+
+    // Graph Processing
+    this->graph_automator();
+
+    // Initialise the water discharge fields according to water input condition
+    // and other monitoring features:
+    this->init_Qw();
+
+    // reinitialising the sediments if needed
+    if (this->morphomode != MORPHO::NONE)
+      this->init_Qs();
+
+    // Am I in SFD or MFD
+    bool SF = (this->hydromode == HYDRO::GRAPH_SFD);
+
+    // To be used if courant dt hydro is selected
+    fT tcourant_dt_hydro = std::numeric_limits<fT>::max();
+
+    // Vertical motions are applied at the end of the timestep
+    std::vector<fT> vmot, vmot_hw(this->graph->nnodes, 0.);
+
+    // -> Only initialising vertical motions for the bedrock if morpho is on
+    if (this->morphomode != MORPHO::NONE)
+      vmot = std::vector<fT>(this->graph->nnodes, 0.);
+
+    // Caching neighbours, slopes and weights
+    auto receivers = this->connector->get_empty_neighbour();
+    std::array<fT, 8> weights, slopes;
+
+    // main loop
+    for (int i = this->graph->nnodes - 1; i >= 0; --i) {
+
+      // Getting next node in line
+      int node = this->get_istack_node(i);
+
+      // Processing case where the node is a model edge, or no data
+      // this function  returns true if the node was boundary and does not need
+      // to be processed THis is where all the boundary treatment happens, if
+      // you need to add something happening at the boundaries
+      if (this->_initial_check_boundary_pit(node, receivers, vmot_hw))
+        continue;
+
+      // if(this->hydrostationary == false)
+      // {
+      // 	if(this->dt_hydro(node) > 0)
+      // 		this->_hw[node] += this->dt_hydro(node) *
+      // this->precipitations(node); 	else 		this->_hw[node] += 1e-3
+      // * this->precipitations(node);
+
+      // }
+
+      // CFL calculator
+      // fT sum_ui_over_dxi = 0.;
+
+      // Deprecated test to switch dynamically between SFD and MFD (does not
+      // really add anything and is buggy in rivers) if(this->hydromode ==
+      // HYDRO::GRAPH_HYBRID) 	SF = this->_Qw[node] < this->Qwin_crit;
+
+      // Getting the receivers
+      int nrecs;
+      if (SF)
+        nrecs = 1;
+      else
+        nrecs = this->connector->get_receivers_idx_links(node, receivers);
+
+      // Caching Slope max
+      fT Smax;
+      fT dw0max;
+      fT dx;
+      int recmax = node;
+
+      // NOTE:
+      //  No need to calculate the topological number anymore, but keeping it
+      //  for recording its value
+      fT topological_number_v2 = 0.;
+
+      this->_compute_slopes_weights_et_al(node, SF, Smax, slopes, weights,
+                                          nrecs, receivers, recmax, dx, dw0max,
+                                          topological_number_v2);
+
+      // Initialising the total Qout
+      fT Qwin = this->_Qw[node];
+
+      // precalculating the power
+      fT pohw = std::pow(this->_hw[node], TWOTHIRD);
+      // std:: cout << "pohw:" << pohw << "|" << this->_hw[node] << std::endl;
+
+      // Squarerooting Smax
+      // fT debug_S = Smax;
+      auto sqrtSmax = std::sqrt(Smax);
+
+      // Flow Velocity
+      fT u_flow = pohw * sqrtSmax / this->mannings(node);
+      // Volumetric discahrge
+      fT Qwout = dw0max * this->_hw[node] * u_flow;
+      // std::cout << Qwout << "|";
+
+      // Eventually recording Smax
+      if (this->record_Sw)
+        this->_rec_Sw[node] = Smax;
+
+      // temp calc for courant
+      // if(this->mode_dt_hydro == PARAM_DT_HYDRO::COURANT && this->_hw[node] >
+      // 0 && dx >0) 	sum_ui_over_dxi = u_flow/dx;
+
+      // Automates the computation of morpho LEM if needed
+      this->_compute_morpho(node, recmax, dx, Smax, vmot);
+
+      // transfer fluxes
+      // Computing the transfer of water and sed
+      this->_compute_transfers(nrecs, recmax, node, SF, receivers, weights,
+                               Qwin, Qwout);
+
+      // Computing courant based dt
+      if (this->mode_dt_hydro == PARAM_DT_HYDRO::COURANT && u_flow > 0) {
+        fT provisional_dt = (this->courant_number * dx) / u_flow;
+        provisional_dt = std::min(provisional_dt, this->max_courant_dt_hydro);
+        provisional_dt = std::max(provisional_dt, this->min_courant_dt_hydro);
+        tcourant_dt_hydro = std::min(provisional_dt, tcourant_dt_hydro);
+      }
+
+      // computing hydro vertical motion changes for next time step
+      if (this->hydrostationary)
+        vmot_hw[node] +=
+            (this->_Qw[node] - Qwout) / this->connector->get_area_at_node(node);
+      else
+        vmot_hw[node] +=
+            (this->_Qw[node] - Qwout) / this->connector->get_area_at_node(node);
+
+      if (this->record_Qw_out)
+        this->_rec_Qwout[node] += Qwout;
     }
-    next = this->get_bottomleft_idx(i);
-    if (this->is_in_bound(next)) {
-      if (!this->boundaries.no_data(next)) {
-        out[n] = next;
-        ++n;
-      }
+
+    // if(this->tau_max > 500)
+    // 	std::cout << "WARNING::tau_max is " << this->tau_max << std::endl;
+
+    // END OF MAIN LOOP
+
+    // Computing final courant based dt
+
+    if (this->mode_dt_hydro == PARAM_DT_HYDRO::COURANT) {
+      if (this->courant_dt_hydro == -1)
+        this->courant_dt_hydro = 1e-3;
+      else if (tcourant_dt_hydro > 0 &&
+               tcourant_dt_hydro != std::numeric_limits<fT>::max())
+        this->courant_dt_hydro = tcourant_dt_hydro;
     }
-    next = this->get_left_idx(i);
-    if (this->is_in_bound(next)) {
-      if (!this->boundaries.no_data(next)) {
-        out[n] = next;
-        ++n;
-      }
+
+    if (this->convergence_mode == CONVERGENCE::ALL ||
+        this->convergence_mode == CONVERGENCE::DHW) {
+      for (int i = 0; i < this->n_nodes_convergence(); ++i)
+        this->conv_dhw[i].emplace_back(
+            vmot_hw[this->conv_nodes
+                        [i]]); // /this->dt_hydro(this->conv_nodes[i]));
     }
-    next = this->get_topleft_idx(i);
-    if (this->is_in_bound(next)) {
-      if (!this->boundaries.no_data(next)) {
-        out[n] = next;
-        ++n;
-      }
+
+    if (this->convergence_mode == CONVERGENCE::ALL ||
+        this->convergence_mode == CONVERGENCE::QWR) {
+      for (int i = 0; i < this->n_nodes_convergence(); ++i)
+        this->conv_Qr[i].emplace_back(this->_rec_Qwout[this->conv_nodes[i]] /
+                                      this->_Qw[this->conv_nodes[i]]);
     }
-    next = this->get_top_idx(i);
-    if (this->is_in_bound(next)) {
-      if (!this->boundaries.no_data(next)) {
-        out[n] = next;
-        ++n;
+
+    // Applying vmots with the right dt
+    this->_compute_vertical_motions(vmot_hw, vmot);
+  }
+
+  void init_Qw() {
+    // resetting Qwin (needed to be stored at all time)
+    this->_Qw = std::vector<fT>(this->graph->nnodes, 0.);
+
+    // resetting global monitors (low cost)
+    this->tot_Qw_input = 0;
+    this->tot_Qw_output = 0;
+    this->tot_Qwin_output = 0;
+
+    if (this->water_input_mode == WATER_INPUT::PRECIPITATIONS_CONSTANT ||
+        this->water_input_mode == WATER_INPUT::PRECIPITATIONS_VARIABLE) {
+      for (int i = 0; i < this->graph->nnodes; ++i) {
+        if (this->connector->boundaries.can_give(i) &&
+            this->connector->flow_out_or_pit(i) == false) {
+          this->_Qw[i] +=
+              this->precipitations(i) * this->connector->get_area_at_node(i);
+          this->tot_Qw_input += this->_Qw[i];
+        }
       }
-    }
-    next = this->get_topright_idx(i);
-    if (this->is_in_bound(next)) {
-      if (!this->boundaries.no_data(next)) {
-        out[n] = next;
-        ++n;
+    } else if (this->water_input_mode == WATER_INPUT::ENTRY_POINTS_H) {
+      for (size_t i = 0; i < this->_water_entries.size(); ++i) {
+        int node = this->_water_entry_nodes[i];
+        this->_Qw[node] +=
+            this->_water_entries[i] * this->connector->get_area_at_node(node);
+        this->tot_Qw_input += this->_Qw[node];
+        // std::cout << node << " is given " << this->_water_entries[i] *
+        // this->connector->get_area_at_node(node);
       }
     }
 
-    return n;
+    if (this->record_Qw_out)
+      this->_rec_Qwout = std::vector<fT>(this->graph->nnodes, 0.);
+
+    if (this->record_Sw)
+      this->_rec_Sw = std::vector<fT>(this->graph->nnodes, 0.);
+    if (this->record_dhw)
+      this->_rec_dhw = std::vector<fT>(this->graph->nnodes, 0.);
+
+    if (record_flowvec)
+      this->_rec_flowvec = std::vector<fT>(this->graph->nnodes * 2, 0.);
   }
 
-  int get_neighbour_idx_links(int i, std::vector<int> &out) {
-    int n = 0;
-    int next = this->get_right_idx_links(i);
-    if (next >= 0 && next < this->nnodes * 4) {
-      out[n] = next;
-      ++n;
-    }
-    next = this->get_bottomright_idx_links(i);
-    if (next >= 0 && next < this->nnodes * 4) {
-      out[n] = next;
-      ++n;
-    }
-    next = this->get_bottom_idx_links(i);
-    if (next >= 0 && next < this->nnodes * 4) {
-      out[n] = next;
-      ++n;
-    }
-    next = this->get_bottomleft_idx_links(i);
-    if (next >= 0 && next < this->nnodes * 4) {
-      out[n] = next;
-      ++n;
-    }
-    next = this->get_left_idx_links(i);
-    if (next >= 0 && next < this->nnodes * 4) {
-      out[n] = next;
-      ++n;
-    }
-    next = this->get_topleft_idx_links(i);
-    if (next >= 0 && next < this->nnodes * 4) {
-      out[n] = next;
-      ++n;
-    }
-    next = this->get_top_idx_links(i);
-    if (next >= 0 && next < this->nnodes * 4) {
-      out[n] = next;
-      ++n;
-    }
-    next = this->get_topright_idx_links(i);
-    if (next >= 0 && next < this->nnodes * 4) {
-      out[n] = next;
-      ++n;
+  void init_Qs() {
+    this->_Qs = std::vector<fT>(this->graph->nnodes, 0.);
+    if (this->sed_input_mode == SED_INPUT::ENTRY_POINTS_Q) {
+      for (size_t i = 0; i < this->_sed_entries.size(); ++i) {
+        int node = this->_sed_entry_nodes[i];
+        this->_Qs[node] += this->_sed_entries[i] * this->connector->dy;
+        // this->tot_Qw_input += this->_Qs[node];
+      }
     }
 
-    if (this->is_on_dem_edge(i)) {
-    }
+    // Initialising the Qs recorders
 
-    return n;
-  }
+    if (this->record_edot)
+      this->_rec_edot = std::vector<fT>(this->connector->nnodes, 0.);
 
-  int get_neighbour_idx_linknodes(int i, std::vector<int> &out) {
-    int n = 0;
-    int next = this->get_right_idx_linknodes(i);
-    if (next >= 0 && next < this->nnodes * 8) {
-      out[n] = next;
-      ++n;
-    }
-    next = this->get_bottomright_idx_linknodes(i);
-    if (next >= 0 && next < this->nnodes * 8) {
-      out[n] = next;
-      ++n;
-    }
-    next = this->get_bottom_idx_linknodes(i);
-    if (next >= 0 && next < this->nnodes * 8) {
-      out[n] = next;
-      ++n;
-    }
-    next = this->get_bottomleft_idx_linknodes(i);
-    if (next >= 0 && next < this->nnodes * 8) {
-      out[n] = next;
-      ++n;
-    }
-    next = this->get_left_idx_linknodes(i);
-    if (next >= 0 && next < this->nnodes * 8) {
-      out[n] = next;
-      ++n;
-    }
-    next = this->get_topleft_idx_linknodes(i);
-    if (next >= 0 && next < this->nnodes * 8) {
-      out[n] = next;
-      ++n;
-    }
-    next = this->get_top_idx_linknodes(i);
-    if (next >= 0 && next < this->nnodes * 8) {
-      out[n] = next;
-      ++n;
-    }
-    next = this->get_topright_idx_linknodes(i);
-    if (next >= 0 && next < this->nnodes * 8) {
-      out[n] = next;
-      ++n;
-    }
-    return n;
+    this->tot_Qs_output = 0.;
   }
 
-  int get_neighbour_idx_distance(int i, std::vector<std::pair<int, T>> &out) {
-    int n = 0;
-    int next = this->get_right_idx(i);
+  /// Automates the processing of the graph
+  /// Function of global parameters for flow topology, local minima management,
+  /// ...
+  void graph_automator() {
 
-    if (!this->boundaries.no_data(next) && this->is_in_bound(next)) {
-      out[n] = std::make_pair(next, this->dx);
-      ++n;
-    }
-    next = this->get_bottomright_idx(i);
-    if (!this->boundaries.no_data(next) && this->is_in_bound(next)) {
-      out[n] = std::make_pair(next, this->dxy);
-      ++n;
-    }
-    next = this->get_bottom_idx(i);
-    if (!this->boundaries.no_data(next) && this->is_in_bound(next)) {
-      out[n] = std::make_pair(next, this->dy);
-      ++n;
-    }
-    next = this->get_bottomleft_idx(i);
-    if (!this->boundaries.no_data(next) && this->is_in_bound(next)) {
-      out[n] = std::make_pair(next, this->dxy);
-      ++n;
-    }
-    next = this->get_left_idx(i);
-    if (!this->boundaries.no_data(next) && this->is_in_bound(next)) {
-      out[n] = std::make_pair(next, this->dx);
-      ++n;
-    }
-    next = this->get_topleft_idx(i);
-    if (!this->boundaries.no_data(next) && this->is_in_bound(next)) {
-      out[n] = std::make_pair(next, this->dxy);
-      ++n;
-    }
-    next = this->get_top_idx(i);
-    if (!this->boundaries.no_data(next) && this->is_in_bound(next)) {
-      out[n] = std::make_pair(next, this->dy);
-      ++n;
-    }
-    next = this->get_topright_idx(i);
-    if (!this->boundaries.no_data(next) && this->is_in_bound(next)) {
-      out[n] = std::make_pair(next, this->dxy);
-      ++n;
-    }
+    // is SS?
+    bool only_SD = (this->hydromode == HYDRO::GRAPH_SFD);
 
-    return n;
-  }
+    // making sure it has the right depression solver (SHOULD BE MOVED TO THE
+    // GRAPH MANAGEMENT LATER)
+    if (this->depression_management == HYDROGRAPH_LM::IGNORE)
+      this->graph->set_LMR_method(DEPRES::none);
 
-  int get_neighbour_idx_distance_links(int i,
-                                       std::vector<std::pair<int, T>> &out) {
-    int n = 0;
-    int next = this->get_right_idx_links(i);
-    if (next >= 0 && next < this->nnodes * 4) {
-      out[n] = std::make_pair(next, this->dx);
-      ++n;
-    }
-    next = this->get_bottomright_idx_links(i);
-    if (next >= 0 && next < this->nnodes * 4) {
-      out[n] = std::make_pair(next, this->dxy);
-      ++n;
-    }
-    next = this->get_bottom_idx_links(i);
-    if (next >= 0 && next < this->nnodes * 4) {
-      out[n] = std::make_pair(next, this->dy);
-      ++n;
-    }
-    next = this->get_bottomleft_idx_links(i);
-    if (next >= 0 && next < this->nnodes * 4) {
-      out[n] = std::make_pair(next, this->dxy);
-      ++n;
-    }
-    next = this->get_left_idx_links(i);
-    if (next >= 0 && next < this->nnodes * 4) {
-      out[n] = std::make_pair(next, this->dx);
-      ++n;
-    }
-    next = this->get_topleft_idx_links(i);
-    if (next >= 0 && next < this->nnodes * 4) {
-      out[n] = std::make_pair(next, this->dxy);
-      ++n;
-    }
-    next = this->get_top_idx_links(i);
-    if (next >= 0 && next < this->nnodes * 4) {
-      out[n] = std::make_pair(next, this->dy);
-      ++n;
+    if (this->record_filling)
+      this->_rec_filling = std::vector<fT>(this->graph->nnodes, 0.);
+
+    // preformatting post-topo
+    std::vector<fT> post_topo(this->_surface.size(), 0);
+    for (int i = 0; i < this->graph->nnodes; ++i) {
+      post_topo[i] = this->_surface[i];
     }
-    next = this->get_topright_idx_links(i);
-    if (next >= 0 && next < this->nnodes * 4) {
-      out[n] = std::make_pair(next, this->dxy);
-      ++n;
+
+    this->graph->_compute_graph(post_topo, only_SD, false);
+
+    // fill water where depressions have been solved
+    if (this->depression_management == HYDROGRAPH_LM::FILL) {
+      for (int i = 0; i < this->graph->nnodes; ++i) {
+        if (this->connector->boundaries.no_data(i) ||
+            this->connector->boundaries.forcing_io(i))
+          continue;
+
+        if (this->_surface[i] < post_topo[i]) {
+
+          fT ddhhee = post_topo[i] - this->_surface[i];
+
+          if (this->record_filling)
+            this->_rec_filling[i] = ddhhee;
+
+          this->_hw[i] += ddhhee;
+
+          this->_surface[i] = post_topo[i];
+        }
+      }
     }
-    return n;
   }
 
-  int get_neighbour_idx_distance_linknodes(
-      int i, std::vector<std::pair<int, T>> &out) {
-    int n = 0;
-    int next = this->get_right_idx_linknodes(i);
-    if (next >= 0 && next < this->nnodes * 8) {
-      out[n] = std::make_pair(next, this->dx);
-      ++n;
-    }
-    next = this->get_bottomright_idx_linknodes(i);
-    if (next >= 0 && next < this->nnodes * 8) {
-      out[n] = std::make_pair(next, this->dxy);
-      ++n;
-    }
-    next = this->get_bottom_idx_linknodes(i);
-    if (next >= 0 && next < this->nnodes * 8) {
-      out[n] = std::make_pair(next, this->dy);
-      ++n;
-    }
-    next = this->get_bottomleft_idx_linknodes(i);
-    if (next >= 0 && next < this->nnodes * 8) {
-      out[n] = std::make_pair(next, this->dxy);
-      ++n;
-    }
-    next = this->get_left_idx_linknodes(i);
-    if (next >= 0 && next < this->nnodes * 8) {
-      out[n] = std::make_pair(next, this->dx);
-      ++n;
-    }
-    next = this->get_topleft_idx_linknodes(i);
-    if (next >= 0 && next < this->nnodes * 8) {
-      out[n] = std::make_pair(next, this->dxy);
-      ++n;
-    }
-    next = this->get_top_idx_linknodes(i);
-    if (next >= 0 && next < this->nnodes * 8) {
-      out[n] = std::make_pair(next, this->dy);
-      ++n;
-    }
-    next = this->get_topright_idx_linknodes(i);
-    if (next >= 0 && next < this->nnodes * 8) {
-      out[n] = std::make_pair(next, this->dxy);
-      ++n;
+  // initial check for boundary conditions and eventually applying relevant
+  // changes
+  bool _initial_check_boundary_pit(int &node, std::array<int, 8> &receivers,
+                                   std::vector<fT> &vmot_hw) {
+    if (this->connector->boundaries.no_data(node) ||
+        this->connector->flow_out_or_pit(node) ||
+        (this->hydrostationary == false && this->_hw[node] == 0 &&
+         this->_Qw[node] == 0)) {
+      // Checking mass conservations
+      this->tot_Qwin_output += this->_Qw[node];
+
+      // I encountered a pit, that happened when LM are not preprocessed
+      // Then I fill it slightly, but it does not really work
+      if (this->connector->flow_out_model(node) == false &&
+          this->connector->boundaries.no_data(node) == false) {
+        // int nn = this->connector->get_neighbour_idx(node,receivers);
+        // fT hzh = this->_surface[node];
+        // for(int j=0; j < nn; ++j)
+        // {
+        // 	if(this->_surface[receivers[j]] > hzh)
+        // 		hzh = this->_surface[receivers[j]];
+        // }
+        vmot_hw[node] =
+            this->_Qw[node] / this->connector->get_area_at_node(node);
+        // if(vmot_hw[node]>0)
+        // {
+        // 	std::cout << this->_Qw[node] << "??::" << vmot_hw[node] *
+        // this->dt_hydro(node) << " ||| " << this->dt_hydro(node) <<
+        // std::endl;; 	if(vmot_hw[node]> 1e6) 		throw
+        // std::runtime_error("flkflsdfkjdsf");
+        // }
+        // vmot_hw[node] += hzh - this->_surface[node];
+      }
+      return true;
     }
-    return n;
+    return false;
   }
 
-  // Takes a node index as input and a normalised displacement in the X and Y
-  // direction (between -1 and 1) Returns the neighbouring node in the given
-  // direction
-  template <class ii_t>
-  ii_t get_neighbour_idx_from_normalised_dxdy(ii_t node, T normdx, T normdy) {
-    if (normdx >= 0.5) {
-      if (normdy <= -0.5)
-        return this->get_topright_idx(node);
-      else if (normdy <= 0.5)
-        return this->get_right_idx(node);
-      else
-        return this->get_bottomright_idx(node);
-    } else if (normdx >= -0.5) {
-      if (normdy <= 0)
-        return this->get_top_idx(node);
-      else
-        return this->get_bottom_idx(node);
+  // offsetting some of the calculations from the run to make it more
+  // undertandable adn reusable
+  void _compute_slopes_weights_et_al(int &node, bool &SF, fT &Smax,
+                                     std::array<fT, 8> &slopes,
+                                     std::array<fT, 8> &weights, int &nrecs,
+                                     std::array<int, 8> &receivers, int &recmax,
+                                     fT &dx, fT &dw0max,
+                                     fT &topological_number_v2) {
+    // Calculating the slopes/weights and topological numbers
+    if (SF == false) {
+
+      // ROUTINES FOR Multiple FLow Directions
+      // fill the arrays of slopes/weights/.. and calculate Smax, dmax, recmas
+      // and all
+      Smax =
+          this->weights_automator_v2(receivers, weights, slopes, node, nrecs,
+                                     topological_number_v2, dw0max, recmax, dx);
+
+      // Debugging, I guess deprecated TODO::CHECK
+      if (topological_number_v2 == 0) {
+        topological_number_v2 = 1.;
+      }
+
+      // Check the recording of topological number
+      if (this->debugntopo) {
+        this->DEBUGNTOPO[node] = topological_number_v2;
+      }
+
     } else {
-      if (normdy <= -0.5)
-        return this->get_topleft_idx(node);
-      else if (normdy < 0.5)
-        return this->get_left_idx(node);
-      else
-        return this->get_bottomleft_idx(node);
-    }
-  }
 
-  // get receivers of node i and put them in the recs vector fed in
-  // It returns the number of receivers in the recs vector
-  // THis whole process optimises repeated receiver fetching, by never
-  // reallocating/initialising the vector recs
-  int get_receivers_idx(int i, std::vector<int> &recs) {
-    // getting the related links stroing them temporarily in the rec vec
-    int nli = this->get_neighbour_idx_links(i, recs);
-
-    // going through the linksß
-    // The idx is the idx of insertion in the recs vectors
-    // the idx of insertion is always <= of the index of reading (both receivers
-    // and links-to-assess are stored in the recs vector)
-    int idx = 0;
-    // counter used to keep track of the number of receivers: starts at the
-    // number of links related to the given node and get decremented at each
-    // donor link
-    int newli = nli;
-
-    // Iterating through the links
-    for (int ti = 0; ti < nli; ++ti) {
-      // current link index
-      int li = recs[ti];
-
-      // this link is a rec if the node is the first of the linknode and links
-      // is true
-      if (i == this->linknodes[li * 2] && this->links[li] == 1) {
-        // in which case the receiver of the current node is the +  1
-        recs[idx] = this->linknodes[li * 2 + 1];
-        ++idx;
-      }
-      // OR if the current node is the +1 and the links false
-      else if (this->links[li] == 0 && i == this->linknodes[li * 2 + 1]) {
-        // in which case the receivers is the 0 node
-        recs[idx] = this->linknodes[li * 2];
-        ++idx;
-      } else {
-        // otherwise, it's not a rec and we decrease the newli
-        --newli;
+      // ROUTINES FOR Single FLow Directions
+      // -> Slope
+      Smax = this->get_Sw(node, this->connector->_Sreceivers[node],
+                          this->connector->Sdistance2receivers[node],
+                          this->minslope);
+      // -> rec
+      recmax = this->connector->_Sreceivers[node];
+      // -> dy (integrated width)
+      dw0max = this->connector->get_travers_dy_from_dx(
+          this->connector->Sdistance2receivers[node]);
+      // -> dx (flow distance)
+      dx = this->connector->Sdistance2receivers[node];
+
+      // boundary case
+      if (this->connector->flow_out_model(recmax) &&
+          this->boundhw == BOUNDARY_HW::FIXED_SLOPE) {
+        dw0max = this->connector->dy;
+        Smax = this->bou_fixed_val;
+        dx = this->connector->dx;
+      }
+    }
+
+    // I can only have an hydraulic slope if I have water
+    if (this->_hw[node] == 0)
+      Smax = 0;
+
+    // Done
+  }
+
+  void _compute_morpho(int &node, int &recmax, fT &dx, fT &Smax,
+                       std::vector<fT> &vmot) {
+    if (this->morphomode != MORPHO::NONE &&
+        this->connector->boundaries.forcing_io(node) == false) {
+
+      // precaching rates
+      fT edot = 0., ddot = 0., eldot_A = 0., eldot_B = 0., dldot_A = 0.,
+         dldot_B = 0.;
+
+      // Lateral dx for lat e/d
+      fT dy = this->connector->get_travers_dy_from_dx(dx);
+
+      // And gathering the orthogonal nodes
+      std::pair<int, int> orthonodes =
+          this->connector->get_orthogonal_nodes(node, recmax);
+
+      // Calculating sheer stress
+      fT tau = this->rho(node) * this->_hw[node] * GRAVITY * Smax;
+
+      if (tau > tau_max)
+        this->tau_max = tau;
+
+      // if(tau>150)
+      // 	tau = 150;
+
+      // Double checking the orthogonal nodes and if needs be to process them
+      // (basically if flow outs model or has boundary exceptions)
+      int oA = orthonodes.first;
+      if (this->connector->boundaries.forcing_io(oA) ||
+          this->connector->is_in_bound(oA) == false ||
+          this->connector->boundaries.no_data(oA) ||
+          this->connector->flow_out_model(oA))
+        oA = -1;
+      int oB = orthonodes.second;
+      if (this->connector->boundaries.forcing_io(oB) ||
+          this->connector->is_in_bound(oB) == false ||
+          this->connector->boundaries.no_data(oB) ||
+          this->connector->flow_out_model(oB))
+        oB = -1;
+
+      // Calculating erosion if sheer stress is above critical
+      if (tau > this->tau_c(node)) {
+        // Basal erosion rates
+        edot = this->ke(node) *
+               std::pow(tau - this->tau_c(node), this->aexp(node));
+        // if recording stuff
+        if (this->record_edot)
+          this->_rec_edot[node] += edot;
+      }
+
+      // Claculating the deposition rates
+      ddot = this->_Qs[node] / this->kd(node);
+
+      // Dealing with lateral deposition if lS > 0 and erosion if lS <0
+      if (oA >= 0) {
+        fT tSwl = this->get_Stopo(node, oA, dy);
+        if (tSwl > 0) {
+          dldot_A = tSwl * this->kd_lateral(node) * ddot;
+        } else {
+          eldot_A = std::abs(tSwl) * this->ke_lateral(node) * edot;
+        }
+      }
+
+      if (oB >= 0) {
+        fT tSwl = this->get_Stopo(node, oB, dy);
+        if (tSwl > 0) {
+          dldot_B = tSwl * this->kd_lateral(node) * ddot;
+        } else {
+          eldot_B = std::abs(tSwl) * this->ke_lateral(node) * edot;
+        }
+      }
+
+      // Am I depositing more than I can chew?
+      fT totdqs = dx * (dldot_B + dldot_A + ddot);
+      if (totdqs > this->_Qs[node]) {
+        // std::cout << " happens??? " << totdqs;
+        fT corrqs = this->_Qs[node] / totdqs;
+        dldot_B *= corrqs;
+        dldot_A *= corrqs;
+        ddot *= corrqs;
+      }
+      fT sqs = this->_Qs[node];
+      fT fbatch = (ddot + dldot_B + dldot_A - edot - eldot_A - eldot_B) * dx;
+      this->_Qs[node] -= fbatch;
+      if (std::isfinite(this->_Qs[node]) == false) {
+        std::cout << "QS NAN:" << this->_Qs[node] << " vs " << sqs << std::endl;
+        throw std::runtime_error("BITE");
+      }
+
+      if (this->_Qs[node] < 0) {
+        this->_Qs[node] = 0;
+      }
+
+      vmot[node] += ddot - edot;
+      if (oA >= 0) {
+        vmot[oA] += dldot_A;
+        vmot[oA] -= eldot_A;
+      }
+      if (oB >= 0) {
+        vmot[oB] += dldot_B;
+        vmot[oB] -= eldot_B;
+      }
+
+      if (std::isfinite(vmot[node]) == false) {
+        std::cout << "edot:" << edot << " ddot" << ddot << std::endl;
+        std::cout << "qs:" << sqs << " tau" << tau << std::endl;
+        throw std::runtime_error("Non finite vmot");
       }
     }
-    // recs is changed in place, and we return the number of recs newli
-    return newli;
   }
 
-  // Getting the id of the receivers in the links array
-  // see get_receivers_idx for full comments about the section
-  int get_receivers_idx_links(int i, std::vector<int> &recs) {
-    // getting the related links
-    int nli = this->get_neighbour_idx_links(i, recs);
-
-    // going through the linksß
-    int idx = 0;
-    int newli = nli;
-
-    for (int ti = 0; ti < nli; ++ti) {
-      // checking the orientation
-      int li = recs[ti];
-      if (i == this->linknodes[li * 2] && this->links[li]) {
-        recs[idx] = li;
-        ++idx;
-      } else if (this->links[li] == 0 && i == this->linknodes[li * 2 + 1]) {
-        recs[idx] = li;
-        ++idx;
+  void _compute_transfers(int &nrecs, int &recmax, int &node, bool &SF,
+                          std::array<int, 8> &receivers,
+                          std::array<fT, 8> &weights, fT &Qwin, fT &Qwout) {
+    // going through the receiver(s)
+    for (int j = 0; j < nrecs; ++j) {
+
+      // Hydro for the link
+      // universal params
+      int rec;
+      if (SF)
+        rec = recmax;
+      else
+        rec = this->connector->get_to_links(receivers[j]);
+
+      if (rec < 0)
+        continue;
+
+      if (this->connector->flow_out_model(rec)) {
+        if (SF) {
+          this->tot_Qw_output += Qwout;
+        } else if (weights[j] > 0 && Qwin > 0) {
+          this->tot_Qw_output += weights[j] * Qwout;
+        }
+      }
+
+      if (this->hydrostationary) {
+        if (SF) {
+          this->_Qw[rec] += Qwin;
+        } else if (weights[j] > 0 && Qwin > 0) {
+          this->_Qw[rec] += weights[j] * Qwin;
+        }
+
       } else {
-        --newli;
+        // this->_Qw[rec] += std::min(Qwout * weights[j], Qwin * weights[j]);
+        if (SF)
+          this->_Qw[rec] += Qwout;
+        else
+          this->_Qw[rec] += Qwout * weights[j];
+        // std::cout << "transferring:" << Qwout << std::endl;
+      }
+
+      if (this->morphomode != MORPHO::NONE) {
+        if (std::isfinite(this->_Qs[node]) == false)
+          throw std::runtime_error("QS NAN");
+        if (std::isfinite(this->_Qs[rec]) == false)
+          throw std::runtime_error("QSREC NAN");
+        this->_Qs[rec] +=
+            (SF == false) ? weights[j] * this->_Qs[node] : this->_Qs[node];
+        if (std::isfinite(this->_Qs[rec]) == false) {
+          std::cout << weights[j] << std::endl;
+          ;
+          throw std::runtime_error("QSREC NAN AFTER");
+        }
       }
     }
-    return newli;
   }
 
-  int get_nth_steepest_donors_of_node(int node, int j) {
-    return this->Sdonors[node * this->nneighbours + j];
-  }
+  void _compute_vertical_motions(std::vector<fT> &vmot_hw,
+                                 std::vector<fT> &vmot, bool use_dt = true) {
 
-  // Getting donor indicies
-  // see get_receivers_idx for full comments about the section
-  int get_donors_idx(int i, std::vector<int> &dons) {
-    // getting the related links
-    int nli = this->get_neighbour_idx_links(i, dons);
+    for (int i = 0; i < this->graph->nnodes; ++i) {
 
-    // going through the links
-    int idx = 0;
-    int newli = nli;
+      if (this->connector->flow_out_model(i) &&
+          this->boundhw == BOUNDARY_HW::FIXED_HW)
+        this->_hw[i] = this->bou_fixed_val;
 
-    for (int ti = 0; ti < nli; ++ti) {
-      // checking the orientation
-      int li = dons[ti];
-      if (i == this->linknodes[li * 2] && this->links[li] == 0) {
-        dons[idx] = this->linknodes[li * 2 + 1];
-        ++idx;
-      } else if (this->links[li] == 1 && i == this->linknodes[li * 2 + 1]) {
-        dons[idx] = this->linknodes[li * 2];
-        ++idx;
-      } else {
-        --newli;
+      if (this->connector->boundaries.forcing_io(i))
+        continue;
+
+      fT tvh = vmot_hw[i];
+      if (use_dt) {
+        tvh *= this->dt_hydro(i);
+        // std::cout << this->dt_hydro(i) << std::endl;
+      }
+      if (tvh < -this->_hw[i]) {
+        tvh = -this->_hw[i];
       }
+
+      this->_hw[i] += tvh;
+      if (this->record_dhw)
+        this->_rec_dhw[i] = tvh;
+
+      this->_surface[i] += tvh;
+
+      if (this->morphomode != MORPHO::NONE)
+        this->_surface[i] += vmot[i] * this->dt_morpho(i);
+
+      if (this->_hw[i] < 0)
+        throw std::runtime_error("hw < 0???");
     }
-    return newli;
   }
 
-  // getting links indices of hte donors (in the links array)
-  // see get_receivers_idx for full comments about the section
-  int get_donors_idx_links(int i, std::vector<int> &dons) {
-    // getting the related links
-    int nli = this->get_neighbour_idx_links(i, dons);
-
-    // going through the linksß
-    int idx = 0;
-    int newli = nli;
-
-    for (int ti = 0; ti < nli; ++ti) {
-      // checking the orientation
-      int li = dons[ti];
-      if (i == this->linknodes[li * 2] && this->links[li] == 0) {
-        dons[idx] = li;
-        ++idx;
-      } else if (this->links[li] == 1 && i == this->linknodes[li * 2 + 1]) {
-        dons[idx] = li;
-        ++idx;
-      } else {
-        --newli;
+  void _compute_vertical_motions_averaged_test(std::vector<fT> &vmot_hw,
+                                               std::vector<fT> &vmot,
+                                               bool use_dt = true) {
+
+    for (int i = 0; i < this->graph->nnodes; ++i) {
+
+      if (this->connector->flow_out_model(i) &&
+          this->boundhw == BOUNDARY_HW::FIXED_HW)
+        this->_hw[i] = this->bou_fixed_val;
+
+      if (this->connector->boundaries.forcing_io(i))
+        continue;
+
+      fT tvh = vmot_hw[i];
+      if (use_dt) {
+        tvh *= this->dt_hydro(i);
+        // std::cout << this->dt_hydro(i) << std::endl;
       }
+      if (tvh < -this->_hw[i]) {
+        tvh = -this->_hw[i];
+      }
+
+      fT newhw = this->_hw[i] + tvh;
+      fT prevhw = this->_hw[i];
+      this->_hw[i] = (this->_hw[i] + newhw) / 2;
+
+      if (this->record_dhw)
+        this->_rec_dhw[i] = tvh;
+
+      this->_surface[i] += newhw - prevhw;
+
+      if (this->morphomode != MORPHO::NONE)
+        this->_surface[i] += vmot[i] * this->dt_morpho(i);
+
+      if (this->_hw[i] < 0)
+        throw std::runtime_error("hw < 0???");
     }
-    return newli;
   }
 
-  // Debug function printing to the prompt the single receiver of a node
-  // Will probably get deprecated
-  std::vector<int> get_rowcol_Sreceivers(int row, int col) {
-    int node = this->nodeid_from_row_col(row, col);
-    std::vector<int> out_receivers;
-    int trow, tcol;
-    this->rowcol_from_node_id(this->Sreceivers[node], trow, tcol);
-    out_receivers = std::vector<int>{trow, tcol};
-
-    std::cout << "Srec is " << this->Sreceivers[node] << " node was " << node
-              << std::endl;
-    return out_receivers;
-  }
-
-  template <class topo_t> void print_receivers(int i, topo_t &ttopography) {
-    std::cout << std::setprecision(12);
-    auto topography = format_input<topo_t>(ttopography);
-
-    auto receivers = this->get_empty_neighbour();
-    int nn = this->get_receivers_idx(i, receivers);
-
-    std::cout << "Topography is " << topography[i] << "# receivers: " << nn
-              << std::endl;
-    for (int tr = 0; tr < nn; ++tr) {
-      int r = receivers[tr];
-      int row, col;
-      this->rowcol_from_node_id(r, row, col);
-      std::cout << "Rec " << r << " row " << row << " col " << col << " topo "
-                << topography[r] << std::endl;
-    }
-
-    auto neighbours = this->get_empty_neighbour();
-    nn = this->get_neighbour_idx(i, neighbours);
-    std::cout << "Neighbours are :" << std::endl;
-
-    for (int tr = 0; tr < nn; ++tr) {
-      int r = neighbours[tr];
-      int row, col;
-      this->rowcol_from_node_id(r, row, col);
-      std::cout << "Neighbour " << r << " row " << row << " col " << col
-                << " topo " << topography[r] << std::endl;
-    }
-  }
-
-  // Returns the number of links stored in the graph
-  // Note that it comprises some unvalid linked!
-  int get_rec_array_size() { return int(this->links.size()); }
-
-  /// Takes an array of nnodes size and sum the values at the outlets
-  /// This can be useful for checking mass balances for example
-  /// if true, include_internal_pits allow the code to add internal unprocessed
-  /// pits, wether they are on purpose or not
-  template <class array_t, class U>
-  U sum_at_outlets(array_t &tarray, bool include_internal_pits = true) {
-    std::cout << "DEPRECATION WARNING::sum_at_outlets::should be moved as a "
-                 "standalone algorithm"
-              << std::endl;
-    auto array = format_input<array_t>(tarray);
-    U out = 0;
-    for (int i = 0; i < this->nnodes; ++i) {
-      if (this->Sreceivers[i] == i) {
-        if (include_internal_pits) {
-          out += array[i];
-        } else if (this->flow_out_model(i)) {
-          out += array[i];
-        }
+  fT weights_automator_v2(std::array<int, 8> &receivers,
+                          std::array<fT, 8> &weights, std::array<fT, 8> &slopes,
+                          int &node, int &nrecs, fT &topological_number_v2,
+                          fT &dw0max, int &recmax, fT &dx) {
+
+    // Placeholders
+    fT sumw = 0., Smax = this->minslope, sumSdw = 0.;
+    ;
+    std::pair<fT, fT> fvech;
+
+    for (int i = 0; i < nrecs; ++i) {
+      int lix = receivers[i];
+
+      if (this->connector->is_link_valid(lix) == false) {
+        continue;
       }
+
+      // int_dw += this->connector->get_dx_from_links_idx(lix);
+      fT tdw = this->connector->get_traverse_dx_from_links_idx(lix);
+      int rec = this->connector->get_to_links(lix);
+      bool isboud = false;
+      if (this->connector->flow_out_or_pit(rec) &&
+          this->boundhw == BOUNDARY_HW::FIXED_SLOPE) {
+        slopes[i] = this->bou_fixed_val;
+        tdw = this->connector->dy;
+        isboud = true;
+      } else
+        slopes[i] = this->get_Sw(lix, this->minslope);
+
+      sumSdw += slopes[i] * tdw;
+
+      if (this->record_flowvec) {
+        this->connector->get_dxdy_from_links_idx(lix, node, fvech, false);
+        this->_rec_flowvec[node * 2] += slopes[i] * tdw * fvech.first;
+        this->_rec_flowvec[node * 2 + 1] += slopes[i] * tdw * fvech.second;
+      }
+
+      if (slopes[i] > Smax) {
+        Smax = slopes[i];
+        dw0max = tdw;
+        dx = (isboud) ? this->connector->dx
+                      : this->connector->get_dx_from_links_idx(lix);
+        recmax = rec;
+      }
+
+      // // slopes[i] = slope;
+      // if(this->stochaslope)
+      // 	weights[i] = this->randu.get();
+
+      if (this->weight_management == MFD_PARTITIONNING::PROPOSLOPE)
+        weights[i] = slopes[i] * tdw;
+
+      else if (this->weight_management == MFD_PARTITIONNING::SQRTSLOPE)
+        weights[i] = std::sqrt(slopes[i] * tdw);
+
+      else if (this->weight_management == MFD_PARTITIONNING::PROPOREC)
+        weights[i] = 1.;
+
+      if (this->stochaslope)
+        weights[i] += this->stochaslope_coeff * this->randu.get();
+
+      sumw += weights[i];
+    }
+
+    fT sumf = 0.;
+    for (int i = 0; i < nrecs; ++i) {
+      int lix = receivers[i];
+
+      if (this->connector->is_link_valid(lix) == false)
+        continue;
+
+      if (sumw > 0)
+        weights[i] = weights[i] / sumw;
+      else
+        weights[i] = 1 / nrecs;
+
+      sumf += weights[i];
     }
-    return out;
-  }
 
-  /// Takes an array of nnodes size and sum the values at the outlets
-  /// This can be useful for checking mass balances for example
-  /// if true, include_internal_pits allow the code to add internal unprocessed
-  /// pits, wether they are on purpose or not
-  template <class array_t, class out_t>
-  out_t keep_only_at_outlets(array_t &tarray,
-                             bool include_internal_pits = true) {
-    auto array = format_input<array_t>(tarray);
-    std::vector<T> out = std::vector<T>(this->nnodes, 0);
-    for (int i = 0; i < this->nnodes; ++i) {
-      if (this->Sreceivers[i] == i) {
-        if (include_internal_pits)
-          out[i] = array[i];
-        else if (this->flow_out_model(i))
-          out[i] = array[i];
+    if (this->record_flowvec) {
+
+      fT length = std::sqrt(std::pow(this->_rec_flowvec[node * 2], 2) +
+                            std::pow(this->_rec_flowvec[node * 2 + 1], 2));
+      if (length != 0) {
+        this->_rec_flowvec[node * 2] /= length;
+        this->_rec_flowvec[node * 2 + 1] /= length;
       }
     }
-    return format_output<decltype(out), out_t>(out);
-  }
 
-  // Checks the validity of a link
-  // Invalid links have a linknode value of -1
-  template <class ti_t> bool is_link_valid(ti_t i) {
-    return (this->links[i] == 2) ? false : true;
+    topological_number_v2 = (Smax * dw0max) / sumSdw;
+
+    return Smax;
   }
 
-  // return true is the node is active: i.e. flow transfer through it
-  // reflects the connector version of the function, but adds extra graph
-  // specific checks. For example a node with permissive outletting border will
-  // be active in the connector sense, but can be inactive in the graph if it
-  // has no downstream neighbours.
-  template <class ti_t> bool flow_out_model(ti_t node) {
+  void init_convergence_checker(int tN, CONVERGENCE conv) {
 
-    bool con_val = this->boundaries.can_out(node);
-    if (con_val && this->Sreceivers[node] == int(node))
-      return true;
-    return false;
-  }
+    this->conv_nodes.clear();
+    this->conv_ini_Qw.clear();
+    this->conv_Qr.clear();
+    this->conv_dhw.clear();
+    this->converged.clear();
 
-  template <class ti_t> bool is_pit(ti_t node) {
+    this->convergence_mode = conv;
 
-    bool con_val = this->boundaries.can_out(node);
-    if (!con_val && this->Sreceivers[node] == int(node))
-      return true;
-    return false;
-  }
+    // init convergence vectors to the right size
+    this->conv_nodes.reserve(tN);
+    this->conv_ini_Qw.reserve(tN);
+    this->converged.reserve(tN);
 
-  template <class ti_t> bool flow_out_or_pit(ti_t node) {
-    if (this->Sreceivers[node] == int(node))
-      return true;
-    return false;
+    if (this->convergence_mode == CONVERGENCE::QWR ||
+        this->convergence_mode == CONVERGENCE::ALL)
+      this->record_Qw_out = true;
+
+    // Calculating relevant metrics
+    auto DA = this->calculate_drainage_area();
+    auto FD = this->calculate_flow_distance();
+
+    // finding the longest flow line
+    auto maxElement = std::max_element(FD.begin(), FD.end());
+    int ti = std::distance(FD.begin(), maxElement);
+
+    std::vector<int> flow_line;
+    flow_line.reserve(this->connector->nnodes);
+
+    while (this->connector->flow_out_or_pit(ti) == false) {
+      flow_line.emplace_back(ti);
+      ti = this->connector->_Sreceivers[ti];
+    }
+    // std::cout << "Last node is " << ti << std::endl;
+
+    if (this->connector->flow_out_model(ti) == false)
+      std::cout << "WARNING::convergence checker flow line ends in a pit, this "
+                   "can impact its liability"
+                << std::endl;
+
+    int nflodes = static_cast<int>(flow_line.size());
+    fT step = static_cast<fT>(nflodes) / tN;
+    if (step == 0)
+      throw std::runtime_error("cannot init convergence checker: Nnodes bigger "
+                               "than the size of the biggest flow line");
+
+    // std::cout << "nflodes is " << nflodes << " step is " << step <<
+    // std::endl;
+
+    fT tstep = 0;
+    while (conv_nodes.size() < tN &&
+           tstep < static_cast<fT>(flow_line.size())) {
+      // std::cout << tstep << " vs " << flow_line.size();
+      int node = flow_line[std::floor(tstep)];
+      // std::cout << " and node is " << node << std::endl;
+      this->conv_nodes.emplace_back(node);
+      this->conv_ini_Qw.emplace_back(DA[node]);
+      tstep += step;
+    }
+
+    std::cout << "Lest tstep is " << tstep << std::endl;
+
+    if (this->n_nodes_convergence() == tN - 1) {
+      this->conv_nodes.emplace_back(flow_line.back());
+      this->conv_ini_Qw.emplace_back(DA[flow_line.back()]);
+    }
+
+    if (this->convergence_mode == CONVERGENCE::ALL ||
+        this->convergence_mode == CONVERGENCE::QWR)
+      this->conv_Qr = std::vector<std::vector<fT>>(tN);
+    if (this->convergence_mode == CONVERGENCE::ALL ||
+        this->convergence_mode == CONVERGENCE::DHW)
+      this->conv_dhw = std::vector<std::vector<fT>>(tN);
   }
 
-  // Returns the pair of node making a link, starting from the donor to the
-  // receiver
-  template <class ti_t> std::pair<ti_t, ti_t> get_from_to_links(ti_t i) {
-    if (this->links[i] == 1)
-      return std::make_pair(this->linknodes[i * 2], this->linknodes[i * 2 + 1]);
-    else if (this->links[i] == 0)
-      return std::make_pair(this->linknodes[i * 2 + 1], this->linknodes[i * 2]);
-    else
-      return {-1, -1};
+  template <class out_t> out_t get_conv_nodes() {
+    return DAGGER::format_output<std::vector<int>, out_t>(this->conv_nodes);
   }
 
-  template <class ti_t>
-  void get_from_to_links(ti_t i, std::pair<ti_t, ti_t> &fromto) {
-    if (this->links[i] == 1) {
-      fromto.first = this->linknodes[i * 2];
-      fromto.second = this->linknodes[i * 2 + 1];
-    } else if (this->links[i] == 2) {
-      fromto.first = this->linknodes[i * 2 + 1];
-      fromto.second = this->linknodes[i * 2];
-    } else
-      fromto = {-1, -1};
+  template <class out_t> out_t get_conv_ini_Qw() {
+    return DAGGER::format_output<std::vector<fT>, out_t>(this->conv_ini_Qw);
   }
 
-  template <class ti_t> ti_t get_from_links(ti_t i) {
-    if (this->links[i] == 1)
-      return this->linknodes[i * 2];
-    else if (this->links[i] == 0)
-      return this->linknodes[i * 2 + 1];
-    else
-      return -1;
+  std::vector<fT> calculate_drainage_area() {
+
+    // Graph Processing (SFD will be calculated whatsoever)
+    this->graph_automator();
+    return this->graph->_accumulate_constant_downstream_SFD(
+        this->connector->get_area_at_node(0));
   }
 
-  template <class ti_t> ti_t get_to_links(ti_t i) {
-    if (this->links[i] == 0)
-      return this->linknodes[i * 2];
-    else if (this->links[i] == 1)
-      return this->linknodes[i * 2 + 1];
-    else
-      return -1;
+  std::vector<fT> calculate_flow_distance() {
+    std::vector<fT> FD(this->graph->nnodes, 0.);
+    this->graph->_get_SFD_distance_from_outlets(FD);
+    return FD;
   }
 
-  template <class ti_t> ti_t get_other_node_from_links(ti_t li, ti_t ni) {
-    if (this->linknodes[li * 2 + 1] == ni)
-      return this->linknodes[li * 2];
-    else if (this->linknodes[li * 2] == ni)
-      return this->linknodes[li * 2 + 1];
-    else
-      return -1;
+  template <class out_t> out_t get_conv_mean_Qr(int n_n) {
+    auto temp = this->_get_conv_mean_Qr(n_n);
+    return DAGGER::format_output<std::vector<fT>, out_t>(temp);
   }
 
-  std::vector<int> get_n_receivers() {
-    std::vector<int> nrecs(this->nnodes, 0);
-    for (size_t i = 0; i < this->links.size(); ++i) {
-      if (this->is_link_valid(i)) {
-        auto frto = this->get_from_to_links(i);
-        ++nrecs[frto.first];
-      }
+  std::vector<fT> _get_conv_mean_Qr(int n_n) {
+    std::vector<fT> out(this->n_nodes_convergence(), 0.);
+    n_n = std::min(static_cast<int>(this->n_stack_convergence()), n_n);
+    if (n_n == 0)
+      return out;
+
+    for (int i = 0; i < this->n_nodes_convergence(); ++i) {
+      out[i] = this->__get_conv_mean_Qr(i, n_n);
     }
-    return nrecs;
+    return out;
   }
 
-  template <class out_t> out_t get_SFD_receivers() {
-    return format_output<std::vector<int>, out_t>(this->Sreceivers);
+  fT __get_conv_mean_Qr(int i, int n_n) {
+    fT mean = 0;
+    for (int j = static_cast<int>(this->conv_Qr[0].size()) - n_n;
+         j < static_cast<int>(this->conv_Qr[0].size()); ++j)
+      mean += this->conv_Qr[i][j];
+    mean /= n_n;
+    return mean;
+  }
+
+  template <class out_t> out_t get_conv_mean_dhw(int n_n) {
+    auto temp = this->_get_conv_mean_dhw(n_n);
+    return DAGGER::format_output<std::vector<fT>, out_t>(temp);
+  }
+
+  std::vector<fT> _get_conv_mean_dhw(int n_n) {
+    std::vector<fT> out(this->n_nodes_convergence(), 0.);
+    n_n = std::min(static_cast<int>(this->n_stack_convergence()), n_n);
+    if (n_n == 0)
+      return out;
+    for (int i = 0; i < this->n_nodes_convergence(); ++i) {
+      out[i] = this->__get_conv_mean_dhw(i, n_n);
+    }
+    return out;
   }
 
-  template <class out_t> out_t get_SFD_dx() {
-    return format_output<std::vector<T>, out_t>(this->Sdistance2receivers);
-  }
+  fT __get_conv_mean_dhw(int i, int n_n) {
+    fT mean = 0;
+    for (int j = static_cast<int>(this->conv_dhw[0].size()) - n_n;
+         j < static_cast<int>(this->conv_dhw[0].size()); ++j)
+      mean += this->conv_dhw[i][j];
+    mean /= n_n;
+    return mean;
+  }
+
+  void catch_nan(fT testval, std::string error_message) {
+    if (std::isfinite(testval) == false)
+      throw std::runtime_error(error_message);
+  }
+
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  //~=~=~=~= Topographic Analysis ~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  // _      _      _      _      _      _      _      _
+  // )`'-.,_)`'-.,_)`'-.,_)`'-.,_)`'-.,_)`'-.,_)`'-.,_)`'-.,_
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+
+  // computes u, q or Q
+  // dim: 1,2 or 3
+  template <class out_t> out_t compute_tuqQ(int dimensions) {
+    if (dimensions < 0 || dimensions > 3)
+      throw std::runtime_error(
+          "Invalid number of dimensions. Needs to be 0 for the topological "
+          "number (dfimensionless coefficient of paritionning), 1 (velocity in "
+          "m/s), 2 (discharge per unit width in m^2/s) or 3 (volumetric "
+          "discarghe in m^3/s)");
+
+    // Graph Processing
+    this->graph_automator();
+
+    // Initialise the water discharge fields according to water input condition
+    // and other monitoring features:
+    this->init_Qw();
+
+    // Am I in SFD or MFD
+    bool SF = (this->hydromode == HYDRO::GRAPH_SFD);
+
+    // Vertical motions are applied at the end of the timestep
+    std::vector<fT> out(this->graph->nnodes, 0.);
+
+    // Caching neighbours, slopes and weights
+    auto receivers = this->connector->get_empty_neighbour();
+    std::array<fT, 8> weights, slopes;
+
+    // main loop
+    for (int i = this->graph->nnodes - 1; i >= 0; --i) {
+
+      // Getting next node in line
+      int node = this->get_istack_node(i);
+
+      // Processing case where the node is a model edge, or no data
+      // this function  returns true if the node was boundary and does not need
+      // to be processed THis is where all the boundary treatment happens, if
+      // you need to add something happening at the boundaries
+      if (this->_initial_check_boundary_pit(node, receivers))
+        continue;
 
-  template <class out_t> out_t get_SFD_ndonors() {
-    return format_output<std::vector<int>, out_t>(this->nSdonors);
-  }
+      // Getting the receivers
+      int nrecs;
+      if (SF)
+        nrecs = 1;
+      else
+        nrecs = this->connector->get_receivers_idx_links(node, receivers);
 
-  template <class out_t> out_t get_SFD_donors_flat() {
-    return format_output<std::vector<int>, out_t>(this->Sdonors);
-  }
+      // Caching Slope max
+      fT Smax;
+      fT dw0max;
+      fT dx;
+      int recmax = node;
+
+      // NOTE:
+      //  No need to calculate the topological number anymore, but keeping it
+      //  for recording its value
+      fT topological_number_v2 = 0.;
+
+      this->_compute_slopes_weights_et_al(node, SF, Smax, slopes, weights,
+                                          nrecs, receivers, recmax, dx, dw0max,
+                                          topological_number_v2);
+
+      // Initialising the total Qout
+      fT Qwin = this->_Qw[node];
+
+      // precalculating the power
+      fT pohw = std::pow(this->_hw[node], TWOTHIRD);
+
+      // Squarerooting Smax
+      // fT debug_S = Smax;
+      auto sqrtSmax = std::sqrt(Smax);
+
+      // Metric to calculate:
+      fT metric = topological_number_v2;
+      if (dimensions > 0)
+        metric = pohw * sqrtSmax / this->mannings(node);
+      if (dimensions > 1)
+        metric *= this->_hw[node];
+      if (dimensions > 2)
+        metric *= dw0max;
+
+      // transfer fluxes
+      // Computing the transfer of water and sed
+      this->_compute_transfers(nrecs, recmax, node, SF, receivers, weights,
+                               Qwin, metric);
 
-  template <class out_t> out_t get_SFD_donors_list() {
-    std::vector<std::vector<int>> out(this->nnodes);
-    for (int i = 0; i < this->nnodes; ++i) {
-      std::vector<int> tvec;
-      for (int j = 0; j < this->nSdonors[i]; ++j)
-        tvec.emplace_back(this->Sdonors[i * this->nneighbours + j]);
-      out[i] = tvec;
+      out[node] = metric;
+
+      // Volumetric discahrge
+      // fT Qwout = dw0max * this->_hw[node] * u_flow;
     }
 
-    return out;
+    return format_output<decltype(out), out_t>(out);
   }
 
-  template <class out_t> out_t get_links() { return this->links; }
+  template <class in_t, class out_t>
+  out_t compute_elemental_transfer(in_t &_production, fT total_time,
+                                   fT concentration_max) {
 
-  template <class out_t> out_t get_linknodes_flat() {
-    return format_output<std::vector<int>, out_t>(this->linknodes);
-  }
+    auto production = format_input(_production);
+
+    // Graph Processing
+    this->graph_automator();
+
+    // Initialise the water discharge fields according to water input condition
+    // and other monitoring features:
+    this->init_Qw();
+
+    // Am I in SFD or MFD
+    bool SF = (this->hydromode == HYDRO::GRAPH_SFD);
+
+    // Vertical motions are applied at the end of the timestep
+    std::vector<fT> out(this->graph->nnodes, 0.),
+        remaining_t(this->graph->nnodes, 0.);
+
+    // Caching neighbours, slopes and weights
+    auto receivers = this->connector->get_empty_neighbour();
+    std::array<fT, 8> weights, slopes;
+
+    // main loop
+    for (int i = this->graph->nnodes - 1; i >= 0; --i) {
+
+      // Getting next node in line
+      int node = this->get_istack_node(i);
 
-  template <class out_t> out_t get_linknodes_flat_D4() {
-    std::vector<int> temp(int(this->linknodes.size() / 2), -1);
-    int j = 0;
-    int counter = -1;
-    for (int i = 0; i < int(this->linknodes.size()); i += 2) {
-      ++counter;
-      if (counter == 0 || counter == 2) {
-        temp[j] = this->linknodes[i];
-        ++j;
-        temp[j] = this->linknodes[i + 1];
-        ++j;
+      production[node] =
+          std::min(production[node], this->_Qw[node] * concentration_max);
+
+      if (production[node] > 0) {
+        remaining_t[node] =
+            (remaining_t[node] * out[node] + production[node] * total_time) /
+            (out[node] + production[node]);
+        out[node] += production[node] / this->_hw[node];
       }
 
-      if (counter == 3)
-        counter = -1;
-    }
+      out[node] = std::min(out[node], this->_Qw[node] * concentration_max);
 
-    return format_output<std::vector<int>, out_t>(temp);
-  }
+      // Processing case where the node is a model edge, or no data
+      // this function  returns true if the node was boundary and does not need
+      // to be processed THis is where all the boundary treatment happens, if
+      // you need to add something happening at the boundaries
+      if (this->_initial_check_boundary_pit(node, receivers))
+        continue;
 
-  template <class out_t> out_t get_linkdx_flat_D4() {
-    std::vector<T> temp(int(this->links.size() / 2), -1);
-    int j = 0;
-    int counter = -1;
-    for (int i = 0; i < int(this->links.size()); ++i) {
-      ++counter;
+      // Getting the receivers
+      int nrecs;
+      if (SF)
+        nrecs = 1;
+      else
+        nrecs = this->connector->get_receivers_idx_links(node, receivers);
+
+      // Caching Slope max
+      fT Smax;
+      fT dw0max;
+      fT dx;
+      int recmax = node;
+
+      // NOTE:
+      //  No need to calculate the topological number anymore, but keeping it
+      //  for recording its value
+      fT topological_number_v2 = 0.;
+
+      this->_compute_slopes_weights_et_al(node, SF, Smax, slopes, weights,
+                                          nrecs, receivers, recmax, dx, dw0max,
+                                          topological_number_v2);
+
+      // Initialising the total Qout
+      fT Qwin = this->_Qw[node];
+
+      // precalculating the power
+      fT pohw = std::pow(this->_hw[node], TWOTHIRD);
+
+      // Squarerooting Smax
+      // fT debug_S = Smax;
+      auto sqrtSmax = std::sqrt(Smax);
+
+      // Metric to calculate:
+      fT transfer_time = dx / (pohw * sqrtSmax / this->mannings(node));
+      remaining_t[node] -= transfer_time;
+
+      // transfer fluxes
+      // Computing the transfer of water and sed
+      this->_compute_transfers(nrecs, recmax, node, SF, receivers, weights,
+                               Qwin, transfer_time);
+
+      if (out[node] > 0 && remaining_t[node] > 0) {
+        for (int j = 0; j < nrecs; ++j) {
+          int trec = this->connector->get_to_links(receivers[j]);
+          fT tadd = out[node] * weights[j];
+
+          remaining_t[trec] =
+              (remaining_t[trec] * out[trec] + remaining_t[node] * tadd) /
+              (tadd + out[trec]);
 
-      if (counter == 0 || counter == 2) {
-        T dx = this->get_dx_from_links_idx(i);
-        temp[j] = dx;
-        ++j;
+          out[trec] = (tadd + out[trec]);
+
+          out[trec] = std::min(out[trec], this->_Qw[trec] * concentration_max);
+        }
       }
 
-      if (counter == 3)
-        counter = -1;
+      // out[node] = metric;
+
+      // Volumetric discahrge
+      // fT Qwout = dw0max * this->_hw[node] * u_flow;
     }
 
-    return format_output<std::vector<T>, out_t>(temp);
-  }
+    for (int i = 0; i < this->connector->nnodes; ++i)
+      out[i] *= remaining_t[i];
 
-  template <class out_t> out_t get_linknodes_list() {
-    std::vector<std::vector<int>> out(this->links.size());
-    for (size_t i = 0; i < this->links.size(); ++i) {
-      out[i] =
-          std::vector<int>{this->linknodes[i * 2], this->linknodes[i * 2 + 1]};
-    }
-    return out;
+    return format_output<decltype(out), out_t>(out);
   }
 
-  template <class out_t> out_t get_linknodes_list_oriented() {
-    std::vector<std::vector<int>> out(this->links.size());
-    for (size_t i = 0; i < this->links.size(); ++i) {
-      out[i] = (this->links[i] >= 1)
-                   ? std::vector<int>{this->linknodes[i * 2],
-                                      this->linknodes[i * 2 + 1]}
-                   : std::vector<int>{this->linknodes[i * 2 + 1],
-                                      this->linknodes[i * 2]};
-    }
-    return out;
-  }
+  // Experimental drainage area stuff
+  // template<class out_t
 
-  int get_SFD_receivers_at_node(int i) { return this->Sreceivers[i]; }
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  //~=~=~=~= Precipitests ~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  // _      _      _      _      _      _      _      _
+  // )`'-.,_)`'-.,_)`'-.,_)`'-.,_)`'-.,_)`'-.,_)`'-.,_)`'-.,_
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+
+  int spawn_precipition() {
+
+    int node;
+
+    do {
+      bool OK = false;
+
+      if (this->water_input_mode == WATER_INPUT::PRECIPITATIONS_CONSTANT ||
+          this->water_input_mode == WATER_INPUT::PRECIPITATIONS_VARIABLE) {
+        node = this->dis(this->gen);
+        if (this->water_input_mode == WATER_INPUT::PRECIPITATIONS_CONSTANT)
+          OK = true;
+        else if (this->precipitations(node) > 0)
+          OK = true;
+      } else if (this->water_input_mode == WATER_INPUT::ENTRY_POINTS_H) {
+        node = this->_water_entry_nodes[this->dis(this->gen)];
+        OK = true;
+      } else
+        throw std::runtime_error("NOT DEFINED");
 
-  int get_SFD_dx_at_node(int i) { return this->Sdistance2receivers[i]; }
+      if (this->connector->boundaries.no_data(node) == false && OK)
+        break;
 
-  int get_SFD_ndonors_at_node(int i) { return this->nSdonors[i]; }
+    } while (true);
+    // std::cout << node << std::endl;
 
-  template <class out_t> out_t get_SFD_donors_at_node(int i) {
-    std::vector<int> out(this->nneighbours);
-    for (int j = 0; j < this->nSdonors[i]; ++j)
-      out.emplace_back(this->Sdonors[i * this->nneighbours + j]);
-    return out;
-  }
+    return node;
+  }
+
+  // Run a basic version of floodos, for testing purposes
+  // - N is the number of precipitons to launch
+  // - precdt is the time step between 2 successive precipitons
+  void run_precipitions(int N, fT precdt) {
+    // check if this is the first lauch and allocate the vectors if needed
+    if (this->last_dt_prec.size() == 0) {
+      this->last_dt_prec = std::vector<fT>(this->connector->nnodes, 0.);
+      this->last_dt_prec_e = std::vector<fT>(this->connector->nnodes, 0.);
+      this->last_sw_prec = std::vector<fT>(this->connector->nnodes, 0.);
+      this->last_dx_prec = std::vector<fT>(this->connector->nnodes, 0.);
+    }
+
+    // Computes the total volume of Qin.dt for all entry points
+    // -> if precipitation: sums all the precipitations * cellarea * dt
+    // -> if entry Qwin: sum all the entryQwin*dt
+    // this also sets the stochastic spawner
+    this->compute_Vp(precdt);
+
+    // current_dt_prec
+    // caching neighbours and slopes
+    auto neighbours = this->connector->get_empty_neighbour();
+
+    // launching n precipitons
+    for (int _ = 0; _ < N; ++_) {
+
+      // Spawn location
+      int node = this->spawn_precipition();
+      // caching the starting point for debugging
+      // int onode = node;
+
+      // increment the global chronometer
+      this->current_dt_prec += precdt;
+
+      // and for erosion if activated
+      if (this->morphomode != MORPHO::NONE)
+        this->current_dt_prec_e += precdt;
+
+      // sediment flux
+      fT tQs = this->Vps * this->connector->dy;
+
+      // adding a safeguard stopping the precipiton if it runs for too long
+      // (mostly used to avoid infinite loop when divergence occurs)
+      int NMAX = this->connector->nnodes * 2;
+      while (true) {
+        --NMAX;
+
+        // stops the precipitons if it has reached model edge
+        if (this->connector->boundaries.has_to_out(node) || NMAX == 0)
+          break;
+
+        // local time step
+        fT tdt = this->current_dt_prec - this->last_dt_prec[node];
+        // this->last_dt_prec[node] = this->current_dt_prec;
+
+        // caching receivers/slope/...
+        int rec = node; // will be rec
+        fT Sw = 0.;     // will be hydraulic slope
+        fT Sw_sel = 0.; // stochastic slope to select next receiver
+        // spatial steps
+        fT dx = 0.;
+        fT dy = 0.;
+
+        // getting the current neighbours
+        int nn = this->connector->get_neighbour_idx_links(node, neighbours);
+        for (int j = 0; j < nn; ++j) {
+          // local neighbour
+          int trec =
+              this->connector->get_other_node_from_links(neighbours[j], node);
+          // ignore no data
+          if (this->connector->boundaries.no_data(trec))
+            continue;
+
+          // if(this->last_dt_prec[trec] != this->current_dt_prec)
+          // decrease the water height of neighbour based on previous sw
+          this->update_hw_prec_and_dt(trec);
+        }
 
-  /*
-          =~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~
-          =~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~
-          =~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~
-                                . - ~ ~ ~ - .
-        ..     _      .-~               ~-.
-       //|     \ `..~                      `.
-      || |      }  }              /       \  \
-  (\   \\ \~^..'                 |         }  \
-   \`.-~  o      /       }       |        /    \
-   (__          |       /        |       /      `.
-    `- - ~ ~ -._|      /_ - ~ ~ ^|      /- _      `.
-                |     /          |     /     ~-.     ~- _
-                |_____|          |_____|         ~ - . _ _~_-_
+        // decrease node's hw based on previous sw
+        this->update_hw_prec_and_dt(node);
 
-          =~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~
-          =~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~
-          Functions computing gradients
-          =~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~
-          =~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~
-  */
+        // Takes care of adding the precipiton's hw (making sure water is not
+        // negative after the decrease too)
+        fT deltah = 0.;
+        if (this->connector->boundaries.can_out(node) == false) {
+          deltah = this->Vp;
+          this->_hw[node] += deltah;
+          if (this->_hw[node] < 0.) {
+            deltah += this->_hw[node];
+            this->_hw[node] = 0.;
+          }
+        }
 
-  template <class out_t, class topo_t>
-  out_t get_SFD_gradient(topo_t &ttopography) {
-    auto topography = format_input<topo_t>(ttopography);
-    auto gradient = this->_get_SFD_gradient(topography);
-    return format_output<decltype(gradient), out_t>(gradient);
-  }
+        // propagating to the surface
+        this->_surface[node] += deltah;
 
-  template <class topo_t> std::vector<T> _get_SFD_gradient(topo_t &topography) {
-    std::vector<T> gradient(this->nnodes, 0.);
-    for (int i = 0; i < this->nnodes; ++i) {
-      if (this->Sreceivers[i] != i)
-        gradient[i] = (topography[i] - topography[this->Sreceivers[i]]) /
-                      this->Sdistance2receivers[i];
-    }
-    return gradient;
-  }
+        // Determining the next path and updating the slopw/time/...
+        for (int j = 0; j < nn; ++j) {
 
-  template <class out_t, class topo_t>
-  out_t get_links_gradient(topo_t &ttopography, T min_slope) {
-    auto topography = format_input<topo_t>(ttopography);
-    std::vector<T> gradient = this->_get_links_gradient(topography, min_slope);
-    return format_output<decltype(gradient), out_t>(gradient);
-  }
+          // testing next receiver
+          int trec =
+              this->connector->get_other_node_from_links(neighbours[j], node);
+
+          if (this->connector->boundaries.no_data(trec)) {
+            continue;
+          }
+
+          // if potential receiver
+          if (this->_surface[trec] <= this->_surface[node]) {
+
+            // calculating slope
+            fT tsw = (this->_surface[node] - this->_surface[trec]) /
+                     this->connector->get_dx_from_links_idx(neighbours[j]);
+            // stochasticity f(sqrt(tsw))
+            fT tsw_sel =
+                std::sqrt(tsw) * this->randu.get() *
+                this->connector->get_traverse_dx_from_links_idx(neighbours[j]);
+
+            // Selecting these info if selected
+            if (tsw_sel > Sw_sel) {
+              Sw_sel = tsw_sel;
+              rec = trec;
+              dx = this->connector->get_dx_from_links_idx(neighbours[j]);
+              dy = this->connector->get_travers_dy_from_dx(dx);
+            }
+
+            // finding Smax
+            if (tsw > Sw)
+              Sw = tsw;
+
+            // managing preboundary conditions
+            if (this->connector->boundaries.can_out(trec) &&
+                this->boundhw == BOUNDARY_HW::FIXED_SLOPE) {
+              Sw_sel = this->bou_fixed_val;
+              Sw = this->bou_fixed_val;
+              rec = trec;
+              dx = this->connector->dx;
+              dy = this->connector->dy;
+              break;
+            }
+          }
+        }
+
+        // I have the Smax and other thingies, saving them
+        this->last_sw_prec[node] = Sw;
+        this->last_dx_prec[node] = dx;
+
+        // Dealing with morpho if enabled
+        if (this->morphomode != MORPHO::NONE &&
+            this->connector->boundaries.forcing_io(node) == false) {
+          if (Sw > 0 && rec != node && dx > 0) {
+            tdt = (this->current_dt_prec_e - this->last_dt_prec_e[node]) *
+                  this->dt_morpho_multiplier;
+            this->last_dt_prec_e[node] = this->current_dt_prec_e;
+            fT tau = this->rho(node) * this->_hw[node] * GRAVITY * Sw;
+            fT edot = 0., ddot = 0., edot_A = 0., edot_B = 0, ddot_A = 0,
+               ddot_B = 0.;
+            if (tau > this->tau_c(node))
+              edot += this->ke(node) *
+                      std::pow(tau - this->tau_c(node), this->aexp(node));
+
+            ddot = tQs / this->kd(node);
+
+            if (tQs < 0) {
+              // std::cout << "happens";
+              tQs = 0;
+            }
+
+            std::pair<int, int> orthonodes =
+                this->connector->get_orthogonal_nodes(node, rec);
+            int oA = orthonodes.first;
+            if (this->connector->boundaries.forcing_io(oA) ||
+                this->connector->is_in_bound(oA) == false ||
+                this->connector->boundaries.no_data(oA) ||
+                this->connector->flow_out_model(oA))
+              oA = -1;
+            int oB = orthonodes.second;
+            if (this->connector->boundaries.forcing_io(oB) ||
+                this->connector->is_in_bound(oB) == false ||
+                this->connector->boundaries.no_data(oB) ||
+                this->connector->flow_out_model(oB))
+              oB = -1;
+
+            // Dealing with lateral deposition if lS > 0 and erosion if lS <0
+            if (oA >= 0) {
+              fT tSwl = this->get_Stopo(node, oA, dy);
+              if (tSwl > 0) {
+                ddot_A = tSwl * this->kd_lateral(node) * ddot;
+              } else {
+                edot_A = std::abs(tSwl) * this->ke_lateral(node) * edot;
+              }
+
+              // std::cout << edot_A << "|" << ddot_A  << std::endl;
+            }
+
+            if (oB >= 0) {
+              fT tSwl = this->get_Stopo(node, oB, dy);
+              if (tSwl > 0) {
+                ddot_B = tSwl * this->kd_lateral(node) * ddot;
+              } else {
+                edot_B = std::abs(tSwl) * this->ke_lateral(node) * edot;
+              }
+            }
+
+            fT totd = ddot + ddot_B + ddot_A;
+            totd *= dx;
+            if (totd > tQs) {
+              auto cor = tQs / totd;
+              ddot *= cor;
+              ddot_B *= cor;
+              ddot_A *= cor;
+            }
+
+            tQs += (edot - ddot) * dx;
+            tQs += (edot_B - ddot_B) * dy;
+            tQs += (edot_A - ddot_A) * dy;
+            if (oA >= 0)
+              this->_surface[oA] += (ddot_A - edot_A) * tdt;
+            if (oB >= 0)
+              this->_surface[oB] += (ddot_B - edot_B) * tdt;
+
+            this->_surface[node] += (ddot - edot) * tdt;
+          }
+          // else
+          // {
+          // 	this->_surface[node] += this->Vp;
+          // }
+        }
 
-  template <class topo_t>
-  std::vector<T> _get_links_gradient(topo_t &topography, T min_slope) {
+        // stopping the loop if node is leaving the model
+        if (node == rec && this->connector->boundaries.can_out(node))
+          break;
 
-    std::vector<T> gradient = std::vector<T>(this->links.size(), 0);
+        // updating positions
+        node = rec;
 
-    for (size_t i = 0; i < this->links.size(); ++i) {
-      if (this->is_link_valid(i)) {
-        gradient[i] = std::max((topography[this->linknodes[i * 2]] -
-                                topography[this->linknodes[i * 2 + 1]]) /
-                                   this->get_dx_from_links_idx(i),
-                               min_slope);
-      }
-    }
+      } // end of while loop for a single precipiton
 
-    return gradient;
-  }
+    } // end of the for loop for all the launches
 
-  template <class out_t, class topo_t>
-  out_t get_MFD_mean_gradient(topo_t &ttopography) {
-    auto topography = format_input<topo_t>(ttopography);
-    auto gradient = this->_get_MFD_mean_gradient(topography);
-    return format_output<decltype(gradient), out_t>(gradient);
+  } // end of the precipiton function
+
+  std::vector<fT> get_precipitations_vector() {
+    std::vector<fT> out(this->connector->nnodes, 0.);
+    for (int i = 0; i < this->connector->nnodes; ++i) {
+      out[i] = this->precipitations(i);
+    }
+    return out;
   }
 
-  template <class topo_t>
-  std::vector<T> _get_MFD_mean_gradient(topo_t &topography) {
+  void define_precipitations_Ath(fT Ath) {
+    std::vector<BC> nBCs(this->connector->boundaries.codes);
+    std::vector<fT> fake(this->_surface);
+    this->graph->_compute_graph(fake, false, false);
+    auto DA = this->graph->_accumulate_constant_downstream_SFD(
+        this->connector->get_area_at_node(0));
+    std::vector<std::uint8_t> vis(this->connector->nnodes, false);
+    std::vector<fT> tprecs = this->get_precipitations_vector();
+
+    for (int i = this->connector->nnodes - 1; i >= 0; --i) {
 
-    std::vector<T> gradient = std::vector<T>(this->nnodes, 0);
-    std::vector<int> ngradient = std::vector<int>(this->nnodes, 0);
+      int node = this->graph->Sstack[i];
 
-    for (size_t i = 0; i < this->links.size(); ++i) {
-      if (this->is_link_valid(i)) {
-        T this_gradient = std::abs(topography[this->linknodes[i * 2] -
-                                              this->linknodes[i * 2 + 1]]) /
-                          this->get_dx_from_links_idx(i);
-        auto frto = this->get_from_to_links(i);
-        gradient[frto.first] += this_gradient;
-        ++ngradient[frto.first];
+      if (this->connector->boundaries.no_data(node))
+        continue;
+
+      // if(vis[node]) continue;
+
+      int rec = this->connector->_Sreceivers[node];
+      if (Ath < DA[node]) {
+        vis[node] = true;
+      } else {
+        tprecs[rec] += tprecs[node];
       }
+
+      vis[rec] = vis[node];
     }
 
-    for (int i = 0; i < this->nnodes; ++i) {
-      if (ngradient[i] > 0)
-        gradient[i] = gradient[i] / ngradient[i];
+    std::cout << "LKDFJDLKF" << std::endl;
+
+    auto receivers = this->connector->get_empty_neighbour();
+    for (int i = this->connector->nnodes - 1; i >= 0; --i) {
+      int node = this->graph->stack[i];
+
+      if (vis[node]) {
+        int nn = this->connector->get_receivers_idx(node, receivers);
+        for (int j = 0; j < nn; ++j)
+          vis[receivers[j]] = true;
+      }
     }
 
-    return gradient;
-  }
+    for (int i = this->connector->nnodes - 1; i >= 0; --i) {
+      if (vis[i] == false)
+        nBCs[i] = BC::NO_FLOW;
+    }
 
-  template <class out_t, class topo_t>
-  out_t get_MFD_weighted_gradient(topo_t &ttopography, topo_t &tweights) {
-    auto topography = format_input<topo_t>(ttopography);
-    auto weights = format_input<topo_t>(tweights);
-    auto gradient = this->_get_MFD_weighted_gradient(topography, weights);
-    return format_output<decltype(gradient), out_t>(gradient);
+    std::cout << "??" << std::endl;
+    this->connector->set_custom_boundaries(nBCs);
+    this->set_water_input_by_variable_precipitation_rate(tprecs);
+    std::cout << "!!" << std::endl;
   }
 
-  template <class topo_t>
-  std::vector<T> _get_MFD_weighted_gradient(topo_t &topography,
-                                            topo_t &weights) {
-
-    std::vector<T> gradient = std::vector<T>(this->nnodes, 0);
-    std::vector<T> wgradient = std::vector<T>(this->nnodes, 0.);
+  void run_graphipiton(int N, fT precdt, fT Ath) {
+    if (this->last_dt_prec.size() == 0) {
+      this->last_dt_prec = std::vector<fT>(this->connector->nnodes, 0.);
+      this->last_dt_prec_e = std::vector<fT>(this->connector->nnodes, 0.);
+      this->last_sw_prec = std::vector<fT>(this->connector->nnodes, 0.);
+      this->last_dx_prec = std::vector<fT>(this->connector->nnodes, 0.);
+    }
 
-    for (size_t i = 0; i < this->links.size(); ++i) {
-      if (this->is_link_valid(i)) {
-        T this_gradient = std::abs(topography[this->linknodes[i * 2] -
-                                              this->linknodes[i * 2 + 1]]) /
-                          this->get_dx_from_links_idx(i);
-        auto frto = this->get_from_to_links(i);
-        gradient[frto.first] += this_gradient * weights[i];
-        wgradient[frto.first] += weights[i];
+    std::vector<fT> fake(this->_surface);
+    this->graph->_compute_graph(fake, true, false);
+    auto DA = this->graph->_accumulate_constant_downstream_SFD(
+        this->connector->get_area_at_node(0));
+    std::vector<std::uint8_t> vis(this->connector->nnodes, false);
+    std::vector<int> starters;
+    starters.reserve(1000);
+    for (int i = this->connector->nnodes - 1; i >= 0; --i) {
+      int node = this->graph->Sstack[i];
+      if (vis[node])
+        continue;
+      int rec = this->connector->_Sreceivers[node];
+      vis[node] = true;
+      if (Ath < DA[node]) {
+        vis[rec] = true;
+        starters.emplace_back(node);
       }
     }
 
-    for (int i = 0; i < this->nnodes; ++i) {
-      if (wgradient[i] > 0)
-        gradient[i] = gradient[i] / wgradient[i];
-    }
+    this->compute_Vp(precdt);
 
-    return gradient;
-  }
+    this->dis = std::uniform_int_distribution<>(0, starters.size() - 1);
 
-  /*
-  =~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~
-  =~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~
-  =~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~
-                        . - ~ ~ ~ - .
-..     _      .-~               ~-.
-//|     \ `..~                      `.
-|| |      }  }              /       \  \
-(\   \\ \~^..'                 |         }  \
-\`.-~  o      /       }       |        /    \
-(__          |       /        |       /      `.
-`- - ~ ~ -._|      /_ - ~ ~ ^|      /- _      `.
-        |     /          |     /     ~-.     ~- _
-        |_____|          |_____|         ~ - . _ _~_-_
+    // current_dt_prec
+    auto neighbours = this->connector->get_empty_neighbour();
 
-  =~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~
-  =~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~
-  Functions to calculate weights
-  =~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~
-  =~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~
-  */
+    for (int _ = 0; _ < N; ++_) {
 
-  template <class out_t, class topo_t>
-  out_t get_link_weights(topo_t &tgradient, T exp) {
-    std::vector<T> weights(this->links.size(), 0.);
-    auto gradient = format_input<topo_t>(tgradient);
+      // int node = this->spawn_precipition();
+      int node = starters[this->dis(this->gen)];
+      // int onode = node;
+      // std::cout << "init at " << node << std::endl;
 
-    if (exp <= 0) {
-      this->_get_link_weights_f_nrecs(weights);
-    } else if (exp == 1) {
-      this->_get_link_weights_proposlope(weights, gradient);
-    } else {
-      this->_get_link_weights_exp(weights, gradient, exp);
-    }
+      this->current_dt_prec += precdt;
 
-    return format_output<decltype(weights), out_t>(weights);
-  }
+      if (this->morphomode != MORPHO::NONE)
+        this->current_dt_prec_e += precdt;
 
-  void _get_link_weights_f_nrecs(std::vector<T> &weights) {
-    auto nrecs = this->get_n_receivers();
-    for (size_t i = 0; i < this->links.size(); ++i) {
-      if (this->is_link_valid(i)) {
-        int nr = nrecs[this->get_from_links(i)];
-        if (nr > 0) {
-          weights[i] = 1. / nr;
-        } else
-          weights[i] = 1.;
-      }
-    }
-  }
-
-  template <class topo_t>
-  void _get_link_weights_proposlope(std::vector<T> &weights, topo_t &gradient) {
-    std::vector<T> sumgrad(this->nnodes, 0.);
-    for (size_t i = 0; i < this->links.size(); ++i) {
-      if (this->is_link_valid(i)) {
-        sumgrad[this->get_from_links(i)] += gradient[i];
-      }
-    }
-
-    for (size_t i = 0; i < this->links.size(); ++i) {
-      if (this->is_link_valid(i))
-        weights[i] = gradient[i] / sumgrad[this->get_from_links(i)];
-    }
-  }
-
-  template <class topo_t>
-  void _get_link_weights_exp(std::vector<T> &weights, topo_t &gradient, T exp) {
-    std::vector<T> sumgrad(this->nnodes, 0.);
-    for (size_t i = 0; i < this->links.size(); ++i) {
-      if (this->is_link_valid(i)) {
-        sumgrad[this->get_from_links(i)] += std::pow(gradient[i], exp);
-      }
-    }
-
-    for (size_t i = 0; i < this->links.size(); ++i) {
-      if (this->is_link_valid(i))
-        weights[i] =
-            std::pow(gradient[i], exp) / sumgrad[this->get_from_links(i)];
-    }
-  }
-
-  // ------------------------------------------------
-  //	                             	              __
-  //                                             / _)
-  //                                    _.----._/ /
-  //   Conversion METHODS              /         /
-  //                                __/ (  | (  |
-  //                               /__.-'|_|--|_|
-
-  // All the methods related to geometrical conversions
-  // ------------------------------------------------
-  // WILL NEED SOME WORK HERE DEPENDING ON THE GRAPH ORIENTATION AND ALL
-
-  inline void rowcol_from_node_id(int node_index, int &row, int &col) {
-    col = node_index % this->nx;
-    row = (int)std::floor(node_index / this->nx);
-  }
-
-  inline int nodeid_from_row_col(int row, int col) {
-    return row * this->nx + col;
-  }
-
-  inline int nodeid_from_XY(T X, T Y) {
-    int col = floor((X - this->Xmin) / this->dx);
-    int row = this->ny - floor((Y - this->Ymin) / this->dy);
-    return this->nodeid_from_row_col(row, col);
-  }
-  // void rowcol_from_XY()
-
-  inline void XY_from_nodeid(int node_index, T &tX, T &tY) {
-    int row, col;
-    this->rowcol_from_node_id(node_index, row, col);
-    this->XY_from_rowcol(row, col, tX, tY);
-  }
-
-  inline void XY_from_rowcol(int row, int col, T &tX, T &tY) {
-    tX = this->Xs[col];
-    tY = this->Ys[row];
-  }
-
-  inline T get_X_from_i(int i) {
-    int col = i % this->nx;
-    return this->Xs[col];
-  }
-
-  inline T get_Y_from_i(int i) {
-    int row = (int)std::floor(i / this->nx);
-    return this->Ys[row];
-  }
-
-  // ------------------------------------------------
-
-  //	                             	            __
-  //                                             / _)
-  //                                    _.----._/ /
-  //   Neighbouring METHODS            /         /
-  //                                __/ (  | (  |
-  //                               /__.-'|_|--|_|
-
-  // All the methods related to accessing and calculating neighbours
-  // ------------------------------------------------
-
-  std::vector<Neighbour<int, T>> get_neighbours(int i,
-                                                bool ignore_nodata = false) {
-
-    // preformatting the output
-    std::vector<Neighbour<int, T>> neighbours;
-
-    // Reserving size depending on the flow topology
-    neighbours.reserve(8);
-
-    size_t id_neighbourer = this->_get_neighbourer_id(i);
-
-    // Now I need to determine the index of the neighbourer vector
-    // Which provides adder to determine the neighbours f(boundary_conditions)
-    // internal node 0
-    // periodic_first_row 1
-    // periodic_last_row 2
-    // periodic_first_col 3
-    // periodic last_col 4
-    // normal_first_row 5
-    // normal_last_row 6
-    // normal_first_col 7
-    // normal_last_col 8
-    // normal_top_left 9
-    // normal_top_right 10
-    // normal_bottom_left 11
-    // normal_bottom_right 12
-    // top_left_periodic 13
-    // top_right_periodic 14
-    // periodic_bottom_left 15
-    // periodic_bottom_right 16
-
-    this->set_neighbours_in_vector(neighbours, i, id_neighbourer,
-                                   ignore_nodata);
-
-    // and return it
-    return neighbours;
-  }
-
-  // This function is the helper of the neighbouring function: it fills the
-  // neighbours vector with the actul values.
-  void set_neighbours_in_vector(std::vector<Neighbour<int, T>> &neighbours,
-                                int &i, size_t &id_neighbourer,
-                                bool ignore_nodata) {
-    // node index of the current neighbour
-    int tn;
-
-    // If you wonder why I am not iterating with a vector and everything here,
-    // it is for the small perf gain of doing it this way
-    tn = this->neighbourer[id_neighbourer][1];
-    if (tn != this->not_a_node &&
-        (ignore_nodata == false ||
-         (ignore_nodata && !this->boundaries.no_data(tn))))
-      neighbours.emplace_back(Neighbour<int, T>(tn + i, this->lengthener[1]));
-    tn = this->neighbourer[id_neighbourer][3];
-    if (tn != this->not_a_node &&
-        (ignore_nodata == false ||
-         (ignore_nodata && !this->boundaries.no_data(tn))))
-      neighbours.emplace_back(Neighbour<int, T>(tn + i, this->lengthener[3]));
-    tn = this->neighbourer[id_neighbourer][4];
-    if (tn != this->not_a_node &&
-        (ignore_nodata == false ||
-         (ignore_nodata && !this->boundaries.no_data(tn))))
-      neighbours.emplace_back(Neighbour<int, T>(tn + i, this->lengthener[4]));
-    tn = this->neighbourer[id_neighbourer][6];
-    if (tn != this->not_a_node &&
-        (ignore_nodata == false ||
-         (ignore_nodata && !this->boundaries.no_data(tn))))
-      neighbours.emplace_back(Neighbour<int, T>(tn + i, this->lengthener[6]));
-    tn = this->neighbourer[id_neighbourer][0];
-    if (tn != this->not_a_node &&
-        (ignore_nodata == false ||
-         (ignore_nodata && !this->boundaries.no_data(tn))))
-      neighbours.emplace_back(Neighbour<int, T>(tn + i, this->lengthener[0]));
-    tn = this->neighbourer[id_neighbourer][2];
-    if (tn != this->not_a_node &&
-        (ignore_nodata == false ||
-         (ignore_nodata && !this->boundaries.no_data(tn))))
-      neighbours.emplace_back(Neighbour<int, T>(tn + i, this->lengthener[2]));
-    tn = this->neighbourer[id_neighbourer][5];
-    if (tn != this->not_a_node &&
-        (ignore_nodata == false ||
-         (ignore_nodata && !this->boundaries.no_data(tn))))
-      neighbours.emplace_back(Neighbour<int, T>(tn + i, this->lengthener[5]));
-    tn = this->neighbourer[id_neighbourer][7];
-    if (tn != this->not_a_node &&
-        (ignore_nodata == false ||
-         (ignore_nodata && !this->boundaries.no_data(tn))))
-      neighbours.emplace_back(Neighbour<int, T>(tn + i, this->lengthener[7]));
-  }
-
-  inline size_t _get_neighbourer_id(int i) {
-
-    size_t id_neighbourer = -1;
-    // internal node, so neighbourer is 0
-    if (this->boundaries.is_normal_node(i))
-      id_neighbourer = 0;
-    else {
-      // Case top left corner
-      if (i == 0) {
-        // Case Periodic
-        if (this->boundaries.is_periodic(i))
-          id_neighbourer = 13;
-        // Case Noraml
-        else if (this->boundaries.normal_neighbouring_at_boundary(i))
-          id_neighbourer = 9;
-      }
-      // Case top right corner
-      else if (i == this->nx - 1) {
-        // Case Periodic
-        if (this->boundaries.is_periodic(i))
-          id_neighbourer = 14;
-        // Case Noraml
-        else if (this->boundaries.normal_neighbouring_at_boundary(i))
-          id_neighbourer = 10;
-      }
-      // Case bottom left corner
-      else if (i == (this->nnodes - this->nx)) {
-        // Case Periodic
-        if (this->boundaries.is_periodic(i))
-          id_neighbourer = 15;
-        // Case Noraml
-        else if (this->boundaries.normal_neighbouring_at_boundary(i))
-          id_neighbourer = 11;
-      }
-      // Case bottom right corner
-      else if (i == (this->nnodes - 1)) {
-        // Case Periodic
-        if (this->boundaries.is_periodic(i))
-          id_neighbourer = 16;
-        // Case Noraml
-        else if (this->boundaries.normal_neighbouring_at_boundary(i))
-          id_neighbourer = 12;
-      }
-      // Cases first row (no corner)
-      else if (i < this->nx - 1) {
-        // Case periodic
-        if (this->boundaries.is_periodic(i))
-          id_neighbourer = 1;
-        // Case normal
-        else if (this->boundaries.normal_neighbouring_at_boundary(i))
-          id_neighbourer = 5;
-      }
-      // Cases last row (no corner)
-      else if (i > (this->ny - 1) * this->nx) {
-        // Case periodic
-        if (this->boundaries.is_periodic(i))
-          id_neighbourer = 2;
-        // Case normal
-        else if (this->boundaries.normal_neighbouring_at_boundary(i))
-          id_neighbourer = 6;
-      }
-      // Cases first col (no corner)
-      else if (i % this->nx == 0) {
-        // Case periodic
-        if (this->boundaries.is_periodic(i))
-          id_neighbourer = 3;
-        // Case normal
-        else if (this->boundaries.normal_neighbouring_at_boundary(i))
-          id_neighbourer = 7;
-      }
-      // Cases last col (no corner)
-      else if (i % this->nx == this->nx - 1) {
-        // Case periodic
-        if (this->boundaries.is_periodic(i))
-          id_neighbourer = 4;
-        // Case normal
-        else if (this->boundaries.normal_neighbouring_at_boundary(i))
-          id_neighbourer = 8;
-      } else
-        id_neighbourer = 0;
-    }
+      // fT tQs = this->Vps * this->connector->dy;
 
-    // if(id_neighbourer == -1)
-    // {
-    // 	int row,col;
-    // 	this->rowcol_from_node_id(i,row,col);
-    // 	std::cout << "boundary was " << this->boundary[i] << " i: " << i << "/"
-    // << this->nnodes << " row: " << row << " col: " << col << std::endl;
-    // throw std::runtime_error("neighbouring issue");
-    // }
+      int NMAX = this->connector->nnodes * 2;
+      while (true) {
+        --NMAX;
+        if (this->connector->boundaries.has_to_out(node) || NMAX == 0)
+          break;
 
-    return id_neighbourer;
-  }
+        // // update step from Qwout
+        // fT tdt = this->current_dt_prec - this->last_dt_prec[node];
+        // // this->last_dt_prec[node] = this->current_dt_prec;
 
-  inline size_t _get_neighbourer_id_assume_periodic(int i) {
+        int rec = node;
+        fT Sw = 0.;
+        fT Sw_sel = 0.;
+        fT dx = 0.;
+        // fT dy = 0.;
+        int nn = this->connector->get_neighbour_idx_links(node, neighbours);
 
-    size_t id_neighbourer = -1;
-    // internal node, so neighbourer is 0
-    if (this->boundaries.is_normal_node(i))
-      id_neighbourer = 0;
-    else {
-      // Case top left corner
-      if (i == 0) {
-        // Case Periodic
-        id_neighbourer = 13;
-      }
-      // Case top right corner
-      else if (i == this->nx - 1) {
-        // Case Periodic
+        for (int j = 0; j < nn; ++j) {
+          int trec =
+              this->connector->get_other_node_from_links(neighbours[j], node);
+          if (this->connector->boundaries.no_data(trec))
+            continue;
 
-        id_neighbourer = 14;
+          // if(this->last_dt_prec[trec] != this->current_dt_prec)
+          this->update_hw_prec_and_dt(trec);
+        }
+        this->update_hw_prec_and_dt(node);
 
-      }
-      // Case bottom left corner
-      else if (i == (this->nnodes - this->nx)) {
+        fT deltah = 0.;
+        if (true) {
+          deltah = this->Vp;
+          this->_hw[node] += deltah;
+          if (this->_hw[node] < 0.) {
+            deltah += this->_hw[node];
+            this->_hw[node] = 0.;
+          }
+        }
+        this->_surface[node] += deltah;
+
+        for (int j = 0; j < nn; ++j) {
+          int trec =
+              this->connector->get_other_node_from_links(neighbours[j], node);
+
+          if (this->connector->boundaries.no_data(trec)) {
+            continue;
+          }
+
+          if (this->_surface[trec] <= this->_surface[node]) {
+
+            fT tsw = (this->_surface[node] - this->_surface[trec]) /
+                     this->connector->get_dx_from_links_idx(neighbours[j]);
+            fT tsw_sel = tsw * this->randu.get();
+            // std::cout << tsw_sel << std::endl;
+            if (tsw_sel > Sw_sel) {
+              Sw_sel = tsw_sel;
+              rec = trec;
+              dx = this->connector->get_dx_from_links_idx(neighbours[j]);
+              // dy = this->connector->get_travers_dy_from_dx(dx);
+            }
+
+            if (tsw > Sw)
+              Sw = tsw;
+
+            if (this->connector->boundaries.can_out(trec) &&
+                this->boundhw == BOUNDARY_HW::FIXED_SLOPE) {
+              Sw_sel = this->bou_fixed_val;
+              Sw = this->bou_fixed_val;
+              rec = trec;
+              dx = this->connector->dx;
+              // dy = this->connector->dy;
+            }
+          }
+        }
 
-        id_neighbourer = 15;
+        this->last_sw_prec[node] = Sw;
+        this->last_dx_prec[node] = dx;
 
-      }
-      // Case bottom right corner
-      else if (i == (this->nnodes - 1)) {
+        // std::cout << onode << "||" << node << " vs " << rec << "||";
 
-        id_neighbourer = 16;
+        if (node == rec && this->connector->boundaries.can_out(node))
+          break;
 
+        // if(node != rec)
+        // 	throw std::runtime_error("DONE!");
+        node = rec;
       }
-      // Cases first row (no corner)
-      else if (i < this->nx - 1) {
+      // throw std::runtime_error("BITE2");
+    }
+  }
 
-        id_neighbourer = 1;
+  void update_hw_prec_and_dt(int node) {
 
-      }
-      // Cases last row (no corner)
-      else if (i > (this->ny - 1) * this->nx) {
+    fT tdt = this->current_dt_prec - this->last_dt_prec[node];
+    this->last_dt_prec[node] = this->current_dt_prec;
 
-        id_neighbourer = 2;
+    if (tdt == 0 || this->last_sw_prec[node] == 0 ||
+        this->last_dx_prec[node] == 0) {
+      return;
+    }
 
-      }
-      // Cases first col (no corner)
-      else if (i % this->nx == 0) {
+    auto delta = tdt * std::pow(this->_hw[node], 5. / 3.) *
+                 std::sqrt(this->last_sw_prec[node]) / this->mannings(node) /
+                 this->last_dx_prec[node];
+    this->_hw[node] -= delta;
+    this->_surface[node] -= delta;
+  }
 
-        id_neighbourer = 3;
+  void update_hw_prec_and_dt_exp_2(int node, std::vector<fT> &gHwin, fT tHwin,
+                                   fT precdt) {
 
-      }
-      // Cases last col (no corner)
-      else if (i % this->nx == this->nx - 1) {
-        id_neighbourer = 4;
+    fT tdt = this->current_dt_prec - this->last_dt_prec[node];
+    this->last_dt_prec[node] = this->current_dt_prec;
 
-      } else
-        id_neighbourer = 0;
+    // SHAKING THINGS HERE
+    tdt = precdt;
+
+    if (tdt == 0 || this->last_sw_prec[node] == 0 ||
+        this->last_dx_prec[node] == 0) {
+      // fT dHwin =  std::max(tHwin, gHwin[node]);
+
+      // this->_hw[node] += dtfill * dHwin ;
+      // this->_surface[node] += dtfill * dHwin ;
+      return;
     }
 
-    // if(id_neighbourer == -1)
-    // {
-    // 	int row,col;
-    // 	this->rowcol_from_node_id(i,row,col);
-    // 	std::cout << "boundary was " << this->boundary[i] << " i: " << i << "/"
-    // << this->nnodes << " row: " << row << " col: " << col << std::endl;
-    // throw std::runtime_error("neighbouring issue");
-    // }
+    fT dHwin = std::max(tHwin, gHwin[node]);
+    // std::cout << "+:" << dHwin * tdt;
 
-    return id_neighbourer;
+    auto delta = tdt * std::pow(this->_hw[node], 5. / 3.) *
+                 std::sqrt(this->last_sw_prec[node]) / this->mannings(node) /
+                 this->last_dx_prec[node];
+    // std::cout << " vs - :" << delta << std::endl;;
+    delta -= dHwin * tdt;
+    if (delta < -this->_hw[node])
+      delta = -this->_hw[node];
+
+    this->_hw[node] -= delta;
+    this->_surface[node] -= delta;
+    // if(delta > 0)
+    // 	std::cout <<"delta::" << delta << std::endl;
   }
 
-  // D4 single neighbour routines
-  Neighbour<int, T> get_left_neighbour(int i) {
-    size_t id_neighbourer = this->_get_neighbourer_id(i);
-    return Neighbour<int, T>(this->neighbourer[id_neighbourer][3] + i,
-                             this->dx);
-  }
-
-  Neighbour<int, T> get_top_neighbour(int i) {
-    size_t id_neighbourer = this->_get_neighbourer_id(i);
-    return Neighbour<int, T>(this->neighbourer[id_neighbourer][1] + i,
-                             this->dy);
-  }
-
-  Neighbour<int, T> get_right_neighbour(int i) {
-    size_t id_neighbourer = this->_get_neighbourer_id(i);
-    return Neighbour<int, T>(this->neighbourer[id_neighbourer][4] + i,
-                             this->dx);
-  }
-
-  Neighbour<int, T> get_bottom_neighbour(int i) {
-    size_t id_neighbourer = this->_get_neighbourer_id(i);
-    return Neighbour<int, T>(this->neighbourer[id_neighbourer][6] + i,
-                             this->dy);
-  }
-
-  // D8 single neighbour extra routines
-  Neighbour<int, T> get_topleft_neighbour(int i) {
-    size_t id_neighbourer = this->_get_neighbourer_id(i);
-    return Neighbour<int, T>(this->neighbourer[id_neighbourer][0] + i,
-                             this->dxy);
-  }
-
-  Neighbour<int, T> get_topright_neighbour(int i) {
-    size_t id_neighbourer = this->_get_neighbourer_id(i);
-    return Neighbour<int, T>(this->neighbourer[id_neighbourer][2] + i,
-                             this->dxy);
-  }
-
-  Neighbour<int, T> get_bottomleft_neighbour(int i) {
-    size_t id_neighbourer = this->_get_neighbourer_id(i);
-    return Neighbour<int, T>(this->neighbourer[id_neighbourer][5] + i,
-                             this->dxy);
-  }
-
-  Neighbour<int, T> get_bottomright_neighbour(int i) {
-    size_t id_neighbourer = this->_get_neighbourer_id(i);
-    return Neighbour<int, T>(this->neighbourer[id_neighbourer][7] + i,
-                             this->dxy);
-  }
-
-  // D4 single neighbour routines
-  int get_left_idx(int i) {
-    size_t id_neighbourer = this->_get_neighbourer_id(i);
-    return this->neighbourer[id_neighbourer][3] + i;
-  }
-
-  int get_top_idx(int i) {
-    size_t id_neighbourer = this->_get_neighbourer_id(i);
-    return this->neighbourer[id_neighbourer][1] + i;
-  }
-
-  int get_right_idx(int i) {
-    size_t id_neighbourer = this->_get_neighbourer_id(i);
-    return this->neighbourer[id_neighbourer][4] + i;
-  }
-
-  int get_bottom_idx(int i) {
-    size_t id_neighbourer = this->_get_neighbourer_id(i);
-    return this->neighbourer[id_neighbourer][6] + i;
-  }
-
-  // D8 single neighbour extra routines
-  int get_topleft_idx(int i) {
-    size_t id_neighbourer = this->_get_neighbourer_id(i);
-    return this->neighbourer[id_neighbourer][0] + i;
-  }
-
-  int get_topright_idx(int i) {
-    size_t id_neighbourer = this->_get_neighbourer_id(i);
-    return this->neighbourer[id_neighbourer][2] + i;
-  }
-
-  int get_bottomleft_idx(int i) {
-    size_t id_neighbourer = this->_get_neighbourer_id(i);
-    return this->neighbourer[id_neighbourer][5] + i;
-  }
-
-  int get_bottomright_idx(int i) {
-    size_t id_neighbourer = this->_get_neighbourer_id(i);
-    return this->neighbourer[id_neighbourer][7] + i;
-  }
-
-  std::vector<int> get_D4_neighbours_only_id(int i) {
-    std::vector<int> neighs;
-    neighs.reserve(4);
-    int tn = this->get_left_idx(i);
-    if (tn >= 0)
-      neighs.emplace_back(tn);
-    tn = this->get_top_idx(i);
-    if (tn >= 0)
-      neighs.emplace_back(tn);
-    tn = this->get_right_idx(i);
-    if (tn >= 0)
-      neighs.emplace_back(tn);
-    tn = this->get_bottom_idx(i);
-    if (tn >= 0)
-      neighs.emplace_back(tn);
-    return neighs;
-  }
-
-  // std::vector<int> get_neighbour_idx(int i)
-  // {
-  // 	std::vector<int> neighs;neighs.reserve(8);
-  // 	int tn = this->get_left_idx(i);
-  // 	if(tn >= 0 )
-  // 		neighs.emplace_back(tn);
-  // 	tn = this->get_top_idx(i);
-  // 	if(tn >= 0 )
-  // 		neighs.emplace_back(tn);
-  // 	tn = this->get_right_idx(i);
-  // 	if(tn >= 0 )
-  // 		neighs.emplace_back(tn);
-  // 	tn = this->get_bottom_idx(i);
-  // 	if(tn >= 0 )
-  // 		neighs.emplace_back(tn);
-  // 	tn = this->get_topleft_idx(i);
-  // 	if(tn >= 0 )
-  // 		neighs.emplace_back(tn);
-  // 	tn = this->get_topright_idx(i);
-  // 	if(tn >= 0 )
-  // 		neighs.emplace_back(tn);
-  // 	tn = this->get_bottomright_idx(i);
-  // 	if(tn >= 0 )
-  // 		neighs.emplace_back(tn);
-  // 	tn = this->get_bottomleft_idx(i);
-  // 	if(tn >= 0 )
-  // 		neighs.emplace_back(tn);
-
-  // 	return neighs;
-  // }
-
-  // Some of my algorithm are adapted from richdem and require iterating through
-  // neighbours the way they do starting from left and going clockwise around
-  // the node
-  int get_neighbours_idx_richdemlike(int i, std::vector<int> &neighs) {
-    int j = 0;
-    neighs[j] = (this->get_left_idx(i));
-    ++j;
-    neighs[j] = (this->get_topleft_idx(i));
-    ++j;
-    neighs[j] = (this->get_top_idx(i));
-    ++j;
-    neighs[j] = (this->get_topright_idx(i));
-    ++j;
-    neighs[j] = (this->get_right_idx(i));
-    ++j;
-    neighs[j] = (this->get_bottomright_idx(i));
-    ++j;
-    neighs[j] = (this->get_bottom_idx(i));
-    ++j;
-    neighs[j] = (this->get_bottomleft_idx(i));
-    ++j;
-    return 8;
-  }
-
-  // Method to test whether a node can outlet flow OUT of the model
-  // DEPRECATED
-  // inline bool can_flow_out_there(int i)
-  // {
-  // 	if(this->boundary[i] == 3 || this->boundary[i] == 0 )
-  // 		return true;
-  // 	else
-  // 	{
-  // 		return false;
-  // 	}
-  // }
-
-  // // method to check if a node can even accept flow
-  // inline bool can_flow_even_go_there(int i)
-  // {
-  // 	if(this->boundary[i] < 0)
-  // 		return false;
-  // 	else
-  // 	{
-  // 		return true;
-  // 	}
-  // }
-
-  // inline bool is_active(int i)
-  // {
-  // 	if(this->can_flow_out_there(i) && this->boundary[i] != 3)
-  // 		return false;
-  // 	else if(this->boundary[i] == 3)
-  // 		return true;
-  // 	else if(this->boundary[i] == 4)
-  // 		return false;
-
-  // 	if(this->can_flow_even_go_there(i))
-  // 		return true;
-  // 	return false;
-  // }
-
-  // Returns true if the node is on the dem edge
-  // (i.e. one of the 4 lines)
-  bool is_on_dem_edge(int i) {
-    if (this->is_on_top_row(i) || this->is_on_bottom_row(i) ||
-        this->is_on_leftest_col(i) || this->is_on_rightest_col(i))
-      return true;
-    return false;
+  void update_hw_prec_and_dt_exp(int node, std::vector<int> &baslab,
+                                 std::vector<fT> &basdt) {
+
+    fT tdt = basdt[baslab[node]] - this->last_dt_prec[node];
+    this->last_dt_prec[node] = basdt[baslab[node]];
+
+    if (tdt == 0 || this->last_sw_prec[node] == 0 ||
+        this->last_dx_prec[node] == 0) {
+      return;
+    }
+
+    auto delta = tdt * std::pow(this->_hw[node], 5. / 3.) *
+                 std::sqrt(this->last_sw_prec[node]) / this->mannings(node) /
+                 this->last_dx_prec[node];
+    this->_hw[node] -= delta;
+    this->_surface[node] -= delta;
   }
 
-  bool is_on_top_row(int i) {
-    if (i < this->nx)
-      return true;
-    return false;
+  void compute_Vp(fT precdt) {
+    this->Vp = 0.;
+    if (this->water_input_mode == WATER_INPUT::PRECIPITATIONS_CONSTANT ||
+        this->water_input_mode == WATER_INPUT::PRECIPITATIONS_VARIABLE) {
+
+      for (int i = 0; i < this->connector->nnodes; ++i) {
+        this->Vp += this->precipitations(i) * precdt;
+      }
+      this->dis =
+          std::uniform_int_distribution<>(0, this->connector->nnodes - 1);
+    } else if (this->water_input_mode == WATER_INPUT::ENTRY_POINTS_H) {
+      for (size_t i = 0; i < this->_water_entries.size(); ++i) {
+        this->Vp += this->_water_entries[i] * precdt;
+      }
+      this->dis =
+          std::uniform_int_distribution<>(0, this->_water_entries.size() - 1);
+    }
+
+    this->Vps = 0;
+    if (this->sed_input_mode == SED_INPUT::ENTRY_POINTS_Q) {
+      for (size_t i = 0; i < this->_sed_entries.size(); ++i) {
+        this->Vps += this->_sed_entries[i] * this->connector->dy * precdt *
+                     this->dt_morpho_multiplier;
+      }
+      // this->dis = std::uniform_int_distribution<>
+      // (0,this->_water_entries.size()-1);
+    }
   }
 
-  bool is_on_bottom_row(int i) {
-    if (i >= this->nnodes - this->nx)
-      return true;
-    else
-      return false;
+  void run_precipitions_exp(int N, fT precdt, fT dtfill) {
+    // place holder for debugging
+    return;
   }
 
-  bool is_on_leftest_col(int i) {
-    if (i % this->nx == 0)
-      return true;
-    else
-      return false;
+  void run_precipitions_exp_1(int N, fT precdt) {
+    // place holder for debugging
+    return;
   }
 
-  bool is_on_rightest_col(int i) {
-    if (i % this->nx == this->nx - 1)
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  //~=~=~=~= Legacy archive ~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  // _      _      _      _      _      _      _      _
+  // )`'-.,_)`'-.,_)`'-.,_)`'-.,_)`'-.,_)`'-.,_)`'-.,_)`'-.,_
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+  //~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=~=
+
+  // Note that A lot of experimental functions have been erased (see former
+  // commit)
+  void run_exp() {
+    std::cout << "Run_exp is not available at the moment" << std::endl;
+  }
+  // initial check for boundary conditions WITHOUT applying relevant changes
+  bool _initial_check_boundary_pit(int &node, std::array<int, 8> &receivers) {
+    if (this->connector->boundaries.no_data(node) ||
+        this->connector->flow_out_or_pit(node)) {
+      // Checking mass conservations
+      this->tot_Qwin_output += this->_Qw[node];
       return true;
-    else
-      return false;
+    }
+    return false;
   }
 
-  void print_dim() {
-    std::cout << "nx:" << this->nx << std::endl;
-    std::cout << "ny:" << this->ny << std::endl;
-    std::cout << "nnodes:" << this->nnodes << std::endl;
-    std::cout << "dx:" << this->dx << std::endl;
-    std::cout << "dy:" << this->dy << std::endl;
-  }
-
-  template <class topo_t, class out_t> out_t get_HS(topo_t &ttopography) {
-    auto topography = format_input(ttopography);
-    double altitude = 45;
-    double azimuth = 315;
-    double z_factor = 1;
-    double pi = 3.1415926;
-
-    // std::vector<double> hillshade(ptr, ptr + this->nnodes);
-    std::vector<double> hillshade(this->nnodes, 0.);
-
-    // convert zenith and azimuth into radians for calculation
-    double zenith_rad = (90 - altitude) * pi / 180.0;
-    double azimuth_math = 360 - azimuth + 90;
-    if (azimuth_math >= 360.0)
-      azimuth_math = azimuth_math - 360;
-    double azimuth_rad = azimuth_math * pi / 180.0;
-
-    for (int i = 0; i < this->nnodes; ++i) {
-      // Ignoring no data
-      if (this->boundaries.no_data(i))
+  fT weights_automator(std::array<int, 8> &receivers, std::vector<fT> &weights,
+                       std::vector<fT> &slopes, int &node, int &nrecs,
+                       fT &topological_number_v2) {
+
+    fT sumw = 0., Smax = this->minslope, dw0max = 0, sumSdw = 0.;
+    ;
+
+    // int_dw = 0;
+    // int yolo1 = node;
+    // bool isit = yolo1 == 300;
+    for (int i = 0; i < nrecs; ++i) {
+      int lix = receivers[i];
+
+      if (this->connector->is_link_valid(lix) == false) {
         continue;
+      }
 
-      double slope_rad = 0;
-      double aspect_rad = 0;
-      double dzdx = 0;
-      double dzdy = 0;
-
-      double ij = topography[i];
-      double ijp1 = topography[this->get_right_neighbour(i).node];
-      double ip1j = topography[this->get_bottom_neighbour(i).node];
-      double ip1jp1 = topography[this->get_bottomright_neighbour(i).node];
-      double im1jm1 = topography[this->get_topleft_neighbour(i).node];
-      double im1j = topography[this->get_top_neighbour(i).node];
-      double im1jp1 = topography[this->get_topright_neighbour(i).node];
-      double ijm1 = topography[this->get_left_neighbour(i).node];
-      double ip1jm1 = topography[this->get_bottomleft_neighbour(i).node];
-
-      if (ij > 0) {
-        dzdx = ((ijp1 + 2 * ip1j + ip1jp1) - (im1jm1 + 2 * im1j + im1jp1)) /
-               (8 * this->dx);
-        dzdy = ((im1jp1 + 2 * ijp1 + ip1jp1) - (im1jm1 + 2 * ijm1 + ip1jm1)) /
-               (8 * this->dy);
-        slope_rad = atan(z_factor * sqrt((dzdx * dzdx) + (dzdy * dzdy)));
-        if (dzdx != 0) {
-          aspect_rad = std::atan2(dzdy, (dzdx * -1));
-          if (aspect_rad < 0)
-            aspect_rad = 2 * pi + aspect_rad;
-        } else {
-          if (dzdy > 0)
-            aspect_rad = pi / 2;
-          else if (dzdy < 0)
-            aspect_rad = 2 * pi - pi / 2;
-        }
+      // int_dw += this->connector->get_dx_from_links_idx(lix);
+      fT tdw = this->connector->get_traverse_dx_from_links_idx(lix);
+      int rec = this->connector->get_to_links(lix);
+      if (this->connector->flow_out_or_pit(rec) &&
+          this->boundhw == BOUNDARY_HW::FIXED_SLOPE) {
+        slopes[i] = this->bou_fixed_val;
+        tdw = this->connector->dy;
+      } else
+        slopes[i] = this->get_Sw(lix, this->minslope);
 
-        hillshade[i] = ((std::cos(zenith_rad) * std::cos(slope_rad)) +
-                        (std::sin(zenith_rad) * std::sin(slope_rad) *
-                         std::cos(azimuth_rad - aspect_rad)));
-        // std::cout << hillshade[i] << "|";
-        if (hillshade[i] < 0)
-          hillshade[i] = 0;
+      sumSdw += slopes[i] * tdw;
+
+      if (slopes[i] > Smax) {
+        Smax = slopes[i];
+        dw0max = tdw;
       }
+
+      // slopes[i] = slope;
+      if (this->weight_management == MFD_PARTITIONNING::PROPOSLOPE)
+        weights[i] = slopes[i] * tdw;
+
+      else if (this->weight_management == MFD_PARTITIONNING::SQRTSLOPE)
+        weights[i] = std::sqrt(slopes[i] * tdw);
+
+      else if (this->weight_management == MFD_PARTITIONNING::PROPOREC)
+        weights[i] = 1.;
+
+      if (this->stochaslope)
+        weights[i] *= this->stochaslope_coeff * this->randu.get();
+
+      sumw += weights[i];
     }
 
-    return format_output<decltype(hillshade), out_t>(hillshade);
-  }
-
-  // this function makes the connector generic and allow other connector to have
-  // varying cellarea
-  template <class i_t> T get_area_at_node(i_t i) { return this->cellarea; }
-
-  // template<>
-  // void fill_neighbour_matrices()
-
-  template <class i_t> T get_dx_from_links_idx(i_t i) {
-    if (i % 4 == 0)
-      return this->dx;
-    else if (i % 4 == 1)
-      return this->dxy;
-    else if (i % 4 == 2)
-      return this->dy;
-    else if (i % 4 == 3)
-      return this->dxy;
-    else
-      return this->dx;
-  }
+    fT sumf = 0.;
+    for (int i = 0; i < nrecs; ++i) {
+      int lix = receivers[i];
 
-  template <class i_t> T get_traverse_dx_from_links_idx(i_t i) {
-    if (i % 4 == 0)
-      return this->dy;
-    else if (i % 4 == 1)
-      return this->dxy;
-    else if (i % 4 == 2)
-      return this->dx;
-    else if (i % 4 == 3)
-      return this->dxy;
-    else
-      return this->dy;
-  }
+      if (this->connector->is_link_valid(lix) == false)
+        continue;
 
-  // return the orthogonal node from a pair of node / link indices
-  template <class i_t>
-  std::pair<i_t, i_t> get_orthogonal_nodes(i_t node_from, i_t node_to) {
-
-    if (node_to == this->get_top_idx(node_from))
-      return {this->get_left_idx(node_from), this->get_right_idx(node_from)};
-    if (node_to == this->get_topright_idx(node_from))
-      return {this->get_top_idx(node_from), this->get_right_idx(node_from)};
-    if (node_to == this->get_right_idx(node_from))
-      return {this->get_top_idx(node_from), this->get_bottom_idx(node_from)};
-    if (node_to == this->get_bottomright_idx(node_from))
-      return {this->get_right_idx(node_from), this->get_bottom_idx(node_from)};
-    if (node_to == this->get_bottom_idx(node_from))
-      return {this->get_left_idx(node_from), this->get_right_idx(node_from)};
-    if (node_to == this->get_bottomleft_idx(node_from))
-      return {this->get_left_idx(node_from), this->get_bottom_idx(node_from)};
-    if (node_to == this->get_left_idx(node_from))
-      return {this->get_top_idx(node_from), this->get_bottom_idx(node_from)};
-    if (node_to == this->get_topleft_idx(node_from))
-      return {this->get_top_idx(node_from), this->get_left_idx(node_from)};
-    else
-      return {-1, -1};
+      weights[i] = weights[i] / sumw;
+      sumf += weights[i];
+    }
 
-    // else
-    // {
-    // 	std::cout << "Node was " << node_from << " to was " << node_to << "
-    // possible neighbours to node_from:" << std::endl; 	std::cout <<
-    // this->get_top_idx(node_from) << std::endl; 	std::cout <<
-    // this->get_topright_idx(node_from) << std::endl; 	std::cout <<
-    // this->get_right_idx(node_from) << std::endl; 	std::cout <<
-    // this->get_bottomright_idx(node_from) << std::endl; 	std::cout <<
-    // this->get_bottom_idx(node_from) << std::endl; 	std::cout <<
-    // this->get_bottomleft_idx(node_from) << std::endl; 	std::cout <<
-    // this->get_left_idx(node_from) << std::endl; 	std::cout <<
-    // this->get_topleft_idx(node_from) << std::endl; 	std::cout << "Boundary
-    // was " << this->boundary[node_from] << std::endl; 	throw
-    // std::runtime_error("Fatal error in
-    // DAGGER::D8connector::get_orthogonal_nodes -> from: " +
-    // std::to_string(node_from) + " and node to " + std::to_string(node_to));
-    // }
-  }
+    topological_number_v2 = (Smax * dw0max) / sumSdw;
 
-  template <class i_t, class ii_t>
-  std::pair<T, T> get_directed_dxdy_from_links_idx(i_t li, ii_t original_node,
-                                                   ii_t n1, ii_t n2) {
-    int C_C = (original_node == n1) ? 1 : -1;
-    if (li % 4 == 0)
-      return std::make_pair(C_C * this->dx, C_C * 0.);
-    else if (li % 4 == 1)
-      return std::make_pair(C_C * this->dx, C_C * this->dy);
-    else if (li % 4 == 2)
-      return std::make_pair(C_C * 0., C_C * this->dy);
-    else if (li % 4 == 3)
-      return std::make_pair(-1 * C_C * this->dx, C_C * this->dy);
-    else
-      return std::make_pair(C_C * this->dx, C_C * 0.);
+    return Smax;
   }
 
-  template <class i_t, class ii_t>
-  std::pair<T, T> get_dxdy_from_links_idx(i_t li) {
-    if (li % 4 == 0)
-      return std::make_pair(this->dx, 0.);
-    else if (li % 4 == 1)
-      return std::make_pair(this->dx, this->dy);
-    else if (li % 4 == 2)
-      return std::make_pair(0., this->dy);
-    else if (li % 4 == 3)
-      return std::make_pair(this->dx, this->dy);
-    else
-      return std::make_pair(this->dx, 0.);
-  }
+  void _compute_transfers_exp(int &nrecs, int &recmax, int &node, bool &SF,
+                              std::array<int, 8> &receivers,
+                              std::array<fT, 8> &weights, fT &Qwin) {
+    // going through the receiver(s)
+    for (int j = 0; j < nrecs; ++j) {
 
-  template <class i_t> T get_dx_from_linknodes_idx(i_t i) {
-    int j = std::floor(i / 2);
-    return this->get_dx_from_links_idx(j);
-  }
+      // Hydro for the link
+      // universal params
+      int rec;
+      if (SF)
+        rec = recmax;
+      else
+        rec = this->connector->get_to_links(receivers[j]);
 
-  T get_travers_dy_from_dx(T tdx) {
-    if (tdx == this->dx)
-      return this->dy;
-    else if (tdx == this->dy)
-      return this->dx;
-    else
-      return this->dxy;
-  }
+      if (rec < 0)
+        continue;
 
-  // EXPERIMENTAL!!!! POSSIBLE ISSUES WITH BC
-  template <class i_t> i_t linkidx_from_nodes(i_t n1, i_t n2) {
-    if (n1 > n2)
-      std::swap(n1, n2);
-    int delta = n2 - n1;
-    // std::cout << n1 << "|" << n2 << "|" << delta << "||" << nnodes <<
-    // std::endl;
+      // if(this->hydrostationary)
+      // {
+      if (SF) {
+        this->_Qw[rec] += Qwin;
+      } else if (weights[j] > 0 && Qwin > 0) {
+        this->_Qw[rec] += weights[j] * Qwin;
+      }
+
+      // if(this->morphomode != MORPHO::NONE)
+      // {
+      // 	if(std::isfinite(this->_Qs[node]) == false)
+      // 		throw std::runtime_error("QS NAN");
+      // 	if(std::isfinite(this->_Qs[rec]) == false)
+      // 		throw std::runtime_error("QSREC NAN");
+      // 	this->_Qs[rec] += (SF == false)?weights[j] *
+      // this->_Qs[node]:this->_Qs[node] ; if(std::isfinite(this->_Qs[rec]) ==
+      // false)
+      // 	{
+      // 		std::cout << weights[j] << std::endl;;
+      // 		throw std::runtime_error("QSREC NAN AFTER");
+      // 	}
+      // }
+    }
+  }
+
+  // EXPERIMENTAL STUFF
+  // # MAin running function
+  void run_hydro_only() {
+    // Saving the topological number if needed
+    if (this->debugntopo)
+      this->DEBUGNTOPO = std::vector<fT>(this->connector->nnodes, 0);
+
+    this->debug_CFL = 0.;
+
+    this->tau_max = 0.;
+
+    if (this->courant_dt_hydro <= 0)
+      this->courant_dt_hydro = 1e-3;
+
+    // Graph Processing
+    this->graph_automator();
+
+    // Initialise the water discharge fields according to water input condition
+    // and other monitoring features:
+    this->init_Qw();
+
+    // Am I in SFD or MFD
+    bool SF = (this->hydromode == HYDRO::GRAPH_SFD);
+
+    // To be used if courant dt hydro is selected
+    fT tcourant_dt_hydro = std::numeric_limits<fT>::max();
+
+    // Caching neighbours, slopes and weights
+    auto receivers = this->connector->get_empty_neighbour();
+    std::array<fT, 8> weights, slopes;
+
+    // main loop
+    for (int i = this->graph->nnodes - 1; i >= 0; --i) {
+
+      // Getting next node in line
+      int node = this->get_istack_node(i);
+
+      // Processing case where the node is a model edge, or no data
+      // this function  returns true if the node was boundary and does not need
+      // to be processed THis is where all the boundary treatment happens, if
+      // you need to add something happening at the boundaries
+      if (this->_initial_check_boundary_pit(node, receivers))
+        continue;
 
-    if (delta == 1)
-      return n1 * 4;
-    else if (delta == this->nx + 1)
-      return n1 * 4 + 1;
-    else if (delta == this->nx)
-      return n1 * 4 + 2;
-    else if (delta == this->nx - 1)
-      return n1 * 4 + 3;
-    else
-      throw std::runtime_error(
-          "Fatal error in DAGGER::D8connector::linkidx_from_nodes");
-  }
+      // Getting the receivers
+      int nrecs;
+      if (SF)
+        nrecs = 1;
+      else
+        nrecs = this->connector->get_receivers_idx_links(node, receivers);
 
-  std::vector<int> get_ilinknodes_from_node_v1(int i) {
-    std::vector<int> out;
-    out.reserve(8);
-    int tn = this->get_right_idx_links(i);
-    if (tn > 0 && tn < this->nnodes * 4)
-      out.emplace_back(tn);
-    tn = this->get_bottomright_idx_links(i);
-    if (tn > 0 && tn < this->nnodes * 4)
-      out.emplace_back(tn);
-    tn = this->get_bottom_idx_links(i);
-    if (tn > 0 && tn < this->nnodes * 4)
-      out.emplace_back(tn);
-    tn = this->get_bottomleft_idx_links(i);
-    if (tn > 0 && tn < this->nnodes * 4)
-      out.emplace_back(tn);
-    tn = this->get_left_idx_links(i);
-    if (tn > 0 && tn < this->nnodes * 4)
-      out.emplace_back(tn);
-    tn = this->get_topleft_idx_links(i);
-    if (tn > 0 && tn < this->nnodes * 4)
-      out.emplace_back(tn);
-    tn = this->get_top_idx_links(i);
-    if (tn > 0 && tn < this->nnodes * 4)
-      out.emplace_back(tn);
-    tn = this->get_topright_idx_links(i);
-    if (tn > 0 && tn < this->nnodes * 4)
-      out.emplace_back(tn);
-    return out;
-  }
+      // Caching Slope max
+      fT Smax;
+      fT dw0max;
+      fT dx;
+      int recmax = node;
 
-  std::vector<std::pair<int, bool>> get_ilinknodes_from_nodev2(int i) {
-    std::vector<std::pair<int, bool>> out;
-    out.reserve(8);
-
-    if (!this->boundaries.normal_neighbouring_at_boundary(i) &&
-        !this->boundaries.is_normal_node(i)) {
-      int tn = this->get_right_idx_links(i);
-      bool val = false;
-      if (tn > 0 && tn < this->nnodes * 4)
-        val = true;
-      out.emplace_back(std::make_pair(tn, val));
-      tn = this->get_bottomright_idx_links(i);
-      if (tn > 0 && tn < this->nnodes * 4)
-        val = true;
-      out.emplace_back(std::make_pair(tn, val));
-      tn = this->get_bottom_idx_links(i);
-      if (tn > 0 && tn < this->nnodes * 4)
-        val = true;
-      out.emplace_back(std::make_pair(tn, val));
-      tn = this->get_bottomleft_idx_links(i);
-      if (tn > 0 && tn < this->nnodes * 4)
-        val = true;
-      out.emplace_back(std::make_pair(tn, val));
-      tn = this->get_left_idx_links(i);
-      if (tn > 0 && tn < this->nnodes * 4)
-        val = true;
-      out.emplace_back(std::make_pair(tn, val));
-      tn = this->get_topleft_idx_links(i);
-      if (tn > 0 && tn < this->nnodes * 4)
-        val = true;
-      out.emplace_back(std::make_pair(tn, val));
-      tn = this->get_top_idx_links(i);
-      if (tn > 0 && tn < this->nnodes * 4)
-        val = true;
-      out.emplace_back(std::make_pair(tn, val));
-      tn = this->get_topright_idx_links(i);
-      if (tn > 0 && tn < this->nnodes * 4)
-        val = true;
-      out.emplace_back(std::make_pair(tn, val));
-    } else
-      out = {std::make_pair(this->get_right_idx_links(i), true),
-             std::make_pair(this->get_bottomright_idx_links(i), true),
-             std::make_pair(this->get_bottom_idx_links(i), true),
-             std::make_pair(this->get_bottomleft_idx_links(i), true),
-             std::make_pair(this->get_left_idx_links(i), true),
-             std::make_pair(this->get_topleft_idx_links(i), true),
-             std::make_pair(this->get_top_idx_links(i), true),
-             std::make_pair(this->get_topright_idx_links(i), true)};
+      // NOTE:
+      //  No need to calculate the topological number anymore, but keeping it
+      //  for recording its value
+      fT topological_number_v2 = 0.;
 
-    return out;
-  }
+      this->_compute_slopes_weights_et_al(node, SF, Smax, slopes, weights,
+                                          nrecs, receivers, recmax, dx, dw0max,
+                                          topological_number_v2);
+
+      // Initialising the total Qout
+      fT Qwin = this->_Qw[node];
+
+      // precalculating the power
+      fT pohw = std::pow(this->_hw[node], TWOTHIRD);
+      // std:: cout << "pohw:" << pohw << "|" << this->_hw[node] << std::endl;
+
+      // Squarerooting Smax
+      // fT debug_S = Smax;
+      auto sqrtSmax = std::sqrt(Smax);
 
-  void get_ilinknodes_from_nodev3(int i,
-                                  std::vector<std::pair<int, bool>> &out) {
+      // Flow Velocity
+      fT u_flow = pohw * sqrtSmax / this->mannings(node);
+      // Volumetric discahrge
+      fT Qwout = dw0max * this->_hw[node] * u_flow;
+      // std::cout << Qwout << "|";
 
-    int tn = this->get_right_idx_links(i);
-    bool val = false;
-    if (tn > 0 && tn < this->nnodes * 4)
-      val = true;
-    out[0].first = tn;
-    out[0].second = val;
-    tn = this->get_bottomright_idx_links(i);
-    val = false;
-    if (tn > 0 && tn < this->nnodes * 4)
-      val = true;
-    out[1].first = tn;
-    out[1].second = val;
-    tn = this->get_bottom_idx_links(i);
-    val = false;
-    if (tn > 0 && tn < this->nnodes * 4)
-      val = true;
-    out[2].first = tn;
-    out[2].second = val;
-    tn = this->get_bottomleft_idx_links(i);
-    val = false;
-    if (tn > 0 && tn < this->nnodes * 4)
-      val = true;
-    out[3].first = tn;
-    out[3].second = val;
-    tn = this->get_left_idx_links(i);
-    val = false;
-    if (tn > 0 && tn < this->nnodes * 4)
-      val = true;
-    out[4].first = tn;
-    out[4].second = val;
-    tn = this->get_topleft_idx_links(i);
-    val = false;
-    if (tn > 0 && tn < this->nnodes * 4)
-      val = true;
-    out[5].first = tn;
-    out[5].second = val;
-    tn = this->get_top_idx_links(i);
-    val = false;
-    if (tn > 0 && tn < this->nnodes * 4)
-      val = true;
-    out[6].first = tn;
-    out[6].second = val;
-    tn = this->get_topright_idx_links(i);
-    val = false;
-    if (tn > 0 && tn < this->nnodes * 4)
-      val = true;
-    out[7].first = tn;
-    out[7].second = val;
-  }
-
-  int get_ilinknodes_from_node(int i, std::vector<int> &out) {
-    int nn = 0;
-    int tn = this->get_right_idx_links(i);
-    if (tn > 0 && tn < this->nnodes * 4) {
-      out[nn] = tn;
-      ++nn;
-    }
-    tn = this->get_bottomright_idx_links(i);
-    if (tn > 0 && tn < this->nnodes * 4) {
-      out[nn] = tn;
-      ++nn;
-    }
-    tn = this->get_bottom_idx_links(i);
-    if (tn > 0 && tn < this->nnodes * 4) {
-      out[nn] = tn;
-      ++nn;
-    }
-    tn = this->get_bottomleft_idx_links(i);
-    if (tn > 0 && tn < this->nnodes * 4) {
-      out[nn] = tn;
-      ++nn;
-    }
-    tn = this->get_left_idx_links(i);
-    if (tn > 0 && tn < this->nnodes * 4) {
-      out[nn] = tn;
-      ++nn;
-    }
-    tn = this->get_topleft_idx_links(i);
-    if (tn > 0 && tn < this->nnodes * 4) {
-      out[nn] = tn;
-      ++nn;
-    }
-    tn = this->get_top_idx_links(i);
-    if (tn > 0 && tn < this->nnodes * 4) {
-      out[nn] = tn;
-      ++nn;
-    }
-    tn = this->get_topright_idx_links(i);
-    if (tn > 0 && tn < this->nnodes * 4) {
-      out[nn] = tn;
-      ++nn;
-    }
-    return nn;
-  }
-
-  // returns a 1D bool array, false where no data
-  std::vector<bool> get_mask_array() {
-    std::vector<bool> mask(this->nnodes, true);
-    for (int i = 0; i < this->nnodes; ++i) {
-      if (this->boundaries.no_data(i))
-        mask[i] = false;
-    }
-    return mask;
-  }
-
-  template <class topo_t> void set_values_at_boundaries(topo_t &tarray, T val) {
-    auto array = format_input(tarray);
-    for (int i = 0; i < this->nnodes; ++i) {
-      if (this->boundaries.can_out(i))
-        array[i] = val;
+      // Eventually recording Smax
+      if (this->record_Sw)
+        this->_rec_Sw[node] = Smax;
+
+      // transfer fluxes
+      // Computing the transfer of water and sed
+      this->_compute_transfers(nrecs, recmax, node, SF, receivers, weights,
+                               Qwin, Qwout);
+
+      // Computing courant based dt
+      if (this->mode_dt_hydro == PARAM_DT_HYDRO::COURANT && u_flow > 0) {
+        fT provisional_dt = (this->courant_number * dx) / u_flow;
+        provisional_dt = std::min(provisional_dt, this->max_courant_dt_hydro);
+        provisional_dt = std::max(provisional_dt, this->min_courant_dt_hydro);
+        tcourant_dt_hydro = std::min(provisional_dt, tcourant_dt_hydro);
+      }
+
+      // computing hydro vertical motion changes for next time step
+      fT dH = this->dt_hydro(node) * (this->_Qw[node] - Qwout) /
+              this->connector->get_area_at_node(node);
+
+      this->_hw[node] += dH;
+      if (this->_hw[node] < 0) {
+        dH -= this->_hw[node];
+        this->_hw[node] = 0;
+      }
+      this->_surface[node] += dH;
+
+      if (this->record_Qw_out)
+        this->_rec_Qwout[node] += Qwout;
+    }
+
+    // if(this->tau_max > 500)
+    //  std::cout << "WARNING::tau_max is " << this->tau_max << std::endl;
+
+    // END OF MAIN LOOP
+
+    // Computing final courant based dt
+
+    if (this->mode_dt_hydro == PARAM_DT_HYDRO::COURANT) {
+      if (this->courant_dt_hydro == -1)
+        this->courant_dt_hydro = 1e-3;
+      else if (tcourant_dt_hydro > 0 &&
+               tcourant_dt_hydro != std::numeric_limits<fT>::max())
+        this->courant_dt_hydro = tcourant_dt_hydro;
+    }
+
+    // if (this->convergence_mode == CONVERGENCE::ALL ||
+    //     this->convergence_mode == CONVERGENCE::DHW) {
+    //   for (int i = 0; i < this->n_nodes_convergence(); ++i)
+    //     this->conv_dhw[i].emplace_back(
+    //         vmot_hw[this->conv_nodes
+    //                     [i]]); // /this->dt_hydro(this->conv_nodes[i]));
+    // }
+
+    if (this->convergence_mode == CONVERGENCE::ALL ||
+        this->convergence_mode == CONVERGENCE::QWR) {
+      for (int i = 0; i < this->n_nodes_convergence(); ++i)
+        this->conv_Qr[i].emplace_back(this->_rec_Qwout[this->conv_nodes[i]] /
+                                      this->_Qw[this->conv_nodes[i]]);
     }
   }
 
-  int get_nneighbours() { return 8; }
-};
+  // EXPERIMENTAL STUFF
+  // # MAin running function
+  void run_experimental() {
+    this->hydromode = HYDRO::GRAPH_SFD;
+    // Saving the topological number if needed
+    if (this->debugntopo)
+      this->DEBUGNTOPO = std::vector<fT>(this->connector->nnodes, 0);
+
+    this->debug_CFL = 0.;
+
+    this->tau_max = 0.;
+
+    if (this->courant_dt_hydro <= 0)
+      this->courant_dt_hydro = 1e-3;
 
-//  DEPRECATED AND MOVED OUTSIDE OF THE CONNECTOR
-// 	template <class topo_t>
-// 	std::vector<double> PriorityFlood(topo_t& ttopography)
-// 	{
-// 		std::random_device rd; // obtain a random number from hardware
-// 	  std::mt19937 gen(rd()); // seed the generator
-// 	  std::uniform_real_distribution<> distr(1e-7, 1e-6); // define the
-// range
-
-// 		auto tttopography = format_input(ttopography);
-// 		std::vector<double> topography = to_vec(tttopography);
-
-// 	  PQ_i_d open;
-// 	  std::queue<PQ_helper<int,double> > pit;
-
-// 	  uint64_t processed_cells = 0;
-// 	  uint64_t pitc            = 0;
-// 	  int      false_pit_cells = 0;
-// 	  double PitTop = -9999;
-
-// 	  std::vector<bool> closed(this->nnodes,false);
-
-// 	  // RDLOG_PROGRESS<<"Adding cells to the priority queue...";
-// 	  for(int i = 0; i<this->nnodes; ++i)
-// 	  {
-// 	  	if(this->can_flow_out_there(i))
-// 	  	{
-// 	  		closed[i] = true;
-// 	  		open.emplace(i,topography[i]);
-// 	  	}
-// 	  }
-
-// 	  // RDLOG_PROGRESS<<"Performing Priority-Flood+Epsilon...";
-// 	  auto neighbours = this->get_empty_neighbour();
-
-// 	  while(open.size()>0 || pit.size()>0)
-// 	  {
-// 	    PQ_helper<int,double> c;
-
-// 	    if(pit.size()>0 && open.size()>0 &&
-// open.top().score==pit.front().score)
-// 	    {
-// 	      c=open.top(); open.pop();
-// 	      PitTop=-9999;
-// 	    }
-// 	    else if(pit.size()>0)
-// 	    {
-// 	      c=pit.front(); pit.pop();
-// 	      if(PitTop==-9999)
-// 	        PitTop=topography[c.node];
-// 	    }
-// 	    else
-// 	    {
-// 	      c=open.top(); open.pop();
-// 	      PitTop=-9999;
-// 	    }
-// 	    processed_cells++;
-
-// 	    int nn = this->get_neighbour_idx(c.node, neighbours);
-// 	    for(int tnn = 0; tnn<nn; ++nn)
-// 	    {
-// 	    	int n = neighbours[tnn];
-// 	      if(this->is_active(n) == false)
-// 	      	continue;
-
-// 	      if(closed[n])
-// 	        continue;
-
-// 	      closed[n]=true;
-// 	      if(topography[n] <=
-// std::nextafter(c.score,std::numeric_limits<double>::infinity()))
-// 	      {
-// 	        if(PitTop!=-9999 && PitTop<topography[n] &&
-// std::nextafter(c.score,std::numeric_limits<double>::infinity())>=topography[n])
-// 	          ++false_pit_cells;
-
-// 	        ++pitc;
-// 	        //
-// topography[n]=std::nextafter(c.score,std::numeric_limits<double>::infinity());
-// 	        topography[n] = c.score + distr(gen);
-// 	        pit.emplace(n,topography[n]);
-// 	      } else
-// 	        open.emplace(n,topography[n]);
-// 	    }
-// 	  }
-
-// 	  return topography;
-// 	}
-
-// 	template<class topo_t>
-// 	void InitPriorityQue(
-// 	  topo_t& topography,
-// 	  std::vector<bool>& flag,
-// 	  PQ_i_d& priorityQueue
-// 	)
-// 	{
-
-// 	  std::queue<PQ_helper<int,double> > depressionQue;
-
-// 	  // push border cells into the PQ
-// 	  auto neighbours = this->get_empty_neighbour();
-// 	  for(int i=0; i < this->nnodes; ++i)
-// 	  {
-// 	    if (flag[i]) continue;
-
-// 	    if (this->can_flow_even_go_there(i) == false)
-// 	    {
-// 	      flag[i] = true;
-// 	      int nn = this->get_neighbour_idx(i,neighbours);
-
-// 	      for (int tnn =0; tnn < nn; ++tnn)
-// 	      {
-
-// 	      	int n = neighbours[tnn];
-
-// 	        if (flag[n])
-// 	          continue;
-// 	        if (this->can_flow_even_go_there(n))
-// 	        {
-// 	          priorityQueue.emplace(n,topography[n]);
-// 	          flag[n]=true;
-// 	        }
-// 	      }
-// 	    }
-// 	    else if(this->can_flow_out_there(i))
-// 	    {
-// 	      //on the DEM border
-// 	      priorityQueue.emplace(i,topography[i]);
-// 	      flag[i]=true;
-// 	    }
-// 	  }
-// 	}
-
-// 	template<class topo_t>
-// 	void ProcessTraceQue(
-// 	  topo_t& topography,
-// 	  std::vector<bool>& flag,
-// 	  std::queue<PQ_helper<int,double> >& traceQueue,
-// 	  PQ_i_d& priorityQueue
-// 	)
-// 	{
-// 	  std::queue<PQ_helper<int,double>  > potentialQueue;
-// 	  int indexThreshold=2;  //index threshold, default to 2
-// 	  auto neighbours = this->get_empty_neighbour();
-// 	  while (!traceQueue.empty())
-// 	  {
-// 	    const auto node = traceQueue.front();
-// 	    traceQueue.pop();
-
-// 	    bool Mask[5][5]={{false},{false},{false},{false},{false}};
-
-// 	    int nn = this->get_neighbour_idx(node.node, neighbours);
-
-// 	    for (int tnn=0; tnn<nn; ++tnn)
-// 	    {
-// 	    	int n = neighbours[tnn];
-
-// 	      if(flag[n])
-// 	        continue;
-
-// 	      if (topography[n] > node.score)
-// 	      {
-// 	        traceQueue.emplace(n, topography[n]);
-// 	        flag[n]=true;
-// 	      }
-// 	      else
-// 	      {
-// 	        //initialize all masks as false
-// 	        bool have_spill_path_or_lower_spill_outlet=false; //whether cell
-// n has a spill path or a lower spill outlet than node if n is a depression
-// cell 	        auto nneighs = this->get_neighbours_idx_richdemlike(n);
-// int row,col; this->rowcol_from_node_id(node.node,row,col); int nrow,ncol;
-// this->rowcol_from_node_id(n,nrow,ncol); 	        int incr=0; for(auto
-// nn:nneighs)
-// 	        {
-// 	        	++incr;
-// 	        	// Checking node validity
-// 	        	if(nn<0 || nn>= this->nnodes)
-// 	        		continue;
-
-// 	        	int nnrow,nncol;
-// 	        	this->rowcol_from_node_id(nn,nnrow,nncol);
-// 	          if( (Mask[nnrow-row+2][nncol-col+2]) || (flag[nn] &&
-// topography[nn] < node.score) )
-// 	          {
-// 	            Mask[nrow-row+2][ncol-col+2]=true;
-// 	            have_spill_path_or_lower_spill_outlet=true;
-// 	            break;
-// 	          }
-// 	        }
-
-// 	        if(!have_spill_path_or_lower_spill_outlet)
-// 	        {
-// 	          if (incr<indexThreshold) potentialQueue.push(node);
-// 	          else
-// 	            priorityQueue.push(node);
-// 	          break; // make sure node is not pushed twice into PQ
-// 	        }
-// 	      }
-// 	    }//end of for loop
-// 	  }
-
-// 	  while (!potentialQueue.empty())
-// 	  {
-// 	    const auto node = potentialQueue.front();
-// 	    potentialQueue.pop();
-
-// 	    //first case
-// 	    auto neigh = this->get_neighbours_idx_richdemlike(node.node);
-// 	    int incr = 0;
-// 	    for (auto n:neigh)
-// 	    {
-// 	    	++incr;
-
-// 	      if(flag[n])
-// 	        continue;
-
-// 	      priorityQueue.push(node);
-// 	      break;
-// 	    }
-// 	  }
-// 	}
-
-// 	template<class topo_t>
-// 	void ProcessPit(
-// 	  topo_t& topography,
-// 	  std::vector<bool>& flag,
-// 	  std::queue<PQ_helper<int,double> >& depressionQue,
-// 	  std::queue<PQ_helper<int,double> >& traceQueue
-// 	)
-// 	{
-// 		auto neighbours = this->get_empty_neighbour();
-// 	  while (!depressionQue.empty())
-// 	  {
-// 	    auto node = depressionQue.front();
-// 	    depressionQue.pop();
-// 	    int nn = this->get_neighbour_idx(node.node, neighbours);
-// 	    for (int tnn = 0; tnn<nn;++tnn)
-// 	    {
-// 	    	int n = neighbours[tnn];
-// 	      if (flag[n])
-// 	        continue;
-
-// 	      const auto iSpill = topography[n];
-// 	      if (iSpill > node.score)
-// 	      { // Dlope cell
-// 	        flag[n]=true;
-// 	        traceQueue.emplace(n,iSpill);
-// 	        continue;
-// 	      }
-// 	      // Depression cell
-// 	      flag[n] = true;
-// 	      topography[n] = node.score + 1e-6 * this->randu->get();
-// 	      depressionQue.emplace(n,topography[n]);
-// 	    }
-// 	  }
-// 	}
-
-// 	template<class topo_t>
-// 	std::vector<double> PriorityFlood_Wei2018(topo_t &ttopography)
-// 	{
-// 	  std::queue<PQ_helper<int,double> > traceQueue;
-// 	  std::queue<PQ_helper<int,double> > depressionQue;
-
-// 	  std::vector<bool> flag(this->nnodes,false);
-// 	  std::vector<double> topography = to_vec(ttopography);
-
-// 	  PQ_i_d priorityQueue;
-
-// 	  this->InitPriorityQue(topography,flag,priorityQueue);
-
-// 	  auto neighbours = this->get_empty_neighbour();
-
-// 	  while (!priorityQueue.empty())
-// 	  {
-// 	    const auto tmpNode = priorityQueue.top();
-// 	    priorityQueue.pop();
-
-// 	    int nn = this->get_neighbour_idx(tmpNode.node, neighbours);
-
-// 	    for(int tnn=0; tnn< nn; ++tnn)
-// 	    {
-// 	    	int n = neighbours[tnn];
-// 	      if(flag[n])
-// 	        continue;
-
-// 	      auto iSpill = topography[n];
-
-// 	      if (iSpill <= tmpNode.score)
-// 	      {
-// 	        //depression cell
-// 	        topography[n] = tmpNode.score + 1e-3 + 1e-6 *
-// this->randu->get(); 	        flag[n] = true;
-// depressionQue.emplace(n,topography[n]);
-// 	        this->ProcessPit(topography,flag,depressionQue,traceQueue);
-// 	      }
-// 	      else
-// 	      {
-// 	        //slope cell
-// 	        flag[n] = true;
-// 	        traceQueue.emplace(n,iSpill);
-// 	      }
-// 	      ProcessTraceQue(topography,flag,traceQueue,priorityQueue);
-// 	    }
-// 	  }
+    // Graph Processing
+    this->graph_automator();
 
-// 	  return topography;
-// 	}
+    // Initialise the water discharge fields according to water input condition
+    // and other monitoring features:
+    this->init_Qw();
 
-// end of namespace
-}; // namespace DAGGER
+    std::vector<fT> tQwin = this->graph->_accumulate_constant_downstream_SFD(
+        this->precipitations(0));
+    std::vector<fT> tQwout(this->connector->nnodes, 0.);
+    ;
 
+// main loop
+#ifdef _OPENMP
+#pragma omp parallel for num_threads(4)
 #endif
+    for (int node = 0; node < this->connector->nnodes; ++node) {
+      // Caching Slope max
+      fT Smax = this->connector->SS[node];
+      fT dx = this->connector->Sdistance2receivers[node];
+      fT dw0max = this->connector->get_travers_dy_from_dx(dx);
+      int recmax = this->connector->_Sreceivers[node];
+
+      // precalculating the power
+      fT pohw = std::pow(this->_hw[node], TWOTHIRD);
+      auto sqrtSmax = std::sqrt(Smax);
+
+      // Flow Velocity
+      fT u_flow = pohw * sqrtSmax / this->mannings(node);
+      // Volumetric discahrge
+      tQwout[node] = dw0max * this->_hw[node] * u_flow;
+
+      // // Computing courant based dt
+      // if (this->mode_dt_hydro == PARAM_DT_HYDRO::COURANT && u_flow > 0) {
+      //   fT provisional_dt = (this->courant_number * dx) / u_flow;
+      //   provisional_dt = std::min(provisional_dt,
+      //   this->max_courant_dt_hydro); provisional_dt =
+      //   std::max(provisional_dt, this->min_courant_dt_hydro);
+      //   tcourant_dt_hydro = std::min(provisional_dt, tcourant_dt_hydro);
+      // }
+    }
+
+#ifdef _OPENMP
+#pragma omp parallel for num_threads(4)
+#endif
+    for (int node = 0; node < this->connector->nnodes; ++node) {
+      // computing hydro vertical motion changes for next time step
+      fT dH = this->dt_hydro(node) * (this->_Qw[node] - tQwout[node]) /
+              this->connector->get_area_at_node(node);
+      this->_hw[node] += dH;
+      if (this->_hw[node] < 0) {
+        dH -= this->_hw[node];
+        this->_hw[node] = 0;
+      }
+      this->_surface[node] += dH;
+    }
+
+    if (this->record_Qw_out)
+      this->_rec_Qwout = tQwout;
+
+    // if(this->tau_max > 500)
+    //  std::cout << "WARNING::tau_max is " << this->tau_max << std::endl;
+
+    // END OF MAIN LOOP
+
+    // Computing final courant based dt
+
+    // if (this->mode_dt_hydro == PARAM_DT_HYDRO::COURANT) {
+    //   if (this->courant_dt_hydro == -1)
+    //     this->courant_dt_hydro = 1e-3;
+    //   else if (tcourant_dt_hydro > 0 &&
+    //            tcourant_dt_hydro != std::numeric_limits<fT>::max())
+    //     this->courant_dt_hydro = tcourant_dt_hydro;
+    // }
+
+    // if (this->convergence_mode == CONVERGENCE::ALL ||
+    //     this->convergence_mode == CONVERGENCE::DHW) {
+    //   for (int i = 0; i < this->n_nodes_convergence(); ++i)
+    //     this->conv_dhw[i].emplace_back(
+    //         vmot_hw[this->conv_nodes
+    //                     [i]]); // /this->dt_hydro(this->conv_nodes[i]));
+    // }
+
+    // if (this->convergence_mode == CONVERGENCE::ALL ||
+    //     this->convergence_mode == CONVERGENCE::QWR) {
+    //   for (int i = 0; i < this->n_nodes_convergence(); ++i)
+    //     this->conv_Qr[i].emplace_back(this->_rec_Qwout[this->conv_nodes[i]] /
+    //                                   this->_Qw[this->conv_nodes[i]]);
+    // }
+  }
+};
+// end of graphflood class
+
+} // namespace DAGGER
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `daggerpy-0.0.5/includes/_priority_flood.hpp` & `daggerpy-0.0.6/includes/_priority_flood.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/includes/boost_spread_sort.hpp` & `daggerpy-0.0.6/includes/boost_spread_sort.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/includes/boundary_conditions.hpp` & `daggerpy-0.0.6/includes/boundary_conditions.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/includes/connector_checker.hpp` & `daggerpy-0.0.6/includes/connector_checker.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,134 @@
 /*
-Defines the standardised loose connection of the connectors.
+Defines the standardised loose connection of the connectors. 
 
 There are 2 different level of standards:
 
-        - the generic standard, defining the functions that will be called in
-the different modules. They are the only one allowed in module accepting
-different types of connectors.
-
-        - the specifyers standards, defining function specific to build, set and
-customise given subsets of connectors. For example a regular grid will need nx
-and ny, not needed by a voronoi one. THESE CAN ONLY BE CALLED OUTSIDE OF THE
-MODULES. The modules should not need to know how the connector is structured
-(loosely connected).
-
-It uses phantom functions, called during the building of a new connector,
-checking the said connector has all the required functions to fit the template.
-
-
-A typical script would construct the connector first, calling generic and
-specific functions, then throw the connector inside the module (e.g. graph,
-graphflood, trackscape) where it would only use the generic functions.
-
-That way, I can for example build a connector from a regular grid, setting the
-nx, ny, dx, dy and boundary condition efficiently and then build graphflood with
-that connector.
+	- the generic standard, defining the functions that will be called in the different modules. 
+They are the only one allowed in module accepting different types of connectors.
+	
+	- the specifyers standards, defining function specific to build, set and customise given subsets of connectors. 
+For example a regular grid will need nx and ny, not needed by a voronoi one. 
+THESE CAN ONLY BE CALLED OUTSIDE OF THE MODULES. The modules should not need to know how the connector is structured (loosely connected). 
+
+It uses phantom functions, called during the building of a new connector, 
+checking the said connector has all the required functions to fit the template. 
+
+
+A typical script would construct the connector first, calling generic and specific functions, 
+then throw the connector inside the module (e.g. graph, graphflood, trackscape)
+where it would only use the generic functions.
+
+That way, I can for example build a connector from a regular grid, setting the nx, ny, dx, dy and boundary condition efficiently
+and then build graphflood with that connector.
 
 */
 
+
 #ifndef CONNECTOR_CHECKER_HPP
 #define CONNECTOR_CHECKER_HPP
 
-/// Generic checker: checks if the connector has the minimal set of functions to
-/// be accepted by the other modules
-template <class Connector_t, class fT, class CONTAINER_NEIGHBOURS_INT,
-          class CONTAINER_NEIGHBOURS_fT, class VECLIKE>
-void check_connector_template_generic(Connector_t &con) {
-
-  // Generic init function
-  // Return nothing, initialise the data structure.
-  // Argument: the number of nodes in the connector (includes no data)
-  void (Connector_t::*init)(int) = &Connector_t::init;
-
-  // Generic function precomputing elements in the graph.
-  // Its interpretation is free and really depends on the type of
-  // grid/connection is needed. This is where, for example, a connector
-  // optimised for cpu can compute all the receivers/donors information from
-  // topography; an irregular grid could regrid there, or simply, if the
-  // neighbouring never caches anything for a memory-saving connector, do
-  // nothing.
-  void (Connector_t::*compute)() = &Connector_t::compute;
-
-  // Connect a (new) topography, to be used for computing receivers/donors.
-  void (Connector_t::*connect_topo)(VECLIKE &) = &Connector_t::connect_topo;
-
-  // return the number of neighbours and fill the CONTAINER_NEIGHBOURS_INT with
-  // nn neighbours
-  int (Connector_t::*Neighbours)(int, CONTAINER_NEIGHBOURS_INT &) =
-      &Connector_t::Neighbours;
-
-  // return the number of neighbours and fill the CONTAINER_NEIGHBOURS_INT and
-  // with nn neighbours
-  int (Connector_t::*Neighbours)(int, CONTAINER_NEIGHBOURS_INT &,
-                                 CONTAINER_NEIGHBOURS_fT &) =
-      &Connector_t::neighbouring_nodes_and_distance;
-
-  // // return the number of neighbours and fill the CONTAINER_NEIGHBOURS_INT
-  // with nn links int (Connector_t::*Neighbours) (int,
-  // CONTAINER_NEIGHBOURS_INT&) = &Connector_t::neighbouring_links;
 
-  // Returns the area at a diven node index
-  fT (Connector_t::*Area)(int) = &Connector_t::Area;
+/// Generic checker: checks if the connector has the minimal set of functions to be accepted by the other modules
+template<class Connector_t, class fT, class CONTAINER_NEIGHBOURS_INT, class CONTAINER_NEIGHBOURS_fT, class VECLIKE>
+void check_connector_template_generic(Connector_t& con)
+{
+
+	// Generic init function
+	// Return nothing, initialise the data structure.
+	// Argument: the number of nodes in the connector (includes no data)
+	void (Connector_t::*init)(int) = &Connector_t::init;
+
+	// Generic function precomputing elements in the graph.
+	// Its interpretation is free and really depends on the type of grid/connection is needed.
+	// This is where, for example, a connector optimised for cpu can compute all the receivers/donors information from topography;
+	// an irregular grid could regrid there, or simply, if the neighbouring never caches anything for a memory-saving connector, do nothing.
+	void (Connector_t::*compute)() = &Connector_t::compute;
+
+	// Connect a (new) topography, to be used for computing receivers/donors.
+	void (Connector_t::*connect_topo)(VECLIKE&) = &Connector_t::connect_topo;
+
+	// return the number of neighbours and fill the CONTAINER_NEIGHBOURS_INT with nn neighbours
+	int (Connector_t::*Neighbours) (int, CONTAINER_NEIGHBOURS_INT&) = &Connector_t::Neighbours;
+
+	// return the number of neighbours and fill the CONTAINER_NEIGHBOURS_INT and  with nn neighbours
+	int (Connector_t::*Neighbours) (int, CONTAINER_NEIGHBOURS_INT&, CONTAINER_NEIGHBOURS_fT&) = &Connector_t::neighbouring_nodes_and_distance;
+
+	// // return the number of neighbours and fill the CONTAINER_NEIGHBOURS_INT with nn links
+	// int (Connector_t::*Neighbours) (int, CONTAINER_NEIGHBOURS_INT&) = &Connector_t::neighbouring_links;
+
+	// Returns the area at a diven node index
+	fT (Connector_t::*Area)(int) = &Connector_t::Area;
+
 }
 
-#endif
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+#endif
```

### Comparing `daggerpy-0.0.5/includes/cordonnier_versatile_2019.hpp` & `daggerpy-0.0.6/includes/cordonnier_versatile_2019.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/includes/depression_hierarchy.hpp` & `daggerpy-0.0.6/includes/depression_hierarchy.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/includes/fastflood.hpp` & `daggerpy-0.0.6/includes/fastflood.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/includes/fastflood_recorder.hpp` & `daggerpy-0.0.6/includes/fastflood_recorder.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/includes/graph.hpp` & `daggerpy-0.0.6/includes/graph.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/includes/hillshading.hpp` & `daggerpy-0.0.6/includes/hillshading.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/includes/npy.hpp` & `daggerpy-0.0.6/includes/npy.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/includes/popscape.hpp` & `daggerpy-0.0.6/includes/popscape.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/includes/popscape_utils.hpp` & `daggerpy-0.0.6/includes/popscape_utils.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/includes/priority_flood.hpp` & `daggerpy-0.0.6/includes/priority_flood.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/includes/simple_depression_solver.hpp` & `daggerpy-0.0.6/includes/simple_depression_solver.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/includes/trackscape.hpp` & `daggerpy-0.0.6/includes/trackscape.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/includes/trackscape_utils.hpp` & `daggerpy-0.0.6/includes/trackscape_utils.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/includes/utils.hpp` & `daggerpy-0.0.6/includes/utils.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/includes/veque.hpp` & `daggerpy-0.0.6/includes/veque.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/includes/wrap_helper.hpp` & `daggerpy-0.0.6/includes/wrap_helper.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/includes/wrap_helper_MATLAB.hpp` & `daggerpy-0.0.6/includes/wrap_helper_MATLAB.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/includes/wrap_helper_julia.hpp` & `daggerpy-0.0.6/includes/wrap_helper_julia.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/includes/wrap_helper_python.hpp` & `daggerpy-0.0.6/includes/wrap_helper_python.hpp`

 * *Files identical despite different names*

### Comparing `daggerpy-0.0.5/main.cpp` & `daggerpy-0.0.6/main.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -17,42 +17,42 @@
 #include "river_tools_python.hpp"
 
 using namespace DAGGER;
 
 template <typename CONNECTOR_T>
 void declare_graph(py::module &m, std::string typestr) {
 
-  py::class_<graph<double, CONNECTOR_T>>(m, typestr.c_str(), R"pdoc(
+	py::class_<graph<double, CONNECTOR_T>>(m, typestr.c_str(), R"pdoc(
 Full Graph module, to plug on a connector to unlock non-local topological operations.
 
 Description:
 ------------
 
 The graph manages all non local connectivity and ensures the graph is acyclic.
 It contains all the routines for topological ordering, local minima resolving
 (multiple methods), or accumulating values in the upstream/downstream directions
 
 
 Authors:
 --------
 B.G.)pdoc")
 
-      .def(py::init<CONNECTOR_T &>())
-      .def(
-          "init_graph", &graph<double, CONNECTOR_T>::init_graph,
-          R"pdoc(Initialise the data structure and allocate memory (mostly used internally).)pdoc")
-      .def(
-          "set_opt_stst_rerouting",
-          &graph<double, CONNECTOR_T>::set_opt_stst_rerouting, py::arg("onoff"),
-          R"pdoc(Activate (true) or deactivate (false) an optimiser. Most of the time does not make a difference but can _eventually_ approximate a few link a bit more precisely when rerouting local minimas.)pdoc")
-      .def("compute_graph",
-           &graph<double, CONNECTOR_T>::template compute_graph<
-               py::array_t<double, 1>, py::array>,
-           py::arg("topography"), py::arg("no_MFD"), py::arg("quicksort_on"),
-           R"pdoc(
+		.def(py::init<CONNECTOR_T &>())
+		.def(
+			"init_graph", &graph<double, CONNECTOR_T>::init_graph,
+			R"pdoc(Initialise the data structure and allocate memory (mostly used internally).)pdoc")
+		.def(
+			"set_opt_stst_rerouting",
+			&graph<double, CONNECTOR_T>::set_opt_stst_rerouting, py::arg("onoff"),
+			R"pdoc(Activate (true) or deactivate (false) an optimiser. Most of the time does not make a difference but can _eventually_ approximate a few link a bit more precisely when rerouting local minimas.)pdoc")
+		.def("compute_graph",
+			 &graph<double, CONNECTOR_T>::template compute_graph<
+				 py::array_t<double, 1>, py::array>,
+			 py::arg("topography"), py::arg("no_MFD"), py::arg("quicksort_on"),
+			 R"pdoc(
 Full computation of the graph (connector updates of links included).
 
 Description
 -------------
 
 COmpute the graph by (i) updating receivers/donors, (ii) resolving local minimas
 with the method and (iii) computing topological sortings. Can be set to SFD only
@@ -79,25 +79,25 @@
 
 Authors:
 --------
 B.G.
 
 )pdoc"
 
-           )
-      .def("is_Sstack_full", &graph<double, CONNECTOR_T>::is_Sstack_full,
-           R"pdoc(Debugging function, to ignore)pdoc")
-      .def("activate_opti_sparse_border_cordonnier",
-           &graph<double, CONNECTOR_T>::activate_opti_sparse_border_cordonnier,
-           R"pdoc(Debugging function, to ignore)pdoc")
-      .def("get_all_nodes_upstream_of",
-           &graph<double, CONNECTOR_T>::template get_all_nodes_upstream_of<
-               py::array_t<int, 1>>,
-           py::arg("node"), py::arg("only_SFD"),
-           R"pdoc(
+			 )
+		.def("is_Sstack_full", &graph<double, CONNECTOR_T>::is_Sstack_full,
+			 R"pdoc(Debugging function, to ignore)pdoc")
+		.def("activate_opti_sparse_border_cordonnier",
+			 &graph<double, CONNECTOR_T>::activate_opti_sparse_border_cordonnier,
+			 R"pdoc(Debugging function, to ignore)pdoc")
+		.def("get_all_nodes_upstream_of",
+			 &graph<double, CONNECTOR_T>::template get_all_nodes_upstream_of<
+				 py::array_t<int, 1>>,
+			 py::arg("node"), py::arg("only_SFD"),
+			 R"pdoc(
 Fecth all the nodes upstream of a given one.
 
 Description
 -------------
 
 Use the SFD stack structure from Braun and Willett (2013) to gather all the
 nodes upstream of a given one. Effectively labels a watershed from a custom
@@ -118,19 +118,19 @@
 indices of upstream locations.
 
 Authors:
 --------
 B.G.
 
 )pdoc")
-      .def("get_all_nodes_downstream_of",
-           &graph<double, CONNECTOR_T>::template get_all_nodes_downstream_of<
-               py::array_t<int, 1>>,
-           py::arg("node"), py::arg("only_SFD"),
-           R"pdoc(
+		.def("get_all_nodes_downstream_of",
+			 &graph<double, CONNECTOR_T>::template get_all_nodes_downstream_of<
+				 py::array_t<int, 1>>,
+			 py::arg("node"), py::arg("only_SFD"),
+			 R"pdoc(
 Fecth all the nodes downstream of a given one.
 
 Description
 -------------
 
 Use the SFD stack structure from Braun and Willett (2013) to gather all the
 nodes downstream of a given one. Effectively labels a water paths from a custom
@@ -151,18 +151,18 @@
 indices of downstream locations.
 
 Authors:
 --------
 B.G.
 
 )pdoc")
-      .def("get_SFD_stack",
-           &graph<double,
-                  CONNECTOR_T>::template get_SFD_stack<py::array_t<size_t, 1>>,
-           R"pdoc(
+		.def("get_SFD_stack",
+			 &graph<double,
+					CONNECTOR_T>::template get_SFD_stack<py::array_t<size_t, 1>>,
+			 R"pdoc(
 Returns the single flow stack (Braun and Willett. 2013) in "stack order".
 
 Description
 -------------
 
 Returns the single flow direction stack (sensu Braun and Willett (2013).
 Warning: it corresponds to the last computation (``compute_graph``) and will
@@ -180,18 +180,18 @@
 SFD stack array.
 
 Authors:
 --------
 B.G.
 
 )pdoc")
-      .def("get_MFD_stack",
-           &graph<double,
-                  CONNECTOR_T>::template get_MFD_stack<py::array_t<size_t, 1>>,
-           R"pdoc(
+		.def("get_MFD_stack",
+			 &graph<double,
+					CONNECTOR_T>::template get_MFD_stack<py::array_t<size_t, 1>>,
+			 R"pdoc(
 Returns the Multiple flow stack in "stack order".
 
 Description
 -------------
 
 Returns the multiple flow direction stack.
 
@@ -213,20 +213,20 @@
 
 Authors:
 --------
 B.G.
 
 )pdoc")
 
-      .def("accumulate_constant_downstream_SFD",
-           &graph<double, CONNECTOR_T>::
-               template accumulate_constant_downstream_SFD<
-                   py::array_t<double, 1>>,
-           py::arg("constant_value"),
-           R"pdoc(
+		.def("accumulate_constant_downstream_SFD",
+			 &graph<double, CONNECTOR_T>::
+				 template accumulate_constant_downstream_SFD<
+					 py::array_t<double, 1>>,
+			 py::arg("constant_value"),
+			 R"pdoc(
 Accumulates (integrate) a constant downstream in the SFD direction.
 
 Description
 -------------
 
 Sums a constant downstream in the single flow direction (each node adds the
 constant value and give it to its receivers following the inverse stack order).
@@ -244,20 +244,20 @@
 The 1D accumulated array (float, node size)
 
 Authors:
 --------
 B.G.
 
 )pdoc")
-      .def("accumulate_variable_downstream_SFD",
-           &graph<double, CONNECTOR_T>::
-               template accumulate_variable_downstream_SFD<
-                   py::array_t<double, 1>, py::array_t<double, 1>>,
-           py::arg("values"),
-           R"pdoc(
+		.def("accumulate_variable_downstream_SFD",
+			 &graph<double, CONNECTOR_T>::
+				 template accumulate_variable_downstream_SFD<
+					 py::array_t<double, 1>, py::array_t<double, 1>>,
+			 py::arg("values"),
+			 R"pdoc(
 Accumulates (integrate) a variable downstream in the SFD direction.
 
 Description
 -------------
 
 Sums a variable downstream in the single flow direction (each node adds the
 variable value and give it to its receivers following the inverse stack order).
@@ -277,20 +277,20 @@
 The 1D accumulated array (float, node size)
 
 Authors:
 --------
 B.G.
 
 )pdoc")
-      .def("accumulate_constant_downstream_MFD",
-           &graph<double, CONNECTOR_T>::
-               template accumulate_constant_downstream_MFD<
-                   py::array_t<double, 1>, py::array_t<double, 1>>,
-           py::arg("weights"), py::arg("constant_value"),
-           R"pdoc(
+		.def("accumulate_constant_downstream_MFD",
+			 &graph<double, CONNECTOR_T>::
+				 template accumulate_constant_downstream_MFD<
+					 py::array_t<double, 1>, py::array_t<double, 1>>,
+			 py::arg("weights"), py::arg("constant_value"),
+			 R"pdoc(
 Accumulates (integrate) a constant downstream in the MFD direction.
 
 Description
 -------------
 
 Sums a constant downstream in the multiple flow direction (each node adds the
 variable value and give it to its receivers following the inverse stack order).
@@ -314,20 +314,20 @@
 The 1D accumulated array (float, node size)
 
 Authors:
 --------
 B.G.
 
 )pdoc")
-      .def("accumulate_variable_downstream_MFD",
-           &graph<double, CONNECTOR_T>::
-               template accumulate_variable_downstream_MFD<
-                   py::array_t<double, 1>, py::array_t<double, 1>>,
-           py::arg("weights"), py::arg("values"),
-           R"pdoc(
+		.def("accumulate_variable_downstream_MFD",
+			 &graph<double, CONNECTOR_T>::
+				 template accumulate_variable_downstream_MFD<
+					 py::array_t<double, 1>, py::array_t<double, 1>>,
+			 py::arg("weights"), py::arg("values"),
+			 R"pdoc(
 Accumulates (integrate) a variable downstream in the MFD direction.
 
 Description
 -------------
 
 Sums a variable value of node size downstream in the multiple flow direction
 (each node adds the variable value and give it to its receivers following the
@@ -353,17 +353,17 @@
 The 1D accumulated array (float, node size)
 
 Authors:
 --------
 B.G.
 
 )pdoc")
-      .def("set_LMR_method", &graph<double, CONNECTOR_T>::set_LMR_method,
-           py::arg("LMR_method"),
-           R"pdoc(
+		.def("set_LMR_method", &graph<double, CONNECTOR_T>::set_LMR_method,
+			 py::arg("LMR_method"),
+			 R"pdoc(
 Sets the Local Minima Resolver method.
 
 Description
 -------------
 
 Select which LMR (Local Minima Resolver) to use. It needs to be a LMR enum value
 and will dictacte if/how the local minima (internal pits) are rerouted (or not).
@@ -386,30 +386,30 @@
 
 
 Authors:
 --------
 B.G.
 
 )pdoc")
-      .def(
-          "set_minimum_slope_for_LMR",
-          &graph<double, CONNECTOR_T>::set_minimum_slope_for_LMR,
-          py::arg("slope"),
-          R"pdoc(LMR solvers impose a numerical topographic gradient to avoid 0 slopes. Default is 1e-5.)pdoc")
-      .def(
-          "set_slope_randomness_for_LMR",
-          &graph<double, CONNECTOR_T>::set_slope_randomness_for_LMR,
-          py::arg("magnitude"),
-          R"pdoc(Avoid falt surfaces by imposing a very small randomness when processing local minimas. Must be an order of magitude smaller than the  minimal slope.)pdoc")
-
-      // Distance functions
-      .def("get_SFD_distance_from_outlets",
-           &graph<double, CONNECTOR_T>::template get_SFD_distance_from_outlets<
-               py::array_t<double, 1>>,
-           R"pdoc(
+		.def(
+			"set_minimum_slope_for_LMR",
+			&graph<double, CONNECTOR_T>::set_minimum_slope_for_LMR,
+			py::arg("slope"),
+			R"pdoc(LMR solvers impose a numerical topographic gradient to avoid 0 slopes. Default is 1e-5.)pdoc")
+		.def(
+			"set_slope_randomness_for_LMR",
+			&graph<double, CONNECTOR_T>::set_slope_randomness_for_LMR,
+			py::arg("magnitude"),
+			R"pdoc(Avoid falt surfaces by imposing a very small randomness when processing local minimas. Must be an order of magitude smaller than the  minimal slope.)pdoc")
+
+		// Distance functions
+		.def("get_SFD_distance_from_outlets",
+			 &graph<double, CONNECTOR_T>::template get_SFD_distance_from_outlets<
+				 py::array_t<double, 1>>,
+			 R"pdoc(
 Calculates the distance from the outlets following the SFD.
 
 Description
 -------------
 
 Uses the SFD stack order to integrate the distance from the outlets to the
 sources. Useful for long profiles.
@@ -421,20 +421,20 @@
 
 Authors:
 --------
 B.G.
 
 )pdoc"
 
-           )
-      .def("get_SFD_min_distance_from_sources",
-           &graph<double, CONNECTOR_T>::
-               template get_SFD_min_distance_from_sources<
-                   py::array_t<double, 1>>,
-           R"pdoc(
+			 )
+		.def("get_SFD_min_distance_from_sources",
+			 &graph<double, CONNECTOR_T>::
+				 template get_SFD_min_distance_from_sources<
+					 py::array_t<double, 1>>,
+			 R"pdoc(
 Calculates the minimum distance from the sources following the SFD.
 
 Description
 -------------
 
 Uses the SFD stack in inverse order to integrate the distance from the sources
 toward the outlets. It keeps the minimum distance. Useful to identify the
@@ -446,19 +446,19 @@
 1D array of flow distance
 
 Authors:
 --------
 B.G.
 
 )pdoc")
-      .def("get_SFD_max_distance_from_sources",
-           &graph<double, CONNECTOR_T>::
-               template get_SFD_max_distance_from_sources<
-                   py::array_t<double, 1>>,
-           R"pdoc(
+		.def("get_SFD_max_distance_from_sources",
+			 &graph<double, CONNECTOR_T>::
+				 template get_SFD_max_distance_from_sources<
+					 py::array_t<double, 1>>,
+			 R"pdoc(
 Calculates the maximum distance from the sources following the SFD.
 
 Description
 -------------
 
 Uses the SFD stack in inverse order to integrate the distance from the sources
 toward the outlets. It keeps the maximum distance. Useful to identify the
@@ -470,19 +470,19 @@
 1D array of flow distance
 
 Authors:
 --------
 B.G.
 
 )pdoc")
-      .def("get_MFD_max_distance_from_sources",
-           &graph<double, CONNECTOR_T>::
-               template get_MFD_max_distance_from_sources<
-                   py::array_t<double, 1>>,
-           R"pdoc(
+		.def("get_MFD_max_distance_from_sources",
+			 &graph<double, CONNECTOR_T>::
+				 template get_MFD_max_distance_from_sources<
+					 py::array_t<double, 1>>,
+			 R"pdoc(
 Calculates the maximum distance from the sources following the MFD.
 
 Description
 -------------
 
 Uses the MFD stack in inverse order to integrate the distance from the sources
 toward the outlets. It keeps the maximum distance. Useful to identify the
@@ -494,19 +494,19 @@
 1D array of flow distance
 
 Authors:
 --------
 B.G.
 
 )pdoc")
-      .def("get_MFD_min_distance_from_sources",
-           &graph<double, CONNECTOR_T>::
-               template get_MFD_min_distance_from_sources<
-                   py::array_t<double, 1>>,
-           R"pdoc(
+		.def("get_MFD_min_distance_from_sources",
+			 &graph<double, CONNECTOR_T>::
+				 template get_MFD_min_distance_from_sources<
+					 py::array_t<double, 1>>,
+			 R"pdoc(
 Calculates the minimum distance from the sources following the MFD.
 
 Description
 -------------
 
 Uses the MFD stack in inverse order to integrate the distance from the sources
 toward the outlets. It keeps the minimum distance. Useful to identify the
@@ -518,19 +518,19 @@
 1D array of flow distance
 
 Authors:
 --------
 B.G.
 
 )pdoc")
-      .def("get_MFD_max_distance_from_outlets",
-           &graph<double, CONNECTOR_T>::
-               template get_MFD_max_distance_from_outlets<
-                   py::array_t<double, 1>>,
-           R"pdoc(
+		.def("get_MFD_max_distance_from_outlets",
+			 &graph<double, CONNECTOR_T>::
+				 template get_MFD_max_distance_from_outlets<
+					 py::array_t<double, 1>>,
+			 R"pdoc(
 Calculates the maximum distance from the outlet following the MFD.
 
 Description
 -------------
 
 Uses the MFD stack in inverse order to integrate the distance from the outlet
 toward the outlets. It keeps the maximum distance. Useful to identify the
@@ -542,19 +542,19 @@
 1D array of flow distance
 
 Authors:
 --------
 B.G.
 
 )pdoc")
-      .def("get_MFD_min_distance_from_outlets",
-           &graph<double, CONNECTOR_T>::
-               template get_MFD_min_distance_from_outlets<
-                   py::array_t<double, 1>>,
-           R"pdoc(
+		.def("get_MFD_min_distance_from_outlets",
+			 &graph<double, CONNECTOR_T>::
+				 template get_MFD_min_distance_from_outlets<
+					 py::array_t<double, 1>>,
+			 R"pdoc(
 Calculates the minimum distance from the outlet following the MFD.
 
 Description
 -------------
 
 Uses the MFD stack in inverse order to integrate the distance from the outlet
 toward the outlets. It keeps the minimum distance. Useful to identify the
@@ -567,19 +567,19 @@
 
 Authors:
 --------
 B.G.
 
 )pdoc")
 
-      // Watershed labelling
-      .def("get_SFD_basin_labels",
-           &graph<double, CONNECTOR_T>::template get_SFD_basin_labels<
-               py::array_t<int, 1>>,
-           R"pdoc(
+		// Watershed labelling
+		.def("get_SFD_basin_labels",
+			 &graph<double, CONNECTOR_T>::template get_SFD_basin_labels<
+				 py::array_t<int, 1>>,
+			 R"pdoc(
 Labels SFD watersheds with unique ID.
 
 Description
 -------------
 
 Uses the SFD stack order to label very efficiently basins.
 
@@ -590,18 +590,18 @@
 
 Authors:
 --------
 B.G.
 
 )pdoc")
 
-      .def("get_drainage_area_SFD",
-           &graph<double, CONNECTOR_T>::template get_drainage_area_SFD<
-               py::array_t<double, 1>>,
-           R"pdoc(
+		.def("get_drainage_area_SFD",
+			 &graph<double, CONNECTOR_T>::template get_drainage_area_SFD<
+				 py::array_t<double, 1>>,
+			 R"pdoc(
 Labels SFD watersheds with unique ID.
 
 Description
 -------------
 
 Uses the SFD stack order to label very efficiently basins.
 
@@ -612,18 +612,18 @@
 
 Authors:
 --------
 B.G.
 
 )pdoc")
 
-      .def("get_drainage_area_MFD",
-           &graph<double, CONNECTOR_T>::template get_drainage_area_MFD<
-               py::array_t<double, 1>, py::array_t<double, 1>>,
-           R"pdoc(
+		.def("get_drainage_area_MFD",
+			 &graph<double, CONNECTOR_T>::template get_drainage_area_MFD<
+				 py::array_t<double, 1>, py::array_t<double, 1>>,
+			 R"pdoc(
 Labels MFD watersheds with unique ID.
 
 Description
 -------------
 
 Uses the MFD stack order to label very efficiently basins.
 
@@ -634,351 +634,351 @@
 
 Authors:
 --------
 B.G.
 
 )pdoc")
 
-      .def("get_n_pits", &graph<double, CONNECTOR_T>::get_n_pits,
-           R"pdoc(Return the number of internal pits (prior solving).)pdoc")
+		.def("get_n_pits", &graph<double, CONNECTOR_T>::get_n_pits,
+			 R"pdoc(Return the number of internal pits (prior solving).)pdoc")
 
-      .def(
-          "get_debug_mask", &graph<double, CONNECTOR_T>::get_debug_mask,
-          R"pdoc(Ignore. Internal debugging mask process. Changes purpose and is mostly deactivated.)pdoc")
-
-      .def(
-          "get_debug_int", &graph<double, CONNECTOR_T>::get_debug_int,
-          R"pdoc(Ignore. Internal debugging int process. Changes purpose and is mostly deactivated.)pdoc")
+		.def(
+			"get_debug_mask", &graph<double, CONNECTOR_T>::get_debug_mask,
+			R"pdoc(Ignore. Internal debugging mask process. Changes purpose and is mostly deactivated.)pdoc")
+
+		.def(
+			"get_debug_int", &graph<double, CONNECTOR_T>::get_debug_int,
+			R"pdoc(Ignore. Internal debugging int process. Changes purpose and is mostly deactivated.)pdoc")
 
-      ;
+		;
 }
 
 template <typename CONNECTOR_T>
 void declare_popscape_old(py::module &m, std::string typestr) {
-  py::class_<
-      popscape_old<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>>(
-      m, typestr.c_str())
-      .def(py::init<RANDNOISE, int, int, double, double>())
-      // .def_readwrite("graph",  &popscape_old<double, DAGGER::graph<double,
-      // CONNECTOR_T>, CONNECTOR_T >::graph) .def_readwrite("connector",
-      // &popscape_old<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T
-      // >::connector)
-      .def("solve_generic",
-           &popscape_old<double, DAGGER::graph<double, CONNECTOR_T>,
-                         CONNECTOR_T>::solve_generic)
-      .def("get_topo", &popscape_old<double, DAGGER::graph<double, CONNECTOR_T>,
-                                     CONNECTOR_T>::template get_topo<py::array>)
-      .def("get_QA", &popscape_old<double, DAGGER::graph<double, CONNECTOR_T>,
-                                   CONNECTOR_T>::template get_QA<py::array>)
-      .def("compute_graph",
-           &popscape_old<double, DAGGER::graph<double, CONNECTOR_T>,
-                         CONNECTOR_T>::compute_graph)
-      .def("compute_DA_SFD",
-           &popscape_old<double, DAGGER::graph<double, CONNECTOR_T>,
-                         CONNECTOR_T>::compute_DA_SFD)
-      .def("apply_uplift",
-           &popscape_old<double, DAGGER::graph<double, CONNECTOR_T>,
-                         CONNECTOR_T>::apply_uplift)
-      .def("apply_variable_uplift",
-           &popscape_old<double, DAGGER::graph<double, CONNECTOR_T>,
-                         CONNECTOR_T>::
-               template apply_variable_uplift<py::array_t<double, 1>>)
-      .def("solve_SFD_SPL_imp",
-           &popscape_old<double, DAGGER::graph<double, CONNECTOR_T>,
-                         CONNECTOR_T>::solve_SFD_SPL_imp)
-      .def("hydraulic_erosion_v0",
-           &popscape_old<double, DAGGER::graph<double, CONNECTOR_T>,
-                         CONNECTOR_T>::hydraulic_erosion_v0)
-      .def("normalise_topography",
-           &popscape_old<double, DAGGER::graph<double, CONNECTOR_T>,
-                         CONNECTOR_T>::normalise_topography)
-      // .def("run_SFD_exp_latmag", &popscape_old<double, DAGGER::graph<double,
-      // CONNECTOR_T>, CONNECTOR_T >::run_SFD_exp_latmag)
+	py::class_<
+		popscape_old<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>>(
+		m, typestr.c_str())
+		.def(py::init<RANDNOISE, int, int, double, double>())
+		// .def_readwrite("graph",  &popscape_old<double, DAGGER::graph<double,
+		// CONNECTOR_T>, CONNECTOR_T >::graph) .def_readwrite("connector",
+		// &popscape_old<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T
+		// >::connector)
+		.def("solve_generic",
+			 &popscape_old<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::solve_generic)
+		.def("get_topo", &popscape_old<double, DAGGER::graph<double, CONNECTOR_T>,
+									 CONNECTOR_T>::template get_topo<py::array>)
+		.def("get_QA", &popscape_old<double, DAGGER::graph<double, CONNECTOR_T>,
+									 CONNECTOR_T>::template get_QA<py::array>)
+		.def("compute_graph",
+			 &popscape_old<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::compute_graph)
+		.def("compute_DA_SFD",
+			 &popscape_old<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::compute_DA_SFD)
+		.def("apply_uplift",
+			 &popscape_old<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::apply_uplift)
+		.def("apply_variable_uplift",
+			 &popscape_old<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::
+				 template apply_variable_uplift<py::array_t<double, 1>>)
+		.def("solve_SFD_SPL_imp",
+			 &popscape_old<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::solve_SFD_SPL_imp)
+		.def("hydraulic_erosion_v0",
+			 &popscape_old<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::hydraulic_erosion_v0)
+		.def("normalise_topography",
+			 &popscape_old<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::normalise_topography)
+		// .def("run_SFD_exp_latmag", &popscape_old<double, DAGGER::graph<double,
+		// CONNECTOR_T>, CONNECTOR_T >::run_SFD_exp_latmag)
 
-      ;
+		;
 }
 
 template <typename CONNECTOR_T>
 void declare_popscape(py::module &m, std::string typestr) {
-  py::class_<popscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>>(
-      m, typestr.c_str())
-      .def(py::init<DAGGER::graph<double, CONNECTOR_T> &, CONNECTOR_T &>())
-      .def("StSt", &popscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                             CONNECTOR_T>::StSt)
-      .def("restriction", &popscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                                    CONNECTOR_T>::restriction)
-      .def("interpolation",
-           &popscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                     CONNECTOR_T>::interpolation)
-      .def("smooth", &popscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                               CONNECTOR_T>::smooth)
-      .def("set_topo",
-           &popscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                     CONNECTOR_T>::template set_topo<py::array_t<double, 1>>)
-      .def("get_topo",
-           &popscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                     CONNECTOR_T>::template get_topo<py::array_t<double, 1>>)
-      .def("get_QA",
-           &popscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                     CONNECTOR_T>::template get_QA<py::array_t<double, 1>>)
-      .def("get_chistar",
-           &popscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                     CONNECTOR_T>::template get_chistar<py::array_t<double, 1>>)
-      .def("simple_Kfchi", &popscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                                     CONNECTOR_T>::simple_Kfchi)
-      .def("simple_Kfz", &popscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                                   CONNECTOR_T>::simple_Kfz);
+	py::class_<popscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>>(
+		m, typestr.c_str())
+		.def(py::init<DAGGER::graph<double, CONNECTOR_T> &, CONNECTOR_T &>())
+		.def("StSt", &popscape<double, DAGGER::graph<double, CONNECTOR_T>,
+							 CONNECTOR_T>::StSt)
+		.def("restriction", &popscape<double, DAGGER::graph<double, CONNECTOR_T>,
+									CONNECTOR_T>::restriction)
+		.def("interpolation",
+			 &popscape<double, DAGGER::graph<double, CONNECTOR_T>,
+					 CONNECTOR_T>::interpolation)
+		.def("smooth", &popscape<double, DAGGER::graph<double, CONNECTOR_T>,
+								 CONNECTOR_T>::smooth)
+		.def("set_topo",
+			 &popscape<double, DAGGER::graph<double, CONNECTOR_T>,
+					 CONNECTOR_T>::template set_topo<py::array_t<double, 1>>)
+		.def("get_topo",
+			 &popscape<double, DAGGER::graph<double, CONNECTOR_T>,
+					 CONNECTOR_T>::template get_topo<py::array_t<double, 1>>)
+		.def("get_QA",
+			 &popscape<double, DAGGER::graph<double, CONNECTOR_T>,
+					 CONNECTOR_T>::template get_QA<py::array_t<double, 1>>)
+		.def("get_chistar",
+			 &popscape<double, DAGGER::graph<double, CONNECTOR_T>,
+					 CONNECTOR_T>::template get_chistar<py::array_t<double, 1>>)
+		.def("simple_Kfchi", &popscape<double, DAGGER::graph<double, CONNECTOR_T>,
+									 CONNECTOR_T>::simple_Kfchi)
+		.def("simple_Kfz", &popscape<double, DAGGER::graph<double, CONNECTOR_T>,
+									 CONNECTOR_T>::simple_Kfz);
 }
 
 template <typename CONNECTOR_T>
 void declare_trackscape(py::module &m, std::string typestr) {
-  py::class_<
-      trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>>(
-      m, typestr.c_str())
-      .def(py::init<>())
-      .def_readwrite("graph",
-                     &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                                 CONNECTOR_T>::graph)
-      .def_readwrite("connector",
-                     &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                                 CONNECTOR_T>::connector)
-      .def("init_random",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::init_random)
-      .def("init_perlin",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::init_perlin)
-      .def("get_topo", &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                                   CONNECTOR_T>::template get_topo<py::array>)
-      .def("get_hillshade",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::template get_hillshade<py::array>)
-      .def("get_h_sed", &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                                    CONNECTOR_T>::template get_h_sed<py::array>)
-      .def("get_Qw", &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                                 CONNECTOR_T>::template get_Qw<py::array>)
-      .def("get_Qs_fluvial",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::template get_Qs_fluvial<py::array>)
-      .def("get_Qs_hillslopes",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::template get_Qs_hillslopes<py::array>)
-      .def("get_precipitations",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::template get_precipitations<py::array>)
-      .def("set_full_stochastic",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::set_full_stochastic)
-      .def("run", &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                              CONNECTOR_T>::run)
-      .def("run_SFD", &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                                  CONNECTOR_T>::run_SFD)
-      .def("block_uplift",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::block_uplift)
-      .def(
-          "external_uplift",
-          &trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
-              template external_uplift<py::array_t<double, 1> &>)
-      .def(
-          "init_TSP_module",
-          &trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
-              template init_TSP_module<py::array_t<double, 1> &>)
-      .def(
-          "update_TSP_source",
-          &trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
-              template update_TSP_source<py::array_t<double, 1> &>)
-      .def(
-          "sample_carrot_TSP",
-          &trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
-              template sample_carrot_TSP<py::array_t<double, 1>>)
-      .def(
-          "sample_carrot_Ch_MTSI",
-          &trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
-              template sample_carrot_Ch_MTSI<py::array_t<double, 1>>)
-      .def(
-          "get_transect_Ch_MTSI",
-          &trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
-              template get_transect_Ch_MTSI<py::array_t<double, 1>>)
-      .def(
-          "get_transect_TSP",
-          &trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
-              template get_transect_TSP<py::array_t<double, 1>>)
-      .def("set_dt", &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                                 CONNECTOR_T>::set_dt)
-      .def("set_transfer_rate_Qs_hs2fl",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::set_transfer_rate_Qs_hs2fl)
-      .def("set_single_Ks",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::set_single_Ks)
-      .def("set_single_Kr",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::set_single_Kr)
-      .def("set_single_Ke",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::set_single_Ke)
-      .def("set_single_Kle",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::set_single_Kle)
-      .def("set_single_Kld",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::set_single_Kld)
-      .def("set_single_depcoeff",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::set_single_depcoeff)
-      .def("set_single_precipitations",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::set_single_precipitations)
-      .def("set_single_kappa_s",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::set_single_kappa_s)
-      .def("set_single_kappa_r",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::set_single_kappa_r)
-      .def("set_single_Sc",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::set_single_Sc)
-      .def("set_single_Sc_M",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::set_single_Sc_M)
-      .def("set_single_lambda",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::set_single_lambda)
-      .def("set_single_sea_level",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::set_single_sea_level)
-      .def("set_single_internal_friction",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::set_single_internal_friction)
-      .def("set_single_tls",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::set_single_tls)
-      .def("set_hillslopes_mode",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::set_hillslopes_mode)
-      .def("set_fluvial_mode",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::set_fluvial_mode)
-      .def("set_secondary_fluvial_mode",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::set_secondary_fluvial_mode)
-      .def("set_flowtopo_mode",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::set_flowtopo_mode)
-      .def("set_marine_mode",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::set_marine_mode)
-      .def("fill_up", &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                                  CONNECTOR_T>::fill_up)
-      .def("init_Ch_MTSI",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::init_Ch_MTSI)
-      .def("rise_boundary_by",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::rise_boundary_by)
-      .def(
-          "get_TSP_surface_concentrations",
-          &trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
-              template get_TSP_surface_concentrations<py::array>)
-      .def(
-          "get_Ch_MTIS_surface_age",
-          &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                      CONNECTOR_T>::template get_Ch_MTIS_surface_age<py::array>)
-      .def(
-          "set_variable_precipitations",
-          &trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
-              template set_variable_precipitations<py::array_t<double, 1> &>)
-      .def(
-          "set_variable_Kr",
-          &trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
-              template set_variable_Kr<py::array_t<double, 1> &>)
-      .def(
-          "set_variable_Ks",
-          &trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
-              template set_variable_Ks<py::array_t<double, 1> &>)
-      .def(
-          "set_variable_depcoeff",
-          &trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
-              template set_variable_depcoeff<py::array_t<double, 1> &>)
-      .def(
-          "set_variable_kappa_s",
-          &trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
-              template set_variable_kappa_s<py::array_t<double, 1> &>)
-      .def(
-          "set_variable_kappa_r",
-          &trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
-              template set_variable_kappa_r<py::array_t<double, 1> &>)
-      .def(
-          "set_variable_Sc",
-          &trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
-              template set_variable_Sc<py::array_t<double, 1> &>)
-      .def(
-          "set_variable_Sc_M",
-          &trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
-              template set_variable_Sc_M<py::array_t<double, 1> &>)
-      .def(
-          "set_variable_Ke",
-          &trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
-              template set_variable_Ke<py::array_t<double, 1> &>)
-      .def(
-          "set_variable_lambda",
-          &trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
-              template set_variable_lambda<py::array_t<double, 1> &>)
-      .def(
-          "set_variable_sea_level",
-          &trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
-              template set_variable_sea_level<py::array_t<double, 1> &>)
-      .def(
-          "feed_topo",
-          &trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
-              template feed_topo<py::array_t<double, 1> &>)
-      .def(
-          "set_extra_Qs_fluvial",
-          &trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
-              template set_extra_Qs_fluvial<py::array_t<int, 1> &,
-                                            py::array_t<double, 1> &>)
-      .def(
-          "set_extra_Qw_fluvial",
-          &trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
-              template set_extra_Qw_fluvial<py::array_t<int, 1> &,
-                                            py::array_t<double, 1> &>)
-      .def("disable_Qs_fluvial",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::disable_Qs_fluvial)
-      .def("disable_Qw_fluvial",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::disable_Qw_fluvial)
-
-      .def("set_m", &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                                CONNECTOR_T>::set_m)
-      .def("set_n", &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                                CONNECTOR_T>::set_n)
-      .def("set_N_boundary_to",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::set_N_boundary_to)
-
-      .def("run_SFD_implicit",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::run_SFD_implicit)
-      .def("lithify", &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                                  CONNECTOR_T>::lithify)
-      .def("strip_sediment",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::strip_sediment)
-
-      // SEt of standalone functions
-      .def("Standalone_hyland_landslides",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::Standalone_hyland_landslides)
-      .def("Standalone_hylands_single_landslide",
-           &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
-                       CONNECTOR_T>::Standalone_hylands_single_landslide)
+	py::class_<
+		trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>>(
+		m, typestr.c_str())
+		.def(py::init<>())
+		.def_readwrite("graph",
+					 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+								 CONNECTOR_T>::graph)
+		.def_readwrite("connector",
+					 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+								 CONNECTOR_T>::connector)
+		.def("init_random",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::init_random)
+		.def("init_perlin",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::init_perlin)
+		.def("get_topo", &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+									 CONNECTOR_T>::template get_topo<py::array>)
+		.def("get_hillshade",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::template get_hillshade<py::array>)
+		.def("get_h_sed", &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+									CONNECTOR_T>::template get_h_sed<py::array>)
+		.def("get_Qw", &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+								 CONNECTOR_T>::template get_Qw<py::array>)
+		.def("get_Qs_fluvial",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::template get_Qs_fluvial<py::array>)
+		.def("get_Qs_hillslopes",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::template get_Qs_hillslopes<py::array>)
+		.def("get_precipitations",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::template get_precipitations<py::array>)
+		.def("set_full_stochastic",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::set_full_stochastic)
+		.def("run", &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+								CONNECTOR_T>::run)
+		.def("run_SFD", &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+									CONNECTOR_T>::run_SFD)
+		.def("block_uplift",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::block_uplift)
+		.def(
+			"external_uplift",
+			&trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
+				template external_uplift<py::array_t<double, 1> &>)
+		.def(
+			"init_TSP_module",
+			&trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
+				template init_TSP_module<py::array_t<double, 1> &>)
+		.def(
+			"update_TSP_source",
+			&trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
+				template update_TSP_source<py::array_t<double, 1> &>)
+		.def(
+			"sample_carrot_TSP",
+			&trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
+				template sample_carrot_TSP<py::array_t<double, 1>>)
+		.def(
+			"sample_carrot_Ch_MTSI",
+			&trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
+				template sample_carrot_Ch_MTSI<py::array_t<double, 1>>)
+		.def(
+			"get_transect_Ch_MTSI",
+			&trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
+				template get_transect_Ch_MTSI<py::array_t<double, 1>>)
+		.def(
+			"get_transect_TSP",
+			&trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
+				template get_transect_TSP<py::array_t<double, 1>>)
+		.def("set_dt", &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+								 CONNECTOR_T>::set_dt)
+		.def("set_transfer_rate_Qs_hs2fl",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::set_transfer_rate_Qs_hs2fl)
+		.def("set_single_Ks",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::set_single_Ks)
+		.def("set_single_Kr",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::set_single_Kr)
+		.def("set_single_Ke",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::set_single_Ke)
+		.def("set_single_Kle",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::set_single_Kle)
+		.def("set_single_Kld",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::set_single_Kld)
+		.def("set_single_depcoeff",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::set_single_depcoeff)
+		.def("set_single_precipitations",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::set_single_precipitations)
+		.def("set_single_kappa_s",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::set_single_kappa_s)
+		.def("set_single_kappa_r",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::set_single_kappa_r)
+		.def("set_single_Sc",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::set_single_Sc)
+		.def("set_single_Sc_M",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::set_single_Sc_M)
+		.def("set_single_lambda",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::set_single_lambda)
+		.def("set_single_sea_level",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::set_single_sea_level)
+		.def("set_single_internal_friction",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::set_single_internal_friction)
+		.def("set_single_tls",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::set_single_tls)
+		.def("set_hillslopes_mode",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::set_hillslopes_mode)
+		.def("set_fluvial_mode",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::set_fluvial_mode)
+		.def("set_secondary_fluvial_mode",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::set_secondary_fluvial_mode)
+		.def("set_flowtopo_mode",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::set_flowtopo_mode)
+		.def("set_marine_mode",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::set_marine_mode)
+		.def("fill_up", &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+									CONNECTOR_T>::fill_up)
+		.def("init_Ch_MTSI",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::init_Ch_MTSI)
+		.def("rise_boundary_by",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::rise_boundary_by)
+		.def(
+			"get_TSP_surface_concentrations",
+			&trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
+				template get_TSP_surface_concentrations<py::array>)
+		.def(
+			"get_Ch_MTIS_surface_age",
+			&trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						CONNECTOR_T>::template get_Ch_MTIS_surface_age<py::array>)
+		.def(
+			"set_variable_precipitations",
+			&trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
+				template set_variable_precipitations<py::array_t<double, 1> &>)
+		.def(
+			"set_variable_Kr",
+			&trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
+				template set_variable_Kr<py::array_t<double, 1> &>)
+		.def(
+			"set_variable_Ks",
+			&trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
+				template set_variable_Ks<py::array_t<double, 1> &>)
+		.def(
+			"set_variable_depcoeff",
+			&trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
+				template set_variable_depcoeff<py::array_t<double, 1> &>)
+		.def(
+			"set_variable_kappa_s",
+			&trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
+				template set_variable_kappa_s<py::array_t<double, 1> &>)
+		.def(
+			"set_variable_kappa_r",
+			&trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
+				template set_variable_kappa_r<py::array_t<double, 1> &>)
+		.def(
+			"set_variable_Sc",
+			&trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
+				template set_variable_Sc<py::array_t<double, 1> &>)
+		.def(
+			"set_variable_Sc_M",
+			&trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
+				template set_variable_Sc_M<py::array_t<double, 1> &>)
+		.def(
+			"set_variable_Ke",
+			&trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
+				template set_variable_Ke<py::array_t<double, 1> &>)
+		.def(
+			"set_variable_lambda",
+			&trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
+				template set_variable_lambda<py::array_t<double, 1> &>)
+		.def(
+			"set_variable_sea_level",
+			&trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
+				template set_variable_sea_level<py::array_t<double, 1> &>)
+		.def(
+			"feed_topo",
+			&trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
+				template feed_topo<py::array_t<double, 1> &>)
+		.def(
+			"set_extra_Qs_fluvial",
+			&trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
+				template set_extra_Qs_fluvial<py::array_t<int, 1> &,
+											py::array_t<double, 1> &>)
+		.def(
+			"set_extra_Qw_fluvial",
+			&trackscape<double, DAGGER::graph<double, CONNECTOR_T>, CONNECTOR_T>::
+				template set_extra_Qw_fluvial<py::array_t<int, 1> &,
+											py::array_t<double, 1> &>)
+		.def("disable_Qs_fluvial",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::disable_Qs_fluvial)
+		.def("disable_Qw_fluvial",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::disable_Qw_fluvial)
+
+		.def("set_m", &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+								CONNECTOR_T>::set_m)
+		.def("set_n", &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+								CONNECTOR_T>::set_n)
+		.def("set_N_boundary_to",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::set_N_boundary_to)
+
+		.def("run_SFD_implicit",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::run_SFD_implicit)
+		.def("lithify", &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+									CONNECTOR_T>::lithify)
+		.def("strip_sediment",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::strip_sediment)
+
+		// SEt of standalone functions
+		.def("Standalone_hyland_landslides",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::Standalone_hyland_landslides)
+		.def("Standalone_hylands_single_landslide",
+			 &trackscape<double, DAGGER::graph<double, CONNECTOR_T>,
+						 CONNECTOR_T>::Standalone_hylands_single_landslide)
 
-      ;
+		;
 }
 
 // template<typename CONNECTOR_T>
 // void declare_ff(py::module &m, std::string typestr)
 // {
 //   py::class_<fastflood<double, DAGGER::graph<double, CONNECTOR_T>,
 //   CONNECTOR_T,  DAGGER::numvec<double> > >(m, typestr.c_str())
@@ -1102,385 +1102,385 @@
 // #endif
 
 //   ;
 // }
 
 template <typename fT, typename GRAPH_T, typename CONNECTOR_T>
 void declare_graphflood(py::module &m, std::string typestr) {
-  py::class_<graphflood<fT, GRAPH_T, CONNECTOR_T>>(m, typestr.c_str())
-      .def(py::init<GRAPH_T &, CONNECTOR_T &>())
-      .def(
-          "run", &graphflood<fT, GRAPH_T, CONNECTOR_T>::run,
-          R"pdoc(Main function running the model from all the input params)pdoc")
-      .def(
-          "set_topo",
-          &graphflood<fT, GRAPH_T,
-                      CONNECTOR_T>::template set_topo<py::array_t<double, 1>>,
-          R"pdoc(Main function running the model from all the input params)pdoc")
-      .def(
-          "set_hw",
-          &graphflood<fT, GRAPH_T,
-                      CONNECTOR_T>::template set_hw<py::array_t<double, 1>>,
-          R"pdoc(Main function running the model from all the input params)pdoc")
-
-      .def(
-          "get_hw",
-          &graphflood<fT, GRAPH_T,
-                      CONNECTOR_T>::template get_hw<py::array_t<double, 1>>,
-          R"pdoc(Main function running the model from all the input params)pdoc")
-      .def(
-          "get_surface_topo",
-          &graphflood<fT, GRAPH_T, CONNECTOR_T>::template get_surface_topo<
-              py::array_t<double, 1>>,
-          R"pdoc(Main function running the model from all the input params)pdoc")
-      .def(
-          "get_bedrock_topo",
-          &graphflood<fT, GRAPH_T, CONNECTOR_T>::template get_bedrock_topo<
-              py::array_t<double, 1>>,
-          R"pdoc(Main function running the model from all the input params)pdoc")
-      .def(
-          "get_Qwin",
-          &graphflood<fT, GRAPH_T,
-                      CONNECTOR_T>::template get_Qwin<py::array_t<double, 1>>,
-          R"pdoc(Main function running the model from all the input params)pdoc")
-      .def(
-          "get_SSTACKDEBUG",
-          &graphflood<fT, GRAPH_T, CONNECTOR_T>::template get_SSTACKDEBUG<
-              py::array_t<size_t, 1>>,
-          R"pdoc(Main function running the model from all the input params)pdoc")
-
-      .def(
-          "enable_MFD", &graphflood<fT, GRAPH_T, CONNECTOR_T>::enable_MFD,
-          R"pdoc(Main function running the model from all the input params)pdoc")
-      .def(
-          "enable_SFD", &graphflood<fT, GRAPH_T, CONNECTOR_T>::enable_SFD,
-          R"pdoc(Main function running the model from all the input params)pdoc")
-      .def("set_dt_hydro", &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_dt_hydro)
-      .def("fill_minima", &graphflood<fT, GRAPH_T, CONNECTOR_T>::fill_minima)
-      .def("reroute_minima",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::reroute_minima)
-      .def("ignore_minima",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::ignore_minima)
-      .def("enable_morpho",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::enable_morpho)
-      .def("disable_morpho",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::disable_morpho)
-      .def("set_dt_morpho_multiplier",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_dt_morpho_multiplier)
-
-      .def("set_dt_morpho",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_dt_morpho)
-      .def("set_single_aexp",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_single_aexp)
-      .def("set_single_ke",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_single_ke)
-      .def("set_single_ke_lateral",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_single_ke_lateral)
-      .def("set_single_kd",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_single_kd)
-      .def("set_single_kd_lateral",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_single_kd_lateral)
-      .def("set_single_tau_c",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_single_kd_lateral)
-      .def("set_variable_ke",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::template set_variable_ke<
-               py::array_t<double, 1>>)
-      .def("set_mannings", &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_mannings)
-
-      .def("init_convergence_checker",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::init_convergence_checker)
-      .def("get_conv_nodes",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::template get_conv_nodes<
-               py::array_t<int, 1>>)
-      .def("get_conv_ini_Qw",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::template get_conv_ini_Qw<
-               py::array_t<double, 1>>)
-      .def("get_conv_mean_Qr",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::template get_conv_mean_Qr<
-               py::array_t<double, 1>>)
-      .def("get_conv_mean_dhw",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::template get_conv_mean_dhw<
-               py::array_t<double, 1>>)
-
-      .def("compute_tuqQ",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::template compute_tuqQ<
-               py::array_t<double, 1>>)
-      .def("compute_elemental_transfer",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::
-               template compute_elemental_transfer<py::array_t<double, 1>,
-                                                   py::array_t<double, 1>>)
-
-      .def("set_water_input_by_entry_points",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::
-               template set_water_input_by_entry_points<py::array_t<double, 1>,
-                                                        py::array_t<int, 1>>)
-      .def("set_water_input_by_constant_precipitation_rate",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::
-               set_water_input_by_constant_precipitation_rate)
-      .def("set_water_input_by_variable_precipitation_rate",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::
-               template set_water_input_by_variable_precipitation_rate<
-                   py::array_t<double, 1>>)
-
-      .def("set_sed_input_by_entry_points",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::
-               template set_sed_input_by_entry_points<py::array_t<double, 1>,
-                                                      py::array_t<int, 1>>)
-
-      .def("enable_Qwout_recording",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::enable_Qwout_recording)
-      .def("disable_Qwout_recording",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::disable_Qwout_recording)
-      .def("get_Qwout_recording",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::template get_Qwout_recording<
-               py::array_t<double, 1>>)
-
-      .def("enable_Sw_recording",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::enable_Sw_recording)
-      .def("disable_Sw_recording",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::disable_Sw_recording)
-      .def("get_Sw_recording",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::template get_Sw_recording<
-               py::array_t<double, 1>>)
-
-      .def("enable_dhw_recording",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::enable_dhw_recording)
-      .def("disable_dhw_recording",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::disable_dhw_recording)
-      .def("get_dhw_recording",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::template get_dhw_recording<
-               py::array_t<double, 1>>)
-
-      .def("enable_filling_recording",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::enable_filling_recording)
-      .def("disable_filling_recording",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::disable_filling_recording)
-      .def(
-          "get_filling_recording",
-          &graphflood<fT, GRAPH_T, CONNECTOR_T>::template get_filling_recording<
-              py::array_t<double, 1>>)
-
-      .def("enable_edot_recording",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::enable_edot_recording)
-      .def("disable_edot_recording",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::disable_edot_recording)
-      .def("get_edot_recording",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::template get_edot_recording<
-               py::array_t<double, 1>>)
-
-      .def("enable_flowvec_recording",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::enable_flowvec_recording)
-      .def("disable_flowvec_recording",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::disable_flowvec_recording)
-      .def(
-          "get_flowvec_recording",
-          &graphflood<fT, GRAPH_T, CONNECTOR_T>::template get_flowvec_recording<
-              py::array_t<double, 1>>)
-
-      .def("get_tot_Qw_input",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::get_tot_Qw_input)
-      .def("get_tot_Qw_output",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::get_tot_Qw_output)
-      .def("get_tot_Qwin_output",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::get_tot_Qwin_output)
-      .def("get_tot_Qs_output",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::get_tot_Qs_output)
-
-      .def("set_stochaslope",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_stochaslope)
-      .def("disable_stochaslope",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::disable_stochaslope)
-      .def("set_fixed_hw_at_boundaries",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_fixed_hw_at_boundaries)
-      .def("set_fixed_slope_at_boundaries",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_fixed_slope_at_boundaries)
-      .def("get_dt_hydro", &graphflood<fT, GRAPH_T, CONNECTOR_T>::get_dt_hydro)
-
-      .def("set_partition_method",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_partition_method)
-      .def("set_topological_number",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_topological_number)
-      .def("get_topological_number",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::get_topological_number)
-
-      .def("get_courant_dt_hydro",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::get_courant_dt_hydro)
-      .def("set_courant_number",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_courant_number)
-      .def("set_max_courant_dt_hydro",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_max_courant_dt_hydro)
-      .def("set_min_courant_dt_hydro",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_min_courant_dt_hydro)
-      .def("enable_courant_dt_hydro",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::enable_courant_dt_hydro)
-      .def("disable_courant_dt_hydro",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::disable_courant_dt_hydro)
-      .def("set_Qwin_crit",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_Qwin_crit)
-      .def("get_nT", &graphflood<fT, GRAPH_T, CONNECTOR_T>::get_nT)
-
-      .def("enable_hydrostationary",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::enable_hydrostationary)
-      .def("disable_hydrostationary",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::disable_hydrostationary)
-
-      .def("block_uplift", &graphflood<fT, GRAPH_T, CONNECTOR_T>::block_uplift)
-      .def("variable_uplift",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::template variable_uplift<
-               py::array_t<double, 1>>)
-
-      .def("run_precipitions",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::run_precipitions)
-      .def("run_precipitions_exp",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::run_precipitions_exp)
-      .def("run_graphipiton",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::run_graphipiton)
-      .def("run_exp", &graphflood<fT, GRAPH_T, CONNECTOR_T>::run_exp)
-      .def("run_hydro_only",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::run_hydro_only)
+	py::class_<graphflood<fT, GRAPH_T, CONNECTOR_T>>(m, typestr.c_str())
+		.def(py::init<GRAPH_T &, CONNECTOR_T &>())
+		.def(
+			"run", &graphflood<fT, GRAPH_T, CONNECTOR_T>::run,
+			R"pdoc(Main function running the model from all the input params)pdoc")
+		.def(
+			"set_topo",
+			&graphflood<fT, GRAPH_T,
+						CONNECTOR_T>::template set_topo<py::array_t<double, 1>>,
+			R"pdoc(Main function running the model from all the input params)pdoc")
+		.def(
+			"set_hw",
+			&graphflood<fT, GRAPH_T,
+						CONNECTOR_T>::template set_hw<py::array_t<double, 1>>,
+			R"pdoc(Main function running the model from all the input params)pdoc")
+
+		.def(
+			"get_hw",
+			&graphflood<fT, GRAPH_T,
+						CONNECTOR_T>::template get_hw<py::array_t<double, 1>>,
+			R"pdoc(Main function running the model from all the input params)pdoc")
+		.def(
+			"get_surface_topo",
+			&graphflood<fT, GRAPH_T, CONNECTOR_T>::template get_surface_topo<
+				py::array_t<double, 1>>,
+			R"pdoc(Main function running the model from all the input params)pdoc")
+		.def(
+			"get_bedrock_topo",
+			&graphflood<fT, GRAPH_T, CONNECTOR_T>::template get_bedrock_topo<
+				py::array_t<double, 1>>,
+			R"pdoc(Main function running the model from all the input params)pdoc")
+		.def(
+			"get_Qwin",
+			&graphflood<fT, GRAPH_T,
+						CONNECTOR_T>::template get_Qwin<py::array_t<double, 1>>,
+			R"pdoc(Main function running the model from all the input params)pdoc")
+		.def(
+			"get_SSTACKDEBUG",
+			&graphflood<fT, GRAPH_T, CONNECTOR_T>::template get_SSTACKDEBUG<
+				py::array_t<size_t, 1>>,
+			R"pdoc(Main function running the model from all the input params)pdoc")
+
+		.def(
+			"enable_MFD", &graphflood<fT, GRAPH_T, CONNECTOR_T>::enable_MFD,
+			R"pdoc(Main function running the model from all the input params)pdoc")
+		.def(
+			"enable_SFD", &graphflood<fT, GRAPH_T, CONNECTOR_T>::enable_SFD,
+			R"pdoc(Main function running the model from all the input params)pdoc")
+		.def("set_dt_hydro", &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_dt_hydro)
+		.def("fill_minima", &graphflood<fT, GRAPH_T, CONNECTOR_T>::fill_minima)
+		.def("reroute_minima",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::reroute_minima)
+		.def("ignore_minima",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::ignore_minima)
+		.def("enable_morpho",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::enable_morpho)
+		.def("disable_morpho",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::disable_morpho)
+		.def("set_dt_morpho_multiplier",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_dt_morpho_multiplier)
+
+		.def("set_dt_morpho",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_dt_morpho)
+		.def("set_single_aexp",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_single_aexp)
+		.def("set_single_ke",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_single_ke)
+		.def("set_single_ke_lateral",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_single_ke_lateral)
+		.def("set_single_kd",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_single_kd)
+		.def("set_single_kd_lateral",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_single_kd_lateral)
+		.def("set_single_tau_c",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_single_kd_lateral)
+		.def("set_variable_ke",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::template set_variable_ke<
+				 py::array_t<double, 1>>)
+		.def("set_mannings", &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_mannings)
+
+		.def("init_convergence_checker",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::init_convergence_checker)
+		.def("get_conv_nodes",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::template get_conv_nodes<
+				 py::array_t<int, 1>>)
+		.def("get_conv_ini_Qw",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::template get_conv_ini_Qw<
+				 py::array_t<double, 1>>)
+		.def("get_conv_mean_Qr",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::template get_conv_mean_Qr<
+				 py::array_t<double, 1>>)
+		.def("get_conv_mean_dhw",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::template get_conv_mean_dhw<
+				 py::array_t<double, 1>>)
+
+		.def("compute_tuqQ",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::template compute_tuqQ<
+				 py::array_t<double, 1>>)
+		.def("compute_elemental_transfer",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::
+				 template compute_elemental_transfer<py::array_t<double, 1>,
+													 py::array_t<double, 1>>)
+
+		.def("set_water_input_by_entry_points",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::
+				 template set_water_input_by_entry_points<py::array_t<double, 1>,
+														py::array_t<int, 1>>)
+		.def("set_water_input_by_constant_precipitation_rate",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::
+				 set_water_input_by_constant_precipitation_rate)
+		.def("set_water_input_by_variable_precipitation_rate",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::
+				 template set_water_input_by_variable_precipitation_rate<
+					 py::array_t<double, 1>>)
+
+		.def("set_sed_input_by_entry_points",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::
+				 template set_sed_input_by_entry_points<py::array_t<double, 1>,
+														py::array_t<int, 1>>)
+
+		.def("enable_Qwout_recording",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::enable_Qwout_recording)
+		.def("disable_Qwout_recording",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::disable_Qwout_recording)
+		.def("get_Qwout_recording",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::template get_Qwout_recording<
+				 py::array_t<double, 1>>)
+
+		.def("enable_Sw_recording",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::enable_Sw_recording)
+		.def("disable_Sw_recording",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::disable_Sw_recording)
+		.def("get_Sw_recording",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::template get_Sw_recording<
+				 py::array_t<double, 1>>)
+
+		.def("enable_dhw_recording",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::enable_dhw_recording)
+		.def("disable_dhw_recording",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::disable_dhw_recording)
+		.def("get_dhw_recording",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::template get_dhw_recording<
+				 py::array_t<double, 1>>)
+
+		.def("enable_filling_recording",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::enable_filling_recording)
+		.def("disable_filling_recording",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::disable_filling_recording)
+		.def(
+			"get_filling_recording",
+			&graphflood<fT, GRAPH_T, CONNECTOR_T>::template get_filling_recording<
+				py::array_t<double, 1>>)
+
+		.def("enable_edot_recording",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::enable_edot_recording)
+		.def("disable_edot_recording",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::disable_edot_recording)
+		.def("get_edot_recording",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::template get_edot_recording<
+				 py::array_t<double, 1>>)
+
+		.def("enable_flowvec_recording",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::enable_flowvec_recording)
+		.def("disable_flowvec_recording",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::disable_flowvec_recording)
+		.def(
+			"get_flowvec_recording",
+			&graphflood<fT, GRAPH_T, CONNECTOR_T>::template get_flowvec_recording<
+				py::array_t<double, 1>>)
+
+		.def("get_tot_Qw_input",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::get_tot_Qw_input)
+		.def("get_tot_Qw_output",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::get_tot_Qw_output)
+		.def("get_tot_Qwin_output",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::get_tot_Qwin_output)
+		.def("get_tot_Qs_output",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::get_tot_Qs_output)
+
+		.def("set_stochaslope",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_stochaslope)
+		.def("disable_stochaslope",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::disable_stochaslope)
+		.def("set_fixed_hw_at_boundaries",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_fixed_hw_at_boundaries)
+		.def("set_fixed_slope_at_boundaries",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_fixed_slope_at_boundaries)
+		.def("get_dt_hydro", &graphflood<fT, GRAPH_T, CONNECTOR_T>::get_dt_hydro)
+
+		.def("set_partition_method",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_partition_method)
+		.def("set_topological_number",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_topological_number)
+		.def("get_topological_number",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::get_topological_number)
+
+		.def("get_courant_dt_hydro",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::get_courant_dt_hydro)
+		.def("set_courant_number",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_courant_number)
+		.def("set_max_courant_dt_hydro",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_max_courant_dt_hydro)
+		.def("set_min_courant_dt_hydro",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_min_courant_dt_hydro)
+		.def("enable_courant_dt_hydro",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::enable_courant_dt_hydro)
+		.def("disable_courant_dt_hydro",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::disable_courant_dt_hydro)
+		.def("set_Qwin_crit",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::set_Qwin_crit)
+		.def("get_nT", &graphflood<fT, GRAPH_T, CONNECTOR_T>::get_nT)
+
+		.def("enable_hydrostationary",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::enable_hydrostationary)
+		.def("disable_hydrostationary",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::disable_hydrostationary)
+
+		.def("block_uplift", &graphflood<fT, GRAPH_T, CONNECTOR_T>::block_uplift)
+		.def("variable_uplift",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::template variable_uplift<
+				 py::array_t<double, 1>>)
+
+		.def("run_precipitions",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::run_precipitions)
+		.def("run_precipitions_exp",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::run_precipitions_exp)
+		.def("run_graphipiton",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::run_graphipiton)
+		.def("run_exp", &graphflood<fT, GRAPH_T, CONNECTOR_T>::run_exp)
+		.def("run_hydro_only",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::run_hydro_only)
 
-      .def("define_precipitations_Ath",
-           &graphflood<fT, GRAPH_T, CONNECTOR_T>::define_precipitations_Ath)
+		.def("define_precipitations_Ath",
+			 &graphflood<fT, GRAPH_T, CONNECTOR_T>::define_precipitations_Ath)
 
-      ;
+		;
 }
 
 PYBIND11_MODULE(dagger, m) {
-  m.doc() = R"pbdoc(
-      DAGGER - python API
-      ===================
-
-      Quick API
-      ---------
-
-      .. autosummary::
-
-          graph
-          graph.init_graph
-          graph.set_opt_stst_rerouting
-          graph.compute_graph
-          graph.is_Sstack_full
-          graph.activate_opti_sparse_border_cordonnier
-          graph.get_all_nodes_upstream_of
-          graph.get_all_nodes_downstream_of
-          graph.get_SFD_stack
-          graph.get_MFD_stack
-          graph.accumulate_constant_downstream_SFD
-          graph.accumulate_variable_downstream_SFD
-          graph.accumulate_constant_downstream_MFD
-          graph.accumulate_variable_downstream_MFD
-          graph.set_LMR_method
-          graph.set_minimum_slope_for_LMR
-          graph.set_slope_randomness_for_LMR
-          graph.get_SFD_distance_from_outlets
-          graph.get_SFD_min_distance_from_sources
-          graph.get_SFD_max_distance_from_sources
-          graph.get_MFD_max_distance_from_sources
-          graph.get_MFD_min_distance_from_sources
-          graph.get_MFD_max_distance_from_outlets
-          graph.get_MFD_min_distance_from_outlets
-          graph.get_SFD_basin_labels
-
-          D8N
-          D8N.__init__
-          D8N.set_default_boundaries
-          D8N.set_custom_boundaries
-          D8N.print_dim
-          D8N.get_HS
-          D8N.get_mask_array
-          D8N.set_values_at_boundaries
-          D8N.set_out_boundaries_to_permissive
-          D8N.get_boundary_at_node
-          D8N.get_rowcol_Sreceivers
-          D8N.print_receivers
-          D8N.get_rec_array_size
-          D8N.update_links_MFD_only
-          D8N.update_links
-          D8N.update_links_from_topo
-          D8N.sum_at_outlets
-          D8N.keep_only_at_outlets
-          D8N.get_SFD_receivers
-          D8N.get_SFD_dx
-          D8N.get_SFD_ndonors
-          D8N.get_SFD_donors_flat
-          D8N.get_SFD_donors_list
-          D8N.get_links
-          D8N.get_linknodes_flat
-          D8N.get_linknodes_list
-          D8N.get_linknodes_list_oriented
-          D8N.get_SFD_receivers_at_node
-          D8N.get_SFD_dx_at_node
-          D8N.get_SFD_ndonors_at_node
-          D8N.get_SFD_donors_at_node
-          D8N.get_SFD_gradient
-          D8N.get_links_gradient
-          D8N.get_MFD_mean_gradient
-          D8N.get_MFD_weighted_gradient
-          D8N.get_link_weights
-          D8N.set_stochaticiy_for_SFD
-
-
-      Full API
-      ---------
-
-      .. autoclass:: D8N
-        :members:
-
-      .. autoclass:: graph
-        :members:
-
-
-  )pbdoc";
-
-  py::enum_<DEPRES>(m, "LMR")
-      .value("cordonnier_fill", DEPRES::cordonnier_fill)
-      .value("cordonnier_carve", DEPRES::cordonnier_carve)
-      .value("cordonnier_simple", DEPRES::cordonnier_simple)
-      .value("priority_flood", DEPRES::priority_flood)
-      .value("priority_flood_opti", DEPRES::priority_flood_opti)
-      .value("priority_full_MFD", DEPRES::priority_full_MFD)
-
-      .value("none", DEPRES::none)
-      .value("dagger_carve", DEPRES::dagger_carve)
-      .value("dagger_fill", DEPRES::dagger_fill);
-
-  py::enum_<MFD_PARTITIONNING>(m, "MFD_PARTITIONNING")
-      .value("PROPOSLOPE", MFD_PARTITIONNING::PROPOSLOPE)
-      .value("SQRTSLOPE", MFD_PARTITIONNING::SQRTSLOPE)
-      .value("PROPOREC", MFD_PARTITIONNING::PROPOREC);
-
-  py::enum_<TSC_HILLSLOPE>(m, "TSC_HILLSLOPE")
-      .value("NONE", TSC_HILLSLOPE::NONE)
-      .value("LINEAR", TSC_HILLSLOPE::LINEAR)
-      .value("CIDRE", TSC_HILLSLOPE::CIDRE)
-      .value("CIDRE_NOCRIT", TSC_HILLSLOPE::CIDRE_NOCRIT)
-      .value("HYLANDS", TSC_HILLSLOPE::HYLANDS);
-
-  py::enum_<TSC_FLUVIAL>(m, "TSC_FLUVIAL")
-      .value("NONE", TSC_FLUVIAL::NONE)
-      .value("DAVY2009", TSC_FLUVIAL::DAVY2009)
-      .value("LATERALDAVY", TSC_FLUVIAL::LATERALDAVY)
-      .value("LATERALSPL", TSC_FLUVIAL::LATERALSPL)
-      .value("FASTSCAPE", TSC_FLUVIAL::FASTSCAPE);
-
-  py::enum_<TSC_MARINE>(m, "TSC_MARINE")
-      .value("NONE", TSC_MARINE::NONE)
-      .value("CHARLIE", TSC_MARINE::CHARLIE);
-
-  py::enum_<TSC_FLOW_TOPOLOGY>(m, "TSC_FLOW_TOPOLOGY")
-      .value("SFD", TSC_FLOW_TOPOLOGY::SFD)
-      .value("MFD", TSC_FLOW_TOPOLOGY::MFD);
-
-  py::enum_<CONVERGENCE>(m, "GRAPHFLOOD_CONVERGENCE")
-      .value("NONE", CONVERGENCE::NONE)
-      .value("DHW", CONVERGENCE::DHW)
-      .value("QWR", CONVERGENCE::QWR)
-      .value("ALL", CONVERGENCE::ALL);
+	m.doc() = R"pbdoc(
+		DAGGER - python API
+		===================
+
+		Quick API
+		---------
+
+		.. autosummary::
+
+			graph
+			graph.init_graph
+			graph.set_opt_stst_rerouting
+			graph.compute_graph
+			graph.is_Sstack_full
+			graph.activate_opti_sparse_border_cordonnier
+			graph.get_all_nodes_upstream_of
+			graph.get_all_nodes_downstream_of
+			graph.get_SFD_stack
+			graph.get_MFD_stack
+			graph.accumulate_constant_downstream_SFD
+			graph.accumulate_variable_downstream_SFD
+			graph.accumulate_constant_downstream_MFD
+			graph.accumulate_variable_downstream_MFD
+			graph.set_LMR_method
+			graph.set_minimum_slope_for_LMR
+			graph.set_slope_randomness_for_LMR
+			graph.get_SFD_distance_from_outlets
+			graph.get_SFD_min_distance_from_sources
+			graph.get_SFD_max_distance_from_sources
+			graph.get_MFD_max_distance_from_sources
+			graph.get_MFD_min_distance_from_sources
+			graph.get_MFD_max_distance_from_outlets
+			graph.get_MFD_min_distance_from_outlets
+			graph.get_SFD_basin_labels
+
+			D8N
+			D8N.__init__
+			D8N.set_default_boundaries
+			D8N.set_custom_boundaries
+			D8N.print_dim
+			D8N.get_HS
+			D8N.get_mask_array
+			D8N.set_values_at_boundaries
+			D8N.set_out_boundaries_to_permissive
+			D8N.get_boundary_at_node
+			D8N.get_rowcol_Sreceivers
+			D8N.print_receivers
+			D8N.get_rec_array_size
+			D8N.update_links_MFD_only
+			D8N.update_links
+			D8N.update_links_from_topo
+			D8N.sum_at_outlets
+			D8N.keep_only_at_outlets
+			D8N.get_SFD_receivers
+			D8N.get_SFD_dx
+			D8N.get_SFD_ndonors
+			D8N.get_SFD_donors_flat
+			D8N.get_SFD_donors_list
+			D8N.get_links
+			D8N.get_linknodes_flat
+			D8N.get_linknodes_list
+			D8N.get_linknodes_list_oriented
+			D8N.get_SFD_receivers_at_node
+			D8N.get_SFD_dx_at_node
+			D8N.get_SFD_ndonors_at_node
+			D8N.get_SFD_donors_at_node
+			D8N.get_SFD_gradient
+			D8N.get_links_gradient
+			D8N.get_MFD_mean_gradient
+			D8N.get_MFD_weighted_gradient
+			D8N.get_link_weights
+			D8N.set_stochaticiy_for_SFD
+
+
+		Full API
+		---------
+
+		.. autoclass:: D8N
+		:members:
+
+		.. autoclass:: graph
+		:members:
+
+
+	)pbdoc";
+
+	py::enum_<DEPRES>(m, "LMR")
+		.value("cordonnier_fill", DEPRES::cordonnier_fill)
+		.value("cordonnier_carve", DEPRES::cordonnier_carve)
+		.value("cordonnier_simple", DEPRES::cordonnier_simple)
+		.value("priority_flood", DEPRES::priority_flood)
+		.value("priority_flood_opti", DEPRES::priority_flood_opti)
+		.value("priority_full_MFD", DEPRES::priority_full_MFD)
+
+		.value("none", DEPRES::none)
+		.value("dagger_carve", DEPRES::dagger_carve)
+		.value("dagger_fill", DEPRES::dagger_fill);
+
+	py::enum_<MFD_PARTITIONNING>(m, "MFD_PARTITIONNING")
+		.value("PROPOSLOPE", MFD_PARTITIONNING::PROPOSLOPE)
+		.value("SQRTSLOPE", MFD_PARTITIONNING::SQRTSLOPE)
+		.value("PROPOREC", MFD_PARTITIONNING::PROPOREC);
+
+	py::enum_<TSC_HILLSLOPE>(m, "TSC_HILLSLOPE")
+		.value("NONE", TSC_HILLSLOPE::NONE)
+		.value("LINEAR", TSC_HILLSLOPE::LINEAR)
+		.value("CIDRE", TSC_HILLSLOPE::CIDRE)
+		.value("CIDRE_NOCRIT", TSC_HILLSLOPE::CIDRE_NOCRIT)
+		.value("HYLANDS", TSC_HILLSLOPE::HYLANDS);
+
+	py::enum_<TSC_FLUVIAL>(m, "TSC_FLUVIAL")
+		.value("NONE", TSC_FLUVIAL::NONE)
+		.value("DAVY2009", TSC_FLUVIAL::DAVY2009)
+		.value("LATERALDAVY", TSC_FLUVIAL::LATERALDAVY)
+		.value("LATERALSPL", TSC_FLUVIAL::LATERALSPL)
+		.value("FASTSCAPE", TSC_FLUVIAL::FASTSCAPE);
+
+	py::enum_<TSC_MARINE>(m, "TSC_MARINE")
+		.value("NONE", TSC_MARINE::NONE)
+		.value("CHARLIE", TSC_MARINE::CHARLIE);
+
+	py::enum_<TSC_FLOW_TOPOLOGY>(m, "TSC_FLOW_TOPOLOGY")
+		.value("SFD", TSC_FLOW_TOPOLOGY::SFD)
+		.value("MFD", TSC_FLOW_TOPOLOGY::MFD);
+
+	py::enum_<CONVERGENCE>(m, "GRAPHFLOOD_CONVERGENCE")
+		.value("NONE", CONVERGENCE::NONE)
+		.value("DHW", CONVERGENCE::DHW)
+		.value("QWR", CONVERGENCE::QWR)
+		.value("ALL", CONVERGENCE::ALL);
 
-  py::class_<D8connector<double>>(m, "D8N", R"pbdoc(
+	py::class_<D8connector<double>>(m, "D8N", R"pbdoc(
 D8 regular grid connector D8N
 
 Description:
 ------------
 
 D8N class: the built-in connector for regular grids. D8N regular grids are the most used type of grids, like most global DEMs for example.
 They are defined by a number of rows (ny) and a number of columns (nx) with associated spacing between nodes in both directions (dy,dx).
@@ -1488,32 +1488,32 @@
 Node index is simply a flat index in the row major direction (idx = row_id * nx + col_id) and the link ID for the top-right, right, bottomright and bottom neighbours are respectiveley idx *4, idx*4 +1, idx * 4+2 and idx*4 + 3
 
 The constructor only needs basics geometrical information.
 
 Parameters:
 -----------
 
-    * nx (int): number of nodes in the X direction (columns)
-    * ny (int): number of nodes in the Y direction (rows)
-    * dx (float64): distance between nodes in the x directions
-    * dy (float64): distance between nodes in the y directions
-    * x_min (float64): X coordinates of the bottom left corner
-    * y_min (float64): Y coordinates of the top left corner
+	* nx (int): number of nodes in the X direction (columns)
+	* ny (int): number of nodes in the Y direction (rows)
+	* dx (float64): distance between nodes in the x directions
+	* dy (float64): distance between nodes in the y directions
+	* x_min (float64): X coordinates of the bottom left corner
+	* y_min (float64): Y coordinates of the top left corner
 
 
 Authors:
 --------
 B.G.
 
 )pbdoc")
 
-      .def(py::init<int, int, double, double, double, double>(), py::arg("nx"),
-           py::arg("ny"), py::arg("dx"), py::arg("dy"), py::arg("x_min"),
-           py::arg("x_max"),
-           R"pbdoc(
+		.def(py::init<int, int, double, double, double, double>(), py::arg("nx"),
+			 py::arg("ny"), py::arg("dx"), py::arg("dy"), py::arg("x_min"),
+			 py::arg("x_max"),
+			 R"pbdoc(
 D8 regular grid connector D8N
 
 Description:
 ------------
 
 D8N class: the built-in connector for regular grids. D8N regular grids are the most used type of grids, like most global DEMs for example.
 They are defined by a number of rows (ny) and a number of columns (nx) with associated spacing between nodes in both directions (dy,dx).
@@ -1521,59 +1521,59 @@
 Node index is simply a flat index in the row major direction (idx = row_id * nx + col_id) and the link ID for the top-right, right, bottomright and bottom neighbours are respectiveley idx *4, idx*4 +1, idx * 4+2 and idx*4 + 3
 
 The constructor only needs basics geometrical information.
 
 Parameters:
 -----------
 
-    * nx (int): number of nodes in the X direction (columns)
-    * ny (int): number of nodes in the Y direction (rows)
-    * dx (float64): distance between nodes in the x directions
-    * dy (float64): distance between nodes in the y directions
-    * x_min (float64): X coordinates of the bottom left corner
-    * y_min (float64): Y coordinates of the top left corner
+	* nx (int): number of nodes in the X direction (columns)
+	* ny (int): number of nodes in the Y direction (rows)
+	* dx (float64): distance between nodes in the x directions
+	* dy (float64): distance between nodes in the y directions
+	* x_min (float64): X coordinates of the bottom left corner
+	* y_min (float64): Y coordinates of the top left corner
 
 
 Authors:
 --------
 B.G.
 
 )pbdoc")
-      .def("set_default_boundaries",
-           &D8connector<double>::set_default_boundaries,
-           py::arg("boundary_preset"),
-           R"pbdoc(
+		.def("set_default_boundaries",
+			 &D8connector<double>::set_default_boundaries,
+			 py::arg("boundary_preset"),
+			 R"pbdoc(
 
 Automatically sets the default boundary system based on predefined presets.
 
 Description:
 ------------
 
 Boundary conditions can be tricky to set. Luckily, most use cases needs
 classical opened bounary at the edge of the dem, or periodic (sometimes called
 cyclic) bounaries at EW or NS edges. This functions automate these (i.e. set the
 right boundary codes and recompute the linknode array)
 
 Parameters:
 -----------
 
-    * boundary_preset (str): the preset. Can be "4edges", "periodic_EW" or
-      "periodic_NS"
+	* boundary_preset (str): the preset. Can be "4edges", "periodic_EW" or
+		"periodic_NS"
 
 
 Authors:
 --------
 B.G.
 
 )pbdoc")
 
-      .def("set_custom_boundaries",
-           &D8connector<double>::set_custom_boundaries<py::array_t<int, 1>>,
-           py::arg("boundary_codes"),
-           R"pbdoc(
+		.def("set_custom_boundaries",
+			 &D8connector<double>::set_custom_boundaries<py::array_t<int, 1>>,
+			 py::arg("boundary_codes"),
+			 R"pbdoc(
 
 Manually sets the boundary codes as uint8 1D array (see doc for options).
 
 Description:
 ------------
 
 Function to manually specify boundary conditions, for cases where the classic
@@ -1581,103 +1581,103 @@
 outlets/inlets location or deactivate some nodes. This is a good function to
 automate the ingestion of nodata, isolating a watershed, or defining entry
 points to the landscape.
 
 Parameters:
 -----------
 
-    * boundary_codes (1D Array): the uint8 array of node size containing the
-      boundary codes (see section :ref:`boundary`)
+	* boundary_codes (1D Array): the uint8 array of node size containing the
+		boundary codes (see section :ref:`boundary`)
 
 
 Authors:
 --------
 B.G.
 
 )pbdoc"
 
-           )
-      .def("print_dim", &D8connector<double>::print_dim,
-           R"pdoc(Debugging function)pdoc")
-      .def(
-          "get_HS",
-          &D8connector<double>::get_HS<std::vector<double>, py::array>,
-          R"pdoc(Deprecated, kept for legacy (see hillshade function outside of ``connector``))pdoc")
-      .def("get_mask_array", &D8connector<double>::get_mask_array,
-           R"pdoc(Returns a 1D array of bool where false are nodata)pdoc")
-
-      .def("set_values_at_boundaries",
-           &D8connector<double>::set_values_at_boundaries<
-               py::array_t<double, 1>>,
-           py::arg("array_to_modify"), py::arg("value"),
-           R"pdoc(
+			 )
+		.def("print_dim", &D8connector<double>::print_dim,
+			 R"pdoc(Debugging function)pdoc")
+		.def(
+			"get_HS",
+			&D8connector<double>::get_HS<std::vector<double>, py::array>,
+			R"pdoc(Deprecated, kept for legacy (see hillshade function outside of ``connector``))pdoc")
+		.def("get_mask_array", &D8connector<double>::get_mask_array,
+			 R"pdoc(Returns a 1D array of bool where false are nodata)pdoc")
+
+		.def("set_values_at_boundaries",
+			 &D8connector<double>::set_values_at_boundaries<
+				 py::array_t<double, 1>>,
+			 py::arg("array_to_modify"), py::arg("value"),
+			 R"pdoc(
 Modify an array in place with given value where connector can out flux
 
 Description:
 ------------
 
 Every nodes on the input array where the connector satisfy the coundary condition
 ``can_out`` will be set to a given value. It modify the array in place (i.e.
 does not return anything but modify the input).
 
 Useful to impose boundary condition in LEMs in a versatile way.
 
 Parameters:
 -----------
 
-    * array_to_modify (1D Array): flot64 array to be modified in place
-    * value (float64): value to impose
+	* array_to_modify (1D Array): flot64 array to be modified in place
+	* value (float64): value to impose
 
 
 Authors:
 --------
 B.G.
 
 )pdoc")
 
-      .def("set_out_boundaries_to_permissive",
-           &D8connector<double>::set_out_boundaries_to_permissive,
-           R"pdoc(
+		.def("set_out_boundaries_to_permissive",
+			 &D8connector<double>::set_out_boundaries_to_permissive,
+			 R"pdoc(
 Converts OUT boundaries to CAN_OUT.
 
 Description:
 ------------
 
 Converts OUT boundaries, where flow entering this cell has to out the model to
 CAN_OUT, where flow leaves the model if the cell has no downslope receivers.
 
 Authors:
 --------
 B.G.
 
 )pdoc")
 
-      .def("get_boundary_at_node", &D8connector<double>::get_boundary_at_node,
-           py::arg("node_idx"),
-           R"pdoc(Returns the boundary code at node index)pdoc")
-
-      .def(
-          "get_rowcol_Sreceivers", &D8connector<double>::get_rowcol_Sreceivers,
-          py::arg("row_index"), py::arg("col_index"),
-          R"pdoc(Debug function to get the receiver (node) indices of a node from its row and column index)pdoc")
-
-      .def(
-          "print_receivers",
-          &D8connector<double>::template print_receivers<std::vector<double>>,
-          py::arg("node_index"), py::arg("topography"),
-          R"pdoc(Debuggin function printing to the terminal the receivers of a node index and their topography (post graph computation! so the topographic field may not be the one used for the receivers/LM computations))pdoc")
-
-      .def("get_rec_array_size", &D8connector<double>::get_rec_array_size,
-           R"pdoc(Debug function - ignore)pdoc")
-
-      .def("update_links_MFD_only",
-           &D8connector<double>::template update_links_MFD_only<
-               std::vector<double>>,
-           py::arg("topography"),
-           R"pdoc(
+		.def("get_boundary_at_node", &D8connector<double>::get_boundary_at_node,
+			 py::arg("node_idx"),
+			 R"pdoc(Returns the boundary code at node index)pdoc")
+
+		.def(
+			"get_rowcol_Sreceivers", &D8connector<double>::get_rowcol_Sreceivers,
+			py::arg("row_index"), py::arg("col_index"),
+			R"pdoc(Debug function to get the receiver (node) indices of a node from its row and column index)pdoc")
+
+		.def(
+			"print_receivers",
+			&D8connector<double>::template print_receivers<std::vector<double>>,
+			py::arg("node_index"), py::arg("topography"),
+			R"pdoc(Debuggin function printing to the terminal the receivers of a node index and their topography (post graph computation! so the topographic field may not be the one used for the receivers/LM computations))pdoc")
+
+		.def("get_rec_array_size", &D8connector<double>::get_rec_array_size,
+			 R"pdoc(Debug function - ignore)pdoc")
+
+		.def("update_links_MFD_only",
+			 &D8connector<double>::template update_links_MFD_only<
+				 std::vector<double>>,
+			 py::arg("topography"),
+			 R"pdoc(
 Updates all the link directionalities - but not the SFD receiver/donors.
 
 Description:
 ------------
 
 Updates all the link directionalities based on a given topography. Note that it
 does not process the SFD receiver/donors and is (paradoxally) faster. However,
@@ -1692,19 +1692,19 @@
 
 Authors:
 --------
 B.G.
 
 )pdoc")
 
-      .def("update_links_from_topo",
-           &D8connector<double>::template update_links_from_topo<
-               std::vector<double>>,
-           py::arg("topography"),
-           R"pdoc(
+		.def("update_links_from_topo",
+			 &D8connector<double>::template update_links_from_topo<
+				 std::vector<double>>,
+			 py::arg("topography"),
+			 R"pdoc(
 Updates all the link directionalities - but not the SFD receiver/donors.
 
 Description:
 ------------
 
 Updates all the link directionalities based on a given topography. This is the
 full updating function computing MFD/SFD links/receivers/donors/... .
@@ -1717,19 +1717,19 @@
 
 Authors:
 --------
 B.G.
 
 )pdoc")
 
-      .def("sum_at_outlets",
-           &D8connector<double>::template sum_at_outlets<py::array_t<double, 1>,
-                                                         double>,
-           py::arg("array"), py::arg("include_pits"),
-           R"pdoc(
+		.def("sum_at_outlets",
+			 &D8connector<double>::template sum_at_outlets<py::array_t<double, 1>,
+														 double>,
+			 py::arg("array"), py::arg("include_pits"),
+			 R"pdoc(
 Sum the values contains in the input array where flux out the model.
 
 Description:
 ------------
 
 Sum the values contains in the input array where flux out the model. It can also
 include the internal pit if needed. Internal pits are only referring to nodes
@@ -1751,19 +1751,19 @@
 
 Authors:
 --------
 B.G.
 
 )pdoc")
 
-      .def("keep_only_at_outlets",
-           &D8connector<double>::template keep_only_at_outlets<
-               py::array_t<double, 1>, py::array>,
-           py::arg("array"), py::arg("include_pits"),
-           R"pdoc(
+		.def("keep_only_at_outlets",
+			 &D8connector<double>::template keep_only_at_outlets<
+				 py::array_t<double, 1>, py::array>,
+			 py::arg("array"), py::arg("include_pits"),
+			 R"pdoc(
 return a copy of the input array where all the non-outting nodes are set to 0.
 
 Description:
 ------------
 
 returns a copy of the input array where all the outting nodes are set to 0.
 It can also include the internal pit if needed. Internal pits are only referring
@@ -1785,18 +1785,18 @@
 
 Authors:
 --------
 B.G.
 
 )pdoc")
 
-      .def(
-          "get_SFD_receivers",
-          &D8connector<double>::template get_SFD_receivers<py::array_t<int, 1>>,
-          R"pdoc(
+		.def(
+			"get_SFD_receivers",
+			&D8connector<double>::template get_SFD_receivers<py::array_t<int, 1>>,
+			R"pdoc(
 returns the array of SFD receivers.
 
 Description:
 ------------
 
 returns the array of SFD receivers according to the current state of the \
 connector. These can be obtained after computing links from a topography, but
@@ -1809,17 +1809,17 @@
 
 Authors:
 --------
 B.G.
 
 )pdoc")
 
-      .def("get_SFD_dx",
-           &D8connector<double>::template get_SFD_dx<py::array_t<double, 1>>,
-           R"pdoc(
+		.def("get_SFD_dx",
+			 &D8connector<double>::template get_SFD_dx<py::array_t<double, 1>>,
+			 R"pdoc(
 returns the array of SFD distance to receivers.
 
 Description:
 ------------
 
 returns the array of SFD dist. to receivers according to the current state of
 the connector. These can be obtained after computing links from a topography,
@@ -1832,17 +1832,17 @@
 
 Authors:
 --------
 B.G.
 
 )pdoc")
 
-      .def("get_SFD_ndonors",
-           &D8connector<double>::template get_SFD_ndonors<py::array_t<int, 1>>,
-           R"pdoc(
+		.def("get_SFD_ndonors",
+			 &D8connector<double>::template get_SFD_ndonors<py::array_t<int, 1>>,
+			 R"pdoc(
 returns the array of SFD number of donors.
 
 Description:
 ------------
 
 returns the array of number of SFD donors for every nodes.
 
@@ -1853,18 +1853,18 @@
 
 Authors:
 --------
 B.G.
 
 )pdoc")
 
-      .def("get_SFD_donors_flat",
-           &D8connector<double>::template get_SFD_donors_flat<
-               py::array_t<int, 1>>,
-           R"pdoc(
+		.def("get_SFD_donors_flat",
+			 &D8connector<double>::template get_SFD_donors_flat<
+				 py::array_t<int, 1>>,
+			 R"pdoc(
 returns a flat array of SFD donors(read description for indexing!).
 
 Description:
 ------------
 
 returns a flat array of SFD donors. It is a sparse array for the sake of simplicity:
 the Donors for a node are every >=0 nodes from the index node_index * 8 to
@@ -1877,18 +1877,18 @@
 
 Authors:
 --------
 B.G.
 
 )pdoc")
 
-      .def("get_SFD_donors_list",
-           &D8connector<double>::template get_SFD_donors_list<
-               std::vector<std::vector<int>>>,
-           R"pdoc(
+		.def("get_SFD_donors_list",
+			 &D8connector<double>::template get_SFD_donors_list<
+				 std::vector<std::vector<int>>>,
+			 R"pdoc(
 returns a list (not an array!) of irregular size with donor indices.
 
 Description:
 ------------
 
 returns a list (not an array!) of irregular size with donor indices. The first
 index is the node index and it points to a list of ndonors size with all the
@@ -1901,17 +1901,17 @@
 
 Authors:
 --------
 B.G.
 
 )pdoc")
 
-      .def("get_links",
-           &D8connector<double>::template get_links<std::vector<std::uint8_t>>,
-           R"pdoc(
+		.def("get_links",
+			 &D8connector<double>::template get_links<std::vector<std::uint8_t>>,
+			 R"pdoc(
 returns an array of link size with link type.
 
 Description:
 ------------
 
 returns an array of link size with link type. See the documentation for the
 relationships between nodes and links. the node indices for a link index can be
@@ -1926,18 +1926,18 @@
 
 Authors:
 --------
 B.G.
 
 )pdoc")
 
-      .def("get_linknodes_flat",
-           &D8connector<double>::template get_linknodes_flat<
-               py::array_t<int, 1>>,
-           R"pdoc(
+		.def("get_linknodes_flat",
+			 &D8connector<double>::template get_linknodes_flat<
+				 py::array_t<int, 1>>,
+			 R"pdoc(
 returns a flat array of linknodes (node indices pair for each links).
 
 Description:
 ------------
 
 1D flat array of linknodes. The node corresponding to link index li can be found
 at linknodes[li*2] and linknodes[li*2 + 1]. Non-existing or invalid links have
@@ -1950,18 +1950,18 @@
 
 Authors:
 --------
 B.G.
 
 )pdoc")
 
-      .def("get_linknodes_list",
-           &D8connector<double>::template get_linknodes_list<
-               std::vector<std::vector<int>>>,
-           R"pdoc(
+		.def("get_linknodes_list",
+			 &D8connector<double>::template get_linknodes_list<
+				 std::vector<std::vector<int>>>,
+			 R"pdoc(
 returns a list (not an array!) of link nodes.
 
 Description:
 ------------
 
 2D link of link nodes. index is link index and it provides a list of nodes
 composing the link.
@@ -1973,18 +1973,18 @@
 
 Authors:
 --------
 B.G.
 
 )pdoc")
 
-      .def("get_linknodes_list_oriented",
-           &D8connector<double>::template get_linknodes_list_oriented<
-               std::vector<std::vector<int>>>,
-           R"pdoc(
+		.def("get_linknodes_list_oriented",
+			 &D8connector<double>::template get_linknodes_list_oriented<
+				 std::vector<std::vector<int>>>,
+			 R"pdoc(
 returns a list (not an array!) of link nodes, donor first, rec second.
 
 Description:
 ------------
 
 2D link of link nodes. index is link index and it provides a list of nodes
 composing the link. This version orients the list with the donor always first
@@ -1997,38 +1997,38 @@
 
 Authors:
 --------
 B.G.
 
 )pdoc")
 
-      .def(
-          "get_SFD_receivers_at_node",
-          &D8connector<double>::get_SFD_receivers_at_node,
-          R"pdoc(Returns the node index of the SFD receivers for a given node index)pdoc")
-
-      .def(
-          "get_SFD_dx_at_node", &D8connector<double>::get_SFD_dx_at_node,
-          R"pdoc(Returns the distance to the SFD receivers for a given node index)pdoc")
-
-      .def("get_SFD_ndonors_at_node",
-           &D8connector<double>::get_SFD_ndonors_at_node
-
-           )
-
-      .def("get_SFD_donors_at_node",
-           &D8connector<double>::template get_SFD_donors_at_node<
-               std::vector<int>>,
-           R"pdoc(Returns a list of SFD donors for a given node index)pdoc")
-
-      .def("get_SFD_gradient",
-           &D8connector<double>::template get_SFD_gradient<
-               py::array_t<double, 1>, py::array_t<double, 1>>,
-           py::arg("topography"),
-           R"pdoc(
+		.def(
+			"get_SFD_receivers_at_node",
+			&D8connector<double>::get_SFD_receivers_at_node,
+			R"pdoc(Returns the node index of the SFD receivers for a given node index)pdoc")
+
+		.def(
+			"get_SFD_dx_at_node", &D8connector<double>::get_SFD_dx_at_node,
+			R"pdoc(Returns the distance to the SFD receivers for a given node index)pdoc")
+
+		.def("get_SFD_ndonors_at_node",
+			 &D8connector<double>::get_SFD_ndonors_at_node
+
+			 )
+
+		.def("get_SFD_donors_at_node",
+			 &D8connector<double>::template get_SFD_donors_at_node<
+				 std::vector<int>>,
+			 R"pdoc(Returns a list of SFD donors for a given node index)pdoc")
+
+		.def("get_SFD_gradient",
+			 &D8connector<double>::template get_SFD_gradient<
+				 py::array_t<double, 1>, py::array_t<double, 1>>,
+			 py::arg("topography"),
+			 R"pdoc(
 returns an array of node size with the topographic gradient
 
 Description:
 ------------
 
 Takes a topography and returns the steepest descent gradient using precomputed
 SFD receivers informations. Note that if you feed the function with a different
@@ -2047,19 +2047,19 @@
 
 Authors:
 --------
 B.G.
 
 )pdoc")
 
-      .def("get_links_gradient",
-           &D8connector<double>::template get_links_gradient<
-               py::array_t<double, 1>, py::array_t<double, 1>>,
-           py::arg("topography"), py::arg("minimum_slope"),
-           R"pdoc(
+		.def("get_links_gradient",
+			 &D8connector<double>::template get_links_gradient<
+				 py::array_t<double, 1>, py::array_t<double, 1>>,
+			 py::arg("topography"), py::arg("minimum_slope"),
+			 R"pdoc(
 returns an array of link size with the topographic gradient for each of them.
 
 Description:
 ------------
 
 Takes a topography and returns the gradient for each topographic link. It can
 recast teh negative/small gradients to a minimum value if needed.
@@ -2078,19 +2078,19 @@
 
 Authors:
 --------
 B.G.
 
 )pdoc")
 
-      .def("get_MFD_mean_gradient",
-           &D8connector<double>::template get_MFD_mean_gradient<
-               py::array_t<double, 1>, py::array_t<double, 1>>,
-           py::arg("topography"),
-           R"pdoc(
+		.def("get_MFD_mean_gradient",
+			 &D8connector<double>::template get_MFD_mean_gradient<
+				 py::array_t<double, 1>, py::array_t<double, 1>>,
+			 py::arg("topography"),
+			 R"pdoc(
 returns an array of node size with the mean topographic gradient for each nodes.
 
 Description:
 ------------
 
 returns an array of node size with the mean topographic gradient for each nodes.
 The gradient is computed for all receivers and averaged.
@@ -2108,21 +2108,21 @@
 
 Authors:
 --------
 B.G.
 
 )pdoc"
 
-           )
+			 )
 
-      .def("get_MFD_weighted_gradient",
-           &D8connector<double>::template get_MFD_weighted_gradient<
-               py::array_t<double, 1>, py::array_t<double, 1>>,
-           py::arg("topography"), py::arg("weights"),
-           R"pdoc(
+		.def("get_MFD_weighted_gradient",
+			 &D8connector<double>::template get_MFD_weighted_gradient<
+				 py::array_t<double, 1>, py::array_t<double, 1>>,
+			 py::arg("topography"), py::arg("weights"),
+			 R"pdoc(
 returns an array of node size with the weighted mean gradient for each nodes.
 
 Description:
 ------------
 
 returns an array of node size with the weighted mean gradient for each nodes.
 It requires a weight for each links which can be obtained using the
@@ -2142,19 +2142,19 @@
 
 Authors:
 --------
 B.G.
 
 )pdoc")
 
-      .def("get_link_weights",
-           &D8connector<double>::template get_link_weights<
-               py::array_t<double, 1>, py::array_t<double, 1>>,
-           py::arg("gradients"), py::arg("exponent"),
-           R"pdoc(
+		.def("get_link_weights",
+			 &D8connector<double>::template get_link_weights<
+				 py::array_t<double, 1>, py::array_t<double, 1>>,
+			 py::arg("gradients"), py::arg("exponent"),
+			 R"pdoc(
 Computes partition weights for each link function of rec slopes per node basis.
 
 Description:
 ------------
 
 Assign a [0,1] weight to each link to partition flow in MFD from every nodes to
 their receivers. The partition uses an exponent to set the sensitivity to slope
@@ -2177,138 +2177,143 @@
 
 Array of link size of partition weights
 
 Authors:
 --------
 B.G.)pdoc")
 
-      .def(
-          "set_stochaticiy_for_SFD",
-          &D8connector<double>::set_stochaticiy_for_SFD, py::arg("magnitude"),
-          R"pdoc(EXPERIMENTAL: adds stochasticity to the SFD receivers calculation. Best to ignore.)pdoc");
-
-  py::class_<D4connector<double>>(
-      m, "D4N",
-      R"pdoc(DEPRECATED - will be back at some points, keeping for legacy)pdoc")
-      .def(py::init<int, int, double, double, double, double>())
-      .def("set_default_boundaries",
-           &D4connector<double>::set_default_boundaries)
-      .def("set_custom_boundaries",
-           &D4connector<double>::set_custom_boundaries<py::array_t<int, 1>>)
-      .def("print_dim", &D4connector<double>::print_dim)
-      .def("get_HS",
-           &D4connector<double>::get_HS<std::vector<double>, py::array>)
-      // .def("fill_barne_2014",
-      // &D4connector<double>::fill_barne_2014<std::vector<double> >)
-      .def("get_mask_array", &D4connector<double>::get_mask_array)
-      .def("set_values_at_boundaries",
-           &D4connector<double>::set_values_at_boundaries<
-               py::array_t<double, 1>>)
-      .def("set_out_boundaries_to_permissive",
-           &D4connector<double>::set_out_boundaries_to_permissive)
-      .def("get_boundary_at_node", &D4connector<double>::get_boundary_at_node);
-
-  py::class_<numvec<double>>(m, "numvecf64")
-      .def(py::init<py::array_t<double, 1> &>())
-      .def("get", &numvec<double>::get)
-      .def("set", &numvec<double>::set);
-
-  declare_graph<D8connector<double>>(m, "graph");
-  // declare_graph<D4connector<double> >(m,"graphD4");
-
-  //=============================================================================================
-  //=============================================================================================
-  //===================== Standalone Algorithms
-  //=================================================
-  //=============================================================================================
-  //=============================================================================================
-
-  m.def("hillshade",
-        &hillshade<D8connector<double>, py::array_t<double, 1>,
-                   py::array_t<double, 1>, double>,
-        py::arg("connector"), py::arg("topography"),
-        R"pbdoc(
+		.def(
+			"set_stochaticiy_for_SFD",
+			&D8connector<double>::set_stochaticiy_for_SFD, py::arg("magnitude"),
+			R"pdoc(EXPERIMENTAL: adds stochasticity to the SFD receivers calculation. Best to ignore.)pdoc");
+
+	py::class_<D4connector<double>>(
+		m, "D4N",
+		R"pdoc(DEPRECATED - will be back at some points, keeping for legacy)pdoc")
+		.def(py::init<int, int, double, double, double, double>())
+		.def("set_default_boundaries",
+			 &D4connector<double>::set_default_boundaries)
+		.def("set_custom_boundaries",
+			 &D4connector<double>::set_custom_boundaries<py::array_t<int, 1>>)
+		.def("print_dim", &D4connector<double>::print_dim)
+		.def("get_HS",
+			 &D4connector<double>::get_HS<std::vector<double>, py::array>)
+		// .def("fill_barne_2014",
+		// &D4connector<double>::fill_barne_2014<std::vector<double> >)
+		.def("get_mask_array", &D4connector<double>::get_mask_array)
+		.def("set_values_at_boundaries",
+			 &D4connector<double>::set_values_at_boundaries<
+				 py::array_t<double, 1>>)
+		.def("set_out_boundaries_to_permissive",
+			 &D4connector<double>::set_out_boundaries_to_permissive)
+		.def("get_boundary_at_node", &D4connector<double>::get_boundary_at_node);
+
+	py::class_<numvec<double>>(m, "numvecf64")
+		.def(py::init<py::array_t<double, 1> &>())
+		.def("get", &numvec<double>::get)
+		.def("set", &numvec<double>::set);
+
+	declare_graph<D8connector<double>>(m, "graph");
+	// declare_graph<D4connector<double> >(m,"graphD4");
+
+	//=============================================================================================
+	//=============================================================================================
+	//===================== Standalone Algorithms
+	//=================================================
+	//=============================================================================================
+	//=============================================================================================
+
+	m.def("hillshade",
+		&hillshade<D8connector<double>, py::array_t<double, 1>,
+					 py::array_t<double, 1>, double>,
+		py::arg("connector"), py::arg("topography"),
+		R"pbdoc(
 Hillshading function for visualisation
 
 Description:
 ------------
 
 Returns a [0,1] hillshade for a regular grid. Negative/nodata are set to 0
 
 Parameters:
 -----------
 
-    * D8connector
-    * Flat topography of node size (1D array)
+	* D8connector
+	* Flat topography of node size (1D array)
 
 Returns:
 --------
 
-    * Flat hillshade of node size (1D array)
+	* Flat hillshade of node size (1D array)
 
 Authors:
 --------
 B.G.
 
 )pbdoc");
 
-  m.def("rayshade",
-        &rayshade<DAGGER::graph<double, DAGGER::D8connector<double>>,
-                  D8connector<double>, py::array_t<double, 1>,
-                  py::array_t<double, 1>, double>);
-
-  m.def("set_BC_to_remove_seas",
-        &set_BC_to_remove_seas<D8connector<double>, py::array_t<double, 1>,
-                               double>);
-
-  m.def("label_depressions_PQ",
-        &label_depressions_PQ<py::array_t<double, 1>, py::array_t<int, 1>,
-                              D8connector<double>>);
-
-  m.def("label_ocean", &label_ocean<py::array_t<double, 1>, py::array_t<int, 1>,
-                                    D8connector<double>>);
-
-  m.def("standalone_priority_flood",
-        &standalone_priority_flood<D8connector<double>, py::array_t<double, 1>,
-                                   py::array_t<double, 1>, double>,
-        py::arg("topography"), py::arg("connector"));
-
-  m.def("standalone_priority_flood_opti",
-        &standalone_priority_flood_opti<
-            D8connector<double>,
-            DAGGER::graph<double, DAGGER::D8connector<double>>,
-            py::array_t<double, 1>, py::array_t<double, 1>, double>,
-        py::arg("topography"), py::arg("connector"), py::arg("graph"));
-
-  m.def("RiverNetwork",
-        RiverNetwork<double, DAGGER::D8connector<double>,
-                     DAGGER::graph<double, DAGGER::D8connector<double>>>);
-
-  // m.def(
-  //   "check_connector_template",
-  //   &check_connector_template< D8connector<double>, double >
-  // );
-
-  declare_popscape_old<DAGGER::D8connector<double>>(m, "popscape_old");
-  declare_popscape<DAGGER::D8connector<double>>(m, "popscape");
-  // // declare_popscape_old<DAGGER::D4connector<double> >(m,"popscape_oldD4");
-  declare_trackscape<DAGGER::D8connector<double>>(m, "trackscape");
-  // // declare_trackscape<DAGGER::D4connector<double> >(m,"trackscapeD4");
-
-  py::enum_<RANDNOISE>(m, "NOISE")
-      .value("WHITE", RANDNOISE::WHITE)
-      .value("RED", RANDNOISE::RED)
-      .value("PERLIN", RANDNOISE::PERLIN);
-
-  declare_graphflood<double, DAGGER::graph<double, DAGGER::D8connector<double>>,
-                     DAGGER::D8connector<double>>(m, "graphflood");
-
-  m.def("generate_perlin_noise_2D",
-        &generate_perlin_noise_2D<py::array_t<double, 1>, double,
-                                  D8connector<double>>);
+	m.def("rayshade",
+		&rayshade<DAGGER::graph<double, DAGGER::D8connector<double>>,
+					D8connector<double>, py::array_t<double, 1>,
+					py::array_t<double, 1>, double>);
+
+	m.def("set_BC_to_remove_seas",
+		&set_BC_to_remove_seas<D8connector<double>, py::array_t<double, 1>,
+								 double>);
+
+	m.def("label_depressions_PQ",
+		&label_depressions_PQ<py::array_t<double, 1>, py::array_t<int, 1>,
+								D8connector<double>>);
+
+	m.def("label_ocean", &label_ocean<py::array_t<double, 1>, py::array_t<int, 1>,
+									D8connector<double>>);
+
+	m.def("standalone_priority_flood",
+		&standalone_priority_flood<D8connector<double>, py::array_t<double, 1>,
+									 py::array_t<double, 1>, double>,
+		py::arg("topography"), py::arg("connector"));
+
+	m.def("standalone_priority_flood_opti",
+		&standalone_priority_flood_opti<
+			D8connector<double>,
+			DAGGER::graph<double, DAGGER::D8connector<double>>,
+			py::array_t<double, 1>, py::array_t<double, 1>, double>,
+		py::arg("topography"), py::arg("connector"), py::arg("graph"));
+
+	m.def("RiverNetwork",
+		RiverNetwork<double, DAGGER::D8connector<double>,
+					 DAGGER::graph<double, DAGGER::D8connector<double>>>);
+	m.def("DrainageDivides",
+		DrainageDivides<double, DAGGER::D8connector<double>,
+					 DAGGER::graph<double, DAGGER::D8connector<double>>>);
+
+	
+
+	// m.def(
+	//   "check_connector_template",
+	//   &check_connector_template< D8connector<double>, double >
+	// );
+
+	declare_popscape_old<DAGGER::D8connector<double>>(m, "popscape_old");
+	declare_popscape<DAGGER::D8connector<double>>(m, "popscape");
+	// // declare_popscape_old<DAGGER::D4connector<double> >(m,"popscape_oldD4");
+	declare_trackscape<DAGGER::D8connector<double>>(m, "trackscape");
+	// // declare_trackscape<DAGGER::D4connector<double> >(m,"trackscapeD4");
+
+	py::enum_<RANDNOISE>(m, "NOISE")
+		.value("WHITE", RANDNOISE::WHITE)
+		.value("RED", RANDNOISE::RED)
+		.value("PERLIN", RANDNOISE::PERLIN);
+
+	declare_graphflood<double, DAGGER::graph<double, DAGGER::D8connector<double>>,
+					 DAGGER::D8connector<double>>(m, "graphflood");
+
+	m.def("generate_perlin_noise_2D",
+		&generate_perlin_noise_2D<py::array_t<double, 1>, double,
+									D8connector<double>>);
 
-  m.def("quick_fluvial_topo",
-        &quick_fluvial_topo<float, py::array_t<float, 1>>);
+	m.def("quick_fluvial_topo",
+		&quick_fluvial_topo<float, py::array_t<float, 1>>);
 };
 ;
 
 // end of file
```

### Comparing `daggerpy-0.0.5/setup.py` & `daggerpy-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # pybind11 is used for c++ integration
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 from setuptools import setup, find_packages
 import os
 import platform
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 
 
 
 #############################################
 # Admin inputs
 #############################################
```

### Comparing `daggerpy-0.0.5/tests/test_dagger.py` & `daggerpy-0.0.6/tests/test_dagger.py`

 * *Files identical despite different names*


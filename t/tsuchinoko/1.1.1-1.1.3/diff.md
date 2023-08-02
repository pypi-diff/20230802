# Comparing `tmp/tsuchinoko-1.1.1.tar.gz` & `tmp/tsuchinoko-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsuchinoko-1.1.1.tar", last modified: Tue Aug  1 19:00:51 2023, max compression
+gzip compressed data, was "tsuchinoko-1.1.3.tar", last modified: Wed Aug  2 20:29:06 2023, max compression
```

## Comparing `tsuchinoko-1.1.1.tar` & `tsuchinoko-1.1.3.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.907714 tsuchinoko-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-08-01 19:00:51.907714 tsuchinoko-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.891714 tsuchinoko-1.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.891714 tsuchinoko-1.1.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/legal.txt
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-01 19:00:51.907714 tsuchinoko-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.895714 tsuchinoko-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tests/test_graphics_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tests/test_gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.907714 tsuchinoko-1.1.1/tsuchinoko/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-01 19:00:51.907714 tsuchinoko-1.1.1/tsuchinoko/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.899714 tsuchinoko-1.1.1/tsuchinoko/adaptive/
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/adaptive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/adaptive/_adaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/adaptive/acquisition_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/adaptive/adaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/adaptive/fvgp_gpCAM_in_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/adaptive/gpCAM_in_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/adaptive/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    17537 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/adaptive/quadtree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/adaptive/random_in_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.899714 tsuchinoko-1.1.1/tsuchinoko/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.899714 tsuchinoko-1.1.1/tsuchinoko/core/
--rw-r--r--   0 runner    (1001) docker     (123)    12841 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/core/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.899714 tsuchinoko-1.1.1/tsuchinoko/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/IRBL_server_demo_LC.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/_launch_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/adaptive_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/bluesky_adaptive_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/client_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/grid_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/headless_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/high_dimensionality_server_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/ir_server_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/multi_task_server_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/quadtree_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/server_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/server_demo_bluesky.py
--rw-r--r--   0 runner    (1001) docker     (123)   112760 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/sombrero_pug.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/vector_metric_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.903714 tsuchinoko-1.1.1/tsuchinoko/execution/
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/execution/bluesky_adaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/execution/bluesky_in_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/execution/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/execution/threaded_in_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.903714 tsuchinoko-1.1.1/tsuchinoko/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.903714 tsuchinoko-1.1.1/tsuchinoko/graphics_items/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/graphics_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24019 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/graphics_items/clouditem.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/graphics_items/indicatoritem.py
--rw-r--r--   0 runner    (1001) docker     (123)    13024 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/graphics_items/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.903714 tsuchinoko-1.1.1/tsuchinoko/graphs/
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/graphs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19804 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/graphs/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.903714 tsuchinoko-1.1.1/tsuchinoko/parameters/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/parameters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.903714 tsuchinoko-1.1.1/tsuchinoko/patches/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/patches/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/patches/pyqode.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/patches/pyqtgraph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.903714 tsuchinoko-1.1.1/tsuchinoko/plan_stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/plan_stubs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.907714 tsuchinoko-1.1.1/tsuchinoko/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/utils/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/utils/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/utils/mutex.py
--rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/utils/runengine.py
--rw-r--r--   0 runner    (1001) docker     (123)    13395 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/utils/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.907714 tsuchinoko-1.1.1/tsuchinoko/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/widgets/debugmenubar.py
--rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/widgets/displays.py
--rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/widgets/graph_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    19662 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/widgets/mainwindow.py
--rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/widgets/server_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/widgets/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.895714 tsuchinoko-1.1.1/tsuchinoko.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-08-01 19:00:51.000000 tsuchinoko-1.1.1/tsuchinoko.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-08-01 19:00:51.000000 tsuchinoko-1.1.1/tsuchinoko.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 19:00:51.000000 tsuchinoko-1.1.1/tsuchinoko.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-01 19:00:51.000000 tsuchinoko-1.1.1/tsuchinoko.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-01 19:00:51.000000 tsuchinoko-1.1.1/tsuchinoko.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 19:00:51.000000 tsuchinoko-1.1.1/tsuchinoko.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:29:06.132493 tsuchinoko-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-08-02 20:29:06.132493 tsuchinoko-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:29:06.120493 tsuchinoko-1.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:29:06.120493 tsuchinoko-1.1.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/legal.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-02 20:29:06.132493 tsuchinoko-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:29:06.120493 tsuchinoko-1.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tests/test_graphics_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tests/test_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:29:06.132493 tsuchinoko-1.1.3/tsuchinoko/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-02 20:29:06.132493 tsuchinoko-1.1.3/tsuchinoko/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:29:06.124493 tsuchinoko-1.1.3/tsuchinoko/adaptive/
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/adaptive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/adaptive/_adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/adaptive/acquisition_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/adaptive/adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/adaptive/fvgp_gpCAM_in_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/adaptive/gpCAM_in_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/adaptive/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17537 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/adaptive/quadtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/adaptive/random_in_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:29:06.124493 tsuchinoko-1.1.3/tsuchinoko/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:29:06.124493 tsuchinoko-1.1.3/tsuchinoko/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    13103 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/core/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:29:06.128493 tsuchinoko-1.1.3/tsuchinoko/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/examples/IRBL_server_demo_LC.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/examples/_launch_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/examples/adaptive_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/examples/bluesky_adaptive_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/examples/client_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/examples/grid_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/examples/headless_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/examples/high_dimensionality_server_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/examples/ir_server_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/examples/multi_task_server_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/examples/quadtree_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/examples/server_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/examples/server_demo_bluesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112760 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/examples/sombrero_pug.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/examples/vector_metric_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:29:06.128493 tsuchinoko-1.1.3/tsuchinoko/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9155 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/execution/bluesky_adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/execution/bluesky_in_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/execution/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/execution/threaded_in_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:29:06.128493 tsuchinoko-1.1.3/tsuchinoko/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:29:06.128493 tsuchinoko-1.1.3/tsuchinoko/graphics_items/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/graphics_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24019 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/graphics_items/clouditem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/graphics_items/indicatoritem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/graphics_items/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:29:06.128493 tsuchinoko-1.1.3/tsuchinoko/graphs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/graphs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20270 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/graphs/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:29:06.128493 tsuchinoko-1.1.3/tsuchinoko/parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/parameters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:29:06.128493 tsuchinoko-1.1.3/tsuchinoko/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/patches/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/patches/pyqode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/patches/pyqtgraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:29:06.128493 tsuchinoko-1.1.3/tsuchinoko/plan_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/plan_stubs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:29:06.132493 tsuchinoko-1.1.3/tsuchinoko/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/utils/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/utils/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/utils/mutex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/utils/runengine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13395 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/utils/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:29:06.132493 tsuchinoko-1.1.3/tsuchinoko/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/widgets/debugmenubar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/widgets/displays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/widgets/graph_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19662 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/widgets/mainwindow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/widgets/server_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/tsuchinoko/widgets/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:29:06.124493 tsuchinoko-1.1.3/tsuchinoko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-08-02 20:29:06.000000 tsuchinoko-1.1.3/tsuchinoko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-08-02 20:29:06.000000 tsuchinoko-1.1.3/tsuchinoko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 20:29:06.000000 tsuchinoko-1.1.3/tsuchinoko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-02 20:29:06.000000 tsuchinoko-1.1.3/tsuchinoko.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-02 20:29:06.000000 tsuchinoko-1.1.3/tsuchinoko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-02 20:29:06.000000 tsuchinoko-1.1.3/tsuchinoko.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-08-02 20:28:55.000000 tsuchinoko-1.1.3/versioneer.py
```

### Comparing `tsuchinoko-1.1.1/CONTRIBUTING.rst` & `tsuchinoko-1.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/LICENSE` & `tsuchinoko-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/PKG-INFO` & `tsuchinoko-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsuchinoko
-Version: 1.1.1
+Version: 1.1.3
 Summary: An adaptive optics alignment tool for ALS beamlines utilizing gpCAM.
 Home-page: https://github.com/lbl-camera/tsuchinoko
 Author: Ronald J Pandolfi
 Author-email: ronpandolfi@lbl.gov
 License: GPLv3+
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `tsuchinoko-1.1.1/README.md` & `tsuchinoko-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/docs/Makefile` & `tsuchinoko-1.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/docs/make.bat` & `tsuchinoko-1.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/docs/source/conf.py` & `tsuchinoko-1.1.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/legal.txt` & `tsuchinoko-1.1.3/legal.txt`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/setup.py` & `tsuchinoko-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tests/test_core.py` & `tsuchinoko-1.1.3/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tests/test_graphics_items.py` & `tsuchinoko-1.1.3/tests/test_graphics_items.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tests/test_gui.py` & `tsuchinoko-1.1.3/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/__init__.py` & `tsuchinoko-1.1.3/tsuchinoko/__init__.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/adaptive/__init__.py` & `tsuchinoko-1.1.3/tsuchinoko/adaptive/__init__.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/adaptive/acquisition_functions.py` & `tsuchinoko-1.1.3/tsuchinoko/adaptive/acquisition_functions.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/adaptive/adaptive.py` & `tsuchinoko-1.1.3/tsuchinoko/adaptive/adaptive.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/adaptive/fvgp_gpCAM_in_process.py` & `tsuchinoko-1.1.3/tsuchinoko/adaptive/fvgp_gpCAM_in_process.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,29 +29,17 @@
                            Table()]
 
     # TODO: refactor this into base
     def init_optimizer(self):
         parameter_bounds = np.asarray([[self.parameters[('bounds', f'axis_{i}_{edge}')]
                                         for edge in ['min', 'max']]
                                        for i in range(self.dimensionality)])
-        hyperparameters = np.asarray([self.parameters[('hyperparameters', f'hyperparameter_{i}')]
-                                      for i in range(self.num_hyperparameters)])
 
         self.optimizer = fvGPOptimizer(self.dimensionality, self.output_dim, self.output_number, parameter_bounds)
 
-        if self.initial_x_data is not None and self.initial_y_data is not None:
-            variance_kwargs = {}
-            if self.initial_v_data is not None:
-                variance_kwargs['variances'] = self.initial_v_data
-            self.optimizer.tell(self.initial_x_data, self.initial_y_data, **variance_kwargs)
-
-        opts = self.gp_opts.copy()
-        # TODO: only fallback to numpy when packaged as an app
-        if sys.platform == 'darwin':
-            opts['compute_device'] = 'numpy'
-
+    def init_gp(self, hyperparameters, **opts):
         self.optimizer.init_fvgp(hyperparameters, **opts)
 
     def _set_hyperparameter(self, parameter, value):
         self.optimizer.gp_initialized = False  # Force re-initialization
         self.optimizer.init_fvgp(np.asarray([self.parameters[('hyperparameters', f'hyperparameter_{i}')]
                                            for i in range(self.num_hyperparameters)]))
```

### Comparing `tsuchinoko-1.1.1/tsuchinoko/adaptive/gpCAM_in_process.py` & `tsuchinoko-1.1.3/tsuchinoko/adaptive/gpCAM_in_process.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,20 +29,19 @@
     """
     An adaptive engine powered by gpCAM: https://gpcam.readthedocs.io/en/latest/
     """
     default_retrain_globally_at = (20, 50, 100, 400, 1000)
     default_retrain_locally_at = (20, 40, 60, 80, 100, 200, 400, 1000)
 
     def __init__(self, dimensionality, parameter_bounds, hyperparameters, hyperparameter_bounds,
-                 x_data=None, y_data=None, v_data = None, acquisition_functions:dict[str, Callable]=None, gp_opts: dict = None):
+                 acquisition_functions:dict[str, Callable]=None,
+                 gp_opts: dict = None, ask_opts: dict = None):
         self.dimensionality = dimensionality
         self.gp_opts = gp_opts or {}
-        self.initial_x_data = x_data
-        self.initial_y_data = y_data
-        self.initial_v_data = v_data
+        self.ask_opts = ask_opts or {}
         self.num_hyperparameters = len(hyperparameters)
         if acquisition_functions:
             prepend_update_acquisition_functions(acquisition_functions)
 
         for i in range(dimensionality):
             for j, edge in enumerate(['min', 'max']):
                 self.parameters[('bounds', f'axis_{i}_{edge}')] = parameter_bounds[i][j]
@@ -67,40 +66,22 @@
                            # GPCamAverageCovariance(),
                            Table()]
 
     def init_optimizer(self):
         parameter_bounds = np.asarray([[self.parameters[('bounds', f'axis_{i}_{edge}')]
                                         for edge in ['min', 'max']]
                                        for i in range(self.dimensionality)])
-        hyperparameters = np.asarray([self.parameters[('hyperparameters', f'hyperparameter_{i}')]
-                                      for i in range(self.num_hyperparameters)])
 
         self.optimizer = GPOptimizer(self.dimensionality, parameter_bounds)
 
-        if self.initial_x_data is not None and self.initial_y_data is not None:
-            variance_kwargs = {}
-            if self.initial_v_data is not None:
-                variance_kwargs['variances'] = self.initial_v_data
-            self.optimizer.tell(self.initial_x_data, self.initial_y_data, **variance_kwargs)
-
-        opts = self.gp_opts.copy()
-        # TODO: only fallback to numpy when packaged as an app
-        if sys.platform == 'darwin':
-            opts['compute_device'] = 'numpy'
-        self.optimizer.init_gp(hyperparameters, **opts)
-
     def reset(self):
         self._completed_training = {'global': set(),
                                     'local': set()}
         self.init_optimizer()
 
-        self.optimizer.points = np.array([])
-        self.optimizer.values = np.array([])
-        self.optimizer.variances = np.array([])
-
     @cached_property
     def parameters(self):
         hyper_parameters = [SimpleParameter(title=f'Hyperparameter #{i + 1}', name=f'hyperparameter_{i}', type='float')
                             for i in range(self.num_hyperparameters)]
         hyper_parameters_bounds = [SimpleParameter(title=f'Hyperparameter #{i + 1} {edge}', name=f'hyperparameter_{i}_{edge}', type='float')
                                    for i in range(self.num_hyperparameters) for edge in ['min', 'max']]
         bounds_parameters = [SimpleParameter(title=f'Axis #{i + 1} {edge}', name=f'axis_{i}_{edge}', type='float')
@@ -138,38 +119,60 @@
                                            for i in range(self.num_hyperparameters)]), **opts)
 
     def update_measurements(self, data: Data):
         with data.r_lock():  # quickly grab values within lock before passing to optimizer
             positions = data.positions.copy()
             scores = data.scores.copy()
             variances = data.variances.copy()
-        self.optimizer.tell(np.asarray(positions), scores, variances)
+        self.optimizer.tell(np.asarray(positions), np.asarray(scores), np.asarray(variances))
+        if not self.optimizer.gp_initialized:
+            hyperparameters = np.asarray([self.parameters[('hyperparameters', f'hyperparameter_{i}')]
+                                          for i in range(self.num_hyperparameters)])
+            opts = self.gp_opts.copy()
+            # TODO: only fallback to numpy when packaged as an app
+            if sys.platform == 'darwin':
+                opts['compute_device'] = 'numpy'
+
+            self.init_gp(hyperparameters, **opts)
+
+    def init_gp(self, hyperparameters, **opts):
+        self.optimizer.init_gp(hyperparameters, **opts)
 
     def update_metrics(self, data: Data):
         for graph in self.graphs:
             try:
                 graph.compute(data, self)
             except Exception as ex:
                 logger.exception(ex)
 
     def request_targets(self, position):
-        kwargs = {key: self.parameters[key] for key in ['acquisition_function', 'method', 'pop_size', 'tol']}
-        kwargs.update({'bounds': np.asarray([[self.parameters[('bounds', f'axis_{i}_{edge}')]
-                                              for edge in ['min', 'max']]
-                                             for i in range(self.dimensionality)])})
+        bounds = np.asarray([[self.parameters[('bounds', f'axis_{i}_{edge}')]
+                     for edge in ['min', 'max']]
+                    for i in range(self.dimensionality)])
         n = self.parameters['n']
-        return self.optimizer.ask(position, n, acquisition_function=gpcam_acquisition_functions[kwargs.pop('acquisition_function')], **kwargs)['x']
+
+        # If the GP is not initialized, generate random targets
+        if not self.optimizer.gp_initialized:
+            return [[np.random.uniform(bounds[i][0], bounds[i][1]) for i in range(self.dimensionality)] for j in range(n)]
+        else:
+            kwargs = {key: self.parameters[key] for key in ['acquisition_function', 'method', 'pop_size', 'tol']}
+            kwargs.update({'bounds': bounds})
+            kwargs.update(self.ask_opts)
+            return self.optimizer.ask(position, n, acquisition_function=gpcam_acquisition_functions[kwargs.pop('acquisition_function')], **kwargs)['x']
 
     def train(self):
         for method in ['global', 'local']:
             train_at = set(child.value() for child in self.parameters.child(f'{method}_training').children())
 
             for N in train_at:
-                if len(self.optimizer.values) > N and N not in self._completed_training[method]:
+                if len(self.optimizer.y_data) > N and N not in self._completed_training[method]:
+                    logger.info('Training in progress. This make take a while...')
                     self.optimizer.train(np.asarray([[self.parameters[('hyperparameters', f'hyperparameter_{i}_{edge}')]
                                                       for edge in ['min', 'max']]
                                                      for i in range(self.num_hyperparameters)]),
                                          np.asarray([self.parameters[('hyperparameters', f'hyperparameter_{i}')]
                                                      for i in range(self.num_hyperparameters)]), method=method)
                     self._completed_training[method].add(N)
+                    logger.info(f"New hyperparameters: {self.optimizer.hyperparameters}")
                     # return  # only does global training if specified for both
+
         return True
```

### Comparing `tsuchinoko-1.1.1/tsuchinoko/adaptive/grid.py` & `tsuchinoko-1.1.3/tsuchinoko/adaptive/grid.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/adaptive/quadtree.py` & `tsuchinoko-1.1.3/tsuchinoko/adaptive/quadtree.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/adaptive/random_in_process.py` & `tsuchinoko-1.1.3/tsuchinoko/adaptive/random_in_process.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/core/__init__.py` & `tsuchinoko-1.1.3/tsuchinoko/core/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -193,15 +193,18 @@
             for i, old_graph in enumerate(graph_list):
                 if old_graph.id == new_graph.id:
                     graph_list[i] = new_graph
                     return
         else:
             raise ValueError('Graph not found in graphs lists.')
 
-
+    def initialize_data(self, x, y, v):
+        with log_time('updating engine with initial measurements'):
+            self.data = Data(dimensionality=len(x[0]), positions=x, scores=y, variances=v)
+            self.adaptive_engine.update_measurements(self.data)
 
 
 class ZMQCore(Core):
     def __init__(self, *args, **kwargs):
         super(ZMQCore, self).__init__(*args, **kwargs)
         # self.start_server()
         self.context = None
```

### Comparing `tsuchinoko-1.1.1/tsuchinoko/core/messages.py` & `tsuchinoko-1.1.3/tsuchinoko/core/messages.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/examples/IRBL_server_demo_LC.py` & `tsuchinoko-1.1.3/tsuchinoko/examples/IRBL_server_demo_LC.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/examples/adaptive_demo.py` & `tsuchinoko-1.1.3/tsuchinoko/examples/adaptive_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/examples/bluesky_adaptive_demo.py` & `tsuchinoko-1.1.3/tsuchinoko/examples/bluesky_adaptive_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/examples/grid_demo.py` & `tsuchinoko-1.1.3/tsuchinoko/examples/grid_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/examples/headless_demo.py` & `tsuchinoko-1.1.3/tsuchinoko/examples/headless_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/examples/high_dimensionality_server_demo.py` & `tsuchinoko-1.1.3/tsuchinoko/examples/high_dimensionality_server_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/examples/ir_server_demo.py` & `tsuchinoko-1.1.3/tsuchinoko/examples/ir_server_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/examples/multi_task_server_demo.py` & `tsuchinoko-1.1.3/tsuchinoko/examples/multi_task_server_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/examples/quadtree_demo.py` & `tsuchinoko-1.1.3/tsuchinoko/examples/quadtree_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/examples/server_demo.py` & `tsuchinoko-1.1.3/tsuchinoko/examples/server_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/examples/server_demo_bluesky.py` & `tsuchinoko-1.1.3/tsuchinoko/examples/server_demo_bluesky.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/examples/sombrero_pug.jpg` & `tsuchinoko-1.1.3/tsuchinoko/examples/sombrero_pug.jpg`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/examples/vector_metric_demo.py` & `tsuchinoko-1.1.3/tsuchinoko/examples/vector_metric_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/execution/__init__.py` & `tsuchinoko-1.1.3/tsuchinoko/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/execution/bluesky_adaptive.py` & `tsuchinoko-1.1.3/tsuchinoko/execution/bluesky_adaptive.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from loguru import logger
 from numpy._typing import ArrayLike
 
 from . import Engine
 
 SLEEP_FOR_AGENT_TIME = .1
 SLEEP_FOR_TSUCHINOKO_TIME = .1
+FORCE_KICKSTART_TIME = 5
 
 
 class BlueskyAdaptiveEngine(Engine):
     """
     A `tsuchinoko.adaptive.Engine` that sends targets to Blueskly-Adaptive and receives back measured data.
     """
 
@@ -70,19 +71,17 @@
         while True:
             try:
                 payload = self.recv_payload(flags=zmq.NOBLOCK)
             except zmq.ZMQError:
                 break
             else:
                 assert 'target_measured' in payload
-                x, y = payload['target_measured']
-                # TODO: Its highly recommended to extract a variance for y; we might piggyback on y,
-                #       s.t. y = [y1, y2, ..., yn, y1variance, y2variance, ..., ynvariance]
+                x, (y, v) = payload['target_measured']
                 # TODO: Any additional quantities to be interrogated in Tsuchinoko can be included in the trailing dict
-                new_measurements.append((x, y, [1] * len(y), {}))
+                new_measurements.append((x, y, v, {}))
                 # stash the last position measured as the 'current' position of the instrument
                 self.position = x
         if new_measurements:
             self.has_fresh_points_on_server = False
         return new_measurements
 
     def get_position(self) -> Tuple:
@@ -133,15 +132,20 @@
         super().__init__(*args, **kwargs)
         self.host = host
         self.port = port
         self.outbound_measurements = []
         self.context = None
         self.socket = None
         self.setup_socket()
+        self.last_targets_received = time.time()
+        self.kickstart()
+
+    def kickstart(self):
         self.send_payload({'send_targets': True})  # kickstart to recover from shutdowns
+        self.last_targets_received = time.time()  # forgive lack of response until now
 
     def setup_socket(self):
         self.context = zmq.Context()
         self.socket = self.context.socket(zmq.PAIR)
 
         # Attempt to connect, retry every second if fails
         while True:
@@ -150,19 +154,20 @@
             except zmq.ZMQError:
                 logger.info(f'Unable to connect to tcp://{self.host}:{self.port}. Retrying in 1 second...')
                 time.sleep(1)
             else:
                 logger.info(f'Connected to tcp://{self.host}:{self.port}.')
                 break
 
-    def tell(self, x, y):
+    def tell(self, x, y, v):
         """
         Send measurement to BlueskyAdaptiveEngine
         """
-        payload = {'target_measured': (x, y)}
+        yv = (y, v)
+        payload = {'target_measured': (x, yv)}
         self.send_payload(payload)
 
     def ask(self, batch_size: int) -> Tuple[Sequence[Dict[str, ArrayLike]], Sequence[ArrayLike]]:
         """
         Wait until at least one target is received, also exhaust the queue of received targets, overwriting old ones
         """
         payload = None
@@ -170,15 +175,18 @@
             try:
                 payload = self.recv_payload(flags=zmq.NOBLOCK)
             except zmq.ZMQError:
                 if payload is not None:
                     break
                 else:
                     time.sleep(SLEEP_FOR_TSUCHINOKO_TIME)
+                    if time.time() > self.last_targets_received + FORCE_KICKSTART_TIME:
+                        self.kickstart()
         assert 'targets' in payload
+        self.last_targets_received = time.time()
         return payload['targets']
 
     def send_payload(self, payload: dict):
         logger.info(f'message: {payload}')
         self.socket.send(pickle.dumps(payload))
 
     def recv_payload(self, flags=0) -> dict:
@@ -192,33 +200,35 @@
     A Bluesky-Adaptive 'Agent'. This Agent communicates with Tsuchinoko over zmq to request new targets and report back
     measurements. This is an abstract class that must be subclassed.
 
     A `tsuchinoko.execution.bluesky_adaptive.BlueskyAdaptiveEngine` is required for the Tsuchinoko server to complement
     one of these `TsuchinokoAgent`.
     """
 
-    def tell(self, x, y) -> Dict[str, ArrayLike]:
-        super().tell(x, y)
-        return self.get_tell_document(x, y)
+    def tell(self, x, y, v) -> Dict[str, ArrayLike]:
+        super().tell(x, y, v)
+        return self.get_tell_document(x, y, v)
 
     def ask(self, batch_size: int) -> Tuple[Sequence[Dict[str, ArrayLike]], Sequence[ArrayLike]]:
         targets = super().ask(batch_size)
         return self.get_ask_documents(targets), targets
 
     @abstractmethod
-    def get_tell_document(self, x, y) -> Dict[str, ArrayLike]:
+    def get_tell_document(self, x, y, v) -> Dict[str, ArrayLike]:
         """
         Return any single document corresponding to 'tell'-ing Tsuchinoko about the newly measured `x`, `y` data
 
         Parameters
         ----------
         x :
             Independent variable for data observed
         y :
             Dependent variable for data observed
+        v :
+            Variance for measurement of y
 
         Returns
         -------
         dict
             Dictionary to be unpacked or added to a document
 
         """
```

### Comparing `tsuchinoko-1.1.1/tsuchinoko/execution/bluesky_in_process.py` & `tsuchinoko-1.1.3/tsuchinoko/execution/bluesky_in_process.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/execution/simple.py` & `tsuchinoko-1.1.3/tsuchinoko/execution/simple.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/execution/threaded_in_process.py` & `tsuchinoko-1.1.3/tsuchinoko/execution/threaded_in_process.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/graphics_items/clouditem.py` & `tsuchinoko-1.1.3/tsuchinoko/graphics_items/clouditem.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/graphics_items/mixins.py` & `tsuchinoko-1.1.3/tsuchinoko/graphics_items/mixins.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Callable
 
 import numpy as np
-from pyqtgraph import ImageView, PlotWidget, RectROI, ImageItem
+from pyqtgraph import ImageView, PlotWidget, RectROI, ImageItem, PlotItem
 from qtpy.QtCore import QPointF, Signal, QObject, QEvent, Qt, QSignalBlocker
 from qtpy.QtWidgets import QAction, QWidget, QHBoxLayout, QVBoxLayout, QPushButton, QSizePolicy
 from pyqtgraph import functions as fn, debug, Point
 
 from tsuchinoko.widgets.displays import Configuration
 
 
@@ -79,14 +79,29 @@
         sizePolicy.setHeightForWidth(self.resetLUTBtn.sizePolicy().hasHeightForWidth())
         # self.resetLUTBtn.setSizePolicy(sizePolicy)
         # self.resetLUTBtn.setObjectName("resetLUTBtn")
         self.ui.right_layout.addWidget(self.resetLUTBtn)
         self.resetLUTBtn.clicked.connect(self.autoLevels)
 
 
+class AspectRatioLock(BetterLayout):
+    def __init__(self, *args, lock_aspect=True, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._aspect_ratio_button = QPushButton('Lock Aspect')
+        self._aspect_ratio_button.setCheckable(True)
+        self.ui.right_layout.addWidget(self._aspect_ratio_button)
+        self._aspect_ratio_button.setChecked(lock_aspect)
+        self._aspect_ratio_button.toggled.connect(self.toggle_lock_aspect)
+
+    def toggle_lock_aspect(self):
+        if self._aspect_ratio_button.isChecked():
+            self.view.setAspectLocked(True)
+        else:
+            self.view.setAspectLocked(False)
+
 
 class ComposableItemImageView(ImageView):
     """
     Used to compose together different image view mixins that may use different ItemImage subclasses.
     See LogScaleIntensity, LogScaleImageItem, ImageViewHistogramOverflowFIx, ImageItemHistorgramOverflowFix.
     Note that any imageItem named argument passed into the ImageView mixins above will discard the item and instead
     create a composition of imageItem_bases with their respective ImageItem class.
@@ -266,14 +281,23 @@
             if ev.button() == Qt.MouseButton.RightButton:
                 self._last_mouse_event_pos = ev.pos()
         ev.ignore()
 
         return False
 
 
+class YInvert(ImageView):
+    def __init__(self, *args, invert_y=False, **kwargs):
+        if 'view' in kwargs:
+            raise ValueError(f'Setting view is incompatible with this widget ({type(self)}')
+        graph = PlotItem()
+        super().__init__(*args, view=graph, **kwargs)
+        graph.vb.invertY(invert_y)
+
+
 class ClickRequester(ClickRequesterBase, ImageView):
     def _scene(self):
         return self.scene
 
     def _install_filter(self):
         self.ui.graphicsView.installEventFilter(self)
```

### Comparing `tsuchinoko-1.1.1/tsuchinoko/graphs/__init__.py` & `tsuchinoko-1.1.3/tsuchinoko/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/graphs/common.py` & `tsuchinoko-1.1.3/tsuchinoko/graphs/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from loguru import logger
 from pyqtgraph import PlotItem, PlotWidget, TableWidget, mkColor, intColor, PlotDataItem, mkPen, mkBrush, colormap, \
     ScatterPlotItem
 from qtpy.QtWidgets import QFormLayout, QWidget, QComboBox, QLabel, QVBoxLayout
 from qtpy.QtCore import Qt, QSignalBlocker, Signal, QRectF
 
 from tsuchinoko.graphics_items.mixins import ClickRequester, DomainROI, BetterButtons, LogScaleIntensity, \
-    BetterAutoLUTRangeImageView, ViridisImageView
+    BetterAutoLUTRangeImageView, ViridisImageView, AspectRatioLock, YInvert
 from tsuchinoko.graphs import Graph, Location, graph_signal_relay
 from tsuchinoko.widgets.displays import Configuration
 from tsuchinoko.widgets.graph_widgets import CloudWidget
 import sklearn
 
 from tsuchinoko.widgets.simple import DoubleSlider, ValueDoubleSlider
 
@@ -83,34 +83,36 @@
         if update_slice.start == 0:
             widget.setData(table)
         else:
             for row, table_row in zip(rows, table):
                 widget.setRow(row, list(table_row.values()))
 
 
-@dataclass(eq=False)  # TODO: Should this be a dataclass?
-class ImageViewBlend(DomainROI,
+class ImageViewBlend(YInvert,
                      ClickRequester,
                      BetterButtons,
                      LogScaleIntensity,
+                     AspectRatioLock,
                      BetterAutoLUTRangeImageView,
                      ViridisImageView):
-    def __init__(self, *args, invert_y=False, **kwargs):
-        graph = PlotItem()
-        super().__init__(*args, view=graph, **kwargs)
-        graph.vb.invertY(invert_y)
+    pass
+
+
+class ImageViewBlendROI(DomainROI, ImageViewBlend):
+    pass
 
 
 # TODO: add option for transforming into parameter space or not
 
 @dataclass(eq=False)
 class Image(Graph):
     widget_class = ImageViewBlend
     data_key: ClassVar[str] = None
     accumulates: ClassVar[bool] = False
+    transform_to_parameter_space = True
     widget_kwargs: dict = field(default_factory=lambda: dict(invert_y=False))
 
     def __post_init__(self):
         if not self.name and self.data_key:
             self.name = self.data_key
 
     def update(self, widget, data, update_slice: slice):
@@ -138,21 +140,25 @@
                 elif v.ndim == 3:
                     # if shape is 3d and #3 is 3, use color, otherwise use t for dimensions
                     if v.shape[2] == 3:
                         axes = {'x': 0, 'y': 1, 'c': 2}
                     else:
                         axes = {'t': 2, 'x': 0, 'y': 1}
 
+                kwargs = {}
+                if self.transform_to_parameter_space:
+                    kwargs['pos'] = (bounds[0][0], bounds[1][0])
+                    kwargs['scale'] = ((bounds[0][1] - bounds[0][0]) / v.shape[0], (bounds[1][1] - bounds[1][0]) / v.shape[1])
+
                 widget.setImage(v,
                                 autoRange=widget.imageItem.image is None,
                                 autoLevels=widget.imageItem.image is None,
                                 autoHistogramRange=widget.imageItem.image is None,
-                                pos=(bounds[0][0], bounds[1][0]),
-                                scale=((bounds[0][1]-bounds[0][0])/v.shape[0], (bounds[1][1]-bounds[1][0])/v.shape[1]),
-                                axes=axes)
+                                axes=axes,
+                                **kwargs)
 
 
 @dataclass(eq=False)
 class Cloud(Graph):
     data_key: ClassVar[str] = None
     accumulates: ClassVar[bool] = True
     widget_class = type('CloudBlend', (CloudWidget, DomainROI), {})
@@ -275,32 +281,38 @@
 
 
 @dataclass(eq=False)
 class GPCamPosteriorCovariance(Image):
     shape = (50, 50)
     data_key = 'Posterior Covariance'
     widget_kwargs: dict = field(default_factory=lambda: dict(invert_y=True))
+    transform_to_parameter_space: ClassVar[bool] = False
 
     def compute(self, data, engine: 'GPCamInProcessEngine'):
         with data.r_lock():  # quickly grab positions within lock before passing to optimizer
             positions = np.asarray(data.positions.copy())
 
+        # if multi-task, extend the grid_positions to include the task dimension
+        if hasattr(engine, 'output_number'):
+            positions = np.vstack([np.hstack([positions, np.full((positions.shape[0], 1), i)]) for i in range(engine.output_number)])
+
         # compute posterior covariance without lock
         result_dict = engine.optimizer.posterior_covariance(positions)
 
         # assign to data object with lock
         with data.w_lock():
             data.states[self.data_key] = result_dict['S(x)']
 
 
 @dataclass(eq=False)
 class GPCamAcquisitionFunction(Image):
     compute_with = Location.AdaptiveEngine
     shape = (50, 50)
     data_key = 'Acquisition Function'
+    widget_class = ImageViewBlendROI
 
     def compute(self, data, engine: 'GPCAMInProcessEngine'):
         from tsuchinoko.adaptive.gpCAM_in_process import gpcam_acquisition_functions  # avoid circular import
 
         bounds = tuple(tuple(engine.parameters[('bounds', f'axis_{i}_{edge}')]
                              for edge in ['min', 'max'])
                        for i in range(engine.dimensionality))
@@ -330,14 +342,15 @@
 
 
 @dataclass(eq=False)
 class GPCamPosteriorMean(Image):
     compute_with = Location.AdaptiveEngine
     shape = (50, 50)
     data_key = 'Posterior Mean'
+    widget_class = ImageViewBlendROI
 
     def compute(self, data, engine: 'GPCAMInProcessEngine'):
         bounds = ((engine.parameters[('bounds', f'axis_{i}_{edge}')]
                    for edge in ['min', 'max'])
                   for i in range(engine.dimensionality))
 
         grid_positions = image_grid(bounds, self.shape)
```

### Comparing `tsuchinoko-1.1.1/tsuchinoko/patches/pyqode.py` & `tsuchinoko-1.1.3/tsuchinoko/patches/pyqode.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/patches/pyqtgraph.py` & `tsuchinoko-1.1.3/tsuchinoko/patches/pyqtgraph.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/plan_stubs/__init__.py` & `tsuchinoko-1.1.3/tsuchinoko/plan_stubs/__init__.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/utils/__init__.py` & `tsuchinoko-1.1.3/tsuchinoko/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/utils/coverage.py` & `tsuchinoko-1.1.3/tsuchinoko/utils/coverage.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/utils/dependencies.py` & `tsuchinoko-1.1.3/tsuchinoko/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/utils/logging.py` & `tsuchinoko-1.1.3/tsuchinoko/utils/logging.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/utils/mutex.py` & `tsuchinoko-1.1.3/tsuchinoko/utils/mutex.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/utils/runengine.py` & `tsuchinoko-1.1.3/tsuchinoko/utils/runengine.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/utils/threads.py` & `tsuchinoko-1.1.3/tsuchinoko/utils/threads.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/widgets/debugmenubar.py` & `tsuchinoko-1.1.3/tsuchinoko/widgets/debugmenubar.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from functools import partial
 
 # Hack to work around PySide being imported from nowhere:
 import qtpy
 from loguru import logger
 from qtpy.QtCore import Qt, QObject, QEvent
 from qtpy.QtGui import QKeySequence
-from qtpy.QtWidgets import QMenuBar, QShortcut, QMenu, QWidget, QAction, QActionGroup
+from qtpy.QtWidgets import QMenuBar, QShortcut, QMenu, QWidget, QAction, QActionGroup, QApplication
 
 if "PySide.QtCore" in sys.modules and qtpy.API != "pyside":
     del sys.modules["PySide.QtCore"]
 
 from qtconsole.rich_jupyter_widget import RichJupyterWidget
 from qtconsole.inprocess import QtInProcessKernelManager
 
@@ -86,15 +86,15 @@
             self.kernel_client.stop_channels()
             self.kernel_manager.shutdown_kernel()
 
         self.exit_requested.connect(stop)
 
 
 if __name__ == "__main__":
-    from qtpy.QtWidgets import QApplication, QMainWindow, QLabel
+    from qtpy.QtWidgets import QMainWindow, QLabel
 
     app = QApplication([])
     window = QMainWindow()
     window.setCentralWidget(QLabel("test"))
     db = DebuggableMenuBar()
     window.setMenuBar(db)
     window.show()
```

### Comparing `tsuchinoko-1.1.1/tsuchinoko/widgets/displays.py` & `tsuchinoko-1.1.3/tsuchinoko/widgets/displays.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/widgets/graph_widgets.py` & `tsuchinoko-1.1.3/tsuchinoko/widgets/graph_widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,17 @@
         self.set_current_index(self.timeline.getXPos() + n)
 
     def update_data(self, data, update_slice: slice):
         # require_clear = False
         timeline_at_end = not self.cache or self.timeline.getXPos() == len(self.cache['v']) - 1
 
         with data.r_lock():
-            v = data[self.data_key].copy()
+            v = np.asarray(data[self.data_key].copy())
+            if v.ndim == 2:
+                v = np.squeeze(v, 1)
 
             x, y = zip(*data.positions)
 
         lengths = len(v), len(x), len(y)
         min_length = min(lengths)
 
         if not np.all(np.array(lengths) == min_length):
```

### Comparing `tsuchinoko-1.1.1/tsuchinoko/widgets/mainwindow.py` & `tsuchinoko-1.1.3/tsuchinoko/widgets/mainwindow.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/widgets/server_editor.py` & `tsuchinoko-1.1.3/tsuchinoko/widgets/server_editor.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko/widgets/simple.py` & `tsuchinoko-1.1.3/tsuchinoko/widgets/simple.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/tsuchinoko.egg-info/PKG-INFO` & `tsuchinoko-1.1.3/tsuchinoko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsuchinoko
-Version: 1.1.1
+Version: 1.1.3
 Summary: An adaptive optics alignment tool for ALS beamlines utilizing gpCAM.
 Home-page: https://github.com/lbl-camera/tsuchinoko
 Author: Ronald J Pandolfi
 Author-email: ronpandolfi@lbl.gov
 License: GPLv3+
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `tsuchinoko-1.1.1/tsuchinoko.egg-info/SOURCES.txt` & `tsuchinoko-1.1.3/tsuchinoko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.1/versioneer.py` & `tsuchinoko-1.1.3/versioneer.py`

 * *Files identical despite different names*


# Comparing `tmp/ocsmesh-1.3.4.tar.gz` & `tmp/ocsmesh-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocsmesh-1.3.4.tar", last modified: Thu Jun 22 19:24:45 2023, max compression
+gzip compressed data, was "ocsmesh-1.3.5.tar", last modified: Wed Aug  2 17:44:06 2023, max compression
```

## Comparing `ocsmesh-1.3.4.tar` & `ocsmesh-1.3.5.tar`

### file list

```diff
@@ -1,104 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.394126 ocsmesh-1.3.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.374125 ocsmesh-1.3.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.378125 ocsmesh-1.3.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/.github/workflows/documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/.github/workflows/functional_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/.github/workflows/functional_test_2.yml
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10967 2023-06-22 19:24:45.394126 ocsmesh-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.378125 ocsmesh-1.3.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)  2851126 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/docs/noaa_33879_DS1.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.382125 ocsmesh-1.3.4/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/docs/source/ocsmesh.command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/docs/source/ocsmesh.geometry.rst
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/docs/source/ocsmesh.mesh.rst
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/docs/source/ocsmesh.size_function.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/docs/source/ocsmesh.utilities.rst
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/docs/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.386125 ocsmesh-1.3.4/ocsmesh/
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.386125 ocsmesh-1.3.4/ocsmesh/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/cli/mesh_upgrader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13271 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/cli/remesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/cli/remesh_by_shape_factor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23645 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/cli/subset_n_combine.py
--rw-r--r--   0 runner    (1001) docker     (123)    17544 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/crs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.390125 ocsmesh-1.3.4/ocsmesh/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/features/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/features/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/features/contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/features/linefeature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/features/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/figures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.390125 ocsmesh-1.3.4/ocsmesh/geom/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/geom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/geom/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    26034 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/geom/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/geom/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/geom/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/geom/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/geom/shapely.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.390125 ocsmesh-1.3.4/ocsmesh/hfun/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/hfun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/hfun/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    81400 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/hfun/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/hfun/hfun.py
--rw-r--r--   0 runner    (1001) docker     (123)    22004 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/hfun/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    59651 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/hfun/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)    15388 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/interp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.390125 ocsmesh-1.3.4/ocsmesh/mesh/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/mesh/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    74313 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/mesh/mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.390125 ocsmesh-1.3.4/ocsmesh/mesh/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/mesh/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/mesh/parsers/grd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/mesh/parsers/sms2dm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.390125 ocsmesh-1.3.4/ocsmesh/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/ops/combine_geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/ops/combine_hfun.py
--rw-r--r--   0 runner    (1001) docker     (123)    64867 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)    68014 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.386125 ocsmesh-1.3.4/ocsmesh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10967 2023-06-22 19:24:45.000000 ocsmesh-1.3.4/ocsmesh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-22 19:24:45.000000 ocsmesh-1.3.4/ocsmesh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:24:45.000000 ocsmesh-1.3.4/ocsmesh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-22 19:24:45.000000 ocsmesh-1.3.4/ocsmesh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-22 19:24:45.000000 ocsmesh-1.3.4/ocsmesh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-22 19:24:45.000000 ocsmesh-1.3.4/ocsmesh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 19:24:45.394126 ocsmesh-1.3.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3082 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.378125 ocsmesh-1.3.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.394126 ocsmesh-1.3.4/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/tests/api/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/tests/api/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    13728 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/tests/api/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/tests/api/geom.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31570 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/tests/api/hfun.py
--rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/tests/api/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    17159 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/tests/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.394126 ocsmesh-1.3.4/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/tests/cli/build_geom.sh
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/tests/cli/build_hfun.sh
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/tests/cli/remesh_by_dem.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:44:06.533075 ocsmesh-1.3.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:44:06.501073 ocsmesh-1.3.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:44:06.509073 ocsmesh-1.3.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/.github/workflows/documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/.github/workflows/functional_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/.github/workflows/functional_test_2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10967 2023-08-02 17:44:06.533075 ocsmesh-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:44:06.513074 ocsmesh-1.3.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)  2851126 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/docs/noaa_33879_DS1.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:44:06.517074 ocsmesh-1.3.5/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/docs/source/ocsmesh.command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/docs/source/ocsmesh.geometry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/docs/source/ocsmesh.mesh.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/docs/source/ocsmesh.size_function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/docs/source/ocsmesh.utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/docs/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:44:06.521074 ocsmesh-1.3.5/ocsmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:44:06.525074 ocsmesh-1.3.5/ocsmesh/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/cli/mesh_upgrader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13271 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/cli/remesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/cli/remesh_by_shape_factor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23645 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/cli/subset_n_combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/crs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:44:06.525074 ocsmesh-1.3.5/ocsmesh/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/features/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/features/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/features/contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/features/linefeature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/features/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/figures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:44:06.529075 ocsmesh-1.3.5/ocsmesh/geom/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/geom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/geom/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26034 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/geom/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/geom/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/geom/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/geom/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/geom/shapely.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:44:06.529075 ocsmesh-1.3.5/ocsmesh/hfun/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/hfun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/hfun/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81400 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/hfun/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/hfun/hfun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22016 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/hfun/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59651 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/hfun/raster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:44:06.533075 ocsmesh-1.3.5/ocsmesh/mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/mesh/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74313 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/mesh/mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:44:06.533075 ocsmesh-1.3.5/ocsmesh/mesh/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/mesh/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/mesh/parsers/grd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/mesh/parsers/sms2dm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:44:06.533075 ocsmesh-1.3.5/ocsmesh/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/ops/combine_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/ops/combine_hfun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64867 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68014 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/ocsmesh/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:44:06.521074 ocsmesh-1.3.5/ocsmesh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10967 2023-08-02 17:44:06.000000 ocsmesh-1.3.5/ocsmesh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-08-02 17:44:06.000000 ocsmesh-1.3.5/ocsmesh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:44:06.000000 ocsmesh-1.3.5/ocsmesh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-02 17:44:06.000000 ocsmesh-1.3.5/ocsmesh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-02 17:44:06.000000 ocsmesh-1.3.5/ocsmesh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 17:44:06.000000 ocsmesh-1.3.5/ocsmesh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 17:44:06.537075 ocsmesh-1.3.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3082 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:44:06.505073 ocsmesh-1.3.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:44:06.533075 ocsmesh-1.3.5/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/tests/api/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/tests/api/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13728 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/tests/api/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/tests/api/geom.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31570 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/tests/api/hfun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/tests/api/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17159 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/tests/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:44:06.533075 ocsmesh-1.3.5/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/tests/cli/build_geom.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/tests/cli/build_hfun.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-02 17:43:50.000000 ocsmesh-1.3.5/tests/cli/remesh_by_dem.sh
```

### Comparing `ocsmesh-1.3.4/.github/workflows/documentation.yml` & `ocsmesh-1.3.5/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/.github/workflows/functional_test.yml` & `ocsmesh-1.3.5/.github/workflows/functional_test.yml`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/.github/workflows/functional_test_2.yml` & `ocsmesh-1.3.5/.github/workflows/functional_test_2.yml`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/.github/workflows/pylint.yml` & `ocsmesh-1.3.5/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/.github/workflows/release.yml` & `ocsmesh-1.3.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/.gitignore` & `ocsmesh-1.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/.pylintrc` & `ocsmesh-1.3.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/LICENSE` & `ocsmesh-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/PKG-INFO` & `ocsmesh-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocsmesh
-Version: 1.3.4
+Version: 1.3.5
 Summary: Package to generate computational unstructured meshes from planetary modeling.
 Author-email: Jaime R Calzada <jreniel@gmail.com>, Soroosh Mani <soroosh.mani@noaa.gov>
 Maintainer-email: Soroosh Mani <soroosh.mani@noaa.gov>
 License: Creative Commons Legal Code
         
         CC0 1.0 Universal
```

### Comparing `ocsmesh-1.3.4/README.md` & `ocsmesh-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/docs/Makefile` & `ocsmesh-1.3.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/docs/make.bat` & `ocsmesh-1.3.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/docs/noaa_33879_DS1.pdf` & `ocsmesh-1.3.5/docs/noaa_33879_DS1.pdf`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/docs/source/conf.py` & `ocsmesh-1.3.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/__init__.py` & `ocsmesh-1.3.5/ocsmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/__main__.py` & `ocsmesh-1.3.5/ocsmesh/__main__.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/cli/cli.py` & `ocsmesh-1.3.5/ocsmesh/cli/cli.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/cli/mesh_upgrader.py` & `ocsmesh-1.3.5/ocsmesh/cli/mesh_upgrader.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/cli/remesh.py` & `ocsmesh-1.3.5/ocsmesh/cli/remesh.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/cli/remesh_by_shape_factor.py` & `ocsmesh-1.3.5/ocsmesh/cli/remesh_by_shape_factor.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/cli/subset_n_combine.py` & `ocsmesh-1.3.5/ocsmesh/cli/subset_n_combine.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/driver.py` & `ocsmesh-1.3.5/ocsmesh/driver.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/features/channel.py` & `ocsmesh-1.3.5/ocsmesh/features/channel.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/features/constraint.py` & `ocsmesh-1.3.5/ocsmesh/features/constraint.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/features/contour.py` & `ocsmesh-1.3.5/ocsmesh/features/contour.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/features/linefeature.py` & `ocsmesh-1.3.5/ocsmesh/features/linefeature.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/features/patch.py` & `ocsmesh-1.3.5/ocsmesh/features/patch.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/figures.py` & `ocsmesh-1.3.5/ocsmesh/figures.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/geom/base.py` & `ocsmesh-1.3.5/ocsmesh/geom/base.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/geom/collector.py` & `ocsmesh-1.3.5/ocsmesh/geom/collector.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/geom/geom.py` & `ocsmesh-1.3.5/ocsmesh/geom/geom.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/geom/mesh.py` & `ocsmesh-1.3.5/ocsmesh/geom/mesh.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/geom/raster.py` & `ocsmesh-1.3.5/ocsmesh/geom/raster.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/geom/shapely.py` & `ocsmesh-1.3.5/ocsmesh/geom/shapely.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/hfun/base.py` & `ocsmesh-1.3.5/ocsmesh/hfun/base.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/hfun/collector.py` & `ocsmesh-1.3.5/ocsmesh/hfun/collector.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/hfun/hfun.py` & `ocsmesh-1.3.5/ocsmesh/hfun/hfun.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/hfun/mesh.py` & `ocsmesh-1.3.5/ocsmesh/hfun/mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,17 +272,17 @@
             raise ValueError('Argument target_size must be specified if no '
                              'global hmin has been set.')
         if target_size <= 0:
             raise ValueError("Argument target_size must be greater than zero.")
 
         # For expansion_rate
         if expansion_rate is not None:
-            exteriors = [ply.exterior for ply in multipolygon]
+            exteriors = [ply.exterior for ply in multipolygon.geoms]
             interiors = [
-                inter for ply in multipolygon for inter in ply.interiors]
+                inter for ply in multipolygon.geoms for inter in ply.interiors]
 
             features = MultiLineString([*exteriors, *interiors])
             # pylint: disable=E1123, E1125
             self.add_feature(
                 feature=features,
                 expansion_rate=expansion_rate,
                 target_size=target_size,
```

### Comparing `ocsmesh-1.3.4/ocsmesh/hfun/raster.py` & `ocsmesh-1.3.5/ocsmesh/hfun/raster.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/mesh/base.py` & `ocsmesh-1.3.5/ocsmesh/mesh/base.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/mesh/mesh.py` & `ocsmesh-1.3.5/ocsmesh/mesh/mesh.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/mesh/parsers/grd.py` & `ocsmesh-1.3.5/ocsmesh/mesh/parsers/grd.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/mesh/parsers/sms2dm.py` & `ocsmesh-1.3.5/ocsmesh/mesh/parsers/sms2dm.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/ops/combine_geom.py` & `ocsmesh-1.3.5/ocsmesh/ops/combine_geom.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/ops/combine_hfun.py` & `ocsmesh-1.3.5/ocsmesh/ops/combine_hfun.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/raster.py` & `ocsmesh-1.3.5/ocsmesh/raster.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh/utils.py` & `ocsmesh-1.3.5/ocsmesh/utils.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/ocsmesh.egg-info/PKG-INFO` & `ocsmesh-1.3.5/ocsmesh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocsmesh
-Version: 1.3.4
+Version: 1.3.5
 Summary: Package to generate computational unstructured meshes from planetary modeling.
 Author-email: Jaime R Calzada <jreniel@gmail.com>, Soroosh Mani <soroosh.mani@noaa.gov>
 Maintainer-email: Soroosh Mani <soroosh.mani@noaa.gov>
 License: Creative Commons Legal Code
         
         CC0 1.0 Universal
```

### Comparing `ocsmesh-1.3.4/ocsmesh.egg-info/SOURCES.txt` & `ocsmesh-1.3.5/ocsmesh.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,20 +21,17 @@
 docs/source/ocsmesh.geometry.rst
 docs/source/ocsmesh.mesh.rst
 docs/source/ocsmesh.size_function.rst
 docs/source/ocsmesh.utilities.rst
 docs/source/readme.rst
 ocsmesh/__init__.py
 ocsmesh/__main__.py
-ocsmesh/cmd.py
 ocsmesh/crs.py
-ocsmesh/db.py
 ocsmesh/driver.py
 ocsmesh/figures.py
-ocsmesh/interp.py
 ocsmesh/raster.py
 ocsmesh/utils.py
 ocsmesh.egg-info/PKG-INFO
 ocsmesh.egg-info/SOURCES.txt
 ocsmesh.egg-info/dependency_links.txt
 ocsmesh.egg-info/entry_points.txt
 ocsmesh.egg-info/requires.txt
```

### Comparing `ocsmesh-1.3.4/pyproject.toml` & `ocsmesh-1.3.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -17,29 +17,28 @@
     {name = "Soroosh Mani", email = "soroosh.mani@noaa.gov"}
 ]
 description = "Package to generate computational unstructured meshes from planetary modeling."
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = '>=3.9' # 3.8 not supported by scipy
 dependencies = [
-    "colored-traceback", "fiona", "geoalchemy2", "geopandas",
+    "colored-traceback", "fiona", "geopandas",
     "jigsawpy", "matplotlib", "netCDF4", "numba",
     "numpy>=1.21", # introduce npt.NDArray
-    "pyarrow", "rtree", "pyproj>=3.0", "rasterio", "requests", "scipy",
-    "shapely", "tqdm", "typing_extensions", "utm",
+    "pyarrow", "rtree", "pyproj>=3.0", "rasterio", "scipy",
+    "shapely", "typing_extensions", "utm",
     ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://noaa-ocs-modeling.github.io/OCSMesh/"
 Source = "https://github.com/noaa-ocs-modeling/OCSMesh/"
 
 [project.scripts]
 ocsmesh = "ocsmesh.__main__:main"
-interp = "ocsmesh.interp:main"
 
 [project.optional-dependencies]
 testing = ['pylint>=2.14']
 documentation = [
     'sphinx < 7.0.0', # due to sphinx_rtd_theme support
     'sphinx-rtd-theme', 'sphinx-argparse',
     'mistune==0.8.4', 'm2r2', 'numpydoc'
```

### Comparing `ocsmesh-1.3.4/setup.py` & `ocsmesh-1.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/tests/api/common.py` & `ocsmesh-1.3.5/tests/api/common.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/tests/api/driver.py` & `ocsmesh-1.3.5/tests/api/driver.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import tempfile
 import warnings
 
 from jigsawpy import jigsaw_msh_t
 import geopandas as gpd
 import numpy as np
 import rasterio as rio
-import requests
 from shapely import geometry
 
 import ocsmesh
 
 from tests.api.common import (
     topo_2rast_1mesh,
 )
```

### Comparing `ocsmesh-1.3.4/tests/api/features.py` & `ocsmesh-1.3.5/tests/api/features.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/tests/api/geom.py` & `ocsmesh-1.3.5/tests/api/geom.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import tempfile
 import warnings
 
 from jigsawpy import jigsaw_msh_t
 import geopandas as gpd
 import numpy as np
 import rasterio as rio
-import requests
 from shapely import geometry
 
 import ocsmesh
 
 from tests.api.common import (
     topo_2rast_1mesh,
 )
```

### Comparing `ocsmesh-1.3.4/tests/api/hfun.py` & `ocsmesh-1.3.5/tests/api/hfun.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/tests/api/mesh.py` & `ocsmesh-1.3.5/tests/api/mesh.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.4/tests/api/utils.py` & `ocsmesh-1.3.5/tests/api/utils.py`

 * *Files identical despite different names*


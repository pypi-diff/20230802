# Comparing `tmp/dragonfly-schema-1.9.3.tar.gz` & `tmp/dragonfly-schema-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dragonfly-schema-1.9.3.tar", last modified: Thu Jul 27 07:19:41 2023, max compression
+gzip compressed data, was "dist/dragonfly-schema-1.9.4.tar", last modified: Tue Aug  1 23:49:29 2023, max compression
```

## Comparing `dragonfly-schema-1.9.3.tar` & `dragonfly-schema-1.9.4.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:19:41.000000 dragonfly-schema-1.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:19:41.000000 dragonfly-schema-1.9.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:19:41.000000 dragonfly-schema-1.9.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/.github/workflows/dependency-release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-27 07:19:41.000000 dragonfly-schema-1.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:19:41.000000 dragonfly-schema-1.9.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/docs/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/docs/model.html
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:19:41.000000 dragonfly-schema-1.9.3/dragonfly_schema/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/dragonfly_schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:19:41.000000 dragonfly-schema-1.9.3/dragonfly_schema/energy/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/dragonfly_schema/energy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/dragonfly_schema/energy/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/dragonfly_schema/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:19:41.000000 dragonfly-schema-1.9.3/dragonfly_schema/radiance/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/dragonfly_schema/radiance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/dragonfly_schema/radiance/gridpar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/dragonfly_schema/radiance/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/dragonfly_schema/roof.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/dragonfly_schema/shading_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/dragonfly_schema/skylight_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/dragonfly_schema/window_parameter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:19:41.000000 dragonfly-schema-1.9.3/dragonfly_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-27 07:19:41.000000 dragonfly-schema-1.9.3/dragonfly_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-27 07:19:41.000000 dragonfly-schema-1.9.3/dragonfly_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 07:19:41.000000 dragonfly-schema-1.9.3/dragonfly_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 07:19:41.000000 dragonfly-schema-1.9.3/dragonfly_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 07:19:41.000000 dragonfly-schema-1.9.3/dragonfly_schema.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:19:41.000000 dragonfly-schema-1.9.3/samples/
--rw-r--r--   0 runner    (1001) docker     (123)    22598 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/samples/building_simple.json
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/samples/context_shade_two_tree_canopy.json
--rw-r--r--   0 runner    (1001) docker     (123)    90404 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/samples/model_complete_simple.dfjson
--rw-r--r--   0 runner    (1001) docker     (123)   112149 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/samples/model_with_doors_skylights.dfjson
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/samples/room2d_simple.json
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/samples/shading_par_extruded_border.json
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/samples/shading_par_louvers_by_count.json
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/samples/shading_par_louvers_by_distance.json
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/samples/shading_par_overhang.json
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/samples/story_air_boundary.json
--rw-r--r--   0 runner    (1001) docker     (123)     9468 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/samples/story_simple.json
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/samples/window_par_detailed_rectangular_windows.json
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/samples/window_par_detailed_windows.json
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/samples/window_par_repeating_window_ratio.json
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/samples/window_par_repeating_window_width_height.json
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/samples/window_par_simple_window_ratio.json
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/samples/window_par_single_window.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:19:41.000000 dragonfly-schema-1.9.3/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/scripts/export_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     9703 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/scripts/sample_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/scripts/sample_shading_par.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/scripts/sample_window_par.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-27 07:19:41.000000 dragonfly-schema-1.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:19:41.000000 dragonfly-schema-1.9.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/tests/test_openapi_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/tests/test_shading_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-27 07:18:17.000000 dragonfly-schema-1.9.3/tests/test_window_parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:49:29.000000 dragonfly-schema-1.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:49:29.000000 dragonfly-schema-1.9.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:49:29.000000 dragonfly-schema-1.9.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/.github/workflows/dependency-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-08-01 23:49:29.000000 dragonfly-schema-1.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:49:29.000000 dragonfly-schema-1.9.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/docs/model.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:49:29.000000 dragonfly-schema-1.9.4/dragonfly_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/dragonfly_schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:49:29.000000 dragonfly-schema-1.9.4/dragonfly_schema/energy/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/dragonfly_schema/energy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/dragonfly_schema/energy/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/dragonfly_schema/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:49:29.000000 dragonfly-schema-1.9.4/dragonfly_schema/radiance/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/dragonfly_schema/radiance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/dragonfly_schema/radiance/gridpar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/dragonfly_schema/radiance/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/dragonfly_schema/roof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/dragonfly_schema/shading_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/dragonfly_schema/skylight_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/dragonfly_schema/window_parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:49:29.000000 dragonfly-schema-1.9.4/dragonfly_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-08-01 23:49:29.000000 dragonfly-schema-1.9.4/dragonfly_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-08-01 23:49:29.000000 dragonfly-schema-1.9.4/dragonfly_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 23:49:29.000000 dragonfly-schema-1.9.4/dragonfly_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 23:49:29.000000 dragonfly-schema-1.9.4/dragonfly_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 23:49:29.000000 dragonfly-schema-1.9.4/dragonfly_schema.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:49:29.000000 dragonfly-schema-1.9.4/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)    22598 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/samples/building_simple.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/samples/context_shade_two_tree_canopy.json
+-rw-r--r--   0 runner    (1001) docker     (123)    90404 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/samples/model_complete_simple.dfjson
+-rw-r--r--   0 runner    (1001) docker     (123)   112149 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/samples/model_with_doors_skylights.dfjson
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/samples/room2d_simple.json
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/samples/shading_par_extruded_border.json
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/samples/shading_par_louvers_by_count.json
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/samples/shading_par_louvers_by_distance.json
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/samples/shading_par_overhang.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/samples/story_air_boundary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9468 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/samples/story_simple.json
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/samples/window_par_detailed_rectangular_windows.json
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/samples/window_par_detailed_windows.json
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/samples/window_par_repeating_window_ratio.json
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/samples/window_par_repeating_window_width_height.json
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/samples/window_par_simple_window_ratio.json
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/samples/window_par_single_window.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:49:29.000000 dragonfly-schema-1.9.4/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/scripts/export_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9703 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/scripts/sample_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/scripts/sample_shading_par.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/scripts/sample_window_par.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-01 23:49:29.000000 dragonfly-schema-1.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:49:29.000000 dragonfly-schema-1.9.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/tests/test_openapi_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/tests/test_shading_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-08-01 23:48:12.000000 dragonfly-schema-1.9.4/tests/test_window_parameter.py
```

### Comparing `dragonfly-schema-1.9.3/.github/workflows/ci.yaml` & `dragonfly-schema-1.9.4/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/.github/workflows/dependency-release.yaml` & `dragonfly-schema-1.9.4/.github/workflows/dependency-release.yaml`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/.releaserc.json` & `dragonfly-schema-1.9.4/.releaserc.json`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/LICENSE` & `dragonfly-schema-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/PKG-INFO` & `dragonfly-schema-1.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragonfly-schema
-Version: 1.9.3
+Version: 1.9.4
 Summary: Dragonfly Data-Model Objects
 Home-page: https://github.com/ladybug-tools/dragonfly-schema
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
```

### Comparing `dragonfly-schema-1.9.3/README.md` & `dragonfly-schema-1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/docs/index.html` & `dragonfly-schema-1.9.4/docs/index.html`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/docs/model.html` & `dragonfly-schema-1.9.4/docs/model.html`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/docs.py` & `dragonfly-schema-1.9.4/docs.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/dragonfly_schema/energy/properties.py` & `dragonfly-schema-1.9.4/dragonfly_schema/energy/properties.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/dragonfly_schema/model.py` & `dragonfly-schema-1.9.4/dragonfly_schema/model.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/dragonfly_schema/radiance/gridpar.py` & `dragonfly-schema-1.9.4/dragonfly_schema/radiance/gridpar.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/dragonfly_schema/radiance/properties.py` & `dragonfly-schema-1.9.4/dragonfly_schema/radiance/properties.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/dragonfly_schema/roof.py` & `dragonfly-schema-1.9.4/dragonfly_schema/roof.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/dragonfly_schema/shading_parameter.py` & `dragonfly-schema-1.9.4/dragonfly_schema/shading_parameter.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/dragonfly_schema/skylight_parameter.py` & `dragonfly-schema-1.9.4/dragonfly_schema/skylight_parameter.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/dragonfly_schema/window_parameter.py` & `dragonfly-schema-1.9.4/dragonfly_schema/window_parameter.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/dragonfly_schema.egg-info/PKG-INFO` & `dragonfly-schema-1.9.4/dragonfly_schema.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragonfly-schema
-Version: 1.9.3
+Version: 1.9.4
 Summary: Dragonfly Data-Model Objects
 Home-page: https://github.com/ladybug-tools/dragonfly-schema
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
```

### Comparing `dragonfly-schema-1.9.3/dragonfly_schema.egg-info/SOURCES.txt` & `dragonfly-schema-1.9.4/dragonfly_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/samples/building_simple.json` & `dragonfly-schema-1.9.4/samples/building_simple.json`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/samples/context_shade_two_tree_canopy.json` & `dragonfly-schema-1.9.4/samples/context_shade_two_tree_canopy.json`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/samples/model_complete_simple.dfjson` & `dragonfly-schema-1.9.4/samples/model_complete_simple.dfjson`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/samples/model_with_doors_skylights.dfjson` & `dragonfly-schema-1.9.4/samples/model_with_doors_skylights.dfjson`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/samples/room2d_simple.json` & `dragonfly-schema-1.9.4/samples/room2d_simple.json`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/samples/story_air_boundary.json` & `dragonfly-schema-1.9.4/samples/story_air_boundary.json`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/samples/story_simple.json` & `dragonfly-schema-1.9.4/samples/story_simple.json`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/samples/window_par_detailed_windows.json` & `dragonfly-schema-1.9.4/samples/window_par_detailed_windows.json`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/scripts/export_samples.py` & `dragonfly-schema-1.9.4/scripts/export_samples.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/scripts/sample_model.py` & `dragonfly-schema-1.9.4/scripts/sample_model.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/scripts/sample_shading_par.py` & `dragonfly-schema-1.9.4/scripts/sample_shading_par.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/scripts/sample_window_par.py` & `dragonfly-schema-1.9.4/scripts/sample_window_par.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/setup.py` & `dragonfly-schema-1.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/tests/test_model.py` & `dragonfly-schema-1.9.4/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/tests/test_shading_parameter.py` & `dragonfly-schema-1.9.4/tests/test_shading_parameter.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.3/tests/test_window_parameter.py` & `dragonfly-schema-1.9.4/tests/test_window_parameter.py`

 * *Files identical despite different names*


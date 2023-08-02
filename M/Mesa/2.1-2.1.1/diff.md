# Comparing `tmp/Mesa-2.1.tar.gz` & `tmp/Mesa-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mesa-2.1.tar", last modified: Sun Jul 23 12:54:25 2023, max compression
+gzip compressed data, was "Mesa-2.1.1.tar", last modified: Wed Aug  2 04:25:30 2023, max compression
```

## Comparing `Mesa-2.1.tar` & `Mesa-2.1.1.tar`

### file list

```diff
@@ -1,218 +1,218 @@
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.744420 Mesa-2.1/
--rw-r--r--   0 jk         (501) staff       (20)    39212 2023-07-23 12:49:52.000000 Mesa-2.1/HISTORY.rst
--rw-r--r--   0 jk         (501) staff       (20)      572 2023-05-15 02:11:02.000000 Mesa-2.1/LICENSE
--rw-r--r--   0 jk         (501) staff       (20)      441 2023-04-25 15:49:54.000000 Mesa-2.1/MANIFEST.in
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.319167 Mesa-2.1/Mesa.egg-info/
--rw-r--r--   0 jk         (501) staff       (20)     6663 2023-07-23 12:54:25.000000 Mesa-2.1/Mesa.egg-info/PKG-INFO
--rw-r--r--   0 jk         (501) staff       (20)    12238 2023-07-23 12:54:25.000000 Mesa-2.1/Mesa.egg-info/SOURCES.txt
--rw-r--r--   0 jk         (501) staff       (20)        1 2023-07-23 12:54:25.000000 Mesa-2.1/Mesa.egg-info/dependency_links.txt
--rw-r--r--   0 jk         (501) staff       (20)       39 2023-07-23 12:54:25.000000 Mesa-2.1/Mesa.egg-info/entry_points.txt
--rw-r--r--   0 jk         (501) staff       (20)        1 2023-03-10 00:33:58.000000 Mesa-2.1/Mesa.egg-info/not-zip-safe
--rw-r--r--   0 jk         (501) staff       (20)      199 2023-07-23 12:54:25.000000 Mesa-2.1/Mesa.egg-info/requires.txt
--rw-r--r--   0 jk         (501) staff       (20)       11 2023-07-23 12:54:25.000000 Mesa-2.1/Mesa.egg-info/top_level.txt
--rw-r--r--   0 jk         (501) staff       (20)     6663 2023-07-23 12:54:25.743772 Mesa-2.1/PKG-INFO
--rw-r--r--   0 jk         (501) staff       (20)     5652 2023-04-25 15:49:54.000000 Mesa-2.1/README.rst
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.332900 Mesa-2.1/mesa/
--rw-r--r--   0 jk         (501) staff       (20)      682 2023-07-23 12:49:52.000000 Mesa-2.1/mesa/__init__.py
--rw-r--r--   0 jk         (501) staff       (20)     1081 2023-04-25 15:49:54.000000 Mesa-2.1/mesa/agent.py
--rw-r--r--   0 jk         (501) staff       (20)     6120 2023-07-17 03:55:09.000000 Mesa-2.1/mesa/batchrunner.py
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.335357 Mesa-2.1/mesa/cookiecutter-mesa/
--rw-r--r--   0 jk         (501) staff       (20)      337 2023-03-06 14:25:55.000000 Mesa-2.1/mesa/cookiecutter-mesa/cookiecutter.json
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.339124 Mesa-2.1/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/
--rw-r--r--   0 jk         (501) staff       (20)       80 2023-03-06 14:25:55.000000 Mesa-2.1/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/README.md
--rw-r--r--   0 jk         (501) staff       (20)       74 2023-03-06 14:25:55.000000 Mesa-2.1/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/run.py
--rw-r--r--   0 jk         (501) staff       (20)      214 2023-04-25 15:49:54.000000 Mesa-2.1/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/setup.py
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.342468 Mesa-2.1/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/{{cookiecutter.snake}}/
--rw-r--r--   0 jk         (501) staff       (20)        0 2023-03-06 14:25:55.000000 Mesa-2.1/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/{{cookiecutter.snake}}/__init__.py
--rw-r--r--   0 jk         (501) staff       (20)     1842 2023-04-25 15:49:54.000000 Mesa-2.1/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/{{cookiecutter.snake}}/model.py
--rw-r--r--   0 jk         (501) staff       (20)      823 2023-04-25 15:49:54.000000 Mesa-2.1/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/{{cookiecutter.snake}}/server.py
--rw-r--r--   0 jk         (501) staff       (20)    11512 2023-05-28 15:25:59.000000 Mesa-2.1/mesa/datacollection.py
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.344952 Mesa-2.1/mesa/experimental/
--rw-r--r--   0 jk         (501) staff       (20)       55 2023-07-21 03:13:23.000000 Mesa-2.1/mesa/experimental/__init__.py
--rw-r--r--   0 jk         (501) staff       (20)     6456 2023-07-21 03:13:23.000000 Mesa-2.1/mesa/experimental/jupyter_viz.py
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.346970 Mesa-2.1/mesa/flat/
--rw-r--r--   0 jk         (501) staff       (20)      218 2023-04-25 15:49:54.000000 Mesa-2.1/mesa/flat/__init__.py
--rw-r--r--   0 jk         (501) staff       (20)      298 2023-04-25 15:49:54.000000 Mesa-2.1/mesa/flat/visualization.py
--rw-r--r--   0 jk         (501) staff       (20)     1468 2023-04-25 15:49:54.000000 Mesa-2.1/mesa/main.py
--rw-r--r--   0 jk         (501) staff       (20)     2708 2023-05-28 15:25:59.000000 Mesa-2.1/mesa/model.py
--rw-r--r--   0 jk         (501) staff       (20)    38769 2023-07-17 03:55:09.000000 Mesa-2.1/mesa/space.py
--rw-r--r--   0 jk         (501) staff       (20)    10415 2023-07-17 03:55:09.000000 Mesa-2.1/mesa/time.py
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.352789 Mesa-2.1/mesa/visualization/
--rw-r--r--   0 jk         (501) staff       (20)    14730 2023-07-17 03:55:09.000000 Mesa-2.1/mesa/visualization/ModularVisualization.py
--rw-r--r--   0 jk         (501) staff       (20)     3792 2023-04-25 15:49:54.000000 Mesa-2.1/mesa/visualization/TextVisualization.py
--rw-r--r--   0 jk         (501) staff       (20)     4127 2023-07-17 03:55:09.000000 Mesa-2.1/mesa/visualization/UserParam.py
--rw-r--r--   0 jk         (501) staff       (20)      268 2023-04-25 15:49:54.000000 Mesa-2.1/mesa/visualization/__init__.py
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.364117 Mesa-2.1/mesa/visualization/modules/
--rw-r--r--   0 jk         (501) staff       (20)     3736 2023-07-17 03:55:09.000000 Mesa-2.1/mesa/visualization/modules/BarChartVisualization.py
--rw-r--r--   0 jk         (501) staff       (20)     4742 2023-04-25 15:49:54.000000 Mesa-2.1/mesa/visualization/modules/CanvasGridVisualization.py
--rw-r--r--   0 jk         (501) staff       (20)     3144 2023-04-25 15:49:54.000000 Mesa-2.1/mesa/visualization/modules/ChartVisualization.py
--rw-r--r--   0 jk         (501) staff       (20)     3541 2023-04-25 15:49:54.000000 Mesa-2.1/mesa/visualization/modules/HexGridVisualization.py
--rw-r--r--   0 jk         (501) staff       (20)      838 2023-04-25 15:49:54.000000 Mesa-2.1/mesa/visualization/modules/NetworkVisualization.py
--rw-r--r--   0 jk         (501) staff       (20)     2450 2023-04-25 15:49:54.000000 Mesa-2.1/mesa/visualization/modules/PieChartVisualization.py
--rw-r--r--   0 jk         (501) staff       (20)      726 2023-04-25 15:49:54.000000 Mesa-2.1/mesa/visualization/modules/__init__.py
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.365283 Mesa-2.1/mesa/visualization/templates/
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.366566 Mesa-2.1/mesa/visualization/templates/css/
--rw-r--r--   0 jk         (501) staff       (20)      377 2023-04-25 15:49:54.000000 Mesa-2.1/mesa/visualization/templates/css/visualization.css
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.286666 Mesa-2.1/mesa/visualization/templates/external/
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.286205 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.466330 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/
--rw-r--r--   0 jk         (501) staff       (20)    72279 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.css
--rw-r--r--   0 jk         (501) staff       (20)   201507 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.css.map
--rw-r--r--   0 jk         (501) staff       (20)    52805 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.min.css
--rw-r--r--   0 jk         (501) staff       (20)   122306 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.min.css.map
--rw-r--r--   0 jk         (501) staff       (20)    72353 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.rtl.css
--rw-r--r--   0 jk         (501) staff       (20)   201511 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.rtl.css.map
--rw-r--r--   0 jk         (501) staff       (20)    52880 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.rtl.min.css
--rw-r--r--   0 jk         (501) staff       (20)   122383 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.rtl.min.css.map
--rw-r--r--   0 jk         (501) staff       (20)     7578 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.css
--rw-r--r--   0 jk         (501) staff       (20)   109619 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.css.map
--rw-r--r--   0 jk         (501) staff       (20)     6120 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.min.css
--rw-r--r--   0 jk         (501) staff       (20)    39730 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.min.css.map
--rw-r--r--   0 jk         (501) staff       (20)     7555 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.rtl.css
--rw-r--r--   0 jk         (501) staff       (20)   109632 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.rtl.css.map
--rw-r--r--   0 jk         (501) staff       (20)     6192 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.rtl.min.css
--rw-r--r--   0 jk         (501) staff       (20)    47717 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.rtl.min.css.map
--rw-r--r--   0 jk         (501) staff       (20)    71560 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.css
--rw-r--r--   0 jk         (501) staff       (20)   192717 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.css.map
--rw-r--r--   0 jk         (501) staff       (20)    53455 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.min.css
--rw-r--r--   0 jk         (501) staff       (20)   111849 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.min.css.map
--rw-r--r--   0 jk         (501) staff       (20)    71427 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.rtl.css
--rw-r--r--   0 jk         (501) staff       (20)   192660 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.rtl.css.map
--rw-r--r--   0 jk         (501) staff       (20)    53383 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.rtl.min.css
--rw-r--r--   0 jk         (501) staff       (20)   111684 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.rtl.min.css.map
--rw-r--r--   0 jk         (501) staff       (20)   205484 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.css
--rw-r--r--   0 jk         (501) staff       (20)   538014 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.css.map
--rw-r--r--   0 jk         (501) staff       (20)   163873 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.min.css
--rw-r--r--   0 jk         (501) staff       (20)   451427 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.min.css.map
--rw-r--r--   0 jk         (501) staff       (20)   205151 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.rtl.css
--rw-r--r--   0 jk         (501) staff       (20)   537928 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.rtl.css.map
--rw-r--r--   0 jk         (501) staff       (20)   163978 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.rtl.min.css
--rw-r--r--   0 jk         (501) staff       (20)   663486 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.rtl.min.css.map
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.512711 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/
--rw-r--r--   0 jk         (501) staff       (20)   209719 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.bundle.js
--rw-r--r--   0 jk         (501) staff       (20)   427637 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.bundle.js.map
--rw-r--r--   0 jk         (501) staff       (20)    78129 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.bundle.min.js
--rw-r--r--   0 jk         (501) staff       (20)   331017 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 jk         (501) staff       (20)   139773 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.esm.js
--rw-r--r--   0 jk         (501) staff       (20)   289576 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.esm.js.map
--rw-r--r--   0 jk         (501) staff       (20)    72614 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.esm.min.js
--rw-r--r--   0 jk         (501) staff       (20)   223558 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.esm.min.js.map
--rw-r--r--   0 jk         (501) staff       (20)   148892 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.js
--rw-r--r--   0 jk         (501) staff       (20)   290776 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.js.map
--rw-r--r--   0 jk         (501) staff       (20)    59219 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.min.js
--rw-r--r--   0 jk         (501) staff       (20)   219918 2023-03-10 00:33:56.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.min.js.map
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.539038 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.544731 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/.github/
--rw-r--r--   0 jk         (501) staff       (20)      451 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/.github/CONTRIBUTING.md
--rw-r--r--   0 jk         (501) staff       (20)      512 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 jk         (501) staff       (20)      747 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 jk         (501) staff       (20)      127 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/.gitignore
--rw-r--r--   0 jk         (501) staff       (20)      103 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/.npmignore
--rw-r--r--   0 jk         (501) staff       (20)       19 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/.npmrc
--rw-r--r--   0 jk         (501) staff       (20)        7 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/.nvmrc
--rw-r--r--   0 jk         (501) staff       (20)      774 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/.sass-lint.yml
--rw-r--r--   0 jk         (501) staff       (20)      108 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/.travis.yml
--rw-r--r--   0 jk         (501) staff       (20)    22936 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/CHANGELOG.md
--rw-r--r--   0 jk         (501) staff       (20)     8974 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/Gruntfile.js
--rw-r--r--   0 jk         (501) staff       (20)     1207 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/LICENSE.md
--rw-r--r--   0 jk         (501) staff       (20)    15619 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/README.md
--rw-r--r--   0 jk         (501) staff       (20)      527 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/bower.json
--rw-r--r--   0 jk         (501) staff       (20)     1087 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/composer.json
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.294844 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dependencies/
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.546102 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dependencies/css/
--rw-r--r--   0 jk         (501) staff       (20)      872 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dependencies/css/highlightjs-github-theme.css
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.552271 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dependencies/js/
--rw-r--r--   0 jk         (501) staff       (20)    44793 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dependencies/js/highlight.min.js
--rw-r--r--   0 jk         (501) staff       (20)    84280 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dependencies/js/jquery.min.js
--rw-r--r--   0 jk         (501) staff       (20)    51351 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dependencies/js/modernizr.js
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.563063 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dist/
--rw-r--r--   0 jk         (501) staff       (20)    71582 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dist/bootstrap-slider.js
--rw-r--r--   0 jk         (501) staff       (20)    38829 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dist/bootstrap-slider.min.js
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.566892 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dist/css/
--rw-r--r--   0 jk         (501) staff       (20)    12347 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dist/css/bootstrap-slider.css
--rw-r--r--   0 jk         (501) staff       (20)    11184 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dist/css/bootstrap-slider.min.css
--rw-r--r--   0 jk         (501) staff       (20)     3510 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/package.json
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.584389 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/scripts/
--rw-r--r--   0 jk         (501) staff       (20)      383 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/scripts/build-preview.sh
--rw-r--r--   0 jk         (501) staff       (20)     1320 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/scripts/release.sh
--rw-r--r--   0 jk         (501) staff       (20)     1246 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/scripts/update-gh-pages.sh
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.297639 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/src/
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.585952 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/src/js/
--rw-r--r--   0 jk         (501) staff       (20)    70254 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/src/js/bootstrap-slider.js
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.605828 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/src/sass/
--rw-r--r--   0 jk         (501) staff       (20)     1033 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/src/sass/_mixins.scss
--rw-r--r--   0 jk         (501) staff       (20)     6652 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/src/sass/_rules.scss
--rw-r--r--   0 jk         (501) staff       (20)      930 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/src/sass/_variables.scss
--rw-r--r--   0 jk         (501) staff       (20)     1638 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/src/sass/bootstrap-slider.scss
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.611435 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/
--rw-r--r--   0 jk         (501) staff       (20)     1130 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/phantom_bind_polyfill.js
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.701203 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/
--rw-r--r--   0 jk         (501) staff       (20)     3442 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/AccessibilitySpec.js
--rw-r--r--   0 jk         (501) staff       (20)     4389 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/AriaValueTextFormatterSpec.js
--rw-r--r--   0 jk         (501) staff       (20)      660 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/AutoRegisterDataProvideSpec.js
--rw-r--r--   0 jk         (501) staff       (20)     1949 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/ConflictingOptionsSpec.js
--rw-r--r--   0 jk         (501) staff       (20)    13555 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/DestroyMethodTests.js
--rw-r--r--   0 jk         (501) staff       (20)    10331 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/DraggingHandlesSpec.js
--rw-r--r--   0 jk         (501) staff       (20)     6587 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/ElementDataAttributesSpec.js
--rw-r--r--   0 jk         (501) staff       (20)    15075 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/EventsSpec.js
--rw-r--r--   0 jk         (501) staff       (20)     1532 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/FocusOptionSpec.js
--rw-r--r--   0 jk         (501) staff       (20)    22847 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/KeyboardSupportSpec.js
--rw-r--r--   0 jk         (501) staff       (20)    20361 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/LockToTicksSpec.js
--rw-r--r--   0 jk         (501) staff       (20)     2248 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/LogarithmicScaleSpec.js
--rw-r--r--   0 jk         (501) staff       (20)     5513 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/LowAndHighTrackSpec.js
--rw-r--r--   0 jk         (501) staff       (20)     2270 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/NamespaceSpec.js
--rw-r--r--   0 jk         (501) staff       (20)     2188 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/OrientationSpec.js
--rw-r--r--   0 jk         (501) staff       (20)    23704 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/PublicMethodsSpec.js
--rw-r--r--   0 jk         (501) staff       (20)     6450 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/RangeHighlightsSpec.js
--rw-r--r--   0 jk         (501) staff       (20)     3402 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/RefreshMethodSpec.js
--rw-r--r--   0 jk         (501) staff       (20)     2131 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/ResizeSpec.js
--rw-r--r--   0 jk         (501) staff       (20)     2519 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/RtlOptionsSpec.js
--rw-r--r--   0 jk         (501) staff       (20)     5305 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/ScrollableBodySpec.js
--rw-r--r--   0 jk         (501) staff       (20)     3085 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/ScrollableContainerSpec.js
--rw-r--r--   0 jk         (501) staff       (20)     1696 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/StepReachMaxValueSpec.js
--rw-r--r--   0 jk         (501) staff       (20)     2712 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/TickClickingBehaviorSpec.js
--rw-r--r--   0 jk         (501) staff       (20)     7767 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/TickLabelSpec.js
--rw-r--r--   0 jk         (501) staff       (20)     7107 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/TickMarksSpec.js
--rw-r--r--   0 jk         (501) staff       (20)    13937 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/TooltipMouseOverOptionSpec.js
--rw-r--r--   0 jk         (501) staff       (20)     5640 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/TooltipPositionOptionSpec.js
--rw-r--r--   0 jk         (501) staff       (20)     2649 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/TooltipSplitOptionSpec.js
--rw-r--r--   0 jk         (501) staff       (20)    18834 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/TouchCapableSpec.js
--rw-r--r--   0 jk         (501) staff       (20)      893 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/offMethodSpec.js
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.703198 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/tpl/
--rw-r--r--   0 jk         (501) staff       (20)     4245 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/tpl/SpecRunner.tpl
--rw-r--r--   0 jk         (501) staff       (20)    44636 2023-03-10 00:33:57.000000 Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/tpl/index.tpl
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.716973 Mesa-2.1/mesa/visualization/templates/js/
--rw-r--r--   0 jk         (501) staff       (20)     4644 2023-04-25 15:49:54.000000 Mesa-2.1/mesa/visualization/templates/js/BarChartModule.js
--rw-r--r--   0 jk         (501) staff       (20)     1610 2023-04-25 15:49:54.000000 Mesa-2.1/mesa/visualization/templates/js/CanvasHexModule.js
--rw-r--r--   0 jk         (501) staff       (20)     1689 2023-04-25 15:49:54.000000 Mesa-2.1/mesa/visualization/templates/js/CanvasModule.js
--rw-r--r--   0 jk         (501) staff       (20)     2204 2023-05-15 02:11:02.000000 Mesa-2.1/mesa/visualization/templates/js/ChartModule.js
--rw-r--r--   0 jk         (501) staff       (20)    12943 2023-04-25 15:49:54.000000 Mesa-2.1/mesa/visualization/templates/js/GridDraw.js
--rw-r--r--   0 jk         (501) staff       (20)     8609 2023-04-25 15:49:54.000000 Mesa-2.1/mesa/visualization/templates/js/HexDraw.js
--rw-r--r--   0 jk         (501) staff       (20)     5295 2023-04-25 15:49:54.000000 Mesa-2.1/mesa/visualization/templates/js/InteractionHandler.js
--rw-r--r--   0 jk         (501) staff       (20)     3002 2023-04-25 15:49:54.000000 Mesa-2.1/mesa/visualization/templates/js/NetworkModule_d3.js
--rw-r--r--   0 jk         (501) staff       (20)     2826 2023-04-25 15:49:54.000000 Mesa-2.1/mesa/visualization/templates/js/PieChartModule.js
--rw-r--r--   0 jk         (501) staff       (20)      327 2023-04-25 15:49:54.000000 Mesa-2.1/mesa/visualization/templates/js/TextModule.js
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.721713 Mesa-2.1/mesa/visualization/templates/js/external/
--rw-r--r--   0 jk         (501) staff       (20)   193884 2023-03-10 00:33:58.000000 Mesa-2.1/mesa/visualization/templates/js/external/chart-3.6.1.min.js
--rw-r--r--   0 jk         (501) staff       (20)   277072 2023-03-10 00:33:58.000000 Mesa-2.1/mesa/visualization/templates/js/external/d3-7.4.3.min.js
--rw-r--r--   0 jk         (501) staff       (20)    10100 2023-05-15 02:11:02.000000 Mesa-2.1/mesa/visualization/templates/js/runcontrol.js
--rw-r--r--   0 jk         (501) staff       (20)     4546 2023-04-25 15:49:54.000000 Mesa-2.1/mesa/visualization/templates/modular_template.html
--rw-r--r--   0 jk         (501) staff       (20)     1895 2023-07-17 03:55:09.000000 Mesa-2.1/pyproject.toml
--rw-r--r--   0 jk         (501) staff       (20)       38 2023-07-23 12:54:25.744590 Mesa-2.1/setup.cfg
--rw-r--r--   0 jk         (501) staff       (20)     5264 2023-07-21 03:13:23.000000 Mesa-2.1/setup.py
-drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-07-23 12:54:25.742442 Mesa-2.1/tests/
--rw-r--r--   0 jk         (501) staff       (20)        0 2023-03-06 14:25:55.000000 Mesa-2.1/tests/__init__.py
--rw-r--r--   0 jk         (501) staff       (20)     5092 2023-07-17 03:55:09.000000 Mesa-2.1/tests/test_batch_run.py
--rw-r--r--   0 jk         (501) staff       (20)     8726 2023-05-28 15:25:59.000000 Mesa-2.1/tests/test_datacollector.py
--rw-r--r--   0 jk         (501) staff       (20)     2506 2023-04-25 15:49:54.000000 Mesa-2.1/tests/test_examples.py
--rw-r--r--   0 jk         (501) staff       (20)    15776 2023-07-17 03:55:09.000000 Mesa-2.1/tests/test_grid.py
--rw-r--r--   0 jk         (501) staff       (20)      780 2023-07-17 03:55:09.000000 Mesa-2.1/tests/test_import_namespace.py
--rw-r--r--   0 jk         (501) staff       (20)     2834 2023-04-25 15:49:54.000000 Mesa-2.1/tests/test_lifespan.py
--rw-r--r--   0 jk         (501) staff       (20)      984 2023-04-25 15:49:54.000000 Mesa-2.1/tests/test_main.py
--rw-r--r--   0 jk         (501) staff       (20)      970 2023-04-25 15:49:54.000000 Mesa-2.1/tests/test_model.py
--rw-r--r--   0 jk         (501) staff       (20)      539 2023-04-25 15:49:54.000000 Mesa-2.1/tests/test_scaffold.py
--rw-r--r--   0 jk         (501) staff       (20)    15823 2023-07-17 03:55:09.000000 Mesa-2.1/tests/test_space.py
--rw-r--r--   0 jk         (501) staff       (20)     8717 2023-07-17 03:55:09.000000 Mesa-2.1/tests/test_time.py
--rw-r--r--   0 jk         (501) staff       (20)     1270 2023-04-25 15:49:54.000000 Mesa-2.1/tests/test_tornado.py
--rw-r--r--   0 jk         (501) staff       (20)     1780 2023-07-17 03:55:09.000000 Mesa-2.1/tests/test_usersettableparam.py
--rw-r--r--   0 jk         (501) staff       (20)     3011 2023-07-17 03:55:09.000000 Mesa-2.1/tests/test_visualization.py
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:30.099189 Mesa-2.1.1/
+-rw-r--r--   0 jk         (501) staff       (20)    39651 2023-08-02 04:20:59.000000 Mesa-2.1.1/HISTORY.rst
+-rw-r--r--   0 jk         (501) staff       (20)      572 2023-05-15 02:11:02.000000 Mesa-2.1.1/LICENSE
+-rw-r--r--   0 jk         (501) staff       (20)      441 2023-04-25 15:49:54.000000 Mesa-2.1.1/MANIFEST.in
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:29.663771 Mesa-2.1.1/Mesa.egg-info/
+-rw-r--r--   0 jk         (501) staff       (20)     6645 2023-08-02 04:25:29.000000 Mesa-2.1.1/Mesa.egg-info/PKG-INFO
+-rw-r--r--   0 jk         (501) staff       (20)    12238 2023-08-02 04:25:29.000000 Mesa-2.1.1/Mesa.egg-info/SOURCES.txt
+-rw-r--r--   0 jk         (501) staff       (20)        1 2023-08-02 04:25:29.000000 Mesa-2.1.1/Mesa.egg-info/dependency_links.txt
+-rw-r--r--   0 jk         (501) staff       (20)       39 2023-08-02 04:25:29.000000 Mesa-2.1.1/Mesa.egg-info/entry_points.txt
+-rw-r--r--   0 jk         (501) staff       (20)        1 2023-03-10 00:33:58.000000 Mesa-2.1.1/Mesa.egg-info/not-zip-safe
+-rw-r--r--   0 jk         (501) staff       (20)      199 2023-08-02 04:25:29.000000 Mesa-2.1.1/Mesa.egg-info/requires.txt
+-rw-r--r--   0 jk         (501) staff       (20)       11 2023-08-02 04:25:29.000000 Mesa-2.1.1/Mesa.egg-info/top_level.txt
+-rw-r--r--   0 jk         (501) staff       (20)     6645 2023-08-02 04:25:30.098617 Mesa-2.1.1/PKG-INFO
+-rw-r--r--   0 jk         (501) staff       (20)     5632 2023-08-02 04:20:59.000000 Mesa-2.1.1/README.rst
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:29.672244 Mesa-2.1.1/mesa/
+-rw-r--r--   0 jk         (501) staff       (20)      684 2023-08-02 04:20:59.000000 Mesa-2.1.1/mesa/__init__.py
+-rw-r--r--   0 jk         (501) staff       (20)     1081 2023-04-25 15:49:54.000000 Mesa-2.1.1/mesa/agent.py
+-rw-r--r--   0 jk         (501) staff       (20)     6120 2023-07-17 03:55:09.000000 Mesa-2.1.1/mesa/batchrunner.py
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:29.673587 Mesa-2.1.1/mesa/cookiecutter-mesa/
+-rw-r--r--   0 jk         (501) staff       (20)      337 2023-03-06 14:25:55.000000 Mesa-2.1.1/mesa/cookiecutter-mesa/cookiecutter.json
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:29.679141 Mesa-2.1.1/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/
+-rw-r--r--   0 jk         (501) staff       (20)       80 2023-03-06 14:25:55.000000 Mesa-2.1.1/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/README.md
+-rw-r--r--   0 jk         (501) staff       (20)       74 2023-03-06 14:25:55.000000 Mesa-2.1.1/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/run.py
+-rw-r--r--   0 jk         (501) staff       (20)      214 2023-04-25 15:49:54.000000 Mesa-2.1.1/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/setup.py
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:29.682130 Mesa-2.1.1/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/{{cookiecutter.snake}}/
+-rw-r--r--   0 jk         (501) staff       (20)        0 2023-03-06 14:25:55.000000 Mesa-2.1.1/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/{{cookiecutter.snake}}/__init__.py
+-rw-r--r--   0 jk         (501) staff       (20)     1842 2023-04-25 15:49:54.000000 Mesa-2.1.1/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/{{cookiecutter.snake}}/model.py
+-rw-r--r--   0 jk         (501) staff       (20)      823 2023-04-25 15:49:54.000000 Mesa-2.1.1/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/{{cookiecutter.snake}}/server.py
+-rw-r--r--   0 jk         (501) staff       (20)    11512 2023-05-28 15:25:59.000000 Mesa-2.1.1/mesa/datacollection.py
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:29.684378 Mesa-2.1.1/mesa/experimental/
+-rw-r--r--   0 jk         (501) staff       (20)       55 2023-07-21 03:13:23.000000 Mesa-2.1.1/mesa/experimental/__init__.py
+-rw-r--r--   0 jk         (501) staff       (20)     6426 2023-08-02 04:20:59.000000 Mesa-2.1.1/mesa/experimental/jupyter_viz.py
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:29.687409 Mesa-2.1.1/mesa/flat/
+-rw-r--r--   0 jk         (501) staff       (20)      218 2023-04-25 15:49:54.000000 Mesa-2.1.1/mesa/flat/__init__.py
+-rw-r--r--   0 jk         (501) staff       (20)      298 2023-04-25 15:49:54.000000 Mesa-2.1.1/mesa/flat/visualization.py
+-rw-r--r--   0 jk         (501) staff       (20)     1468 2023-04-25 15:49:54.000000 Mesa-2.1.1/mesa/main.py
+-rw-r--r--   0 jk         (501) staff       (20)     2708 2023-05-28 15:25:59.000000 Mesa-2.1.1/mesa/model.py
+-rw-r--r--   0 jk         (501) staff       (20)    38769 2023-08-02 04:20:59.000000 Mesa-2.1.1/mesa/space.py
+-rw-r--r--   0 jk         (501) staff       (20)    10415 2023-07-17 03:55:09.000000 Mesa-2.1.1/mesa/time.py
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:29.695022 Mesa-2.1.1/mesa/visualization/
+-rw-r--r--   0 jk         (501) staff       (20)    14730 2023-07-17 03:55:09.000000 Mesa-2.1.1/mesa/visualization/ModularVisualization.py
+-rw-r--r--   0 jk         (501) staff       (20)     3792 2023-04-25 15:49:54.000000 Mesa-2.1.1/mesa/visualization/TextVisualization.py
+-rw-r--r--   0 jk         (501) staff       (20)     4127 2023-07-17 03:55:09.000000 Mesa-2.1.1/mesa/visualization/UserParam.py
+-rw-r--r--   0 jk         (501) staff       (20)      268 2023-04-25 15:49:54.000000 Mesa-2.1.1/mesa/visualization/__init__.py
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:29.712062 Mesa-2.1.1/mesa/visualization/modules/
+-rw-r--r--   0 jk         (501) staff       (20)     3736 2023-07-17 03:55:09.000000 Mesa-2.1.1/mesa/visualization/modules/BarChartVisualization.py
+-rw-r--r--   0 jk         (501) staff       (20)     4742 2023-04-25 15:49:54.000000 Mesa-2.1.1/mesa/visualization/modules/CanvasGridVisualization.py
+-rw-r--r--   0 jk         (501) staff       (20)     3144 2023-04-25 15:49:54.000000 Mesa-2.1.1/mesa/visualization/modules/ChartVisualization.py
+-rw-r--r--   0 jk         (501) staff       (20)     3541 2023-04-25 15:49:54.000000 Mesa-2.1.1/mesa/visualization/modules/HexGridVisualization.py
+-rw-r--r--   0 jk         (501) staff       (20)      838 2023-04-25 15:49:54.000000 Mesa-2.1.1/mesa/visualization/modules/NetworkVisualization.py
+-rw-r--r--   0 jk         (501) staff       (20)     2450 2023-04-25 15:49:54.000000 Mesa-2.1.1/mesa/visualization/modules/PieChartVisualization.py
+-rw-r--r--   0 jk         (501) staff       (20)      726 2023-04-25 15:49:54.000000 Mesa-2.1.1/mesa/visualization/modules/__init__.py
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:29.714318 Mesa-2.1.1/mesa/visualization/templates/
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:29.715953 Mesa-2.1.1/mesa/visualization/templates/css/
+-rw-r--r--   0 jk         (501) staff       (20)      377 2023-04-25 15:49:54.000000 Mesa-2.1.1/mesa/visualization/templates/css/visualization.css
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:29.639533 Mesa-2.1.1/mesa/visualization/templates/external/
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:29.639131 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:29.817902 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/
+-rw-r--r--   0 jk         (501) staff       (20)    72279 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.css
+-rw-r--r--   0 jk         (501) staff       (20)   201507 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.css.map
+-rw-r--r--   0 jk         (501) staff       (20)    52805 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.min.css
+-rw-r--r--   0 jk         (501) staff       (20)   122306 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.min.css.map
+-rw-r--r--   0 jk         (501) staff       (20)    72353 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.rtl.css
+-rw-r--r--   0 jk         (501) staff       (20)   201511 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.rtl.css.map
+-rw-r--r--   0 jk         (501) staff       (20)    52880 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0 jk         (501) staff       (20)   122383 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.rtl.min.css.map
+-rw-r--r--   0 jk         (501) staff       (20)     7578 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.css
+-rw-r--r--   0 jk         (501) staff       (20)   109619 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.css.map
+-rw-r--r--   0 jk         (501) staff       (20)     6120 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.min.css
+-rw-r--r--   0 jk         (501) staff       (20)    39730 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0 jk         (501) staff       (20)     7555 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0 jk         (501) staff       (20)   109632 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.rtl.css.map
+-rw-r--r--   0 jk         (501) staff       (20)     6192 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0 jk         (501) staff       (20)    47717 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.rtl.min.css.map
+-rw-r--r--   0 jk         (501) staff       (20)    71560 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.css
+-rw-r--r--   0 jk         (501) staff       (20)   192717 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.css.map
+-rw-r--r--   0 jk         (501) staff       (20)    53455 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.min.css
+-rw-r--r--   0 jk         (501) staff       (20)   111849 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.min.css.map
+-rw-r--r--   0 jk         (501) staff       (20)    71427 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0 jk         (501) staff       (20)   192660 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.rtl.css.map
+-rw-r--r--   0 jk         (501) staff       (20)    53383 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0 jk         (501) staff       (20)   111684 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.rtl.min.css.map
+-rw-r--r--   0 jk         (501) staff       (20)   205484 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.css
+-rw-r--r--   0 jk         (501) staff       (20)   538014 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.css.map
+-rw-r--r--   0 jk         (501) staff       (20)   163873 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.min.css
+-rw-r--r--   0 jk         (501) staff       (20)   451427 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.min.css.map
+-rw-r--r--   0 jk         (501) staff       (20)   205151 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.rtl.css
+-rw-r--r--   0 jk         (501) staff       (20)   537928 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.rtl.css.map
+-rw-r--r--   0 jk         (501) staff       (20)   163978 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.rtl.min.css
+-rw-r--r--   0 jk         (501) staff       (20)   663486 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.rtl.min.css.map
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:29.891611 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/
+-rw-r--r--   0 jk         (501) staff       (20)   209719 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.bundle.js
+-rw-r--r--   0 jk         (501) staff       (20)   427637 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.bundle.js.map
+-rw-r--r--   0 jk         (501) staff       (20)    78129 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.bundle.min.js
+-rw-r--r--   0 jk         (501) staff       (20)   331017 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 jk         (501) staff       (20)   139773 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.esm.js
+-rw-r--r--   0 jk         (501) staff       (20)   289576 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.esm.js.map
+-rw-r--r--   0 jk         (501) staff       (20)    72614 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.esm.min.js
+-rw-r--r--   0 jk         (501) staff       (20)   223558 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.esm.min.js.map
+-rw-r--r--   0 jk         (501) staff       (20)   148892 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.js
+-rw-r--r--   0 jk         (501) staff       (20)   290776 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.js.map
+-rw-r--r--   0 jk         (501) staff       (20)    59219 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.min.js
+-rw-r--r--   0 jk         (501) staff       (20)   219918 2023-03-10 00:33:56.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.min.js.map
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:29.914945 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:29.918539 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/.github/
+-rw-r--r--   0 jk         (501) staff       (20)      451 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/.github/CONTRIBUTING.md
+-rw-r--r--   0 jk         (501) staff       (20)      512 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 jk         (501) staff       (20)      747 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 jk         (501) staff       (20)      127 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/.gitignore
+-rw-r--r--   0 jk         (501) staff       (20)      103 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/.npmignore
+-rw-r--r--   0 jk         (501) staff       (20)       19 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/.npmrc
+-rw-r--r--   0 jk         (501) staff       (20)        7 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/.nvmrc
+-rw-r--r--   0 jk         (501) staff       (20)      774 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/.sass-lint.yml
+-rw-r--r--   0 jk         (501) staff       (20)      108 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/.travis.yml
+-rw-r--r--   0 jk         (501) staff       (20)    22936 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/CHANGELOG.md
+-rw-r--r--   0 jk         (501) staff       (20)     8974 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/Gruntfile.js
+-rw-r--r--   0 jk         (501) staff       (20)     1207 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/LICENSE.md
+-rw-r--r--   0 jk         (501) staff       (20)    15619 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/README.md
+-rw-r--r--   0 jk         (501) staff       (20)      527 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/bower.json
+-rw-r--r--   0 jk         (501) staff       (20)     1087 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/composer.json
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:29.642439 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dependencies/
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:29.919643 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dependencies/css/
+-rw-r--r--   0 jk         (501) staff       (20)      872 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dependencies/css/highlightjs-github-theme.css
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:29.930996 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dependencies/js/
+-rw-r--r--   0 jk         (501) staff       (20)    44793 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dependencies/js/highlight.min.js
+-rw-r--r--   0 jk         (501) staff       (20)    84280 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dependencies/js/jquery.min.js
+-rw-r--r--   0 jk         (501) staff       (20)    51351 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dependencies/js/modernizr.js
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:29.935675 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dist/
+-rw-r--r--   0 jk         (501) staff       (20)    71582 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dist/bootstrap-slider.js
+-rw-r--r--   0 jk         (501) staff       (20)    38829 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dist/bootstrap-slider.min.js
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:29.939199 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dist/css/
+-rw-r--r--   0 jk         (501) staff       (20)    12347 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dist/css/bootstrap-slider.css
+-rw-r--r--   0 jk         (501) staff       (20)    11184 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dist/css/bootstrap-slider.min.css
+-rw-r--r--   0 jk         (501) staff       (20)     3510 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/package.json
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:29.943394 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/scripts/
+-rw-r--r--   0 jk         (501) staff       (20)      383 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/scripts/build-preview.sh
+-rw-r--r--   0 jk         (501) staff       (20)     1320 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/scripts/release.sh
+-rw-r--r--   0 jk         (501) staff       (20)     1246 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/scripts/update-gh-pages.sh
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:29.646430 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/src/
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:29.944585 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/src/js/
+-rw-r--r--   0 jk         (501) staff       (20)    70254 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/src/js/bootstrap-slider.js
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:29.950855 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/src/sass/
+-rw-r--r--   0 jk         (501) staff       (20)     1033 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/src/sass/_mixins.scss
+-rw-r--r--   0 jk         (501) staff       (20)     6652 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/src/sass/_rules.scss
+-rw-r--r--   0 jk         (501) staff       (20)      930 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/src/sass/_variables.scss
+-rw-r--r--   0 jk         (501) staff       (20)     1638 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/src/sass/bootstrap-slider.scss
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:29.952275 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/
+-rw-r--r--   0 jk         (501) staff       (20)     1130 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/phantom_bind_polyfill.js
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:30.024567 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/
+-rw-r--r--   0 jk         (501) staff       (20)     3442 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/AccessibilitySpec.js
+-rw-r--r--   0 jk         (501) staff       (20)     4389 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/AriaValueTextFormatterSpec.js
+-rw-r--r--   0 jk         (501) staff       (20)      660 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/AutoRegisterDataProvideSpec.js
+-rw-r--r--   0 jk         (501) staff       (20)     1949 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/ConflictingOptionsSpec.js
+-rw-r--r--   0 jk         (501) staff       (20)    13555 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/DestroyMethodTests.js
+-rw-r--r--   0 jk         (501) staff       (20)    10331 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/DraggingHandlesSpec.js
+-rw-r--r--   0 jk         (501) staff       (20)     6587 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/ElementDataAttributesSpec.js
+-rw-r--r--   0 jk         (501) staff       (20)    15075 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/EventsSpec.js
+-rw-r--r--   0 jk         (501) staff       (20)     1532 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/FocusOptionSpec.js
+-rw-r--r--   0 jk         (501) staff       (20)    22847 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/KeyboardSupportSpec.js
+-rw-r--r--   0 jk         (501) staff       (20)    20361 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/LockToTicksSpec.js
+-rw-r--r--   0 jk         (501) staff       (20)     2248 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/LogarithmicScaleSpec.js
+-rw-r--r--   0 jk         (501) staff       (20)     5513 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/LowAndHighTrackSpec.js
+-rw-r--r--   0 jk         (501) staff       (20)     2270 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/NamespaceSpec.js
+-rw-r--r--   0 jk         (501) staff       (20)     2188 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/OrientationSpec.js
+-rw-r--r--   0 jk         (501) staff       (20)    23704 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/PublicMethodsSpec.js
+-rw-r--r--   0 jk         (501) staff       (20)     6450 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/RangeHighlightsSpec.js
+-rw-r--r--   0 jk         (501) staff       (20)     3402 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/RefreshMethodSpec.js
+-rw-r--r--   0 jk         (501) staff       (20)     2131 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/ResizeSpec.js
+-rw-r--r--   0 jk         (501) staff       (20)     2519 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/RtlOptionsSpec.js
+-rw-r--r--   0 jk         (501) staff       (20)     5305 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/ScrollableBodySpec.js
+-rw-r--r--   0 jk         (501) staff       (20)     3085 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/ScrollableContainerSpec.js
+-rw-r--r--   0 jk         (501) staff       (20)     1696 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/StepReachMaxValueSpec.js
+-rw-r--r--   0 jk         (501) staff       (20)     2712 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/TickClickingBehaviorSpec.js
+-rw-r--r--   0 jk         (501) staff       (20)     7767 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/TickLabelSpec.js
+-rw-r--r--   0 jk         (501) staff       (20)     7107 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/TickMarksSpec.js
+-rw-r--r--   0 jk         (501) staff       (20)    13937 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/TooltipMouseOverOptionSpec.js
+-rw-r--r--   0 jk         (501) staff       (20)     5640 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/TooltipPositionOptionSpec.js
+-rw-r--r--   0 jk         (501) staff       (20)     2649 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/TooltipSplitOptionSpec.js
+-rw-r--r--   0 jk         (501) staff       (20)    18834 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/TouchCapableSpec.js
+-rw-r--r--   0 jk         (501) staff       (20)      893 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/offMethodSpec.js
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:30.030621 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/tpl/
+-rw-r--r--   0 jk         (501) staff       (20)     4245 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/tpl/SpecRunner.tpl
+-rw-r--r--   0 jk         (501) staff       (20)    44636 2023-03-10 00:33:57.000000 Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/tpl/index.tpl
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:30.067980 Mesa-2.1.1/mesa/visualization/templates/js/
+-rw-r--r--   0 jk         (501) staff       (20)     4644 2023-04-25 15:49:54.000000 Mesa-2.1.1/mesa/visualization/templates/js/BarChartModule.js
+-rw-r--r--   0 jk         (501) staff       (20)     1610 2023-04-25 15:49:54.000000 Mesa-2.1.1/mesa/visualization/templates/js/CanvasHexModule.js
+-rw-r--r--   0 jk         (501) staff       (20)     1689 2023-04-25 15:49:54.000000 Mesa-2.1.1/mesa/visualization/templates/js/CanvasModule.js
+-rw-r--r--   0 jk         (501) staff       (20)     2204 2023-05-15 02:11:02.000000 Mesa-2.1.1/mesa/visualization/templates/js/ChartModule.js
+-rw-r--r--   0 jk         (501) staff       (20)    12943 2023-04-25 15:49:54.000000 Mesa-2.1.1/mesa/visualization/templates/js/GridDraw.js
+-rw-r--r--   0 jk         (501) staff       (20)     8609 2023-04-25 15:49:54.000000 Mesa-2.1.1/mesa/visualization/templates/js/HexDraw.js
+-rw-r--r--   0 jk         (501) staff       (20)     5295 2023-04-25 15:49:54.000000 Mesa-2.1.1/mesa/visualization/templates/js/InteractionHandler.js
+-rw-r--r--   0 jk         (501) staff       (20)     3002 2023-04-25 15:49:54.000000 Mesa-2.1.1/mesa/visualization/templates/js/NetworkModule_d3.js
+-rw-r--r--   0 jk         (501) staff       (20)     2826 2023-04-25 15:49:54.000000 Mesa-2.1.1/mesa/visualization/templates/js/PieChartModule.js
+-rw-r--r--   0 jk         (501) staff       (20)      327 2023-04-25 15:49:54.000000 Mesa-2.1.1/mesa/visualization/templates/js/TextModule.js
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:30.073113 Mesa-2.1.1/mesa/visualization/templates/js/external/
+-rw-r--r--   0 jk         (501) staff       (20)   193884 2023-03-10 00:33:58.000000 Mesa-2.1.1/mesa/visualization/templates/js/external/chart-3.6.1.min.js
+-rw-r--r--   0 jk         (501) staff       (20)   277072 2023-03-10 00:33:58.000000 Mesa-2.1.1/mesa/visualization/templates/js/external/d3-7.4.3.min.js
+-rw-r--r--   0 jk         (501) staff       (20)    10100 2023-05-15 02:11:02.000000 Mesa-2.1.1/mesa/visualization/templates/js/runcontrol.js
+-rw-r--r--   0 jk         (501) staff       (20)     4546 2023-04-25 15:49:54.000000 Mesa-2.1.1/mesa/visualization/templates/modular_template.html
+-rw-r--r--   0 jk         (501) staff       (20)     1895 2023-07-17 03:55:09.000000 Mesa-2.1.1/pyproject.toml
+-rw-r--r--   0 jk         (501) staff       (20)       38 2023-08-02 04:25:30.099356 Mesa-2.1.1/setup.cfg
+-rw-r--r--   0 jk         (501) staff       (20)     5264 2023-07-21 03:13:23.000000 Mesa-2.1.1/setup.py
+drwxr-xr-x   0 jk         (501) staff       (20)        0 2023-08-02 04:25:30.097615 Mesa-2.1.1/tests/
+-rw-r--r--   0 jk         (501) staff       (20)        0 2023-03-06 14:25:55.000000 Mesa-2.1.1/tests/__init__.py
+-rw-r--r--   0 jk         (501) staff       (20)     5092 2023-07-17 03:55:09.000000 Mesa-2.1.1/tests/test_batch_run.py
+-rw-r--r--   0 jk         (501) staff       (20)     8726 2023-05-28 15:25:59.000000 Mesa-2.1.1/tests/test_datacollector.py
+-rw-r--r--   0 jk         (501) staff       (20)     2506 2023-04-25 15:49:54.000000 Mesa-2.1.1/tests/test_examples.py
+-rw-r--r--   0 jk         (501) staff       (20)    15776 2023-07-17 03:55:09.000000 Mesa-2.1.1/tests/test_grid.py
+-rw-r--r--   0 jk         (501) staff       (20)      780 2023-07-17 03:55:09.000000 Mesa-2.1.1/tests/test_import_namespace.py
+-rw-r--r--   0 jk         (501) staff       (20)     2834 2023-04-25 15:49:54.000000 Mesa-2.1.1/tests/test_lifespan.py
+-rw-r--r--   0 jk         (501) staff       (20)      984 2023-04-25 15:49:54.000000 Mesa-2.1.1/tests/test_main.py
+-rw-r--r--   0 jk         (501) staff       (20)      970 2023-04-25 15:49:54.000000 Mesa-2.1.1/tests/test_model.py
+-rw-r--r--   0 jk         (501) staff       (20)      539 2023-04-25 15:49:54.000000 Mesa-2.1.1/tests/test_scaffold.py
+-rw-r--r--   0 jk         (501) staff       (20)    15823 2023-07-17 03:55:09.000000 Mesa-2.1.1/tests/test_space.py
+-rw-r--r--   0 jk         (501) staff       (20)     8717 2023-07-17 03:55:09.000000 Mesa-2.1.1/tests/test_time.py
+-rw-r--r--   0 jk         (501) staff       (20)     1270 2023-04-25 15:49:54.000000 Mesa-2.1.1/tests/test_tornado.py
+-rw-r--r--   0 jk         (501) staff       (20)     1780 2023-07-17 03:55:09.000000 Mesa-2.1.1/tests/test_usersettableparam.py
+-rw-r--r--   0 jk         (501) staff       (20)     3011 2023-07-17 03:55:09.000000 Mesa-2.1.1/tests/test_visualization.py
```

### Comparing `Mesa-2.1/HISTORY.rst` & `Mesa-2.1.1/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 .. :changelog:
 
 Release History
 ---------------
 
+2.1.1 (2023-08-02)
++++++++++++++++++++
+
+This release improves the introductory and visualization tutorial. Ensures both are Google Colab compatible with
+working badges.
+
+Changes:
+    * Update `intro_tutorial` to warn users to ensure up to date version, and make colab compatible #1739, #1744
+    * Improve new/experimental Solara based visualization to ensure pause button works #1745
+    * Fix bug in `space.py` -> `get_heading()` #1739
+
 2.1.0 (2023-07-22) Youngtown
 +++++++++++++++++++++++++++++
 
 This release creates `mesa.experimental` namespace, this solves the issue that PyPI release will not allow git-based install.
 
 **Users should read the Mesa 2.0.0 release note (directly below this), as this contains the details about the breaking
 changes and other major changes that were part of Mesa 2.0 release.**
```

### Comparing `Mesa-2.1/LICENSE` & `Mesa-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/Mesa.egg-info/PKG-INFO` & `Mesa-2.1.1/Mesa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mesa
-Version: 2.1
+Version: 2.1.1
 Summary: Agent-based modeling (ABM) in Python 3+
 Home-page: https://github.com/projectmesa/mesa
 Author: Project Mesa Team
 Author-email: projectmesa@googlegroups.com
 License: Apache 2.0
 Keywords: agent based modeling model ABM simulation multi-agent
 Classifier: Topic :: Scientific/Engineering
@@ -44,16 +44,15 @@
 
 .. image:: https://raw.githubusercontent.com/projectmesa/mesa/main/docs/images/Mesa_Screenshot.png
    :width: 100%
    :scale: 100%
    :alt: A screenshot of the Schelling Model in Mesa
 
 *Above: A Mesa implementation of the Schelling segregation model,
-being visualized in a browser window and analyzed in a Jupyter
-notebook.*
+this can be displayed in browser windows or Jupyter.*
 
 .. _`Mesa` : https://github.com/projectmesa/mesa/
 
 
 Features
 ------------
```

### Comparing `Mesa-2.1/Mesa.egg-info/SOURCES.txt` & `Mesa-2.1.1/Mesa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/PKG-INFO` & `Mesa-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mesa
-Version: 2.1
+Version: 2.1.1
 Summary: Agent-based modeling (ABM) in Python 3+
 Home-page: https://github.com/projectmesa/mesa
 Author: Project Mesa Team
 Author-email: projectmesa@googlegroups.com
 License: Apache 2.0
 Keywords: agent based modeling model ABM simulation multi-agent
 Classifier: Topic :: Scientific/Engineering
@@ -44,16 +44,15 @@
 
 .. image:: https://raw.githubusercontent.com/projectmesa/mesa/main/docs/images/Mesa_Screenshot.png
    :width: 100%
    :scale: 100%
    :alt: A screenshot of the Schelling Model in Mesa
 
 *Above: A Mesa implementation of the Schelling segregation model,
-being visualized in a browser window and analyzed in a Jupyter
-notebook.*
+this can be displayed in browser windows or Jupyter.*
 
 .. _`Mesa` : https://github.com/projectmesa/mesa/
 
 
 Features
 ------------
```

### Comparing `Mesa-2.1/README.rst` & `Mesa-2.1.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 
 .. image:: https://raw.githubusercontent.com/projectmesa/mesa/main/docs/images/Mesa_Screenshot.png
    :width: 100%
    :scale: 100%
    :alt: A screenshot of the Schelling Model in Mesa
 
 *Above: A Mesa implementation of the Schelling segregation model,
-being visualized in a browser window and analyzed in a Jupyter
-notebook.*
+this can be displayed in browser windows or Jupyter.*
 
 .. _`Mesa` : https://github.com/projectmesa/mesa/
 
 
 Features
 ------------
```

### Comparing `Mesa-2.1/mesa/__init__.py` & `Mesa-2.1.1/mesa/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -21,11 +21,11 @@
     "visualization",
     "DataCollector",
     "batch_run",
     "experimental",
 ]
 
 __title__ = "mesa"
-__version__ = "2.1"
+__version__ = "2.1.1"
 __license__ = "Apache 2.0"
 _this_year = datetime.datetime.now(tz=datetime.timezone.utc).date().year
 __copyright__ = f"Copyright {_this_year} Project Mesa Team"
```

### Comparing `Mesa-2.1/mesa/agent.py` & `Mesa-2.1.1/mesa/agent.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/batchrunner.py` & `Mesa-2.1.1/mesa/batchrunner.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/{{cookiecutter.snake}}/model.py` & `Mesa-2.1.1/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/{{cookiecutter.snake}}/model.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/{{cookiecutter.snake}}/server.py` & `Mesa-2.1.1/mesa/cookiecutter-mesa/{{cookiecutter.snake}}/{{cookiecutter.snake}}/server.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/datacollection.py` & `Mesa-2.1.1/mesa/datacollection.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/experimental/jupyter_viz.py` & `Mesa-2.1.1/mesa/experimental/jupyter_viz.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,15 +156,14 @@
     )
 
     # 3. Buttons
     playing = solara.use_reactive(False)
 
     def on_value_play(change):
         if viz.model.running:
-            playing.value = True
             viz.do_step()
         else:
             playing.value = False
 
     with solara.Row():
         solara.Button(label="Step", color="primary", on_click=viz.do_step)
         # This style is necessary so that the play widget has almost the same
@@ -179,15 +178,15 @@
         widgets.Play(
             value=0,
             interval=play_interval,
             repeat=True,
             show_repeat=False,
             on_value=on_value_play,
             playing=playing.value,
-            on_play=playing.set,
+            on_playing=playing.set,
         )
         # threaded_do_play is not used for now because it
         # doesn't work in Google colab. We use
         # ipywidgets.Play until it is fixed. The threading
         # version is definite a much better implementation,
         # if it works.
         # solara.Button(label="▶", color="primary", on_click=viz.threaded_do_play)
```

### Comparing `Mesa-2.1/mesa/main.py` & `Mesa-2.1.1/mesa/main.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/model.py` & `Mesa-2.1.1/mesa/model.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/space.py` & `Mesa-2.1.1/mesa/space.py`

 * *Files 0% similar despite different names*

```diff
@@ -930,15 +930,15 @@
 
             # Choose the smaller heading based on their absolute value for
             # each dimension independently.
             heading = tuple(
                 get_min_abs(heading[i], inverse_heading[i]) for i in range(2)
             )
         if isinstance(pos_1, np.ndarray):
-            heading = np.ndarray(heading)
+            heading = np.asarray(heading)
         else:
             heading = tuple(heading)
         return heading
 
     def get_distance(self, pos_1: FloatCoordinate, pos_2: FloatCoordinate) -> float:
         """Get the distance between two point, accounting for toroidal space.
```

### Comparing `Mesa-2.1/mesa/time.py` & `Mesa-2.1.1/mesa/time.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/ModularVisualization.py` & `Mesa-2.1.1/mesa/visualization/ModularVisualization.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/TextVisualization.py` & `Mesa-2.1.1/mesa/visualization/TextVisualization.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/UserParam.py` & `Mesa-2.1.1/mesa/visualization/UserParam.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/modules/BarChartVisualization.py` & `Mesa-2.1.1/mesa/visualization/modules/BarChartVisualization.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/modules/CanvasGridVisualization.py` & `Mesa-2.1.1/mesa/visualization/modules/CanvasGridVisualization.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/modules/ChartVisualization.py` & `Mesa-2.1.1/mesa/visualization/modules/ChartVisualization.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/modules/HexGridVisualization.py` & `Mesa-2.1.1/mesa/visualization/modules/HexGridVisualization.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/modules/NetworkVisualization.py` & `Mesa-2.1.1/mesa/visualization/modules/NetworkVisualization.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/modules/PieChartVisualization.py` & `Mesa-2.1.1/mesa/visualization/modules/PieChartVisualization.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/modules/__init__.py` & `Mesa-2.1.1/mesa/visualization/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.css` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.css.map` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.min.css` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.min.css.map` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.rtl.css` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.rtl.css.map` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.rtl.min.css` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.rtl.min.css.map` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.css` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.css.map` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.min.css` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.min.css.map` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.rtl.css` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.rtl.css.map` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.rtl.min.css` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.rtl.min.css.map` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.css` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.css.map` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.min.css` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.min.css.map` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.rtl.css` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.rtl.css.map` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.rtl.min.css` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.rtl.min.css.map` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.css` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.css.map` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.min.css` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.min.css.map` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.rtl.css` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.rtl.css.map` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.rtl.min.css` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.rtl.min.css.map` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.bundle.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.bundle.js.map` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.bundle.min.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.bundle.min.js.map` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.esm.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.esm.js.map` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.esm.min.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.esm.min.js.map` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.js.map` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.min.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.min.js.map` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-5.1.3-dist/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/.github/ISSUE_TEMPLATE.md` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/.github/PULL_REQUEST_TEMPLATE.md` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/.sass-lint.yml` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/.sass-lint.yml`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/CHANGELOG.md` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/Gruntfile.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/Gruntfile.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/LICENSE.md` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/README.md` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/README.md`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/bower.json` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/bower.json`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/composer.json` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/composer.json`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dependencies/css/highlightjs-github-theme.css` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dependencies/css/highlightjs-github-theme.css`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dependencies/js/highlight.min.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dependencies/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dependencies/js/jquery.min.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dependencies/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dependencies/js/modernizr.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dependencies/js/modernizr.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dist/bootstrap-slider.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dist/bootstrap-slider.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dist/bootstrap-slider.min.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dist/bootstrap-slider.min.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dist/css/bootstrap-slider.css` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dist/css/bootstrap-slider.css`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dist/css/bootstrap-slider.min.css` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/dist/css/bootstrap-slider.min.css`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/package.json` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/package.json`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/scripts/release.sh` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/scripts/release.sh`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/scripts/update-gh-pages.sh` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/scripts/update-gh-pages.sh`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/src/js/bootstrap-slider.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/src/js/bootstrap-slider.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/src/sass/_mixins.scss` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/src/sass/_mixins.scss`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/src/sass/_rules.scss` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/src/sass/_rules.scss`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/src/sass/_variables.scss` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/src/sass/_variables.scss`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/src/sass/bootstrap-slider.scss` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/src/sass/bootstrap-slider.scss`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/phantom_bind_polyfill.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/phantom_bind_polyfill.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/AccessibilitySpec.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/AccessibilitySpec.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/AriaValueTextFormatterSpec.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/AriaValueTextFormatterSpec.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/AutoRegisterDataProvideSpec.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/AutoRegisterDataProvideSpec.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/ConflictingOptionsSpec.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/ConflictingOptionsSpec.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/DestroyMethodTests.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/DestroyMethodTests.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/DraggingHandlesSpec.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/DraggingHandlesSpec.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/ElementDataAttributesSpec.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/ElementDataAttributesSpec.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/EventsSpec.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/EventsSpec.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/FocusOptionSpec.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/FocusOptionSpec.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/KeyboardSupportSpec.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/KeyboardSupportSpec.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/LockToTicksSpec.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/LockToTicksSpec.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/LogarithmicScaleSpec.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/LogarithmicScaleSpec.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/LowAndHighTrackSpec.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/LowAndHighTrackSpec.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/NamespaceSpec.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/NamespaceSpec.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/OrientationSpec.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/OrientationSpec.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/PublicMethodsSpec.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/PublicMethodsSpec.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/RangeHighlightsSpec.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/RangeHighlightsSpec.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/RefreshMethodSpec.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/RefreshMethodSpec.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/ResizeSpec.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/ResizeSpec.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/RtlOptionsSpec.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/RtlOptionsSpec.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/ScrollableBodySpec.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/ScrollableBodySpec.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/ScrollableContainerSpec.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/ScrollableContainerSpec.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/StepReachMaxValueSpec.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/StepReachMaxValueSpec.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/TickClickingBehaviorSpec.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/TickClickingBehaviorSpec.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/TickLabelSpec.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/TickLabelSpec.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/TickMarksSpec.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/TickMarksSpec.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/TooltipMouseOverOptionSpec.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/TooltipMouseOverOptionSpec.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/TooltipPositionOptionSpec.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/TooltipPositionOptionSpec.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/TooltipSplitOptionSpec.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/TooltipSplitOptionSpec.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/TouchCapableSpec.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/TouchCapableSpec.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/offMethodSpec.js` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/test/specs/offMethodSpec.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/tpl/SpecRunner.tpl` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/tpl/SpecRunner.tpl`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/tpl/index.tpl` & `Mesa-2.1.1/mesa/visualization/templates/external/bootstrap-slider-11.0.2/tpl/index.tpl`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/js/BarChartModule.js` & `Mesa-2.1.1/mesa/visualization/templates/js/BarChartModule.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/js/CanvasHexModule.js` & `Mesa-2.1.1/mesa/visualization/templates/js/CanvasHexModule.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/js/CanvasModule.js` & `Mesa-2.1.1/mesa/visualization/templates/js/CanvasModule.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/js/ChartModule.js` & `Mesa-2.1.1/mesa/visualization/templates/js/ChartModule.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/js/GridDraw.js` & `Mesa-2.1.1/mesa/visualization/templates/js/GridDraw.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/js/HexDraw.js` & `Mesa-2.1.1/mesa/visualization/templates/js/HexDraw.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/js/InteractionHandler.js` & `Mesa-2.1.1/mesa/visualization/templates/js/InteractionHandler.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/js/NetworkModule_d3.js` & `Mesa-2.1.1/mesa/visualization/templates/js/NetworkModule_d3.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/js/PieChartModule.js` & `Mesa-2.1.1/mesa/visualization/templates/js/PieChartModule.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/js/external/chart-3.6.1.min.js` & `Mesa-2.1.1/mesa/visualization/templates/js/external/chart-3.6.1.min.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/js/external/d3-7.4.3.min.js` & `Mesa-2.1.1/mesa/visualization/templates/js/external/d3-7.4.3.min.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/js/runcontrol.js` & `Mesa-2.1.1/mesa/visualization/templates/js/runcontrol.js`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/mesa/visualization/templates/modular_template.html` & `Mesa-2.1.1/mesa/visualization/templates/modular_template.html`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/pyproject.toml` & `Mesa-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/setup.py` & `Mesa-2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/tests/test_batch_run.py` & `Mesa-2.1.1/tests/test_batch_run.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/tests/test_datacollector.py` & `Mesa-2.1.1/tests/test_datacollector.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/tests/test_examples.py` & `Mesa-2.1.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/tests/test_grid.py` & `Mesa-2.1.1/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/tests/test_import_namespace.py` & `Mesa-2.1.1/tests/test_import_namespace.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/tests/test_lifespan.py` & `Mesa-2.1.1/tests/test_lifespan.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/tests/test_main.py` & `Mesa-2.1.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/tests/test_model.py` & `Mesa-2.1.1/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/tests/test_scaffold.py` & `Mesa-2.1.1/tests/test_scaffold.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/tests/test_space.py` & `Mesa-2.1.1/tests/test_space.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/tests/test_time.py` & `Mesa-2.1.1/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/tests/test_tornado.py` & `Mesa-2.1.1/tests/test_tornado.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/tests/test_usersettableparam.py` & `Mesa-2.1.1/tests/test_usersettableparam.py`

 * *Files identical despite different names*

### Comparing `Mesa-2.1/tests/test_visualization.py` & `Mesa-2.1.1/tests/test_visualization.py`

 * *Files identical despite different names*


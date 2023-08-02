# Comparing `tmp/cellfinder-core-0.5.0.tar.gz` & `tmp/cellfinder-core-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellfinder-core-0.5.0.tar", last modified: Thu Jul  6 11:10:40 2023, max compression
+gzip compressed data, was "cellfinder-core-0.5.1.tar", last modified: Wed Aug  2 12:21:53 2023, max compression
```

## Comparing `cellfinder-core-0.5.0.tar` & `cellfinder-core-0.5.1.tar`

### file list

```diff
@@ -1,106 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.287268 cellfinder-core-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/.codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.259268 cellfinder-core-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.271268 cellfinder-core-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/.github/workflows/test_numba_off.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13398 2023-07-06 11:10:40.287268 cellfinder-core-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12361 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.271268 cellfinder-core-0.5.0/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/benchmarks/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/benchmarks/detect_and_classify.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/benchmarks/filter_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/benchmarks/filter_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 11:10:40.287268 cellfinder-core-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.263268 cellfinder-core-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.271268 cellfinder-core-0.5.0/src/cellfinder_core/
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.279268 cellfinder-core-0.5.0/src/cellfinder_core/classify/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/classify/augment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/classify/classify.py
--rw-r--r--   0 runner    (1001) docker     (123)    16614 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/classify/cube_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/classify/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/classify/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.279268 cellfinder-core-0.5.0/src/cellfinder_core/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/config/cellfinder.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.279268 cellfinder-core-0.5.0/src/cellfinder_core/detect/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/detect/detect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.279268 cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.279268 cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/plane/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/plane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/plane/classical_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/plane/plane_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/plane/tile_walker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/setup_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.283268 cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/volume/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/volume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11173 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/volume/ball_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9152 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/volume/structure_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/volume/structure_splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/volume/volume_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.283268 cellfinder-core-0.5.0/src/cellfinder_core/download/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/download/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/download/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/download/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.287268 cellfinder-core-0.5.0/src/cellfinder_core/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/tools/IO.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/tools/array_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/tools/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/tools/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/tools/prep.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/tools/source_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/tools/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/tools/tf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/tools/tiff.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/tools/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.287268 cellfinder-core-0.5.0/src/cellfinder_core/train/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/train/train_yml.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/src/cellfinder_core/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.275268 cellfinder-core-0.5.0/src/cellfinder_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13398 2023-07-06 11:10:38.000000 cellfinder-core-0.5.0/src/cellfinder_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-07-06 11:10:40.000000 cellfinder-core-0.5.0/src/cellfinder_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 11:10:38.000000 cellfinder-core-0.5.0/src/cellfinder_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-06 11:10:38.000000 cellfinder-core-0.5.0/src/cellfinder_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-06 11:10:38.000000 cellfinder-core-0.5.0/src/cellfinder_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 11:10:38.000000 cellfinder-core-0.5.0/src/cellfinder_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.287268 cellfinder-core-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:25.000000 cellfinder-core-0.5.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.287268 cellfinder-core-0.5.0/tests/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.287268 cellfinder-core-0.5.0/tests/tests/test_integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/test_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/test_integration/test_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/test_integration/test_detection_structure_splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/test_integration/test_train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.287268 cellfinder-core-0.5.0/tests/tests/test_unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/test_unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.287268 cellfinder-core-0.5.0/tests/tests/test_unit/test_detect/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/test_unit/test_detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/test_unit/test_detect/test_detect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.267268 cellfinder-core-0.5.0/tests/tests/test_unit/test_detect/test_filters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.287268 cellfinder-core-0.5.0/tests/tests/test_unit/test_detect/test_filters/test_volume_filters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/test_unit/test_detect/test_filters/test_volume_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/test_unit/test_detect/test_filters/test_volume_filters/test_structure_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:40.287268 cellfinder-core-0.5.0/tests/tests/test_unit/test_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/test_unit/test_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/test_unit/test_tools/test_IO.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/test_unit/test_tools/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/test_unit/test_tools/test_image_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/test_unit/test_tools/test_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tests/tests/test_unit/test_tools/test_tools_general.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-06 11:10:26.000000 cellfinder-core-0.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:21:52.998518 cellfinder-core-0.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:21:52.990518 cellfinder-core-0.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:21:52.994518 cellfinder-core-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/.github/workflows/test_include_guard.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/.github/workflows/test_numba_off.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-08-02 12:21:52.998518 cellfinder-core-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12361 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 12:21:52.998518 cellfinder-core-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:21:52.990518 cellfinder-core-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:21:52.994518 cellfinder-core-0.5.1/src/cellfinder_core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:21:52.994518 cellfinder-core-0.5.1/src/cellfinder_core/classify/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/classify/augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/classify/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16614 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/classify/cube_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/classify/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/classify/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:21:52.994518 cellfinder-core-0.5.1/src/cellfinder_core/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/config/cellfinder.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:21:52.994518 cellfinder-core-0.5.1/src/cellfinder_core/detect/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/detect/detect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:21:52.994518 cellfinder-core-0.5.1/src/cellfinder_core/detect/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/detect/filters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:21:52.998518 cellfinder-core-0.5.1/src/cellfinder_core/detect/filters/plane/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/detect/filters/plane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/detect/filters/plane/classical_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/detect/filters/plane/plane_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/detect/filters/plane/tile_walker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/detect/filters/setup_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:21:52.998518 cellfinder-core-0.5.1/src/cellfinder_core/detect/filters/volume/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/detect/filters/volume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11173 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/detect/filters/volume/ball_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9152 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/detect/filters/volume/structure_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/detect/filters/volume/structure_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/detect/filters/volume/volume_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:21:52.998518 cellfinder-core-0.5.1/src/cellfinder_core/download/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/download/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/download/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/download/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:21:52.998518 cellfinder-core-0.5.1/src/cellfinder_core/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/tools/IO.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/tools/array_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/tools/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/tools/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/tools/prep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/tools/source_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/tools/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/tools/tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/tools/tiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/tools/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:21:52.998518 cellfinder-core-0.5.1/src/cellfinder_core/train/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/train/train_yml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-02 12:21:36.000000 cellfinder-core-0.5.1/src/cellfinder_core/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:21:52.994518 cellfinder-core-0.5.1/src/cellfinder_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-08-02 12:21:51.000000 cellfinder-core-0.5.1/src/cellfinder_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-08-02 12:21:52.000000 cellfinder-core-0.5.1/src/cellfinder_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 12:21:51.000000 cellfinder-core-0.5.1/src/cellfinder_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-02 12:21:51.000000 cellfinder-core-0.5.1/src/cellfinder_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-08-02 12:21:51.000000 cellfinder-core-0.5.1/src/cellfinder_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-02 12:21:51.000000 cellfinder-core-0.5.1/src/cellfinder_core.egg-info/top_level.txt
```

### Comparing `cellfinder-core-0.5.0/.github/workflows/test_and_deploy.yml` & `cellfinder-core-0.5.1/.github/workflows/test_and_deploy.yml`

 * *Files 7% similar despite different names*

```diff
@@ -8,17 +8,24 @@
   pull_request:
     branches: [ '*' ]
 
 jobs:
   linting:
     runs-on: ubuntu-latest
     steps:
-      - uses: neuroinformatics-unit/actions/lint@v1.2.0
+      - uses: neuroinformatics-unit/actions/lint@v2
+
+  manifest:
+    name: Check Manifest
+    runs-on: ubuntu-latest
+    steps:
+      - uses: neuroinformatics-unit/actions/check_manifest@v2
 
   test:
+    needs: [linting, manifest]
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         # Run all supported Python versions on linux
         os: [ubuntu-latest]
         python-version: ["3.8", "3.9", "3.10"]
         # Include one windows, one macos run
@@ -38,14 +45,15 @@
         with:
           python-version: ${{ matrix.python-version }}
 
 
   # Run cellfinder tests to make sure cellfinder is still compatible
   # with cellfinder-core
   test_cellfinder:
+    needs: [linting, manifest]
     name: Run cellfinder tests
     runs-on: ubuntu-latest
     steps:
       - name: Cache tensorflow model
         uses: actions/cache@v3
         with:
           path: "~/.cellfinder"
```

### Comparing `cellfinder-core-0.5.0/.github/workflows/test_numba_off.yml` & `cellfinder-core-0.5.1/.github/workflows/test_numba_off.yml`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.5.0/.gitignore` & `cellfinder-core-0.5.1/.gitignore`

 * *Files 10% similar despite different names*

```diff
@@ -120,7 +120,13 @@
 *.~lock.*
 
 pip-wheel-metadata/
 
 mprofile*.dat
 
 *.DS_Store
+
+# asv
+.asv
+benchmarks/results
+benchmarks/html
+benchmarks/env
```

### Comparing `cellfinder-core-0.5.0/LICENSE` & `cellfinder-core-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.5.0/PKG-INFO` & `cellfinder-core-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: cellfinder-core
-Version: 0.5.0
+Version: 0.5.1
 Summary: Automated 3D cell detection in large microscopy images
 Author-email: "Adam Tyson, Christian Niedworok, Charly Rousseau" <code@adamltyson.com>
-Project-URL: Homepage, https://brainglobe.info/cellfinder
+Project-URL: Homepage, https://brainglobe.info
 Project-URL: Source Code, https://github.com/brainglobe/cellfinder-core
 Project-URL: Bug Tracker, https://github.com/brainglobe/cellfinder-core/issues
-Project-URL: Documentation, https://docs.brainglobe.info/cellfinder
+Project-URL: Documentation, https://brainglobe.info/documentation/cellfinder/index.html
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `cellfinder-core-0.5.0/README.md` & `cellfinder-core-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.5.0/pyproject.toml` & `cellfinder-core-0.5.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -31,27 +31,28 @@
     "tensorflow>=2.5.0,<2.12.0; platform_system!='Darwin' or platform_machine!='arm64'",
     "tifffile",
     "tqdm",
 ]
 dynamic = ['version']
 
 [project.urls]
-Homepage = "https://brainglobe.info/cellfinder"
+Homepage = "https://brainglobe.info"
 "Source Code" = "https://github.com/brainglobe/cellfinder-core"
 "Bug Tracker" = "https://github.com/brainglobe/cellfinder-core/issues"
-Documentation = "https://docs.brainglobe.info/cellfinder"
+Documentation = "https://brainglobe.info/documentation/cellfinder/index.html"
 
 [project.optional-dependencies]
 dev = [
     "black",
     "gitpython",
     "pre-commit",
     "pyinstrument",
     "pytest",
     "pytest-cov",
+    "pytest-lazy-fixture",
     "pytest-mock",
     "pytest-timeout",
     "tox",
 ]
 
 [project.scripts]
 cellfinder_download = "cellfinder_core.download.cli:main"
@@ -114,21 +115,23 @@
     "brainglobe_utils.*",
     "natsort.*",
     "numba.*",
     "tensorflow.*",
     "tifffile.*",
     "pyinstrument.*",
     "pytest.*",
+    "pytest_lazyfixture.*",
     "scipy.*",
     "skimage.*",
     "sklearn.*",
+    "cellfinder_core.tools.prep.*",
 ]
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = [
     "cellfinder_core.detect.*",
-    "cellfinder_core.classify.*"
+    "cellfinder_core.classify.*",
 ]
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
 disallow_untyped_calls = true
```

### Comparing `cellfinder-core-0.5.0/src/cellfinder_core/__init__.py` & `cellfinder-core-0.5.1/src/cellfinder_core/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,20 +6,23 @@
     raise PackageNotFoundError("cellfinder-core package not installed") from e
 
 # If tensorflow is not present, tools cannot be used.
 # Throw an error in this case to prevent invocation of functions.
 try:
     TF_VERSION = version("tensorflow")
 except PackageNotFoundError as e:
-    raise PackageNotFoundError(
-        f"cellfinder tools cannot be invoked without tensorflow. "
-        f"Please install tensorflow into your environment to use cellfinder tools. "
-        f"For more information, please see "
-        f"https://github.com/brainglobe/brainglobe-meta#readme."
-    ) from e
+    try:
+        TF_VERSION = version("tensorflow-macos")
+    except PackageNotFoundError as e:
+        raise PackageNotFoundError(
+            f"cellfinder tools cannot be invoked without tensorflow. "
+            f"Please install tensorflow into your environment to use cellfinder tools. "
+            f"For more information, please see "
+            f"https://github.com/brainglobe/brainglobe-meta#readme."
+        ) from e
 
 __author__ = "Adam Tyson, Christian Niedworok, Charly Rousseau"
 __license__ = "BSD-3-Clause"
 
 import logging
 
 logger = logging.getLogger("cellfinder_core")
```

### Comparing `cellfinder-core-0.5.0/src/cellfinder_core/classify/augment.py` & `cellfinder-core-0.5.1/src/cellfinder_core/classify/augment.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.5.0/src/cellfinder_core/classify/classify.py` & `cellfinder-core-0.5.1/src/cellfinder_core/classify/classify.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.5.0/src/cellfinder_core/classify/cube_generator.py` & `cellfinder-core-0.5.1/src/cellfinder_core/classify/cube_generator.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.5.0/src/cellfinder_core/classify/resnet.py` & `cellfinder-core-0.5.1/src/cellfinder_core/classify/resnet.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.5.0/src/cellfinder_core/classify/tools.py` & `cellfinder-core-0.5.1/src/cellfinder_core/classify/tools.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.5.0/src/cellfinder_core/detect/detect.py` & `cellfinder-core-0.5.1/src/cellfinder_core/detect/detect.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     """
     if not np.issubdtype(signal_array.dtype, np.integer):
         raise ValueError(
             "signal_array must be integer datatype, but has datatype "
             f"{signal_array.dtype}"
         )
     n_processes = get_num_processes(min_free_cpu_cores=n_free_cpus)
-    n_ball_procs = n_processes - 1
+    n_ball_procs = max(n_processes - 1, 1)
     start_time = datetime.now()
 
     (
         soma_diameter,
         max_cluster_size,
         ball_xy_size,
         ball_z_size,
```

### Comparing `cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/plane/classical_filter.py` & `cellfinder-core-0.5.1/src/cellfinder_core/detect/filters/plane/classical_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/plane/plane_filter.py` & `cellfinder-core-0.5.1/src/cellfinder_core/detect/filters/plane/plane_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/plane/tile_walker.py` & `cellfinder-core-0.5.1/src/cellfinder_core/detect/filters/plane/tile_walker.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/setup_filters.py` & `cellfinder-core-0.5.1/src/cellfinder_core/detect/filters/setup_filters.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/volume/ball_filter.py` & `cellfinder-core-0.5.1/src/cellfinder_core/detect/filters/volume/ball_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/volume/structure_detection.py` & `cellfinder-core-0.5.1/src/cellfinder_core/detect/filters/volume/structure_detection.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/volume/structure_splitting.py` & `cellfinder-core-0.5.1/src/cellfinder_core/detect/filters/volume/structure_splitting.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.5.0/src/cellfinder_core/detect/filters/volume/volume_filter.py` & `cellfinder-core-0.5.1/src/cellfinder_core/detect/filters/volume/volume_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.5.0/src/cellfinder_core/download/cli.py` & `cellfinder-core-0.5.1/src/cellfinder_core/download/cli.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.5.0/src/cellfinder_core/download/download.py` & `cellfinder-core-0.5.1/src/cellfinder_core/download/download.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.5.0/src/cellfinder_core/download/models.py` & `cellfinder-core-0.5.1/src/cellfinder_core/download/models.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.5.0/src/cellfinder_core/main.py` & `cellfinder-core-0.5.1/src/cellfinder_core/main.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.5.0/src/cellfinder_core/tools/IO.py` & `cellfinder-core-0.5.1/src/cellfinder_core/tools/IO.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.5.0/src/cellfinder_core/tools/array_operations.py` & `cellfinder-core-0.5.1/src/cellfinder_core/tools/array_operations.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.5.0/src/cellfinder_core/tools/geometry.py` & `cellfinder-core-0.5.1/src/cellfinder_core/tools/geometry.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.5.0/src/cellfinder_core/tools/image_processing.py` & `cellfinder-core-0.5.1/src/cellfinder_core/tools/image_processing.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.5.0/src/cellfinder_core/tools/prep.py` & `cellfinder-core-0.5.1/src/cellfinder_core/tools/prep.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.5.0/src/cellfinder_core/tools/system.py` & `cellfinder-core-0.5.1/src/cellfinder_core/tools/system.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.5.0/src/cellfinder_core/tools/tf.py` & `cellfinder-core-0.5.1/src/cellfinder_core/tools/tf.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.5.0/src/cellfinder_core/tools/tiff.py` & `cellfinder-core-0.5.1/src/cellfinder_core/tools/tiff.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.5.0/src/cellfinder_core/tools/tools.py` & `cellfinder-core-0.5.1/src/cellfinder_core/tools/tools.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.5.0/src/cellfinder_core/train/train_yml.py` & `cellfinder-core-0.5.1/src/cellfinder_core/train/train_yml.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.5.0/src/cellfinder_core.egg-info/PKG-INFO` & `cellfinder-core-0.5.1/src/cellfinder_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: cellfinder-core
-Version: 0.5.0
+Version: 0.5.1
 Summary: Automated 3D cell detection in large microscopy images
 Author-email: "Adam Tyson, Christian Niedworok, Charly Rousseau" <code@adamltyson.com>
-Project-URL: Homepage, https://brainglobe.info/cellfinder
+Project-URL: Homepage, https://brainglobe.info
 Project-URL: Source Code, https://github.com/brainglobe/cellfinder-core
 Project-URL: Bug Tracker, https://github.com/brainglobe/cellfinder-core/issues
-Project-URL: Documentation, https://docs.brainglobe.info/cellfinder
+Project-URL: Documentation, https://brainglobe.info/documentation/cellfinder/index.html
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


# Comparing `tmp/napari_brainways-0.1.6.1.tar.gz` & `tmp/napari_brainways-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_brainways-0.1.6.1.tar", last modified: Sun Jun 18 09:50:29 2023, max compression
+gzip compressed data, was "napari_brainways-0.1.7.tar", last modified: Wed Aug  2 08:56:55 2023, max compression
```

## Comparing `napari_brainways-0.1.6.1.tar` & `napari_brainways-0.1.7.tar`

### file list

```diff
@@ -1,72 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:50:29.268422 napari_brainways-0.1.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:50:29.256422 napari_brainways-0.1.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:50:29.260422 napari_brainways-0.1.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:50:29.260422 napari_brainways-0.1.6.1/.napari/
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/.napari/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-06-18 09:50:29.268422 napari_brainways-0.1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:50:29.260422 napari_brainways-0.1.6.1/data/
--rw-r--r--   0 runner    (1001) docker     (123)   269441 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/data/test_data.npz
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-18 09:50:29.272422 napari_brainways-0.1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:50:29.256422 napari_brainways-0.1.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:50:29.264422 napari_brainways-0.1.6.1/src/napari_brainways/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/_sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:50:29.264422 napari_brainways-0.1.6.1/src/napari_brainways/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/_tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/_tests/test_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-18 09:50:29.000000 napari_brainways-0.1.6.1/src/napari_brainways/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    18697 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/brainways_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:50:29.264422 napari_brainways-0.1.6.1/src/napari_brainways/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/controllers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:50:29.268422 napari_brainways-0.1.6.1/src/napari_brainways/controllers/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/controllers/_tests/test_affine_2d_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/controllers/_tests/test_annotation_viewer_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/controllers/_tests/test_cell_3d_viewer_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/controllers/_tests/test_cell_detector_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/controllers/_tests/test_registration_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/controllers/_tests/test_tps_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/controllers/affine_2d_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/controllers/annotation_viewer_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/controllers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/controllers/cell_3d_viewer_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    10951 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/controllers/cell_detector_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/controllers/registration_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/controllers/tps_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/napari_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:50:29.268422 napari_brainways-0.1.6.1/src/napari_brainways/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   231054 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/resources/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:50:29.268422 napari_brainways-0.1.6.1/src/napari_brainways/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:50:29.268422 napari_brainways-0.1.6.1/src/napari_brainways/widgets/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/widgets/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/widgets/_tests/test_create_project_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/widgets/_tests/test_registration_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/widgets/affine_2d_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/widgets/cell_detector_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/widgets/cell_viewer_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/widgets/create_subject_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/widgets/registration_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/widgets/tps_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    22436 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/src/napari_brainways/widgets/workflow_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:50:29.264422 napari_brainways-0.1.6.1/src/napari_brainways.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-06-18 09:50:29.000000 napari_brainways-0.1.6.1/src/napari_brainways.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-18 09:50:29.000000 napari_brainways-0.1.6.1/src/napari_brainways.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 09:50:29.000000 napari_brainways-0.1.6.1/src/napari_brainways.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-18 09:50:29.000000 napari_brainways-0.1.6.1/src/napari_brainways.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-18 09:50:29.000000 napari_brainways-0.1.6.1/src/napari_brainways.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-18 09:50:29.000000 napari_brainways-0.1.6.1/src/napari_brainways.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-18 09:50:07.000000 napari_brainways-0.1.6.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:56:55.056484 napari_brainways-0.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:56:55.040483 napari_brainways-0.1.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:56:55.044484 napari_brainways-0.1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:56:55.044484 napari_brainways-0.1.7/.napari/
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/.napari/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-08-02 08:56:55.056484 napari_brainways-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:56:55.044484 napari_brainways-0.1.7/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   269441 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/data/test_data.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-08-02 08:56:55.056484 napari_brainways-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:56:55.040483 napari_brainways-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:56:55.048483 napari_brainways-0.1.7/src/napari_brainways/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/_sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:56:55.048483 napari_brainways-0.1.7/src/napari_brainways/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/_tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/_tests/test_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-02 08:56:54.000000 napari_brainways-0.1.7/src/napari_brainways/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18128 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/brainways_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:56:55.052483 napari_brainways-0.1.7/src/napari_brainways/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/controllers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:56:55.052483 napari_brainways-0.1.7/src/napari_brainways/controllers/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/controllers/_tests/test_affine_2d_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/controllers/_tests/test_annotation_viewer_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/controllers/_tests/test_cell_3d_viewer_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/controllers/_tests/test_cell_detector_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/controllers/_tests/test_registration_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/controllers/_tests/test_tps_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/controllers/affine_2d_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/controllers/analysis_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/controllers/annotation_viewer_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/controllers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/controllers/cell_3d_viewer_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/controllers/cell_detector_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/controllers/registration_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/controllers/tps_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/napari_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:56:55.052483 napari_brainways-0.1.7/src/napari_brainways/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   231054 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/resources/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:56:55.056484 napari_brainways-0.1.7/src/napari_brainways/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:56:55.056484 napari_brainways-0.1.7/src/napari_brainways/widgets/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/widgets/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/widgets/_tests/test_create_project_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/widgets/_tests/test_registration_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/widgets/affine_2d_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/widgets/analysis_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/widgets/cell_detector_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/widgets/cell_viewer_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/widgets/create_subject_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/widgets/registration_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/widgets/tps_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20913 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/src/napari_brainways/widgets/workflow_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:56:55.048483 napari_brainways-0.1.7/src/napari_brainways.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-08-02 08:56:55.000000 napari_brainways-0.1.7/src/napari_brainways.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-08-02 08:56:55.000000 napari_brainways-0.1.7/src/napari_brainways.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 08:56:55.000000 napari_brainways-0.1.7/src/napari_brainways.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-02 08:56:55.000000 napari_brainways-0.1.7/src/napari_brainways.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-02 08:56:55.000000 napari_brainways-0.1.7/src/napari_brainways.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-02 08:56:55.000000 napari_brainways-0.1.7/src/napari_brainways.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-02 08:56:34.000000 napari_brainways-0.1.7/tox.ini
```

### Comparing `napari_brainways-0.1.6.1/.github/workflows/test_and_deploy.yml` & `napari_brainways-0.1.7/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.6.1/.gitignore` & `napari_brainways-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.6.1/.napari/DESCRIPTION.md` & `napari_brainways-0.1.7/.napari/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.6.1/.pre-commit-config.yaml` & `napari_brainways-0.1.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.6.1/LICENSE` & `napari_brainways-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.6.1/PKG-INFO` & `napari_brainways-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari_brainways
-Version: 0.1.6.1
+Version: 0.1.7
 Summary: Brainways UI
 Home-page: https://github.com/bkntr/napari-brainways
 Author: Ben Kantor
 Author-email: benkantor@mail.tau.ac.il
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/bkntr/napari-brainways/issues
 Project-URL: Documentation, https://github.com/bkntr/napari-brainways#README.md
```

### Comparing `napari_brainways-0.1.6.1/README.md` & `napari_brainways-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.6.1/data/test_data.npz` & `napari_brainways-0.1.7/data/test_data.npz`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.6.1/setup.cfg` & `napari_brainways-0.1.7/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 	Documentation = https://github.com/bkntr/napari-brainways#README.md
 	Source Code = https://github.com/bkntr/napari-brainways
 	User Support = https://github.com/bkntr/napari-brainways/issues
 
 [options]
 packages = find:
 install_requires = 
-	brainways==0.1.6
+	brainways==0.1.7
 	importlib-resources
 	napari
 	qtpy
 	stardist==0.8.3
 	tensorflow
 python_requires = >=3.8
 include_package_data = True
```

### Comparing `napari_brainways-0.1.6.1/src/napari_brainways/_sample_data.py` & `napari_brainways-0.1.7/src/napari_brainways/_sample_data.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.6.1/src/napari_brainways/_tests/test_reader.py` & `napari_brainways-0.1.7/src/napari_brainways/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.6.1/src/napari_brainways/_tests/test_widget.py` & `napari_brainways-0.1.7/src/napari_brainways/_tests/test_widget.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 
 @fixture(params=[0, 1])
 def subject_index(request):
     return request.param
 
 
-STEP_INDICES = [0, 1, 2, 3, 4, 5]
+STEP_INDICES = [0, 1, 2, 3, 4, 5, 6]
 
 
 @fixture(params=STEP_INDICES)
 def step_index(opened_app: BrainwaysUI, request) -> int:
     assert len(STEP_INDICES) == len(opened_app.steps)
     return request.param
 
@@ -95,30 +95,30 @@
     worker = opened_app.run_workflow_async()
     worker_join(worker, qtbot)
 
 
 def test_open_project(
     qtbot: QtBot,
     app: BrainwaysUI,
-    project_path: Path,
+    mock_project: BrainwaysProject,
 ):
     assert app.project is None
-    worker = app.open_project_async(project_path)
+    worker = app.open_project_async(mock_project.path)
     worker_join(worker, qtbot)
     assert isinstance(app.project, BrainwaysProject)
     assert isinstance(app.current_subject, BrainwaysSubject)
 
 
 def test_open_project_without_subjects(
-    qtbot: QtBot, app: BrainwaysUI, project_path: Path
+    qtbot: QtBot, app: BrainwaysUI, mock_project: BrainwaysProject
 ):
-    for subject_dir in project_path.parent.glob("subject*"):
+    for subject_dir in mock_project.path.parent.glob("subject*"):
         shutil.rmtree(subject_dir)
     assert app.project is None
-    worker = app.open_project_async(project_path)
+    worker = app.open_project_async(mock_project.path)
     worker_join(worker, qtbot)
     assert isinstance(app.project, BrainwaysProject)
     assert app._current_valid_subject_index is None
 
 
 def test_set_subject_index_async(
     qtbot: QtBot,
```

### Comparing `napari_brainways-0.1.6.1/src/napari_brainways/brainways_ui.py` & `napari_brainways-0.1.7/src/napari_brainways/brainways_ui.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 from typing import Callable, Optional, Tuple
 
 import napari
 import numpy as np
 from brainways.pipeline.brainways_params import BrainwaysParams
 from brainways.project.brainways_project import BrainwaysProject
 from brainways.project.brainways_subject import BrainwaysSubject
-from brainways.project.info_classes import ExcelMode, SliceInfo
+from brainways.project.info_classes import SliceInfo
 from brainways.utils.cell_detection_importer.cell_detection_importer import (
     CellDetectionImporter,
 )
 from napari.qt.threading import FunctionWorker, GeneratorWorker, create_worker
 from qtpy.QtWidgets import QVBoxLayout, QWidget
 
 from napari_brainways.controllers.affine_2d_controller import Affine2DController
+from napari_brainways.controllers.analysis_controller import AnalysisController
 from napari_brainways.controllers.annotation_viewer_controller import (
     AnnotationViewerController,
 )
 from napari_brainways.controllers.cell_3d_viewer_controller import (
     Cell3DViewerController,
 )
 from napari_brainways.controllers.cell_detector_controller import CellDetectorController
@@ -37,22 +38,24 @@
 
         self.registration_controller = RegistrationController(self)
         self.affine_2d_controller = Affine2DController(self)
         self.tps_controller = TpsController(self)
         self.annotation_viewer_controller = AnnotationViewerController(self)
         self.cell_detector_controller = CellDetectorController(self)
         self.cell_viewer_controller = Cell3DViewerController(self)
+        self.analysis_controller = AnalysisController(self)
 
         self.steps = [
             self.registration_controller,
             self.affine_2d_controller,
             self.tps_controller,
             self.annotation_viewer_controller,
             self.cell_detector_controller,
             self.cell_viewer_controller,
+            self.analysis_controller,
         ]
 
         self.project: Optional[BrainwaysProject] = None
         self._current_valid_subject_index: Optional[int] = None
         self._current_valid_document_index: Optional[int] = None
         self._current_step_index: int = 0
 
@@ -189,15 +192,15 @@
         self._set_title()
 
     def _set_title(self, valid_document_index: Optional[int] = None):
         if valid_document_index is None:
             valid_document_index = self._current_valid_document_index
         _, document = self.current_subject.valid_documents[valid_document_index]
         self.viewer.title = (
-            f"{self.current_subject.subject_path.name} - {document.path}"
+            f"{self.current_subject.subject_info.name} - {document.path}"
         )
 
     def _on_project_opened(self):
         self.widget.on_project_changed(len(self.project.subjects))
         if len(self.project.subjects) > 0:
             self._on_subject_opened()
         self.widget.hide_progress_bar()
@@ -213,45 +216,25 @@
         self.widget.update_enabled_steps()
         self.widget.hide_progress_bar()
 
     def _on_progress_returned(self):
         self.widget.hide_progress_bar()
 
     def persist_current_params(self):
+        assert self.current_step.params is not None
         self.current_document = replace(
             self.current_document, params=self.current_step.params
         )
 
     def save_subject(self, persist: bool = True) -> None:
         if persist:
             self.persist_current_params()
         self.current_subject.save()
         self.project.save()
 
-    def create_excel_async(
-        self,
-        path: Path,
-        min_region_area_um2: Optional[int] = None,
-        cells_per_area_um2: Optional[int] = None,
-        min_cell_size_um: Optional[float] = None,
-        max_cell_size_um: Optional[float] = None,
-        excel_mode: ExcelMode = ExcelMode.ROW_PER_SUBJECT,
-    ) -> FunctionWorker:
-        return self.do_work_async(
-            self.project.create_excel_iter,
-            path=path,
-            min_region_area_um2=min_region_area_um2,
-            cells_per_area_um2=cells_per_area_um2,
-            min_cell_size_um=min_cell_size_um,
-            max_cell_size_um=max_cell_size_um,
-            excel_mode=excel_mode,
-            progress_label="Creating Results Excel...",
-            progress_max_value=len(self.project.subjects),
-        )
-
     def set_subject_index_async(
         self,
         subject_index: int,
         force: bool = False,
         save_current_subject: bool = True,
     ) -> FunctionWorker | None:
         if not force and self._current_valid_subject_index == subject_index:
@@ -464,15 +447,15 @@
         return current_document_index
 
     @property
     def current_valid_document_index(self):
         return self._current_valid_document_index
 
     @property
-    def current_subject(self):
+    def current_subject(self) -> BrainwaysSubject:
         return self.project.subjects[self._current_valid_subject_index]
 
     @current_subject.setter
     def current_subject(self, value: BrainwaysSubject):
         assert self._current_valid_subject_index is not None
         self.project.subjects[self._current_valid_subject_index] = value
```

### Comparing `napari_brainways-0.1.6.1/src/napari_brainways/controllers/_tests/test_affine_2d_controller.py` & `napari_brainways-0.1.7/src/napari_brainways/controllers/_tests/test_affine_2d_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.6.1/src/napari_brainways/controllers/_tests/test_annotation_viewer_controller.py` & `napari_brainways-0.1.7/src/napari_brainways/controllers/_tests/test_annotation_viewer_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.6.1/src/napari_brainways/controllers/_tests/test_cell_3d_viewer_controller.py` & `napari_brainways-0.1.7/src/napari_brainways/controllers/_tests/test_cell_3d_viewer_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.6.1/src/napari_brainways/controllers/_tests/test_tps_controller.py` & `napari_brainways-0.1.7/src/napari_brainways/controllers/_tests/test_tps_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 
 @fixture
 def elastix_mock(
     app_on_tps: Tuple[BrainwaysUI, TpsController],
 ):
     app, controller = app_on_tps
-    elastix_result = deepcopy(controller.params.tps.points_dst)
+    elastix_result = deepcopy(np.array(controller.params.tps.points_dst))
     elastix_result[0, 0] += 1
     with patch(
         "brainways.pipeline.tps.elastix_registration",
         return_value=elastix_result,
     ):
         yield
     print("a")
@@ -52,31 +52,31 @@
 
 def test_run_elastix_updates_params(
     qtbot: QtBot,
     app_on_tps: Tuple[BrainwaysUI, TpsController],
     elastix_mock,
 ):
     app, controller = app_on_tps
-    expected = controller.params.tps.points_dst.copy()
+    expected = np.array(controller.params.tps.points_dst).copy()
     expected[0, 0] -= 1
     worker_join(controller.run_elastix_async(), qtbot)
     numpy.testing.assert_allclose(controller.params.tps.points_dst, expected, atol=0.1)
 
 
 def test_run_elastix_updates_ui(
     qtbot: QtBot,
     app_on_tps: Tuple[BrainwaysUI, TpsController],
     elastix_mock,
 ):
     app, controller = app_on_tps
     expected = controller.params.tps.points_dst.copy()
-    expected[0, 0] -= 1
+    expected[0][0] -= 1
     worker_join(controller.run_elastix_async(), qtbot)
     numpy.testing.assert_allclose(
-        controller.points_atlas_layer.data, expected[:, ::-1], atol=0.1
+        controller.points_atlas_layer.data, np.array(expected)[:, ::-1], atol=0.1
     )
 
 
 @pytest.mark.parametrize("hemisphere", ["left", "right", "both"])
 def test_default_tps_params_uses_hemispheres(
     qtbot: QtBot,
     app_on_tps: Tuple[BrainwaysUI, TpsController],
@@ -119,16 +119,16 @@
     app_on_tps: Tuple[BrainwaysUI, TpsController],
 ):
     app, controller = app_on_tps
     val = controller.points_atlas_layer.data[0, 0]
     modified = val + 1
     controller.points_atlas_layer.data[0, 0] = modified
     controller.on_points_changed()
-    assert isinstance(controller.params.tps.points_dst, np.ndarray)
-    assert isinstance(controller.params.tps.points_dst[0, 0], np.float32)
+    assert isinstance(controller.params.tps.points_dst, list)
+    assert isinstance(controller.params.tps.points_dst[0][0], float)
 
 
 def test_reset_params(
     qtbot: QtBot,
     app_on_tps: Tuple[BrainwaysUI, TpsController],
 ):
     app, controller = app_on_tps
```

### Comparing `napari_brainways-0.1.6.1/src/napari_brainways/controllers/affine_2d_controller.py` & `napari_brainways-0.1.7/src/napari_brainways/controllers/affine_2d_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,14 @@
             self.atlas_slice_layer.scale = (self.display_scale, self.display_scale)
             self.widget.set_ranges(
                 tx=(-image.shape[1], image.shape[1]),
                 ty=(-image.shape[0], image.shape[0]),
             )
             self.input_layer.data = image
             update_layer_contrast_limits(self.input_layer)
-            self.ui.viewer.reset_view()
 
         if not from_ui:
             self.widget.set_params(
                 angle=params.affine.angle,
                 tx=params.affine.tx,
                 ty=params.affine.ty,
                 sx=params.affine.sx,
@@ -161,14 +160,16 @@
             params=params,
             until_step=PipelineStep.AFFINE_2D,
             scale=self.display_scale,
         )
 
         self.input_layer.data = registered_image
 
+        self.ui.viewer.reset_view()
+
         # transform = self.pipeline.get_image_to_atlas_transform(
         #     brainways_params=params,
         #     lowres_image_size=self._image.shape,
         #     until_step=PipelineStep.AFFINE_2D,
         # )
         #
         # transformed_atlas_slice = transform.inv().transform_image(
```

### Comparing `napari_brainways-0.1.6.1/src/napari_brainways/controllers/annotation_viewer_controller.py` & `napari_brainways-0.1.7/src/napari_brainways/controllers/annotation_viewer_controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             np.zeros((10, 10), np.int32), name="Annotations"
         )
         self.annotations_layer.mouse_move_callbacks.append(self.on_mouse_move)
         self._is_open = True
 
     def on_mouse_move(self, _layer, event):
         struct_id = self.annotations_layer.get_value(event.position, world=True)
-        if struct_id:
+        if struct_id and struct_id in self.pipeline.atlas.brainglobe_atlas.structures:
             struct_name = self.pipeline.atlas.brainglobe_atlas.structures[struct_id][
                 "name"
             ]
         else:
             struct_name = ""
         _layer.help = struct_name
```

### Comparing `napari_brainways-0.1.6.1/src/napari_brainways/controllers/base.py` & `napari_brainways-0.1.7/src/napari_brainways/controllers/base.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.6.1/src/napari_brainways/controllers/cell_3d_viewer_controller.py` & `napari_brainways-0.1.7/src/napari_brainways/controllers/cell_3d_viewer_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,46 +28,45 @@
         self._image: np.ndarray | None = None
         self._atlas: BrainwaysAtlas | None = None
         # TODO: ability to switch between modes
         self._3d_view_mode = False
         self.widget = CellViewerWidget(self)
 
     def set_2d_mode(self):
+        if not self._3d_view_mode:
+            return
         self._3d_view_mode = False
         self.show(params=self._params, image=self._image)
 
     def set_3d_mode(self):
+        if self._3d_view_mode:
+            return
         self._3d_view_mode = True
         self.show(params=self._params, image=self._image)
 
     def open(self) -> None:
         if self._is_open:
             return
 
         self._atlas = self.ui.project.atlas
-        self.input_layer = self.ui.viewer.add_image(np.zeros((10, 10)), name="Image")
-        self.atlas_layer = self.ui.viewer.add_image(
-            self._atlas.reference.numpy(),
-            name="Atlas",
-            rendering="attenuated_mip",
-            attenuation=0.5,
-        )
         self.points_layer = self.ui.viewer.add_points(
             size=1, ndim=3, name="Detected Cells"
         )
         self.ui.viewer.dims.ndisplay = 3
         self.ui.viewer.reset_view()
         self._is_open = True
 
     def close(self) -> None:
         if not self._is_open:
             return
 
-        self.ui.viewer.layers.remove(self.input_layer)
-        self.ui.viewer.layers.remove(self.atlas_layer)
+        if self._3d_view_mode:
+            self.ui.viewer.layers.remove(self.atlas_layer)
+        else:
+            self.ui.viewer.layers.remove(self.input_layer)
         self.ui.viewer.layers.remove(self.points_layer)
         self.atlas_layer = None
         self.points_layer = None
         self.ui.viewer.dims.ndisplay = 2
         self._atlas = None
         self._params = None
         self._image = None
@@ -85,16 +84,23 @@
 
         if self._3d_view_mode:
             self.show_3d()
         else:
             self.show_2d(image=self._image, from_ui=from_ui)
 
     def show_3d(self):
-        self.input_layer.visible = False
-        self.atlas_layer.visible = True
+        if self.input_layer is not None:
+            self.ui.viewer.layers.remove(self.input_layer)
+            self.input_layer = None
+        self.atlas_layer = self.ui.viewer.add_image(
+            self._atlas.reference.numpy(),
+            name="Atlas",
+            rendering="attenuated_mip",
+            attenuation=0.5,
+        )
         self.ui.viewer.dims.ndisplay = 3
 
         self.ui.viewer.layers.remove(self.points_layer)
         self.points_layer = self.ui.viewer.add_points(
             size=1, ndim=3, name="Detected Cells"
         )
 
@@ -107,34 +113,36 @@
             self.points_layer.data = all_cells[["z", "y", "x"]].values
             self.points_layer.face_color = colors
             self.points_layer.edge_color = colors
             self.points_layer.selected_data = set()
         else:
             self.points_layer.data = []
 
+        self.ui.viewer.reset_view()
+
     def show_2d(self, image: np.ndarray | None = None, from_ui: bool = False):
         if image is None:
             return
 
-        self.input_layer.visible = True
-        self.atlas_layer.visible = False
+        if self.atlas_layer is not None:
+            self.ui.viewer.layers.remove(self.atlas_layer)
+            self.atlas_layer = None
+        self.input_layer = self.ui.viewer.add_image(image, name="Image")
+        update_layer_contrast_limits(self.input_layer)
         self.ui.viewer.dims.ndisplay = 2
 
         self.ui.viewer.layers.remove(self.points_layer)
         self.points_layer = self.ui.viewer.add_points(
             size=max(image.shape) * 0.002, ndim=2, name="Detected Cells"
         )
 
         subject = self.ui.current_subject
         document = self.ui.current_document
 
-        # TODO: read image from disk with options for highres and other channels
-        self.input_layer.data = image
-        update_layer_contrast_limits(self.input_layer)
-        self.ui.viewer.reset_view()
+        # TODO: read image from disk with options for other channels
 
         cells_atlas = subject.get_cells_on_atlas([document])
         if cells_atlas is not None:
             cells = subject.get_valid_cells(document)
             # TODO: get struct ids from annotation, not from brainglobe
             struct_ids = get_cell_struct_ids(
                 cells_atlas, subject.atlas.brainglobe_atlas
@@ -144,14 +152,16 @@
             self.points_layer.data = cell_xy
             self.points_layer.face_color = colors
             self.points_layer.edge_color = colors
             self.points_layer.selected_data = set()
         else:
             self.points_layer.data = []
 
+        self.ui.viewer.reset_view()
+
     def default_params(
         self, image: np.ndarray, params: BrainwaysParams
     ) -> BrainwaysParams:
         return params
 
     @staticmethod
     def has_current_step_params(params: BrainwaysParams) -> bool:
@@ -182,8 +192,8 @@
 
     @property
     def params(self) -> BrainwaysParams:
         return self._params
 
     @property
     def name(self) -> str:
-        return "3D Cell Viewer"
+        return "Cell Viewer"
```

### Comparing `napari_brainways-0.1.6.1/src/napari_brainways/controllers/cell_detector_controller.py` & `napari_brainways-0.1.7/src/napari_brainways/controllers/cell_detector_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,15 +295,15 @@
 
         highres_crop = (
             self.ui.current_document.image_reader()
             .get_image_dask_data(
                 "YX",
                 X=slice(x0, x1),
                 Y=slice(y0, y1),
-                C=self.ui.current_subject.settings.channel,
+                C=self.ui.project.settings.channel,
             )
             .compute()
         )
 
         # if self._params.cell is not None:
         #     cell_detector_params = self._params.cell
         # else:
```

### Comparing `napari_brainways-0.1.6.1/src/napari_brainways/controllers/registration_controller.py` & `napari_brainways-0.1.7/src/napari_brainways/controllers/registration_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.6.1/src/napari_brainways/controllers/tps_controller.py` & `napari_brainways-0.1.7/src/napari_brainways/controllers/tps_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,19 +97,19 @@
 
             atlas_slice = self.pipeline.get_atlas_slice(params)
             self.atlas_layer.data = atlas_slice.annotation.numpy()
             self.atlas_layer.scale = (display_scale, display_scale)
             self.points_input_layer.scale = (display_scale, display_scale)
             self.points_atlas_layer.scale = (display_scale, display_scale)
         with self.points_input_layer.events.data.blocker():
-            np_pts = params.tps.points_src[:, ::-1]
+            np_pts = np.array(params.tps.points_src)[:, ::-1]
             self.points_input_layer.data = np_pts.copy()
             self.points_input_layer.selected_data = set()
         with self.points_atlas_layer.events.data.blocker():
-            np_pts = params.tps.points_dst[:, ::-1]
+            np_pts = np.array(params.tps.points_dst)[:, ::-1]
             self.points_atlas_layer.data = np_pts.copy()
             self.points_atlas_layer.selected_data = set()
 
         self.input_layer.data = self.pipeline.transform_image(
             image=self._image,
             params=params,
             until_step=PipelineStep.TPS,
@@ -211,16 +211,16 @@
             self.points_input_layer.add(point_to_add_transformed[0, ::-1])
             self.points_atlas_layer.mode = "select"
 
         points_src = self.points_input_layer.data[:, ::-1]
         points_dst = self.points_atlas_layer.data[:, ::-1]
 
         tps_params = TPSTransformParams(
-            points_src=points_src.astype(np.float32),
-            points_dst=points_dst.astype(np.float32),
+            points_src=points_src.astype(np.float32).tolist(),
+            points_dst=points_dst.astype(np.float32).tolist(),
         )
         updated_params = replace(self._params, tps=tps_params)
         self.show(params=updated_params, from_ui=True)
 
     def _run_elastix(self) -> BrainwaysParams:
         return self.run_model(self._image, self._params)
```

### Comparing `napari_brainways-0.1.6.1/src/napari_brainways/napari.yaml` & `napari_brainways-0.1.7/src/napari_brainways/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.6.1/src/napari_brainways/napari_reader.py` & `napari_brainways-0.1.7/src/napari_brainways/napari_reader.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.6.1/src/napari_brainways/resources/logo.png` & `napari_brainways-0.1.7/src/napari_brainways/resources/logo.png`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.6.1/src/napari_brainways/test_utils.py` & `napari_brainways-0.1.7/src/napari_brainways/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
         modified_atlas = replace(params.atlas, ap=random.uniform(0, 1))
     if params.affine is not None:
         modified_affine = replace(
             params.affine, angle=random.randint(10, 90), sx=0.5, sy=0.5
         )
     if params.tps is not None:
         modified_tps = TPSTransformParams(
-            np.random.randint(10, size=(10, 2)),
-            np.random.randint(10, size=(10, 2)),
+            np.random.randint(10, size=(10, 2)).tolist(),
+            np.random.randint(10, size=(10, 2)).tolist(),
         )
     if params.cell is not None:
         modified_cell = replace(params.cell, diameter=random.randint(0, 100))
     modified_params = BrainwaysParams(
         atlas=modified_atlas,
         affine=modified_affine,
         tps=modified_tps,
```

### Comparing `napari_brainways-0.1.6.1/src/napari_brainways/utils.py` & `napari_brainways-0.1.7/src/napari_brainways/utils.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.6.1/src/napari_brainways/widgets/_tests/test_registration_widget.py` & `napari_brainways-0.1.7/src/napari_brainways/widgets/_tests/test_registration_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.6.1/src/napari_brainways/widgets/affine_2d_widget.py` & `napari_brainways-0.1.7/src/napari_brainways/widgets/affine_2d_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.6.1/src/napari_brainways/widgets/cell_detector_widget.py` & `napari_brainways-0.1.7/src/napari_brainways/widgets/cell_detector_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.6.1/src/napari_brainways/widgets/cell_viewer_widget.py` & `napari_brainways-0.1.7/src/napari_brainways/widgets/cell_viewer_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.6.1/src/napari_brainways/widgets/create_subject_dialog.py` & `napari_brainways-0.1.7/src/napari_brainways/widgets/create_subject_dialog.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import functools
 from dataclasses import replace
 from pathlib import Path
-from typing import List, Optional, Tuple
+from typing import Dict, List, Optional, Tuple
 
 import numpy as np
 from brainways.project.brainways_project import BrainwaysProject
-from brainways.project.info_classes import SliceInfo
+from brainways.project.brainways_subject import BrainwaysSubject
+from brainways.project.info_classes import SliceInfo, SubjectInfo
 from brainways.utils.image import resize_image
 from brainways.utils.io_utils import ImagePath
 from brainways.utils.io_utils.readers import get_channels, get_scenes
+from magicgui import widgets
 from napari.qt.threading import FunctionWorker, create_worker
 from qtpy import QtCore
 from qtpy.QtGui import QImage, QPixmap
 from qtpy.QtWidgets import (
     QAbstractItemView,
     QCheckBox,
     QComboBox,
@@ -30,30 +32,36 @@
 
 
 class CreateSubjectDialog(QDialog):
     def __init__(self, project: BrainwaysProject, parent: Optional[QWidget] = None):
         super().__init__(parent)
 
         self.project = project
+        self.subject: Optional[BrainwaysSubject] = None
         self._add_documents_worker: Optional[FunctionWorker] = None
         self.create_subject_button = QPushButton("&Create", self)
         self.create_subject_button.clicked.connect(self.on_create_subject_clicked)
         self.channels_combobox = QComboBox()
         self.add_images_button = QPushButton("&Add Image(s)...", self)
         self.add_images_button.clicked.connect(self.on_add_images_clicked)
         self.files_table = self.create_table()
+        self.conditions_widget = self._create_conditions_widget()
         self.bottom_label = QLabel("")
 
         self.layout = QGridLayout(self)
         self.setLayout(self.layout)
 
         cur_row = 0
         self.layout.addWidget(QLabel("Channel:"), cur_row, 0)
         self.layout.addWidget(self.channels_combobox, cur_row, 1)
 
+        if self.project.settings.condition_names:
+            cur_row += 1
+            self.layout.addWidget(self.conditions_widget.native, cur_row, 0, 1, 3)
+
         cur_row += 1
         self.layout.addWidget(self.files_table, cur_row, 0, 1, 3)
 
         cur_row += 1
         self.layout.addWidget(self.bottom_label, cur_row, 0, 1, 2)
 
         cur_row += 1
@@ -69,34 +77,62 @@
                 int(parent.parent().parent().parent().height() * 0.8),
             )
 
     def edit_subject_async(
         self, subject_index: int, document_index: int
     ) -> FunctionWorker:
         self.setWindowTitle("Edit Subject")
-        self.subject = self.project.subjects[subject_index]
+        self._set_subject(self.project.subjects[subject_index])
         self.create_subject_button.setText("Done")
         return self.add_document_rows_async(
             documents=self.subject.documents, select_document_index=document_index
         )
 
-    def new_subject(self, subject_id: str):
+    def new_subject(self, subject_id: str, conditions: Dict[str, str]):
         assert subject_id is not None
         self.setWindowTitle(f"New Subject ({subject_id})")
-        self.subject = self.project.add_subject(id=subject_id)
+        self._set_subject(
+            self.project.add_subject(
+                SubjectInfo(name=subject_id, conditions=conditions)
+            )
+        )
+
+    def _set_subject(self, subject: BrainwaysSubject):
+        self.subject = subject
+        for index, condition in enumerate(self.project.settings.condition_names):
+            self.conditions_widget[index].value = subject.subject_info.conditions.get(
+                condition, ""
+            )
+            self.conditions_widget[index].changed.disconnect()
+            self.conditions_widget[index].changed.connect(
+                self._get_set_condition_callback(subject=subject, condition=condition)
+            )
+
+    def _get_set_condition_callback(self, subject: BrainwaysSubject, condition: str):
+        def __set_condition(value: str):
+            subject.subject_info.conditions[condition] = value
+
+        return __set_condition
 
     def create_table(self) -> QTableWidget:
         table = QTableWidget(0, 4)
         table.setSelectionBehavior(QAbstractItemView.SelectionBehavior.SelectRows)
         table.setHorizontalHeaderLabels(["", "Thumbnail", "Path", "Scene"])
         table.horizontalHeader().setSectionResizeMode(2, QHeaderView.Stretch)
         table.verticalHeader().hide()
         table.setShowGrid(False)
         return table
 
+    def _create_conditions_widget(self) -> widgets.Widget:
+        condition_widgets = [
+            widgets.LineEdit(label=condition)
+            for condition in self.project.settings.condition_names
+        ]
+        return widgets.Container(widgets=condition_widgets)
+
     def add_filenames_async(self, filenames: List[str]) -> FunctionWorker:
         progress = QProgressDialog(
             "Loading image scenes...", "Cancel", 0, len(filenames), self
         )
         progress.setModal(True)
         progress.setValue(0)
         progress.setWindowTitle("Loading...")
@@ -169,15 +205,15 @@
         )
         progress.setModal(True)
         progress.setValue(0)
         progress.setWindowTitle("Loading...")
         progress.show()
 
         def on_work_returned():
-            self.channels_combobox.setCurrentIndex(self.subject.settings.channel)
+            self.channels_combobox.setCurrentIndex(self.project.settings.channel)
             if select_document_index is not None:
                 self.files_table.selectRow(select_document_index)
             progress.close()
 
         def on_work_yielded(result: Tuple[SliceInfo, np.ndarray]):
             document, thumbnail = result
             row = self.files_table.rowCount()
@@ -238,15 +274,15 @@
         self.files_table.setCellWidget(
             document_index, 1, self.get_image_widget(thumbnail)
         )
         self.subject.documents[document_index] = document
 
     def on_selected_channel_changed(self, _=None):
         new_channel = int(self.channels_combobox.currentIndex())
-        self.subject.settings = replace(self.subject.settings, channel=new_channel)
+        self.project.settings = replace(self.project.settings, channel=new_channel)
         self.files_table.setRowCount(0)
         self.add_document_rows_async(self.subject.documents)
 
     def on_add_images_clicked(self, _=None):
         filenames, _ = QFileDialog.getOpenFileNames(
             self,
             "Add Image(s)",
```

### Comparing `napari_brainways-0.1.6.1/src/napari_brainways/widgets/registration_widget.py` & `napari_brainways-0.1.7/src/napari_brainways/widgets/registration_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.6.1/src/napari_brainways/widgets/tps_widget.py` & `napari_brainways-0.1.7/src/napari_brainways/widgets/tps_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.6.1/src/napari_brainways/widgets/workflow_widget.py` & `napari_brainways-0.1.7/src/napari_brainways/widgets/workflow_widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 
 import functools
 import os
+from dataclasses import replace
 from pathlib import Path
 from typing import Callable, List, Union
 
 import importlib_resources
 import PIL.Image
 from bg_atlasapi.list_atlases import get_all_atlases_lastversions
 from brainways.pipeline.brainways_params import BrainwaysParams
 from brainways.project.brainways_project import BrainwaysProject
-from brainways.project.info_classes import ExcelMode, ProjectSettings
+from brainways.project.info_classes import ProjectSettings
 from brainways.utils.cell_detection_importer.utils import (
     cell_detection_importer_types,
     get_cell_detection_importer,
 )
 from magicgui import magicgui
 from magicgui.widgets import Image, request_values
 from qtpy.QtCore import Qt
@@ -41,27 +42,27 @@
         super().__init__(controller)
         self.controller = controller
         self.steps = steps
         self._prev_path = str(Path.home())
 
         self.project_buttons = ProjectButtons(
             open_project=self.on_open_project_clicked,
-            edit_project=self.on_edit_subject_clicked,
+            edit_project=self.on_edit_project_clicked,
             new_project=self.on_create_project_clicked,
         )
         self.project_actions_section = ProjectActionsSection(
-            export_excel=self.on_export_clicked,
             import_cells=self.on_import_cells_clicked,
             run_cell_detector=self.on_run_cell_detector_clicked,
         )
         self.subject_navigation = SubjectControls(
             select_callback=self.select_subject,
             prev_callback=self.controller.prev_subject,
             next_callback=self.controller.next_subject,
             add_subject_callback=self.on_add_subject_clicked,
+            edit_subject_callback=self.on_edit_subject_clicked,
             visible=False,
         )
         self.image_navigation = NavigationControls(
             title="<b>Select Image:</b> [b/n]",
             label="Image",
             select_callback=self.select_image,
             prev_callback=self.controller.prev_image,
@@ -133,37 +134,62 @@
         user_values = request_values(
             title="New Brainways Project",
             atlas=dict(
                 value="whs_sd_rat_39um",
                 widget_type="ComboBox",
                 options=dict(choices=available_atlases),
                 annotation=str,
-                label="Importer Type",
+                label="Atlas",
+            ),
+            condition_names=dict(
+                value="condition1;condition2",
+                annotation=str,
+                label="Conditions",
             ),
         )
         if user_values is None:
             return
 
-        atlas = user_values["atlas"]
-
-        settings = ProjectSettings(atlas=atlas, channel=0)
+        settings = ProjectSettings(
+            atlas=user_values["atlas"],
+            channel=0,
+            condition_names=user_values["condition_names"].split(";"),
+        )
         project = BrainwaysProject.create(path=path, settings=settings, lazy_init=True)
         self.controller.open_project_async(project.path)
 
+    def on_edit_project_clicked(self, _=None):
+        settings: ProjectSettings = self.controller.project.settings
+        user_values = request_values(
+            title="Edit Brainways Project",
+            condition_names=dict(
+                value=";".join(settings.condition_names),
+                annotation=str,
+                label="Conditions",
+            ),
+        )
+        if user_values is None:
+            return
+
+        self.controller.project.settings = replace(
+            settings, condition_names=user_values["condition_names"].split(";")
+        )
+        self.controller.project.save()
+
     def on_add_subject_clicked(self, _=None):
         values = request_values(
             subject_id=dict(annotation=str, label="Subject ID:"),
             title="New Subject",
         )
         if values is None or values["subject_id"] == "":
             return
 
         subject_id = values["subject_id"]
         dialog = CreateSubjectDialog(project=self.controller.project, parent=self)
-        dialog.new_subject(subject_id)
+        dialog.new_subject(subject_id=subject_id, conditions={})
         result = dialog.exec()
         if result == QDialog.DialogCode.Rejected:
             return
         subject_index = self.controller.project.subjects.index(dialog.subject)
         self.on_project_changed(n_subjects=len(self.controller.project))
         self.controller.set_subject_index_async(subject_index)
 
@@ -229,90 +255,14 @@
 
     def on_run_workflow_clicked(self, _=None):
         self.controller.run_workflow_async()
 
     def on_save_button_clicked(self, _=None):
         self.controller.save_subject()
 
-    def on_export_clicked(self, _=None):
-        kwargs = {}
-        if "SNAP" in os.environ:
-            kwargs["options"] = QFileDialog.DontUseNativeDialog
-
-        path, _ = QFileDialog.getSaveFileName(
-            self,
-            "Export Results",
-            self._prev_path,
-            "XLSX File (*.xlsx)",
-            **kwargs,
-        )
-        if path == "":
-            return
-        self._prev_path = str(Path(path).parent)
-
-        values = request_values(
-            title="Excel Parameters",
-            excel_mode=dict(
-                value=ExcelMode.ROW_PER_SUBJECT,
-                annotation=ExcelMode,
-                label="Excel Mode",
-                options=dict(
-                    tooltip=(
-                        "Output a row per subject or row per image (useful for "
-                        "error analysis)"
-                    )
-                ),
-            ),
-            min_region_area_um2=dict(
-                value=250,
-                annotation=int,
-                label="Min Structure Square Area (μm)",
-                options=dict(
-                    tooltip="Filter out structures with an area smaller than this value"
-                ),
-            ),
-            cells_per_area_um2=dict(
-                value=250,
-                annotation=int,
-                label="Cells Per Square Area (μm)",
-                options=dict(
-                    tooltip="Normalize number of cells to number of cells per area unit"
-                ),
-            ),
-            min_cell_size_um=dict(
-                value=0,
-                annotation=int,
-                label="Min Cell Area (μm)",
-                options=dict(
-                    tooltip=(
-                        "Filter out detected cells with area smaller than this value"
-                    )
-                ),
-            ),
-            max_cell_size_um=dict(
-                value=0,
-                annotation=int,
-                label="Max Cell Area (μm)",
-                options=dict(
-                    tooltip="Filter out detected cells with area larger than this value"
-                ),
-            ),
-        )
-        if values is None:
-            return
-
-        self.controller.create_excel_async(
-            Path(path),
-            min_region_area_um2=values["min_region_area_um2"],
-            cells_per_area_um2=values["cells_per_area_um2"],
-            min_cell_size_um=values["min_cell_size_um"],
-            max_cell_size_um=values["max_cell_size_um"],
-            excel_mode=values["excel_mode"],
-        )
-
     def on_import_cells_clicked(self, _=None):
         kwargs = {}
         if "SNAP" in os.environ:
             kwargs["options"] = QFileDialog.DontUseNativeDialog
 
         path = QFileDialog.getExistingDirectory(
             self,
@@ -446,29 +396,26 @@
     def project_closed(self):
         self.edit_project.setVisible(False)
 
 
 class ProjectActionsSection(TitledGroupBox):
     def __init__(
         self,
-        export_excel: Callable,
         import_cells: Callable,
         run_cell_detector: Callable,
     ):
-        self.export_excel = QPushButton("Create Results Excel")
         self.import_cells = QPushButton("Import Cell Detections")
         self.run_cell_detector = QPushButton("Run Cell Detector")
 
-        self.export_excel.clicked.connect(export_excel)
         self.import_cells.clicked.connect(import_cells)
         self.run_cell_detector.clicked.connect(run_cell_detector)
 
         super().__init__(
             title="<b>Project Actions:</b>",
-            widgets=[self.export_excel, self.run_cell_detector, self.import_cells],
+            widgets=[self.run_cell_detector, self.import_cells],
         )
 
 
 class NavigationControls(TitledGroupBox):
     def __init__(
         self,
         title: str,
@@ -543,44 +490,50 @@
 class SubjectControls(NavigationControls):
     def __init__(
         self,
         select_callback: Callable,
         prev_callback: Callable,
         next_callback: Callable,
         add_subject_callback: Callable,
+        edit_subject_callback: Callable,
         visible: bool = True,
     ):
         self.add_subject_button = QPushButton("Add Subject")
         self.add_subject_button.clicked.connect(add_subject_callback)
 
+        self.edit_subject_button = QPushButton("Edit Subject")
+        self.edit_subject_button.clicked.connect(edit_subject_callback)
+
         super().__init__(
             title="<b>Select Subject:</b> [B/N]",
             label="Subject",
             select_callback=select_callback,
             prev_callback=prev_callback,
             next_callback=next_callback,
             visible=visible,
         )
 
     def _build_layout(self) -> List[QWidget]:
         widgets = super()._build_layout()
         widgets.append(self.add_subject_button)
+        widgets.append(self.edit_subject_button)
         return widgets
 
     def project_opened(self, n_subjects: int):
         self.visible = True
         if n_subjects == 0:
             navigation_visible = False
         else:
             self.max = n_subjects
             navigation_visible = True
 
         self.selector_widget.visible = navigation_visible
         self.next_button.setVisible(navigation_visible)
         self.prev_button.setVisible(navigation_visible)
+        self.edit_subject_button.setVisible(navigation_visible)
 
     def project_closed(self, n_subjects: int):
         self.visible = False
 
 
 class StepButtons(TitledGroupBox):
     def __init__(self, steps: List[Controller], clicked: Callable, title: str):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `napari_brainways-0.1.6.1/src/napari_brainways.egg-info/PKG-INFO` & `napari_brainways-0.1.7/src/napari_brainways.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-brainways
-Version: 0.1.6.1
+Version: 0.1.7
 Summary: Brainways UI
 Home-page: https://github.com/bkntr/napari-brainways
 Author: Ben Kantor
 Author-email: benkantor@mail.tau.ac.il
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/bkntr/napari-brainways/issues
 Project-URL: Documentation, https://github.com/bkntr/napari-brainways#README.md
```

### Comparing `napari_brainways-0.1.6.1/src/napari_brainways.egg-info/SOURCES.txt` & `napari_brainways-0.1.7/src/napari_brainways.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 src/napari_brainways.egg-info/top_level.txt
 src/napari_brainways/_tests/__init__.py
 src/napari_brainways/_tests/test_reader.py
 src/napari_brainways/_tests/test_sample_data.py
 src/napari_brainways/_tests/test_widget.py
 src/napari_brainways/controllers/__init__.py
 src/napari_brainways/controllers/affine_2d_controller.py
+src/napari_brainways/controllers/analysis_controller.py
 src/napari_brainways/controllers/annotation_viewer_controller.py
 src/napari_brainways/controllers/base.py
 src/napari_brainways/controllers/cell_3d_viewer_controller.py
 src/napari_brainways/controllers/cell_detector_controller.py
 src/napari_brainways/controllers/registration_controller.py
 src/napari_brainways/controllers/tps_controller.py
 src/napari_brainways/controllers/_tests/test_affine_2d_controller.py
@@ -42,14 +43,15 @@
 src/napari_brainways/controllers/_tests/test_cell_3d_viewer_controller.py
 src/napari_brainways/controllers/_tests/test_cell_detector_controller.py
 src/napari_brainways/controllers/_tests/test_registration_controller.py
 src/napari_brainways/controllers/_tests/test_tps_controller.py
 src/napari_brainways/resources/logo.png
 src/napari_brainways/widgets/__init__.py
 src/napari_brainways/widgets/affine_2d_widget.py
+src/napari_brainways/widgets/analysis_widget.py
 src/napari_brainways/widgets/cell_detector_widget.py
 src/napari_brainways/widgets/cell_viewer_widget.py
 src/napari_brainways/widgets/create_subject_dialog.py
 src/napari_brainways/widgets/registration_widget.py
 src/napari_brainways/widgets/tps_widget.py
 src/napari_brainways/widgets/workflow_widget.py
 src/napari_brainways/widgets/_tests/__init__.py
```

### Comparing `napari_brainways-0.1.6.1/tox.ini` & `napari_brainways-0.1.7/tox.ini`

 * *Files identical despite different names*


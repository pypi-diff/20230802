# Comparing `tmp/brainways-0.1.6.tar.gz` & `tmp/brainways-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainways-0.1.6.tar", last modified: Thu Jun 15 09:13:26 2023, max compression
+gzip compressed data, was "brainways-0.1.7.tar", last modified: Wed Aug  2 08:49:47 2023, max compression
```

## Comparing `brainways-0.1.6.tar` & `brainways-0.1.7.tar`

### file list

```diff
@@ -1,188 +1,195 @@
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.988741 brainways-0.1.6/
--rw-rw-r--   0 ben       (1001) ben       (1001)      292 2022-07-13 13:47:58.000000 brainways-0.1.6/.editorconfig
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.972741 brainways-0.1.6/.github/
--rw-rw-r--   0 ben       (1001) ben       (1001)      320 2022-07-13 13:47:58.000000 brainways-0.1.6/.github/ISSUE_TEMPLATE.md
--rw-rw-r--   0 ben       (1001) ben       (1001)     1248 2022-07-13 14:46:16.000000 brainways-0.1.6/.gitignore
--rw-rw-r--   0 ben       (1001) ben       (1001)     1194 2022-07-14 13:50:01.000000 brainways-0.1.6/.pre-commit-config.yaml
--rw-rw-r--   0 ben       (1001) ben       (1001)      681 2022-07-13 13:47:58.000000 brainways-0.1.6/.travis.yml
--rw-rw-r--   0 ben       (1001) ben       (1001)      160 2022-07-13 13:47:58.000000 brainways-0.1.6/AUTHORS.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     3523 2022-07-13 13:47:58.000000 brainways-0.1.6/CONTRIBUTING.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)       89 2022-07-13 13:47:58.000000 brainways-0.1.6/HISTORY.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)    35148 2022-08-24 08:26:24.000000 brainways-0.1.6/LICENSE
--rw-rw-r--   0 ben       (1001) ben       (1001)      262 2022-07-13 13:47:58.000000 brainways-0.1.6/MANIFEST.in
--rw-rw-r--   0 ben       (1001) ben       (1001)     2430 2023-05-26 08:21:13.000000 brainways-0.1.6/Makefile
--rw-rw-r--   0 ben       (1001) ben       (1001)     2343 2023-06-15 09:13:26.988741 brainways-0.1.6/PKG-INFO
--rw-rw-r--   0 ben       (1001) ben       (1001)      962 2023-05-26 08:25:05.000000 brainways-0.1.6/README.rst
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.972741 brainways-0.1.6/data/
--rw-rw-r--   0 ben       (1001) ben       (1001)   269441 2022-03-11 09:30:01.000000 brainways-0.1.6/data/test_data.npz
--rw-rw-r--   0 ben       (1001) ben       (1001)    47973 2022-06-30 11:17:43.000000 brainways-0.1.6/data/test_image.jpg
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.972741 brainways-0.1.6/docs/
--rw-rw-r--   0 ben       (1001) ben       (1001)      610 2022-07-13 13:47:58.000000 brainways-0.1.6/docs/Makefile
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.968741 brainways-0.1.6/docs/_build/
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.968741 brainways-0.1.6/docs/_build/html/
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.972741 brainways-0.1.6/docs/_build/html/_static/
--rw-rw-r--   0 ben       (1001) ben       (1001)      286 2022-10-06 11:03:00.000000 brainways-0.1.6/docs/_build/html/_static/file.png
--rw-rw-r--   0 ben       (1001) ben       (1001)       90 2022-10-06 11:03:00.000000 brainways-0.1.6/docs/_build/html/_static/minus.png
--rw-rw-r--   0 ben       (1001) ben       (1001)       90 2022-10-06 11:03:00.000000 brainways-0.1.6/docs/_build/html/_static/plus.png
--rw-rw-r--   0 ben       (1001) ben       (1001)       28 2022-07-13 13:47:58.000000 brainways-0.1.6/docs/authors.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      361 2023-05-26 08:18:55.000000 brainways-0.1.6/docs/brainways.elastix.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     1317 2023-05-26 08:18:55.000000 brainways-0.1.6/docs/brainways.pipeline.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      770 2023-05-26 08:18:55.000000 brainways-0.1.6/docs/brainways.project.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      500 2023-05-26 08:26:43.000000 brainways-0.1.6/docs/brainways.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     2137 2023-05-26 08:18:55.000000 brainways-0.1.6/docs/brainways.scripts.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     1387 2023-05-26 08:18:55.000000 brainways-0.1.6/docs/brainways.transforms.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      601 2023-05-26 08:18:55.000000 brainways-0.1.6/docs/brainways.utils.atlas.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     1405 2023-05-26 08:18:55.000000 brainways-0.1.6/docs/brainways.utils.cell_detection_importer.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      386 2023-05-26 08:18:55.000000 brainways-0.1.6/docs/brainways.utils.czi.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      971 2023-05-26 08:18:55.000000 brainways-0.1.6/docs/brainways.utils.io_utils.file_iterators.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     1145 2023-05-26 08:18:55.000000 brainways-0.1.6/docs/brainways.utils.io_utils.readers.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      553 2023-05-26 08:18:55.000000 brainways-0.1.6/docs/brainways.utils.io_utils.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     1833 2023-05-26 08:18:55.000000 brainways-0.1.6/docs/brainways.utils.rst
--rwxrwxr-x   0 ben       (1001) ben       (1001)     4967 2023-05-26 08:17:55.000000 brainways-0.1.6/docs/conf.py
--rw-rw-r--   0 ben       (1001) ben       (1001)       33 2022-07-13 13:47:58.000000 brainways-0.1.6/docs/contributing.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)       28 2022-07-13 13:47:58.000000 brainways-0.1.6/docs/history.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      306 2022-07-13 13:47:58.000000 brainways-0.1.6/docs/index.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     1118 2022-07-13 13:47:58.000000 brainways-0.1.6/docs/installation.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      807 2022-07-13 13:47:58.000000 brainways-0.1.6/docs/make.bat
--rw-rw-r--   0 ben       (1001) ben       (1001)       64 2023-05-26 08:26:43.000000 brainways-0.1.6/docs/modules.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)       27 2022-07-13 13:47:58.000000 brainways-0.1.6/docs/readme.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)       73 2022-07-13 13:47:58.000000 brainways-0.1.6/docs/usage.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      383 2023-05-26 08:03:19.000000 brainways-0.1.6/pyproject.toml
--rw-rw-r--   0 ben       (1001) ben       (1001)      165 2022-07-13 14:08:33.000000 brainways-0.1.6/requirements_dev.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)     1967 2023-06-15 09:13:26.988741 brainways-0.1.6/setup.cfg
--rw-rw-r--   0 ben       (1001) ben       (1001)       60 2023-05-26 07:59:05.000000 brainways-0.1.6/setup.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.968741 brainways-0.1.6/src/
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.972741 brainways-0.1.6/src/brainways/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-13 14:28:10.000000 brainways-0.1.6/src/brainways/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      160 2023-06-15 09:13:26.000000 brainways-0.1.6/src/brainways/_version.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     7627 2023-06-14 09:09:25.000000 brainways-0.1.6/src/brainways/conftest.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.976741 brainways-0.1.6/src/brainways/elastix/
--rw-rw-r--   0 ben       (1001) ben       (1001)     2596 2022-07-14 13:40:58.000000 brainways-0.1.6/src/brainways/elastix/Par0033bspline.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)     2316 2022-07-14 13:40:58.000000 brainways-0.1.6/src/brainways/elastix/Par0033similarity.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-12-09 12:20:50.000000 brainways-0.1.6/src/brainways/elastix/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.976741 brainways-0.1.6/src/brainways/elastix/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)      592 2022-10-27 09:03:02.000000 brainways-0.1.6/src/brainways/elastix/_tests/test_elastix.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2649 2022-09-08 14:32:33.000000 brainways-0.1.6/src/brainways/elastix/elastix.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.976741 brainways-0.1.6/src/brainways/pipeline/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-07 09:39:04.000000 brainways-0.1.6/src/brainways/pipeline/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.976741 brainways-0.1.6/src/brainways/pipeline/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)      430 2022-10-27 09:03:02.000000 brainways-0.1.6/src/brainways/pipeline/_tests/test_atlas_registration.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      552 2022-11-23 11:34:52.000000 brainways-0.1.6/src/brainways/pipeline/_tests/test_brainways_pipeline.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      370 2023-06-09 09:30:50.000000 brainways-0.1.6/src/brainways/pipeline/_tests/test_cell_detector.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1097 2022-11-30 13:23:46.000000 brainways-0.1.6/src/brainways/pipeline/affine_2d.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2339 2023-05-24 12:27:57.000000 brainways-0.1.6/src/brainways/pipeline/atlas_registration.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1165 2023-06-07 14:11:19.000000 brainways-0.1.6/src/brainways/pipeline/brainways_params.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     3712 2022-11-30 13:35:53.000000 brainways-0.1.6/src/brainways/pipeline/brainways_pipeline.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     5186 2023-06-09 09:29:12.000000 brainways-0.1.6/src/brainways/pipeline/cell_detector.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1596 2022-11-30 13:25:23.000000 brainways-0.1.6/src/brainways/pipeline/tps.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.976741 brainways-0.1.6/src/brainways/project/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-07 09:39:04.000000 brainways-0.1.6/src/brainways/project/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.976741 brainways-0.1.6/src/brainways/project/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-14 12:32:42.000000 brainways-0.1.6/src/brainways/project/_tests/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2145 2023-06-15 09:11:39.000000 brainways-0.1.6/src/brainways/project/_tests/conftest.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     3207 2023-06-09 09:25:09.000000 brainways-0.1.6/src/brainways/project/_tests/test_brainways_project.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     8662 2023-06-09 09:09:06.000000 brainways-0.1.6/src/brainways/project/_tests/test_brainways_subject.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.968741 brainways-0.1.6/src/brainways/project/_tests/test_projects/
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.976741 brainways-0.1.6/src/brainways/project/_tests/test_projects/v0.1.1/
--rw-rw-r--   0 ben       (1001) ben       (1001)       38 2023-06-07 15:59:39.000000 brainways-0.1.6/src/brainways/project/_tests/test_projects/v0.1.1/project.bwp
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.976741 brainways-0.1.6/src/brainways/project/_tests/test_projects/v0.1.1/subject1/
--rw-rw-r--   0 ben       (1001) ben       (1001)     2016 2023-06-15 09:11:42.000000 brainways-0.1.6/src/brainways/project/_tests/test_projects/v0.1.1/subject1/brainways.bin
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.980741 brainways-0.1.6/src/brainways/project/_tests/test_projects/v0.1.4/
--rw-rw-r--   0 ben       (1001) ben       (1001)      153 2023-06-09 09:30:50.000000 brainways-0.1.6/src/brainways/project/_tests/test_projects/v0.1.4/project.bwp
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.980741 brainways-0.1.6/src/brainways/project/_tests/test_projects/v0.1.4/subject1/
--rw-rw-r--   0 ben       (1001) ben       (1001)     1902 2023-06-15 09:11:42.000000 brainways-0.1.6/src/brainways/project/_tests/test_projects/v0.1.4/subject1/brainways.bin
--rw-rw-r--   0 ben       (1001) ben       (1001)      697 2023-06-09 08:13:53.000000 brainways-0.1.6/src/brainways/project/_tests/test_utils.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2428 2023-06-09 09:30:50.000000 brainways-0.1.6/src/brainways/project/_utils.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     8792 2023-06-15 08:57:35.000000 brainways-0.1.6/src/brainways/project/brainways_project.py
--rw-rw-r--   0 ben       (1001) ben       (1001)    18570 2023-06-09 09:06:00.000000 brainways-0.1.6/src/brainways/project/brainways_subject.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1388 2023-06-07 15:59:32.000000 brainways-0.1.6/src/brainways/project/info_classes.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.980741 brainways-0.1.6/src/brainways/scripts/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-14 12:32:42.000000 brainways-0.1.6/src/brainways/scripts/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.980741 brainways-0.1.6/src/brainways/scripts/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)      920 2023-05-26 08:21:13.000000 brainways-0.1.6/src/brainways/scripts/_tests/test_cli.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     3031 2022-09-08 14:06:58.000000 brainways-0.1.6/src/brainways/scripts/batch_create_thumbnails.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     3053 2023-05-07 14:18:30.000000 brainways-0.1.6/src/brainways/scripts/cell_detection.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1142 2023-05-04 08:18:52.000000 brainways-0.1.6/src/brainways/scripts/cli.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1588 2023-05-07 14:18:29.000000 brainways-0.1.6/src/brainways/scripts/create_excel.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     4944 2022-11-30 14:10:59.000000 brainways-0.1.6/src/brainways/scripts/create_excel_colabelling.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     4023 2022-11-23 12:26:10.000000 brainways-0.1.6/src/brainways/scripts/create_reg_model_data.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     5253 2022-11-23 12:35:34.000000 brainways-0.1.6/src/brainways/scripts/display_area.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1618 2022-12-08 14:20:04.000000 brainways-0.1.6/src/brainways/scripts/import_cell_detections_keren.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1192 2022-11-23 12:26:10.000000 brainways-0.1.6/src/brainways/scripts/import_cells.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      920 2022-12-11 10:14:02.000000 brainways-0.1.6/src/brainways/scripts/move_images.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.980741 brainways-0.1.6/src/brainways/transforms/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-04-27 09:13:34.000000 brainways-0.1.6/src/brainways/transforms/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.980741 brainways-0.1.6/src/brainways/transforms/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-04-27 09:13:34.000000 brainways-0.1.6/src/brainways/transforms/_tests/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2173 2022-07-14 13:48:40.000000 brainways-0.1.6/src/brainways/transforms/_tests/test_affine_transform_2d.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1813 2022-11-23 11:35:37.000000 brainways-0.1.6/src/brainways/transforms/_tests/test_depth_registration.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2034 2022-07-14 13:48:40.000000 brainways-0.1.6/src/brainways/transforms/_tests/test_image_to_atlas_transform.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2667 2022-07-14 13:48:40.000000 brainways-0.1.6/src/brainways/transforms/_tests/test_tps_transform.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     4104 2022-11-30 13:34:33.000000 brainways-0.1.6/src/brainways/transforms/affine_transform_2d.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      436 2022-07-14 12:46:19.000000 brainways-0.1.6/src/brainways/transforms/base.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      623 2022-07-14 13:40:58.000000 brainways-0.1.6/src/brainways/transforms/compose.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2594 2022-07-14 13:48:40.000000 brainways-0.1.6/src/brainways/transforms/depth_registration.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2205 2022-09-08 13:13:42.000000 brainways-0.1.6/src/brainways/transforms/image_to_atlas_transform.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2185 2022-11-30 13:46:38.000000 brainways-0.1.6/src/brainways/transforms/tps_transform.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.984741 brainways-0.1.6/src/brainways/utils/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-07-21 08:14:53.000000 brainways-0.1.6/src/brainways/utils/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1674 2022-07-17 07:51:20.000000 brainways-0.1.6/src/brainways/utils/_imports.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.984741 brainways-0.1.6/src/brainways/utils/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-14 12:32:42.000000 brainways-0.1.6/src/brainways/utils/_tests/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     7710 2023-05-26 08:21:13.000000 brainways-0.1.6/src/brainways/utils/_tests/test_cell_count_summary.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2715 2023-05-07 14:18:30.000000 brainways-0.1.6/src/brainways/utils/_tests/test_cells.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2412 2022-07-14 13:48:40.000000 brainways-0.1.6/src/brainways/utils/_tests/test_image.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.984741 brainways-0.1.6/src/brainways/utils/atlas/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-07-21 11:07:35.000000 brainways-0.1.6/src/brainways/utils/atlas/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.984741 brainways-0.1.6/src/brainways/utils/atlas/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-04-27 09:13:34.000000 brainways-0.1.6/src/brainways/utils/atlas/_tests/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      222 2023-06-14 09:20:14.000000 brainways-0.1.6/src/brainways/utils/atlas/_tests/test_brainways_atlas.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     3708 2022-07-14 13:40:59.000000 brainways-0.1.6/src/brainways/utils/atlas/_tests/test_slice_atlas.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     3790 2023-06-15 08:58:02.000000 brainways-0.1.6/src/brainways/utils/atlas/brainways_atlas.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2280 2023-05-04 09:01:16.000000 brainways-0.1.6/src/brainways/utils/atlas/slice_atlas.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     5751 2023-05-14 15:00:03.000000 brainways-0.1.6/src/brainways/utils/cell_count_summary.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.984741 brainways-0.1.6/src/brainways/utils/cell_detection_importer/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-10-06 09:31:17.000000 brainways-0.1.6/src/brainways/utils/cell_detection_importer/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.984741 brainways-0.1.6/src/brainways/utils/cell_detection_importer/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)     7465 2022-10-06 10:12:40.000000 brainways-0.1.6/src/brainways/utils/cell_detection_importer/_tests/qupath_sample_file.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)     1240 2022-11-23 12:23:47.000000 brainways-0.1.6/src/brainways/utils/cell_detection_importer/_tests/test_brainways_cell_detection_importer.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1722 2022-12-08 14:20:04.000000 brainways-0.1.6/src/brainways/utils/cell_detection_importer/_tests/test_qupath_cell_detection_importer.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1343 2022-11-23 12:26:10.000000 brainways-0.1.6/src/brainways/utils/cell_detection_importer/brainways_cell_detection_importer.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      507 2022-11-27 15:04:03.000000 brainways-0.1.6/src/brainways/utils/cell_detection_importer/cell_detection_importer.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2438 2022-12-11 10:33:01.000000 brainways-0.1.6/src/brainways/utils/cell_detection_importer/keren_cell_detection_importer.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      731 2022-12-08 14:20:04.000000 brainways-0.1.6/src/brainways/utils/cell_detection_importer/utils.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     4985 2023-05-02 09:29:03.000000 brainways-0.1.6/src/brainways/utils/cells.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     4270 2022-09-11 13:34:36.000000 brainways-0.1.6/src/brainways/utils/config.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.984741 brainways-0.1.6/src/brainways/utils/czi/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-07-15 08:31:32.000000 brainways-0.1.6/src/brainways/utils/czi/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1112 2022-07-14 13:48:40.000000 brainways-0.1.6/src/brainways/utils/czi/czi_to_jpg.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      793 2022-07-14 12:49:34.000000 brainways-0.1.6/src/brainways/utils/dataclasses.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     9025 2023-05-26 13:51:47.000000 brainways-0.1.6/src/brainways/utils/image.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.984741 brainways-0.1.6/src/brainways/utils/io_utils/
--rw-rw-r--   0 ben       (1001) ben       (1001)       42 2022-07-17 07:44:03.000000 brainways-0.1.6/src/brainways/utils/io_utils/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.984741 brainways-0.1.6/src/brainways/utils/io_utils/file_iterators/
--rw-rw-r--   0 ben       (1001) ben       (1001)      379 2022-09-08 08:38:22.000000 brainways-0.1.6/src/brainways/utils/io_utils/file_iterators/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      230 2022-07-07 09:39:04.000000 brainways-0.1.6/src/brainways/utils/io_utils/file_iterators/image_entry.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      407 2022-07-07 09:39:04.000000 brainways-0.1.6/src/brainways/utils/io_utils/file_iterators/path.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      914 2022-11-23 12:29:43.000000 brainways-0.1.6/src/brainways/utils/io_utils/file_iterators/qupath.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      630 2022-07-07 09:39:09.000000 brainways-0.1.6/src/brainways/utils/io_utils/image_path.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.984741 brainways-0.1.6/src/brainways/utils/io_utils/readers/
--rw-rw-r--   0 ben       (1001) ben       (1001)     1041 2022-09-11 12:16:49.000000 brainways-0.1.6/src/brainways/utils/io_utils/readers/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.988741 brainways-0.1.6/src/brainways/utils/io_utils/readers/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)      218 2022-09-22 07:42:16.000000 brainways-0.1.6/src/brainways/utils/io_utils/readers/_tests/test_qupath_reader.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1419 2022-09-08 08:38:21.000000 brainways-0.1.6/src/brainways/utils/io_utils/readers/aicsimageio_reader.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      649 2022-07-14 12:39:58.000000 brainways-0.1.6/src/brainways/utils/io_utils/readers/base.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1364 2022-09-08 08:38:21.000000 brainways-0.1.6/src/brainways/utils/io_utils/readers/czi_reader.py
--rw-rw-r--   0 ben       (1001) ben       (1001)    15748 2023-05-21 10:26:48.000000 brainways-0.1.6/src/brainways/utils/io_utils/readers/qupath_reader.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      108 2022-09-11 13:34:36.000000 brainways-0.1.6/src/brainways/utils/paths.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1181 2022-07-14 13:48:40.000000 brainways-0.1.6/src/brainways/utils/preprocess.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     3183 2022-09-11 10:47:30.000000 brainways-0.1.6/src/brainways/utils/qupath.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1083 2022-07-14 13:48:39.000000 brainways-0.1.6/src/brainways/utils/test_utils.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.976741 brainways-0.1.6/src/brainways.egg-info/
--rw-rw-r--   0 ben       (1001) ben       (1001)     2343 2023-06-15 09:13:26.000000 brainways-0.1.6/src/brainways.egg-info/PKG-INFO
--rw-rw-r--   0 ben       (1001) ben       (1001)     5786 2023-06-15 09:13:26.000000 brainways-0.1.6/src/brainways.egg-info/SOURCES.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)        1 2023-06-15 09:13:26.000000 brainways-0.1.6/src/brainways.egg-info/dependency_links.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)       57 2023-06-15 09:13:26.000000 brainways-0.1.6/src/brainways.egg-info/entry_points.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)      413 2023-06-15 09:13:26.000000 brainways-0.1.6/src/brainways.egg-info/requires.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)       10 2023-06-15 09:13:26.000000 brainways-0.1.6/src/brainways.egg-info/top_level.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)      540 2022-07-13 13:47:58.000000 brainways-0.1.6/tox.ini
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.629055 brainways-0.1.7/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      292 2022-07-13 13:47:58.000000 brainways-0.1.7/.editorconfig
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.609055 brainways-0.1.7/.github/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      320 2022-07-13 13:47:58.000000 brainways-0.1.7/.github/ISSUE_TEMPLATE.md
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1248 2022-07-13 14:46:16.000000 brainways-0.1.7/.gitignore
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1194 2022-07-14 13:50:01.000000 brainways-0.1.7/.pre-commit-config.yaml
+-rw-rw-r--   0 ben       (1001) ben       (1001)      681 2022-07-13 13:47:58.000000 brainways-0.1.7/.travis.yml
+-rw-rw-r--   0 ben       (1001) ben       (1001)      160 2022-07-13 13:47:58.000000 brainways-0.1.7/AUTHORS.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1475 2023-08-02 08:34:50.000000 brainways-0.1.7/CHANGELOG.md
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3523 2022-07-13 13:47:58.000000 brainways-0.1.7/CONTRIBUTING.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)       89 2022-07-13 13:47:58.000000 brainways-0.1.7/HISTORY.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)    35148 2022-08-24 08:26:24.000000 brainways-0.1.7/LICENSE
+-rw-rw-r--   0 ben       (1001) ben       (1001)      262 2022-07-13 13:47:58.000000 brainways-0.1.7/MANIFEST.in
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2430 2023-05-26 08:21:13.000000 brainways-0.1.7/Makefile
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2343 2023-08-02 08:49:47.629055 brainways-0.1.7/PKG-INFO
+-rw-rw-r--   0 ben       (1001) ben       (1001)      962 2023-05-26 08:25:05.000000 brainways-0.1.7/README.rst
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.609055 brainways-0.1.7/data/
+-rw-rw-r--   0 ben       (1001) ben       (1001)   269441 2022-03-11 09:30:01.000000 brainways-0.1.7/data/test_data.npz
+-rw-rw-r--   0 ben       (1001) ben       (1001)    47973 2022-06-30 11:17:43.000000 brainways-0.1.7/data/test_image.jpg
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.613055 brainways-0.1.7/docs/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      610 2022-07-13 13:47:58.000000 brainways-0.1.7/docs/Makefile
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.605055 brainways-0.1.7/docs/_build/
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.605055 brainways-0.1.7/docs/_build/html/
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.613055 brainways-0.1.7/docs/_build/html/_static/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      286 2022-10-06 11:03:00.000000 brainways-0.1.7/docs/_build/html/_static/file.png
+-rw-rw-r--   0 ben       (1001) ben       (1001)       90 2022-10-06 11:03:00.000000 brainways-0.1.7/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 ben       (1001) ben       (1001)       90 2022-10-06 11:03:00.000000 brainways-0.1.7/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 ben       (1001) ben       (1001)       28 2022-07-13 13:47:58.000000 brainways-0.1.7/docs/authors.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      361 2023-05-26 08:18:55.000000 brainways-0.1.7/docs/brainways.elastix.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1317 2023-05-26 08:18:55.000000 brainways-0.1.7/docs/brainways.pipeline.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      770 2023-05-26 08:18:55.000000 brainways-0.1.7/docs/brainways.project.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      500 2023-05-26 08:26:43.000000 brainways-0.1.7/docs/brainways.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2137 2023-05-26 08:18:55.000000 brainways-0.1.7/docs/brainways.scripts.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1387 2023-05-26 08:18:55.000000 brainways-0.1.7/docs/brainways.transforms.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      601 2023-05-26 08:18:55.000000 brainways-0.1.7/docs/brainways.utils.atlas.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1405 2023-05-26 08:18:55.000000 brainways-0.1.7/docs/brainways.utils.cell_detection_importer.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      386 2023-05-26 08:18:55.000000 brainways-0.1.7/docs/brainways.utils.czi.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      971 2023-05-26 08:18:55.000000 brainways-0.1.7/docs/brainways.utils.io_utils.file_iterators.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1145 2023-05-26 08:18:55.000000 brainways-0.1.7/docs/brainways.utils.io_utils.readers.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      553 2023-05-26 08:18:55.000000 brainways-0.1.7/docs/brainways.utils.io_utils.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1833 2023-05-26 08:18:55.000000 brainways-0.1.7/docs/brainways.utils.rst
+-rwxrwxr-x   0 ben       (1001) ben       (1001)     4967 2023-05-26 08:17:55.000000 brainways-0.1.7/docs/conf.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)       33 2022-07-13 13:47:58.000000 brainways-0.1.7/docs/contributing.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)       28 2022-07-13 13:47:58.000000 brainways-0.1.7/docs/history.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      306 2022-07-13 13:47:58.000000 brainways-0.1.7/docs/index.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1118 2022-07-13 13:47:58.000000 brainways-0.1.7/docs/installation.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      807 2022-07-13 13:47:58.000000 brainways-0.1.7/docs/make.bat
+-rw-rw-r--   0 ben       (1001) ben       (1001)       64 2023-05-26 08:26:43.000000 brainways-0.1.7/docs/modules.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)       27 2022-07-13 13:47:58.000000 brainways-0.1.7/docs/readme.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)       73 2022-07-13 13:47:58.000000 brainways-0.1.7/docs/usage.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      383 2023-05-26 08:03:19.000000 brainways-0.1.7/pyproject.toml
+-rw-rw-r--   0 ben       (1001) ben       (1001)      165 2022-07-13 14:08:33.000000 brainways-0.1.7/requirements_dev.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2012 2023-08-02 08:49:47.629055 brainways-0.1.7/setup.cfg
+-rw-rw-r--   0 ben       (1001) ben       (1001)       60 2023-05-26 07:59:05.000000 brainways-0.1.7/setup.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.605055 brainways-0.1.7/src/
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.613055 brainways-0.1.7/src/brainways/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2023-06-21 08:03:13.000000 brainways-0.1.7/src/brainways/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      160 2023-08-02 08:49:47.000000 brainways-0.1.7/src/brainways/_version.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     8827 2023-08-02 08:34:50.000000 brainways-0.1.7/src/brainways/conftest.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.617055 brainways-0.1.7/src/brainways/elastix/
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2596 2022-07-14 13:40:58.000000 brainways-0.1.7/src/brainways/elastix/Par0033bspline.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2316 2022-07-14 13:40:58.000000 brainways-0.1.7/src/brainways/elastix/Par0033similarity.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-12-09 12:20:50.000000 brainways-0.1.7/src/brainways/elastix/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.617055 brainways-0.1.7/src/brainways/elastix/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      592 2022-10-27 09:03:02.000000 brainways-0.1.7/src/brainways/elastix/_tests/test_elastix.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2649 2022-09-08 14:32:33.000000 brainways-0.1.7/src/brainways/elastix/elastix.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.617055 brainways-0.1.7/src/brainways/pipeline/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-07 09:39:04.000000 brainways-0.1.7/src/brainways/pipeline/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.617055 brainways-0.1.7/src/brainways/pipeline/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      430 2022-10-27 09:03:02.000000 brainways-0.1.7/src/brainways/pipeline/_tests/test_atlas_registration.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      552 2022-11-23 11:34:52.000000 brainways-0.1.7/src/brainways/pipeline/_tests/test_brainways_pipeline.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      370 2023-06-09 09:30:50.000000 brainways-0.1.7/src/brainways/pipeline/_tests/test_cell_detector.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1097 2022-11-30 13:23:46.000000 brainways-0.1.7/src/brainways/pipeline/affine_2d.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2339 2023-05-24 12:27:57.000000 brainways-0.1.7/src/brainways/pipeline/atlas_registration.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1165 2023-08-02 08:34:50.000000 brainways-0.1.7/src/brainways/pipeline/brainways_params.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3712 2022-11-30 13:35:53.000000 brainways-0.1.7/src/brainways/pipeline/brainways_pipeline.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     5186 2023-06-09 09:29:12.000000 brainways-0.1.7/src/brainways/pipeline/cell_detector.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1633 2023-08-02 08:34:50.000000 brainways-0.1.7/src/brainways/pipeline/tps.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.617055 brainways-0.1.7/src/brainways/project/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-07 09:39:04.000000 brainways-0.1.7/src/brainways/project/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.617055 brainways-0.1.7/src/brainways/project/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-14 12:32:42.000000 brainways-0.1.7/src/brainways/project/_tests/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2582 2023-08-02 08:34:50.000000 brainways-0.1.7/src/brainways/project/_tests/conftest.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     5774 2023-08-02 08:34:50.000000 brainways-0.1.7/src/brainways/project/_tests/test_brainways_project.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     6274 2023-08-02 08:34:50.000000 brainways-0.1.7/src/brainways/project/_tests/test_brainways_subject.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.609055 brainways-0.1.7/src/brainways/project/_tests/test_projects/
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.617055 brainways-0.1.7/src/brainways/project/_tests/test_projects/v0.1.1/
+-rw-rw-r--   0 ben       (1001) ben       (1001)       38 2023-06-07 15:59:39.000000 brainways-0.1.7/src/brainways/project/_tests/test_projects/v0.1.1/project.bwp
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.617055 brainways-0.1.7/src/brainways/project/_tests/test_projects/v0.1.1/subject1/
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2016 2023-06-15 09:11:42.000000 brainways-0.1.7/src/brainways/project/_tests/test_projects/v0.1.1/subject1/brainways.bin
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.617055 brainways-0.1.7/src/brainways/project/_tests/test_projects/v0.1.4/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      153 2023-06-09 09:30:50.000000 brainways-0.1.7/src/brainways/project/_tests/test_projects/v0.1.4/project.bwp
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.617055 brainways-0.1.7/src/brainways/project/_tests/test_projects/v0.1.4/subject1/
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1902 2023-06-15 09:11:42.000000 brainways-0.1.7/src/brainways/project/_tests/test_projects/v0.1.4/subject1/brainways.bin
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.617055 brainways-0.1.7/src/brainways/project/_tests/test_projects/v0.1.5/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      153 2023-08-02 08:34:50.000000 brainways-0.1.7/src/brainways/project/_tests/test_projects/v0.1.5/project.bwp
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.617055 brainways-0.1.7/src/brainways/project/_tests/test_projects/v0.1.5/subject1/
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1958 2023-08-02 08:34:50.000000 brainways-0.1.7/src/brainways/project/_tests/test_projects/v0.1.5/subject1/brainways.bin
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1133 2023-08-02 08:34:50.000000 brainways-0.1.7/src/brainways/project/_tests/test_utils.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     4065 2023-08-02 08:34:50.000000 brainways-0.1.7/src/brainways/project/_utils.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)    10852 2023-08-02 08:34:50.000000 brainways-0.1.7/src/brainways/project/brainways_project.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)    16785 2023-08-02 08:34:50.000000 brainways-0.1.7/src/brainways/project/brainways_subject.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1567 2023-08-02 08:34:50.000000 brainways-0.1.7/src/brainways/project/info_classes.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.621055 brainways-0.1.7/src/brainways/scripts/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-14 12:32:42.000000 brainways-0.1.7/src/brainways/scripts/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.621055 brainways-0.1.7/src/brainways/scripts/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      920 2023-05-26 08:21:13.000000 brainways-0.1.7/src/brainways/scripts/_tests/test_cli.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3031 2022-09-08 14:06:58.000000 brainways-0.1.7/src/brainways/scripts/batch_create_thumbnails.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3053 2023-05-07 14:18:30.000000 brainways-0.1.7/src/brainways/scripts/cell_detection.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1142 2023-05-04 08:18:52.000000 brainways-0.1.7/src/brainways/scripts/cli.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1593 2023-08-02 08:34:50.000000 brainways-0.1.7/src/brainways/scripts/create_excel.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     4944 2022-11-30 14:10:59.000000 brainways-0.1.7/src/brainways/scripts/create_excel_colabelling.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     4023 2022-11-23 12:26:10.000000 brainways-0.1.7/src/brainways/scripts/create_reg_model_data.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     5253 2022-11-23 12:35:34.000000 brainways-0.1.7/src/brainways/scripts/display_area.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1618 2022-12-08 14:20:04.000000 brainways-0.1.7/src/brainways/scripts/import_cell_detections_keren.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1192 2022-11-23 12:26:10.000000 brainways-0.1.7/src/brainways/scripts/import_cells.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      920 2022-12-11 10:14:02.000000 brainways-0.1.7/src/brainways/scripts/move_images.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.621055 brainways-0.1.7/src/brainways/transforms/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-04-27 09:13:34.000000 brainways-0.1.7/src/brainways/transforms/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.621055 brainways-0.1.7/src/brainways/transforms/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-04-27 09:13:34.000000 brainways-0.1.7/src/brainways/transforms/_tests/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2173 2022-07-14 13:48:40.000000 brainways-0.1.7/src/brainways/transforms/_tests/test_affine_transform_2d.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1813 2022-11-23 11:35:37.000000 brainways-0.1.7/src/brainways/transforms/_tests/test_depth_registration.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2082 2023-08-02 08:34:50.000000 brainways-0.1.7/src/brainways/transforms/_tests/test_image_to_atlas_transform.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2685 2023-08-02 08:34:50.000000 brainways-0.1.7/src/brainways/transforms/_tests/test_tps_transform.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     4104 2022-11-30 13:34:33.000000 brainways-0.1.7/src/brainways/transforms/affine_transform_2d.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      436 2022-07-14 12:46:19.000000 brainways-0.1.7/src/brainways/transforms/base.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      623 2022-07-14 13:40:58.000000 brainways-0.1.7/src/brainways/transforms/compose.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2594 2022-07-14 13:48:40.000000 brainways-0.1.7/src/brainways/transforms/depth_registration.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2205 2022-09-08 13:13:42.000000 brainways-0.1.7/src/brainways/transforms/image_to_atlas_transform.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2239 2023-08-02 08:34:50.000000 brainways-0.1.7/src/brainways/transforms/tps_transform.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.625055 brainways-0.1.7/src/brainways/utils/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-07-21 08:14:53.000000 brainways-0.1.7/src/brainways/utils/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1674 2022-07-17 07:51:20.000000 brainways-0.1.7/src/brainways/utils/_imports.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.625055 brainways-0.1.7/src/brainways/utils/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-14 12:32:42.000000 brainways-0.1.7/src/brainways/utils/_tests/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     9665 2023-08-02 08:34:50.000000 brainways-0.1.7/src/brainways/utils/_tests/test_cell_count_summary.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2715 2023-05-07 14:18:30.000000 brainways-0.1.7/src/brainways/utils/_tests/test_cells.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      864 2023-08-02 08:34:50.000000 brainways-0.1.7/src/brainways/utils/_tests/test_contrast.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2412 2022-07-14 13:48:40.000000 brainways-0.1.7/src/brainways/utils/_tests/test_image.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.625055 brainways-0.1.7/src/brainways/utils/atlas/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-07-21 11:07:35.000000 brainways-0.1.7/src/brainways/utils/atlas/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.625055 brainways-0.1.7/src/brainways/utils/atlas/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-04-27 09:13:34.000000 brainways-0.1.7/src/brainways/utils/atlas/_tests/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      222 2023-06-14 09:20:14.000000 brainways-0.1.7/src/brainways/utils/atlas/_tests/test_brainways_atlas.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3708 2022-07-14 13:40:59.000000 brainways-0.1.7/src/brainways/utils/atlas/_tests/test_slice_atlas.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3790 2023-06-15 08:58:02.000000 brainways-0.1.7/src/brainways/utils/atlas/brainways_atlas.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2280 2023-05-04 09:01:16.000000 brainways-0.1.7/src/brainways/utils/atlas/slice_atlas.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     5990 2023-08-02 08:34:50.000000 brainways-0.1.7/src/brainways/utils/cell_count_summary.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.625055 brainways-0.1.7/src/brainways/utils/cell_detection_importer/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-10-06 09:31:17.000000 brainways-0.1.7/src/brainways/utils/cell_detection_importer/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.625055 brainways-0.1.7/src/brainways/utils/cell_detection_importer/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)     7465 2022-10-06 10:12:40.000000 brainways-0.1.7/src/brainways/utils/cell_detection_importer/_tests/qupath_sample_file.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1240 2022-11-23 12:23:47.000000 brainways-0.1.7/src/brainways/utils/cell_detection_importer/_tests/test_brainways_cell_detection_importer.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1722 2022-12-08 14:20:04.000000 brainways-0.1.7/src/brainways/utils/cell_detection_importer/_tests/test_qupath_cell_detection_importer.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1343 2022-11-23 12:26:10.000000 brainways-0.1.7/src/brainways/utils/cell_detection_importer/brainways_cell_detection_importer.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      507 2022-11-27 15:04:03.000000 brainways-0.1.7/src/brainways/utils/cell_detection_importer/cell_detection_importer.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2438 2022-12-11 10:33:01.000000 brainways-0.1.7/src/brainways/utils/cell_detection_importer/keren_cell_detection_importer.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      731 2022-12-08 14:20:04.000000 brainways-0.1.7/src/brainways/utils/cell_detection_importer/utils.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     4985 2023-05-02 09:29:03.000000 brainways-0.1.7/src/brainways/utils/cells.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     4270 2022-09-11 13:34:36.000000 brainways-0.1.7/src/brainways/utils/config.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3724 2023-08-02 08:34:50.000000 brainways-0.1.7/src/brainways/utils/contrast.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.625055 brainways-0.1.7/src/brainways/utils/czi/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-07-15 08:31:32.000000 brainways-0.1.7/src/brainways/utils/czi/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1112 2022-07-14 13:48:40.000000 brainways-0.1.7/src/brainways/utils/czi/czi_to_jpg.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      793 2022-07-14 12:49:34.000000 brainways-0.1.7/src/brainways/utils/dataclasses.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     9025 2023-05-26 13:51:47.000000 brainways-0.1.7/src/brainways/utils/image.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.625055 brainways-0.1.7/src/brainways/utils/io_utils/
+-rw-rw-r--   0 ben       (1001) ben       (1001)       42 2022-07-17 07:44:03.000000 brainways-0.1.7/src/brainways/utils/io_utils/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.625055 brainways-0.1.7/src/brainways/utils/io_utils/file_iterators/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      379 2022-09-08 08:38:22.000000 brainways-0.1.7/src/brainways/utils/io_utils/file_iterators/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      230 2022-07-07 09:39:04.000000 brainways-0.1.7/src/brainways/utils/io_utils/file_iterators/image_entry.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      407 2022-07-07 09:39:04.000000 brainways-0.1.7/src/brainways/utils/io_utils/file_iterators/path.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      914 2022-11-23 12:29:43.000000 brainways-0.1.7/src/brainways/utils/io_utils/file_iterators/qupath.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      630 2022-07-07 09:39:09.000000 brainways-0.1.7/src/brainways/utils/io_utils/image_path.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.629055 brainways-0.1.7/src/brainways/utils/io_utils/readers/
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1041 2022-09-11 12:16:49.000000 brainways-0.1.7/src/brainways/utils/io_utils/readers/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.629055 brainways-0.1.7/src/brainways/utils/io_utils/readers/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      218 2022-09-22 07:42:16.000000 brainways-0.1.7/src/brainways/utils/io_utils/readers/_tests/test_qupath_reader.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1419 2022-09-08 08:38:21.000000 brainways-0.1.7/src/brainways/utils/io_utils/readers/aicsimageio_reader.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      649 2022-07-14 12:39:58.000000 brainways-0.1.7/src/brainways/utils/io_utils/readers/base.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1364 2022-09-08 08:38:21.000000 brainways-0.1.7/src/brainways/utils/io_utils/readers/czi_reader.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)    15678 2023-08-02 08:34:50.000000 brainways-0.1.7/src/brainways/utils/io_utils/readers/qupath_reader.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      108 2022-09-11 13:34:36.000000 brainways-0.1.7/src/brainways/utils/paths.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1181 2022-07-14 13:48:40.000000 brainways-0.1.7/src/brainways/utils/preprocess.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3024 2023-08-02 08:34:50.000000 brainways-0.1.7/src/brainways/utils/qupath.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1101 2023-08-02 08:34:50.000000 brainways-0.1.7/src/brainways/utils/test_utils.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-08-02 08:49:47.613055 brainways-0.1.7/src/brainways.egg-info/
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2343 2023-08-02 08:49:47.000000 brainways-0.1.7/src/brainways.egg-info/PKG-INFO
+-rw-rw-r--   0 ben       (1001) ben       (1001)     6010 2023-08-02 08:49:47.000000 brainways-0.1.7/src/brainways.egg-info/SOURCES.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)        1 2023-08-02 08:49:47.000000 brainways-0.1.7/src/brainways.egg-info/dependency_links.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)       57 2023-08-02 08:49:47.000000 brainways-0.1.7/src/brainways.egg-info/entry_points.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)      456 2023-08-02 08:49:47.000000 brainways-0.1.7/src/brainways.egg-info/requires.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)       10 2023-08-02 08:49:47.000000 brainways-0.1.7/src/brainways.egg-info/top_level.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)      540 2022-07-13 13:47:58.000000 brainways-0.1.7/tox.ini
```

### Comparing `brainways-0.1.6/.gitignore` & `brainways-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/.pre-commit-config.yaml` & `brainways-0.1.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/.travis.yml` & `brainways-0.1.7/.travis.yml`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/CONTRIBUTING.rst` & `brainways-0.1.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/LICENSE` & `brainways-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/Makefile` & `brainways-0.1.7/Makefile`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/PKG-INFO` & `brainways-0.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainways
-Version: 0.1.6
+Version: 0.1.7
 Summary: Brainways
 Home-page: https://github.com/bkntr/brainways
 Author: Ben Kantor
 Author-email: benkantor@mail.tau.ac.il
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/bkntr/brainways/issues
 Project-URL: Documentation, https://github.com/bkntr/brainways#README.md
```

### Comparing `brainways-0.1.6/README.rst` & `brainways-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/data/test_data.npz` & `brainways-0.1.7/data/test_data.npz`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/data/test_image.jpg` & `brainways-0.1.7/data/test_image.jpg`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/docs/Makefile` & `brainways-0.1.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/docs/brainways.pipeline.rst` & `brainways-0.1.7/docs/brainways.pipeline.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/docs/brainways.project.rst` & `brainways-0.1.7/docs/brainways.project.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/docs/brainways.scripts.rst` & `brainways-0.1.7/docs/brainways.scripts.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/docs/brainways.transforms.rst` & `brainways-0.1.7/docs/brainways.transforms.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/docs/brainways.utils.atlas.rst` & `brainways-0.1.7/docs/brainways.utils.atlas.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/docs/brainways.utils.cell_detection_importer.rst` & `brainways-0.1.7/docs/brainways.utils.cell_detection_importer.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/docs/brainways.utils.io_utils.file_iterators.rst` & `brainways-0.1.7/docs/brainways.utils.io_utils.file_iterators.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/docs/brainways.utils.io_utils.readers.rst` & `brainways-0.1.7/docs/brainways.utils.io_utils.readers.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/docs/brainways.utils.io_utils.rst` & `brainways-0.1.7/docs/brainways.utils.io_utils.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/docs/brainways.utils.rst` & `brainways-0.1.7/docs/brainways.utils.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/docs/conf.py` & `brainways-0.1.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/docs/installation.rst` & `brainways-0.1.7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/docs/make.bat` & `brainways-0.1.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/setup.cfg` & `brainways-0.1.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -45,18 +45,20 @@
 	kornia==0.6.7
 	natsort
 	numpy
 	opencv-contrib-python-headless
 	opencv-python-headless
 	openpyxl
 	pandas
-	paquo==0.5.1
+	paquo==0.6.1
 	readlif>=0.6.4
 	scikit-image
 	scikit-learn
+	scikit-posthocs==0.7.0
+	statsmodels==0.14.0
 	torch==1.10.*
 	torchvision==0.11.*
 python_requires = >=3.6
 include_package_data = True
 package_dir = 
 	=src
 setup_requires =
```

### Comparing `brainways-0.1.6/src/brainways/conftest.py` & `brainways-0.1.7/src/brainways/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
-import pickle
 import shutil
+from copy import deepcopy
 from dataclasses import asdict, replace
 from pathlib import Path
 from typing import List, Tuple
 from unittest.mock import Mock, create_autospec, patch
 
 import numpy as np
 import pytest
@@ -17,16 +17,22 @@
 from brainways.pipeline.brainways_params import (
     AffineTransform2DParams,
     AtlasRegistrationParams,
     BrainwaysParams,
     CellDetectorParams,
     TPSTransformParams,
 )
+from brainways.project.brainways_project import BrainwaysProject
 from brainways.project.brainways_subject import BrainwaysSubject
-from brainways.project.info_classes import ProjectSettings, SliceInfo
+from brainways.project.info_classes import (
+    ProjectSettings,
+    SliceInfo,
+    SubjectFileFormat,
+    SubjectInfo,
+)
 from brainways.utils.atlas.brainways_atlas import AtlasSlice, BrainwaysAtlas
 from brainways.utils.image import ImageSizeHW
 from brainways.utils.io_utils import ImagePath
 from brainways.utils.io_utils.readers.base import ImageReader
 from brainways.utils.io_utils.readers.qupath_reader import QupathReader
 
 
@@ -150,16 +156,18 @@
 @pytest.fixture
 def mock_subject_documents(
     mock_image_path: ImagePath, test_data: Tuple[np.ndarray, AtlasSlice]
 ) -> List[SliceInfo]:
     test_image, test_atlas_slice = test_data
     image_height = test_image.shape[0]
     image_width = test_image.shape[1]
-    tps_points = (np.random.rand(10, 2) * (image_width, image_height)).astype(
-        np.float32
+    tps_points = (
+        (np.random.rand(10, 2) * (image_width, image_height))
+        .astype(np.float32)
+        .tolist()
     )
 
     params = BrainwaysParams(
         atlas=AtlasRegistrationParams(ap=5),
         affine=AffineTransform2DParams(),
         tps=TPSTransformParams(
             points_src=tps_points,
@@ -194,42 +202,78 @@
 def mock_project_settings() -> ProjectSettings:
     return ProjectSettings(atlas="MOCK_ATLAS", channel=0)
 
 
 @pytest.fixture
 def subject_path(
     tmpdir,
-    mock_project_settings: ProjectSettings,
-    mock_subject_documents: List[SliceInfo],
+    mock_subject_file_format: SubjectFileFormat,
 ) -> Path:
-    subject_path = Path(tmpdir) / "project/subject1/brainways.bin"
+    subject_path = Path(tmpdir) / "test_subject/data.bws"
     subject_path.parent.mkdir(parents=True)
-    serialized_subject_settings = asdict(mock_project_settings)
-    serialized_subject_documents = [asdict(doc) for doc in mock_subject_documents]
-    with open(subject_path, "wb") as f:
-        pickle.dump((serialized_subject_settings, serialized_subject_documents), f)
+    serialized_subject_file_format = asdict(mock_subject_file_format)
+    with open(subject_path, "w") as f:
+        json.dump(serialized_subject_file_format, f)
     yield subject_path
 
 
 @pytest.fixture
+def mock_subject_info() -> SubjectInfo:
+    return SubjectInfo(name="subject1", conditions={"condition": "a"})
+
+
+@pytest.fixture
+def mock_subject_file_format(
+    mock_subject_info: SubjectInfo, mock_subject_documents: List[SliceInfo]
+) -> SubjectFileFormat:
+    return SubjectFileFormat(
+        subject_info=mock_subject_info, slice_infos=mock_subject_documents
+    )
+
+
+@pytest.fixture
 def project_path(
     subject_path: Path,
     mock_project_settings: ProjectSettings,
 ) -> Path:
     project_path = subject_path.parent.parent / "project.bwp"
     serialized_project_settings = asdict(mock_project_settings)
     with open(project_path, "w") as f:
         json.dump(serialized_project_settings, f)
     yield project_path
 
 
 @pytest.fixture
-def brainways_subject(
-    subject_path: Path,
-    test_data: Tuple[np.ndarray, AtlasSlice],
+def brainways_project(
+    mock_subject_info: SubjectInfo,
+    mock_subject_documents: List[SliceInfo],
+    mock_project_settings: ProjectSettings,
     mock_atlas: BrainwaysAtlas,
-) -> BrainwaysSubject:
-    brainways_subject = BrainwaysSubject.open(subject_path)
-    brainways_subject.atlas = mock_atlas
-    for document in brainways_subject.documents:
-        brainways_subject.read_lowres_image(document)
-    return brainways_subject
+    test_data: Tuple[np.ndarray, AtlasSlice],
+    tmpdir,
+) -> BrainwaysProject:
+    project_path = Path(tmpdir / "project/project.bwp")
+    project_path.parent.mkdir()
+    brainways_project = BrainwaysProject(
+        subjects=[],
+        settings=mock_project_settings,
+        path=project_path,
+        lazy_init=True,
+    )
+    brainways_project.atlas = mock_atlas
+    brainways_project.load_pipeline()
+
+    # add mock subject to project
+    brainways_project.add_subject(mock_subject_info)
+    brainways_project.add_subject(
+        SubjectInfo(name="subject2", conditions={"condition": "b"})
+    )
+    for brainways_subject in brainways_project.subjects:
+        brainways_subject.documents = deepcopy(mock_subject_documents)
+        for document in brainways_subject.documents:
+            brainways_subject.read_lowres_image(document)
+    return brainways_project
+
+
+@pytest.fixture
+def brainways_subject(brainways_project: BrainwaysProject) -> BrainwaysSubject:
+    return brainways_project.subjects[0]
```

### Comparing `brainways-0.1.6/src/brainways/elastix/Par0033bspline.txt` & `brainways-0.1.7/src/brainways/elastix/Par0033bspline.txt`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/elastix/Par0033similarity.txt` & `brainways-0.1.7/src/brainways/elastix/Par0033similarity.txt`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/elastix/_tests/test_elastix.py` & `brainways-0.1.7/src/brainways/elastix/_tests/test_elastix.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/elastix/elastix.py` & `brainways-0.1.7/src/brainways/elastix/elastix.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/pipeline/_tests/test_brainways_pipeline.py` & `brainways-0.1.7/src/brainways/pipeline/_tests/test_brainways_pipeline.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/pipeline/affine_2d.py` & `brainways-0.1.7/src/brainways/pipeline/affine_2d.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/pipeline/atlas_registration.py` & `brainways-0.1.7/src/brainways/pipeline/atlas_registration.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/pipeline/brainways_params.py` & `brainways-0.1.7/src/brainways/pipeline/brainways_params.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import Optional, Tuple
-
-import numpy as np
+from typing import List, Optional, Tuple
 
 from brainways.utils.dataclasses import dataclass_eq
 
 
 @dataclass(frozen=True)
 class BrainwaysParams:
     atlas: Optional[AtlasRegistrationParams] = None
@@ -31,16 +29,16 @@
     sy: float = 1.0
     cx: Optional[float] = None
     cy: Optional[float] = None
 
 
 @dataclass(frozen=True)
 class TPSTransformParams:
-    points_src: np.ndarray
-    points_dst: np.ndarray
+    points_src: List[List[float]]
+    points_dst: List[List[float]]
 
     def __eq__(self, other):
         return dataclass_eq(self, other)
 
 
 @dataclass(frozen=True)
 class AtlasRegistrationParams:
```

### Comparing `brainways-0.1.6/src/brainways/pipeline/brainways_pipeline.py` & `brainways-0.1.7/src/brainways/pipeline/brainways_pipeline.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/pipeline/cell_detector.py` & `brainways-0.1.7/src/brainways/pipeline/cell_detector.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/pipeline/tps.py` & `brainways-0.1.7/src/brainways/pipeline/tps.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,21 +22,21 @@
         fixed = atlas_slice.reference.numpy()
         fixed_mask = None
         moving = image
         moving_mask = None
         registered_src_points = elastix_registration(
             fixed=fixed,
             moving=moving,
-            fixed_points=params.tps.points_src,
+            fixed_points=np.array(params.tps.points_src, dtype=np.float32),
             fixed_mask=fixed_mask,
             moving_mask=moving_mask,
         )
         transform = TPSTransform(
             TPSTransformParams(
-                points_src=registered_src_points,
+                points_src=registered_src_points.tolist(),
                 points_dst=params.tps.points_src,
             )
         )
         registered_dst_points = transform.transform_points(params.tps.points_src)
         return replace(
             params,
             tps=TPSTransformParams(
```

### Comparing `brainways-0.1.6/src/brainways/project/_tests/conftest.py` & `brainways-0.1.7/src/brainways/project/_tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,25 @@
     )
     tmp_project_dir = Path(tmpdir / "v0.1.4")
     shutil.copytree(project_path.parent, tmp_project_dir)
     rewrite_image_path(project_path=tmp_project_dir, image_path=mock_image_path)
     return tmp_project_dir / "project.bwp"
 
 
+@pytest.fixture
+def brainways_project_path_v0_1_5(mock_image_path: ImagePath, tmpdir) -> Path:
+    project_path = (
+        Path(os.path.realpath(__file__)).parent / "test_projects/v0.1.5/project.bwp"
+    )
+    tmp_project_dir = Path(tmpdir / "v0.1.5")
+    shutil.copytree(project_path.parent, tmp_project_dir)
+    rewrite_image_path(project_path=tmp_project_dir, image_path=mock_image_path)
+    return tmp_project_dir / "project.bwp"
+
+
 def rewrite_image_path(project_path: Path, image_path: ImagePath):
     brainways_subject_paths = project_path.parent.rglob("brainways.bin")
     for brainways_subject_path in brainways_subject_paths:
         with open(brainways_subject_path, "rb") as f:
             serialized_settings, serialized_slice_infos = pickle.load(f)
         for serialized_slice_info in serialized_slice_infos:
             serialized_slice_info["path"]["filename"] = image_path.filename
```

### Comparing `brainways-0.1.6/src/brainways/project/_tests/test_projects/v0.1.1/subject1/brainways.bin` & `brainways-0.1.7/src/brainways/project/_tests/test_projects/v0.1.1/subject1/brainways.bin`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/project/_tests/test_projects/v0.1.4/subject1/brainways.bin` & `brainways-0.1.7/src/brainways/project/_tests/test_projects/v0.1.4/subject1/brainways.bin`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/project/_tests/test_utils.py` & `brainways-0.1.7/src/brainways/project/_tests/test_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,7 +9,16 @@
     BrainwaysProject.open(brainways_project_path_v0_1_1, lazy_init=True)
 
 
 def test_update_project_from_v0_1_4(brainways_project_path_v0_1_4: Path):
     update_project_from_previous_versions(brainways_project_path_v0_1_4)
     project = BrainwaysProject.open(brainways_project_path_v0_1_4, lazy_init=True)
     assert project.subjects[0].documents[0].physical_pixel_sizes is not None
+
+
+def test_update_project_from_v0_1_5(
+    brainways_project_path_v0_1_5: Path, mock_subject_documents
+):
+    update_project_from_previous_versions(brainways_project_path_v0_1_5)
+    project = BrainwaysProject.open(brainways_project_path_v0_1_5, lazy_init=True)
+    assert project.subjects[0].documents[0].params == mock_subject_documents[0].params
+    assert project.subjects[0].subject_info.name == project.subjects[0]._save_dir.name
```

### Comparing `brainways-0.1.6/src/brainways/project/_utils.py` & `brainways-0.1.7/src/brainways/project/_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import json
 import pickle
+from dataclasses import asdict
 from pathlib import Path
 from typing import Optional
 
+import dacite
 from packaging import version
 
 import brainways
+from brainways.project.info_classes import SliceInfo, SubjectFileFormat, SubjectInfo
 from brainways.utils.io_utils.readers.qupath_reader import QupathReader
 
 
 def rewrite_project_version(path: Path, version: Optional[str] = None):
     if version is None:
         version = brainways._version.version
 
@@ -21,41 +24,74 @@
 
 
 def update_project_from_previous_versions(path: Path):
     with open(path) as f:
         serialized_settings = json.load(f)
     project_version = serialized_settings.get("version", "0.1.1")
     if version.parse(project_version) <= version.parse("0.1.1"):
-        update_project_from_0_1_1_to_0_1_4(path)
+        update_project_to_0_1_4(path)
     if version.parse(project_version) <= version.parse("0.1.4"):
-        update_project_from_0_1_4_to_0_1_5(path)
+        update_project_to_0_1_5(path)
+    if version.parse(project_version) <= version.parse("0.1.7"):
+        update_project_to_0_1_7(path)
 
-    rewrite_project_version(path)
+    if project_version != brainways._version.version:
+        rewrite_project_version(path)
 
 
-def update_project_from_0_1_1_to_0_1_4(path: Path):
+def update_project_to_0_1_4(path: Path):
     brainways_subject_paths = path.parent.rglob("brainways.bin")
     for brainways_subject_path in brainways_subject_paths:
         with open(brainways_subject_path, "rb") as f:
             serialized_settings, serialized_slice_infos = pickle.load(f)
         for serialized_slice_info in serialized_slice_infos:
             if "cell" in serialized_slice_info["params"]:
                 del serialized_slice_info["params"]["cell"]
         with open(brainways_subject_path, "wb") as f:
             pickle.dump((serialized_settings, serialized_slice_infos), f)
 
     rewrite_project_version(path=path, version="0.1.4")
 
 
-def update_project_from_0_1_4_to_0_1_5(path: Path):
+def update_project_to_0_1_5(path: Path):
     brainways_subject_paths = path.parent.rglob("brainways.bin")
     for brainways_subject_path in brainways_subject_paths:
         with open(brainways_subject_path, "rb") as f:
             serialized_settings, serialized_slice_infos = pickle.load(f)
         for serialized_slice_info in serialized_slice_infos:
             reader = QupathReader(serialized_slice_info["path"]["filename"])
             pps = reader.physical_pixel_sizes
             serialized_slice_info["physical_pixel_sizes"] = (pps.Y, pps.X)
         with open(brainways_subject_path, "wb") as f:
             pickle.dump((serialized_settings, serialized_slice_infos), f)
 
     rewrite_project_version(path=path, version="0.1.5")
+
+
+def update_project_to_0_1_7(path: Path):
+    brainways_subject_paths = path.parent.rglob("brainways.bin")
+    for brainways_subject_path in brainways_subject_paths:
+        with open(brainways_subject_path, "rb") as f:
+            serialized_settings, serialized_slice_infos = pickle.load(f)
+        subject_info = SubjectInfo(name=brainways_subject_path.parent.name)
+        slice_infos = []
+        for serialized_slice_info in serialized_slice_infos:
+            if (
+                "tps" in serialized_slice_info["params"]
+                and serialized_slice_info["params"]["tps"] is not None
+            ):
+                serialized_slice_info["params"]["tps"][
+                    "points_src"
+                ] = serialized_slice_info["params"]["tps"]["points_src"].tolist()
+                serialized_slice_info["params"]["tps"][
+                    "points_dst"
+                ] = serialized_slice_info["params"]["tps"]["points_dst"].tolist()
+                slice_infos.append(dacite.from_dict(SliceInfo, serialized_slice_info))
+        subject_file = SubjectFileFormat(
+            subject_info=subject_info,
+            slice_infos=slice_infos,
+        )
+        with open(brainways_subject_path.parent / "data.bws", "w") as f:
+            json.dump(asdict(subject_file), f)
+        brainways_subject_path.unlink()
+
+    rewrite_project_version(path=path, version="0.1.7")
```

### Comparing `brainways-0.1.6/src/brainways/project/brainways_project.py` & `brainways-0.1.7/src/brainways/project/brainways_project.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,48 @@
 import json
-from dataclasses import asdict
+from dataclasses import asdict, fields
+from itertools import combinations
 from pathlib import Path
-from typing import Callable, Iterator, List, Optional, Union
+from typing import Callable, Iterator, List, Optional, Tuple, Union
 
 import dacite
 import pandas as pd
 from natsort import natsorted, ns
 from pandas import ExcelWriter
 
 from brainways.pipeline.brainways_pipeline import BrainwaysPipeline
 from brainways.pipeline.cell_detector import CellDetector
 from brainways.project._utils import update_project_from_previous_versions
 from brainways.project.brainways_subject import BrainwaysSubject
-from brainways.project.info_classes import ExcelMode, ProjectSettings, SliceInfo
+from brainways.project.info_classes import (
+    ExcelMode,
+    ProjectSettings,
+    SliceInfo,
+    SubjectInfo,
+)
 from brainways.utils.atlas.brainways_atlas import BrainwaysAtlas
 from brainways.utils.cell_detection_importer.cell_detection_importer import (
     CellDetectionImporter,
 )
+from brainways.utils.contrast import calculate_contrast
 
 
 class BrainwaysProject:
     def __init__(
         self,
         subjects: List[BrainwaysSubject],
         settings: ProjectSettings,
-        path: Optional[Path] = None,
+        path: Path,
         lazy_init: bool = False,
     ):
-        if path is not None and path.suffix != ".bwp":
+        if path.suffix != ".bwp":
             raise ValueError(f"Brainways project must be of .bwp file type, got {path}")
 
         self.path = path
+        self._results_path = self.path.parent / "results.xlsx"
         self.subjects = subjects
         self.settings = settings
 
         self.atlas: Optional[BrainwaysAtlas] = None
         self.pipeline: Optional[BrainwaysPipeline] = None
 
         if not lazy_init:
@@ -56,20 +64,18 @@
             project_dir = path
             path = path / "brainways.bwp"
 
         if not force and project_dir.exists() and len(list(project_dir.glob("*"))) > 0:
             raise FileExistsError(f"Directory is not empty: {project_dir}")
 
         project_dir.mkdir(parents=True, exist_ok=True)
+        project = cls(subjects=[], settings=settings, path=path, lazy_init=lazy_init)
+        project.save()
 
-        serialized_settings = asdict(settings)
-        with open(path, "w") as f:
-            json.dump(serialized_settings, f)
-
-        return cls.open(path, lazy_init=lazy_init)
+        return project
 
     @classmethod
     def open(cls, path: Union[Path, str], lazy_init: bool = False):
         path = Path(path)
         if not path.exists():
             raise FileNotFoundError(f"BrainwaysProject file not found: {path}")
         if not path.suffix == ".bwp":
@@ -79,127 +85,107 @@
 
         with open(path) as f:
             serialized_settings = json.load(f)
 
         settings = dacite.from_dict(
             ProjectSettings, serialized_settings, config=dacite.Config(cast=[tuple])
         )
+
+        project = cls(subjects=[], settings=settings, path=path, lazy_init=lazy_init)
         subject_directories = [d for d in path.parent.glob("*") if d.is_dir()]
         subject_directories = natsorted(
             subject_directories, alg=ns.IGNORECASE, key=lambda x: x.name
         )
         subjects = [
-            BrainwaysSubject.open(subject_path) for subject_path in subject_directories
+            BrainwaysSubject.open(path=subject_path / "data.bws", project=project)
+            for subject_path in subject_directories
         ]
-        return cls(subjects=subjects, settings=settings, path=path, lazy_init=lazy_init)
+        project.subjects = subjects
+        return project
 
     def save(self):
         serialized_settings = asdict(self.settings)
         with open(self.path, "w") as f:
             json.dump(serialized_settings, f)
 
-    def add_subject(self, id: str) -> BrainwaysSubject:
-        subject = BrainwaysSubject(
-            settings=self.settings, subject_path=self.path.parent / id
-        )
+    def add_subject(self, subject_info: SubjectInfo) -> BrainwaysSubject:
+        subject = BrainwaysSubject.create(subject_info=subject_info, project=self)
         self.subjects.append(subject)
         return subject
 
     def load_atlas(self, load_volumes: bool = True):
         self.atlas = BrainwaysAtlas.load(
             self.settings.atlas, exclude_regions=[76, 42, 41]
         )  # TODO: from model
 
-        for subject in self.subjects:
-            subject.atlas = self.atlas
-
         # load volumes to cache
         if load_volumes:
             _ = self.atlas.reference
             _ = self.atlas.annotation
             _ = self.atlas.hemispheres
 
     def load_pipeline(self):
         if self.atlas is None:
             self.load_atlas()
         self.pipeline = BrainwaysPipeline(self.atlas)
-        for subject in self.subjects:
-            subject.pipeline = self.pipeline
 
     def move_images_directory(
         self, new_images_root: Path, old_images_root: Optional[Path] = None
     ):
         for subject in self.subjects:
             subject.move_images_root(
                 new_images_root=new_images_root, old_images_root=old_images_root
             )
             subject.save()
 
-    def create_excel_iter(
+    def calculate_results_iter(
         self,
-        path: Union[Path, str],
+        path: Optional[Union[Path, str]] = None,
         slice_info_predicate: Optional[Callable[[SliceInfo], bool]] = None,
         min_region_area_um2: Optional[int] = None,
         cells_per_area_um2: Optional[int] = None,
         min_cell_size_um: Optional[float] = None,
         max_cell_size_um: Optional[float] = None,
         excel_mode: ExcelMode = ExcelMode.ROW_PER_SUBJECT,
     ) -> Iterator:
+        if path is None:
+            path = self._results_path
         if not path.suffix == ".xlsx":
             path = Path(str(path) + ".xlsx")
 
-        cells_per_area_sheet = []
-        cells_count_sheet = []
+        results = []
         for subject in self.subjects:
-            cells_per_area_sheet.append(
+            results.append(
                 subject.cell_count_summary(
                     slice_info_predicate=slice_info_predicate,
                     min_region_area_um2=min_region_area_um2,
                     cells_per_area_um2=cells_per_area_um2,
                     min_cell_size_um=min_cell_size_um,
                     max_cell_size_um=max_cell_size_um,
                     excel_mode=excel_mode,
                 )
             )
 
-            cells_count_sheet.append(
-                subject.cell_count_summary(
-                    slice_info_predicate=slice_info_predicate,
-                    min_region_area_um2=min_region_area_um2,
-                    min_cell_size_um=min_cell_size_um,
-                    max_cell_size_um=max_cell_size_um,
-                    excel_mode=excel_mode,
-                )
-            )
-
             yield
 
-        cells_per_area_sheet = pd.concat(
-            [sheet for sheet in cells_per_area_sheet if sheet is not None], axis=0
-        )
-        cells_count_sheet = pd.concat(
-            [sheet for sheet in cells_count_sheet if sheet is not None], axis=0
-        )
+        results = pd.concat([sheet for sheet in results if sheet is not None], axis=0)
         with ExcelWriter(path) as writer:
-            cells_per_area_sheet.to_excel(
-                writer, sheet_name=f"Cells per {cells_per_area_um2}um2", index=False
-            )
-            cells_count_sheet.to_excel(writer, sheet_name="Cell count", index=False)
+            results.to_excel(writer, index=False)
 
-    def create_excel(
+    def calculate_results(
         self,
-        path: Union[Path, str],
+        path: Optional[Union[Path, str]] = None,
         slice_info_predicate: Optional[Callable[[SliceInfo], bool]] = None,
         min_region_area_um2: Optional[int] = None,
         cells_per_area_um2: Optional[int] = None,
         min_cell_size_um: Optional[float] = None,
         max_cell_size_um: Optional[float] = None,
         excel_mode: ExcelMode = ExcelMode.ROW_PER_SUBJECT,
     ) -> None:
-        for _ in self.create_excel_iter(
+        for _ in self.calculate_results_iter(
             path=path,
             slice_info_predicate=slice_info_predicate,
             min_region_area_um2=min_region_area_um2,
             cells_per_area_um2=cells_per_area_um2,
             min_cell_size_um=min_cell_size_um,
             max_cell_size_um=max_cell_size_um,
             excel_mode=excel_mode,
@@ -238,13 +224,83 @@
     def run_cell_detector(self) -> None:
         cell_detector = CellDetector()
         for subject in self.subjects:
             subject.run_cell_detector(
                 cell_detector, default_params=self.settings.default_cell_detector_params
             )
 
+    def calculate_contrast(
+        self,
+        condition_col: str,
+        values_col: str,
+        min_group_size: int,
+        pvalue: float,
+        multiple_comparisons_method: str = "fdr_bh",
+    ):
+        if not self.can_calculate_contrast(condition_col):
+            raise RuntimeError(
+                "Can't calculate contrast, some slice has missing parameters or missing"
+                " conditions"
+            )
+
+        if not self._results_path.exists():
+            raise RuntimeError("Calculate results before calculating contrast")
+
+        results_df = pd.read_excel(self._results_path)
+        anova_df, posthoc_df = calculate_contrast(
+            results_df=results_df,
+            condition_col=condition_col,
+            values_col=values_col,
+            posthoc_comparisons=self.possible_contrasts(condition_col),
+            min_group_size=min_group_size,
+            pvalue=pvalue,
+            multiple_comparisons_method=multiple_comparisons_method,
+        )
+
+        contrast_path = self.path.parent / f"contrast-{condition_col}-{values_col}.xlsx"
+        with ExcelWriter(contrast_path) as writer:
+            anova_df.to_excel(writer, sheet_name="ANOVA")
+            posthoc_df.to_excel(writer, sheet_name="Posthoc")
+
+        return anova_df, posthoc_df
+
+    def next_slice_missing_params(self) -> Optional[Tuple[int, int]]:
+        for subject_idx, subject in enumerate(self.subjects):
+            for slice_idx, slice_info in subject.valid_documents:
+                for field in fields(slice_info.params):
+                    if (
+                        getattr(slice_info.params, field.name) is None
+                        and field.name != "cell"
+                    ):
+                        return subject_idx, slice_idx
+        return None
+
+    def can_calculate_results(self) -> bool:
+        return self.next_slice_missing_params() is None
+
+    def can_calculate_contrast(self, condition: str) -> bool:
+        conditions = set()
+        for subject in self.subjects:
+            if subject.subject_info.conditions is not None:
+                conditions.add(subject.subject_info.conditions.get(condition))
+            else:
+                conditions.add(None)
+        return (
+            self.can_calculate_results()
+            and None not in conditions
+            and len(conditions) > 1
+        )
+
     @property
     def n_valid_images(self):
         return sum(len(subject.valid_documents) for subject in self.subjects)
 
+    def possible_contrasts(self, condition: str) -> List[Tuple[str, str]]:
+        condition_values = {
+            subject.subject_info.conditions.get(condition) for subject in self.subjects
+        }
+        condition_values -= {None}
+        possible_contrasts = list(combinations(sorted(condition_values), 2))
+        return possible_contrasts
+
     def __len__(self) -> int:
         return len(self.subjects)
```

### Comparing `brainways-0.1.6/src/brainways/project/brainways_subject.py` & `brainways-0.1.7/src/brainways/project/brainways_subject.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+import json
 import logging
-import pickle
-import shutil
-import tempfile
 from collections import Counter
 from dataclasses import asdict, replace
 from pathlib import Path
-from typing import Callable, Iterator, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Callable, Iterator, List, Optional, Tuple, Union
 
 import dacite
 import numpy as np
 import pandas as pd
 from PIL import Image
 
 from brainways.pipeline.brainways_params import CellDetectorParams
 from brainways.pipeline.brainways_pipeline import BrainwaysPipeline, PipelineStep
 from brainways.pipeline.cell_detector import CellDetector
-from brainways.project.info_classes import ExcelMode, ProjectSettings, SliceInfo
+from brainways.project.info_classes import (
+    ExcelMode,
+    SliceInfo,
+    SubjectFileFormat,
+    SubjectInfo,
+)
 from brainways.utils.atlas.brainways_atlas import BrainwaysAtlas
 from brainways.utils.cell_count_summary import cell_count_summary
 from brainways.utils.cell_detection_importer.cell_detection_importer import (
     CellDetectionImporter,
 )
 from brainways.utils.cells import (
     filter_cells_by_size,
@@ -28,82 +31,80 @@
     get_region_areas,
 )
 from brainways.utils.image import brain_mask_simple, get_resize_size, slice_to_uint8
 from brainways.utils.io_utils import ImagePath
 from brainways.utils.io_utils.readers import get_image_size
 from brainways.utils.io_utils.readers.qupath_reader import QupathReader
 
+if TYPE_CHECKING:
+    from brainways.project.brainways_project import BrainwaysProject
+
 
 class BrainwaysSubject:
     def __init__(
         self,
-        settings: ProjectSettings,
-        documents: List[SliceInfo] = None,
-        subject_path: Optional[Union[Path, str]] = None,
-        atlas: Optional[BrainwaysAtlas] = None,
-        pipeline: Optional[BrainwaysPipeline] = None,
+        subject_info: SubjectInfo,
+        slice_infos: List[SliceInfo],
+        project: "BrainwaysProject",
     ):
-        if atlas is not None:
-            if atlas.brainglobe_atlas.atlas_name != settings.atlas:
-                raise ValueError(
-                    "Input atlas doesn't match atlas in subject settings "
-                    f"({atlas.brainglobe_atlas.atlas_name} != {settings.atlas})"
-                )
-        self.documents: List[SliceInfo] = documents or []
-        self.settings = settings
-        self.atlas = atlas
-        self.pipeline = pipeline
-        self._tmpdir = None
-
-        # TODO: refactor, BrainwaysSubject.create() and BrainwaysSubject.open()
-        if subject_path is None:
-            self._tmpdir = tempfile.TemporaryDirectory()
-            self.subject_path = Path(self._tmpdir.name)
-        else:
-            self.subject_path = self._get_subject_dir(subject_path)
-            if not (self.subject_path / "brainways.bin").exists():
-                if self.subject_path.exists():
-                    if not self.subject_path.is_dir() or any(
-                        self.subject_path.iterdir()
-                    ):
-                        raise FileExistsError(
-                            f"New subject directory {self.subject_path} is not empty!"
-                        )
-                else:
-                    self.subject_path.mkdir()
+        self.subject_info = subject_info
+        self.documents = slice_infos
+        self.project = project
+        self._save_dir = project.path.parent / self.subject_info.name
+
+    @classmethod
+    def create(
+        cls, subject_info: SubjectInfo, project: "BrainwaysProject"
+    ) -> "BrainwaysSubject":
+        subject = cls(subject_info=subject_info, slice_infos=[], project=project)
+
+        if subject._save_dir.exists():
+            raise FileExistsError(
+                f"Subject directory {subject._save_dir} already exists"
+            )
 
-        if not self.thumbnails_root.exists():
-            self.thumbnails_root.mkdir()
+        subject._save_dir.mkdir()
+        subject.thumbnails_root.mkdir()
+        subject.cell_detections_root.mkdir()
+        subject.save()
+        return subject
+
+    @classmethod
+    def open(cls, path: Union[Path, str], project: "BrainwaysProject"):
+        if not path.exists():
+            raise FileNotFoundError(f"Subject file not found: {path}")
+
+        with open(path) as f:
+            serialized_file = json.load(f)
 
-        if not self.cell_detections_root.exists():
-            self.cell_detections_root.mkdir()
+        subject_file = dacite.from_dict(
+            SubjectFileFormat, serialized_file, config=dacite.Config(cast=[tuple])
+        )
+        subject = BrainwaysSubject(
+            subject_info=subject_file.subject_info,
+            slice_infos=subject_file.slice_infos,
+            project=project,
+        )
 
-    def close(self):
-        self.documents = []
-        self.settings = None
-        self.atlas = None
-        self.pipeline = None
-        self.subject_path = None
-        if self._tmpdir is not None:
-            self._tmpdir.cleanup()
+        return subject
 
     def read_lowres_image(
         self, document: SliceInfo, channel: Optional[int] = None
     ) -> np.ndarray:
         thumbnail_path = self.thumbnail_path(
-            document.path, channel=channel or self.settings.channel
+            document.path, channel=channel or self.project.settings.channel
         )
         if thumbnail_path.exists():
             image = np.array(Image.open(thumbnail_path))
         else:
             reader = QupathReader(document.path.filename)
             reader.set_scene(document.path.scene)
             image = reader.get_thumbnail(
                 target_size=document.lowres_image_size,
-                channel=channel or self.settings.channel,
+                channel=channel or self.project.settings.channel,
             )
             image = slice_to_uint8(image)
             Image.fromarray(image).save(thumbnail_path)
         return image
 
     def read_highres_image(self, document: SliceInfo, level: Optional[int] = None):
         reader = QupathReader(document.path.filename)
@@ -126,66 +127,21 @@
             physical_pixel_sizes=(pps.Y, pps.X),
         )
         if load_thumbnail:
             self.read_lowres_image(document)
         self.documents.append(document)
         return document
 
-    @staticmethod
-    def _get_subject_dir(path: Union[Path, str]):
-        subject_dir = Path(path)
-        if subject_dir.name == "brainways.bin":
-            subject_dir = subject_dir.parent
-        return subject_dir
-
-    @classmethod
-    def open(
-        cls,
-        path: Union[Path, str],
-        atlas: Optional[BrainwaysAtlas] = None,
-        pipeline: Optional[BrainwaysPipeline] = None,
-    ):
-        subject_dir = BrainwaysSubject._get_subject_dir(path)
-        if not subject_dir.exists():
-            raise FileNotFoundError(f"subject path not found: {path}")
-
-        with open(subject_dir / "brainways.bin", "rb") as f:
-            serialized_settings, serialized_documents = pickle.load(f)
-
-        settings = dacite.from_dict(ProjectSettings, serialized_settings)
-        documents = [dacite.from_dict(SliceInfo, d) for d in serialized_documents]
-        subject = BrainwaysSubject(
-            settings=settings,
-            documents=documents,
-            subject_path=subject_dir,
-            atlas=atlas,
-            pipeline=pipeline,
+    def save(self):
+        subject_file = SubjectFileFormat(
+            subject_info=self.subject_info, slice_infos=self.documents
         )
-
-        return subject
-
-    def save(self, path: Optional[Union[Path, str]] = None):
-        if path is None:
-            path = self.subject_path
-        path = Path(path)
-        subject_dir = self._get_subject_dir(path)
-        if subject_dir != self.subject_path:
-            if subject_dir.exists():
-                if subject_dir.is_dir() and not any(subject_dir.iterdir()):
-                    shutil.rmtree(str(subject_dir))
-                else:
-                    raise FileExistsError(
-                        f"subject directory {subject_dir} is not empty!"
-                    )
-            shutil.move(str(self.subject_path), str(subject_dir))
-            self.subject_path = subject_dir
-        serialized_settings = asdict(self.settings)
-        serialized_documents = [asdict(d) for d in self.documents]
-        with open(subject_dir / "brainways.bin", "wb") as f:
-            pickle.dump((serialized_settings, serialized_documents), f)
+        serialized_file = asdict(subject_file)
+        with open(self._save_dir / "data.bws", "w") as f:
+            json.dump(serialized_file, f)
 
     def move_images_root(
         self,
         new_images_root: Union[Path, str],
         old_images_root: Optional[Union[Path, str]] = None,
     ):
         new_images_root = Path(new_images_root)
@@ -240,14 +196,15 @@
     def run_cell_detector_iter(
         self, cell_detector: CellDetector, default_params: CellDetectorParams
     ) -> Iterator:
         for i, document in self.valid_documents:
             try:
                 cell_detections_path = self.cell_detections_path(document.path)
                 if cell_detections_path.exists():
+                    yield
                     continue
                 reader = document.image_reader()
                 image = reader.get_image_dask_data(
                     "YX", C=self.settings.channel
                 ).compute()
                 if document.params.cell is not None:
                     cell_detector_params = document.params.cell
@@ -409,14 +366,15 @@
                     cell_count_summary(
                         animal_id=str(document.path),
                         cells=cells,
                         region_areas_um=region_areas,
                         atlas=self.atlas,
                         min_region_area_um2=min_region_area_um2,
                         cells_per_area_um2=cells_per_area_um2,
+                        conditions=self.subject_info.conditions,
                     )
                 )
             else:
                 all_cells_on_atlas.append(cells)
                 all_region_areas.update(region_areas)
 
         if excel_mode == ExcelMode.ROW_PER_IMAGE:
@@ -424,46 +382,55 @@
         else:
             if len(all_cells_on_atlas) == 0:
                 logging.warning(f"{document.path}: not found cells on atlas")
                 return
 
             all_cells_on_atlas = pd.concat(all_cells_on_atlas, axis=0)
             df = cell_count_summary(
-                animal_id=self.subject_path.name,
+                animal_id=self.subject_info.name,
                 cells=all_cells_on_atlas,
                 region_areas_um=all_region_areas,
                 atlas=self.atlas,
                 min_region_area_um2=min_region_area_um2,
                 cells_per_area_um2=cells_per_area_um2,
+                conditions=self.subject_info.conditions,
             )
         return df
 
     def thumbnail_path(self, image_path: ImagePath, channel: Optional[int] = None):
         if channel is None:
-            channel = self.settings.channel
+            channel = self.project.settings.channel
 
         suffixes = []
         if image_path.scene is not None:
             suffixes.append(f"Scene #{image_path.scene}")
         suffixes.append(f"Channel #{channel}")
         suffix = " ".join(suffixes)
         thumbnail_filename = f"{Path(image_path.filename).stem} [{suffix}].jpg"
         return self.thumbnails_root / thumbnail_filename
 
     def cell_detections_path(self, image_path: ImagePath) -> Path:
         return self.cell_detections_root / (Path(str(image_path)).name + ".csv")
 
     @property
     def thumbnails_root(self) -> Path:
-        return self.subject_path / "thumbnails"
+        return self._save_dir / "thumbnails"
 
     @property
     def cell_detections_root(self) -> Path:
-        return self.subject_path / "cell_detections"
+        return self._save_dir / "cell_detections"
 
     @property
     def valid_documents(self) -> List[Tuple[int, SliceInfo]]:
         return [
             (i, document)
             for i, document in enumerate(self.documents)
             if not document.ignore
         ]
+
+    @property
+    def pipeline(self) -> BrainwaysPipeline:
+        return self.project.pipeline
+
+    @property
+    def atlas(self) -> BrainwaysAtlas:
+        return self.project.atlas
```

### Comparing `brainways-0.1.6/src/brainways/project/info_classes.py` & `brainways-0.1.7/src/brainways/project/info_classes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,56 @@
 from __future__ import annotations
 
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from enum import Enum, auto
-from typing import Optional, Tuple, Union
+from typing import Dict, List, Optional, Tuple, Union
 
 import brainways._version
 from brainways.pipeline.brainways_params import BrainwaysParams, CellDetectorParams
 from brainways.utils.dataclasses import dataclass_eq
 from brainways.utils.image import ImageSizeHW
 from brainways.utils.io_utils import ImagePath
 from brainways.utils.io_utils.readers import QupathReader
 
 
 @dataclass(frozen=True)
 class ProjectSettings:
     atlas: str
     channel: Union[int, str]
     default_cell_detector_params: CellDetectorParams = CellDetectorParams()
+    condition_names: List[str] = field(default_factory=list)
     version: str = brainways._version.version
 
 
 @dataclass(frozen=True)
-class SubjectSettings:
+class SubjectInfo:
     name: str
-    condition: Optional[str] = None
-    exclude: bool = False
+    conditions: Dict[str, str] = field(default_factory=dict)
 
 
 @dataclass(frozen=True, eq=False)
 class SliceInfo:
     path: ImagePath
     image_size: ImageSizeHW
     lowres_image_size: ImageSizeHW
-    params: Optional[BrainwaysParams] = BrainwaysParams()
+    params: BrainwaysParams = BrainwaysParams()
     ignore: bool = False
     physical_pixel_sizes: Optional[Tuple[float, float]] = None
 
     def image_reader(self) -> QupathReader:
         reader = QupathReader(self.path.filename)
         reader.set_scene(self.path.scene)
         return reader
 
     def __eq__(self, other):
         return dataclass_eq(self, other)
 
 
+@dataclass(frozen=True)
+class SubjectFileFormat:
+    subject_info: SubjectInfo
+    slice_infos: List[SliceInfo]
+
+
 class ExcelMode(Enum):
     ROW_PER_SUBJECT = auto()
     ROW_PER_IMAGE = auto()
```

### Comparing `brainways-0.1.6/src/brainways/scripts/_tests/test_cli.py` & `brainways-0.1.7/src/brainways/scripts/_tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/scripts/batch_create_thumbnails.py` & `brainways-0.1.7/src/brainways/scripts/batch_create_thumbnails.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/scripts/cell_detection.py` & `brainways-0.1.7/src/brainways/scripts/cell_detection.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/scripts/cli.py` & `brainways-0.1.7/src/brainways/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/scripts/create_excel.py` & `brainways-0.1.7/src/brainways/scripts/create_excel.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     cells_per_area_um2: Optional[int],
     min_cell_size_um: Optional[float],
     max_cell_size_um: Optional[float],
     excel_mode: ExcelMode,
 ):
     project = BrainwaysProject.open(project_path)
     for _ in tqdm(
-        project.create_excel_iter(
+        project.calculate_results_iter(
             path=output,
             min_region_area_um2=min_region_area_um2,
             cells_per_area_um2=cells_per_area_um2,
             min_cell_size_um=min_cell_size_um,
             max_cell_size_um=max_cell_size_um,
             excel_mode=excel_mode,
         ),
```

### Comparing `brainways-0.1.6/src/brainways/scripts/create_excel_colabelling.py` & `brainways-0.1.7/src/brainways/scripts/create_excel_colabelling.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/scripts/create_reg_model_data.py` & `brainways-0.1.7/src/brainways/scripts/create_reg_model_data.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/scripts/display_area.py` & `brainways-0.1.7/src/brainways/scripts/display_area.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/scripts/import_cell_detections_keren.py` & `brainways-0.1.7/src/brainways/scripts/import_cell_detections_keren.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/scripts/import_cells.py` & `brainways-0.1.7/src/brainways/scripts/import_cells.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/scripts/move_images.py` & `brainways-0.1.7/src/brainways/scripts/move_images.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/transforms/_tests/test_affine_transform_2d.py` & `brainways-0.1.7/src/brainways/transforms/_tests/test_affine_transform_2d.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/transforms/_tests/test_depth_registration.py` & `brainways-0.1.7/src/brainways/transforms/_tests/test_depth_registration.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/transforms/_tests/test_image_to_atlas_transform.py` & `brainways-0.1.7/src/brainways/transforms/_tests/test_image_to_atlas_transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,17 @@
         atlas_transform=DepthRegistration(
             DepthRegistrationParams(), volume_shape=(10, 10, 10)
         ),
         affine_2d_transform=BrainwaysAffineTransform2D(
             AffineTransform2DParams(tx=10, ty=10), input_size=(64, 64)
         ),
         tps_transform=TPSTransform(
-            TPSTransformParams(points_src=tps_points_src, points_dst=tps_points_dst)
+            TPSTransformParams(
+                points_src=tps_points_src.tolist(), points_dst=tps_points_dst.tolist()
+            )
         ),
     )
 
 
 @pytest.mark.skip
 def test_image_to_atlas_transform_inv_points(
     image_to_atlas_transform: ImageToAtlasTransform,
```

### Comparing `brainways-0.1.6/src/brainways/transforms/_tests/test_tps_transform.py` & `brainways-0.1.7/src/brainways/transforms/_tests/test_tps_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from brainways.pipeline.brainways_params import TPSTransformParams
 from brainways.transforms.tps_transform import TPSTransform
 
 
 def test_tps_transform_points():
     points_src = np.random.randint(0, 10, (5, 2))
     points_dst = points_src + np.random.randint(0, 2, (5, 2))
-    params = TPSTransformParams(points_src, points_dst)
+    params = TPSTransformParams(points_src.tolist(), points_dst.tolist())
     transform = TPSTransform(params)
     points_transformed = transform.transform_points(points_src)
     npt.assert_allclose(points_transformed, points_dst, rtol=1e-4, atol=1e-3)
 
 
 def test_tps_transform_image_doesnt_change_image_on_same_points():
     points = np.random.rand(5, 2).astype(np.float32) * 5
```

### Comparing `brainways-0.1.6/src/brainways/transforms/affine_transform_2d.py` & `brainways-0.1.7/src/brainways/transforms/affine_transform_2d.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/transforms/compose.py` & `brainways-0.1.7/src/brainways/transforms/compose.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/transforms/depth_registration.py` & `brainways-0.1.7/src/brainways/transforms/depth_registration.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/transforms/image_to_atlas_transform.py` & `brainways-0.1.7/src/brainways/transforms/image_to_atlas_transform.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/transforms/tps_transform.py` & `brainways-0.1.7/src/brainways/transforms/tps_transform.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,24 +14,24 @@
     def __init__(self, params: TPSTransformParams, scale: Optional[float] = None):
         self.scale = scale
 
         scale = scale or 1.0
         self.params = params
         matches = [cv2.DMatch(i, i, 0) for i in range(len(self.params.points_src))]
         self.tps_image = cv2.createThinPlateSplineShapeTransformer()
+
+        points_src_np = np.array(self.params.points_src, dtype=np.float32)[None]
+        points_dst_np = np.array(self.params.points_dst, dtype=np.float32)[None]
+
         self.tps_image.estimateTransformation(
-            self.params.points_dst[None] * scale,
-            self.params.points_src[None] * scale,
-            matches,
+            points_dst_np * scale, points_src_np * scale, matches
         )
         self.tps_points = cv2.createThinPlateSplineShapeTransformer()
         self.tps_points.estimateTransformation(
-            self.params.points_src[None] * scale,
-            self.params.points_dst[None] * scale,
-            matches,
+            points_src_np * scale, points_dst_np * scale, matches
         )
 
     def inv(self):
         params_inv = TPSTransformParams(
             points_src=self.params.points_dst,
             points_dst=self.params.points_src,
         )
```

### Comparing `brainways-0.1.6/src/brainways/utils/_imports.py` & `brainways-0.1.7/src/brainways/utils/_imports.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/utils/_tests/test_cells.py` & `brainways-0.1.7/src/brainways/utils/_tests/test_cells.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/utils/_tests/test_image.py` & `brainways-0.1.7/src/brainways/utils/_tests/test_image.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/utils/atlas/_tests/test_slice_atlas.py` & `brainways-0.1.7/src/brainways/utils/atlas/_tests/test_slice_atlas.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/utils/atlas/brainways_atlas.py` & `brainways-0.1.7/src/brainways/utils/atlas/brainways_atlas.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/utils/atlas/slice_atlas.py` & `brainways-0.1.7/src/brainways/utils/atlas/slice_atlas.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/utils/cell_count_summary.py` & `brainways-0.1.7/src/brainways/utils/cell_count_summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,61 +97,68 @@
 def cell_count_summary(
     animal_id: str,
     cells: pd.DataFrame,
     region_areas_um: Dict[int, int],
     atlas: BrainwaysAtlas,
     min_region_area_um2: Optional[int] = None,
     cells_per_area_um2: Optional[int] = None,
+    conditions: Optional[Dict[str, str]] = None,
 ):
     cells = set_co_labelling_product(cells)
     cell_counts = get_cell_counts(cells)
     all_leaf_structures = list(
         set(list(cell_counts.index) + list(region_areas_um.keys()))
     )
     cell_counts = extend_cell_counts_to_parent_regions(
         cell_counts=cell_counts, atlas=atlas, structure_ids=all_leaf_structures
     )
     region_areas_um = extend_region_areas_to_parent_regions(
         region_areas=region_areas_um, atlas=atlas, structure_ids=all_leaf_structures
     )
 
+    cell_counts = format_cell_counts_to_output(cell_counts)
+
     if cells_per_area_um2:
         region_areas_um_list = [region_areas_um[i] for i in cell_counts.index]
-        cell_counts = (
+        cell_counts_normalized = (
             cell_counts.div(region_areas_um_list, axis=0) * cells_per_area_um2**2
         )
 
+        cell_counts = pd.concat(
+            [cell_counts_normalized, cell_counts.add_suffix(" (not normalized)")],
+            axis="columns",
+        )
+
     df = []
     atlas_structure_leave_ids = [
         node.identifier for node in atlas.brainglobe_atlas.structures.tree.leaves()
     ]
 
-    cell_counts_output = format_cell_counts_to_output(cell_counts)
-
     for struct_id in region_areas_um:
         if struct_id not in atlas.brainglobe_atlas.structures:
             continue
         struct = atlas.brainglobe_atlas.structures[struct_id]
 
         if min_region_area_um2 is not None and region_areas_um[struct_id] < (
             min_region_area_um2**2
         ):
             continue
 
         df.append(
             {
+                **(conditions or {}),
                 "animal_id": animal_id,
                 "acronym": struct["acronym"],
                 "name": struct["name"],
                 "is_parent_structure": struct_id not in atlas_structure_leave_ids,
                 "is_gray_matter": get_struct_is_gray_matter(
                     struct_id=struct_id, atlas=atlas
                 ),
                 "total_area_um2": int(region_areas_um[struct_id]),
-                **dict(cell_counts_output.loc[struct_id]),
+                **dict(cell_counts.loc[struct_id]),
             }
         )
     df = pd.DataFrame(df)
     return df
 
 
 def format_cell_counts_to_output(cells: pd.DataFrame) -> pd.DataFrame:
```

### Comparing `brainways-0.1.6/src/brainways/utils/cell_detection_importer/_tests/qupath_sample_file.txt` & `brainways-0.1.7/src/brainways/utils/cell_detection_importer/_tests/qupath_sample_file.txt`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/utils/cell_detection_importer/_tests/test_brainways_cell_detection_importer.py` & `brainways-0.1.7/src/brainways/utils/cell_detection_importer/_tests/test_brainways_cell_detection_importer.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/utils/cell_detection_importer/_tests/test_qupath_cell_detection_importer.py` & `brainways-0.1.7/src/brainways/utils/cell_detection_importer/_tests/test_qupath_cell_detection_importer.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/utils/cell_detection_importer/brainways_cell_detection_importer.py` & `brainways-0.1.7/src/brainways/utils/cell_detection_importer/brainways_cell_detection_importer.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/utils/cell_detection_importer/keren_cell_detection_importer.py` & `brainways-0.1.7/src/brainways/utils/cell_detection_importer/keren_cell_detection_importer.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/utils/cell_detection_importer/utils.py` & `brainways-0.1.7/src/brainways/utils/cell_detection_importer/utils.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/utils/cells.py` & `brainways-0.1.7/src/brainways/utils/cells.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/utils/config.py` & `brainways-0.1.7/src/brainways/utils/config.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/utils/czi/czi_to_jpg.py` & `brainways-0.1.7/src/brainways/utils/czi/czi_to_jpg.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/utils/dataclasses.py` & `brainways-0.1.7/src/brainways/utils/dataclasses.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/utils/image.py` & `brainways-0.1.7/src/brainways/utils/image.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/utils/io_utils/file_iterators/qupath.py` & `brainways-0.1.7/src/brainways/utils/io_utils/file_iterators/qupath.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/utils/io_utils/image_path.py` & `brainways-0.1.7/src/brainways/utils/io_utils/image_path.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/utils/io_utils/readers/__init__.py` & `brainways-0.1.7/src/brainways/utils/io_utils/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/utils/io_utils/readers/aicsimageio_reader.py` & `brainways-0.1.7/src/brainways/utils/io_utils/readers/aicsimageio_reader.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/utils/io_utils/readers/base.py` & `brainways-0.1.7/src/brainways/utils/io_utils/readers/base.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/utils/io_utils/readers/czi_reader.py` & `brainways-0.1.7/src/brainways/utils/io_utils/readers/czi_reader.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/utils/io_utils/readers/qupath_reader.py` & `brainways-0.1.7/src/brainways/utils/io_utils/readers/qupath_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,35 +17,31 @@
 from fsspec.implementations.local import LocalFileSystem
 from resource_backed_dask_array import (
     ResourceBackedDaskArray,
     resource_backed_dask_array,
 )
 
 from brainways.utils.image import ImageSizeHW, resize_image
-from brainways.utils.qupath import (
-    add_brainways_qupath_dir_to_paquo_settings,
-    download_qupath,
-    is_qupath_downloaded,
-)
+from brainways.utils.qupath import download_qupath, is_qupath_downloaded
 
 
 class QupathReader(Reader):
+    _qupath_version = "0.4.3"
     _qupath_initialized = False
     ImageServerProvider = None
     BufferedImage = None
     redirect = None
 
     @staticmethod
     def _initialize_qupath():
         if QupathReader._qupath_initialized:
             return
 
         # TODO: move this code to some init function inside QupathReader
-        add_brainways_qupath_dir_to_paquo_settings()
-        if not is_qupath_downloaded():
+        if not is_qupath_downloaded(QupathReader._qupath_version):
             download_qupath()
         from paquo._logging import redirect
         from paquo.java import BufferedImage, ImageServerProvider, JClass, String
         from paquo.projects import DEFAULT_IMAGE_PROVIDER
 
         QupathReader.ImageServerProvider = ImageServerProvider
         QupathReader.BufferedImage = BufferedImage
@@ -229,15 +225,15 @@
                     0,
                     0,
                     self._current_server.getWidth(),
                     self._current_server.getHeight(),
                     0,
                     0,
                 )
-                buffered_image = self._current_server.readBufferedImage(request)
+                buffered_image = self._current_server.readRegion(request)
             image_data = buffered_image_to_numpy_array(buffered_image)  # TCZYX
             image_data = image_data[np.newaxis, :, np.newaxis, :, :]
         return xr.DataArray(
             image_data,
             dims=dimensions.DEFAULT_DIMENSION_ORDER_LIST,
         )
 
@@ -339,15 +335,15 @@
         # Our convention is that the final dask array is in the order TCZYX, so
         # block_id will be coming in as (T, C, Z, Y, X).
         t, c, z, y, x, *_ = block_id
 
         tile_request = self._tile_requests[(y, x)]
         with QupathReader.redirect(stderr=True, stdout=True):
             request = tile_request.getRegionRequest()
-            buffered_image = self.image_server.readBufferedImage(request)
+            buffered_image = self.image_server.readRegion(request)
             # buffered_image = self.image_server.readTile(tile_request)
         im = buffered_image_to_numpy_array(buffered_image, channel=c)
 
         return im[np.newaxis, np.newaxis, np.newaxis]
 
     def to_dask(self) -> ResourceBackedDaskArray:
         """Create dask array for the specified or current series.
```

### Comparing `brainways-0.1.6/src/brainways/utils/preprocess.py` & `brainways-0.1.7/src/brainways/utils/preprocess.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.6/src/brainways/utils/qupath.py` & `brainways-0.1.7/src/brainways/utils/qupath.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import platform
+import shutil
 from pathlib import Path
 
 from bg_atlasapi.utils import check_internet_connection
 from paquo import settings as paquo_settings
 from paquo.jpype_backend import find_qupath
 
 from brainways.utils.config import get_brainways_dir, get_interim_download_dir
@@ -18,38 +19,36 @@
 
 def add_brainways_qupath_dir_to_paquo_settings():
     qupath_brainways_dir = str(get_brainways_qupath_dir())
     if qupath_brainways_dir not in paquo_settings.qupath_search_dirs:
         paquo_settings.qupath_search_dirs = paquo_settings.qupath_search_dirs + [
             qupath_brainways_dir
         ]
-        # TODO: this is a workaround to enable BioFormats memoization.
-        # It stops working in Java 17, and will be fixed in QuPath 0.4.0.
-        # See https://github.com/ome/bioformats/issues/3659
-        paquo_settings.java_opts = paquo_settings.java_opts + [
-            "--add-opens=java.base/java.util.regex=ALL-UNNAMED",
-            "--illegal-access=permit",
-        ]
 
 
-def is_qupath_downloaded():
+def is_qupath_downloaded(version: str):
     """As we can't know the local version a priori, search candidate dirs
     using name and not version number. If none is found, return None.
     """
     add_brainways_qupath_dir_to_paquo_settings()
     try:
-        find_qupath(**{k.lower(): v for k, v in paquo_settings.to_dict().items()})
+        app_dir, runtime_dir, jvm_dir, jvm_options = find_qupath(
+            **{k.lower(): v for k, v in paquo_settings.to_dict().items()}
+        )
+        if f"QuPath-{version}" not in str(app_dir):
+            shutil.rmtree(get_brainways_qupath_dir())
+            return False
         return True
     except ValueError:
         return False
 
 
 def download_qupath(
     install_path: Path = get_brainways_qupath_dir(),
-    version: str = "0.3.2",
+    version: str = "0.4.3",
     system: str = platform.system(),
     download_path: str = get_interim_download_dir(),
     ssl_verify: bool = False,
 ):
     """
     Adapted from:
     https://github.com/bayer-science-for-a-better-life/paquo/blob/main/paquo/__main__.py#L316
```

### Comparing `brainways-0.1.6/src/brainways/utils/test_utils.py` & `brainways-0.1.7/src/brainways/utils/test_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,16 +18,16 @@
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

### Comparing `brainways-0.1.6/src/brainways.egg-info/PKG-INFO` & `brainways-0.1.7/src/brainways.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainways
-Version: 0.1.6
+Version: 0.1.7
 Summary: Brainways
 Home-page: https://github.com/bkntr/brainways
 Author: Ben Kantor
 Author-email: benkantor@mail.tau.ac.il
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/bkntr/brainways/issues
 Project-URL: Documentation, https://github.com/bkntr/brainways#README.md
```

### Comparing `brainways-0.1.6/src/brainways.egg-info/SOURCES.txt` & `brainways-0.1.7/src/brainways.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .editorconfig
 .gitignore
 .pre-commit-config.yaml
 .travis.yml
 AUTHORS.rst
+CHANGELOG.md
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
 Makefile
 README.rst
 pyproject.toml
@@ -78,14 +79,16 @@
 src/brainways/project/_tests/test_brainways_project.py
 src/brainways/project/_tests/test_brainways_subject.py
 src/brainways/project/_tests/test_utils.py
 src/brainways/project/_tests/test_projects/v0.1.1/project.bwp
 src/brainways/project/_tests/test_projects/v0.1.1/subject1/brainways.bin
 src/brainways/project/_tests/test_projects/v0.1.4/project.bwp
 src/brainways/project/_tests/test_projects/v0.1.4/subject1/brainways.bin
+src/brainways/project/_tests/test_projects/v0.1.5/project.bwp
+src/brainways/project/_tests/test_projects/v0.1.5/subject1/brainways.bin
 src/brainways/scripts/__init__.py
 src/brainways/scripts/batch_create_thumbnails.py
 src/brainways/scripts/cell_detection.py
 src/brainways/scripts/cli.py
 src/brainways/scripts/create_excel.py
 src/brainways/scripts/create_excel_colabelling.py
 src/brainways/scripts/create_reg_model_data.py
@@ -107,23 +110,25 @@
 src/brainways/transforms/_tests/test_image_to_atlas_transform.py
 src/brainways/transforms/_tests/test_tps_transform.py
 src/brainways/utils/__init__.py
 src/brainways/utils/_imports.py
 src/brainways/utils/cell_count_summary.py
 src/brainways/utils/cells.py
 src/brainways/utils/config.py
+src/brainways/utils/contrast.py
 src/brainways/utils/dataclasses.py
 src/brainways/utils/image.py
 src/brainways/utils/paths.py
 src/brainways/utils/preprocess.py
 src/brainways/utils/qupath.py
 src/brainways/utils/test_utils.py
 src/brainways/utils/_tests/__init__.py
 src/brainways/utils/_tests/test_cell_count_summary.py
 src/brainways/utils/_tests/test_cells.py
+src/brainways/utils/_tests/test_contrast.py
 src/brainways/utils/_tests/test_image.py
 src/brainways/utils/atlas/__init__.py
 src/brainways/utils/atlas/brainways_atlas.py
 src/brainways/utils/atlas/slice_atlas.py
 src/brainways/utils/atlas/_tests/__init__.py
 src/brainways/utils/atlas/_tests/test_brainways_atlas.py
 src/brainways/utils/atlas/_tests/test_slice_atlas.py
```

### Comparing `brainways-0.1.6/tox.ini` & `brainways-0.1.7/tox.ini`

 * *Files identical despite different names*


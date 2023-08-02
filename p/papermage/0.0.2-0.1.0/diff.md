# Comparing `tmp/papermage-0.0.2.tar.gz` & `tmp/papermage-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "papermage-0.0.2.tar", last modified: Fri Jan  6 18:30:41 2023, max compression
+gzip compressed data, was "papermage-0.1.0.tar", last modified: Wed Aug  2 04:58:56 2023, max compression
```

## Comparing `papermage-0.0.2.tar` & `papermage-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,69 @@
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-01-06 18:30:41.458526 papermage-0.0.2/
--rw-r--r--   0 lucas      (502) staff       (20)      527 2023-01-06 18:30:41.458379 papermage-0.0.2/PKG-INFO
--rw-r--r--   0 lucas      (502) staff       (20)       63 2023-01-06 18:27:11.000000 papermage-0.0.2/README.md
--rwxr-xr-x   0 lucas      (502) staff       (20)     1770 2023-01-06 18:27:01.000000 papermage-0.0.2/pyproject.toml
--rw-r--r--   0 lucas      (502) staff       (20)       38 2023-01-06 18:30:41.458572 papermage-0.0.2/setup.cfg
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-01-06 18:30:41.456837 papermage-0.0.2/src/
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-01-06 18:30:41.457477 papermage-0.0.2/src/papermage/
--rw-r--r--   0 lucas      (502) staff       (20)      238 2023-01-06 18:26:11.000000 papermage-0.0.2/src/papermage/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)        0 2023-01-06 18:22:09.000000 papermage-0.0.2/src/papermage/py.typed
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-01-06 18:30:41.458177 papermage-0.0.2/src/papermage.egg-info/
--rw-r--r--   0 lucas      (502) staff       (20)      527 2023-01-06 18:30:41.000000 papermage-0.0.2/src/papermage.egg-info/PKG-INFO
--rw-r--r--   0 lucas      (502) staff       (20)      257 2023-01-06 18:30:41.000000 papermage-0.0.2/src/papermage.egg-info/SOURCES.txt
--rw-r--r--   0 lucas      (502) staff       (20)        1 2023-01-06 18:30:41.000000 papermage-0.0.2/src/papermage.egg-info/dependency_links.txt
--rw-r--r--   0 lucas      (502) staff       (20)      170 2023-01-06 18:30:41.000000 papermage-0.0.2/src/papermage.egg-info/requires.txt
--rw-r--r--   0 lucas      (502) staff       (20)       10 2023-01-06 18:30:41.000000 papermage-0.0.2/src/papermage.egg-info/top_level.txt
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.027852 papermage-0.1.0/
+-rw-r--r--   0 lucas      (502) staff       (20)    11358 2023-08-02 01:44:14.000000 papermage-0.1.0/LICENSE
+-rw-r--r--   0 lucas      (502) staff       (20)     7545 2023-08-02 04:58:56.027721 papermage-0.1.0/PKG-INFO
+-rw-r--r--   0 lucas      (502) staff       (20)     6328 2023-08-02 01:44:14.000000 papermage-0.1.0/README.md
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.014024 papermage-0.1.0/examples/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-02 01:44:14.000000 papermage-0.1.0/examples/__init__.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.014128 papermage-0.1.0/papermage/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/__init__.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.015619 papermage-0.1.0/papermage/parsers/
+-rw-r--r--   0 lucas      (502) staff       (20)      102 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/parsers/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)      593 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/parsers/parser.py
+-rw-r--r--   0 lucas      (502) staff       (20)    18967 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/parsers/pdfplumber_parser.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.016143 papermage-0.1.0/papermage/predictors/
+-rw-r--r--   0 lucas      (502) staff       (20)      149 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/predictors/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1444 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/predictors/base_predictor.py
+-rw-r--r--   0 lucas      (502) staff       (20)    15068 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/predictors/entity_classification_predictor.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.016455 papermage-0.1.0/papermage/rasterizers/
+-rw-r--r--   0 lucas      (502) staff       (20)      105 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/rasterizers/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     2047 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/rasterizers/rasterizer.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.016703 papermage-0.1.0/papermage/trainers/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/trainers/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)    20509 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/trainers/entity_classification_predictor_trainer.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.018215 papermage-0.1.0/papermage/types/
+-rw-r--r--   0 lucas      (502) staff       (20)      930 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/types/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     2544 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/types/annotation.py
+-rw-r--r--   0 lucas      (502) staff       (20)     4542 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/types/box.py
+-rw-r--r--   0 lucas      (502) staff       (20)     4057 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/types/document.py
+-rw-r--r--   0 lucas      (502) staff       (20)     2880 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/types/entity.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3947 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/types/image.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3061 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/types/indexer.py
+-rw-r--r--   0 lucas      (502) staff       (20)    15532 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/types/metadata.py
+-rw-r--r--   0 lucas      (502) staff       (20)     5341 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/types/span.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.018399 papermage-0.1.0/papermage/visualizers/
+-rw-r--r--   0 lucas      (502) staff       (20)     1810 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/visualizers/visualizer.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.014776 papermage-0.1.0/papermage.egg-info/
+-rw-r--r--   0 lucas      (502) staff       (20)     7545 2023-08-02 04:58:56.000000 papermage-0.1.0/papermage.egg-info/PKG-INFO
+-rw-r--r--   0 lucas      (502) staff       (20)     1643 2023-08-02 04:58:56.000000 papermage-0.1.0/papermage.egg-info/SOURCES.txt
+-rw-r--r--   0 lucas      (502) staff       (20)        1 2023-08-02 04:58:56.000000 papermage-0.1.0/papermage.egg-info/dependency_links.txt
+-rw-r--r--   0 lucas      (502) staff       (20)      516 2023-08-02 04:58:56.000000 papermage-0.1.0/papermage.egg-info/requires.txt
+-rw-r--r--   0 lucas      (502) staff       (20)       43 2023-08-02 04:58:56.000000 papermage-0.1.0/papermage.egg-info/top_level.txt
+-rw-r--r--   0 lucas      (502) staff       (20)     3900 2023-08-02 04:58:01.000000 papermage-0.1.0/pyproject.toml
+-rw-r--r--   0 lucas      (502) staff       (20)       21 2023-08-02 01:44:14.000000 papermage-0.1.0/requirements.txt
+-rw-r--r--   0 lucas      (502) staff       (20)       38 2023-08-02 04:58:56.027896 papermage-0.1.0/setup.cfg
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.018561 papermage-0.1.0/tests/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/__init__.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.018784 papermage-0.1.0/tests/test_parsers/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_parsers/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     8969 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_parsers/test_pdf_plumber_parser.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.019196 papermage-0.1.0/tests/test_predictors/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_predictors/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3180 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_predictors/test_entity_classification_predictor.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.019593 papermage-0.1.0/tests/test_rasterizers/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_rasterizers/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1053 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_rasterizers/test_pdf2image_rasterizer.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.019820 papermage-0.1.0/tests/test_trainers/
+-rw-r--r--   0 lucas      (502) staff       (20)     7861 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_trainers/test_entity_classification_predictor_trainer.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.027033 papermage-0.1.0/tests/test_types/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_types/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1438 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_types/test_annotation.py
+-rw-r--r--   0 lucas      (502) staff       (20)     4926 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_types/test_box.py
+-rw-r--r--   0 lucas      (502) staff       (20)     2685 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_types/test_document.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3222 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_types/test_entity.py
+-rw-r--r--   0 lucas      (502) staff       (20)     2668 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_types/test_image.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1950 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_types/test_indexer.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1851 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_types/test_metadata.py
+-rw-r--r--   0 lucas      (502) staff       (20)     4133 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_types/test_span.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.027472 papermage-0.1.0/tests/test_visualizers/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_visualizers/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)      927 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_visualizers/test_visualizer.py
```


# Comparing `tmp/vdk-impala-0.4.944393829.tar.gz` & `tmp/vdk-impala-0.4.953562131.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-impala-0.4.944393829.tar", last modified: Tue Jul 25 09:01:02 2023, max compression
+gzip compressed data, was "vdk-impala-0.4.953562131.tar", last modified: Wed Aug  2 15:48:37 2023, max compression
```

## Comparing `vdk-impala-0.4.944393829.tar` & `vdk-impala-0.4.953562131.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.812218 vdk-impala-0.4.944393829/
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6530 2023-07-25 09:01:02.812218 vdk-impala-0.4.944393829/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5936 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 09:01:02.812218 vdk-impala-0.4.944393829/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1223 2023-07-25 09:00:50.000000 vdk-impala-0.4.944393829/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.800218 vdk-impala-0.4.944393829/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.800218 vdk-impala-0.4.944393829/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.800218 vdk-impala-0.4.944393829/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.804218 vdk-impala-0.4.944393829/src/vdk/plugin/impala/
--rw-rw-rw-   0 root         (0) root         (0)     6381 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/impala_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     2060 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/impala_connection.py
--rw-rw-rw-   0 root         (0) root         (0)     4518 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/impala_error_classifier.py
--rw-rw-rw-   0 root         (0) root         (0)    20197 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/impala_error_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     7846 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/impala_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     7448 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/impala_lineage_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     6722 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/impala_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.804218 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1029 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/data_quality_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.804218 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.804218 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.804218 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd1/
--rw-rw-rw-   0 root         (0) root         (0)      894 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd1/00-dimension-scd1-definition.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd1/01-test-if-view-matches-target.sql
--rw-rw-rw-   0 root         (0) root         (0)     2703 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd1/02-handle-quality-checks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.804218 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd1/02-requisite-sql-scripts/
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd1/02-requisite-sql-scripts/02-insert-into-target.sql
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd1/03-refresh.sql
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd1/04-compute-stats.sql
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.804218 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd2/
--rw-rw-rw-   0 root         (0) root         (0)      847 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd2/00-dimension-scd2-definition.py
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd2/01-test-if-view-matches-target.sql
--rw-rw-rw-   0 root         (0) root         (0)     1718 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd2/02-insert-into-target.sql
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd2/03-refresh.sql
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd2/04-compute-stats.sql
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.808218 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.808218 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/insert/
--rw-rw-rw-   0 root         (0) root         (0)      804 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/insert/00-fact-snapshot-definition.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/insert/01-test-if-view-matches-target.sql
--rw-rw-rw-   0 root         (0) root         (0)     3373 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/insert/02-handle-quality-checks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.808218 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/insert/02-requisite-sql-scripts/
--rw-rw-rw-   0 root         (0) root         (0)      186 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/insert/02-requisite-sql-scripts/02-create-consolidated-view.sql
--rw-rw-rw-   0 root         (0) root         (0)      309 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/insert/02-requisite-sql-scripts/02-insert-into-target.sql
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/insert/03-refresh.sql
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/insert/04-compute-stats.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.808218 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/snapshot/
--rw-rw-rw-   0 root         (0) root         (0)      829 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/snapshot/00-fact-snapshot-definition.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/snapshot/01-test-if-view-matches-target.sql
--rw-rw-rw-   0 root         (0) root         (0)     3190 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/snapshot/02-handle-quality-checks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.808218 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/snapshot/02-requisite-sql-scripts/
--rw-rw-rw-   0 root         (0) root         (0)      491 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/snapshot/02-requisite-sql-scripts/02-insert-into-target.sql
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/snapshot/02-requisite-sql-scripts/02-overwrite-target.sql
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/snapshot/03-refresh.sql
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/snapshot/04-compute-stats.sql
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/snapshot/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.812218 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/versioned/
--rw-rw-rw-   0 root         (0) root         (0)     3032 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/versioned/00-versioned-definition.py
--rw-rw-rw-   0 root         (0) root         (0)      294 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/versioned/01-test-if-view-matches-target.sql
--rw-rw-rw-   0 root         (0) root         (0)     4358 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/versioned/02-insert-into-target.sql
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/versioned/03-refresh.sql
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/versioned/04-compute-stats.sql
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/versioned/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2669 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/template_arguments_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     2298 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.812218 vdk-impala-0.4.944393829/src/vdk_impala.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6530 2023-07-25 09:01:02.000000 vdk-impala-0.4.944393829/src/vdk_impala.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3918 2023-07-25 09:01:02.000000 vdk-impala-0.4.944393829/src/vdk_impala.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 09:01:02.000000 vdk-impala-0.4.944393829/src/vdk_impala.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-07-25 09:01:02.000000 vdk-impala-0.4.944393829/src/vdk_impala.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-07-25 09:01:02.000000 vdk-impala-0.4.944393829/src/vdk_impala.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-07-25 09:01:02.000000 vdk-impala-0.4.944393829/src/vdk_impala.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.812218 vdk-impala-0.4.944393829/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.800218 vdk-impala-0.4.944393829/tests/functional/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.800218 vdk-impala-0.4.944393829/tests/functional/jobs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.812218 vdk-impala-0.4.944393829/tests/functional/jobs/sql-job/
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/tests/functional/jobs/sql-job/10_create_table.sql
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/tests/functional/jobs/sql-job/20_populate_table.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.812218 vdk-impala-0.4.944393829/tests/functional/jobs/sql-job-non-lineage/
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/tests/functional/jobs/sql-job-non-lineage/10_create_table.sql
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/tests/functional/jobs/sql-job-non-lineage/20_compute_table.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.812218 vdk-impala-0.4.944393829/tests/functional/jobs/sql-job-syntax-error/
--rw-rw-rw-   0 root         (0) root         (0)       13 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/tests/functional/jobs/sql-job-syntax-error/10_bad_query.sql
--rw-rw-rw-   0 root         (0) root         (0)     3952 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/tests/test_error_classifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.956859 vdk-impala-0.4.953562131/
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6530 2023-08-02 15:48:37.956859 vdk-impala-0.4.953562131/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5936 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-02 15:48:37.956859 vdk-impala-0.4.953562131/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1223 2023-08-02 15:48:24.000000 vdk-impala-0.4.953562131/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.940859 vdk-impala-0.4.953562131/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.940859 vdk-impala-0.4.953562131/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.940859 vdk-impala-0.4.953562131/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.940859 vdk-impala-0.4.953562131/src/vdk/plugin/impala/
+-rw-rw-rw-   0 root         (0) root         (0)     7458 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/impala_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     2060 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/impala_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     4518 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/impala_error_classifier.py
+-rw-rw-rw-   0 root         (0) root         (0)    20341 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/impala_error_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     7846 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/impala_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     7448 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/impala_lineage_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     6850 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/impala_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.944859 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1029 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/data_quality_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.944859 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.944859 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.944859 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd1/
+-rw-rw-rw-   0 root         (0) root         (0)      894 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd1/00-dimension-scd1-definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd1/01-test-if-view-matches-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2703 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd1/02-handle-quality-checks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.944859 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd1/02-requisite-sql-scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd1/02-requisite-sql-scripts/02-insert-into-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd1/03-refresh.sql
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd1/04-compute-stats.sql
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.944859 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd2/
+-rw-rw-rw-   0 root         (0) root         (0)      847 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd2/00-dimension-scd2-definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd2/01-test-if-view-matches-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1718 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd2/02-insert-into-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd2/03-refresh.sql
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd2/04-compute-stats.sql
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.944859 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.944859 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/insert/
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/insert/00-fact-snapshot-definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/insert/01-test-if-view-matches-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3373 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/insert/02-handle-quality-checks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.944859 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/insert/02-requisite-sql-scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/insert/02-requisite-sql-scripts/02-create-consolidated-view.sql
+-rw-rw-rw-   0 root         (0) root         (0)      309 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/insert/02-requisite-sql-scripts/02-insert-into-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/insert/03-refresh.sql
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/insert/04-compute-stats.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.948859 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/snapshot/
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/snapshot/00-fact-snapshot-definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/snapshot/01-test-if-view-matches-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3190 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/snapshot/02-handle-quality-checks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.952859 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/snapshot/02-requisite-sql-scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      491 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/snapshot/02-requisite-sql-scripts/02-insert-into-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/snapshot/02-requisite-sql-scripts/02-overwrite-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/snapshot/03-refresh.sql
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/snapshot/04-compute-stats.sql
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/snapshot/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.952859 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/versioned/
+-rw-rw-rw-   0 root         (0) root         (0)     3032 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/versioned/00-versioned-definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      294 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/versioned/01-test-if-view-matches-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)     4358 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/versioned/02-insert-into-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/versioned/03-refresh.sql
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/versioned/04-compute-stats.sql
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/versioned/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2669 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/template_arguments_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2298 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.952859 vdk-impala-0.4.953562131/src/vdk_impala.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6530 2023-08-02 15:48:37.000000 vdk-impala-0.4.953562131/src/vdk_impala.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3918 2023-08-02 15:48:37.000000 vdk-impala-0.4.953562131/src/vdk_impala.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 15:48:37.000000 vdk-impala-0.4.953562131/src/vdk_impala.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-08-02 15:48:37.000000 vdk-impala-0.4.953562131/src/vdk_impala.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-08-02 15:48:37.000000 vdk-impala-0.4.953562131/src/vdk_impala.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-08-02 15:48:37.000000 vdk-impala-0.4.953562131/src/vdk_impala.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.952859 vdk-impala-0.4.953562131/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.940859 vdk-impala-0.4.953562131/tests/functional/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.940859 vdk-impala-0.4.953562131/tests/functional/jobs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.956859 vdk-impala-0.4.953562131/tests/functional/jobs/sql-job/
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/tests/functional/jobs/sql-job/10_create_table.sql
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/tests/functional/jobs/sql-job/20_populate_table.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.956859 vdk-impala-0.4.953562131/tests/functional/jobs/sql-job-non-lineage/
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/tests/functional/jobs/sql-job-non-lineage/10_create_table.sql
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/tests/functional/jobs/sql-job-non-lineage/20_compute_table.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.956859 vdk-impala-0.4.953562131/tests/functional/jobs/sql-job-syntax-error/
+-rw-rw-rw-   0 root         (0) root         (0)       13 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/tests/functional/jobs/sql-job-syntax-error/10_bad_query.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3952 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/tests/test_error_classifier.py
```

### Comparing `vdk-impala-0.4.944393829/PKG-INFO` & `vdk-impala-0.4.953562131/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-impala
-Version: 0.4.944393829
+Version: 0.4.953562131
 Summary: Versatile Data Kit SDK plugin provides support for Impala database.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-impala-0.4.944393829/README.md` & `vdk-impala-0.4.953562131/README.md`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.944393829/setup.py` & `vdk-impala-0.4.953562131/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.4.944393829"
+__version__ = "0.4.953562131"
 
 setuptools.setup(
     name="vdk-impala",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK plugin provides support for Impala database.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-impala-0.4.944393829/src/vdk/plugin/impala/impala_configuration.py` & `vdk-impala-0.4.953562131/src/vdk/plugin/impala/impala_configuration.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 IMPALA_KRB_HOST = "IMPALA_KRB_HOST"
 IMPALA_USE_HTTP_TRANSPORT = "IMPALA_USE_HTTP_TRANSPORT"
 IMPALA_HTTP_PATH = "IMPALA_HTTP_PATH"
 IMPALA_AUTH_COOKIE_NAMES = "IMPALA_AUTH_COOKIE_NAMES"
 IMPALA_RETRIES = "IMPALA_RETRIES"
 IMPALA_SYNC_DDL = "IMPALA_SYNC_DDL"
 IMPALA_QUERY_POOL = "IMPALA_QUERY_POOL"
+IMPALA_RETRIES_ON_ERROR = "IMPALA_RETRIES_ON_ERROR"
+IMPALA_RETRIES_ON_ERROR_BACKOFF_SECONDS = "IMPALA_RETRIES_ON_ERROR_BACKOFF_SECONDS"
 
 
 class ImpalaPluginConfiguration:
     def __init__(self, config):
         self.__config = config
 
     def host(self):
@@ -72,14 +74,20 @@
 
     def sync_ddl(self):
         return self.__config.get_value(IMPALA_SYNC_DDL)
 
     def query_pool(self):
         return self.__config.get_value(IMPALA_QUERY_POOL)
 
+    def retries_on_error(self):
+        return self.__config.get_value(IMPALA_RETRIES_ON_ERROR)
+
+    def error_backoff_seconds(self):
+        return self.__config.get_value(IMPALA_RETRIES_ON_ERROR_BACKOFF_SECONDS)
+
 
 def add_definitions(config_builder: ConfigurationBuilder) -> None:
     """
     Here we define what configuration settings are needed for Impala with reasonable defaults
     """
     config_builder.add(
         key=IMPALA_HOST,
@@ -176,7 +184,23 @@
         ),
     )
     config_builder.add(
         key=IMPALA_QUERY_POOL,
         default_value=None,
         description="The name of the Impala pool to execute queries in.",
     )
+    config_builder.add(
+        key=IMPALA_RETRIES_ON_ERROR,
+        default_value=5,
+        description="The number of times a query will be retried if an exception is raised.",
+    )
+    config_builder.add(
+        key=IMPALA_RETRIES_ON_ERROR_BACKOFF_SECONDS,
+        default_value=30,
+        description=(
+            "Exponential backoff in seconds, in case retries of a failed query are needed. "
+            "Calculated as `(2 ^ retry-attempt) * backoff_seconds`, where "
+            "`retry-attempt` is the number of times the query has already been retried."
+            "For example, if the value of this configuration is 30 seconds, the time intervals will "
+            "be 30s, 60s, 2m, 4m, 8m"
+        ),
+    )
```

### Comparing `vdk-impala-0.4.944393829/src/vdk/plugin/impala/impala_connection.py` & `vdk-impala-0.4.953562131/src/vdk/plugin/impala/impala_connection.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.944393829/src/vdk/plugin/impala/impala_error_classifier.py` & `vdk-impala-0.4.953562131/src/vdk/plugin/impala/impala_error_classifier.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.944393829/src/vdk/plugin/impala/impala_error_handler.py` & `vdk-impala-0.4.953562131/src/vdk/plugin/impala/impala_error_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,26 +5,27 @@
 import time
 
 from vdk.internal.builtin_plugins.connection.recovery_cursor import RecoveryCursor
 from vdk.internal.core import errors
 
 
 class ImpalaErrorHandler:
-    def __init__(self, log=None, num_retries=5):
+    def __init__(self, log=None, num_retries=5, backoff_seconds=30):
         """
         This module offers error handling and error recovery for an Impala connection.
 
         :param log: a logger object, creates a new one if one isn't passed as a parameter
         :param num_retries: number of times a query will be re-tried
         """
         if not log:
             log = logging.getLogger(__name__)
         self._log = log
 
         self._num_retries = num_retries
+        self._backoff_seconds = backoff_seconds
 
     def handle_error(
         self, caught_exception: Exception, recovery_cursor: RecoveryCursor
     ) -> bool:
         """
         Handles an exception/error thrown by Impala.
         It examines the error and depending on which case it matches it will
@@ -155,15 +156,15 @@
                         "invalidate metadata `" + database + "`.`" + table + "`"
                     )
                 else:
                     recovery_cursor.execute(
                         "refresh `" + database + "`.`" + table + "`"
                     )
                     time.sleep(
-                        2 ** recovery_cursor.get_retries() * 30
+                        2 ** recovery_cursor.get_retries() * self._backoff_seconds
                     )  # exponential backoff 30s, 60s, 2m, 4m, 8m
                 recovery_cursor.retry_operation()
                 return True
             else:
                 self._log.info(
                     f"Cannot auto-recover as it cannot detect table name in error: {exception}"
                 )
@@ -191,15 +192,15 @@
                 "Query failed with network error. This is most likely a recoverable error. "
                 "We are retrying the query. "
                 f"Error was: {exception.__class__}: {str(exception)}"
             )
             # wait a little before retrying the query, giving time for the network to recover
             if recovery_cursor.get_retries() > 0:
                 time.sleep(
-                    2 ** recovery_cursor.get_retries() * 30
+                    2 ** recovery_cursor.get_retries() * self._backoff_seconds
                 )  # exponential backoff 60s, 2m, 4m, 8m
             # retry the query
             recovery_cursor.retry_operation()
             return True
         else:
             return False
 
@@ -224,15 +225,15 @@
             )
             or errors.exception_matches(
                 exception,
                 classname_with_package="impala.error.OperationalError",
                 exception_message_matcher_regex=".*ImpalaRuntimeException: Error making 'updateTableColumnStatistics'.*",
             )
         ):
-            sleep_seconds = 2 ** recovery_cursor.get_retries() * 30
+            sleep_seconds = 2 ** recovery_cursor.get_retries() * self._backoff_seconds
             self._log.info(
                 f"Query failed with: {exception.__class__} : {str(exception)}"
                 f"Will sleep for {sleep_seconds} seconds and try the query again."
             )
             # wait a little before retrying the query, giving time for the metadata to sync
             time.sleep(sleep_seconds)  # exponential backoff 30s, 60s, 2m, 4m, 8m
             # retry the query
@@ -281,15 +282,15 @@
             pattern_for_the_table_name = (
                 ".*AnalysisException: Could not resolve table reference: '(\\S+)'.*"
             )
 
         if (
             pattern_for_the_table_name
         ):  # then one of the exceptions matched and we can handle with invalidate
-            sleep_seconds = 2 ** recovery_cursor.get_retries() * 30
+            sleep_seconds = 2 ** recovery_cursor.get_retries() * self._backoff_seconds
             self._log.info(
                 f"Query failed with: {exception.__class__} : {str(exception)}"
                 f"Will sleep for {sleep_seconds} seconds, will issue invalidate metadata on the table and try the query again."
             )
 
             # Get the fully qualified table name from the exception message.
             matcher = re.compile(pattern=pattern_for_the_table_name)
```

### Comparing `vdk-impala-0.4.944393829/src/vdk/plugin/impala/impala_helper.py` & `vdk-impala-0.4.953562131/src/vdk/plugin/impala/impala_helper.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.944393829/src/vdk/plugin/impala/impala_lineage_plugin.py` & `vdk-impala-0.4.953562131/src/vdk/plugin/impala/impala_lineage_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.944393829/src/vdk/plugin/impala/impala_plugin.py` & `vdk-impala-0.4.953562131/src/vdk/plugin/impala/impala_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,18 +129,20 @@
                         what=f"Error occurred. Exception message: {exception}",
                         why="Review exception for details.",
                         consequences="Data Job execution will not continue.",
                         countermeasures="Review exception for details.",
                     )
                 ) from exception
 
-    @staticmethod
     @hookimpl
-    def db_connection_recover_operation(recovery_cursor: RecoveryCursor) -> None:
-        impala_error_handler = ImpalaErrorHandler()
+    def db_connection_recover_operation(self, recovery_cursor: RecoveryCursor) -> None:
+        impala_error_handler = ImpalaErrorHandler(
+            num_retries=self._impala_cfg.retries_on_error(),
+            backoff_seconds=self._impala_cfg.error_backoff_seconds(),
+        )
 
         if impala_error_handler.handle_error(
             recovery_cursor.get_exception(), recovery_cursor
         ):
             logging.getLogger(__name__).info(
                 "Error handled successfully! Query execution has succeeded."
             )
```

### Comparing `vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/data_quality_exception.py` & `vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/data_quality_exception.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd1/00-dimension-scd1-definition.py` & `vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd1/00-dimension-scd1-definition.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd1/02-handle-quality-checks.py` & `vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd1/02-handle-quality-checks.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd1/02-requisite-sql-scripts/02-insert-into-target.sql` & `vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd1/02-requisite-sql-scripts/02-insert-into-target.sql`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd2/00-dimension-scd2-definition.py` & `vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd2/00-dimension-scd2-definition.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd2/02-insert-into-target.sql` & `vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd2/02-insert-into-target.sql`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/insert/00-fact-snapshot-definition.py` & `vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/insert/00-fact-snapshot-definition.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/insert/02-handle-quality-checks.py` & `vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/insert/02-handle-quality-checks.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/snapshot/00-fact-snapshot-definition.py` & `vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/snapshot/00-fact-snapshot-definition.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/snapshot/02-handle-quality-checks.py` & `vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/snapshot/02-handle-quality-checks.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/versioned/00-versioned-definition.py` & `vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/versioned/00-versioned-definition.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/versioned/02-insert-into-target.sql` & `vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/versioned/02-insert-into-target.sql`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/template_arguments_validator.py` & `vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/template_arguments_validator.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/utility.py` & `vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/utility.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.944393829/src/vdk_impala.egg-info/PKG-INFO` & `vdk-impala-0.4.953562131/src/vdk_impala.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-impala
-Version: 0.4.944393829
+Version: 0.4.953562131
 Summary: Versatile Data Kit SDK plugin provides support for Impala database.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-impala-0.4.944393829/src/vdk_impala.egg-info/SOURCES.txt` & `vdk-impala-0.4.953562131/src/vdk_impala.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.944393829/tests/test_error_classifier.py` & `vdk-impala-0.4.953562131/tests/test_error_classifier.py`

 * *Files identical despite different names*


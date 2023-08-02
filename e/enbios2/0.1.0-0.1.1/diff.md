# Comparing `tmp/enbios2-0.1.0.tar.gz` & `tmp/enbios2-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enbios2-0.1.0.tar", last modified: Wed Aug  2 08:31:32 2023, max compression
+gzip compressed data, was "enbios2-0.1.1.tar", last modified: Wed Aug  2 08:33:00 2023, max compression
```

## Comparing `enbios2-0.1.0.tar` & `enbios2-0.1.1.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:31:32.113179 enbios2-0.1.0/
--rw-rw-r--   0 ram       (1001) ram       (1001)     1302 2023-07-11 09:20:15.000000 enbios2-0.1.0/LICENSE
--rw-rw-r--   0 ram       (1001) ram       (1001)     2007 2023-08-02 08:31:32.109179 enbios2-0.1.0/PKG-INFO
--rw-rw-r--   0 ram       (1001) ram       (1001)      943 2023-08-01 12:38:59.000000 enbios2-0.1.0/README.md
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:31:32.085179 enbios2-0.1.0/enbios2/
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/__init__.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:31:32.085179 enbios2-0.1.0/enbios2/analyse/
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/analyse/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)    14940 2023-08-01 12:40:02.000000 enbios2-0.1.0/enbios2/analyse/ana_experiment.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     6369 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/analyse/callipope_ana.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      425 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/analyse/const.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     4981 2023-08-01 12:38:59.000000 enbios2-0.1.0/enbios2/analyse/experiment_exporter.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      561 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/analyse/util.py
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-08-01 12:41:34.000000 enbios2-0.1.0/enbios2/analyse/vizprevexperiment.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:31:32.089179 enbios2-0.1.0/enbios2/base/
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/base/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      615 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/base/databases.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     2243 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/base/db_fields.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     6821 2023-08-02 08:20:29.000000 enbios2-0.1.0/enbios2/base/db_models.py
--rw-rw-r--   0 ram       (1001) ram       (1001)    22830 2023-08-02 08:20:29.000000 enbios2-0.1.0/enbios2/base/experiment.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     5141 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/base/experiment_io.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     7615 2023-08-02 08:20:29.000000 enbios2-0.1.0/enbios2/base/scenario.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     3257 2023-08-02 08:21:39.000000 enbios2-0.1.0/enbios2/base/stacked_MultiLCA.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      798 2023-07-13 10:46:47.000000 enbios2-0.1.0/enbios2/base/unit_registry.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:31:32.093179 enbios2-0.1.0/enbios2/bw2/
--rw-rw-r--   0 ram       (1001) ram       (1001)       49 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/bw2/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     2917 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/bw2/bw_autoimporter.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     1921 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/bw2/experiment_multiLCA.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     1185 2023-07-11 09:20:15.000000 enbios2-0.1.0/enbios2/bw2/extract_from_xml.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     4219 2023-08-01 12:39:42.000000 enbios2-0.1.0/enbios2/bw2/project_index.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     3497 2023-08-01 12:39:42.000000 enbios2-0.1.0/enbios2/bw2/util.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      508 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/const.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:31:32.093179 enbios2-0.1.0/enbios2/demos/
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/demos/__init__.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:31:32.093179 enbios2-0.1.0/enbios2/dev/
--rw-rw-r--   0 ram       (1001) ram       (1001)      529 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/dev/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      585 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/dev/create_experiment_schema.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      504 2023-08-01 12:39:42.000000 enbios2-0.1.0/enbios2/dev/evoinvent_dbs.py
--rw-rw-r--   0 ram       (1001) ram       (1001)       71 2023-08-01 12:38:59.000000 enbios2-0.1.0/enbios2/dev/pull_docs.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:31:32.093179 enbios2-0.1.0/enbios2/ecoinvent/
--rw-rw-r--   0 ram       (1001) ram       (1001)       58 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/ecoinvent/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     7890 2023-08-01 13:51:15.000000 enbios2-0.1.0/enbios2/ecoinvent/ecoinvent_index.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     8217 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/ecoinvent/ecoinvent_resolved_dataset_db.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     1663 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/ecoinvent/spatial.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:31:32.101179 enbios2-0.1.0/enbios2/experiment/
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/experiment/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     3541 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/experiment/activity_search.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     6925 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/experiment/ai_lcia.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:31:32.101179 enbios2-0.1.0/enbios2/experiment/bw2/
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/experiment/bw2/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      869 2023-08-01 12:39:42.000000 enbios2-0.1.0/enbios2/experiment/bw2/excel_importer.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      741 2023-08-01 12:39:42.000000 enbios2-0.1.0/enbios2/experiment/bw2/multiLCA.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      333 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/experiment/bw2/non_linear_methods.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     3678 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/experiment/bw2sigma.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     1094 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/experiment/bw_manipulation.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:31:32.101179 enbios2-0.1.0/enbios2/experiment/bw_vector_db/
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-08-01 12:39:42.000000 enbios2-0.1.0/enbios2/experiment/bw_vector_db/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     1766 2023-08-01 12:39:42.000000 enbios2-0.1.0/enbios2/experiment/bw_vector_db/cluster.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     5148 2023-08-01 12:39:42.000000 enbios2-0.1.0/enbios2/experiment/bw_vector_db/create_vectors.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     1893 2023-08-01 12:39:42.000000 enbios2-0.1.0/enbios2/experiment/bw_vector_db/plotting.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     2346 2023-08-01 12:39:42.000000 enbios2-0.1.0/enbios2/experiment/bw_vector_db/psql_vectorDB.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     3462 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/experiment/characterizations.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      232 2023-07-11 21:09:47.000000 enbios2-0.1.0/enbios2/experiment/class_static_me.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     1954 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/experiment/comp_numba.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     1764 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/experiment/create_networkx.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     7578 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/experiment/dot2bw.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     8238 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/experiment/fast_tree.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:31:32.105179 enbios2-0.1.0/enbios2/experiment/gnn/
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-08-01 12:39:42.000000 enbios2-0.1.0/enbios2/experiment/gnn/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     2409 2023-07-14 23:13:54.000000 enbios2-0.1.0/enbios2/experiment/gnn/base.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:31:32.105179 enbios2-0.1.0/enbios2/experiment/my_numba/
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/experiment/my_numba/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      811 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/experiment/my_numba/simple.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:31:32.105179 enbios2-0.1.0/enbios2/experiment/nlp/
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-08-01 12:39:42.000000 enbios2-0.1.0/enbios2/experiment/nlp/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      510 2023-08-01 12:39:42.000000 enbios2-0.1.0/enbios2/experiment/nlp/models.py
--rw-rw-r--   0 ram       (1001) ram       (1001)    12309 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/experiment/promt_toolkit_checker.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      593 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/experiment/schema_builder.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     3342 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/experiment/spold2json.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      977 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/experiment/starcoder.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     4012 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/experiment/sum_hierarchy.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     4241 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/experiment/tree_transformer.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      346 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/experiment/util.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:31:32.105179 enbios2-0.1.0/enbios2/generic/
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/generic/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     3116 2023-08-01 12:39:42.000000 enbios2-0.1.0/enbios2/generic/enbios2_logging.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     3231 2023-08-01 12:39:42.000000 enbios2-0.1.0/enbios2/generic/files.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:31:32.105179 enbios2-0.1.0/enbios2/generic/tree/
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/generic/tree/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)    28844 2023-08-01 12:39:42.000000 enbios2-0.1.0/enbios2/generic/tree/basic_tree.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     2846 2023-08-01 12:39:42.000000 enbios2-0.1.0/enbios2/generic/util.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:31:32.109179 enbios2-0.1.0/enbios2/models/
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/models/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     1256 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/models/bw_project_models.py
--rw-rw-r--   0 ram       (1001) ram       (1001)    11907 2023-08-01 12:42:09.000000 enbios2-0.1.0/enbios2/models/experiment_models.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      378 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/models/prepare.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:31:32.109179 enbios2-0.1.0/enbios2/plot/
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/plot/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     1440 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/plot/sanky1.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:31:32.109179 enbios2-0.1.0/enbios2/plotting/
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-08-01 08:59:04.000000 enbios2-0.1.0/enbios2/plotting/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     1599 2023-08-01 08:59:04.000000 enbios2-0.1.0/enbios2/plotting/plot_experiment.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      273 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/settings.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:31:32.109179 enbios2-0.1.0/enbios2/test/
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/test/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      338 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/test/conftest.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      593 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/test/master_index.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      549 2023-08-01 12:39:42.000000 enbios2-0.1.0/enbios2/test/regunit.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     1444 2023-07-11 08:36:40.000000 enbios2-0.1.0/enbios2/test/test_dot2bw.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      999 2023-08-01 12:39:42.000000 enbios2-0.1.0/enbios2/test/units_conv.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:31:32.085179 enbios2-0.1.0/enbios2.egg-info/
--rw-rw-r--   0 ram       (1001) ram       (1001)     2007 2023-08-02 08:31:32.000000 enbios2-0.1.0/enbios2.egg-info/PKG-INFO
--rw-rw-r--   0 ram       (1001) ram       (1001)     2973 2023-08-02 08:31:32.000000 enbios2-0.1.0/enbios2.egg-info/SOURCES.txt
--rw-rw-r--   0 ram       (1001) ram       (1001)        1 2023-08-02 08:31:32.000000 enbios2-0.1.0/enbios2.egg-info/dependency_links.txt
--rw-rw-r--   0 ram       (1001) ram       (1001)     1034 2023-08-02 08:31:32.000000 enbios2-0.1.0/enbios2.egg-info/requires.txt
--rw-rw-r--   0 ram       (1001) ram       (1001)        8 2023-08-02 08:31:32.000000 enbios2-0.1.0/enbios2.egg-info/top_level.txt
--rw-rw-r--   0 ram       (1001) ram       (1001)     2362 2023-08-02 08:31:23.000000 enbios2-0.1.0/pyproject.toml
--rw-rw-r--   0 ram       (1001) ram       (1001)       38 2023-08-02 08:31:32.113179 enbios2-0.1.0/setup.cfg
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:33:00.205650 enbios2-0.1.1/
+-rw-rw-r--   0 ram       (1001) ram       (1001)     1302 2023-07-11 09:20:15.000000 enbios2-0.1.1/LICENSE
+-rw-rw-r--   0 ram       (1001) ram       (1001)     2007 2023-08-02 08:33:00.205650 enbios2-0.1.1/PKG-INFO
+-rw-rw-r--   0 ram       (1001) ram       (1001)      943 2023-08-01 12:38:59.000000 enbios2-0.1.1/README.md
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:33:00.189650 enbios2-0.1.1/enbios2/
+-rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/__init__.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:33:00.189650 enbios2-0.1.1/enbios2/analyse/
+-rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/analyse/__init__.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)    14940 2023-08-01 12:40:02.000000 enbios2-0.1.1/enbios2/analyse/ana_experiment.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     6369 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/analyse/callipope_ana.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      425 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/analyse/const.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     4981 2023-08-01 12:38:59.000000 enbios2-0.1.1/enbios2/analyse/experiment_exporter.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      561 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/analyse/util.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-08-01 12:41:34.000000 enbios2-0.1.1/enbios2/analyse/vizprevexperiment.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:33:00.193650 enbios2-0.1.1/enbios2/base/
+-rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/base/__init__.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      615 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/base/databases.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     2243 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/base/db_fields.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     6821 2023-08-02 08:20:29.000000 enbios2-0.1.1/enbios2/base/db_models.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)    22830 2023-08-02 08:20:29.000000 enbios2-0.1.1/enbios2/base/experiment.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     5141 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/base/experiment_io.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     7615 2023-08-02 08:20:29.000000 enbios2-0.1.1/enbios2/base/scenario.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     3257 2023-08-02 08:21:39.000000 enbios2-0.1.1/enbios2/base/stacked_MultiLCA.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      798 2023-07-13 10:46:47.000000 enbios2-0.1.1/enbios2/base/unit_registry.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:33:00.193650 enbios2-0.1.1/enbios2/bw2/
+-rw-rw-r--   0 ram       (1001) ram       (1001)       49 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/bw2/__init__.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     2917 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/bw2/bw_autoimporter.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     1921 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/bw2/experiment_multiLCA.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     1185 2023-07-11 09:20:15.000000 enbios2-0.1.1/enbios2/bw2/extract_from_xml.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     4219 2023-08-01 12:39:42.000000 enbios2-0.1.1/enbios2/bw2/project_index.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     3497 2023-08-01 12:39:42.000000 enbios2-0.1.1/enbios2/bw2/util.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      508 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/const.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:33:00.193650 enbios2-0.1.1/enbios2/demos/
+-rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/demos/__init__.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:33:00.193650 enbios2-0.1.1/enbios2/dev/
+-rw-rw-r--   0 ram       (1001) ram       (1001)      529 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/dev/__init__.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      585 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/dev/create_experiment_schema.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      504 2023-08-01 12:39:42.000000 enbios2-0.1.1/enbios2/dev/evoinvent_dbs.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)       71 2023-08-01 12:38:59.000000 enbios2-0.1.1/enbios2/dev/pull_docs.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:33:00.193650 enbios2-0.1.1/enbios2/ecoinvent/
+-rw-rw-r--   0 ram       (1001) ram       (1001)       58 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/ecoinvent/__init__.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     7890 2023-08-01 13:51:15.000000 enbios2-0.1.1/enbios2/ecoinvent/ecoinvent_index.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     8217 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/ecoinvent/ecoinvent_resolved_dataset_db.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     1663 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/ecoinvent/spatial.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:33:00.197650 enbios2-0.1.1/enbios2/experiment/
+-rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/experiment/__init__.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     3541 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/experiment/activity_search.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     6925 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/experiment/ai_lcia.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:33:00.197650 enbios2-0.1.1/enbios2/experiment/bw2/
+-rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/experiment/bw2/__init__.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      869 2023-08-01 12:39:42.000000 enbios2-0.1.1/enbios2/experiment/bw2/excel_importer.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      741 2023-08-01 12:39:42.000000 enbios2-0.1.1/enbios2/experiment/bw2/multiLCA.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      333 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/experiment/bw2/non_linear_methods.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     3678 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/experiment/bw2sigma.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     1094 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/experiment/bw_manipulation.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:33:00.201650 enbios2-0.1.1/enbios2/experiment/bw_vector_db/
+-rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-08-01 12:39:42.000000 enbios2-0.1.1/enbios2/experiment/bw_vector_db/__init__.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     1766 2023-08-01 12:39:42.000000 enbios2-0.1.1/enbios2/experiment/bw_vector_db/cluster.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     5148 2023-08-01 12:39:42.000000 enbios2-0.1.1/enbios2/experiment/bw_vector_db/create_vectors.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     1893 2023-08-01 12:39:42.000000 enbios2-0.1.1/enbios2/experiment/bw_vector_db/plotting.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     2346 2023-08-01 12:39:42.000000 enbios2-0.1.1/enbios2/experiment/bw_vector_db/psql_vectorDB.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     3462 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/experiment/characterizations.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      232 2023-07-11 21:09:47.000000 enbios2-0.1.1/enbios2/experiment/class_static_me.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     1954 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/experiment/comp_numba.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     1764 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/experiment/create_networkx.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     7578 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/experiment/dot2bw.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     8238 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/experiment/fast_tree.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:33:00.201650 enbios2-0.1.1/enbios2/experiment/gnn/
+-rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-08-01 12:39:42.000000 enbios2-0.1.1/enbios2/experiment/gnn/__init__.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     2409 2023-07-14 23:13:54.000000 enbios2-0.1.1/enbios2/experiment/gnn/base.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:33:00.201650 enbios2-0.1.1/enbios2/experiment/my_numba/
+-rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/experiment/my_numba/__init__.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      811 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/experiment/my_numba/simple.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:33:00.201650 enbios2-0.1.1/enbios2/experiment/nlp/
+-rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-08-01 12:39:42.000000 enbios2-0.1.1/enbios2/experiment/nlp/__init__.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      510 2023-08-01 12:39:42.000000 enbios2-0.1.1/enbios2/experiment/nlp/models.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)    12309 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/experiment/promt_toolkit_checker.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      593 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/experiment/schema_builder.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     3342 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/experiment/spold2json.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      977 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/experiment/starcoder.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     4012 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/experiment/sum_hierarchy.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     4241 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/experiment/tree_transformer.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      346 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/experiment/util.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:33:00.201650 enbios2-0.1.1/enbios2/generic/
+-rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/generic/__init__.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     3116 2023-08-01 12:39:42.000000 enbios2-0.1.1/enbios2/generic/enbios2_logging.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     3231 2023-08-01 12:39:42.000000 enbios2-0.1.1/enbios2/generic/files.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:33:00.201650 enbios2-0.1.1/enbios2/generic/tree/
+-rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/generic/tree/__init__.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)    28844 2023-08-01 12:39:42.000000 enbios2-0.1.1/enbios2/generic/tree/basic_tree.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     2846 2023-08-01 12:39:42.000000 enbios2-0.1.1/enbios2/generic/util.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:33:00.205650 enbios2-0.1.1/enbios2/models/
+-rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/models/__init__.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     1256 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/models/bw_project_models.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)    11907 2023-08-01 12:42:09.000000 enbios2-0.1.1/enbios2/models/experiment_models.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      378 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/models/prepare.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:33:00.205650 enbios2-0.1.1/enbios2/plot/
+-rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/plot/__init__.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     1440 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/plot/sanky1.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:33:00.205650 enbios2-0.1.1/enbios2/plotting/
+-rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-08-01 08:59:04.000000 enbios2-0.1.1/enbios2/plotting/__init__.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     1599 2023-08-01 08:59:04.000000 enbios2-0.1.1/enbios2/plotting/plot_experiment.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      273 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/settings.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:33:00.205650 enbios2-0.1.1/enbios2/test/
+-rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/test/__init__.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      338 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/test/conftest.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      593 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/test/master_index.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      549 2023-08-01 12:39:42.000000 enbios2-0.1.1/enbios2/test/regunit.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     1444 2023-07-11 08:36:40.000000 enbios2-0.1.1/enbios2/test/test_dot2bw.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      999 2023-08-01 12:39:42.000000 enbios2-0.1.1/enbios2/test/units_conv.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-08-02 08:33:00.189650 enbios2-0.1.1/enbios2.egg-info/
+-rw-rw-r--   0 ram       (1001) ram       (1001)     2007 2023-08-02 08:33:00.000000 enbios2-0.1.1/enbios2.egg-info/PKG-INFO
+-rw-rw-r--   0 ram       (1001) ram       (1001)     2973 2023-08-02 08:33:00.000000 enbios2-0.1.1/enbios2.egg-info/SOURCES.txt
+-rw-rw-r--   0 ram       (1001) ram       (1001)        1 2023-08-02 08:33:00.000000 enbios2-0.1.1/enbios2.egg-info/dependency_links.txt
+-rw-rw-r--   0 ram       (1001) ram       (1001)     1034 2023-08-02 08:33:00.000000 enbios2-0.1.1/enbios2.egg-info/requires.txt
+-rw-rw-r--   0 ram       (1001) ram       (1001)        8 2023-08-02 08:33:00.000000 enbios2-0.1.1/enbios2.egg-info/top_level.txt
+-rw-rw-r--   0 ram       (1001) ram       (1001)     2362 2023-08-02 08:32:52.000000 enbios2-0.1.1/pyproject.toml
+-rw-rw-r--   0 ram       (1001) ram       (1001)       38 2023-08-02 08:33:00.205650 enbios2-0.1.1/setup.cfg
```

### Comparing `enbios2-0.1.0/LICENSE` & `enbios2-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/PKG-INFO` & `enbios2-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enbios2
-Version: 0.1.0
+Version: 0.1.1
 Summary: Enbios 2
 Author: Ramin Soleymani
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `enbios2-0.1.0/README.md` & `enbios2-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/analyse/ana_experiment.py` & `enbios2-0.1.1/enbios2/analyse/ana_experiment.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/analyse/callipope_ana.py` & `enbios2-0.1.1/enbios2/analyse/callipope_ana.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/analyse/experiment_exporter.py` & `enbios2-0.1.1/enbios2/analyse/experiment_exporter.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/analyse/util.py` & `enbios2-0.1.1/enbios2/analyse/util.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/base/databases.py` & `enbios2-0.1.1/enbios2/base/databases.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/base/db_fields.py` & `enbios2-0.1.1/enbios2/base/db_fields.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/base/db_models.py` & `enbios2-0.1.1/enbios2/base/db_models.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/base/experiment.py` & `enbios2-0.1.1/enbios2/base/experiment.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/base/experiment_io.py` & `enbios2-0.1.1/enbios2/base/experiment_io.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/base/scenario.py` & `enbios2-0.1.1/enbios2/base/scenario.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/base/stacked_MultiLCA.py` & `enbios2-0.1.1/enbios2/base/stacked_MultiLCA.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/base/unit_registry.py` & `enbios2-0.1.1/enbios2/base/unit_registry.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/bw2/bw_autoimporter.py` & `enbios2-0.1.1/enbios2/bw2/bw_autoimporter.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/bw2/experiment_multiLCA.py` & `enbios2-0.1.1/enbios2/bw2/experiment_multiLCA.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/bw2/extract_from_xml.py` & `enbios2-0.1.1/enbios2/bw2/extract_from_xml.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/bw2/project_index.py` & `enbios2-0.1.1/enbios2/bw2/project_index.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/bw2/util.py` & `enbios2-0.1.1/enbios2/bw2/util.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/dev/__init__.py` & `enbios2-0.1.1/enbios2/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/dev/create_experiment_schema.py` & `enbios2-0.1.1/enbios2/dev/create_experiment_schema.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/ecoinvent/ecoinvent_index.py` & `enbios2-0.1.1/enbios2/ecoinvent/ecoinvent_index.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/ecoinvent/ecoinvent_resolved_dataset_db.py` & `enbios2-0.1.1/enbios2/ecoinvent/ecoinvent_resolved_dataset_db.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/ecoinvent/spatial.py` & `enbios2-0.1.1/enbios2/ecoinvent/spatial.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/experiment/activity_search.py` & `enbios2-0.1.1/enbios2/experiment/activity_search.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/experiment/ai_lcia.py` & `enbios2-0.1.1/enbios2/experiment/ai_lcia.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/experiment/bw2/excel_importer.py` & `enbios2-0.1.1/enbios2/experiment/bw2/excel_importer.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/experiment/bw2/multiLCA.py` & `enbios2-0.1.1/enbios2/experiment/bw2/multiLCA.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/experiment/bw2sigma.py` & `enbios2-0.1.1/enbios2/experiment/bw2sigma.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/experiment/bw_manipulation.py` & `enbios2-0.1.1/enbios2/experiment/bw_manipulation.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/experiment/bw_vector_db/cluster.py` & `enbios2-0.1.1/enbios2/experiment/bw_vector_db/cluster.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/experiment/bw_vector_db/create_vectors.py` & `enbios2-0.1.1/enbios2/experiment/bw_vector_db/create_vectors.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/experiment/bw_vector_db/plotting.py` & `enbios2-0.1.1/enbios2/experiment/bw_vector_db/plotting.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/experiment/bw_vector_db/psql_vectorDB.py` & `enbios2-0.1.1/enbios2/experiment/bw_vector_db/psql_vectorDB.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/experiment/characterizations.py` & `enbios2-0.1.1/enbios2/experiment/characterizations.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/experiment/comp_numba.py` & `enbios2-0.1.1/enbios2/experiment/comp_numba.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/experiment/create_networkx.py` & `enbios2-0.1.1/enbios2/experiment/create_networkx.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/experiment/dot2bw.py` & `enbios2-0.1.1/enbios2/experiment/dot2bw.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/experiment/fast_tree.py` & `enbios2-0.1.1/enbios2/experiment/fast_tree.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/experiment/gnn/base.py` & `enbios2-0.1.1/enbios2/experiment/gnn/base.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/experiment/my_numba/simple.py` & `enbios2-0.1.1/enbios2/experiment/my_numba/simple.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/experiment/promt_toolkit_checker.py` & `enbios2-0.1.1/enbios2/experiment/promt_toolkit_checker.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/experiment/schema_builder.py` & `enbios2-0.1.1/enbios2/experiment/schema_builder.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/experiment/spold2json.py` & `enbios2-0.1.1/enbios2/experiment/spold2json.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/experiment/starcoder.py` & `enbios2-0.1.1/enbios2/experiment/starcoder.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/experiment/sum_hierarchy.py` & `enbios2-0.1.1/enbios2/experiment/sum_hierarchy.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/experiment/tree_transformer.py` & `enbios2-0.1.1/enbios2/experiment/tree_transformer.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/generic/enbios2_logging.py` & `enbios2-0.1.1/enbios2/generic/enbios2_logging.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/generic/files.py` & `enbios2-0.1.1/enbios2/generic/files.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/generic/tree/basic_tree.py` & `enbios2-0.1.1/enbios2/generic/tree/basic_tree.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/generic/util.py` & `enbios2-0.1.1/enbios2/generic/util.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/models/bw_project_models.py` & `enbios2-0.1.1/enbios2/models/bw_project_models.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/models/experiment_models.py` & `enbios2-0.1.1/enbios2/models/experiment_models.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/plot/sanky1.py` & `enbios2-0.1.1/enbios2/plot/sanky1.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/plotting/plot_experiment.py` & `enbios2-0.1.1/enbios2/plotting/plot_experiment.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/test/master_index.py` & `enbios2-0.1.1/enbios2/test/master_index.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/test/regunit.py` & `enbios2-0.1.1/enbios2/test/regunit.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/test/test_dot2bw.py` & `enbios2-0.1.1/enbios2/test/test_dot2bw.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2/test/units_conv.py` & `enbios2-0.1.1/enbios2/test/units_conv.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2.egg-info/PKG-INFO` & `enbios2-0.1.1/enbios2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enbios2
-Version: 0.1.0
+Version: 0.1.1
 Summary: Enbios 2
 Author: Ramin Soleymani
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `enbios2-0.1.0/enbios2.egg-info/SOURCES.txt` & `enbios2-0.1.1/enbios2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/enbios2.egg-info/requires.txt` & `enbios2-0.1.1/enbios2.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `enbios2-0.1.0/pyproject.toml` & `enbios2-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "enbios2"
-version = "0.1.0"
+version = "0.1.1"
 description = "Enbios 2"
 authors = [
     { name = "Ramin Soleymani" },
 ]
 
 classifiers = [
     "Development Status :: 4 - Beta",
```


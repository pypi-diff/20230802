# Comparing `tmp/amulog-0.3.8.tar.gz` & `tmp/amulog-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amulog-0.3.8.tar", last modified: Mon Dec 20 07:55:57 2021, max compression
+gzip compressed data, was "amulog-0.3.9.tar", last modified: Fri Mar 11 08:21:10 2022, max compression
```

## Comparing `amulog-0.3.8.tar` & `amulog-0.3.9.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 sat        (501) staff       (20)        0 2021-12-20 07:55:57.286131 amulog-0.3.8/
--rw-r--r--   0 sat        (501) staff       (20)     1463 2020-11-15 13:23:08.000000 amulog-0.3.8/LICENSE
--rw-r--r--   0 sat        (501) staff       (20)       64 2020-11-15 13:23:08.000000 amulog-0.3.8/MANIFEST.in
--rw-r--r--   0 sat        (501) staff       (20)     6815 2021-12-20 07:55:57.285708 amulog-0.3.8/PKG-INFO
--rw-r--r--   0 sat        (501) staff       (20)     4506 2021-12-20 07:46:26.000000 amulog-0.3.8/README.rst
-drwxr-xr-x   0 sat        (501) staff       (20)        0 2021-12-20 07:55:57.259092 amulog-0.3.8/amulog/
--rwxr-xr-x   0 sat        (501) staff       (20)      209 2021-12-20 07:44:30.000000 amulog-0.3.8/amulog/__init__.py
--rwxr-xr-x   0 sat        (501) staff       (20)    22923 2021-11-19 06:05:00.000000 amulog-0.3.8/amulog/__main__.py
-drwxr-xr-x   0 sat        (501) staff       (20)        0 2021-12-20 07:55:57.262441 amulog-0.3.8/amulog/alg/
--rw-r--r--   0 sat        (501) staff       (20)       28 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/alg/__init__.py
-drwxr-xr-x   0 sat        (501) staff       (20)        0 2021-12-20 07:55:57.266419 amulog-0.3.8/amulog/alg/crf/
--rw-r--r--   0 sat        (501) staff       (20)       87 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/alg/crf/__init__.py
--rw-r--r--   0 sat        (501) staff       (20)     6649 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/alg/crf/__main__.py
--rw-r--r--   0 sat        (501) staff       (20)     4439 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/alg/crf/_convert.py
--rw-r--r--   0 sat        (501) staff       (20)     1614 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/alg/crf/_items.py
--rw-r--r--   0 sat        (501) staff       (20)    23187 2021-07-24 17:40:16.000000 amulog-0.3.8/amulog/alg/crf/lt_crf.py
--rw-r--r--   0 sat        (501) staff       (20)     3604 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/alg/crf/train.py
-drwxr-xr-x   0 sat        (501) staff       (20)        0 2021-12-20 07:55:57.267844 amulog-0.3.8/amulog/alg/dlog/
--rw-r--r--   0 sat        (501) staff       (20)       66 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/alg/dlog/__init__.py
--rw-r--r--   0 sat        (501) staff       (20)     4699 2021-07-26 05:12:42.000000 amulog-0.3.8/amulog/alg/dlog/dlog.py
-drwxr-xr-x   0 sat        (501) staff       (20)        0 2021-12-20 07:55:57.268964 amulog-0.3.8/amulog/alg/drain/
--rw-r--r--   0 sat        (501) staff       (20)      151 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/alg/drain/__init__.py
--rw-r--r--   0 sat        (501) staff       (20)     4250 2021-07-26 05:13:05.000000 amulog-0.3.8/amulog/alg/drain/drain.py
-drwxr-xr-x   0 sat        (501) staff       (20)        0 2021-12-20 07:55:57.270117 amulog-0.3.8/amulog/alg/fttree/
--rw-r--r--   0 sat        (501) staff       (20)      156 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/alg/fttree/__init__.py
--rw-r--r--   0 sat        (501) staff       (20)     4492 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/alg/fttree/fttree.py
-drwxr-xr-x   0 sat        (501) staff       (20)        0 2021-12-20 07:55:57.270801 amulog-0.3.8/amulog/alg/lenma/
--rw-r--r--   0 sat        (501) staff       (20)      151 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/alg/lenma/__init__.py
--rw-r--r--   0 sat        (501) staff       (20)     4114 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/alg/lenma/lenma.py
--rw-r--r--   0 sat        (501) staff       (20)      500 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/alg/meta.py
-drwxr-xr-x   0 sat        (501) staff       (20)        0 2021-12-20 07:55:57.271746 amulog-0.3.8/amulog/alg/shiso/
--rw-r--r--   0 sat        (501) staff       (20)       91 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/alg/shiso/__init__.py
--rwxr-xr-x   0 sat        (501) staff       (20)     8312 2021-07-13 07:42:08.000000 amulog-0.3.8/amulog/alg/shiso/shiso.py
--rw-r--r--   0 sat        (501) staff       (20)     6634 2021-07-16 02:34:24.000000 amulog-0.3.8/amulog/anonymize.py
--rw-r--r--   0 sat        (501) staff       (20)     1544 2021-07-05 06:11:28.000000 amulog-0.3.8/amulog/cli.py
--rwxr-xr-x   0 sat        (501) staff       (20)    12161 2021-09-01 08:44:27.000000 amulog-0.3.8/amulog/common.py
--rwxr-xr-x   0 sat        (501) staff       (20)    17885 2021-09-01 10:30:33.000000 amulog-0.3.8/amulog/config.py
-drwxr-xr-x   0 sat        (501) staff       (20)        0 2021-12-20 07:55:57.275393 amulog-0.3.8/amulog/data/
--rw-r--r--   0 sat        (501) staff       (20)     8011 2021-11-05 06:50:56.000000 amulog-0.3.8/amulog/data/config.conf.default
--rw-r--r--   0 sat        (501) staff       (20)      144 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/data/crf_template.default
--rw-r--r--   0 sat        (501) staff       (20)       83 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/data/crf_template.sample
--rw-r--r--   0 sat        (501) staff       (20)       73 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/data/drain_regex.conf
--rw-r--r--   0 sat        (501) staff       (20)      308 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/data/host_alias.txt.sample
--rw-r--r--   0 sat        (501) staff       (20)      926 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/data/lt_label.conf.sample
--rw-r--r--   0 sat        (501) staff       (20)     1729 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/data/testlog.conf
--rwxr-xr-x   0 sat        (501) staff       (20)     7486 2021-11-17 06:57:47.000000 amulog-0.3.8/amulog/db_common.py
--rw-r--r--   0 sat        (501) staff       (20)     3476 2021-08-15 15:29:17.000000 amulog-0.3.8/amulog/db_mysql.py
--rw-r--r--   0 sat        (501) staff       (20)     2918 2021-08-15 15:29:17.000000 amulog-0.3.8/amulog/db_sqlite.py
-drwxr-xr-x   0 sat        (501) staff       (20)        0 2021-12-20 07:55:57.277264 amulog-0.3.8/amulog/edit/
--rw-r--r--   0 sat        (501) staff       (20)        0 2021-07-05 06:11:28.000000 amulog-0.3.8/amulog/edit/__init__.py
--rw-r--r--   0 sat        (501) staff       (20)    12028 2021-07-17 03:52:30.000000 amulog-0.3.8/amulog/edit/__main__.py
--rwxr-xr-x   0 sat        (501) staff       (20)     8593 2021-07-17 04:05:51.000000 amulog-0.3.8/amulog/edit/lt_tool.py
--rw-r--r--   0 sat        (501) staff       (20)     2671 2021-07-05 06:11:28.000000 amulog-0.3.8/amulog/edit/search.py
-drwxr-xr-x   0 sat        (501) staff       (20)        0 2021-12-20 07:55:57.280227 amulog-0.3.8/amulog/eval/
--rw-r--r--   0 sat        (501) staff       (20)        0 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/eval/__init__.py
--rw-r--r--   0 sat        (501) staff       (20)    16444 2021-07-05 06:11:28.000000 amulog-0.3.8/amulog/eval/__main__.py
--rw-r--r--   0 sat        (501) staff       (20)     5461 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/eval/cluster_metrics.py
--rw-r--r--   0 sat        (501) staff       (20)    35547 2021-07-05 06:11:28.000000 amulog-0.3.8/amulog/eval/maketpl.py
--rw-r--r--   0 sat        (501) staff       (20)     3319 2021-07-05 06:11:28.000000 amulog-0.3.8/amulog/eval/param_searcher.py
--rw-r--r--   0 sat        (501) staff       (20)     3063 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/eval/structure_metrics.py
-drwxr-xr-x   0 sat        (501) staff       (20)        0 2021-12-20 07:55:57.281731 amulog-0.3.8/amulog/external/
--rw-r--r--   0 sat        (501) staff       (20)       98 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/external/__init__.py
--rw-r--r--   0 sat        (501) staff       (20)     1557 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/external/mod_tplseq.py
--rw-r--r--   0 sat        (501) staff       (20)     2113 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/external/regexhash.py
--rw-r--r--   0 sat        (501) staff       (20)     1587 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/external/tpl_match.py
--rwxr-xr-x   0 sat        (501) staff       (20)     6016 2021-04-04 19:18:33.000000 amulog-0.3.8/amulog/host_alias.py
--rwxr-xr-x   0 sat        (501) staff       (20)    42309 2021-11-25 04:55:39.000000 amulog-0.3.8/amulog/log_db.py
--rwxr-xr-x   0 sat        (501) staff       (20)    10338 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/logparser.py
--rwxr-xr-x   0 sat        (501) staff       (20)    17963 2021-10-30 08:24:05.000000 amulog-0.3.8/amulog/lt_common.py
--rwxr-xr-x   0 sat        (501) staff       (20)     2881 2021-02-08 11:25:00.000000 amulog-0.3.8/amulog/lt_import.py
--rwxr-xr-x   0 sat        (501) staff       (20)     3639 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/lt_import_ext.py
--rwxr-xr-x   0 sat        (501) staff       (20)     5096 2021-07-09 03:32:33.000000 amulog-0.3.8/amulog/lt_label.py
--rwxr-xr-x   0 sat        (501) staff       (20)     4048 2021-07-13 07:42:08.000000 amulog-0.3.8/amulog/lt_misc.py
--rw-r--r--   0 sat        (501) staff       (20)     3882 2021-07-27 14:06:03.000000 amulog-0.3.8/amulog/lt_regex.py
--rw-r--r--   0 sat        (501) staff       (20)    14377 2021-04-16 02:31:14.000000 amulog-0.3.8/amulog/lt_search.py
--rwxr-xr-x   0 sat        (501) staff       (20)     3290 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/lt_va.py
--rw-r--r--   0 sat        (501) staff       (20)    13487 2021-11-08 03:21:21.000000 amulog-0.3.8/amulog/ltg_semantics.py
--rw-r--r--   0 sat        (501) staff       (20)    20052 2021-10-28 07:27:44.000000 amulog-0.3.8/amulog/manager.py
--rw-r--r--   0 sat        (501) staff       (20)     3664 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/mproc_queue.py
--rwxr-xr-x   0 sat        (501) staff       (20)     1095 2020-11-15 13:23:08.000000 amulog-0.3.8/amulog/strutil.py
--rw-r--r--   0 sat        (501) staff       (20)     8874 2021-05-04 09:05:07.000000 amulog-0.3.8/amulog/testutil.py
-drwxr-xr-x   0 sat        (501) staff       (20)        0 2021-12-20 07:55:57.261095 amulog-0.3.8/amulog.egg-info/
--rw-r--r--   0 sat        (501) staff       (20)     6815 2021-12-20 07:55:56.000000 amulog-0.3.8/amulog.egg-info/PKG-INFO
--rw-r--r--   0 sat        (501) staff       (20)     1901 2021-12-20 07:55:56.000000 amulog-0.3.8/amulog.egg-info/SOURCES.txt
--rw-r--r--   0 sat        (501) staff       (20)        1 2021-12-20 07:55:56.000000 amulog-0.3.8/amulog.egg-info/dependency_links.txt
--rw-r--r--   0 sat        (501) staff       (20)      129 2021-12-20 07:55:56.000000 amulog-0.3.8/amulog.egg-info/entry_points.txt
--rw-r--r--   0 sat        (501) staff       (20)       72 2021-12-20 07:55:56.000000 amulog-0.3.8/amulog.egg-info/requires.txt
--rw-r--r--   0 sat        (501) staff       (20)       23 2021-12-20 07:55:56.000000 amulog-0.3.8/amulog.egg-info/top_level.txt
--rw-r--r--   0 sat        (501) staff       (20)       72 2021-07-29 08:17:58.000000 amulog-0.3.8/requirements.txt
--rw-r--r--   0 sat        (501) staff       (20)       38 2021-12-20 07:55:57.286244 amulog-0.3.8/setup.cfg
--rw-r--r--   0 sat        (501) staff       (20)     2068 2021-11-16 15:20:33.000000 amulog-0.3.8/setup.py
-drwxr-xr-x   0 sat        (501) staff       (20)        0 2021-12-20 07:55:57.283831 amulog-0.3.8/tests/
--rw-r--r--   0 sat        (501) staff       (20)        0 2020-11-15 13:23:08.000000 amulog-0.3.8/tests/__init__.py
--rw-r--r--   0 sat        (501) staff       (20)     1824 2021-07-05 22:00:21.000000 amulog-0.3.8/tests/test_crf.py
--rw-r--r--   0 sat        (501) staff       (20)     4037 2021-07-05 21:59:20.000000 amulog-0.3.8/tests/test_db.py
--rw-r--r--   0 sat        (501) staff       (20)     2912 2021-07-05 21:59:59.000000 amulog-0.3.8/tests/test_ltgen.py
-drwxr-xr-x   0 sat        (501) staff       (20)        0 2021-12-20 07:55:57.284757 amulog-0.3.8/tests-ext/
--rw-r--r--   0 sat        (501) staff       (20)        0 2020-11-15 13:23:08.000000 amulog-0.3.8/tests-ext/__init__.py
--rw-r--r--   0 sat        (501) staff       (20)     2534 2021-06-20 14:54:48.000000 amulog-0.3.8/tests-ext/test_mysql.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-11 08:21:10.436699 amulog-0.3.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1463 2022-03-11 08:20:15.000000 amulog-0.3.9/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)       64 2022-03-11 08:20:15.000000 amulog-0.3.9/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5330 2022-03-11 08:21:10.436699 amulog-0.3.9/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4506 2022-03-11 08:20:15.000000 amulog-0.3.9/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-11 08:21:10.428695 amulog-0.3.9/amulog/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      209 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/__init__.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    22923 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/__main__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-11 08:21:10.432697 amulog-0.3.9/amulog/alg/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       28 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/alg/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-11 08:21:10.432697 amulog-0.3.9/amulog/alg/crf/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       87 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/alg/crf/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6649 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/alg/crf/__main__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4439 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/alg/crf/_convert.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1614 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/alg/crf/_items.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23187 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/alg/crf/lt_crf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3604 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/alg/crf/train.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-11 08:21:10.432697 amulog-0.3.9/amulog/alg/dlog/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       66 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/alg/dlog/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4699 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/alg/dlog/dlog.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-11 08:21:10.432697 amulog-0.3.9/amulog/alg/drain/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      151 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/alg/drain/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4250 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/alg/drain/drain.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-11 08:21:10.432697 amulog-0.3.9/amulog/alg/fttree/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      156 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/alg/fttree/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4492 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/alg/fttree/fttree.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-11 08:21:10.432697 amulog-0.3.9/amulog/alg/lenma/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      151 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/alg/lenma/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4114 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/alg/lenma/lenma.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      500 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/alg/meta.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-11 08:21:10.432697 amulog-0.3.9/amulog/alg/shiso/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       91 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/alg/shiso/__init__.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     8312 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/alg/shiso/shiso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6634 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/anonymize.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1544 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/cli.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    12161 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/common.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    17933 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/config.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-11 08:21:10.436699 amulog-0.3.9/amulog/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8616 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/data/config.conf.default
+-rw-rw-r--   0 travis    (2000) travis    (2000)      144 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/data/crf_template.default
+-rw-rw-r--   0 travis    (2000) travis    (2000)       83 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/data/crf_template.sample
+-rw-rw-r--   0 travis    (2000) travis    (2000)       73 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/data/drain_regex.conf
+-rw-rw-r--   0 travis    (2000) travis    (2000)      308 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/data/host_alias.txt.sample
+-rw-rw-r--   0 travis    (2000) travis    (2000)      926 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/data/lt_label.conf.sample
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1729 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/data/testlog.conf
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     7486 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/db_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3476 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/db_mysql.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2918 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/db_sqlite.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-11 08:21:10.436699 amulog-0.3.9/amulog/edit/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/edit/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12028 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/edit/__main__.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     8593 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/edit/lt_tool.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2671 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/edit/search.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-11 08:21:10.436699 amulog-0.3.9/amulog/eval/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/eval/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16444 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/eval/__main__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5461 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/eval/cluster_metrics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35547 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/eval/maketpl.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3319 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/eval/param_searcher.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3063 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/eval/structure_metrics.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-11 08:21:10.436699 amulog-0.3.9/amulog/external/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       98 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/external/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1557 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/external/mod_tplseq.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2113 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/external/regexhash.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1587 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/external/tpl_match.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     6016 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/host_alias.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    42308 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/log_db.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    10338 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/logparser.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    18026 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/lt_common.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2881 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/lt_import.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3639 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/lt_import_ext.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     5096 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/lt_label.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     4048 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/lt_misc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3882 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/lt_regex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14377 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/lt_search.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3290 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/lt_va.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9054 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/ltg_semantics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20052 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/manager.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3664 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/mproc_queue.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1095 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/strutil.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8874 2022-03-11 08:20:15.000000 amulog-0.3.9/amulog/testutil.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-11 08:21:10.432697 amulog-0.3.9/amulog.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5330 2022-03-11 08:21:10.000000 amulog-0.3.9/amulog.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1901 2022-03-11 08:21:10.000000 amulog-0.3.9/amulog.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-03-11 08:21:10.000000 amulog-0.3.9/amulog.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      128 2022-03-11 08:21:10.000000 amulog-0.3.9/amulog.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       72 2022-03-11 08:21:10.000000 amulog-0.3.9/amulog.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       23 2022-03-11 08:21:10.000000 amulog-0.3.9/amulog.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       72 2022-03-11 08:20:15.000000 amulog-0.3.9/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2022-03-11 08:21:10.440701 amulog-0.3.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2068 2022-03-11 08:20:15.000000 amulog-0.3.9/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-11 08:21:10.436699 amulog-0.3.9/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2022-03-11 08:20:15.000000 amulog-0.3.9/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1824 2022-03-11 08:20:15.000000 amulog-0.3.9/tests/test_crf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4037 2022-03-11 08:20:15.000000 amulog-0.3.9/tests/test_db.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2912 2022-03-11 08:20:15.000000 amulog-0.3.9/tests/test_ltgen.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-11 08:21:10.436699 amulog-0.3.9/tests-ext/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2022-03-11 08:20:15.000000 amulog-0.3.9/tests-ext/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2534 2022-03-11 08:20:15.000000 amulog-0.3.9/tests-ext/test_mysql.py
```

### Comparing `amulog-0.3.8/LICENSE` & `amulog-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/README.rst` & `amulog-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/__main__.py` & `amulog-0.3.9/amulog/__main__.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/alg/crf/__main__.py` & `amulog-0.3.9/amulog/alg/crf/__main__.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/alg/crf/_convert.py` & `amulog-0.3.9/amulog/alg/crf/_convert.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/alg/crf/_items.py` & `amulog-0.3.9/amulog/alg/crf/_items.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/alg/crf/lt_crf.py` & `amulog-0.3.9/amulog/alg/crf/lt_crf.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/alg/crf/train.py` & `amulog-0.3.9/amulog/alg/crf/train.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/alg/dlog/dlog.py` & `amulog-0.3.9/amulog/alg/dlog/dlog.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/alg/drain/drain.py` & `amulog-0.3.9/amulog/alg/drain/drain.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/alg/fttree/fttree.py` & `amulog-0.3.9/amulog/alg/fttree/fttree.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/alg/lenma/lenma.py` & `amulog-0.3.9/amulog/alg/lenma/lenma.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/alg/shiso/shiso.py` & `amulog-0.3.9/amulog/alg/shiso/shiso.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/anonymize.py` & `amulog-0.3.9/amulog/anonymize.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/cli.py` & `amulog-0.3.9/amulog/cli.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/common.py` & `amulog-0.3.9/amulog/common.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/config.py` & `amulog-0.3.9/amulog/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-#!/usr/bin/env python
-# coding: utf-8
-
 import sys
 import os
 import datetime
 import logging
 import configparser
 from collections import defaultdict
 from dateutil.tz import tzlocal
+from typing import Tuple, Dict, List
 
 CONFIG_ENV = "AMULOG_CONFIG"
 DEFAULT_CONFIG = "/".join((os.path.dirname(os.path.abspath(__file__)),
                            "data/config.conf.default"))
 LOAD_SECTION = 'general'
 LOAD_OPTION = 'base_filename'
 IMPORT_SECTION = 'general'
@@ -81,33 +79,33 @@
 
     def iter_def(self):
         for group, l_val in self.gdict.items():
             for val in l_val:
                 yield group, val
 
 
-def gettuple(conf, section, name, sep=","):
-    ret = conf.get(section, name)
+def gettuple(conf, section, name, sep=",") -> Tuple[str]:
+    ret: str = conf.get(section, name)
     if ret.strip() == "":
         return tuple()
     else:
         return tuple(e.strip() for e in ret.split(sep)
                      if not len(e.strip()) == 0)
 
 
-def getlist(conf, section, name, sep=","):
+def getlist(conf, section, name, sep=",") -> List[str]:
     ret = conf.get(section, name)
     if ret.strip() == "":
         return []
     else:
         return [e.strip() for e in ret.split(sep)
                 if not len(e.strip()) == 0]
 
 
-def getdict(conf, section, name):
+def getdict(conf, section, name) -> Dict[str, str]:
     val = conf.get(section, name)
     ret = {}
     for e in val.split(","):
         e = e.strip()
         assert "=" in e
         k, _, v = e.partition("=")
         ret[k] = v
```

### Comparing `amulog-0.3.8/amulog/data/config.conf.default` & `amulog-0.3.9/amulog/data/config.conf.default`

 * *Files 12% similar despite different names*

```diff
@@ -244,29 +244,53 @@
 # If log_template_crf.normalizer_conf specified,
 # the inpu words are normalized with log-normalizer (currently not public)
 normalizer_conf =
 normalizer_rule = DEFAULT
 
 
 [log_template_group_semantics]
-# ['self', 'rfc'] or their combination
+use_cache = true
+
+# training sources
+# ['self', 'rfc', 'ltjunos'] or their combination
 # 'rfc' requires rfcyaml library
+# 'ltjunos' requires json file parsed by ltjunos library
 lda_knowledge_sources = self
-rfc_use_cache = True
 rfc_document_unit = rfc
+ltjunos_filepath =
+use_template_replacer = false
 
-lda_model = gensim
+# LDA parameters
+lda_library = gensim
 lda_stop_words =
 lda_use_nltk_stopwords = false
 lda_use_sklearn_stopwords = false
 lda_seed =
 lda_n_topics =
-cluster_eps =
-cluster_size_min = 5
-tuning_metrics = cluster
+lda_use_zscore = true
+lda_cachename = ldamodel
+guidedlda_seed_topic_list_file =
+guidedlda_seed_confidence = 0.15
+
+# clustering method
+# one of [DBSCAN, RecursiveDBSCAN]
+cluster_method = DBSCAN
+
+# used if cluster_method in [DBSCAN, RecursiveDBSCAN]
+# Empty in default for automated parameter tuning
+dbscan_eps =
+
+# used if cluster_method is DBSCAN
+dbscan_cluster_size_min = 5
+dbscan_tuning_metrics = cluster
+
+# used if cluster_method is RecursiveDBSCAN
+rdbscan_cluster_size_max = 20
+
+# rule-based parameter tuning
 tuning_union_rules =
 tuning_separation_rules =
 tuning_term_class = topic
 tuning_topwords = 10
 
 
 [nlp_preprocess]
```

### Comparing `amulog-0.3.8/amulog/data/lt_label.conf.sample` & `amulog-0.3.9/amulog/data/lt_label.conf.sample`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/data/testlog.conf` & `amulog-0.3.9/amulog/data/testlog.conf`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/db_common.py` & `amulog-0.3.9/amulog/db_common.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/db_mysql.py` & `amulog-0.3.9/amulog/db_mysql.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/db_sqlite.py` & `amulog-0.3.9/amulog/db_sqlite.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/edit/__main__.py` & `amulog-0.3.9/amulog/edit/__main__.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/edit/lt_tool.py` & `amulog-0.3.9/amulog/edit/lt_tool.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/edit/search.py` & `amulog-0.3.9/amulog/edit/search.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/eval/__main__.py` & `amulog-0.3.9/amulog/eval/__main__.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/eval/cluster_metrics.py` & `amulog-0.3.9/amulog/eval/cluster_metrics.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/eval/maketpl.py` & `amulog-0.3.9/amulog/eval/maketpl.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/eval/param_searcher.py` & `amulog-0.3.9/amulog/eval/param_searcher.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/eval/structure_metrics.py` & `amulog-0.3.9/amulog/eval/structure_metrics.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/external/mod_tplseq.py` & `amulog-0.3.9/amulog/external/mod_tplseq.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/external/regexhash.py` & `amulog-0.3.9/amulog/external/regexhash.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/external/tpl_match.py` & `amulog-0.3.9/amulog/external/tpl_match.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/host_alias.py` & `amulog-0.3.9/amulog/host_alias.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/log_db.py` & `amulog-0.3.9/amulog/log_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,15 +323,15 @@
         self.db.drop_all()
 
 
 class LogDB:
     """Interface of DB transaction for log data.
 
     Note:
-        It is not recommended to use this class directly.
+        It is not recommended using this class directly.
         Instead, use LogData.
     """
 
     tablename_log = "log"
     tablename_lt = "lt"
     tablename_ltg = "ltg"
     tablename_tag = "tag"
```

### Comparing `amulog-0.3.8/amulog/logparser.py` & `amulog-0.3.9/amulog/logparser.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/lt_common.py` & `amulog-0.3.9/amulog/lt_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -620,14 +620,18 @@
         from . import host_alias
         self.ha = host_alias.init_hostalias(conf)
 
     def replace_word(self, w):
         return self.ha.get_group(w)
 
 
+def is_replacer(word):
+    return REPLACER_REGEX.match(word)
+
+
 def merged_template(m1, m2):
     """Return common area of log message (to be log template)"""
     ret = []
     for w1, w2 in zip(m1, m2):
         if w1 == w2:
             ret.append(w1)
         else:
```

### Comparing `amulog-0.3.8/amulog/lt_import.py` & `amulog-0.3.9/amulog/lt_import.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/lt_import_ext.py` & `amulog-0.3.9/amulog/lt_import_ext.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/lt_label.py` & `amulog-0.3.9/amulog/lt_label.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/lt_misc.py` & `amulog-0.3.9/amulog/lt_misc.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/lt_regex.py` & `amulog-0.3.9/amulog/lt_regex.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/lt_search.py` & `amulog-0.3.9/amulog/lt_search.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/lt_va.py` & `amulog-0.3.9/amulog/lt_va.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/manager.py` & `amulog-0.3.9/amulog/manager.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/mproc_queue.py` & `amulog-0.3.9/amulog/mproc_queue.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/strutil.py` & `amulog-0.3.9/amulog/strutil.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog/testutil.py` & `amulog-0.3.9/amulog/testutil.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/amulog.egg-info/SOURCES.txt` & `amulog-0.3.9/amulog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/setup.py` & `amulog-0.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/tests/test_crf.py` & `amulog-0.3.9/tests/test_crf.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/tests/test_db.py` & `amulog-0.3.9/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/tests/test_ltgen.py` & `amulog-0.3.9/tests/test_ltgen.py`

 * *Files identical despite different names*

### Comparing `amulog-0.3.8/tests-ext/test_mysql.py` & `amulog-0.3.9/tests-ext/test_mysql.py`

 * *Files identical despite different names*


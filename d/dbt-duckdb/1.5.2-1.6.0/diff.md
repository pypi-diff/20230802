# Comparing `tmp/dbt-duckdb-1.5.2.tar.gz` & `tmp/dbt-duckdb-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-duckdb-1.5.2.tar", last modified: Thu Jun 22 16:53:39 2023, max compression
+gzip compressed data, was "dbt-duckdb-1.6.0.tar", last modified: Wed Aug  2 19:57:53 2023, max compression
```

## Comparing `dbt-duckdb-1.5.2.tar` & `dbt-duckdb-1.6.0.tar`

### file list

```diff
@@ -1,62 +1,64 @@
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-06-22 16:53:39.680233 dbt-duckdb-1.5.2/
--rw-r--r--   0 jwills     (501) staff       (20)    11357 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.2/LICENSE
--rw-r--r--   0 jwills     (501) staff       (20)       47 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.2/MANIFEST.in
--rw-r--r--   0 jwills     (501) staff       (20)    20476 2023-06-22 16:53:39.680080 dbt-duckdb-1.5.2/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)    20172 2023-06-22 16:52:09.000000 dbt-duckdb-1.5.2/README.md
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-06-22 16:53:39.671136 dbt-duckdb-1.5.2/dbt/
--rw-r--r--   0 jwills     (501) staff       (20)       92 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.2/dbt/__init__.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-06-22 16:53:39.671374 dbt-duckdb-1.5.2/dbt/adapters/
--rw-r--r--   0 jwills     (501) staff       (20)       92 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.2/dbt/adapters/__init__.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-06-22 16:53:39.673392 dbt-duckdb-1.5.2/dbt/adapters/duckdb/
--rw-r--r--   0 jwills     (501) staff       (20)      407 2023-03-23 17:19:15.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/__init__.py
--rw-r--r--   0 jwills     (501) staff       (20)       18 2023-06-22 16:14:09.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/__version__.py
--rw-r--r--   0 jwills     (501) staff       (20)     3573 2023-06-16 14:13:23.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/connections.py
--rw-r--r--   0 jwills     (501) staff       (20)     7027 2023-06-17 00:24:18.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/credentials.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-06-22 16:53:39.674112 dbt-duckdb-1.5.2/dbt/adapters/duckdb/environments/
--rw-r--r--   0 jwills     (501) staff       (20)     5307 2023-06-12 21:38:22.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/environments/__init__.py
--rw-r--r--   0 jwills     (501) staff       (20)     2399 2023-06-12 21:38:22.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/environments/buenavista.py
--rw-r--r--   0 jwills     (501) staff       (20)     4923 2023-06-16 14:13:23.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/environments/local.py
--rw-r--r--   0 jwills     (501) staff       (20)     8792 2023-06-07 23:05:31.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/impl.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-06-22 16:53:39.675505 dbt-duckdb-1.5.2/dbt/adapters/duckdb/plugins/
--rw-r--r--   0 jwills     (501) staff       (20)     4014 2023-06-07 23:05:31.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/plugins/__init__.py
--rw-r--r--   0 jwills     (501) staff       (20)      489 2023-06-07 23:05:31.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/plugins/excel.py
--rw-r--r--   0 jwills     (501) staff       (20)     8530 2023-06-07 23:05:31.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/plugins/glue.py
--rw-r--r--   0 jwills     (501) staff       (20)     1666 2023-06-07 23:05:31.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/plugins/gsheet.py
--rw-r--r--   0 jwills     (501) staff       (20)     1029 2023-06-07 23:05:31.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/plugins/iceberg.py
--rw-r--r--   0 jwills     (501) staff       (20)      533 2023-06-19 18:11:47.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/plugins/pd_utils.py
--rw-r--r--   0 jwills     (501) staff       (20)     1457 2023-06-19 18:11:47.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/plugins/sqlalchemy.py
--rw-r--r--   0 jwills     (501) staff       (20)     2519 2023-06-21 13:23:49.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/relation.py
--rw-r--r--   0 jwills     (501) staff       (20)     2213 2023-06-07 23:05:31.000000 dbt-duckdb-1.5.2/dbt/adapters/duckdb/utils.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-06-22 16:53:39.675672 dbt-duckdb-1.5.2/dbt/include/
--rw-r--r--   0 jwills     (501) staff       (20)       92 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.2/dbt/include/__init__.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-06-22 16:53:39.675922 dbt-duckdb-1.5.2/dbt/include/duckdb/
--rw-r--r--   0 jwills     (501) staff       (20)       52 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/__init__.py
--rw-r--r--   0 jwills     (501) staff       (20)       74 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/dbt_project.yml
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-06-22 16:53:39.677340 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/
--rw-r--r--   0 jwills     (501) staff       (20)     7996 2023-06-12 18:31:23.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/adapters.sql
--rw-r--r--   0 jwills     (501) staff       (20)      950 2023-05-05 22:17:51.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/catalog.sql
--rw-r--r--   0 jwills     (501) staff       (20)      643 2023-06-12 18:31:23.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/columns.sql
--rw-r--r--   0 jwills     (501) staff       (20)     1429 2023-06-16 14:13:23.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/incremental_helper.sql
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-06-22 16:53:39.677911 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/materializations/
--rw-r--r--   0 jwills     (501) staff       (20)     4128 2023-06-07 23:05:31.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/materializations/external.sql
--rw-r--r--   0 jwills     (501) staff       (20)     4679 2023-06-12 18:31:23.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/materializations/incremental.sql
--rw-r--r--   0 jwills     (501) staff       (20)     2529 2023-02-15 20:16:22.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/materializations/table.sql
--rw-r--r--   0 jwills     (501) staff       (20)     1755 2023-06-07 23:05:13.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/seed.sql
--rw-r--r--   0 jwills     (501) staff       (20)     1359 2023-06-16 14:13:23.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/snapshot_helper.sql
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-06-22 16:53:39.679323 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/utils/
--rw-r--r--   0 jwills     (501) staff       (20)       93 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/utils/any_value.sql
--rw-r--r--   0 jwills     (501) staff       (20)      175 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/utils/dateadd.sql
--rw-r--r--   0 jwills     (501) staff       (20)     2338 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/utils/datediff.sql
--rw-r--r--   0 jwills     (501) staff       (20)      357 2023-03-21 22:16:25.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/utils/external_location.sql
--rw-r--r--   0 jwills     (501) staff       (20)      378 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/utils/lastday.sql
--rw-r--r--   0 jwills     (501) staff       (20)      568 2022-12-21 20:35:46.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/utils/listagg.sql
--rw-r--r--   0 jwills     (501) staff       (20)      315 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/utils/splitpart.sql
--rw-r--r--   0 jwills     (501) staff       (20)     1724 2023-03-30 04:33:01.000000 dbt-duckdb-1.5.2/dbt/include/duckdb/macros/utils/upstream.sql
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-06-22 16:53:39.679936 dbt-duckdb-1.5.2/dbt_duckdb.egg-info/
--rw-r--r--   0 jwills     (501) staff       (20)    20476 2023-06-22 16:53:39.000000 dbt-duckdb-1.5.2/dbt_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)     1751 2023-06-22 16:53:39.000000 dbt-duckdb-1.5.2/dbt_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 jwills     (501) staff       (20)        1 2023-06-22 16:53:39.000000 dbt-duckdb-1.5.2/dbt_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 jwills     (501) staff       (20)       60 2023-06-22 16:53:39.000000 dbt-duckdb-1.5.2/dbt_duckdb.egg-info/requires.txt
--rw-r--r--   0 jwills     (501) staff       (20)        4 2023-06-22 16:53:39.000000 dbt-duckdb-1.5.2/dbt_duckdb.egg-info/top_level.txt
--rw-r--r--   0 jwills     (501) staff       (20)       38 2023-06-22 16:53:39.680261 dbt-duckdb-1.5.2/setup.cfg
--rw-r--r--   0 jwills     (501) staff       (20)     1366 2023-05-10 21:35:29.000000 dbt-duckdb-1.5.2/setup.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-08-02 19:57:53.985119 dbt-duckdb-1.6.0/
+-rw-r--r--   0 jwills     (501) staff       (20)    11357 2022-12-17 04:32:15.000000 dbt-duckdb-1.6.0/LICENSE
+-rw-r--r--   0 jwills     (501) staff       (20)       47 2022-12-17 04:32:15.000000 dbt-duckdb-1.6.0/MANIFEST.in
+-rw-r--r--   0 jwills     (501) staff       (20)    21631 2023-08-02 19:57:53.984985 dbt-duckdb-1.6.0/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)    20834 2023-08-02 19:57:40.000000 dbt-duckdb-1.6.0/README.md
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-08-02 19:57:53.974378 dbt-duckdb-1.6.0/dbt/
+-rw-r--r--   0 jwills     (501) staff       (20)       92 2022-12-17 04:32:15.000000 dbt-duckdb-1.6.0/dbt/__init__.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-08-02 19:57:53.974618 dbt-duckdb-1.6.0/dbt/adapters/
+-rw-r--r--   0 jwills     (501) staff       (20)       92 2022-12-17 04:32:15.000000 dbt-duckdb-1.6.0/dbt/adapters/__init__.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-08-02 19:57:53.976513 dbt-duckdb-1.6.0/dbt/adapters/duckdb/
+-rw-r--r--   0 jwills     (501) staff       (20)      407 2023-03-23 17:19:15.000000 dbt-duckdb-1.6.0/dbt/adapters/duckdb/__init__.py
+-rw-r--r--   0 jwills     (501) staff       (20)       18 2023-08-01 23:45:18.000000 dbt-duckdb-1.6.0/dbt/adapters/duckdb/__version__.py
+-rw-r--r--   0 jwills     (501) staff       (20)     3683 2023-08-01 23:45:18.000000 dbt-duckdb-1.6.0/dbt/adapters/duckdb/connections.py
+-rw-r--r--   0 jwills     (501) staff       (20)     7962 2023-08-01 23:45:18.000000 dbt-duckdb-1.6.0/dbt/adapters/duckdb/credentials.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-08-02 19:57:53.977160 dbt-duckdb-1.6.0/dbt/adapters/duckdb/environments/
+-rw-r--r--   0 jwills     (501) staff       (20)     5710 2023-08-01 23:45:18.000000 dbt-duckdb-1.6.0/dbt/adapters/duckdb/environments/__init__.py
+-rw-r--r--   0 jwills     (501) staff       (20)     2404 2023-07-04 14:25:31.000000 dbt-duckdb-1.6.0/dbt/adapters/duckdb/environments/buenavista.py
+-rw-r--r--   0 jwills     (501) staff       (20)     4968 2023-07-08 20:47:28.000000 dbt-duckdb-1.6.0/dbt/adapters/duckdb/environments/local.py
+-rw-r--r--   0 jwills     (501) staff       (20)     8748 2023-07-21 15:04:53.000000 dbt-duckdb-1.6.0/dbt/adapters/duckdb/impl.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-08-02 19:57:53.979209 dbt-duckdb-1.6.0/dbt/adapters/duckdb/plugins/
+-rw-r--r--   0 jwills     (501) staff       (20)     4095 2023-08-01 23:45:18.000000 dbt-duckdb-1.6.0/dbt/adapters/duckdb/plugins/__init__.py
+-rw-r--r--   0 jwills     (501) staff       (20)      489 2023-06-07 23:05:31.000000 dbt-duckdb-1.6.0/dbt/adapters/duckdb/plugins/excel.py
+-rw-r--r--   0 jwills     (501) staff       (20)     8732 2023-07-31 18:19:28.000000 dbt-duckdb-1.6.0/dbt/adapters/duckdb/plugins/glue.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1666 2023-06-07 23:05:31.000000 dbt-duckdb-1.6.0/dbt/adapters/duckdb/plugins/gsheet.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1029 2023-06-07 23:05:31.000000 dbt-duckdb-1.6.0/dbt/adapters/duckdb/plugins/iceberg.py
+-rw-r--r--   0 jwills     (501) staff       (20)      510 2023-07-21 15:04:53.000000 dbt-duckdb-1.6.0/dbt/adapters/duckdb/plugins/motherduck.py
+-rw-r--r--   0 jwills     (501) staff       (20)      533 2023-06-19 18:11:47.000000 dbt-duckdb-1.6.0/dbt/adapters/duckdb/plugins/pd_utils.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1296 2023-07-06 21:33:50.000000 dbt-duckdb-1.6.0/dbt/adapters/duckdb/plugins/postgres.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1484 2023-07-06 21:33:50.000000 dbt-duckdb-1.6.0/dbt/adapters/duckdb/plugins/sqlalchemy.py
+-rw-r--r--   0 jwills     (501) staff       (20)     2519 2023-06-21 13:23:49.000000 dbt-duckdb-1.6.0/dbt/adapters/duckdb/relation.py
+-rw-r--r--   0 jwills     (501) staff       (20)     2213 2023-06-07 23:05:31.000000 dbt-duckdb-1.6.0/dbt/adapters/duckdb/utils.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-08-02 19:57:53.979423 dbt-duckdb-1.6.0/dbt/include/
+-rw-r--r--   0 jwills     (501) staff       (20)       92 2022-12-17 04:32:15.000000 dbt-duckdb-1.6.0/dbt/include/__init__.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-08-02 19:57:53.979722 dbt-duckdb-1.6.0/dbt/include/duckdb/
+-rw-r--r--   0 jwills     (501) staff       (20)       52 2022-12-17 04:32:15.000000 dbt-duckdb-1.6.0/dbt/include/duckdb/__init__.py
+-rw-r--r--   0 jwills     (501) staff       (20)       74 2022-12-17 04:32:15.000000 dbt-duckdb-1.6.0/dbt/include/duckdb/dbt_project.yml
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-08-02 19:57:53.981137 dbt-duckdb-1.6.0/dbt/include/duckdb/macros/
+-rw-r--r--   0 jwills     (501) staff       (20)     7416 2023-07-21 15:04:53.000000 dbt-duckdb-1.6.0/dbt/include/duckdb/macros/adapters.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      950 2023-05-05 22:17:51.000000 dbt-duckdb-1.6.0/dbt/include/duckdb/macros/catalog.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      643 2023-06-12 18:31:23.000000 dbt-duckdb-1.6.0/dbt/include/duckdb/macros/columns.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     1429 2023-06-16 14:13:23.000000 dbt-duckdb-1.6.0/dbt/include/duckdb/macros/incremental_helper.sql
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-08-02 19:57:53.981815 dbt-duckdb-1.6.0/dbt/include/duckdb/macros/materializations/
+-rw-r--r--   0 jwills     (501) staff       (20)     4087 2023-07-21 15:04:53.000000 dbt-duckdb-1.6.0/dbt/include/duckdb/macros/materializations/external.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     4679 2023-06-12 18:31:23.000000 dbt-duckdb-1.6.0/dbt/include/duckdb/macros/materializations/incremental.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     2529 2023-02-15 20:16:22.000000 dbt-duckdb-1.6.0/dbt/include/duckdb/macros/materializations/table.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     1761 2023-08-01 18:48:11.000000 dbt-duckdb-1.6.0/dbt/include/duckdb/macros/seed.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     1359 2023-06-16 14:13:23.000000 dbt-duckdb-1.6.0/dbt/include/duckdb/macros/snapshot_helper.sql
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-08-02 19:57:53.984050 dbt-duckdb-1.6.0/dbt/include/duckdb/macros/utils/
+-rw-r--r--   0 jwills     (501) staff       (20)       93 2022-12-17 04:32:15.000000 dbt-duckdb-1.6.0/dbt/include/duckdb/macros/utils/any_value.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      175 2023-07-05 22:07:45.000000 dbt-duckdb-1.6.0/dbt/include/duckdb/macros/utils/dateadd.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     2338 2022-12-17 04:32:15.000000 dbt-duckdb-1.6.0/dbt/include/duckdb/macros/utils/datediff.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      357 2023-03-21 22:16:25.000000 dbt-duckdb-1.6.0/dbt/include/duckdb/macros/utils/external_location.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      378 2022-12-17 04:32:15.000000 dbt-duckdb-1.6.0/dbt/include/duckdb/macros/utils/lastday.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      568 2022-12-21 20:35:46.000000 dbt-duckdb-1.6.0/dbt/include/duckdb/macros/utils/listagg.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      167 2023-08-01 23:45:18.000000 dbt-duckdb-1.6.0/dbt/include/duckdb/macros/utils/splitpart.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     1683 2023-07-21 15:04:53.000000 dbt-duckdb-1.6.0/dbt/include/duckdb/macros/utils/upstream.sql
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-08-02 19:57:53.984738 dbt-duckdb-1.6.0/dbt_duckdb.egg-info/
+-rw-r--r--   0 jwills     (501) staff       (20)    21631 2023-08-02 19:57:53.000000 dbt-duckdb-1.6.0/dbt_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)     1833 2023-08-02 19:57:53.000000 dbt-duckdb-1.6.0/dbt_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 jwills     (501) staff       (20)        1 2023-08-02 19:57:53.000000 dbt-duckdb-1.6.0/dbt_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       60 2023-08-02 19:57:53.000000 dbt-duckdb-1.6.0/dbt_duckdb.egg-info/requires.txt
+-rw-r--r--   0 jwills     (501) staff       (20)        4 2023-08-02 19:57:53.000000 dbt-duckdb-1.6.0/dbt_duckdb.egg-info/top_level.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       38 2023-08-02 19:57:53.985150 dbt-duckdb-1.6.0/setup.cfg
+-rw-r--r--   0 jwills     (501) staff       (20)     1881 2023-08-01 23:45:18.000000 dbt-duckdb-1.6.0/setup.py
```

### Comparing `dbt-duckdb-1.5.2/LICENSE` & `dbt-duckdb-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.2/PKG-INFO` & `dbt-duckdb-1.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: dbt-duckdb
-Version: 1.5.2
-Summary: The duckdb adapter plugin for dbt (data build tool)
-Home-page: https://github.com/jwills/dbt-duckdb
-Author: Josh Wills
-Author-email: joshwills+dbt@gmail.com
-Description-Content-Type: text/markdown
-Provides-Extra: glue
-License-File: LICENSE
-
 ## dbt-duckdb
 
 [DuckDB](http://duckdb.org) is an embedded database, similar to SQLite, but designed for OLAP-style analytics.
 It is crazy fast and allows you to read and write data stored in CSV, JSON, and Parquet files directly, without requiring you to load
 them into the database first.
 
 [dbt](http://getdbt.com) is the best way to manage a collection of data transformations written in SQL or Python for analytics
@@ -62,16 +51,15 @@
 
 MotherDuck databases generally work the same way as local DuckDB databases from the perspective of dbt, but
 there are a [few differences to be aware of](https://motherduck.com/docs/architecture-and-capabilities#considerations-and-limitations):
 1. For the moment, MotherDuck _requires_ DuckDB version `0.8.1`.
 1. MotherDuck databases do not suppport transactions, so there is a new `disable_transactions` profile
 option that will be automatically enabled if you are connecting to a MotherDuck database in your `path`.
 1. MotherDuck preloads a set of the most common DuckDB extensions for you, but does not support loading custom extensions or user-defined functions.
-1. A small subset of advanced SQL features are currently unsupported; the only impact of this on the dbt adapter is that the [dbt.listagg](https://docs.getdbt.com/reference/dbt-jinja-functions/cross-database-macros#listagg) macro will work against a local DuckDB database, but will
-not work against MotherDuck.
+1. A small subset of advanced SQL features are currently unsupported; the only impact of this on the dbt adapter is that the [dbt.listagg](https://docs.getdbt.com/reference/dbt-jinja-functions/cross-database-macros#listagg) macro and foreign-key constraints will work against a local DuckDB database, but will not work against a MotherDuck database.
 
 #### DuckDB Extensions, Settings, and Filesystems
 
 You can load any supported [DuckDB extensions](https://duckdb.org/docs/extensions/overview) by listing them in
 the `extensions` field in your profile. You can also set any additional [DuckDB configuration options](https://duckdb.org/docs/sql/configuration)
 via the `settings` field, including options that are supported in any loaded extensions. For example, to be able to connect to S3 and read/write
 Parquet files using an AWS access key and secret, your profile would look something like this:
@@ -174,30 +162,40 @@
         - module: sqlalchemy
           alias: sql
           config:
             connection_url: "{{ env_var('DBT_ENV_SECRET_SQLALCHEMY_URI') }}"
         - module: path.to.custom_udf_module
 ```
 
-Every plugin must have a `module` property that indicates where the `Plugin` class to load is defined. Values of
-the `module` property that do not contain a "." are assumed to be one of the built-in plugins that are defined in
-[dbt.adapters.duckdb.plugins](dbt/adapters/duckdb/plugins/), while any values that do contain a "." are assumed to
-be user-defined modules that are visible on the Python path. Each plugin instance has a name for logging and reference
-purposes that defaults to the name of the module, but that may be overridden by the user by setting the `alias`
-property. Finally, modules may be initialized using an arbitrary set of key-value pairs that are defined in the
+Every plugin must have a `module` property that indicates where the `Plugin` class to load is defined. There is
+a set of built-in plugins that are defined in [dbt.adapters.duckdb.plugins](dbt/adapters/duckdb/plugins/) that
+may be referenced by their base filename (e.g., `excel` or `gsheet`), while user-defined plugins (which are
+described later in this document) should be referred to via their full module path name (e.g. a `lib.my.custom` module that defines a class named `Plugin`.)
+
+Each plugin instance has a name for logging and reference purposes that defaults to the name of the module
+but that may be overridden by the user by setting the `alias` property in the configuration. Finally,
+modules may be initialized using an arbitrary set of key-value pairs that are defined in the
 `config` dictionary. In this example, we initialize the `gsheet` plugin with the setting `method: oauth` and we
 initialize the `sqlalchemy` plugin (aliased as "sql") with a `connection_url` that is set via an environment variable.
 
 Please remember that using plugins may require you to add additional dependencies to the Python environment that your dbt-duckdb pipeline runs in:
 
 * `excel` depends on `pandas`
 * `gsheet` depends on `gspread` and `pandas`
 *  `iceberg` depends on `pyiceberg` and Python >= 3.8
 * `sqlalchemy` depends on `pandas`, `sqlalchemy`, and the driver(s) you need
 
+#### Using Local Python Modules
+
+In dbt-duckdb 1.6.0, we added a new profile setting named `module_paths` that allows users to specify a list
+of paths on the filesystem that contain additional Python modules that should be added to the Python processes'
+`sys.path` property. This allows users to include additional helper Python modules in their dbt projects that
+can be accessed by the running dbt process and used to define custom dbt-duckdb Plugins or library code that is
+helpful for creating dbt Python models.
+
 ### Reading and Writing External Files
 
 One of DuckDB's most powerful features is its ability to read and write CSV, JSON, and Parquet files directly, without needing to import/export
 them from the database first.
 
 #### Reading from external files
```

### Comparing `dbt-duckdb-1.5.2/README.md` & `dbt-duckdb-1.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: dbt-duckdb
+Version: 1.6.0
+Summary: The duckdb adapter plugin for dbt (data build tool)
+Home-page: https://github.com/jwills/dbt-duckdb
+Author: Josh Wills
+Author-email: joshwills+dbt@gmail.com
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: glue
+License-File: LICENSE
+
 ## dbt-duckdb
 
 [DuckDB](http://duckdb.org) is an embedded database, similar to SQLite, but designed for OLAP-style analytics.
 It is crazy fast and allows you to read and write data stored in CSV, JSON, and Parquet files directly, without requiring you to load
 them into the database first.
 
 [dbt](http://getdbt.com) is the best way to manage a collection of data transformations written in SQL or Python for analytics
@@ -51,16 +72,15 @@
 
 MotherDuck databases generally work the same way as local DuckDB databases from the perspective of dbt, but
 there are a [few differences to be aware of](https://motherduck.com/docs/architecture-and-capabilities#considerations-and-limitations):
 1. For the moment, MotherDuck _requires_ DuckDB version `0.8.1`.
 1. MotherDuck databases do not suppport transactions, so there is a new `disable_transactions` profile
 option that will be automatically enabled if you are connecting to a MotherDuck database in your `path`.
 1. MotherDuck preloads a set of the most common DuckDB extensions for you, but does not support loading custom extensions or user-defined functions.
-1. A small subset of advanced SQL features are currently unsupported; the only impact of this on the dbt adapter is that the [dbt.listagg](https://docs.getdbt.com/reference/dbt-jinja-functions/cross-database-macros#listagg) macro will work against a local DuckDB database, but will
-not work against MotherDuck.
+1. A small subset of advanced SQL features are currently unsupported; the only impact of this on the dbt adapter is that the [dbt.listagg](https://docs.getdbt.com/reference/dbt-jinja-functions/cross-database-macros#listagg) macro and foreign-key constraints will work against a local DuckDB database, but will not work against a MotherDuck database.
 
 #### DuckDB Extensions, Settings, and Filesystems
 
 You can load any supported [DuckDB extensions](https://duckdb.org/docs/extensions/overview) by listing them in
 the `extensions` field in your profile. You can also set any additional [DuckDB configuration options](https://duckdb.org/docs/sql/configuration)
 via the `settings` field, including options that are supported in any loaded extensions. For example, to be able to connect to S3 and read/write
 Parquet files using an AWS access key and secret, your profile would look something like this:
@@ -163,30 +183,40 @@
         - module: sqlalchemy
           alias: sql
           config:
             connection_url: "{{ env_var('DBT_ENV_SECRET_SQLALCHEMY_URI') }}"
         - module: path.to.custom_udf_module
 ```
 
-Every plugin must have a `module` property that indicates where the `Plugin` class to load is defined. Values of
-the `module` property that do not contain a "." are assumed to be one of the built-in plugins that are defined in
-[dbt.adapters.duckdb.plugins](dbt/adapters/duckdb/plugins/), while any values that do contain a "." are assumed to
-be user-defined modules that are visible on the Python path. Each plugin instance has a name for logging and reference
-purposes that defaults to the name of the module, but that may be overridden by the user by setting the `alias`
-property. Finally, modules may be initialized using an arbitrary set of key-value pairs that are defined in the
+Every plugin must have a `module` property that indicates where the `Plugin` class to load is defined. There is
+a set of built-in plugins that are defined in [dbt.adapters.duckdb.plugins](dbt/adapters/duckdb/plugins/) that
+may be referenced by their base filename (e.g., `excel` or `gsheet`), while user-defined plugins (which are
+described later in this document) should be referred to via their full module path name (e.g. a `lib.my.custom` module that defines a class named `Plugin`.)
+
+Each plugin instance has a name for logging and reference purposes that defaults to the name of the module
+but that may be overridden by the user by setting the `alias` property in the configuration. Finally,
+modules may be initialized using an arbitrary set of key-value pairs that are defined in the
 `config` dictionary. In this example, we initialize the `gsheet` plugin with the setting `method: oauth` and we
 initialize the `sqlalchemy` plugin (aliased as "sql") with a `connection_url` that is set via an environment variable.
 
 Please remember that using plugins may require you to add additional dependencies to the Python environment that your dbt-duckdb pipeline runs in:
 
 * `excel` depends on `pandas`
 * `gsheet` depends on `gspread` and `pandas`
 *  `iceberg` depends on `pyiceberg` and Python >= 3.8
 * `sqlalchemy` depends on `pandas`, `sqlalchemy`, and the driver(s) you need
 
+#### Using Local Python Modules
+
+In dbt-duckdb 1.6.0, we added a new profile setting named `module_paths` that allows users to specify a list
+of paths on the filesystem that contain additional Python modules that should be added to the Python processes'
+`sys.path` property. This allows users to include additional helper Python modules in their dbt projects that
+can be accessed by the running dbt process and used to define custom dbt-duckdb Plugins or library code that is
+helpful for creating dbt Python models.
+
 ### Reading and Writing External Files
 
 One of DuckDB's most powerful features is its ability to read and write CSV, JSON, and Parquet files directly, without needing to import/export
 them from the database first.
 
 #### Reading from external files
```

### Comparing `dbt-duckdb-1.5.2/dbt/adapters/duckdb/connections.py` & `dbt-duckdb-1.6.0/dbt/adapters/duckdb/connections.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import atexit
 import threading
 from contextlib import contextmanager
+from typing import Optional
 from typing import Tuple
 
 import agate
 
 import dbt.exceptions
 from . import environments
 from dbt.adapters.sql import SQLConnectionManager
@@ -36,15 +37,15 @@
         if connection.state == ConnectionState.OPEN:
             logger.debug("Connection is already open, skipping open.")
             return connection
 
         credentials = cls.get_credentials(connection.credentials)
         with cls._LOCK:
             try:
-                if not cls._ENV:
+                if not cls._ENV or cls._ENV.creds != credentials:
                     cls._ENV = environments.create(credentials)
                 connection.handle = cls._ENV.handle()
                 connection.state = ConnectionState.OPEN
 
             except RuntimeError as e:
                 logger.debug("Got an error when attempting to connect to DuckDB: '{}'".format(e))
                 connection.handle = None
@@ -91,15 +92,19 @@
     @classmethod
     def close_all_connections(cls):
         with cls._LOCK:
             if cls._ENV is not None:
                 cls._ENV = None
 
     def execute(
-        self, sql: str, auto_begin: bool = False, fetch: bool = False, **kwargs
+        self,
+        sql: str,
+        auto_begin: bool = False,
+        fetch: bool = False,
+        limit: Optional[int] = None,
     ) -> Tuple[AdapterResponse, agate.Table]:
         if self.disable_transactions:
             auto_begin = False
-        return super().execute(sql, auto_begin, fetch, **kwargs)
+        return super().execute(sql, auto_begin, fetch, limit)
 
 
 atexit.register(DuckDBConnectionManager.close_all_connections)
```

### Comparing `dbt-duckdb-1.5.2/dbt/adapters/duckdb/credentials.py` & `dbt-duckdb-1.6.0/dbt/adapters/duckdb/credentials.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from urllib.parse import urlparse
 
-import duckdb
-
 import dbt.exceptions
 from dbt.adapters.base import Credentials
 from dbt.dataclass_schema import dbtClassMixin
 
 
 @dataclass
 class Attachment(dbtClassMixin):
@@ -113,55 +111,85 @@
     plugins: Optional[List[PluginConfig]] = None
 
     # Whether to disable transactions when executing SQL statements; this
     # is useful when we would like the resulting DuckDB database file to
     # be as small as possible.
     disable_transactions: bool = False
 
+    # Whether to keep the DuckDB connection open between invocations of dbt
+    # (we do this automatically for in-memory or MD connections, but not for
+    # local DuckDB files, but this is a way to override that behavior)
+    keep_open: bool = False
+
+    # A list of paths to Python modules that should be loaded into the
+    # running Python environment when dbt is invoked; this is useful for
+    # loading custom dbt-duckdb plugins or locally defined modules that
+    # provide helper functions for dbt Python models.
+    module_paths: Optional[List[str]] = None
+
     @classmethod
     def __pre_deserialize__(cls, data: Dict[Any, Any]) -> Dict[Any, Any]:
-        if duckdb.__version__ >= "0.7.0":
-            data = super().__pre_deserialize__(data)
-            if "database" not in data:
-                # if no database is specified in the profile, figure out
-                # the database value to use from the path argument
-                path = data.get("path")
-                if path is None or path == ":memory:":
-                    data["database"] = "memory"
-                else:
-                    parsed = urlparse(path)
-                    base_file = os.path.basename(parsed.path)
-                    db = os.path.splitext(base_file)[0]
-                    if db:
-                        data["database"] = db
-                    else:
-                        raise dbt.exceptions.DbtRuntimeError(
-                            "Unable to determine database name from path"
-                            " and no database was specified in profile"
-                        )
-                    # For MotherDuck, turn on disable_transactions unless
-                    # it's explicitly set already by the user
-                    if parsed.scheme in {"md", "motherduck"}:
-                        if "disable_transactions" not in data:
-                            data["disable_transactions"] = True
+        data = super().__pre_deserialize__(data)
+        path = data.get("path")
+        path_db = None
+        if path is None or path == ":memory:":
+            path_db = "memory"
+        else:
+            parsed = urlparse(path)
+            base_file = os.path.basename(parsed.path)
+            path_db = os.path.splitext(base_file)[0]
+            # For MotherDuck, turn on disable_transactions unless
+            # it's explicitly set already by the user
+            if parsed.scheme in {"md", "motherduck"}:
+                if "disable_transactions" not in data:
+                    data["disable_transactions"] = True
+                if path_db == "":
+                    path_db = "my_db"
+
+        if path_db and "database" not in data:
+            data["database"] = path_db
+        elif path_db and data["database"] != path_db:
+            if not data.get("remote"):
+                raise dbt.exceptions.DbtRuntimeError(
+                    "Inconsistency detected between 'path' and 'database' fields in profile; "
+                    f"the 'database' property must be set to '{path_db}' to match the 'path'"
+                )
+        elif not path_db:
+            raise dbt.exceptions.DbtRuntimeError(
+                "Unable to determine target database name from 'path' field in profile"
+            )
         return data
 
     @property
     def unique_field(self) -> str:
         if self.remote:
             return self.remote.host + str(self.remote.port)
         else:
             return self.path + self.external_root
 
     @property
     def type(self):
         return "duckdb"
 
     def _connection_keys(self):
-        return ("database", "schema", "path")
+        return (
+            "database",
+            "schema",
+            "path",
+            "config_options",
+            "extensions",
+            "settings",
+            "external_root",
+            "use_credential_provider",
+            "attach",
+            "filesystems",
+            "remote",
+            "plugins",
+            "disable_transactions",
+        )
 
     def load_settings(self) -> Dict[str, str]:
         settings = self.settings or {}
         if self.use_credential_provider:
             if self.use_credential_provider == "aws":
                 settings.update(_load_aws_credentials(ttl=_get_ttl_hash()))
             else:
```

### Comparing `dbt-duckdb-1.5.2/dbt/adapters/duckdb/environments/__init__.py` & `dbt-duckdb-1.6.0/dbt/adapters/duckdb/environments/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import abc
 import importlib.util
 import os
+import sys
 import tempfile
 from typing import Dict
 from typing import Optional
 
 import duckdb
 
 from ..credentials import DuckDBCredentials
@@ -32,14 +33,27 @@
 
 class Environment(abc.ABC):
     """An Environment is an abstraction to describe *where* the code you execute in your dbt-duckdb project
     actually runs. This could be the local Python process that runs dbt (which is the default),
     a remote server (like a Buena Vista instance), or even a Jupyter notebook kernel.
     """
 
+    def __init__(self, creds: DuckDBCredentials):
+        self._creds = creds
+
+        # Add any module paths to the Python path for the environment
+        if creds.module_paths:
+            for path in creds.module_paths:
+                if path not in sys.path:
+                    sys.path.append(path)
+
+    @property
+    def creds(self) -> DuckDBCredentials:
+        return self._creds
+
     @abc.abstractmethod
     def handle(self):
         pass
 
     @abc.abstractmethod
     def submit_python_job(self, handle, parsed_model: dict, compiled_code: str) -> AdapterResponse:
         pass
```

### Comparing `dbt-duckdb-1.5.2/dbt/adapters/duckdb/environments/buenavista.py` & `dbt-duckdb-1.6.0/dbt/adapters/duckdb/environments/buenavista.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             user=remote.user,
             host=remote.host,
             port=remote.port,
             password=remote.password,
         )
 
     def __init__(self, credentials: credentials.DuckDBCredentials):
-        self.creds = credentials
+        super().__init__(credentials)
         if not self.creds.remote:
             raise Exception("BVConnection only works with a remote host")
 
     def handle(self):
         # Extensions/settings need to be configured per cursor
         conn = self._get_conn(self.creds.database, self.creds.remote)
         cursor = self.initialize_cursor(self.creds, conn.cursor())
```

### Comparing `dbt-duckdb-1.5.2/dbt/adapters/duckdb/environments/local.py` & `dbt-duckdb-1.6.0/dbt/adapters/duckdb/environments/local.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,23 +38,24 @@
         return self._cursor
 
 
 class LocalEnvironment(Environment):
     def __init__(self, credentials: credentials.DuckDBCredentials):
         # Set the conn attribute to None so it always exists even if
         # DB initialization fails
+        super().__init__(credentials)
         self.conn = None
         self._plugins = self.initialize_plugins(credentials)
-        self.creds = credentials
         self.handle_count = 0
         self.lock = threading.RLock()
         self._keep_open = (
-            self.creds.path == ":memory:"
-            or self.creds.path.startswith("md:")
-            or self.creds.path.startswith("motherduck:")
+            credentials.keep_open
+            or credentials.path == ":memory:"
+            or credentials.path.startswith("md:")
+            or credentials.path.startswith("motherduck:")
         )
 
     def notify_closed(self):
         with self.lock:
             self.handle_count -= 1
             if self.handle_count == 0 and not self._keep_open:
                 self.close()
```

### Comparing `dbt-duckdb-1.5.2/dbt/adapters/duckdb/impl.py` & `dbt-duckdb-1.6.0/dbt/adapters/duckdb/impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 from typing import List
 from typing import Optional
 from typing import Sequence
 
 import agate
-import duckdb
 
 from dbt.adapters.base import BaseRelation
 from dbt.adapters.base.column import Column
 from dbt.adapters.base.impl import ConstraintSupport
 from dbt.adapters.base.meta import available
 from dbt.adapters.duckdb.connections import DuckDBConnectionManager
 from dbt.adapters.duckdb.relation import DuckDBRelation
@@ -38,14 +37,17 @@
     def date_function(cls) -> str:
         return "now()"
 
     @classmethod
     def is_cancelable(cls) -> bool:
         return False
 
+    def debug_query(self):
+        self.execute("select 1 as id")
+
     @available
     def convert_datetimes_to_strs(self, table: agate.Table) -> agate.Table:
         for column in table.columns:
             if isinstance(column.data_type, agate.DateTime):
                 table = table.compute(
                     [
                         (
@@ -90,18 +92,14 @@
         DuckDBConnectionManager.env().store_relation(plugin_name, target_config)
 
     @available
     def external_root(self) -> str:
         return self.config.credentials.external_root
 
     @available
-    def use_database(self) -> bool:
-        return duckdb.__version__ >= "0.7.0"
-
-    @available
     def get_binding_char(self):
         return DuckDBConnectionManager.env().get_binding_char()
 
     @available
     def external_write_options(self, write_location: str, rendered_options: dict) -> str:
         if "format" not in rendered_options:
             ext = os.path.splitext(write_location)[1].lower()
```

### Comparing `dbt-duckdb-1.5.2/dbt/adapters/duckdb/plugins/__init__.py` & `dbt-duckdb-1.6.0/dbt/adapters/duckdb/plugins/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import importlib
+import os
 from typing import Any
 from typing import Dict
 from typing import Optional
 
 from duckdb import DuckDBPyConnection
 
 from ..utils import SourceConfig
@@ -19,14 +20,19 @@
 class BasePlugin:
     """
     BasePlugin is the base class for creating plugins. A plugin can be created
     from a module name, an optional configuration, and an alias. Each plugin
     contains a name and its configuration.
     """
 
+    # A set of built-in plugins that are included with dbt-duckdb.
+    _BUILTIN = set(
+        [x.split(".")[0] for x in os.listdir(os.path.dirname(__file__)) if "_" not in x]
+    )
+
     @classmethod
     def create(
         cls,
         module: str,
         *,
         config: Optional[Dict[str, Any]] = None,
         alias: Optional[str] = None,
@@ -39,26 +45,24 @@
         :param alias: An optional string representing the alias name of the module.
         :return: A Plugin instance.
         :raises ImportError: If the module cannot be imported.
         """
         if not isinstance(module, str):
             raise TypeError("Module name must be a string.")
 
-        if "." not in module:
-            # if the module does not have a dot, assume it is a builtin
-            # plugin module and prepend the path name
+        if module in cls._BUILTIN:
             name = module
             module = f"dbt.adapters.duckdb.plugins.{module}"
         else:
             name = module.split(".")[-1]
 
         try:
             mod = importlib.import_module(module)
-        except ImportError:
-            raise ImportError(f"Unable to import module '{module}'.")
+        except ImportError as e:
+            raise ImportError(f"Unable to import module '{module}': {e}")
 
         if not hasattr(mod, "Plugin"):
             raise ImportError(f"Module '{module}' does not have a Plugin class.")
         else:
             return mod.Plugin(alias or name, config or {})
 
     def __init__(self, name: str, plugin_config: Dict[str, Any]):
```

### Comparing `dbt-duckdb-1.5.2/dbt/adapters/duckdb/plugins/glue.py` & `dbt-duckdb-1.6.0/dbt/adapters/duckdb/plugins/glue.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,22 @@
         return None
 
 
 def _get_column_type_def(
     table_def: "GetTableResponseTypeDef",
 ) -> Optional[Sequence["ColumnTypeDef"]]:
     """Get columns definition from Glue Table Definition"""
-    return table_def.get("Table", {}).get("StorageDescriptor", {}).get("Columns")
+    raw = table_def.get("Table", {}).get("StorageDescriptor", {}).get("Columns")
+    if raw:
+        converted = []
+        for column in raw:
+            converted.append(ColumnTypeDef(Name=column["Name"], Type=column["Type"]))
+        return converted
+    else:
+        return None
 
 
 def _get_table_def(
     table: str,
     s3_path: str,
     columns: Sequence["ColumnTypeDef"],
     file_format: str,
```

### Comparing `dbt-duckdb-1.5.2/dbt/adapters/duckdb/plugins/gsheet.py` & `dbt-duckdb-1.6.0/dbt/adapters/duckdb/plugins/gsheet.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.2/dbt/adapters/duckdb/plugins/iceberg.py` & `dbt-duckdb-1.6.0/dbt/adapters/duckdb/plugins/iceberg.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.2/dbt/adapters/duckdb/plugins/pd_utils.py` & `dbt-duckdb-1.6.0/dbt/adapters/duckdb/plugins/pd_utils.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.2/dbt/adapters/duckdb/plugins/sqlalchemy.py` & `dbt-duckdb-1.6.0/dbt/adapters/duckdb/plugins/sqlalchemy.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,7 +35,8 @@
         df = pd_utils.target_to_df(target_config)
         table_name = target_config.relation.identifier
         # then, write it to the database
         df.to_sql(table_name, self.engine, if_exists="replace", index=False)
 
     def __del__(self):
         self.engine.dispose()
+        self.engine = None
```

### Comparing `dbt-duckdb-1.5.2/dbt/adapters/duckdb/relation.py` & `dbt-duckdb-1.6.0/dbt/adapters/duckdb/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.2/dbt/adapters/duckdb/utils.py` & `dbt-duckdb-1.6.0/dbt/adapters/duckdb/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.2/dbt/include/duckdb/macros/adapters.sql` & `dbt-duckdb-1.6.0/dbt/include/duckdb/macros/adapters.sql`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 
 {% macro duckdb__create_schema(relation) -%}
   {%- call statement('create_schema') -%}
-    create schema if not exists {{ relation.without_identifier().include(database=adapter.use_database()) }}
+    create schema if not exists {{ relation.without_identifier() }}
   {%- endcall -%}
 {% endmacro %}
 
 {% macro duckdb__drop_schema(relation) -%}
   {%- call statement('drop_schema') -%}
-    drop schema if exists {{ relation.without_identifier().include(database=adapter.use_database()) }} cascade
+    drop schema if exists {{ relation.without_identifier() }} cascade
   {%- endcall -%}
 {% endmacro %}
 
 {% macro duckdb__list_schemas(database) -%}
   {% set sql %}
     select schema_name
     from system.information_schema.schemata
@@ -23,17 +23,15 @@
 {% endmacro %}
 
 {% macro duckdb__check_schema_exists(information_schema, schema) -%}
   {% set sql -%}
         select count(*)
         from system.information_schema.schemata
         where schema_name = '{{ schema }}'
-        {% if adapter.use_database() %}
         and catalog_name = '{{ information_schema.database }}'
-        {% endif %}
   {%- endset %}
   {{ return(run_query(sql)) }}
 {% endmacro %}
 
 {% macro get_column_names() %}
   {# loop through user_provided_columns to get column names #}
     {%- set user_provided_columns = model['columns'] -%}
@@ -53,15 +51,15 @@
       {{ get_assert_columns_equivalent(compiled_code) }}
     {% endif %}
     {%- set sql_header = config.get('sql_header', none) -%}
 
     {{ sql_header if sql_header is not none }}
 
     create {% if temporary: -%}temporary{%- endif %} table
-      {{ relation.include(database=(not temporary and adapter.use_database()), schema=(not temporary)) }}
+      {{ relation.include(database=(not temporary), schema=(not temporary)) }}
   {% if contract_config.enforced and not temporary %}
     {#-- DuckDB doesnt support constraints on temp tables --#}
     {{ get_table_columns_and_constraints() }} ;
     insert into {{ relation }} {{ get_column_names() }} (
       {{ get_select_subquery(compiled_code) }}
     );
   {% else %}
@@ -85,26 +83,26 @@
         pyarrow_available = True
     except ImportError:
         pyarrow_available = False
     finally:
         if pyarrow_available and isinstance(df, pyarrow.Table):
             # https://github.com/duckdb/duckdb/issues/6584
             import pyarrow.dataset
-    con.execute('create table {{ relation.include(database=adapter.use_database()) }} as select * from df')
+    con.execute('create table {{ relation }} as select * from df')
 {% endmacro %}
 
 {% macro duckdb__create_view_as(relation, sql) -%}
   {% set contract_config = config.get('contract') %}
   {% if contract_config.enforced %}
     {{ get_assert_columns_equivalent(sql) }}
   {%- endif %}
   {%- set sql_header = config.get('sql_header', none) -%}
 
   {{ sql_header if sql_header is not none }}
-  create view {{ relation.include(database=adapter.use_database()) }} as (
+  create view {{ relation }} as (
     {{ sql }}
   );
 {% endmacro %}
 
 {% macro duckdb__get_columns_in_relation(relation) -%}
   {% call statement('get_columns_in_relation', fetch_result=True) %}
       select
@@ -115,15 +113,15 @@
           numeric_scale
 
       from system.information_schema.columns
       where table_name = '{{ relation.identifier }}'
       {% if relation.schema %}
       and table_schema = '{{ relation.schema }}'
       {% endif %}
-      {% if adapter.use_database() and relation.database %}
+      {% if relation.database %}
       and table_catalog = '{{ relation.database }}'
       {% endif %}
       order by ordinal_position
 
   {% endcall %}
   {% set table = load_result('get_columns_in_relation').table %}
   {{ return(sql_convert_columns_in_relation(table)) }}
@@ -138,30 +136,22 @@
       CASE table_type
         WHEN 'BASE TABLE' THEN 'table'
         WHEN 'VIEW' THEN 'view'
         WHEN 'LOCAL TEMPORARY' THEN 'table'
         END as type
     from system.information_schema.tables
     where table_schema = '{{ schema_relation.schema }}'
-    {% if adapter.use_database() %}
     and table_catalog = '{{ schema_relation.database }}'
-    {% endif %}
   {% endcall %}
   {{ return(load_result('list_relations_without_caching').table) }}
 {% endmacro %}
 
 {% macro duckdb__drop_relation(relation) -%}
   {% call statement('drop_relation', auto_begin=False) -%}
-    drop {{ relation.type }} if exists {{ relation.include(database=adapter.use_database()) }} cascade
-  {%- endcall %}
-{% endmacro %}
-
-{% macro duckdb__truncate_relation(relation) -%}
-  {% call statement('truncate_relation') -%}
-    DELETE FROM {{ relation.include(database=adapter.use_database()) }} WHERE 1=1
+    drop {{ relation.type }} if exists {{ relation }} cascade
   {%- endcall %}
 {% endmacro %}
 
 {% macro duckdb__rename_relation(from_relation, to_relation) -%}
   {% set target_name = adapter.quote_as_configured(to_relation.identifier, 'identifier') %}
   {% call statement('rename_relation') -%}
     alter {{ to_relation.type }} {{ from_relation }} rename to {{ target_name }}
```

### Comparing `dbt-duckdb-1.5.2/dbt/include/duckdb/macros/catalog.sql` & `dbt-duckdb-1.6.0/dbt/include/duckdb/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.2/dbt/include/duckdb/macros/columns.sql` & `dbt-duckdb-1.6.0/dbt/include/duckdb/macros/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.2/dbt/include/duckdb/macros/incremental_helper.sql` & `dbt-duckdb-1.6.0/dbt/include/duckdb/macros/incremental_helper.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.2/dbt/include/duckdb/macros/materializations/external.sql` & `dbt-duckdb-1.6.0/dbt/include/duckdb/macros/materializations/external.sql`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     {{- create_table_as(False, temp_relation, compiled_code, language) }}
   {%- endcall %}
 
   -- write an temp relation into file
   {{ write_to_file(temp_relation, location, write_options) }}
   -- create a view on top of the location
   {% call statement('main', language='sql') -%}
-    create or replace view {{ intermediate_relation.include(database=adapter.use_database()) }} as (
+    create or replace view {{ intermediate_relation }} as (
         select * from '{{ read_location }}'
     );
   {%- endcall %}
 
   -- cleanup
   {% if existing_relation is not none %}
       {{ adapter.rename_relation(existing_relation, backup_relation) }}
```

### Comparing `dbt-duckdb-1.5.2/dbt/include/duckdb/macros/materializations/incremental.sql` & `dbt-duckdb-1.6.0/dbt/include/duckdb/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.2/dbt/include/duckdb/macros/materializations/table.sql` & `dbt-duckdb-1.6.0/dbt/include/duckdb/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.2/dbt/include/duckdb/macros/seed.sql` & `dbt-duckdb-1.6.0/dbt/include/duckdb/macros/seed.sql`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 {% endmacro %}
 
 {% macro duckdb__get_batch_size() %}
   {{ return(10000) }}
 {% endmacro %}
 
 {% macro duckdb__load_csv_rows(model, agate_table) %}
-    {% if config.get('fast') %}
+    {% if config.get('fast', true) %}
         {% set seed_file_path = adapter.get_seed_file_path(model) %}
         {% set sql %}
           COPY {{ this.render() }} FROM '{{ seed_file_path }}' (FORMAT CSV, HEADER TRUE)
         {% endset %}
         {% do adapter.add_query(sql, abridge_sql_log=True) %}
         {{ return(sql) }}
     {% endif %}
```

### Comparing `dbt-duckdb-1.5.2/dbt/include/duckdb/macros/snapshot_helper.sql` & `dbt-duckdb-1.6.0/dbt/include/duckdb/macros/snapshot_helper.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.2/dbt/include/duckdb/macros/utils/datediff.sql` & `dbt-duckdb-1.6.0/dbt/include/duckdb/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.2/dbt/include/duckdb/macros/utils/listagg.sql` & `dbt-duckdb-1.6.0/dbt/include/duckdb/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.2/dbt/include/duckdb/macros/utils/upstream.sql` & `dbt-duckdb-1.6.0/dbt/include/duckdb/macros/utils/upstream.sql`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         {% if upstream_rel.schema not in upstream_schemas %}
           {% call statement('main', language='sql') -%}
             create schema if not exists {{ upstream_rel.schema }}
           {%- endcall %}
           {% do upstream_schemas.update({upstream_rel.schema: None}) %}
         {% endif %}
         {% call statement('main', language='sql') -%}
-          create or replace view {{ upstream_rel.include(database=adapter.use_database()) }} as (
+          create or replace view {{ upstream_rel }} as (
             select * from '{{ upstream_location }}'
           );
         {%- endcall %}
       {%- endif %}
     {% endif %}
   {% endfor %}
 {% endfor %}
```

### Comparing `dbt-duckdb-1.5.2/dbt_duckdb.egg-info/PKG-INFO` & `dbt-duckdb-1.6.0/dbt_duckdb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 Metadata-Version: 2.1
 Name: dbt-duckdb
-Version: 1.5.2
+Version: 1.6.0
 Summary: The duckdb adapter plugin for dbt (data build tool)
 Home-page: https://github.com/jwills/dbt-duckdb
 Author: Josh Wills
 Author-email: joshwills+dbt@gmail.com
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: glue
 License-File: LICENSE
 
 ## dbt-duckdb
 
 [DuckDB](http://duckdb.org) is an embedded database, similar to SQLite, but designed for OLAP-style analytics.
@@ -62,16 +72,15 @@
 
 MotherDuck databases generally work the same way as local DuckDB databases from the perspective of dbt, but
 there are a [few differences to be aware of](https://motherduck.com/docs/architecture-and-capabilities#considerations-and-limitations):
 1. For the moment, MotherDuck _requires_ DuckDB version `0.8.1`.
 1. MotherDuck databases do not suppport transactions, so there is a new `disable_transactions` profile
 option that will be automatically enabled if you are connecting to a MotherDuck database in your `path`.
 1. MotherDuck preloads a set of the most common DuckDB extensions for you, but does not support loading custom extensions or user-defined functions.
-1. A small subset of advanced SQL features are currently unsupported; the only impact of this on the dbt adapter is that the [dbt.listagg](https://docs.getdbt.com/reference/dbt-jinja-functions/cross-database-macros#listagg) macro will work against a local DuckDB database, but will
-not work against MotherDuck.
+1. A small subset of advanced SQL features are currently unsupported; the only impact of this on the dbt adapter is that the [dbt.listagg](https://docs.getdbt.com/reference/dbt-jinja-functions/cross-database-macros#listagg) macro and foreign-key constraints will work against a local DuckDB database, but will not work against a MotherDuck database.
 
 #### DuckDB Extensions, Settings, and Filesystems
 
 You can load any supported [DuckDB extensions](https://duckdb.org/docs/extensions/overview) by listing them in
 the `extensions` field in your profile. You can also set any additional [DuckDB configuration options](https://duckdb.org/docs/sql/configuration)
 via the `settings` field, including options that are supported in any loaded extensions. For example, to be able to connect to S3 and read/write
 Parquet files using an AWS access key and secret, your profile would look something like this:
@@ -174,30 +183,40 @@
         - module: sqlalchemy
           alias: sql
           config:
             connection_url: "{{ env_var('DBT_ENV_SECRET_SQLALCHEMY_URI') }}"
         - module: path.to.custom_udf_module
 ```
 
-Every plugin must have a `module` property that indicates where the `Plugin` class to load is defined. Values of
-the `module` property that do not contain a "." are assumed to be one of the built-in plugins that are defined in
-[dbt.adapters.duckdb.plugins](dbt/adapters/duckdb/plugins/), while any values that do contain a "." are assumed to
-be user-defined modules that are visible on the Python path. Each plugin instance has a name for logging and reference
-purposes that defaults to the name of the module, but that may be overridden by the user by setting the `alias`
-property. Finally, modules may be initialized using an arbitrary set of key-value pairs that are defined in the
+Every plugin must have a `module` property that indicates where the `Plugin` class to load is defined. There is
+a set of built-in plugins that are defined in [dbt.adapters.duckdb.plugins](dbt/adapters/duckdb/plugins/) that
+may be referenced by their base filename (e.g., `excel` or `gsheet`), while user-defined plugins (which are
+described later in this document) should be referred to via their full module path name (e.g. a `lib.my.custom` module that defines a class named `Plugin`.)
+
+Each plugin instance has a name for logging and reference purposes that defaults to the name of the module
+but that may be overridden by the user by setting the `alias` property in the configuration. Finally,
+modules may be initialized using an arbitrary set of key-value pairs that are defined in the
 `config` dictionary. In this example, we initialize the `gsheet` plugin with the setting `method: oauth` and we
 initialize the `sqlalchemy` plugin (aliased as "sql") with a `connection_url` that is set via an environment variable.
 
 Please remember that using plugins may require you to add additional dependencies to the Python environment that your dbt-duckdb pipeline runs in:
 
 * `excel` depends on `pandas`
 * `gsheet` depends on `gspread` and `pandas`
 *  `iceberg` depends on `pyiceberg` and Python >= 3.8
 * `sqlalchemy` depends on `pandas`, `sqlalchemy`, and the driver(s) you need
 
+#### Using Local Python Modules
+
+In dbt-duckdb 1.6.0, we added a new profile setting named `module_paths` that allows users to specify a list
+of paths on the filesystem that contain additional Python modules that should be added to the Python processes'
+`sys.path` property. This allows users to include additional helper Python modules in their dbt projects that
+can be accessed by the running dbt process and used to define custom dbt-duckdb Plugins or library code that is
+helpful for creating dbt Python models.
+
 ### Reading and Writing External Files
 
 One of DuckDB's most powerful features is its ability to read and write CSV, JSON, and Parquet files directly, without needing to import/export
 them from the database first.
 
 #### Reading from external files
```

### Comparing `dbt-duckdb-1.5.2/dbt_duckdb.egg-info/SOURCES.txt` & `dbt-duckdb-1.6.0/dbt_duckdb.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 dbt/adapters/duckdb/environments/buenavista.py
 dbt/adapters/duckdb/environments/local.py
 dbt/adapters/duckdb/plugins/__init__.py
 dbt/adapters/duckdb/plugins/excel.py
 dbt/adapters/duckdb/plugins/glue.py
 dbt/adapters/duckdb/plugins/gsheet.py
 dbt/adapters/duckdb/plugins/iceberg.py
+dbt/adapters/duckdb/plugins/motherduck.py
 dbt/adapters/duckdb/plugins/pd_utils.py
+dbt/adapters/duckdb/plugins/postgres.py
 dbt/adapters/duckdb/plugins/sqlalchemy.py
 dbt/include/__init__.py
 dbt/include/duckdb/__init__.py
 dbt/include/duckdb/dbt_project.yml
 dbt/include/duckdb/macros/adapters.sql
 dbt/include/duckdb/macros/catalog.sql
 dbt/include/duckdb/macros/columns.sql
```

### Comparing `dbt-duckdb-1.5.2/setup.py` & `dbt-duckdb-1.6.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -33,14 +33,26 @@
     long_description_content_type="text/markdown",
     author="Josh Wills",
     author_email="joshwills+dbt@gmail.com",
     url="https://github.com/jwills/dbt-duckdb",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
-        "dbt-core~=1.5.0",
-        "duckdb>=0.5.0",
+        "dbt-core~=1.6.0",
+        "duckdb>=0.7.0",
     ],
     extras_require={
         "glue": ["boto3", "mypy-boto3-glue"],
     },
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "License :: OSI Approved :: Apache Software License",
+        "Operating System :: Microsoft :: Windows",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: POSIX :: Linux",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+    ],
+    python_requires=">=3.8",
 )
```


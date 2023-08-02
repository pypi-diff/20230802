# Comparing `tmp/dbt-cloud-cli-0.7.6.tar.gz` & `tmp/dbt-cloud-cli-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-cloud-cli-0.7.6.tar", last modified: Mon Jul 10 10:51:10 2023, max compression
+gzip compressed data, was "dbt-cloud-cli-0.8.0.tar", last modified: Wed Aug  2 13:09:10 2023, max compression
```

## Comparing `dbt-cloud-cli-0.7.6.tar` & `dbt-cloud-cli-0.8.0.tar`

### file list

```diff
@@ -1,62 +1,65 @@
-drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-07-10 10:51:10.447767 dbt-cloud-cli-0.7.6/
--rw-r--r--   0 simo      (1000) simo      (1000)    11342 2021-12-07 10:27:17.000000 dbt-cloud-cli-0.7.6/LICENSE
--rw-r--r--   0 simo      (1000) simo      (1000)    50991 2023-07-10 10:51:10.447767 dbt-cloud-cli-0.7.6/PKG-INFO
--rw-r--r--   0 simo      (1000) simo      (1000)    50430 2023-02-09 11:57:38.000000 dbt-cloud-cli-0.7.6/README.md
-drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-07-10 10:51:10.447767 dbt-cloud-cli-0.7.6/dbt_cloud/
--rw-r--r--   0 simo      (1000) simo      (1000)       39 2022-01-12 14:59:36.000000 dbt-cloud-cli-0.7.6/dbt_cloud/__init__.py
--rw-r--r--   0 simo      (1000) simo      (1000)    12820 2023-04-13 05:30:17.000000 dbt-cloud-cli-0.7.6/dbt_cloud/cli.py
-drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-07-10 10:51:10.447767 dbt-cloud-cli-0.7.6/dbt_cloud/command/
--rw-r--r--   0 simo      (1000) simo      (1000)      715 2022-07-14 08:37:14.000000 dbt-cloud-cli-0.7.6/dbt_cloud/command/__init__.py
-drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-07-10 10:51:10.447767 dbt-cloud-cli-0.7.6/dbt_cloud/command/account/
--rw-r--r--   0 simo      (1000) simo      (1000)       88 2022-07-14 08:09:18.000000 dbt-cloud-cli-0.7.6/dbt_cloud/command/account/__init__.py
--rw-r--r--   0 simo      (1000) simo      (1000)      336 2022-07-14 08:25:40.000000 dbt-cloud-cli-0.7.6/dbt_cloud/command/account/get.py
--rw-r--r--   0 simo      (1000) simo      (1000)      407 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.6/dbt_cloud/command/account/list.py
-drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-07-10 10:51:10.447767 dbt-cloud-cli-0.7.6/dbt_cloud/command/audit_log/
--rw-r--r--   0 simo      (1000) simo      (1000)       44 2022-05-18 07:39:36.000000 dbt-cloud-cli-0.7.6/dbt_cloud/command/audit_log/__init__.py
--rw-r--r--   0 simo      (1000) simo      (1000)     1250 2022-05-18 07:39:36.000000 dbt-cloud-cli-0.7.6/dbt_cloud/command/audit_log/get.py
--rw-r--r--   0 simo      (1000) simo      (1000)     3923 2022-07-14 07:58:26.000000 dbt-cloud-cli-0.7.6/dbt_cloud/command/command.py
-drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-07-10 10:51:10.447767 dbt-cloud-cli-0.7.6/dbt_cloud/command/environment/
--rw-r--r--   0 simo      (1000) simo      (1000)       49 2022-03-25 16:24:22.000000 dbt-cloud-cli-0.7.6/dbt_cloud/command/environment/__init__.py
--rw-r--r--   0 simo      (1000) simo      (1000)      632 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.6/dbt_cloud/command/environment/list.py
-drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-07-10 10:51:10.447767 dbt-cloud-cli-0.7.6/dbt_cloud/command/job/
--rw-r--r--   0 simo      (1000) simo      (1000)      209 2022-01-27 08:25:48.000000 dbt-cloud-cli-0.7.6/dbt_cloud/command/job/__init__.py
--rw-r--r--   0 simo      (1000) simo      (1000)     3157 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.6/dbt_cloud/command/job/create.py
--rw-r--r--   0 simo      (1000) simo      (1000)      547 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.6/dbt_cloud/command/job/delete.py
--rw-r--r--   0 simo      (1000) simo      (1000)      782 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.6/dbt_cloud/command/job/get.py
--rw-r--r--   0 simo      (1000) simo      (1000)      795 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.6/dbt_cloud/command/job/list.py
--rw-r--r--   0 simo      (1000) simo      (1000)     2169 2023-01-02 09:04:34.000000 dbt-cloud-cli-0.7.6/dbt_cloud/command/job/run.py
-drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-07-10 10:51:10.447767 dbt-cloud-cli-0.7.6/dbt_cloud/command/metadata/
--rw-r--r--   0 simo      (1000) simo      (1000)       48 2022-01-12 14:59:36.000000 dbt-cloud-cli-0.7.6/dbt_cloud/command/metadata/__init__.py
--rw-r--r--   0 simo      (1000) simo      (1000)      700 2022-05-17 07:10:38.000000 dbt-cloud-cli-0.7.6/dbt_cloud/command/metadata/query.py
-drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-07-10 10:51:10.447767 dbt-cloud-cli-0.7.6/dbt_cloud/command/project/
--rw-r--r--   0 simo      (1000) simo      (1000)       88 2022-07-14 08:37:14.000000 dbt-cloud-cli-0.7.6/dbt_cloud/command/project/__init__.py
--rw-r--r--   0 simo      (1000) simo      (1000)      529 2022-07-14 08:37:14.000000 dbt-cloud-cli-0.7.6/dbt_cloud/command/project/get.py
--rw-r--r--   0 simo      (1000) simo      (1000)      429 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.6/dbt_cloud/command/project/list.py
-drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-07-10 10:51:10.447767 dbt-cloud-cli-0.7.6/dbt_cloud/command/run/
--rw-r--r--   0 simo      (1000) simo      (1000)      260 2022-03-14 13:54:59.000000 dbt-cloud-cli-0.7.6/dbt_cloud/command/run/__init__.py
--rw-r--r--   0 simo      (1000) simo      (1000)      661 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.6/dbt_cloud/command/run/cancel.py
--rw-r--r--   0 simo      (1000) simo      (1000)     1049 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.6/dbt_cloud/command/run/get.py
--rw-r--r--   0 simo      (1000) simo      (1000)     1112 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.6/dbt_cloud/command/run/get_artifact.py
--rw-r--r--   0 simo      (1000) simo      (1000)     2344 2023-02-09 11:57:38.000000 dbt-cloud-cli-0.7.6/dbt_cloud/command/run/list.py
--rw-r--r--   0 simo      (1000) simo      (1000)      859 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.7.6/dbt_cloud/command/run/list_artifacts.py
-drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-07-10 10:51:10.447767 dbt-cloud-cli-0.7.6/dbt_cloud/demo/
--rw-r--r--   0 simo      (1000) simo      (1000)       34 2022-02-09 20:32:20.000000 dbt-cloud-cli-0.7.6/dbt_cloud/demo/__init__.py
--rw-r--r--   0 simo      (1000) simo      (1000)     4886 2022-02-13 13:33:26.000000 dbt-cloud-cli-0.7.6/dbt_cloud/demo/catalog.py
--rw-r--r--   0 simo      (1000) simo      (1000)       45 2021-12-07 10:42:57.000000 dbt-cloud-cli-0.7.6/dbt_cloud/exc.py
--rw-r--r--   0 simo      (1000) simo      (1000)     1814 2023-01-02 09:04:34.000000 dbt-cloud-cli-0.7.6/dbt_cloud/field.py
--rw-r--r--   0 simo      (1000) simo      (1000)      160 2021-12-25 10:54:57.000000 dbt-cloud-cli-0.7.6/dbt_cloud/serde.py
-drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-07-10 10:51:10.447767 dbt-cloud-cli-0.7.6/dbt_cloud_cli.egg-info/
--rw-r--r--   0 simo      (1000) simo      (1000)    50991 2023-07-10 10:51:10.000000 dbt-cloud-cli-0.7.6/dbt_cloud_cli.egg-info/PKG-INFO
--rw-r--r--   0 simo      (1000) simo      (1000)     1376 2023-07-10 10:51:10.000000 dbt-cloud-cli-0.7.6/dbt_cloud_cli.egg-info/SOURCES.txt
--rw-r--r--   0 simo      (1000) simo      (1000)        1 2023-07-10 10:51:10.000000 dbt-cloud-cli-0.7.6/dbt_cloud_cli.egg-info/dependency_links.txt
--rw-r--r--   0 simo      (1000) simo      (1000)       55 2023-07-10 10:51:10.000000 dbt-cloud-cli-0.7.6/dbt_cloud_cli.egg-info/entry_points.txt
--rw-r--r--   0 simo      (1000) simo      (1000)      133 2023-07-10 10:51:10.000000 dbt-cloud-cli-0.7.6/dbt_cloud_cli.egg-info/requires.txt
--rw-r--r--   0 simo      (1000) simo      (1000)       10 2023-07-10 10:51:10.000000 dbt-cloud-cli-0.7.6/dbt_cloud_cli.egg-info/top_level.txt
--rw-r--r--   0 simo      (1000) simo      (1000)       90 2022-07-14 07:58:26.000000 dbt-cloud-cli-0.7.6/pyproject.toml
--rw-r--r--   0 simo      (1000) simo      (1000)       38 2023-07-10 10:51:10.447767 dbt-cloud-cli-0.7.6/setup.cfg
--rw-r--r--   0 simo      (1000) simo      (1000)     1071 2023-07-10 10:50:44.000000 dbt-cloud-cli-0.7.6/setup.py
-drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-07-10 10:51:10.447767 dbt-cloud-cli-0.7.6/tests/
--rw-r--r--   0 simo      (1000) simo      (1000)        0 2022-01-12 14:59:36.000000 dbt-cloud-cli-0.7.6/tests/__init__.py
--rw-r--r--   0 simo      (1000) simo      (1000)     6282 2023-02-09 11:53:22.000000 dbt-cloud-cli-0.7.6/tests/conftest.py
--rw-r--r--   0 simo      (1000) simo      (1000)      896 2022-01-12 16:57:47.000000 dbt-cloud-cli-0.7.6/tests/test_command.py
--rw-r--r--   0 simo      (1000) simo      (1000)     1229 2022-03-25 17:06:38.000000 dbt-cloud-cli-0.7.6/tests/test_job.py
+drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-08-02 13:09:10.323615 dbt-cloud-cli-0.8.0/
+-rw-r--r--   0 simo      (1000) simo      (1000)    11342 2021-12-07 10:27:17.000000 dbt-cloud-cli-0.8.0/LICENSE
+-rw-r--r--   0 simo      (1000) simo      (1000)    19514 2023-08-02 13:09:10.323615 dbt-cloud-cli-0.8.0/PKG-INFO
+-rw-r--r--   0 simo      (1000) simo      (1000)    18953 2023-08-02 12:07:22.000000 dbt-cloud-cli-0.8.0/README.md
+drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-08-02 13:09:10.323615 dbt-cloud-cli-0.8.0/dbt_cloud/
+-rw-r--r--   0 simo      (1000) simo      (1000)       39 2023-08-02 13:08:43.000000 dbt-cloud-cli-0.8.0/dbt_cloud/__init__.py
+-rw-r--r--   0 simo      (1000) simo      (1000)    13703 2023-08-02 13:08:43.000000 dbt-cloud-cli-0.8.0/dbt_cloud/cli.py
+drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-08-02 13:09:10.323615 dbt-cloud-cli-0.8.0/dbt_cloud/command/
+-rw-r--r--   0 simo      (1000) simo      (1000)      844 2023-08-02 13:08:43.000000 dbt-cloud-cli-0.8.0/dbt_cloud/command/__init__.py
+drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-08-02 13:09:10.323615 dbt-cloud-cli-0.8.0/dbt_cloud/command/account/
+-rw-r--r--   0 simo      (1000) simo      (1000)       88 2022-07-14 08:09:18.000000 dbt-cloud-cli-0.8.0/dbt_cloud/command/account/__init__.py
+-rw-r--r--   0 simo      (1000) simo      (1000)      336 2022-07-14 08:25:40.000000 dbt-cloud-cli-0.8.0/dbt_cloud/command/account/get.py
+-rw-r--r--   0 simo      (1000) simo      (1000)      407 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.8.0/dbt_cloud/command/account/list.py
+drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-08-02 13:09:10.323615 dbt-cloud-cli-0.8.0/dbt_cloud/command/audit_log/
+-rw-r--r--   0 simo      (1000) simo      (1000)       44 2022-05-18 07:39:36.000000 dbt-cloud-cli-0.8.0/dbt_cloud/command/audit_log/__init__.py
+-rw-r--r--   0 simo      (1000) simo      (1000)     1250 2022-05-18 07:39:36.000000 dbt-cloud-cli-0.8.0/dbt_cloud/command/audit_log/get.py
+-rw-r--r--   0 simo      (1000) simo      (1000)     4158 2023-08-02 13:08:43.000000 dbt-cloud-cli-0.8.0/dbt_cloud/command/command.py
+drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-08-02 13:09:10.323615 dbt-cloud-cli-0.8.0/dbt_cloud/command/environment/
+-rw-r--r--   0 simo      (1000) simo      (1000)      149 2023-08-02 11:37:57.000000 dbt-cloud-cli-0.8.0/dbt_cloud/command/environment/__init__.py
+-rw-r--r--   0 simo      (1000) simo      (1000)      607 2023-08-02 11:37:57.000000 dbt-cloud-cli-0.8.0/dbt_cloud/command/environment/delete.py
+-rw-r--r--   0 simo      (1000) simo      (1000)      708 2023-08-02 07:08:36.000000 dbt-cloud-cli-0.8.0/dbt_cloud/command/environment/get.py
+-rw-r--r--   0 simo      (1000) simo      (1000)     1031 2023-08-02 07:35:51.000000 dbt-cloud-cli-0.8.0/dbt_cloud/command/environment/list.py
+drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-08-02 13:09:10.323615 dbt-cloud-cli-0.8.0/dbt_cloud/command/job/
+-rw-r--r--   0 simo      (1000) simo      (1000)      209 2022-01-27 08:25:48.000000 dbt-cloud-cli-0.8.0/dbt_cloud/command/job/__init__.py
+-rw-r--r--   0 simo      (1000) simo      (1000)     3157 2023-08-02 08:19:15.000000 dbt-cloud-cli-0.8.0/dbt_cloud/command/job/create.py
+-rw-r--r--   0 simo      (1000) simo      (1000)      547 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.8.0/dbt_cloud/command/job/delete.py
+-rw-r--r--   0 simo      (1000) simo      (1000)      782 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.8.0/dbt_cloud/command/job/get.py
+-rw-r--r--   0 simo      (1000) simo      (1000)      795 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.8.0/dbt_cloud/command/job/list.py
+-rw-r--r--   0 simo      (1000) simo      (1000)     2169 2023-01-02 09:04:34.000000 dbt-cloud-cli-0.8.0/dbt_cloud/command/job/run.py
+drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-08-02 13:09:10.323615 dbt-cloud-cli-0.8.0/dbt_cloud/command/metadata/
+-rw-r--r--   0 simo      (1000) simo      (1000)       48 2022-01-12 14:59:36.000000 dbt-cloud-cli-0.8.0/dbt_cloud/command/metadata/__init__.py
+-rw-r--r--   0 simo      (1000) simo      (1000)      700 2022-05-17 07:10:38.000000 dbt-cloud-cli-0.8.0/dbt_cloud/command/metadata/query.py
+drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-08-02 13:09:10.323615 dbt-cloud-cli-0.8.0/dbt_cloud/command/project/
+-rw-r--r--   0 simo      (1000) simo      (1000)      137 2023-08-02 08:54:52.000000 dbt-cloud-cli-0.8.0/dbt_cloud/command/project/__init__.py
+-rw-r--r--   0 simo      (1000) simo      (1000)     1398 2023-08-02 08:23:09.000000 dbt-cloud-cli-0.8.0/dbt_cloud/command/project/create.py
+-rw-r--r--   0 simo      (1000) simo      (1000)      529 2022-07-14 08:37:14.000000 dbt-cloud-cli-0.8.0/dbt_cloud/command/project/get.py
+-rw-r--r--   0 simo      (1000) simo      (1000)      429 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.8.0/dbt_cloud/command/project/list.py
+drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-08-02 13:09:10.323615 dbt-cloud-cli-0.8.0/dbt_cloud/command/run/
+-rw-r--r--   0 simo      (1000) simo      (1000)      260 2022-03-14 13:54:59.000000 dbt-cloud-cli-0.8.0/dbt_cloud/command/run/__init__.py
+-rw-r--r--   0 simo      (1000) simo      (1000)      661 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.8.0/dbt_cloud/command/run/cancel.py
+-rw-r--r--   0 simo      (1000) simo      (1000)     1049 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.8.0/dbt_cloud/command/run/get.py
+-rw-r--r--   0 simo      (1000) simo      (1000)     1112 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.8.0/dbt_cloud/command/run/get_artifact.py
+-rw-r--r--   0 simo      (1000) simo      (1000)     2344 2023-02-09 11:57:38.000000 dbt-cloud-cli-0.8.0/dbt_cloud/command/run/list.py
+-rw-r--r--   0 simo      (1000) simo      (1000)      859 2022-04-04 14:38:37.000000 dbt-cloud-cli-0.8.0/dbt_cloud/command/run/list_artifacts.py
+drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-08-02 13:09:10.323615 dbt-cloud-cli-0.8.0/dbt_cloud/demo/
+-rw-r--r--   0 simo      (1000) simo      (1000)       34 2022-02-09 20:32:20.000000 dbt-cloud-cli-0.8.0/dbt_cloud/demo/__init__.py
+-rw-r--r--   0 simo      (1000) simo      (1000)     4886 2022-02-13 13:33:26.000000 dbt-cloud-cli-0.8.0/dbt_cloud/demo/catalog.py
+-rw-r--r--   0 simo      (1000) simo      (1000)       45 2021-12-07 10:42:57.000000 dbt-cloud-cli-0.8.0/dbt_cloud/exc.py
+-rw-r--r--   0 simo      (1000) simo      (1000)     2145 2023-08-02 08:48:48.000000 dbt-cloud-cli-0.8.0/dbt_cloud/field.py
+-rw-r--r--   0 simo      (1000) simo      (1000)      160 2021-12-25 10:54:57.000000 dbt-cloud-cli-0.8.0/dbt_cloud/serde.py
+drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-08-02 13:09:10.323615 dbt-cloud-cli-0.8.0/dbt_cloud_cli.egg-info/
+-rw-r--r--   0 simo      (1000) simo      (1000)    19514 2023-08-02 13:09:10.000000 dbt-cloud-cli-0.8.0/dbt_cloud_cli.egg-info/PKG-INFO
+-rw-r--r--   0 simo      (1000) simo      (1000)     1489 2023-08-02 13:09:10.000000 dbt-cloud-cli-0.8.0/dbt_cloud_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 simo      (1000) simo      (1000)        1 2023-08-02 13:09:10.000000 dbt-cloud-cli-0.8.0/dbt_cloud_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 simo      (1000) simo      (1000)       55 2023-08-02 13:09:10.000000 dbt-cloud-cli-0.8.0/dbt_cloud_cli.egg-info/entry_points.txt
+-rw-r--r--   0 simo      (1000) simo      (1000)      133 2023-08-02 13:09:10.000000 dbt-cloud-cli-0.8.0/dbt_cloud_cli.egg-info/requires.txt
+-rw-r--r--   0 simo      (1000) simo      (1000)       10 2023-08-02 13:09:10.000000 dbt-cloud-cli-0.8.0/dbt_cloud_cli.egg-info/top_level.txt
+-rw-r--r--   0 simo      (1000) simo      (1000)       90 2022-07-14 07:58:26.000000 dbt-cloud-cli-0.8.0/pyproject.toml
+-rw-r--r--   0 simo      (1000) simo      (1000)       38 2023-08-02 13:09:10.323615 dbt-cloud-cli-0.8.0/setup.cfg
+-rw-r--r--   0 simo      (1000) simo      (1000)     1071 2023-08-02 13:08:57.000000 dbt-cloud-cli-0.8.0/setup.py
+drwxr-xr-x   0 simo      (1000) simo      (1000)        0 2023-08-02 13:09:10.323615 dbt-cloud-cli-0.8.0/tests/
+-rw-r--r--   0 simo      (1000) simo      (1000)        0 2022-01-12 14:59:36.000000 dbt-cloud-cli-0.8.0/tests/__init__.py
+-rw-r--r--   0 simo      (1000) simo      (1000)     7554 2023-08-02 11:37:57.000000 dbt-cloud-cli-0.8.0/tests/conftest.py
+-rw-r--r--   0 simo      (1000) simo      (1000)     1878 2023-08-02 08:23:09.000000 dbt-cloud-cli-0.8.0/tests/test_command.py
+-rw-r--r--   0 simo      (1000) simo      (1000)     1229 2022-03-25 17:06:38.000000 dbt-cloud-cli-0.8.0/tests/test_job.py
```

### Comparing `dbt-cloud-cli-0.7.6/LICENSE` & `dbt-cloud-cli-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.6/dbt_cloud/cli.py` & `dbt-cloud-cli-0.8.0/dbt_cloud/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,18 @@
     DbtCloudRunGetArtifactCommand,
     DbtCloudMetadataQueryCommand,
     DbtCloudRunListCommand,
     DbtCloudRunCancelCommand,
     DbtCloudJobListCommand,
     DbtCloudProjectGetCommand,
     DbtCloudProjectListCommand,
+    DbtCloudProjectCreateCommand,
     DbtCloudEnvironmentListCommand,
+    DbtCloudEnvironmentGetCommand,
+    DbtCloudEnvironmentDeleteCommand,
     DbtCloudAccountListCommand,
     DbtCloudAccountGetCommand,
     DbtCloudAuditLogGetCommand,
 )
 from dbt_cloud.demo import data_catalog
 from dbt_cloud.serde import json_to_dict, dict_to_json
 from dbt_cloud.exc import DbtCloudException
@@ -354,21 +357,42 @@
 @project.command(help=DbtCloudProjectListCommand.get_description())
 @DbtCloudProjectListCommand.click_options
 def list(**kwargs):
     command = DbtCloudProjectListCommand.from_click_options(**kwargs)
     response = execute_and_print(command)
 
 
+@project.command(help=DbtCloudProjectCreateCommand.get_description())
+@DbtCloudProjectCreateCommand.click_options
+def create(**kwargs):
+    command = DbtCloudProjectCreateCommand.from_click_options(**kwargs)
+    response = execute_and_print(command)
+
+
 @environment.command(help=DbtCloudEnvironmentListCommand.get_description())
 @DbtCloudEnvironmentListCommand.click_options
 def list(**kwargs):
     command = DbtCloudEnvironmentListCommand.from_click_options(**kwargs)
     response = execute_and_print(command)
 
 
+@environment.command(help=DbtCloudEnvironmentGetCommand.get_description())
+@DbtCloudEnvironmentGetCommand.click_options
+def get(**kwargs):
+    command = DbtCloudEnvironmentGetCommand.from_click_options(**kwargs)
+    response = execute_and_print(command)
+
+
+@environment.command(help=DbtCloudEnvironmentDeleteCommand.get_description())
+@DbtCloudEnvironmentDeleteCommand.click_options
+def delete(**kwargs):
+    command = DbtCloudEnvironmentDeleteCommand.from_click_options(**kwargs)
+    response = execute_and_print(command)
+
+
 @account.command(help=DbtCloudAccountListCommand.get_description())
 @DbtCloudAccountListCommand.click_options
 def list(**kwargs):
     command = DbtCloudAccountListCommand.from_click_options(**kwargs)
     response = execute_and_print(command)
```

### Comparing `dbt-cloud-cli-0.7.6/dbt_cloud/command/audit_log/get.py` & `dbt-cloud-cli-0.8.0/dbt_cloud/command/audit_log/get.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.6/dbt_cloud/command/command.py` & `dbt-cloud-cli-0.8.0/dbt_cloud/command/command.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,17 +100,24 @@
     def request_headers(self) -> dict:
         return {"Authorization": f"Token {self.api_token}"}
 
     @property
     def api_url(self) -> str:
         return f"https://{self.dbt_cloud_host}/api/{self._api_version}"
 
-    def get_payload(self, exclude=["api_token", "dbt_cloud_host"]) -> dict:
+    def get_payload(
+        self, exclude=["api_token", "dbt_cloud_host"], exclude_empty: bool = False
+    ) -> dict:
         payload = self.json(exclude=set(exclude))
-        return json_to_dict(payload)
+        payload_dict = json_to_dict(payload)
+        if exclude_empty:
+            payload_dict = {
+                key: value for key, value in payload_dict.items() if value is not None
+            }
+        return payload_dict
 
 
 class DbtCloudAccountCommand(DbtCloudCommand):
     account_id: int = ACCOUNT_ID_FIELD
 
     @property
     def api_url(self) -> str:
```

### Comparing `dbt-cloud-cli-0.7.6/dbt_cloud/command/environment/list.py` & `dbt-cloud-cli-0.8.0/dbt_cloud/command/environment/get.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import requests
-from pydantic import Field, PrivateAttr
+from pydantic import PrivateAttr
 from dbt_cloud.command.command import DbtCloudAccountCommand
-from dbt_cloud.field import PROJECT_ID_FIELD
+from dbt_cloud.field import ACCOUNT_ID_FIELD, ENVIRONMENT_ID_FIELD
 
 
-class DbtCloudEnvironmentListCommand(DbtCloudAccountCommand):
-    """Retrieves environments for a given project."""
+class DbtCloudEnvironmentGetCommand(DbtCloudAccountCommand):
+    """Retrieves information about an environment in a given account."""
 
-    project_id: int = PROJECT_ID_FIELD
-    _api_version: str = PrivateAttr("v3")
+    environment_id: int = ENVIRONMENT_ID_FIELD
+    account_id: int = ACCOUNT_ID_FIELD
+    _api_version: str = PrivateAttr("v2")
 
     @property
     def api_url(self) -> str:
-        return f"{super().api_url}/projects/{self.project_id}/environments"
+        return f"{super().api_url}/environments/{self.environment_id}/"
 
     def execute(self) -> requests.Response:
         response = requests.get(url=self.api_url, headers=self.request_headers)
         return response
```

### Comparing `dbt-cloud-cli-0.7.6/dbt_cloud/command/job/create.py` & `dbt-cloud-cli-0.8.0/dbt_cloud/command/job/create.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.6/dbt_cloud/command/job/delete.py` & `dbt-cloud-cli-0.8.0/dbt_cloud/command/job/delete.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.6/dbt_cloud/command/job/get.py` & `dbt-cloud-cli-0.8.0/dbt_cloud/command/job/get.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.6/dbt_cloud/command/job/list.py` & `dbt-cloud-cli-0.8.0/dbt_cloud/command/job/list.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.6/dbt_cloud/command/job/run.py` & `dbt-cloud-cli-0.8.0/dbt_cloud/command/job/run.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.6/dbt_cloud/command/metadata/query.py` & `dbt-cloud-cli-0.8.0/dbt_cloud/command/metadata/query.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.6/dbt_cloud/command/project/get.py` & `dbt-cloud-cli-0.8.0/dbt_cloud/command/project/get.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.6/dbt_cloud/command/run/cancel.py` & `dbt-cloud-cli-0.8.0/dbt_cloud/command/run/cancel.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.6/dbt_cloud/command/run/get.py` & `dbt-cloud-cli-0.8.0/dbt_cloud/command/run/get.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.6/dbt_cloud/command/run/get_artifact.py` & `dbt-cloud-cli-0.8.0/dbt_cloud/command/run/get_artifact.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.6/dbt_cloud/command/run/list.py` & `dbt-cloud-cli-0.8.0/dbt_cloud/command/run/list.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.6/dbt_cloud/command/run/list_artifacts.py` & `dbt-cloud-cli-0.8.0/dbt_cloud/command/run/list_artifacts.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.6/dbt_cloud/demo/catalog.py` & `dbt-cloud-cli-0.8.0/dbt_cloud/demo/catalog.py`

 * *Files identical despite different names*

### Comparing `dbt-cloud-cli-0.7.6/dbt_cloud/field.py` & `dbt-cloud-cli-0.8.0/dbt_cloud/field.py`

 * *Files 16% similar despite different names*

```diff
@@ -46,7 +46,19 @@
     default_factory=lambda: get_env("DBT_CLOUD_JOB_ID"),
     description="Numeric ID of a dbt Cloud job (default: DBT_CLOUD_JOB_ID environment variable)",
 )
 RUN_ID_FIELD = Field(
     ...,
     description="Numeric ID of a dbt Cloud run",
 )
+
+LIMIT_FIELD = Field(
+    ge=0,
+    description="A limit on the number of rows to be returned. Must be a positive integer.",
+)
+OFFSET_FIELD = Field(
+    ge=0,
+    description="Offset for the returned rows. Must be a positive integer.",
+)
+DBT_VERSION_FIELD = Field(
+    description="Filter by dbt version (e.g., '1.4.0-latest')",
+)
```

### Comparing `dbt-cloud-cli-0.7.6/dbt_cloud_cli.egg-info/SOURCES.txt` & `dbt-cloud-cli-0.8.0/dbt_cloud_cli.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,27 @@
 dbt_cloud/command/command.py
 dbt_cloud/command/account/__init__.py
 dbt_cloud/command/account/get.py
 dbt_cloud/command/account/list.py
 dbt_cloud/command/audit_log/__init__.py
 dbt_cloud/command/audit_log/get.py
 dbt_cloud/command/environment/__init__.py
+dbt_cloud/command/environment/delete.py
+dbt_cloud/command/environment/get.py
 dbt_cloud/command/environment/list.py
 dbt_cloud/command/job/__init__.py
 dbt_cloud/command/job/create.py
 dbt_cloud/command/job/delete.py
 dbt_cloud/command/job/get.py
 dbt_cloud/command/job/list.py
 dbt_cloud/command/job/run.py
 dbt_cloud/command/metadata/__init__.py
 dbt_cloud/command/metadata/query.py
 dbt_cloud/command/project/__init__.py
+dbt_cloud/command/project/create.py
 dbt_cloud/command/project/get.py
 dbt_cloud/command/project/list.py
 dbt_cloud/command/run/__init__.py
 dbt_cloud/command/run/cancel.py
 dbt_cloud/command/run/get.py
 dbt_cloud/command/run/get_artifact.py
 dbt_cloud/command/run/list.py
```

### Comparing `dbt-cloud-cli-0.7.6/setup.py` & `dbt-cloud-cli-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 
 README = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name="dbt-cloud-cli",
-    version="0.7.6",
+    version="0.8.0",
     description="dbt Cloud command line interface (CLI)",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/data-mie/dbt-cloud-cli",
     author="Simo Tumelius",
     author_email="simo@datamie.fi",
     license="Apache Software License",
```

### Comparing `dbt-cloud-cli-0.7.6/tests/conftest.py` & `dbt-cloud-cli-0.8.0/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,52 @@
 import json
 import pytest
+import os
 from pathlib import Path
 from dbt_cloud.command import (
     DbtCloudJobCreateCommand,
     DbtCloudJobDeleteCommand,
     DbtCloudJobGetCommand,
     DbtCloudJobListCommand,
     DbtCloudJobRunCommand,
     DbtCloudProjectGetCommand,
     DbtCloudProjectListCommand,
+    DbtCloudProjectCreateCommand,
     DbtCloudRunCancelCommand,
     DbtCloudRunGetArtifactCommand,
     DbtCloudRunGetCommand,
     DbtCloudRunListArtifactsCommand,
     DbtCloudRunListCommand,
     DbtCloudEnvironmentListCommand,
+    DbtCloudEnvironmentGetCommand,
+    DbtCloudEnvironmentDeleteCommand,
     DbtCloudAccountListCommand,
     DbtCloudAccountGetCommand,
     DbtCloudAuditLogGetCommand,
 )
 
 
 API_TOKEN = "foo"
 ACCOUNT_ID = 123456
 PROJECT_ID = 123457
 ENVIRONMENT_ID = 49819
 JOB_ID = 43167
 RUN_ID = 36053848
 
 
+@pytest.fixture
+def account_id():
+    return int(os.environ.get("DBT_CLOUD_ACCOUNT_ID", ACCOUNT_ID))
+
+
+@pytest.fixture
+def environment_id():
+    return int(os.environ.get("DBT_CLOUD_ENVIRONMENT_ID", ENVIRONMENT_ID))
+
+
 def load_response(response_name):
     shared_datadir = Path(__file__).parent / "data"
     response_file = shared_datadir / f"{response_name}.json"
     response_json = response_file.read_text()
     return json.loads(response_json)
 
 
@@ -147,23 +161,53 @@
         "project_list",
         DbtCloudProjectListCommand(api_token=API_TOKEN, account_id=ACCOUNT_ID),
         load_response("project_list_response"),
         "get",
         marks=pytest.mark.project,
     ),
     pytest.param(
+        "project_create",
+        DbtCloudProjectCreateCommand(
+            api_token=API_TOKEN,
+            account_id=ACCOUNT_ID,
+            name="My test project",
+            dbt_project_subdirectory="dbt/",
+        ),
+        load_response("project_get_response"),
+        "post",
+        marks=pytest.mark.project,
+    ),
+    pytest.param(
         "environment_list",
         DbtCloudEnvironmentListCommand(
             api_token=API_TOKEN, account_id=ACCOUNT_ID, project_id=PROJECT_ID
         ),
         load_response("environment_list_response"),
         "get",
         marks=pytest.mark.environment,
     ),
     pytest.param(
+        "environment_get",
+        DbtCloudEnvironmentGetCommand(
+            api_token=API_TOKEN, account_id=ACCOUNT_ID, environment_id=ENVIRONMENT_ID
+        ),
+        load_response("environment_get_response"),
+        "get",
+        marks=pytest.mark.environment,
+    ),
+    pytest.param(
+        "environment_delete",
+        DbtCloudEnvironmentDeleteCommand(
+            api_token=API_TOKEN, account_id=ACCOUNT_ID, environment_id=222062
+        ),
+        load_response("environment_delete_response"),
+        "delete",
+        marks=pytest.mark.environment,
+    ),
+    pytest.param(
         "account_list",
         DbtCloudAccountListCommand(api_token=API_TOKEN),
         load_response("account_list_response"),
         "get",
         marks=pytest.mark.account,
     ),
     pytest.param(
```

### Comparing `dbt-cloud-cli-0.7.6/tests/test_job.py` & `dbt-cloud-cli-0.8.0/tests/test_job.py`

 * *Files identical despite different names*


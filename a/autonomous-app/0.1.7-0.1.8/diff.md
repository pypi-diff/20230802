# Comparing `tmp/autonomous-app-0.1.7.tar.gz` & `tmp/autonomous-app-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autonomous-app-0.1.7.tar", last modified: Fri Jul 28 15:59:43 2023, max compression
+gzip compressed data, was "autonomous-app-0.1.8.tar", last modified: Wed Aug  2 17:38:23 2023, max compression
```

## Comparing `autonomous-app-0.1.7.tar` & `autonomous-app-0.1.8.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.880172 autonomous-app-0.1.7/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1076 2023-03-07 12:36:40.000000 autonomous-app-0.1.7/LICENSE
--rw-r--r--   0 samoore   (1000) samoore   (1000)     3809 2023-07-28 15:59:43.880172 autonomous-app-0.1.7/PKG-INFO
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2011 2023-06-20 21:09:23.000000 autonomous-app-0.1.7/README.md
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1469 2023-07-20 14:57:42.000000 autonomous-app-0.1.7/pyproject.toml
--rw-r--r--   0 samoore   (1000) samoore   (1000)      523 2023-07-27 14:43:37.000000 autonomous-app-0.1.7/requirements.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-07-28 15:59:43.880172 autonomous-app-0.1.7/setup.cfg
--rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-04-04 14:14:59.000000 autonomous-app-0.1.7/setup.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.875172 autonomous-app-0.1.7/src/
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.876172 autonomous-app-0.1.7/src/autonomous/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       86 2023-07-28 15:57:58.000000 autonomous-app-0.1.7/src/autonomous/__init__.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.876172 autonomous-app-0.1.7/src/autonomous/apis/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       27 2023-06-20 19:34:19.000000 autonomous-app-0.1.7/src/autonomous/apis/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2149 2023-07-07 13:12:31.000000 autonomous-app-0.1.7/src/autonomous/apis/openai.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.876172 autonomous-app-0.1.7/src/autonomous/apis/version_control/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1069 2023-03-07 16:24:11.000000 autonomous-app-0.1.7/src/autonomous/apis/version_control/GHCallbacks.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1155 2023-03-07 21:09:26.000000 autonomous-app-0.1.7/src/autonomous/apis/version_control/GHOrganization.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     4622 2023-03-07 16:24:11.000000 autonomous-app-0.1.7/src/autonomous/apis/version_control/GHRepo.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      196 2023-03-07 16:24:11.000000 autonomous-app-0.1.7/src/autonomous/apis/version_control/GHVersionControl.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      117 2023-03-07 16:24:11.000000 autonomous-app-0.1.7/src/autonomous/apis/version_control/__init__.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.875172 autonomous-app-0.1.7/src/autonomous/app_template/
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.877172 autonomous-app-0.1.7/src/autonomous/app_template/app/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       54 2023-07-28 15:13:30.000000 autonomous-app-0.1.7/src/autonomous/app_template/app/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1598 2023-07-27 16:48:05.000000 autonomous-app-0.1.7/src/autonomous/app_template/app/app.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1316 2023-07-27 17:51:13.000000 autonomous-app-0.1.7/src/autonomous/app_template/app/config.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.877172 autonomous-app-0.1.7/src/autonomous/app_template/app/models/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-04-04 14:32:12.000000 autonomous-app-0.1.7/src/autonomous/app_template/app/models/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      203 2023-04-04 15:41:08.000000 autonomous-app-0.1.7/src/autonomous/app_template/app/models/model.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      517 2023-07-28 15:15:34.000000 autonomous-app-0.1.7/src/autonomous/app_template/app/tasks.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.877172 autonomous-app-0.1.7/src/autonomous/app_template/app/views/
--rwxr-xr-x   0 samoore   (1000) samoore   (1000)      589 2023-04-04 14:32:12.000000 autonomous-app-0.1.7/src/autonomous/app_template/app/views/admin.py
--rwxr-xr-x   0 samoore   (1000) samoore   (1000)      589 2023-04-28 17:48:57.000000 autonomous-app-0.1.7/src/autonomous/app_template/app/views/index.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.878172 autonomous-app-0.1.7/src/autonomous/app_template/tests/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-04-04 14:32:12.000000 autonomous-app-0.1.7/src/autonomous/app_template/tests/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      545 2023-07-28 15:11:47.000000 autonomous-app-0.1.7/src/autonomous/app_template/tests/conftest.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      204 2023-04-04 18:40:47.000000 autonomous-app-0.1.7/src/autonomous/app_template/tests/test_app.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1021 2023-07-28 15:54:14.000000 autonomous-app-0.1.7/src/autonomous/app_template/tests/test_tasks.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.878172 autonomous-app-0.1.7/src/autonomous/app_template/vendor/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1124 2023-04-13 17:57:17.000000 autonomous-app-0.1.7/src/autonomous/app_template/vendor/gunicorn.conf.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2252 2023-06-08 19:19:57.000000 autonomous-app-0.1.7/src/autonomous/assets.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)       42 2023-04-04 14:14:59.000000 autonomous-app-0.1.7/src/autonomous/cli.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.878172 autonomous-app-0.1.7/src/autonomous/db/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       94 2023-07-07 12:00:23.000000 autonomous-app-0.1.7/src/autonomous/db/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      812 2023-07-07 12:05:15.000000 autonomous-app-0.1.7/src/autonomous/db/autodb.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      531 2023-04-04 14:14:59.000000 autonomous-app-0.1.7/src/autonomous/db/storage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2521 2023-06-20 21:17:55.000000 autonomous-app-0.1.7/src/autonomous/db/table.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1245 2023-06-01 20:06:24.000000 autonomous-app-0.1.7/src/autonomous/logger.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.879172 autonomous-app-0.1.7/src/autonomous/model/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-04-02 18:01:05.000000 autonomous-app-0.1.7/src/autonomous/model/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     4035 2023-07-20 15:46:58.000000 autonomous-app-0.1.7/src/autonomous/model/automodel.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      650 2023-06-13 18:03:23.000000 autonomous-app-0.1.7/src/autonomous/model/orm.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.879172 autonomous-app-0.1.7/src/autonomous/storage/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       88 2023-06-13 18:11:53.000000 autonomous-app-0.1.7/src/autonomous/storage/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      447 2023-06-05 17:49:27.000000 autonomous-app-0.1.7/src/autonomous/storage/basestorage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1620 2023-07-07 13:13:20.000000 autonomous-app-0.1.7/src/autonomous/storage/cloudinarystorage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      156 2023-06-13 18:11:43.000000 autonomous-app-0.1.7/src/autonomous/storage/localstorage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1381 2023-06-13 18:12:16.000000 autonomous-app-0.1.7/src/autonomous/storage/s3storage.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.879172 autonomous-app-0.1.7/src/autonomous/tasks/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       34 2023-07-27 15:55:55.000000 autonomous-app-0.1.7/src/autonomous/tasks/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      615 2023-07-28 14:38:22.000000 autonomous-app-0.1.7/src/autonomous/tasks/task.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.880172 autonomous-app-0.1.7/src/autonomous_app.egg-info/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     3809 2023-07-28 15:59:43.000000 autonomous-app-0.1.7/src/autonomous_app.egg-info/PKG-INFO
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1788 2023-07-28 15:59:43.000000 autonomous-app-0.1.7/src/autonomous_app.egg-info/SOURCES.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-07-28 15:59:43.000000 autonomous-app-0.1.7/src/autonomous_app.egg-info/dependency_links.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)       53 2023-07-28 15:59:43.000000 autonomous-app-0.1.7/src/autonomous_app.egg-info/entry_points.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)      162 2023-07-28 15:59:43.000000 autonomous-app-0.1.7/src/autonomous_app.egg-info/requires.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)       11 2023-07-28 15:59:43.000000 autonomous-app-0.1.7/src/autonomous_app.egg-info/top_level.txt
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.899062 autonomous-app-0.1.8/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1076 2023-03-07 12:36:40.000000 autonomous-app-0.1.8/LICENSE
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     3809 2023-08-02 17:38:23.898062 autonomous-app-0.1.8/PKG-INFO
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     2011 2023-06-20 21:09:23.000000 autonomous-app-0.1.8/README.md
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1469 2023-07-20 14:57:42.000000 autonomous-app-0.1.8/pyproject.toml
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      523 2023-07-27 14:43:37.000000 autonomous-app-0.1.8/requirements.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-08-02 17:38:23.900061 autonomous-app-0.1.8/setup.cfg
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-04-04 14:14:59.000000 autonomous-app-0.1.8/setup.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.891062 autonomous-app-0.1.8/src/
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.893061 autonomous-app-0.1.8/src/autonomous/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       86 2023-08-02 17:38:13.000000 autonomous-app-0.1.8/src/autonomous/__init__.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.893061 autonomous-app-0.1.8/src/autonomous/apis/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       27 2023-06-20 19:34:19.000000 autonomous-app-0.1.8/src/autonomous/apis/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     2149 2023-07-07 13:12:31.000000 autonomous-app-0.1.8/src/autonomous/apis/openai.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.894062 autonomous-app-0.1.8/src/autonomous/apis/version_control/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1069 2023-03-07 16:24:11.000000 autonomous-app-0.1.8/src/autonomous/apis/version_control/GHCallbacks.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1155 2023-03-07 21:09:26.000000 autonomous-app-0.1.8/src/autonomous/apis/version_control/GHOrganization.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     4622 2023-03-07 16:24:11.000000 autonomous-app-0.1.8/src/autonomous/apis/version_control/GHRepo.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      196 2023-03-07 16:24:11.000000 autonomous-app-0.1.8/src/autonomous/apis/version_control/GHVersionControl.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      117 2023-03-07 16:24:11.000000 autonomous-app-0.1.8/src/autonomous/apis/version_control/__init__.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.890062 autonomous-app-0.1.8/src/autonomous/app_template/
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.894062 autonomous-app-0.1.8/src/autonomous/app_template/app/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       54 2023-07-28 15:13:30.000000 autonomous-app-0.1.8/src/autonomous/app_template/app/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1598 2023-07-27 16:48:05.000000 autonomous-app-0.1.8/src/autonomous/app_template/app/app.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1316 2023-07-27 17:51:13.000000 autonomous-app-0.1.8/src/autonomous/app_template/app/config.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.894062 autonomous-app-0.1.8/src/autonomous/app_template/app/models/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-04-04 14:32:12.000000 autonomous-app-0.1.8/src/autonomous/app_template/app/models/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      203 2023-04-04 15:41:08.000000 autonomous-app-0.1.8/src/autonomous/app_template/app/models/model.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      517 2023-07-28 15:15:34.000000 autonomous-app-0.1.8/src/autonomous/app_template/app/tasks.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.894062 autonomous-app-0.1.8/src/autonomous/app_template/app/views/
+-rwxr-xr-x   0 samoore   (1000) samoore   (1000)      589 2023-04-04 14:32:12.000000 autonomous-app-0.1.8/src/autonomous/app_template/app/views/admin.py
+-rwxr-xr-x   0 samoore   (1000) samoore   (1000)      589 2023-04-28 17:48:57.000000 autonomous-app-0.1.8/src/autonomous/app_template/app/views/index.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.895062 autonomous-app-0.1.8/src/autonomous/app_template/tests/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-04-04 14:32:12.000000 autonomous-app-0.1.8/src/autonomous/app_template/tests/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      545 2023-07-28 15:11:47.000000 autonomous-app-0.1.8/src/autonomous/app_template/tests/conftest.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      432 2023-08-02 17:36:52.000000 autonomous-app-0.1.8/src/autonomous/app_template/tests/test_app.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1021 2023-07-28 15:54:14.000000 autonomous-app-0.1.8/src/autonomous/app_template/tests/test_tasks.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.895062 autonomous-app-0.1.8/src/autonomous/app_template/vendor/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1124 2023-04-13 17:57:17.000000 autonomous-app-0.1.8/src/autonomous/app_template/vendor/gunicorn.conf.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     2252 2023-06-08 19:19:57.000000 autonomous-app-0.1.8/src/autonomous/assets.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       42 2023-04-04 14:14:59.000000 autonomous-app-0.1.8/src/autonomous/cli.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.895062 autonomous-app-0.1.8/src/autonomous/db/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       94 2023-07-07 12:00:23.000000 autonomous-app-0.1.8/src/autonomous/db/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      812 2023-07-07 12:05:15.000000 autonomous-app-0.1.8/src/autonomous/db/autodb.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      531 2023-04-04 14:14:59.000000 autonomous-app-0.1.8/src/autonomous/db/storage.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     2521 2023-06-20 21:17:55.000000 autonomous-app-0.1.8/src/autonomous/db/table.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1245 2023-06-01 20:06:24.000000 autonomous-app-0.1.8/src/autonomous/logger.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.896062 autonomous-app-0.1.8/src/autonomous/model/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-04-02 18:01:05.000000 autonomous-app-0.1.8/src/autonomous/model/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     4159 2023-08-02 16:53:49.000000 autonomous-app-0.1.8/src/autonomous/model/automodel.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      683 2023-08-02 17:35:38.000000 autonomous-app-0.1.8/src/autonomous/model/orm.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.896062 autonomous-app-0.1.8/src/autonomous/storage/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       88 2023-06-13 18:11:53.000000 autonomous-app-0.1.8/src/autonomous/storage/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      447 2023-06-05 17:49:27.000000 autonomous-app-0.1.8/src/autonomous/storage/basestorage.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1620 2023-07-07 13:13:20.000000 autonomous-app-0.1.8/src/autonomous/storage/cloudinarystorage.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      156 2023-06-13 18:11:43.000000 autonomous-app-0.1.8/src/autonomous/storage/localstorage.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1381 2023-06-13 18:12:16.000000 autonomous-app-0.1.8/src/autonomous/storage/s3storage.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.896062 autonomous-app-0.1.8/src/autonomous/tasks/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       34 2023-07-27 15:55:55.000000 autonomous-app-0.1.8/src/autonomous/tasks/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      615 2023-07-28 14:38:22.000000 autonomous-app-0.1.8/src/autonomous/tasks/task.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.898062 autonomous-app-0.1.8/src/autonomous_app.egg-info/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     3809 2023-08-02 17:38:23.000000 autonomous-app-0.1.8/src/autonomous_app.egg-info/PKG-INFO
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1788 2023-08-02 17:38:23.000000 autonomous-app-0.1.8/src/autonomous_app.egg-info/SOURCES.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-08-02 17:38:23.000000 autonomous-app-0.1.8/src/autonomous_app.egg-info/dependency_links.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       53 2023-08-02 17:38:23.000000 autonomous-app-0.1.8/src/autonomous_app.egg-info/entry_points.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      162 2023-08-02 17:38:23.000000 autonomous-app-0.1.8/src/autonomous_app.egg-info/requires.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       11 2023-08-02 17:38:23.000000 autonomous-app-0.1.8/src/autonomous_app.egg-info/top_level.txt
```

### Comparing `autonomous-app-0.1.7/LICENSE` & `autonomous-app-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.7/PKG-INFO` & `autonomous-app-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomous-app
-Version: 0.1.7
+Version: 0.1.8
 Summary: Containerized application framework built on Flask with additional libraries and tools for rapid development of web applications.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autonomous-app-0.1.7/README.md` & `autonomous-app-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.7/pyproject.toml` & `autonomous-app-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.7/requirements.txt` & `autonomous-app-0.1.8/requirements.txt`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.7/src/autonomous/apis/openai.py` & `autonomous-app-0.1.8/src/autonomous/apis/openai.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.7/src/autonomous/apis/version_control/GHCallbacks.py` & `autonomous-app-0.1.8/src/autonomous/apis/version_control/GHCallbacks.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.7/src/autonomous/apis/version_control/GHOrganization.py` & `autonomous-app-0.1.8/src/autonomous/apis/version_control/GHOrganization.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.7/src/autonomous/apis/version_control/GHRepo.py` & `autonomous-app-0.1.8/src/autonomous/apis/version_control/GHRepo.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.7/src/autonomous/app_template/app/app.py` & `autonomous-app-0.1.8/src/autonomous/app_template/app/app.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.7/src/autonomous/app_template/app/config.py` & `autonomous-app-0.1.8/src/autonomous/app_template/app/config.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.7/src/autonomous/app_template/app/tasks.py` & `autonomous-app-0.1.8/src/autonomous/app_template/app/tasks.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.7/src/autonomous/app_template/app/views/admin.py` & `autonomous-app-0.1.8/src/autonomous/app_template/app/views/admin.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.7/src/autonomous/app_template/app/views/index.py` & `autonomous-app-0.1.8/src/autonomous/app_template/app/views/index.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.7/src/autonomous/app_template/tests/conftest.py` & `autonomous-app-0.1.8/src/autonomous/app_template/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.7/src/autonomous/app_template/tests/test_tasks.py` & `autonomous-app-0.1.8/src/autonomous/app_template/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.7/src/autonomous/app_template/vendor/gunicorn.conf.py` & `autonomous-app-0.1.8/src/autonomous/app_template/vendor/gunicorn.conf.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.7/src/autonomous/assets.py` & `autonomous-app-0.1.8/src/autonomous/assets.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.7/src/autonomous/db/autodb.py` & `autonomous-app-0.1.8/src/autonomous/db/autodb.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.7/src/autonomous/db/storage.py` & `autonomous-app-0.1.8/src/autonomous/db/storage.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.7/src/autonomous/db/table.py` & `autonomous-app-0.1.8/src/autonomous/db/table.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.7/src/autonomous/logger.py` & `autonomous-app-0.1.8/src/autonomous/logger.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.7/src/autonomous/model/automodel.py` & `autonomous-app-0.1.8/src/autonomous/model/automodel.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from autonomous import log
 
 from .orm import ORM
 
 
 class AutoModel(ABC):
     _table = None
+    _table_name = ""
     _orm = ORM
     attributes = {}
 
     def __new__(cls, *args, **kwargs):
         obj = super().__new__(cls)
 
         # set default attributes
@@ -31,15 +32,17 @@
         return obj
 
     @classmethod
     def table(cls):
         """The ORM table for this model"""
 
         if not cls._table:
-            cls._table = cls._orm(table=cls.__name__)
+            table_name = cls._table_name or cls.__name__
+            log(f"Creating table {table_name}")
+            cls._table = cls._orm(table=table_name)
         return cls._table
 
     @classmethod
     def model_name(cls):
         """The fully qualified name of this model"""
         return f"{cls.__module__}.{cls.__name__}"
```

### Comparing `autonomous-app-0.1.7/src/autonomous/model/orm.py` & `autonomous-app-0.1.8/src/autonomous/model/orm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from ..db import db as _database
 
 
 class ORM:
     def __init__(self, table):
+        self._table_name = table
         self._table = _database.get_table(table=table)
 
     @property
     def table(self):
         return self._table
 
     def save(self, data):
```

### Comparing `autonomous-app-0.1.7/src/autonomous/storage/cloudinarystorage.py` & `autonomous-app-0.1.8/src/autonomous/storage/cloudinarystorage.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.7/src/autonomous/storage/s3storage.py` & `autonomous-app-0.1.8/src/autonomous/storage/s3storage.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.7/src/autonomous/tasks/task.py` & `autonomous-app-0.1.8/src/autonomous/tasks/task.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.7/src/autonomous_app.egg-info/PKG-INFO` & `autonomous-app-0.1.8/src/autonomous_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomous-app
-Version: 0.1.7
+Version: 0.1.8
 Summary: Containerized application framework built on Flask with additional libraries and tools for rapid development of web applications.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autonomous-app-0.1.7/src/autonomous_app.egg-info/SOURCES.txt` & `autonomous-app-0.1.8/src/autonomous_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*


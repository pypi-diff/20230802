# Comparing `tmp/datagrowth-0.18.2.tar.gz` & `tmp/datagrowth-0.19.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datagrowth-0.18.2.tar", last modified: Mon Nov 14 14:39:59 2022, max compression
+gzip compressed data, was "datagrowth-0.19.0.tar", last modified: Wed Aug  2 12:34:29 2023, max compression
```

## Comparing `datagrowth-0.18.2.tar` & `datagrowth-0.19.0.tar`

### file list

```diff
@@ -1,94 +1,97 @@
-drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2022-11-14 14:39:59.417041 datagrowth-0.18.2/
--rw-rw-r--   0 fako      (1000) fako      (1000)     7652 2020-10-07 14:48:05.000000 datagrowth-0.18.2/LICENSE
--rw-rw-r--   0 fako      (1000) fako      (1000)     2598 2022-11-14 14:39:59.417041 datagrowth-0.18.2/PKG-INFO
--rw-rw-r--   0 fako      (1000) fako      (1000)     1554 2022-03-17 14:21:12.000000 datagrowth-0.18.2/README.md
-drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2022-11-14 14:39:59.409041 datagrowth-0.18.2/datagrowth/
--rw-rw-r--   0 fako      (1000) fako      (1000)       56 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/__init__.py
--rw-rw-r--   0 fako      (1000) fako      (1000)      274 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/admin.py
--rw-rw-r--   0 fako      (1000) fako      (1000)     1176 2021-04-13 09:25:44.000000 datagrowth-0.18.2/datagrowth/apps.py
-drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2022-11-14 14:39:59.413041 datagrowth-0.18.2/datagrowth/configuration/
--rw-rw-r--   0 fako      (1000) fako      (1000)      373 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/configuration/__init__.py
--rw-rw-r--   0 fako      (1000) fako      (1000)      159 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/configuration/configs.py
--rw-rw-r--   0 fako      (1000) fako      (1000)     4126 2021-04-13 09:52:52.000000 datagrowth-0.18.2/datagrowth/configuration/fields.py
--rw-rw-r--   0 fako      (1000) fako      (1000)     2601 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/configuration/serializers.py
--rw-rw-r--   0 fako      (1000) fako      (1000)    15989 2021-05-10 11:35:16.000000 datagrowth-0.18.2/datagrowth/configuration/types.py
-drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2022-11-14 14:39:59.413041 datagrowth-0.18.2/datagrowth/datatypes/
--rw-rw-r--   0 fako      (1000) fako      (1000)      204 2022-11-13 17:31:35.000000 datagrowth-0.18.2/datagrowth/datatypes/__init__.py
--rw-rw-r--   0 fako      (1000) fako      (1000)      108 2021-05-10 11:35:16.000000 datagrowth-0.18.2/datagrowth/datatypes/admin.py
-drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2022-11-14 14:39:59.413041 datagrowth-0.18.2/datagrowth/datatypes/annotations/
--rw-rw-r--   0 fako      (1000) fako      (1000)        0 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/datatypes/annotations/__init__.py
--rw-rw-r--   0 fako      (1000) fako      (1000)      213 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/datatypes/annotations/admin.py
--rw-rw-r--   0 fako      (1000) fako      (1000)      754 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/datatypes/annotations/base.py
--rw-rw-r--   0 fako      (1000) fako      (1000)     3357 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/datatypes/annotations/views.py
-drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2022-11-14 14:39:59.413041 datagrowth-0.18.2/datagrowth/datatypes/datasets/
--rw-rw-r--   0 fako      (1000) fako      (1000)        0 2021-05-10 11:35:16.000000 datagrowth-0.18.2/datagrowth/datatypes/datasets/__init__.py
-drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2022-11-14 14:39:59.413041 datagrowth-0.18.2/datagrowth/datatypes/documents/
--rw-rw-r--   0 fako      (1000) fako      (1000)        0 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/datatypes/documents/__init__.py
--rw-rw-r--   0 fako      (1000) fako      (1000)      213 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/datatypes/documents/admin.py
-drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2022-11-14 14:39:59.413041 datagrowth-0.18.2/datagrowth/datatypes/documents/db/
--rw-rw-r--   0 fako      (1000) fako      (1000)        0 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/datatypes/documents/db/__init__.py
--rw-rw-r--   0 fako      (1000) fako      (1000)     1087 2022-11-13 17:31:35.000000 datagrowth-0.18.2/datagrowth/datatypes/documents/db/base.py
--rw-rw-r--   0 fako      (1000) fako      (1000)    11193 2022-11-13 17:31:35.000000 datagrowth-0.18.2/datagrowth/datatypes/documents/db/collection.py
--rw-rw-r--   0 fako      (1000) fako      (1000)     5352 2021-05-10 11:35:16.000000 datagrowth-0.18.2/datagrowth/datatypes/documents/db/document.py
-drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2022-11-14 14:39:59.413041 datagrowth-0.18.2/datagrowth/datatypes/documents/views/
--rw-rw-r--   0 fako      (1000) fako      (1000)        0 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/datatypes/documents/views/__init__.py
--rw-rw-r--   0 fako      (1000) fako      (1000)     1096 2021-05-10 11:35:16.000000 datagrowth-0.18.2/datagrowth/datatypes/documents/views/collection.py
--rw-rw-r--   0 fako      (1000) fako      (1000)     1919 2021-05-10 11:35:16.000000 datagrowth-0.18.2/datagrowth/datatypes/documents/views/content.py
--rw-rw-r--   0 fako      (1000) fako      (1000)      327 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/datatypes/documents/views/document.py
--rw-rw-r--   0 fako      (1000) fako      (1000)      316 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/datatypes/views.py
--rw-rw-r--   0 fako      (1000) fako      (1000)      709 2022-11-13 17:31:35.000000 datagrowth-0.18.2/datagrowth/exceptions.py
-drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2022-11-14 14:39:59.413041 datagrowth-0.18.2/datagrowth/management/
--rw-rw-r--   0 fako      (1000) fako      (1000)        0 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/management/__init__.py
--rw-rw-r--   0 fako      (1000) fako      (1000)     1876 2022-11-13 17:06:04.000000 datagrowth-0.18.2/datagrowth/management/base.py
-drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2022-11-14 14:39:59.413041 datagrowth-0.18.2/datagrowth/management/commands/
--rw-rw-r--   0 fako      (1000) fako      (1000)        0 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/management/commands/__init__.py
--rw-rw-r--   0 fako      (1000) fako      (1000)      854 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/management/commands/dump_dataset.py
--rw-rw-r--   0 fako      (1000) fako      (1000)      699 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/management/commands/dump_resource.py
--rw-rw-r--   0 fako      (1000) fako      (1000)      689 2021-04-25 07:49:49.000000 datagrowth-0.18.2/datagrowth/management/commands/grow_dataset.py
--rw-rw-r--   0 fako      (1000) fako      (1000)     3838 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/management/commands/load_dataset.py
--rw-rw-r--   0 fako      (1000) fako      (1000)      864 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/management/commands/load_resource.py
--rw-rw-r--   0 fako      (1000) fako      (1000)     1391 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/management/commands/migrate_absolute_media_paths.py
-drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2022-11-14 14:39:59.417041 datagrowth-0.18.2/datagrowth/processors/
--rw-rw-r--   0 fako      (1000) fako      (1000)       64 2022-11-13 17:31:35.000000 datagrowth-0.18.2/datagrowth/processors/__init__.py
--rw-rw-r--   0 fako      (1000) fako      (1000)     3116 2021-05-10 11:35:16.000000 datagrowth-0.18.2/datagrowth/processors/base.py
-drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2022-11-14 14:39:59.417041 datagrowth-0.18.2/datagrowth/processors/input/
--rw-rw-r--   0 fako      (1000) fako      (1000)       41 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/processors/input/__init__.py
--rw-rw-r--   0 fako      (1000) fako      (1000)     7699 2022-03-27 08:59:22.000000 datagrowth-0.18.2/datagrowth/processors/input/extraction.py
-drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2022-11-14 14:39:59.417041 datagrowth-0.18.2/datagrowth/resources/
--rw-rw-r--   0 fako      (1000) fako      (1000)      239 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/resources/__init__.py
--rw-rw-r--   0 fako      (1000) fako      (1000)       86 2021-05-10 11:35:16.000000 datagrowth-0.18.2/datagrowth/resources/admin.py
--rw-rw-r--   0 fako      (1000) fako      (1000)     5259 2022-11-13 17:31:35.000000 datagrowth-0.18.2/datagrowth/resources/base.py
-drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2022-11-14 14:39:59.417041 datagrowth-0.18.2/datagrowth/resources/http/
--rw-rw-r--   0 fako      (1000) fako      (1000)      154 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/resources/http/__init__.py
--rw-rw-r--   0 fako      (1000) fako      (1000)      220 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/resources/http/admin.py
--rw-rw-r--   0 fako      (1000) fako      (1000)     7451 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/resources/http/files.py
--rw-rw-r--   0 fako      (1000) fako      (1000)    29480 2022-11-14 14:33:37.000000 datagrowth-0.18.2/datagrowth/resources/http/generic.py
--rw-rw-r--   0 fako      (1000) fako      (1000)     5150 2021-05-10 11:35:16.000000 datagrowth-0.18.2/datagrowth/resources/http/tasks.py
-drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2022-11-14 14:39:59.417041 datagrowth-0.18.2/datagrowth/resources/shell/
--rw-rw-r--   0 fako      (1000) fako      (1000)      157 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/resources/shell/__init__.py
--rw-rw-r--   0 fako      (1000) fako      (1000)      235 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/resources/shell/admin.py
-drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2022-11-14 14:39:59.417041 datagrowth-0.18.2/datagrowth/resources/shell/apache/
--rw-rw-r--   0 fako      (1000) fako      (1000)        0 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/resources/shell/apache/__init__.py
--rw-rw-r--   0 fako      (1000) fako      (1000)     2815 2021-04-13 09:25:44.000000 datagrowth-0.18.2/datagrowth/resources/shell/apache/tika.py
--rw-rw-r--   0 fako      (1000) fako      (1000)    13978 2022-10-27 16:01:06.000000 datagrowth-0.18.2/datagrowth/resources/shell/generic.py
-drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2022-11-14 14:39:59.417041 datagrowth-0.18.2/datagrowth/resources/shell/kaldi/
--rw-rw-r--   0 fako      (1000) fako      (1000)        0 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/resources/shell/kaldi/__init__.py
--rw-rw-r--   0 fako      (1000) fako      (1000)     1683 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/resources/shell/kaldi/aspire.py
--rw-rw-r--   0 fako      (1000) fako      (1000)     1912 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/resources/shell/kaldi/nl.py
--rw-rw-r--   0 fako      (1000) fako      (1000)     1161 2022-03-17 14:21:12.000000 datagrowth-0.18.2/datagrowth/resources/shell/tasks.py
--rw-rw-r--   0 fako      (1000) fako      (1000)     3438 2022-11-13 17:31:35.000000 datagrowth-0.18.2/datagrowth/settings.py
-drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2022-11-14 14:39:59.417041 datagrowth-0.18.2/datagrowth/utils/
--rw-rw-r--   0 fako      (1000) fako      (1000)      264 2021-04-13 09:25:44.000000 datagrowth-0.18.2/datagrowth/utils/__init__.py
--rw-rw-r--   0 fako      (1000) fako      (1000)     2789 2021-04-13 09:25:44.000000 datagrowth-0.18.2/datagrowth/utils/data.py
--rw-rw-r--   0 fako      (1000) fako      (1000)     1029 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/utils/datetime.py
--rw-rw-r--   0 fako      (1000) fako      (1000)     2909 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/utils/io.py
--rw-rw-r--   0 fako      (1000) fako      (1000)     1326 2020-10-07 14:48:05.000000 datagrowth-0.18.2/datagrowth/utils/iterators.py
--rw-rw-r--   0 fako      (1000) fako      (1000)      198 2022-11-14 14:35:45.000000 datagrowth-0.18.2/datagrowth/version.py
-drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2022-11-14 14:39:59.409041 datagrowth-0.18.2/datagrowth.egg-info/
--rw-rw-r--   0 fako      (1000) fako      (1000)     2598 2022-11-14 14:39:59.000000 datagrowth-0.18.2/datagrowth.egg-info/PKG-INFO
--rw-rw-r--   0 fako      (1000) fako      (1000)     2601 2022-11-14 14:39:59.000000 datagrowth-0.18.2/datagrowth.egg-info/SOURCES.txt
--rw-rw-r--   0 fako      (1000) fako      (1000)        1 2022-11-14 14:39:59.000000 datagrowth-0.18.2/datagrowth.egg-info/dependency_links.txt
--rw-rw-r--   0 fako      (1000) fako      (1000)      102 2022-11-14 14:39:59.000000 datagrowth-0.18.2/datagrowth.egg-info/requires.txt
--rw-rw-r--   0 fako      (1000) fako      (1000)       11 2022-11-14 14:39:59.000000 datagrowth-0.18.2/datagrowth.egg-info/top_level.txt
--rw-rw-r--   0 fako      (1000) fako      (1000)       38 2022-11-14 14:39:59.417041 datagrowth-0.18.2/setup.cfg
--rw-rw-r--   0 fako      (1000) fako      (1000)     1289 2022-10-27 16:11:05.000000 datagrowth-0.18.2/setup.py
+drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2023-08-02 12:34:29.931023 datagrowth-0.19.0/
+-rw-rw-r--   0 fako      (1000) fako      (1000)     7652 2020-10-07 14:48:05.000000 datagrowth-0.19.0/LICENSE
+-rw-rw-r--   0 fako      (1000) fako      (1000)     2688 2023-08-02 12:34:29.931023 datagrowth-0.19.0/PKG-INFO
+-rw-rw-r--   0 fako      (1000) fako      (1000)     1554 2022-03-17 14:21:12.000000 datagrowth-0.19.0/README.md
+drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2023-08-02 12:34:29.923023 datagrowth-0.19.0/datagrowth/
+-rw-rw-r--   0 fako      (1000) fako      (1000)       56 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/__init__.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)      274 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/admin.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)     1176 2021-04-13 09:25:44.000000 datagrowth-0.19.0/datagrowth/apps.py
+drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2023-08-02 12:34:29.923023 datagrowth-0.19.0/datagrowth/configuration/
+-rw-rw-r--   0 fako      (1000) fako      (1000)      373 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/configuration/__init__.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)      159 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/configuration/configs.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)     4126 2023-07-27 19:05:39.000000 datagrowth-0.19.0/datagrowth/configuration/fields.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)     2601 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/configuration/serializers.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)    15989 2021-05-10 11:35:16.000000 datagrowth-0.19.0/datagrowth/configuration/types.py
+drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2023-08-02 12:34:29.923023 datagrowth-0.19.0/datagrowth/datatypes/
+-rw-rw-r--   0 fako      (1000) fako      (1000)      204 2023-07-27 19:11:58.000000 datagrowth-0.19.0/datagrowth/datatypes/__init__.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)      108 2021-05-10 11:35:16.000000 datagrowth-0.19.0/datagrowth/datatypes/admin.py
+drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2023-08-02 12:34:29.927023 datagrowth-0.19.0/datagrowth/datatypes/annotations/
+-rw-rw-r--   0 fako      (1000) fako      (1000)        0 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/datatypes/annotations/__init__.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)      213 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/datatypes/annotations/admin.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)      754 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/datatypes/annotations/base.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)     3357 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/datatypes/annotations/views.py
+drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2023-08-02 12:34:29.927023 datagrowth-0.19.0/datagrowth/datatypes/datasets/
+-rw-rw-r--   0 fako      (1000) fako      (1000)        0 2021-05-10 11:35:16.000000 datagrowth-0.19.0/datagrowth/datatypes/datasets/__init__.py
+drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2023-08-02 12:34:29.927023 datagrowth-0.19.0/datagrowth/datatypes/documents/
+-rw-rw-r--   0 fako      (1000) fako      (1000)        0 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/datatypes/documents/__init__.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)      213 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/datatypes/documents/admin.py
+drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2023-08-02 12:34:29.927023 datagrowth-0.19.0/datagrowth/datatypes/documents/db/
+-rw-rw-r--   0 fako      (1000) fako      (1000)        0 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/datatypes/documents/db/__init__.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)     1087 2023-07-27 19:11:58.000000 datagrowth-0.19.0/datagrowth/datatypes/documents/db/base.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)    13136 2023-08-02 09:45:06.000000 datagrowth-0.19.0/datagrowth/datatypes/documents/db/collection.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)     6995 2023-07-28 08:30:00.000000 datagrowth-0.19.0/datagrowth/datatypes/documents/db/document.py
+drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2023-08-02 12:34:29.927023 datagrowth-0.19.0/datagrowth/datatypes/documents/views/
+-rw-rw-r--   0 fako      (1000) fako      (1000)        0 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/datatypes/documents/views/__init__.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)     1096 2021-05-10 11:35:16.000000 datagrowth-0.19.0/datagrowth/datatypes/documents/views/collection.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)     1919 2021-05-10 11:35:16.000000 datagrowth-0.19.0/datagrowth/datatypes/documents/views/content.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)      327 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/datatypes/documents/views/document.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)      316 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/datatypes/views.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)      709 2023-07-27 19:11:58.000000 datagrowth-0.19.0/datagrowth/exceptions.py
+drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2023-08-02 12:34:29.927023 datagrowth-0.19.0/datagrowth/management/
+-rw-rw-r--   0 fako      (1000) fako      (1000)        0 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/management/__init__.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)     1876 2022-11-13 17:06:04.000000 datagrowth-0.19.0/datagrowth/management/base.py
+drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2023-08-02 12:34:29.927023 datagrowth-0.19.0/datagrowth/management/commands/
+-rw-rw-r--   0 fako      (1000) fako      (1000)        0 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/management/commands/__init__.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)      854 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/management/commands/dump_dataset.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)      699 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/management/commands/dump_resource.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)      689 2021-04-25 07:49:49.000000 datagrowth-0.19.0/datagrowth/management/commands/grow_dataset.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)     3838 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/management/commands/load_dataset.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)      864 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/management/commands/load_resource.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)     1391 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/management/commands/migrate_absolute_media_paths.py
+drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2023-08-02 12:34:29.927023 datagrowth-0.19.0/datagrowth/processors/
+-rw-rw-r--   0 fako      (1000) fako      (1000)       64 2023-07-27 19:11:58.000000 datagrowth-0.19.0/datagrowth/processors/__init__.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)     3116 2021-05-10 11:35:16.000000 datagrowth-0.19.0/datagrowth/processors/base.py
+drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2023-08-02 12:34:29.927023 datagrowth-0.19.0/datagrowth/processors/input/
+-rw-rw-r--   0 fako      (1000) fako      (1000)       81 2023-07-27 19:05:39.000000 datagrowth-0.19.0/datagrowth/processors/input/__init__.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)     7762 2023-08-02 09:32:23.000000 datagrowth-0.19.0/datagrowth/processors/input/extraction.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)      429 2023-07-27 19:05:39.000000 datagrowth-0.19.0/datagrowth/processors/input/iterators.py
+drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2023-08-02 12:34:29.931023 datagrowth-0.19.0/datagrowth/resources/
+-rw-rw-r--   0 fako      (1000) fako      (1000)      239 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/resources/__init__.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)       86 2021-05-10 11:35:16.000000 datagrowth-0.19.0/datagrowth/resources/admin.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)     5259 2023-07-27 19:11:58.000000 datagrowth-0.19.0/datagrowth/resources/base.py
+drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2023-08-02 12:34:29.931023 datagrowth-0.19.0/datagrowth/resources/http/
+-rw-rw-r--   0 fako      (1000) fako      (1000)      249 2023-07-27 19:05:39.000000 datagrowth-0.19.0/datagrowth/resources/http/__init__.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)      220 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/resources/http/admin.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)     1426 2023-07-27 19:05:39.000000 datagrowth-0.19.0/datagrowth/resources/http/decorators.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)     7451 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/resources/http/files.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)    29479 2023-08-02 10:19:29.000000 datagrowth-0.19.0/datagrowth/resources/http/generic.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)     2082 2023-07-27 19:05:39.000000 datagrowth-0.19.0/datagrowth/resources/http/iterators.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)     3308 2023-07-27 19:05:39.000000 datagrowth-0.19.0/datagrowth/resources/http/tasks.py
+drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2023-08-02 12:34:29.931023 datagrowth-0.19.0/datagrowth/resources/shell/
+-rw-rw-r--   0 fako      (1000) fako      (1000)      157 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/resources/shell/__init__.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)      235 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/resources/shell/admin.py
+drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2023-08-02 12:34:29.931023 datagrowth-0.19.0/datagrowth/resources/shell/apache/
+-rw-rw-r--   0 fako      (1000) fako      (1000)        0 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/resources/shell/apache/__init__.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)     2815 2021-04-13 09:25:44.000000 datagrowth-0.19.0/datagrowth/resources/shell/apache/tika.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)    13978 2022-10-27 16:01:06.000000 datagrowth-0.19.0/datagrowth/resources/shell/generic.py
+drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2023-08-02 12:34:29.931023 datagrowth-0.19.0/datagrowth/resources/shell/kaldi/
+-rw-rw-r--   0 fako      (1000) fako      (1000)        0 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/resources/shell/kaldi/__init__.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)     1683 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/resources/shell/kaldi/aspire.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)     1912 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/resources/shell/kaldi/nl.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)     1138 2023-07-27 19:05:39.000000 datagrowth-0.19.0/datagrowth/resources/shell/tasks.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)     3307 2023-07-28 08:59:14.000000 datagrowth-0.19.0/datagrowth/settings.py
+drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2023-08-02 12:34:29.931023 datagrowth-0.19.0/datagrowth/utils/
+-rw-rw-r--   0 fako      (1000) fako      (1000)      264 2021-04-13 09:25:44.000000 datagrowth-0.19.0/datagrowth/utils/__init__.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)     2789 2021-04-13 09:25:44.000000 datagrowth-0.19.0/datagrowth/utils/data.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)     1029 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/utils/datetime.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)     2909 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/utils/io.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)     1326 2020-10-07 14:48:05.000000 datagrowth-0.19.0/datagrowth/utils/iterators.py
+-rw-rw-r--   0 fako      (1000) fako      (1000)      198 2023-07-28 06:43:05.000000 datagrowth-0.19.0/datagrowth/version.py
+drwxrwxr-x   0 fako      (1000) fako      (1000)        0 2023-08-02 12:34:29.923023 datagrowth-0.19.0/datagrowth.egg-info/
+-rw-rw-r--   0 fako      (1000) fako      (1000)     2688 2023-08-02 12:34:29.000000 datagrowth-0.19.0/datagrowth.egg-info/PKG-INFO
+-rw-rw-r--   0 fako      (1000) fako      (1000)     2721 2023-08-02 12:34:29.000000 datagrowth-0.19.0/datagrowth.egg-info/SOURCES.txt
+-rw-rw-r--   0 fako      (1000) fako      (1000)        1 2023-08-02 12:34:29.000000 datagrowth-0.19.0/datagrowth.egg-info/dependency_links.txt
+-rw-rw-r--   0 fako      (1000) fako      (1000)       84 2023-08-02 12:34:29.000000 datagrowth-0.19.0/datagrowth.egg-info/requires.txt
+-rw-rw-r--   0 fako      (1000) fako      (1000)       11 2023-08-02 12:34:29.000000 datagrowth-0.19.0/datagrowth.egg-info/top_level.txt
+-rw-rw-r--   0 fako      (1000) fako      (1000)       38 2023-08-02 12:34:29.931023 datagrowth-0.19.0/setup.cfg
+-rw-rw-r--   0 fako      (1000) fako      (1000)     1348 2023-07-27 19:05:39.000000 datagrowth-0.19.0/setup.py
```

### Comparing `datagrowth-0.18.2/LICENSE` & `datagrowth-0.19.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datagrowth-0.18.2/PKG-INFO` & `datagrowth-0.19.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datagrowth
-Version: 0.18.2
+Version: 0.19.0
 Summary: Data engineering tools to create data mash ups using Django
 Home-page: https://github.com/fako/datagrowth
 Author: Fako Berkers
 Author-email: email@fakoberkers.nl
 License: UNKNOWN
 Description: [![datagrowth workflow](https://github.com/fako/datagrowth/actions/workflows/tests.yml/badge.svg)](https://github.com/fako/datagrowth/actions) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/datagrowth.svg)](https://pypi.python.org/pypi/datagrowth/) [![GPLv3 license](https://img.shields.io/badge/License-LGPLv3-blue.svg)](https://github.com/fako/datagrowth/blob/master/LICENSE)
         
@@ -55,12 +55,14 @@
         tox
         ```
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
```

### Comparing `datagrowth-0.18.2/README.md` & `datagrowth-0.19.0/README.md`

 * *Files identical despite different names*

### Comparing `datagrowth-0.18.2/datagrowth/apps.py` & `datagrowth-0.19.0/datagrowth/apps.py`

 * *Files identical despite different names*

### Comparing `datagrowth-0.18.2/datagrowth/configuration/fields.py` & `datagrowth-0.19.0/datagrowth/configuration/fields.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -53,22 +53,22 @@
         """
         super(ConfigurationField, self).__init__(*args, **kwargs)
         self._namespace = namespace
         self._private = private
         self._defaults = config_defaults
 
     def contribute_to_class(self, cls, name, private_only=False, **kwargs):
+        super(ConfigurationField, self).contribute_to_class(cls, name)
         configuration_property = ConfigurationProperty(
             storage_attribute=name,
             defaults=getattr(cls, 'CONFIG_DEFAULTS', self._defaults),
             namespace=getattr(cls, 'CONFIG_NAMESPACE', self._namespace),
             private=getattr(cls, 'CONFIG_PRIVATE', self._private)
         )
         setattr(cls, name, configuration_property)
-        super(ConfigurationField, self).contribute_to_class(cls, name)
 
     def from_db_value(self, value, expression, connection):
         return json.loads(value)
 
     def to_python(self, value):
         if isinstance(value, str):
             try:
```

### Comparing `datagrowth-0.18.2/datagrowth/configuration/serializers.py` & `datagrowth-0.19.0/datagrowth/configuration/serializers.py`

 * *Files identical despite different names*

### Comparing `datagrowth-0.18.2/datagrowth/configuration/types.py` & `datagrowth-0.19.0/datagrowth/configuration/types.py`

 * *Files identical despite different names*

### Comparing `datagrowth-0.18.2/datagrowth/datatypes/annotations/base.py` & `datagrowth-0.19.0/datagrowth/datatypes/annotations/base.py`

 * *Files identical despite different names*

### Comparing `datagrowth-0.18.2/datagrowth/datatypes/annotations/views.py` & `datagrowth-0.19.0/datagrowth/datatypes/annotations/views.py`

 * *Files identical despite different names*

### Comparing `datagrowth-0.18.2/datagrowth/datatypes/documents/db/base.py` & `datagrowth-0.19.0/datagrowth/datatypes/documents/db/base.py`

 * *Files identical despite different names*

### Comparing `datagrowth-0.18.2/datagrowth/datatypes/documents/db/collection.py` & `datagrowth-0.19.0/datagrowth/datatypes/documents/db/collection.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,26 +53,49 @@
         """
         Document = cls.get_document_model()
         if not isinstance(data, Iterable):
             data = [data]
         for instance in data:
             Document.validate(instance, schema)
 
-    def add(self, data, reset=False, batch_size=500, collection=None, modified_at=None, validate=True):
+    def add(self, data, reset=False, collection=None, modified_at=None):
         """
-        Add new data to the Collection in batches, possibly deleting all data before adding.
+        Add new data to the Collection, possibly deleting all data before adding.
+        This method will load all data into memory before inserting it into the database.
+        Use ``add_batches`` for a more memory footprint friendly version.
 
-        :param data: The data to use for the update
+        :param data: The data to use for the inserts
         :param reset: (optional) whether to delete existing data or not (no by default)
-        :param batch_size: (optional) how many instances to add in a single batch (default: 500)
         :param collection: (optional) a collection instance to add the data to (default: self)
         :param modified_at: (optional) the datetime to use as modified_at value for the collection (default: now)
-        :param validate: (deprecated) used to allow JSON schema validation before addition
-        :return: A list of updated or created instances.
+        :return: A list of created instances.
+        """
+        batches = self.add_batches(
+            data,
+            reset=reset,
+            collection=collection,
+            modified_at=modified_at
+        )
+        additions = []
+        for batch in batches:
+            additions += batch
+        return additions
+
+    def add_batches(self, data, batch_size=None, reset=False, collection=None, modified_at=None):
+        """
+        Add new data to the Collection, possibly deleting all data before adding.
+
+        :param data: The data to use for the inserts
+        :param batch_size: The amount of objects to load in memory and insert at once
+        :param reset: (optional) whether to delete existing data or not (no by default)
+        :param collection: (optional) a collection instance to add the data to (default: self)
+        :param modified_at: (optional) the datetime to use as modified_at value for the collection (default: now)
+        :return: An iterator of batches with created instances.
         """
+        batch_size = batch_size or datagrowth_settings.DATAGROWTH_MAX_BATCH_SIZE
         collection = collection or self
         modified_at = modified_at or make_aware(datetime.now())
         Document = collection.get_document_model()
         assert isinstance(data, (Iterator, list, tuple, dict, Document)), \
             f"Collection.add expects data to be formatted as iteratable, dict or {type(Document)} not {type(data)}"
 
         if reset:
@@ -90,80 +113,100 @@
                 data.clean()
                 prepared.append(data)
             else:  # type is list
                 for instance in data:
                     prepared += prepare_additions(instance)
             return prepared
 
-        count = 0
         for additions in ibatch(data, batch_size=batch_size):
             additions = prepare_additions(additions)
-            count += len(additions)
-            Document.objects.bulk_create(additions, batch_size=datagrowth_settings.DATAGROWTH_MAX_BATCH_SIZE)
+            yield Document.objects.bulk_create(additions, batch_size=batch_size)
 
         if collection.modified_at.replace(microsecond=0) != modified_at.replace(microsecond=0):
             collection.modified_at = modified_at
             collection.save()
-        return count
 
-    def update(self, data, by_property, batch_size=32, collection=None, modified_at=None, validate=True):
+    def update(self, data, by_property, collection=None, modified_at=None):
         """
-        Update data to the Collection in batches, using a property value to identify which Documents to update.
+        Update data to the Collection, using a property value to identify which Documents to update.
+        Any data that does not exist will be added instead.
+        This method will load all data into memory before performing upserts into the database.
+        Use ``update_batches`` for a more memory footprint friendly version.
 
-        :param data: The data to use for the update
+        :param data: The data to use for the upsert
         :param by_property: The property to identify a Document with
-        :param batch_size: (optional) how many instances to add in a single batch (default: 32)
-        :param collection: (optional) a collection instance to update the data to (default: self)
+        :param collection: (optional) a collection instance to upsert the data to (default: self)
         :param modified_at: (optional) the datetime to use as modified_at value for the collection (default: now)
-        :param validate: (deprecated) used to allow JSON schema validation before updates
         :return: A list of updated or created instances.
         """
+        batches = self.update_batches(
+            data,
+            by_property=by_property,
+            collection=collection,
+            modified_at=modified_at
+        )
+        upserts = []
+        for batch in batches:
+            upserts += batch
+        return upserts
+
+    def update_batches(self, data, by_property, batch_size=32, collection=None, modified_at=None):
+        """
+        Update data to the Collection, using a property value to identify which Documents to update.
+        Any data that does not exist will be added instead.
+
+        :param data: The data to use for the upsert
+        :param by_property: The property to identify a Document with
+        :param batch_size: The amount of objects to load in memory and insert at once
+        :param collection: (optional) a collection instance to upsert the data to (default: self)
+        :param modified_at: (optional) the datetime to use as modified_at value for the collection (default: now)
+        :return: An iterator of batches with updated or created instances.
+        """
+        batch_size = batch_size or datagrowth_settings.DATAGROWTH_MAX_BATCH_SIZE
         collection = collection or self
         modified_at = modified_at or make_aware(datetime.now())
         Document = collection.get_document_model()
         assert isinstance(data, (Iterator, list, tuple,)), \
             f"Collection.update expects data to be formatted as iteratable not {type(data)}"
 
-        count = 0
-        for updates in ibatch(data, batch_size=batch_size):
+        for update_data in ibatch(data, batch_size=batch_size):
             # We bulk update by getting all objects whose property matches
             # any update's "by_property" property value and then updating these source objects.
             # One update object can potentially target multiple sources
             # if multiple objects with the same value for the by_property property exist.
             updated = set()
-            prepared = []
+            updates = []
             sources_by_lookup = defaultdict(list)
-            for update in updates:
+            for update in update_data:
                 sources_by_lookup[update[by_property]].append(update)
             target_filters = Q()
             for lookup_value in sources_by_lookup.keys():
                 target_filters |= Q(**{f"properties__{by_property}": lookup_value})
             for target in collection.documents.filter(target_filters):
                 for update_value in sources_by_lookup[target.properties[by_property]]:
                     target.update(update_value, commit=False)
-                count += 1
                 updated.add(target.properties[by_property])
-                prepared.append(target)
+                updates.append(target)
             Document.objects.bulk_update(
-                prepared,
+                updates,
                 ["properties", "identity", "reference", "modified_at"],
-                batch_size=datagrowth_settings.DATAGROWTH_MAX_BATCH_SIZE
+                batch_size=batch_size
             )
             # After all updates we add all data that hasn't been used in any update operation
             additions = []
             for lookup_value, sources in sources_by_lookup.items():
                 if lookup_value not in updated:
                     additions += sources
             if len(additions):
-                count += self.add(additions, batch_size=batch_size, collection=collection, modified_at=modified_at)
+                additions = self.add(additions, collection=collection, modified_at=modified_at)
+            yield updates + additions
 
         if collection.modified_at.replace(microsecond=0) != modified_at.replace(microsecond=0):
             collection.modified_at = modified_at
             collection.save()
-        return count
 
     @property
     def content(self):
         """
         Returns the content of the documents of this Collection
 
         :return: a generator yielding properties from Documents
```

### Comparing `datagrowth-0.18.2/datagrowth/datatypes/documents/views/collection.py` & `datagrowth-0.19.0/datagrowth/datatypes/documents/views/collection.py`

 * *Files identical despite different names*

### Comparing `datagrowth-0.18.2/datagrowth/datatypes/documents/views/content.py` & `datagrowth-0.19.0/datagrowth/datatypes/documents/views/content.py`

 * *Files identical despite different names*

### Comparing `datagrowth-0.18.2/datagrowth/exceptions.py` & `datagrowth-0.19.0/datagrowth/exceptions.py`

 * *Files identical despite different names*

### Comparing `datagrowth-0.18.2/datagrowth/management/base.py` & `datagrowth-0.19.0/datagrowth/management/base.py`

 * *Files identical despite different names*

### Comparing `datagrowth-0.18.2/datagrowth/management/commands/dump_dataset.py` & `datagrowth-0.19.0/datagrowth/management/commands/dump_dataset.py`

 * *Files identical despite different names*

### Comparing `datagrowth-0.18.2/datagrowth/management/commands/dump_resource.py` & `datagrowth-0.19.0/datagrowth/management/commands/dump_resource.py`

 * *Files identical despite different names*

### Comparing `datagrowth-0.18.2/datagrowth/management/commands/grow_dataset.py` & `datagrowth-0.19.0/datagrowth/management/commands/grow_dataset.py`

 * *Files identical despite different names*

### Comparing `datagrowth-0.18.2/datagrowth/management/commands/load_dataset.py` & `datagrowth-0.19.0/datagrowth/management/commands/load_dataset.py`

 * *Files identical despite different names*

### Comparing `datagrowth-0.18.2/datagrowth/management/commands/load_resource.py` & `datagrowth-0.19.0/datagrowth/management/commands/load_resource.py`

 * *Files identical despite different names*

### Comparing `datagrowth-0.18.2/datagrowth/management/commands/migrate_absolute_media_paths.py` & `datagrowth-0.19.0/datagrowth/management/commands/migrate_absolute_media_paths.py`

 * *Files identical despite different names*

### Comparing `datagrowth-0.18.2/datagrowth/processors/base.py` & `datagrowth-0.19.0/datagrowth/processors/base.py`

 * *Files identical despite different names*

### Comparing `datagrowth-0.18.2/datagrowth/processors/input/extraction.py` & `datagrowth-0.19.0/datagrowth/processors/input/extraction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from types import GeneratorType
 from copy import copy
 
 from datagrowth.configuration import ConfigurationProperty
 from datagrowth.utils import reach, is_json_mimetype
 from datagrowth.processors.base import Processor
 from datagrowth.exceptions import DGNoContent
 
@@ -17,15 +18,15 @@
      * A JSON path as described by the reach function (for JSON extraction)
      * A string containing BeautifulSoup expressions using the "soup" and "el" variables (for HTML/XML extraction, not recommended)
      * A processor name and method name (like: Processor.method) that take a soup and el argument (for HTML/XML extraction, recommended)
 
     These values will be called/parsed to extract data from the input data.
     The extracted data gets stored under the keys.
 
-    The special "@" key indicates where extraction should start and its value should result in a list.
+    The special "@" key indicates where extraction should start and its value should result in a list or generator.
     By default objective values get evaluated against elements in the list retrieved from the '@' value.
     Objective items who's keys start with "#" will get evaluated against the entire input.
 
     The output of the ``ExtractProcessor`` will typically consist of a list of objects.
     Each object shares the same keys as the objective except the "@" key.
     Any keys in the objective that start with "#" will have the same value for all extracted objects,
     but the "#" will get stripped from the object keys.
@@ -124,15 +125,15 @@
             context[name] = reach(objective, data) if not callable(objective) else objective(data)
 
         nodes = reach(self._at, data) if not callable(self._at) else self._at(data)
         if isinstance(nodes, dict) and self.config.extract_from_object_values:
             nodes = nodes.values()
         elif nodes is None:
             raise DGNoContent("Found no nodes at {}".format(self._at))
-        elif not isinstance(nodes, list):
+        elif not isinstance(nodes, (list, GeneratorType,)):
             nodes = [nodes]
 
         for node in nodes:
             result = copy(context)
             for name, objective in self._objective.items():
                 result[name] = reach(objective, node) if not callable(objective) else objective(node)
             yield result
```

### Comparing `datagrowth-0.18.2/datagrowth/resources/base.py` & `datagrowth-0.19.0/datagrowth/resources/base.py`

 * *Files identical despite different names*

### Comparing `datagrowth-0.18.2/datagrowth/resources/http/files.py` & `datagrowth-0.19.0/datagrowth/resources/http/files.py`

 * *Files identical despite different names*

### Comparing `datagrowth-0.18.2/datagrowth/resources/http/generic.py` & `datagrowth-0.19.0/datagrowth/resources/http/generic.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
         if self.success:
             content_type = self.head.get("content-type", "unknown/unknown").split(';')[0]
             if is_json_mimetype(content_type):
                 return content_type, json.loads(self.body)
             elif content_type == "text/html":
                 return content_type, BeautifulSoup(self.body, "html.parser")
             elif content_type == "text/xml" or content_type == "application/xml":
-                return content_type, BeautifulSoup(self.body, "lxml")
+                return content_type, BeautifulSoup(self.body, "xml")
             else:
                 return content_type, None
         return None, None
 
     #######################################################
     # CREATE REQUEST
     #######################################################
```

### Comparing `datagrowth-0.18.2/datagrowth/resources/http/tasks.py` & `datagrowth-0.19.0/datagrowth/resources/http/tasks.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,20 @@
 import logging
-import requests
 
 from django.apps import apps
 from celery import current_app as app
 
-from datagrowth.processors.base import Processor
 from datagrowth.configuration import ConfigurationType, load_config
-
-from datagrowth.exceptions import DGResourceException
+from datagrowth.resources.http import load_session
+from datagrowth.resources.http import send_iterator
 
 
 log = logging.getLogger("datascope")
 
 
-def load_session():  # TODO: test to unlock
-    """
-    This decorator will try to fetch a session object based on the "session" keyword argument.
-    If the argument is a string it is assumed to be the name of a processor that implements the get_session method.
-    Whatever this method returns gets injected under the "session" keyword argument for the decorated function.
-    If the argument is not a string it gets returned as being a valid session for the resource.
-
-    :param defaults: (mixed) Name of the session provider or the session object.
-    :return:
-    """
-    def wrap(func):
-        def session_func(config, *args, **kwargs):
-            assert isinstance(config, ConfigurationType), \
-                "load_session expects a fully prepared ConfigurationType for config"
-            session_injection = kwargs.pop("session", None)
-            if not session_injection:
-                session_injection = requests.Session()
-            if not isinstance(session_injection, str):
-                return func(config, session=session_injection, *args, **kwargs)
-            session_provider = Processor.get_processor_class(session_injection)
-            session = session_provider.get_session(config)
-            return func(config, session=session, *args, **kwargs)
-        return session_func
-    return wrap
-
-
 def get_resource_link(config, session=None):
     assert isinstance(config, ConfigurationType), \
         "get_resource_link expects a fully prepared ConfigurationType for config"
     Resource = apps.get_model(config.resource)
     link = Resource(config=config.to_dict(protected=True))
 
     if session is not None:
@@ -60,36 +32,20 @@
 @load_session()
 def send(config, *args, **kwargs):
     # Set vars
     session = kwargs.pop("session", None)
     method = kwargs.pop("method", None)
     success = []
     errors = []
-    has_next_request = True
-    current_request = {}
-    count = 0
-    limit = config.continuation_limit or 1
-    # Continue as long as there are subsequent requests
-    while has_next_request and count < limit:
-        # Get payload
-        link = get_resource_link(config, session)
-        link.request = current_request
-        link.interval_duration = config.interval_duration
-        try:
-            link = link.send(method, *args, **kwargs)
-            link.close()
+    # Send initial Resource as well as any followup Resources and iterator over all of them
+    for link in send_iterator(method=method, config=config, session=session, *args, **kwargs):
+        if link.success:
             success.append(link.id)
-        except DGResourceException as exc:
-            log.debug(exc)
-            link = exc.resource
-            link.close()
+        else:
             errors.append(link.id)
-        # Prepare next request
-        has_next_request = current_request = link.create_next_request()
-        count += 1
     # Output results in simple type for json serialization
     return [success, errors]
 
 
 @app.task(name="http_resource.send_serie")
 @load_config()
 @load_session()
```

### Comparing `datagrowth-0.18.2/datagrowth/resources/shell/apache/tika.py` & `datagrowth-0.19.0/datagrowth/resources/shell/apache/tika.py`

 * *Files identical despite different names*

### Comparing `datagrowth-0.18.2/datagrowth/resources/shell/generic.py` & `datagrowth-0.19.0/datagrowth/resources/shell/generic.py`

 * *Files identical despite different names*

### Comparing `datagrowth-0.18.2/datagrowth/resources/shell/kaldi/aspire.py` & `datagrowth-0.19.0/datagrowth/resources/shell/kaldi/aspire.py`

 * *Files identical despite different names*

### Comparing `datagrowth-0.18.2/datagrowth/resources/shell/kaldi/nl.py` & `datagrowth-0.19.0/datagrowth/resources/shell/kaldi/nl.py`

 * *Files identical despite different names*

### Comparing `datagrowth-0.18.2/datagrowth/resources/shell/tasks.py` & `datagrowth-0.19.0/datagrowth/resources/shell/tasks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-from time import sleep
 
 from django.apps import apps
 from celery import current_app as app
 
 from datagrowth.configuration import load_config
 from datagrowth.exceptions import DGResourceException
```

### Comparing `datagrowth-0.18.2/datagrowth/settings.py` & `datagrowth-0.19.0/datagrowth/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 DATAGROWTH_BIN_DIR = getattr(settings, "DATAGROWTH_BIN_DIR",
     os.path.join(settings.BASE_DIR, "datagrowth", "resources", "shell", "bin")
 )
 
 DATAGROWTH_REQUESTS_PROXIES = getattr(settings, "DATAGROWTH_REQUESTS_PROXIES", None)
 DATAGROWTH_REQUESTS_VERIFY = getattr(settings, "DATAGROWTH_REQUESTS_VERIFY", True)
 
-DATAGROWTH_MAX_BATCH_SIZE = getattr(settings, "DATAGROWTH_MAX_BATCH_SIZE", 500)
+DATAGROWTH_MAX_BATCH_SIZE = getattr(settings, "DATAGROWTH_MAX_BATCH_SIZE", 100)
 
 DATAGROWTH_KALDI_BASE_PATH = getattr(settings, "DATAGROWTH_KALDI_BASE_PATH", "")
 DATAGROWTH_KALDI_ASPIRE_BASE_PATH = getattr(settings, "DATAGROWTH_KALDI_ASPIRE_BASE_PATH", "")
 DATAGROWTH_KALDI_NL_BASE_PATH = getattr(settings, "DATAGROWTH_KALDI_NL_BASE_PATH", "")
 
 
 ######################################
@@ -58,17 +58,14 @@
     "wikipedia_wiki_full_extracts": False,
     "wikipedia_wiki_domain": "en.wikipedia.org",
     "wikipedia_wiki_show_categories": "!hidden",
 
     "google_api_key": getattr(settings, 'GOOGLE_API_KEY', ''),
     "google_cx": getattr(settings, 'GOOGLE_CX', ''),
 
-    "indico_api_key": getattr(settings, 'INDICO_API_KEY', ''),
-    "wizenoze_api_key": getattr(settings, 'WIZENOZE_API_KEY', ''),
-
     "rank_processor_batch_size": 1000,
     "rank_processor_result_size": 20,
 
     "extract_processor_extract_from_object_values": False,
 
     "micro_service_connections": {
         "image_recognition": {
```

### Comparing `datagrowth-0.18.2/datagrowth/utils/data.py` & `datagrowth-0.19.0/datagrowth/utils/data.py`

 * *Files identical despite different names*

### Comparing `datagrowth-0.18.2/datagrowth/utils/datetime.py` & `datagrowth-0.19.0/datagrowth/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `datagrowth-0.18.2/datagrowth/utils/io.py` & `datagrowth-0.19.0/datagrowth/utils/io.py`

 * *Files identical despite different names*

### Comparing `datagrowth-0.18.2/datagrowth/utils/iterators.py` & `datagrowth-0.19.0/datagrowth/utils/iterators.py`

 * *Files identical despite different names*

### Comparing `datagrowth-0.18.2/datagrowth.egg-info/PKG-INFO` & `datagrowth-0.19.0/datagrowth.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datagrowth
-Version: 0.18.2
+Version: 0.19.0
 Summary: Data engineering tools to create data mash ups using Django
 Home-page: https://github.com/fako/datagrowth
 Author: Fako Berkers
 Author-email: email@fakoberkers.nl
 License: UNKNOWN
 Description: [![datagrowth workflow](https://github.com/fako/datagrowth/actions/workflows/tests.yml/badge.svg)](https://github.com/fako/datagrowth/actions) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/datagrowth.svg)](https://pypi.python.org/pypi/datagrowth/) [![GPLv3 license](https://img.shields.io/badge/License-LGPLv3-blue.svg)](https://github.com/fako/datagrowth/blob/master/LICENSE)
         
@@ -55,12 +55,14 @@
         tox
         ```
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
```

### Comparing `datagrowth-0.18.2/datagrowth.egg-info/SOURCES.txt` & `datagrowth-0.19.0/datagrowth.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -44,21 +44,24 @@
 datagrowth/management/commands/load_dataset.py
 datagrowth/management/commands/load_resource.py
 datagrowth/management/commands/migrate_absolute_media_paths.py
 datagrowth/processors/__init__.py
 datagrowth/processors/base.py
 datagrowth/processors/input/__init__.py
 datagrowth/processors/input/extraction.py
+datagrowth/processors/input/iterators.py
 datagrowth/resources/__init__.py
 datagrowth/resources/admin.py
 datagrowth/resources/base.py
 datagrowth/resources/http/__init__.py
 datagrowth/resources/http/admin.py
+datagrowth/resources/http/decorators.py
 datagrowth/resources/http/files.py
 datagrowth/resources/http/generic.py
+datagrowth/resources/http/iterators.py
 datagrowth/resources/http/tasks.py
 datagrowth/resources/shell/__init__.py
 datagrowth/resources/shell/admin.py
 datagrowth/resources/shell/generic.py
 datagrowth/resources/shell/tasks.py
 datagrowth/resources/shell/apache/__init__.py
 datagrowth/resources/shell/apache/tika.py
```

### Comparing `datagrowth-0.18.2/setup.py` & `datagrowth-0.19.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,20 +29,21 @@
         "jsonschema",
         "lxml",
         "beautifulsoup4",
         "urlobject",
         "requests",
         "Pillow>=8",
         "tqdm",
-        "django-json-field",
     ],
     python_requires="~=3.8",
     include_package_data=True,
     classifiers=(
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Framework :: Django :: 3.2",
+        "Framework :: Django :: 4.2",
         "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
         "Operating System :: OS Independent",
     ),
 )
```


# Comparing `tmp/vzg.jconv-1.2.6.tar.gz` & `tmp/vzg.jconv-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vzg.jconv-1.2.6.tar", last modified: Wed Aug  2 11:36:15 2023, max compression
+gzip compressed data, was "vzg.jconv-1.2.7.tar", last modified: Wed Aug  2 12:08:41 2023, max compression
```

## Comparing `vzg.jconv-1.2.6.tar` & `vzg.jconv-1.2.7.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 11:36:15.765669 vzg.jconv-1.2.6/
--rw-rw-r--   0 teg       (1000) teg       (1000)    34520 2020-02-07 11:02:19.000000 vzg.jconv-1.2.6/LICENSE.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)      149 2020-02-08 11:53:49.000000 vzg.jconv-1.2.6/MANIFEST.in
--rw-rw-r--   0 teg       (1000) teg       (1000)      843 2023-08-02 11:36:15.765669 vzg.jconv-1.2.6/PKG-INFO
--rw-rw-r--   0 teg       (1000) teg       (1000)      463 2023-02-16 10:38:51.000000 vzg.jconv-1.2.6/README.md
--rw-rw-r--   0 teg       (1000) teg       (1000)        6 2023-08-02 11:35:45.000000 vzg.jconv-1.2.6/VERSION.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)       38 2023-08-02 11:36:15.765669 vzg.jconv-1.2.6/setup.cfg
--rw-rw-r--   0 teg       (1000) teg       (1000)     1679 2023-02-16 10:38:51.000000 vzg.jconv-1.2.6/setup.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 11:36:15.765669 vzg.jconv-1.2.6/src/
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 11:36:15.765669 vzg.jconv-1.2.6/src/vzg/
--rw-rw-r--   0 teg       (1000) teg       (1000)       80 2020-11-05 11:14:17.000000 vzg.jconv-1.2.6/src/vzg/__init__.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 11:36:15.765669 vzg.jconv-1.2.6/src/vzg/jconv/
--rw-rw-r--   0 teg       (1000) teg       (1000)      275 2020-02-07 09:30:55.000000 vzg.jconv-1.2.6/src/vzg/jconv/__init__.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 11:36:15.765669 vzg.jconv-1.2.6/src/vzg/jconv/converter/
--rw-rw-r--   0 teg       (1000) teg       (1000)      378 2020-02-07 13:03:16.000000 vzg.jconv-1.2.6/src/vzg/jconv/converter/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)    15052 2023-08-02 11:31:38.000000 vzg.jconv-1.2.6/src/vzg/jconv/converter/jats.py
--rw-rw-r--   0 teg       (1000) teg       (1000)      450 2020-07-07 11:26:12.000000 vzg.jconv-1.2.6/src/vzg/jconv/errors.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     4136 2023-08-01 08:59:23.000000 vzg.jconv-1.2.6/src/vzg/jconv/gapi.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     1112 2023-07-31 15:01:19.000000 vzg.jconv-1.2.6/src/vzg/jconv/interfaces.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 11:36:15.765669 vzg.jconv-1.2.6/src/vzg/jconv/journal/
--rw-rw-r--   0 teg       (1000) teg       (1000)     6603 2023-07-31 15:28:18.000000 vzg.jconv-1.2.6/src/vzg/jconv/journal/__init__.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 11:36:15.765669 vzg.jconv-1.2.6/src/vzg/jconv/langcode/
--rw-rw-r--   0 teg       (1000) teg       (1000)     1156 2020-02-07 12:48:06.000000 vzg.jconv-1.2.6/src/vzg/jconv/langcode/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)    11245 2020-02-07 12:11:08.000000 vzg.jconv-1.2.6/src/vzg/jconv/langcode/language-codes.json
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 11:36:15.765669 vzg.jconv-1.2.6/src/vzg/jconv/person/
--rw-rw-r--   0 teg       (1000) teg       (1000)     5949 2023-07-21 15:51:03.000000 vzg.jconv-1.2.6/src/vzg/jconv/person/__init__.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 11:36:15.765669 vzg.jconv-1.2.6/src/vzg/jconv/publisher/
--rw-rw-r--   0 teg       (1000) teg       (1000)     1314 2023-07-28 13:58:32.000000 vzg.jconv-1.2.6/src/vzg/jconv/publisher/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)      263 2020-07-02 08:39:22.000000 vzg.jconv-1.2.6/src/vzg/jconv/publisher/publisher-codes.json
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 11:36:15.765669 vzg.jconv-1.2.6/src/vzg/jconv/schema/
--rw-rw-r--   0 teg       (1000) teg       (1000)    17321 2022-01-14 16:28:18.000000 vzg.jconv-1.2.6/src/vzg/jconv/schema/article_schema.json
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 11:36:15.765669 vzg.jconv-1.2.6/src/vzg/jconv/test/
--rw-rw-r--   0 teg       (1000) teg       (1000)      960 2020-02-11 12:04:12.000000 vzg.jconv-1.2.6/src/vzg/jconv/test/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     1218 2023-07-21 15:51:03.000000 vzg.jconv-1.2.6/src/vzg/jconv/test/conftest.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     6068 2023-07-21 15:51:03.000000 vzg.jconv-1.2.6/src/vzg/jconv/test/test_jats_article.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     3627 2023-08-01 07:25:20.000000 vzg.jconv-1.2.6/src/vzg/jconv/test/test_jats_converter.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     7302 2023-08-01 07:22:39.000000 vzg.jconv-1.2.6/src/vzg/jconv/test/test_jats_degruyter.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     2406 2023-08-01 09:54:23.000000 vzg.jconv-1.2.6/src/vzg/jconv/test/test_jatsdate.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     4008 2023-07-31 15:20:44.000000 vzg.jconv-1.2.6/src/vzg/jconv/test/test_journal.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     1038 2020-02-11 12:04:12.000000 vzg.jconv-1.2.6/src/vzg/jconv/test/test_langcode.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     2803 2023-02-16 12:17:30.000000 vzg.jconv-1.2.6/src/vzg/jconv/test/test_person.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     1029 2020-07-02 09:05:29.000000 vzg.jconv-1.2.6/src/vzg/jconv/test/test_publisher.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 11:36:15.765669 vzg.jconv-1.2.6/src/vzg/jconv/tools/
--rw-rw-r--   0 teg       (1000) teg       (1000)      378 2020-02-12 10:22:25.000000 vzg.jconv-1.2.6/src/vzg/jconv/tools/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     6790 2023-07-21 15:51:03.000000 vzg.jconv-1.2.6/src/vzg/jconv/tools/simple_conv.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 11:36:15.765669 vzg.jconv-1.2.6/src/vzg/jconv/utils/
--rw-rw-r--   0 teg       (1000) teg       (1000)     2932 2023-07-24 11:56:32.000000 vzg.jconv-1.2.6/src/vzg/jconv/utils/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     1989 2023-08-01 09:44:49.000000 vzg.jconv-1.2.6/src/vzg/jconv/utils/date.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 11:36:15.765669 vzg.jconv-1.2.6/src/vzg.jconv.egg-info/
--rw-rw-r--   0 teg       (1000) teg       (1000)      843 2023-08-02 11:36:15.000000 vzg.jconv-1.2.6/src/vzg.jconv.egg-info/PKG-INFO
--rw-rw-r--   0 teg       (1000) teg       (1000)     1316 2023-08-02 11:36:15.000000 vzg.jconv-1.2.6/src/vzg.jconv.egg-info/SOURCES.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)        1 2023-08-02 11:36:15.000000 vzg.jconv-1.2.6/src/vzg.jconv.egg-info/dependency_links.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)       65 2023-08-02 11:36:15.000000 vzg.jconv-1.2.6/src/vzg.jconv.egg-info/entry_points.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)        4 2023-08-02 11:36:15.000000 vzg.jconv-1.2.6/src/vzg.jconv.egg-info/namespace_packages.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)        1 2020-02-07 10:31:14.000000 vzg.jconv-1.2.6/src/vzg.jconv.egg-info/not-zip-safe
--rw-rw-r--   0 teg       (1000) teg       (1000)       48 2023-08-02 11:36:15.000000 vzg.jconv-1.2.6/src/vzg.jconv.egg-info/requires.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)        4 2023-08-02 11:36:15.000000 vzg.jconv-1.2.6/src/vzg.jconv.egg-info/top_level.txt
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/
+-rw-rw-r--   0 teg       (1000) teg       (1000)    34520 2020-02-07 11:02:19.000000 vzg.jconv-1.2.7/LICENSE.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)      149 2020-02-08 11:53:49.000000 vzg.jconv-1.2.7/MANIFEST.in
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1339 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/PKG-INFO
+-rw-rw-r--   0 teg       (1000) teg       (1000)      463 2023-02-16 10:38:51.000000 vzg.jconv-1.2.7/README.md
+-rw-rw-r--   0 teg       (1000) teg       (1000)        6 2023-08-02 12:07:14.000000 vzg.jconv-1.2.7/VERSION.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)       38 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/setup.cfg
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1868 2023-08-02 11:54:02.000000 vzg.jconv-1.2.7/setup.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/src/
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/src/vzg/
+-rw-rw-r--   0 teg       (1000) teg       (1000)       80 2020-11-05 11:14:17.000000 vzg.jconv-1.2.7/src/vzg/__init__.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/src/vzg/jconv/
+-rw-rw-r--   0 teg       (1000) teg       (1000)      275 2020-02-07 09:30:55.000000 vzg.jconv-1.2.7/src/vzg/jconv/__init__.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/src/vzg/jconv/converter/
+-rw-rw-r--   0 teg       (1000) teg       (1000)      378 2020-02-07 13:03:16.000000 vzg.jconv-1.2.7/src/vzg/jconv/converter/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)    15052 2023-08-02 11:31:38.000000 vzg.jconv-1.2.7/src/vzg/jconv/converter/jats.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)      450 2020-07-07 11:26:12.000000 vzg.jconv-1.2.7/src/vzg/jconv/errors.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     4136 2023-08-01 08:59:23.000000 vzg.jconv-1.2.7/src/vzg/jconv/gapi.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1112 2023-07-31 15:01:19.000000 vzg.jconv-1.2.7/src/vzg/jconv/interfaces.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/src/vzg/jconv/journal/
+-rw-rw-r--   0 teg       (1000) teg       (1000)     6603 2023-07-31 15:28:18.000000 vzg.jconv-1.2.7/src/vzg/jconv/journal/__init__.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/src/vzg/jconv/langcode/
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1156 2020-02-07 12:48:06.000000 vzg.jconv-1.2.7/src/vzg/jconv/langcode/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)    11245 2020-02-07 12:11:08.000000 vzg.jconv-1.2.7/src/vzg/jconv/langcode/language-codes.json
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/src/vzg/jconv/person/
+-rw-rw-r--   0 teg       (1000) teg       (1000)     5949 2023-07-21 15:51:03.000000 vzg.jconv-1.2.7/src/vzg/jconv/person/__init__.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/src/vzg/jconv/publisher/
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1314 2023-07-28 13:58:32.000000 vzg.jconv-1.2.7/src/vzg/jconv/publisher/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)      263 2020-07-02 08:39:22.000000 vzg.jconv-1.2.7/src/vzg/jconv/publisher/publisher-codes.json
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/src/vzg/jconv/schema/
+-rw-rw-r--   0 teg       (1000) teg       (1000)    17321 2022-01-14 16:28:18.000000 vzg.jconv-1.2.7/src/vzg/jconv/schema/article_schema.json
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/src/vzg/jconv/test/
+-rw-rw-r--   0 teg       (1000) teg       (1000)      960 2020-02-11 12:04:12.000000 vzg.jconv-1.2.7/src/vzg/jconv/test/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1218 2023-07-21 15:51:03.000000 vzg.jconv-1.2.7/src/vzg/jconv/test/conftest.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     6068 2023-07-21 15:51:03.000000 vzg.jconv-1.2.7/src/vzg/jconv/test/test_jats_article.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     3627 2023-08-01 07:25:20.000000 vzg.jconv-1.2.7/src/vzg/jconv/test/test_jats_converter.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     7302 2023-08-01 07:22:39.000000 vzg.jconv-1.2.7/src/vzg/jconv/test/test_jats_degruyter.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     2406 2023-08-01 09:54:23.000000 vzg.jconv-1.2.7/src/vzg/jconv/test/test_jatsdate.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     4008 2023-07-31 15:20:44.000000 vzg.jconv-1.2.7/src/vzg/jconv/test/test_journal.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1038 2020-02-11 12:04:12.000000 vzg.jconv-1.2.7/src/vzg/jconv/test/test_langcode.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     2803 2023-02-16 12:17:30.000000 vzg.jconv-1.2.7/src/vzg/jconv/test/test_person.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1029 2020-07-02 09:05:29.000000 vzg.jconv-1.2.7/src/vzg/jconv/test/test_publisher.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/src/vzg/jconv/tools/
+-rw-rw-r--   0 teg       (1000) teg       (1000)      378 2020-02-12 10:22:25.000000 vzg.jconv-1.2.7/src/vzg/jconv/tools/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     6790 2023-07-21 15:51:03.000000 vzg.jconv-1.2.7/src/vzg/jconv/tools/simple_conv.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/src/vzg/jconv/utils/
+-rw-rw-r--   0 teg       (1000) teg       (1000)     2932 2023-07-24 11:56:32.000000 vzg.jconv-1.2.7/src/vzg/jconv/utils/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1989 2023-08-01 09:44:49.000000 vzg.jconv-1.2.7/src/vzg/jconv/utils/date.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/src/vzg.jconv.egg-info/
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1339 2023-08-02 12:08:41.000000 vzg.jconv-1.2.7/src/vzg.jconv.egg-info/PKG-INFO
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1316 2023-08-02 12:08:41.000000 vzg.jconv-1.2.7/src/vzg.jconv.egg-info/SOURCES.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)        1 2023-08-02 12:08:41.000000 vzg.jconv-1.2.7/src/vzg.jconv.egg-info/dependency_links.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)       65 2023-08-02 12:08:41.000000 vzg.jconv-1.2.7/src/vzg.jconv.egg-info/entry_points.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)        4 2023-08-02 12:08:41.000000 vzg.jconv-1.2.7/src/vzg.jconv.egg-info/namespace_packages.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)        1 2020-02-07 10:31:14.000000 vzg.jconv-1.2.7/src/vzg.jconv.egg-info/not-zip-safe
+-rw-rw-r--   0 teg       (1000) teg       (1000)       48 2023-08-02 12:08:41.000000 vzg.jconv-1.2.7/src/vzg.jconv.egg-info/requires.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)        4 2023-08-02 12:08:41.000000 vzg.jconv-1.2.7/src/vzg.jconv.egg-info/top_level.txt
```

### Comparing `vzg.jconv-1.2.6/LICENSE.txt` & `vzg.jconv-1.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.6/setup.py` & `vzg.jconv-1.2.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,29 +6,34 @@
 # All Rights Reserved.
 #
 ##############################################################################
 """
 
 # Imports
 from setuptools import setup, find_packages
+from pathlib import Path
 
 __author__ = """Marc-J. Tegethoff <marc.tegethoff@gbv.de>"""
 __docformat__ = "plaintext"
 
 
 def gc(fname):
-    return open(fname).read()
+    mod_directory = Path(__file__).parent
+    fpath = mod_directory / fname
+    return fpath.read_text()
 
 
 setup(
     name="vzg.jconv",
     version=gc("VERSION.txt"),
     author="Marc-J. Tegethoff",
     author_email="tegethoff@gbv.de",
     description="Python library to create JSON Data",
+    long_description=gc("README.md"),
+    long_description_content_type="text/markdown",
     keywords="VZG Python JSON XML JAST",
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
```

### Comparing `vzg.jconv-1.2.6/src/vzg/jconv/converter/jats.py` & `vzg.jconv-1.2.7/src/vzg/jconv/converter/jats.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.6/src/vzg/jconv/gapi.py` & `vzg.jconv-1.2.7/src/vzg/jconv/gapi.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.6/src/vzg/jconv/interfaces.py` & `vzg.jconv-1.2.7/src/vzg/jconv/interfaces.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.6/src/vzg/jconv/journal/__init__.py` & `vzg.jconv-1.2.7/src/vzg/jconv/journal/__init__.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.6/src/vzg/jconv/langcode/__init__.py` & `vzg.jconv-1.2.7/src/vzg/jconv/langcode/__init__.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.6/src/vzg/jconv/langcode/language-codes.json` & `vzg.jconv-1.2.7/src/vzg/jconv/langcode/language-codes.json`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.6/src/vzg/jconv/person/__init__.py` & `vzg.jconv-1.2.7/src/vzg/jconv/person/__init__.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.6/src/vzg/jconv/publisher/__init__.py` & `vzg.jconv-1.2.7/src/vzg/jconv/publisher/__init__.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.6/src/vzg/jconv/schema/article_schema.json` & `vzg.jconv-1.2.7/src/vzg/jconv/schema/article_schema.json`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.6/src/vzg/jconv/test/__init__.py` & `vzg.jconv-1.2.7/src/vzg/jconv/test/__init__.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.6/src/vzg/jconv/test/conftest.py` & `vzg.jconv-1.2.7/src/vzg/jconv/test/conftest.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.6/src/vzg/jconv/test/test_jats_article.py` & `vzg.jconv-1.2.7/src/vzg/jconv/test/test_jats_article.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.6/src/vzg/jconv/test/test_jats_converter.py` & `vzg.jconv-1.2.7/src/vzg/jconv/test/test_jats_converter.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.6/src/vzg/jconv/test/test_jats_degruyter.py` & `vzg.jconv-1.2.7/src/vzg/jconv/test/test_jats_degruyter.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.6/src/vzg/jconv/test/test_jatsdate.py` & `vzg.jconv-1.2.7/src/vzg/jconv/test/test_jatsdate.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.6/src/vzg/jconv/test/test_journal.py` & `vzg.jconv-1.2.7/src/vzg/jconv/test/test_journal.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.6/src/vzg/jconv/test/test_langcode.py` & `vzg.jconv-1.2.7/src/vzg/jconv/test/test_langcode.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.6/src/vzg/jconv/test/test_person.py` & `vzg.jconv-1.2.7/src/vzg/jconv/test/test_person.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.6/src/vzg/jconv/test/test_publisher.py` & `vzg.jconv-1.2.7/src/vzg/jconv/test/test_publisher.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.6/src/vzg/jconv/tools/simple_conv.py` & `vzg.jconv-1.2.7/src/vzg/jconv/tools/simple_conv.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.6/src/vzg/jconv/utils/__init__.py` & `vzg.jconv-1.2.7/src/vzg/jconv/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.6/src/vzg/jconv/utils/date.py` & `vzg.jconv-1.2.7/src/vzg/jconv/utils/date.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.6/src/vzg.jconv.egg-info/SOURCES.txt` & `vzg.jconv-1.2.7/src/vzg.jconv.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/bw_matchbox-0.2.2.tar.gz` & `tmp/bw_matchbox-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_matchbox-0.2.2.tar", last modified: Tue Aug  1 12:30:23 2023, max compression
+gzip compressed data, was "bw_matchbox-0.2.3.tar", last modified: Wed Aug  2 20:58:42 2023, max compression
```

## Comparing `bw_matchbox-0.2.2.tar` & `bw_matchbox-0.2.3.tar`

### file list

```diff
@@ -1,62 +1,60 @@
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:30:23.156120 bw_matchbox-0.2.2/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1067 2023-06-20 12:26:53.000000 bw_matchbox-0.2.2/LICENSE
--rw-r--r--   0 chrismutel   (501) staff       (20)      216 2023-08-01 11:41:22.000000 bw_matchbox-0.2.2/MANIFEST.in
--rw-r--r--   0 chrismutel   (501) staff       (20)     6349 2023-08-01 12:30:23.156182 bw_matchbox-0.2.2/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)     5325 2023-08-01 07:10:26.000000 bw_matchbox-0.2.2/README.md
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:30:23.146602 bw_matchbox-0.2.2/bw_matchbox/
--rw-r--r--   0 chrismutel   (501) staff       (20)        6 2023-08-01 12:29:57.000000 bw_matchbox-0.2.2/bw_matchbox/VERSION
--rw-r--r--   0 chrismutel   (501) staff       (20)      215 2023-07-29 11:35:17.000000 bw_matchbox-0.2.2/bw_matchbox/__init__.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:30:23.144765 bw_matchbox-0.2.2/bw_matchbox/assets/
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:30:23.148184 bw_matchbox-0.2.2/bw_matchbox/assets/css/
--rw-r--r--   0 chrismutel   (501) staff       (20)     4955 2023-08-01 07:10:26.000000 bw_matchbox-0.2.2/bw_matchbox/assets/css/compare.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     1501 2023-08-01 07:10:26.000000 bw_matchbox-0.2.2/bw_matchbox/assets/css/customizations.css
--rw-r--r--   0 chrismutel   (501) staff       (20)      146 2023-08-01 07:10:26.000000 bw_matchbox-0.2.2/bw_matchbox/assets/css/layout.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     7618 2023-08-01 07:10:26.000000 bw_matchbox-0.2.2/bw_matchbox/assets/css/normalize.css
--rw-r--r--   0 chrismutel   (501) staff       (20)    11556 2023-08-01 07:10:26.000000 bw_matchbox-0.2.2/bw_matchbox/assets/css/skeleton.css
--rw-r--r--   0 chrismutel   (501) staff       (20)      916 2023-08-01 07:10:26.000000 bw_matchbox-0.2.2/bw_matchbox/assets/css/tooltip.css
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:30:23.148305 bw_matchbox-0.2.2/bw_matchbox/assets/images/
--rw-r--r--   0 chrismutel   (501) staff       (20)    32038 2023-06-20 12:27:44.000000 bw_matchbox-0.2.2/bw_matchbox/assets/images/favicon.ico
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:30:23.149133 bw_matchbox-0.2.2/bw_matchbox/assets/js/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1534 2023-08-01 07:10:26.000000 bw_matchbox-0.2.2/bw_matchbox/assets/js/common-helpers.js
--rw-r--r--   0 chrismutel   (501) staff       (20)    18008 2023-08-01 07:10:26.000000 bw_matchbox-0.2.2/bw_matchbox/assets/js/compare-core.js
--rw-r--r--   0 chrismutel   (501) staff       (20)      946 2023-08-01 07:10:26.000000 bw_matchbox-0.2.2/bw_matchbox/assets/js/compare-row-click.js
--rw-r--r--   0 chrismutel   (501) staff       (20)    10108 2023-08-01 07:10:26.000000 bw_matchbox-0.2.2/bw_matchbox/assets/js/compare-rows-helpers.js
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:30:23.151810 bw_matchbox-0.2.2/bw_matchbox/assets/templates/
--rw-r--r--   0 chrismutel   (501) staff       (20)     3929 2023-08-01 07:10:26.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/compare.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     2566 2023-07-23 12:42:57.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/databases.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      461 2023-07-23 15:09:13.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/expand.html
--rw-r--r--   0 chrismutel   (501) staff       (20)    11784 2023-06-20 12:27:44.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/file.html
--rw-r--r--   0 chrismutel   (501) staff       (20)       16 2023-06-20 12:27:44.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/footer.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     2336 2023-08-01 07:10:26.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/header.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     1751 2023-08-01 07:10:26.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/index.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      733 2023-06-21 04:56:26.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/match-status.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     1711 2023-06-21 09:42:53.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/match.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      798 2023-07-23 12:44:06.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/navigation.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     3536 2023-08-01 11:49:18.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/process_detail.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      599 2023-07-22 21:06:00.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/project.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      412 2023-08-01 07:10:26.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/search-embedded.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      850 2023-06-20 12:27:44.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/search.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      947 2023-06-20 12:27:44.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/search_result.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     1243 2023-07-23 08:33:52.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/select_files.html
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:30:23.152079 bw_matchbox-0.2.2/bw_matchbox/bin/
--rw-r--r--   0 chrismutel   (501) staff       (20)        0 2023-06-20 12:27:44.000000 bw_matchbox-0.2.2/bw_matchbox/bin/__init__.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2913 2023-08-01 07:14:42.000000 bw_matchbox-0.2.2/bw_matchbox/bin/matchbox.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:30:23.154140 bw_matchbox-0.2.2/bw_matchbox/data/
--rw-r--r--   0 chrismutel   (501) staff       (20)   123245 2023-06-13 11:22:50.000000 bw_matchbox-0.2.2/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
--rw-r--r--   0 chrismutel   (501) staff       (20)    93862 2023-07-23 09:30:53.000000 bw_matchbox-0.2.2/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
--rw-r--r--   0 chrismutel   (501) staff       (20)   116071 2023-06-13 11:23:32.000000 bw_matchbox-0.2.2/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
--rw-r--r--   0 chrismutel   (501) staff       (20)      603 2023-07-23 09:34:59.000000 bw_matchbox-0.2.2/bw_matchbox/data/dare.json
--rw-r--r--   0 chrismutel   (501) staff       (20)      346 2023-08-01 07:14:42.000000 bw_matchbox-0.2.2/bw_matchbox/utils.py
--rw-r--r--   0 chrismutel   (501) staff       (20)    20933 2023-08-01 07:14:48.000000 bw_matchbox-0.2.2/bw_matchbox/webapp.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:30:23.155315 bw_matchbox-0.2.2/bw_matchbox.egg-info/
--rw-r--r--   0 chrismutel   (501) staff       (20)     6349 2023-08-01 12:30:23.000000 bw_matchbox-0.2.2/bw_matchbox.egg-info/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)     3256 2023-08-01 12:30:23.000000 bw_matchbox-0.2.2/bw_matchbox.egg-info/SOURCES.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-08-01 12:30:23.000000 bw_matchbox-0.2.2/bw_matchbox.egg-info/dependency_links.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       59 2023-08-01 12:30:23.000000 bw_matchbox-0.2.2/bw_matchbox.egg-info/entry_points.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-07-23 07:30:31.000000 bw_matchbox-0.2.2/bw_matchbox.egg-info/not-zip-safe
--rw-r--r--   0 chrismutel   (501) staff       (20)      155 2023-08-01 12:30:23.000000 bw_matchbox-0.2.2/bw_matchbox.egg-info/requires.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       12 2023-08-01 12:30:23.000000 bw_matchbox-0.2.2/bw_matchbox.egg-info/top_level.txt
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:30:23.154376 bw_matchbox-0.2.2/docs/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1145 2023-07-23 07:23:19.000000 bw_matchbox-0.2.2/docs/conf.py
--rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-06-20 12:26:53.000000 bw_matchbox-0.2.2/pyproject.toml
--rw-r--r--   0 chrismutel   (501) staff       (20)     1862 2023-08-01 12:30:23.156547 bw_matchbox-0.2.2/setup.cfg
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 20:58:42.413441 bw_matchbox-0.2.3/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1067 2023-06-20 12:26:53.000000 bw_matchbox-0.2.3/LICENSE
+-rw-r--r--   0 chrismutel   (501) staff       (20)      216 2023-08-01 11:41:22.000000 bw_matchbox-0.2.3/MANIFEST.in
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6349 2023-08-02 20:58:42.413569 bw_matchbox-0.2.3/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5325 2023-08-01 07:10:26.000000 bw_matchbox-0.2.3/README.md
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 20:58:42.396561 bw_matchbox-0.2.3/bw_matchbox/
+-rw-r--r--   0 chrismutel   (501) staff       (20)        6 2023-08-02 20:57:58.000000 bw_matchbox-0.2.3/bw_matchbox/VERSION
+-rw-r--r--   0 chrismutel   (501) staff       (20)      215 2023-08-01 17:17:21.000000 bw_matchbox-0.2.3/bw_matchbox/__init__.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 20:58:42.394621 bw_matchbox-0.2.3/bw_matchbox/assets/
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 20:58:42.399222 bw_matchbox-0.2.3/bw_matchbox/assets/css/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2144 2023-08-02 20:57:45.000000 bw_matchbox-0.2.3/bw_matchbox/assets/css/common.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5022 2023-08-02 20:57:45.000000 bw_matchbox-0.2.3/bw_matchbox/assets/css/compare.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1501 2023-08-01 07:10:26.000000 bw_matchbox-0.2.3/bw_matchbox/assets/css/customizations.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)     7618 2023-08-01 07:10:26.000000 bw_matchbox-0.2.3/bw_matchbox/assets/css/normalize.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3320 2023-08-02 20:57:45.000000 bw_matchbox-0.2.3/bw_matchbox/assets/css/processes-list.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)    11556 2023-08-01 07:10:26.000000 bw_matchbox-0.2.3/bw_matchbox/assets/css/skeleton.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)      916 2023-08-01 07:10:26.000000 bw_matchbox-0.2.3/bw_matchbox/assets/css/tooltip.css
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 20:58:42.399584 bw_matchbox-0.2.3/bw_matchbox/assets/images/
+-rw-r--r--   0 chrismutel   (501) staff       (20)    32038 2023-06-20 12:27:44.000000 bw_matchbox-0.2.3/bw_matchbox/assets/images/favicon.ico
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 20:58:42.400144 bw_matchbox-0.2.3/bw_matchbox/assets/js/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4283 2023-08-02 20:57:45.000000 bw_matchbox-0.2.3/bw_matchbox/assets/js/CommonHelpers.js
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 20:58:42.406078 bw_matchbox-0.2.3/bw_matchbox/assets/templates/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4144 2023-08-02 20:57:45.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/compare.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2566 2023-07-23 12:42:57.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/databases.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      461 2023-07-23 15:09:13.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/expand.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)    11784 2023-06-20 12:27:44.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/file.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)       16 2023-06-20 12:27:44.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/footer.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2341 2023-08-02 20:57:45.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/header.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4135 2023-08-02 20:57:45.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/index.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      733 2023-06-21 04:56:26.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/match-status.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1711 2023-06-21 09:42:53.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/match.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      798 2023-07-23 12:44:06.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/navigation.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3536 2023-08-01 11:49:18.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/process_detail.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      599 2023-07-22 21:06:00.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/project.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      412 2023-08-01 07:10:26.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/search-embedded.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      850 2023-06-20 12:27:44.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/search.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      947 2023-06-20 12:27:44.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/search_result.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1243 2023-07-23 08:33:52.000000 bw_matchbox-0.2.3/bw_matchbox/assets/templates/select_files.html
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 20:58:42.406568 bw_matchbox-0.2.3/bw_matchbox/bin/
+-rw-r--r--   0 chrismutel   (501) staff       (20)        0 2023-06-20 12:27:44.000000 bw_matchbox-0.2.3/bw_matchbox/bin/__init__.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2931 2023-08-01 17:17:21.000000 bw_matchbox-0.2.3/bw_matchbox/bin/matchbox.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 20:58:42.409586 bw_matchbox-0.2.3/bw_matchbox/data/
+-rw-r--r--   0 chrismutel   (501) staff       (20)   123246 2023-08-01 17:17:21.000000 bw_matchbox-0.2.3/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)    93862 2023-07-23 09:30:53.000000 bw_matchbox-0.2.3/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)   116072 2023-08-01 17:17:21.000000 bw_matchbox-0.2.3/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)      603 2023-07-23 09:34:59.000000 bw_matchbox-0.2.3/bw_matchbox/data/dare.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1388 2023-08-01 17:17:21.000000 bw_matchbox-0.2.3/bw_matchbox/utils.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)    20517 2023-08-01 17:17:21.000000 bw_matchbox-0.2.3/bw_matchbox/webapp.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 20:58:42.412288 bw_matchbox-0.2.3/bw_matchbox.egg-info/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6349 2023-08-02 20:58:42.000000 bw_matchbox-0.2.3/bw_matchbox.egg-info/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3080 2023-08-02 20:58:42.000000 bw_matchbox-0.2.3/bw_matchbox.egg-info/SOURCES.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-08-02 20:58:42.000000 bw_matchbox-0.2.3/bw_matchbox.egg-info/dependency_links.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       59 2023-08-02 20:58:42.000000 bw_matchbox-0.2.3/bw_matchbox.egg-info/entry_points.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-07-23 07:30:31.000000 bw_matchbox-0.2.3/bw_matchbox.egg-info/not-zip-safe
+-rw-r--r--   0 chrismutel   (501) staff       (20)      167 2023-08-02 20:58:42.000000 bw_matchbox-0.2.3/bw_matchbox.egg-info/requires.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       12 2023-08-02 20:58:42.000000 bw_matchbox-0.2.3/bw_matchbox.egg-info/top_level.txt
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 20:58:42.410283 bw_matchbox-0.2.3/docs/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1145 2023-07-23 07:23:19.000000 bw_matchbox-0.2.3/docs/conf.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-06-20 12:26:53.000000 bw_matchbox-0.2.3/pyproject.toml
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1881 2023-08-02 20:58:42.414655 bw_matchbox-0.2.3/setup.cfg
```

### Comparing `bw_matchbox-0.2.2/LICENSE` & `bw_matchbox-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.2/PKG-INFO` & `bw_matchbox-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_matchbox
-Version: 0.2.2
+Version: 0.2.3
 Summary: Browser to match Brightway databases
 Home-page: https://github.com/cauldron/bw_matchbox
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: MIT
```

### Comparing `bw_matchbox-0.2.2/README.md` & `bw_matchbox-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.2/bw_matchbox/assets/css/compare.css` & `bw_matchbox-0.2.3/bw_matchbox/assets/css/compare.css`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,45 @@
-/* stylelint-disable declaration-block-single-line-max-declarations, declaration-colon-space-after */
+/* stylelint-disable
+    declaration-block-single-line-max-declarations
+    declaration-colon-space-after
+ */
 
 :root {
-  --compare-collapsed-color: #f60;
-  --compare-collapsed-bg-color: rgb(255 102 0 / 10%);
-  --compare-selected-color: #1eaedb;
+  /* // UNUSED: Collapsed rows are just hidden.
+   * --compare-collapsed-color: #F60;
+   * --compare-collapsed-bg-color: rgba(255,102,0,.1);
+   */
+  --compare-selected-color: var(--layout-theme-primary-color-dark1); /* #1EAEDB; */
   --compare-selected-bg-color05: rgb(30 174 219 / 5%);
   --compare-selected-bg-color1: rgb(30 174 219 / 10%);
   --compare-selected-bg-color2: rgb(30 174 219 / 20%);
   --compare-selected-bg-color3: rgb(30 174 219 / 30%);
   --compare-selected-bg-color4: rgb(30 174 219 / 40%);
   --compare-selected-bg-color5: rgb(30 174 219 / 50%);
-  --compare-animation-time: 250ms;
+  --compare-animation-time: var(--common-animation-time);
   --compare-selected-animation-time: 3s;
   --compare-td-padding-h-at-edges: 8px;
   --compare-td-padding-h: 4px;
   --compare-td-padding-v: 8px;
 }
 
 .compare .compare-tables {
   width: 100%;
 }
 
 .compare .compare-tables > .column {
-  /* DEBUG */
-
-  /* border: 2px solid red; */
-
-  /* overflow: hidden; */
   position: relative;
 }
 
 .compare .compare-tables > .column + .column {
   /* Tables spacing */
   margin-left: 15px;
 }
 
 .compare .compare-tables > .column > table {
-  /* DEBUG */
-
-  /* border: 1px solid green; */
   border: 0;
   table-layout: fixed;
   width: 100%;
   border-style: solid;
 
   /* word-break: break-all; */
 }
@@ -176,18 +173,18 @@
   /* Remove nested td borders */
   border-color: transparent;
 }
 
 /* Collapsed row... */
 
 .compare-table tr.collapsed {
-  box-shadow:
-    0 0 4px var(--compare-collapsed-color),
-    inset 0 0 2px var(--compare-collapsed-color);
-  background-color: var(--compare-collapsed-bg-color);
+  /* // UNUSED: Collapsed rows are just hidden.
+   * box-shadow: 0 0 4px var(--compare-collapsed-color), inset 0 0 2px var(--compare-collapsed-color);
+   * background-color: var(--compare-collapsed-bg-color);
+   */
   display: none;
 }
 
 .compare-table tr.collapsed-handler {
   /* box-shadow: 0 0 4px var(--compare-selected-bg-color5), inset 0 0 4px var(--compare-selected-bg-color5); */
   cursor: pointer;
   background: var(--compare-selected-bg-color1);
```

### Comparing `bw_matchbox-0.2.2/bw_matchbox/assets/css/customizations.css` & `bw_matchbox-0.2.3/bw_matchbox/assets/css/customizations.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.2/bw_matchbox/assets/css/normalize.css` & `bw_matchbox-0.2.3/bw_matchbox/assets/css/normalize.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.2/bw_matchbox/assets/css/skeleton.css` & `bw_matchbox-0.2.3/bw_matchbox/assets/css/skeleton.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.2/bw_matchbox/assets/css/tooltip.css` & `bw_matchbox-0.2.3/bw_matchbox/assets/css/tooltip.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.2/bw_matchbox/assets/images/favicon.ico` & `bw_matchbox-0.2.3/bw_matchbox/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.2/bw_matchbox/assets/templates/compare.html` & `bw_matchbox-0.2.3/bw_matchbox/assets/templates/compare.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 {% include 'header.html' %}
 
 <link rel="stylesheet" href="{{ url_for('static', filename='css/compare.css') }}">
 
-<script src="{{ url_for('static', filename='js/compare-rows-helpers.js') }}"></script>
-<script src="{{ url_for('static', filename='js/compare-row-click.js') }}"></script>
-<script src="{{ url_for('static', filename='js/compare-core.js') }}"></script>
+<script src="{{ url_for('static', filename='js/Compare/CompareRowsHelpers.js') }}"></script>
+<script src="{{ url_for('static', filename='js/Compare/CompareRowClick.js') }}"></script>
+<script src="{{ url_for('static', filename='js/Compare/CompareCore.js') }}"></script>
+
+{# Globals:
+  - `CompareCore` (from `bw_matchbox/assets/js/compare-core.js`)
+#}
 
 <div class="container compare">
   {% include 'navigation.html' %}
   <span class="modal-wrapper">
     <div class="modal" id="number-editor">
       <div class="modal-content">
         <span class="close">&times;</span>
@@ -31,27 +35,26 @@
   <div class="row compare-tables">
     <div class="column one-half">
       <h3>{{ source_node.name }}</h3>
       <table class="compare-table" id="source-table" width="100%">
       </table>
     </div>
     <div class="column one-half">
-      <h3>{{ target_node.name }} <span onclick="compareCore.replaceWithTarget(this)"><a><i class="fa-solid fa-arrow-up"></i></a></span></h3>
+      <h3>{{ target_node.name }} <span onclick="CompareCore.replaceWithTarget(this)"><a><i class="fa-solid fa-arrow-up"></i></a></span></h3>
       <table class="compare-table" id="target-table" width="100%">
       </table>
     </div>
   </div>
 </div>
 
 <script>
 
-  // const useDebug = true; // DEBUG!
-
-  // Globals:
-  // - `compareCore` (from `bw_matchbox/assets/js/compare-core.js`)
+  /* // Enable debug mode...
+   * const useDebug = true;
+   */
 
   /* // Common types (ts-like):
    *
    * Data record item (for `source_data` and `target_data` tables):
    *
    * interface TDataRecord {
    *   amount: number; // Eg: 7.135225509515751e-9
@@ -76,14 +79,21 @@
     source_id: {{ source_node.id }},
     target_id: {{ target_node.id }},
     target_name: '{{ target_node.name|safe }}',
     source_node_unit: '{{source_node.unit}}',
     source_node_location: '{{source_node.location}}',
   };
 
+  /* // DEBUG: Crop data table to easier debugging...
+   * if (useDebug) {
+   *   sharedData.source_data.length = 2;
+   *   sharedData.target_data.length = 2;
+   * }
+   */
+
   /* // DEBUG: Emulate pre-collapsed elements data...
    * if (useDebug) {
    *   // Link first columns...
    *   const collapsedGroupId = 'Collapsed-0-abcdef'
    *   sharedData.source_data[0].collapsed = true
    *   sharedData.source_data[0]['collapsed-group'] = collapsedGroupId;
    *   sharedData.target_data[0].collapsed = true
@@ -92,11 +102,11 @@
    *     source_data: sharedData.source_data,
    *     target_data: sharedData.target_data,
    *   });
    *   debugger;
    * }
    */
 
-  compareCore.initCompare(sharedData);
+  CompareCore.initCompare(sharedData);
 
 </script>
 {% include 'footer.html' %}
```

#### html2text {}

```diff
@@ -1,8 +1,9 @@
 {% include 'header.html' %}
+ {# Globals: - `CompareCore` (from `bw_matchbox/assets/js/compare-core.js`) #}
 {% include 'navigation.html' %}
 × Number Editor
 *** Location: {% if source_node.location == target_node.location %}Same{% else
 %}{{ source_node.location }} | {{ target_node.location }}{% endif %} ***
 *** Unit: {% if source_node.unit == target_node.unit %}Same{% else %}{
 { source_node.unit }} | {{ target_node.unit }}{% endif %} ***
 {% if proxy and proxy != "None" %}Create Proxy 1-to-1 Proxy{% else %}Save{%
```

### Comparing `bw_matchbox-0.2.2/bw_matchbox/assets/templates/databases.html` & `bw_matchbox-0.2.3/bw_matchbox/assets/templates/databases.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.2/bw_matchbox/assets/templates/file.html` & `bw_matchbox-0.2.3/bw_matchbox/assets/templates/file.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.2/bw_matchbox/assets/templates/header.html` & `bw_matchbox-0.2.3/bw_matchbox/assets/templates/header.html`

 * *Files 7% similar despite different names*

```diff
@@ -23,19 +23,20 @@
 
   <!-- CSS
   –––––––––––––––––––––––––––––––––––––––––––––––––– -->
   <link rel="stylesheet" href="{{ url_for('static', filename='css/normalize.css') }}">
   <link rel="stylesheet" href="{{ url_for('static', filename='css/tooltip.css') }}">
   <link rel="stylesheet" href="{{ url_for('static', filename='css/skeleton.css') }}">
   <link rel="stylesheet" href="{{ url_for('static', filename='css/customizations.css') }}">
-  <link rel="stylesheet" href="{{ url_for('static', filename='css/layout.css') }}">
+  <link rel="stylesheet" href="{{ url_for('static', filename='css/common.css') }}">
 
-  <!-- Scripts (TODO: to move to the body end?)
+  <!-- Scripts
   –––––––––––––––––––––––––––––––––––––––––––––––––– -->
-  <script src="{{ url_for('static', filename='js/common-helpers.js') }}"></script>
+  <script src="{{ url_for('static', filename='js/CommonHelpers.js') }}"></script>
+  {# TODO: to move to the body end? #}
 
   <!-- Favicon
   –––––––––––––––––––––––––––––––––––––––––––––––––– -->
   <link rel="icon" type="image/png" href="{{ url_for('static', filename='images/favicon.ico') }}">
 
 </head>
 <body>
```

#### html2text {}

```diff
@@ -5,8 +5,8 @@
 
 
 
 
 
 
 
-
+ {# TODO: to move to the body end? #}
```

### Comparing `bw_matchbox-0.2.2/bw_matchbox/assets/templates/match-status.html` & `bw_matchbox-0.2.3/bw_matchbox/assets/templates/match-status.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.2/bw_matchbox/assets/templates/match.html` & `bw_matchbox-0.2.3/bw_matchbox/assets/templates/match.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.2/bw_matchbox/assets/templates/navigation.html` & `bw_matchbox-0.2.3/bw_matchbox/assets/templates/navigation.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.2/bw_matchbox/assets/templates/process_detail.html` & `bw_matchbox-0.2.3/bw_matchbox/assets/templates/process_detail.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.2/bw_matchbox/assets/templates/project.html` & `bw_matchbox-0.2.3/bw_matchbox/assets/templates/project.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.2/bw_matchbox/assets/templates/search.html` & `bw_matchbox-0.2.3/bw_matchbox/assets/templates/search.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.2/bw_matchbox/assets/templates/search_result.html` & `bw_matchbox-0.2.3/bw_matchbox/assets/templates/search_result.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.2/bw_matchbox/assets/templates/select_files.html` & `bw_matchbox-0.2.3/bw_matchbox/assets/templates/select_files.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.2/bw_matchbox/bin/matchbox.py` & `bw_matchbox-0.2.3/bw_matchbox/bin/matchbox.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,22 +8,23 @@
   matchbox webapp <config> [--port=<port>] [--localhost]
 
 Options:
   -h --help     Show this screen.
   --version     Show version.
 
 """
-from bw_matchbox.webapp import matchbox_app, configure_app
-from docopt import docopt
+import datetime
+import json
 from pathlib import Path
+
 import bw2data as bd
 import bw2io as bi
-import datetime
-import json
+from docopt import docopt
 
+from bw_matchbox.webapp import configure_app, matchbox_app
 
 CWD = Path.cwd()
 
 CONFIG_TEMPLATE = """[users]
 johnny = "mnemonic"
 
 [files]
@@ -80,15 +81,16 @@
         create_setup_files("config.toml", "changes.json")
     elif args["example_project"]:
         name = args["<project_name>"] or "matchbox-example"
         bi.install_project("USEEIO-1.1", name)
         bd.projects.set_current(name)
         bd.Database("USEEIO-1.1").copy("USEEIO-copy")
         print(
-            f"Create project {name}. Make sure to select `USEEIO-1.1` for one database and `USEEIO-copy` for the other."
+            f"Create project {name}. Make sure to select `USEEIO-1.1` for one "
+            + "database and `USEEIO-copy` for the other."
         )
     elif args["webapp"]:
         filepath = args["<config>"]
         port = int(args.get("--port", False) or 5000)
         host = "localhost" if args.get("--localhost", False) else "0.0.0.0"
 
         try:
```

### Comparing `bw_matchbox-0.2.2/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json` & `bw_matchbox-0.2.3/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -7696,8 +7696,8 @@
 0001e0f0: 6e61 6d65 223a 2022 676f 6c64 206d 696e  name": "gold min
 0001e100: 6520 6f70 6572 6174 696f 6e20 616e 6420  e operation and 
 0001e110: 7265 6669 6e69 6e67 222c 0a20 2020 2020  refining",.     
 0001e120: 2020 2022 7265 6665 7265 6e63 6520 7072     "reference pr
 0001e130: 6f64 7563 7422 3a20 227a 696e 6322 2c0a  oduct": "zinc",.
 0001e140: 2020 2020 2020 2020 2261 6c6c 6f63 6174          "allocat
 0001e150: 696f 6e22 3a20 312e 300a 2020 2020 2020  ion": 1.0.      
-0001e160: 7d0a 2020 2020 7d0a 2020 5d0a 7d         }.    }.  ].}
+0001e160: 7d0a 2020 2020 7d0a 2020 5d0a 7d0a       }.    }.  ].}.
```

### Comparing `bw_matchbox-0.2.2/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json` & `bw_matchbox-0.2.3/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.2/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json` & `bw_matchbox-0.2.3/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -7248,8 +7248,8 @@
 0001c4f0: 6661 6374 6f72 7920 636f 6e73 7472 7563  factory construc
 0001c500: 7469 6f6e 222c 0a20 2020 2020 2020 2022  tion",.        "
 0001c510: 756e 6974 223a 2022 756e 6974 222c 0a20  unit": "unit",. 
 0001c520: 2020 2020 2020 2022 7265 6665 7265 6e63         "referenc
 0001c530: 6520 7072 6f64 7563 7422 3a20 2273 796e  e product": "syn
 0001c540: 7468 6574 6963 2067 6173 2066 6163 746f  thetic gas facto
 0001c550: 7279 220a 2020 2020 2020 7d0a 2020 2020  ry".      }.    
-0001c560: 7d0a 2020 5d0a 7d                        }.  ].}
+0001c560: 7d0a 2020 5d0a 7d0a                      }.  ].}.
```

### Comparing `bw_matchbox-0.2.2/bw_matchbox/data/dare.json` & `bw_matchbox-0.2.3/bw_matchbox/data/dare.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.2/bw_matchbox/webapp.py` & `bw_matchbox-0.2.3/bw_matchbox/webapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from functools import total_ordering
-from bw2data.backends import ActivityDataset as AD
-from flask_httpauth import HTTPBasicAuth
-from pathlib import Path
-from peewee import fn
-from werkzeug.security import check_password_hash, generate_password_hash
-import bw2data as bd
-import flask
 import json
 import math
 import os
 import random
 import string
-import tomli
 import uuid
+from pathlib import Path
 
+import bw2data as bd
+import flask
+import tomli
+from bw2data.backends import ActivityDataset as AD
+from flask_httpauth import HTTPBasicAuth
+from peewee import fn
+from werkzeug.security import check_password_hash, generate_password_hash
+
+from .utils import name_close_enough, similar_location
 
 BASE_DIR = Path(__file__).resolve().parent
 DATA_DIR = BASE_DIR / "data"
 
 matchbox_app = flask.Flask(
     "matchbox_app",
     static_folder=BASE_DIR / "assets",
@@ -247,21 +248,23 @@
 @matchbox_app.route("/processes", methods=["GET"])
 @auth.login_required
 def processes():
     """API Endpoint to get process data for dynamic table population.
 
     GET args:
 
-        * database (str): Name of database to draw processes from. Defaults to source database (stored in cookie) if not given.
-        * order_by (str): Parameter to sort by. Random if not provided. Valid parameters:
-            * name (will be used 99% of the time)
-            * location
-            * product (short name for reference product)
-        * offset (int): Offset from beginning of sorted values. Zero-indexed. Only used if sorting.
-        * limit (int): Number of results to return
+    * database (str): Name of database to draw processes from. Defaults to source
+                      database (stored in cookie) if not given.
+    * order_by (str): Parameter to sort by. Random if not provided. Valid parameters:
+        * name (will be used 99% of the time)
+        * location
+        * product (short name for reference product)
+    * offset (int): Offset from beginning of sorted values. Zero-indexed.
+                    Only used if sorting.
+    * limit (int): Number of results to return
 
     Response data format (JSON):
 
     ```
         [
             {
                 'details_url': 'URL for `process_detail` page for this activity',
@@ -359,15 +362,16 @@
 #             data = json.load(open(filename))
 #             for key in OPERATIONS:
 #                 for elem in data.get(key, []):
 #                     lookup = frozendict(elem['source'])
 #                     value = frozendict(elem['target'])
 #                     file_status['count'] += 1
 #                     if lookup in crud and crud.get(lookup) != value:
-#                         error = "Source: {}. Already have: {}. Given: {}".format(dict(lookup), dict(crud[lookup]), dict(value))
+#                         error = "Source: {}. Already have: {}. Given: {}".format(
+#                            dict(lookup), dict(crud[lookup]), dict(value))
 #                         if error not in file_status['duplicates']:
 #                             file_status['duplicates'].append(error)
 #                     else:
 #                         crud[lookup] = value
 #             status[filename.name] = file_status
 #         except:
 #             failed.append(filename.name)
@@ -491,41 +495,20 @@
         user=auth.current_user(),
         changes_file=Path(matchbox_app.config["mb_changes_file"]).name,
         query_string=node["name"] + " " + node.get("location", ""),
         matches=matches,
     )
 
 
-def normalize_name(string):
-    return (
-        string.lower()
-        .replace("market group for", "")
-        .replace("market for", "")
-        .replace(", at plant", "")
-        .strip()
-    )
-
-
-def similar_location(a, b):
-    return any(
-        [
-            (b == a),
-            (b == "CH" and a in ("CH", "RER", "GLO", "RoW")),
-            (len(b) == 2 and a in ("GLO", "RoW")),
-            (b == "RER" and a in ("GLO", "RoW", "RoE")),
-        ]
-    )
-
-
 def check_similar(node, candidates):
     for index, candidate in enumerate(candidates):
         if node.get("collapsed") or candidate.get("collapsed"):
             continue
         if (
-            normalize_name(node["name"]) == normalize_name(candidate["name"])
+            name_close_enough(node["name"], candidate["name"])
             and similar_location(node["location"], candidate["location"])
             and node["unit"] == candidate["unit"]
             and math.isclose(
                 node["amount"], candidate["amount"], rel_tol=0.025, abs_tol=1e-6
             )
         ):
             node["collapsed"] = candidate["collapsed"] = True
```

### Comparing `bw_matchbox-0.2.2/bw_matchbox.egg-info/PKG-INFO` & `bw_matchbox-0.2.3/bw_matchbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw-matchbox
-Version: 0.2.2
+Version: 0.2.3
 Summary: Browser to match Brightway databases
 Home-page: https://github.com/cauldron/bw_matchbox
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: MIT
```

### Comparing `bw_matchbox-0.2.2/bw_matchbox.egg-info/SOURCES.txt` & `bw_matchbox-0.2.3/bw_matchbox.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,23 @@
 README.md
 pyproject.toml
 setup.cfg
 ./bw_matchbox/VERSION
 ./bw_matchbox/__init__.py
 ./bw_matchbox/utils.py
 ./bw_matchbox/webapp.py
+./bw_matchbox/assets/css/common.css
 ./bw_matchbox/assets/css/compare.css
 ./bw_matchbox/assets/css/customizations.css
-./bw_matchbox/assets/css/layout.css
 ./bw_matchbox/assets/css/normalize.css
+./bw_matchbox/assets/css/processes-list.css
 ./bw_matchbox/assets/css/skeleton.css
 ./bw_matchbox/assets/css/tooltip.css
 ./bw_matchbox/assets/images/favicon.ico
-./bw_matchbox/assets/js/common-helpers.js
-./bw_matchbox/assets/js/compare-core.js
-./bw_matchbox/assets/js/compare-row-click.js
-./bw_matchbox/assets/js/compare-rows-helpers.js
+./bw_matchbox/assets/js/CommonHelpers.js
 ./bw_matchbox/assets/templates/compare.html
 ./bw_matchbox/assets/templates/databases.html
 ./bw_matchbox/assets/templates/expand.html
 ./bw_matchbox/assets/templates/file.html
 ./bw_matchbox/assets/templates/footer.html
 ./bw_matchbox/assets/templates/header.html
 ./bw_matchbox/assets/templates/index.html
@@ -45,25 +43,23 @@
 bw_matchbox.egg-info/PKG-INFO
 bw_matchbox.egg-info/SOURCES.txt
 bw_matchbox.egg-info/dependency_links.txt
 bw_matchbox.egg-info/entry_points.txt
 bw_matchbox.egg-info/not-zip-safe
 bw_matchbox.egg-info/requires.txt
 bw_matchbox.egg-info/top_level.txt
+bw_matchbox/assets/css/common.css
 bw_matchbox/assets/css/compare.css
 bw_matchbox/assets/css/customizations.css
-bw_matchbox/assets/css/layout.css
 bw_matchbox/assets/css/normalize.css
+bw_matchbox/assets/css/processes-list.css
 bw_matchbox/assets/css/skeleton.css
 bw_matchbox/assets/css/tooltip.css
 bw_matchbox/assets/images/favicon.ico
-bw_matchbox/assets/js/common-helpers.js
-bw_matchbox/assets/js/compare-core.js
-bw_matchbox/assets/js/compare-row-click.js
-bw_matchbox/assets/js/compare-rows-helpers.js
+bw_matchbox/assets/js/CommonHelpers.js
 bw_matchbox/assets/templates/compare.html
 bw_matchbox/assets/templates/databases.html
 bw_matchbox/assets/templates/expand.html
 bw_matchbox/assets/templates/file.html
 bw_matchbox/assets/templates/footer.html
 bw_matchbox/assets/templates/header.html
 bw_matchbox/assets/templates/index.html
```

### Comparing `bw_matchbox-0.2.2/docs/conf.py` & `bw_matchbox-0.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.2/setup.cfg` & `bw_matchbox-0.2.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 	=.
 python_requires = >=3.8
 install_requires = 
 	brightway25
 	docopt-ng
 	flask
 	flask_httpauth
+	levenshtein
 	tomli
 	werkzeug
 
 [options.packages.find]
 where = .
 exclude = 
 	tests
@@ -84,15 +85,15 @@
 
 [devpi:upload]
 no_vcs = 1
 formats = bdist_wheel
 
 [flake8]
 max_line_length = 88
-extend_ignore = E203, W503
+extend_ignore = E203, W503, E722
 exclude = 
 	.tox
 	build
 	dist
 	.eggs
 	docs/conf.py
```


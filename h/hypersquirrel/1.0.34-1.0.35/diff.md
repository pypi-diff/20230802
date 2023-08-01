# Comparing `tmp/hypersquirrel-1.0.34.tar.gz` & `tmp/hypersquirrel-1.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypersquirrel-1.0.34.tar", last modified: Tue Aug  1 22:24:20 2023, max compression
+gzip compressed data, was "hypersquirrel-1.0.35.tar", last modified: Tue Aug  1 22:54:15 2023, max compression
```

## Comparing `hypersquirrel-1.0.34.tar` & `hypersquirrel-1.0.35.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:24:20.016209 hypersquirrel-1.0.34/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-01 22:24:20.016209 hypersquirrel-1.0.34/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:24:20.012209 hypersquirrel-1.0.34/hypersquirrel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:24:20.012209 hypersquirrel-1.0.34/hypersquirrel/literalinterpreter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/literalinterpreter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/literalinterpreter/ehen.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/literalinterpreter/instagram.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/literalinterpreter/ph.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/literalinterpreterfactory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:24:20.016209 hypersquirrel-1.0.34/hypersquirrel/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/scraper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/scraper/buondua.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/scraper/cosplayporntube.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/scraper/drts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/scraper/ehen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/scraper/fseg.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/scraper/googleimagesearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/scraper/hcos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/scraper/hellp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/scraper/hnlg.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/scraper/lgbb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/scraper/nh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/scraper/nlgs.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/scraper/opendir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/scraper/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/scraper/sb.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/scraper/sbgx.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/scraper/v2ph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/scraper/vg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/scraper/xh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/scraper/xv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/scraper/youtubeapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/scraperfactory.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/hypersquirrel/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:24:20.012209 hypersquirrel-1.0.34/hypersquirrel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-01 22:24:19.000000 hypersquirrel-1.0.34/hypersquirrel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-08-01 22:24:20.000000 hypersquirrel-1.0.34/hypersquirrel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 22:24:19.000000 hypersquirrel-1.0.34/hypersquirrel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 22:24:19.000000 hypersquirrel-1.0.34/hypersquirrel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 22:24:19.000000 hypersquirrel-1.0.34/hypersquirrel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 22:24:20.016209 hypersquirrel-1.0.34/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:24:20.016209 hypersquirrel-1.0.34/ytdlwrapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/ytdlwrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-01 22:24:04.000000 hypersquirrel-1.0.34/ytdlwrapper/ytdlpscrape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:54:15.115794 hypersquirrel-1.0.35/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-01 22:54:15.115794 hypersquirrel-1.0.35/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:54:15.111794 hypersquirrel-1.0.35/hypersquirrel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:54:15.115794 hypersquirrel-1.0.35/hypersquirrel/literalinterpreter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/literalinterpreter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/literalinterpreter/ehen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/literalinterpreter/instagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/literalinterpreter/ph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/literalinterpreterfactory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:54:15.115794 hypersquirrel-1.0.35/hypersquirrel/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/scraper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/scraper/buondua.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/scraper/cosplayporntube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/scraper/drts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/scraper/ehen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/scraper/fseg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/scraper/googleimagesearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/scraper/hcos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/scraper/hellp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/scraper/hnlg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/scraper/lgbb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/scraper/nh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/scraper/nlgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/scraper/opendir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/scraper/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/scraper/sb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/scraper/sbgx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/scraper/v2ph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/scraper/vg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/scraper/xh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/scraper/xv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/scraper/youtubeapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/scraperfactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/hypersquirrel/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:54:15.115794 hypersquirrel-1.0.35/hypersquirrel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-01 22:54:15.000000 hypersquirrel-1.0.35/hypersquirrel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-08-01 22:54:15.000000 hypersquirrel-1.0.35/hypersquirrel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 22:54:15.000000 hypersquirrel-1.0.35/hypersquirrel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 22:54:15.000000 hypersquirrel-1.0.35/hypersquirrel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 22:54:15.000000 hypersquirrel-1.0.35/hypersquirrel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 22:54:15.115794 hypersquirrel-1.0.35/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:54:15.115794 hypersquirrel-1.0.35/ytdlwrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/ytdlwrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-01 22:54:02.000000 hypersquirrel-1.0.35/ytdlwrapper/ytdlpscrape.py
```

### Comparing `hypersquirrel-1.0.34/LICENSE` & `hypersquirrel-1.0.35/LICENSE`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.34/PKG-INFO` & `hypersquirrel-1.0.35/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypersquirrel
-Version: 1.0.34
+Version: 1.0.35
 Summary: Scrapes posts from various websites
 Home-page: UNKNOWN
 Author: vka
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `hypersquirrel-1.0.34/hypersquirrel/core.py` & `hypersquirrel-1.0.35/hypersquirrel/core.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.34/hypersquirrel/entry.py` & `hypersquirrel-1.0.35/hypersquirrel/entry.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.34/hypersquirrel/literalinterpreterfactory.py` & `hypersquirrel-1.0.35/hypersquirrel/literalinterpreterfactory.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.34/hypersquirrel/scraper/buondua.py` & `hypersquirrel-1.0.35/hypersquirrel/scraper/buondua.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.34/hypersquirrel/scraper/cosplayporntube.py` & `hypersquirrel-1.0.35/hypersquirrel/scraper/cosplayporntube.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.34/hypersquirrel/scraper/drts.py` & `hypersquirrel-1.0.35/hypersquirrel/scraper/drts.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.34/hypersquirrel/scraper/ehen.py` & `hypersquirrel-1.0.35/hypersquirrel/scraper/ehen.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.34/hypersquirrel/scraper/fseg.py` & `hypersquirrel-1.0.35/hypersquirrel/scraper/fseg.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.34/hypersquirrel/scraper/hcos.py` & `hypersquirrel-1.0.35/hypersquirrel/scraper/hcos.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.34/hypersquirrel/scraper/hellp.py` & `hypersquirrel-1.0.35/hypersquirrel/scraper/hellp.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.34/hypersquirrel/scraper/hnlg.py` & `hypersquirrel-1.0.35/hypersquirrel/scraper/hnlg.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.34/hypersquirrel/scraper/lgbb.py` & `hypersquirrel-1.0.35/hypersquirrel/scraper/lgbb.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.34/hypersquirrel/scraper/nh.py` & `hypersquirrel-1.0.35/hypersquirrel/scraper/nh.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.34/hypersquirrel/scraper/nlgs.py` & `hypersquirrel-1.0.35/hypersquirrel/scraper/nlgs.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.34/hypersquirrel/scraper/reddit.py` & `hypersquirrel-1.0.35/hypersquirrel/scraper/reddit.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.34/hypersquirrel/scraper/sb.py` & `hypersquirrel-1.0.35/hypersquirrel/scraper/sb.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.34/hypersquirrel/scraper/sbgx.py` & `hypersquirrel-1.0.35/hypersquirrel/scraper/sbgx.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.34/hypersquirrel/scraper/v2ph.py` & `hypersquirrel-1.0.35/hypersquirrel/scraper/v2ph.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.34/hypersquirrel/scraper/vg.py` & `hypersquirrel-1.0.35/hypersquirrel/scraper/vg.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.34/hypersquirrel/scraper/xh.py` & `hypersquirrel-1.0.35/hypersquirrel/scraper/xh.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 from commmons import html_from_url
 from lxml import html
 from pydash import head
 
 from hypersquirrel.core import Watchlist
 
 
-def get_url_and_filename(root, fileid):
-    atag = root.xpath(f"//div[@data-video-id='{fileid}']/div/a")[0]
-    url = atag.attrib["href"]
-    return url, atag.text
-
-
 def get_divs_with_fileid(root):
     divs = root.xpath("//div[contains(@class, 'video-thumb')]")
     for div in divs:
         fileid = div.attrib.get("data-video-id")
         if fileid:
             yield div
 
 
 def _scrape(root):
     for div in get_divs_with_fileid(root):
         fileid = div.attrib.get("data-video-id")
-        sourceurl, filename = get_url_and_filename(div, fileid)
-        thumbnailurl = div.xpath(".//img")[0].attrib["src"]
+        sourceurl = head(root.xpath(f"//div[@data-video-id='{fileid}']/div/a")).attrib["href"]
+        img = head(div.xpath(".//img"))
         yield {
             "fileid": f"xh{fileid}",
             "sourceurl": sourceurl,
-            "filename": filename,
-            "thumbnailurl": thumbnailurl
+            "filename": img.attrib["alt"],
+            "thumbnailurl": img.attrib["src"]
         }
 
 
 def scrape(url):
     root = html_from_url(url)
     yield from _scrape(root)
```

### Comparing `hypersquirrel-1.0.34/hypersquirrel/scraper/xv.py` & `hypersquirrel-1.0.35/hypersquirrel/scraper/xv.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.34/hypersquirrel/scraper/youtubeapi.py` & `hypersquirrel-1.0.35/hypersquirrel/scraper/youtubeapi.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.34/hypersquirrel/scraperfactory.py` & `hypersquirrel-1.0.35/hypersquirrel/scraperfactory.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.34/hypersquirrel/util.py` & `hypersquirrel-1.0.35/hypersquirrel/util.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.34/hypersquirrel.egg-info/PKG-INFO` & `hypersquirrel-1.0.35/hypersquirrel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypersquirrel
-Version: 1.0.34
+Version: 1.0.35
 Summary: Scrapes posts from various websites
 Home-page: UNKNOWN
 Author: vka
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `hypersquirrel-1.0.34/hypersquirrel.egg-info/SOURCES.txt` & `hypersquirrel-1.0.35/hypersquirrel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.34/setup.py` & `hypersquirrel-1.0.35/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hypersquirrel",
-    version="v1.0.34",
+    version="v1.0.35",
     author="vka",
     description="Scrapes posts from various websites",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=("test",)),
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `hypersquirrel-1.0.34/ytdlwrapper/ytdlpscrape.py` & `hypersquirrel-1.0.35/ytdlwrapper/ytdlpscrape.py`

 * *Files identical despite different names*


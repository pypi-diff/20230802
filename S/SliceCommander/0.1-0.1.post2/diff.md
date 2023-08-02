# Comparing `tmp/SliceCommander-0.1.tar.gz` & `tmp/SliceCommander-0.1.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SliceCommander-0.1.tar", last modified: Wed Aug  2 19:50:12 2023, max compression
+gzip compressed data, was "SliceCommander-0.1.post2.tar", last modified: Wed Aug  2 20:00:04 2023, max compression
```

## Comparing `SliceCommander-0.1.tar` & `SliceCommander-0.1.post2.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2023-08-02 19:50:12.718105 SliceCommander-0.1/
--rw-r--r--   0 ezra      (1000) ezra      (1000)      480 2023-08-02 19:50:12.718105 SliceCommander-0.1/PKG-INFO
--rw-r--r--   0 ezra      (1000) ezra      (1000)     1060 2022-12-20 19:23:00.000000 SliceCommander-0.1/README.md
-drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2023-08-02 19:50:12.718105 SliceCommander-0.1/SliceCommander.egg-info/
--rw-r--r--   0 ezra      (1000) ezra      (1000)      480 2023-08-02 19:50:12.000000 SliceCommander-0.1/SliceCommander.egg-info/PKG-INFO
--rw-r--r--   0 ezra      (1000) ezra      (1000)      343 2023-08-02 19:50:12.000000 SliceCommander-0.1/SliceCommander.egg-info/SOURCES.txt
--rw-r--r--   0 ezra      (1000) ezra      (1000)        1 2023-08-02 19:50:12.000000 SliceCommander-0.1/SliceCommander.egg-info/dependency_links.txt
--rw-r--r--   0 ezra      (1000) ezra      (1000)       55 2023-08-02 19:50:12.000000 SliceCommander-0.1/SliceCommander.egg-info/entry_points.txt
--rw-r--r--   0 ezra      (1000) ezra      (1000)       35 2023-08-02 19:50:12.000000 SliceCommander-0.1/SliceCommander.egg-info/requires.txt
--rw-r--r--   0 ezra      (1000) ezra      (1000)       10 2023-08-02 19:50:12.000000 SliceCommander-0.1/SliceCommander.egg-info/top_level.txt
-drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2023-08-02 19:50:12.718105 SliceCommander-0.1/commander/
--rw-r--r--   0 ezra      (1000) ezra      (1000)        0 2022-12-19 19:11:09.000000 SliceCommander-0.1/commander/__init__.py
--rwxr-xr-x   0 ezra      (1000) ezra      (1000)    15746 2023-08-02 19:42:52.000000 SliceCommander-0.1/commander/cli.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)      865 2022-12-19 19:11:09.000000 SliceCommander-0.1/commander/spinner.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)     2565 2023-08-02 17:06:40.000000 SliceCommander-0.1/commander/ssh.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)     2970 2022-12-19 19:11:09.000000 SliceCommander-0.1/commander/util.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)       38 2023-08-02 19:50:12.718105 SliceCommander-0.1/setup.cfg
--rw-r--r--   0 ezra      (1000) ezra      (1000)      789 2022-12-19 19:11:15.000000 SliceCommander-0.1/setup.py
+drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2023-08-02 20:00:04.577834 SliceCommander-0.1.post2/
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     1513 2023-08-02 19:58:53.000000 SliceCommander-0.1.post2/LICENSE
+-rw-r--r--   0 ezra      (1000) ezra      (1000)       41 2023-08-02 19:58:57.000000 SliceCommander-0.1.post2/MANIFEST.in
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     1609 2023-08-02 20:00:04.577834 SliceCommander-0.1.post2/PKG-INFO
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     1060 2022-12-20 19:23:00.000000 SliceCommander-0.1.post2/README.md
+drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2023-08-02 20:00:04.577834 SliceCommander-0.1.post2/SliceCommander.egg-info/
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     1609 2023-08-02 20:00:04.000000 SliceCommander-0.1.post2/SliceCommander.egg-info/PKG-INFO
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      380 2023-08-02 20:00:04.000000 SliceCommander-0.1.post2/SliceCommander.egg-info/SOURCES.txt
+-rw-r--r--   0 ezra      (1000) ezra      (1000)        1 2023-08-02 20:00:04.000000 SliceCommander-0.1.post2/SliceCommander.egg-info/dependency_links.txt
+-rw-r--r--   0 ezra      (1000) ezra      (1000)       55 2023-08-02 20:00:04.000000 SliceCommander-0.1.post2/SliceCommander.egg-info/entry_points.txt
+-rw-r--r--   0 ezra      (1000) ezra      (1000)       67 2023-08-02 20:00:04.000000 SliceCommander-0.1.post2/SliceCommander.egg-info/requires.txt
+-rw-r--r--   0 ezra      (1000) ezra      (1000)       10 2023-08-02 20:00:04.000000 SliceCommander-0.1.post2/SliceCommander.egg-info/top_level.txt
+drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2023-08-02 20:00:04.577834 SliceCommander-0.1.post2/commander/
+-rw-r--r--   0 ezra      (1000) ezra      (1000)        0 2022-12-19 19:11:09.000000 SliceCommander-0.1.post2/commander/__init__.py
+-rwxr-xr-x   0 ezra      (1000) ezra      (1000)    15746 2023-08-02 19:42:52.000000 SliceCommander-0.1.post2/commander/cli.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      865 2022-12-19 19:11:09.000000 SliceCommander-0.1.post2/commander/spinner.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     2565 2023-08-02 17:06:40.000000 SliceCommander-0.1.post2/commander/ssh.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     2970 2022-12-19 19:11:09.000000 SliceCommander-0.1.post2/commander/util.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)       67 2023-08-02 19:54:26.000000 SliceCommander-0.1.post2/requirements.txt
+-rw-r--r--   0 ezra      (1000) ezra      (1000)       38 2023-08-02 20:00:04.577834 SliceCommander-0.1.post2/setup.cfg
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     2650 2023-08-02 19:56:14.000000 SliceCommander-0.1.post2/setup.py
```

### Comparing `SliceCommander-0.1/README.md` & `SliceCommander-0.1.post2/README.md`

 * *Files identical despite different names*

### Comparing `SliceCommander-0.1/commander/cli.py` & `SliceCommander-0.1.post2/commander/cli.py`

 * *Files identical despite different names*

### Comparing `SliceCommander-0.1/commander/spinner.py` & `SliceCommander-0.1.post2/commander/spinner.py`

 * *Files identical despite different names*

### Comparing `SliceCommander-0.1/commander/ssh.py` & `SliceCommander-0.1.post2/commander/ssh.py`

 * *Files identical despite different names*

### Comparing `SliceCommander-0.1/commander/util.py` & `SliceCommander-0.1.post2/commander/util.py`

 * *Files identical despite different names*


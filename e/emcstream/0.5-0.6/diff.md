# Comparing `tmp/emcstream-0.5.tar.gz` & `tmp/emcstream-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emcstream-0.5.tar", last modified: Wed Aug  2 20:37:39 2023, max compression
+gzip compressed data, was "emcstream-0.6.tar", last modified: Wed Aug  2 20:58:44 2023, max compression
```

## Comparing `emcstream-0.5.tar` & `emcstream-0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 leyla     (1000) leyla     (1000)        0 2023-08-02 20:37:39.264744 emcstream-0.5/
--rw-rw-r--   0 leyla     (1000) leyla     (1000)     1076 2023-07-30 11:31:21.000000 emcstream-0.5/LICENSE
--rw-rw-r--   0 leyla     (1000) leyla     (1000)       26 2023-07-30 11:26:24.000000 emcstream-0.5/MANIFEST.in
--rw-rw-r--   0 leyla     (1000) leyla     (1000)      340 2023-08-02 20:37:39.264744 emcstream-0.5/PKG-INFO
--rw-rw-r--   0 leyla     (1000) leyla     (1000)     8175 2023-07-30 11:37:20.000000 emcstream-0.5/README.md
-drwxrwxr-x   0 leyla     (1000) leyla     (1000)        0 2023-08-02 20:37:39.264744 emcstream-0.5/emcstream/
--rw-rw-r--   0 leyla     (1000) leyla     (1000)     1947 2023-01-21 22:29:14.000000 emcstream-0.5/emcstream/DataManager.py
--rw-rw-r--   0 leyla     (1000) leyla     (1000)        0 2023-08-02 20:24:04.000000 emcstream-0.5/emcstream/__init__.py
--rw-rw-r--   0 leyla     (1000) leyla     (1000)    14092 2023-08-02 20:36:15.000000 emcstream-0.5/emcstream/emcstream.py
-drwxrwxr-x   0 leyla     (1000) leyla     (1000)        0 2023-08-02 20:37:39.264744 emcstream-0.5/emcstream.egg-info/
--rw-rw-r--   0 leyla     (1000) leyla     (1000)      340 2023-08-02 20:37:39.000000 emcstream-0.5/emcstream.egg-info/PKG-INFO
--rw-rw-r--   0 leyla     (1000) leyla     (1000)      289 2023-08-02 20:37:39.000000 emcstream-0.5/emcstream.egg-info/SOURCES.txt
--rw-rw-r--   0 leyla     (1000) leyla     (1000)        1 2023-08-02 20:37:39.000000 emcstream-0.5/emcstream.egg-info/dependency_links.txt
--rw-rw-r--   0 leyla     (1000) leyla     (1000)       48 2023-08-02 20:37:39.000000 emcstream-0.5/emcstream.egg-info/requires.txt
--rw-rw-r--   0 leyla     (1000) leyla     (1000)       10 2023-08-02 20:37:39.000000 emcstream-0.5/emcstream.egg-info/top_level.txt
--rw-rw-r--   0 leyla     (1000) leyla     (1000)       58 2023-07-30 11:29:22.000000 emcstream-0.5/requirements.txt
--rw-rw-r--   0 leyla     (1000) leyla     (1000)       38 2023-08-02 20:37:39.264744 emcstream-0.5/setup.cfg
--rw-rw-r--   0 leyla     (1000) leyla     (1000)      501 2023-08-02 20:37:33.000000 emcstream-0.5/setup.py
+drwxrwxr-x   0 leyla     (1000) leyla     (1000)        0 2023-08-02 20:58:44.465969 emcstream-0.6/
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)     1076 2023-07-30 11:31:21.000000 emcstream-0.6/LICENSE
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)       26 2023-07-30 11:26:24.000000 emcstream-0.6/MANIFEST.in
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)     8548 2023-08-02 20:58:44.465969 emcstream-0.6/PKG-INFO
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)     8175 2023-07-30 11:37:20.000000 emcstream-0.6/README.md
+drwxrwxr-x   0 leyla     (1000) leyla     (1000)        0 2023-08-02 20:58:44.465969 emcstream-0.6/emcstream/
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)     1947 2023-01-21 22:29:14.000000 emcstream-0.6/emcstream/DataManager.py
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)        0 2023-08-02 20:24:04.000000 emcstream-0.6/emcstream/__init__.py
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)    14092 2023-08-02 20:36:15.000000 emcstream-0.6/emcstream/emcstream.py
+drwxrwxr-x   0 leyla     (1000) leyla     (1000)        0 2023-08-02 20:58:44.465969 emcstream-0.6/emcstream.egg-info/
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)     8548 2023-08-02 20:58:44.000000 emcstream-0.6/emcstream.egg-info/PKG-INFO
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)      289 2023-08-02 20:58:44.000000 emcstream-0.6/emcstream.egg-info/SOURCES.txt
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)        1 2023-08-02 20:58:44.000000 emcstream-0.6/emcstream.egg-info/dependency_links.txt
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)       48 2023-08-02 20:58:44.000000 emcstream-0.6/emcstream.egg-info/requires.txt
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)       10 2023-08-02 20:58:44.000000 emcstream-0.6/emcstream.egg-info/top_level.txt
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)       58 2023-07-30 11:29:22.000000 emcstream-0.6/requirements.txt
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)       38 2023-08-02 20:58:44.465969 emcstream-0.6/setup.cfg
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)      717 2023-08-02 20:58:41.000000 emcstream-0.6/setup.py
```

### Comparing `emcstream-0.5/LICENSE` & `emcstream-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `emcstream-0.5/README.md` & `emcstream-0.6/README.md`

 * *Files identical despite different names*

### Comparing `emcstream-0.5/emcstream/DataManager.py` & `emcstream-0.6/emcstream/DataManager.py`

 * *Files identical despite different names*

### Comparing `emcstream-0.5/emcstream/emcstream.py` & `emcstream-0.6/emcstream/emcstream.py`

 * *Files identical despite different names*


# Comparing `tmp/emcstream-0.2.tar.gz` & `tmp/emcstream-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emcstream-0.2.tar", last modified: Wed Aug  2 19:08:57 2023, max compression
+gzip compressed data, was "emcstream-0.3.tar", last modified: Wed Aug  2 19:59:03 2023, max compression
```

## Comparing `emcstream-0.2.tar` & `emcstream-0.3.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxrwxr-x   0 leyla     (1000) leyla     (1000)        0 2023-08-02 19:08:57.573519 emcstream-0.2/
--rw-rw-r--   0 leyla     (1000) leyla     (1000)     1076 2023-07-30 11:31:21.000000 emcstream-0.2/LICENSE
--rw-rw-r--   0 leyla     (1000) leyla     (1000)       26 2023-07-30 11:26:24.000000 emcstream-0.2/MANIFEST.in
--rw-rw-r--   0 leyla     (1000) leyla     (1000)      340 2023-08-02 19:08:57.573519 emcstream-0.2/PKG-INFO
--rw-rw-r--   0 leyla     (1000) leyla     (1000)     8175 2023-07-30 11:37:20.000000 emcstream-0.2/README.md
-drwxrwxr-x   0 leyla     (1000) leyla     (1000)        0 2023-08-02 19:08:57.573519 emcstream-0.2/emcstream.egg-info/
--rw-rw-r--   0 leyla     (1000) leyla     (1000)      340 2023-08-02 19:08:57.000000 emcstream-0.2/emcstream.egg-info/PKG-INFO
--rw-rw-r--   0 leyla     (1000) leyla     (1000)      219 2023-08-02 19:08:57.000000 emcstream-0.2/emcstream.egg-info/SOURCES.txt
--rw-rw-r--   0 leyla     (1000) leyla     (1000)        1 2023-08-02 19:08:57.000000 emcstream-0.2/emcstream.egg-info/dependency_links.txt
--rw-rw-r--   0 leyla     (1000) leyla     (1000)       61 2023-08-02 19:08:57.000000 emcstream-0.2/emcstream.egg-info/requires.txt
--rw-rw-r--   0 leyla     (1000) leyla     (1000)        1 2023-08-02 19:08:57.000000 emcstream-0.2/emcstream.egg-info/top_level.txt
--rw-rw-r--   0 leyla     (1000) leyla     (1000)       58 2023-07-30 11:29:22.000000 emcstream-0.2/requirements.txt
--rw-rw-r--   0 leyla     (1000) leyla     (1000)       38 2023-08-02 19:08:57.573519 emcstream-0.2/setup.cfg
--rw-rw-r--   0 leyla     (1000) leyla     (1000)      525 2023-08-02 19:08:40.000000 emcstream-0.2/setup.py
+drwxrwxr-x   0 leyla     (1000) leyla     (1000)        0 2023-08-02 19:59:03.679550 emcstream-0.3/
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)     1076 2023-07-30 11:31:21.000000 emcstream-0.3/LICENSE
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)       26 2023-07-30 11:26:24.000000 emcstream-0.3/MANIFEST.in
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)      340 2023-08-02 19:59:03.679550 emcstream-0.3/PKG-INFO
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)     8175 2023-07-30 11:37:20.000000 emcstream-0.3/README.md
+drwxrwxr-x   0 leyla     (1000) leyla     (1000)        0 2023-08-02 19:59:03.679550 emcstream-0.3/emcstream/
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)     1947 2023-01-21 22:29:14.000000 emcstream-0.3/emcstream/DataManager.py
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)      528 2023-07-30 11:27:51.000000 emcstream-0.3/emcstream/__init__.py
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)    13680 2023-08-02 19:58:26.000000 emcstream-0.3/emcstream/emcstream.py
+drwxrwxr-x   0 leyla     (1000) leyla     (1000)        0 2023-08-02 19:59:03.679550 emcstream-0.3/emcstream.egg-info/
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)      340 2023-08-02 19:59:03.000000 emcstream-0.3/emcstream.egg-info/PKG-INFO
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)      289 2023-08-02 19:59:03.000000 emcstream-0.3/emcstream.egg-info/SOURCES.txt
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)        1 2023-08-02 19:59:03.000000 emcstream-0.3/emcstream.egg-info/dependency_links.txt
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)       48 2023-08-02 19:59:03.000000 emcstream-0.3/emcstream.egg-info/requires.txt
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)       10 2023-08-02 19:59:03.000000 emcstream-0.3/emcstream.egg-info/top_level.txt
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)       58 2023-07-30 11:29:22.000000 emcstream-0.3/requirements.txt
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)       38 2023-08-02 19:59:03.679550 emcstream-0.3/setup.cfg
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)      501 2023-08-02 19:58:47.000000 emcstream-0.3/setup.py
```

### Comparing `emcstream-0.2/LICENSE` & `emcstream-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `emcstream-0.2/README.md` & `emcstream-0.3/README.md`

 * *Files identical despite different names*


# Comparing `tmp/pc_mouseparty-0.0.0.tar.gz` & `tmp/pc_mouseparty-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pc_mouseparty-0.0.0.tar", last modified: Wed Aug  2 02:36:49 2023, max compression
+gzip compressed data, was "pc_mouseparty-0.1.1.tar", last modified: Tue Jul 25 19:59:21 2023, max compression
```

## Comparing `pc_mouseparty-0.0.0.tar` & `pc_mouseparty-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:36:49.806304 pc_mouseparty-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-02 02:36:37.000000 pc_mouseparty-0.0.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-02 02:36:37.000000 pc_mouseparty-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-02 02:36:37.000000 pc_mouseparty-0.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-08-02 02:36:49.806304 pc_mouseparty-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-08-02 02:36:37.000000 pc_mouseparty-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:36:49.806304 pc_mouseparty-0.0.0/pc_mouseparty/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-02 02:36:37.000000 pc_mouseparty-0.0.0/pc_mouseparty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-02 02:36:37.000000 pc_mouseparty-0.0.0/pc_mouseparty/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-02 02:36:37.000000 pc_mouseparty-0.0.0/pc_mouseparty/common.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 02:36:37.000000 pc_mouseparty-0.0.0/pc_mouseparty/pc_mouseparty.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:36:49.806304 pc_mouseparty-0.0.0/pc_mouseparty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-08-02 02:36:49.000000 pc_mouseparty-0.0.0/pc_mouseparty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-08-02 02:36:49.000000 pc_mouseparty-0.0.0/pc_mouseparty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 02:36:49.000000 pc_mouseparty-0.0.0/pc_mouseparty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-02 02:36:49.000000 pc_mouseparty-0.0.0/pc_mouseparty.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 02:36:49.000000 pc_mouseparty-0.0.0/pc_mouseparty.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-02 02:36:49.000000 pc_mouseparty-0.0.0/pc_mouseparty.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 02:36:37.000000 pc_mouseparty-0.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-08-02 02:36:49.806304 pc_mouseparty-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-08-02 02:36:37.000000 pc_mouseparty-0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:59:21.896717 pc_mouseparty-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-25 19:59:03.000000 pc_mouseparty-0.1.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-25 19:59:03.000000 pc_mouseparty-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-25 19:59:03.000000 pc_mouseparty-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-25 19:59:21.896717 pc_mouseparty-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-25 19:59:03.000000 pc_mouseparty-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:59:21.896717 pc_mouseparty-0.1.1/pc_mouseparty/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-25 19:59:03.000000 pc_mouseparty-0.1.1/pc_mouseparty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-25 19:59:03.000000 pc_mouseparty-0.1.1/pc_mouseparty/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-25 19:59:03.000000 pc_mouseparty-0.1.1/pc_mouseparty/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-25 19:59:03.000000 pc_mouseparty-0.1.1/pc_mouseparty/pc_mouseparty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:59:21.896717 pc_mouseparty-0.1.1/pc_mouseparty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-25 19:59:21.000000 pc_mouseparty-0.1.1/pc_mouseparty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-25 19:59:21.000000 pc_mouseparty-0.1.1/pc_mouseparty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:59:21.000000 pc_mouseparty-0.1.1/pc_mouseparty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-25 19:59:21.000000 pc_mouseparty-0.1.1/pc_mouseparty.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:59:21.000000 pc_mouseparty-0.1.1/pc_mouseparty.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 19:59:21.000000 pc_mouseparty-0.1.1/pc_mouseparty.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:59:03.000000 pc_mouseparty-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-25 19:59:21.896717 pc_mouseparty-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-25 19:59:03.000000 pc_mouseparty-0.1.1/setup.py
```

### Comparing `pc_mouseparty-0.0.0/LICENSE` & `pc_mouseparty-0.1.1/LICENSE`

 * *Files identical despite different names*


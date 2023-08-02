# Comparing `tmp/hecdbetz-1.0.tar.gz` & `tmp/hecdbetz-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hecdbetz-1.0.tar", last modified: Wed Aug  2 07:25:55 2023, max compression
+gzip compressed data, was "dist/hecdbetz-2.0.tar", last modified: Wed Aug  2 07:39:59 2023, max compression
```

## Comparing `hecdbetz-1.0.tar` & `hecdbetz-2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 zhangmingwei  (1000) zhangmingwei  (1000)        0 2023-08-02 07:25:54.999105 hecdbetz-1.0/
--rwxrw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)      582 2023-08-02 07:23:55.000000 hecdbetz-1.0/LICENSE
--rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)       84 2023-08-02 07:25:54.999105 hecdbetz-1.0/PKG-INFO
--rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)       21 2023-08-02 06:06:04.000000 hecdbetz-1.0/README.md
-drwxrwxr-x   0 zhangmingwei  (1000) zhangmingwei  (1000)        0 2023-08-02 07:25:54.999105 hecdbetz-1.0/hecdbetz/
--rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)       21 2023-08-02 06:45:08.000000 hecdbetz-1.0/hecdbetz/__init__.py
--rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)       33 2023-08-02 06:44:58.000000 hecdbetz-1.0/hecdbetz/add_num.py
--rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)      683 2023-08-02 06:13:22.000000 hecdbetz-1.0/hecdbetz/calculate.py
-drwxrwxr-x   0 zhangmingwei  (1000) zhangmingwei  (1000)        0 2023-08-02 07:25:54.999105 hecdbetz-1.0/hecdbetz.egg-info/
--rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)       84 2023-08-02 07:25:54.000000 hecdbetz-1.0/hecdbetz.egg-info/PKG-INFO
--rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)      217 2023-08-02 07:25:54.000000 hecdbetz-1.0/hecdbetz.egg-info/SOURCES.txt
--rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)        1 2023-08-02 07:25:54.000000 hecdbetz-1.0/hecdbetz.egg-info/dependency_links.txt
--rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)        9 2023-08-02 07:25:54.000000 hecdbetz-1.0/hecdbetz.egg-info/top_level.txt
--rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)       38 2023-08-02 07:25:54.999105 hecdbetz-1.0/setup.cfg
--rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)      229 2023-08-02 07:23:40.000000 hecdbetz-1.0/setup.py
+drwxrwxr-x   0 zhangmingwei  (1000) zhangmingwei  (1000)        0 2023-08-02 07:39:59.000000 hecdbetz-2.0/
+-rwxrw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)      582 2023-08-02 07:23:55.000000 hecdbetz-2.0/LICENSE
+-rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)       84 2023-08-02 07:39:59.000000 hecdbetz-2.0/PKG-INFO
+-rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)       21 2023-08-02 06:06:04.000000 hecdbetz-2.0/README.md
+drwxrwxr-x   0 zhangmingwei  (1000) zhangmingwei  (1000)        0 2023-08-02 07:39:59.000000 hecdbetz-2.0/hecdbetz/
+-rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)       21 2023-08-02 06:45:08.000000 hecdbetz-2.0/hecdbetz/__init__.py
+-rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)       33 2023-08-02 06:44:58.000000 hecdbetz-2.0/hecdbetz/add_num.py
+-rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)      683 2023-08-02 06:13:22.000000 hecdbetz-2.0/hecdbetz/calculate.py
+drwxrwxr-x   0 zhangmingwei  (1000) zhangmingwei  (1000)        0 2023-08-02 07:39:59.000000 hecdbetz-2.0/hecdbetz.egg-info/
+-rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)       84 2023-08-02 07:39:59.000000 hecdbetz-2.0/hecdbetz.egg-info/PKG-INFO
+-rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)      217 2023-08-02 07:39:59.000000 hecdbetz-2.0/hecdbetz.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)        1 2023-08-02 07:39:59.000000 hecdbetz-2.0/hecdbetz.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)        9 2023-08-02 07:39:59.000000 hecdbetz-2.0/hecdbetz.egg-info/top_level.txt
+-rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)       38 2023-08-02 07:39:59.000000 hecdbetz-2.0/setup.cfg
+-rwxrw-rw-   0 zhangmingwei  (1000) zhangmingwei  (1000)      229 2023-08-02 07:39:39.000000 hecdbetz-2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `hecdbetz-1.0/LICENSE` & `hecdbetz-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hecdbetz-1.0/hecdbetz/calculate.py` & `hecdbetz-2.0/hecdbetz/calculate.py`

 * *Files identical despite different names*


# Comparing `tmp/litellm-0.1.210.tar.gz` & `tmp/litellm-0.1.211.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.210.tar", last modified: Tue Aug  1 23:27:06 2023, max compression
+gzip compressed data, was "litellm-0.1.211.tar", last modified: Tue Aug  1 23:31:24 2023, max compression
```

## Comparing `litellm-0.1.210.tar` & `litellm-0.1.211.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 23:27:06.092991 litellm-0.1.210/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1065 2023-08-01 23:26:54.000000 litellm-0.1.210/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-08-01 23:27:06.092991 litellm-0.1.210/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2474 2023-08-01 23:26:54.000000 litellm-0.1.210/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 23:27:06.088991 litellm-0.1.210/litellm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2023-08-01 23:26:54.000000 litellm-0.1.210/litellm/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10735 2023-08-01 23:26:54.000000 litellm-0.1.210/litellm/main.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2546 2023-08-01 23:26:54.000000 litellm-0.1.210/litellm/timeout.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12522 2023-08-01 23:26:54.000000 litellm-0.1.210/litellm/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 23:27:06.092991 litellm-0.1.210/litellm.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-08-01 23:27:06.000000 litellm-0.1.210/litellm.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      252 2023-08-01 23:27:06.000000 litellm-0.1.210/litellm.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-01 23:27:06.000000 litellm-0.1.210/litellm.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       71 2023-08-01 23:27:06.000000 litellm-0.1.210/litellm.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        8 2023-08-01 23:27:06.000000 litellm-0.1.210/litellm.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-01 23:27:06.092991 litellm-0.1.210/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      407 2023-08-01 23:26:54.000000 litellm-0.1.210/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 23:31:24.207503 litellm-0.1.211/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1065 2023-08-01 23:31:12.000000 litellm-0.1.211/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-08-01 23:31:24.203503 litellm-0.1.211/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2474 2023-08-01 23:31:12.000000 litellm-0.1.211/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 23:31:24.203503 litellm-0.1.211/litellm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2023-08-01 23:31:12.000000 litellm-0.1.211/litellm/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10735 2023-08-01 23:31:12.000000 litellm-0.1.211/litellm/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2546 2023-08-01 23:31:12.000000 litellm-0.1.211/litellm/timeout.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12522 2023-08-01 23:31:12.000000 litellm-0.1.211/litellm/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 23:31:24.203503 litellm-0.1.211/litellm.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-08-01 23:31:24.000000 litellm-0.1.211/litellm.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      252 2023-08-01 23:31:24.000000 litellm-0.1.211/litellm.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-01 23:31:24.000000 litellm-0.1.211/litellm.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       71 2023-08-01 23:31:24.000000 litellm-0.1.211/litellm.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        8 2023-08-01 23:31:24.000000 litellm-0.1.211/litellm.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-01 23:31:24.207503 litellm-0.1.211/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      407 2023-08-01 23:31:12.000000 litellm-0.1.211/setup.py
```

### Comparing `litellm-0.1.210/LICENSE` & `litellm-0.1.211/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.210/README.md` & `litellm-0.1.211/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.210/litellm/__init__.py` & `litellm-0.1.211/litellm/__init__.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.210/litellm/main.py` & `litellm-0.1.211/litellm/main.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.210/litellm/timeout.py` & `litellm-0.1.211/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.210/litellm/utils.py` & `litellm-0.1.211/litellm/utils.py`

 * *Files identical despite different names*


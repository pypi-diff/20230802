# Comparing `tmp/litellm-0.1.207.tar.gz` & `tmp/litellm-0.1.208.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.207.tar", last modified: Tue Aug  1 21:45:31 2023, max compression
+gzip compressed data, was "litellm-0.1.208.tar", last modified: Tue Aug  1 22:58:41 2023, max compression
```

## Comparing `litellm-0.1.207.tar` & `litellm-0.1.208.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:45:31.413084 litellm-0.1.207/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-01 21:45:15.000000 litellm-0.1.207/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-01 21:45:31.413084 litellm-0.1.207/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-08-01 21:45:15.000000 litellm-0.1.207/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:45:31.409083 litellm-0.1.207/litellm/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-01 21:45:15.000000 litellm-0.1.207/litellm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-08-01 21:45:15.000000 litellm-0.1.207/litellm/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-08-01 21:45:15.000000 litellm-0.1.207/litellm/timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)    12522 2023-08-01 21:45:15.000000 litellm-0.1.207/litellm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:45:31.413084 litellm-0.1.207/litellm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-01 21:45:31.000000 litellm-0.1.207/litellm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-01 21:45:31.000000 litellm-0.1.207/litellm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 21:45:31.000000 litellm-0.1.207/litellm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-01 21:45:31.000000 litellm-0.1.207/litellm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 21:45:31.000000 litellm-0.1.207/litellm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 21:45:31.413084 litellm-0.1.207/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-01 21:45:15.000000 litellm-0.1.207/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:58:41.421200 litellm-0.1.208/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-01 22:58:28.000000 litellm-0.1.208/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-01 22:58:41.421200 litellm-0.1.208/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-08-01 22:58:28.000000 litellm-0.1.208/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:58:41.421200 litellm-0.1.208/litellm/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-01 22:58:28.000000 litellm-0.1.208/litellm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-08-01 22:58:28.000000 litellm-0.1.208/litellm/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-08-01 22:58:28.000000 litellm-0.1.208/litellm/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12522 2023-08-01 22:58:28.000000 litellm-0.1.208/litellm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:58:41.421200 litellm-0.1.208/litellm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-01 22:58:41.000000 litellm-0.1.208/litellm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-01 22:58:41.000000 litellm-0.1.208/litellm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 22:58:41.000000 litellm-0.1.208/litellm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-01 22:58:41.000000 litellm-0.1.208/litellm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 22:58:41.000000 litellm-0.1.208/litellm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 22:58:41.421200 litellm-0.1.208/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-01 22:58:28.000000 litellm-0.1.208/setup.py
```

### Comparing `litellm-0.1.207/LICENSE` & `litellm-0.1.208/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.207/README.md` & `litellm-0.1.208/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.207/litellm/__init__.py` & `litellm-0.1.208/litellm/__init__.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.207/litellm/main.py` & `litellm-0.1.208/litellm/main.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.207/litellm/timeout.py` & `litellm-0.1.208/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.207/litellm/utils.py` & `litellm-0.1.208/litellm/utils.py`

 * *Files identical despite different names*


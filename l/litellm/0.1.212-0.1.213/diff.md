# Comparing `tmp/litellm-0.1.212.tar.gz` & `tmp/litellm-0.1.213.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.212.tar", last modified: Wed Aug  2 03:14:27 2023, max compression
+gzip compressed data, was "litellm-0.1.213.tar", last modified: Wed Aug  2 03:14:59 2023, max compression
```

## Comparing `litellm-0.1.212.tar` & `litellm-0.1.213.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 03:14:27.358550 litellm-0.1.212/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1065 2023-08-02 03:14:14.000000 litellm-0.1.212/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-08-02 03:14:27.358550 litellm-0.1.212/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2129 2023-08-02 03:14:14.000000 litellm-0.1.212/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 03:14:27.354550 litellm-0.1.212/litellm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2023-08-02 03:14:14.000000 litellm-0.1.212/litellm/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10735 2023-08-02 03:14:14.000000 litellm-0.1.212/litellm/main.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2546 2023-08-02 03:14:14.000000 litellm-0.1.212/litellm/timeout.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12522 2023-08-02 03:14:14.000000 litellm-0.1.212/litellm/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 03:14:27.358550 litellm-0.1.212/litellm.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-08-02 03:14:27.000000 litellm-0.1.212/litellm.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      252 2023-08-02 03:14:27.000000 litellm-0.1.212/litellm.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-02 03:14:27.000000 litellm-0.1.212/litellm.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       71 2023-08-02 03:14:27.000000 litellm-0.1.212/litellm.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        8 2023-08-02 03:14:27.000000 litellm-0.1.212/litellm.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-02 03:14:27.358550 litellm-0.1.212/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      407 2023-08-02 03:14:14.000000 litellm-0.1.212/setup.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-08-02 03:14:59.260458 litellm-0.1.213/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-07-27 00:10:35.000000 litellm-0.1.213/LICENSE
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      215 2023-08-02 03:14:59.260364 litellm-0.1.213/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     2129 2023-08-02 03:09:05.000000 litellm-0.1.213/README.md
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-08-02 03:14:59.259564 litellm-0.1.213/litellm/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      626 2023-08-01 22:01:24.000000 litellm-0.1.213/litellm/__init__.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)    10735 2023-08-02 00:06:25.000000 litellm-0.1.213/litellm/main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     2546 2023-08-01 22:01:24.000000 litellm-0.1.213/litellm/timeout.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)    12522 2023-08-01 22:01:24.000000 litellm-0.1.213/litellm/utils.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-08-02 03:14:59.260197 litellm-0.1.213/litellm.egg-info/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      215 2023-08-02 03:14:59.000000 litellm-0.1.213/litellm.egg-info/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      252 2023-08-02 03:14:59.000000 litellm-0.1.213/litellm.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-08-02 03:14:59.000000 litellm-0.1.213/litellm.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       71 2023-08-02 03:14:59.000000 litellm-0.1.213/litellm.egg-info/requires.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        8 2023-08-02 03:14:59.000000 litellm-0.1.213/litellm.egg-info/top_level.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-08-02 03:14:59.260492 litellm-0.1.213/setup.cfg
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      407 2023-08-02 03:14:16.000000 litellm-0.1.213/setup.py
```

### Comparing `litellm-0.1.212/LICENSE` & `litellm-0.1.213/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.212/README.md` & `litellm-0.1.213/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.212/litellm/__init__.py` & `litellm-0.1.213/litellm/__init__.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.212/litellm/main.py` & `litellm-0.1.213/litellm/main.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.212/litellm/timeout.py` & `litellm-0.1.213/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.212/litellm/utils.py` & `litellm-0.1.213/litellm/utils.py`

 * *Files identical despite different names*


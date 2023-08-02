# Comparing `tmp/regex_toolkit-0.0.3.tar.gz` & `tmp/regex_toolkit-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regex_toolkit-0.0.3.tar", last modified: Sun Jan 15 18:06:27 2023, max compression
+gzip compressed data, was "regex_toolkit-0.0.4.tar", last modified: Wed Aug  2 03:22:32 2023, max compression
```

## Comparing `regex_toolkit-0.0.3.tar` & `regex_toolkit-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,24 @@
-drwxrwxr-x   0 yaphott   (1000) yaphott   (1000)        0 2023-01-15 18:06:27.654442 regex_toolkit-0.0.3/
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    35149 2023-01-15 17:24:23.000000 regex_toolkit-0.0.3/LICENSE
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    12269 2023-01-15 18:06:27.654442 regex_toolkit-0.0.3/PKG-INFO
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    10770 2023-01-15 17:09:04.000000 regex_toolkit-0.0.3/README.md
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     1726 2023-01-15 17:53:20.000000 regex_toolkit-0.0.3/pyproject.toml
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)       38 2023-01-15 18:06:27.654442 regex_toolkit-0.0.3/setup.cfg
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     1516 2023-01-15 18:04:54.000000 regex_toolkit-0.0.3/setup.py
-drwxrwxr-x   0 yaphott   (1000) yaphott   (1000)        0 2023-01-15 18:06:27.654442 regex_toolkit-0.0.3/src/
-drwxrwxr-x   0 yaphott   (1000) yaphott   (1000)        0 2023-01-15 18:06:27.654442 regex_toolkit-0.0.3/src/regex_toolkit/
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)       43 2023-01-15 18:06:15.000000 regex_toolkit-0.0.3/src/regex_toolkit/__init__.py
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     7450 2023-01-15 12:06:24.000000 regex_toolkit-0.0.3/src/regex_toolkit/base.py
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    10103 2022-11-18 18:38:58.000000 regex_toolkit-0.0.3/src/regex_toolkit/base_BAK_2022-11-18.py
-drwxrwxr-x   0 yaphott   (1000) yaphott   (1000)        0 2023-01-15 18:06:27.654442 regex_toolkit-0.0.3/src/regex_toolkit.egg-info/
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    12269 2023-01-15 18:06:27.000000 regex_toolkit-0.0.3/src/regex_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)      302 2023-01-15 18:06:27.000000 regex_toolkit-0.0.3/src/regex_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)        1 2023-01-15 18:06:27.000000 regex_toolkit-0.0.3/src/regex_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 yaphott   (1000) yaphott   (1000)       14 2023-01-15 18:06:27.000000 regex_toolkit-0.0.3/src/regex_toolkit.egg-info/top_level.txt
+drwxrwxr-x   0 yaphott   (1000) yaphott   (1000)        0 2023-08-02 03:22:32.709417 regex_toolkit-0.0.4/
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    35149 2023-02-23 04:14:09.000000 regex_toolkit-0.0.4/LICENSE
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    50313 2023-08-02 03:22:32.709417 regex_toolkit-0.0.4/PKG-INFO
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     8538 2023-08-02 03:14:19.000000 regex_toolkit-0.0.4/README.md
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     3947 2023-08-02 03:14:19.000000 regex_toolkit-0.0.4/pyproject.toml
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)       38 2023-08-02 03:22:32.709417 regex_toolkit-0.0.4/setup.cfg
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)      573 2023-08-02 03:14:19.000000 regex_toolkit-0.0.4/setup.py
+drwxrwxr-x   0 yaphott   (1000) yaphott   (1000)        0 2023-08-02 03:22:32.705417 regex_toolkit-0.0.4/src/
+drwxrwxr-x   0 yaphott   (1000) yaphott   (1000)        0 2023-08-02 03:22:32.709417 regex_toolkit-0.0.4/src/regex_toolkit/
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)      593 2023-08-02 03:14:19.000000 regex_toolkit-0.0.4/src/regex_toolkit/__init__.py
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     3268 2023-08-02 03:14:19.000000 regex_toolkit-0.0.4/src/regex_toolkit/base.py
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)      698 2023-08-02 03:14:19.000000 regex_toolkit-0.0.4/src/regex_toolkit/constants.py
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)      231 2023-08-02 03:14:19.000000 regex_toolkit-0.0.4/src/regex_toolkit/enums.py
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     4813 2023-08-02 03:14:19.000000 regex_toolkit-0.0.4/src/regex_toolkit/utils.py
+drwxrwxr-x   0 yaphott   (1000) yaphott   (1000)        0 2023-08-02 03:22:32.709417 regex_toolkit-0.0.4/src/regex_toolkit.egg-info/
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    50313 2023-08-02 03:22:32.000000 regex_toolkit-0.0.4/src/regex_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)      445 2023-08-02 03:22:32.000000 regex_toolkit-0.0.4/src/regex_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)        1 2023-08-02 03:22:32.000000 regex_toolkit-0.0.4/src/regex_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)       16 2023-08-02 03:22:32.000000 regex_toolkit-0.0.4/src/regex_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)       14 2023-08-02 03:22:32.000000 regex_toolkit-0.0.4/src/regex_toolkit.egg-info/top_level.txt
+drwxrwxr-x   0 yaphott   (1000) yaphott   (1000)        0 2023-08-02 03:22:32.709417 regex_toolkit-0.0.4/tests/
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)    25488 2023-08-02 03:14:19.000000 regex_toolkit-0.0.4/tests/test_base.py
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)      510 2023-08-02 03:14:19.000000 regex_toolkit-0.0.4/tests/test_enums.py
+-rw-rw-r--   0 yaphott   (1000) yaphott   (1000)     4022 2023-08-02 03:14:19.000000 regex_toolkit-0.0.4/tests/test_utils.py
```

### Comparing `regex_toolkit-0.0.3/LICENSE` & `regex_toolkit-0.0.4/LICENSE`

 * *Files identical despite different names*


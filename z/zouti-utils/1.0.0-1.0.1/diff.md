# Comparing `tmp/zouti-utils-1.0.0.tar.gz` & `tmp/zouti-utils-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zouti-utils-1.0.0.tar", last modified: Tue Aug  1 22:42:32 2023, max compression
+gzip compressed data, was "zouti-utils-1.0.1.tar", last modified: Tue Aug  1 22:47:09 2023, max compression
```

## Comparing `zouti-utils-1.0.0.tar` & `zouti-utils-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:42:32.786304 zouti-utils-1.0.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1069 2023-08-01 22:42:23.000000 zouti-utils-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-01 22:42:32.786304 zouti-utils-1.0.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)       34 2023-08-01 22:42:23.000000 zouti-utils-1.0.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      489 2023-08-01 22:42:23.000000 zouti-utils-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 22:42:32.786304 zouti-utils-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:42:32.786304 zouti-utils-1.0.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:42:23.000000 zouti-utils-1.0.0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-01 22:42:23.000000 zouti-utils-1.0.0/src/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-08-01 22:42:23.000000 zouti-utils-1.0.0/src/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:42:32.786304 zouti-utils-1.0.0/src/zouti_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-01 22:42:32.000000 zouti-utils-1.0.0/src/zouti_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-08-01 22:42:32.000000 zouti-utils-1.0.0/src/zouti_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 22:42:32.000000 zouti-utils-1.0.0/src/zouti_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 22:42:32.000000 zouti-utils-1.0.0/src/zouti_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 22:42:32.000000 zouti-utils-1.0.0/src/zouti_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:47:09.104815 zouti-utils-1.0.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1069 2023-08-01 22:46:59.000000 zouti-utils-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-01 22:47:09.104815 zouti-utils-1.0.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)       34 2023-08-01 22:46:59.000000 zouti-utils-1.0.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      489 2023-08-01 22:46:59.000000 zouti-utils-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 22:47:09.104815 zouti-utils-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:47:09.104815 zouti-utils-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:47:09.104815 zouti-utils-1.0.1/src/zouti_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:46:59.000000 zouti-utils-1.0.1/src/zouti_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-01 22:46:59.000000 zouti-utils-1.0.1/src/zouti_utils/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-08-01 22:46:59.000000 zouti-utils-1.0.1/src/zouti_utils/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:47:09.104815 zouti-utils-1.0.1/src/zouti_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-01 22:47:09.000000 zouti-utils-1.0.1/src/zouti_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-08-01 22:47:09.000000 zouti-utils-1.0.1/src/zouti_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 22:47:09.000000 zouti-utils-1.0.1/src/zouti_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 22:47:09.000000 zouti-utils-1.0.1/src/zouti_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 22:47:09.000000 zouti-utils-1.0.1/src/zouti_utils.egg-info/top_level.txt
```

### Comparing `zouti-utils-1.0.0/LICENSE` & `zouti-utils-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zouti-utils-1.0.0/src/database.py` & `zouti-utils-1.0.1/src/zouti_utils/database.py`

 * *Files identical despite different names*

### Comparing `zouti-utils-1.0.0/src/model.py` & `zouti-utils-1.0.1/src/zouti_utils/model.py`

 * *Files identical despite different names*


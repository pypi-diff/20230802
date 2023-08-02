# Comparing `tmp/chained-recurrence-0.0.8.tar.gz` & `tmp/chained-recurrence-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chained-recurrence-0.0.8.tar", last modified: Wed Jan  4 19:33:45 2023, max compression
+gzip compressed data, was "chained-recurrence-0.0.9.tar", last modified: Thu Jan  5 06:26:53 2023, max compression
```

## Comparing `chained-recurrence-0.0.8.tar` & `chained-recurrence-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 matt      (1000) users      (985)        0 2023-01-04 19:33:45.845072 chained-recurrence-0.0.8/
--rw-r--r--   0 matt      (1000) users      (985)      745 2022-12-20 06:47:59.000000 chained-recurrence-0.0.8/LICENCE
--rw-r--r--   0 matt      (1000) users      (985)     4321 2023-01-04 19:33:45.845072 chained-recurrence-0.0.8/PKG-INFO
--rw-r--r--   0 matt      (1000) users      (985)     2072 2022-12-30 19:45:43.000000 chained-recurrence-0.0.8/README.md
--rw-r--r--   0 matt      (1000) users      (985)     1849 2023-01-04 19:32:17.000000 chained-recurrence-0.0.8/pyproject.toml
--rw-r--r--   0 matt      (1000) users      (985)       38 2023-01-04 19:33:45.845072 chained-recurrence-0.0.8/setup.cfg
-drwxr-xr-x   0 matt      (1000) users      (985)        0 2023-01-04 19:33:45.845072 chained-recurrence-0.0.8/src/
-drwxr-xr-x   0 matt      (1000) users      (985)        0 2023-01-04 19:33:45.845072 chained-recurrence-0.0.8/src/chained_recurrence/
--rw-r--r--   0 matt      (1000) users      (985)       22 2023-01-04 19:32:34.000000 chained-recurrence-0.0.8/src/chained_recurrence/__init__.py
--rwxr-xr-x   0 matt      (1000) users      (985)     3125 2023-01-04 19:27:01.000000 chained-recurrence-0.0.8/src/chained_recurrence/__main__.py
--rwxr--r--   0 matt      (1000) users      (985)     2788 2023-01-04 12:35:30.000000 chained-recurrence-0.0.8/src/chained_recurrence/on-modify-chained.py
-drwxr-xr-x   0 matt      (1000) users      (985)        0 2023-01-04 19:33:45.845072 chained-recurrence-0.0.8/src/chained_recurrence.egg-info/
--rw-r--r--   0 matt      (1000) users      (985)     4321 2023-01-04 19:33:45.000000 chained-recurrence-0.0.8/src/chained_recurrence.egg-info/PKG-INFO
--rw-r--r--   0 matt      (1000) users      (985)      424 2023-01-04 19:33:45.000000 chained-recurrence-0.0.8/src/chained_recurrence.egg-info/SOURCES.txt
--rw-r--r--   0 matt      (1000) users      (985)        1 2023-01-04 19:33:45.000000 chained-recurrence-0.0.8/src/chained_recurrence.egg-info/dependency_links.txt
--rw-r--r--   0 matt      (1000) users      (985)       72 2023-01-04 19:33:45.000000 chained-recurrence-0.0.8/src/chained_recurrence.egg-info/entry_points.txt
--rw-r--r--   0 matt      (1000) users      (985)       47 2023-01-04 19:33:45.000000 chained-recurrence-0.0.8/src/chained_recurrence.egg-info/requires.txt
--rw-r--r--   0 matt      (1000) users      (985)       19 2023-01-04 19:33:45.000000 chained-recurrence-0.0.8/src/chained_recurrence.egg-info/top_level.txt
+drwxr-xr-x   0 matt      (1000) users      (985)        0 2023-01-05 06:26:53.857818 chained-recurrence-0.0.9/
+-rw-r--r--   0 matt      (1000) users      (985)      745 2022-12-20 06:47:59.000000 chained-recurrence-0.0.9/LICENCE
+-rw-r--r--   0 matt      (1000) users      (985)     4099 2023-01-05 06:26:53.857818 chained-recurrence-0.0.9/PKG-INFO
+-rw-r--r--   0 matt      (1000) users      (985)     1850 2023-01-04 19:47:03.000000 chained-recurrence-0.0.9/README.md
+-rw-r--r--   0 matt      (1000) users      (985)     1849 2023-01-04 19:32:17.000000 chained-recurrence-0.0.9/pyproject.toml
+-rw-r--r--   0 matt      (1000) users      (985)       38 2023-01-05 06:26:53.857818 chained-recurrence-0.0.9/setup.cfg
+drwxr-xr-x   0 matt      (1000) users      (985)        0 2023-01-05 06:26:53.854485 chained-recurrence-0.0.9/src/
+drwxr-xr-x   0 matt      (1000) users      (985)        0 2023-01-05 06:26:53.854485 chained-recurrence-0.0.9/src/chained_recurrence/
+-rw-r--r--   0 matt      (1000) users      (985)       22 2023-01-05 06:26:19.000000 chained-recurrence-0.0.9/src/chained_recurrence/__init__.py
+-rwxr-xr-x   0 matt      (1000) users      (985)     3125 2023-01-04 19:27:01.000000 chained-recurrence-0.0.9/src/chained_recurrence/__main__.py
+-rwxr--r--   0 matt      (1000) users      (985)     2788 2023-01-04 12:35:30.000000 chained-recurrence-0.0.9/src/chained_recurrence/on-modify-chained.py
+drwxr-xr-x   0 matt      (1000) users      (985)        0 2023-01-05 06:26:53.854485 chained-recurrence-0.0.9/src/chained_recurrence.egg-info/
+-rw-r--r--   0 matt      (1000) users      (985)     4099 2023-01-05 06:26:53.000000 chained-recurrence-0.0.9/src/chained_recurrence.egg-info/PKG-INFO
+-rw-r--r--   0 matt      (1000) users      (985)      424 2023-01-05 06:26:53.000000 chained-recurrence-0.0.9/src/chained_recurrence.egg-info/SOURCES.txt
+-rw-r--r--   0 matt      (1000) users      (985)        1 2023-01-05 06:26:53.000000 chained-recurrence-0.0.9/src/chained_recurrence.egg-info/dependency_links.txt
+-rw-r--r--   0 matt      (1000) users      (985)       72 2023-01-05 06:26:53.000000 chained-recurrence-0.0.9/src/chained_recurrence.egg-info/entry_points.txt
+-rw-r--r--   0 matt      (1000) users      (985)       47 2023-01-05 06:26:53.000000 chained-recurrence-0.0.9/src/chained_recurrence.egg-info/requires.txt
+-rw-r--r--   0 matt      (1000) users      (985)       19 2023-01-05 06:26:53.000000 chained-recurrence-0.0.9/src/chained_recurrence.egg-info/top_level.txt
```

### Comparing `chained-recurrence-0.0.8/LICENCE` & `chained-recurrence-0.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `chained-recurrence-0.0.8/PKG-INFO` & `chained-recurrence-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chained-recurrence
-Version: 0.0.8
+Version: 0.0.9
 Summary: Painless chained recurrence for Taskwarrior.
 Author-email: Matt Deacalion Stevens <matt@dirtymonkey.co.uk>
 License: ISC License
         
         Copyright © 2023 Matthew Stevens
         
         Permission to use, copy, modify, and/or distribute this software for any
@@ -106,15 +106,7 @@
 
 ## Uninstall
 
 ```bash
 $ chained-recurrence uninstall
 $ pip uninstall chained-recurrence
 ```
-
-
-## TODO
-
-- the `entry` field is used calculate `due` and `wait`, this makes the time you
-  enter data crucial. what way could we make this configurable?
-
-  `$ t add chained:on entry:sod-3d wait:entry+2d due:wait+1d xxx`
```

### Comparing `chained-recurrence-0.0.8/README.md` & `chained-recurrence-0.0.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -59,15 +59,7 @@
 
 ## Uninstall
 
 ```bash
 $ chained-recurrence uninstall
 $ pip uninstall chained-recurrence
 ```
-
-
-## TODO
-
-- the `entry` field is used calculate `due` and `wait`, this makes the time you
-  enter data crucial. what way could we make this configurable?
-
-  `$ t add chained:on entry:sod-3d wait:entry+2d due:wait+1d xxx`
```

### Comparing `chained-recurrence-0.0.8/pyproject.toml` & `chained-recurrence-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chained-recurrence-0.0.8/src/chained_recurrence/__main__.py` & `chained-recurrence-0.0.9/src/chained_recurrence/__main__.py`

 * *Files identical despite different names*

### Comparing `chained-recurrence-0.0.8/src/chained_recurrence/on-modify-chained.py` & `chained-recurrence-0.0.9/src/chained_recurrence/on-modify-chained.py`

 * *Files identical despite different names*

### Comparing `chained-recurrence-0.0.8/src/chained_recurrence.egg-info/PKG-INFO` & `chained-recurrence-0.0.9/src/chained_recurrence.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chained-recurrence
-Version: 0.0.8
+Version: 0.0.9
 Summary: Painless chained recurrence for Taskwarrior.
 Author-email: Matt Deacalion Stevens <matt@dirtymonkey.co.uk>
 License: ISC License
         
         Copyright © 2023 Matthew Stevens
         
         Permission to use, copy, modify, and/or distribute this software for any
@@ -106,15 +106,7 @@
 
 ## Uninstall
 
 ```bash
 $ chained-recurrence uninstall
 $ pip uninstall chained-recurrence
 ```
-
-
-## TODO
-
-- the `entry` field is used calculate `due` and `wait`, this makes the time you
-  enter data crucial. what way could we make this configurable?
-
-  `$ t add chained:on entry:sod-3d wait:entry+2d due:wait+1d xxx`
```


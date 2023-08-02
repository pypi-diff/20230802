# Comparing `tmp/pyscabbard-0.0.1.tar.gz` & `tmp/pyscabbard-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscabbard-0.0.1.tar", last modified: Mon Jul 31 09:58:50 2023, max compression
+gzip compressed data, was "pyscabbard-0.0.2.tar", last modified: Wed Aug  2 09:50:25 2023, max compression
```

## Comparing `pyscabbard-0.0.1.tar` & `pyscabbard-0.0.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-31 09:58:50.401345 pyscabbard-0.0.1/
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      172 2023-01-25 13:44:54.000000 pyscabbard-0.0.1/AUTHORS.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     3542 2023-01-25 13:44:54.000000 pyscabbard-0.0.1/CONTRIBUTING.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       89 2023-01-25 13:44:54.000000 pyscabbard-0.0.1/HISTORY.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1074 2023-01-25 13:44:54.000000 pyscabbard-0.0.1/LICENSE
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      262 2023-01-25 13:44:54.000000 pyscabbard-0.0.1/MANIFEST.in
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1692 2023-07-31 09:58:50.401345 pyscabbard-0.0.1/PKG-INFO
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      878 2023-01-25 13:44:54.000000 pyscabbard-0.0.1/README.rst
-drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-31 09:58:50.401345 pyscabbard-0.0.1/docs/
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      609 2023-01-25 13:44:54.000000 pyscabbard-0.0.1/docs/Makefile
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       28 2023-01-25 13:44:54.000000 pyscabbard-0.0.1/docs/authors.rst
--rwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)     4800 2023-01-25 13:44:54.000000 pyscabbard-0.0.1/docs/conf.py
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       33 2023-01-25 13:44:54.000000 pyscabbard-0.0.1/docs/contributing.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       28 2023-01-25 13:44:54.000000 pyscabbard-0.0.1/docs/history.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      305 2023-01-25 13:44:54.000000 pyscabbard-0.0.1/docs/index.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1130 2023-01-25 13:44:54.000000 pyscabbard-0.0.1/docs/installation.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      806 2023-01-25 13:44:54.000000 pyscabbard-0.0.1/docs/make.bat
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       27 2023-01-25 13:44:54.000000 pyscabbard-0.0.1/docs/readme.rst
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       71 2023-01-25 13:44:54.000000 pyscabbard-0.0.1/docs/usage.rst
-drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-31 09:58:50.401345 pyscabbard-0.0.1/pyscabbard.egg-info/
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1692 2023-07-31 09:58:50.000000 pyscabbard-0.0.1/pyscabbard.egg-info/PKG-INFO
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      853 2023-07-31 09:58:50.000000 pyscabbard-0.0.1/pyscabbard.egg-info/SOURCES.txt
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        1 2023-07-31 09:58:50.000000 pyscabbard-0.0.1/pyscabbard.egg-info/dependency_links.txt
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      158 2023-07-31 09:58:50.000000 pyscabbard-0.0.1/pyscabbard.egg-info/entry_points.txt
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        1 2023-07-31 09:58:50.000000 pyscabbard-0.0.1/pyscabbard.egg-info/not-zip-safe
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       11 2023-07-31 09:58:50.000000 pyscabbard-0.0.1/pyscabbard.egg-info/requires.txt
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        9 2023-07-31 09:58:50.000000 pyscabbard-0.0.1/pyscabbard.egg-info/top_level.txt
-drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-31 09:58:50.401345 pyscabbard-0.0.1/scabbard/
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     3309 2023-04-11 08:10:58.000000 pyscabbard-0.0.1/scabbard/Dax.py
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1323 2023-04-02 17:37:29.000000 pyscabbard-0.0.1/scabbard/Dfig.py
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      486 2023-03-03 15:35:42.000000 pyscabbard-0.0.1/scabbard/Dplot.py
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      102 2023-03-01 12:51:53.000000 pyscabbard-0.0.1/scabbard/Dutils.py
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      399 2023-06-26 09:33:06.000000 pyscabbard-0.0.1/scabbard/__init__.py
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      402 2023-01-25 13:44:54.000000 pyscabbard-0.0.1/scabbard/cli.py
--rw-r--r--   0 bgailleton  (1000) bgailleton  (1000)      197 2022-09-20 12:25:47.000000 pyscabbard-0.0.1/scabbard/enumeration.py
--rw-r--r--   0 bgailleton  (1000) bgailleton  (1000)     6384 2023-02-06 18:16:04.000000 pyscabbard-0.0.1/scabbard/fastflood.py
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-27 14:40:17.000000 pyscabbard-0.0.1/scabbard/flow.py
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      401 2023-07-31 09:32:29.000000 pyscabbard-0.0.1/scabbard/geography.py
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    14221 2023-04-19 12:53:42.000000 pyscabbard-0.0.1/scabbard/graphflood.py
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     6372 2023-07-28 16:40:11.000000 pyscabbard-0.0.1/scabbard/graphflood_helper.py
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     7065 2023-07-31 09:32:52.000000 pyscabbard-0.0.1/scabbard/grid.py
--rw-r--r--   0 bgailleton  (1000) bgailleton  (1000)     3358 2023-06-07 08:27:19.000000 pyscabbard-0.0.1/scabbard/io.py
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2676 2023-07-25 12:52:22.000000 pyscabbard-0.0.1/scabbard/phineas.py
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       19 2023-01-25 13:44:54.000000 pyscabbard-0.0.1/scabbard/scabbard.py
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      380 2023-07-31 09:58:50.401345 pyscabbard-0.0.1/setup.cfg
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1398 2023-07-31 09:57:59.000000 pyscabbard-0.0.1/setup.py
-drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-31 09:58:50.401345 pyscabbard-0.0.1/tests/
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       38 2023-01-25 13:44:54.000000 pyscabbard-0.0.1/tests/__init__.py
--rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      859 2023-01-25 13:44:54.000000 pyscabbard-0.0.1/tests/test_scabbard.py
+drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-08-02 09:50:25.717770 pyscabbard-0.0.2/
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      172 2023-01-25 13:44:54.000000 pyscabbard-0.0.2/AUTHORS.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     3542 2023-01-25 13:44:54.000000 pyscabbard-0.0.2/CONTRIBUTING.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      365 2023-08-02 09:49:32.000000 pyscabbard-0.0.2/HISTORY.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1074 2023-01-25 13:44:54.000000 pyscabbard-0.0.2/LICENSE
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      262 2023-01-25 13:44:54.000000 pyscabbard-0.0.2/MANIFEST.in
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1969 2023-08-02 09:50:25.717770 pyscabbard-0.0.2/PKG-INFO
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      878 2023-01-25 13:44:54.000000 pyscabbard-0.0.2/README.rst
+drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-08-02 09:50:25.713770 pyscabbard-0.0.2/docs/
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      609 2023-01-25 13:44:54.000000 pyscabbard-0.0.2/docs/Makefile
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       28 2023-01-25 13:44:54.000000 pyscabbard-0.0.2/docs/authors.rst
+-rwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)     4800 2023-01-25 13:44:54.000000 pyscabbard-0.0.2/docs/conf.py
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       33 2023-01-25 13:44:54.000000 pyscabbard-0.0.2/docs/contributing.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       28 2023-01-25 13:44:54.000000 pyscabbard-0.0.2/docs/history.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      305 2023-01-25 13:44:54.000000 pyscabbard-0.0.2/docs/index.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1130 2023-01-25 13:44:54.000000 pyscabbard-0.0.2/docs/installation.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      806 2023-01-25 13:44:54.000000 pyscabbard-0.0.2/docs/make.bat
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       27 2023-01-25 13:44:54.000000 pyscabbard-0.0.2/docs/readme.rst
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       71 2023-01-25 13:44:54.000000 pyscabbard-0.0.2/docs/usage.rst
+drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-08-02 09:50:25.713770 pyscabbard-0.0.2/pyscabbard.egg-info/
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1969 2023-08-02 09:50:25.000000 pyscabbard-0.0.2/pyscabbard.egg-info/PKG-INFO
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      853 2023-08-02 09:50:25.000000 pyscabbard-0.0.2/pyscabbard.egg-info/SOURCES.txt
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        1 2023-08-02 09:50:25.000000 pyscabbard-0.0.2/pyscabbard.egg-info/dependency_links.txt
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      158 2023-08-02 09:50:25.000000 pyscabbard-0.0.2/pyscabbard.egg-info/entry_points.txt
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        1 2023-07-31 09:58:50.000000 pyscabbard-0.0.2/pyscabbard.egg-info/not-zip-safe
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       11 2023-08-02 09:50:25.000000 pyscabbard-0.0.2/pyscabbard.egg-info/requires.txt
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        9 2023-08-02 09:50:25.000000 pyscabbard-0.0.2/pyscabbard.egg-info/top_level.txt
+drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-08-02 09:50:25.713770 pyscabbard-0.0.2/scabbard/
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     3309 2023-04-11 08:10:58.000000 pyscabbard-0.0.2/scabbard/Dax.py
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1323 2023-04-02 17:37:29.000000 pyscabbard-0.0.2/scabbard/Dfig.py
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      486 2023-03-03 15:35:42.000000 pyscabbard-0.0.2/scabbard/Dplot.py
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      102 2023-03-01 12:51:53.000000 pyscabbard-0.0.2/scabbard/Dutils.py
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      399 2023-06-26 09:33:06.000000 pyscabbard-0.0.2/scabbard/__init__.py
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      402 2023-01-25 13:44:54.000000 pyscabbard-0.0.2/scabbard/cli.py
+-rw-r--r--   0 bgailleton  (1000) bgailleton  (1000)      197 2022-09-20 12:25:47.000000 pyscabbard-0.0.2/scabbard/enumeration.py
+-rw-r--r--   0 bgailleton  (1000) bgailleton  (1000)     6384 2023-02-06 18:16:04.000000 pyscabbard-0.0.2/scabbard/fastflood.py
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)        0 2023-07-27 14:40:17.000000 pyscabbard-0.0.2/scabbard/flow.py
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      401 2023-07-31 09:32:29.000000 pyscabbard-0.0.2/scabbard/geography.py
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)    14221 2023-04-19 12:53:42.000000 pyscabbard-0.0.2/scabbard/graphflood.py
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     6372 2023-07-28 16:40:11.000000 pyscabbard-0.0.2/scabbard/graphflood_helper.py
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     8883 2023-08-02 09:28:04.000000 pyscabbard-0.0.2/scabbard/grid.py
+-rw-r--r--   0 bgailleton  (1000) bgailleton  (1000)     3358 2023-06-07 08:27:19.000000 pyscabbard-0.0.2/scabbard/io.py
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     2676 2023-07-25 12:52:22.000000 pyscabbard-0.0.2/scabbard/phineas.py
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       19 2023-01-25 13:44:54.000000 pyscabbard-0.0.2/scabbard/scabbard.py
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      380 2023-08-02 09:50:25.717770 pyscabbard-0.0.2/setup.cfg
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)     1398 2023-08-02 09:48:05.000000 pyscabbard-0.0.2/setup.py
+drwxrwxr-x   0 bgailleton  (1000) bgailleton  (1000)        0 2023-08-02 09:50:25.717770 pyscabbard-0.0.2/tests/
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)       38 2023-01-25 13:44:54.000000 pyscabbard-0.0.2/tests/__init__.py
+-rw-rw-r--   0 bgailleton  (1000) bgailleton  (1000)      859 2023-01-25 13:44:54.000000 pyscabbard-0.0.2/tests/test_scabbard.py
```

### Comparing `pyscabbard-0.0.1/CONTRIBUTING.rst` & `pyscabbard-0.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyscabbard-0.0.1/LICENSE` & `pyscabbard-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscabbard-0.0.1/PKG-INFO` & `pyscabbard-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscabbard
-Version: 0.0.1
+Version: 0.0.2
 Summary: high-level python package for the DAGGER suite
 Home-page: https://github.com/bgailleton/scabbard
 Author: Boris Gailleton
 Author-email: boris.gailleton@univ-rennes1.fr
 License: MIT license
 Keywords: scabbard
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -58,11 +58,20 @@
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
-0.0.1 (2023-01-25)
+0.0.2 (2023-07-31)
+------------------
+
+* Adding drainage divide quick extraction tools
+* Fixing sea_level/Z0 stuff 
+
+0.0.1 (2023-07-25)
 ------------------
 
 * First release on PyPI.
+* Adding tools for quick river extraction
+* Started a big behind-the-scene refactoring and standardisation (invisible at top level)
+* Maintenance and bug fixes
```

### Comparing `pyscabbard-0.0.1/README.rst` & `pyscabbard-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `pyscabbard-0.0.1/docs/Makefile` & `pyscabbard-0.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyscabbard-0.0.1/docs/conf.py` & `pyscabbard-0.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyscabbard-0.0.1/docs/installation.rst` & `pyscabbard-0.0.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pyscabbard-0.0.1/docs/make.bat` & `pyscabbard-0.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyscabbard-0.0.1/pyscabbard.egg-info/PKG-INFO` & `pyscabbard-0.0.2/pyscabbard.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscabbard
-Version: 0.0.1
+Version: 0.0.2
 Summary: high-level python package for the DAGGER suite
 Home-page: https://github.com/bgailleton/scabbard
 Author: Boris Gailleton
 Author-email: boris.gailleton@univ-rennes1.fr
 License: MIT license
 Keywords: scabbard
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -58,11 +58,20 @@
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
-0.0.1 (2023-01-25)
+0.0.2 (2023-07-31)
+------------------
+
+* Adding drainage divide quick extraction tools
+* Fixing sea_level/Z0 stuff 
+
+0.0.1 (2023-07-25)
 ------------------
 
 * First release on PyPI.
+* Adding tools for quick river extraction
+* Started a big behind-the-scene refactoring and standardisation (invisible at top level)
+* Maintenance and bug fixes
```

### Comparing `pyscabbard-0.0.1/pyscabbard.egg-info/SOURCES.txt` & `pyscabbard-0.0.2/pyscabbard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyscabbard-0.0.1/scabbard/Dax.py` & `pyscabbard-0.0.2/scabbard/Dax.py`

 * *Files identical despite different names*

### Comparing `pyscabbard-0.0.1/scabbard/Dfig.py` & `pyscabbard-0.0.2/scabbard/Dfig.py`

 * *Files identical despite different names*

### Comparing `pyscabbard-0.0.1/scabbard/fastflood.py` & `pyscabbard-0.0.2/scabbard/fastflood.py`

 * *Files identical despite different names*

### Comparing `pyscabbard-0.0.1/scabbard/graphflood.py` & `pyscabbard-0.0.2/scabbard/graphflood.py`

 * *Files identical despite different names*

### Comparing `pyscabbard-0.0.1/scabbard/graphflood_helper.py` & `pyscabbard-0.0.2/scabbard/graphflood_helper.py`

 * *Files identical despite different names*

### Comparing `pyscabbard-0.0.1/scabbard/grid.py` & `pyscabbard-0.0.2/scabbard/grid.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,30 @@
 	"""
 	Manages a regular grid with helper functions
 	"""
 	
 
 	def __init__(self, nx, ny, dx, dy, Z, geography = None):
 
+		'''
+		Contruct a grid from base char:
+		- nx = number of cols
+		- ny = number of rows
+		- dx = spacing in the X direction
+		- dy = spacing in the Y direction
+		- Z = a numpy array of ny * nx coordinates containing elevation data
+
+		And optional specs:
+		- geography: custom geogrphic info
+
+		It is recommended to use premade automatic functions (bellow) as much as you can: they would create grid from loading a DEM or with random noise or slope surface for example
+
+		'''
+
+		# Ignore
 		super(RGrid, self).__init__()
 		
 		# Number of col
 		self.nx = nx
 		# Number of rows
 		self.ny = ny
 		#nnodes
@@ -40,53 +56,80 @@
 		self.rshp = (ny,nx)
 
 		if(geography is None):
 			self.geography = geo.geog(xmin = 0., ymin = 0., xmax = self.lx, ymax = self.ly)
 		else:
 			self.geography = geography
 
+		# Elevation flat array 
 		self._Z = Z.ravel()
 
+		# Placeholders for connector and graph objects
 		self.con = None
 		self.graph = None
 
 		
 
 	def extent(self, y_min_top = True):
+		'''
+		Bounding box for the dem: [xmin,xmax, ymin, ymax].
+		Can be directly used in matplotlib's imshow function
+		'''
 		return [self.geography.xmin, self.geography.xmax, self.geography.ymin if y_min_top else self.geography.ymax, self.geography.ymax if y_min_top else self.geography.ymin ]
 
 
 	@property
 	def X(self):
+		'''
+		1D array [nx] of flat X coordinates
+		'''
 		return np.linspace(self.geography.xmin + self.dx/2, self.geography.xmax - self.dx/2, self.nx)
 
 	@property
 	def Y(self):
+		'''
+		1D array [ny] of flat Y coordinates
+		'''
 		return np.linspace(self.geography.ymin + self.dy/2, self.geography.ymax - self.dy/2, self.ny)
 
 	@property
 	def XY(self):
+		'''
+		2D array of XY coordinates for each node -  as a  meshgrid.
+		'''
 		xx,yy = np.meshgrid(self.X, self.Y)
 		return xx, yy[::-1]
 
 	@property
 	def Z(self):
+		'''
+		Accessing the 1D flat elevation array [nx * ny]
+		'''
 		return self._Z
 
 	@property
 	def Z2D(self):
+		'''
+		Accessing the 2D elevation array [ny,nx]
+		'''
 		return self._Z.reshape(self.ny,self.nx)
 
 	@property
 	def XYZ(self):
+		'''
+		meshgrid of XYZ coordinates
+		'''
 		xx,yy = np.meshgrid(self.X, self.Y)
 		return xx, yy, self.Z2D
 
 	@property
 	def hillshade(self):
+		'''
+		2D array of hillshaded relief (values between 0 and 1)
+		'''
 		if(self.con is None):
 			con = dag.D8N(self.nx, self.ny, self.dx, self.dy, self.geography.xmin, self.geography.ymin)
 		else:
 			con = self.con
 		return dag.hillshade(con, self._Z).reshape(self.rshp)
 
 	
@@ -100,19 +143,22 @@
 		
 		con = dag.D8N(self.nx, self.ny, self.dx, self.dy, self.geography.xmin, self.geography.ymin)
 		graph = dag.graph(con)
 		if(process):
 			graph.compute_graph(self._Z, True, False)
 		return graph, con
 
-	def compute_graphcon(self, SFD = False, BCs = None, LM = dag.LMR.none, preprocess_topo = False ):
+	def compute_graphcon(self, SFD = False, BCs = None, LM = dag.LMR.none, preprocess_topo = False, Z0 = None ):
 		self.con = dag.D8N(self.nx, self.ny, self.dx, self.dy, self.geography.xmin, self.geography.ymin)
 		
 		if(BCs is not None):
 			self.con.set_custom_boundaries(BCs.ravel())
+
+		if(Z0 is not None):
+			dag.set_BC_to_remove_seas(self.con, self._Z, Z0) 
 		
 		self.graph = dag.graph(self.con)
 		self.graph.set_LMR_method(LM)
 		if(preprocess_topo):
 			self._Z = self.graph.compute_graph(self._Z, SFD, False)
 		else:
 			self.graph.compute_graph(self._Z, SFD, False)
@@ -139,14 +185,33 @@
 		rivdict["rows"] = rivdict["nodes"] // self.nx
 		rivdict["cols"] = rivdict["nodes"] % self.nx
 		rivdict["X"] = self.XY[0].ravel()[rivdict["nodes"]]
 		rivdict["Y"] = self.XY[1].ravel()[rivdict["nodes"]]
 
 		return rivdict
 
+	def quick_basin_extraction(self, basinID = None, return_basinID = False):
+		if(self.graph is None):
+			self.compute_graphcon(SFD = True, BCs = None, LM = dag.LMR.cordonnier_carve, preprocess_topo = False)
+
+		if(basinID is None):
+			basinID = self.graph.get_SFD_basin_labels()
+
+		DDdict = dag.DrainageDivides(self.con, self.graph, self._Z, basinID.ravel())
+		DDdict["rows"] = DDdict["nodes"] // self.nx
+		DDdict["cols"] = DDdict["nodes"] % self.nx
+		DDdict["X"] = self.XY[0].ravel()[DDdict["nodes"]]
+		DDdict["Y"] = self.XY[1].ravel()[DDdict["nodes"]]
+
+
+		if(return_basinID):
+			return DDdict, basinID.reshape(self.rshp)
+		else:
+			return DDdict
+
 	def baseplot(self, alpha_hs = 0.65, cmap = "gist_earth", clim = None, figsize = None, fig = None, ax = None, colorbar = True ):
 		need_return = False
 		if(fig is None):
 			fig,ax = plt.subplots(figsize = figsize)
 			need_return = True
 		cb = ax.imshow(self.Z2D, cmap = cmap, vmin = self._Z.min() if clim is None else clim[0], vmax = self._Z.max() if clim is None else clim[1], extent = self.extent())
```

### Comparing `pyscabbard-0.0.1/scabbard/io.py` & `pyscabbard-0.0.2/scabbard/io.py`

 * *Files identical despite different names*

### Comparing `pyscabbard-0.0.1/scabbard/phineas.py` & `pyscabbard-0.0.2/scabbard/phineas.py`

 * *Files identical despite different names*

### Comparing `pyscabbard-0.0.1/setup.py` & `pyscabbard-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,10 +42,10 @@
 	include_package_data=True,
 	keywords='scabbard',
 	name='pyscabbard',
 	packages=find_packages(include=['scabbard', 'scabbard.*']),
 	test_suite='tests',
 	tests_require=test_requirements,
 	url='https://github.com/bgailleton/scabbard',
-	version='0.0.1',
+	version='0.0.2',
 	zip_safe=False,
 )
```

### Comparing `pyscabbard-0.0.1/tests/test_scabbard.py` & `pyscabbard-0.0.2/tests/test_scabbard.py`

 * *Files identical despite different names*


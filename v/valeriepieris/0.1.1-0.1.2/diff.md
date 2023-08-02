# Comparing `tmp/valeriepieris-0.1.1.tar.gz` & `tmp/valeriepieris-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valeriepieris-0.1.1.tar", last modified: Sun Jul 30 08:10:30 2023, max compression
+gzip compressed data, was "valeriepieris-0.1.2.tar", last modified: Wed Aug  2 06:34:41 2023, max compression
```

## Comparing `valeriepieris-0.1.1.tar` & `valeriepieris-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ra414     (1000) ra414     (1000)        0 2023-07-30 08:10:30.356798 valeriepieris-0.1.1/
--rw-rw-r--   0 ra414     (1000) ra414     (1000)    35149 2023-07-30 06:24:37.000000 valeriepieris-0.1.1/LICENSE.txt
--rw-rw-r--   0 ra414     (1000) ra414     (1000)       45 2023-07-30 07:20:50.000000 valeriepieris-0.1.1/MANIFEST.in
--rw-rw-r--   0 ra414     (1000) ra414     (1000)     2151 2023-07-30 08:10:30.356798 valeriepieris-0.1.1/PKG-INFO
--rw-rw-r--   0 ra414     (1000) ra414     (1000)      544 2023-07-30 08:08:11.000000 valeriepieris-0.1.1/README.md
--rw-rw-r--   0 ra414     (1000) ra414     (1000)      609 2023-07-30 08:09:20.000000 valeriepieris-0.1.1/pyproject.toml
--rw-rw-r--   0 ra414     (1000) ra414     (1000)       14 2023-07-30 07:20:20.000000 valeriepieris-0.1.1/requirements.txt
--rw-rw-r--   0 ra414     (1000) ra414     (1000)     1509 2023-07-30 08:10:30.356798 valeriepieris-0.1.1/setup.cfg
--rw-rw-r--   0 ra414     (1000) ra414     (1000)      414 2023-07-30 07:45:27.000000 valeriepieris-0.1.1/setup.py
-drwxrwxr-x   0 ra414     (1000) ra414     (1000)        0 2023-07-30 08:10:30.352798 valeriepieris-0.1.1/src/
--rw-rw-r--   0 ra414     (1000) ra414     (1000)  1696289 2023-07-30 07:45:29.000000 valeriepieris-0.1.1/src/valeriepieris.c
-drwxrwxr-x   0 ra414     (1000) ra414     (1000)        0 2023-07-30 08:10:30.356798 valeriepieris-0.1.1/src/valeriepieris.egg-info/
--rw-rw-r--   0 ra414     (1000) ra414     (1000)     2151 2023-07-30 08:10:30.000000 valeriepieris-0.1.1/src/valeriepieris.egg-info/PKG-INFO
--rw-rw-r--   0 ra414     (1000) ra414     (1000)      308 2023-07-30 08:10:30.000000 valeriepieris-0.1.1/src/valeriepieris.egg-info/SOURCES.txt
--rw-rw-r--   0 ra414     (1000) ra414     (1000)        1 2023-07-30 08:10:30.000000 valeriepieris-0.1.1/src/valeriepieris.egg-info/dependency_links.txt
--rw-rw-r--   0 ra414     (1000) ra414     (1000)        1 2023-07-30 07:45:30.000000 valeriepieris-0.1.1/src/valeriepieris.egg-info/not-zip-safe
--rw-rw-r--   0 ra414     (1000) ra414     (1000)       14 2023-07-30 08:10:30.000000 valeriepieris-0.1.1/src/valeriepieris.egg-info/top_level.txt
+drwxrwxr-x   0 ra414     (1000) ra414     (1000)        0 2023-08-02 06:34:41.758360 valeriepieris-0.1.2/
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)    35149 2023-07-30 06:24:37.000000 valeriepieris-0.1.2/LICENSE.txt
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)       45 2023-07-30 07:20:50.000000 valeriepieris-0.1.2/MANIFEST.in
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)     5223 2023-08-02 06:34:41.758360 valeriepieris-0.1.2/PKG-INFO
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)     3184 2023-08-02 06:33:23.000000 valeriepieris-0.1.2/README.md
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)      609 2023-08-02 06:34:08.000000 valeriepieris-0.1.2/pyproject.toml
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)       14 2023-07-30 07:20:20.000000 valeriepieris-0.1.2/requirements.txt
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)     1509 2023-08-02 06:34:41.758360 valeriepieris-0.1.2/setup.cfg
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)      414 2023-07-30 07:45:27.000000 valeriepieris-0.1.2/setup.py
+drwxrwxr-x   0 ra414     (1000) ra414     (1000)        0 2023-08-02 06:34:41.758360 valeriepieris-0.1.2/src/
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)  1696289 2023-07-30 07:45:29.000000 valeriepieris-0.1.2/src/valeriepieris.c
+drwxrwxr-x   0 ra414     (1000) ra414     (1000)        0 2023-08-02 06:34:41.758360 valeriepieris-0.1.2/src/valeriepieris.egg-info/
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)     5223 2023-08-02 06:34:41.000000 valeriepieris-0.1.2/src/valeriepieris.egg-info/PKG-INFO
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)      308 2023-08-02 06:34:41.000000 valeriepieris-0.1.2/src/valeriepieris.egg-info/SOURCES.txt
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)        1 2023-08-02 06:34:41.000000 valeriepieris-0.1.2/src/valeriepieris.egg-info/dependency_links.txt
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)        1 2023-07-30 07:45:30.000000 valeriepieris-0.1.2/src/valeriepieris.egg-info/not-zip-safe
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)       14 2023-08-02 06:34:41.000000 valeriepieris-0.1.2/src/valeriepieris.egg-info/top_level.txt
```

### Comparing `valeriepieris-0.1.1/LICENSE.txt` & `valeriepieris-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `valeriepieris-0.1.1/pyproject.toml` & `valeriepieris-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "valeriepieris"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Rudy Arthur", email="rudy.d.arthur@gmail.com" },
 ]
 description = "calculate valeriepieris circles"
 readme = "README.md"
 requires-python = ">=3.8"
 requires = ["setuptools", "wheel", "numpy >= 1.24", "Cython>=0.29.33"]
```

### Comparing `valeriepieris-0.1.1/setup.cfg` & `valeriepieris-0.1.2/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = valeriepieris
-version = 0.1.1
+version = 0.1.2
 description = Finding valeriepieris circles
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = GNU GENERAL PUBLIC LICENSE Version 3
 author = Rudy Arthur
 author_email = rudy.d.arthur@gmail.com
 url = https://github.com/rudyarthur/valeriepieris
```

### Comparing `valeriepieris-0.1.1/src/valeriepieris.c` & `valeriepieris-0.1.2/src/valeriepieris.c`

 * *Files identical despite different names*


# Comparing `tmp/apify_shared-1.0.2.tar.gz` & `tmp/apify_shared-1.0.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apify_shared-1.0.2.tar", last modified: Wed Aug  2 06:52:10 2023, max compression
+gzip compressed data, was "apify_shared-1.0.2b1.tar", last modified: Tue Aug  1 21:55:24 2023, max compression
```

## Comparing `apify_shared-1.0.2.tar` & `apify_shared-1.0.2b1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:52:10.653856 apify_shared-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-08-02 06:51:36.000000 apify_shared-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-08-02 06:52:10.653856 apify_shared-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-02 06:51:36.000000 apify_shared-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-08-02 06:51:36.000000 apify_shared-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 06:52:10.653856 apify_shared-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:52:10.653856 apify_shared-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:52:10.653856 apify_shared-1.0.2/src/apify_shared/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 06:51:36.000000 apify_shared-1.0.2/src/apify_shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-08-02 06:51:36.000000 apify_shared-1.0.2/src/apify_shared/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-08-02 06:51:36.000000 apify_shared-1.0.2/src/apify_shared/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 06:51:36.000000 apify_shared-1.0.2/src/apify_shared/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-02 06:51:36.000000 apify_shared-1.0.2/src/apify_shared/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-08-02 06:51:36.000000 apify_shared-1.0.2/src/apify_shared/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:52:10.653856 apify_shared-1.0.2/src/apify_shared.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-08-02 06:52:10.000000 apify_shared-1.0.2/src/apify_shared.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-02 06:52:10.000000 apify_shared-1.0.2/src/apify_shared.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 06:52:10.000000 apify_shared-1.0.2/src/apify_shared.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-02 06:52:10.000000 apify_shared-1.0.2/src/apify_shared.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-02 06:52:10.000000 apify_shared-1.0.2/src/apify_shared.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:55:24.263535 apify_shared-1.0.2b1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-08-01 21:54:52.000000 apify_shared-1.0.2b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-08-01 21:55:24.263535 apify_shared-1.0.2b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-01 21:54:52.000000 apify_shared-1.0.2b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-08-01 21:55:19.000000 apify_shared-1.0.2b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 21:55:24.263535 apify_shared-1.0.2b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:55:24.259535 apify_shared-1.0.2b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:55:24.259535 apify_shared-1.0.2b1/src/apify_shared/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-01 21:54:52.000000 apify_shared-1.0.2b1/src/apify_shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-08-01 21:54:52.000000 apify_shared-1.0.2b1/src/apify_shared/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-08-01 21:54:52.000000 apify_shared-1.0.2b1/src/apify_shared/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 21:54:52.000000 apify_shared-1.0.2b1/src/apify_shared/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-01 21:54:52.000000 apify_shared-1.0.2b1/src/apify_shared/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-08-01 21:54:52.000000 apify_shared-1.0.2b1/src/apify_shared/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:55:24.263535 apify_shared-1.0.2b1/src/apify_shared.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-08-01 21:55:24.000000 apify_shared-1.0.2b1/src/apify_shared.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-01 21:55:24.000000 apify_shared-1.0.2b1/src/apify_shared.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 21:55:24.000000 apify_shared-1.0.2b1/src/apify_shared.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-01 21:55:24.000000 apify_shared-1.0.2b1/src/apify_shared.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 21:55:24.000000 apify_shared-1.0.2b1/src/apify_shared.egg-info/top_level.txt
```

### Comparing `apify_shared-1.0.2/LICENSE` & `apify_shared-1.0.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `apify_shared-1.0.2/PKG-INFO` & `apify_shared-1.0.2b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify_shared
-Version: 1.0.2
+Version: 1.0.2b1
 Summary: Tools and constants shared across Apify projects.
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Apify Homepage, https://apify.com
 Project-URL: Changelog, https://github.com/apify/apify-shared-python/blob/master/CHANGELOG.md
 Project-URL: Issue tracker, https://github.com/apify/apify-shared-python/issues
 Project-URL: Source, https://github.com/apify/apify-shared-python
```

### Comparing `apify_shared-1.0.2/README.md` & `apify_shared-1.0.2b1/README.md`

 * *Files identical despite different names*

### Comparing `apify_shared-1.0.2/pyproject.toml` & `apify_shared-1.0.2b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 dependencies = []
 description = "Tools and constants shared across Apify projects."
 keywords = ["apify", "api", "shared", "scraping", "automation"]
 license = {text = "Apache Software License"}
 name = "apify_shared"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "1.0.2"
+version = "1.0.2b1"
 
 [project.optional-dependencies]
 dev = [
   "autopep8 ~= 2.0.2",
   "build ~= 0.10.0",
   "flake8 ~= 6.0.0",
   "flake8-bugbear ~= 23.5.9",
```

### Comparing `apify_shared-1.0.2/src/apify_shared/consts.py` & `apify_shared-1.0.2b1/src/apify_shared/consts.py`

 * *Files identical despite different names*

### Comparing `apify_shared-1.0.2/src/apify_shared/models.py` & `apify_shared-1.0.2b1/src/apify_shared/models.py`

 * *Files identical despite different names*

### Comparing `apify_shared-1.0.2/src/apify_shared/utils.py` & `apify_shared-1.0.2b1/src/apify_shared/utils.py`

 * *Files identical despite different names*

### Comparing `apify_shared-1.0.2/src/apify_shared.egg-info/PKG-INFO` & `apify_shared-1.0.2b1/src/apify_shared.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify-shared
-Version: 1.0.2
+Version: 1.0.2b1
 Summary: Tools and constants shared across Apify projects.
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Apify Homepage, https://apify.com
 Project-URL: Changelog, https://github.com/apify/apify-shared-python/blob/master/CHANGELOG.md
 Project-URL: Issue tracker, https://github.com/apify/apify-shared-python/issues
 Project-URL: Source, https://github.com/apify/apify-shared-python
```

### Comparing `apify_shared-1.0.2/src/apify_shared.egg-info/requires.txt` & `apify_shared-1.0.2b1/src/apify_shared.egg-info/requires.txt`

 * *Files identical despite different names*


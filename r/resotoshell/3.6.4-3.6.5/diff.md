# Comparing `tmp/resotoshell-3.6.4.tar.gz` & `tmp/resotoshell-3.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotoshell-3.6.4.tar", last modified: Mon Jul 24 18:29:40 2023, max compression
+gzip compressed data, was "resotoshell-3.6.5.tar", last modified: Wed Aug  2 19:22:23 2023, max compression
```

## Comparing `resotoshell-3.6.4.tar` & `resotoshell-3.6.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:29:40.922045 resotoshell-3.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 18:24:30.000000 resotoshell-3.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-24 18:29:40.922045 resotoshell-3.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-07-24 18:24:30.000000 resotoshell-3.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-24 18:24:30.000000 resotoshell-3.6.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:29:40.918045 resotoshell-3.6.4/resotoshell/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-24 18:24:30.000000 resotoshell-3.6.4/resotoshell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-07-24 18:24:30.000000 resotoshell-3.6.4/resotoshell/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-07-24 18:24:30.000000 resotoshell-3.6.4/resotoshell/authorized_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    37474 2023-07-24 18:24:30.000000 resotoshell-3.6.4/resotoshell/promptsession.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-24 18:24:30.000000 resotoshell-3.6.4/resotoshell/protected_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     9941 2023-07-24 18:24:30.000000 resotoshell-3.6.4/resotoshell/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:29:40.922045 resotoshell-3.6.4/resotoshell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-24 18:29:40.000000 resotoshell-3.6.4/resotoshell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-24 18:29:40.000000 resotoshell-3.6.4/resotoshell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:29:40.000000 resotoshell-3.6.4/resotoshell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-24 18:29:40.000000 resotoshell-3.6.4/resotoshell.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:26:00.000000 resotoshell-3.6.4/resotoshell.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-24 18:29:40.000000 resotoshell-3.6.4/resotoshell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 18:29:40.000000 resotoshell-3.6.4/resotoshell.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-24 18:29:40.922045 resotoshell-3.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:29:40.922045 resotoshell-3.6.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-24 18:24:30.000000 resotoshell-3.6.4/test/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    14196 2023-07-24 18:24:30.000000 resotoshell-3.6.4/test/test_promptsession.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-24 18:24:30.000000 resotoshell-3.6.4/test/test_protected_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:23.119378 resotoshell-3.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 19:17:16.000000 resotoshell-3.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-08-02 19:22:23.119378 resotoshell-3.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-08-02 19:17:16.000000 resotoshell-3.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-08-02 19:17:16.000000 resotoshell-3.6.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:23.119378 resotoshell-3.6.5/resotoshell/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-08-02 19:17:16.000000 resotoshell-3.6.5/resotoshell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-08-02 19:17:16.000000 resotoshell-3.6.5/resotoshell/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-08-02 19:17:16.000000 resotoshell-3.6.5/resotoshell/authorized_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37474 2023-08-02 19:17:16.000000 resotoshell-3.6.5/resotoshell/promptsession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-02 19:17:16.000000 resotoshell-3.6.5/resotoshell/protected_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9941 2023-08-02 19:17:16.000000 resotoshell-3.6.5/resotoshell/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:23.119378 resotoshell-3.6.5/resotoshell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-08-02 19:22:23.000000 resotoshell-3.6.5/resotoshell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-02 19:22:23.000000 resotoshell-3.6.5/resotoshell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:22:23.000000 resotoshell-3.6.5/resotoshell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-02 19:22:23.000000 resotoshell-3.6.5/resotoshell.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:18:45.000000 resotoshell-3.6.5/resotoshell.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-02 19:22:23.000000 resotoshell-3.6.5/resotoshell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-02 19:22:23.000000 resotoshell-3.6.5/resotoshell.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-02 19:22:23.123379 resotoshell-3.6.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:22:23.119378 resotoshell-3.6.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-02 19:17:16.000000 resotoshell-3.6.5/test/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14196 2023-08-02 19:17:16.000000 resotoshell-3.6.5/test/test_promptsession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-08-02 19:17:16.000000 resotoshell-3.6.5/test/test_protected_files.py
```

### Comparing `resotoshell-3.6.4/PKG-INFO` & `resotoshell-3.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoshell
-Version: 3.6.4
+Version: 3.6.5
 Summary: Commandline interpreter to interact with Resoto.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotoshell
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
```

### Comparing `resotoshell-3.6.4/README.md` & `resotoshell-3.6.5/README.md`

 * *Files identical despite different names*

### Comparing `resotoshell-3.6.4/pyproject.toml` & `resotoshell-3.6.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resotoshell"
-version = "3.6.4"
+version = "3.6.5"
 authors = [{name="Some Engineering Inc."}]
 description = "Commandline interpreter to interact with Resoto."
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
@@ -24,15 +24,15 @@
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 keywords = ["cloud security"]
 
 dependencies = [
-    "resotolib==3.6.4",
+    "resotolib==3.6.5",
     "prompt-toolkit",
     "rich",
     "resotoclient",
     "aiohttp[speedups]",
 ]
 
 [project.scripts]
```

### Comparing `resotoshell-3.6.4/resotoshell/__main__.py` & `resotoshell-3.6.5/resotoshell/__main__.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.6.4/resotoshell/authorized_client.py` & `resotoshell-3.6.5/resotoshell/authorized_client.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.6.4/resotoshell/promptsession.py` & `resotoshell-3.6.5/resotoshell/promptsession.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.6.4/resotoshell/protected_files.py` & `resotoshell-3.6.5/resotoshell/protected_files.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.6.4/resotoshell/shell.py` & `resotoshell-3.6.5/resotoshell/shell.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.6.4/resotoshell.egg-info/PKG-INFO` & `resotoshell-3.6.5/resotoshell.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoshell
-Version: 3.6.4
+Version: 3.6.5
 Summary: Commandline interpreter to interact with Resoto.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotoshell
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
```

### Comparing `resotoshell-3.6.4/resotoshell.egg-info/SOURCES.txt` & `resotoshell-3.6.5/resotoshell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resotoshell-3.6.4/test/test_promptsession.py` & `resotoshell-3.6.5/test/test_promptsession.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.6.4/test/test_protected_files.py` & `resotoshell-3.6.5/test/test_protected_files.py`

 * *Files identical despite different names*


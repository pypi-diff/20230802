# Comparing `tmp/lsstream-1.2.0.tar.gz` & `tmp/lsstream-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsstream-1.2.0.tar", last modified: Wed Aug  2 20:38:48 2023, max compression
+gzip compressed data, was "lsstream-1.2.1.tar", last modified: Wed Aug  2 20:47:57 2023, max compression
```

## Comparing `lsstream-1.2.0.tar` & `lsstream-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:38:48.107345 lsstream-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-02 20:38:38.000000 lsstream-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-08-02 20:38:48.107345 lsstream-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-08-02 20:38:38.000000 lsstream-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-02 20:38:38.000000 lsstream-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 20:38:48.107345 lsstream-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:38:48.107345 lsstream-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:38:48.107345 lsstream-1.2.0/src/lsstream/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 20:38:38.000000 lsstream-1.2.0/src/lsstream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-02 20:38:38.000000 lsstream-1.2.0/src/lsstream/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-02 20:38:38.000000 lsstream-1.2.0/src/lsstream/file_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-08-02 20:38:38.000000 lsstream-1.2.0/src/lsstream/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-08-02 20:38:38.000000 lsstream-1.2.0/src/lsstream/run.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-02 20:38:38.000000 lsstream-1.2.0/src/lsstream/style.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-02 20:38:38.000000 lsstream-1.2.0/src/lsstream/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:38:48.107345 lsstream-1.2.0/src/lsstream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-08-02 20:38:48.000000 lsstream-1.2.0/src/lsstream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-02 20:38:48.000000 lsstream-1.2.0/src/lsstream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 20:38:48.000000 lsstream-1.2.0/src/lsstream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 20:38:48.000000 lsstream-1.2.0/src/lsstream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 20:38:48.000000 lsstream-1.2.0/src/lsstream.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:47:57.234718 lsstream-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-02 20:47:47.000000 lsstream-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-08-02 20:47:57.234718 lsstream-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-08-02 20:47:47.000000 lsstream-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-02 20:47:47.000000 lsstream-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 20:47:57.234718 lsstream-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:47:57.230718 lsstream-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:47:57.234718 lsstream-1.2.1/src/lsstream/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 20:47:47.000000 lsstream-1.2.1/src/lsstream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-02 20:47:47.000000 lsstream-1.2.1/src/lsstream/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-02 20:47:47.000000 lsstream-1.2.1/src/lsstream/file_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-08-02 20:47:47.000000 lsstream-1.2.1/src/lsstream/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-08-02 20:47:47.000000 lsstream-1.2.1/src/lsstream/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-02 20:47:47.000000 lsstream-1.2.1/src/lsstream/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-02 20:47:47.000000 lsstream-1.2.1/src/lsstream/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:47:57.234718 lsstream-1.2.1/src/lsstream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-08-02 20:47:57.000000 lsstream-1.2.1/src/lsstream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-02 20:47:57.000000 lsstream-1.2.1/src/lsstream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 20:47:57.000000 lsstream-1.2.1/src/lsstream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 20:47:57.000000 lsstream-1.2.1/src/lsstream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 20:47:57.000000 lsstream-1.2.1/src/lsstream.egg-info/top_level.txt
```

### Comparing `lsstream-1.2.0/LICENSE` & `lsstream-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lsstream-1.2.0/PKG-INFO` & `lsstream-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsstream
-Version: 1.2.0
+Version: 1.2.1
 Summary: To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests 😴 🖥️ 🎞️
 Author-email: Wermutton <redacted@redacted.redacted>
 Project-URL: Homepage, https://github.com/Wermutton/lsstream
 Project-URL: Bug Tracker, https://github.com/Wermutton/lsstream/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lsstream-1.2.0/README.md` & `lsstream-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lsstream-1.2.0/pyproject.toml` & `lsstream-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lsstream"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="Wermutton", email="redacted@redacted.redacted" },
 ]
 description = "To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests 😴 🖥️ 🎞️"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `lsstream-1.2.0/src/lsstream/file_generation.py` & `lsstream-1.2.1/src/lsstream/file_generation.py`

 * *Files identical despite different names*

### Comparing `lsstream-1.2.0/src/lsstream/prompts.py` & `lsstream-1.2.1/src/lsstream/prompts.py`

 * *Files identical despite different names*

### Comparing `lsstream-1.2.0/src/lsstream/run.py` & `lsstream-1.2.1/src/lsstream/run.py`

 * *Files identical despite different names*

### Comparing `lsstream-1.2.0/src/lsstream.egg-info/PKG-INFO` & `lsstream-1.2.1/src/lsstream.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsstream
-Version: 1.2.0
+Version: 1.2.1
 Summary: To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests 😴 🖥️ 🎞️
 Author-email: Wermutton <redacted@redacted.redacted>
 Project-URL: Homepage, https://github.com/Wermutton/lsstream
 Project-URL: Bug Tracker, https://github.com/Wermutton/lsstream/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


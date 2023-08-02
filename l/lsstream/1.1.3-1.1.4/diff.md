# Comparing `tmp/lsstream-1.1.3.tar.gz` & `tmp/lsstream-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsstream-1.1.3.tar", last modified: Wed Aug  2 19:40:30 2023, max compression
+gzip compressed data, was "lsstream-1.1.4.tar", last modified: Wed Aug  2 19:44:29 2023, max compression
```

## Comparing `lsstream-1.1.3.tar` & `lsstream-1.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:40:30.984837 lsstream-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-02 19:40:21.000000 lsstream-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-08-02 19:40:30.984837 lsstream-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-08-02 19:40:21.000000 lsstream-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-02 19:40:21.000000 lsstream-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 19:40:30.984837 lsstream-1.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:40:30.984837 lsstream-1.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:40:30.984837 lsstream-1.1.3/src/lsstream/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:40:21.000000 lsstream-1.1.3/src/lsstream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-02 19:40:21.000000 lsstream-1.1.3/src/lsstream/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-08-02 19:40:21.000000 lsstream-1.1.3/src/lsstream/file_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-08-02 19:40:21.000000 lsstream-1.1.3/src/lsstream/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-08-02 19:40:21.000000 lsstream-1.1.3/src/lsstream/run.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-02 19:40:21.000000 lsstream-1.1.3/src/lsstream/style.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-02 19:40:21.000000 lsstream-1.1.3/src/lsstream/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:40:30.984837 lsstream-1.1.3/src/lsstream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-08-02 19:40:30.000000 lsstream-1.1.3/src/lsstream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-02 19:40:30.000000 lsstream-1.1.3/src/lsstream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:40:30.000000 lsstream-1.1.3/src/lsstream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 19:40:30.000000 lsstream-1.1.3/src/lsstream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 19:40:30.000000 lsstream-1.1.3/src/lsstream.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:44:29.533567 lsstream-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-02 19:44:19.000000 lsstream-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-08-02 19:44:29.533567 lsstream-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-08-02 19:44:19.000000 lsstream-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-02 19:44:19.000000 lsstream-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 19:44:29.533567 lsstream-1.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:44:29.529567 lsstream-1.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:44:29.533567 lsstream-1.1.4/src/lsstream/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:44:19.000000 lsstream-1.1.4/src/lsstream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-02 19:44:19.000000 lsstream-1.1.4/src/lsstream/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-08-02 19:44:19.000000 lsstream-1.1.4/src/lsstream/file_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-08-02 19:44:19.000000 lsstream-1.1.4/src/lsstream/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-08-02 19:44:19.000000 lsstream-1.1.4/src/lsstream/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-02 19:44:19.000000 lsstream-1.1.4/src/lsstream/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-08-02 19:44:19.000000 lsstream-1.1.4/src/lsstream/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:44:29.533567 lsstream-1.1.4/src/lsstream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-08-02 19:44:29.000000 lsstream-1.1.4/src/lsstream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-02 19:44:29.000000 lsstream-1.1.4/src/lsstream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:44:29.000000 lsstream-1.1.4/src/lsstream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 19:44:29.000000 lsstream-1.1.4/src/lsstream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 19:44:29.000000 lsstream-1.1.4/src/lsstream.egg-info/top_level.txt
```

### Comparing `lsstream-1.1.3/LICENSE` & `lsstream-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lsstream-1.1.3/PKG-INFO` & `lsstream-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsstream
-Version: 1.1.3
+Version: 1.1.4
 Summary: To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests 😴 🖥️ 🎞️
 Author-email: Wermutton <redacted@redacted.redacted>
 Project-URL: Homepage, https://github.com/Wermutton/lsstream
 Project-URL: Bug Tracker, https://github.com/Wermutton/lsstream/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lsstream-1.1.3/README.md` & `lsstream-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `lsstream-1.1.3/pyproject.toml` & `lsstream-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lsstream"
-version = "1.1.3"
+version = "1.1.4"
 authors = [
   { name="Wermutton", email="redacted@redacted.redacted" },
 ]
 description = "To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests 😴 🖥️ 🎞️"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `lsstream-1.1.3/src/lsstream/file_generation.py` & `lsstream-1.1.4/src/lsstream/file_generation.py`

 * *Files identical despite different names*

### Comparing `lsstream-1.1.3/src/lsstream/prompts.py` & `lsstream-1.1.4/src/lsstream/prompts.py`

 * *Files identical despite different names*

### Comparing `lsstream-1.1.3/src/lsstream/run.py` & `lsstream-1.1.4/src/lsstream/run.py`

 * *Files identical despite different names*

### Comparing `lsstream-1.1.3/src/lsstream.egg-info/PKG-INFO` & `lsstream-1.1.4/src/lsstream.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsstream
-Version: 1.1.3
+Version: 1.1.4
 Summary: To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests 😴 🖥️ 🎞️
 Author-email: Wermutton <redacted@redacted.redacted>
 Project-URL: Homepage, https://github.com/Wermutton/lsstream
 Project-URL: Bug Tracker, https://github.com/Wermutton/lsstream/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


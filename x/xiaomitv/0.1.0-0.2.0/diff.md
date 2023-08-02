# Comparing `tmp/xiaomitv-0.1.0.tar.gz` & `tmp/xiaomitv-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaomitv-0.1.0.tar", last modified: Wed Aug  2 03:58:33 2023, max compression
+gzip compressed data, was "xiaomitv-0.2.0.tar", last modified: Wed Aug  2 04:26:46 2023, max compression
```

## Comparing `xiaomitv-0.1.0.tar` & `xiaomitv-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-02 03:58:33.464590 xiaomitv-0.1.0/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:39.000000 xiaomitv-0.1.0/LICENSE
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      555 2023-08-02 03:58:33.464590 xiaomitv-0.1.0/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       12 2023-08-02 03:55:35.000000 xiaomitv-0.1.0/README.md
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      676 2023-08-02 03:54:32.000000 xiaomitv-0.1.0/pyproject.toml
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-08-02 03:58:33.464590 xiaomitv-0.1.0/setup.cfg
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-02 03:58:33.460590 xiaomitv-0.1.0/src/
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-02 03:58:33.460590 xiaomitv-0.1.0/src/xiaomi_tv/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     4509 2023-08-01 09:07:01.000000 xiaomitv-0.1.0/src/xiaomi_tv/__init__.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-02 03:58:33.464590 xiaomitv-0.1.0/src/xiaomitv.egg-info/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      555 2023-08-02 03:58:33.000000 xiaomitv-0.1.0/src/xiaomitv.egg-info/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      237 2023-08-02 03:58:33.000000 xiaomitv-0.1.0/src/xiaomitv.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-08-02 03:58:33.000000 xiaomitv-0.1.0/src/xiaomitv.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       15 2023-08-02 03:58:33.000000 xiaomitv-0.1.0/src/xiaomitv.egg-info/requires.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       10 2023-08-02 03:58:33.000000 xiaomitv-0.1.0/src/xiaomitv.egg-info/top_level.txt
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-02 04:26:46.544285 xiaomitv-0.2.0/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:39.000000 xiaomitv-0.2.0/LICENSE
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      555 2023-08-02 04:26:46.544285 xiaomitv-0.2.0/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       12 2023-08-02 03:55:35.000000 xiaomitv-0.2.0/README.md
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      676 2023-08-02 04:26:36.000000 xiaomitv-0.2.0/pyproject.toml
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-08-02 04:26:46.544285 xiaomitv-0.2.0/setup.cfg
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-02 04:26:46.540285 xiaomitv-0.2.0/src/
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-02 04:26:46.540285 xiaomitv-0.2.0/src/xiaomitv/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     4509 2023-08-01 09:07:01.000000 xiaomitv-0.2.0/src/xiaomitv/__init__.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-02 04:26:46.544285 xiaomitv-0.2.0/src/xiaomitv.egg-info/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      555 2023-08-02 04:26:46.000000 xiaomitv-0.2.0/src/xiaomitv.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      236 2023-08-02 04:26:46.000000 xiaomitv-0.2.0/src/xiaomitv.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-08-02 04:26:46.000000 xiaomitv-0.2.0/src/xiaomitv.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       15 2023-08-02 04:26:46.000000 xiaomitv-0.2.0/src/xiaomitv.egg-info/requires.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        9 2023-08-02 04:26:46.000000 xiaomitv-0.2.0/src/xiaomitv.egg-info/top_level.txt
```

### Comparing `xiaomitv-0.1.0/LICENSE` & `xiaomitv-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaomitv-0.1.0/PKG-INFO` & `xiaomitv-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaomitv
-Version: 0.1.0
+Version: 0.2.0
 Summary: Remote control for Xiaomi TVs
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/xiaomitv
 Project-URL: Bug Tracker, https://github.com/zhbjsh/xiaomitv/issues
 Keywords: xiaomi tv,mi tv,xiaomi,remote control
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `xiaomitv-0.1.0/pyproject.toml` & `xiaomitv-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xiaomitv"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Remote control for Xiaomi TVs"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `xiaomitv-0.1.0/src/xiaomi_tv/__init__.py` & `xiaomitv-0.2.0/src/xiaomitv/__init__.py`

 * *Files identical despite different names*

### Comparing `xiaomitv-0.1.0/src/xiaomitv.egg-info/PKG-INFO` & `xiaomitv-0.2.0/src/xiaomitv.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaomitv
-Version: 0.1.0
+Version: 0.2.0
 Summary: Remote control for Xiaomi TVs
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/xiaomitv
 Project-URL: Bug Tracker, https://github.com/zhbjsh/xiaomitv/issues
 Keywords: xiaomi tv,mi tv,xiaomi,remote control
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```


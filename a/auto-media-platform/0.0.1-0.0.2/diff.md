# Comparing `tmp/auto_media_platform-0.0.1.tar.gz` & `tmp/auto_media_platform-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_media_platform-0.0.1.tar", max compression
+gzip compressed data, was "auto_media_platform-0.0.2.tar", max compression
```

## Comparing `auto_media_platform-0.0.1.tar` & `auto_media_platform-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-08-02 15:22:43.172769 auto_media_platform-0.0.1/LICENSE
--rw-r--r--   0        0        0      156 2023-08-02 15:22:43.161464 auto_media_platform-0.0.1/README.md
--rw-r--r--   0        0        0      453 2023-08-02 15:22:43.170278 auto_media_platform-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-02 15:13:26.021330 auto_media_platform-0.0.1/src/auto_media_platform/__init__.py
--rw-r--r--   0        0        0      282 2023-08-02 15:27:52.529290 auto_media_platform-0.0.1/src/auto_media_platform/__version__.py
--rw-r--r--   0        0        0       78 2023-08-02 15:29:11.815674 auto_media_platform-0.0.1/src/auto_media_platform/main.py
--rw-r--r--   0        0        0      779 1970-01-01 00:00:00.000000 auto_media_platform-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-02 15:22:43.172769 auto_media_platform-0.0.2/LICENSE
+-rw-r--r--   0        0        0      193 2023-08-02 15:37:16.595456 auto_media_platform-0.0.2/README.md
+-rw-r--r--   0        0        0      453 2023-08-02 15:37:51.410538 auto_media_platform-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-02 15:13:26.021330 auto_media_platform-0.0.2/src/auto_media_platform/__init__.py
+-rw-r--r--   0        0        0      282 2023-08-02 15:38:01.604776 auto_media_platform-0.0.2/src/auto_media_platform/__version__.py
+-rw-r--r--   0        0        0       78 2023-08-02 15:29:11.815674 auto_media_platform-0.0.2/src/auto_media_platform/main.py
+-rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 auto_media_platform-0.0.2/PKG-INFO
```

### Comparing `auto_media_platform-0.0.1/LICENSE` & `auto_media_platform-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_media_platform-0.0.1/PKG-INFO` & `auto_media_platform-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-media-platform
-Version: 0.0.1
+Version: 0.0.2
 Summary: generate video and upload to multiple media platform automatically
 License: MIT
 Author: idlewith
 Author-email: newellzhou@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,21 @@
 Description-Content-Type: text/markdown
 
 # Auto Media Platform
 
 generate video and upload to multiple media platform automatically
 
 
-## install ask_robot
+## install auto_media_platform
 
 ```
 pip install auto_media_platform
 ```
 
+## how to use
+
+```
+mp
+```
+
```


# Comparing `tmp/auto_media_platform-0.0.2.tar.gz` & `tmp/auto_media_platform-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_media_platform-0.0.2.tar", max compression
+gzip compressed data, was "auto_media_platform-0.0.3.tar", max compression
```

## Comparing `auto_media_platform-0.0.2.tar` & `auto_media_platform-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1065 2023-08-02 15:22:43.172769 auto_media_platform-0.0.2/LICENSE
--rw-r--r--   0        0        0      193 2023-08-02 15:37:16.595456 auto_media_platform-0.0.2/README.md
--rw-r--r--   0        0        0      453 2023-08-02 15:37:51.410538 auto_media_platform-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-02 15:13:26.021330 auto_media_platform-0.0.2/src/auto_media_platform/__init__.py
--rw-r--r--   0        0        0      282 2023-08-02 15:38:01.604776 auto_media_platform-0.0.2/src/auto_media_platform/__version__.py
--rw-r--r--   0        0        0       78 2023-08-02 15:29:11.815674 auto_media_platform-0.0.2/src/auto_media_platform/main.py
--rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 auto_media_platform-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-02 15:22:43.172769 auto_media_platform-0.0.3/LICENSE
+-rw-r--r--   0        0        0      193 2023-08-02 15:37:16.595456 auto_media_platform-0.0.3/README.md
+-rw-r--r--   0        0        0      732 2023-08-02 16:00:36.334896 auto_media_platform-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-02 15:13:26.021330 auto_media_platform-0.0.3/src/auto_media_platform/__init__.py
+-rw-r--r--   0        0        0       78 2023-08-02 15:29:11.815674 auto_media_platform-0.0.3/src/auto_media_platform/main.py
+-rw-r--r--   0        0        0     1093 1970-01-01 00:00:00.000000 auto_media_platform-0.0.3/PKG-INFO
```

### Comparing `auto_media_platform-0.0.2/LICENSE` & `auto_media_platform-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_media_platform-0.0.2/PKG-INFO` & `auto_media_platform-0.0.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 Metadata-Version: 2.1
 Name: auto-media-platform
-Version: 0.0.2
+Version: 0.0.3
 Summary: generate video and upload to multiple media platform automatically
+Home-page: https://github.com/idlewith/auto_media_platform
 License: MIT
 Author: idlewith
 Author-email: newellzhou@163.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.7,<4
+Classifier: Development Status :: 1 - Planning
+Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```


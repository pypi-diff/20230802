# Comparing `tmp/efrem_utils-0.1.5.tar.gz` & `tmp/efrem_utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efrem_utils-0.1.5.tar", max compression
+gzip compressed data, was "efrem_utils-0.2.0.tar", max compression
```

## Comparing `efrem_utils-0.1.5.tar` & `efrem_utils-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4683 2023-08-01 22:52:36.611027 efrem_utils-0.1.5/efrem_utils.py
--rw-r--r--   0        0        0     1087 2023-07-13 00:02:18.108824 efrem_utils-0.1.5/LICENSE
--rw-r--r--   0        0        0      361 2023-08-01 22:53:36.708740 efrem_utils-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3010 2023-08-01 19:41:39.325507 efrem_utils-0.1.5/README.md
--rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 efrem_utils-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11332 2023-08-02 12:54:32.674919 efrem_utils-0.2.0/efrem_utils.py
+-rw-r--r--   0        0        0     1087 2023-07-13 00:02:18.108824 efrem_utils-0.2.0/LICENSE
+-rw-r--r--   0        0        0      361 2023-08-02 12:54:17.079720 efrem_utils-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3010 2023-08-01 19:41:39.325507 efrem_utils-0.2.0/README.md
+-rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 efrem_utils-0.2.0/PKG-INFO
```

### Comparing `efrem_utils-0.1.5/LICENSE` & `efrem_utils-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `efrem_utils-0.1.5/README.md` & `efrem_utils-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `efrem_utils-0.1.5/PKG-INFO` & `efrem_utils-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efrem-utils
-Version: 0.1.5
+Version: 0.2.0
 Summary: Efrem's utilities
 Home-page: https://github.com/NikitaNightBot/efrem-utils
 Author: lone_druid
 Author-email: enikita332@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```


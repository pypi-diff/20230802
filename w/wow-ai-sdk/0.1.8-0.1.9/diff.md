# Comparing `tmp/wow_ai_sdk-0.1.8.tar.gz` & `tmp/wow_ai_sdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wow_ai_sdk-0.1.8.tar", max compression
+gzip compressed data, was "wow_ai_sdk-0.1.9.tar", max compression
```

## Comparing `wow_ai_sdk-0.1.8.tar` & `wow_ai_sdk-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     7857 2023-06-30 11:57:05.323031 wow_ai_sdk-0.1.8/README.md
--rw-r--r--   0        0        0      262 2023-08-02 05:21:12.362050 wow_ai_sdk-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      149 2023-01-28 11:24:39.272410 wow_ai_sdk-0.1.8/wow_ai_sdk/__init__.py
--rw-r--r--   0        0        0     8908 2023-08-01 04:06:56.101016 wow_ai_sdk-0.1.8/wow_ai_sdk/client.py
--rw-r--r--   0        0        0     7914 2023-01-28 11:24:40.157550 wow_ai_sdk-0.1.8/wow_ai_sdk/data_manager.py
--rw-r--r--   0        0        0    68851 2023-08-01 04:06:56.102486 wow_ai_sdk-0.1.8/wow_ai_sdk/project.py
--rw-r--r--   0        0        0     1325 2023-01-28 11:24:40.436036 wow_ai_sdk-0.1.8/wow_ai_sdk/users.py
--rw-r--r--   0        0        0     4218 2023-01-28 11:24:40.801400 wow_ai_sdk-0.1.8/wow_ai_sdk/utils.py
--rw-r--r--   0        0        0     1889 2023-01-28 11:24:41.002364 wow_ai_sdk-0.1.8/wow_ai_sdk/workspaces.py
--rw-r--r--   0        0        0     8289 1970-01-01 00:00:00.000000 wow_ai_sdk-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     7857 2023-06-30 11:57:05.323031 wow_ai_sdk-0.1.9/README.md
+-rw-r--r--   0        0        0      262 2023-08-02 05:42:32.233487 wow_ai_sdk-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      149 2023-01-28 11:24:39.272410 wow_ai_sdk-0.1.9/wow_ai_sdk/__init__.py
+-rw-r--r--   0        0        0     8908 2023-08-01 04:06:56.101016 wow_ai_sdk-0.1.9/wow_ai_sdk/client.py
+-rw-r--r--   0        0        0     7914 2023-01-28 11:24:40.157550 wow_ai_sdk-0.1.9/wow_ai_sdk/data_manager.py
+-rw-r--r--   0        0        0    68851 2023-08-01 04:06:56.102486 wow_ai_sdk-0.1.9/wow_ai_sdk/project.py
+-rw-r--r--   0        0        0     1325 2023-01-28 11:24:40.436036 wow_ai_sdk-0.1.9/wow_ai_sdk/users.py
+-rw-r--r--   0        0        0     4218 2023-01-28 11:24:40.801400 wow_ai_sdk-0.1.9/wow_ai_sdk/utils.py
+-rw-r--r--   0        0        0     1889 2023-01-28 11:24:41.002364 wow_ai_sdk-0.1.9/wow_ai_sdk/workspaces.py
+-rw-r--r--   0        0        0     8289 1970-01-01 00:00:00.000000 wow_ai_sdk-0.1.9/PKG-INFO
```

### Comparing `wow_ai_sdk-0.1.8/README.md` & `wow_ai_sdk-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `wow_ai_sdk-0.1.8/wow_ai_sdk/client.py` & `wow_ai_sdk-0.1.9/wow_ai_sdk/client.py`

 * *Files identical despite different names*

### Comparing `wow_ai_sdk-0.1.8/wow_ai_sdk/data_manager.py` & `wow_ai_sdk-0.1.9/wow_ai_sdk/data_manager.py`

 * *Files identical despite different names*

### Comparing `wow_ai_sdk-0.1.8/wow_ai_sdk/project.py` & `wow_ai_sdk-0.1.9/wow_ai_sdk/project.py`

 * *Files identical despite different names*

### Comparing `wow_ai_sdk-0.1.8/wow_ai_sdk/users.py` & `wow_ai_sdk-0.1.9/wow_ai_sdk/users.py`

 * *Files identical despite different names*

### Comparing `wow_ai_sdk-0.1.8/wow_ai_sdk/utils.py` & `wow_ai_sdk-0.1.9/wow_ai_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `wow_ai_sdk-0.1.8/wow_ai_sdk/workspaces.py` & `wow_ai_sdk-0.1.9/wow_ai_sdk/workspaces.py`

 * *Files identical despite different names*

### Comparing `wow_ai_sdk-0.1.8/PKG-INFO` & `wow_ai_sdk-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wow-ai-sdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: TonyShark
 Author-email: quoi@wow-ai.inc
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


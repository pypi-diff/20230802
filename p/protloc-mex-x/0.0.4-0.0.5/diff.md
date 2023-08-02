# Comparing `tmp/protloc_mex_x-0.0.4.tar.gz` & `tmp/protloc_mex_x-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protloc_mex_x-0.0.4.tar", max compression
+gzip compressed data, was "protloc_mex_x-0.0.5.tar", max compression
```

## Comparing `protloc_mex_x-0.0.4.tar` & `protloc_mex_x-0.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1091 2023-04-25 08:38:35.586641 protloc_mex_x-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0        2 2023-05-09 03:41:02.000000 protloc_mex_x-0.0.4/protloc_mex_X/__init__.py
--rw-r--r--   0        0        0    39068 2023-06-01 11:45:18.000000 protloc_mex_x-0.0.4/protloc_mex_X/ESM2_fr.py
--rw-r--r--   0        0        0     2999 2023-05-08 12:33:04.000000 protloc_mex_x-0.0.4/protloc_mex_X/examples/test1.txt
--rw-r--r--   0        0        0     2749 2023-05-09 03:13:02.000000 protloc_mex_x-0.0.4/protloc_mex_X/feature_corrlation.py
--rw-r--r--   0        0        0      863 2023-06-02 07:08:20.652284 protloc_mex_x-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       35 2023-05-10 08:06:08.458858 protloc_mex_x-0.0.4/README.md
--rw-r--r--   0        0        0     1024 1970-01-01 00:00:00.000000 protloc_mex_x-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-04-25 08:38:35.586641 protloc_mex_x-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0        2 2023-05-09 03:41:02.000000 protloc_mex_x-0.0.5/protloc_mex_X/__init__.py
+-rw-r--r--   0        0        0    39068 2023-06-01 11:45:18.000000 protloc_mex_x-0.0.5/protloc_mex_X/ESM2_fr.py
+-rw-r--r--   0        0        0     2999 2023-05-08 12:33:04.000000 protloc_mex_x-0.0.5/protloc_mex_X/examples/test1.txt
+-rw-r--r--   0        0        0     2749 2023-05-09 03:13:02.000000 protloc_mex_x-0.0.5/protloc_mex_X/feature_corrlation.py
+-rw-r--r--   0        0        0      863 2023-08-02 04:10:05.751249 protloc_mex_x-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     6573 2023-08-02 04:09:16.308133 protloc_mex_x-0.0.5/README.md
+-rw-r--r--   0        0        0     7452 1970-01-01 00:00:00.000000 protloc_mex_x-0.0.5/PKG-INFO
```

### Comparing `protloc_mex_x-0.0.4/LICENSE.txt` & `protloc_mex_x-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `protloc_mex_x-0.0.4/protloc_mex_X/ESM2_fr.py` & `protloc_mex_x-0.0.5/protloc_mex_X/ESM2_fr.py`

 * *Files identical despite different names*

### Comparing `protloc_mex_x-0.0.4/protloc_mex_X/examples/test1.txt` & `protloc_mex_x-0.0.5/protloc_mex_X/examples/test1.txt`

 * *Files identical despite different names*

### Comparing `protloc_mex_x-0.0.4/protloc_mex_X/feature_corrlation.py` & `protloc_mex_x-0.0.5/protloc_mex_X/feature_corrlation.py`

 * *Files identical despite different names*

### Comparing `protloc_mex_x-0.0.4/pyproject.toml` & `protloc_mex_x-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "protloc_mex_X"
-version = "0.0.4"
+version = "0.0.5"
 description = "Internal use kit"
 authors = ["Ze Yu Luo <1024226968@qq.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/yujuan-zhang/ProtLoc-mexl"
 repository = "https://github.com/yujuan-zhang/ProtLoc-mexl"
 documentation = "https://github.com/yujuan-zhang/ProtLoc-mexl/issues"
```


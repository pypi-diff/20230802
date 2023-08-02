# Comparing `tmp/sungrow_http_config-0.0.2.tar.gz` & `tmp/sungrow_http_config-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sungrow_http_config-0.0.2.tar", last modified: Wed Aug  2 01:04:01 2023, max compression
+gzip compressed data, was "sungrow_http_config-0.0.3.tar", last modified: Wed Aug  2 01:09:33 2023, max compression
```

## Comparing `sungrow_http_config-0.0.2.tar` & `sungrow_http_config-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-02 01:04:01.400730 sungrow_http_config-0.0.2/
--rw-r--r--   0 ross       (501) staff       (20)     1072 2023-08-01 09:53:21.000000 sungrow_http_config-0.0.2/LICENSE
--rw-r--r--   0 ross       (501) staff       (20)     1305 2023-08-02 01:04:01.400417 sungrow_http_config-0.0.2/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)      747 2023-08-01 09:51:37.000000 sungrow_http_config-0.0.2/README.md
--rw-r--r--   0 ross       (501) staff       (20)      708 2023-08-02 01:03:50.000000 sungrow_http_config-0.0.2/pyproject.toml
--rw-r--r--   0 ross       (501) staff       (20)       38 2023-08-02 01:04:01.400823 sungrow_http_config-0.0.2/setup.cfg
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-02 01:04:01.394172 sungrow_http_config-0.0.2/src/
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-02 01:04:01.397700 sungrow_http_config-0.0.2/src/sungrow_http_config/
--rw-r--r--   0 ross       (501) staff       (20)     7222 2023-08-01 11:14:11.000000 sungrow_http_config-0.0.2/src/sungrow_http_config/SungrowHttpConfig.py
--rw-r--r--   0 ross       (501) staff       (20)        1 2023-08-01 09:55:24.000000 sungrow_http_config-0.0.2/src/sungrow_http_config/__init__.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-02 01:04:01.399982 sungrow_http_config-0.0.2/src/sungrow_http_config.egg-info/
--rw-r--r--   0 ross       (501) staff       (20)     1305 2023-08-02 01:04:01.000000 sungrow_http_config-0.0.2/src/sungrow_http_config.egg-info/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)      347 2023-08-02 01:04:01.000000 sungrow_http_config-0.0.2/src/sungrow_http_config.egg-info/SOURCES.txt
--rw-r--r--   0 ross       (501) staff       (20)        1 2023-08-02 01:04:01.000000 sungrow_http_config-0.0.2/src/sungrow_http_config.egg-info/dependency_links.txt
--rw-r--r--   0 ross       (501) staff       (20)       42 2023-08-02 01:04:01.000000 sungrow_http_config-0.0.2/src/sungrow_http_config.egg-info/requires.txt
--rw-r--r--   0 ross       (501) staff       (20)       20 2023-08-02 01:04:01.000000 sungrow_http_config-0.0.2/src/sungrow_http_config.egg-info/top_level.txt
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-02 01:09:33.564301 sungrow_http_config-0.0.3/
+-rw-r--r--   0 ross       (501) staff       (20)     1072 2023-08-01 09:53:21.000000 sungrow_http_config-0.0.3/LICENSE
+-rw-r--r--   0 ross       (501) staff       (20)     1305 2023-08-02 01:09:33.564035 sungrow_http_config-0.0.3/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)      747 2023-08-01 09:51:37.000000 sungrow_http_config-0.0.3/README.md
+-rw-r--r--   0 ross       (501) staff       (20)      698 2023-08-02 01:09:14.000000 sungrow_http_config-0.0.3/pyproject.toml
+-rw-r--r--   0 ross       (501) staff       (20)       38 2023-08-02 01:09:33.564394 sungrow_http_config-0.0.3/setup.cfg
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-02 01:09:33.557514 sungrow_http_config-0.0.3/src/
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-02 01:09:33.560613 sungrow_http_config-0.0.3/src/sungrow_http_config/
+-rw-r--r--   0 ross       (501) staff       (20)     7222 2023-08-01 11:14:11.000000 sungrow_http_config-0.0.3/src/sungrow_http_config/SungrowHttpConfig.py
+-rw-r--r--   0 ross       (501) staff       (20)        1 2023-08-01 09:55:24.000000 sungrow_http_config-0.0.3/src/sungrow_http_config/__init__.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-02 01:09:33.563626 sungrow_http_config-0.0.3/src/sungrow_http_config.egg-info/
+-rw-r--r--   0 ross       (501) staff       (20)     1305 2023-08-02 01:09:33.000000 sungrow_http_config-0.0.3/src/sungrow_http_config.egg-info/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)      347 2023-08-02 01:09:33.000000 sungrow_http_config-0.0.3/src/sungrow_http_config.egg-info/SOURCES.txt
+-rw-r--r--   0 ross       (501) staff       (20)        1 2023-08-02 01:09:33.000000 sungrow_http_config-0.0.3/src/sungrow_http_config.egg-info/dependency_links.txt
+-rw-r--r--   0 ross       (501) staff       (20)       37 2023-08-02 01:09:33.000000 sungrow_http_config-0.0.3/src/sungrow_http_config.egg-info/requires.txt
+-rw-r--r--   0 ross       (501) staff       (20)       20 2023-08-02 01:09:33.000000 sungrow_http_config-0.0.3/src/sungrow_http_config.egg-info/top_level.txt
```

### Comparing `sungrow_http_config-0.0.2/LICENSE` & `sungrow_http_config-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sungrow_http_config-0.0.2/PKG-INFO` & `sungrow_http_config-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sungrow_http_config
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package to manipulate settings on Sungrow Inverters
 Author-email: Ross Williamson <ross@inertia.net.nz>
 Project-URL: Homepage, https://github.com/ross-w/sungrow_exportlimit
 Project-URL: Bug Tracker, https://github.com/ross-w/sungrow_exportlimit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sungrow_http_config-0.0.2/README.md` & `sungrow_http_config-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `sungrow_http_config-0.0.2/pyproject.toml` & `sungrow_http_config-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sungrow_http_config"
-version = "0.0.2"
+version = "0.0.3"
 dependencies = [
   "requests_retry_on_exceptions",
-  "json",
   "urllib3",
 ]
 authors = [
   { name="Ross Williamson", email="ross@inertia.net.nz" },
 ]
 description = "A package to manipulate settings on Sungrow Inverters"
 readme = "README.md"
```

### Comparing `sungrow_http_config-0.0.2/src/sungrow_http_config/SungrowHttpConfig.py` & `sungrow_http_config-0.0.3/src/sungrow_http_config/SungrowHttpConfig.py`

 * *Files identical despite different names*

### Comparing `sungrow_http_config-0.0.2/src/sungrow_http_config.egg-info/PKG-INFO` & `sungrow_http_config-0.0.3/src/sungrow_http_config.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sungrow-http-config
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package to manipulate settings on Sungrow Inverters
 Author-email: Ross Williamson <ross@inertia.net.nz>
 Project-URL: Homepage, https://github.com/ross-w/sungrow_exportlimit
 Project-URL: Bug Tracker, https://github.com/ross-w/sungrow_exportlimit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


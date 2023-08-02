# Comparing `tmp/dataframe_api_compat-0.1.4.tar.gz` & `tmp/dataframe_api_compat-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataframe_api_compat-0.1.4.tar", last modified: Wed Aug  2 19:15:23 2023, max compression
+gzip compressed data, was "dataframe_api_compat-0.1.5.tar", last modified: Wed Aug  2 19:22:09 2023, max compression
```

## Comparing `dataframe_api_compat-0.1.4.tar` & `dataframe_api_compat-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 19:15:23.928086 dataframe_api_compat-0.1.4/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     1071 2023-05-05 10:36:05.000000 dataframe_api_compat-0.1.4/LICENSE
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     2365 2023-08-02 19:15:23.928086 dataframe_api_compat-0.1.4/PKG-INFO
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     1731 2023-08-02 10:23:41.000000 dataframe_api_compat-0.1.4/README.md
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 19:15:23.928086 dataframe_api_compat-0.1.4/dataframe_api_compat/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      184 2023-08-02 18:57:06.000000 dataframe_api_compat-0.1.4/dataframe_api_compat/__init__.py
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 19:15:23.928086 dataframe_api_compat-0.1.4/dataframe_api_compat/pandas_standard/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     4298 2023-08-02 15:50:33.000000 dataframe_api_compat-0.1.4/dataframe_api_compat/pandas_standard/__init__.py
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)    28860 2023-08-02 15:50:34.000000 dataframe_api_compat-0.1.4/dataframe_api_compat/pandas_standard/pandas_standard.py
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 19:15:23.928086 dataframe_api_compat-0.1.4/dataframe_api_compat/polars_standard/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     3740 2023-08-02 15:47:51.000000 dataframe_api_compat-0.1.4/dataframe_api_compat/polars_standard/__init__.py
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)    25380 2023-08-02 16:45:27.000000 dataframe_api_compat-0.1.4/dataframe_api_compat/polars_standard/polars_standard.py
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 19:15:23.928086 dataframe_api_compat-0.1.4/dataframe_api_compat.egg-info/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     2365 2023-08-02 19:15:23.000000 dataframe_api_compat-0.1.4/dataframe_api_compat.egg-info/PKG-INFO
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      470 2023-08-02 19:15:23.000000 dataframe_api_compat-0.1.4/dataframe_api_compat.egg-info/SOURCES.txt
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)        1 2023-08-02 19:15:23.000000 dataframe_api_compat-0.1.4/dataframe_api_compat.egg-info/dependency_links.txt
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)       21 2023-08-02 19:15:23.000000 dataframe_api_compat-0.1.4/dataframe_api_compat.egg-info/top_level.txt
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      449 2023-08-02 10:29:22.000000 dataframe_api_compat-0.1.4/pyproject.toml
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      835 2023-08-02 19:15:23.928086 dataframe_api_compat-0.1.4/setup.cfg
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)       74 2023-08-02 10:13:15.000000 dataframe_api_compat-0.1.4/setup.py
+drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 19:22:09.058094 dataframe_api_compat-0.1.5/
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     1071 2023-05-05 10:36:05.000000 dataframe_api_compat-0.1.5/LICENSE
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     2365 2023-08-02 19:22:09.058094 dataframe_api_compat-0.1.5/PKG-INFO
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     1731 2023-08-02 10:23:41.000000 dataframe_api_compat-0.1.5/README.md
+drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 19:22:09.048094 dataframe_api_compat-0.1.5/dataframe_api_compat/
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      184 2023-08-02 18:57:06.000000 dataframe_api_compat-0.1.5/dataframe_api_compat/__init__.py
+drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 19:22:09.058094 dataframe_api_compat-0.1.5/dataframe_api_compat/pandas_standard/
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     4298 2023-08-02 15:50:33.000000 dataframe_api_compat-0.1.5/dataframe_api_compat/pandas_standard/__init__.py
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)    28860 2023-08-02 15:50:34.000000 dataframe_api_compat-0.1.5/dataframe_api_compat/pandas_standard/pandas_standard.py
+drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 19:22:09.058094 dataframe_api_compat-0.1.5/dataframe_api_compat/polars_standard/
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     3740 2023-08-02 15:47:51.000000 dataframe_api_compat-0.1.5/dataframe_api_compat/polars_standard/__init__.py
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)    25380 2023-08-02 16:45:27.000000 dataframe_api_compat-0.1.5/dataframe_api_compat/polars_standard/polars_standard.py
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 19:14:05.000000 dataframe_api_compat-0.1.5/dataframe_api_compat/py.typed
+drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 19:22:09.058094 dataframe_api_compat-0.1.5/dataframe_api_compat.egg-info/
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     2365 2023-08-02 19:22:09.000000 dataframe_api_compat-0.1.5/dataframe_api_compat.egg-info/PKG-INFO
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      500 2023-08-02 19:22:09.000000 dataframe_api_compat-0.1.5/dataframe_api_compat.egg-info/SOURCES.txt
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)        1 2023-08-02 19:22:09.000000 dataframe_api_compat-0.1.5/dataframe_api_compat.egg-info/dependency_links.txt
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)       21 2023-08-02 19:22:09.000000 dataframe_api_compat-0.1.5/dataframe_api_compat.egg-info/top_level.txt
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      449 2023-08-02 10:29:22.000000 dataframe_api_compat-0.1.5/pyproject.toml
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      947 2023-08-02 19:22:09.058094 dataframe_api_compat-0.1.5/setup.cfg
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)       74 2023-08-02 10:13:15.000000 dataframe_api_compat-0.1.5/setup.py
```

### Comparing `dataframe_api_compat-0.1.4/LICENSE` & `dataframe_api_compat-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.1.4/PKG-INFO` & `dataframe_api_compat-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataframe_api_compat
-Version: 0.1.4
+Version: 0.1.5
 Summary: Implementation of the DataFrame Standard for pandas and polars
 Home-page: https://github.com/data-apis/dataframe-api-compat
 Author: Marco Gorelli
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dataframe_api_compat-0.1.4/README.md` & `dataframe_api_compat-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.1.4/dataframe_api_compat/pandas_standard/__init__.py` & `dataframe_api_compat-0.1.5/dataframe_api_compat/pandas_standard/__init__.py`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.1.4/dataframe_api_compat/pandas_standard/pandas_standard.py` & `dataframe_api_compat-0.1.5/dataframe_api_compat/pandas_standard/pandas_standard.py`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.1.4/dataframe_api_compat/polars_standard/__init__.py` & `dataframe_api_compat-0.1.5/dataframe_api_compat/polars_standard/__init__.py`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.1.4/dataframe_api_compat/polars_standard/polars_standard.py` & `dataframe_api_compat-0.1.5/dataframe_api_compat/polars_standard/polars_standard.py`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.1.4/dataframe_api_compat.egg-info/PKG-INFO` & `dataframe_api_compat-0.1.5/dataframe_api_compat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataframe-api-compat
-Version: 0.1.4
+Version: 0.1.5
 Summary: Implementation of the DataFrame Standard for pandas and polars
 Home-page: https://github.com/data-apis/dataframe-api-compat
 Author: Marco Gorelli
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dataframe_api_compat-0.1.4/setup.cfg` & `dataframe_api_compat-0.1.5/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dataframe_api_compat
-version = 0.1.4
+version = 0.1.5
 description = Implementation of the DataFrame Standard for pandas and polars
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/data-apis/dataframe-api-compat
 author = Marco Gorelli
 license = MIT
 license_files = LICENSE
@@ -12,17 +12,22 @@
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 
 [options]
+name = dataframe_api_compat
 packages = find:
 py_modules = dataframe_api_compat
 python_requires = >=3.8
+include-package-data = True
+
+[options.package_data]
+dataframe_api_compat = py.typed
 
 [options.packages.find]
 exclude = 
 	tests*
 	testing*
 
 [bdist_wheel]
```


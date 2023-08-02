# Comparing `tmp/valeriepieris-0.1.3.tar.gz` & `tmp/valeriepieris-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valeriepieris-0.1.3.tar", last modified: Wed Aug  2 06:39:07 2023, max compression
+gzip compressed data, was "valeriepieris-0.1.4.tar", last modified: Wed Aug  2 06:41:38 2023, max compression
```

## Comparing `valeriepieris-0.1.3.tar` & `valeriepieris-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ra414     (1000) ra414     (1000)        0 2023-08-02 06:39:07.902602 valeriepieris-0.1.3/
--rw-rw-r--   0 ra414     (1000) ra414     (1000)    35149 2023-07-30 06:24:37.000000 valeriepieris-0.1.3/LICENSE.txt
--rw-rw-r--   0 ra414     (1000) ra414     (1000)       45 2023-07-30 07:20:50.000000 valeriepieris-0.1.3/MANIFEST.in
--rw-rw-r--   0 ra414     (1000) ra414     (1000)     5236 2023-08-02 06:39:07.902602 valeriepieris-0.1.3/PKG-INFO
--rw-rw-r--   0 ra414     (1000) ra414     (1000)     3189 2023-08-02 06:38:19.000000 valeriepieris-0.1.3/README.md
--rw-rw-r--   0 ra414     (1000) ra414     (1000)      609 2023-08-02 06:38:28.000000 valeriepieris-0.1.3/pyproject.toml
--rw-rw-r--   0 ra414     (1000) ra414     (1000)       14 2023-07-30 07:20:20.000000 valeriepieris-0.1.3/requirements.txt
--rw-rw-r--   0 ra414     (1000) ra414     (1000)     1509 2023-08-02 06:39:07.902602 valeriepieris-0.1.3/setup.cfg
--rw-rw-r--   0 ra414     (1000) ra414     (1000)      414 2023-07-30 07:45:27.000000 valeriepieris-0.1.3/setup.py
-drwxrwxr-x   0 ra414     (1000) ra414     (1000)        0 2023-08-02 06:39:07.902602 valeriepieris-0.1.3/src/
--rw-rw-r--   0 ra414     (1000) ra414     (1000)  1696289 2023-07-30 07:45:29.000000 valeriepieris-0.1.3/src/valeriepieris.c
-drwxrwxr-x   0 ra414     (1000) ra414     (1000)        0 2023-08-02 06:39:07.902602 valeriepieris-0.1.3/src/valeriepieris.egg-info/
--rw-rw-r--   0 ra414     (1000) ra414     (1000)     5236 2023-08-02 06:39:07.000000 valeriepieris-0.1.3/src/valeriepieris.egg-info/PKG-INFO
--rw-rw-r--   0 ra414     (1000) ra414     (1000)      308 2023-08-02 06:39:07.000000 valeriepieris-0.1.3/src/valeriepieris.egg-info/SOURCES.txt
--rw-rw-r--   0 ra414     (1000) ra414     (1000)        1 2023-08-02 06:39:07.000000 valeriepieris-0.1.3/src/valeriepieris.egg-info/dependency_links.txt
--rw-rw-r--   0 ra414     (1000) ra414     (1000)        1 2023-07-30 07:45:30.000000 valeriepieris-0.1.3/src/valeriepieris.egg-info/not-zip-safe
--rw-rw-r--   0 ra414     (1000) ra414     (1000)       14 2023-08-02 06:39:07.000000 valeriepieris-0.1.3/src/valeriepieris.egg-info/top_level.txt
+drwxrwxr-x   0 ra414     (1000) ra414     (1000)        0 2023-08-02 06:41:38.286830 valeriepieris-0.1.4/
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)    35149 2023-07-30 06:24:37.000000 valeriepieris-0.1.4/LICENSE.txt
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)       45 2023-07-30 07:20:50.000000 valeriepieris-0.1.4/MANIFEST.in
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)     5300 2023-08-02 06:41:38.286830 valeriepieris-0.1.4/PKG-INFO
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)     3253 2023-08-02 06:41:13.000000 valeriepieris-0.1.4/README.md
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)      609 2023-08-02 06:41:24.000000 valeriepieris-0.1.4/pyproject.toml
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)       14 2023-07-30 07:20:20.000000 valeriepieris-0.1.4/requirements.txt
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)     1509 2023-08-02 06:41:38.290830 valeriepieris-0.1.4/setup.cfg
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)      414 2023-07-30 07:45:27.000000 valeriepieris-0.1.4/setup.py
+drwxrwxr-x   0 ra414     (1000) ra414     (1000)        0 2023-08-02 06:41:38.286830 valeriepieris-0.1.4/src/
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)  1696289 2023-07-30 07:45:29.000000 valeriepieris-0.1.4/src/valeriepieris.c
+drwxrwxr-x   0 ra414     (1000) ra414     (1000)        0 2023-08-02 06:41:38.286830 valeriepieris-0.1.4/src/valeriepieris.egg-info/
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)     5300 2023-08-02 06:41:38.000000 valeriepieris-0.1.4/src/valeriepieris.egg-info/PKG-INFO
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)      308 2023-08-02 06:41:38.000000 valeriepieris-0.1.4/src/valeriepieris.egg-info/SOURCES.txt
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)        1 2023-08-02 06:41:38.000000 valeriepieris-0.1.4/src/valeriepieris.egg-info/dependency_links.txt
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)        1 2023-07-30 07:45:30.000000 valeriepieris-0.1.4/src/valeriepieris.egg-info/not-zip-safe
+-rw-rw-r--   0 ra414     (1000) ra414     (1000)       14 2023-08-02 06:41:38.000000 valeriepieris-0.1.4/src/valeriepieris.egg-info/top_level.txt
```

### Comparing `valeriepieris-0.1.3/LICENSE.txt` & `valeriepieris-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `valeriepieris-0.1.3/PKG-INFO` & `valeriepieris-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valeriepieris
-Version: 0.1.3
+Version: 0.1.4
 Summary: Finding valeriepieris circles
 Home-page: https://github.com/rudyarthur/valeriepieris
 Author: Rudy Arthur
 Author-email: rudy.d.arthur@gmail.com
 License: GNU GENERAL PUBLIC LICENSE Version 3
 Project-URL: Documentation, https://github.com/rudyarthur/valeriepieris
 Project-URL: Code, https://github.com/rudyarthur/valeriepieris
@@ -70,15 +70,15 @@
         	print("At f={}, radius={}, population={}, centre={}".format( f, rmin[i], smin[i], best_latlon[i] ) )
         ```
         ```
         At f=0.5, radius=10344.885492078058, population=3987443544.209256, centre=[(50.5, -66.5)]
         ```
         
         ## Plotting the circles
-        Remember the earth is round, so don't just draw a circle on a flat map! See `tests.py` for example to make the plot at the top
+        Remember the earth is round, so don't just draw a circle on a flat map! See [test.py](https://github.com/rudyarthur/valeriepieris/raw/main/tests/test.py) for code to make the plot at the top
```

### Comparing `valeriepieris-0.1.3/README.md` & `valeriepieris-0.1.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -59,14 +59,14 @@
 	print("At f={}, radius={}, population={}, centre={}".format( f, rmin[i], smin[i], best_latlon[i] ) )
 ```
 ```
 At f=0.5, radius=10344.885492078058, population=3987443544.209256, centre=[(50.5, -66.5)]
 ```
 
 ## Plotting the circles
-Remember the earth is round, so don't just draw a circle on a flat map! See `tests.py` for example to make the plot at the top
+Remember the earth is round, so don't just draw a circle on a flat map! See [test.py](https://github.com/rudyarthur/valeriepieris/raw/main/tests/test.py) for code to make the plot at the top
```

### Comparing `valeriepieris-0.1.3/pyproject.toml` & `valeriepieris-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "valeriepieris"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Rudy Arthur", email="rudy.d.arthur@gmail.com" },
 ]
 description = "calculate valeriepieris circles"
 readme = "README.md"
 requires-python = ">=3.8"
 requires = ["setuptools", "wheel", "numpy >= 1.24", "Cython>=0.29.33"]
```

### Comparing `valeriepieris-0.1.3/setup.cfg` & `valeriepieris-0.1.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = valeriepieris
-version = 0.1.3
+version = 0.1.4
 description = Finding valeriepieris circles
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = GNU GENERAL PUBLIC LICENSE Version 3
 author = Rudy Arthur
 author_email = rudy.d.arthur@gmail.com
 url = https://github.com/rudyarthur/valeriepieris
```

### Comparing `valeriepieris-0.1.3/src/valeriepieris.c` & `valeriepieris-0.1.4/src/valeriepieris.c`

 * *Files identical despite different names*

### Comparing `valeriepieris-0.1.3/src/valeriepieris.egg-info/PKG-INFO` & `valeriepieris-0.1.4/src/valeriepieris.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valeriepieris
-Version: 0.1.3
+Version: 0.1.4
 Summary: Finding valeriepieris circles
 Home-page: https://github.com/rudyarthur/valeriepieris
 Author: Rudy Arthur
 Author-email: rudy.d.arthur@gmail.com
 License: GNU GENERAL PUBLIC LICENSE Version 3
 Project-URL: Documentation, https://github.com/rudyarthur/valeriepieris
 Project-URL: Code, https://github.com/rudyarthur/valeriepieris
@@ -70,15 +70,15 @@
         	print("At f={}, radius={}, population={}, centre={}".format( f, rmin[i], smin[i], best_latlon[i] ) )
         ```
         ```
         At f=0.5, radius=10344.885492078058, population=3987443544.209256, centre=[(50.5, -66.5)]
         ```
         
         ## Plotting the circles
-        Remember the earth is round, so don't just draw a circle on a flat map! See `tests.py` for example to make the plot at the top
+        Remember the earth is round, so don't just draw a circle on a flat map! See [test.py](https://github.com/rudyarthur/valeriepieris/raw/main/tests/test.py) for code to make the plot at the top
```


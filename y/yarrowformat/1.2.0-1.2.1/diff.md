# Comparing `tmp/yarrowformat-1.2.0.tar.gz` & `tmp/yarrowformat-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yarrowformat-1.2.0.tar", last modified: Thu Apr 20 09:47:27 2023, max compression
+gzip compressed data, was "dist/yarrowformat-1.2.1.tar", last modified: Wed Aug  2 16:21:33 2023, max compression
```

## Comparing `yarrowformat-1.2.0.tar` & `yarrowformat-1.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:47:27.000000 yarrowformat-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)     2392 2023-04-20 09:47:27.000000 yarrowformat-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2037 2023-04-20 09:47:10.000000 yarrowformat-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)    81180 2023-04-20 09:47:10.000000 yarrowformat-1.2.0/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:47:27.000000 yarrowformat-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:47:27.000000 yarrowformat-1.2.0/src/yarrow/
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-04-20 09:47:10.000000 yarrowformat-1.2.0/src/yarrow/_yarrow_version.py
--rw-r--r--   0 runner    (1001) docker     (122)    29424 2023-04-20 09:47:10.000000 yarrowformat-1.2.0/src/yarrow/yarrow_cls.py
--rw-r--r--   0 runner    (1001) docker     (122)      207 2023-04-20 09:47:10.000000 yarrowformat-1.2.0/src/yarrow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:47:27.000000 yarrowformat-1.2.0/src/yarrow/cli/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-04-20 09:47:10.000000 yarrowformat-1.2.0/src/yarrow/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-04-20 09:47:10.000000 yarrowformat-1.2.0/src/yarrow/cli/save.py
--rw-r--r--   0 runner    (1001) docker     (122)      850 2023-04-20 09:47:10.000000 yarrowformat-1.2.0/src/yarrow/cli/open.py
--rw-r--r--   0 runner    (1001) docker     (122)     1243 2023-04-20 09:47:10.000000 yarrowformat-1.2.0/src/yarrow/cli/check.py
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-04-20 09:47:27.000000 yarrowformat-1.2.0/src/yarrow/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)    13733 2023-04-20 09:47:10.000000 yarrowformat-1.2.0/src/yarrow/yarrow.py
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-04-20 09:47:10.000000 yarrowformat-1.2.0/src/yarrow/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     6466 2023-04-20 09:47:10.000000 yarrowformat-1.2.0/src/yarrow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:47:27.000000 yarrowformat-1.2.0/src/yarrowformat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2392 2023-04-20 09:47:27.000000 yarrowformat-1.2.0/src/yarrowformat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-04-20 09:47:27.000000 yarrowformat-1.2.0/src/yarrowformat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      118 2023-04-20 09:47:27.000000 yarrowformat-1.2.0/src/yarrowformat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)      601 2023-04-20 09:47:27.000000 yarrowformat-1.2.0/src/yarrowformat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 09:47:27.000000 yarrowformat-1.2.0/src/yarrowformat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-20 09:47:27.000000 yarrowformat-1.2.0/src/yarrowformat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 09:47:27.000000 yarrowformat-1.2.0/src/yarrowformat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      884 2023-04-20 09:47:27.000000 yarrowformat-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)    11380 2023-04-20 09:47:10.000000 yarrowformat-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-20 09:47:10.000000 yarrowformat-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-04-20 09:47:10.000000 yarrowformat-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:21:33.000000 yarrowformat-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      889 2023-08-02 16:21:33.000000 yarrowformat-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2037 2023-08-02 16:21:29.000000 yarrowformat-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-08-02 16:21:29.000000 yarrowformat-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-08-02 16:21:29.000000 yarrowformat-1.2.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11380 2023-08-02 16:21:29.000000 yarrowformat-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     2392 2023-08-02 16:21:33.000000 yarrowformat-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    81180 2023-08-02 16:21:29.000000 yarrowformat-1.2.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:21:33.000000 yarrowformat-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:21:33.000000 yarrowformat-1.2.1/src/yarrowformat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-08-02 16:21:33.000000 yarrowformat-1.2.1/src/yarrowformat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      601 2023-08-02 16:21:33.000000 yarrowformat-1.2.1/src/yarrowformat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 16:21:33.000000 yarrowformat-1.2.1/src/yarrowformat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)     2392 2023-08-02 16:21:33.000000 yarrowformat-1.2.1/src/yarrowformat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-08-02 16:21:33.000000 yarrowformat-1.2.1/src/yarrowformat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 16:21:33.000000 yarrowformat-1.2.1/src/yarrowformat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-08-02 16:21:33.000000 yarrowformat-1.2.1/src/yarrowformat.egg-info/requires.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:21:33.000000 yarrowformat-1.2.1/src/yarrow/
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-08-02 16:21:33.000000 yarrowformat-1.2.1/src/yarrow/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29560 2023-08-02 16:21:29.000000 yarrowformat-1.2.1/src/yarrow/yarrow_cls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-08-02 16:21:29.000000 yarrowformat-1.2.1/src/yarrow/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-08-02 16:21:29.000000 yarrowformat-1.2.1/src/yarrow/_yarrow_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:21:33.000000 yarrowformat-1.2.1/src/yarrow/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-08-02 16:21:29.000000 yarrowformat-1.2.1/src/yarrow/cli/save.py
+-rw-r--r--   0 runner    (1001) docker     (122)      850 2023-08-02 16:21:29.000000 yarrowformat-1.2.1/src/yarrow/cli/open.py
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-08-02 16:21:29.000000 yarrowformat-1.2.1/src/yarrow/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1243 2023-08-02 16:21:29.000000 yarrowformat-1.2.1/src/yarrow/cli/check.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13733 2023-08-02 16:21:29.000000 yarrowformat-1.2.1/src/yarrow/yarrow.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6466 2023-08-02 16:21:29.000000 yarrowformat-1.2.1/src/yarrow/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-08-02 16:21:29.000000 yarrowformat-1.2.1/src/yarrow/__init__.py
```

### Comparing `yarrowformat-1.2.0/PKG-INFO` & `yarrowformat-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yarrowformat
-Version: 1.2.0
+Version: 1.2.1
 Summary: Yarrow Format parsing lib
 Home-page: https://github.com/michelin/YarrowFormat
 Author: Mathieu Pichon
 Author-email: mathieu.pichon_ext@michelin.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `yarrowformat-1.2.0/README.md` & `yarrowformat-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `yarrowformat-1.2.0/versioneer.py` & `yarrowformat-1.2.1/versioneer.py`

 * *Files identical despite different names*

### Comparing `yarrowformat-1.2.0/src/yarrow/yarrow_cls.py` & `yarrowformat-1.2.1/src/yarrow/yarrow_cls.py`

 * *Files 0% similar despite different names*

```diff
@@ -486,27 +486,29 @@
         else:
             return elem_in
         return annot
 
     def add_images(self, images: List[Image]) -> List[Image]:
         """Add an image list and its confidential objects if they exists
         and returns the actual images found in the yarrow in case they
-        are already present
+        are already present. SHould preserve image order in the list but
+        does not guarantee only unique images are present in the returned
+        image list
 
         Args:
             images (List[Image])
 
         Return:
             (List[Images])
         """
-        result = set()
+        result = list()
         for img in images:
-            result.add(self.add_image(img))
+            result.append(self.add_image(img))
 
-        return list(result)
+        return result
 
     def add_image(self, image: Image) -> Image:
         """Add an image and its confidential object if it exists
         Returns the
 
         Args:
             image (Image)
```

### Comparing `yarrowformat-1.2.0/src/yarrow/cli/save.py` & `yarrowformat-1.2.1/src/yarrow/cli/save.py`

 * *Files identical despite different names*

### Comparing `yarrowformat-1.2.0/src/yarrow/cli/open.py` & `yarrowformat-1.2.1/src/yarrow/cli/open.py`

 * *Files identical despite different names*

### Comparing `yarrowformat-1.2.0/src/yarrow/cli/check.py` & `yarrowformat-1.2.1/src/yarrow/cli/check.py`

 * *Files identical despite different names*

### Comparing `yarrowformat-1.2.0/src/yarrow/yarrow.py` & `yarrowformat-1.2.1/src/yarrow/yarrow.py`

 * *Files identical despite different names*

### Comparing `yarrowformat-1.2.0/src/yarrow/utils.py` & `yarrowformat-1.2.1/src/yarrow/utils.py`

 * *Files identical despite different names*

### Comparing `yarrowformat-1.2.0/src/yarrowformat.egg-info/PKG-INFO` & `yarrowformat-1.2.1/src/yarrowformat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yarrowformat
-Version: 1.2.0
+Version: 1.2.1
 Summary: Yarrow Format parsing lib
 Home-page: https://github.com/michelin/YarrowFormat
 Author: Mathieu Pichon
 Author-email: mathieu.pichon_ext@michelin.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `yarrowformat-1.2.0/src/yarrowformat.egg-info/SOURCES.txt` & `yarrowformat-1.2.1/src/yarrowformat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yarrowformat-1.2.0/setup.cfg` & `yarrowformat-1.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 package_dir = 
 	= src
 packages = find:
 python_requires = >= 3.6
 install_requires = 
 	setuptools
 	wheel
-	pydantic >= 1.8
+	pydantic >= 1.8,<2.0
 	numpy >= 1.19
 	click
 zip_safe = False
 include_package_data = True
 
 [options.extras_require]
 dev =
```

### Comparing `yarrowformat-1.2.0/LICENSE` & `yarrowformat-1.2.1/LICENSE`

 * *Files identical despite different names*


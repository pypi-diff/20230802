# Comparing `tmp/symbolicmode-1.0.tar.gz` & `tmp/symbolicmode-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbolicmode-1.0.tar", last modified: Wed Apr 12 15:00:54 2023, max compression
+gzip compressed data, was "symbolicmode-1.0.1.tar", last modified: Wed Aug  2 12:03:21 2023, max compression
```

## Comparing `symbolicmode-1.0.tar` & `symbolicmode-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:00:54.685901 symbolicmode-1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-12 15:00:44.000000 symbolicmode-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-04-12 15:00:54.685901 symbolicmode-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-04-12 15:00:44.000000 symbolicmode-1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-12 15:00:47.000000 symbolicmode-1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 15:00:54.685901 symbolicmode-1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:00:54.681902 symbolicmode-1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:00:54.681902 symbolicmode-1.0/src/symbolicmode/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9621 2023-04-12 15:00:44.000000 symbolicmode-1.0/src/symbolicmode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:00:54.685901 symbolicmode-1.0/src/symbolicmode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-04-12 15:00:54.000000 symbolicmode-1.0/src/symbolicmode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-12 15:00:54.000000 symbolicmode-1.0/src/symbolicmode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 15:00:54.000000 symbolicmode-1.0/src/symbolicmode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 15:00:54.000000 symbolicmode-1.0/src/symbolicmode.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:00:54.685901 symbolicmode-1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-12 15:00:44.000000 symbolicmode-1.0/tests/test_chmod.py
--rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-04-12 15:00:44.000000 symbolicmode-1.0/tests/test_modes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:03:21.118315 symbolicmode-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-08-02 12:03:08.000000 symbolicmode-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-08-02 12:03:21.118315 symbolicmode-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-08-02 12:03:08.000000 symbolicmode-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-08-02 12:03:11.000000 symbolicmode-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 12:03:21.118315 symbolicmode-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:03:21.118315 symbolicmode-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:03:21.118315 symbolicmode-1.0.1/src/symbolicmode/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9621 2023-08-02 12:03:08.000000 symbolicmode-1.0.1/src/symbolicmode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:03:21.118315 symbolicmode-1.0.1/src/symbolicmode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-08-02 12:03:21.000000 symbolicmode-1.0.1/src/symbolicmode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-02 12:03:21.000000 symbolicmode-1.0.1/src/symbolicmode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 12:03:21.000000 symbolicmode-1.0.1/src/symbolicmode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-02 12:03:21.000000 symbolicmode-1.0.1/src/symbolicmode.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:03:21.118315 symbolicmode-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-08-02 12:03:08.000000 symbolicmode-1.0.1/tests/test_chmod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-08-02 12:03:08.000000 symbolicmode-1.0.1/tests/test_modes.py
```

### Comparing `symbolicmode-1.0/LICENSE` & `symbolicmode-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `symbolicmode-1.0/PKG-INFO` & `symbolicmode-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: symbolicmode
-Version: 1.0
+Version: 1.0.1
 Summary: Code to handle symbolic permissions like GNU chmod does ('a=rx,u+w')
 Author-email: Sean Reifschneider <jafo00@gmail.com>
 Project-URL: Homepage, https://github.com/linsomniac/symbolicmode
 Project-URL: Bug Tracker, https://github.com/linsomniac/symbolicmode/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SymbolicMode -- Code to handle symbolic file permissions
 
 This python library parses symbolic file permission modes as used by GNU chmod, part
 of the coreutils package.  For example:
```

### Comparing `symbolicmode-1.0/README.md` & `symbolicmode-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `symbolicmode-1.0/pyproject.toml` & `symbolicmode-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
 pythonpath = "src"
 
 [project]
 name = "symbolicmode"
-version = "1.0"
+version = "1.0.1"
 authors = [
   { name="Sean Reifschneider", email="jafo00@gmail.com" },
 ]
 description = "Code to handle symbolic permissions like GNU chmod does ('a=rx,u+w')"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `symbolicmode-1.0/src/symbolicmode/__init__.py` & `symbolicmode-1.0.1/src/symbolicmode/__init__.py`

 * *Files identical despite different names*

### Comparing `symbolicmode-1.0/src/symbolicmode.egg-info/PKG-INFO` & `symbolicmode-1.0.1/src/symbolicmode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: symbolicmode
-Version: 1.0
+Version: 1.0.1
 Summary: Code to handle symbolic permissions like GNU chmod does ('a=rx,u+w')
 Author-email: Sean Reifschneider <jafo00@gmail.com>
 Project-URL: Homepage, https://github.com/linsomniac/symbolicmode
 Project-URL: Bug Tracker, https://github.com/linsomniac/symbolicmode/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SymbolicMode -- Code to handle symbolic file permissions
 
 This python library parses symbolic file permission modes as used by GNU chmod, part
 of the coreutils package.  For example:
```

### Comparing `symbolicmode-1.0/tests/test_chmod.py` & `symbolicmode-1.0.1/tests/test_chmod.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,11 +44,14 @@
 
         chmod("u=rx,go=", topdir, recurse=True)
         self.assertEqual(stat.S_IMODE(os.stat(topdir).st_mode), 0o500)
         self.assertEqual(stat.S_IMODE(os.stat(topfile).st_mode), 0o500)
         self.assertEqual(stat.S_IMODE(os.stat(lowerdir).st_mode), 0o500)
         self.assertEqual(stat.S_IMODE(os.stat(lowerfile).st_mode), 0o500)
 
+        #  clean up, allow removal
+        chmod("u=rwx,go=", topdir, recurse=True)
+
 
 # Run the unit tests
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `symbolicmode-1.0/tests/test_modes.py` & `symbolicmode-1.0.1/tests/test_modes.py`

 * *Files identical despite different names*


# Comparing `tmp/envkeeper-0.0.2.tar.gz` & `tmp/envkeeper-0.0.3.tar.gz`

## Comparing `envkeeper-0.0.2.tar` & `envkeeper-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 envkeeper-0.0.2/envkeeper/__init__.py
--rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 envkeeper-0.0.2/envkeeper/container.py
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 envkeeper-0.0.2/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 envkeeper-0.0.2/LICENSE
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 envkeeper-0.0.2/README.md
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 envkeeper-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 envkeeper-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 envkeeper-0.0.3/envkeeper/__init__.py
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 envkeeper-0.0.3/envkeeper/container.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 envkeeper-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 envkeeper-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 envkeeper-0.0.3/README.md
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 envkeeper-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 envkeeper-0.0.3/PKG-INFO
```

### Comparing `envkeeper-0.0.2/envkeeper/container.py` & `envkeeper-0.0.3/envkeeper/container.py`

 * *Files identical despite different names*

### Comparing `envkeeper-0.0.2/.gitignore` & `envkeeper-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `envkeeper-0.0.2/LICENSE` & `envkeeper-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `envkeeper-0.0.2/README.md` & `envkeeper-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `envkeeper-0.0.2/pyproject.toml` & `envkeeper-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = [
   "hatchling >= 1.11.0",
   "pip >= 22.0.0"
 ]
 
 [project]
 name            = "envkeeper"
-version         = "0.0.2"
+version         = "0.0.3"
 description     = "Use environmental variables to store global data. Like localStorage, but for python!"
 readme          = "README.md"
 license         = "MIT"
 requires-python = ">=3.9"
 
 authors = [
   { name = "Christopher Woodall", email = "woodall.christopher@gmail.com" },
```

### Comparing `envkeeper-0.0.2/PKG-INFO` & `envkeeper-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: envkeeper
-Version: 0.0.2
+Version: 0.0.3
 Summary: Use environmental variables to store global data. Like localStorage, but for python!
 Project-URL: GitHub, https://github.com/christopherwoodall/blobstorage
 Author-email: Christopher Woodall <woodall.christopher@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
```


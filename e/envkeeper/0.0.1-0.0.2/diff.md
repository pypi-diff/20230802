# Comparing `tmp/envkeeper-0.0.1.tar.gz` & `tmp/envkeeper-0.0.2.tar.gz`

## Comparing `envkeeper-0.0.1.tar` & `envkeeper-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 envkeeper-0.0.1/envkeeper/__init__.py
--rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 envkeeper-0.0.1/envkeeper/container.py
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 envkeeper-0.0.1/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 envkeeper-0.0.1/LICENSE
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 envkeeper-0.0.1/README.md
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 envkeeper-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 envkeeper-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 envkeeper-0.0.2/envkeeper/__init__.py
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 envkeeper-0.0.2/envkeeper/container.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 envkeeper-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 envkeeper-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 envkeeper-0.0.2/README.md
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 envkeeper-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 envkeeper-0.0.2/PKG-INFO
```

### Comparing `envkeeper-0.0.1/envkeeper/container.py` & `envkeeper-0.0.2/envkeeper/container.py`

 * *Files identical despite different names*

### Comparing `envkeeper-0.0.1/.gitignore` & `envkeeper-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `envkeeper-0.0.1/LICENSE` & `envkeeper-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `envkeeper-0.0.1/README.md` & `envkeeper-0.0.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-# blobStorage [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/christopherwoodall/blobstorage/blob/master/examples/blobstorage_example.ipynb)
+# EnvKeeper [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/christopherwoodall/blobstorage/blob/master/examples/blobstorage_example.ipynb)
 ### Like `localStorage`, but for `python`!
 
 Simple Python library for managing and storing variables as JSON-encoded dictionaries in environment variables. It provides a dictionary-like interface for storing and retrieving data in environment variables, and allows for global access once stored.
 
 
 ## Installation
 
-Install BlobStorage via pip:
+Install EnvKeeper via pip:
 ```bash
-pip install blobstorage
+pip install envkeeper
 ```
 
 
 ## Usage
 
 See the `Makefile` for a list of examples and available commands.
 
 Here's a basic example of using BlobStorage:
 
 ```python
-from blobstorage import StorageContainer
+from envkeeper import StorageContainer
 
 # Create an instance with an environment variable key
 # Be sure to replace `'MY_VAR'` with the actual name of the environment variable you want to use.
 store = StorageContainer('MY_VAR')
 
 # Set items
 store['foo'] = 'bar'
```

### Comparing `envkeeper-0.0.1/pyproject.toml` & `envkeeper-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = [
   "hatchling >= 1.11.0",
   "pip >= 22.0.0"
 ]
 
 [project]
 name            = "envkeeper"
-version         = "0.0.1"
+version         = "0.0.2"
 description     = "Use environmental variables to store global data. Like localStorage, but for python!"
 readme          = "README.md"
 license         = "MIT"
 requires-python = ">=3.9"
 
 authors = [
   { name = "Christopher Woodall", email = "woodall.christopher@gmail.com" },
```

### Comparing `envkeeper-0.0.1/PKG-INFO` & `envkeeper-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: envkeeper
-Version: 0.0.1
+Version: 0.0.2
 Summary: Use environmental variables to store global data. Like localStorage, but for python!
 Project-URL: GitHub, https://github.com/christopherwoodall/blobstorage
 Author-email: Christopher Woodall <woodall.christopher@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
@@ -23,36 +23,36 @@
 Provides-Extra: developer
 Requires-Dist: hatch; extra == 'developer'
 Requires-Dist: mypy; extra == 'developer'
 Requires-Dist: pydantic; extra == 'developer'
 Requires-Dist: types-pyyaml; extra == 'developer'
 Description-Content-Type: text/markdown
 
-# blobStorage [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/christopherwoodall/blobstorage/blob/master/examples/blobstorage_example.ipynb)
+# EnvKeeper [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/christopherwoodall/blobstorage/blob/master/examples/blobstorage_example.ipynb)
 ### Like `localStorage`, but for `python`!
 
 Simple Python library for managing and storing variables as JSON-encoded dictionaries in environment variables. It provides a dictionary-like interface for storing and retrieving data in environment variables, and allows for global access once stored.
 
 
 ## Installation
 
-Install BlobStorage via pip:
+Install EnvKeeper via pip:
 ```bash
-pip install blobstorage
+pip install envkeeper
 ```
 
 
 ## Usage
 
 See the `Makefile` for a list of examples and available commands.
 
 Here's a basic example of using BlobStorage:
 
 ```python
-from blobstorage import StorageContainer
+from envkeeper import StorageContainer
 
 # Create an instance with an environment variable key
 # Be sure to replace `'MY_VAR'` with the actual name of the environment variable you want to use.
 store = StorageContainer('MY_VAR')
 
 # Set items
 store['foo'] = 'bar'
```


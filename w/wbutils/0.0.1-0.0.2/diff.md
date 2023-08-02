# Comparing `tmp/wbutils-0.0.1.tar.gz` & `tmp/wbutils-0.0.2.tar.gz`

## Comparing `wbutils-0.0.1.tar` & `wbutils-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 wbutils-0.0.1/src/wbutils/__init__.py
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 wbutils-0.0.1/src/wbutils/artifact.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 wbutils-0.0.1/src/wbutils/directory.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 wbutils-0.0.1/src/wbutils/framework.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 wbutils-0.0.1/src/wbutils/include.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 wbutils-0.0.1/src/wbutils/io.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 wbutils-0.0.1/src/wbutils/keys.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 wbutils-0.0.1/src/wbutils/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wbutils-0.0.1/src/wbutils/parsing/__init__.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 wbutils-0.0.1/src/wbutils/parsing/pytorch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wbutils-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 wbutils-0.0.1/tests/test_directory.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 wbutils-0.0.1/tests/test_framework.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 wbutils-0.0.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 wbutils-0.0.1/LICENSE
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 wbutils-0.0.1/README.md
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 wbutils-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 wbutils-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 wbutils-0.0.2/src/wbutils/__init__.py
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 wbutils-0.0.2/src/wbutils/artifact.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 wbutils-0.0.2/src/wbutils/directory.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 wbutils-0.0.2/src/wbutils/framework.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 wbutils-0.0.2/src/wbutils/include.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 wbutils-0.0.2/src/wbutils/io.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 wbutils-0.0.2/src/wbutils/keys.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 wbutils-0.0.2/src/wbutils/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wbutils-0.0.2/src/wbutils/parsing/__init__.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 wbutils-0.0.2/src/wbutils/parsing/pytorch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wbutils-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 wbutils-0.0.2/tests/test_directory.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 wbutils-0.0.2/tests/test_framework.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 wbutils-0.0.2/tests/test_io.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 wbutils-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 wbutils-0.0.2/LICENSE
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 wbutils-0.0.2/README.md
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 wbutils-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 wbutils-0.0.2/PKG-INFO
```

### Comparing `wbutils-0.0.1/src/wbutils/__init__.py` & `wbutils-0.0.2/src/wbutils/__init__.py`

 * *Files identical despite different names*

### Comparing `wbutils-0.0.1/src/wbutils/artifact.py` & `wbutils-0.0.2/src/wbutils/artifact.py`

 * *Files identical despite different names*

### Comparing `wbutils-0.0.1/src/wbutils/directory.py` & `wbutils-0.0.2/src/wbutils/directory.py`

 * *Files identical despite different names*

### Comparing `wbutils-0.0.1/src/wbutils/include.py` & `wbutils-0.0.2/src/wbutils/include.py`

 * *Files identical despite different names*

### Comparing `wbutils-0.0.1/src/wbutils/io.py` & `wbutils-0.0.2/src/wbutils/io.py`

 * *Files identical despite different names*

### Comparing `wbutils-0.0.1/src/wbutils/keys.py` & `wbutils-0.0.2/src/wbutils/keys.py`

 * *Files identical despite different names*

### Comparing `wbutils-0.0.1/src/wbutils/parsing/pytorch.py` & `wbutils-0.0.2/src/wbutils/parsing/pytorch.py`

 * *Files identical despite different names*

### Comparing `wbutils-0.0.1/tests/test_directory.py` & `wbutils-0.0.2/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `wbutils-0.0.1/LICENSE` & `wbutils-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wbutils-0.0.1/pyproject.toml` & `wbutils-0.0.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -18,40 +18,43 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "torch",
     "wandb",
-    "ujson",
-    "click>=8.0.3"
+    "ujson"
 ]
 
 [project.urls]
 Homepage = "https://github.com/ankur-gupta/wbutils"
 Repository = "https://github.com/ankur-gupta/wbutils.git"
 
 [tool.hatch.version]
 path = "src/wbutils/version.py"
 
 [tool.hatch.envs.test]
 dependencies = [
-    "wandb",
-    "coverage[toml]",
+    "coverage",
+    "codecov",
     "pytest",
     "pytest-cov",
     "pytest-mock",
 ]
 
-# Run using `hatch run test:coverage`, `hatch run test:no-coverage`, `hatch run test:notslow`, ...
+# Run using `hatch run test:run-coverage`, `hatch run test:no-coverage`, `hatch run test:not-slow`, ...
 [tool.hatch.envs.test.scripts]
-coverage = "pytest --cov-config=pyproject.toml --cov=wbutils --cov=tests"
-no-coverage = "coverage --no-cov"
-notslow = "coverage -m \"not slow\""
-notrandom = "coverage -m \"not random\""
+with-coverage = "pytest --cov-config=pyproject.toml --cov=wbutils --cov=tests"
+no-coverage = "with-coverage --no-cov"
+not-slow = "with-coverage -m \"not slow\""
+not-random = "with-coverage -m \"not random\""
+coverage-json = "coverage json"
+coverage-xml = "coverage xml"
+coverage-html = "coverage html"
+
 
 [[tool.hatch.envs.test.matrix]]
 python = ["3.8", "3.9", "3.11"]
 
 [tool.coverage.run]
 omit = [
     "src/wbutils/resources/",
```

### Comparing `wbutils-0.0.1/PKG-INFO` & `wbutils-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbutils
-Version: 0.0.1
+Version: 0.0.2
 Summary: Helpful utilities to use Weights & Biases
 Project-URL: Homepage, https://github.com/ankur-gupta/wbutils
 Project-URL: Repository, https://github.com/ankur-gupta/wbutils.git
 Author-email: Ankur Gupta <7110058+ankur-gupta@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2023 Ankur Gupta
@@ -28,15 +28,14 @@
         SOFTWARE.
 License-File: LICENSE
 Keywords: experiment-tracking,ml,wandb
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
-Requires-Dist: click>=8.0.3
 Requires-Dist: torch
 Requires-Dist: ujson
 Requires-Dist: wandb
 Description-Content-Type: text/markdown
 
 # wbutils
```


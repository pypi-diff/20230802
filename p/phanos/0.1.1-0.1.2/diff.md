# Comparing `tmp/phanos-0.1.1.tar.gz` & `tmp/phanos-0.1.2.tar.gz`

## Comparing `phanos-0.1.1.tar` & `phanos-0.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 phanos-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 phanos-0.1.1/Pipfile
--rw-r--r--   0        0        0    22933 2020-02-02 00:00:00.000000 phanos-0.1.1/Pipfile.lock
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 phanos-0.1.1/requirements.txt
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 phanos-0.1.1/deactivate/pyvenv.cfg
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 phanos-0.1.1/deactivate/bin/Activate.ps1
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 phanos-0.1.1/deactivate/bin/activate
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 phanos-0.1.1/deactivate/bin/activate.csh
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 phanos-0.1.1/deactivate/bin/activate.fish
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.1.1/deactivate/bin/pip
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.1.1/deactivate/bin/pip3
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.1.1/deactivate/bin/pip3.10
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.1.1/deactivate/bin/pip3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.1.1/deactivate/bin/python -> python3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.1.1/deactivate/bin/python3 -> python3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.1.1/deactivate/bin/python3.11 -> /usr/bin/python3.11
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 phanos-0.1.1/src/phanos/__init__.py
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 phanos-0.1.1/src/phanos/config.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 phanos-0.1.1/src/phanos/log.py
--rw-r--r--   0        0        0    17132 2020-02-02 00:00:00.000000 phanos-0.1.1/src/phanos/metrics.py
--rw-r--r--   0        0        0    20338 2020-02-02 00:00:00.000000 phanos-0.1.1/src/phanos/publisher.py
--rw-r--r--   0        0        0     5517 2020-02-02 00:00:00.000000 phanos-0.1.1/src/phanos/tree.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 phanos-0.1.1/test/__init__.py
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 phanos-0.1.1/test/dummy_api.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 phanos-0.1.1/test/requirements.txt
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 phanos-0.1.1/test/run_tests.py
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 phanos-0.1.1/test/test_config.py
--rw-r--r--   0        0        0    26021 2020-02-02 00:00:00.000000 phanos-0.1.1/test/test_metric.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 phanos-0.1.1/test/testing_data.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 phanos-0.1.1/.gitignore
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 phanos-0.1.1/LICENSE
--rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 phanos-0.1.1/README.md
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 phanos-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 phanos-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 phanos-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 phanos-0.1.2/Pipfile
+-rw-r--r--   0        0        0    22933 2020-02-02 00:00:00.000000 phanos-0.1.2/Pipfile.lock
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 phanos-0.1.2/requirements.txt
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 phanos-0.1.2/deactivate/pyvenv.cfg
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 phanos-0.1.2/deactivate/bin/Activate.ps1
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 phanos-0.1.2/deactivate/bin/activate
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 phanos-0.1.2/deactivate/bin/activate.csh
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 phanos-0.1.2/deactivate/bin/activate.fish
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.1.2/deactivate/bin/pip
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.1.2/deactivate/bin/pip3
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.1.2/deactivate/bin/pip3.10
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.1.2/deactivate/bin/pip3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.1.2/deactivate/bin/python -> python3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.1.2/deactivate/bin/python3 -> python3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.1.2/deactivate/bin/python3.11 -> /usr/bin/python3.11
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 phanos-0.1.2/src/phanos/__init__.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 phanos-0.1.2/src/phanos/config.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 phanos-0.1.2/src/phanos/log.py
+-rw-r--r--   0        0        0    17132 2020-02-02 00:00:00.000000 phanos-0.1.2/src/phanos/metrics.py
+-rw-r--r--   0        0        0    20338 2020-02-02 00:00:00.000000 phanos-0.1.2/src/phanos/publisher.py
+-rw-r--r--   0        0        0     5517 2020-02-02 00:00:00.000000 phanos-0.1.2/src/phanos/tree.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 phanos-0.1.2/test/__init__.py
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 phanos-0.1.2/test/dummy_api.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 phanos-0.1.2/test/requirements.txt
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 phanos-0.1.2/test/run_tests.py
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 phanos-0.1.2/test/test_config.py
+-rw-r--r--   0        0        0    26021 2020-02-02 00:00:00.000000 phanos-0.1.2/test/test_metric.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 phanos-0.1.2/test/testing_data.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 phanos-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 phanos-0.1.2/LICENSE
+-rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 phanos-0.1.2/README.md
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 phanos-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6827 2020-02-02 00:00:00.000000 phanos-0.1.2/PKG-INFO
```

### Comparing `phanos-0.1.1/Pipfile.lock` & `phanos-0.1.2/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `phanos-0.1.1/deactivate/bin/Activate.ps1` & `phanos-0.1.2/deactivate/bin/Activate.ps1`

 * *Files identical despite different names*

### Comparing `phanos-0.1.1/deactivate/bin/activate` & `phanos-0.1.2/deactivate/bin/activate`

 * *Files identical despite different names*

### Comparing `phanos-0.1.1/deactivate/bin/activate.csh` & `phanos-0.1.2/deactivate/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `phanos-0.1.1/deactivate/bin/activate.fish` & `phanos-0.1.2/deactivate/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `phanos-0.1.1/src/phanos/config.py` & `phanos-0.1.2/src/phanos/config.py`

 * *Files identical despite different names*

### Comparing `phanos-0.1.1/src/phanos/log.py` & `phanos-0.1.2/src/phanos/log.py`

 * *Files identical despite different names*

### Comparing `phanos-0.1.1/src/phanos/metrics.py` & `phanos-0.1.2/src/phanos/metrics.py`

 * *Files identical despite different names*

### Comparing `phanos-0.1.1/src/phanos/publisher.py` & `phanos-0.1.2/src/phanos/publisher.py`

 * *Files identical despite different names*

### Comparing `phanos-0.1.1/src/phanos/tree.py` & `phanos-0.1.2/src/phanos/tree.py`

 * *Files identical despite different names*

### Comparing `phanos-0.1.1/test/dummy_api.py` & `phanos-0.1.2/test/dummy_api.py`

 * *Files identical despite different names*

### Comparing `phanos-0.1.1/test/run_tests.py` & `phanos-0.1.2/test/run_tests.py`

 * *Files identical despite different names*

### Comparing `phanos-0.1.1/test/test_config.py` & `phanos-0.1.2/test/test_config.py`

 * *Files identical despite different names*

### Comparing `phanos-0.1.1/test/test_metric.py` & `phanos-0.1.2/test/test_metric.py`

 * *Files identical despite different names*

### Comparing `phanos-0.1.1/test/testing_data.py` & `phanos-0.1.2/test/testing_data.py`

 * *Files identical despite different names*

### Comparing `phanos-0.1.1/.gitignore` & `phanos-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `phanos-0.1.1/LICENSE` & `phanos-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `phanos-0.1.1/README.md` & `phanos-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `phanos-0.1.1/pyproject.toml` & `phanos-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "phanos"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Miroslav Bulička", email="bulickamiroslav@gmail.com" },
 ]
 description = "Python client to gather data for Prometheus logging in server with multiple instances and workers."
 readme = "README.md"
 requires-python = ">=3.10.6"
 classifiers = [
@@ -18,16 +18,14 @@
     "Programming Language :: Python :: 3",
     "Topic :: System :: Monitoring",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "pip>=23.1.2",
-    "Flask>=2.2.3",
     "pika>=1.3.2",
-    "flask-restx>=1.1.0",
     "imp_prof>=0.1.2",
     ]
 
 [project.urls]
 "Homepage" = "https://github.com/kajotgames/phanos"
 "Bug Tracker" = "https://github.com/kajotgames/phanos/issues"
```

### Comparing `phanos-0.1.1/PKG-INFO` & `phanos-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: phanos
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python client to gather data for Prometheus logging in server with multiple instances and workers.
 Project-URL: Homepage, https://github.com/kajotgames/phanos
 Project-URL: Bug Tracker, https://github.com/kajotgames/phanos/issues
 Author-email: Miroslav Bulička <bulickamiroslav@gmail.com>
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Monitoring
 Requires-Python: >=3.10.6
-Requires-Dist: flask-restx>=1.1.0
-Requires-Dist: flask>=2.2.3
 Requires-Dist: imp-prof>=0.1.2
 Requires-Dist: pika>=1.3.2
 Requires-Dist: pip>=23.1.2
 Description-Content-Type: text/markdown
 
 # PHANOS
```


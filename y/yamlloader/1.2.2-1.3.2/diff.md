# Comparing `tmp/yamlloader-1.2.2.tar.gz` & `tmp/yamlloader-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamlloader-1.2.2.tar", last modified: Fri Dec  2 16:53:50 2022, max compression
+gzip compressed data, was "yamlloader-1.3.2.tar", last modified: Wed Aug  2 12:46:34 2023, max compression
```

## Comparing `yamlloader-1.2.2.tar` & `yamlloader-1.3.2.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 16:53:50.661130 yamlloader-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (122)     2279 2022-12-02 16:53:43.000000 yamlloader-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       60 2022-12-02 16:53:43.000000 yamlloader-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5077 2022-12-02 16:53:50.661130 yamlloader-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3844 2022-12-02 16:53:43.000000 yamlloader-1.2.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      174 2022-12-02 16:53:43.000000 yamlloader-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)        7 2022-12-02 16:53:43.000000 yamlloader-1.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-02 16:53:50.661130 yamlloader-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1871 2022-12-02 16:53:43.000000 yamlloader-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 16:53:50.657130 yamlloader-1.2.2/yamlloader/
--rw-r--r--   0 runner    (1001) docker     (122)      527 2022-12-02 16:53:43.000000 yamlloader-1.2.2/yamlloader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 16:53:50.661130 yamlloader-1.2.2/yamlloader/ordereddict/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2022-12-02 16:53:43.000000 yamlloader-1.2.2/yamlloader/ordereddict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1596 2022-12-02 16:53:43.000000 yamlloader-1.2.2/yamlloader/ordereddict/dumpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1942 2022-12-02 16:53:43.000000 yamlloader-1.2.2/yamlloader/ordereddict/loaders.py
--rw-r--r--   0 runner    (1001) docker     (122)       83 2022-12-02 16:53:43.000000 yamlloader-1.2.2/yamlloader/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 16:53:50.661130 yamlloader-1.2.2/yamlloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)       88 2022-12-02 16:53:43.000000 yamlloader-1.2.2/yamlloader.egg-info/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     5077 2022-12-02 16:53:50.000000 yamlloader-1.2.2/yamlloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      453 2022-12-02 16:53:50.000000 yamlloader-1.2.2/yamlloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-02 16:53:50.000000 yamlloader-1.2.2/yamlloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-02 16:53:50.000000 yamlloader-1.2.2/yamlloader.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       32 2022-12-02 16:53:50.000000 yamlloader-1.2.2/yamlloader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2022-12-02 16:53:50.000000 yamlloader-1.2.2/yamlloader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:46:34.660501 yamlloader-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-08-02 12:46:25.000000 yamlloader-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-02 12:46:25.000000 yamlloader-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-08-02 12:46:34.660501 yamlloader-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-08-02 12:46:25.000000 yamlloader-1.3.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-02 12:46:25.000000 yamlloader-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-02 12:46:25.000000 yamlloader-1.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 12:46:34.660501 yamlloader-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-08-02 12:46:25.000000 yamlloader-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:46:34.656501 yamlloader-1.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    71023 2023-08-02 12:46:25.000000 yamlloader-1.3.2/tests/test_ext_anatools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-08-02 12:46:25.000000 yamlloader-1.3.2/tests/test_ordereddict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:46:34.656501 yamlloader-1.3.2/yamlloader/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-02 12:46:25.000000 yamlloader-1.3.2/yamlloader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:46:34.660501 yamlloader-1.3.2/yamlloader/ordereddict/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-02 12:46:25.000000 yamlloader-1.3.2/yamlloader/ordereddict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-02 12:46:25.000000 yamlloader-1.3.2/yamlloader/ordereddict/dumpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-08-02 12:46:25.000000 yamlloader-1.3.2/yamlloader/ordereddict/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-02 12:46:25.000000 yamlloader-1.3.2/yamlloader/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:46:34.660501 yamlloader-1.3.2/yamlloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-02 12:46:25.000000 yamlloader-1.3.2/yamlloader.egg-info/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-08-02 12:46:34.000000 yamlloader-1.3.2/yamlloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-02 12:46:34.000000 yamlloader-1.3.2/yamlloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 12:46:34.000000 yamlloader-1.3.2/yamlloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 12:46:34.000000 yamlloader-1.3.2/yamlloader.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 12:46:34.000000 yamlloader-1.3.2/yamlloader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-02 12:46:34.000000 yamlloader-1.3.2/yamlloader.egg-info/top_level.txt
```

### Comparing `yamlloader-1.2.2/LICENSE` & `yamlloader-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yamlloader-1.2.2/PKG-INFO` & `yamlloader-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamlloader
-Version: 1.2.2
+Version: 1.3.2
 Summary: Ordered YAML loader and dumper for PyYAML.
 Home-page: https://github.com/Phynix/yamlloader
 Download-URL: https://github.com/Phynix/yamlloader
 Author: Jonas Eschle "Mayou36", Johannes Lade "SebastianJL"
 Author-email: jonas.eschle@phynix.science, johannes.lade@phynix.science
 Maintainer: Jonas Eschle "Mayou36"
 Maintainer-email: jonas.eschle@phynix.science
@@ -13,22 +13,21 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Provides-Extra: dev
 License-File: LICENSE
 
 
 .. image:: https://github.com/Phynix/yamlloader/actions/workflows/ci.yml/badge.svg
     :target: https://github.com/Phynix/yamlloader/actions
 .. image:: https://img.shields.io/pypi/pyversions/yamlloader.svg
```

### Comparing `yamlloader-1.2.2/README.rst` & `yamlloader-1.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `yamlloader-1.2.2/setup.py` & `yamlloader-1.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     with open("README.rst", encoding="utf-8") as f:
         return f.read()
 
 
 dev_requiremnets = ["pytest", "hypothesis"]
 setup(
     name="yamlloader",
-    version="1.2.2",
+    version="1.3.2",
     author='Jonas Eschle "Mayou36", Johannes Lade "SebastianJL"',
     author_email="jonas.eschle@phynix.science, johannes.lade@phynix.science",
     maintainer='Jonas Eschle "Mayou36"',
     maintainer_email="jonas.eschle@phynix.science",
     url="https://github.com/Phynix/yamlloader",
     download_url="https://github.com/Phynix/yamlloader",
     license="MIT License",
@@ -32,22 +32,21 @@
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: System Administrators",
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Utilities",
     ],
     packages=["yamlloader", "yamlloader.ordereddict"],
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     install_requires=requirements,
     tests_require=dev_requiremnets,
     extras_require={"dev": dev_requiremnets},
     zip_safe=False,
 )
```

### Comparing `yamlloader-1.2.2/yamlloader/__init__.py` & `yamlloader-1.3.2/yamlloader/__init__.py`

 * *Files identical despite different names*

### Comparing `yamlloader-1.2.2/yamlloader/ordereddict/dumpers.py` & `yamlloader-1.3.2/yamlloader/ordereddict/dumpers.py`

 * *Files identical despite different names*

### Comparing `yamlloader-1.2.2/yamlloader/ordereddict/loaders.py` & `yamlloader-1.3.2/yamlloader/ordereddict/loaders.py`

 * *Files identical despite different names*

### Comparing `yamlloader-1.2.2/yamlloader.egg-info/PKG-INFO` & `yamlloader-1.3.2/yamlloader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamlloader
-Version: 1.2.2
+Version: 1.3.2
 Summary: Ordered YAML loader and dumper for PyYAML.
 Home-page: https://github.com/Phynix/yamlloader
 Download-URL: https://github.com/Phynix/yamlloader
 Author: Jonas Eschle "Mayou36", Johannes Lade "SebastianJL"
 Author-email: jonas.eschle@phynix.science, johannes.lade@phynix.science
 Maintainer: Jonas Eschle "Mayou36"
 Maintainer-email: jonas.eschle@phynix.science
@@ -13,22 +13,21 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Provides-Extra: dev
 License-File: LICENSE
 
 
 .. image:: https://github.com/Phynix/yamlloader/actions/workflows/ci.yml/badge.svg
     :target: https://github.com/Phynix/yamlloader/actions
 .. image:: https://img.shields.io/pypi/pyversions/yamlloader.svg
```


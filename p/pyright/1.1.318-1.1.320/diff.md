# Comparing `tmp/pyright-1.1.318.tar.gz` & `tmp/pyright-1.1.320.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyright-1.1.318.tar", last modified: Fri Jul 21 09:35:52 2023, max compression
+gzip compressed data, was "pyright-1.1.320.tar", last modified: Wed Aug  2 11:08:32 2023, max compression
```

## Comparing `pyright-1.1.318.tar` & `pyright-1.1.320.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:35:52.043554 pyright-1.1.318/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-21 09:35:42.000000 pyright-1.1.318/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-21 09:35:42.000000 pyright-1.1.318/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-21 09:35:52.043554 pyright-1.1.318/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-07-21 09:35:42.000000 pyright-1.1.318/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-21 09:35:42.000000 pyright-1.1.318/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:35:52.043554 pyright-1.1.318/pyright/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-21 09:35:42.000000 pyright-1.1.318/pyright/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-21 09:35:42.000000 pyright-1.1.318/pyright/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14622 2023-07-21 09:35:42.000000 pyright-1.1.318/pyright/_mureq.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-07-21 09:35:42.000000 pyright-1.1.318/pyright/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-21 09:35:42.000000 pyright-1.1.318/pyright/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-21 09:35:42.000000 pyright-1.1.318/pyright/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-21 09:35:42.000000 pyright-1.1.318/pyright/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-21 09:35:42.000000 pyright-1.1.318/pyright/langserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-07-21 09:35:42.000000 pyright-1.1.318/pyright/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-21 09:35:42.000000 pyright-1.1.318/pyright/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-21 09:35:42.000000 pyright-1.1.318/pyright/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:35:52.043554 pyright-1.1.318/pyright.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-21 09:35:51.000000 pyright-1.1.318/pyright.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-21 09:35:51.000000 pyright-1.1.318/pyright.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 09:35:51.000000 pyright-1.1.318/pyright.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-21 09:35:51.000000 pyright-1.1.318/pyright.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 09:35:51.000000 pyright-1.1.318/pyright.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-21 09:35:51.000000 pyright-1.1.318/pyright.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-21 09:35:51.000000 pyright-1.1.318/pyright.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-21 09:35:42.000000 pyright-1.1.318/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 09:35:52.043554 pyright-1.1.318/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2149 2023-07-21 09:35:42.000000 pyright-1.1.318/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:08:32.029809 pyright-1.1.320/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-02 11:08:19.000000 pyright-1.1.320/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-02 11:08:19.000000 pyright-1.1.320/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-08-02 11:08:32.029809 pyright-1.1.320/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-08-02 11:08:19.000000 pyright-1.1.320/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-02 11:08:19.000000 pyright-1.1.320/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:08:32.025809 pyright-1.1.320/pyright/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-08-02 11:08:19.000000 pyright-1.1.320/pyright/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-02 11:08:19.000000 pyright-1.1.320/pyright/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14622 2023-08-02 11:08:19.000000 pyright-1.1.320/pyright/_mureq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-08-02 11:08:19.000000 pyright-1.1.320/pyright/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-02 11:08:19.000000 pyright-1.1.320/pyright/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-08-02 11:08:19.000000 pyright-1.1.320/pyright/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-08-02 11:08:19.000000 pyright-1.1.320/pyright/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-08-02 11:08:19.000000 pyright-1.1.320/pyright/langserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-08-02 11:08:19.000000 pyright-1.1.320/pyright/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-02 11:08:19.000000 pyright-1.1.320/pyright/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-08-02 11:08:19.000000 pyright-1.1.320/pyright/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:08:32.029809 pyright-1.1.320/pyright.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-08-02 11:08:31.000000 pyright-1.1.320/pyright.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-02 11:08:31.000000 pyright-1.1.320/pyright.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:08:31.000000 pyright-1.1.320/pyright.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-02 11:08:31.000000 pyright-1.1.320/pyright.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:08:31.000000 pyright-1.1.320/pyright.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-02 11:08:31.000000 pyright-1.1.320/pyright.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-02 11:08:31.000000 pyright-1.1.320/pyright.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-02 11:08:19.000000 pyright-1.1.320/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 11:08:32.029809 pyright-1.1.320/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2149 2023-08-02 11:08:19.000000 pyright-1.1.320/setup.py
```

### Comparing `pyright-1.1.318/LICENSE` & `pyright-1.1.320/LICENSE`

 * *Files identical despite different names*

### Comparing `pyright-1.1.318/PKG-INFO` & `pyright-1.1.320/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyright
-Version: 1.1.318
+Version: 1.1.320
 Summary: Command line wrapper for pyright
 Home-page: https://github.com/RobertCraigie/pyright-python
 Author: Robert Craigie
 Maintainer: Robert Craigie
 License: MIT
 Project-URL: Source, https://github.com/RobertCraigie/pyright-python
 Project-URL: Tracker, https://github.com/RobertCraigie/pyright-python/issues
@@ -61,15 +61,15 @@
 ### Pre-commit
 
 You can also setup pyright to run automatically before each commit by setting up [pre-commit](https://pre-commit.com) and registering pyright in your `.pre-commit-config.yaml` file
 
 ```yaml
 repos:
   - repo: https://github.com/RobertCraigie/pyright-python
-    rev: v1.1.318
+    rev: v1.1.320
     hooks:
     - id: pyright
 ```
 
 Pre-commit will install pyright-python in its own virtual environment which can cause pyright to not be able to detect your installed dependencies.
 
 To fix this you can either [tell pre-commit](https://pre-commit.com/#config-additional_dependencies) to also install those dependencies or explicitly tell pyright which virtual environment to use by updating your [pyright configuration file](https://github.com/microsoft/pyright/blob/main/docs/configuration.md):
```

### Comparing `pyright-1.1.318/README.md` & `pyright-1.1.320/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 ### Pre-commit
 
 You can also setup pyright to run automatically before each commit by setting up [pre-commit](https://pre-commit.com) and registering pyright in your `.pre-commit-config.yaml` file
 
 ```yaml
 repos:
   - repo: https://github.com/RobertCraigie/pyright-python
-    rev: v1.1.318
+    rev: v1.1.320
     hooks:
     - id: pyright
 ```
 
 Pre-commit will install pyright-python in its own virtual environment which can cause pyright to not be able to detect your installed dependencies.
 
 To fix this you can either [tell pre-commit](https://pre-commit.com/#config-additional_dependencies) to also install those dependencies or explicitly tell pyright which virtual environment to use by updating your [pyright configuration file](https://github.com/microsoft/pyright/blob/main/docs/configuration.md):
```

### Comparing `pyright-1.1.318/pyright/__init__.py` & `pyright-1.1.320/pyright/__init__.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.318/pyright/_mureq.py` & `pyright-1.1.320/pyright/_mureq.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.318/pyright/_utils.py` & `pyright-1.1.320/pyright/_utils.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.318/pyright/cli.py` & `pyright-1.1.320/pyright/cli.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.318/pyright/errors.py` & `pyright-1.1.320/pyright/errors.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.318/pyright/langserver.py` & `pyright-1.1.320/pyright/langserver.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.318/pyright/node.py` & `pyright-1.1.320/pyright/node.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.318/pyright/types.py` & `pyright-1.1.320/pyright/types.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.318/pyright/utils.py` & `pyright-1.1.320/pyright/utils.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.318/pyright.egg-info/PKG-INFO` & `pyright-1.1.320/pyright.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyright
-Version: 1.1.318
+Version: 1.1.320
 Summary: Command line wrapper for pyright
 Home-page: https://github.com/RobertCraigie/pyright-python
 Author: Robert Craigie
 Maintainer: Robert Craigie
 License: MIT
 Project-URL: Source, https://github.com/RobertCraigie/pyright-python
 Project-URL: Tracker, https://github.com/RobertCraigie/pyright-python/issues
@@ -61,15 +61,15 @@
 ### Pre-commit
 
 You can also setup pyright to run automatically before each commit by setting up [pre-commit](https://pre-commit.com) and registering pyright in your `.pre-commit-config.yaml` file
 
 ```yaml
 repos:
   - repo: https://github.com/RobertCraigie/pyright-python
-    rev: v1.1.318
+    rev: v1.1.320
     hooks:
     - id: pyright
 ```
 
 Pre-commit will install pyright-python in its own virtual environment which can cause pyright to not be able to detect your installed dependencies.
 
 To fix this you can either [tell pre-commit](https://pre-commit.com/#config-additional_dependencies) to also install those dependencies or explicitly tell pyright which virtual environment to use by updating your [pyright configuration file](https://github.com/microsoft/pyright/blob/main/docs/configuration.md):
```

### Comparing `pyright-1.1.318/setup.py` & `pyright-1.1.320/setup.py`

 * *Files identical despite different names*


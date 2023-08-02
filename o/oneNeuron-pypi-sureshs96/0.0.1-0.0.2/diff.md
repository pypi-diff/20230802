# Comparing `tmp/oneNeuron_pypi-sureshs96-0.0.1.tar.gz` & `tmp/oneNeuron_pypi-sureshs96-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/oneNeuron_pypi/oneNeuron_pypi/dist/.tmp-gfyk12zg/oneNeuron_pypi-sureshs96-0.0.1.tar", last modified: Wed Aug  2 20:03:45 2023, max compression
+gzip compressed data, was "/home/runner/work/oneNeuron_pypi/oneNeuron_pypi/dist/.tmp-jjw8vba_/oneNeuron_pypi-sureshs96-0.0.2.tar", last modified: Wed Aug  2 20:47:08 2023, max compression
```

## Comparing `oneNeuron_pypi-sureshs96-0.0.1.tar` & `oneNeuron_pypi-sureshs96-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:03:45.000000 oneNeuron_pypi-sureshs96-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-02 20:03:32.000000 oneNeuron_pypi-sureshs96-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-02 20:03:45.000000 oneNeuron_pypi-sureshs96-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-02 20:03:32.000000 oneNeuron_pypi-sureshs96-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-02 20:03:32.000000 oneNeuron_pypi-sureshs96-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 20:03:45.000000 oneNeuron_pypi-sureshs96-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-08-02 20:03:32.000000 oneNeuron_pypi-sureshs96-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:03:45.000000 oneNeuron_pypi-sureshs96-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:03:45.000000 oneNeuron_pypi-sureshs96-0.0.1/src/oneNeuron/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 20:03:32.000000 oneNeuron_pypi-sureshs96-0.0.1/src/oneNeuron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-08-02 20:03:32.000000 oneNeuron_pypi-sureshs96-0.0.1/src/oneNeuron/perceptron.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:03:45.000000 oneNeuron_pypi-sureshs96-0.0.1/src/oneNeuron_pypi_sureshs96.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-02 20:03:45.000000 oneNeuron_pypi-sureshs96-0.0.1/src/oneNeuron_pypi_sureshs96.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-02 20:03:45.000000 oneNeuron_pypi-sureshs96-0.0.1/src/oneNeuron_pypi_sureshs96.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 20:03:45.000000 oneNeuron_pypi-sureshs96-0.0.1/src/oneNeuron_pypi_sureshs96.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-02 20:03:45.000000 oneNeuron_pypi-sureshs96-0.0.1/src/oneNeuron_pypi_sureshs96.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-02 20:03:45.000000 oneNeuron_pypi-sureshs96-0.0.1/src/oneNeuron_pypi_sureshs96.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:47:08.000000 oneNeuron_pypi-sureshs96-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-02 20:46:56.000000 oneNeuron_pypi-sureshs96-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-08-02 20:47:08.000000 oneNeuron_pypi-sureshs96-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-02 20:46:56.000000 oneNeuron_pypi-sureshs96-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-02 20:46:56.000000 oneNeuron_pypi-sureshs96-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 20:47:08.000000 oneNeuron_pypi-sureshs96-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-08-02 20:46:56.000000 oneNeuron_pypi-sureshs96-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:47:08.000000 oneNeuron_pypi-sureshs96-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:47:08.000000 oneNeuron_pypi-sureshs96-0.0.2/src/oneNeuron/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 20:46:56.000000 oneNeuron_pypi-sureshs96-0.0.2/src/oneNeuron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-08-02 20:46:56.000000 oneNeuron_pypi-sureshs96-0.0.2/src/oneNeuron/perceptron.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:47:08.000000 oneNeuron_pypi-sureshs96-0.0.2/src/oneNeuron_pypi_sureshs96.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-08-02 20:47:08.000000 oneNeuron_pypi-sureshs96-0.0.2/src/oneNeuron_pypi_sureshs96.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-08-02 20:47:08.000000 oneNeuron_pypi-sureshs96-0.0.2/src/oneNeuron_pypi_sureshs96.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 20:47:08.000000 oneNeuron_pypi-sureshs96-0.0.2/src/oneNeuron_pypi_sureshs96.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-02 20:47:08.000000 oneNeuron_pypi-sureshs96-0.0.2/src/oneNeuron_pypi_sureshs96.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-02 20:47:08.000000 oneNeuron_pypi-sureshs96-0.0.2/src/oneNeuron_pypi_sureshs96.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:47:08.000000 oneNeuron_pypi-sureshs96-0.0.2/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 20:46:56.000000 oneNeuron_pypi-sureshs96-0.0.2/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-08-02 20:46:56.000000 oneNeuron_pypi-sureshs96-0.0.2/src/utils/common_utils.py
```

### Comparing `oneNeuron_pypi-sureshs96-0.0.1/LICENSE` & `oneNeuron_pypi-sureshs96-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oneNeuron_pypi-sureshs96-0.0.1/PKG-INFO` & `oneNeuron_pypi-sureshs96-0.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oneNeuron_pypi-sureshs96
-Version: 0.0.1
+Version: 0.0.2
 Summary: its an implimentation of Perceptron
 Home-page: https://github.com/sureshs96/oneNeuron_pypi
 Author: sureshs96
 Author-email: sunny.c17hawke@gmail.com
 Project-URL: Bug Tracker, https://github.com/sureshs96/oneNeuron_pypi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,11 +12,23 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # oneNeuron_pypi
 oneNeuron python package creation
 
+## How to use -
+```python
+    from oneNeuron.perceptron import Perceptron
+    from utils.common_utils import prepare_data, save_model, save_plot
+    ## Get X and y from dataframe
+    X,y = prepare_data(df)
+    model = Perceptron(eta, epochs)
+    model.fit(X,y)
+    _ = model.total_loss()
+    save_model(model, modelname)
+    save_plot(df , plotfilename, model)
+```
 # Reference -
 [official python docs](https://packaging.python.org/tutorials/packaging-projects/)
 
 [github docs for github actions](https://docs.github.com/en/actions/guides/building-and-testing-python#publishing-to-package-registeries)
```

### Comparing `oneNeuron_pypi-sureshs96-0.0.1/setup.py` & `oneNeuron_pypi-sureshs96-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 PROJECT_NAME = "oneNeuron_pypi"
 USER_NAME = "sureshs96"
 
 setuptools.setup(
     name=f"{PROJECT_NAME}-{USER_NAME}",
-    version="0.0.1",
+    version="0.0.2",
     author=USER_NAME,
     author_email="sunny.c17hawke@gmail.com",
     description="its an implimentation of Perceptron",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=f"https://github.com/{USER_NAME}/{PROJECT_NAME}",
     project_urls={
```

### Comparing `oneNeuron_pypi-sureshs96-0.0.1/src/oneNeuron/perceptron.py` & `oneNeuron_pypi-sureshs96-0.0.2/src/oneNeuron/perceptron.py`

 * *Files identical despite different names*


# Comparing `tmp/mltb2-0.4.0.tar.gz` & `tmp/mltb2-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mltb2-0.4.0.tar", last modified: Wed Aug  2 20:51:53 2023, max compression
+gzip compressed data, was "mltb2-0.4.2.tar", last modified: Wed Aug  2 21:46:28 2023, max compression
```

## Comparing `mltb2-0.4.0.tar` & `mltb2-0.4.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:51:53.592503 mltb2-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-02 20:51:43.000000 mltb2-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 20:51:43.000000 mltb2-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-08-02 20:51:53.592503 mltb2-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-02 20:51:43.000000 mltb2-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:51:53.588503 mltb2-0.4.0/mltb2/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-08-02 20:51:43.000000 mltb2-0.4.0/mltb2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-08-02 20:51:43.000000 mltb2-0.4.0/mltb2/fasttext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-08-02 20:51:43.000000 mltb2-0.4.0/mltb2/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-08-02 20:51:43.000000 mltb2-0.4.0/mltb2/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-08-02 20:51:43.000000 mltb2-0.4.0/mltb2/optuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-08-02 20:51:43.000000 mltb2-0.4.0/mltb2/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-08-02 20:51:43.000000 mltb2-0.4.0/mltb2/somajo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-08-02 20:51:43.000000 mltb2-0.4.0/mltb2/somajo_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-08-02 20:51:43.000000 mltb2-0.4.0/mltb2/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:51:53.592503 mltb2-0.4.0/mltb2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-08-02 20:51:53.000000 mltb2-0.4.0/mltb2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-08-02 20:51:53.000000 mltb2-0.4.0/mltb2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 20:51:53.000000 mltb2-0.4.0/mltb2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 20:51:53.000000 mltb2-0.4.0/mltb2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-02 20:51:53.000000 mltb2-0.4.0/mltb2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-02 20:51:53.000000 mltb2-0.4.0/mltb2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-08-02 20:51:43.000000 mltb2-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-02 20:51:53.592503 mltb2-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-08-02 20:51:43.000000 mltb2-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:51:53.592503 mltb2-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 20:51:43.000000 mltb2-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-08-02 20:51:43.000000 mltb2-0.4.0/tests/test__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-08-02 20:51:43.000000 mltb2-0.4.0/tests/test_fasttext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-08-02 20:51:43.000000 mltb2-0.4.0/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-02 20:51:43.000000 mltb2-0.4.0/tests/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-02 20:51:43.000000 mltb2-0.4.0/tests/test_optuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-08-02 20:51:43.000000 mltb2-0.4.0/tests/test_somajo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-08-02 20:51:43.000000 mltb2-0.4.0/tests/test_somajo_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-08-02 20:51:43.000000 mltb2-0.4.0/tests/test_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:46:28.700294 mltb2-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-02 21:46:16.000000 mltb2-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 21:46:16.000000 mltb2-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-08-02 21:46:28.700294 mltb2-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-02 21:46:16.000000 mltb2-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:46:28.696294 mltb2-0.4.2/mltb2/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-08-02 21:46:16.000000 mltb2-0.4.2/mltb2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-08-02 21:46:16.000000 mltb2-0.4.2/mltb2/fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-08-02 21:46:16.000000 mltb2-0.4.2/mltb2/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-08-02 21:46:16.000000 mltb2-0.4.2/mltb2/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-08-02 21:46:16.000000 mltb2-0.4.2/mltb2/optuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-08-02 21:46:16.000000 mltb2-0.4.2/mltb2/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-08-02 21:46:16.000000 mltb2-0.4.2/mltb2/somajo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-08-02 21:46:16.000000 mltb2-0.4.2/mltb2/somajo_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-08-02 21:46:16.000000 mltb2-0.4.2/mltb2/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:46:28.696294 mltb2-0.4.2/mltb2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-08-02 21:46:28.000000 mltb2-0.4.2/mltb2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-08-02 21:46:28.000000 mltb2-0.4.2/mltb2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:46:28.000000 mltb2-0.4.2/mltb2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:46:28.000000 mltb2-0.4.2/mltb2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-02 21:46:28.000000 mltb2-0.4.2/mltb2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-02 21:46:28.000000 mltb2-0.4.2/mltb2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-08-02 21:46:16.000000 mltb2-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-02 21:46:28.700294 mltb2-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-08-02 21:46:16.000000 mltb2-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:46:28.700294 mltb2-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 21:46:16.000000 mltb2-0.4.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-08-02 21:46:16.000000 mltb2-0.4.2/tests/test__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-08-02 21:46:16.000000 mltb2-0.4.2/tests/test_fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-08-02 21:46:16.000000 mltb2-0.4.2/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-02 21:46:16.000000 mltb2-0.4.2/tests/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-02 21:46:16.000000 mltb2-0.4.2/tests/test_optuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-08-02 21:46:16.000000 mltb2-0.4.2/tests/test_somajo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-08-02 21:46:16.000000 mltb2-0.4.2/tests/test_somajo_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-08-02 21:46:16.000000 mltb2-0.4.2/tests/test_transformers.py
```

### Comparing `mltb2-0.4.0/LICENSE` & `mltb2-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.0/PKG-INFO` & `mltb2-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mltb2
-Version: 0.4.0
+Version: 0.4.2
 Summary: Machine Learning Toolbox
 Home-page: https://github.com/telekom/mltb2
 Author: Philip May
 Author-email: philip@may.la
 Maintainer: Philip May
 Project-URL: Bug Tracker, https://github.com/telekom/mltb2/issues
 Project-URL: Documentation, https://telekom.github.io/mltb2/
```

### Comparing `mltb2-0.4.0/README.md` & `mltb2-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.0/mltb2/fasttext.py` & `mltb2-0.4.2/mltb2/fasttext.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.0/mltb2/files.py` & `mltb2-0.4.2/mltb2/files.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.0/mltb2/openai.py` & `mltb2-0.4.2/mltb2/openai.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.0/mltb2/optuna.py` & `mltb2-0.4.2/mltb2/optuna.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.0/mltb2/plot.py` & `mltb2-0.4.2/mltb2/plot.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.0/mltb2/somajo.py` & `mltb2-0.4.2/mltb2/somajo.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.0/mltb2/somajo_transformers.py` & `mltb2-0.4.2/mltb2/somajo_transformers.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.0/mltb2/transformers.py` & `mltb2-0.4.2/mltb2/transformers.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.0/mltb2.egg-info/PKG-INFO` & `mltb2-0.4.2/mltb2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mltb2
-Version: 0.4.0
+Version: 0.4.2
 Summary: Machine Learning Toolbox
 Home-page: https://github.com/telekom/mltb2
 Author: Philip May
 Author-email: philip@may.la
 Maintainer: Philip May
 Project-URL: Bug Tracker, https://github.com/telekom/mltb2/issues
 Project-URL: Documentation, https://telekom.github.io/mltb2/
```

### Comparing `mltb2-0.4.0/mltb2.egg-info/SOURCES.txt` & `mltb2-0.4.2/mltb2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.0/mltb2.egg-info/requires.txt` & `mltb2-0.4.2/mltb2.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 numpy
 scipy
 tqdm
 
 [all]
-transformers
-black
-flake8
-pydocstyle
-pylint
-tqdm
+scikit-learn
+optuna
+fasttext-wheel
 tiktoken
+sphinx
+numpy
+flake8
+SoMaJo
+packaging
 sphinx_copybutton
-optuna
+mypy
+pydocstyle
+matplotlib
+transformers
 sphinx_rtd_theme
+isort
 platformdirs
 torch
-fasttext-wheel
 pylintfileheader
-scikit-learn
-packaging
-mypy
-sphinx
+black
 scipy
-isort
-matplotlib
-numpy
-SoMaJo
-pytest
 mdformat
+tqdm
+pylint
+pytest
 
 [checking]
 black
 flake8
 isort
 mdformat
 pydocstyle
@@ -42,59 +42,59 @@
 [doc]
 sphinx
 sphinx_rtd_theme
 sphinx_copybutton
 
 [fasttext]
 fasttext-wheel
-scikit-learn
 platformdirs
+scikit-learn
 
 [files]
-scikit-learn
 platformdirs
+scikit-learn
 
 [openai]
 tiktoken
 
 [optional]
-transformers
+torch
+scikit-learn
 SoMaJo
-scipy
-optuna
 matplotlib
+tiktoken
+transformers
+optuna
+scipy
+fasttext-wheel
+platformdirs
 numpy
 tqdm
-torch
-platformdirs
-fasttext-wheel
-scikit-learn
-tiktoken
 
 [optuna]
 numpy
 optuna
 scipy
 
 [plot]
 matplotlib
 
 [somajo]
-SoMaJo
 tqdm
+SoMaJo
 
 [somajo_transformers]
-transformers
-scikit-learn
-tqdm
 torch
+scikit-learn
+transformers
 SoMaJo
+tqdm
 
 [testing]
 pytest
 packaging
 
 [transformers]
-transformers
+torch
 scikit-learn
+transformers
 tqdm
-torch
```

### Comparing `mltb2-0.4.0/pyproject.toml` & `mltb2-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.0/setup.py` & `mltb2-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.0/tests/test_fasttext.py` & `mltb2-0.4.2/tests/test_fasttext.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.0/tests/test_files.py` & `mltb2-0.4.2/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.0/tests/test_openai.py` & `mltb2-0.4.2/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.0/tests/test_optuna.py` & `mltb2-0.4.2/tests/test_optuna.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.0/tests/test_somajo.py` & `mltb2-0.4.2/tests/test_somajo.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.0/tests/test_somajo_transformers.py` & `mltb2-0.4.2/tests/test_somajo_transformers.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.0/tests/test_transformers.py` & `mltb2-0.4.2/tests/test_transformers.py`

 * *Files identical despite different names*


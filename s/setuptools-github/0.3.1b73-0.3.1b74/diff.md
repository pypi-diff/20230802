# Comparing `tmp/setuptools-github-0.3.1b73.tar.gz` & `tmp/setuptools-github-0.3.1b74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-github-0.3.1b73.tar", last modified: Wed Aug  2 18:28:20 2023, max compression
+gzip compressed data, was "setuptools-github-0.3.1b74.tar", last modified: Wed Aug  2 18:41:00 2023, max compression
```

## Comparing `setuptools-github-0.3.1b73.tar` & `setuptools-github-0.3.1b74.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:20.819696 setuptools-github-0.3.1b73/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-08-02 18:28:20.819696 setuptools-github-0.3.1b73/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-08-02 18:28:20.000000 setuptools-github-0.3.1b73/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 18:28:20.819696 setuptools-github-0.3.1b73/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:20.815696 setuptools-github-0.3.1b73/setuptools_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-08-02 18:28:20.000000 setuptools-github-0.3.1b73/setuptools_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-02 18:28:20.000000 setuptools-github-0.3.1b73/setuptools_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 18:28:20.000000 setuptools-github-0.3.1b73/setuptools_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-02 18:28:20.000000 setuptools-github-0.3.1b73/setuptools_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 18:28:20.000000 setuptools-github-0.3.1b73/setuptools_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 18:28:20.000000 setuptools-github-0.3.1b73/setuptools_github.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:20.815696 setuptools-github-0.3.1b73/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:20.815696 setuptools-github-0.3.1b73/src/setuptools_github/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 18:28:20.000000 setuptools-github-0.3.1b73/src/setuptools_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/src/setuptools_github/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/src/setuptools_github/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/src/setuptools_github/scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/src/setuptools_github/script.py
--rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/src/setuptools_github/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:20.815696 setuptools-github-0.3.1b73/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/tests/test_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:41:00.706325 setuptools-github-0.3.1b74/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-08-02 18:41:00.706325 setuptools-github-0.3.1b74/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-08-02 18:41:00.000000 setuptools-github-0.3.1b74/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 18:41:00.706325 setuptools-github-0.3.1b74/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:41:00.702324 setuptools-github-0.3.1b74/setuptools_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-08-02 18:41:00.000000 setuptools-github-0.3.1b74/setuptools_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-02 18:41:00.000000 setuptools-github-0.3.1b74/setuptools_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 18:41:00.000000 setuptools-github-0.3.1b74/setuptools_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-02 18:41:00.000000 setuptools-github-0.3.1b74/setuptools_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 18:41:00.000000 setuptools-github-0.3.1b74/setuptools_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 18:41:00.000000 setuptools-github-0.3.1b74/setuptools_github.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:41:00.702324 setuptools-github-0.3.1b74/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:41:00.702324 setuptools-github-0.3.1b74/src/setuptools_github/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 18:41:00.000000 setuptools-github-0.3.1b74/src/setuptools_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/src/setuptools_github/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/src/setuptools_github/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/src/setuptools_github/scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/src/setuptools_github/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/src/setuptools_github/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:41:00.706325 setuptools-github-0.3.1b74/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/tests/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/tests/test_tools.py
```

### Comparing `setuptools-github-0.3.1b73/LICENSE` & `setuptools-github-0.3.1b74/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b73/PKG-INFO` & `setuptools-github-0.3.1b74/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.1b73
+Version: 0.3.1b74
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `setuptools-github-0.3.1b73/README.md` & `setuptools-github-0.3.1b74/README.md`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b73/pyproject.toml` & `setuptools-github-0.3.1b74/pyproject.toml`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b73/setup.py` & `setuptools-github-0.3.1b74/setup.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b73/setuptools_github.egg-info/PKG-INFO` & `setuptools-github-0.3.1b74/setuptools_github.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.1b73
+Version: 0.3.1b74
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `setuptools-github-0.3.1b73/setuptools_github.egg-info/SOURCES.txt` & `setuptools-github-0.3.1b74/setuptools_github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b73/src/setuptools_github/checks.py` & `setuptools-github-0.3.1b74/src/setuptools_github/checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b73/src/setuptools_github/cli.py` & `setuptools-github-0.3.1b74/src/setuptools_github/cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b73/src/setuptools_github/scm.py` & `setuptools-github-0.3.1b74/src/setuptools_github/scm.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b73/src/setuptools_github/script.py` & `setuptools-github-0.3.1b74/src/setuptools_github/script.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b73/src/setuptools_github/tools.py` & `setuptools-github-0.3.1b74/src/setuptools_github/tools.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b73/tests/conftest.py` & `setuptools-github-0.3.1b74/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b73/tests/test_checks.py` & `setuptools-github-0.3.1b74/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b73/tests/test_cli.py` & `setuptools-github-0.3.1b74/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b73/tests/test_conftest.py` & `setuptools-github-0.3.1b74/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b73/tests/test_scm.py` & `setuptools-github-0.3.1b74/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b73/tests/test_script.py` & `setuptools-github-0.3.1b74/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b73/tests/test_tools.py` & `setuptools-github-0.3.1b74/tests/test_tools.py`

 * *Files identical despite different names*


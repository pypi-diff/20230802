# Comparing `tmp/setuptools-github-0.3.1b70.tar.gz` & `tmp/setuptools-github-0.3.1b72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-github-0.3.1b70.tar", last modified: Wed Aug  2 17:53:05 2023, max compression
+gzip compressed data, was "setuptools-github-0.3.1b72.tar", last modified: Wed Aug  2 18:06:36 2023, max compression
```

## Comparing `setuptools-github-0.3.1b70.tar` & `setuptools-github-0.3.1b72.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:53:05.194146 setuptools-github-0.3.1b70/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-08-02 17:53:05.194146 setuptools-github-0.3.1b70/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-08-02 17:53:05.000000 setuptools-github-0.3.1b70/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 17:53:05.194146 setuptools-github-0.3.1b70/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:53:05.190146 setuptools-github-0.3.1b70/setuptools_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-08-02 17:53:05.000000 setuptools-github-0.3.1b70/setuptools_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-02 17:53:05.000000 setuptools-github-0.3.1b70/setuptools_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:53:05.000000 setuptools-github-0.3.1b70/setuptools_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-02 17:53:05.000000 setuptools-github-0.3.1b70/setuptools_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 17:53:05.000000 setuptools-github-0.3.1b70/setuptools_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 17:53:05.000000 setuptools-github-0.3.1b70/setuptools_github.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:53:05.186146 setuptools-github-0.3.1b70/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:53:05.190146 setuptools-github-0.3.1b70/src/setuptools_github/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 17:53:05.000000 setuptools-github-0.3.1b70/src/setuptools_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/src/setuptools_github/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/src/setuptools_github/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/src/setuptools_github/scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/src/setuptools_github/script.py
--rw-r--r--   0 runner    (1001) docker     (123)    10918 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/src/setuptools_github/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:53:05.194146 setuptools-github-0.3.1b70/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/tests/test_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     9070 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:06:36.280653 setuptools-github-0.3.1b72/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-08-02 18:06:36.280653 setuptools-github-0.3.1b72/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-08-02 18:06:36.000000 setuptools-github-0.3.1b72/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 18:06:36.280653 setuptools-github-0.3.1b72/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:06:36.280653 setuptools-github-0.3.1b72/setuptools_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-08-02 18:06:36.000000 setuptools-github-0.3.1b72/setuptools_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-02 18:06:36.000000 setuptools-github-0.3.1b72/setuptools_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 18:06:36.000000 setuptools-github-0.3.1b72/setuptools_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-02 18:06:36.000000 setuptools-github-0.3.1b72/setuptools_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 18:06:36.000000 setuptools-github-0.3.1b72/setuptools_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 18:06:36.000000 setuptools-github-0.3.1b72/setuptools_github.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:06:36.280653 setuptools-github-0.3.1b72/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:06:36.280653 setuptools-github-0.3.1b72/src/setuptools_github/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 18:06:36.000000 setuptools-github-0.3.1b72/src/setuptools_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/src/setuptools_github/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/src/setuptools_github/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/src/setuptools_github/scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/src/setuptools_github/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10918 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/src/setuptools_github/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:06:36.280653 setuptools-github-0.3.1b72/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/tests/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9070 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/tests/test_tools.py
```

### Comparing `setuptools-github-0.3.1b70/LICENSE` & `setuptools-github-0.3.1b72/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b70/PKG-INFO` & `setuptools-github-0.3.1b72/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.1b70
+Version: 0.3.1b72
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -17,22 +17,21 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # setuptools-github
 [![PyPI version](https://img.shields.io/pypi/v/setuptools-github.svg?color=blue)](https://pypi.org/project/setuptools-github)
 [![Python versions](https://img.shields.io/pypi/pyversions/setuptools-github.svg)](https://pypi.org/project/setuptools-github)
 [![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions)
-[![Codecov](https://codecov.io/gh/cav71/setuptools-github/branch/0.3.1/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/0.3.1)
+[![Codecov](https://codecov.io/gh/cav71/setuptools-github/branch/beta%2F0.3.1/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.1)
+
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
 [![Types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 
 
-[![An old rock in the desert](/assets/images/shiprock.jpg "Shiprock, New Mexico by Beau Rogers")](https://www.flickr.com/photos/beaurogers/31833779864/in/photolist-Qv3rFw-34mt9F-a9Cmfy-5Ha3Zi-9msKdv-o3hgjr-hWpUte-4WMsJ1-KUQ8N-deshUb-vssBD-6CQci6-8AFCiD-zsJWT-nNfsgB-dPDwZJ-bn9JGn-5HtSXY-6CUhAL-a4UTXB-ugPum-KUPSo-fBLNm-6CUmpy-4WMsc9-8a7D3T-83KJev-6CQ2bK-nNusHJ-a78rQH-nw3NvT-7aq2qf-8wwBso-3nNceh-ugSKP-4mh4kh-bbeeqH-a7biME-q3PtTf-brFpgb-cg38zw-bXMZc-nJPELD-f58Lmo-bXMYG-bz8AAi-bxNtNT-bXMYi-bXMY6-bXMYv)
-
 ## Quick start
 setuptools-github helps to implement a simple project life cycle
 aimed at delivering packages into [PyPI](https://pypi.org). Basically:
 - beta packages are built from a /beta/N.M.O branch generating a **project-name-N.M.ObX** into PyPI
 - tagging with /release/N.M.O a /beta/N.M.O branch commit will release **project-name-N.M.O**
 
 This integrates well with the standard release logic in PyPI (see [example](https://pypi.org/project/setuptools-github/#history))
```

### Comparing `setuptools-github-0.3.1b70/README.md` & `setuptools-github-0.3.1b72/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # setuptools-github
 [![PyPI version](https://img.shields.io/pypi/v/setuptools-github.svg?color=blue)](https://pypi.org/project/setuptools-github)
 [![Python versions](https://img.shields.io/pypi/pyversions/setuptools-github.svg)](https://pypi.org/project/setuptools-github)
 [![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions)
-[![Codecov](https://codecov.io/gh/cav71/setuptools-github/branch/0.3.1/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/0.3.1)
+[![Codecov](https://codecov.io/gh/cav71/setuptools-github/branch/beta%2F0.3.1/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.1)
+
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
 [![Types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 
 
-[![An old rock in the desert](/assets/images/shiprock.jpg "Shiprock, New Mexico by Beau Rogers")](https://www.flickr.com/photos/beaurogers/31833779864/in/photolist-Qv3rFw-34mt9F-a9Cmfy-5Ha3Zi-9msKdv-o3hgjr-hWpUte-4WMsJ1-KUQ8N-deshUb-vssBD-6CQci6-8AFCiD-zsJWT-nNfsgB-dPDwZJ-bn9JGn-5HtSXY-6CUhAL-a4UTXB-ugPum-KUPSo-fBLNm-6CUmpy-4WMsc9-8a7D3T-83KJev-6CQ2bK-nNusHJ-a78rQH-nw3NvT-7aq2qf-8wwBso-3nNceh-ugSKP-4mh4kh-bbeeqH-a7biME-q3PtTf-brFpgb-cg38zw-bXMZc-nJPELD-f58Lmo-bXMYG-bz8AAi-bxNtNT-bXMYi-bXMY6-bXMYv)
-
 ## Quick start
 setuptools-github helps to implement a simple project life cycle
 aimed at delivering packages into [PyPI](https://pypi.org). Basically:
 - beta packages are built from a /beta/N.M.O branch generating a **project-name-N.M.ObX** into PyPI
 - tagging with /release/N.M.O a /beta/N.M.O branch commit will release **project-name-N.M.O**
 
 This integrates well with the standard release logic in PyPI (see [example](https://pypi.org/project/setuptools-github/#history))
```

### Comparing `setuptools-github-0.3.1b70/pyproject.toml` & `setuptools-github-0.3.1b72/pyproject.toml`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b70/setup.py` & `setuptools-github-0.3.1b72/setup.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b70/setuptools_github.egg-info/PKG-INFO` & `setuptools-github-0.3.1b72/setuptools_github.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.1b70
+Version: 0.3.1b72
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -17,22 +17,21 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # setuptools-github
 [![PyPI version](https://img.shields.io/pypi/v/setuptools-github.svg?color=blue)](https://pypi.org/project/setuptools-github)
 [![Python versions](https://img.shields.io/pypi/pyversions/setuptools-github.svg)](https://pypi.org/project/setuptools-github)
 [![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions)
-[![Codecov](https://codecov.io/gh/cav71/setuptools-github/branch/0.3.1/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/0.3.1)
+[![Codecov](https://codecov.io/gh/cav71/setuptools-github/branch/beta%2F0.3.1/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.1)
+
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
 [![Types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 
 
-[![An old rock in the desert](/assets/images/shiprock.jpg "Shiprock, New Mexico by Beau Rogers")](https://www.flickr.com/photos/beaurogers/31833779864/in/photolist-Qv3rFw-34mt9F-a9Cmfy-5Ha3Zi-9msKdv-o3hgjr-hWpUte-4WMsJ1-KUQ8N-deshUb-vssBD-6CQci6-8AFCiD-zsJWT-nNfsgB-dPDwZJ-bn9JGn-5HtSXY-6CUhAL-a4UTXB-ugPum-KUPSo-fBLNm-6CUmpy-4WMsc9-8a7D3T-83KJev-6CQ2bK-nNusHJ-a78rQH-nw3NvT-7aq2qf-8wwBso-3nNceh-ugSKP-4mh4kh-bbeeqH-a7biME-q3PtTf-brFpgb-cg38zw-bXMZc-nJPELD-f58Lmo-bXMYG-bz8AAi-bxNtNT-bXMYi-bXMY6-bXMYv)
-
 ## Quick start
 setuptools-github helps to implement a simple project life cycle
 aimed at delivering packages into [PyPI](https://pypi.org). Basically:
 - beta packages are built from a /beta/N.M.O branch generating a **project-name-N.M.ObX** into PyPI
 - tagging with /release/N.M.O a /beta/N.M.O branch commit will release **project-name-N.M.O**
 
 This integrates well with the standard release logic in PyPI (see [example](https://pypi.org/project/setuptools-github/#history))
```

### Comparing `setuptools-github-0.3.1b70/setuptools_github.egg-info/SOURCES.txt` & `setuptools-github-0.3.1b72/setuptools_github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b70/src/setuptools_github/checks.py` & `setuptools-github-0.3.1b72/src/setuptools_github/checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b70/src/setuptools_github/cli.py` & `setuptools-github-0.3.1b72/src/setuptools_github/cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b70/src/setuptools_github/scm.py` & `setuptools-github-0.3.1b72/src/setuptools_github/scm.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b70/src/setuptools_github/script.py` & `setuptools-github-0.3.1b72/src/setuptools_github/script.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b70/src/setuptools_github/tools.py` & `setuptools-github-0.3.1b72/src/setuptools_github/tools.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b70/tests/conftest.py` & `setuptools-github-0.3.1b72/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b70/tests/test_checks.py` & `setuptools-github-0.3.1b72/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b70/tests/test_cli.py` & `setuptools-github-0.3.1b72/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b70/tests/test_conftest.py` & `setuptools-github-0.3.1b72/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b70/tests/test_scm.py` & `setuptools-github-0.3.1b72/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b70/tests/test_script.py` & `setuptools-github-0.3.1b72/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b70/tests/test_tools.py` & `setuptools-github-0.3.1b72/tests/test_tools.py`

 * *Files identical despite different names*


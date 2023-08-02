# Comparing `tmp/setuptools-github-0.3.1b69.tar.gz` & `tmp/setuptools-github-0.3.1b70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-github-0.3.1b69.tar", last modified: Wed Aug  2 16:17:30 2023, max compression
+gzip compressed data, was "setuptools-github-0.3.1b70.tar", last modified: Wed Aug  2 17:53:05 2023, max compression
```

## Comparing `setuptools-github-0.3.1b69.tar` & `setuptools-github-0.3.1b70.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:17:30.159953 setuptools-github-0.3.1b69/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-08-02 16:17:30.159953 setuptools-github-0.3.1b69/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-08-02 16:17:30.000000 setuptools-github-0.3.1b69/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 16:17:30.159953 setuptools-github-0.3.1b69/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:17:30.155953 setuptools-github-0.3.1b69/setuptools_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-08-02 16:17:30.000000 setuptools-github-0.3.1b69/setuptools_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-02 16:17:30.000000 setuptools-github-0.3.1b69/setuptools_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:17:30.000000 setuptools-github-0.3.1b69/setuptools_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-02 16:17:30.000000 setuptools-github-0.3.1b69/setuptools_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 16:17:30.000000 setuptools-github-0.3.1b69/setuptools_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 16:17:30.000000 setuptools-github-0.3.1b69/setuptools_github.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:17:30.155953 setuptools-github-0.3.1b69/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:17:30.159953 setuptools-github-0.3.1b69/src/setuptools_github/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 16:17:30.000000 setuptools-github-0.3.1b69/src/setuptools_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/src/setuptools_github/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/src/setuptools_github/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/src/setuptools_github/scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/src/setuptools_github/script.py
--rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/src/setuptools_github/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:17:30.159953 setuptools-github-0.3.1b69/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/tests/test_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     9070 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:53:05.194146 setuptools-github-0.3.1b70/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-08-02 17:53:05.194146 setuptools-github-0.3.1b70/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-08-02 17:53:05.000000 setuptools-github-0.3.1b70/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 17:53:05.194146 setuptools-github-0.3.1b70/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:53:05.190146 setuptools-github-0.3.1b70/setuptools_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-08-02 17:53:05.000000 setuptools-github-0.3.1b70/setuptools_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-02 17:53:05.000000 setuptools-github-0.3.1b70/setuptools_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:53:05.000000 setuptools-github-0.3.1b70/setuptools_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-02 17:53:05.000000 setuptools-github-0.3.1b70/setuptools_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 17:53:05.000000 setuptools-github-0.3.1b70/setuptools_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 17:53:05.000000 setuptools-github-0.3.1b70/setuptools_github.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:53:05.186146 setuptools-github-0.3.1b70/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:53:05.190146 setuptools-github-0.3.1b70/src/setuptools_github/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 17:53:05.000000 setuptools-github-0.3.1b70/src/setuptools_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/src/setuptools_github/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/src/setuptools_github/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/src/setuptools_github/scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/src/setuptools_github/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10918 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/src/setuptools_github/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:53:05.194146 setuptools-github-0.3.1b70/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/tests/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9070 2023-08-02 17:52:31.000000 setuptools-github-0.3.1b70/tests/test_tools.py
```

### Comparing `setuptools-github-0.3.1b69/LICENSE` & `setuptools-github-0.3.1b70/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b69/PKG-INFO` & `setuptools-github-0.3.1b70/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.1b69
+Version: 0.3.1b70
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -16,22 +16,22 @@
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # setuptools-github
 [![PyPI version](https://img.shields.io/pypi/v/setuptools-github.svg?color=blue)](https://pypi.org/project/setuptools-github)
 [![Python versions](https://img.shields.io/pypi/pyversions/setuptools-github.svg)](https://pypi.org/project/setuptools-github)
-[![Build](https://github.com/cav71/setuptools-github/actions/workflows/master.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions)
-[![Coverage](https://codecov.io/gh/cav71/setuptools-github/branch/beta/0.3.1/graph/badge.svg)](Coverage)
-
+[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions)
+[![Codecov](https://codecov.io/gh/cav71/setuptools-github/branch/0.3.1/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/0.3.1)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
 [![Types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 
 
+[![An old rock in the desert](/assets/images/shiprock.jpg "Shiprock, New Mexico by Beau Rogers")](https://www.flickr.com/photos/beaurogers/31833779864/in/photolist-Qv3rFw-34mt9F-a9Cmfy-5Ha3Zi-9msKdv-o3hgjr-hWpUte-4WMsJ1-KUQ8N-deshUb-vssBD-6CQci6-8AFCiD-zsJWT-nNfsgB-dPDwZJ-bn9JGn-5HtSXY-6CUhAL-a4UTXB-ugPum-KUPSo-fBLNm-6CUmpy-4WMsc9-8a7D3T-83KJev-6CQ2bK-nNusHJ-a78rQH-nw3NvT-7aq2qf-8wwBso-3nNceh-ugSKP-4mh4kh-bbeeqH-a7biME-q3PtTf-brFpgb-cg38zw-bXMZc-nJPELD-f58Lmo-bXMYG-bz8AAi-bxNtNT-bXMYi-bXMY6-bXMYv)
 
 ## Quick start
 setuptools-github helps to implement a simple project life cycle
 aimed at delivering packages into [PyPI](https://pypi.org). Basically:
 - beta packages are built from a /beta/N.M.O branch generating a **project-name-N.M.ObX** into PyPI
 - tagging with /release/N.M.O a /beta/N.M.O branch commit will release **project-name-N.M.O**
```

### Comparing `setuptools-github-0.3.1b69/README.md` & `setuptools-github-0.3.1b70/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # setuptools-github
 [![PyPI version](https://img.shields.io/pypi/v/setuptools-github.svg?color=blue)](https://pypi.org/project/setuptools-github)
 [![Python versions](https://img.shields.io/pypi/pyversions/setuptools-github.svg)](https://pypi.org/project/setuptools-github)
-[![Build](https://github.com/cav71/setuptools-github/actions/workflows/master.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions)
-[![Coverage](https://codecov.io/gh/cav71/setuptools-github/branch/beta/0.3.1/graph/badge.svg)](Coverage)
-
+[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions)
+[![Codecov](https://codecov.io/gh/cav71/setuptools-github/branch/0.3.1/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/0.3.1)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
 [![Types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 
 
+[![An old rock in the desert](/assets/images/shiprock.jpg "Shiprock, New Mexico by Beau Rogers")](https://www.flickr.com/photos/beaurogers/31833779864/in/photolist-Qv3rFw-34mt9F-a9Cmfy-5Ha3Zi-9msKdv-o3hgjr-hWpUte-4WMsJ1-KUQ8N-deshUb-vssBD-6CQci6-8AFCiD-zsJWT-nNfsgB-dPDwZJ-bn9JGn-5HtSXY-6CUhAL-a4UTXB-ugPum-KUPSo-fBLNm-6CUmpy-4WMsc9-8a7D3T-83KJev-6CQ2bK-nNusHJ-a78rQH-nw3NvT-7aq2qf-8wwBso-3nNceh-ugSKP-4mh4kh-bbeeqH-a7biME-q3PtTf-brFpgb-cg38zw-bXMZc-nJPELD-f58Lmo-bXMYG-bz8AAi-bxNtNT-bXMYi-bXMY6-bXMYv)
 
 ## Quick start
 setuptools-github helps to implement a simple project life cycle
 aimed at delivering packages into [PyPI](https://pypi.org). Basically:
 - beta packages are built from a /beta/N.M.O branch generating a **project-name-N.M.ObX** into PyPI
 - tagging with /release/N.M.O a /beta/N.M.O branch commit will release **project-name-N.M.O**
```

### Comparing `setuptools-github-0.3.1b69/pyproject.toml` & `setuptools-github-0.3.1b70/pyproject.toml`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b69/setup.py` & `setuptools-github-0.3.1b70/setup.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b69/setuptools_github.egg-info/PKG-INFO` & `setuptools-github-0.3.1b70/setuptools_github.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.1b69
+Version: 0.3.1b70
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -16,22 +16,22 @@
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # setuptools-github
 [![PyPI version](https://img.shields.io/pypi/v/setuptools-github.svg?color=blue)](https://pypi.org/project/setuptools-github)
 [![Python versions](https://img.shields.io/pypi/pyversions/setuptools-github.svg)](https://pypi.org/project/setuptools-github)
-[![Build](https://github.com/cav71/setuptools-github/actions/workflows/master.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions)
-[![Coverage](https://codecov.io/gh/cav71/setuptools-github/branch/beta/0.3.1/graph/badge.svg)](Coverage)
-
+[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions)
+[![Codecov](https://codecov.io/gh/cav71/setuptools-github/branch/0.3.1/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/0.3.1)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
 [![Types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 
 
+[![An old rock in the desert](/assets/images/shiprock.jpg "Shiprock, New Mexico by Beau Rogers")](https://www.flickr.com/photos/beaurogers/31833779864/in/photolist-Qv3rFw-34mt9F-a9Cmfy-5Ha3Zi-9msKdv-o3hgjr-hWpUte-4WMsJ1-KUQ8N-deshUb-vssBD-6CQci6-8AFCiD-zsJWT-nNfsgB-dPDwZJ-bn9JGn-5HtSXY-6CUhAL-a4UTXB-ugPum-KUPSo-fBLNm-6CUmpy-4WMsc9-8a7D3T-83KJev-6CQ2bK-nNusHJ-a78rQH-nw3NvT-7aq2qf-8wwBso-3nNceh-ugSKP-4mh4kh-bbeeqH-a7biME-q3PtTf-brFpgb-cg38zw-bXMZc-nJPELD-f58Lmo-bXMYG-bz8AAi-bxNtNT-bXMYi-bXMY6-bXMYv)
 
 ## Quick start
 setuptools-github helps to implement a simple project life cycle
 aimed at delivering packages into [PyPI](https://pypi.org). Basically:
 - beta packages are built from a /beta/N.M.O branch generating a **project-name-N.M.ObX** into PyPI
 - tagging with /release/N.M.O a /beta/N.M.O branch commit will release **project-name-N.M.O**
```

### Comparing `setuptools-github-0.3.1b69/setuptools_github.egg-info/SOURCES.txt` & `setuptools-github-0.3.1b70/setuptools_github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b69/src/setuptools_github/checks.py` & `setuptools-github-0.3.1b70/src/setuptools_github/checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b69/src/setuptools_github/cli.py` & `setuptools-github-0.3.1b70/src/setuptools_github/cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b69/src/setuptools_github/scm.py` & `setuptools-github-0.3.1b70/src/setuptools_github/scm.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b69/src/setuptools_github/script.py` & `setuptools-github-0.3.1b70/src/setuptools_github/script.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b69/src/setuptools_github/tools.py` & `setuptools-github-0.3.1b70/src/setuptools_github/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -330,27 +330,37 @@
     Args:
         paths (str, Path): path(s) to files jinja2 processeable
         initfile (str, Path): path to the __init__.py file with a __version__ variable
         github_dump (str): the os.getenv("GITHUB_DUMP") value
 
     Returns:
         str: the new version for the package
+
+    Example:
+        {'branch': 'beta/0.3.1',
+         'build': 0,
+         'current': '0.3.1',
+         'hash': 'c9e484a*',
+         'version': '0.3.1b0'}
     """
     from jinja2 import Environment
     from argparse import Namespace
+    from urllib.parse import quote
+    from functools import partial
 
     class Context(Namespace):
         def items(self):
             for name, value in self.__dict__.items():
                 if name.startswith("_"):
                     continue
                 yield (name, value)
 
     data = get_data(initfile, github_dump, abort)
     set_module_var(initfile, "__version__", data["version"])
     set_module_var(initfile, "__hash__", data["hash"])
 
     env = Environment()
+    env.filters["urlquote"] = partial(quote, safe="")
     for path in list_of_paths(paths):
         tmpl = env.from_string(path.read_text())
         path.write_text(tmpl.render(ctx=Context(**data)))
     return data
```

### Comparing `setuptools-github-0.3.1b69/tests/conftest.py` & `setuptools-github-0.3.1b70/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b69/tests/test_checks.py` & `setuptools-github-0.3.1b70/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b69/tests/test_cli.py` & `setuptools-github-0.3.1b70/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b69/tests/test_conftest.py` & `setuptools-github-0.3.1b70/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b69/tests/test_scm.py` & `setuptools-github-0.3.1b70/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b69/tests/test_script.py` & `setuptools-github-0.3.1b70/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b69/tests/test_tools.py` & `setuptools-github-0.3.1b70/tests/test_tools.py`

 * *Files identical despite different names*

